# Comparing `tmp/mbta-gtfs-sqlite-0.9.8.tar.gz` & `tmp/mbta-gtfs-sqlite-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.9.8.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.9.9.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.9.8.tar` & `mbta-gtfs-sqlite-0.9.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0     3014 2023-05-04 05:00:58.846666 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/build.py
--rw-r--r--   0        0        0      389 2023-05-04 05:03:03.344844 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0     4369 2023-05-04 15:02:00.233311 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6333 2023-05-04 22:19:23.539885 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1504 2023-05-02 13:18:44.004053 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1745 2023-05-02 13:18:22.018700 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     2005 2023-05-04 22:18:43.022321 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/indexes.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      454 2023-05-04 22:22:42.864670 mbta-gtfs-sqlite-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      742 2023-05-04 22:23:04.506645 mbta-gtfs-sqlite-0.9.8/setup.py
--rw-r--r--   0        0        0      494 2023-05-04 22:23:04.506902 mbta-gtfs-sqlite-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0     3014 2023-05-04 05:00:58.846666 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/build.py
+-rw-r--r--   0        0        0      389 2023-05-04 05:03:03.344844 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0     4369 2023-05-04 15:02:00.233311 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6333 2023-05-04 22:19:23.539885 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1504 2023-05-02 13:18:44.004053 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      865 2023-05-28 23:25:35.414018 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1745 2023-05-02 13:18:22.018700 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     2005 2023-05-04 22:18:43.022321 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/indexes.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      454 2023-05-28 23:26:42.128230 mbta-gtfs-sqlite-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-05-28 23:27:00.437581 mbta-gtfs-sqlite-0.9.9/setup.py
+-rw-r--r--   0        0        0      494 2023-05-28 23:27:00.437810 mbta-gtfs-sqlite-0.9.9/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/archive.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/build.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/build.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/feed.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/feed.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/ingest.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,10 +11,11 @@
     feed_publisher_url: Mapped[str] = mapped_column(String)
     feed_lang: Mapped[str] = mapped_column(String)
     feed_start_date: Mapped[date] = mapped_column(Date)
     feed_end_date: Mapped[date] = mapped_column(Date)
     feed_version: Mapped[str] = mapped_column(String)
     feed_contact_email: Mapped[str] = mapped_column(String, nullable=True)
     feed_contact_url: Mapped[str] = mapped_column(String, nullable=True)
+    feed_id: Mapped[str] = mapped_column(String, nullable=True)
     # These are not part of GTFS
     retrieved_from_url: Mapped[str] = mapped_column(String)
     zip_md5_checksum: Mapped[str] = mapped_column(String)
```

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/trips.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/indexes.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/indexes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.8/setup.py` & `mbta-gtfs-sqlite-0.9.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['SQLAlchemy>=2.0.7,<3.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

