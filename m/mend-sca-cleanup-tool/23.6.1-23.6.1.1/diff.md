# Comparing `tmp/mend_sca_cleanup_tool-23.6.1-py3-none-any.whl.zip` & `tmp/mend_sca_cleanup_tool-23.6.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14015 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    20717 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool/sca_cleanup_tool.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool-23.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     8197 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool-23.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool-23.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool-23.6.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool-23.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      847 b- defN 23-Jun-13 21:15 mend_sca_cleanup_tool-23.6.1.dist-info/RECORD
-9 files, 41419 bytes uncompressed, 12517 bytes compressed:  69.8%
+Zip file size: 14546 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    20958 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9116 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-13 22:11 mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD
+9 files, 42593 bytes uncompressed, 13024 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
 Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.dist-info/LICENSE
+Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.dist-info/METADATA
+Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.dist-info/WHEEL
+Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.dist-info/entry_points.txt
+Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.dist-info/top_level.txt
+Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.dist-info/RECORD
+Filename: mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_sca_cleanup_tool/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.6.1"
+__version__ = "23.6.1.1"
 __tool_name__ = "sca_cleanup_tool"
 __description__ = "Mend SCA Cleanup Tool"
```

## mend_sca_cleanup_tool/sca_cleanup_tool.py

```diff
@@ -287,30 +287,30 @@
                 projects_to_remove[product['productToken']] = filtered_projects
         else:
             print(f"No projects found for product: {product['productName']}")
     return projects_to_remove
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Mend SCA Clean up tool")
-    parser.add_argument('-a', '--mendURL', '--wsURL', help="Mend URL", dest='mend_url', required=True)
+    parser.add_argument('-a', '--mendURL', '--wsURL', help="Mend URL", dest='mend_url', default="saas.whitesourcesoftware.com")
     parser.add_argument('-e', '--excludedProductTokens', help="Excluded Product Tokens (comma seperated list)", dest='excluded_product_tokens')
     parser.add_argument('-g', '--analyzedProjectTag', help="Analyze only the projects whose contain the specific Mend tag (key:value)", dest='analyzed_project_tag')
     parser.add_argument('-i', '--includedProductTokens', help="Included Product Tokens (comma seperated list)", dest='included_product_tokens')
     parser.add_argument('-j', '--skipProjectDeletion', help="Skip Project Deletion", dest='skip_project_deletion', type=strtobool, default=False)
     parser.add_argument('-k', '--apiToken', '--orgToken', help="Mend API token", dest='mend_api_token', required=True)
     parser.add_argument('-m', '--operationMode', help="Clean up operation method", dest='operation_mode', default=FILTER_PROJECTS_BY_UPDATE_TIME,
                                 choices=[s for s in [FILTER_PROJECTS_BY_UPDATE_TIME, FILTER_PROJECTS_BY_LAST_CREATED_COPIES]])
     parser.add_argument('-n', '--excludedProjectNamePatterns', help="List of excluded project name patterns (comma seperated list)", dest='excluded_project_name_patterns')
     parser.add_argument('-o', '--outputDir', help="Output directory", dest='output_dir', default=os.getcwd() + "\\Mend\\Reports\\")
     parser.add_argument('-p', '--projectParallelismLevel', help="Project parallelism level directory Note: This is currently not used in this version of the mend-sca-cleanup-tool", dest='project_parallelism_level')
-    parser.add_argument('-r', '--daysToKeep', help="Number of days to keep (overridden by --dateToKeep)", dest='days_to_keep', type=int, default=21)
+    parser.add_argument('-r', '--daysToKeep', help="Number of days to keep (overridden by --dateToKeep)", dest='days_to_keep', type=int, default=50000)
     parser.add_argument('-s', '--skipReportGeneration', help="Skip Report Generation", dest='skip_report_generation', type=strtobool, default=False)
     parser.add_argument('-t', '--reportTypes', help="Report Types to generate (comma seperated list)", dest='report_types')
     parser.add_argument('-u', '--userKey', help="Mend UserKey", dest='mend_user_key', required=True)
-    parser.add_argument('-v', '--analyzedProjectTagRegexInValue', help="Analyze only the projects whose match their tag key and the tag value contains the specified regex (key:regexValue)", dest='analyzed_project_tag_regex_in_value')
+    parser.add_argument('-v', '--analyzedProjectTagRegexInValue', help="Analyze only the projects whose match their tag key and the tag value contains the specified regex (key:value) Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convention is a misnomer but was kept to avoid breaking existing integrations.", dest='analyzed_project_tag_regex_in_value')
     parser.add_argument('-x', '--excludedProjectTokens', help="Excluded Project Tokens (comma seperated list)", dest='excluded_project_tokens')
     parser.add_argument('-y', '--dryRun', help="Whether to run the tool without performing anything", dest='dry_run', type=strtobool, default=False)
     return parser.parse_args()
 
 def parse_config_file(filepath):
     if os.path.exists(filepath):
         config = ConfigParser()
```

## Comparing `mend_sca_cleanup_tool-23.6.1.dist-info/LICENSE` & `mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_sca_cleanup_tool-23.6.1.dist-info/METADATA` & `mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-sca-cleanup-tool
-Version: 23.6.1
+Version: 23.6.1.1
 Summary: Mend SCA Cleanup Tool
 Home-page: https://github.com/JRMendDemo/mend-sca-cleanup-tool
 Author: WhiteSource Professional Services
 Author-email: ps@whitesourcesoftware.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -25,14 +25,15 @@
 [![PyPI](https://img.shields.io/pypi/v/ws-cleanup-tool?style=plastic)](https://pypi.org/project/ws-cleanup-tool/)
 
 # Mend Projects Cleanup CLI Tool
 * The self-hosted CLI tool features cleaning up projects and generating reports before deletion in 2 modes:
   * By stating _OperationMode=FilterProjectsByUpdateTime_ and how many days to keep (-r/ DaysToKeep=)
   * By stating _OperationMode=FilterProjectsByLastCreatedCopies_ and how many copies to keep (-r/ DaysToKeep=)
 * The reports are saved in the designated location as follows: _[Output_DIR]/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_  
+  * The default location is the _[WORKING DIRECTORY]/Mend/Reports/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_
 * To review the outcome before actual deletion use _-y true_ / _DryRun=True_ flag. It will _NOT_ delete any project nor create reports 
 * By default, the tool generates all possible project-level reports. By specifying ((_-t_ / _Reports=_/) it is possible to select specific reports
   * The full list of available reports is below
 * The full parameters list is available below
 * There are two ways to configure the tool:
   * By configuring _params.config_ on the executed dir or passing a path to the file in the same format
   * By setting command line parameters as specified in the usage below
@@ -47,55 +48,55 @@
 ## Permissions
 * The user used to execute the tool has to have "Organization Administrator" or "Product Administrator" on all the maintained products and "Organization Auditor" permissions. 
 * It is recommended to use a service user.
 
 ## Installation and Execution from PyPi (recommended):
 1. Install by executing: `pip install mend-sca-cleanup-tool`
 2. Configure the appropriate parameters either by using the command line or in `params.config`.
-3. Execute the tool (`mend-sca_cleanup_tool ...`). 
+3. Execute the tool (`mend_sca_cleanup_tool ...`). 
 
 ## Installation and Execution from GitHub:
-1. Download and unzip **ws-cleanup-tool.zip** 
+1. Download and unzip **mend-sca-cleanup-tool.zip** from the most recent tagged release.
 2. Install requirements: `pip install -r requirements.txt`
 3. Configure the appropriate parameters either by using the command line or `params.config`.
-4. Execute: `python cleanup_tool.py <CONFIG_FILE>` 
+4. Execute: `python sca_cleanup_tool.py <CONFIG_FILE>` 
 
 ## Examples:
 Perform dry run check-in to get to know which projects would have been deleted:  
-`ws_cleanup_tool -r 30 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -y true`
+`mend_sca_cleanup_tool -r 30 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -y true`
 
 ---
 
 Keep the last 60 days on each product, omitting a product token <PRODUCT_1> from analyzing:  
-`ws_cleanup_tool -r 60 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -e <PRODUCT_TOKEN_1>`
+`mend_sca_cleanup_tool -r 60 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -e <PRODUCT_TOKEN_1>`
 
 ---
 
 Keep only two of the newest projects in each product token PRODUCT_1 and PRODUCT_2:  
-`ws_cleanup_tool -r 2 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2>`
+`mend_sca_cleanup_tool -r 2 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2>`
 
 ---
 
 Analyze only the projects that have the specified Mend tag and keep the newest project in each product:  
-`ws_cleanup_tool -r 1 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<VALUE>`
+`mend_sca_cleanup_tool -r 1 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<VALUE>`
 
 ---
 
 Keep the last 2 weeks and analyze only the projects whose match their tag key and the tag value contains the specified regex:  
-`ws_cleanup_tool -r 14 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<REGEX_VALUE>`
+`mend_sca_cleanup_tool -r 14 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<REGEX_VALUE>`
 
 ---
 
 Keep the last 100 days for both PRODUCT_1 and PRODUCT_2, but do not delete the project PROJECT_1 (which is a project in one of the included products):  
-`ws_cleanup_tool -r 100 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -x <PROJECT_TOKEN_1>`
+`mend_sca_cleanup_tool -r 100 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -x <PROJECT_TOKEN_1>`
 
 ---
 
 Keep the last month for both PRODUCT_1 and PRODUCT_2, but do not delete projects that contain provided strings in their names:  
-`ws_cleanup_tool -r 31 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -n CI_,-test`
+`mend_sca_cleanup_tool -r 31 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -n CI_,-test`
 
 ---
 
 
 ## Full Usage flags:
 ```shell
 usage: ws_cleanup_tool [-h] -u MEND_USER_KEY -k MEND_TOKEN [-a MEND_URL] [-t REPORT_TYPES] [-m {FilterProjectsByUpdateTime,FilterProjectsByLastCreatedCopies}] [-o OUTPUT_DIR] [-e EXCLUDED_PRODUCT_TOKENS] [-i INCLUDED_PRODUCT_TOKENS]
@@ -103,18 +104,18 @@
 
 Mend Cleanup Tool
 
 optional arguments:
   -h, --help            show this help message and exit
   -u MEND_USER_KEY, --userKey 
                     Mend User Key
-  -k MEND_ORG_TOKEN, --orgToken
+  -k MEND_API_TOKEN, --apiToken, --orgToken
                     Mend Organization Key (API Key)
-  -a MEND_URL, --wsUrl
-                    Mend URL
+  -a MEND_URL, --mendUrl, --wsURL
+                    Mend URL. This value defaults to saas.whitesourcesoftware.com.
   -t REPORT_TYPES, --reportTypes
                     Report Types to generate (comma seperated list)
   -m OPERATION_MODE, --operationMode {FilterProjectsByUpdateTime,FilterProjectsByLastCreatedCopies}
                     Cleanup operation mode
   -o OUTPUT_DIR, --outputDir
                     Output directory
   -e EXCLUDED_PRODUCT_TOKENS, --excludedProductTokens
@@ -142,10 +143,32 @@
                     default False                                        
   -x EXCLUDED_PROJECT_TOKENS, --excludedProjectTokens
                     List of excluded projects
   -n EXCLUDED_PROJECT_NAME_PATTERNS, --excludedProjectNamePatterns
                     List of excluded project name patterns                 
 ```
 
+## Available reports
+The following Mend project reports are available through the clean-up tool. These values can be specified with the -t flag to generate specific reports.
+* alerts
+* alerts_rejected_by_policy
+* attribution
+* bugs
+* due_diligence
+* ignored_alerts
+* in_house_libraries
+* inventory
+* license_compatibility
+* resolved_alerts
+* request_history
+* source_files
+* source_file_inventory
+* vulnerability
+
+## SAST Clean up
+If you need to run a clean up script for your SAST environment, please refer to the Mend SAST clean up kit in the [Mend Toolkit](https://github.com/mend-toolkit/mend-examples/tree/main/Scripts/Mend%20SAST) 
+
 **note:** The optimal cleanup scope is derived from the size of the environment, Mend scope size (memory and CPU) allocated for the server, and runtime time constraints.    
 
 
+
+
```

## Comparing `mend_sca_cleanup_tool-23.6.1.dist-info/RECORD` & `mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mend_sca_cleanup_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_sca_cleanup_tool/_version.py,sha256=Nb5HGWjRwIgIeY9iUEJLL6q7qRwyzyxkcN7bkw2FysA,100
-mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=hZZMdTmkB_x5RnI3h3JE85gV8WV031p0M2XSSr_FRIg,20717
-mend_sca_cleanup_tool-23.6.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_sca_cleanup_tool-23.6.1.dist-info/METADATA,sha256=JfrGZDnxH9dk24EKkkBwfnSyPPxhXWl1qVV8iKMDa0Q,8197
-mend_sca_cleanup_tool-23.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_sca_cleanup_tool-23.6.1.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
-mend_sca_cleanup_tool-23.6.1.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
-mend_sca_cleanup_tool-23.6.1.dist-info/RECORD,,
+mend_sca_cleanup_tool/_version.py,sha256=0PxJlAFQcv_72t4q6XWUsiO_afOSZ-OpVl1fisDf2b0,102
+mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=jnqnJglRWkL__KJXJ3eeTyPjp-BGcTMTK2JKGy74_TY,20958
+mend_sca_cleanup_tool-23.6.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_sca_cleanup_tool-23.6.1.1.dist-info/METADATA,sha256=l1x7VgVO2QRFd2G6HjERvnRKNXkqe9D5AeBRhblLvQQ,9116
+mend_sca_cleanup_tool-23.6.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_sca_cleanup_tool-23.6.1.1.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
+mend_sca_cleanup_tool-23.6.1.1.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
+mend_sca_cleanup_tool-23.6.1.1.dist-info/RECORD,,
```

