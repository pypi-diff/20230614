# Comparing `tmp/pytebis-0.5.11.tar.gz` & `tmp/pytebis-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\dev\pytebis_dev\pytebis\dist\.tmp-rpczfjch\pytebis-0.5.11.tar", last modified: Wed Jun 14 08:58:20 2023, max compression
+gzip compressed data, was "C:\dev\pytebis_dev\pytebis\dist\tmpxh2ht_hp\pytebis-0.5.2.tar", last modified: Wed Aug  4 12:15:59 2021, max compression
```

## Comparing `pytebis-0.5.11.tar` & `pytebis-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:58:20.562638 pytebis-0.5.11/
--rw-rw-rw-   0        0        0     1085 2021-08-03 12:59:02.000000 pytebis-0.5.11/LICENSE
--rw-rw-rw-   0        0        0     7228 2023-06-14 08:58:20.562638 pytebis-0.5.11/PKG-INFO
--rw-rw-rw-   0        0        0     6654 2023-06-14 08:50:19.000000 pytebis-0.5.11/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:58:20.534632 pytebis-0.5.11/pytebis/
--rw-rw-rw-   0        0        0       33 2021-08-03 12:59:02.000000 pytebis-0.5.11/pytebis/__init__.py
--rw-rw-rw-   0        0        0     1468 2021-08-03 12:59:02.000000 pytebis-0.5.11/pytebis/lazyloader.py
--rw-rw-rw-   0        0        0      289 2023-06-14 08:35:50.000000 pytebis-0.5.11/pytebis/main.py
--rw-rw-rw-   0        0        0    46176 2023-06-14 08:26:36.000000 pytebis-0.5.11/pytebis/tebis.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:58:20.558632 pytebis-0.5.11/pytebis.egg-info/
--rw-rw-rw-   0        0        0     7228 2023-06-14 08:58:20.000000 pytebis-0.5.11/pytebis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-14 08:58:20.000000 pytebis-0.5.11/pytebis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:58:20.000000 pytebis-0.5.11/pytebis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-14 08:58:20.000000 pytebis-0.5.11/pytebis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 08:58:20.000000 pytebis-0.5.11/pytebis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-14 08:58:20.568631 pytebis-0.5.11/setup.cfg
--rw-rw-rw-   0        0        0     1777 2023-06-14 08:48:06.000000 pytebis-0.5.11/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-04 12:15:59.138290 pytebis-0.5.2/
+-rw-rw-rw-   0        0        0     1085 2021-08-03 12:59:02.000000 pytebis-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0     6820 2021-08-04 12:15:59.139289 pytebis-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6071 2021-08-03 14:27:19.000000 pytebis-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2021-08-04 12:15:59.105287 pytebis-0.5.2/pytebis/
+-rw-rw-rw-   0        0        0       33 2021-08-03 12:59:02.000000 pytebis-0.5.2/pytebis/__init__.py
+-rw-rw-rw-   0        0        0     1468 2021-08-03 12:59:02.000000 pytebis-0.5.2/pytebis/lazyloader.py
+-rw-rw-rw-   0        0        0    40960 2021-08-04 12:15:03.000000 pytebis-0.5.2/pytebis/tebis.py
+drwxrwxrwx   0        0        0        0 2021-08-04 12:15:59.137315 pytebis-0.5.2/pytebis.egg-info/
+-rw-rw-rw-   0        0        0     6820 2021-08-04 12:15:59.000000 pytebis-0.5.2/pytebis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2021-08-04 12:15:59.000000 pytebis-0.5.2/pytebis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-04 12:15:59.000000 pytebis-0.5.2/pytebis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2021-08-04 12:15:59.000000 pytebis-0.5.2/pytebis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-08-04 12:15:59.000000 pytebis-0.5.2/pytebis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2021-08-04 12:15:59.141290 pytebis-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1927 2021-08-04 12:15:40.000000 pytebis-0.5.2/setup.py
```

### Comparing `pytebis-0.5.11/LICENSE` & `pytebis-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytebis-0.5.11/PKG-INFO` & `pytebis-0.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: pytebis
-Version: 0.5.11
+Version: 0.5.2
 Summary: Python Connector for TeBIS from Steinhaus
 Home-page: https://github.com/MrLight/pytebis
 Author: MrLight
 Author-email: mrlight1@gmx.de
 License: mit
 Keywords: Python,Connector,TeBIS,Steinhaus
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytebis Python Connector for TeBIS from Steinhaus
 
 pytebis is a connector for interacting with a TeBIS Server.
 
@@ -80,30 +84,22 @@
 
 There are different functions to read data from the TeBIS Server. All functions have the some parameters. Only the return is specific to the function.
 Parameters:
 
 `result = teb.getDataAsJson(names, start, end, rate=1)`
 
 - names = Array of all mst-names to read. You can pass a array of IDs, names, TebisMst-Objects or Group-Objects (even mixed).
-- start = Unix-Timestamp where to start the read
-          - or -
-          Unix-Timestamp in microsecond precision
-          - or - 
-          float value where the fraction is the microseconds part
+- start = Unix-Timestamp where to start the read 
           - or -
           DateTimeObject
           - or -
           String in Format '%Y-%m-%d %H:%M:%S.%f'
           (always the same timezone as the server is)
 - end = Unix-Timestamp where to end the read
           - or -
-          Unix-Timestamp in microsecond precision
-          - or - 
-          float value where the fraction is the microseconds part
-          - or -
           DateTimeObject
           - or -
           String in Format '%Y-%m-%d %H:%M:%S.%f'
           (always the same timezone as the server is)
 - rate = What reduction should be used for the read. If your System supports Values smaller than 1second use Fractions of Seconds. eg: 0.1 for 100ms
 
 The Data which is returned by the TeBIS-Server is vectorized into a structured numpy array. Which is working super fast and is totally comparable with the performance of the TeBIS A Client. You can use different functions to get the data in std. Python formats for further analysis.
@@ -118,38 +114,23 @@
 You can directly access the elements e.g. by indexing them by name `resNP["timestamp"]`
 
 #### as Pandas
 
 ```python
 df = teb.getDataAsPD(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
 ```
-will return a pandas dataframe
-
-
-```python
-df = teb.getDataAsPD([13, 14, 15, 16],  [[1626779900,1626779930],[1626779950,1626779960]],1)
-```
-
-The Pandas Function can even handel multiple slices of timeframes by adding start and endpoint into an array.
-
 
+The Pandas DataFrame will not return a column with the timestamp. But a DateTimeIndex. So you can directly use this for TimeSeries Operations. The creation of the Pandas Dataframe is a bit slower than the generic NumPy function, as the DataFrame and the DateTimeIndex is generated afterwards.
 
 #### as Json
 
 ```python
 resJSON = teb.getDataAsJson(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
 ```
 
-#### as RawValues
-
-```python
-resJSON = teb.getDataRAW(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
-```
-Returns the raw tebis socket data. This could be used if the value calculation should happen on the clientside. e.g. if you want to save bandwidth and gain speed in a client server setup.
-
 #### Example
 
 This will show a plot containing the last hour of data of the point-ids 1 and 2. The reduction is 10 seconds.
 
 ```python
 import time
 import matplotlib.pyplot as plt
@@ -180,7 +161,9 @@
 
 Just call ```teb.refreshMsts()``` to reload the data.
 
 
 ### Logging
 
 The package is implementing a logger using the std. logging framework of Python. The loggername is: ```pytebis```. There is no handler configured. To setup a specific log-level for the package use a config like this after ```logging.basicConfig()``` e.g. ```logging.getLogger('pytebis').setLevel(logging.INFO)``` 
+
+
```

### Comparing `pytebis-0.5.11/README.md` & `pytebis-0.5.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -63,30 +63,22 @@
 
 There are different functions to read data from the TeBIS Server. All functions have the some parameters. Only the return is specific to the function.
 Parameters:
 
 `result = teb.getDataAsJson(names, start, end, rate=1)`
 
 - names = Array of all mst-names to read. You can pass a array of IDs, names, TebisMst-Objects or Group-Objects (even mixed).
-- start = Unix-Timestamp where to start the read
-          - or -
-          Unix-Timestamp in microsecond precision
-          - or - 
-          float value where the fraction is the microseconds part
+- start = Unix-Timestamp where to start the read 
           - or -
           DateTimeObject
           - or -
           String in Format '%Y-%m-%d %H:%M:%S.%f'
           (always the same timezone as the server is)
 - end = Unix-Timestamp where to end the read
           - or -
-          Unix-Timestamp in microsecond precision
-          - or - 
-          float value where the fraction is the microseconds part
-          - or -
           DateTimeObject
           - or -
           String in Format '%Y-%m-%d %H:%M:%S.%f'
           (always the same timezone as the server is)
 - rate = What reduction should be used for the read. If your System supports Values smaller than 1second use Fractions of Seconds. eg: 0.1 for 100ms
 
 The Data which is returned by the TeBIS-Server is vectorized into a structured numpy array. Which is working super fast and is totally comparable with the performance of the TeBIS A Client. You can use different functions to get the data in std. Python formats for further analysis.
@@ -101,38 +93,23 @@
 You can directly access the elements e.g. by indexing them by name `resNP["timestamp"]`
 
 #### as Pandas
 
 ```python
 df = teb.getDataAsPD(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
 ```
-will return a pandas dataframe
-
-
-```python
-df = teb.getDataAsPD([13, 14, 15, 16],  [[1626779900,1626779930],[1626779950,1626779960]],1)
-```
-
-The Pandas Function can even handel multiple slices of timeframes by adding start and endpoint into an array.
-
 
+The Pandas DataFrame will not return a column with the timestamp. But a DateTimeIndex. So you can directly use this for TimeSeries Operations. The creation of the Pandas Dataframe is a bit slower than the generic NumPy function, as the DataFrame and the DateTimeIndex is generated afterwards.
 
 #### as Json
 
 ```python
 resJSON = teb.getDataAsJson(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
 ```
 
-#### as RawValues
-
-```python
-resJSON = teb.getDataRAW(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
-```
-Returns the raw tebis socket data. This could be used if the value calculation should happen on the clientside. e.g. if you want to save bandwidth and gain speed in a client server setup.
-
 #### Example
 
 This will show a plot containing the last hour of data of the point-ids 1 and 2. The reduction is 10 seconds.
 
 ```python
 import time
 import matplotlib.pyplot as plt
```

### Comparing `pytebis-0.5.11/pytebis/lazyloader.py` & `pytebis-0.5.2/pytebis/lazyloader.py`

 * *Files identical despite different names*

### Comparing `pytebis-0.5.11/pytebis/tebis.py` & `pytebis-0.5.2/pytebis/tebis.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,92 +74,41 @@
                     ids.append(member.mst.id)
             elif isinstance(name, TebisGroupMember):
                 id = name.mst.id
             if id is not None:
                 ids.append(id)
         if isinstance(start, datetime.datetime):
             start = start.timestamp()
-        elif isinstance(start, float):
-            start = start*1000.0
-        elif isinstance(start, int) and start < 100000000000: #and start > 100000000000 and start < 100000000000000:
-            start = start*1000.0
         elif isinstance(start, str):
             start = datetime.datetime.strptime(start, '%Y-%m-%d %H:%M:%S.%f').timestamp()
         if isinstance(end, datetime.datetime):
             end = end.timestamp()
-        elif isinstance(end, float):
-            end = end*1000.0
-        elif isinstance(end, int) and end < 100000000000: #and start > 100000000000 and start < 100000000000000:
-            end = end*1000.0
         elif isinstance(end, str):
             end = datetime.datetime.strptime(end, '%Y-%m-%d %H:%M:%S.%f').timestamp()
 
         nCT = rate*1000.0
-        nTimeR = end
+        nTimeR = end*1000.0
         nTimeR = (int(float(nTimeR)) / int(nCT)) * int(nCT)
 
-        nTimeL = start
+        nTimeL = start*1000.0
         nTimeL = (int(float(nTimeL)) / int(nCT)) * int(nCT)
         nNmbX = int(nTimeR - nTimeL) / int(nCT)
         if nNmbX <= 0:
             nNmbX = 1
         
         return self.__getBinData(ids=ids, nNmbX=nNmbX, TimeR=nTimeR, nCT=nCT/1000.0)
 
+    # TODO: implement return RawData for Client based Converters like Javascript
+    def getRawData(self, names, start, end, rate=1):
+        return None
 
     def getDataAsJson(self, names, start, end, rate=1):
         return getDataSeries_as_Json(self.getDataAsNP(names, start, end, rate))
 
-    # returns RawData for Client based Converters like Javascript
-    def getDataRAW(self,filepath, names, start, end, rate=1):
-        ids = []
-        # find Mst with id as a number, id as MST name a str, id
-        for name in names:
-            id = None
-            if isinstance(name, numbers.Number):
-                id = self.getMst(id=name).id
-            elif isinstance(name, str):
-                id = self.getMst(name=name).id
-            elif isinstance(name, TebisMST):
-                id = name.id
-            elif isinstance(name, TebisGroupElement):
-                for member in name.members:
-                    ids.append(member.mst.id)
-            elif isinstance(name, TebisGroupMember):
-                id = name.mst.id
-            if id is not None:
-                ids.append(id)
-        if isinstance(start, datetime.datetime):
-            start = start.timestamp()
-        elif isinstance(start, float):
-            start = start*1000.0
-        elif isinstance(start, int) and start < 100000000000: #and start > 100000000000 and start < 100000000000000:
-            start = start*1000.0
-        elif isinstance(start, str):
-            start = datetime.datetime.strptime(start, '%Y-%m-%d %H:%M:%S.%f').timestamp()
-        if isinstance(end, datetime.datetime):
-            end = end.timestamp()
-        elif isinstance(end, float):
-            end = end*1000.0
-        elif isinstance(end, int) and end < 100000000000: #and start > 100000000000 and start < 100000000000000:
-            end = end*1000.0
-        elif isinstance(end, str):
-            end = datetime.datetime.strptime(end, '%Y-%m-%d %H:%M:%S.%f').timestamp()
 
-        nCT = rate*1000.0
-        nTimeR = end
-        nTimeR = (int(float(nTimeR)) / int(nCT)) * int(nCT)
-
-        nTimeL = start
-        nTimeL = (int(float(nTimeL)) / int(nCT)) * int(nCT)
-        nNmbX = int(nTimeR - nTimeL) / int(nCT)
-        if nNmbX <= 0:
-            nNmbX = 1
-        
-        return self.getBinDataRAW(filepath,ids=ids, nNmbX=nNmbX, TimeR=nTimeR, nCT=nCT/1000.0)
 
     def getDataAsPD(self, names, start, end = None, rate=1):
         if isinstance(start, list) and all(isinstance(elem, list) for elem in start):
             df = None
             for tuple in start:
                 if df is None:
                     df = pd.DataFrame(self.getDataAsNP(names, tuple[0], tuple[1], rate))            
@@ -406,15 +355,15 @@
         array = np.dtype([('ID', (np.int64)), ('MSTName', np.unicode_, 100), ('UNIT', np.unicode_, 10), ('MSTDesc', np.unicode_, 255), (
             'Val1', (np.float32)), ('Val2', (np.float32)), ('Val3', (np.float32)), ('Val4', (np.float32)), ('Val5', (np.float32))])
         data = self.getConfigData("Msts", array)
         return data
 
     def loadVmstsFromSocket(self):
         array = np.dtype([('ID', (np.int64)), ('MSTName', np.unicode_, 100), ('UNIT', 'U10'), (
-            'MSTDesc', np.unicode_, 255), ('Rate', (np.int64)), ('Formula', np.unicode_, 255), ('refresh', (np.int64))])
+            'MSTDesc', np.unicode_, 255), ('Rate', (np.int)), ('Formula', np.unicode_, 255), ('refresh', (np.int))])
         data = self.getConfigData("VMsts", array)
         return data
 
     """
     lädt die Messstellen direkt über die SocketVerbindung
     hier wird kein DB Zugriff benötigt
     Der Tree und die Gruppen kommen hier allerdings nicht zurück
@@ -510,17 +459,17 @@
                     m_intPos += 1
                     if np.issubdtype(resultarr[resultarr.dtype.names[x]].dtype, np.integer):
                         intStart = np.int64(result[m_intPos])
                         m_intPos += 1
                         intInc = np.int64(result[m_intPos])
                         m_intPos += 1
                     elif np.issubdtype(resultarr[resultarr.dtype.names[x]].dtype, np.floating):
-                        intStart = np.float64(result[m_intPos])
+                        intStart = np.float(result[m_intPos])
                         m_intPos += 1
-                        intInc = np.float64(result[m_intPos])
+                        intInc = np.float(result[m_intPos])
                         m_intPos += 1
                     resultarr[resultarr.dtype.names[x]][y:(y + intStackLen)] = np.linspace(
                         intStart, intStart + (intStackLen * intInc) - intInc, num=intStackLen)
                     y += intStackLen - 1
                 elif result[m_intPos] == "i":
                     findindex += 1
                     m_intPos += 1
@@ -566,15 +515,15 @@
         if np.issubdtype(var_dtype, np.dtype(float).type):
             if isinstance(value, (np.ndarray)):
                 try:
                     val = value
                     find = np.nonzero(value == '')
                     for res in find[0]:
                         value[res] = np.NaN
-                    value = np.array(value, dtype=np.float64)
+                    value = np.array(value, dtype=np.float)
                 except ValueError as e:
                     None
             else:
                 if value == '':
                     return np.NaN
                 value = float(value)
             try:
@@ -799,81 +748,15 @@
             if chunk == '':
                 raise RuntimeError("socket connection broken")
             chunks.append(chunk)
             bytes_recd = bytes_recd + len(chunk)
         return b''.join(chunks)
 
 # endregion
-    def getBinDataRAW(self, filepath, ids=None, nCT=1, nNmbX=1, TimeR=time.time()):
-        
-        start = round(time.time() * 1000)
-        #TimeR = TimeR * 1000.0
-        nCT = int(nCT*1000.0)
-        nCT = self.checkIfReductionAvailable(nCT)
-        if TimeR > start:
-            dif = int(TimeR - start) / int(nCT)
-            TimeR = int(start)
-            nNmbX = int(nNmbX - dif)
-        timeR_new = int(int(int(int(TimeR) / int(nCT)) * int(nCT)))
-        dif = int(int(int(TimeR) - timeR_new) / int(nCT))
-        nNmbX = int(nNmbX - dif)
-        n = 50
-        data = None
-        types = [('timestamp', (np.int64))]
-        for id in ids:
-            mst = self.getMst(id=id)
-            types.append((str(mst.name), (np.float32)))
-        x = [ids[i:i + n] for i in range(0, len(ids), n)]
-        offset = 0
-        
-        for ids in x:
-            rawdata = bytearray()
-            arrMsts = ""
-            rawdata.extend(len(ids).to_bytes(8,'big'))
-            for id in ids:
-                arrMsts += str(id) + ', '
-                rawdata.extend(id.item().to_bytes(8,'big'))
-            arrMsts = arrMsts[:-2]
-            #print(arrMsts)
-            if nNmbX > 0:
-                strRequest = "<tebis>\n"
-                strRequest += "<szConfigFile>" + \
-                    self.config['configfile'] + "</szConfigFile>\n"
-                strRequest += "<szProcedure>LoadData</szProcedure>\n"
-                strRequest += "<arrMsts>" + arrMsts + "</arrMsts>\n"
-                strRequest += "<nNmbX>" + str(nNmbX) + "</nNmbX>\n"
-                strRequest += "<nCT>" + str(int(nCT)) + "</nCT>\n"
-                strRequest += "<nTimeR>" + \
-                    str(timeR_new) + "</nTimeR>\n"
-                strRequest += "<tebis>"
-                try:
-                    self.socketConnect()
-                    # Send Request
-                    self.sendOnSocket(strRequest)
-                    # Recieve MSTS Packet
-                    MSTSRaw = self.receiveOnSocket()
-                except TebisException:
-                    self.socketConnect()
-                    # Send Request
-                    self.sendOnSocket(strRequest)
-                    # Recieve MSTS Packet
-                    MSTSRaw = self.receiveOnSocket()  
-                rawdata.extend(len(MSTSRaw).to_bytes(8,'big'))
-                rawdata.extend(MSTSRaw)
-                #print(len(ids)) 
-                #print(MSTSRaw)
-                #data = self.__checkBinaryResultHeader(
-                #    MSTSRaw, types, data, offset)
-                #offset += len(ids)
-            #data['timestamp'] = data['timestamp'] / 1000.0
-            with open(filepath, 'ab') as fpout:
-                fpout.write(rawdata)
-            #print(os.path.getsize(filepath))
-        return rawdata
-    
+
     """
     schnelles Lesen von Messreihen
     ids= Array mit den Messtellen-Namen
     nCT = Auflösung der Messwerte
     nNmbX= Anzahl der Messpunkt rückwärts ab TimeR
     TimeR= Unixtimestamp rechte Seite der Daten
     """
```

### Comparing `pytebis-0.5.11/pytebis.egg-info/PKG-INFO` & `pytebis-0.5.2/pytebis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: pytebis
-Version: 0.5.11
+Version: 0.5.2
 Summary: Python Connector for TeBIS from Steinhaus
 Home-page: https://github.com/MrLight/pytebis
 Author: MrLight
 Author-email: mrlight1@gmx.de
 License: mit
 Keywords: Python,Connector,TeBIS,Steinhaus
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytebis Python Connector for TeBIS from Steinhaus
 
 pytebis is a connector for interacting with a TeBIS Server.
 
@@ -80,30 +84,22 @@
 
 There are different functions to read data from the TeBIS Server. All functions have the some parameters. Only the return is specific to the function.
 Parameters:
 
 `result = teb.getDataAsJson(names, start, end, rate=1)`
 
 - names = Array of all mst-names to read. You can pass a array of IDs, names, TebisMst-Objects or Group-Objects (even mixed).
-- start = Unix-Timestamp where to start the read
-          - or -
-          Unix-Timestamp in microsecond precision
-          - or - 
-          float value where the fraction is the microseconds part
+- start = Unix-Timestamp where to start the read 
           - or -
           DateTimeObject
           - or -
           String in Format '%Y-%m-%d %H:%M:%S.%f'
           (always the same timezone as the server is)
 - end = Unix-Timestamp where to end the read
           - or -
-          Unix-Timestamp in microsecond precision
-          - or - 
-          float value where the fraction is the microseconds part
-          - or -
           DateTimeObject
           - or -
           String in Format '%Y-%m-%d %H:%M:%S.%f'
           (always the same timezone as the server is)
 - rate = What reduction should be used for the read. If your System supports Values smaller than 1second use Fractions of Seconds. eg: 0.1 for 100ms
 
 The Data which is returned by the TeBIS-Server is vectorized into a structured numpy array. Which is working super fast and is totally comparable with the performance of the TeBIS A Client. You can use different functions to get the data in std. Python formats for further analysis.
@@ -118,38 +114,23 @@
 You can directly access the elements e.g. by indexing them by name `resNP["timestamp"]`
 
 #### as Pandas
 
 ```python
 df = teb.getDataAsPD(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
 ```
-will return a pandas dataframe
-
-
-```python
-df = teb.getDataAsPD([13, 14, 15, 16],  [[1626779900,1626779930],[1626779950,1626779960]],1)
-```
-
-The Pandas Function can even handel multiple slices of timeframes by adding start and endpoint into an array.
-
 
+The Pandas DataFrame will not return a column with the timestamp. But a DateTimeIndex. So you can directly use this for TimeSeries Operations. The creation of the Pandas Dataframe is a bit slower than the generic NumPy function, as the DataFrame and the DateTimeIndex is generated afterwards.
 
 #### as Json
 
 ```python
 resJSON = teb.getDataAsJson(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
 ```
 
-#### as RawValues
-
-```python
-resJSON = teb.getDataRAW(['My_mst_1','My_mst_2'], 1581324153, 1581325153, 10)
-```
-Returns the raw tebis socket data. This could be used if the value calculation should happen on the clientside. e.g. if you want to save bandwidth and gain speed in a client server setup.
-
 #### Example
 
 This will show a plot containing the last hour of data of the point-ids 1 and 2. The reduction is 10 seconds.
 
 ```python
 import time
 import matplotlib.pyplot as plt
@@ -180,7 +161,9 @@
 
 Just call ```teb.refreshMsts()``` to reload the data.
 
 
 ### Logging
 
 The package is implementing a logger using the std. logging framework of Python. The loggername is: ```pytebis```. There is no handler configured. To setup a specific log-level for the package use a config like this after ```logging.basicConfig()``` e.g. ```logging.getLogger('pytebis').setLevel(logging.INFO)``` 
+
+
```

### Comparing `pytebis-0.5.11/setup.py` & `pytebis-0.5.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pytebis',         # How you named your package folder (MyLib)
     packages=['pytebis'],   # Chose the same as "name"
-    version='v0.5.11',      # Start with a small number and increase it with every change you make
+    version='v0.5.02',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='mit',
     # Give a short description about your library
     description='Python Connector for TeBIS from Steinhaus',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='MrLight',                   # Type in your name
@@ -32,9 +32,12 @@
         'Development Status :: 4 - Beta',
         # Define that your audience are developers
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',   # Again, pick a license
         # Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
     ],
 )
```

