# Comparing `tmp/openai_dbd-0.0.8-py3-none-any.whl.zip` & `tmp/openai_dbd-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3799 bytes, number of entries: 6
--rw-rw-r--  2.0 unx      117 b- defN 23-Jun-13 11:10 openai_dbd/__init__.py
--rw-rw-r--  2.0 unx     7486 b- defN 23-Jun-13 12:00 openai_dbd/openai_dbd.py
--rw-rw-r--  2.0 unx      302 b- defN 23-Jun-13 12:04 openai_dbd-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 12:04 openai_dbd-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-13 12:04 openai_dbd-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      468 b- defN 23-Jun-13 12:04 openai_dbd-0.0.8.dist-info/RECORD
-6 files, 8476 bytes uncompressed, 2949 bytes compressed:  65.2%
+Zip file size: 3785 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx      117 b- defN 23-Jun-14 06:34 openai_dbd/__init__.py
+-rw-rw-r--  2.0 unx     7239 b- defN 23-Jun-14 06:38 openai_dbd/openai_dbd.py
+-rw-rw-r--  2.0 unx      302 b- defN 23-Jun-14 06:38 openai_dbd-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 06:38 openai_dbd-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-14 06:38 openai_dbd-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      468 b- defN 23-Jun-14 06:38 openai_dbd-0.0.9.dist-info/RECORD
+6 files, 8229 bytes uncompressed, 2935 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: openai_dbd/__init__.py
 Comment: 
 
 Filename: openai_dbd/openai_dbd.py
 Comment: 
 
-Filename: openai_dbd-0.0.8.dist-info/METADATA
+Filename: openai_dbd-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: openai_dbd-0.0.8.dist-info/WHEEL
+Filename: openai_dbd-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: openai_dbd-0.0.8.dist-info/top_level.txt
+Filename: openai_dbd-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_dbd-0.0.8.dist-info/RECORD
+Filename: openai_dbd-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_dbd/openai_dbd.py

```diff
@@ -65,30 +65,26 @@
     }]
     """
 
     return callOpenAI(open_ai_data['url'], open_ai_data['headers'], promptX)
 
 def correct_schema(sql_schema, open_ai_data):
     promptX = f"""
-    I want you to act as SQL parser. 
-    I will give you instructions and you will only reply me with SQl query.
+    I want you to act as SQL Parser, I will give you SQL  query and you will only reply me with the SQL Query.
 
-    I have an existing database schema that I want you to review.
-    I would like you to correct any issues with the schema and redesign whole schema including create statments. 
-    Additionally, if the schema is not normalized, please normalize it.
-    Also, modify the current schema if it has performance issues.
-    Also, don't add any sql comments in result.
-    Also, if tables dosn't have created_at and updated_at columns, add it.
-    Please keep in mind every table i provide you in schema should be there and modified if required, 
-    Place all root tables at the top, as other tables depend on them
-    Here is my current schema.
-    `{sql_schema}`
+    I want you to review my existing database schema and update if required any changes in it.
+    Additionally, i want you to normalize database tables if required.
+    Also modify schemas if you find it has any performance related issues.
+    Also don't add any database comments.
+
+    What ever schema i am providing you are required to build my project so please reply with all tables including in it.
 
-    I want you to only reply the sql queries and nothing else, 
-    do not write explanations and any starting and ending sentences follow my instructions strictly.
+    Reply only in SQL Query, no explanation or any other text  at the beginning of your response and ending are not required.
+    Here is my existing Schema  
+    `{sql_schema}`
     """
 
     return callOpenAI(open_ai_data['url'], open_ai_data['headers'], promptX)
 
 def generate_sql(db_name, data):
     fName = giveRandName(10)
     with open(f"{fName}.sql", 'w') as file:
```

