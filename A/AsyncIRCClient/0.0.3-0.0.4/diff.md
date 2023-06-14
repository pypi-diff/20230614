# Comparing `tmp/AsyncIRCClient-0.0.3.tar.gz` & `tmp/AsyncIRCClient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsyncIRCClient-0.0.3.tar", last modified: Wed Jun 14 12:28:35 2023, max compression
+gzip compressed data, was "AsyncIRCClient-0.0.4.tar", last modified: Wed Jun 14 13:58:15 2023, max compression
```

## Comparing `AsyncIRCClient-0.0.3.tar` & `AsyncIRCClient-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 12:28:35.600429 AsyncIRCClient-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-14 12:28:35.597432 AsyncIRCClient-0.0.3/AsyncIRCClient.egg-info/
--rw-rw-rw-   0        0        0     1339 2023-06-14 12:28:35.000000 AsyncIRCClient-0.0.3/AsyncIRCClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-14 12:28:35.000000 AsyncIRCClient-0.0.3/AsyncIRCClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 12:28:35.000000 AsyncIRCClient-0.0.3/AsyncIRCClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 12:28:35.000000 AsyncIRCClient-0.0.3/AsyncIRCClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 12:28:35.000000 AsyncIRCClient-0.0.3/AsyncIRCClient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1339 2023-06-14 12:28:35.599430 AsyncIRCClient-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 12:28:35.598431 AsyncIRCClient-0.0.3/async_irc_client/
--rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.3/async_irc_client/__init__.py
--rw-rw-rw-   0        0        0    32342 2023-06-14 12:28:08.000000 AsyncIRCClient-0.0.3/async_irc_client/async_irc_client.py
--rw-rw-rw-   0        0        0       42 2023-06-14 12:28:35.600429 AsyncIRCClient-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      460 2023-06-14 12:28:08.000000 AsyncIRCClient-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:58:15.512573 AsyncIRCClient-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:58:15.510490 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/
+-rw-rw-rw-   0        0        0     1339 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1339 2023-06-14 13:58:15.512573 AsyncIRCClient-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 13:58:15.511574 AsyncIRCClient-0.0.4/async_irc_client/
+-rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.4/async_irc_client/__init__.py
+-rw-rw-rw-   0        0        0    32657 2023-06-14 13:57:07.000000 AsyncIRCClient-0.0.4/async_irc_client/async_irc_client.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 13:58:15.513574 AsyncIRCClient-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      460 2023-06-14 13:57:29.000000 AsyncIRCClient-0.0.4/setup.py
```

### Comparing `AsyncIRCClient-0.0.3/AsyncIRCClient.egg-info/PKG-INFO` & `AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.3
+Version: 0.0.4
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
```

### Comparing `AsyncIRCClient-0.0.3/PKG-INFO` & `AsyncIRCClient-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.3
+Version: 0.0.4
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
```

### Comparing `AsyncIRCClient-0.0.3/README.md` & `AsyncIRCClient-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `AsyncIRCClient-0.0.3/async_irc_client/async_irc_client.py` & `AsyncIRCClient-0.0.4/async_irc_client/async_irc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,19 +678,28 @@
     def _send_ping(self) -> None:
         """
         send pong response
         :returns: None
         """
         self.send_irc_data("PING :tmi.twitch.tv")
 
+    def _on_pong(self) -> None:
+        """
+        on pong received
+        :return: None
+        """
+        self._pong_response_timer.cancel()
+
     def _reconnect(self) -> None:
         """
         reconnect to server
         :returns: None
         """
+        self._pong_response_timer.cancel()
+        self._disconnect_timer.cancel()
 
         def wrapper():
             self._transport.close()
             pending_tasks = asyncio.all_tasks(self._loop)
             for task in pending_tasks:
                 logger.warning(f"Stopping task {task}")
                 task.cancel()
@@ -733,14 +742,15 @@
 
     async def _on_disconnect_timer_timeout(self) -> None:
         """
         on disconnect timer times out
         :return: None
         """
         self._send_ping()
+        self._pong_response_timer.start()
 
     async def _on_pong_response_timer_timeout(self) -> None:
         """
         on pong response timer times out
         :return: None
         """
         self._reconnect()
@@ -843,14 +853,15 @@
                 callback = self.on_global_user_state
 
             case "PING":
                 self._send_pong()
                 callback = self.on_ping
 
             case "PONG":
+                self._on_pong()
                 callback = self.on_pong
 
             case "RECONNECT":
                 self._reconnect()
                 callback = self.on_reconnect
 
             case "USERNOTICE":
```

