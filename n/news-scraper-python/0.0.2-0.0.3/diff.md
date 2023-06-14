# Comparing `tmp/news-scraper-python-0.0.2.tar.gz` & `tmp/news_scraper_python-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-scraper-python-0.0.2.tar", last modified: Tue Jun 13 10:11:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

