# Comparing `tmp/robocorp_vault-0.1.0.tar.gz` & `tmp/robocorp_vault-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_vault-0.1.0.tar", max compression
+gzip compressed data, was "robocorp_vault-0.3.0.tar", max compression
```

## Comparing `robocorp_vault-0.1.0.tar` & `robocorp_vault-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0       36 2023-04-25 10:39:03.649692 robocorp_vault-0.1.0/README.md
--rw-r--r--   0        0        0      563 2023-04-25 10:39:03.650316 robocorp_vault-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-04-25 10:39:03.650570 robocorp_vault-0.1.0/src/robocorp/vault/__init__.py
--rw-r--r--   0        0        0     1840 2023-04-25 10:39:03.650655 robocorp_vault-0.1.0/src/robocorp/vault/_utils.py
--rw-r--r--   0        0        0    18270 2023-04-25 10:39:03.650968 robocorp_vault-0.1.0/src/robocorp/vault/vault.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 robocorp_vault-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/README.md
+-rw-r--r--   0        0        0      704 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4147 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/src/robocorp/vault/__init__.py
+-rw-r--r--   0        0        0      112 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/src/robocorp/vault/_errors.py
+-rw-r--r--   0        0        0     1587 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/src/robocorp/vault/_secrets.py
+-rw-r--r--   0        0        0     1858 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/src/robocorp/vault/_utils.py
+-rw-r--r--   0        0        0    18337 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/src/robocorp/vault/_vault.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:22:00.550131 robocorp_vault-0.3.0/src/robocorp/vault/py.typed
+-rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 robocorp_vault-0.3.0/PKG-INFO
```

### Comparing `robocorp_vault-0.1.0/pyproject.toml` & `robocorp_vault-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 [tool.poetry]
 name = "robocorp-vault"
-version = "0.1.0"
+version = "0.3.0"
 description = "Robocorp Control Room API integration library"
 authors = [
-	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
-	"Kerkko P. <kerkko@robocorp.com>",
-    "Antero V. <antero@robocorp.com>",
+	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cryptography = "^39.0.1"
+requests = "^2.31"
+pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
-libs-devdeps = {path = ".."}
+robocorp-devutils = {path = "../devutils/", develop = true}
+mock = "^5.0"
+types-requests = "^2.31"
+types-mock = "^5.0"
+types-PyYAML = "^6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
+
+[tool.mypy]
+mypy_path = "src:tests"
```

### Comparing `robocorp_vault-0.1.0/src/robocorp/vault/_utils.py` & `robocorp_vault-0.3.0/src/robocorp/vault/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import importlib
 import os
 from pathlib import Path
-
-from typing import Any
-
+from typing import Any, Optional
 
 # Sentinel value for undefined argument
 UNDEFINED = object()
 
 
 def required_env(name: str, default: Any = UNDEFINED) -> str:
     """Load required environment variable.
@@ -20,15 +18,15 @@
     """
     val = os.getenv(name, default)
     if val is UNDEFINED:
         raise KeyError(f"Missing required environment variable: {name}")
     return val
 
 
-def import_by_name(name: str, caller: str = None) -> Any:
+def import_by_name(name: str, caller: Optional[str] = None) -> Any:
     """Import module (or attribute) by name.
 
     Args:
         name: Import path, e.g. RPA.Robocorp.WorkItems.RobocorpAdapter
         caller: Caller file name
 
     """
```

### Comparing `robocorp_vault-0.1.0/src/robocorp/vault/vault.py` & `robocorp_vault-0.3.0/src/robocorp/vault/_vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,51 @@
 import base64
 import binascii
-import collections
 import copy
 import json
 import logging
 import os
 import traceback
-from abc import abstractmethod, ABCMeta
-from typing import Tuple
+from abc import ABCMeta, abstractmethod
+from typing import Callable, Tuple
 
 import requests
-import yaml
 from cryptography.exceptions import InvalidTag
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 
-from robocorp.vault._utils import (
-    import_by_name,
-    required_env,
-    resolve_path,
-    url_join,
-)
-
-
-class RobocorpVaultError(RuntimeError):
-    """Raised when there's problem with reading from Robocorp Vault."""
-
-
-class Secret(collections.abc.Mapping):
-    """Container for a secret with name, description, and multiple key-value pairs.
-
-    Immutable and avoids logging internal values when possible.
-
-    Args:
-        name:        Name of secret
-        description: Human-friendly description for secret
-        values:      Dictionary of key-value pairs stored in secret
-
-    """
-
-    def __init__(self, name, description, values):
-        self._name = name
-        self._desc = description
-        self._dict = collections.OrderedDict(**values)
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def description(self):
-        return self._desc
-
-    def update(self, kvpairs):
-        self._dict.update(kvpairs)
-
-    def __getitem__(self, key):
-        return self._dict[key]
-
-    def __setitem__(self, key, value):
-        self._dict[key] = value
-
-    def __contains__(self, key):
-        return key in self._dict
-
-    def __iter__(self):
-        return iter(self._dict)
-
-    def __len__(self):
-        return len(self._dict)
-
-    def __repr__(self):
-        return "Secret(name={name}, keys=[{keys}])".format(
-            name=self.name, keys=", ".join(str(key) for key in self.keys())
-        )
+from ._errors import RobocorpVaultError
+from ._secrets import SecretContainer
+from ._utils import import_by_name, required_env, resolve_path, url_join
 
 
 class BaseSecretManager(metaclass=ABCMeta):
     """Abstract class for secrets management.
 
     Should be used as a base-class for any adapter implementation.
-
     """
 
     @abstractmethod
     def get_secret(self, secret_name):
-        """Return ``Secret`` object with given name."""
+        """Return ``SecretContainer`` object with given name."""
 
     @abstractmethod
-    def set_secret(self, secret: Secret):
+    def set_secret(self, secret: SecretContainer):
         """Set a secret with a new value."""
 
 
 class FileSecrets(BaseSecretManager):
     """Adapter for secrets stored in a database file.
 
     Supports only plaintext secrets, and should be used mainly for debugging.
 
     The path to the secrets file can be set with the
-    environment variable ``RPA_SECRET_FILE``, or as
+    environment variable ``RC_VAULT_SECRETS_FILE``, or as
     an argument to the library.
 
     The format of the secrets file should be one of the following:
 
     .. code-block:: JSON
 
       {
@@ -124,102 +65,111 @@
       name1:
         key1: value1
         key2: value2
       name2:
         key1: value1
     """
 
-    SERIALIZERS = {
-        ".json": (json.load, json.dump),
-        ".yaml": (yaml.full_load, yaml.dump),
-    }
-
     def __init__(self, secret_file="secrets.json"):
         self.logger = logging.getLogger(__name__)
 
-        path = required_env("RPA_SECRET_FILE", secret_file)
+        if "RC_VAULT_SECRETS_FILE" in os.environ:
+            path = required_env("RC_VAULT_SECRETS_FILE", secret_file)
+        elif "RPA_SECRET_FILE" in os.environ:  # Backward-compatibility
+            path = required_env("RPA_SECRET_FILE", secret_file)
+        else:
+            path = secret_file
+
         self.logger.info("Resolving path: %s", path)
         self.path = resolve_path(path)
 
         extension = self.path.suffix
-        serializer = self.SERIALIZERS.get(extension)
+        self._loader, self._dumper = self._get_serializer(extension)
+
+    def _get_serializer(self, extension: str) -> Tuple[Callable, Callable]:
+        if extension == ".json":
+            return (json.load, json.dump)
+
+        if extension == ".yaml":
+            import yaml
+
+            return (yaml.safe_load, yaml.dump)
+
         # NOTE(cmin764): This will raise instead of returning an empty secrets object
         #  because it is wrong starting from the "env.json" configuration level.
-        if not serializer:
-            raise ValueError(
-                f"Not supported local vault secrets file extension {extension!r}"
-            )
-        self._loader, self._dumper = serializer
-
-        self.data = self.load()
+        raise ValueError(
+            f"Local vault secrets file extension {extension!r} not supported."
+        )
 
-    def load(self):
+    def _load(self):
         """Load secrets file."""
         try:
             with open(self.path, encoding="utf-8") as fd:
                 data = self._loader(fd)
 
             if not isinstance(data, dict):
                 raise ValueError("Invalid content format")
 
             return data
         except (IOError, ValueError) as err:
             self.logger.error("Failed to load secrets file: %s", err)
             return {}
 
-    def save(self):
+    def _save(self, data):
         """Save the secrets content to disk."""
         try:
             with open(self.path, "w", encoding="utf-8") as f:
-                if not isinstance(self.data, dict):
+                if not isinstance(data, dict):
                     raise ValueError("Invalid content format")
-                self._dumper(self.data, f, indent=4)
+                self._dumper(data, f, indent=4)
         except (IOError, ValueError) as err:
-            self.logger.error("Failed to save secrets file: %s", err)
+            self.logger.error("Failed to _save secrets file: %s", err)
 
-    def get_secret(self, secret_name) -> Secret:
+    def get_secret(self, secret_name: str) -> SecretContainer:
         """Get secret defined with given name from file.
 
         Args:
             secret_name: Name of secret to fetch
         Returns:
-            Secret: Secret object
+            SecretContainer: SecretContainer object
 
         Raises:
             KeyError: No secret with given name
 
         """
-        values = self.data.get(secret_name)
+        values = self._load().get(secret_name)
         if values is None:
             raise KeyError(f"Undefined secret: {secret_name}")
 
-        return Secret(secret_name, "", values)
+        return SecretContainer(secret_name, "", values)
 
-    def set_secret(self, secret: Secret) -> None:
-        """Set the secret value in the local Vault with the given ``Secret`` object.
+    def set_secret(self, secret: SecretContainer) -> None:
+        """Set the secret value in the local Vault with the given
+        ``SecretContainer`` object.
 
         Args:
-            secret: A ``Secret`` object.
+            secret: A ``SecretContainer`` object.
 
         Raises:
             IOError: Writing the local vault failed.
             ValueError: Writing the local vault failed.
 
         """
-        self.data[secret.name] = dict(secret)
-        self.save()
+        data = self._load()
+        data[secret.name] = dict(secret)
+        self._save(data)
 
 
 class RobocorpVault(BaseSecretManager):
     """Adapter for secrets stored in Robocorp Vault.
 
     The following environment variables should exist:
 
-    - RC_API_SECRET_HOST:   URL to Robocorp Secrets API
-    - RC_API_SECRET_TOKEN:  API token with access to Robocorp Secrets API
+    - RC_API_SECRET_HOST:   URL to Robocorp Secret API
+    - RC_API_SECRET_TOKEN:  API token with access to Robocorp Secret API
     - RC_WORKSPACE_ID:      Robocorp Workspace ID
 
     If the robot run is started from the Robocorp Control Room these environment
     variables will be configured automatically.
 
     """
 
@@ -285,25 +235,24 @@
             "secrets-v1",
             "workspaces",
             self._workspace,
             "secrets",
             "publicKey",
         )
 
-    def get_secret(self, secret_name) -> Secret:
+    def get_secret(self, secret_name: str) -> SecretContainer:
         """Get secret defined with given name from Robocorp Vault.
 
         Args:
             secret_name: Name of secret to fetch
         Returns:
-            Secret: Secret object
+            SecretContainer object
 
         Raises:
             RobocorpVaultError: Error with API request or response payload
-
         """
         url = self.create_secret_url(secret_name)
 
         try:
             response = requests.get(url, headers=self.headers, params=self.params)
             response.raise_for_status()
 
@@ -312,15 +261,17 @@
         except InvalidTag as e:
             self.logger.debug(traceback.format_exc())
             raise RobocorpVaultError("Failed to validate authentication tag") from e
         except Exception as exc:
             self.logger.debug(traceback.format_exc())
             raise RobocorpVaultError from exc
 
-        return Secret(payload["name"], payload["description"], payload["values"])
+        return SecretContainer(
+            payload["name"], payload["description"], payload["values"]
+        )
 
     def _decrypt_payload(self, payload):
         payload = copy.deepcopy(payload)
 
         fields = payload.pop("encryption", None)
         if fields is None:
             raise KeyError("Missing encryption fields from response")
@@ -346,24 +297,24 @@
         # Decrypt actual value using decrypted AES key
         ciphertext = base64.b64decode(payload.pop("value")) + aes_tag
         data = AESGCM(aes_key).decrypt(binascii.hexlify(aes_iv), ciphertext, b"")
         payload["values"] = json.loads(data)
 
         return payload
 
-    def set_secret(self, secret: Secret) -> None:
+    def set_secret(self, secret: SecretContainer) -> None:
         """Set the secret value in the Vault.
 
         Note:
             The secret possibly consists of multiple key-value pairs,
             which will all be overwritten with the values given here.
             So don't try to update only one item of the secret, update all of them.
 
         Args:
-            secret: A ``Secret`` object
+            secret: A ``SecretContainer`` object
 
         """
         value, aes_iv, aes_key, aes_tag = self._encrypt_secret_value_with_aes(secret)
         pub_key = self.get_publickey()
         aes_enc = self._encrypt_aes_key_with_public_rsa(aes_key, pub_key)
 
         payload = {
@@ -402,15 +353,15 @@
                 "Failed to fetch public key. Is your token valid?"
             ) from e
 
         return response.content
 
     @staticmethod
     def _encrypt_secret_value_with_aes(
-        secret: Secret,
+        secret: SecretContainer,
     ) -> Tuple[bytes, bytes, bytes, bytes]:
         def generate_aes_key() -> Tuple[bytes, bytes]:
             aes_key = AESGCM.generate_key(bit_length=256)
             aes_iv = os.urandom(16)
             return aes_key, aes_iv
 
         def split_auth_tag_from_encrypted_value(
@@ -439,15 +390,15 @@
         )
 
     @staticmethod
     def _encrypt_aes_key_with_public_rsa(aes_key: bytes, public_rsa: bytes) -> bytes:
         pub_decoded = base64.b64decode(public_rsa)
         public_key = serialization.load_der_public_key(pub_decoded)
 
-        aes_enc = public_key.encrypt(
+        aes_enc = public_key.encrypt(  # type: ignore [union-attr]
             aes_key,
             padding.OAEP(
                 mgf=padding.MGF1(algorithm=hashes.SHA256()),
                 algorithm=hashes.SHA256(),
                 label=None,
             ),
         )
@@ -477,16 +428,16 @@
 
     .. _Robocorp Control Room Vault: https://robocorp.com/docs/development-guide/variables-and-secrets/vault
     .. _Robocorp Code Extension: https://robocorp.com/docs/developer-tools/visual-studio-code/extension-features#connecting-to-control-room-vault
     .. _rcc: https://robocorp.com/docs/rcc/workflow
 
     File-based secrets can be set by defining two environment variables.
 
-    - ``RPA_SECRET_MANAGER``: RPA.Robocorp.Vault.FileSecrets
-    - ``RPA_SECRET_FILE``: Absolute path to the secrets database file
+    - ``RC_VAULT_SECRET_MANAGER``: FileSecrets
+    - ``RC_VAULT_SECRET_FILE``: Absolute path to the secrets database file
 
     Example content of local secrets file:
 
     .. code-block:: json
 
         {
             "swaglabs": {
@@ -502,16 +453,14 @@
         swaglabs:
             username: standard_user
             password: secret_sauce
 
     Example:
         .. code-block:: python
 
-            from RPA.Robocorp.Vault import Vault
-
             VAULT = Vault()
 
             def reading_secrets():
                 print(f"My secrets: {VAULT.get_secret('swaglabs')}")
 
             def modifying_secrets():
                 secret = VAULT.get_secret("swaglabs")
@@ -519,69 +468,85 @@
                 VAULT.set_secret(secret)
 
     """  # noqa: E501
 
     def __init__(self, *args, **kwargs):
         """The selected adapter can be set with the environment variable.
 
-        Use the environment variable ``RPA_SECRET_MANAGER``, or the argument ``default_adapter``.
+        Use the environment variable ``RC_VAULT_SECRET_MANAGER``, or the
+        argument ``default_adapter``.
         Defaults to Robocorp Vault if not defined.
 
         All other library arguments are passed to the adapter.
 
         Args:
             default_adapter: Override default secret adapter
 
         """
         self.logger = logging.getLogger(__name__)
 
         default = kwargs.pop("default_adapter", RobocorpVault)
-        adapter = required_env("RPA_SECRET_MANAGER", default)
+        if "RC_VAULT_SECRET_MANAGER" in os.environ:
+            adapter = required_env("RC_VAULT_SECRET_MANAGER", default)
+        elif "RPA_SECRET_MANAGER" in os.environ:  # Backward-compatibility
+            adapter = required_env("RPA_SECRET_MANAGER", default)
+        else:
+            adapter = default
 
         self._adapter_factory = self._create_factory(adapter, args, kwargs)
         self._adapter = None
 
     @property
-    def adapter(self):
+    def adapter(self) -> BaseSecretManager:
         if self._adapter is None:
             self._adapter = self._adapter_factory()
 
         return self._adapter
 
     def _create_factory(self, adapter, args, kwargs):
         if isinstance(adapter, str):
-            adapter = import_by_name(adapter, __name__)
+            if adapter in ("FileSecrets", "RPA.Robocorp.Vault.FileSecrets"):
+                adapter = FileSecrets
+            else:
+                try:
+                    adapter = import_by_name(adapter, __name__)
+                except Exception as e:
+                    raise ValueError(
+                        f"RC_VAULT_SECRET_MANAGER environment variable seems to "
+                        f"have a wrong value: {adapter!r}.\n"
+                        f'It should be unset to load from Control Room, "FileSecrets" '
+                        f'to load from a file or the name of the "BaseSecretManager" '
+                        f"implementation class."
+                    ) from e
 
         if not issubclass(adapter, BaseSecretManager):
             raise ValueError(
                 f"Adapter '{adapter}' does not inherit from BaseSecretManager"
             )
 
         def factory():
             return adapter(*args, **kwargs)
 
         return factory
 
-    def get_secret(self, secret_name: str) -> Secret:
+    def get_secret(self, secret_name: str) -> SecretContainer:
         """Read a secret from the configured source, e.g. Robocorp Vault.
 
         Args:
-            secret_name: Name of secret
+            secret_name: Name of secret.
 
         Returns:
-            Secret: ``Secret`` object
-
+            `SecretContainer` object.
         """
         return self.adapter.get_secret(secret_name)
 
-    def set_secret(self, secret: Secret) -> None:
+    def set_secret(self, secret: SecretContainer) -> None:
         """Overwrite an existing secret with new values.
 
         Note:
             Only allows modifying existing secrets, and replaces
               all values contained within it.
 
         Args:
-            secret: Secret as a ``Secret`` object, from e.g. ``Get Secret``
-
+            secret: `SecretContainer` object, from e.g. `get_secret`.
         """
         self.adapter.set_secret(secret)
```

### Comparing `robocorp_vault-0.1.0/PKG-INFO` & `robocorp_vault-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: robocorp-vault
-Version: 0.1.0
+Version: 0.3.0
 Summary: Robocorp Control Room API integration library
-Author: Ossi R.
-Author-email: ossi@robocorp.com
+Author: Fabio Z.
+Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=39.0.1,<40.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.31,<3.0)
 Description-Content-Type: text/markdown
 
 # Robocorp Control Room API library
```

