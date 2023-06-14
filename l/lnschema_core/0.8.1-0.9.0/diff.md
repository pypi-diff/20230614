# Comparing `tmp/lnschema_core-0.8.1.tar.gz` & `tmp/lnschema_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_core-0.8.1.tar", last modified: Mon Sep 26 11:57:43 2022, max compression
+gzip compressed data, was "lnschema_core-0.9.0.tar", last modified: Fri Sep 30 06:25:52 2022, max compression
```

## Comparing `lnschema_core-0.8.1.tar` & `lnschema_core-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     2483 2022-08-19 10:09:17.295659 lnschema_core-0.8.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-23 06:43:02.921791 lnschema_core-0.8.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-23 06:43:02.922104 lnschema_core-0.8.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1200 2022-08-19 10:09:17.295787 lnschema_core-0.8.1/.gitignore
--rw-r--r--   0        0        0     1753 2022-07-23 06:43:02.901998 lnschema_core-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2022-07-23 06:43:02.901038 lnschema_core-0.8.1/LICENSE
--rw-r--r--   0        0        0      230 2022-08-22 19:24:56.660829 lnschema_core-0.8.1/README.md
--rw-r--r--   0        0        0       55 2022-08-19 10:09:17.296021 lnschema_core-0.8.1/docs/api.md
--rw-r--r--   0        0        0     4857 2022-09-26 11:57:12.681089 lnschema_core-0.8.1/docs/changelog.md
--rw-r--r--   0        0        0       49 2022-09-24 06:30:40.670917 lnschema_core-0.8.1/docs/guide/index.md
--rw-r--r--   0        0        0     2523 2022-09-26 11:56:28.912605 lnschema_core-0.8.1/docs/guide/models.ipynb
--rw-r--r--   0        0        0      116 2022-09-24 06:30:40.671322 lnschema_core-0.8.1/docs/index.md
--rw-r--r--   0        0        0     3224 2022-09-24 06:30:40.672068 lnschema_core-0.8.1/docs/notes/2022-09-18-fix.ipynb
--rw-r--r--   0        0        0       49 2022-09-24 06:30:40.672314 lnschema_core-0.8.1/docs/notes/index.md
--rw-r--r--   0        0        0      144 2022-08-22 19:25:17.353750 lnschema_core-0.8.1/lamin-project.yaml
--rw-r--r--   0        0        0      958 2022-09-26 11:57:01.945094 lnschema_core-0.8.1/lnschema_core/__init__.py
--rw-r--r--   0        0        0    12461 2022-09-26 11:56:42.012097 lnschema_core-0.8.1/lnschema_core/_core.py
--rw-r--r--   0        0        0     2596 2022-08-26 18:42:44.483607 lnschema_core-0.8.1/lnschema_core/_id.py
--rw-r--r--   0        0        0      228 2022-09-25 14:48:18.348553 lnschema_core-0.8.1/lnschema_core/_timestamps.py
--rw-r--r--   0        0        0      222 2022-09-24 06:30:40.674364 lnschema_core-0.8.1/lnschema_core/_type.py
--rw-r--r--   0        0        0      715 2022-09-25 14:34:42.651236 lnschema_core-0.8.1/lnschema_core/alembic.ini
--rw-r--r--   0        0        0      964 2022-08-26 18:42:44.484667 lnschema_core-0.8.1/lnschema_core/id.py
--rw-r--r--   0        0        0     1811 2022-09-24 06:30:40.675051 lnschema_core-0.8.1/lnschema_core/migrations/env.py
--rw-r--r--   0        0        0      542 2022-09-24 06:30:40.675275 lnschema_core-0.8.1/lnschema_core/migrations/script.py.mako
--rw-r--r--   0        0        0     3774 2022-09-24 06:30:40.675378 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py
--rw-r--r--   0        0        0     6694 2022-09-24 06:30:40.675476 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py
--rw-r--r--   0        0        0     2073 2022-09-24 06:30:40.675565 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py
--rw-r--r--   0        0        0     4461 2022-09-24 06:30:40.675655 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py
--rw-r--r--   0        0        0     3495 2022-09-24 06:30:40.675742 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py
--rw-r--r--   0        0        0      853 2022-09-24 06:30:40.675826 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py
--rw-r--r--   0        0        0      536 2022-09-24 06:30:40.675906 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py
--rw-r--r--   0        0        0      976 2022-09-24 06:30:40.676224 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py
--rw-r--r--   0        0        0     6662 2022-09-24 06:30:40.676315 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py
--rw-r--r--   0        0        0     2886 2022-09-26 11:56:42.012247 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py
--rw-r--r--   0        0        0      762 2022-09-25 18:44:02.967433 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py
--rw-r--r--   0        0        0      668 2022-09-26 11:56:42.012346 lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py
--rw-r--r--   0        0        0       97 2022-08-26 18:42:44.485140 lnschema_core-0.8.1/lnschema_core/type.py
--rw-r--r--   0        0        0      686 2022-08-19 10:09:17.297020 lnschema_core-0.8.1/noxfile.py
--rw-r--r--   0        0        0      623 2022-08-19 10:09:17.297235 lnschema_core-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      215 2022-08-26 18:42:44.487026 lnschema_core-0.8.1/tests/test_base.py
--rw-r--r--   0        0        0      481 2022-09-24 06:30:40.676895 lnschema_core-0.8.1/tests/test_notebooks.py
--rw-r--r--   0        0        0   262144 2022-09-26 11:56:42.012720 lnschema_core-0.8.1/tests/testdb.lndb
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 lnschema_core-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2564 2022-09-26 14:29:40.490742 lnschema_core-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-23 06:43:02.921791 lnschema_core-0.9.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-23 06:43:02.922104 lnschema_core-0.9.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1200 2022-08-19 10:09:17.295787 lnschema_core-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1753 2022-07-23 06:43:02.901998 lnschema_core-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2022-07-23 06:43:02.901038 lnschema_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0      237 2022-09-26 18:51:01.648333 lnschema_core-0.9.0/README.md
+-rw-r--r--   0        0        0       55 2022-08-19 10:09:17.296021 lnschema_core-0.9.0/docs/api.md
+-rw-r--r--   0        0        0     5160 2022-09-30 06:25:26.884398 lnschema_core-0.9.0/docs/changelog.md
+-rw-r--r--   0        0        0       49 2022-09-24 06:30:40.670917 lnschema_core-0.9.0/docs/guide/index.md
+-rw-r--r--   0        0        0     2523 2022-09-26 11:56:28.912605 lnschema_core-0.9.0/docs/guide/models.ipynb
+-rw-r--r--   0        0        0      841 2022-09-26 19:05:13.593235 lnschema_core-0.9.0/docs/index.md
+-rw-r--r--   0        0        0     3224 2022-09-24 06:30:40.672068 lnschema_core-0.9.0/docs/notes/2022-09-18-fix.ipynb
+-rw-r--r--   0        0        0       49 2022-09-24 06:30:40.672314 lnschema_core-0.9.0/docs/notes/index.md
+-rw-r--r--   0        0        0      144 2022-08-22 19:25:17.353750 lnschema_core-0.9.0/lamin-project.yaml
+-rw-r--r--   0        0        0      962 2022-09-30 06:25:12.477130 lnschema_core-0.9.0/lnschema_core/__init__.py
+-rw-r--r--   0        0        0    11550 2022-09-30 06:23:04.429987 lnschema_core-0.9.0/lnschema_core/_core.py
+-rw-r--r--   0        0        0     2596 2022-08-26 18:42:44.483607 lnschema_core-0.9.0/lnschema_core/_id.py
+-rw-r--r--   0        0        0      228 2022-09-25 14:48:18.348553 lnschema_core-0.9.0/lnschema_core/_timestamps.py
+-rw-r--r--   0        0        0      222 2022-09-24 06:30:40.674364 lnschema_core-0.9.0/lnschema_core/_type.py
+-rw-r--r--   0        0        0      715 2022-09-26 19:54:23.308348 lnschema_core-0.9.0/lnschema_core/alembic.ini
+-rw-r--r--   0        0        0      964 2022-08-26 18:42:44.484667 lnschema_core-0.9.0/lnschema_core/id.py
+-rw-r--r--   0        0        0     1811 2022-09-24 06:30:40.675051 lnschema_core-0.9.0/lnschema_core/migrations/env.py
+-rw-r--r--   0        0        0      542 2022-09-24 06:30:40.675275 lnschema_core-0.9.0/lnschema_core/migrations/script.py.mako
+-rw-r--r--   0        0        0     3774 2022-09-24 06:30:40.675378 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py
+-rw-r--r--   0        0        0     6694 2022-09-24 06:30:40.675476 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py
+-rw-r--r--   0        0        0     2073 2022-09-24 06:30:40.675565 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py
+-rw-r--r--   0        0        0     4461 2022-09-24 06:30:40.675655 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py
+-rw-r--r--   0        0        0     3495 2022-09-24 06:30:40.675742 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py
+-rw-r--r--   0        0        0      853 2022-09-24 06:30:40.675826 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py
+-rw-r--r--   0        0        0      536 2022-09-24 06:30:40.675906 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py
+-rw-r--r--   0        0        0      976 2022-09-24 06:30:40.676224 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py
+-rw-r--r--   0        0        0     6662 2022-09-24 06:30:40.676315 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py
+-rw-r--r--   0        0        0     2886 2022-09-26 11:56:42.012247 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py
+-rw-r--r--   0        0        0      762 2022-09-25 18:44:02.967433 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py
+-rw-r--r--   0        0        0      668 2022-09-26 11:56:42.012346 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py
+-rw-r--r--   0        0        0     1082 2022-09-30 06:23:04.430102 lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-30-439c4ee0a22a-v0_9_0.py
+-rw-r--r--   0        0        0       97 2022-08-26 18:42:44.485140 lnschema_core-0.9.0/lnschema_core/type.py
+-rw-r--r--   0        0        0      814 2022-09-26 14:10:17.444890 lnschema_core-0.9.0/noxfile.py
+-rw-r--r--   0        0        0      623 2022-08-19 10:09:17.297235 lnschema_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      215 2022-08-26 18:42:44.487026 lnschema_core-0.9.0/tests/test_base.py
+-rw-r--r--   0        0        0      481 2022-09-24 06:30:40.676895 lnschema_core-0.9.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0   262144 2022-09-30 06:23:04.430450 lnschema_core-0.9.0/tests/testdb.lndb
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 lnschema_core-0.9.0/PKG-INFO
```

### Comparing `lnschema_core-0.8.1/.github/workflows/build.yml` & `lnschema_core-0.9.0/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -29,27 +29,28 @@
       - name: Setup Python
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - name: Cache
         uses: actions/cache@v3
         env:
-          cache-name: cache-0
+          cache-name: cache-1
         with:
           path: |
             .nox
             ~/.cache/pre-commit
           key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
       - name: Install pip and nox
         run: |
           python -m pip install --upgrade pip
           pip install nox
       - name: Lint
+        if: matrix.python-version == '3.9'
         run: |
-          nox -s lint
+          nox -s lint --python ${{ matrix.python-version }}
       - name: Build
         run: |
           nox -s build --python ${{ matrix.python-version }}
       - name: Codecov
         if: matrix.python-version == '3.9'
         uses: codecov/codecov-action@v2
         with:
```

### Comparing `lnschema_core-0.8.1/.github/workflows/latest-changes.yml` & `lnschema_core-0.9.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/.gitignore` & `lnschema_core-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/.pre-commit-config.yaml` & `lnschema_core-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/LICENSE` & `lnschema_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/docs/changelog.md` & `lnschema_core-0.9.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🏗️ Remove version column from dobject | [39](https://github.com/laminlabs/lnschema-core/pull/39) | [falexwolf](https://github.com/falexwolf) | 2022-09-30 | 0.9.0
+👷 Fix CI setup | [37](https://github.com/laminlabs/lnschema-core/pull/37) | [falexwolf](https://github.com/falexwolf) | 2022-09-26 |
 🚸 Fix type annotations of primary keys and add docstrings everywhere  | [35](https://github.com/laminlabs/lnschema-core/pull/35) | [falexwolf](https://github.com/falexwolf) | 2022-09-26 | 0.8.1
 ✨ Add `size` field to `dobject` | [32](https://github.com/laminlabs/lnschema-core/pull/32) | [falexwolf](https://github.com/falexwolf) | 2022-09-25 | 0.8.0
 🍱 Add migration script | [34](https://github.com/laminlabs/lnschema-core/pull/34) | [falexwolf](https://github.com/falexwolf) | 2022-09-24 | 0.7.3
 🩹 Fix type annotation of timestamps | [33](https://github.com/laminlabs/lnschema-core/pull/33) | [falexwolf](https://github.com/falexwolf) | 2022-09-24 |
 💄 Add noqa to script mako & simpler unique constraint | [31](https://github.com/laminlabs/lnschema-core/pull/31) | [falexwolf](https://github.com/falexwolf) | 2022-09-23 |
 ✨ Add `insert` to `type.usage` | [30](https://github.com/laminlabs/lnschema-core/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2022-09-21 |
 🚚 Move migrations to package | [29](https://github.com/laminlabs/lnschema-core/pull/29) | [falexwolf](https://github.com/falexwolf) | 2022-09-20 | 0.7.2
```

### Comparing `lnschema_core-0.8.1/docs/guide/models.ipynb` & `lnschema_core-0.9.0/docs/guide/models.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/docs/notes/2022-09-18-fix.ipynb` & `lnschema_core-0.9.0/docs/notes/2022-09-18-fix.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/__init__.py` & `lnschema_core-0.9.0/lnschema_core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Schema module core (`yvzi`).
+"""Data provenance & flow (`yvzi`).
 
 Import the package::
 
    import lnschema_core
 
 Data objects & transformations:
 
@@ -46,16 +46,16 @@
 
    type
    id
 
 """
 # This is lnschema-module yvzi.
 _schema_id = "yvzi"
-_migration = "1190648443cb"
-__version__ = "0.8.1"  # denote a pre-release for 0.1.0 with 0.1a1
+_migration = "439c4ee0a22a"
+__version__ = "0.9.0"  # denote a pre-release for 0.1.0 with 0.1a1
 
 from . import id, type  # noqa
 from ._core import (  # noqa
     dobject,
     dtransform,
     dtransform_in,
     jupynb,
```

### Comparing `lnschema_core-0.8.1/lnschema_core/_core.py` & `lnschema_core-0.9.0/lnschema_core/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,26 +78,15 @@
     - Tensor: zarr directory, TileDB store ⟷ zarr loader, TileDB loader
     - Fastq: `.fastq` ⟷ /
     - VCF: `.vcf` ⟷ /
     - QC: `.html` ⟷ /
     """
 
     id: str = Field(default_factory=idg.dobject, primary_key=True)
-    """Universal base62 ID, generated by :func:`~lnschema_core.id.dobject`.
-
-    Any row in dobject is uniquely identified by the composite primary key `(id, v)`.
-    """
-    v: str = Field(default="1", primary_key=True)
-    """Version identifier, defaults to `"1"`.
-
-    Use this to label different versions of the same data object.
-
-    Consider using `semantic versioning <https://semver.org>`__
-    with `Python versioning <https://peps.python.org/pep-0440/>`__.
-    """
+    """Universal base62 ID, generated by :func:`~lnschema_core.id.dobject`."""
     name: Optional[str] = Field(index=True)
     """Semantic name or title. Defaults to `None`."""
     suffix: Optional[str] = Field(default=None, index=True)
     """Suffix to construct the storage key. Defaults to `None`.
 
     This is a file extension if the `dobject` is stored in a file format.
     It's `None` if the storage format doesn't have a canonical extension.
@@ -168,26 +157,17 @@
 
     A data transformation can have an arbitrary number of data objects as inputs.
 
     - The same `dobject` can be used as input in many different `dtransforms`.
     - One `dtransform` can have several `dobjects` as inputs.
     """
 
-    __table_args__ = (
-        ForeignKeyConstraint(
-            ["dobject_id", "dobject_v"],
-            ["dobject.id", "dobject.v"],
-            name="dtransform_in_dobject",
-        ),
-    )
     dtransform_id: str = Field(foreign_key="dtransform.id", primary_key=True)
     """Link to :class:`~lnschema_core.dtransform`."""
-    dobject_id: str = Field(primary_key=True)
-    """Link to :class:`~lnschema_core.dobject`."""
-    dobject_v: str = Field(primary_key=True)
+    dobject_id: str = Field(foreign_key="dobject.id", primary_key=True)
     """Link to :class:`~lnschema_core.dobject`."""
 
 
 class jupynb(SQLModel, table=True):  # type: ignore
     """Jupyter notebooks.
 
     Jupyter notebooks (`jupynbs`) represent one type of data transformation
@@ -263,34 +243,24 @@
 
 class usage(SQLModel, table=True):  # type: ignore
     """Data usage log.
 
     Any API call in the `lamindb.db` API is logged here.
     """
 
-    __table_args__ = (
-        ForeignKeyConstraint(
-            ["dobject_id", "dobject_v"],
-            ["dobject.id", "dobject.v"],
-            name="usage_dobject",
-        ),
-    )
-
     id: str = Field(default_factory=idg.usage, primary_key=True)
     """Universal base62 ID & primary key, generated by :func:`~lnschema_core.id.usage`."""  # noqa
     type: usage_type = Field(nullable=False, index=True)
     """Usage type."""
     user_id: str = Field(foreign_key="user.id", nullable=False, index=True)
     """Link to :class:`~lnschema_core.user`."""
     time: datetime = CreatedAt
     """Time of event."""
-    dobject_id: str = Field(index=True)
+    dobject_id: str = Field(foreign_key="dobject.id", index=True)
     """Link to the affected :class:`~lnschema_core.dobject`."""
-    dobject_v: str = Field(index=True)
-    """Link to :class:`~lnschema_core.dobject`."""
 
 
 class version_yvzi(SQLModel, table=True):  # type: ignore
     """Core schema module versions deployed in a given instance.
 
     Migrations of the schema module add rows to this table, storing the schema
     module version to which we migrated along with the user who performed the
```

### Comparing `lnschema_core-0.8.1/lnschema_core/_id.py` & `lnschema_core-0.9.0/lnschema_core/_id.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/alembic.ini` & `lnschema_core-0.9.0/lnschema_core/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/id.py` & `lnschema_core-0.9.0/lnschema_core/id.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/env.py` & `lnschema_core-0.9.0/lnschema_core/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/script.py.mako` & `lnschema_core-0.9.0/lnschema_core/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py` & `lnschema_core-0.9.0/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/noxfile.py` & `lnschema_core-0.9.0/noxfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from pathlib import Path
 
 import nox
 
 nox.options.reuse_existing_virtualenvs = True
+nox.options.error_on_external_run = False
+nox.options.default_venv_backend = None
 
 
-@nox.session
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
 def lint(session: nox.Session) -> None:
     session.install("pre-commit")
     session.run("pre-commit", "install")
     session.run("pre-commit", "run", "--all-files")
 
 
 @nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
```

### Comparing `lnschema_core-0.8.1/pyproject.toml` & `lnschema_core-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnschema_core-0.8.1/tests/testdb.lndb` & `lnschema_core-0.9.0/tests/testdb.lndb`

 * *Files 5% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -1,63 +1,25 @@
 PRAGMA foreign_keys=OFF;
 BEGIN TRANSACTION;
-CREATE TABLE dtransform_in (
-	dtransform_id VARCHAR NOT NULL, 
-	dobject_id VARCHAR NOT NULL, 
-	dobject_v VARCHAR NOT NULL, 
-	PRIMARY KEY (dtransform_id, dobject_id, dobject_v), 
-	CONSTRAINT dtransform_in_dobject FOREIGN KEY(dobject_id, dobject_v) REFERENCES dobject (id, v), 
-	FOREIGN KEY(dtransform_id) REFERENCES dtransform (id)
-);
 CREATE TABLE migration_yvzi (
 	version_num VARCHAR NOT NULL, 
 	PRIMARY KEY (version_num)
 );
-INSERT INTO migration_yvzi VALUES('1190648443cb');
+INSERT INTO migration_yvzi VALUES('439c4ee0a22a');
 CREATE TABLE IF NOT EXISTS "dtransform" (
 	id VARCHAR NOT NULL, 
 	jupynb_id VARCHAR, 
 	jupynb_v VARCHAR, 
 	pipeline_run_id VARCHAR, 
 	PRIMARY KEY (id), 
 	CONSTRAINT dtransform_jupynb FOREIGN KEY(jupynb_id, jupynb_v) REFERENCES jupynb (id, v), 
 	FOREIGN KEY(pipeline_run_id) REFERENCES pipeline_run (id)
 );
 INSERT INTO dtransform VALUES('GgD4VJbXtOOS','GgD4VJbXtOOS','1',NULL);
 INSERT INTO dtransform VALUES('ZCdINSMzjawp','ZCdINSMzjawp','1',NULL);
-CREATE TABLE IF NOT EXISTS "usage" (
-	id VARCHAR NOT NULL, 
-	type VARCHAR NOT NULL, 
-	user_id VARCHAR NOT NULL, 
-	time DATETIME NOT NULL, 
-	dobject_id VARCHAR NOT NULL, 
-	dobject_v VARCHAR NOT NULL, 
-	PRIMARY KEY (id), 
-	CONSTRAINT usage_dobject FOREIGN KEY(dobject_id, dobject_v) REFERENCES dobject (id, v), 
-	FOREIGN KEY(user_id) REFERENCES user (id)
-);
-INSERT INTO usage VALUES('WO3RxPpY8mS5xgcQsHMlLYKn','ingest','9ypQ1yrW','2022-07-21 18:06:08.000000','4SYxweB1zI1PjgyiYmhHP','1');
-INSERT INTO usage VALUES('muL0I4sGi6hlyQr6NISXI7q5','ingest','9ypQ1yrW','2022-07-21 18:07:54.000000','Jxpe4xf0j5guH3wZgAZEz','1');
-INSERT INTO usage VALUES('uj4rF6GCgLIsZho5LlT70s1j','ingest','tSJNTgoM','2022-07-21 18:08:15.000000','uIHge4bsgwc0ndqcoC9Ii','1');
-CREATE TABLE IF NOT EXISTS "dobject" (
-	id VARCHAR NOT NULL, 
-	v VARCHAR NOT NULL, 
-	name VARCHAR, 
-	dtransform_id VARCHAR NOT NULL, 
-	storage_id VARCHAR NOT NULL, 
-	created_at DATETIME DEFAULT (CURRENT_TIMESTAMP) NOT NULL, 
-	updated_at DATETIME, 
-	suffix VARCHAR, size FLOAT, 
-	PRIMARY KEY (id, v), 
-	CONSTRAINT fk_object_storage_id_storage FOREIGN KEY(storage_id) REFERENCES storage (id), 
-	FOREIGN KEY(dtransform_id) REFERENCES dtransform (id)
-);
-INSERT INTO dobject VALUES('4SYxweB1zI1PjgyiYmhHP','1','scanpy_pbmc68k_reduced','GgD4VJbXtOOS','V2NSFBdCfP','2022-09-18 14:38:37',NULL,'.h5ad',NULL);
-INSERT INTO dobject VALUES('Jxpe4xf0j5guH3wZgAZEz','1','scanpy_pbmc68k_reduced','GgD4VJbXtOOS','V2NSFBdCfP','2022-09-18 14:38:37',NULL,'.h5ad',NULL);
-INSERT INTO dobject VALUES('uIHge4bsgwc0ndqcoC9Ii','1','iris','ZCdINSMzjawp','V2NSFBdCfP','2022-09-18 14:38:37',NULL,'.csv',NULL);
 CREATE TABLE IF NOT EXISTS "pipeline" (
 	id VARCHAR NOT NULL, 
 	created_at DATETIME DEFAULT (CURRENT_TIMESTAMP) NOT NULL, 
 	updated_at DATETIME, 
 	v VARCHAR NOT NULL, 
 	name VARCHAR, 
 	reference VARCHAR, 
@@ -109,28 +71,53 @@
 	name VARCHAR NOT NULL, 
 	user_id VARCHAR NOT NULL, 
 	PRIMARY KEY (id, v), 
 	FOREIGN KEY(user_id) REFERENCES user (id)
 );
 INSERT INTO jupynb VALUES('GgD4VJbXtOOS','2022-09-18 14:38:37',NULL,'1','Get started','9ypQ1yrW');
 INSERT INTO jupynb VALUES('ZCdINSMzjawp','2022-09-18 14:38:37',NULL,'1','Add another user','tSJNTgoM');
+CREATE TABLE IF NOT EXISTS "dobject" (
+	id VARCHAR NOT NULL, 
+	name VARCHAR, 
+	dtransform_id VARCHAR NOT NULL, 
+	storage_id VARCHAR NOT NULL, 
+	created_at DATETIME DEFAULT (CURRENT_TIMESTAMP) NOT NULL, 
+	updated_at DATETIME, 
+	suffix VARCHAR, 
+	size FLOAT, 
+	PRIMARY KEY (id), 
+	CONSTRAINT fk_object_storage_id_storage FOREIGN KEY(storage_id) REFERENCES storage (id), 
+	FOREIGN KEY(dtransform_id) REFERENCES dtransform (id)
+);
+INSERT INTO dobject VALUES('4SYxweB1zI1PjgyiYmhHP','scanpy_pbmc68k_reduced','GgD4VJbXtOOS','V2NSFBdCfP','2022-09-18 14:38:37',NULL,'.h5ad',NULL);
+INSERT INTO dobject VALUES('Jxpe4xf0j5guH3wZgAZEz','scanpy_pbmc68k_reduced','GgD4VJbXtOOS','V2NSFBdCfP','2022-09-18 14:38:37',NULL,'.h5ad',NULL);
+INSERT INTO dobject VALUES('uIHge4bsgwc0ndqcoC9Ii','iris','ZCdINSMzjawp','V2NSFBdCfP','2022-09-18 14:38:37',NULL,'.csv',NULL);
+CREATE TABLE IF NOT EXISTS "dtransform_in" (
+	dtransform_id VARCHAR NOT NULL, 
+	dobject_id VARCHAR NOT NULL, 
+	PRIMARY KEY (dtransform_id, dobject_id), 
+	CONSTRAINT fk_dobject_id FOREIGN KEY(dobject_id) REFERENCES dobject (id), 
+	FOREIGN KEY(dtransform_id) REFERENCES dtransform (id)
+);
+CREATE TABLE IF NOT EXISTS "usage" (
+	id VARCHAR NOT NULL, 
+	type VARCHAR NOT NULL, 
+	user_id VARCHAR NOT NULL, 
+	time DATETIME NOT NULL, 
+	dobject_id VARCHAR NOT NULL, 
+	PRIMARY KEY (id), 
+	CONSTRAINT fk_dobject_id FOREIGN KEY(dobject_id) REFERENCES dobject (id), 
+	FOREIGN KEY(user_id) REFERENCES user (id)
+);
+INSERT INTO usage VALUES('WO3RxPpY8mS5xgcQsHMlLYKn','ingest','9ypQ1yrW','2022-07-21 18:06:08.000000','4SYxweB1zI1PjgyiYmhHP');
+INSERT INTO usage VALUES('muL0I4sGi6hlyQr6NISXI7q5','ingest','9ypQ1yrW','2022-07-21 18:07:54.000000','Jxpe4xf0j5guH3wZgAZEz');
+INSERT INTO usage VALUES('uj4rF6GCgLIsZho5LlT70s1j','ingest','tSJNTgoM','2022-07-21 18:08:15.000000','uIHge4bsgwc0ndqcoC9Ii');
 CREATE INDEX ix_dtransform_pipeline_run_id ON dtransform (pipeline_run_id);
 CREATE INDEX ix_dtransform_jupynb_id ON dtransform (jupynb_id);
 CREATE INDEX ix_dtransform_jupynb_v ON dtransform (jupynb_v);
-CREATE INDEX ix_usage_dobject_id ON usage (dobject_id);
-CREATE INDEX ix_usage_user_id ON usage (user_id);
-CREATE INDEX ix_usage_time ON usage (time);
-CREATE INDEX ix_usage_dobject_v ON usage (dobject_v);
-CREATE INDEX ix_usage_type ON usage (type);
-CREATE INDEX ix_dobject_suffix ON dobject (suffix);
-CREATE INDEX ix_dobject_name ON dobject (name);
-CREATE INDEX ix_dobject_storage_id ON dobject (storage_id);
-CREATE INDEX ix_dobject_created_at ON dobject (created_at);
-CREATE INDEX ix_dobject_dtransform_id ON dobject (dtransform_id);
-CREATE INDEX ix_dobject_updated_at ON dobject (updated_at);
 CREATE INDEX ix_pipeline_reference ON pipeline (reference);
 CREATE INDEX ix_pipeline_updated_at ON pipeline (updated_at);
 CREATE INDEX ix_pipeline_name ON pipeline (name);
 CREATE INDEX ix_pipeline_created_at ON pipeline (created_at);
 CREATE INDEX ix_pipeline_run_created_at ON pipeline_run (created_at);
 CREATE INDEX ix_pipeline_run_pipeline_id ON pipeline_run (pipeline_id);
 CREATE INDEX ix_pipeline_run_name ON pipeline_run (name);
@@ -139,13 +126,23 @@
 CREATE INDEX ix_storage_updated_at ON storage (updated_at);
 CREATE INDEX ix_storage_created_at ON storage (created_at);
 CREATE INDEX ix_user_updated_at ON user (updated_at);
 CREATE INDEX ix_user_created_at ON user (created_at);
 CREATE UNIQUE INDEX ix_user_email ON user (email);
 CREATE UNIQUE INDEX ix_user_handle ON user (handle);
 CREATE INDEX ix_version_yvzi_created_at ON version_yvzi (created_at);
-CREATE INDEX ix_dobject_size ON dobject (size);
 CREATE INDEX ix_jupynb_user_id ON jupynb (user_id);
 CREATE INDEX ix_jupynb_name ON jupynb (name);
 CREATE INDEX ix_jupynb_created_at ON jupynb (created_at);
 CREATE INDEX ix_jupynb_updated_at ON jupynb (updated_at);
+CREATE INDEX ix_dobject_created_at ON dobject (created_at);
+CREATE INDEX ix_dobject_suffix ON dobject (suffix);
+CREATE INDEX ix_dobject_updated_at ON dobject (updated_at);
+CREATE INDEX ix_dobject_size ON dobject (size);
+CREATE INDEX ix_dobject_name ON dobject (name);
+CREATE INDEX ix_dobject_storage_id ON dobject (storage_id);
+CREATE INDEX ix_dobject_dtransform_id ON dobject (dtransform_id);
+CREATE INDEX ix_usage_time ON usage (time);
+CREATE INDEX ix_usage_type ON usage (type);
+CREATE INDEX ix_usage_user_id ON usage (user_id);
+CREATE INDEX ix_usage_dobject_id ON usage (dobject_id);
 COMMIT;
```

### Comparing `lnschema_core-0.8.1/PKG-INFO` & `lnschema_core-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lnschema_core
-Version: 0.8.1
-Summary: Schema module core (`yvzi`).
+Version: 0.9.0
+Summary: Data provenance & flow (`yvzi`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: nbproject
 Requires-Dist: sqlmodel
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnschema-core
 Provides-Extra: dev
 Provides-Extra: test
 
 [![pypi](https://img.shields.io/pypi/v/lnschema_core?color=%2334D058&label=pypi%20package)](https://pypi.org/project/lnschema_core)
 
-# lnschema-core: Data provenance (`yvzi`)
+# lnschema-core: Data provenance & flow (`yvzi`)
 
 Read the [docs](https://lamin.ai/docs/lnschema-core).
```

