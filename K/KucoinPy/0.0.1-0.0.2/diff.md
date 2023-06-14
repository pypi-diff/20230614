# Comparing `tmp/KucoinPy-0.0.1.tar.gz` & `tmp/KucoinPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KucoinPy-0.0.1.tar", last modified: Sun Jun 11 17:57:36 2023, max compression
+gzip compressed data, was "KucoinPy-0.0.2.tar", last modified: Wed Jun 14 18:24:35 2023, max compression
```

## Comparing `KucoinPy-0.0.1.tar` & `KucoinPy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-11 17:57:36.432055 KucoinPy-0.0.1/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-11 17:57:36.429449 KucoinPy-0.0.1/KucoinPy/
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-06-11 17:55:30.000000 KucoinPy-0.0.1/KucoinPy/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      860 2023-06-04 20:07:32.000000 KucoinPy-0.0.1/KucoinPy/classes.py
--rwxrwxrwx   0 root         (0) root         (0)     3314 2023-06-11 10:07:52.000000 KucoinPy-0.0.1/KucoinPy/http.py
--rwxrwxrwx   0 root         (0) root         (0)    19353 2023-06-11 17:56:25.000000 KucoinPy-0.0.1/KucoinPy/wrapper.py
--rwxrwxrwx   0 root         (0) root         (0)     1937 2023-05-28 08:51:12.000000 KucoinPy-0.0.1/KucoinPy/ws.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-11 17:57:36.431305 KucoinPy-0.0.1/KucoinPy.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4783 2023-06-11 17:57:36.000000 KucoinPy-0.0.1/KucoinPy.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-06-11 17:57:36.000000 KucoinPy-0.0.1/KucoinPy.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-11 17:57:36.000000 KucoinPy-0.0.1/KucoinPy.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-06-11 17:57:36.000000 KucoinPy-0.0.1/KucoinPy.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-11 17:57:36.000000 KucoinPy-0.0.1/KucoinPy.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)    18092 2023-06-08 16:53:44.000000 KucoinPy-0.0.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     4783 2023-06-11 17:57:36.431792 KucoinPy-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4291 2023-06-11 17:56:10.000000 KucoinPy-0.0.1/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-11 17:57:36.432142 KucoinPy-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      698 2023-06-11 17:57:25.000000 KucoinPy-0.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 18:24:35.887347 KucoinPy-0.0.2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 18:24:35.885065 KucoinPy-0.0.2/KucoinPy/
+-rwxrwxrwx   0 root         (0) root         (0)      117 2023-06-11 17:55:30.000000 KucoinPy-0.0.2/KucoinPy/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      860 2023-06-04 20:07:32.000000 KucoinPy-0.0.2/KucoinPy/classes.py
+-rwxrwxrwx   0 root         (0) root         (0)     3314 2023-06-11 10:07:52.000000 KucoinPy-0.0.2/KucoinPy/http.py
+-rwxrwxrwx   0 root         (0) root         (0)    19127 2023-06-14 18:22:20.000000 KucoinPy-0.0.2/KucoinPy/wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1937 2023-05-28 08:51:12.000000 KucoinPy-0.0.2/KucoinPy/ws.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 18:24:35.886661 KucoinPy-0.0.2/KucoinPy.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4875 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)    18092 2023-06-08 16:53:44.000000 KucoinPy-0.0.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     4875 2023-06-14 18:24:35.887087 KucoinPy-0.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4291 2023-06-11 17:56:10.000000 KucoinPy-0.0.2/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-14 18:24:35.887424 KucoinPy-0.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      789 2023-06-14 18:24:06.000000 KucoinPy-0.0.2/setup.py
```

### Comparing `KucoinPy-0.0.1/KucoinPy/classes.py` & `KucoinPy-0.0.2/KucoinPy/classes.py`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.1/KucoinPy/http.py` & `KucoinPy-0.0.2/KucoinPy/http.py`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.1/KucoinPy/wrapper.py` & `KucoinPy-0.0.2/KucoinPy/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,15 +406,15 @@
                 self.sockets.append(HTTP(self.kc_api_key, self.kc_api_secret, self.kc_api_passphrase))
             time.sleep(0.5)  # not spam :)
 
     def calc_lots(self, raw: str, lot_size: str) -> str:
         return raw[: len(raw.split(".")[0]) + 1 + len(lot_size.split(".")[1])]
 
     def order(self, order: Order, autosplit: int = 1, response=False, sock=None) -> str:
-        sock = sock or self.order_socks.pop()
+        sock = sock or self.sockets.pop()
         if autosplit > 6 or autosplit < 1:
             return "bad autosplit"
 
         base = order.symbol.split("-")[0]
 
         if order.type == "limit":
             order.price = self.calc_lots(str(order.price), self.lots[base]["price_lot"])
@@ -424,74 +424,71 @@
             try:
                 order.funds = self.calc_lots(str(float(order.funds)), self.lots[base]["coin_lot"])
             except:
                 try:
                     order.size = self.calc_lots(str(float(order.size)), self.lots[base]["coin_lot"])
                 except:
                     pass
-            return self.single_order(order, sock, response)
+            return self._single_order(order, sock, response)
 
         if len(orders) == 1:
-            return self.single_order(orders[0], sock, response)
+            return self._single_order(orders[0], sock, response)
         else:
-            return self.multi_order(orders, sock, response)
+            return self._multi_order(orders, sock, response)
 
-    def single_order(self, order: Order, sock, response=False) -> Union[bool, Response]:
-        for i in range(3):
-            try:
-                sock.send(
-                    method="POST",
-                    location="/api/v1/hf/orders",
-                    payload=order.__dict__,
-                )
-                if response:
-                    return sock.recv()
-
-                return True
-            except Exception as e:
-                self.logger.log(
-                    "WARNING",
-                    "Kucoin Client",
-                    msg="Failed to place order",
-                    extras={
-                        "error": str(e),
-                        "traceback": traceback.format_exc(),
-                        "dumped": order.__dict__,
-                    },
-                )
-                continue
-
-        return "end of single_order"
-
-    def multi_order(self, orders: List[Order], sock, response=False) -> Union[bool, Response]:
+    def _single_order(self, order: Order, sock, response=False) -> Union[bool, Response]:
+        try:
+            sock.send(
+                method="POST",
+                location="/api/v1/hf/orders",
+                payload=order.__dict__,
+            )
+            if response:
+                return sock.recv()
+
+            return True
+        except Exception as e:
+            self.logger.log(
+                "WARNING",
+                "Kucoin Client",
+                msg="Failed to place order",
+                extras={
+                    "error": str(e),
+                    "traceback": traceback.format_exc(),
+                    "dumped": order.__dict__,
+                },
+            )
+            return
+
+    def _multi_order(self, orders: List[Order], sock, response=False) -> Union[bool, Response]:
+        for order in orders:
+            order.clientOid = uuid.uuid4().hex
         payload = {"symbol": orders[0].symbol, "orderList": [i.__dict__ for i in orders]}
-        for i in range(3):
-            try:
-                sock.send(
-                    method="POST",
-                    location="/api/v1/hf/orders/multi",
-                    payload=payload,
-                )
-                if response:
-                    return sock.recv()
-                return True
-            except Exception as e:
-                self.logger.log(
-                    "WARNING",
-                    "Kucoin Client",
-                    msg="Failed to place order",
-                    extras={
-                        "error": str(e),
-                        "traceback": traceback.format_exc(),
-                        "payload": payload,
-                    },
-                )
-                continue
+        try:
+            sock.send(
+                method="POST",
+                location="/api/v1/hf/orders/multi",
+                payload=payload,
+            )
+            if response:
+                return sock.recv()
+            return True
+        except Exception as e:
+            self.logger.log(
+                "WARNING",
+                "Kucoin Client",
+                msg="Failed to place order",
+                extras={
+                    "error": str(e),
+                    "traceback": traceback.format_exc(),
+                    "payload": payload,
+                },
+            )
+            return
 
-        return "end of multi_order"
 
     def cancel_all(self, symbol, retries=5, response=False):
         for i in range(retries):
             try:
                 sock = self.sockets.pop()
                 sock.send(
                     method="DELETE",
```

### Comparing `KucoinPy-0.0.1/KucoinPy/ws.py` & `KucoinPy-0.0.2/KucoinPy/ws.py`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.1/KucoinPy.egg-info/PKG-INFO` & `KucoinPy-0.0.2/KucoinPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: KucoinPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Probably the fastest kucoin API wrapper in python
 Home-page: https://www.github.com/PrivatePandaCO/KucoinPy
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: GNU GENERAL PUBLIC LICENSE Version 2
 Project-URL: Documentation, https://github.com/PrivatePandaCO/KucoinPy/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/KucoinPy
+Project-URL: Changelog, https://github.com/PrivatePandaCO/KucoinPy/blob/master/changelog.md
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KucoinPy (KCW)
 The stuff that speeds my crypto trading bots. My very own kucoin API wrapper in python, using sockets and conversing with the new HFT endpoints
 
 ### WIP Warning
```

### Comparing `KucoinPy-0.0.1/LICENSE` & `KucoinPy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.1/PKG-INFO` & `KucoinPy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: KucoinPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Probably the fastest kucoin API wrapper in python
 Home-page: https://www.github.com/PrivatePandaCO/KucoinPy
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: GNU GENERAL PUBLIC LICENSE Version 2
 Project-URL: Documentation, https://github.com/PrivatePandaCO/KucoinPy/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/KucoinPy
+Project-URL: Changelog, https://github.com/PrivatePandaCO/KucoinPy/blob/master/changelog.md
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KucoinPy (KCW)
 The stuff that speeds my crypto trading bots. My very own kucoin API wrapper in python, using sockets and conversing with the new HFT endpoints
 
 ### WIP Warning
```

### Comparing `KucoinPy-0.0.1/README.md` & `KucoinPy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.1/setup.py` & `KucoinPy-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from distutils.core import setup
 
 setup(
     name="KucoinPy",
-    version="0.0.1",
+    version="0.0.2",
     description="Probably the fastest kucoin API wrapper in python",
     author="Parth Mittal",
     author_email="parth@privatepanda.co",
     url="https://www.github.com/PrivatePandaCO/KucoinPy",
     license="GNU GENERAL PUBLIC LICENSE Version 2",
     packages=["KucoinPy"],
     install_requires=["orjson", "requests", "pyloggor"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     project_urls={
         "Documentation": "https://github.com/PrivatePandaCO/KucoinPy/blob/master/README.md",
         "Github": "https://github.com/PrivatePandaCO/KucoinPy",
+        "Changelog": "https://github.com/PrivatePandaCO/KucoinPy/blob/master/changelog.md"
     },
 )
```

