# Comparing `tmp/velesresearch-0.0.7.tar.gz` & `tmp/velesresearch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velesresearch-0.0.7.tar", max compression
+gzip compressed data, was "velesresearch-0.0.8.tar", max compression
```

## Comparing `velesresearch-0.0.7.tar` & `velesresearch-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-11 02:01:05.236054 velesresearch-0.0.7/LICENSE
--rw-r--r--   0        0        0     1707 2023-06-11 02:01:05.236054 velesresearch-0.0.7/README.md
--rw-r--r--   0        0        0      825 2023-06-11 02:01:05.240054 velesresearch-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      158 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/__init__.py
--rw-r--r--   0        0        0      795 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/options.py
--rw-r--r--   0        0        0     6562 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/structure.py
--rw-r--r--   0        0        0     2358 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/tools.py
--rw-r--r--   0        0        0     2473 1970-01-01 00:00:00.000000 velesresearch-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-13 15:18:11.932737 velesresearch-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1946 2023-06-13 15:18:11.932737 velesresearch-0.0.8/README.md
+-rw-r--r--   0        0        0      825 2023-06-13 15:18:26.591014 velesresearch-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      186 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/options.py
+-rw-r--r--   0        0        0      572 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/questiontypes.py
+-rw-r--r--   0        0        0     6686 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/structure.py
+-rw-r--r--   0        0        0     2330 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/tools.py
+-rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 velesresearch-0.0.8/PKG-INFO
```

### Comparing `velesresearch-0.0.7/LICENSE` & `velesresearch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.7/README.md` & `velesresearch-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,34 +11,46 @@
 
 [![PyPI](https://img.shields.io/pypi/v/velesresearch)](https://pypi.org/project/velesresearch/)
 [![GitHub](https://img.shields.io/badge/license-GPL--3.0-informational)](https://github.com/jakub-jedrusiak/VelesResearch/blob/main/LICENSE)
 [![codecov](https://codecov.io/gh/jakub-jedrusiak/VelesResearch/branch/main/graph/badge.svg?token=CGc3zeDxFi)](https://codecov.io/gh/jakub-jedrusiak/VelesResearch)
 
 <!-- badges: end -->
 
-Veles is a free and open source python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
+Veles is a free and open source Python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with Python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
 
 Veles is in pre-alpha development, but the goal features are:
 
 -   Free and open source.
 
 -   Text-based, so automatable and easily modifiable.
 
 -   Integration with GitHub.
 
 -   Ability to use JavaScript and CSS directly.
 
 -   [Open source documentation](https://jakub-jedrusiak.github.io/veles-docs/).
 
--   Python-based, so every python tools work.
+-   Python-based, so every Python tools work.
 
 -   Esay to collaborate through git.
 
 -   VS code extension pack.
 
 -   Custom redirection in the end (for panels).
 
 -   PsychoPy integration.
 
 -   JavaScript code preview.
 
 -   Modifiable themes.
+
+# Installation
+
+You can install the current version of Veles with:
+``` bash
+pip install velesresearch
+```
+
+You can install development version (unstable) with:
+``` bash
+pip install https://github.com/jakub-jedrusiak/VelesResearch.git
+```
```

### Comparing `velesresearch-0.0.7/pyproject.toml` & `velesresearch-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "velesresearch"
-version = "0.0.7"
+version = "0.0.8"
 description = "Veles is a free and open source python survey tool for researchers."
 license = "GPL-3.0-or-later"
 authors = ["Jakub Jędrusiak <kuba23031999@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jakub-jedrusiak/VelesResearch"
 documentation = "https://jakub-jedrusiak.github.io/VelesDocs"
 packages = [{include = "velesresearch"}]
```

### Comparing `velesresearch-0.0.7/velesresearch/options.py` & `velesresearch-0.0.8/velesresearch/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     "Options for Page object"
     read_only: bool = False
     time_limit: int | None = None
     visible: bool = True
 
 
 class SurveyOptions(BaseModel):
-    "Optrions for Survey object"
+    "Options for Survey object"
     language: str = "en"
     url_on_complete: str | None = None
```

### Comparing `velesresearch-0.0.7/velesresearch/structure.py` & `velesresearch-0.0.8/velesresearch/structure.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import numpy as np
 from .options import QuestionOptions, PageOptions, SurveyOptions
 
 
 class Question(BaseModel):
     "General question class"
     label: str
-    question_type: str
     question_text: str
     answers: str | Sequence[str]
+    question_type: str = "radio"
     options: QuestionOptions | None = None
     description: str | None = None
 
     def __str__(self):
         answers = "  - " + "\n  - ".join(self.answers)
         return (
             f"{self.label}:\n  {self.question_text} ({self.question_type})\n{answers}"
@@ -112,84 +112,83 @@
                     return page
 
 
 class SurveyEncoder(JSONEncoder):
     "Create SurveyJS-compliant json from Question object"
 
     def default(self, o):
-        if isinstance(o, Survey):
+        # dictionary for mapping question types to SurveyJS types
+        surveyjs_types = {"radio": "radiogroup", "checkbox": "checkbox"}
+
+        if isinstance(o, Question):
             json = {
-                "title": o.title,
-                "description": o.description,
-                "pages": [self.default(p) for p in o.pages],
+                "name": o.label,
+                "type": surveyjs_types[o.question_type],
+                "title": o.question_text,
+                "choices": o.answers,
             }
 
             if o.options:
+                # dictionary for mapping question options to SurveyJS options
+                surveyjs_question_options = {
+                    "required": ["isRequired", False],
+                    "answers_order": ["choicesOrder", "none"],
+                    "inherit_answers": ["choicesByUrl", None],
+                    "comment": ["hasComment", False],
+                    "comment_text": ["commentText", "Other"],
+                    "comment_placeholder": ["commentPlaceHolder", ""],
+                    "visible": ["visible", True],
+                    "other": ["hasOther", False],
+                    "other_text": ["otherText", "Other"],
+                    "other_placeholder": ["otherPlaceHolder", ""],
+                    "none": ["hasNone", False],
+                    "none_text": ["noneText", "None"],
+                    "clear_button": ["showClearButton", False],
+                }
                 opts = o.options.__dict__
-                if opts["language"] != "en":
-                    json["locale"] = opts["language"]
-                if opts["url_on_complete"]:
-                    json["navigateToUrl"] = opts["url_on_complete"]
+                for key in opts.keys():
+                    if opts[key] != surveyjs_question_options[key][1]:
+                        json[surveyjs_question_options[key][0]] = opts[key]
 
         elif isinstance(o, Page):
+            # dictionary for mapping page options to SurveyJS options
+            surveyjs_page_options = {
+                "read_only": ["readOnly", False],
+                "time_limit": ["maxTimeToFinish", None],
+                "visible": ["visible", True],
+            }
+
             json = {
                 "name": o.label,
                 "elements": [self.default(q) for q in o.questions],
             }
 
             if o.title:
                 json["title"] = o.title
             if o.description:
                 json["description"] = o.description
             if o.options:
                 opts = o.options.__dict__
-                if opts["read_only"]:
-                    json["readOnly"] = True
-                if opts["time_limit"]:
-                    json["maxTimeToFinish"] = opts["time_limit"]
-                if not opts["visible"]:
-                    json["visible"] = False
-
-        else:
-            # SurveyJS types dictionary
-            surveyjs_types = {"radio": "radiogroup", "checkbox": "checkbox"}
+                for key in opts.keys():
+                    if opts[key] != surveyjs_page_options[key][1]:
+                        json[surveyjs_page_options[key][0]] = opts[key]
 
-            json = {
-                "name": o.label,
-                "type": surveyjs_types[o.question_type],
-                "title": o.question_text,
-                "choices": o.answers,
+        if isinstance(o, Survey):
+            # dictionary for mapping survey options to SurveyJS options
+            surveyjs_survey_options = {
+                "language": ["locale", "en"],
+                "url_on_complete": ["navigateToUrl", None],
             }
 
-            if o.description:
-                json["description"] = o.description
+            json = {
+                "title": o.title,
+                "description": o.description,
+                "pages": [self.default(p) for p in o.pages],
+            }
 
             if o.options:
                 opts = o.options.__dict__
-                if not opts["visible"]:
-                    json["visible"] = False
-                if opts["required"]:
-                    json["isRequired"] = True
-                if opts["answers_order"] != "none":
-                    json["choicesOrder"] = opts["answers_order"]
-                if opts["inherit_answers"]:
-                    json["choicesFromQuestion"] = opts["inherit_answers"]
-                if opts["comment"]:
-                    json["showCommentArea"] = True
-                    if opts["comment_text"]:
-                        json["commentText"] = opts["comment_text"]
-                    if opts["comment_placeholder"]:
-                        json["commentPlaceholder"] = opts["comment_placeholder"]
-                if opts["other"]:
-                    json["showOtherItem"] = True
-                    if opts["other_text"]:
-                        json["otherText"] = opts["other_text"]
-                    if opts["other_placeholder"]:
-                        json["otherPlaceHolder"] = opts["other_placeholder"]
-                if opts["none"]:
-                    json["showNoneItem"] = True
-                    if opts["none_text"]:
-                        json["noneText"] = opts["none_text"]
-                if opts["clear_button"]:
-                    json["showClearButton"] = True
+                for key in opts.keys():
+                    if opts[key] != surveyjs_survey_options[key][1]:
+                        json[surveyjs_survey_options[key][0]] = opts[key]
 
         return json
```

### Comparing `velesresearch-0.0.7/velesresearch/tools.py` & `velesresearch-0.0.8/velesresearch/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,85 +2,77 @@
 from collections.abc import Sequence
 from pydantic import validate_arguments
 import numpy as np
 from .structure import Question, Page, Survey
 from .options import QuestionOptions, PageOptions, SurveyOptions
 
 
+@validate_arguments
 def question(
     label: str,
-    question_type: str,
-    question_text: str,
+    question_text: str | Sequence[str],
     *answers: str | Sequence[str],
-    options: QuestionOptions | None = None,
+    question_type: str = "radio",
     description: str | None = None,
+    options: QuestionOptions | None = None,
 ) -> Question:
     "Wrapper around Question class"
-    answers = list(np.concatenate([answers]).flat)
-    return Question(
-        label=label,
-        question_type=question_type,
-        question_text=question_text,
-        answers=answers,
-        options=options,
-        description=description,
-    )
-
-
-@validate_arguments
-def questionnaire(
-    label: str,
-    items: Sequence[str] | str,
-    answers: Sequence[str] | str,
-    question_type: str = "radio",
-    options: QuestionOptions | None = None,
-    description: str | None = None,
-) -> list[Question]:
-    "Convert whole questionnaire to Question objects list"
-    q_list = []
-    for i in enumerate(items):
-        q_list.append(
-            Question(
-                label=f"{label}_{i[0] + 1}",
-                question_type=question_type,
-                question_text=i[1],
-                answers=answers,
-                options=options,
-                description=description,
-            )
+    answers_list = list(np.concatenate([answers]).flat)
+    if isinstance(question_text, str):
+        return Question(
+            label=label,
+            question_text=question_text,
+            answers=answers_list,
+            question_type=question_type,
+            description=description,
+            options=options,
         )
-    return q_list
+    else:
+        question_list = list(np.concatenate([question_text]).flat)
+        q_list = []
+        for i in enumerate(question_list):
+            q_list.append(
+                Question(
+                    label=f"{label}_{i[0] + 1}",
+                    question_text=i[1],
+                    answers=answers_list,
+                    question_type=question_type,
+                    description=description,
+                    options=options,
+                )
+            )
+        return q_list
 
 
 def page(
     label: str,
     *questions: Question | Sequence[Question],
     title: str | None = None,
     description: str | None = None,
     options: PageOptions | None = None,
 ) -> Page:
     "Wrapper around Page class"
-    questions = list(np.concatenate([questions]).flat)
+    questions_list = list(np.concatenate([questions]).flat)
     return Page(
         label=label,
-        questions=questions,
+        questions=questions_list,
         title=title,
         description=description,
         options=options,
     )
 
 
 def survey(
     *pages: Page | Sequence[Page],
     title: str | None = None,
     description: str | None = None,
     options: SurveyOptions | None = None,
     create_file: bool = True,
 ) -> Survey:
     "Create Survey object from pages, create json file"
-    pages = list(np.concatenate([pages]).flat)
+    pages_list = list(np.concatenate([pages]).flat)
     survey_obj = Survey(
-        pages=pages, title=title, description=description, options=options
+        pages=pages_list, title=title, description=description, options=options
     )
     if create_file:
         survey_obj.create()
     return survey_obj
```

### Comparing `velesresearch-0.0.7/PKG-INFO` & `velesresearch-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velesresearch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Veles is a free and open source python survey tool for researchers.
 Home-page: https://github.com/jakub-jedrusiak/VelesResearch
 License: GPL-3.0-or-later
 Author: Jakub Jędrusiak
 Author-email: kuba23031999@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -29,35 +29,47 @@
 
 [![PyPI](https://img.shields.io/pypi/v/velesresearch)](https://pypi.org/project/velesresearch/)
 [![GitHub](https://img.shields.io/badge/license-GPL--3.0-informational)](https://github.com/jakub-jedrusiak/VelesResearch/blob/main/LICENSE)
 [![codecov](https://codecov.io/gh/jakub-jedrusiak/VelesResearch/branch/main/graph/badge.svg?token=CGc3zeDxFi)](https://codecov.io/gh/jakub-jedrusiak/VelesResearch)
 
 <!-- badges: end -->
 
-Veles is a free and open source python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
+Veles is a free and open source Python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with Python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
 
 Veles is in pre-alpha development, but the goal features are:
 
 -   Free and open source.
 
 -   Text-based, so automatable and easily modifiable.
 
 -   Integration with GitHub.
 
 -   Ability to use JavaScript and CSS directly.
 
 -   [Open source documentation](https://jakub-jedrusiak.github.io/veles-docs/).
 
--   Python-based, so every python tools work.
+-   Python-based, so every Python tools work.
 
 -   Esay to collaborate through git.
 
 -   VS code extension pack.
 
 -   Custom redirection in the end (for panels).
 
 -   PsychoPy integration.
 
 -   JavaScript code preview.
 
 -   Modifiable themes.
 
+# Installation
+
+You can install the current version of Veles with:
+``` bash
+pip install velesresearch
+```
+
+You can install development version (unstable) with:
+``` bash
+pip install https://github.com/jakub-jedrusiak/VelesResearch.git
+```
+
```

