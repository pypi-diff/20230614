# Comparing `tmp/opendaq-0.3.2.tar.gz` & `tmp/opendaq-0.9.8-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opendaq-0.3.2.tar", last modified: Mon Feb 27 19:31:32 2017, max compression
+Zip archive data, at least v1.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

