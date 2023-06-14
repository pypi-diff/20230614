# Comparing `tmp/psbs-0.0.9.tar.gz` & `tmp/psbs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psbs-0.0.9.tar", last modified: Sun Jun 11 16:17:51 2023, max compression
+gzip compressed data, was "psbs-0.1.0.tar", last modified: Wed Jun 14 19:41:29 2023, max compression
```

## Comparing `psbs-0.0.9.tar` & `psbs-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-11 16:17:51.901202 psbs-0.0.9/
--rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.0.9/LICENSE
--rw-r--r--   0 jcmiller   (501) staff       (20)     5494 2023-06-11 16:17:51.901419 psbs-0.0.9/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)     4774 2023-06-11 15:18:39.000000 psbs-0.0.9/README.md
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-11 16:17:51.896973 psbs-0.0.9/psbs/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.0.9/psbs/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.0.9/psbs/__main__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-06-07 15:11:32.000000 psbs-0.0.9/psbs/config.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      871 2023-06-10 00:05:18.000000 psbs-0.0.9/psbs/example.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)     2721 2023-06-11 15:23:02.000000 psbs-0.0.9/psbs/gister.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     2301 2023-06-09 23:14:31.000000 psbs-0.0.9/psbs/images.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     3847 2023-06-11 15:25:11.000000 psbs-0.0.9/psbs/project.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     3184 2023-06-11 15:10:39.000000 psbs-0.0.9/psbs/psbs.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1573 2023-06-07 22:59:45.000000 psbs-0.0.9/psbs/psparser.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1256 2023-06-09 23:02:50.000000 psbs-0.0.9/psbs/template.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      728 2023-06-09 22:23:16.000000 psbs-0.0.9/psbs/templatebuilder.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.0.9/psbs/token.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1923 2023-06-07 22:50:58.000000 psbs-0.0.9/psbs/utils.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-11 16:17:51.900730 psbs-0.0.9/psbs.egg-info/
--rw-r--r--   0 jcmiller   (501) staff       (20)     5494 2023-06-11 16:17:51.000000 psbs-0.0.9/psbs.egg-info/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)      417 2023-06-11 16:17:51.000000 psbs-0.0.9/psbs.egg-info/SOURCES.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-06-11 16:17:51.000000 psbs-0.0.9/psbs.egg-info/dependency_links.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-06-11 16:17:51.000000 psbs-0.0.9/psbs.egg-info/entry_points.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       34 2023-06-11 16:17:51.000000 psbs-0.0.9/psbs.egg-info/requires.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-06-11 16:17:51.000000 psbs-0.0.9/psbs.egg-info/top_level.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-06-11 16:17:51.902142 psbs-0.0.9/setup.cfg
--rw-r--r--   0 jcmiller   (501) staff       (20)     1263 2023-06-11 16:16:57.000000 psbs-0.0.9/setup.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.641049 psbs-0.1.0/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.1.0/LICENSE
+-rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-14 19:41:29.641291 psbs-0.1.0/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)     4874 2023-06-14 19:38:32.000000 psbs-0.1.0/README.md
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.634924 psbs-0.1.0/psbs/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.1.0/psbs/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.1.0/psbs/__main__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-06-07 15:11:32.000000 psbs-0.1.0/psbs/config.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      871 2023-06-10 00:05:18.000000 psbs-0.1.0/psbs/example.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      545 2023-06-14 19:27:02.000000 psbs-0.1.0/psbs/extension.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      125 2023-06-14 19:20:28.000000 psbs-0.1.0/psbs/extensionloader.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.640067 psbs-0.1.0/psbs/extensions/
+-rw-r--r--   0 jcmiller   (501) staff       (20)      225 2023-06-14 16:33:22.000000 psbs-0.1.0/psbs/extensions/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3101 2023-06-14 19:25:25.000000 psbs-0.1.0/psbs/extensions/images.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2721 2023-06-11 15:23:02.000000 psbs-0.1.0/psbs/gister.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     4117 2023-06-14 19:20:01.000000 psbs-0.1.0/psbs/project.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-06-14 10:55:45.000000 psbs-0.1.0/psbs/psbs.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1573 2023-06-07 22:59:45.000000 psbs-0.1.0/psbs/psparser.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1549 2023-06-14 19:36:41.000000 psbs-0.1.0/psbs/template.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      728 2023-06-09 22:23:16.000000 psbs-0.1.0/psbs/templatebuilder.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.1.0/psbs/token.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.1.0/psbs/utils.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.638650 psbs-0.1.0/psbs.egg-info/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)      498 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/entry_points.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       34 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/requires.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/top_level.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-06-14 19:41:29.642054 psbs-0.1.0/setup.cfg
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1239 2023-06-14 19:39:12.000000 psbs-0.1.0/setup.py
```

### Comparing `psbs-0.0.9/LICENSE` & `psbs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psbs-0.0.9/PKG-INFO` & `psbs-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.0.9
+Version: 0.1.0
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.0.9.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.0.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
-Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.8
@@ -37,37 +36,42 @@
  - Supports most PuzzleScript forks including [Pattern:Script](https://github.com/ClementSparrow/Pattern-Script)
  - Use your favorite version control for your PuzzleScript Projects
 
 ## Installing
 
 If you already have Python 3.8 or greater and pip installed simply run the following command from your terminal
 
-`pip install 'psbs @ git+https://github.com/jcmiller11/PSBS'`
+`pip install psbs`
 
 If you don't have Python and pip installed: [Download Python](https://www.python.org/downloads/)
 
 ## Connecting to GitHub
 
 PSBS will build your projects into PuzzleScript source without interacting with GitHub at all, however uploading and running your projects requires an authorization token.
 
 By default PSBS will attempt to run `gh auth token` to recieve an authorization token from the GitHub command line tool.  If you would like to use a different token or prefer not to install the GitHub command line tool you can run the following command.
 
-`psbs token insert your token here`
+`psbs token `*`insert_your_token_here`*
 
 ## Usage
 
 Enter `psbs` into your terminal to get a list of commands
 
 Commands:
 
 `psbs new` Creates a new project
+
 `psbs build` Builds the project in the current working directory
+
 `psbs upload` Builds project then uploads it to gist
+
 `psbs run` Builds project, uploads it, then runs it in your web browser
 
+`psbs token` Check or set the GitHub auth token
+
 For more information on these commands and to see available flags enter `psbs help `*`command`*
 
 ## CLI Example
 
     psbs new myProject
     cd myProject
     psbs build
@@ -95,17 +99,24 @@
         └── wincondition.pss
 
 
 ## Config.yaml
 
 At the root of your project you will find a file called config.yaml containing configuration variables for your project
 
-- engine: the url of the fork you are using, by default https://www.puzzlescript.net/
 - gist_id: the id of the gist the upload and run commands should use to store this project in
-- template: the name of your root template file, by default main.pss
+- engine: the url of the fork you are using, by default https://www.puzzlescript.net/
+- template: the name of your root template file, by default main.pssengine: https://auroriax.github.io/PuzzleScript/
+
+Below these are optional config variables for template extensions
+
+- Images:
+  - alpha: whether to include the RGBA alpha values for transparency supported by some forks
+  - max_colors: maximum colors in output object, PuzzleScript can only handle 10 by default but some forks support up to 36 colors
+
 
 ## Templates
 
 PSBS uses Jinja2, a fast, expressive, extensible templating engine, to build your PuzzleScript project.  To learn more about all of the features available to you check out the Jinja2 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
 To avoid conflicting with valid PuzzleScript code, the Jinja2 Tags have been changed as follows:
 
@@ -116,16 +127,14 @@
 A helper function has been added to the template environment `Image(filename)` that will import an image file directly into your game as a PuzzleScript object!
 
     Target
     ((image("images/target.png")))
 
 Additionally, this helper function contains the following optional parameters (alpha=False, max_colors=10, x=0, y=0, width=None, height=None)
 
-- alpha: (true/false) if true will include the RGBA alpha values for transparency supported by some forks
-- max_colors: (int) maximum colors in output object, PuzzleScript can only handle 10 by default but some forks such as Pattern:Script support up to 36 colors
 - x: (int) horizontal position in image to start importing from
 - y: (int) vertical position in image to start importing from
 - width: (int) width of the object to import, if None set to the width of the image file
 - height: (int) height of the object to import, if None set to the height of the image file
 
 By using the last four parameters listed one can load objects from a single image as a spritesheet.
```

### Comparing `psbs-0.0.9/README.md` & `psbs-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,37 +17,42 @@
  - Supports most PuzzleScript forks including [Pattern:Script](https://github.com/ClementSparrow/Pattern-Script)
  - Use your favorite version control for your PuzzleScript Projects
 
 ## Installing
 
 If you already have Python 3.8 or greater and pip installed simply run the following command from your terminal
 
-`pip install 'psbs @ git+https://github.com/jcmiller11/PSBS'`
+`pip install psbs`
 
 If you don't have Python and pip installed: [Download Python](https://www.python.org/downloads/)
 
 ## Connecting to GitHub
 
 PSBS will build your projects into PuzzleScript source without interacting with GitHub at all, however uploading and running your projects requires an authorization token.
 
 By default PSBS will attempt to run `gh auth token` to recieve an authorization token from the GitHub command line tool.  If you would like to use a different token or prefer not to install the GitHub command line tool you can run the following command.
 
-`psbs token insert your token here`
+`psbs token `*`insert_your_token_here`*
 
 ## Usage
 
 Enter `psbs` into your terminal to get a list of commands
 
 Commands:
 
 `psbs new` Creates a new project
+
 `psbs build` Builds the project in the current working directory
+
 `psbs upload` Builds project then uploads it to gist
+
 `psbs run` Builds project, uploads it, then runs it in your web browser
 
+`psbs token` Check or set the GitHub auth token
+
 For more information on these commands and to see available flags enter `psbs help `*`command`*
 
 ## CLI Example
 
     psbs new myProject
     cd myProject
     psbs build
@@ -75,17 +80,24 @@
         └── wincondition.pss
 
 
 ## Config.yaml
 
 At the root of your project you will find a file called config.yaml containing configuration variables for your project
 
-- engine: the url of the fork you are using, by default https://www.puzzlescript.net/
 - gist_id: the id of the gist the upload and run commands should use to store this project in
-- template: the name of your root template file, by default main.pss
+- engine: the url of the fork you are using, by default https://www.puzzlescript.net/
+- template: the name of your root template file, by default main.pssengine: https://auroriax.github.io/PuzzleScript/
+
+Below these are optional config variables for template extensions
+
+- Images:
+  - alpha: whether to include the RGBA alpha values for transparency supported by some forks
+  - max_colors: maximum colors in output object, PuzzleScript can only handle 10 by default but some forks support up to 36 colors
+
 
 ## Templates
 
 PSBS uses Jinja2, a fast, expressive, extensible templating engine, to build your PuzzleScript project.  To learn more about all of the features available to you check out the Jinja2 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
 To avoid conflicting with valid PuzzleScript code, the Jinja2 Tags have been changed as follows:
 
@@ -96,16 +108,14 @@
 A helper function has been added to the template environment `Image(filename)` that will import an image file directly into your game as a PuzzleScript object!
 
     Target
     ((image("images/target.png")))
 
 Additionally, this helper function contains the following optional parameters (alpha=False, max_colors=10, x=0, y=0, width=None, height=None)
 
-- alpha: (true/false) if true will include the RGBA alpha values for transparency supported by some forks
-- max_colors: (int) maximum colors in output object, PuzzleScript can only handle 10 by default but some forks such as Pattern:Script support up to 36 colors
 - x: (int) horizontal position in image to start importing from
 - y: (int) vertical position in image to start importing from
 - width: (int) width of the object to import, if None set to the width of the image file
 - height: (int) height of the object to import, if None set to the height of the image file
 
 By using the last four parameters listed one can load objects from a single image as a spritesheet.
```

### Comparing `psbs-0.0.9/psbs/example.txt` & `psbs-0.1.0/psbs/example.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.0.9/psbs/gister.py` & `psbs-0.1.0/psbs/gister.py`

 * *Files identical despite different names*

### Comparing `psbs-0.0.9/psbs/images.py` & `psbs-0.1.0/psbs/extensions/images.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,101 @@
 from textwrap import wrap
 
 import jinja2
 from PIL import Image
+from psbs.extension import Extension
 
 
-def rgba_to_hex(rgba_tuple, alpha=False):
-    output = ""
-    if rgba_tuple[3] == 0:
-        return "transparent"
-    if not alpha:
-        rgba_tuple = rgba_tuple[:-1]
-    for value in rgba_tuple:
-        output += format(value, "x").zfill(2)
-    return f"#{output}"
-
-
-def pixel_list_to_sprite(pixel_values, width=5, alpha=False):
-    colors = {}
-    colors["transparent"] = None
-    for pixel in pixel_values:
-        colors[rgba_to_hex(pixel, alpha)] = None
-
-    colors_list = list(colors.keys())
-
-    sprite = ""
-
-    for pixel in pixel_values:
-        color = colors_list.index(rgba_to_hex(pixel, alpha)) - 1
-        if color > 9:
-            color = chr(ord("a") + color - 10)
-        if color == -1:
-            color = "."
-        sprite += str(color)
-
-    sprite = wrap(sprite, width)
-    sprite = "\n".join(sprite)
-    return {"sprite": sprite, "colors": colors}
-
-
-def image_to_object(
-    file, alpha=False, max_colors=10, x=0, y=0, width=None, height=None
-):
-    if max_colors > 36:
-        raise jinja2.exceptions.TemplateError(
-            "Image helper function doesn't support more than 36 colors"
-        )
-    try:
-        image = Image.open(file, "r")
-    except IOError as err:
-        raise jinja2.exceptions.TemplateError(
-            f"Unable to read image file\n  {err}"
-        )
-    # Crop image if needed
-    if width:
-        right = x + width
-    else:
-        right = image.size[0]
-    if height:
-        bottom = y + height
-    else:
-        bottom = image.size[1]
-    image = image.crop((x, y, right, bottom))
-    image = image.convert("RGBA")
-    result = pixel_list_to_sprite(
-        image.getdata(), width=image.size[0], alpha=alpha
-    )
-    sprite = result["sprite"]
-    colors = result["colors"]
-    if len(colors) > 10:
-        if "." in sprite:
-            image = image.quantize(colors=max_colors + 1)
+class Images(Extension):
+    def __init__(self, config):
+        super().__init__(config)
+        self.register("image", self.image_to_object)
+        self.loaded_images = {}
+
+    @staticmethod
+    def get_config():
+        return {"alpha": False, "max_colors": 10}
+
+    def __rgba_to_hex(self, rgba_tuple):
+        output = ""
+        if rgba_tuple[3] == 0:
+            return "transparent"
+        if not self.config["alpha"]:
+            rgba_tuple = rgba_tuple[:-1]
+        for value in rgba_tuple:
+            output += format(value, "x").zfill(2)
+        return f"#{output}"
+
+    def __pixel_list_to_sprite(self, pixel_values, width):
+        colors = {}
+        colors["transparent"] = None
+        for pixel in pixel_values:
+            colors[self.__rgba_to_hex(pixel)] = None
+
+        colors_list = list(colors.keys())
+
+        sprite = ""
+
+        for pixel in pixel_values:
+            color = colors_list.index(self.__rgba_to_hex(pixel)) - 1
+            if color > 9:
+                color = chr(ord("a") + color - 10)
+            if color == -1:
+                color = "."
+            sprite += str(color)
+
+        sprite = wrap(sprite, width)
+        sprite = "\n".join(sprite)
+        return {"sprite": sprite, "colors": colors}
+
+    def image_to_object(
+        self,
+        file,
+        x=0,
+        y=0,
+        width=None,
+        height=None,
+    ):
+        if self.config["max_colors"] > 36:
+            raise jinja2.exceptions.TemplateError(
+                "Image helper function doesn't support more than 36 colors"
+            )
+        if file in self.loaded_images:
+            image = self.loaded_images[file]
+        else:
+            try:
+                image = Image.open(file, "r")
+            except IOError as err:
+                raise jinja2.exceptions.TemplateError(
+                    f"Unable to read image file\n  {err}"
+                )
+            self.loaded_images[file] = image
+        # Crop image if needed
+        if width:
+            right = x + width
+        else:
+            right = image.size[0]
+        if height:
+            bottom = y + height
         else:
-            image = image.quantize(colors=max_colors)
+            bottom = image.size[1]
+        image = image.crop((x, y, right, bottom))
         image = image.convert("RGBA")
-        result = pixel_list_to_sprite(
-            image.getdata(), width=image.size[0], alpha=alpha
+        result = self.__pixel_list_to_sprite(
+            image.getdata(), width=image.size[0]
         )
         sprite = result["sprite"]
         colors = result["colors"]
-    if len(colors) > 1:
-        colors.pop("transparent", None)
-    return f'{" ".join(colors)}\n{sprite}'
+        if len(colors) > 10:
+            if "." in sprite:
+                image = image.quantize(colors=self.config["max_colors"] + 1)
+            else:
+                image = image.quantize(colors=self.config["max_colors"])
+            image = image.convert("RGBA")
+            result = self.__pixel_list_to_sprite(
+                image.getdata(), width=image.size[0]
+            )
+            sprite = result["sprite"]
+            colors = result["colors"]
+        if len(colors) > 1:
+            colors.pop("transparent", None)
+        return f'{" ".join(colors)}\n{sprite}'
```

### Comparing `psbs-0.0.9/psbs/project.py` & `psbs-0.1.0/psbs/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from .gister import Gister
 from .config import Config
 from .psparser import split_ps, get_engine
 from .templatebuilder import make_template
 from .utils import read_file, write_file, write_yaml, make_dir, run_in_browser
 from .template import render_template
+from .extensionloader import get_extensions
 
 
 class PSBSProject:
     def __init__(self, config_filename="config.yaml"):
         self.config = Config(config_filename)
 
     def build(self):
@@ -28,15 +29,17 @@
             readme_path,
             "Play this game by pasting the script in "
             f"{self.config['engine']}editor.html",
         )
 
         # Build the script.txt
         print("Building script.txt")
-        source = render_template(path.join("src", self.config["template"]))
+        source = render_template(
+            path.join("src", self.config["template"]), self.config
+        )
 
         print(f"Writing file {script_path}")
         write_file(script_path, source)
 
     def upload(self):
         gist_id = self.config["gist_id"]
         if not self.config["gist_id"]:
@@ -78,25 +81,32 @@
         src_tree = split_ps(source)
 
         if new_gist:
             print("Creating new gist")
             gist = Gister()
             gist_id = gist.create(name=project_name)
 
+        config_dict = {
+            "gist_id": gist_id,
+            "engine": engine,
+            "template": "main.pss",
+        }
+
+        for extension in get_extensions():
+            if extension.get_config():
+                config_dict[extension.__name__] = extension.get_config()
+
         print("Building directory structure")
         make_dir(project_name)
         try:
             make_dir(path.join(project_name, "src"))
             make_dir(path.join(project_name, "bin"))
 
             print("Creating config file")
-            write_yaml(
-                path.join(project_name, "config.yaml"),
-                {"gist_id": gist_id, "engine": engine, "template": "main.pss"},
-            )
+            write_yaml(path.join(project_name, "config.yaml"), config_dict)
 
             print("Creating template file")
             write_file(
                 path.join(project_name, "src", "main.pss"),
                 make_template(src_tree),
             )
```

### Comparing `psbs-0.0.9/psbs/psbs.py` & `psbs-0.1.0/psbs/psbs.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,29 +81,25 @@
         project.upload()
     elif args.command == "run":
         project = PSBSProject()
         project.build()
         project.upload()
         project.run(editor=args.editor)
     elif args.command == "new":
-        if args.gist_id is not None:
-            PSBSProject.create(
-                args.name, gist_id=args.gist_id, new_gist=args.new_gist
-            )
-        elif args.file is not None:
-            PSBSProject.create(
-                args.name, file=args.file, new_gist=args.new_gist
-            )
-        else:
-            PSBSProject.create(args.name, new_gist=args.new_gist)
+        PSBSProject.create(
+            args.name,
+            gist_id=args.gist_id,
+            file=args.file,
+            new_gist=args.new_gist,
+        )
     elif args.command == "token":
-        if args.token is None:
-            print(get_token(verbose=True))
-        else:
+        if args.token:
             set_token(args.token)
-    elif args.command == "help":
-        if args.topic is None:
-            parser.print_help()
         else:
+            print(get_token(verbose=True))
+    elif args.command == "help":
+        if args.topic:
             commands[args.topic].print_help()
+        else:
+            parser.print_help()
     elif args.command is None:
         parser.print_help()
```

### Comparing `psbs-0.0.9/psbs/psparser.py` & `psbs-0.1.0/psbs/psparser.py`

 * *Files identical despite different names*

### Comparing `psbs-0.0.9/psbs/template.py` & `psbs-0.1.0/psbs/template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from os import path
 import traceback
 
 import jinja2
-from .images import image_to_object
+from .extensionloader import get_extensions
 
 
-def render_template(filename):
+def render_template(filename, config):
     directory = path.dirname(filename)
     file = path.basename(filename)
     jinja_env = jinja2.Environment(
         loader=jinja2.FileSystemLoader(directory),
         autoescape=False,
         block_start_string="(%",
         block_end_string="%)",
         variable_start_string="((",
         variable_end_string="))",
         comment_start_string="(#",
         comment_end_string="#)",
     )
-
-    jinja_env.globals.update(image=image_to_object)
+    extensions = get_extensions()
+    for extension in extensions:
+        if extension.__name__ not in config:
+            config[extension.__name__] = {}
+        ext_object = extension(config[extension.__name__])
+        for func_name, function in ext_object.methods.items():
+            jinja_env.globals[func_name] = function
 
     try:
         template = jinja_env.get_template(file)
         return template.render()
     except jinja2.exceptions.TemplateNotFound as err:
         print(f"Error: Unable to find template '{err}'")
         raise SystemExit(1) from err
```

### Comparing `psbs-0.0.9/psbs/templatebuilder.py` & `psbs-0.1.0/psbs/templatebuilder.py`

 * *Files identical despite different names*

### Comparing `psbs-0.0.9/psbs/token.py` & `psbs-0.1.0/psbs/token.py`

 * *Files identical despite different names*

### Comparing `psbs-0.0.9/psbs/utils.py` & `psbs-0.1.0/psbs/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         raise SystemExit(1) from err
     return output
 
 
 def write_yaml(filename, data):
     try:
         with open(filename, "w", encoding="UTF-8") as file:
-            yaml.dump(data, file)
+            yaml.safe_dump(data, file, sort_keys=False)
     except IOError as err:
         print(f"Error: Unable to write file {filename}\n  {err}")
         raise SystemExit(1) from err
 
 
 def make_dir(filename):
     try:
```

### Comparing `psbs-0.0.9/psbs.egg-info/PKG-INFO` & `psbs-0.1.0/psbs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.0.9
+Version: 0.1.0
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.0.9.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.0.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
-Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.8
@@ -37,37 +36,42 @@
  - Supports most PuzzleScript forks including [Pattern:Script](https://github.com/ClementSparrow/Pattern-Script)
  - Use your favorite version control for your PuzzleScript Projects
 
 ## Installing
 
 If you already have Python 3.8 or greater and pip installed simply run the following command from your terminal
 
-`pip install 'psbs @ git+https://github.com/jcmiller11/PSBS'`
+`pip install psbs`
 
 If you don't have Python and pip installed: [Download Python](https://www.python.org/downloads/)
 
 ## Connecting to GitHub
 
 PSBS will build your projects into PuzzleScript source without interacting with GitHub at all, however uploading and running your projects requires an authorization token.
 
 By default PSBS will attempt to run `gh auth token` to recieve an authorization token from the GitHub command line tool.  If you would like to use a different token or prefer not to install the GitHub command line tool you can run the following command.
 
-`psbs token insert your token here`
+`psbs token `*`insert_your_token_here`*
 
 ## Usage
 
 Enter `psbs` into your terminal to get a list of commands
 
 Commands:
 
 `psbs new` Creates a new project
+
 `psbs build` Builds the project in the current working directory
+
 `psbs upload` Builds project then uploads it to gist
+
 `psbs run` Builds project, uploads it, then runs it in your web browser
 
+`psbs token` Check or set the GitHub auth token
+
 For more information on these commands and to see available flags enter `psbs help `*`command`*
 
 ## CLI Example
 
     psbs new myProject
     cd myProject
     psbs build
@@ -95,17 +99,24 @@
         └── wincondition.pss
 
 
 ## Config.yaml
 
 At the root of your project you will find a file called config.yaml containing configuration variables for your project
 
-- engine: the url of the fork you are using, by default https://www.puzzlescript.net/
 - gist_id: the id of the gist the upload and run commands should use to store this project in
-- template: the name of your root template file, by default main.pss
+- engine: the url of the fork you are using, by default https://www.puzzlescript.net/
+- template: the name of your root template file, by default main.pssengine: https://auroriax.github.io/PuzzleScript/
+
+Below these are optional config variables for template extensions
+
+- Images:
+  - alpha: whether to include the RGBA alpha values for transparency supported by some forks
+  - max_colors: maximum colors in output object, PuzzleScript can only handle 10 by default but some forks support up to 36 colors
+
 
 ## Templates
 
 PSBS uses Jinja2, a fast, expressive, extensible templating engine, to build your PuzzleScript project.  To learn more about all of the features available to you check out the Jinja2 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
 To avoid conflicting with valid PuzzleScript code, the Jinja2 Tags have been changed as follows:
 
@@ -116,16 +127,14 @@
 A helper function has been added to the template environment `Image(filename)` that will import an image file directly into your game as a PuzzleScript object!
 
     Target
     ((image("images/target.png")))
 
 Additionally, this helper function contains the following optional parameters (alpha=False, max_colors=10, x=0, y=0, width=None, height=None)
 
-- alpha: (true/false) if true will include the RGBA alpha values for transparency supported by some forks
-- max_colors: (int) maximum colors in output object, PuzzleScript can only handle 10 by default but some forks such as Pattern:Script support up to 36 colors
 - x: (int) horizontal position in image to start importing from
 - y: (int) vertical position in image to start importing from
 - width: (int) width of the object to import, if None set to the width of the image file
 - height: (int) height of the object to import, if None set to the height of the image file
 
 By using the last four parameters listed one can load objects from a single image as a spritesheet.
```

### Comparing `psbs-0.0.9/setup.py` & `psbs-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 from pathlib import Path
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='psbs',
-    version='0.0.9',
+    version='0.1.0',
     python_requires='>=3.8',
     description='PuzzleScript Build System',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='J.C. Miller',
     author_email='johncoreymiller@gmail.com',
     url='https://github.com/jcmiller11/PSBS',
-    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.0.9.tar.gz',
+    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.0.tar.gz',
     license='MIT',
-    packages=['psbs'],
+    packages=find_packages(),
     package_data={'': ['example.txt']},
     include_package_data=True,
     install_requires=[
         'jinja2',
         'pyyaml',
         'Pillow',
         'platformdirs'
     ],
 
     classifiers=[
-        'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Topic :: Games/Entertainment :: Puzzle Games',
         'Topic :: Software Development :: Build Tools'
     ],
```

