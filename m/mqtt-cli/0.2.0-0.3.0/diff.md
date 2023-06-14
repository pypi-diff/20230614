# Comparing `tmp/mqtt-cli-0.2.0.tar.gz` & `tmp/mqtt-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-cli-0.2.0.tar", last modified: Thu Jun  8 11:55:42 2023, max compression
+gzip compressed data, was "mqtt-cli-0.3.0.tar", last modified: Wed Jun 14 19:17:29 2023, max compression
```

## Comparing `mqtt-cli-0.2.0.tar` & `mqtt-cli-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 11:55:42.098796 mqtt-cli-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-08 11:55:16.000000 mqtt-cli-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-08 11:55:42.098796 mqtt-cli-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-08 11:55:16.000000 mqtt-cli-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 11:55:42.098796 mqtt-cli-0.2.0/mqtt_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-08 11:55:42.000000 mqtt-cli-0.2.0/mqtt_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-08 11:55:42.000000 mqtt-cli-0.2.0/mqtt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 11:55:42.000000 mqtt-cli-0.2.0/mqtt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-08 11:55:42.000000 mqtt-cli-0.2.0/mqtt_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-08 11:55:42.000000 mqtt-cli-0.2.0/mqtt_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-08 11:55:42.000000 mqtt-cli-0.2.0/mqtt_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-08 11:55:16.000000 mqtt-cli-0.2.0/mqtt_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 11:55:42.098796 mqtt-cli-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-08 11:55:16.000000 mqtt-cli-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/mqtt_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-14 19:17:29.000000 mqtt-cli-0.3.0/mqtt_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/mqtt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 19:17:29.993892 mqtt-cli-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-14 19:17:08.000000 mqtt-cli-0.3.0/setup.py
```

### Comparing `mqtt-cli-0.2.0/LICENSE` & `mqtt-cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt-cli-0.2.0/PKG-INFO` & `mqtt-cli-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-cli
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI for Paho MQTT
 Home-page: https://github.com/MO-RISE/mqtt-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
```

### Comparing `mqtt-cli-0.2.0/mqtt_cli.egg-info/PKG-INFO` & `mqtt-cli-0.3.0/mqtt_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-cli
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI for Paho MQTT
 Home-page: https://github.com/MO-RISE/mqtt-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
```

### Comparing `mqtt-cli-0.2.0/mqtt_cli.py` & `mqtt-cli-0.3.0/mqtt_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Main entrypoint for this application"""
 import sys
 import time
+import atexit
 import logging
 import warnings
 import argparse
 from pathlib import Path
 from threading import Thread
 
 from parse import compile
@@ -21,14 +22,17 @@
     ):  # pylint: disable=unused-argument
         """Subscribe on connect"""
         if reason_code != 0:
             logger.error(
                 "Disconnected from %s with reason code: %s", client, reason_code
             )
 
+    if args.transport == "websockets":
+        mq.ws_set_options(path=args.path)
+
     # Keyword argument handling
     kwargs = {}
     if args.protocol == 5:
         kwargs["clean_start"] = args.clean_start
 
     # Connect!
     mq.connect(args.host, args.port, **kwargs)
@@ -106,14 +110,17 @@
         mq.publish(
             topic=args.topic,
             payload=args.message,
             qos=args.qos,
             retain=args.retain,
         )
 
+    # Done, stop loop
+    mq.loop_stop()
+
 
 def subscribe(mq: Client, parser: argparse.ArgumentParser, args: argparse.Namespace):
     @mq.connect_callback()
     def _(client, userdata, flags, reason_code, props=None):
         """Subscribe on connect"""
         if reason_code != 0:
             logger.error(
@@ -153,14 +160,15 @@
     parser.add_argument("--transport", choices=["tcp", "websockets"], default="tcp")
     parser.add_argument("--clientid", type=str, default=None)
     parser.add_argument("--user", type=str, default=None)
     parser.add_argument("--password", type=str, default=None)
     parser.add_argument(
         "--protocol", type=int, choices=[MQTTv31, MQTTv311, MQTTv5], default=MQTTv5
     )
+    parser.add_argument("--path", type=str, default="/mqtt")
     parser.add_argument("--tls", action="store_true", default=False)
     parser.add_argument("--clean-start", action="store_true", default=False)
     parser.add_argument("--log-level", type=int, default=logging.WARNING)
 
     ## Subcommands
     subparsers = parser.add_subparsers(required=True)
 
@@ -202,14 +210,16 @@
     )
     mq.username_pw_set(args.user, args.password)
     if args.tls:
         mq.tls_set()
 
     mq.enable_logger(logger.getChild("paho.client"))
 
+    atexit.register(mq.disconnect)
+
     # Dispatch to correct function
     try:
         args.func(mq, parser, args)
     except KeyboardInterrupt:
         sys.exit(0)
```

### Comparing `mqtt-cli-0.2.0/setup.py` & `mqtt-cli-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="mqtt-cli",
-    version="0.2.0",
+    version="0.3.0",
     license="Apache License 2.0",
     description="CLI for Paho MQTT",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/MO-RISE/mqtt-cli",
     author="Fredrik Olsson",
     author_email="fredrik.x.olsson@ri.se",
```

