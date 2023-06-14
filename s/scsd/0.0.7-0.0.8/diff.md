# Comparing `tmp/scsd-0.0.7.tar.gz` & `tmp/scsd-0.0.8.tar.gz`

## Comparing `scsd-0.0.7.tar` & `scsd-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scsd-0.0.7/Dockerfile
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scsd-0.0.7/requirements.txt
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.7/scsd
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scsd-0.0.7/scsd.conf.sample
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 scsd-0.0.7/docker/cron-root
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/__init__.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/__main__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/args.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/auth.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/config.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/db.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/err.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/logger.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/notifier.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/parser.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/storage.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scsd-0.0.7/steamCloudSaveDownloader/web.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 scsd-0.0.7/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.7/LICENSE
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 scsd-0.0.7/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scsd-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 scsd-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scsd-0.0.8/Dockerfile
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scsd-0.0.8/requirements.txt
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.8/scsd
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scsd-0.0.8/scsd.conf.sample
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scsd-0.0.8/docker/cron-root
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/__main__.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/args.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/auth.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/config.py
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/db.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/err.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/notifier.py
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/parser.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/storage.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/web.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 scsd-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.8/LICENSE
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 scsd-0.0.8/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scsd-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 scsd-0.0.8/PKG-INFO
```

### Comparing `scsd-0.0.7/steamCloudSaveDownloader/__main__.py` & `scsd-0.0.8/steamCloudSaveDownloader/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,85 @@
 from . import args
 from . import web
 from . import db
 from . import storage
 from .auth import auth
-from .err import err
+from . import err
 from .notifier import notifier
 from .config import config
 import logging
 import sys
 import os
+import traceback
 
 logger = None
 
-def __main__():
+def setup_logger():
+    global logger
+
     logging.basicConfig(
         format='%(asctime)s [%(levelname)s] %(message)s',
         datefmt='%Y-%m-%d %H:%M:%S')
-    global logger
     logger = logging.getLogger('scsd')
-    try:
-        notifier_ = None
-        parsed_args = args.args().parse(sys.argv[1:])
 
-        if 'auth' in parsed_args and \
-                parsed_args['auth'] is not None and \
-                len(parsed_args['auth']) != 0:
-            print("Auth")
-            auth_ = auth(parsed_args['auth'], parsed_args['save_dir'])
-            exit(1)
+def parse():
+    parsed_args = args.args().parse(sys.argv[1:])
+
+    if 'auth' in parsed_args and \
+            parsed_args['auth'] is not None and \
+            len(parsed_args['auth']) != 0:
+        auth_ = auth(parsed_args['save_dir'])
+        auth_.new_session(parsed_args['auth'])
+        exit(0)
+
+    if parsed_args['conf'] is not None:
+        parsed_args = config(parsed_args['conf']).get_conf()
+
+    return parsed_args
+
+def __main__():
+    global logger
 
-        if parsed_args['conf'] is not None:
-            parsed_args = config(parsed_args['conf']).get_conf()
+    notifier_ = None
+
+    try:
+        setup_logger()
+        parsed_args = parse()
 
         logger.setLevel(args.args.convert_log_level(parsed_args['log_level']))
         logger.debug(parsed_args)
 
         notifier_ = notifier.create_instance(
             parsed_args['notifier'],
             **parsed_args)
 
         main(parsed_args)
-    except err as e:
+    except err.err as e:
         if notifier_:
             notifier_.send(e.get_msg(), False)
         e.log()
         exit(e.num())
+    except Exception:
+        if notifier_:
+            notifier_.send(traceback.format_exc(), False)
+        exit(e.num())
 
     end_msg = "Process ended noramlly"
     logger.info(end_msg)
     notifier_.send(end_msg, True)
     exit(0)
 
 def main(parsed_args):
 
-    web_ = web.web(os.path.join(parsed_args['save_dir'], 'session.sb'))
+    auth_ = auth(parsed_args['save_dir'])
+
+    session_pkl = auth_.get_session_path()
+    if not os.path.isfile(session_pkl):
+        raise err.err(err.err_enum.NO_SESSION)
+    web_ = web.web(session_pkl)
 
     db_ = db.db(parsed_args['save_dir'], parsed_args['rotation'])
     storage_ = storage.storage(parsed_args['save_dir'], db_)
 
     game_list = web_.get_list()
 
     for game in game_list:
@@ -84,22 +106,28 @@
                                                    0),
                 )
             continue
 
         for file_info in file_infos:
             file_id = db_.get_file_id(game['app_id'], file_info['filename'])
             if (not db_.is_file_outdated(file_id, file_info['time'])):
+                logger.info(f"Ignore {file_info['filename']} (no change)")
                 continue
-            logger.info(f"  Downloading {file_info['filename']}")
+            logger.info(f"Downloading {file_info['filename']}")
             storage_.rotate_file(
                 game['app_id'],
                 file_info['filename'],
                 file_info['path'],
-                file_id)
+                file_id,
+                file_info['time'])
             web_.download_game_save(
                 file_info['link'],
                 storage_.get_filename_location(game['app_id'],
                                                file_info['filename'],
                                                file_info['path'],
                                                0)
             )
-            storage_.remove_outdated(file_id)
+            storage_.remove_outdated(
+                game['app_id'],
+                file_info['filename'],
+                file_info['path'],
+                file_id)
```

### Comparing `scsd-0.0.7/steamCloudSaveDownloader/args.py` & `scsd-0.0.8/steamCloudSaveDownloader/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,24 +30,14 @@
             "-a",
             metavar="username",
             type=str,
             dest="auth",
             help="Save authentication"
         )
 
-
-        self.parser.add_argument(
-            "-c",
-            metavar="cookie_file",
-            dest="cookie",
-            type=argparse.FileType('r'),
-            required=False,
-            help="Netscape HTTP Cookie File of store.steampowered.com"
-        )
-
         self.parser.add_argument(
             "-d",
             metavar="save_dir",
             dest="save_dir",
             type=self.is_path,
             required=True,
             help="Directory to save the downloaded saves and db"
```

### Comparing `scsd-0.0.7/steamCloudSaveDownloader/config.py` & `scsd-0.0.8/steamCloudSaveDownloader/config.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.7/steamCloudSaveDownloader/db.py` & `scsd-0.0.8/steamCloudSaveDownloader/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sqlite3
 import os
 import datetime
 from . import err
 from .err import err_enum
+import logging
 
 DB_FILENAME = 'scsd.sqlite3'
 
 '''Schema
 TABLE GAMES
 app_id (integer) PK, CONSTRAINT >0
 game_name (text)
@@ -21,28 +22,29 @@
 TABLE VERSION
 version_id (INT) PK AUTOINC
 file_id foreign key
 time (datetime)
 version_num (INT) >= 0
 
 '''
-
+logger = logging.getLogger('scsd')
 class db:
     def __init__(self, db_location:str, rotation:int):
         self.location = db_location
         self.rotation = rotation
         self.db_file = os.path.join(db_location, DB_FILENAME)
 
         self.con = sqlite3.connect(self.db_file, detect_types=sqlite3.PARSE_DECLTYPES)
 
         if not self.schema_ok():
             self.initialize_schema()
 
     def __del__(self):
-        self.con.close()
+        if hasattr(self, 'con'):
+            self.con.close()
 
     def schema_ok(self) -> bool:
         cur = self.con.cursor()
         res = cur.execute("SELECT name FROM sqlite_master WHERE type='table' AND name='GAMES';")
         if res.fetchone() is None:
             return False
 
@@ -126,50 +128,64 @@
     # Expect [(filename, path, app_id, last_update_time), ...]
     def add_new_files(self, file_tuples:list):
         cur = self.con.cursor()
         for tup in file_tuples:
             res = cur.execute("INSERT INTO FILES VALUES (NULL, ?, ?, ?);", tup[0:3])
             file_id = cur.lastrowid
 
-            res = cur.execute("INSERT INTO VERSION VALUES (NULL, ?, ?, ?);", (file_id, tup[3], 0))
+            no_tz_time = tup[3].replace(tzinfo=None)
+            res = cur.execute("INSERT INTO VERSION VALUES (NULL, ?, ?, ?);", (file_id, no_tz_time, 0))
 
         self.con.commit()
 
-    def is_file_outdated(self, file_id:int, time:datetime) -> bool:
+    def is_file_outdated(self, file_id:int, server_time:datetime) -> bool:
         cur = self.con.cursor()
+        # TODO: Bug timezone in DB
         res = cur.execute("SELECT time FROM VERSION WHERE file_id = ? and version_num = 0;", (file_id,))
-        time_tuple = res.fetchone()
-        if time_tuple is None:
+        db_time_tuple = res.fetchone()
+        if db_time_tuple is None:
+            logger.warning(f'Failed to retrieve newest version time for file_id {file_id}')
             return True
 
-        if time_tuple[0] < time:
+        tz_db_time = db_time_tuple[0].replace(tzinfo=datetime.timezone.utc)
+
+        logger.debug(f'DB time: {tz_db_time}, Server time: {server_time}')
+
+        if tz_db_time < server_time:
             return True
         else:
             return False
 
     # +1 for each version
     # Insert 0 as now
     # Return max version
-    def update_file_update_time_to_now(self, file_id:int) -> int:
+    def update_file_update_time_to_now(self, file_id:int, newest_file_time: datetime.datetime) -> int:
         cur = self.con.cursor()
-        now = datetime.datetime.now()
-        now = datetime.datetime(now.year, now.month, now.day, now.hour, now.minute)
 
         # Increment one for all
         res = cur.execute("UPDATE VERSION SET version_num = version_num + 1 WHERE file_id = ?;", (file_id,))
 
+        time_without_tz = newest_file_time.replace(tzinfo=None)
         # Insert newest as 0
-        res = cur.execute("INSERT INTO VERSION VALUES (NULL, ?, ?, 0)", (file_id, now))
+        res = cur.execute("INSERT INTO VERSION VALUES (NULL, ?, ?, 0)", (file_id, time_without_tz))
         self.con.commit()
 
         res = cur.execute("SELECT COUNT(*) FROM VERSION WHERE file_id = ?", (file_id,))
         count = res.fetchone();
 
         if (count is None):
             return 0
         else:
             return count[0]
 
-    # TODO Rotation
-    def get_outdated_file(file_id:int):
-        res = cur.execute("SELECT version_id FROM WHERE file_id = ? AND version_num >= ?", (file_id, self.rotation))
+    def remove_outdated_file(self, file_id:int):
+        cur = self.con.cursor()
+        res = cur.execute("SELECT version_num FROM VERSION WHERE file_id = ? AND version_num >= ?", (file_id, self.rotation))
+        outdated_version_num = res.fetchall();
+
+        res = cur.execute("DELETE FROM VERSION WHERE file_id = ? AND version_num >= ?", (file_id, self.rotation))
+
+        self.con.commit()
+
+        logger.debug(f"DB Removing version {outdated_version_num}")
 
+        return outdated_version_num
```

### Comparing `scsd-0.0.7/steamCloudSaveDownloader/err.py` & `scsd-0.0.8/steamCloudSaveDownloader/err.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import sys
 from enum import IntEnum
 import logging
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger('scsd')
 
 class err_enum(IntEnum):
     CANNOT_RETRIEVE_LIST = 1
     CANNOT_PARSE_LIST = 2
     CANNOT_RETRIEVE_GAME_FILES = 3
     CANNOT_PARSE_GAME_FILES = 4
     CANNOT_INITIALIZE_DB = 5
     CANNOT_CREATE_DIRECTORY = 6
     INVALID_WEBHOOK_URL = 7
     INVALID_COOKIE_FORMAT = 8,
-    INVALID_CONFIG = 9
-    LOGIN_FAIL = 10
+    INVALID_CONFIG = 9,
+    LOGIN_FAIL = 10,
+    NO_SESSION = 11,
+    CANNOT_REMOVE_OUTDATED = 12
 
 ERR_INFO = {
     err_enum.CANNOT_RETRIEVE_LIST: [
         logging.ERROR,
         "Cannot retrieve list from steam. Please make sure connected to Internet and cookie is valid."
     ],
     err_enum.CANNOT_PARSE_LIST: [
@@ -52,14 +54,22 @@
     err_enum.INVALID_CONFIG: [
         logging.ERROR,
         "Invalid config format: "
     ],
     err_enum.LOGIN_FAIL: [
         logging.ERROR,
         "Login fail, please try again"
+    ],
+    err_enum.NO_SESSION: [
+        logging.ERROR,
+        "No session found. Please re-run the program with -a <username> -d <data_dir> first"
+    ],
+    err_enum.CANNOT_REMOVE_OUTDATED: [
+        logging.WARNING,
+        "Cannot remove outdated file: "
     ]
 }
 
 
 class err(Exception):
     def log(self):
         msg = self.message
```

### Comparing `scsd-0.0.7/steamCloudSaveDownloader/notifier.py` & `scsd-0.0.8/steamCloudSaveDownloader/notifier.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.7/steamCloudSaveDownloader/parser.py` & `scsd-0.0.8/steamCloudSaveDownloader/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .notifier import notifier
 from .err import err_enum
 from bs4 import BeautifulSoup
 import datetime
 import os
 import logging
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger('scsd')
 
 def get_tbody(soup):
     main_content = soup.find(id='main_content')
 
     if (main_content is None):
         raise err.err(err_enum.CANNOT_PARSE_LIST)
 
@@ -25,20 +25,21 @@
 
     # Assume 'DD MMM [YYYY] @ HH:MM{a|p}m' format
 
     tokens = input.split(' ')
     datetime_ = None
     try:
         if len(tokens) == 4:
-            now = datetime.datetime.now()
+            now = datetime.datetime.now(tz=datetime.timezone.utc)
             year = now.year
             d = datetime.datetime.strptime(input, "%d %b @ %I:%M%p")
-            datetime_ = d.replace(year=year)
+            datetime_ = d.replace(year=year, tzinfo=datetime.timezone.utc)
         elif len(tokens) == 5:
             datetime_ = datetime.datetime.strptime(input, "%d %b, %Y @ %I:%M%p")
+            datetime_ = d.replace(tzinfo=datetime.timezone.utc)
         else:
             raise err.err(er_enum.CANNOT_PARSE_GAME_FILES)
     except ValueError:
         raise err.err(er_enum.CANNOT_PARSE_GAME_FILES)
 
     return datetime_
 
@@ -93,18 +94,21 @@
 
         data = list()
         rows = tbody.find_all('tr')
 
         for row in rows:
             cols = row.find_all('td')
             path, filename = os.path.split(cols[1].text.strip())
+            time_str = cols[3].text.strip()
+            parsed_time = parse_time(time_str)
+            logger.debug(f"Parse {filename} time '{time_str}' as '{parsed_time.isoformat()}'")
             data.append({
                 "filename": filename,
                 "path": path,
-                "time": parse_time(cols[3].text.strip()),
+                "time": parsed_time,
                 "link": cols[4].a['href']})
 
         has_next = soup.find('a', text='next >>')
 
         if (has_next is None):
             return (data, None)
         else:
```

### Comparing `scsd-0.0.7/.gitignore` & `scsd-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `scsd-0.0.7/LICENSE` & `scsd-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scsd-0.0.7/pyproject.toml` & `scsd-0.0.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['hatchling', 'hatch-requirements-txt']
 build-backend = "hatchling.build"
 
 [project]
 name = "scsd"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="hchsu"}
 ]
 description = "Steam Cloud Save Downloader"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

