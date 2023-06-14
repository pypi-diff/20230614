# Comparing `tmp/tgwrap-0.6.2.tar.gz` & `tmp/tgwrap-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.6.2.tar", max compression
+gzip compressed data, was "tgwrap-0.6.3.tar", max compression
```

## Comparing `tgwrap-0.6.2.tar` & `tgwrap-0.6.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.6.2/LICENSE
--rw-r--r--   0        0        0     7169 2023-05-26 12:45:31.451829 tgwrap-0.6.2/README.md
--rw-r--r--   0        0        0      902 2023-06-02 09:54:17.516206 tgwrap-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.6.2/tgwrap/__init__.py
--rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.6.2/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    25922 2023-05-26 13:18:56.546086 tgwrap-0.6.2/tgwrap/cli.py
--rwxr-xr-x   0        0        0    56767 2023-06-02 09:52:17.133141 tgwrap-0.6.2/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.6.2/tgwrap/printer.py
--rw-r--r--   0        0        0     8321 1970-01-01 00:00:00.000000 tgwrap-0.6.2/setup.py
--rw-r--r--   0        0        0     8252 1970-01-01 00:00:00.000000 tgwrap-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.6.3/LICENSE
+-rw-r--r--   0        0        0     7169 2023-05-26 12:45:31.451829 tgwrap-0.6.3/README.md
+-rw-r--r--   0        0        0      902 2023-06-14 08:03:33.130998 tgwrap-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.6.3/tgwrap/__init__.py
+-rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.6.3/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    25922 2023-05-26 13:18:56.546086 tgwrap-0.6.3/tgwrap/cli.py
+-rwxr-xr-x   0        0        0    56945 2023-06-14 08:01:07.947011 tgwrap-0.6.3/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.6.3/tgwrap/printer.py
+-rw-r--r--   0        0        0     8321 1970-01-01 00:00:00.000000 tgwrap-0.6.3/setup.py
+-rw-r--r--   0        0        0     8252 1970-01-01 00:00:00.000000 tgwrap-0.6.3/PKG-INFO
```

### Comparing `tgwrap-0.6.2/LICENSE` & `tgwrap-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.2/README.md` & `tgwrap-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.2/pyproject.toml` & `tgwrap-0.6.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.6.2"
+version = "0.6.3"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.6.2/tgwrap/analyze.py` & `tgwrap-0.6.3/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.2/tgwrap/cli.py` & `tgwrap-0.6.3/tgwrap/cli.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.2/tgwrap/main.py` & `tgwrap-0.6.3/tgwrap/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1219,23 +1219,26 @@
             self.printer.header(
                 'Deployed versions:' if len(versions) > 0 else 'No deployed versions detected'
                 )
             
             for version in versions:
                 days_since_release = version.get("days_since_release", 0)
                 message = f'-> {version["path"]}: {version["tag"]} (released {days_since_release} days ago)'
-                if days_since_release > 60:
+                if version['release_date'] == 'unknown':
+                    self.printer.normal(message)
+                elif days_since_release > 60:
                     self.printer.error(message)
                 elif days_since_release > 30:
                     self.printer.error(message)
                 elif days_since_release < 7:
                     self.printer.success(message)
                 else:
                     self.printer.normal(message)
 
+            self.printer.normal("\n") # just to get an empty line :-/
             self.printer.warning("""
 Note:
     This result only says something about the freshness of the deployed configurations,
     but not whether the actual resources are in sync with these.
     Check the drift of these configurations with the actual deployments by
     planning and analyzing the results.
             """)
```

### Comparing `tgwrap-0.6.2/tgwrap/printer.py` & `tgwrap-0.6.3/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.2/setup.py` & `tgwrap-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'terrasafe>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['tgwrap = tgwrap.cli:main']}
 
 setup_kwargs = {
     'name': 'tgwrap',
-    'version': '0.6.2',
+    'version': '0.6.3',
     'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
     'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.\n\nIt needs a config file as follows:\n\n```yaml\n---\n#\n# Critically of resources as interpreted by \'tgwrap analyze\'.\n# It uses it for a \'terrasafe\' like validation if resources can safely be deleted.\n# On top of that it tries to analyze and quantify the drift impact of the changes,\n# so that this can be monitored.\n#\nlow:\n  # defaults:\n  #   terrasafe_level: ignore_deletions\n  #   drift_impact:\n  #     default: minor\n  #     delete: medium\n  azuread_application.: {} # if we you want to use the defaults\n  azuread_app_role_assignment: # or if you want to override these\n    drift_impact:\n      delete: minor\n  # and so on, and so forth\nmedium:\n  # defaults:\n  #   terrasafe_level: ignore_deletion_if_recreation\n  #   drift_impact:\n  #     default: medium\n  #     delete: major\n  azurerm_data_factory_linked_service_key_vault.: {}\n  # and so on, and so forth\nhigh:\n  # defaults:\n  #   terrasafe_level: unauthorized_deletion\n  #   drift_impact:\n  #     default: major\n  #     update: medium\n  azuread_group.:\n    drift_impact:\n      create: minor\n      update: minor\n  azurerm_application_insights.: {}\n  # and so on, and so forth\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/lunadata/tgwrap',
```

### Comparing `tgwrap-0.6.2/PKG-INFO` & `tgwrap-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.6.2
+Version: 0.6.3
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
```

