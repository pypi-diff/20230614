# Comparing `tmp/pipen_report-0.8.0.tar.gz` & `tmp/pipen_report-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_report-0.8.0.tar", max compression
+gzip compressed data, was "pipen_report-0.9.0.tar", max compression
```

## Comparing `pipen_report-0.8.0.tar` & `pipen_report-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      783 2023-03-30 03:59:00.944538 pipen_report-0.8.0/README.md
--rw-r--r--   0        0        0       76 2023-03-30 03:59:00.952539 pipen_report-0.8.0/pipen_report/__init__.py
--rw-r--r--   0        0        0     7468 2023-03-30 03:59:00.952539 pipen_report-0.8.0/pipen_report/cli.py
--rw-r--r--   0        0        0      886 2023-03-30 03:59:00.952539 pipen_report-0.8.0/pipen_report/defaults.py
--rw-r--r--   0        0        0     1981 2023-03-30 03:59:00.952539 pipen_report-0.8.0/pipen_report/filters.py
--rw-r--r--   0        0        0       80 2023-03-30 03:59:00.952539 pipen_report-0.8.0/pipen_report/frontend/copier.yml
--rw-r--r--   0        0        0    53598 2023-03-30 03:59:00.952539 pipen_report-0.8.0/pipen_report/frontend/package-lock.json
--rw-r--r--   0        0        0      748 2023-03-30 03:59:00.952539 pipen_report-0.8.0/pipen_report/frontend/package.json
--rw-r--r--   0        0        0   754873 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/public/assets/ccs.css
--rw-r--r--   0        0        0     7369 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/public/assets/favicon.png
--rw-r--r--   0        0        0     2419 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/public/assets/global.css
--rw-r--r--   0        0        0        0 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/public/data/.keep
--rw-r--r--   0        0        0      428 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/public/index.html
--rw-r--r--   0        0        0     2665 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/rollup.config.js.jinja
--rw-r--r--   0        0        0     1042 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/DataTable/DataTable.svelte
--rw-r--r--   0        0        0     3889 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/DataTable/DataTableInner.svelte
--rw-r--r--   0        0        0       59 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/DataTable/index.js
--rw-r--r--   0        0        0      189 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/DataTable/paginate.js
--rw-r--r--   0        0        0      284 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/Image/Image.svelte
--rw-r--r--   0        0        0     3538 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/Image/ImageInner.svelte
--rw-r--r--   0        0        0       51 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/Image/index.js
--rw-r--r--   0        0        0     1344 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/PageNavButton.svelte
--rw-r--r--   0        0        0       74 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/components/index.js
--rw-r--r--   0        0        0      350 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/data.json
--rw-r--r--   0        0        0      177 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/layouts/Footer.svelte
--rw-r--r--   0        0        0     1469 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/layouts/Header.svelte
--rw-r--r--   0        0        0      332 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/layouts/Index.svelte
--rw-r--r--   0        0        0      247 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/layouts/ProcCard.svelte
--rw-r--r--   0        0        0      742 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/layouts/ProcLayout.svelte
--rw-r--r--   0        0        0     2068 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/layouts/ProcToc.svelte
--rw-r--r--   0        0        0      250 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/pages/_index/index.js
--rw-r--r--   0        0        0      822 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/pages/_index/index.svelte
--rw-r--r--   0        0        0      161 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/pages/proc/index.js.jinja
--rw-r--r--   0        0        0      801 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/pages/proc/index.svelte
--rw-r--r--   0        0        0       61 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/pages/proc/proc.svelte
--rw-r--r--   0        0        0        2 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/pages/proc/toc.json
--rw-r--r--   0        0        0     1181 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/frontend/src/proc.html
--rw-r--r--   0        0        0     6620 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/preprocess.py
--rw-r--r--   0        0        0    13378 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/report_manager.py
--rw-r--r--   0        0        0     4388 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/report_plugin.py
--rw-r--r--   0        0        0      295 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/utils.py
--rw-r--r--   0        0        0      387 2023-03-30 03:59:00.956539 pipen_report-0.8.0/pipen_report/versions.py
--rwxr-xr-x   0        0        0     1440 2023-03-30 03:59:00.960539 pipen_report-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 pipen_report-0.8.0/setup.py
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 pipen_report-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      783 2023-04-15 08:00:52.792220 pipen_report-0.9.0/README.md
+-rw-r--r--   0        0        0       76 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/__init__.py
+-rw-r--r--   0        0        0     7468 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/cli.py
+-rw-r--r--   0        0        0      886 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/defaults.py
+-rw-r--r--   0        0        0     1981 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/filters.py
+-rw-r--r--   0        0        0       80 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/copier.yml
+-rw-r--r--   0        0        0    53995 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/package-lock.json
+-rw-r--r--   0        0        0      748 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/package.json
+-rw-r--r--   0        0        0   754873 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/public/assets/ccs.css
+-rw-r--r--   0        0        0     7369 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/public/assets/favicon.png
+-rw-r--r--   0        0        0     2419 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/public/assets/global.css
+-rw-r--r--   0        0        0        0 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/public/data/.keep
+-rw-r--r--   0        0        0      428 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/public/index.html
+-rw-r--r--   0        0        0     2843 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/rollup.config.js.jinja
+-rw-r--r--   0        0        0     1042 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/DataTable/DataTable.svelte
+-rw-r--r--   0        0        0     3889 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/DataTable/DataTableInner.svelte
+-rw-r--r--   0        0        0       59 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/DataTable/index.js
+-rw-r--r--   0        0        0      189 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/DataTable/paginate.js
+-rw-r--r--   0        0        0      284 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/Image/Image.svelte
+-rw-r--r--   0        0        0     3538 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/Image/ImageInner.svelte
+-rw-r--r--   0        0        0       51 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/Image/index.js
+-rw-r--r--   0        0        0     1344 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/PageNavButton.svelte
+-rw-r--r--   0        0        0       74 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/components/index.js
+-rw-r--r--   0        0        0      350 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/data.json
+-rw-r--r--   0        0        0      177 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/layouts/Footer.svelte
+-rw-r--r--   0        0        0     1469 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/layouts/Header.svelte
+-rw-r--r--   0        0        0      332 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/layouts/Index.svelte
+-rw-r--r--   0        0        0      247 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/layouts/ProcCard.svelte
+-rw-r--r--   0        0        0      742 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/layouts/ProcLayout.svelte
+-rw-r--r--   0        0        0     2068 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/layouts/ProcToc.svelte
+-rw-r--r--   0        0        0      250 2023-04-15 08:00:52.800221 pipen_report-0.9.0/pipen_report/frontend/src/pages/_index/index.js
+-rw-r--r--   0        0        0      822 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/frontend/src/pages/_index/index.svelte
+-rw-r--r--   0        0        0      161 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/frontend/src/pages/proc/index.js.jinja
+-rw-r--r--   0        0        0      801 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/frontend/src/pages/proc/index.svelte
+-rw-r--r--   0        0        0       61 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/frontend/src/pages/proc/proc.svelte
+-rw-r--r--   0        0        0        2 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/frontend/src/pages/proc/toc.json
+-rw-r--r--   0        0        0     1181 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/frontend/src/proc.html
+-rw-r--r--   0        0        0     6625 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/preprocess.py
+-rw-r--r--   0        0        0    13418 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/report_manager.py
+-rw-r--r--   0        0        0     4388 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/report_plugin.py
+-rw-r--r--   0        0        0      295 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/utils.py
+-rw-r--r--   0        0        0      387 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pipen_report/versions.py
+-rwxr-xr-x   0        0        0     1490 2023-04-15 08:00:52.804221 pipen_report-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 pipen_report-0.9.0/setup.py
+-rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 pipen_report-0.9.0/PKG-INFO
```

### Comparing `pipen_report-0.8.0/README.md` & `pipen_report-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/cli.py` & `pipen_report-0.9.0/pipen_report/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/defaults.py` & `pipen_report-0.9.0/pipen_report/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/filters.py` & `pipen_report-0.9.0/pipen_report/filters.py`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/package-lock.json` & `pipen_report-0.9.0/pipen_report/frontend/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977549200986701%*

 * *Differences: {"'packages'": "{'': {'devDependencies': {'@rollup/plugin-alias': '^5.0', "*

 * *               "'@rollup/plugin-commonjs': '^24.1', 'svelte': '^3.58.0'}}, "*

 * *               "'node_modules/@jridgewell/gen-mapping': {'version': '0.3.3', 'resolved': "*

 * *               "'https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ=='}, "*

 * *               "'node_m […]*

```diff
@@ -1,27 +1,27 @@
 {
     "lockfileVersion": 3,
     "name": "pipen-report",
     "packages": {
         "": {
             "devDependencies": {
-                "@rollup/plugin-alias": "^4.0",
-                "@rollup/plugin-commonjs": "^24.0",
+                "@rollup/plugin-alias": "^5.0",
+                "@rollup/plugin-commonjs": "^24.1",
                 "@rollup/plugin-json": "^6.0",
                 "@rollup/plugin-node-resolve": "^15.0",
                 "@rollup/plugin-terser": "^0.4",
                 "acorn": "^8.8",
                 "carbon-components-svelte": "^0.73.5",
                 "carbon-icons-svelte": "^11.3",
                 "rollup": "^3.17",
                 "rollup-plugin-copy": "^3.4",
                 "rollup-plugin-css-only": "^4.3",
                 "rollup-plugin-livereload": "^2.0",
                 "rollup-plugin-svelte": "^7.1",
-                "svelte": "^3.56.0"
+                "svelte": "^3.58.0"
             },
             "license": "MIT",
             "name": "pipen-report",
             "version": "1.0.0"
         },
         "node_modules/@jridgewell/gen-mapping": {
             "dependencies": {
@@ -29,17 +29,17 @@
                 "@jridgewell/sourcemap-codec": "^1.4.10",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz",
-            "version": "0.3.2"
+            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "node_modules/@jridgewell/resolve-uri": {
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
@@ -57,33 +57,39 @@
         },
         "node_modules/@jridgewell/source-map": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
-            "integrity": "sha512-m7O9o2uR8k2ObDysZYzdfhb08VuEml5oWGiosa1VdaPZ/A6QyPkAJuwN0Q1lhULOf6B7MtQmHENS743hWtCrgw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.2.tgz",
-            "version": "0.3.2"
+            "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "node_modules/@jridgewell/sourcemap-codec": {
             "dev": true,
-            "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
-            "version": "1.4.14"
+            "integrity": "sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz",
+            "version": "1.4.15"
         },
         "node_modules/@jridgewell/trace-mapping": {
             "dependencies": {
                 "@jridgewell/resolve-uri": "3.1.0",
                 "@jridgewell/sourcemap-codec": "1.4.14"
             },
             "dev": true,
-            "integrity": "sha512-MCNzAp77qzKca9+W/+I0+sEpaUnZoeasnghNeVc41VZCEKaCH73Vq3BZZ/SzWIgrqE4H4ceI+p+b6C0mHf9T4g==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.17.tgz",
-            "version": "0.3.17"
+            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
+            "version": "0.3.18"
+        },
+        "node_modules/@jridgewell/trace-mapping/node_modules/@jridgewell/sourcemap-codec": {
+            "dev": true,
+            "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
+            "version": "1.4.14"
         },
         "node_modules/@nodelib/fs.scandir": {
             "dependencies": {
                 "@nodelib/fs.stat": "2.0.5",
                 "run-parallel": "^1.1.9"
             },
             "dev": true,
@@ -120,50 +126,50 @@
             "dependencies": {
                 "slash": "^4.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-ZuDWE1q4PQDhvm/zc5Prun8sBpLJy41DMptYrS6MhAy9s9kL/doN1613BWfEchGVfKxzliJ3BjbOPizXX38DbQ==",
+            "integrity": "sha512-l9hY5chSCjuFRPsnRm16twWBiSApl2uYFLsepQYwtBuAxNMQ/1dJqADld40P0Jkqm65GRTLy/AC6hnpVebtLsA==",
             "peerDependencies": {
                 "rollup": "^1.20.0||^2.0.0||^3.0.0"
             },
             "peerDependenciesMeta": {
                 "rollup": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@rollup/plugin-alias/-/plugin-alias-4.0.3.tgz",
-            "version": "4.0.3"
+            "resolved": "https://registry.npmjs.org/@rollup/plugin-alias/-/plugin-alias-5.0.0.tgz",
+            "version": "5.0.0"
         },
         "node_modules/@rollup/plugin-commonjs": {
             "dependencies": {
                 "@rollup/pluginutils": "^5.0.1",
                 "commondir": "^1.0.1",
                 "estree-walker": "^2.0.2",
                 "glob": "^8.0.3",
                 "is-reference": "1.2.1",
                 "magic-string": "^0.27.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-15LsiWRZk4eOGqvrJyu3z3DaBu5BhXIMeWnijSRvd8irrrg9SHpQ1pH+BUK4H6Z9wL9yOxZJMTLU+Au86XHxow==",
+            "integrity": "sha512-eSL45hjhCWI0jCCXcNtLVqM5N1JlBGvlFfY0m6oOYnLCJ6N0qEXoZql4sY2MOUArzhH4SA/qBpTxvvZp2Sc+DQ==",
             "peerDependencies": {
                 "rollup": "^2.68.0||^3.0.0"
             },
             "peerDependenciesMeta": {
                 "rollup": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@rollup/plugin-commonjs/-/plugin-commonjs-24.0.1.tgz",
-            "version": "24.0.1"
+            "resolved": "https://registry.npmjs.org/@rollup/plugin-commonjs/-/plugin-commonjs-24.1.0.tgz",
+            "version": "24.1.0"
         },
         "node_modules/@rollup/plugin-json": {
             "dependencies": {
                 "@rollup/pluginutils": "^5.0.1"
             },
             "dev": true,
             "engines": {
@@ -182,55 +188,55 @@
             "version": "6.0.0"
         },
         "node_modules/@rollup/plugin-node-resolve": {
             "dependencies": {
                 "@rollup/pluginutils": "^5.0.1",
                 "@types/resolve": "1.20.2",
                 "deepmerge": "^4.2.2",
-                "is-builtin-module": "^3.2.0",
+                "is-builtin-module": "^3.2.1",
                 "is-module": "^1.0.0",
                 "resolve": "^1.22.1"
             },
             "dev": true,
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-ReY88T7JhJjeRVbfCyNj+NXAG3IIsVMsX9b5/9jC98dRP8/yxlZdz7mHZbHk5zHr24wZZICS5AcXsFZAXYUQEg==",
+            "integrity": "sha512-Y35fRGUjC3FaurG722uhUuG8YHOJRJQbI6/CkbRkdPotSpDj9NtIN85z1zrcyDcCQIW4qp5mgG72U+gJ0TAFEg==",
             "peerDependencies": {
                 "rollup": "^2.78.0||^3.0.0"
             },
             "peerDependenciesMeta": {
                 "rollup": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@rollup/plugin-node-resolve/-/plugin-node-resolve-15.0.1.tgz",
-            "version": "15.0.1"
+            "resolved": "https://registry.npmjs.org/@rollup/plugin-node-resolve/-/plugin-node-resolve-15.0.2.tgz",
+            "version": "15.0.2"
         },
         "node_modules/@rollup/plugin-terser": {
             "dependencies": {
                 "serialize-javascript": "^6.0.0",
                 "smob": "^0.0.6",
                 "terser": "^5.15.1"
             },
             "dev": true,
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-Ipcf3LPNerey1q9ZMjiaWHlNPEHNU/B5/uh9zXLltfEQ1lVSLLeZSgAtTPWGyw8Ip1guOeq+mDtdOlEj/wNxQw==",
+            "integrity": "sha512-aKS32sw5a7hy+fEXVy+5T95aDIwjpGHCTv833HXVtyKMDoVS7pBr5K3L9hEQoNqbJFjfANPrNpIXlTQ7is00eA==",
             "peerDependencies": {
                 "rollup": "^2.x || ^3.x"
             },
             "peerDependenciesMeta": {
                 "rollup": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@rollup/plugin-terser/-/plugin-terser-0.4.0.tgz",
-            "version": "0.4.0"
+            "resolved": "https://registry.npmjs.org/@rollup/plugin-terser/-/plugin-terser-0.4.1.tgz",
+            "version": "0.4.1"
         },
         "node_modules/@rollup/pluginutils": {
             "dependencies": {
                 "@types/estree": "^1.0.0",
                 "estree-walker": "^2.0.2",
                 "picomatch": "^2.3.1"
             },
@@ -732,17 +738,17 @@
             "dependencies": {
                 "has": "^1.0.3"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-RRjxlvLDkD1YJwDbroBHMb+cukurkDWNyHx7D3oNB5x9rb5ogcksMC5wHCadcXoo67gVr/+3GFySh3134zi6rw==",
-            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.11.0.tgz",
-            "version": "2.11.0"
+            "integrity": "sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==",
+            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.0.tgz",
+            "version": "2.12.0"
         },
         "node_modules/is-extglob": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==",
@@ -975,25 +981,25 @@
             "version": "3.6.0"
         },
         "node_modules/resolve": {
             "bin": {
                 "resolve": "bin/resolve"
             },
             "dependencies": {
-                "is-core-module": "^2.9.0",
+                "is-core-module": "^2.12.0",
                 "path-parse": "^1.0.7",
                 "supports-preserve-symlinks-flag": "^1.0.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-nBpuuYuY5jFsli/JIs1oldw6fOQCBioohqWZg/2hiaOybXOft4lonv85uDOKXdf8rhyK159cxU5cDcK/NKk8zw==",
-            "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.1.tgz",
-            "version": "1.22.1"
+            "integrity": "sha512-P8ur/gp/AmbEzjr729bZnLjXK5Z+4P0zhIJgBgzqRih7hL7BOukHGtSTA3ACMY467GRFz3duQsi0bDZdR7DKdw==",
+            "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.3.tgz",
+            "version": "1.22.3"
         },
         "node_modules/resolve.exports": {
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "integrity": "sha512-X2UW6Nw3n/aMgDVy+0rSqgHlv39WZAlZrXCdnbyEiKm17DSqHX4MmQMaST3FbeWR5FTuRcUwYAziZajji0Y7mg==",
@@ -1201,17 +1207,17 @@
             "version": "1.0.0"
         },
         "node_modules/svelte": {
             "dev": true,
             "engines": {
                 "node": ">= 8"
             },
-            "integrity": "sha512-WMXEvF+RtAaclw0t3bPDTUe19pplMlfyKDsixbHQYgCWi9+O9VN0kXU1OppzrB9gPAvz4NALuoca2LfW2bOjTQ==",
-            "resolved": "https://registry.npmjs.org/svelte/-/svelte-3.57.0.tgz",
-            "version": "3.57.0"
+            "integrity": "sha512-brIBNNB76mXFmU/Kerm4wFnkskBbluBDCjx/8TcpYRb298Yh2dztS2kQ6bhtjMcvUhd5ynClfwpz5h2gnzdQ1A==",
+            "resolved": "https://registry.npmjs.org/svelte/-/svelte-3.58.0.tgz",
+            "version": "3.58.0"
         },
         "node_modules/terser": {
             "bin": {
                 "terser": "bin/terser"
             },
             "dependencies": {
                 "@jridgewell/source-map": "^0.3.2",
@@ -1219,17 +1225,17 @@
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QI5g1E/ef7d+PsDifb+a6nnVgC4F22Bg6T0xrBrz6iloVB4PUkkunp6V8nzoOOZJIzjWVdAGqCdlKlhLq/TbIA==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.16.8.tgz",
-            "version": "5.16.8"
+            "integrity": "sha512-HPa/FdTB9XGI2H1/keLFZHxl6WNvAI4YalHGtDQTlMnJcoqSab1UwL4l1hGEhs6/GmLHBZIg/YgB++jcbzoOEg==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.16.9.tgz",
+            "version": "5.16.9"
         },
         "node_modules/to-regex-range": {
             "dependencies": {
                 "is-number": "^7.0.0"
             },
             "dev": true,
             "engines": {
```

### Comparing `pipen_report-0.8.0/pipen_report/frontend/package.json` & `pipen_report-0.9.0/pipen_report/frontend/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923469387755102%*

 * *Differences: {"'devDependencies'": "{'@rollup/plugin-alias': '^5.0', '@rollup/plugin-commonjs': '^24.1', "*

 * *                      "'svelte': '^3.58.0'}"}*

```diff
@@ -1,23 +1,23 @@
 {
     "devDependencies": {
-        "@rollup/plugin-alias": "^4.0",
-        "@rollup/plugin-commonjs": "^24.0",
+        "@rollup/plugin-alias": "^5.0",
+        "@rollup/plugin-commonjs": "^24.1",
         "@rollup/plugin-json": "^6.0",
         "@rollup/plugin-node-resolve": "^15.0",
         "@rollup/plugin-terser": "^0.4",
         "acorn": "^8.8",
         "carbon-components-svelte": "^0.73.5",
         "carbon-icons-svelte": "^11.3",
         "rollup": "^3.17",
         "rollup-plugin-copy": "^3.4",
         "rollup-plugin-css-only": "^4.3",
         "rollup-plugin-livereload": "^2.0",
         "rollup-plugin-svelte": "^7.1",
-        "svelte": "^3.56.0"
+        "svelte": "^3.58.0"
     },
     "license": "MIT",
     "name": "pipen-report",
     "private": true,
     "scripts": {
         "build": "rollup -c"
     },
```

### Comparing `pipen_report-0.8.0/pipen_report/frontend/public/assets/ccs.css` & `pipen_report-0.9.0/pipen_report/frontend/public/assets/ccs.css`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/public/assets/favicon.png` & `pipen_report-0.9.0/pipen_report/frontend/public/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/public/assets/global.css` & `pipen_report-0.9.0/pipen_report/frontend/public/assets/global.css`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/rollup.config.js.jinja` & `pipen_report-0.9.0/pipen_report/frontend/rollup.config.js.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,23 @@
 import css from 'rollup-plugin-css-only';
 import copy from 'rollup-plugin-copy';
 import json from '@rollup/plugin-json';
 import data from './src/data.json' assert { type: 'json' };
 
 const commonConfig = (proc_slug = null, page = 0, cssfile = 'index.css') => ({
 	plugins: [
-		svelte({ compilerOptions: { dev: false } }),
+		svelte({
+			compilerOptions: { dev: false },
+			onwarn: (warning, handler) => {
+				// carbon-components-svelte 0.37.5
+				// svelte 3.58.0
+				if (warning.code.startsWith("a11y-")) return;
+				handler(warning);
+			}
+		}),
 		alias({
 			entries: [
 				{ find: '$components', replacement: '../../components' },
 				{ find: '$component', replacement: '../../components' },
 				{ find: '$layouts', replacement: '../../layouts' },
 				{ find: '$layout', replacement: '../../layouts' },
 				{ find: '$libs', replacement: '../../components' },
```

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/components/DataTable/DataTable.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/components/DataTable/DataTable.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/components/DataTable/DataTableInner.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/components/DataTable/DataTableInner.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/components/Image/ImageInner.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/components/Image/ImageInner.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/components/PageNavButton.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/components/PageNavButton.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/layouts/Header.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/layouts/Header.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/layouts/ProcLayout.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/layouts/ProcLayout.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/layouts/ProcToc.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/layouts/ProcToc.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/pages/_index/index.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/pages/_index/index.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/pages/proc/index.svelte` & `pipen_report-0.9.0/pipen_report/frontend/src/pages/proc/index.svelte`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/frontend/src/proc.html` & `pipen_report-0.9.0/pipen_report/frontend/src/proc.html`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pipen_report/preprocess.py` & `pipen_report-0.9.0/pipen_report/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,18 +102,18 @@
 
 def _preprocess_markdown(source: str) -> str:
     """Preprocess Markdown tag
 
     A Markdown tag with markdown content within it, which will be then rendered
     as html.
     """
-    import markdown
+    from markdown import markdown
 
     def callback(matching):
-        return markdown.markdown(matching.group(1))
+        return markdown(matching.group(1))
 
     return re.sub(
         r"<Markdown>(.+?)</Markdown>",
         callback,
         source,
         flags=re.DOTALL,
     )
```

### Comparing `pipen_report-0.8.0/pipen_report/report_manager.py` & `pipen_report-0.9.0/pipen_report/report_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,26 +178,26 @@
                 ):
                     flog.write(line)
                     if chars_to_log in line:
                         line = line.replace("\033[1m", "[bold]")
                         line = line.replace("\033[22m", "[/bold]")
                         line = line.replace("\033[39m", "")
                         logger.info(f"- {line.rstrip()}")
-                    elif chars_to_error in line:
+                    elif chars_to_error in line:  # pragma: no cover
                         line = line.replace("\033[1m", "[bold]")
                         line = line.replace("\033[22m", "[/bold]")
                         line = line.replace("\033[33m", "[red]")
                         line = line.replace("\033[39m", "[/red]")
                         logger.error(f"- {line.rstrip()}")
                         raise RuntimeError("Failed to build reports")
             except CmdyReturnCodeError as e:  # pragma: no cover
                 flog.write(str(e))
                 logger.error("Failed to build reports")
                 logger.error("See %s for details", logfile)
-            except RuntimeError as e:
+            except RuntimeError as e:  # pragma: no cover
                 logger.error(str(e))
                 logger.error("See %s for details", logfile)
             else:
                 logger.info("View the reports at %s", self.outdir)
                 logger.info("Or run the following command to serve them:")
                 logger.info("> pipen report serve -r %s", self.outdir.parent)
```

### Comparing `pipen_report-0.8.0/pipen_report/report_plugin.py` & `pipen_report-0.9.0/pipen_report/report_plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_report-0.8.0/pyproject.toml` & `pipen_report-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "pipen-report"
-version = "0.8.0"
+version = "0.9.0"
 description = "Report generation system for pipen"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-report"
 repository = "https://github.com/pwwang/pipen-report"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen = "^0.7"
+python = "^3.8"
+pipen = "^0.9"
 cmdy = "^0.5"
 Markdown = "^3"
 copier = "^7"
+python-slugify = "^8.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
 pytest-xdist = "^2"
 pytest-forked = "^1"
+pipen-filters = "^0.7.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.plugins.pipen]
 report = "pipen_report.report_plugin:PipenReport"
@@ -47,9 +49,9 @@
 allow_redefinition = true
 disable_error_code = ["attr-defined", "no-redef", "import"]
 show_error_codes = true
 strict_optional = false
 
 [tool.black]
 line-length = 79
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
```

### Comparing `pipen_report-0.8.0/setup.py` & `pipen_report-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,32 +15,36 @@
                   'frontend/src/components/DataTable/*',
                   'frontend/src/components/Image/*',
                   'frontend/src/layouts/*',
                   'frontend/src/pages/_index/*',
                   'frontend/src/pages/proc/*']}
 
 install_requires = \
-['Markdown>=3,<4', 'cmdy>=0.5,<0.6', 'copier>=7,<8', 'pipen>=0.7,<0.8']
+['Markdown>=3,<4',
+ 'cmdy>=0.5,<0.6',
+ 'copier>=7,<8',
+ 'pipen>=0.9,<0.10',
+ 'python-slugify>=8.0.1,<9.0.0']
 
 entry_points = \
 {'pipen': ['report = pipen_report.report_plugin:PipenReport'],
  'pipen_cli': ['cli-report = pipen_report.cli:PipenCliReport']}
 
 setup_kwargs = {
     'name': 'pipen-report',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Report generation system for pipen',
     'long_description': '# pipen-report\n\nReport generation system for [pipen][1]\n\n## Installation\n\n```shell\n❯ pip install -U pipen-report\n\n# update configurations if needed:\n❯ pipen report config\n\n# then update frontend dependencies:\n❯ pipen report update\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it: `plugins=[..., "no:report"]`, or uninstall this plugin.\n\n## Example\n\nSee the pipeline in `example/`, and the reports generated by the pipeline:\n\n[https://pwwang.github.io/pipen-report/example/output/REPORTS][2]\n\n## Documentation\n\nSee: [https://pwwang.github.io/pipen-report][3]\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://pwwang.github.io/pipen-report/example/output/REPORTS\n[3]: https://pwwang.github.io/pipen-report\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-report',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pipen_report-0.8.0/PKG-INFO` & `pipen_report-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pipen-report
-Version: 0.8.0
+Version: 0.9.0
 Summary: Report generation system for pipen
 Home-page: https://github.com/pwwang/pipen-report
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Markdown (>=3,<4)
 Requires-Dist: cmdy (>=0.5,<0.6)
 Requires-Dist: copier (>=7,<8)
-Requires-Dist: pipen (>=0.7,<0.8)
+Requires-Dist: pipen (>=0.9,<0.10)
+Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/pwwang/pipen-report
 Description-Content-Type: text/markdown
 
 # pipen-report
 
 Report generation system for [pipen][1]
```

