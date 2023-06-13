# Comparing `tmp/readonce-1.0.3.tar.gz` & `tmp/readonce-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readonce-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "readonce-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `readonce-1.0.3.tar` & `readonce-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      117 2023-05-21 14:27:51.727887 readonce-1.0.3/.flake8
--rw-r--r--   0        0        0      427 2023-05-21 14:27:51.727887 readonce-1.0.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      502 2023-05-21 14:27:51.727887 readonce-1.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      374 2023-05-21 14:27:51.727887 readonce-1.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1805 2023-05-21 14:27:51.727887 readonce-1.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2023-05-21 14:27:51.727887 readonce-1.0.3/LICENSE
--rw-r--r--   0        0        0      650 2023-05-21 14:27:51.727887 readonce-1.0.3/Makefile
--rw-r--r--   0        0        0    17317 2023-05-21 14:27:51.727887 readonce-1.0.3/README.md
--rw-r--r--   0        0        0      947 2023-05-21 14:27:51.727887 readonce-1.0.3/pyproject.toml
--rwxr-xr-x   0        0        0      156 2023-05-21 14:27:51.727887 readonce-1.0.3/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      166 2023-05-21 14:27:51.727887 readonce-1.0.3/scripts/format.sh
--rwxr-xr-x   0        0        0      108 2023-05-21 14:27:51.727887 readonce-1.0.3/scripts/lint.sh
--rw-r--r--   0        0        0     6770 2023-05-21 14:27:51.727887 readonce-1.0.3/src/readonce.py
--rw-r--r--   0        0        0     3736 2023-05-21 14:27:51.727887 readonce-1.0.3/tests/conftest.py
--rw-r--r--   0        0        0     9209 2023-05-21 14:27:51.727887 readonce-1.0.3/tests/test_readonce.py
--rw-r--r--   0        0        0    18230 1970-01-01 00:00:00.000000 readonce-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-06-13 22:34:50.718847 readonce-1.1.3/.flake8
+-rw-r--r--   0        0        0      427 2023-06-13 22:34:50.718847 readonce-1.1.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      502 2023-06-13 22:34:50.718847 readonce-1.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      374 2023-06-13 22:34:50.718847 readonce-1.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1805 2023-06-13 22:34:50.718847 readonce-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1073 2023-06-13 22:34:50.718847 readonce-1.1.3/LICENSE
+-rw-r--r--   0        0        0      650 2023-06-13 22:34:50.718847 readonce-1.1.3/Makefile
+-rw-r--r--   0        0        0    17491 2023-06-13 22:34:50.718847 readonce-1.1.3/README.md
+-rw-r--r--   0        0        0      947 2023-06-13 22:34:50.718847 readonce-1.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0      156 2023-06-13 22:34:50.718847 readonce-1.1.3/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      166 2023-06-13 22:34:50.718847 readonce-1.1.3/scripts/format.sh
+-rwxr-xr-x   0        0        0      108 2023-06-13 22:34:50.718847 readonce-1.1.3/scripts/lint.sh
+-rw-r--r--   0        0        0     6530 2023-06-13 22:34:50.718847 readonce-1.1.3/src/readonce.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:34:50.718847 readonce-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     3736 2023-06-13 22:34:50.718847 readonce-1.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     9875 2023-06-13 22:34:50.718847 readonce-1.1.3/tests/test_readonce.py
+-rw-r--r--   0        0        0    18404 1970-01-01 00:00:00.000000 readonce-1.1.3/PKG-INFO
```

### Comparing `readonce-1.0.3/.gitignore` & `readonce-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `readonce-1.0.3/LICENSE` & `readonce-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readonce-1.0.3/Makefile` & `readonce-1.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `readonce-1.0.3/README.md` & `readonce-1.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,29 +29,35 @@
 # Important information
 
 The ReadOnce object is not a cryptography library. 
 It is not responsible for encrypting/decrypting or dictating any type of cryptography methods to store and retrieve your secrets.
 
 The main idea behind the ReadOnce objects is hardening the access and allow only one time access to the stored secrets in the object.
 
-Question: Are the secrets stored in plain text?
-Answer: No, we use symmetric encryption from cryptography named [Fernet](https://cryptography.io/en/latest/fernet/).
+-------------------------------------------------
+**Question: Are the secrets stored in plain text?**
+
+*Answer: No, we use symmetric encryption from cryptography named [Fernet](https://cryptography.io/en/latest/fernet/).
 And we store passed secret data internally as so called fernet token(ciphertext+hash value).
-When you try to retrieve the secret back, it is decrypted with the same key and send back as a plain text.
+When you try to retrieve the secret back, it is decrypted with the same key and send back as a plain text.*
+
+--------------------------------------------------
+**Question: Then we have an encryption+hashing of plaintext?**
 
-Question: Then we have an encryption+hashing of plaintext?
-Answer: Yes, but ReadOnce class expects already encrypted(+ peppered, salted, hashed etc.) string to be passed as a secret, 
+*Answer: Yes, but ReadOnce class expects already encrypted(+ peppered, salted, hashed etc.) string to be passed as a secret, 
 because when you retrieve the secret it will return what it was originally passed. 
 If you passed the secret as "12345" you will get back "12345".
-If you passed the secret something like "HmDVbz6N3MlXqZ4q3TvLakMQ9fQjI45yhuoRHyZWiM4=" you will get back the same string.
+If you passed the secret something like "HmDVbz6N3MlXqZ4q3TvLakMQ9fQjI45yhuoRHyZWiM4=" you will get back the same string.*
+
+---------------------------------------------------
+**Question: Then why you store the secret as a token(ciphertext+hash value)?**
 
-Question: Then why you store the secret as a token(ciphertext+hash value)?
-Answer: It is an extra layer of hardening, if somehow, somebody could get the ReadOnce object and tries to steal the secret, lovely attacker should also have the key.
+*Answer: It is an extra layer of hardening, if somehow, somebody could get the ReadOnce object and tries to steal the secret, lovely attacker should also have the key.
 Okay the key also stored in ReadOnce object, but it is a non-trivial to get the key back. 
-If the attacker tries to add new secret over old one, the encryption key also updated.
+If the attacker tries to add new secret over old one, the encryption key also updated.*
 
 
 ### Install using pip:
 
 `pip install readonce`
 
 Then just inherit from the `ReadOnce`:
```

### Comparing `readonce-1.0.3/pyproject.toml` & `readonce-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `readonce-1.0.3/src/readonce.py` & `readonce-1.1.3/src/readonce.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import inspect
 from typing import Any, Iterable, List, Optional
 
 import icontract
 from cryptography.fernet import Fernet
 
-__version__ = "1.0.3"
+__version__ = "1.1.3"
 
 
 class UnsupportedOperationException(Exception):
     def __init__(self, *args: object) -> None:
         self.message = "Not allowed on sensitive value"
         super().__init__(self.message, *args)
 
@@ -26,186 +26,181 @@
 
 
 @icontract.invariant(
     lambda self: len(self) == 0 or len(self) == 1,
     "There can be no or only single secret data stored",
 )
 class ReadOnce(metaclass=Final):
-    """
-    Read-once object implementation:
-    * Sensitive data can be added only using add_secret
-    * Sensitive data can be read only once
-    * Sensitive class - inherited from ReadOnce can not be further subclassed
-    * Sensitive data can not be pickled
-    * Sensitive data can not be JSON serialized
-    * All properties, fields are hidden and can not be accessed directly - even from subclass
-    * The secrets can not be updated directly from outside - even from subclass
-    """
-
-    __secrets: List[bytes] = []
-    __is_consumed: bool = False
-    __key: Optional[bytes] = None
-
     @icontract.ensure(
-        lambda self: not self.__secrets and not self.__is_consumed and not self.__key
+        lambda self: not self.secrets_ and not self.is_consumed_ and not self.key_
     )
     def __init__(self) -> None:
-        self.__reset_secrets()
-        self.__reset_is_consumed()
-        self.__reset_key()
-
-    @classmethod
-    def __reset_secrets(cls) -> None:
-        cls.__secrets = []
-
-    @classmethod
-    def __reset_is_consumed(cls):
-        cls.__is_consumed = False
-
-    @classmethod
-    def __reset_key(cls):
-        cls.__key = None
-
-    @classmethod
-    def __update_is_consumed(cls):
-        cls.__is_consumed = True
-
-    @classmethod
-    def __update_key(cls, key: bytes):
-        cls.__key = key
+        self.secrets_: List[bytes] = []
+        self.is_consumed_: bool = False
+        self.key_: Optional[bytes] = None
+
+    @property
+    def secrets(self):
+        return []
+
+    @property
+    def is_consumed(self):
+        return None
+
+    @property
+    def key(self):
+        return None
 
     def add_secret(self, secret: Any):
         def __get_token():
             key_ = Fernet.generate_key()
             fernet = Fernet(key_)
             return key_, fernet.encrypt(bytes(secret_, encoding="utf-8"))
 
-        if self.__is_consumed:
+        if self.is_consumed_:
             raise UnsupportedOperationException(
                 "Sensitive object exhausted; you can not use it twice"
             )
         secret_ = str(secret)
-        self.__reset_secrets()
-        self.__reset_key()
+        self.reset_secrets()
+        self.reset_key()
         key, token = __get_token()
-        self.__update_key(key)
-        if not self.__key:
+        self.update_key(key)
+        if not self.key_:
             raise UnsupportedOperationException(
                 "Missing encryption key; impossible to store the secret"
             )
-        self.__secrets.append(token)
+        self.secrets_.append(token)
 
     def get_secret(self):
         frame = inspect.currentframe()
         # get two upper/back frame; one is getting back from icontract wrapper, second to get encoder default function
         function_name = frame.f_back.f_back.f_code.co_name
         if function_name == "default":
             raise UnsupportedOperationException("Sensitive data can not be serialized")
-        if self.__secrets:
-            self.__update_is_consumed()
-            if not self.__key:
+        if self.secrets_:
+            self.update_is_consumed()
+            if not self.is_consumed_:
+                raise UnsupportedOperationException("Failed to set consumed flag")
+            if not self.key_:
                 raise UnsupportedOperationException(
                     "Missing encryption key; impossible decrypt the secret"
                 )
-            fernet = Fernet(self.__key)
-            token = self.__secrets.pop()
+            fernet = Fernet(self.key_)
+            token = self.secrets_.pop()
             secret = fernet.decrypt(token)
-            self.__reset_key()
+            self.reset_key()
             return secret.decode(encoding="utf-8")
         raise UnsupportedOperationException("Sensitive data was already consumed")
 
-    @property
-    def secrets(self):
-        return []
-
-    @property
-    def is_consumed(self):
-        return None
-
-    @property
-    def key(self):
-        return None
-
-    def __getattribute__(self, __name: str) -> Any:
+    def __getattribute__(self, attr):
         frame = inspect.currentframe()
         # get the outer frame or caller frame
         function_name = frame.f_back.f_code.co_name
-        if __name == "_ReadOnce__secrets" and function_name not in (
+
+        if attr == "secrets_" and function_name not in (
             "add_secret",
             "get_secret",
+            "reset_secrets",
             "__len__",
         ):
             return []
 
-        if __name == "_ReadOnce__is_consumed" and function_name not in (
+        if attr == "reset_secrets" and function_name not in (
             "add_secret",
-            "get_secret",
             "__init__",
         ):
-            return None
+            raise UnsupportedOperationException()
 
-        if __name == "_ReadOnce__key" and function_name not in (
+        if attr == "is_consumed_" and function_name not in (
             "add_secret",
             "get_secret",
+            "reset_is_consumed",
+            "update_is_consumed",
             "__init__",
         ):
             return None
 
-        if __name == "_ReadOnce__update_is_consumed" and function_name not in (
-            "get_secret",
-        ):
+        if attr == "reset_is_consumed" and function_name not in ("__init__",):
             raise UnsupportedOperationException()
 
-        if __name == "_ReadOnce__reset_secrets" and function_name not in (
-            "add_secret",
-            "__init__",
-        ):
+        if attr == "update_is_consumed" and function_name not in ("get_secret",):
             raise UnsupportedOperationException()
 
-        if __name == "_ReadOnce__reset_is_consumed" and function_name not in (
+        if attr == "key_" and function_name not in (
+            "add_secret",
+            "get_secret",
+            "update_key",
+            "reset_key",
             "__init__",
         ):
-            raise UnsupportedOperationException()
+            return None
 
-        if __name == "_ReadOnce__reset_key" and function_name not in (
-            "get_secret",
+        if attr == "reset_key" and function_name not in (
             "add_secret",
+            "get_secret",
             "__init__",
         ):
             raise UnsupportedOperationException()
 
-        if __name == "_ReadOnce__update_key" and function_name not in ("add_secret",):
+        if attr == "update_key" and function_name not in ("add_secret",):
             raise UnsupportedOperationException()
 
-        return super().__getattribute__(__name)
+        return super().__getattribute__(attr)
 
-    def __setattr__(self, __name: str, __value: str) -> Any:
+    def __setattr__(self, attr: str, value: str) -> Any:
         frame = inspect.currentframe()
         # get the outer frame or caller frame
         function_name = frame.f_back.f_code.co_name
-
-        if __name == "_ReadOnce__secrets" and function_name not in (
+        if attr == "secrets_" and function_name not in (
             "add_secret",
+            "reset_secrets",
             "__init__",
         ):
             raise UnsupportedOperationException()
 
-        if __name == "_ReadOnce__is_consumed" and function_name not in (
+        if attr == "is_consumed_" and function_name not in (
             "get_secret",
+            "update_is_consumed",
             "__init__",
         ):
             raise UnsupportedOperationException()
 
-        if __name == "_ReadOnce__key" and function_name not in (
+        if attr == "key_" and function_name not in (
             "get_secret",
             "add_secret",
+            "reset_key",
+            "update_key",
             "__init__",
         ):
             raise UnsupportedOperationException()
 
+        if attr == "get_secret":
+            raise UnsupportedOperationException()
+
+        if attr == "add_secret":
+            raise UnsupportedOperationException()
+
+        super().__setattr__(attr, value)
+
+    def reset_secrets(self) -> None:
+        self.secrets_ = []
+
+    def reset_is_consumed(self):
+        self.is_consumed_ = False
+
+    def update_is_consumed(self):
+        self.is_consumed_ = True
+
+    def reset_key(self):
+        self.key_ = None
+
+    def update_key(self, key: bytes):
+        self.key_ = key
+
     def __dir__(self) -> Iterable[str]:
         return []
 
     def __str__(self) -> str:
         return f"{__class__.__name__}[secrets=*****]"
 
     def __repr__(self) -> str:
@@ -214,8 +209,11 @@
     def __getstate__(self):
         raise UnsupportedOperationException()
 
     def __setstate__(self, value):
         raise UnsupportedOperationException()
 
     def __len__(self):
-        return len(self.__secrets)
+        return len(self.secrets_)
+
+    def __dict__(self):
+        return {}
```

### Comparing `readonce-1.0.3/tests/conftest.py` & `readonce-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `readonce-1.0.3/tests/test_readonce.py` & `readonce-1.1.3/tests/test_readonce.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import pickle
 
 import pytest
 
 from readonce import UnsupportedOperationException
+from tests.conftest import Password
 
 
 def test_finalized_class_can_not_be_subclassed(get_password_class):
     with pytest.raises(TypeError):
 
         class TryPassword(get_password_class):
             ...
@@ -26,48 +27,49 @@
 def test_if_can_pickle_the_secret_class(get_password_obj):
     with pytest.raises(UnsupportedOperationException):
         pickle.dumps(get_password_obj)
 
 
 def test_direct_secrets_access_is_empty_list(get_password_obj):
     assert get_password_obj.secrets == []
+    assert get_password_obj.secrets_ == []
 
 
 def test_direct_access_to_is_consumed_field(get_password_obj):
     assert get_password_obj.is_consumed is None
-    assert get_password_obj._ReadOnce__is_consumed is None
+    assert get_password_obj.is_consumed_ is None
 
     with pytest.raises(UnsupportedOperationException):
-        get_password_obj._ReadOnce__is_consumed = True
+        get_password_obj.is_consumed_ = True
 
     with pytest.raises(UnsupportedOperationException):
-        get_password_obj._ReadOnce__update_is_consumed()
+        get_password_obj.update_is_consumed()
 
 
-def test_direct__reset_is_consumed_call(get_password_obj):
+def test_direct_reset_is_consumed_call(get_password_obj):
     with pytest.raises(UnsupportedOperationException):
-        get_password_obj._ReadOnce__reset_is_consumed()
+        get_password_obj.reset_is_consumed()
 
 
 def test_direct_reset_secrets_call(get_password_obj):
     with pytest.raises(UnsupportedOperationException):
-        get_password_obj._ReadOnce__reset_secrets()
+        get_password_obj.reset_secrets()
 
 
 def test_sensitive_class_dict_is_empty(get_password_obj):
-    assert get_password_obj.__dict__ == {}
+    assert get_password_obj.__dict__() == {}
 
 
 def test_sensitive_class_dir_output_is_empty(get_password_obj):
     assert not dir(get_password_obj)
     assert get_password_obj.__dir__() == []
 
 
 def test_sensitive_class_super_class_secrets_is_empty(get_password_obj):
-    assert get_password_obj._ReadOnce__secrets == []
+    assert get_password_obj.secrets_ == []
     assert get_password_obj.secrets == []
 
 
 def test_len_of_secrets(get_password_class):
     obj = get_password_class("new_password")
     assert len(obj) == 1
     pass_ = obj.get_secret()
@@ -210,64 +212,83 @@
 
 
 def test_monkeypatch_get_secret(get_password_obj, monkeypatch):
     def mock_return():
         return "12345"
 
     get_password_obj.add_secret("new_secret")
-    monkeypatch.setattr(get_password_obj, "get_secret", mock_return)
+    with pytest.raises(UnsupportedOperationException):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "get_secret", mock_return)
     # the original secret was not affected
     assert get_password_obj.get_secret() != mock_return()
 
 
 def test_monkeypatch_add_secret(get_password_obj, monkeypatch):
     def mock_return():
         return "12345"
 
     # basically has no effect on add_secret
-    monkeypatch.setattr(get_password_obj, "add_secret", mock_return)
+    with pytest.raises(UnsupportedOperationException):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "add_secret", mock_return)
     get_password_obj.add_secret("fake")
-    monkeypatch.setattr(get_password_obj, "get_secret", mock_return)
+
+    with pytest.raises(UnsupportedOperationException):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "get_secret", mock_return)
     # the original secret was not affected
     assert get_password_obj.get_secret() != mock_return()
 
 
 def test_monkeypatch_change_secrets_property(get_password_obj, monkeypatch):
     # It has no effect either for the secrets property
-    monkeypatch.setattr(get_password_obj, "secrets", ["12345"])
+    with pytest.raises(AttributeError):
+        with monkeypatch.context() as m:
+            m.setattr(get_password_obj, "secrets", ["12345"])
     # Still original secret is there
     assert get_password_obj.get_secret() != "12345"
 
 
 def test_monkeypatch_change_secrets_storage(get_password_obj, monkeypatch):
     # Directly trying to monkeypatch will raise double UnsupportedOperationException;
     # As monkeypatch in its default undo() section tries to again edit "_ReadOnce__secrets" which raises same exception
     # That's why we use context() below
 
     # with pytest.raises(UnsupportedOperationException):
     #     monkeypatch.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=False)
 
     with pytest.raises(UnsupportedOperationException):
         with monkeypatch.context() as m:
-            m.setattr(get_password_obj, "_ReadOnce__secrets", ["12345"], raising=True)
+            m.setattr(get_password_obj, "secrets_", ["12345"], raising=True)
 
 
 def test_direct_access_to_key_field(get_password_obj):
     assert get_password_obj.key is None
-    assert get_password_obj._ReadOnce__key is None
+    assert get_password_obj.key_ is None
 
     with pytest.raises(UnsupportedOperationException):
-        get_password_obj._ReadOnce__key = b"new key"
+        get_password_obj.key_ = b"new key"
 
     with pytest.raises(UnsupportedOperationException):
-        get_password_obj._ReadOnce__update_key(b"new key")
+        get_password_obj.update_key(b"new key")
 
     with pytest.raises(UnsupportedOperationException):
-        get_password_obj._ReadOnce__reset_key()
+        get_password_obj.reset_key()
 
 
 def test_monkeypatch_the_key(get_password_obj, monkeypatch):
     get_password_obj.add_secret("new_secret")
 
     with pytest.raises(UnsupportedOperationException):
         with monkeypatch.context() as m:
-            m.setattr(get_password_obj, "_ReadOnce__key", None)
+            m.setattr(get_password_obj, "key_", None)
+
+
+def test_if_can_create_and_consume_same_secret_multiple_times(get_password_obj):
+    get_password_obj.add_secret("new_secret")
+    pass_1 = Password("new_secret")
+    pass_2 = Password("new_secret")
+
+    assert pass_1 is not pass_2
+    assert pass_1 != pass_2
+    assert get_password_obj.get_secret() == pass_1.get_secret() == pass_2.get_secret()
```

### Comparing `readonce-1.0.3/PKG-INFO` & `readonce-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readonce
-Version: 1.0.3
+Version: 1.1.3
 Summary: Read-Once Object implementation in Python - Inspired by Secure by Design book.
 Author-email: Shako Rzayev <rzayev.sehriyar@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: icontract >=2.6.2
 Requires-Dist: cryptography >=40.0.2
@@ -52,29 +52,35 @@
 # Important information
 
 The ReadOnce object is not a cryptography library. 
 It is not responsible for encrypting/decrypting or dictating any type of cryptography methods to store and retrieve your secrets.
 
 The main idea behind the ReadOnce objects is hardening the access and allow only one time access to the stored secrets in the object.
 
-Question: Are the secrets stored in plain text?
-Answer: No, we use symmetric encryption from cryptography named [Fernet](https://cryptography.io/en/latest/fernet/).
+-------------------------------------------------
+**Question: Are the secrets stored in plain text?**
+
+*Answer: No, we use symmetric encryption from cryptography named [Fernet](https://cryptography.io/en/latest/fernet/).
 And we store passed secret data internally as so called fernet token(ciphertext+hash value).
-When you try to retrieve the secret back, it is decrypted with the same key and send back as a plain text.
+When you try to retrieve the secret back, it is decrypted with the same key and send back as a plain text.*
+
+--------------------------------------------------
+**Question: Then we have an encryption+hashing of plaintext?**
 
-Question: Then we have an encryption+hashing of plaintext?
-Answer: Yes, but ReadOnce class expects already encrypted(+ peppered, salted, hashed etc.) string to be passed as a secret, 
+*Answer: Yes, but ReadOnce class expects already encrypted(+ peppered, salted, hashed etc.) string to be passed as a secret, 
 because when you retrieve the secret it will return what it was originally passed. 
 If you passed the secret as "12345" you will get back "12345".
-If you passed the secret something like "HmDVbz6N3MlXqZ4q3TvLakMQ9fQjI45yhuoRHyZWiM4=" you will get back the same string.
+If you passed the secret something like "HmDVbz6N3MlXqZ4q3TvLakMQ9fQjI45yhuoRHyZWiM4=" you will get back the same string.*
+
+---------------------------------------------------
+**Question: Then why you store the secret as a token(ciphertext+hash value)?**
 
-Question: Then why you store the secret as a token(ciphertext+hash value)?
-Answer: It is an extra layer of hardening, if somehow, somebody could get the ReadOnce object and tries to steal the secret, lovely attacker should also have the key.
+*Answer: It is an extra layer of hardening, if somehow, somebody could get the ReadOnce object and tries to steal the secret, lovely attacker should also have the key.
 Okay the key also stored in ReadOnce object, but it is a non-trivial to get the key back. 
-If the attacker tries to add new secret over old one, the encryption key also updated.
+If the attacker tries to add new secret over old one, the encryption key also updated.*
 
 
 ### Install using pip:
 
 `pip install readonce`
 
 Then just inherit from the `ReadOnce`:
```

