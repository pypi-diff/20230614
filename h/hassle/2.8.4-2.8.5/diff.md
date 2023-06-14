# Comparing `tmp/hassle-2.8.4.tar.gz` & `tmp/hassle-2.8.5.tar.gz`

## Comparing `hassle-2.8.4.tar` & `hassle-2.8.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 hassle-2.8.4/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/index.html
--rw-r--r--   0        0        0    45086 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/search.js
--rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   139420 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/new_project.html
--rw-r--r--   0        0        0    54156 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     8266 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/new_project.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.4/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.4/README.md
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.4/pyproject.toml
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.4/PKG-INFO
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 hassle-2.8.5/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/index.html
+-rw-r--r--   0        0        0    45086 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/search.js
+-rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   139468 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    54156 2020-02-02 00:00:00.000000 hassle-2.8.5/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/new_project.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 hassle-2.8.5/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.5/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.5/README.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.5/pyproject.toml
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.5/PKG-INFO
```

### Comparing `hassle-2.8.4/CHANGELOG.md` & `hassle-2.8.5/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 # Changelog
 
-## 2.8.3 (2023-05-10)
+## 2.8.4 (2023-05-12)
+
+#### Fixes
+
+* run_tests() returns True if no tests are found
+
+
+## v2.8.3 (2023-05-10)
 
 #### Fixes
 
 * fix bug where the package would get built before the version was incremented
 #### Others
 
+* build v2.8.3
+* update changelog
 * build v2.8.2
 
 
 ## v2.8.2 (2023-05-10)
 
 #### Fixes
 
@@ -42,16 +51,16 @@
 #### Fixes
 
 * catch Black.main()'s SystemExit
 * fix Pathier.mkcwd() usage
 * invoke build with sys.executable instead of py
 #### Refactorings
 
-* replace os.system call to git with gitbetter.git methods
 * replace os.system calls for black and isort with direct invocations
+* replace os.system calls for git functions with gitbetter.git methods
 * extract build process into it's own function
 * make run_tests() invoke pytest and coverage directly and return pytest result
 #### Others
 
 * build v2.8.0
 * update changelog
 * remove unused import
```

### Comparing `hassle-2.8.4/docs/hassle.html` & `hassle-2.8.5/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/docs/search.js` & `hassle-2.8.5/docs/search.js`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/docs/hassle/generate_tests.html` & `hassle-2.8.5/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/docs/hassle/hassle.html` & `hassle-2.8.5/docs/hassle/hassle.html`

 * *Files 0% similar despite different names*

```diff
@@ -324,16 +324,16 @@
 </span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
 </span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
 </span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
 </span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="si">}</span><span class="s2"> -m pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span>
 </span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="p">)</span>
 </span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
 </span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;origin main --tags&quot;</span><span class="p">)</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;origin main --tags&quot;</span><span class="p">)</span>
 </span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
 </span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
 </span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
 </span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
@@ -644,16 +644,16 @@
 </span><span id="main-263"><a href="#main-263"><span class="linenos">263</span></a>
 </span><span id="main-264"><a href="#main-264"><span class="linenos">264</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
 </span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
 </span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="si">}</span><span class="s2"> -m pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span>
 </span><span id="main-267"><a href="#main-267"><span class="linenos">267</span></a>        <span class="p">)</span>
 </span><span id="main-268"><a href="#main-268"><span class="linenos">268</span></a>
 </span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="main-270"><a href="#main-270"><span class="linenos">270</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
-</span><span id="main-271"><a href="#main-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="main-270"><a href="#main-270"><span class="linenos">270</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;origin main --tags&quot;</span><span class="p">)</span>
+</span><span id="main-271"><a href="#main-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;origin main --tags&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -285,16 +285,16 @@
 263    if args.install:
 264        os.system(
 265            f"{sys.executable} -m pip install {args.package} --no-deps --
 upgrade --no-cache-dir"
 266        )
 267
 268    if args.sync:
-269        git.pull("--tags")
-270        git.push("--tags")
+269        git.pull("origin main --tags")
+270        git.push("origin main --tags")
 271
 272
 273if __name__ == "__main__":
 274    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
 _17def get_args() -> argparse.Namespace:
@@ -572,10 +572,10 @@
 264    if args.install:
 265        os.system(
 266            f"{sys.executable} -m pip install {args.package} --no-deps --
 upgrade --no-cache-dir"
 267        )
 268
 269    if args.sync:
-270        git.pull("--tags")
-271        git.push("--tags")
+270        git.pull("origin main --tags")
+271        git.push("origin main --tags")
```

### Comparing `hassle-2.8.4/docs/hassle/hassle_config.html` & `hassle-2.8.5/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/docs/hassle/hassle_utilities.html` & `hassle-2.8.5/docs/hassle/hassle_utilities.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/docs/hassle/new_project.html` & `hassle-2.8.5/docs/hassle/new_project.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/docs/hassle/run_tests.html` & `hassle-2.8.5/docs/hassle/run_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/src/hassle/generate_tests.py` & `hassle-2.8.5/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/src/hassle/hassle.py` & `hassle-2.8.5/src/hassle/hassle.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,13 +262,13 @@
 
     if args.install:
         os.system(
             f"{sys.executable} -m pip install {args.package} --no-deps --upgrade --no-cache-dir"
         )
 
     if args.sync:
-        git.pull("--tags")
-        git.push("--tags")
+        git.pull("origin main --tags")
+        git.push("origin main --tags")
 
 
 if __name__ == "__main__":
     main(get_args())
```

### Comparing `hassle-2.8.4/src/hassle/hassle_config.py` & `hassle-2.8.5/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/src/hassle/hassle_utilities.py` & `hassle-2.8.5/src/hassle/hassle_utilities.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/src/hassle/license_template.txt` & `hassle-2.8.5/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/src/hassle/new_project.py` & `hassle-2.8.5/src/hassle/new_project.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/src/hassle/pyproject_template.toml` & `hassle-2.8.5/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/src/hassle/run_tests.py` & `hassle-2.8.5/src/hassle/run_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/LICENSE.txt` & `hassle-2.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/README.md` & `hassle-2.8.5/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.8.4/pyproject.toml` & `hassle-2.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 382e 3422 0d0a 7265 7175 6972 6573  2.8.4"..requires
+00000100: 322e 382e 3522 0d0a 7265 7175 6972 6573  2.8.5"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..
```

### Comparing `hassle-2.8.4/PKG-INFO` & `hassle-2.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.8.4
+Version: 2.8.5
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

