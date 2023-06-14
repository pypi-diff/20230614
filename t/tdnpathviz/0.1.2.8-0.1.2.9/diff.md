# Comparing `tmp/tdnpathviz-0.1.2.8-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 381451 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 12:54 tdnpathviz/__init__.py
+Zip file size: 381465 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 13:23 tdnpathviz/__init__.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat    24197 b- defN 23-Jun-07 12:52 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat    24528 b- defN 23-Jun-07 13:20 tdnpathviz/visualizations.py
 -rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      724 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/RECORD
-9 files, 2205878 bytes uncompressed, 380201 bytes compressed:  82.8%
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-07 13:23 tdnpathviz-0.1.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 13:23 tdnpathviz-0.1.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-07 13:23 tdnpathviz-0.1.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      724 b- defN 23-Jun-07 13:23 tdnpathviz-0.1.2.9.dist-info/RECORD
+9 files, 2206209 bytes uncompressed, 380215 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.8.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.8.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.8.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.8.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2.8'
+__version__ = '0.1.2.9'
```

## tdnpathviz/visualizations.py

```diff
@@ -65,15 +65,15 @@
         - width (int, optional): define the width of the figure. Defaults is 1200.
         - height (int, optional): define the height of the figure. Defaults is 800.
         - weight_column (str, optional): define the column to aggregate. If None, just count the number of pathes.
           Default is None.
         - weight_agg (str, optional): when weight_column is not None, then the weight is the result of the aggregation
           defined by weight_agg on the weight_column. Permitted values are 'count', 'avg', 'max', 'min', 'sum'.
           Default is 'count'.
-        - justify (str, optional): define if you want to justify 'right' or 'left' the output sankey. Defaults is 'left'.
+        - justify (str, optional): define if you want to justify 'right' or 'left' or 'both' the output sankey. Defaults is 'left'.
 
         Returns:
         - None (it display an interactive Sankey plot)
     """
     if type(id_column) != list:
         id_column = [id_column]
 
@@ -109,31 +109,33 @@
         QUALIFY id < {nb_paths}+1"""
 
     df_selection = tdml.DataFrame.from_query(query)
 
     if justify == 'left':
         justify_query = 'AAA.id_end_temp AS id_end'
         ascending     = ''
+        init          = '0'
     elif justify == 'right':
         justify_query = '''AAA.id_end_temp as id_end'''
         ascending     = ' DESC'
+        init          = 'max_path_length'
 
     query2 = f"""
     sel
         CC.id
     ,   CC.node_source
     ,	CC.node_target
     ,	CC.beg
     ,	CC."end"
     ,	sum(CC.weight) as weight
     FROM 
     (
     sel
         B.*
-    ,	LAG(id_end,1,0) OVER (PARTITION BY B."path" ORDER BY B."index") as id_beg
+    ,	LAG(id_end,1,{init}) OVER (PARTITION BY B."path" ORDER BY B."index") as id_beg
     ,	B."beg" || '_' || TRIM(CAST(id_beg AS VARCHAR(200))) as node_source
     ,	B."end" || '_' || TRIM(CAST(id_end AS VARCHAR(200))) as node_target
     FROM 
     (
         SEL
             AAA.*
         ,   {justify_query}
@@ -220,15 +222,15 @@
 
         Parameters:
         - myPathAnalysis (DataFrame or tdml.dataframe.dataframe.DataFrame): The input DataFrame containing path analysis data.
         - root_name (str, optional): The root name to be used for naming the created views. Defaults to 'mytest'.
         - schema (str, optional): The schema to create the views in. Defaults to the current database schema.
         - path_column (str, optional): The column name representing the path. Defaults to 'mypath'.
         - id_column (str or list, optional): The column name(s) representing the unique identifier(s). Defaults to 'travelid'.
-        - justify (str, optional): define if you want to justify 'right' or 'left' the output sankey. Defaults is 'left'.
+        - justify (str, optional): define if you want to justify 'right' or 'left' or 'both' the output sankey. Defaults is 'left'.
 
         Returns:
         - None
     """
 
     if type(id_column) != list:
         id_column = [id_column]
@@ -273,17 +275,24 @@
     ,	count_{id_column[0]} as weight
     FROM {aggregated_npath_view} A"""
     tdml.get_context().execute(query)
     print(f'clean aggregated npath view created : {clean_aggregated_npath_view}')
 
     if justify == 'left':
         justify_query = 'AAA.id_end_temp AS id_end'
+        ascending     = ''
+        init          = '0'
     elif justify == 'right':
-        justify_query = '''AAA.id_end_temp + max_max_path_length - max_path_length as id_end'''
-
+        justify_query = '''AAA.id_end_temp as id_end'''
+        ascending     = ' DESC'
+        init          = 'max_path_length'
+    elif justify == 'both':
+        justify_query = '''AAA.id_end_temp as id_end'''
+        ascending = ' DESC'
+        init = '0'
 
     # Create the graph view of the aggregated npath view
     graph_aggregated_npath_view =  f"{schema}.{root_name}_GRAPH_NPATH_VIEW_AGG"
     query = f"""
     REPLACE VIEW {graph_aggregated_npath_view} AS
     SELECT
         CC.id
@@ -292,28 +301,28 @@
     ,	CC.beg
     ,	CC."end"
     ,	sum(CC.weight) as weight
     FROM 
     (
     sel
         B.*
-    ,	LAG(id_end,1,0) OVER (PARTITION BY B."path" ORDER BY B."path",B."index") as id_beg
+    ,	LAG(id_end,1,{init}) OVER (PARTITION BY B."path" ORDER BY B."path",B."index") as id_beg
     ,	B."beg" || '_' || TRIM(CAST(id_beg AS VARCHAR(10))) as node_source
     ,	B."end" || '_' || TRIM(CAST(id_end AS VARCHAR(10))) as node_target
     FROM 
         (
         SEL
             AAA.*
         ,   {justify_query}
         ,   MAX(AAA.id_end_temp) OVER (PARTITION BY AAA."path") AS max_path_length
         ,   MAX(AAA.id_end_temp) OVER (PARTITION BY 1) AS max_max_path_length
         FROM (
             sel 
                 A.*
-            ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."path",A."index") as id_end_temp
+            ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."index" {ascending}) as id_end_temp
             from (
                 SELECT
         
                     lag(AA.token,1) IGNORE NULLS OVER (PARTITION BY AA.outkey ORDER BY AA.tokennum) as "beg"
                 ,	AA.token as "end"
                 ,	AA.outkey as "path"
                 ,	B.weight
```

