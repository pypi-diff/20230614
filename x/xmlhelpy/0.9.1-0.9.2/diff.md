# Comparing `tmp/xmlhelpy-0.9.1-py3-none-any.whl.zip` & `tmp/xmlhelpy-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 18887 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1111 b- defN 21-Sep-17 18:28 xmlhelpy/__init__.py
--rw-r--r--  2.0 unx    10275 b- defN 21-Dec-01 08:58 xmlhelpy/core.py
--rw-r--r--  2.0 unx    11237 b- defN 21-Nov-18 09:15 xmlhelpy/decorators.py
--rw-r--r--  2.0 unx     2502 b- defN 21-Nov-18 09:15 xmlhelpy/formatting.py
--rw-r--r--  2.0 unx     7925 b- defN 21-Nov-18 09:15 xmlhelpy/types.py
--rw-r--r--  2.0 unx      621 b- defN 21-Dec-01 09:05 xmlhelpy/version.py
--rw-r--r--  2.0 unx    11358 b- defN 21-Dec-01 09:20 xmlhelpy-0.9.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     9538 b- defN 21-Dec-01 09:20 xmlhelpy-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-01 09:20 xmlhelpy-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 21-Dec-01 09:20 xmlhelpy-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      850 b- defN 21-Dec-01 09:20 xmlhelpy-0.9.1.dist-info/RECORD
-11 files, 55518 bytes uncompressed, 17469 bytes compressed:  68.5%
+Zip file size: 19268 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1111 b- defN 22-Feb-04 11:25 xmlhelpy/__init__.py
+-rw-r--r--  2.0 unx    10275 b- defN 22-Feb-04 11:25 xmlhelpy/core.py
+-rw-r--r--  2.0 unx    11237 b- defN 22-Feb-04 11:25 xmlhelpy/decorators.py
+-rw-r--r--  2.0 unx     2502 b- defN 22-Feb-04 11:25 xmlhelpy/formatting.py
+-rw-r--r--  2.0 unx     7925 b- defN 22-Feb-04 11:25 xmlhelpy/types.py
+-rw-r--r--  2.0 unx      621 b- defN 22-Feb-04 11:25 xmlhelpy/version.py
+-rw-rw-rw-  2.0 unx      270 b- defN 22-Feb-04 11:25 xmlhelpy-0.9.2.dist-info/AUTHORS.md
+-rw-rw-rw-  2.0 unx    11358 b- defN 22-Feb-04 11:25 xmlhelpy-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9562 b- defN 22-Feb-04 11:25 xmlhelpy-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Feb-04 11:25 xmlhelpy-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 22-Feb-04 11:25 xmlhelpy-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      941 b- defN 22-Feb-04 11:25 xmlhelpy-0.9.2.dist-info/RECORD
+12 files, 55903 bytes uncompressed, 17704 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -12,23 +12,26 @@
 
 Filename: xmlhelpy/types.py
 Comment: 
 
 Filename: xmlhelpy/version.py
 Comment: 
 
-Filename: xmlhelpy-0.9.1.dist-info/LICENSE
+Filename: xmlhelpy-0.9.2.dist-info/AUTHORS.md
 Comment: 
 
-Filename: xmlhelpy-0.9.1.dist-info/METADATA
+Filename: xmlhelpy-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: xmlhelpy-0.9.1.dist-info/WHEEL
+Filename: xmlhelpy-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: xmlhelpy-0.9.1.dist-info/top_level.txt
+Filename: xmlhelpy-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: xmlhelpy-0.9.1.dist-info/RECORD
+Filename: xmlhelpy-0.9.2.dist-info/top_level.txt
+Comment: 
+
+Filename: xmlhelpy-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xmlhelpy/version.py

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

## Comparing `xmlhelpy-0.9.1.dist-info/LICENSE` & `xmlhelpy-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xmlhelpy-0.9.1.dist-info/METADATA` & `xmlhelpy-0.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: xmlhelpy
-Version: 0.9.1
+Version: 0.9.2
 Summary: CLI wrapper for the xmlhelp interface.
 Home-page: https://gitlab.com/iam-cms/workflows/xmlhelpy
 Author: Karlsruhe Institute of Technology
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: AUTHORS.md
 Requires-Dist: click (<9.0.0,>=7.0.0)
 Requires-Dist: lxml (<5.0.0)
 Provides-Extra: dev
-Requires-Dist: black (==21.11b1) ; extra == 'dev'
+Requires-Dist: black (==22.1.0) ; extra == 'dev'
 Requires-Dist: build (<1.0.0) ; extra == 'dev'
 Requires-Dist: pre-commit (<3.0.0) ; extra == 'dev'
-Requires-Dist: pylint (<2.12.0) ; extra == 'dev'
+Requires-Dist: pylint (<2.13.0) ; extra == 'dev'
 Requires-Dist: pytest (<7.0.0) ; extra == 'dev'
 Requires-Dist: tox (<4.0.0) ; extra == 'dev'
 Requires-Dist: twine (<4.0.0) ; extra == 'dev'
 
 # xmlhelpy
 
 **xmlhelpy** is a wrapper library based on
```

## Comparing `xmlhelpy-0.9.1.dist-info/RECORD` & `xmlhelpy-0.9.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 xmlhelpy/__init__.py,sha256=WN7NCtUapRenbuZnWJo8GQPWcjpAVAhz4yY1ew32B1o,1111
 xmlhelpy/core.py,sha256=hizIlEBteaW1Vbbt1UfTknRRw07N8-c6-UqXaIvQcxM,10275
 xmlhelpy/decorators.py,sha256=uccTGEedbepq-P9ZdRTv3SV4B2EPjKL2zW2VHUu23T4,11237
 xmlhelpy/formatting.py,sha256=z5WSjNge8effMbo1Ll-Dvwg9lz59MJPrUzqf7-G0U3w,2502
 xmlhelpy/types.py,sha256=m2r0cFvTyF2YF5lPnAooGkgk_R11zlC-nP5A2XdoyPM,7925
-xmlhelpy/version.py,sha256=oo2TQE4ZQzf1HaD_F4oLpnL1ePQnjedPS23AKRMEjQE,621
-xmlhelpy-0.9.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-xmlhelpy-0.9.1.dist-info/METADATA,sha256=zC-KrGIqV9VHX7qfrOOpI8EshSiLdDGVpVEokyBH3BY,9538
-xmlhelpy-0.9.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-xmlhelpy-0.9.1.dist-info/top_level.txt,sha256=lLM0gegxJ4pjetNVrZKgyT60X7c7szF_4sdcADlPD6s,9
-xmlhelpy-0.9.1.dist-info/RECORD,,
+xmlhelpy/version.py,sha256=KB71exxrJTOeYqsElx-jZtkM__7_EsIi10LwmH0OEX0,621
+xmlhelpy-0.9.2.dist-info/AUTHORS.md,sha256=WB6jxk0ds_W89Imteny3Q0FnElMGI6c6W3P_oDh7OZ8,270
+xmlhelpy-0.9.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+xmlhelpy-0.9.2.dist-info/METADATA,sha256=hsaEfPApDolyKuP2hFgrMcaS4bhk-4OZrERIOdqEXy0,9562
+xmlhelpy-0.9.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xmlhelpy-0.9.2.dist-info/top_level.txt,sha256=lLM0gegxJ4pjetNVrZKgyT60X7c7szF_4sdcADlPD6s,9
+xmlhelpy-0.9.2.dist-info/RECORD,,
```

