# Comparing `tmp/pretext-1.6.1.dev20230613.tar.gz` & `tmp/pretext-1.6.1.dev20230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230613.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230614.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230613.tar` & `pretext-1.6.1.dev20230614.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-13 06:18:21.829306 pretext-1.6.1.dev20230613/LICENSE
--rw-r--r--   0        0        0     9757 2023-06-13 06:18:21.829306 pretext-1.6.1.dev20230613/README.md
--rw-r--r--   0        0        0     1901 2023-06-13 06:18:55.333512 pretext-1.6.1.dev20230613/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/__main__.py
--rw-r--r--   0        0        0     8170 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/build.py
--rw-r--r--   0        0        0    25351 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-13 06:19:00.437544 pretext-1.6.1.dev20230613/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/core/resources.py
--rw-r--r--   0        0        0  1034865 2023-06-13 06:19:00.437544 pretext-1.6.1.dev20230613/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/generate.py
--rw-r--r--   0        0        0    27475 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/project.py
--rw-r--r--   0        0        0      516 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-13 06:19:00.521544 pretext-1.6.1.dev20230613/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-13 06:19:00.521544 pretext-1.6.1.dev20230613/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160064 2023-06-13 06:19:00.489544 pretext-1.6.1.dev20230613/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7570 2023-06-13 06:19:00.497544 pretext-1.6.1.dev20230613/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173263 2023-06-13 06:19:00.513544 pretext-1.6.1.dev20230613/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-06-13 06:19:00.521544 pretext-1.6.1.dev20230613/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4611 2023-06-13 06:19:00.517544 pretext-1.6.1.dev20230613/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-13 06:19:00.521544 pretext-1.6.1.dev20230613/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-13 06:19:00.521544 pretext-1.6.1.dev20230613/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8346 2023-06-13 06:19:00.521544 pretext-1.6.1.dev20230613/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18416 2023-06-13 06:18:21.833306 pretext-1.6.1.dev20230613/pretext/utils.py
--rw-r--r--   0        0        0     1143 2023-06-13 06:18:55.333512 pretext-1.6.1.dev20230613/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230613/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/README.md
+-rw-r--r--   0        0        0     1901 2023-06-14 06:19:41.464059 pretext-1.6.1.dev20230614/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/__main__.py
+-rw-r--r--   0        0        0     8170 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/build.py
+-rw-r--r--   0        0        0    25351 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-14 06:19:46.556099 pretext-1.6.1.dev20230614/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/core/resources.py
+-rw-r--r--   0        0        0  1035294 2023-06-14 06:19:46.552099 pretext-1.6.1.dev20230614/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/generate.py
+-rw-r--r--   0        0        0    27475 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160064 2023-06-14 06:19:46.600100 pretext-1.6.1.dev20230614/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7570 2023-06-14 06:19:46.604100 pretext-1.6.1.dev20230614/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173263 2023-06-14 06:19:46.616100 pretext-1.6.1.dev20230614/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4611 2023-06-14 06:19:46.620100 pretext-1.6.1.dev20230614/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8346 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18416 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/utils.py
+-rw-r--r--   0        0        0     1143 2023-06-14 06:19:41.464059 pretext-1.6.1.dev20230614/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230614/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230613/LICENSE` & `pretext-1.6.1.dev20230614/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/README.md` & `pretext-1.6.1.dev20230614/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/__init__.py` & `pretext-1.6.1.dev20230614/pretext/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = 'c90ba4bee68ab6fd4ba41d4831f2bfea13838fb7'
+CORE_COMMIT = 'dff67ac239d84354138b15cf6a729200f606ea94'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230613/pretext/build.py` & `pretext-1.6.1.dev20230614/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/cli.py` & `pretext-1.6.1.dev20230614/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/codechat.py` & `pretext-1.6.1.dev20230614/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230614/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/core/pretext.py` & `pretext-1.6.1.dev20230614/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/core/resources.py` & `pretext-1.6.1.dev20230614/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/core/resources.zip` & `pretext-1.6.1.dev20230614/pretext/core/resources.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,143 +1,143 @@
-Zip file size: 1034865 bytes, number of entries: 141
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 xsl/utilities/
--rw-r--r--  2.0 unx   231248 b- defN 23-Jun-13 06:19 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   611196 b- defN 23-Jun-13 06:19 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-13 06:19 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-13 06:19 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-13 06:19 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-13 06:19 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-13 06:19 xsl/entities.ent
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-13 06:19 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-13 06:19 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-13 06:19 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-13 06:19 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-13 06:19 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-13 06:19 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-13 06:19 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   111931 b- defN 23-Jun-13 06:19 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-13 06:19 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-13 06:19 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-13 06:19 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-13 06:19 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-13 06:19 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-13 06:19 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-13 06:19 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-13 06:19 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-13 06:19 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-13 06:19 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-13 06:19 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-13 06:19 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx   106649 b- defN 23-Jun-13 06:19 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-13 06:19 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-13 06:19 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-13 06:19 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-13 06:19 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-13 06:19 xsl/README.md
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-13 06:19 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-13 06:19 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-13 06:19 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-13 06:19 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-13 06:19 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-13 06:19 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-13 06:19 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-13 06:19 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-13 06:19 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-13 06:19 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-13 06:19 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-13 06:19 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 xsl/support/play-button/
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-13 06:19 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-13 06:19 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-13 06:19 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-13 06:19 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-13 06:19 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-13 06:19 xsl/support/README.md
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-13 06:19 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-13 06:19 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-13 06:19 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-13 06:19 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-13 06:19 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-13 06:19 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-13 06:19 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-13 06:19 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-13 06:19 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-13 06:19 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-13 06:19 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-13 06:19 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-13 06:19 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-13 06:19 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-13 06:19 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-13 06:19 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-13 06:19 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-13 06:19 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-13 06:19 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-13 06:19 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-13 06:19 xsl/localizations/README.md
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-13 06:19 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-13 06:19 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-13 06:19 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-13 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-13 06:19 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-13 06:18 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-13 06:18 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-13 06:18 css/kindle.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-13 06:18 css/update_css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-13 06:18 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-13 06:18 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-13 06:18 css/colors_default.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-13 06:18 css/colors_red_blue.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-13 06:18 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-13 06:18 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-13 06:18 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-13 06:18 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-13 06:18 css/colors_blue_green.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-13 06:18 css/mathbook-content.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-13 06:18 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-13 06:18 css/pretext.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-13 06:18 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-13 06:18 css/epub.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-13 06:18 css/mathbook-add-on.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-13 06:18 css/setcolors.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-13 06:18 css/pretext_add_on.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-13 06:18 css/mathbook-3.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-13 06:18 css/colors_green_plum.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-13 06:18 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-13 06:18 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-13 06:18 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-13 06:18 css/README.md
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-13 06:18 css/style_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-13 06:18 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-13 06:19 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 06:19 pretext/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-13 06:19 pretext/pretext.cfg
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-13 06:19 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-13 06:19 pretext/module-test.py
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-13 06:19 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-13 06:19 pretext/README.md
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-13 06:19 schema/xml.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-13 06:19 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-13 06:19 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-13 06:19 schema/pretext.xml
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-13 06:19 schema/pretext.rnc
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-13 06:19 schema/pretext.rng
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-13 06:19 schema/pretext-dev.rng
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-13 06:19 schema/build.sh
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-13 06:19 schema/pretext.xsd
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-13 06:19 schema/README.md
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-13 06:19 schema/pretext-validation-plus.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 script/mjsre/
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-13 06:19 script/mbx
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-13 06:19 script/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 06:19 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-13 06:19 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-13 06:19 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-13 06:19 script/mjsre/mj-sre-page.js
-141 files, 4810376 bytes uncompressed, 1017423 bytes compressed:  78.9%
+Zip file size: 1035294 bytes, number of entries: 141
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/utilities/
+-rw-r--r--  2.0 unx   231248 b- defN 23-Jun-14 06:19 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   611581 b- defN 23-Jun-14 06:19 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-14 06:19 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-14 06:19 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-14 06:19 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-14 06:19 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-14 06:19 xsl/entities.ent
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-14 06:19 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-14 06:19 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-14 06:19 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-14 06:19 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-14 06:19 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-14 06:19 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-14 06:19 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jun-14 06:19 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-14 06:19 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-14 06:19 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-14 06:19 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-14 06:19 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-14 06:19 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-14 06:19 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-14 06:19 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-14 06:19 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-14 06:19 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-14 06:19 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-14 06:19 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-14 06:19 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx   109017 b- defN 23-Jun-14 06:19 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-14 06:19 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-14 06:19 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-14 06:19 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-14 06:19 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-14 06:19 xsl/README.md
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-14 06:19 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-14 06:19 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-14 06:19 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-14 06:19 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-14 06:19 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-14 06:19 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-14 06:19 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-14 06:19 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-14 06:19 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-14 06:19 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-14 06:19 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-14 06:19 xsl/utilities/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/support/play-button/
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-14 06:19 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-14 06:19 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-14 06:19 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-14 06:19 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-14 06:19 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-14 06:19 xsl/support/README.md
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-14 06:19 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-14 06:19 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-14 06:19 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-14 06:19 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-14 06:19 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-14 06:19 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-14 06:19 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-14 06:19 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-14 06:19 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-14 06:19 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-14 06:19 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-14 06:19 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-14 06:19 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-14 06:19 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-14 06:19 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-14 06:19 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-14 06:19 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-14 06:19 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-14 06:19 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-14 06:19 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-14 06:19 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-14 06:19 css/kindle.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-14 06:19 css/update_css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-14 06:19 css/colors_default.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-14 06:19 css/colors_red_blue.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-14 06:19 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-14 06:19 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-14 06:19 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-14 06:19 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-14 06:19 css/colors_blue_green.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-14 06:19 css/mathbook-content.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-14 06:19 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-14 06:19 css/pretext.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-14 06:19 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-14 06:19 css/epub.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-14 06:19 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-14 06:19 css/setcolors.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-14 06:19 css/pretext_add_on.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-14 06:19 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_green_plum.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-14 06:19 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-14 06:19 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-14 06:19 css/README.md
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-14 06:19 css/style_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-14 06:19 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 06:19 pretext/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-14 06:19 pretext/pretext.cfg
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-14 06:19 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-14 06:19 pretext/module-test.py
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-14 06:19 pretext/pretext.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-14 06:19 pretext/README.md
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-14 06:19 schema/xml.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-14 06:19 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-14 06:19 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-14 06:19 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-14 06:19 schema/pretext.rnc
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-14 06:19 schema/pretext.rng
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-14 06:19 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-14 06:19 schema/build.sh
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-14 06:19 schema/pretext.xsd
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-14 06:19 schema/README.md
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-14 06:19 schema/pretext-validation-plus.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 script/mjsre/
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-14 06:19 script/mbx
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-14 06:19 script/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 06:19 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-14 06:19 script/mjsre/package.json
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-14 06:19 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-14 06:19 script/mjsre/mj-sre-page.js
+141 files, 4813648 bytes uncompressed, 1017852 bytes compressed:  78.9%
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -4464,14 +4464,21 @@
     <xsl:param name="b-has-solution"/>
     <xsl:choose>
       <!-- signal on intentional, temporary, hack      -->
       <!-- simply duplicated in assembly, no solutions -->
       <xsl:when test="@exercise-interactive = 'htmlhack'">
         <xsl:apply-templates select="." mode="runestone-to-interactive"/>
       </xsl:when>
+      <!-- Select -->
+      <!-- Largely a Runestone/database operation referencing -->
+      <!-- existing questions supplied by the manifest,       -->
+      <!-- so we go straight to an HTML version               -->
+      <xsl:when test="@exercise-interactive = 'select'">
+        <xsl:apply-templates select="." mode="runestone-to-interactive"/>
+      </xsl:when>
       <!-- True/False        -->
       <!-- Multiple Choice   -->
       <!-- Parson problems   -->
       <!-- Matching problems -->
       <!-- Clickable Area    -->
       <!-- Fill-In (Basic)   -->
       <!-- Coding Exercise   -->
```

#### xsl/pretext-assembly.xsl

##### xsl/pretext-assembly.xsl

```diff
@@ -1562,14 +1562,17 @@
         </xsl:when>
         <xsl:when test="statement and matches">
           <xsl:text>matching</xsl:text>
         </xsl:when>
         <xsl:when test="statement and areas">
           <xsl:text>clickablearea</xsl:text>
         </xsl:when>
+        <xsl:when test="select">
+          <xsl:text>select</xsl:text>
+        </xsl:when>
         <!-- noted WeBWork earlier, so this is Runestone fillin -->
         <xsl:when test="statement//var">
           <xsl:text>fillin-basic</xsl:text>
         </xsl:when>
         <!-- new dynamic fillin goes here, perhaps:                     -->
         <!-- statement//fillin[(@*|node()) and not(@characters|@fill)]? -->
         <!-- only interactive programs make sense after a "statement" -->
@@ -1637,15 +1640,15 @@
   <!-- Parson problems   -->
   <!-- Matching problems -->
   <!-- Clickable Area    -->
   <!-- ActiveCode        -->
   <!-- TODO: definitely need better filters -->
   <!-- complement (not()), single attribute -->
   <!-- Also in Runestone manifest creation  -->
-  <xsl:template match="exercise[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                       |                       project[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                      activity[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                   exploration[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                 investigation[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                          task[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]" mode="representations">
+  <xsl:template match="exercise[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                       |                       project[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                      activity[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                   exploration[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                 investigation[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                          task[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]" mode="representations">
     <!-- always preserve "exercise/project" container here, with attributes -->
     <xsl:copy>
       <xsl:apply-templates select="@*" mode="representations"/>
       <xsl:choose>
         <!-- make a static version, in a PreTeXt   -->
         <!-- statement|hint|answer|solution style  -->
         <!-- for use naturally by most conversions -->
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -666,15 +666,15 @@
   <!--   - every horizontal Parsons problem "exercise"  -->
   <!--   - every matching problem "exercise"            -->
   <!--   - every clickable area problem "exercise"      -->
   <!--   - every "exercise" with fill-in blanks         -->
   <!--   - every "exercise" with additional "program"   -->
   <!--   - every "exercise" elected as "shortanswer"    -->
   <!--   - every PROJECT-LIKE with additional "program" -->
-  <xsl:template match="exercise[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                       |                       project[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                      activity[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                   exploration[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                 investigation[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                          task[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]" mode="runestone-manifest">
+  <xsl:template match="exercise[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                       |                       project[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                      activity[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                   exploration[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                 investigation[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]                      |                          task[ (@exercise-interactive = 'truefalse') or                                (@exercise-interactive = 'multiplechoice') or                                (@exercise-interactive = 'parson') or                                (@exercise-interactive = 'parson-horizontal') or                                (@exercise-interactive = 'matching') or                                (@exercise-interactive = 'clickablearea') or                                (@exercise-interactive = 'select') or                                (@exercise-interactive = 'fillin-basic') or                                (@exercise-interactive = 'coding') or                                (@exercise-interactive = 'shortanswer')]" mode="runestone-manifest">
     <question>
       <!-- label is from the "exercise" -->
       <xsl:apply-templates select="." mode="runestone-manifest-label"/>
       <!-- Duplicate, but still should look like original (ID, etc.),  -->
       <!-- not knowled. Solutions are available in the originals, via  -->
       <!-- an "in context" link off the Assignment page                -->
       <htmlsrc>
@@ -1355,14 +1355,50 @@
         <xsl:otherwise>
           <xsl:attribute name="data-correct"/>
         </xsl:otherwise>
       </xsl:choose>
       <xsl:apply-templates/>
     </span>
   </xsl:template>
+  <!-- Select Questions -->
+  <!-- "Select" questions come in three types                            -->
+  <!--   * Question List - several equivalent problems,                  -->
+  <!--     reader is assigned just one (good for exams)                  -->
+  <!--   * A/B Experiment - two choices, experiment managed by Runestone -->
+  <xsl:template match="*[@exercise-interactive = 'select']" mode="runestone-to-interactive">
+    <div class="runestone sqcontainer">
+      <div data-component="selectquestion" data-points="1" data-limit-basecourse="false">
+        <xsl:attribute name="id">
+          <xsl:apply-templates select="." mode="runestone-id"/>
+        </xsl:attribute>
+        <!-- condition on an attribute of the "select" element -->
+        <xsl:choose>
+          <xsl:when test="select/@questions">
+            <xsl:attribute name="data-questionlist">
+              <xsl:apply-templates select="select/@questions" mode="runestone-targets">
+                <xsl:with-param name="separator" select="', '"/>
+              </xsl:apply-templates>
+            </xsl:attribute>
+            <p>Loading a dynamic question-list question...</p>
+          </xsl:when>
+          <xsl:when test="select/@ab-experiment">
+            <xsl:attribute name="data-ab">
+              <xsl:value-of select="select/@experiment-name"/>
+            </xsl:attribute>
+            <xsl:attribute name="data-questionlist">
+              <xsl:apply-templates select="select/@ab-experiment" mode="runestone-targets">
+                <xsl:with-param name="separator" select="', '"/>
+              </xsl:apply-templates>
+            </xsl:attribute>
+            <p>Loading a dynamic A/B question...</p>
+          </xsl:when>
+        </xsl:choose>
+      </div>
+    </div>
+  </xsl:template>
   <!-- Fill-in-the-Blanks problem -->
   <!-- Runestone structure -->
   <xsl:template match="*[@exercise-interactive = 'fillin-basic']" mode="runestone-to-interactive">
     <div class="ptx-runestone-container">
       <div class="runestone">
         <!-- dropped "visibility: hidden" on next div -->
         <div data-component="fillintheblank" data-question_label="">
```

### Comparing `pretext-1.6.1.dev20230613/pretext/generate.py` & `pretext-1.6.1.dev20230614/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/project.py` & `pretext-1.6.1.dev20230614/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230614/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230614/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230614/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160064 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-13 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-13 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-13 06:19 project.ptx
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-13 06:18 README.md
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-13 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-13 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-13 06:18 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-13 06:18 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-13 06:18 source/section-2.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-13 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-14 06:19 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-14 06:19 README.md
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-14 06:19 assets/frog.jpg
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-14 06:19 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-14 06:19 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-14 06:19 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-14 06:19 source/section-2.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
 14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
```

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230614/pretext/templates/resources/book.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7570 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-13 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-13 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-13 06:19 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-13 06:18 README.md
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-13 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-13 06:18 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-13 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-14 06:19 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-14 06:19 README.md
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-14 06:19 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-14 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
 10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230614/pretext/templates/resources/demo.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173263 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-13 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-13 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-13 06:19 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-13 06:18 README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-13 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-13 06:18 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-13 06:18 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 source/images/
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-13 06:18 source/sec-features.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-13 06:18 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-13 06:18 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-13 06:18 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-13 06:18 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-13 06:18 source/main.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-13 06:18 source/ch-generate.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-13 06:18 source/backmatter.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-13 06:18 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-13 06:18 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-13 06:18 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-13 06:18 source/ch-features.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-13 06:18 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-13 06:18 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-13 06:18 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-13 06:18 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-13 06:18 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-13 06:18 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-13 06:18 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-13 06:18 source/images/cflag.asy
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-13 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-14 06:19 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-14 06:19 README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-14 06:19 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-14 06:19 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-14 06:19 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/images/
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-14 06:19 source/sec-features.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-14 06:19 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-14 06:19 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-14 06:19 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-14 06:19 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-14 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-14 06:19 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-14 06:19 source/backmatter.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-14 06:19 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-14 06:19 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-14 06:19 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-14 06:19 source/ch-features.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-14 06:19 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-14 06:19 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-14 06:19 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-14 06:19 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-14 06:19 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-14 06:19 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-14 06:19 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-14 06:19 source/images/cflag.asy
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
 34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230614/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230614/pretext/templates/resources/hello.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4611 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-13 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-13 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-13 06:18 project.ptx
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-13 06:18 README.md
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-13 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-13 06:18 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-13 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-14 06:19 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-14 06:19 README.md
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-14 06:19 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-14 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
 10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
```

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230614/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230614/pretext/templates/resources/slideshow.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8346 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:18 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-13 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-13 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-13 06:18 project.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-13 06:18 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-13 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-13 06:18 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-13 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-14 06:19 project.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-14 06:19 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-14 06:19 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-14 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
 11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230613/pretext/utils.py` & `pretext-1.6.1.dev20230614/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230613/pyproject.toml` & `pretext-1.6.1.dev20230614/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230613"
+version = "1.6.1.dev20230614"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230613/PKG-INFO` & `pretext-1.6.1.dev20230614/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230613
+Version: 1.6.1.dev20230614
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

