# Comparing `tmp/ukrdc-xsdata-3.3.0.post1.tar.gz` & `tmp/ukrdc_xsdata-3.4.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukrdc-xsdata-3.3.0.post1.tar", last modified: Mon Jan 31 14:49:23 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

