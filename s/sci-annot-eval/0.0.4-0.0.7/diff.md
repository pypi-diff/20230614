# Comparing `tmp/sci_annot_eval-0.0.4.tar.gz` & `tmp/sci_annot_eval-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sci_annot_eval-0.0.4.tar", last modified: Thu Nov 18 17:22:25 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

