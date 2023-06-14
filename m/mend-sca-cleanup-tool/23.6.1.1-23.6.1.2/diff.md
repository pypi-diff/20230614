# Comparing `tmp/mend_sca_cleanup_tool-23.6.1.1-py3-none-any.whl.zip` & `tmp/mend_sca_cleanup_tool-23.6.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14546 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    20958 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool/sca_cleanup_tool.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     9116 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      859 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD
-9 files, 42593 bytes uncompressed, 13024 bytes compressed:  69.4%
+Zip file size: 14524 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    20930 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9107 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD
+9 files, 42556 bytes uncompressed, 13002 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
 Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE
+Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA
+Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/WHEEL
+Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/entry_points.txt
+Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/top_level.txt
+Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD
+Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_sca_cleanup_tool/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.6.1.1"
+__version__ = "23.6.1.2"
 __tool_name__ = "sca_cleanup_tool"
 __description__ = "Mend SCA Cleanup Tool"
```

## mend_sca_cleanup_tool/sca_cleanup_tool.py

```diff
@@ -388,12 +388,12 @@
     CONFIG.included_product_tokens = CONFIG.included_product_tokens.replace(" ", "").split(",") if CONFIG.included_product_tokens else []
     CONFIG.excluded_product_tokens = CONFIG.excluded_product_tokens.replace(" ", "").split(",") if CONFIG.excluded_product_tokens else []
     CONFIG.excluded_project_tokens = CONFIG.excluded_project_tokens.replace(" ", "").split(",") if CONFIG.excluded_project_tokens else []
     CONFIG.excluded_project_name_patterns = CONFIG.excluded_project_name_patterns.split(",") if CONFIG.excluded_project_name_patterns else []
     CONFIG.report_types = CONFIG.report_types if CONFIG.report_types else []
 
     if CONFIG.excluded_project_name_patterns:
-        CONFIG.project_name_exclude_list = CONFIG.excluded_project_name_patterns.replace(" ", "").split(',')
+        CONFIG.project_name_exclude_list = CONFIG.excluded_project_name_patterns
    
 
 if __name__ == "__main__":
     main()
```

## Comparing `mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE` & `mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA` & `mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mend-sca-cleanup-tool
-Version: 23.6.1.1
+Version: 23.6.1.2
 Summary: Mend SCA Cleanup Tool
-Home-page: https://github.com/JRMendDemo/mend-sca-cleanup-tool
-Author: WhiteSource Professional Services
+Home-page: https://github.com/whitesource-ps/mend-sca-cleanup-tool
+Author: Mend Professional Services
 Author-email: ps@whitesourcesoftware.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
@@ -77,16 +77,16 @@
 ---
 
 Analyze only the projects that have the specified Mend tag and keep the newest project in each product:  
 `mend_sca_cleanup_tool -r 1 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<VALUE>`
 
 ---
 
-Keep the last 2 weeks and analyze only the projects whose match their tag key and the tag value contains the specified regex:  
-`mend_sca_cleanup_tool -r 14 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<REGEX_VALUE>`
+Keep the last 2 weeks and analyze only the projects whose match their tag key and the tag value contains the specified value:  
+`mend_sca_cleanup_tool -r 14 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -v <KEY>:<VALUE>`
 
 ---
 
 Keep the last 100 days for both PRODUCT_1 and PRODUCT_2, but do not delete the project PROJECT_1 (which is a project in one of the included products):  
 `mend_sca_cleanup_tool -r 100 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -x <PROJECT_TOKEN_1>`
 
 ---
@@ -122,15 +122,15 @@
                     List of excluded products
   -i INCLUDED_PRODUCT_TOKENS, --includedProductTokens
                     List of included products
   -g ANALYZED_PROJECT_TAG, --AnalyzedProjectTag
                     Analyze only the projects whose contain the specific Mend tag (key:value)
   -v ANALYZED_PROJECT_TAG_REGEX_IN_VALUE, --AnalyzedProjectTagRegexInValue
                     Analyze only the projects whose match their tag key and the tag value contains the specified value (key:value)
-                    Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convension is a misnomer but was kept to avoid breaking existing integrations.
+                    Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convention is a misnomer but was kept to avoid breaking existing integrations.
   -r DAYS_TO_KEEP, --DaysToKeep
                     Number of days to keep in FilterProjectsByUpdateTime or number of copies in FilterProjectsByLastCreatedCopies
   -p PROJECT_PARALLELISM_LEVEL, --ProjectParallelismLevel
                     Project parallelism level
                     Note: This is currently not used in this version of the mend-sca-cleanup-tool. Was kept to prevent breaking existing integrations.
   -y DRY_RUN, --DryRun
                     Logging the projects that are supposed to be deleted without deleting and creating reports
```

## Comparing `mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD` & `mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mend_sca_cleanup_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_sca_cleanup_tool/_version.py,sha256=0PxJlAFQcv_72t4q6XWUsiO_afOSZ-OpVl1fisDf2b0,102
-mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=jnqnJglRWkL__KJXJ3eeTyPjp-BGcTMTK2JKGy74_TY,20958
-mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA,sha256=l1x7VgVO2QRFd2G6HjERvnRKNXkqe9D5AeBRhblLvQQ,9116
-mend_sca_cleanup_tool-23.6.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_sca_cleanup_tool-23.6.1.1.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
-mend_sca_cleanup_tool-23.6.1.1.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
-mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD,,
+mend_sca_cleanup_tool/_version.py,sha256=lO6f6bjBTbV6kyBSXBMNyWNAqxcmEId4bg-H39-5Atw,102
+mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=mKMZ5vjti-vqBlz7FxKnvnxDii831N3dFC0PU4xGpQQ,20930
+mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA,sha256=XX4fm7b3-RbatlQe3awixwNzTKmqPfisj19wVsaafgI,9107
+mend_sca_cleanup_tool-23.6.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_sca_cleanup_tool-23.6.1.2.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
+mend_sca_cleanup_tool-23.6.1.2.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
+mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD,,
```

