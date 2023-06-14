# Comparing `tmp/censys-2.2.2.tar.gz` & `tmp/censys-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censys-2.2.2.tar", max compression
+gzip compressed data, was "censys-2.2.3.tar", max compression
```

## Comparing `censys-2.2.2.tar` & `censys-2.2.3.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0    10174 2023-05-09 14:00:31.082041 censys-2.2.2/LICENSE
--rw-r--r--   0        0        0     4466 2023-05-09 14:00:31.082041 censys-2.2.2/README.md
--rw-r--r--   0        0        0       91 2023-05-09 14:00:31.082041 censys-2.2.2/censys/__main__.py
--rw-r--r--   0        0        0      633 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/__init__.py
--rw-r--r--   0        0        0     3474 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/api.py
--rw-r--r--   0        0        0      410 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/__init__.py
--rw-r--r--   0        0        0     5900 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/assets.py
--rw-r--r--   0        0        0      424 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/certificates.py
--rw-r--r--   0        0        0     1118 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/domains.py
--rw-r--r--   0        0        0      389 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/hosts.py
--rw-r--r--   0        0        0     2075 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/subdomains.py
--rw-r--r--   0        0        0     1775 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/web_entities.py
--rw-r--r--   0        0        0     1598 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/client.py
--rw-r--r--   0        0        0     2380 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/clouds.py
--rw-r--r--   0        0        0     2519 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/events.py
--rw-r--r--   0        0        0     2482 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/inventory.py
--rw-r--r--   0        0        0     3981 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/risks.py
--rw-r--r--   0        0        0     2784 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/seeds.py
--rw-r--r--   0        0        0      675 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/__init__.py
--rw-r--r--   0        0        0     1901 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/args.py
--rw-r--r--   0        0        0      174 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/__init__.py
--rw-r--r--   0        0        0     2045 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/account.py
--rw-r--r--   0        0        0     6793 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/asm.py
--rw-r--r--   0        0        0     3171 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/config.py
--rw-r--r--   0        0        0     5526 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/hnri.py
--rw-r--r--   0        0        0     6603 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/search.py
--rw-r--r--   0        0        0     3492 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/subdomains.py
--rw-r--r--   0        0        0     3760 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/view.py
--rw-r--r--   0        0        0   233252 2023-05-09 14:00:31.086041 censys-2.2.2/censys/cli/data/certificates_autocomplete.json
--rw-r--r--   0        0        0   324545 2023-05-09 14:00:31.086041 censys-2.2.2/censys/cli/data/hosts_autocomplete.json
--rw-r--r--   0        0        0     3279 2023-05-09 14:00:31.086041 censys-2.2.2/censys/cli/utils.py
--rw-r--r--   0        0        0      105 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/__init__.py
--rw-r--r--   0        0        0     8552 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/base.py
--rw-r--r--   0        0        0     1690 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/config.py
--rw-r--r--   0        0        0     1106 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/deprecation.py
--rw-r--r--   0        0        0    12446 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/exceptions.py
--rw-r--r--   0        0        0      144 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/types.py
--rw-r--r--   0        0        0      453 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/utils.py
--rw-r--r--   0        0        0      242 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/version.py
--rw-r--r--   0        0        0        0 2023-05-09 14:00:31.086041 censys-2.2.2/censys/py.typed
--rw-r--r--   0        0        0      375 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/__init__.py
--rw-r--r--   0        0        0     2133 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/client.py
--rw-r--r--   0        0        0      169 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/__init__.py
--rw-r--r--   0        0        0     5805 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/api.py
--rw-r--r--   0        0        0     1830 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/certificates.py
--rw-r--r--   0        0        0     1224 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/data.py
--rw-r--r--   0        0        0      151 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/__init__.py
--rw-r--r--   0        0        0    17200 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/api.py
--rw-r--r--   0        0        0    12823 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/certs.py
--rw-r--r--   0        0        0    10570 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/hosts.py
--rw-r--r--   0        0        0     3449 2023-05-09 14:00:31.090041 censys-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     7112 1970-01-01 00:00:00.000000 censys-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-06-14 20:56:28.089279 censys-2.2.3/LICENSE
+-rw-r--r--   0        0        0     4699 2023-06-14 20:56:28.089279 censys-2.2.3/README.md
+-rw-r--r--   0        0        0       91 2023-06-14 20:56:28.089279 censys-2.2.3/censys/__main__.py
+-rw-r--r--   0        0        0      693 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/__init__.py
+-rw-r--r--   0        0        0     3474 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/api.py
+-rw-r--r--   0        0        0      485 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/__init__.py
+-rw-r--r--   0        0        0     6470 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/assets.py
+-rw-r--r--   0        0        0      424 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/certificates.py
+-rw-r--r--   0        0        0     1118 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/domains.py
+-rw-r--r--   0        0        0      389 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/hosts.py
+-rw-r--r--   0        0        0      847 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/object_storage.py
+-rw-r--r--   0        0        0     2075 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/subdomains.py
+-rw-r--r--   0        0        0     1775 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/assets/web_entities.py
+-rw-r--r--   0        0        0     3356 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/beta.py
+-rw-r--r--   0        0        0     1798 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/client.py
+-rw-r--r--   0        0        0     2054 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/clouds.py
+-rw-r--r--   0        0        0     2482 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/inventory.py
+-rw-r--r--   0        0        0     2576 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/logbook.py
+-rw-r--r--   0        0        0     3981 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/risks.py
+-rw-r--r--   0        0        0     2784 2023-06-14 20:56:28.089279 censys-2.2.3/censys/asm/seeds.py
+-rw-r--r--   0        0        0      675 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/args.py
+-rw-r--r--   0        0        0      174 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2045 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/account.py
+-rw-r--r--   0        0        0     6793 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/asm.py
+-rw-r--r--   0        0        0     3171 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/config.py
+-rw-r--r--   0        0        0     5526 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/hnri.py
+-rw-r--r--   0        0        0     6603 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/search.py
+-rw-r--r--   0        0        0     3492 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/subdomains.py
+-rw-r--r--   0        0        0     3760 2023-06-14 20:56:28.089279 censys-2.2.3/censys/cli/commands/view.py
+-rw-r--r--   0        0        0   233252 2023-06-14 20:56:28.093281 censys-2.2.3/censys/cli/data/certificates_autocomplete.json
+-rw-r--r--   0        0        0   324545 2023-06-14 20:56:28.093281 censys-2.2.3/censys/cli/data/hosts_autocomplete.json
+-rw-r--r--   0        0        0     3279 2023-06-14 20:56:28.093281 censys-2.2.3/censys/cli/utils.py
+-rw-r--r--   0        0        0      105 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/__init__.py
+-rw-r--r--   0        0        0     8552 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/base.py
+-rw-r--r--   0        0        0     1690 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/config.py
+-rw-r--r--   0        0        0     1106 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/deprecation.py
+-rw-r--r--   0        0        0    12446 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/exceptions.py
+-rw-r--r--   0        0        0      144 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/types.py
+-rw-r--r--   0        0        0      797 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/utils.py
+-rw-r--r--   0        0        0      242 2023-06-14 20:56:28.093281 censys-2.2.3/censys/common/version.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:56:28.093281 censys-2.2.3/censys/py.typed
+-rw-r--r--   0        0        0      375 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/__init__.py
+-rw-r--r--   0        0        0     2133 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/client.py
+-rw-r--r--   0        0        0      169 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v1/__init__.py
+-rw-r--r--   0        0        0     5805 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v1/api.py
+-rw-r--r--   0        0        0     1830 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v1/certificates.py
+-rw-r--r--   0        0        0     1224 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v1/data.py
+-rw-r--r--   0        0        0      151 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v2/__init__.py
+-rw-r--r--   0        0        0    17200 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v2/api.py
+-rw-r--r--   0        0        0    12823 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v2/certs.py
+-rw-r--r--   0        0        0    10573 2023-06-14 20:56:28.093281 censys-2.2.3/censys/search/v2/hosts.py
+-rw-r--r--   0        0        0     3400 2023-06-14 20:56:28.097283 censys-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7095 1970-01-01 00:00:00.000000 censys-2.2.3/PKG-INFO
```

### Comparing `censys-2.2.2/LICENSE` & `censys-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/README.md` & `censys-2.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 To upgraded using `pip`.
 
 ```sh
 pip install --upgrade censys
 ```
 
-Or, you can install the library from source using `poetry`.
+Alternatively, you can install the library using `poetry`.
 
 ```sh
 git clone https://github.com/censys/censys-python.git
 cd censys-python/
 poetry install
 ```
 
@@ -61,26 +61,30 @@
 Censys API ID: XXX
 Censys API Secret: XXX
 Do you want color output? [y/n]: y
 
 Successfully authenticated for your@email.com
 ```
 
-To configure your ASM credentials run `censys asm config` or set the `CENSYS_ASM_API_KEY` environment variables.
+If you have a Censys ASM account, you can configure your ASM credentials by running `censys asm config` or set both `CENSYS_ASM_API_KEY` environment variables.
 
 ```sh
 $ censys asm config
 
 Censys ASM API Key: XXX
 Do you want color output? [y/n]: y
 
 Successfully authenticated
 ```
 
-## API Reference and User Guide available on [Read the Docs](https://censys-python.readthedocs.io/)
+## Examples
+
+The examples located in the [`examples/`](examples/) directory are a great place to start. You can also find more examples in the [usage documentation](https://censys-python.readthedocs.io/en/stable/usage-v2.html).
+
+## [Documentation](https://censys-python.readthedocs.io/)
 
 [![Read the Docs](https://raw.githubusercontent.com/censys/censys-python/main/docs/_static/readthedocs.png)](https://censys-python.readthedocs.io/)
 
 ## Resources
 
 - [Source](https://github.com/censys/censys-python)
 - [Issue Tracker](https://github.com/censys/censys-python/issues)
@@ -113,8 +117,8 @@
 poetry run pytest --cov-report html
 ```
 
 ## License
 
 This software is licensed under [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
 
-- Copyright (C) 2022 Censys, Inc.
+- Copyright (C) 2023 Censys, Inc.
```

#### html2text {}

```diff
@@ -21,28 +21,31 @@
 (https://censys-python.readthedocs.io/en/stable/usage-v1.html#bulk) - [Download
 Bulk Data](https://censys-python.readthedocs.io/en/stable/usage-v1.html#data) -
 [Manage assets, events, and seeds in Censys ASM](https://censys-
 python.readthedocs.io/en/stable/usage-asm.html) - [Command-line interface]
 (https://censys-python.readthedocs.io/en/stable/cli.html)  [https://
 asciinema.org/a/500416.svg]  ## Getting Started The library can be installed
 using `pip`. ```sh pip install censys ``` To upgraded using `pip`. ```sh pip
-install --upgrade censys ``` Or, you can install the library from source using
+install --upgrade censys ``` Alternatively, you can install the library using
 `poetry`. ```sh git clone https://github.com/censys/censys-python.git cd
 censys-python/ poetry install ``` Optionally, you can enable tab completion for
 the CLI by adding this line to your `~/.bashrc`, `~/.zshrc`, or equivalent. >
 Please note that autocomplete is supported for field names in the `search`
 command. ```sh eval "$(register-python-argcomplete censys)" ``` To configure
 your search credentials run `censys config` or set both `CENSYS_API_ID` and
 `CENSYS_API_SECRET` environment variables. ```sh $ censys config Censys API ID:
 XXX Censys API Secret: XXX Do you want color output? [y/n]: y Successfully
-authenticated for your@email.com ``` To configure your ASM credentials run
-`censys asm config` or set the `CENSYS_ASM_API_KEY` environment variables.
-```sh $ censys asm config Censys ASM API Key: XXX Do you want color output? [y/
-n]: y Successfully authenticated ``` ## API Reference and User Guide available
-on [Read the Docs](https://censys-python.readthedocs.io/) [![Read the Docs]
+authenticated for your@email.com ``` If you have a Censys ASM account, you can
+configure your ASM credentials by running `censys asm config` or set both
+`CENSYS_ASM_API_KEY` environment variables. ```sh $ censys asm config Censys
+ASM API Key: XXX Do you want color output? [y/n]: y Successfully authenticated
+``` ## Examples The examples located in the [`examples/`](examples/) directory
+are a great place to start. You can also find more examples in the [usage
+documentation](https://censys-python.readthedocs.io/en/stable/usage-v2.html).
+## [Documentation](https://censys-python.readthedocs.io/) [![Read the Docs]
 (https://raw.githubusercontent.com/censys/censys-python/main/docs/_static/
 readthedocs.png)](https://censys-python.readthedocs.io/) ## Resources -
 [Source](https://github.com/censys/censys-python) - [Issue Tracker](https://
 github.com/censys/censys-python/issues) - [Changelog](https://github.com/
 censys/censys-python/releases) - [Documentation](https://censys-python.rtfd.io)
 - [Discussions](https://github.com/censys/censys-python/discussions) - [Censys
 Homepage](https://censys.io/) - [Censys Search](https://search.censys.io/) ##
@@ -50,8 +53,8 @@
 [Contributing to Censys Python](.github/CONTRIBUTING.md) ## Development This
 project uses [poetry](https://python-poetry.org/) for dependency management.
 Please ensure you have [installed the latest version](https://python-
 poetry.org/docs/#installation). ```sh git clone git@github.com:censys/censys-
 python.git cd censys-python/ poetry install ``` ## Testing ```sh # Run tests
 poetry run pytest # With coverage report poetry run pytest --cov-report html
 ``` ## License This software is licensed under [Apache License, Version 2.0]
-(http://www.apache.org/licenses/LICENSE-2.0) - Copyright (C) 2022 Censys, Inc.
+(http://www.apache.org/licenses/LICENSE-2.0) - Copyright (C) 2023 Censys, Inc.
```

### Comparing `censys-2.2.2/censys/asm/__init__.py` & `censys-2.2.3/censys/asm/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,28 +3,31 @@
     Assets,
     CertificatesAssets,
     DomainsAssets,
     HostsAssets,
     SubdomainsAssets,
     WebEntitiesAssets,
 )
+from .beta import Beta
 from .client import AsmClient
 from .clouds import Clouds
-from .events import Events
 from .inventory import InventorySearch
+from .logbook import Events, Logbook
 from .risks import Risks
 from .seeds import Seeds
 
 __all__ = [
     "AsmClient",
     "Assets",
+    "Beta",
     "CertificatesAssets",
     "Clouds",
     "DomainsAssets",
     "Events",
     "HostsAssets",
     "InventorySearch",
+    "Logbook",
     "Risks",
     "Seeds",
     "SubdomainsAssets",
     "WebEntitiesAssets",
 ]
```

### Comparing `censys-2.2.2/censys/asm/api.py` & `censys-2.2.3/censys/asm/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/asm/assets/assets.py` & `censys-2.2.3/censys/asm/assets/assets.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,39 @@
 
 HEX_REGEX = re.compile(r"^#(?:[0-9a-fA-F]{3}){1,2}$")
 
 
 class Assets(CensysAsmAPI):
     """Assets API class."""
 
+    asset_type: str
+
     def __init__(self, asset_type: str, *args, **kwargs):
         """Inits Assets.
 
         Args:
             asset_type (str): Type of asset to interact with.
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
         """
         CensysAsmAPI.__init__(self, *args, **kwargs)
-        self.base_path = f"/v1/assets/{asset_type}"
+        api_version = kwargs.get("api_version", "v1")
+        self.base_path = f"/{api_version}/assets/{asset_type}"
+        self.asset_type = asset_type
+
+    def _format_asset_id(self, asset_id: str) -> str:
+        """Formats asset ID.
+
+        Args:
+            asset_id (str): Asset ID to format.
+
+        Returns:
+            str: Formatted asset ID.
+        """
+        return asset_id
 
     def get_assets(
         self,
         page_number: int = 1,
         page_size: Optional[int] = None,
         tag: Optional[List[str]] = None,
         tag_operator: Optional[str] = None,
@@ -62,15 +77,15 @@
 
         Args:
             asset_id (str): Requested asset ID.
 
         Returns:
             dict: Asset search result.
         """
-        path = f"{self.base_path}/{asset_id}"
+        path = f"{self.base_path}/{self._format_asset_id(asset_id)}"
 
         return self._get(path)
 
     def get_comments(
         self,
         asset_id: str,
         page_number: int = 1,
@@ -82,15 +97,15 @@
             asset_id (str): Asset ID for requested comments.
             page_number (int): Optional; Page number to begin at when searching.
             page_size (int): Optional; Page size for retrieving comments.
 
         Returns:
             generator: Comment search results.
         """
-        path = f"{self.base_path}/{asset_id}/comments"
+        path = f"{self.base_path}/{self._format_asset_id(asset_id)}/comments"
 
         return self._get_page(
             path, page_number=page_number, page_size=page_size, keyword="comments"
         )
 
     def get_comment_by_id(self, asset_id: str, comment_id: int) -> dict:
         """Requests a comment on a specified asset by comment ID.
@@ -98,74 +113,78 @@
         Args:
             asset_id (str): Asset ID for requested comments.
             comment_id (int): Requested comment ID.
 
         Returns:
             dict: Comment search result.
         """
-        path = f"{self.base_path}/{asset_id}/comments/{comment_id}"
+        path = (
+            f"{self.base_path}/{self._format_asset_id(asset_id)}/comments/{comment_id}"
+        )
 
         return self._get(path)
 
     def add_comment(self, asset_id: str, comment: str) -> dict:
         """Adds a comment to a specified asset on the ASM platform.
 
         Args:
             asset_id (str): Asset ID to add comment to.
             comment (str): New comment text.
 
         Returns:
             dict: Added comment results.
         """
-        path = f"{self.base_path}/{asset_id}/comments"
+        path = f"{self.base_path}/{self._format_asset_id(asset_id)}/comments"
         data = {"markdown": str(comment)}
 
         return self._post(path, data=data)
 
     def delete_comment(self, asset_id: str, comment_id: int) -> dict:
         """Deletes a comment from a specified asset on the ASM platform by comment ID.
 
         Args:
             asset_id (str): Asset ID to delete comment from.
             comment_id (int): Comment ID to delete.
 
         Returns:
             dict: Deleted comment results.
         """
-        path = f"{self.base_path}/{asset_id}/comments/{comment_id}"
+        path = (
+            f"{self.base_path}/{self._format_asset_id(asset_id)}/comments/{comment_id}"
+        )
 
         return self._delete(path)
 
     def add_tag(self, asset_id: str, name: str, color: Optional[str] = None) -> dict:
         """Adds a tag to a specified asset on the ASM platform.
 
         Args:
             asset_id (str): Asset ID to add tag to.
             name (str): New tag name.
             color (str): Optional; New tag color (hex).
 
         Returns:
             dict: Added tag results.
         """
-        path = f"{self.base_path}/{asset_id}/tags"
+        path = f"{self.base_path}/{self._format_asset_id(asset_id)}/tags"
         data = format_tag(name, color)
 
         return self._post(path, data=data)
 
     def delete_tag(self, asset_id: str, name: str) -> dict:
         """Deletes a tag from a specified asset on the ASM platform by tag name.
 
         Args:
             asset_id (str): Asset ID to delete tag from.
             name (str): Tag name to delete.
 
         Returns:
             dict: Deleted tag results.
         """
-        path = f"{self.base_path}/{asset_id}/tags/{name}"
+        path = f"{self.base_path}/{self._format_asset_id(asset_id)}/tags/{name}"
 
         return self._delete(path)
 
 
 def format_tag(name: str, color: Optional[str] = None) -> dict:
     """Formats tag name and color request data.
```

### Comparing `censys-2.2.2/censys/asm/assets/domains.py` & `censys-2.2.3/censys/asm/assets/domains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/asm/assets/subdomains.py` & `censys-2.2.3/censys/asm/assets/subdomains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/asm/assets/web_entities.py` & `censys-2.2.3/censys/asm/assets/web_entities.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/asm/client.py` & `censys-2.2.3/censys/asm/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Interact with the Censys Seeds, Assets, and Logbook APIs."""
 from typing import Optional
 
 from .assets import (
     CertificatesAssets,
     DomainsAssets,
     HostsAssets,
+    ObjectStorageAssets,
     SubdomainsAssets,
     WebEntitiesAssets,
 )
+from .beta import Beta
 from .clouds import Clouds
-from .events import Events
 from .inventory import InventorySearch
+from .logbook import Logbook
 from .risks import Risks
 from .seeds import Seeds
 
 
 class AsmClient:
     """Client ASM API class."""
 
@@ -25,19 +27,22 @@
             api_key (str): Optional; The API Key provided by Censys.
             **kwargs: Arbitrary keyword arguments.
         """
         self.seeds = Seeds(api_key, **kwargs)
         self.hosts = HostsAssets(api_key, **kwargs)
         self.certificates = CertificatesAssets(api_key, **kwargs)
         self.domains = DomainsAssets(api_key, **kwargs)
-        self.events = Events(api_key, **kwargs)
+        self.logbook = Logbook(api_key, **kwargs)
+        self.events = self.logbook
         self.clouds = Clouds(api_key, **kwargs)
         self.risks = Risks(api_key, **kwargs)
         self.inventory = InventorySearch(api_key, **kwargs)
+        self.object_storage = ObjectStorageAssets(api_key, **kwargs)
         self.web_entities = WebEntitiesAssets(api_key, **kwargs)
+        self.beta = Beta(api_key, **kwargs)
 
         # Save the arguments for parameterized client usage
         self.__api_kwargs = kwargs
 
     def get_subdomains(self, domain: str):
         """Get an API instance for subdomains of the parent domain.
```

### Comparing `censys-2.2.2/censys/asm/clouds.py` & `censys-2.2.3/censys/asm/clouds.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,69 @@
 """Interact with the Censys Clouds API."""
-import datetime
-from typing import Union
-
+from ..common.types import Datetime
+from ..common.utils import format_iso8601
 from .api import CensysAsmAPI
 
-Since = Union[str, datetime.date, datetime.datetime]
-
-
-def format_since_date(since: Since) -> str:
-    """Formats since date as ISO 8601 format.
-
-    Args:
-        since (Since): Date.
-
-    Returns:
-        str: ISO 8601 formatted date string.
-    """
-    if isinstance(since, (datetime.date, datetime.datetime)):
-        return since.strftime("%Y-%m-%d")
-    return since
-
 
 class Clouds(CensysAsmAPI):
     """Clouds API class."""
 
     base_path = "/v1/clouds"
 
     def get_host_counts(
         self,
-        since: Since,
+        since: Datetime,
     ) -> dict:
         """Retrieve host counts by cloud.
 
         Hosts found after the date provided in the `since` parameter will be included in the new asset counts.
 
         Args:
-            since (Since): Date to include hosts from.
+            since (Datetime): Date to include hosts from.
 
         Returns:
             dict: Host count result.
         """
-        since = format_since_date(since)
+        since = format_iso8601(since)
         return self._get(f"{self.base_path}/hostCounts/{since}")
 
-    def get_domain_counts(self, since: Since) -> dict:
+    def get_domain_counts(self, since: Datetime) -> dict:
         """Retrieve domain counts by cloud.
 
         Args:
-            since (Since): Date to include domains from.
+            since (Datetime): Date to include domains from.
 
         Returns:
             dict: Domain count result.
         """
-        since = format_since_date(since)
+        since = format_iso8601(since)
         return self._get(f"{self.base_path}/domainCounts/{since}")
 
-    def get_object_store_counts(self, since: Since) -> dict:
+    def get_object_store_counts(self, since: Datetime) -> dict:
         """Retrieve object store counts by cloud.
 
         Args:
-            since (Since): Date to include object stores from.
+            since (Datetime): Date to include object stores from.
 
         Returns:
             dict: Object store count result.
         """
-        since = format_since_date(since)
+        since = format_iso8601(since)
         return self._get(f"{self.base_path}/objectStoreCounts/{since}")
 
-    def get_subdomain_counts(self, since: Since) -> dict:
+    def get_subdomain_counts(self, since: Datetime) -> dict:
         """Retrieve subdomain counts by cloud.
 
         Args:
-            since (Since): Date to include subdomains from.
+            since (Datetime): Date to include subdomains from.
 
         Returns:
             dict: Subdomain count result.
         """
-        since = format_since_date(since)
+        since = format_iso8601(since)
         return self._get(f"{self.base_path}/subdomainCounts/{since}")
 
     def get_unknown_counts(self) -> dict:
         """Retrieve known and unknown counts for hosts by cloud.
 
         Returns:
             dict: Unknown count result.
```

### Comparing `censys-2.2.2/censys/asm/events.py` & `censys-2.2.3/censys/asm/logbook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Interact with the Censys Logbook API."""
 import datetime
 from typing import Iterator, List, Optional, Union
 
 from .api import CensysAsmAPI
 
 
-class Events(CensysAsmAPI):
-    """Events API class."""
+class Logbook(CensysAsmAPI):
+    """Logbook API class."""
 
     base_path = "/v1/logbook"
 
     def get_cursor(
         self,
         start: Optional[Union[datetime.datetime, int]] = None,
         filters: Optional[List[str]] = None,
@@ -39,14 +39,18 @@
             dict: Logbook event.
         """
         args = {"cursor": cursor}
 
         yield from self._get_logbook_page(self.base_path, args)
 
 
+# Alias for backwards compatibility
+Events = Logbook
+
+
 class Filters:
     """Logbook filters class."""
 
     CERT = "CERT"
     CERT_RISK = "CERT_RISK"
     DOMAIN = "DOMAIN"
     DOMAIN_EXPIRATION_DATE = "DOMAIN_EXPIRATION_DATE"
```

### Comparing `censys-2.2.2/censys/asm/inventory.py` & `censys-2.2.3/censys/asm/inventory.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/asm/risks.py` & `censys-2.2.3/censys/asm/risks.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/asm/seeds.py` & `censys-2.2.3/censys/asm/seeds.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/__init__.py` & `censys-2.2.3/censys/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/args.py` & `censys-2.2.3/censys/cli/args.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/commands/account.py` & `censys-2.2.3/censys/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/commands/asm.py` & `censys-2.2.3/censys/cli/commands/asm.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/commands/config.py` & `censys-2.2.3/censys/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/commands/hnri.py` & `censys-2.2.3/censys/cli/commands/hnri.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/commands/search.py` & `censys-2.2.3/censys/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/commands/subdomains.py` & `censys-2.2.3/censys/cli/commands/subdomains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/commands/view.py` & `censys-2.2.3/censys/cli/commands/view.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/data/certificates_autocomplete.json` & `censys-2.2.3/censys/cli/data/certificates_autocomplete.json`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/data/hosts_autocomplete.json` & `censys-2.2.3/censys/cli/data/hosts_autocomplete.json`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/cli/utils.py` & `censys-2.2.3/censys/cli/utils.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/common/base.py` & `censys-2.2.3/censys/common/base.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/common/config.py` & `censys-2.2.3/censys/common/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/common/deprecation.py` & `censys-2.2.3/censys/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/common/exceptions.py` & `censys-2.2.3/censys/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/search/client.py` & `censys-2.2.3/censys/search/client.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/search/v1/api.py` & `censys-2.2.3/censys/search/v1/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/search/v1/certificates.py` & `censys-2.2.3/censys/search/v1/certificates.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/search/v1/data.py` & `censys-2.2.3/censys/search/v1/data.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/search/v2/api.py` & `censys-2.2.3/censys/search/v2/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/search/v2/certs.py` & `censys-2.2.3/censys/search/v2/certs.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.2/censys/search/v2/hosts.py` & `censys-2.2.3/censys/search/v2/hosts.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         Inits Censys Hosts.
 
         >>> from censys.search import CensysHosts
         >>> h = CensysHosts()
 
         Simple host search.
 
-        >>> for page in h.search("service.service_name: HTTP"):
+        >>> for page in h.search("services.service_name: HTTP"):
         >>>     print(page)
         [
             {
             'services':
                 [
                     {'service_name': 'HTTP', 'port': 80},
                     {'service_name': 'HTTP', 'port': 443}
@@ -38,27 +38,27 @@
             'ip': '8.8.8.8',
             'services': [{}],
             ...
         }
 
         Simple host aggregate.
 
-        >>> h.aggregate("service.service_name: HTTP", "services.port", num_buckets=5)
+        >>> h.aggregate("services.service_name: HTTP", "services.port", num_buckets=5)
         {
             'total_omitted': 591527370,
             'buckets': [
                 {'count': 56104072, 'key': '80'},
                 {'count': 43527894, 'key': '443'},
                 {'count': 23070429, 'key': '7547'},
                 {'count': 12970769, 'key': '30005'},
                 {'count': 12825150, 'key': '22'}
             ],
             'potential_deviation': 3985101,
             'field': 'services.port',
-            'query': 'service.service_name: HTTP',
+            'query': 'services.service_name: HTTP',
             'total': 172588754
         }
 
         Fetch a list of host names for the specified IP address.
 
         >>> h.view_host_names("1.1.1.1")
         ['one.one.one.one']
```

### Comparing `censys-2.2.2/pyproject.toml` & `censys-2.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censys"
-version = "2.2.2"
+version = "2.2.3"
 description = "An easy-to-use and lightweight API wrapper for Censys APIs (censys.io)."
 authors = ["Censys, Inc. <support@censys.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = ["censys/py.typed"]
 keywords = ["censys", "api", "search", "attack surface management"]
 classifiers = [
@@ -49,15 +49,15 @@
 
 [tool.poetry.scripts]
 censys = "censys.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4.0.0"
 requests = ">=2.29.0"
-urllib3 = "<2.0.0" # Waiting until requests supports urllib3>=2.0.0
+urllib3 = "<3.0.0"
 backoff = ">=2.0.0,<3.0.0"
 rich = ">=10.16.2"
 importlib-metadata = { version = "*", python = "<3.8" }
 argcomplete = ">=2.0.0,<4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 # Lint
```

### Comparing `censys-2.2.2/PKG-INFO` & `censys-2.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censys
-Version: 2.2.2
+Version: 2.2.3
 Summary: An easy-to-use and lightweight API wrapper for Censys APIs (censys.io).
 License: Apache-2.0
 Keywords: censys,api,search,attack surface management
 Author: Censys, Inc.
 Author-email: support@censys.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,21 +18,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
@@ -41,15 +36,15 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: argcomplete (>=2.0.0,<4.0.0)
 Requires-Dist: backoff (>=2.0.0,<3.0.0)
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: requests (>=2.29.0)
 Requires-Dist: rich (>=10.16.2)
-Requires-Dist: urllib3 (<2.0.0)
+Requires-Dist: urllib3 (<3.0.0)
 Project-URL: Censys Homepage, https://censys.io/
 Project-URL: Censys Search, https://search.censys.io/
 Project-URL: Changelog, https://github.com/censys/censys-python/releases
 Project-URL: Discussions, https://github.com/censys/censys-python/discussions
 Project-URL: Documentation, https://censys-python.rtfd.io
 Project-URL: Source, https://github.com/censys/censys-python
 Project-URL: Tracker, https://github.com/censys/censys-python/issues
@@ -90,15 +85,15 @@
 
 To upgraded using `pip`.
 
 ```sh
 pip install --upgrade censys
 ```
 
-Or, you can install the library from source using `poetry`.
+Alternatively, you can install the library using `poetry`.
 
 ```sh
 git clone https://github.com/censys/censys-python.git
 cd censys-python/
 poetry install
 ```
 
@@ -118,26 +113,30 @@
 Censys API ID: XXX
 Censys API Secret: XXX
 Do you want color output? [y/n]: y
 
 Successfully authenticated for your@email.com
 ```
 
-To configure your ASM credentials run `censys asm config` or set the `CENSYS_ASM_API_KEY` environment variables.
+If you have a Censys ASM account, you can configure your ASM credentials by running `censys asm config` or set both `CENSYS_ASM_API_KEY` environment variables.
 
 ```sh
 $ censys asm config
 
 Censys ASM API Key: XXX
 Do you want color output? [y/n]: y
 
 Successfully authenticated
 ```
 
-## API Reference and User Guide available on [Read the Docs](https://censys-python.readthedocs.io/)
+## Examples
+
+The examples located in the [`examples/`](examples/) directory are a great place to start. You can also find more examples in the [usage documentation](https://censys-python.readthedocs.io/en/stable/usage-v2.html).
+
+## [Documentation](https://censys-python.readthedocs.io/)
 
 [![Read the Docs](https://raw.githubusercontent.com/censys/censys-python/main/docs/_static/readthedocs.png)](https://censys-python.readthedocs.io/)
 
 ## Resources
 
 - [Source](https://github.com/censys/censys-python)
 - [Issue Tracker](https://github.com/censys/censys-python/issues)
@@ -170,9 +169,9 @@
 poetry run pytest --cov-report html
 ```
 
 ## License
 
 This software is licensed under [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
 
-- Copyright (C) 2022 Censys, Inc.
+- Copyright (C) 2023 Censys, Inc.
```

