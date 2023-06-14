# Comparing `tmp/unfolded.data-sdk-0.9.1.tar.gz` & `tmp/unfolded.data-sdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfolded.data-sdk-0.9.1.tar", max compression
+gzip compressed data, was "unfolded.data-sdk-0.9.2.tar", max compression
```

## Comparing `unfolded.data-sdk-0.9.1.tar` & `unfolded.data-sdk-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      201 2022-05-06 02:34:45.352235 unfolded.data-sdk-0.9.1/README.md
--rw-r--r--   0        0        0     1269 2022-06-10 21:31:31.573254 unfolded.data-sdk-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       83 2022-06-10 21:31:31.574221 unfolded.data-sdk-0.9.1/unfolded/data_sdk/__init__.py
--rw-r--r--   0        0        0    12862 2022-05-06 02:34:45.353258 unfolded.data-sdk-0.9.1/unfolded/data_sdk/_query.py
--rw-r--r--   0        0        0    11435 2022-06-03 16:11:08.784398 unfolded.data-sdk-0.9.1/unfolded/data_sdk/cli.py
--rw-r--r--   0        0        0    41475 2022-06-10 21:31:31.574896 unfolded.data-sdk-0.9.1/unfolded/data_sdk/data_sdk.py
--rw-r--r--   0        0        0     1892 2022-05-06 02:34:45.353608 unfolded.data-sdk-0.9.1/unfolded/data_sdk/enums.py
--rw-r--r--   0        0        0      369 2022-05-06 02:34:45.353668 unfolded.data-sdk-0.9.1/unfolded/data_sdk/errors.py
--rw-r--r--   0        0        0     7439 2022-05-06 02:34:45.353760 unfolded.data-sdk-0.9.1/unfolded/data_sdk/models.py
--rw-r--r--   0        0        0        0 2022-05-06 02:34:45.353785 unfolded.data-sdk-0.9.1/unfolded/data_sdk/py.typed
--rw-r--r--   0        0        0     2066 2022-06-10 21:31:31.575413 unfolded.data-sdk-0.9.1/unfolded/data_sdk/utils.py
--rw-r--r--   0        0        0     1284 2022-06-10 21:31:43.966361 unfolded.data-sdk-0.9.1/setup.py
--rw-r--r--   0        0        0     1281 2022-06-10 21:31:43.966542 unfolded.data-sdk-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      201 2021-06-22 21:38:51.906788 unfolded.data-sdk-0.9.2/README.md
+-rw-r--r--   0        0        0     1269 2022-08-02 17:36:03.907671 unfolded.data-sdk-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       83 2022-08-02 17:36:03.910112 unfolded.data-sdk-0.9.2/unfolded/data_sdk/__init__.py
+-rw-r--r--   0        0        0    12862 2022-06-02 18:45:53.820934 unfolded.data-sdk-0.9.2/unfolded/data_sdk/_query.py
+-rw-r--r--   0        0        0    11371 2022-08-01 22:25:04.715584 unfolded.data-sdk-0.9.2/unfolded/data_sdk/cli.py
+-rw-r--r--   0        0        0    41852 2022-08-01 22:25:04.717202 unfolded.data-sdk-0.9.2/unfolded/data_sdk/data_sdk.py
+-rw-r--r--   0        0        0     1892 2022-06-02 18:45:53.823334 unfolded.data-sdk-0.9.2/unfolded/data_sdk/enums.py
+-rw-r--r--   0        0        0      369 2021-08-27 16:13:59.593929 unfolded.data-sdk-0.9.2/unfolded/data_sdk/errors.py
+-rw-r--r--   0        0        0     7439 2022-08-01 22:25:04.718606 unfolded.data-sdk-0.9.2/unfolded/data_sdk/models.py
+-rw-r--r--   0        0        0        0 2021-06-22 21:38:51.908606 unfolded.data-sdk-0.9.2/unfolded/data_sdk/py.typed
+-rw-r--r--   0        0        0     2066 2022-07-22 15:02:11.756415 unfolded.data-sdk-0.9.2/unfolded/data_sdk/utils.py
+-rw-r--r--   0        0        0     1284 2022-08-02 18:24:00.398170 unfolded.data-sdk-0.9.2/setup.py
+-rw-r--r--   0        0        0     1230 2022-08-02 18:24:00.398501 unfolded.data-sdk-0.9.2/PKG-INFO
```

### Comparing `unfolded.data-sdk-0.9.1/pyproject.toml` & `unfolded.data-sdk-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unfolded.data-sdk"
-version = "0.9.1"
+version = "0.9.2"
 description = "Module for working with Unfolded Studio's Data SDK"
 authors = ["Kyle Barron <kyle@unfolded.ai>"]
 license = "(c) 2022 Foursquare Labs, Inc. Terms available at https://www.unfolded.ai/terms-of-service/"
 readme = "README.md"
 packages = [
     { include = "unfolded/data_sdk" },
 ]
```

### Comparing `unfolded.data-sdk-0.9.1/unfolded/data_sdk/_query.py` & `unfolded.data-sdk-0.9.2/unfolded/data_sdk/_query.py`

 * *Files identical despite different names*

### Comparing `unfolded.data-sdk-0.9.1/unfolded/data_sdk/cli.py` & `unfolded.data-sdk-0.9.2/unfolded/data_sdk/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,16 @@
     data_sdk = DataSDK()
     data_sdk.delete_dataset(dataset=dataset_id)
     click.echo("Dataset deleted.", file=sys.stderr)
 
 
 @click.command()
 @click.argument("map_id", type=str)
-@click.argument("dataset-to-replace-id", type=str, help="ID of dataset to replace.")
-@click.argument("dataset-to-use-id", type=str, help="ID of dataset to use.")
+@click.argument("dataset-to-replace-id", type=str)
+@click.argument("dataset-to-use-id", type=str)
 @click.option(
     "--force",
     is_flag=True,
     callback=abort_if_false,
     expose_value=False,
     help="Force replace dataset (even if not compatible)",
 )
```

### Comparing `unfolded.data-sdk-0.9.1/unfolded/data_sdk/data_sdk.py` & `unfolded.data-sdk-0.9.2/unfolded/data_sdk/data_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -730,14 +730,16 @@
 
         Args:
             map: the map record to update with the new field.
 
         Returns:
             The updated map record.
         """
+        if isinstance(map_id, Map):
+            map_id = map_id.id
 
         if not map_id:
             raise DataSDKError("Map id is required to perform the update")
 
         dataset_ids = None
         if datasets:
             dataset_ids = [
@@ -787,23 +789,23 @@
         r = requests.get(url, headers=self._headers)
         raise_for_status(r)
 
         return HexTileMetadata(**r.json())
 
     def enrich(
         self,
-        dataset: Union[pd.DataFrame, Dataset, UUID, str],
+        dataset: Union["pd.DataFrame", Dataset, UUID, str],
         source_id: UUID,
         source_column: Union[str, List[str]],
         *,
         h3_column: Optional[str] = None,
         lat_column: Optional[str] = None,
         lng_column: Optional[str] = None,
         time_column: Optional[str] = None,
-    ) -> pd.DataFrame:
+    ) -> "pd.DataFrame":
         """Enriches a dataset with a given enrichment source
 
         Enriches a dataset with a given enrichment source and column based on either a h3_column
         or a combination of lat_column and lng_column
 
         Args:
             dataset: the dataset to enrich, could be in one of the following shapes:
@@ -816,14 +818,16 @@
             lat_column: the dataset latitude column to use for enrichment (enrichment by lat/lng).
             lng_column: the dataset longitude column to use for enrichment (enrichment by lat/lng).
             time_column: the dataset time column to use for temporal enrichment.
 
         Returns:
             A pandas data frame with the resulting enriched dataset.
         """
+        if pd is None:
+            raise ImportError("Pandas required to use the enrich method.")
 
         if h3_column:
             index_columns = [h3_column]
         elif lat_column and lng_column:
             index_columns = [lat_column, lng_column]
         else:
             raise DataSDKError(
@@ -877,15 +881,15 @@
         geojson: Dict,
         *,
         source_column: Optional[Union[str, List[str]]] = None,
         res: Optional[int] = None,
         h3_column: Optional[str] = None,
         time_column: Optional[str] = None,
         time_interval: Optional[Union[Dict, TimeInterval]] = None,
-    ) -> pd.DataFrame:
+    ) -> "pd.DataFrame":
         """Extract data from a HexTile dataset
 
         Args:
             source_id: the uuid of the EnrichmentDataset to enrich with.
             geojson: the GeoJSON geometry of the area to extract
 
         Kwargs:
@@ -894,14 +898,17 @@
             h3_column: name of column for h3 index
             time_column: name of column for time index
             time_interval: time interval of data to extract
 
         Returns:
             A pandas data frame with the extracted dataset.
         """
+        if pd is None:
+            raise ImportError("Pandas required to use the tile_extract method.")
+
         # Build and run the enrichment query
         query = Query()
         query = query.tile_extract(
             source_id=source_id,
             geojson=geojson,
             source_column=source_column,
             res=res,
@@ -954,23 +961,26 @@
             data=config.json(exclude_none=True, by_alias=True),
             headers=headers,
         )
         raise_for_status(r)
 
         return Dataset(**r.json().get("item"))
 
-    def _query(self, query: Query) -> pd.DataFrame:
+    def _query(self, query: Query) -> "pd.DataFrame":
         """Runs a query using the Unfolded Query API
 
         Args:
             query: the Query describing the operations to run
 
         Returns:
             A pandas data frame with the result of the query.
         """
+        if pd is None:
+            raise ImportError("Pandas required to use the _query method.")
+
         url = f"{self.base_url}/v1/query"
         headers = {**self._headers, "Content-Type": "application/json"}
         r = requests.post(url, headers=headers, data=query.json())
         raise_for_status(r)
 
         with BytesIO(r.content) as buf:
             return pd.read_csv(buf)
```

### Comparing `unfolded.data-sdk-0.9.1/unfolded/data_sdk/enums.py` & `unfolded.data-sdk-0.9.2/unfolded/data_sdk/enums.py`

 * *Files identical despite different names*

### Comparing `unfolded.data-sdk-0.9.1/unfolded/data_sdk/models.py` & `unfolded.data-sdk-0.9.2/unfolded/data_sdk/models.py`

 * *Files identical despite different names*

### Comparing `unfolded.data-sdk-0.9.1/unfolded/data_sdk/utils.py` & `unfolded.data-sdk-0.9.2/unfolded/data_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `unfolded.data-sdk-0.9.1/setup.py` & `unfolded.data-sdk-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'test': ['pandas>=1.0,<2.0', 'geopandas>=0.8.0,<0.9.0']}
 
 entry_points = \
 {'console_scripts': ['uf-data-sdk = unfolded.data_sdk.cli:main']}
 
 setup_kwargs = {
     'name': 'unfolded.data-sdk',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': "Module for working with Unfolded Studio's Data SDK",
     'long_description': "# `unfolded.data-sdk`\n\nPython package for interfacing with [Unfolded](https://unfolded.ai)'s Data SDK.\n\nFor more documentation, refer to the [documentation website](https://docs.unfolded.ai/data-sdk).\n",
     'author': 'Kyle Barron',
     'author_email': 'kyle@unfolded.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `unfolded.data-sdk-0.9.1/PKG-INFO` & `unfolded.data-sdk-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: unfolded.data-sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Module for working with Unfolded Studio's Data SDK
 License: (c) 2022 Foursquare Labs, Inc. Terms available at https://www.unfolded.ai/terms-of-service/
 Author: Kyle Barron
 Author-email: kyle@unfolded.ai
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dataframe
 Provides-Extra: test
 Requires-Dist: PyJWT (>=2.0.0,<3.0.0)
 Requires-Dist: click (>=7.0,<9.0)
```

