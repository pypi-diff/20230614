# Comparing `tmp/dfschema-0.0.7.tar.gz` & `tmp/dfschema-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfschema-0.0.7.tar", max compression
+gzip compressed data, was "dfschema-0.0.8.tar", max compression
```

## Comparing `dfschema-0.0.7.tar` & `dfschema-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1109 2023-03-14 21:42:20.025769 dfschema-0.0.7/LICENSE
--rw-r--r--   0        0        0     3067 2023-03-14 21:42:20.025769 dfschema-0.0.7/README.md
--rw-r--r--   0        0        0      416 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/__init__.py
--rw-r--r--   0        0        0     2711 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/cli.py
--rw-r--r--   0        0        0       52 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/__init__.py
--rw-r--r--   0        0        0      786 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/collector.py
--rw-r--r--   0        0        0    12514 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/column.py
--rw-r--r--   0        0        0    15104 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/core.py
--rw-r--r--   0        0        0      999 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/dtype.py
--rw-r--r--   0        0        0      525 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/exceptions.py
--rw-r--r--   0        0        0     1704 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/generate.py
--rw-r--r--   0        0        0      369 2023-03-14 21:42:20.025769 dfschema-0.0.7/dfschema/core/legacy/__init__.py
--rw-r--r--   0        0        0     4185 2023-03-14 21:42:20.029769 dfschema-0.0.7/dfschema/core/legacy/v1.py
--rw-r--r--   0        0        0       94 2023-03-14 21:42:20.029769 dfschema-0.0.7/dfschema/core/logger.py
--rw-r--r--   0        0        0     1684 2023-03-14 21:42:20.029769 dfschema-0.0.7/dfschema/core/misc.py
--rw-r--r--   0        0        0     1791 2023-03-14 21:42:20.029769 dfschema-0.0.7/dfschema/core/shape.py
--rw-r--r--   0        0        0     3315 2023-03-14 21:42:20.029769 dfschema-0.0.7/dfschema/utils.py
--rw-r--r--   0        0        0     1139 2023-03-14 21:42:20.029769 dfschema-0.0.7/dfschema/validate.py
--rw-r--r--   0        0        0     1118 2023-03-14 21:42:33.722053 dfschema-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 dfschema-0.0.7/setup.py
--rw-r--r--   0        0        0     3936 1970-01-01 00:00:00.000000 dfschema-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-03-15 14:58:57.969417 dfschema-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3067 2023-03-15 14:58:57.969417 dfschema-0.0.8/README.md
+-rw-r--r--   0        0        0      416 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/__init__.py
+-rw-r--r--   0        0        0     2710 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/cli.py
+-rw-r--r--   0        0        0       52 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/__init__.py
+-rw-r--r--   0        0        0      786 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/collector.py
+-rw-r--r--   0        0        0    12514 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/column.py
+-rw-r--r--   0        0        0    15104 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/core.py
+-rw-r--r--   0        0        0      999 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/dtype.py
+-rw-r--r--   0        0        0      525 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/exceptions.py
+-rw-r--r--   0        0        0     1704 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/generate.py
+-rw-r--r--   0        0        0      369 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/legacy/__init__.py
+-rw-r--r--   0        0        0     4756 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/legacy/v1.py
+-rw-r--r--   0        0        0       94 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/logger.py
+-rw-r--r--   0        0        0     1684 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/misc.py
+-rw-r--r--   0        0        0     1791 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/core/shape.py
+-rw-r--r--   0        0        0     3315 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/utils.py
+-rw-r--r--   0        0        0     1139 2023-03-15 14:58:57.969417 dfschema-0.0.8/dfschema/validate.py
+-rw-r--r--   0        0        0     1118 2023-03-15 14:59:10.633606 dfschema-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 dfschema-0.0.8/setup.py
+-rw-r--r--   0        0        0     3936 1970-01-01 00:00:00.000000 dfschema-0.0.8/PKG-INFO
```

### Comparing `dfschema-0.0.7/LICENSE` & `dfschema-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/README.md` & `dfschema-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/cli.py` & `dfschema-0.0.8/dfschema/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     json = "json"
 
 
 app = typer.Typer()
 
 
 def _infer_read_df(path: Path, **kwargs) -> pd.DataFrame:
-
     methods = {
         ".csv": pd.read_csv,
         ".xlsx": pd.read_excel,
         ".parquet": pd.read_parquet,
         ".feather": pd.read_feather,
     }
```

### Comparing `dfschema-0.0.7/dfschema/core/collector.py` & `dfschema-0.0.8/dfschema/core/collector.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/core/column.py` & `dfschema-0.0.8/dfschema/core/column.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/core/core.py` & `dfschema-0.0.8/dfschema/core/core.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/core/dtype.py` & `dfschema-0.0.8/dfschema/core/dtype.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/core/exceptions.py` & `dfschema-0.0.8/dfschema/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/core/generate.py` & `dfschema-0.0.8/dfschema/core/generate.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/core/legacy/v1.py` & `dfschema-0.0.8/dfschema/core/legacy/v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,24 +22,25 @@
     max_rows: Optional[PositiveInt] = Field(None, description="maximum number of rows")
     min_rows: Optional[PositiveInt] = Field(None, description="minimum number of rows")
 
 
 class V1_ColObj(BaseModel):
     class Config:
         extra = Extra.forbid
+        allow_population_by_field_name = True
 
     dtype: Optional[DtypeLiteral]  # type: ignore
 
-    min_value: Optional[float]
-    max_value: Optional[float]
+    min_value: Optional[float] = Field(None, alias="min")
+    max_value: Optional[float] = Field(None, alias="max")
 
     na_limit: Union[None, bool, float] = Field(None, gt=0, le=1.0)
 
     include: Optional[List[str]] = None
-    oneof: Optional[List[str]] = None
+    oneof: Optional[List[str]] = Field(None, alias="one_of")
     unique: Optional[bool] = None
 
 
 class V1_ColumnsSchema(BaseModel):
     __root__: Dict[str, V1_ColObj]
 
     class Config:
@@ -74,19 +75,23 @@
     def migrate(self) -> Tuple[dict, float]:
         logger.info("Migrating schema v1 to v2")
         schema = self.dict(exclude_none=True)
 
         if "protocol_version" in schema:
             schema.pop("protocol_version")
 
-        schema["metadata"] = {"protocol_version": 2.0}
+        if "version" in schema:
+            version = schema.pop("version")
+        else:
+            version = None
+
+        schema["metadata"] = {"protocol_version": 2.0, "version": version}
         schema["additionalColumns"] = schema.pop("strict_cols", False)
 
         if "columns" in schema:
-
             if isinstance(schema["columns"], dict):
                 schema["columns"] = [
                     dict(name=k, **v) for k, v in schema["columns"].items()
                 ]
             elif isinstance(schema["columns"], list):
                 schema["columns"] = [dict(name=name) for name in schema["columns"]]
 
@@ -100,14 +105,23 @@
                 for vl in {"max_value", "min_value"}:
                     if vl in col:
                         value_limits = col.get("value_limits", {})
                         value_limits[vl[:3]] = col.pop(vl)
                         col["value_limits"] = value_limits
 
                 # categorical
+                if (
+                    ("oneof" in col)
+                    and ("include" in col)
+                    and col.get("oneof") == col.get("include")
+                ):
+                    set_ = col.pop("oneof")
+                    col.pop("include")
+                    col["exact_set"] = set_
+
                 for k in ("oneof", "include", "exact_set"):
                     if col.get(k) is not None:
                         categorical = col.get("categorical", dict())
                         try:
                             categorical["value_set"] = set(col.pop(k, {}))
                         except TypeError as e:
                             raise TypeError(k, col, e)
```

### Comparing `dfschema-0.0.7/dfschema/core/misc.py` & `dfschema-0.0.8/dfschema/core/misc.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/core/shape.py` & `dfschema-0.0.8/dfschema/core/shape.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/utils.py` & `dfschema-0.0.8/dfschema/utils.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/dfschema/validate.py` & `dfschema-0.0.8/dfschema/validate.py`

 * *Files identical despite different names*

### Comparing `dfschema-0.0.7/pyproject.toml` & `dfschema-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfschema"
-version = "v0.0.7"
+version = "v0.0.8"
 description = "lightweight pandas.DataFrame schema"
 authors = ["Philipp <philippk@zillowgroup.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 dfschema = "dfschema.cli:app"
```

### Comparing `dfschema-0.0.7/setup.py` & `dfschema-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'yaml': ['PyYAML>=6.0,<7.0']}
 
 entry_points = \
 {'console_scripts': ['dfschema = dfschema.cli:app']}
 
 setup_kwargs = {
     'name': 'dfschema',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'lightweight pandas.DataFrame schema',
     'long_description': '# DFS (aka Dataframe_Schema)\n\n**DFS** is a lightweight validator for `pandas.DataFrame`. You can think of it as a `jsonschema` for dataframe. \n\nKey features:\n1. **Lightweight**: only dependent on `pandas`  and `pydantic` (which depends only on `typing_extensions`)\n2. **Explicit**: inspired by `JsonSchema`, all schemas are stored as json (or yaml) files and can be generated or changed on the fly.\n3. **Simple**: Easy to use, no need to change your workflow and dive into the implementation details. \n4. **Comprehensive**: Summarizes all errors in a single summary exception, checks for distributions, works on subsets of the dataframe \n5. **Rapid**: base schemas can be generated from given dataframe or sql query (using `pd.read_sql`).\n6. **Handy**: Supports command line interface (with `[cli]` extra).\n7. **Extendable**: Core idea is to validate *dataframes* of any type. While now supports only pandas, we\'ll add abstractions to run same checks on different types of dataframes (CuDF, Dask, SparkDF, etc )\n\n## QuickStart\n\n### 1. Validate DataFrame\n\nVia wrapper\n```python\nimport pandas as pd\nimport dfschema as dfs\n\n\ndf = pd.DataFrame({\n  "a": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n  "b": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n})\n\nschema_pass = {\n  "shape": {"min_rows": 10}\n}\n\nschema_raise = {\n  "shape": {"min_rows": 20}\n}\n\n\ndfs.validate(df, schema_pass)  # won\'t raise any issues\ndfs.validate(df, schema_raise) # will Raise DataFrameSchemaError\n```\nAlternatively (v2 optional), you can use the root class, `DfSchema`:\n```python\ndfs.DfSchema.from_dict(schema_pass).validate(df)  # won\'t raise any issues\ndfs.DfSchema.from_dict(schema_raise).validate(df)  # will Raise DataFrameSchemaError\n```\n\n### 2. Generate Schema\n\n```python\ndfs.DfSchema.from_df(df)\n```\n### 3. Read and Write Schemas\n  \n```python\nschema = dfs.DfSchema.from_file(\'schema.json\')\nschema.to_file("schema.yml")\n```\n\n### 4. Using CLI\n> Note: requires [cli] extra as relies on `Typer` and `click`\n\n#### Validate via CLI\n```shell\ndfschema validate --read_kwargs_json \'{delimiter="|"}\' FILEPATH SCHEMA_FILEPATH\n```\nSupports\n- csv\n- xlsx\n- parquet\n- feather\n\n#### Generate via CLI\n```shell\ndfs generate --format \'yaml\' DATA_PATH > schema.yaml\n```\n\n## Installation\n\nWIP\n\n## Alternatives\n- [TableScheme](https://pypi.org/project/tableschema/)\n- [GreatExpectations](https://greatexpectations.io/). Large and complex package with Html reports, Airflow Operator, connectors, etc. an work on out-of-memory data, SQL databases, parquet, etc\n- [Pandera](https://pandera.readthedocs.io/en/stable/) - awesome package, great and suitable for type hinting, compatible with `hypothesis`\n  - [great talk](https://www.youtube.com/watch?v=PI5UmKi14cM)\n- [Tensorflow validate](https://www.tensorflow.org/tfx/guide/tfdv)\n- [DTF expectations](https://github.com/calogica/dbt-expectations)\n\n## Changes\n- [[changelog]]\n\n## Roadmap\n- [ ] Add tutorial Notebook\n- [ ] Support tableschema\n- [ ] Support Modin models\n- [ ] Support SQLAlchemy ORM models\n- [ ] Built-in Airflow Operator?\n- [ ] Interactive CLI/jupyter for schema generation',
     'author': 'Philipp',
     'author_email': 'philippk@zillowgroup.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dfschema-0.0.7/PKG-INFO` & `dfschema-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfschema
-Version: 0.0.7
+Version: 0.0.8
 Summary: lightweight pandas.DataFrame schema
 Author: Philipp
 Author-email: philippk@zillowgroup.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

