# Comparing `tmp/problem_bank_scripts-0.4.8.tar.gz` & `tmp/problem_bank_scripts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.4.8.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.5.0.tar", max compression
```

## Comparing `problem_bank_scripts-0.4.8.tar` & `problem_bank_scripts-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.4.8/LICENSE
--rw-r--r--   0        0        0     1244 2021-05-17 01:13:34.351180 problem_bank_scripts-0.4.8/README.md
--rw-r--r--   0        0        0     1052 2023-04-27 22:44:16.983311 problem_bank_scripts-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-27 22:44:29.527049 problem_bank_scripts-0.4.8/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.4.8/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    42266 2023-04-27 22:42:38.360459 problem_bank_scripts-0.4.8/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.4.8/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.4.8/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2263 2023-04-27 22:45:31.903769 problem_bank_scripts-0.4.8/setup.py
--rw-r--r--   0        0        0     2318 2023-04-27 22:45:31.904000 problem_bank_scripts-0.4.8/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1244 2021-05-17 01:13:34.351180 problem_bank_scripts-0.5.0/README.md
+-rw-r--r--   0        0        0     1052 2023-06-14 21:39:32.611573 problem_bank_scripts-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-06-14 21:39:35.225325 problem_bank_scripts-0.5.0/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.5.0/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    43948 2023-06-14 21:36:06.930925 problem_bank_scripts-0.5.0/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.5.0/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.5.0/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2263 2023-06-14 21:40:22.378440 problem_bank_scripts-0.5.0/setup.py
+-rw-r--r--   0        0        0     2318 2023-06-14 21:40:22.378661 problem_bank_scripts-0.5.0/PKG-INFO
```

### Comparing `problem_bank_scripts-0.4.8/README.md` & `problem_bank_scripts-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.4.8/pyproject.toml` & `problem_bank_scripts-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.4.8"
+version = "0.5.0"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
```

### Comparing `problem_bank_scripts-0.4.8/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.5.0/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.4.8/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.5.0/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -412,25 +412,26 @@
         parsed_question (dict]): [description]
     """
 
     # Deal with optional tags in info.json
     optional = ""
 
     if parsed_question["header"].get("gradingMethod"):
-        optional += """ "gradingMethod": parsed_question['header']['gradingMethod'],\n"""
-    elif parsed_question["header"].get("partialCredit"):
-        optional += """ "partialCredit": parsed_question['header']['partialCredit'],\n"""
-    elif parsed_question["header"].get("externalGradingOptions"):
-        optional += """ "externalGradingOptions": parsed_question['header']['externalGradingOptions'],\n"""
-    elif parsed_question["header"].get("dependencies"):
-        optional += """ "dependencies": parsed_question['header']['dependencies'],\n"""
-    elif parsed_question["header"].get("singleVariant"):
-        optional += """ "singleVariant": parsed_question['header']['singleVariant'],\n"""
-    elif parsed_question["header"].get("showCorrectAnswer"):
-        optional += """ "showCorrectAnswer": parsed_question['header']['showCorrectAnswer'],\n"""
+        optional += """\"gradingMethod": \"""" + parsed_question['header']['gradingMethod'] + """\",\n\t\t"""
+    if parsed_question["header"].get("partialCredit"):
+        optional += """\"partialCredit":""" + str(parsed_question['header']['partialCredit']).lower() + """,\n\t\t"""
+    if parsed_question["header"].get("dependencies"):
+        optional += """\"dependencies": """ + parsed_question['header']['dependencies'] + """,\n\t\t"""
+    if parsed_question["header"].get("singleVariant"):
+        optional += """\"singleVariant": """ + str(parsed_question['header']['singleVariant']).lower() + """,\n\t\t"""
+    if parsed_question["header"].get("showCorrectAnswer"):
+        optional += """\"showCorrectAnswer": """ + str(parsed_question['header']['showCorrectAnswer']).lower() + """,\n\t\t"""
+    if parsed_question["header"].get("externalGradingOptions"):
+        optional += """\"externalGradingOptions": """ + json.dumps(parsed_question['header']['externalGradingOptions']) + """,\n\t\t"""
+    optional = optional[:-4] + """\n"""
 
     # Add tags based on part type
     q_types = []
 
     for pnum in range(1, parsed_question["num_parts"] + 1):
         part = "part" + f"{pnum}"
         q_types.append(parsed_question["header"][part]["type"])
@@ -448,23 +449,26 @@
     pathlib.Path(output_path / "info.json").write_text(
         """{
             "uuid": \""""
         + str(uuid.uuid3(uuid.NAMESPACE_DNS, str(output_path)))
         + """\",
             "title": \""""
         + parsed_question["header"]["title"]
-        + """",
+        + """\",
             "topic": \""""
         + parsed_question["header"]["topic"]
-        + """",
+        + """\",
             "tags":  """
         + json.dumps(auto_tags)
         + """,
-            "type": "v3"
-        }""",
+            "type": "v3\""""
+        + ((""",
+            """
+        + optional) if (optional) else ("""\n"""))
+        + """}""",
         encoding="utf8",
     )
 
 
 def assemble_server_py(parsed_question, location):
     """Assembles a string version of the server.py file from the YAML header of the md file.
 
@@ -686,14 +690,35 @@
     # TODO: Add better support for what students see when they upload a file where many are possible. Currently: Error: The following required files were missing: *.jpg, *.pdf, foo.py, bar.c, filename space.txt
     # TODO: Add support for wildcard *.png
     # TODO: Add better message telling students the question needs to be manually graded.
 
     return replace_tags(html)
 
 
+def process_file_editor(part_name, parsed_question, data_dict):
+    """Processes markdown format of code-input questions and returns PL HTML
+    Args:
+        part_name (string): Name of the question part being processed (e.g., part1, part2, etc...)
+        parsed_question (dict): Dictionary of the MD-parsed question (output of `read_md_problem`)
+        data_dict (dict): Dictionary of the `data` dict created after running server.py using `exec()`
+
+    Returns:
+        html: A string of HTML that is part of the final PL question.html file.
+    """
+    pl_customizations = " ".join(
+        [f'{k} = "{v}"' for k, v in parsed_question["header"][part_name]["pl-customizations"].items()]
+    )  # PL-customizations
+
+    html = f"""<pl-question-panel>\n<markdown>{parsed_question['body_parts_split'][part_name]['content']}</markdown>\n</pl-question-panel>\n\n"""
+
+    html += f"""<pl-file-editor { pl_customizations } > </pl-file-editor>"""
+
+    return replace_tags(html)
+
+
 def replace_tags(string):
     """Takes in a string with tags: |@ and @| and returns {{ and }} respectively. This is because Python strings can't have double curly braces.
 
     Args:
         string (str): String to be processed, can be multi-line.
 
     Returns:
@@ -1017,14 +1042,16 @@
             question_html += process_symbolic_input(part, parsed_q, data2)
         elif "dropdown" in q_type:
             question_html += process_dropdown(part, parsed_q, data2)
         elif "longtext" in q_type:
             question_html += process_longtext(part, parsed_q, data2)
         elif "file-upload" in q_type:
             question_html += process_file_upload(part, parsed_q, data2)
+        elif "file-editor" in q_type:
+            question_html += process_file_editor(part, parsed_q, data2)
         else:
             raise NotImplementedError(f"This question type ({q_type}) is not yet implemented.")
 
         if parsed_q["num_parts"] > 1:
             question_html += "</div>\n</div>\n"
 
         # Add pl-submission-panel and pl-answer-panel (if they exist)
@@ -1062,14 +1089,21 @@
     # Move image assets
     files_to_copy = parsed_q["header"].get("assets")
     if files_to_copy:
         pl_path = output_path / "clientFilesQuestion"
         pl_path.mkdir(parents=True, exist_ok=True)
         [copy2(pathlib.Path(source_filepath).parent / fl, pl_path / fl) for fl in files_to_copy]
 
+    # Move autograde py test files
+    files_to_copy = parsed_q["header"].get("autogradeTestFiles")
+    if files_to_copy:
+        pl_path = output_path / "tests"
+        pl_path.mkdir(parents=True, exist_ok=True)
+        [copy2(pathlib.Path(source_filepath).parent / "tests" / fl, pl_path / fl) for fl in files_to_copy]
+
 
 def pl_image_path(html):
 
     """Adds `{{options.client_files_question_url}}` directory before the path automatically"""
 
     # TODO: Figure out the regex to make this into a single expression, maybe with |
     # If image files are included as markdown format, add {{options.client_files_question_url}}
```

### Comparing `problem_bank_scripts-0.4.8/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.5.0/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.4.8/setup.py` & `problem_bank_scripts-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'numpy>=1.22,<2.0',
  'pandas>=1.2.4,<2.0.0',
  'problem-bank-helpers>=0.1.12,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.4.8',
+    'version': '0.5.0',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
```

### Comparing `problem_bank_scripts-0.4.8/PKG-INFO` & `problem_bank_scripts-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.4.8
+Version: 0.5.0
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

