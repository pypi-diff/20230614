# Comparing `tmp/pytlgateway-0.2.8.tar.gz` & `tmp/pytlgateway-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/impl-pytg/impl-pytg/dist/.tmp-a3k5v17s/pytlgateway-0.2.8.tar", last modified: Thu Mar  9 08:28:07 2023, max compression
+gzip compressed data, was "/__w/impl-pytg/impl-pytg/dist/.tmp-9qesugv7/pytlgateway-0.2.9.tar", last modified: Fri Mar 17 00:42:22 2023, max compression
```

## Comparing `pytlgateway-0.2.8.tar` & `pytlgateway-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/
--rw-r--r--   0 root         (0) root         (0)      720 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pyatxgateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pyatxgateway/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31765 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pyatxgateway/atx_server.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pyatxgateway/constants.py
--rw-r--r--   0 root         (0) root         (0)     6002 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pyatxgateway/logger.py
--rw-r--r--   0 root         (0) root         (0)     9459 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pyatxgateway/mongo_client_gateway.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pyatxgateway/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pytlgateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pytlgateway/__init__.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pytlgateway/constants.py
--rw-r--r--   0 root         (0) root         (0)    62800 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pytlgateway/ft_server.py
--rw-r--r--   0 root         (0) root         (0)    47156 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pytlgateway/ft_tool.py
--rw-r--r--   0 root         (0) root         (0)     6002 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pytlgateway/logger.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/pytlgateway/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pytlgateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)      720 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pytlgateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pytlgateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pytlgateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pytlgateway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/pytlgateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 08:28:07.000000 pytlgateway-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1116 2023-03-09 08:27:39.000000 pytlgateway-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       15 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pyatxgateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pyatxgateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31765 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pyatxgateway/atx_server.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pyatxgateway/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pyatxgateway/logger.py
+-rw-r--r--   0 root         (0) root         (0)     9439 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pyatxgateway/mongo_client_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pyatxgateway/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pytlgateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pytlgateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pytlgateway/constants.py
+-rw-r--r--   0 root         (0) root         (0)    63267 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pytlgateway/ft_server.py
+-rw-r--r--   0 root         (0) root         (0)    47126 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pytlgateway/ft_tool.py
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pytlgateway/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/pytlgateway/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pytlgateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pytlgateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pytlgateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pytlgateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pytlgateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/pytlgateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-17 00:42:21.000000 pytlgateway-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-03-17 00:41:46.000000 pytlgateway-0.2.9/setup.py
```

### Comparing `pytlgateway-0.2.8/PKG-INFO` & `pytlgateway-0.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytlgateway
-Version: 0.2.8
+Version: 0.2.9
 Summary: scripts for ft
 Home-page: http://www.puyuan.tech
 Author: puyuan.tech
 Author-email: info@puyuan.tech
 Maintainer: puyuan_staff
 Maintainer-email: github@puyuan.tech
 License: MIT License
```

### Comparing `pytlgateway-0.2.8/pyatxgateway/atx_server.py` & `pytlgateway-0.2.9/pyatxgateway/atx_server.py`

 * *Files identical despite different names*

### Comparing `pytlgateway-0.2.8/pyatxgateway/constants.py` & `pytlgateway-0.2.9/pyatxgateway/constants.py`

 * *Files identical despite different names*

### Comparing `pytlgateway-0.2.8/pyatxgateway/logger.py` & `pytlgateway-0.2.9/pyatxgateway/logger.py`

 * *Files identical despite different names*

### Comparing `pytlgateway-0.2.8/pyatxgateway/mongo_client_gateway.py` & `pytlgateway-0.2.9/pyatxgateway/mongo_client_gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,29 +49,29 @@
             try:
                 return func(self,*args, **kwargs)
             except Exception as e:
                 err = traceback.format_exc()
                 exc_type, exc_value, exc_traceback = sys.exc_info()
                 traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
                 self.logger.error(f'[{wrapper}] (exception){err}')
-                self.send_to_feishu(err)
+                self.send_to_user(err)
                 return 'error'
         return wrapper
         
     def load_gateway_setting(self, config_path):
         try:
             #固定配置文件的名字
             config_filename = os.path.join(config_path, 'atx_server_config.json')
             #f = open(config_filename, encoding="utf-8")
             f = open(config_filename, encoding='gbk')
             setting = json.load(f)
             
             log_path = setting['log_filepath']
             self.log_file_path = log_path.replace('/', '\\')
-            self.feishu_url = setting.get('feishu_url')
+            self.url_list = setting.get('url_list')
 
             self.logname = setting['logname']
             self.scan_interval = setting['scan_interval']
             
             self.accounts_config = setting['accounts']
             self.accounts_run = setting['run']
             
@@ -137,15 +137,15 @@
             #for test
             #self.db_client = MongoClient()
             #test for req_position
             #self.db_client_test = MongoClient("127.0.0.1", 27017, connectTimeoutMS=10000)
             #self.test_trading_account = self.db_client_test['tradingAccount']
         except Exception as e:
             err = traceback.format_exc()
-            self.send_to_feishu(err)
+            self.send_to_user(err)
             self.logger.error(f'[init] DB_connect_failed! (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
             exit()
 
     #通过tradingAccount.accountinfo表获取产品属性
     def get_account_info(self):
@@ -163,38 +163,38 @@
             log_accountname = account_info['account_name']
             self.log_account_names[acc] = log_accountname
             target_accountname = tgname + '@' + log_accountname
             self.target_account_names[acc] = target_accountname # 下单时用self
             self.logger.info(
                 f"[get_account_info] (tg_name){self.tgnames} (logacc_name){self.log_account_names} (target_accountnames){self.target_account_names}") 
 
-    def send_to_feishu(self, error):
+    def send_to_user(self, error):
         try:
-            if self.feishu_url == None:
-                self.logger.info("[send_to_feishu] send_message_failed")
+            if self.url_list == None:
+                self.logger.info("[send_to_user] send_message_failed")
                 return
-            url = self.feishu_url
+            url = self.url_list
 
             payload_message = {
                 "msg_type": "text",
                 "content": {
                     "text": f'ERROR! (exception){error}'
                 }
             }
             headers = {
                 'Content-Type': 'application/json'
             }
 
             response = requests.request("POST", url, headers=headers, data=json.dumps(payload_message))
-            self.logger.info(f"[send_to_feishu] (response){response}")
+            self.logger.info(f"[send_to_user] (response){response}")
         except Exception as e:
             err = traceback.format_exc()
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
-            self.logger.error(f'[send_to_feishu] send_message_failed(exception){err}')
+            self.logger.error(f'[send_to_user] send_message_failed(exception){err}')
     
     def signal_handler(self, signum=None, frame=None):
         self.is_stopped = True
     
     def gen_local_id(self):
         self.id_base = 1377779200 * LL9
         self.sp = time.time_ns()
```

### Comparing `pytlgateway-0.2.8/pyatxgateway/utils.py` & `pytlgateway-0.2.9/pyatxgateway/utils.py`

 * *Files identical despite different names*

### Comparing `pytlgateway-0.2.8/pytlgateway/ft_server.py` & `pytlgateway-0.2.9/pytlgateway/ft_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import signal
 import sys
 import traceback
 import getopt
 import argparse
 
 from pymongo import MongoClient, ASCENDING, DESCENDING
-from utils import decode_ft_flag, decode_exchange_id, send_to_feishu
+from utils import decode_ft_flag, decode_exchange_id, send_to_user
 from logger import Logger
 # websocket-client
 
 import websocket
 from websocket import WebSocketApp, ABNF
 
 
@@ -59,15 +59,15 @@
                 db_client.server_info()
                 self.tradelog_db[acc] = db_client["tradingLog"] 
                 
             #for test
             #self.db_client = MongoClient()
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url,msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list,msg=err)
             self.logger.error(f'[init] DB_connect_failed! (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
             exit()
 
         
         #test for req_position
@@ -99,33 +99,35 @@
         # self.sid_to_oid = {} sid可对应多个oid
 
         self.oid_to_ref = {}
         self.ref_to_oid = {}
 
         self.sid_to_req = {}
         self.oid_to_req = {}
+        
+        self.ft_local_id_list = []
 
         self.token = ""
         self.date_change_token = True
 
         self.is_stopped = False
 
     def load_ft_setting(self, config_filename):
         try:
             #f = open(config_filename, encoding="utf-8")
             f = open(config_filename, encoding='gbk')
             setting = json.load(f)
-             
+        
             self.socket_url = setting['websocket_url']
             self.login_url = setting['login_url']
             path = setting['log_filepath']
             self.log_file_path = path.replace('/', '\\')
             self.ft_tradecsv_path = setting['ft_tradecsv_path'].replace('/', '\\')
             self.upload_mudan_url = setting['upload_mudan_url']
-            self.feishu_url = setting.get('feishu_url')
+            self.url_list = setting.get('url_list')
             self.cancel_url = setting['cancel_url']
             # self.log_accountname = setting['ACCOUNT_NAME'] #用于tradinglog数据库,order/trade
             # 产品名称，用于获取tg_name和account_name
             self.req_position_open = setting['req_position_open'] #设置同步持仓的时间
             self.req_position_close = setting['req_position_close']
             #self.tgname = setting['tg_name']
             # self.target_accountname = self.tgname + '@' + self.log_accountname #下单时用
@@ -199,35 +201,35 @@
             while not self.is_stopped:
                 time_now = datetime.now()
                 _dt_endtime = datetime.strptime(self.endtime, "%H:%M")
                 dt_endtime = datetime.combine(time_now, _dt_endtime.time())
                 if time_now > dt_endtime:
                     self.req_position()
                     msg = f"[date_change] close (now){time_now}"
-                    send_to_feishu(logger=self.logger, feishu_url=self.feishu_url,msg=msg)
+                    send_to_user(logger=self.logger, url_list=self.url_list,msg=msg)
                     self.ft_close()         
                 else:
                     self.req_position()
                     self.logger.info(f"[date_change] not_closed (now){time_now}")
                 time.sleep(60)
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url,msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list,msg=err)
             self.logger.error(f'[date_change] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
     
     def ft_close(self):
         self.is_stopped = True
         self.ws.close()
         print (f"[ft_close] (close_time){self.endtime}")
         self.logger.info(f"[ft_close] (close_time){self.endtime}")
         
         msg= f"[ft_close] (close_time){self.endtime}"
-        send_to_feishu(logger=self.logger, feishu_url=self.feishu_url,msg=msg)
+        send_to_user(logger=self.logger, url_list=self.url_list,msg=msg)
         
         os._exit(0)
 
     def req_position(self):
         try:
             for acc in self.accounts_run:
                 target_account_name = self.target_account_names[acc]
@@ -264,15 +266,15 @@
                             query = {'ticker' : ticker, 'trade_acc' : trade_acc, 'target_account_name' : target_account_name}
                             res = ft_position_collection.replace_one(query, position_db_msg, True)
                             self.logger.info(f"[req_position] save_position_info (res){res} (position_db_msg){position_db_msg}")
                 else:
                     self.logger.error(f"[req_position] failed (error_msg){data}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url,msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list,msg=err)
             self.logger.error(f'[req_position] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     # webserver
 
     def on_message(self, ws, message):
@@ -283,15 +285,15 @@
                 self.pong(data)
             elif (data['topic'] == 'Zidan'):
                 self.on_zidan_message(data)
             elif (data['topic'] == 'Mudan'):
                 self.on_mudan_message(data)
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url,msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list,msg=err)
             self.logger.error(f'[on_message] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     def pong(self, data):
         text = {"topic": "Pong", "data": int(data["data"])}
         _text = json.dumps(text)
@@ -374,15 +376,18 @@
                     self.oid_to_traded_money[oid] += amt
                 elif target_type == 'sell':
                     self.oid_to_traded_money[oid] -= amt
 
                 ms = int(msg['update_tm'] / 1000) % 1000
                 update_tm = float(msg['update_tm'] / 1000)
                 local_id = msg['local_id']
+                if local_id in self.ft_local_id_list:
+                    self.logger.error(f"[rtn_trade] ft_local_id_existed! (msg){msg}")
                 trade_time = datetime.utcfromtimestamp(update_tm)
+                
                 trade_ref = local_id
                 exchange = decode_exchange_id(msg['exchange_id'])
                 self.oid_to_req[oid]['exchange_id'] = exchange
                 ticker = msg['stock_code']
                 trade_vol = msg['trade_vol']
                 traded_price = msg['trade_price']
                 db_side = msg['bs_flag']
@@ -454,15 +459,15 @@
                 }
                 ft_trade_query = {"local_id": local_id}
                 res = ft_trade_collection.replace_one(ft_trade_query, trade_db_msg, True)
                 #res = save_trade_collection.insert_one(trade_db_msg)
                 self.logger.info(f"[zidan_message] update_ft_trade (res){res} (local_id){local_id}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url,msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list,msg=err)
             self.logger.error(f'[on_zidan_message] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
             
 
     def update_position(self, msg, order, sid , oid, side, trade_amt):
         try:
@@ -566,15 +571,15 @@
                 query = {'sid': sid,
                          'accountName': accountName}
                 res = position_collection.replace_one(query, position_msg, True)
                 self.logger.info(
                     f"[update_position] (res){res} (msg){position_msg}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[update_position] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     def update_order_filled(self, data, sid, oid):
         try:
             order = self.oid_to_req[oid]
@@ -622,29 +627,29 @@
             res = order_collection.replace_one(
                 query, db_msg, True)  # 覆盖之前的order记录，修改状态
             #db_msg_json = json.dumps(db_msg)
             self.logger.info(
                 f"[on_rtn_filled_order] order_filled (db_res){res} (msg){db_msg}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[update_order_filled] DB_connect_failed! (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     def on_mudan_message(self, data):  # no use
         self.logger.info(f"[on_mudan_message] (mudan){data}")
 
     def on_error(self, ws, error):
         self.logger.error(
             f"[on_error] disconnect (type){type(error)} (msg){error}")
         if type(error) == ConnectionRefusedError or type(error) == ConnectionAbortedError or type(error) == ConnectionResetError or type(error) == websocket._exceptions.WebSocketConnectionClosedException:
             self.reconnect_count += 1
             self.logger.info(f"[on_error] 正在尝试第{self.reconnect_count}次重连")
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=error)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=error)
             if self.reconnect_count < 100:
                 self.ws.close()
                 t = threading.Thread(target=self.run_socket)
                 t.setDaemon(True)
                 t.start()
 
         else:
@@ -710,19 +715,19 @@
             self.logger.info(f"[login] logged (token){self.token} (data){data}")
             for myacc in accs:
                 trade_acc = myacc['trade_acc']
                 self.broker_id[trade_acc] = myacc['broker_id']
                 self.logger.info(f"(trade_acc){trade_acc} broker_id{self.broker_id[trade_acc]}")
             
             _msg = f"[login] logged (token){self.token} (data){data}"
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=_msg)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=_msg)
                 
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[login] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
             exit(0)
 
     def on_open(self, ws):
         self.logger.info(f"[on_open] (ws){ws}")
@@ -789,15 +794,15 @@
                         for sell_target in sell_targets:
                             if sell_target['_id'] not in self.sell_order_dbids:
                                 self.sell_order_dbids.append(sell_target['_id'])
                                 self.req_sell_order_insert(sell_target)
                 time.sleep(self.scan_interval)
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[monitor_algo_order_insert] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
 
 
     def req_buy_order_insert(self, obj: dict):
@@ -818,36 +823,36 @@
 
             begin_time = obj['executionPlan']["start_time"].replace(':', '')
             end_time = obj['executionPlan']["end_time"].replace(':', '')
 
             ft_flag = 'buy'
             row = [stock_code, ft_flag, order_vol, begin_time,
                    end_time, account_id, basket_name]
-            dict = {}
-            dict["basket_name"] = basket_name
-            dict['order_vol'] = order_vol
-            dict['stock_code'] = stock_code
-            dict['begin_time'] = begin_time
-            dict['end_time'] = end_time
-            dict['bs_flag'] = ft_flag
-            dict['trade_acc'] = account_id
+            order_dict = {}
+            order_dict["basket_name"] = basket_name
+            order_dict['order_vol'] = order_vol
+            order_dict['stock_code'] = stock_code
+            order_dict['begin_time'] = begin_time
+            order_dict['end_time'] = end_time
+            order_dict['bs_flag'] = ft_flag
+            order_dict['trade_acc'] = account_id
 
-            mudans = [dict]
+            mudans = [order_dict]
             out = {"mudans": mudans, "token": self.token}
             data = json.dumps(out)
             r = requests.post(self.upload_mudan_url, json=out)
 
             
             text = r.text
             data = json.loads(text)
             
             if data['code'] != 0:
                 self.logger.error(
                     f"[on_buy_req_insert] insert_msg_send_failed (errcode){data['code']} (err_msg){data['data']}")
-                order_msg = dict
+                order_msg = order_dict
                 order_msg['sid'] = sid
                 order_msg['status'] = 'rejected'
                 self.insert_ft_proposed_target(acc, sid, order_msg)
                 
                 acc = self.target_account_names_to_acc[target_account_name]
                 target_collection =  self.order_info_db[acc]['target']
                 delete_query = {
@@ -862,24 +867,24 @@
             db_id = obj['_id']
             ref = data['data'][0]['id']
             status = data['data'][0]['status']
             err_msg = data['data'][0]['status_msg']
             
             
             order_type = obj['executionPlan']["order_type"]
-            dict['order_type'] = order_type
+            order_dict['order_type'] = order_type
             exchange = decode_exchange_id(data['data'][0]['exchange_id'])
-            dict['exchange_id'] = exchange
-            dict['target_account_name'] = target_account_name
+            order_dict['exchange_id'] = exchange
+            order_dict['target_account_name'] = target_account_name
             tgname = target_account_name.split('@', 1)[0]
-            dict['tgname'] = tgname
+            order_dict['tgname'] = tgname
             log_accountname = target_account_name.split('@', 1)[1]
-            dict['log_accountname'] = log_accountname
-            dict['begin_time'] = obj['executionPlan']["start_time"]
-            dict['end_time'] = obj['executionPlan']["end_time"]
+            order_dict['log_accountname'] = log_accountname
+            order_dict['begin_time'] = obj['executionPlan']["start_time"]
+            order_dict['end_time'] = obj['executionPlan']["end_time"]
             ft_proposed_target_collection = self.order_info_db[acc]['ft_proposed_target']
             '''
             返回母单状态：
             1启动 2暂停 3完成 4取消 6废单
             
             '''
             
@@ -908,41 +913,41 @@
                 self.sid_to_traded[sid] = 0
                 self.oid_to_traded[oid] = 0
                 self.oid_to_traded_money[oid] = 0
                 self.oid_to_ref[oid] = ref
                 self.sids.append(sid)
 
                 
-                self.sid_to_req[sid] = dict
-                self.oid_to_req[oid] = dict
+                self.sid_to_req[sid] = order_dict
+                self.oid_to_req[oid] = order_dict
                 self.oid_to_sid[oid] = sid
                 self.db_id_to_oid[db_id] = oid
                 ft_local_ids = []
-                
                 self.ref_to_oid[ref] = oid
+                
                 self.logger.info(
                     f"[on_req_order_insert] order_insert_success! (response){text} (ref){ref}")
                 self.rtn_order_insert(sid, oid, exchange)
                 #ft_order用于恢复
                 ft_order_collection = self.order_info_db[acc]['ft_order']
                 db_msg = {
                     "oid" : oid,
                     "sid" : sid,
                     "mudan_id" : ref,
                     "local_ids" : ft_local_ids,
                     'log_accountname' : log_accountname,
                     "traded_vol" : 0,
                     "traded_amt" : 0,
-                    "order_msg": dict
+                    "order_msg": order_dict
                 }
                 query = {"oid": oid}
                 res = ft_order_collection.replace_one(query, db_msg, True)
                 self.logger.info(f"[on_req_order_insert] insert_ft_order_info (res){res} (msg){db_msg}")
                 
-                order_msg = dict
+                order_msg = order_dict
                 order_msg['sid'] = sid
                 order_msg['status'] = 'inserted'
                 self.insert_ft_proposed_target(acc,sid,order_msg)
                 
                 acc = self.target_account_names_to_acc[target_account_name]
                 target_collection =  self.order_info_db[acc]['target']
                 delete_query = {
@@ -952,28 +957,28 @@
                     'volume' : vol
                 }
                 delete_res = target_collection.delete_one(delete_query)
                 self.logger.info(f"[on_req_buy_order] delete (target){obj}")
             
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[req_buy_order_insert] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
     
     def insert_ft_proposed_target(self, acc, sid, order_msg:dict):
         try:
             ft_proposed_target_collection = self.order_info_db[acc]['ft_proposed_target']
             insert_query = {'sid' : sid, 'target_account_name': order_msg['target_account_name']}
             insert_res = ft_proposed_target_collection.replace_one(insert_query, order_msg, True)
             self.logger.info(f"[on_req_buy_order_insert] ft_proposed_target_collection (insert_res){insert_res} (order_msg){order_msg}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[insert_ft_proposed_target] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     def rtn_order_insert(self, sid, oid, exchange):
         try:
             
@@ -1019,15 +1024,15 @@
             order_collection = self.tradelog_db[acc]['order']
             res = order_collection.insert_one(db_msg)
             #db_msg_json = json.dumps(db_msg)
             self.logger.info(
                 f"[rtn_order_inserted] order_inserted (db_res){res} (db_msg){db_msg}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[rtn_order_insert] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     #not use
     def monitor_sell_order(self):
         try:
@@ -1046,70 +1051,68 @@
                                 self.req_sell_order_insert(sell_target)
                         result = self.orderinfo_db["sell_target"].delete_many(query)
                         self.logger.info(
                             f"[monitor_sell_order] delete{result.deleted_count}messages_by(query){query}")
                 time.sleep(self.scan_interval)
         except Exception as e:
                 err = traceback.format_exc()
-                send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+                send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
                 self.logger.error(f'[rtn_order_insert] (exception){err}')
                 exc_type, exc_value, exc_traceback = sys.exc_info()
                 traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
                 
     def req_sell_order_insert(self, obj: dict):
         try:
             target_account_name = obj['accountName']
             acc = self.target_account_names_to_acc[target_account_name]
             account_id = self.account_id[acc]
             
-
-            dict = {}
-            
+            order_dict = {}
             sid = str(obj['sid'])
             vol = int(obj["volume"])
             order_vol = f'{vol:d}'
             int_stock_code = int(obj['ticker'])
             stock_code = f'{int_stock_code:06d}'
             begin_time = obj['executionPlan']["start_time"].replace(':', '')
             end_time = obj['executionPlan']["end_time"].replace(':', '')
             ft_flag = 'sell'
             basket_name = sid
-            dict["basket_name"] = basket_name
-            dict['order_vol'] = order_vol
-            dict['stock_code'] = stock_code
-            dict['begin_time'] = begin_time
-            dict['end_time'] = end_time
-            dict['bs_flag'] = ft_flag
-            dict['trade_acc'] = account_id
-            mudans = [dict]
+            order_dict["basket_name"] = basket_name
+            order_dict['order_vol'] = order_vol
+            order_dict['stock_code'] = stock_code
+            order_dict['begin_time'] = begin_time
+            order_dict['end_time'] = end_time
+            order_dict['bs_flag'] = ft_flag
+            order_dict['trade_acc'] = account_id
+            mudans = [order_dict]
             out = {"mudans": mudans, "token": self.token}
 
             data = json.dumps(out)
             r = requests.post(self.upload_mudan_url, json=out)
 
             text = r.text
             data = json.loads(text)
             
             order_type = obj['executionPlan']["order_type"]
-            dict['order_type'] = order_type
+            order_dict['order_type'] = order_type
             exchange = decode_exchange_id(data['data'][0]['exchange_id'])
-            dict['target_account_name'] = target_account_name
-            dict['exchange_id'] = exchange
+            order_dict['target_account_name'] = target_account_name
+            order_dict['exchange_id'] = exchange
             tgname = target_account_name.split('@', 1)[0]
-            dict['tgname'] = tgname
+            order_dict['tgname'] = tgname
             log_accountname = target_account_name.split('@', 1)[1]
-            dict['log_accountname'] = log_accountname
-            dict['begin_time'] = obj['executionPlan']["start_time"]
-            dict['end_time'] = obj['executionPlan']["end_time"]
+            order_dict['log_accountname'] = log_accountname
+            order_dict['begin_time'] = obj['executionPlan']["start_time"]
+            order_dict['end_time'] = obj['executionPlan']["end_time"]
             ft_proposed_target_collection = self.order_info_db[acc]['ft_proposed_target']
 
             if data['code'] != 0:
                 self.logger.error(
                     f"[on_req_sell_insert] insert_msg_send_failed (errcode){data['code']} (err_msg){data['data']}")
-                order_msg = dict
+                order_msg = order_dict
                 order_msg['sid'] = sid
                 order_msg['status'] = 'rejected'
                 self.insert_ft_proposed_target(acc, sid, order_msg)
                 
                 acc = self.target_account_names_to_acc[target_account_name]
                 target_collection =  self.order_info_db[acc]['sell_target']
                 delete_query = {
@@ -1126,41 +1129,44 @@
             
             ref = data['data'][0]['id']
             status = data['data'][0]['status']
             err_msg = data['data'][0]['status_msg']
             if status >= 4:
                 self.logger.error(
                     f"[req_sell_order_insert] order_insert_failed! (err_msg){err_msg}")
-                order_msg = dict
+                order_msg = order_dict
                 order_msg['sid'] = sid
                 order_msg['status'] = 'rejected'
                 self.insert_ft_proposed_target(acc, sid, order_msg)
                 
                 acc = self.target_account_names_to_acc[target_account_name]
                 target_collection =  self.order_info_db[acc]['sell_target']
                 delete_query = {
                     'accountName' : target_account_name,
                     'sid' : sid,
                     'ticker' : stock_code,
                     'volume' : vol
                 }
                 delete_res = target_collection.delete_one(delete_query)
-                self.logger.info(f"[on_req_buy_order] delete (target){obj}")
+                self.logger.info(f"[on_req_sell_order] delete (target){obj}")
                 return
             oid = self.gen_order_id()
             self.sid_to_traded[sid] = 0
             self.oid_to_traded[oid] = 0
             self.oid_to_traded_money[oid] = 0
             self.sids.append(sid)
 
-            self.sid_to_req[sid] = dict
-            self.oid_to_req[oid] = dict
+            self.sid_to_req[sid] = order_dict
+            self.oid_to_req[oid] = order_dict
             self.oid_to_ref[oid] = ref
             self.oid_to_sid[oid] = sid
             self.db_id_to_oid[db_id] = oid
+            if ref in self.ref_to_oid:
+                self.logger.error(f"[req_sell_order_insert] trade_ref_exist! (trade_ref){ref}")
+                return
             self.ref_to_oid[ref] = oid
             self.logger.info(
                 f"[on_req_order_insert] order_inserted (response){text} (order_ref){ref}")
             
             self.rtn_order_insert(sid, oid, exchange)
             
             #ft_order用于恢复
@@ -1170,22 +1176,22 @@
                 "oid" : oid,
                 "sid" : sid,
                 "mudan_id" : ref,
                 "local_ids" : ft_local_ids,
                 "log_accountname" : log_accountname,
                 "traded_vol" : 0,
                 "traded_amt" : 0,
-                "order_msg": dict
+                "order_msg": order_dict
             }
             query = {"oid": oid}
             res = collection.replace_one(query, db_msg, True)
             self.logger.info(f"[on_req_order_insert] insert_ft_order_info (res){res} (msg){db_msg}")
             
             
-            order_msg = dict
+            order_msg = order_dict
             order_msg['sid'] = sid
             order_msg['status'] = 'inserted'
             self.insert_ft_proposed_target(acc, sid, order_msg)
             #delete sell_target
             acc = self.target_account_names_to_acc[target_account_name]
             target_collection =  self.order_info_db[acc]['sell_target']
             delete_query = {
@@ -1194,15 +1200,15 @@
                 'ticker' : stock_code,
                 'volume' : vol
             }
             delete_res = target_collection.delete_one(delete_query)
             self.logger.info(f"[on_req_buy_order] delete (target){obj}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[req_sell_order_insert] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     def monitor_cancel_order(self):
         try:
             while not self.is_stopped:
@@ -1220,15 +1226,15 @@
                         for cancel_target in cancel_targets:
                             if cancel_target['_id'] not in self.cancel_order_ids:
                                 self.cancel_order_ids.append(cancel_target['_id'])
                                 self.req_cancel_order(cancel_target)
                 time.sleep(self.scan_interval)
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[monitor_cancel_order] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
     def rtn_order_canceled(self, oid, sid):
         try:
             if oid not in self.oid_to_req:
@@ -1281,15 +1287,15 @@
                 query, db_msg, True)  # 覆盖之前的order记录，修改状态
             #res = self.order_collection.insert_one(db_msg)
             #db_msg_json = json.dumps(db_msg)
             self.logger.info(
                 f"[rtn_order_canceled] order_canceled (db_res){res} (db_msg){db_msg}")
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[rtn_order_cancel] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
             
 
     def req_cancel_order(self, obj: dict):
         try:
@@ -1321,15 +1327,15 @@
                 'oid' : oid
             }
             delete_res = target_collection.delete_one(delete_query)
             self.logger.info(f"[on_req_buy_order] delete (target){obj}")
             # cancel success 所以回rtn_order,实际什么时候撤单不确定
         except Exception as e:
             err = traceback.format_exc()
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=err)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=err)
             self.logger.error(f'[req_cancel_order] (exception){err}')
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
 
 
 if __name__ == "__main__":
```

### Comparing `pytlgateway-0.2.8/pytlgateway/ft_tool.py` & `pytlgateway-0.2.9/pytlgateway/ft_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import traceback
 import getopt
 import argparse
 from pathlib import Path
 import requests
 
 from pymongo import MongoClient, ASCENDING, DESCENDING
-from utils import decode_ft_flag,  decode_exchange_id, send_to_feishu
+from utils import decode_ft_flag,  decode_exchange_id, send_to_user
 from logger import Logger
 
 
 class FtTool(object): 
     
     def __init__(self, config_filename, update_trade_date, sync_pos, sync_trade, sync_add, sync_trade_in_trading):
         self.load_ft_setting(config_filename)
@@ -72,15 +72,15 @@
             self.socket_url = setting['websocket_url']
             self.login_url = setting['login_url']
             path = setting['log_filepath']
             self.log_file_path = path.replace('/', '\\')
             self.ft_tradecsv_path = setting['ft_tradecsv_path'].replace('/', '\\')
             self.ft_zidan_message_path = setting['ft_zidan_message_path'].replace('/', '\\')
             self.upload_mudan_url = setting['upload_mudan_url']
-            self.feishu_url = setting.get('feishu_url')
+            self.url_list = setting.get('url_list')
             self.cancel_url = setting['cancel_url']
             # self.log_accountname = setting['ACCOUNT_NAME'] #用于tradinglog数据库,order/trade
             # 产品名称，用于获取tg_name和account_name
             self.sync_position_open = setting['sync_position_open'] #设置同步持仓的时间
             self.sync_position_close = setting['sync_position_close']
             #self.tgname = setting['tg_name']
             # self.target_accountname = self.tgname + '@' + self.log_accountname #下单时用
@@ -160,31 +160,31 @@
     def start(self):
         
         #trade_export_path = r'C:\Users\Administrator\Downloads\ft_client_win_1.6.4\ft_client_win\export\20221201\20221201_326000024361_trade.csv'
         if self.sync_trade == True:
             self.logger.info(f"in get_trade")
             self.get_trade_from_csv()
             _msg = "[get_trade_from_csv] executed"
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=_msg)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=_msg)
             
             
         if self.sync_trade_in_trading == True:
             self.get_trade_from_csv_in_trading()
             _msg = "[get_trade_from_csv_in_trading] executed"
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=_msg)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=_msg)
         
         if self.sync_pos == True:
             self.date_change()
             _msg = "[date_change] executed"
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=_msg)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=_msg)
         
         if self.sync_add == True:
             self.sync_position_add()
             _msg = "[sync_add] executed"   
-            send_to_feishu(logger=self.logger, feishu_url=self.feishu_url, msg=_msg)
+            send_to_user(logger=self.logger, url_list=self.url_list, msg=_msg)
         
     def get_trade_from_csv(self):
         try:
             #delete old trade msgs
             for acc in self.accounts_run:
                 ft_sync_trade_collection = self.order_info_db[acc]['ft_sync_trade']
                 del_res = ft_sync_trade_collection.delete_many({})
```

### Comparing `pytlgateway-0.2.8/pytlgateway/logger.py` & `pytlgateway-0.2.9/pytlgateway/logger.py`

 * *Files identical despite different names*

### Comparing `pytlgateway-0.2.8/pytlgateway/utils.py` & `pytlgateway-0.2.9/pytlgateway/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -54,31 +54,44 @@
     num = str(os.environ.get(env_name))
     return int(num) if num.isdigit() else default_num
 
 def get_log_given_path(path):
     dirs = os.path.join(path)
     return path
 
-def send_to_feishu(logger, feishu_url, msg):
+def send_to_user(logger, url_list, msg):
         try:
-            if feishu_url == None:
-                logger.info("[send_to_feishu] send_message_failed")
+            if len(url_list) == 0:
+                logger.info("[send_to_user] send_message_failed")
                 return
-            url = feishu_url
-
-            payload_message = {
+            
+            payload_message_feishu = {
                 "msg_type": "text",
                 "content": {
                     "text": msg
                 }
             }
+            
             headers = {
                 'Content-Type': 'application/json'
             }
-
-            response = requests.request("POST", url, headers=headers, data=json.dumps(payload_message))
-            logger.info(f"[send_to_feishu] (response){response}")
+            
+            payload_message_dingding = {
+                "msgtype": "text",
+                "text": {"content": msg},
+                "at": {
+                    "atMobiles": [""],
+                    "isAtAll": "false"  # @所有人 时为true，上面的atMobiles就失效了
+                }
+            }
+            response = requests.request("POST", url_list[0], headers=headers, data=json.dumps(payload_message_feishu))
+            data = response.json()
+            logger.info(f"[send_to_user] (response){response} (data){data}")
+            if len(url_list) > 1: 
+                response_ding = requests.request("POST", url_list[1], headers=headers, data=json.dumps(payload_message_dingding))
+                data_ding = response_ding.json()
+                logger.info(f"[send_to_user] (response){response_ding} (data){data_ding}")
         except Exception as e:
             err = traceback.format_exc()
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback, limit=None, file=sys.stdout)
-            logger.error(f'[send_to_feishu] send_message_failed(exception){err}')
+            logger.error(f'[send_to_user] send_message_failed(exception){err}')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytlgateway-0.2.8/pytlgateway.egg-info/PKG-INFO` & `pytlgateway-0.2.9/pytlgateway.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytlgateway
-Version: 0.2.8
+Version: 0.2.9
 Summary: scripts for ft
 Home-page: http://www.puyuan.tech
 Author: puyuan.tech
 Author-email: info@puyuan.tech
 Maintainer: puyuan_staff
 Maintainer-email: github@puyuan.tech
 License: MIT License
```

### Comparing `pytlgateway-0.2.8/setup.py` & `pytlgateway-0.2.9/setup.py`

 * *Files identical despite different names*

