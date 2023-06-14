# Comparing `tmp/meltanolabs_target_snowflake-0.1.1a1.tar.gz` & `tmp/meltanolabs_target_snowflake-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.1.1a1.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.2.0.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.1.1a1.tar` & `meltanolabs_target_snowflake-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3135 2023-04-17 21:16:34.330190 meltanolabs_target_snowflake-0.1.1a1/README.md
--rw-r--r--   0        0        0     1091 2023-04-17 21:17:03.655981 meltanolabs_target_snowflake-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-17 21:17:03.655981 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/__init__.py
--rw-r--r--   0        0        0    15115 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/sinks.py
--rw-r--r--   0        0        0     2163 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/target.py
--rw-r--r--   0        0        0       39 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/tests/__init__.py
--rw-r--r--   0        0        0      656 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/tests/test_core.py
--rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-06-14 14:59:00.277687 meltanolabs_target_snowflake-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3924 2023-06-14 14:59:00.277687 meltanolabs_target_snowflake-0.2.0/README.md
+-rw-r--r--   0        0        0     1282 2023-06-14 14:59:23.657910 meltanolabs_target_snowflake-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-06-14 14:59:23.657910 meltanolabs_target_snowflake-0.2.0/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    16204 2023-06-14 14:59:00.281687 meltanolabs_target_snowflake-0.2.0/target_snowflake/connector.py
+-rw-r--r--   0        0        0     7060 2023-06-14 14:59:00.281687 meltanolabs_target_snowflake-0.2.0/target_snowflake/sinks.py
+-rw-r--r--   0        0        0     4057 2023-06-14 14:59:00.281687 meltanolabs_target_snowflake-0.2.0/target_snowflake/target.py
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.2.0/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.1.1a1/pyproject.toml` & `meltanolabs_target_snowflake-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.1.1-a.1"
+version = "0.2.0"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
 license = "Apache 2.0"
 packages = [
     { include = "target_snowflake" }
 ]
 
 [tool.poetry.dependencies]
-python = "<3.11,>=3.7.1"
-requests = "^2.25.1"
-singer-sdk = "0.17.0"
+python = "<3.12,>=3.7.1"
+requests = "^2.31.0"
 snowflake-sqlalchemy = "^1.4.1"
+singer-sdk = "0.28.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-tox = "^3.24.4"
-flake8 = "^3.9.2"
-black = "^21.9b0"
-pydocstyle = "^6.1.1"
-mypy = "^0.910"
-types-requests = "^2.26.1"
-isort = "^5.10.1"
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3 # Vertical Hanging Indent
-src_paths = "target_snowflake"
+pytest = "^7.3.1"
+singer-sdk = { version="0.28.0", extras = ["testing"] }
+
+[tool.poetry.group.dev.dependencies]
+coverage = "^7.2.7"
+
+[tool.ruff]
+ignore = [
+    "ANN101",  # missing-type-self
+    "ANN102",  # missing-type-cls
+]
+select = ["ALL"]
+src = ["target_snowflake"]
+target-version = "py37"
+
+[tool.ruff.flake8-annotations]
+allow-star-arg-any = true
+
+[tool.ruff.isort]
+known-first-party = ["target_snowflake"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
 
 [build-system]
 requires = ["poetry-core>=1.0.8", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
 # CLI declaration
```

