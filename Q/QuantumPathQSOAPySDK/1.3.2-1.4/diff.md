# Comparing `tmp/QuantumPathQSOAPySDK-1.3.2.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.3.2.tar", last modified: Tue Mar 21 12:02:38 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.4.tar", last modified: Mon Apr 10 09:33:49 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.3.2.tar` & `QuantumPathQSOAPySDK-1.4.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:38.793802 QuantumPathQSOAPySDK-1.3.2/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-03-21 12:02:38.792717 QuantumPathQSOAPySDK-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:38.639278 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/Exception.py
--rw-rw-rw-   0        0        0    58397 2023-03-21 11:41:52.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2022-11-22 13:09:53.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:38.762118 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/AssetManagementResult.py
--rw-rw-rw-   0        0        0     5606 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/CircuitAnnealing.py
--rw-rw-rw-   0        0        0     5307 2022-11-29 11:45:17.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/CircuitFlow.py
--rw-rw-rw-   0        0        0    43529 2023-03-16 08:48:54.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/CircuitGates.py
--rw-rw-rw-   0        0        0      681 2022-11-24 16:19:48.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Context.py
--rw-rw-rw-   0        0        0     1044 2022-11-24 16:20:46.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/SolutionItem.py
--rw-rw-rw-   0        0        0      657 2022-11-30 08:30:14.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/__init__.py
--rw-rw-rw-   0        0        0     1517 2022-12-13 11:06:32.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/apiConnection.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:38.684158 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-03-21 12:02:38.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-03-21 12:02:38.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 12:02:38.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-03-21 12:02:38.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-21 12:02:38.000000 QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-21 12:02:38.794608 QuantumPathQSOAPySDK-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-03-21 12:01:07.000000 QuantumPathQSOAPySDK-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:38.789475 QuantumPathQSOAPySDK-1.3.2/test/
--rw-rw-rw-   0        0        0       83 2023-03-21 12:01:34.000000 QuantumPathQSOAPySDK-1.3.2/test/test.py
--rw-rw-rw-   0        0        0     6549 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.3.2/test/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     5624 2022-11-29 12:13:27.000000 QuantumPathQSOAPySDK-1.3.2/test/test_CircuitFlow.py
--rw-rw-rw-   0        0        0     7545 2022-11-29 15:44:41.000000 QuantumPathQSOAPySDK-1.3.2/test/test_CircuitGates_MultipleGates.py
--rw-rw-rw-   0        0        0    12740 2022-11-29 15:45:08.000000 QuantumPathQSOAPySDK-1.3.2/test/test_CircuitGates_SimpleGates.py
--rw-rw-rw-   0        0        0   109946 2022-12-13 10:11:15.000000 QuantumPathQSOAPySDK-1.3.2/test/test_QSOAPlatform.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:33:49.871329 QuantumPathQSOAPySDK-1.4/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      926 2023-04-10 09:33:49.870332 QuantumPathQSOAPySDK-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 09:33:49.531618 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/Exception.py
+-rw-rw-rw-   0        0        0    59112 2023-03-30 11:50:48.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2022-11-22 13:09:53.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:33:49.839532 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     5606 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     5307 2022-11-29 11:45:17.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/CircuitFlow.py
+-rw-rw-rw-   0        0        0    52897 2023-04-04 13:05:25.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/CircuitGates.py
+-rw-rw-rw-   0        0        0      681 2022-11-24 16:19:48.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Context.py
+-rw-rw-rw-   0        0        0     1044 2022-11-24 16:20:46.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/SolutionItem.py
+-rw-rw-rw-   0        0        0      657 2023-03-23 09:26:45.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-03-21 16:02:18.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/apiConnection.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:33:49.585576 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      926 2023-04-10 09:33:49.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1158 2023-04-10 09:33:49.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 09:33:49.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-10 09:33:49.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-10 09:33:49.000000 QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 09:33:49.872328 QuantumPathQSOAPySDK-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      955 2023-04-10 09:33:02.000000 QuantumPathQSOAPySDK-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:33:49.868337 QuantumPathQSOAPySDK-1.4/test/
+-rw-rw-rw-   0        0        0      553 2023-04-04 09:22:53.000000 QuantumPathQSOAPySDK-1.4/test/test.py
+-rw-rw-rw-   0        0        0     6549 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.4/test/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     5624 2022-11-29 12:13:27.000000 QuantumPathQSOAPySDK-1.4/test/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0    72233 2023-04-04 10:25:22.000000 QuantumPathQSOAPySDK-1.4/test/test_CircuitGates.py
+-rw-rw-rw-   0        0        0   115890 2023-03-31 08:11:48.000000 QuantumPathQSOAPySDK-1.4/test/test_QSOAPlatform.py
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/PKG-INFO` & `QuantumPathQSOAPySDK-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.3.2
+Version: 1.4
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/Exception.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             'echostatus': 'login/echostatus',
             'authenticate': 'login/authenticate/',
             'authenticateEx': 'login/authenticateEx/'
         }
 
         self.connectionPoints = {
             'getVersion': 'connectionPoint/getVersion/',
+            'getLicenceInfo': 'connectionPoint/getLicenceInfo/',
             'getQuantumSolutions': 'connectionPoint/getQuantumSolutions/',
             'getQuantumDevices': 'connectionPoint/getQuantumDevices/',
             'getQuantumFlows': 'connectionPoint/getQuantumFlows/',
             'runQuantumApplication': 'connectionPoint/runQuantumApplication/',
             'getQuantumExecutionResponse': 'connectionPoint/getQuantumExecutionResponse/',
             'getQuantumDevicesEx': 'connectionPoint/getQuantumDevicesEx/'
         }
@@ -139,21 +140,21 @@
         }
 
     def __checkInputTypes(self, *args):
         for argTuple in args:
             expextedTypes = str([i.__name__ for i in argTuple[2]]).replace("['", "<").replace(" '", " <").replace("']", ">").replace("',", ">,")
 
             if type(argTuple[1]) not in argTuple[2]:
-                raise ValueError(f'Argument "{argTuple[0]}" expected to be {expextedTypes}, not <{type(argTuple[1]).__name__}>')
+                raise TypeError(f'Argument "{argTuple[0]}" expected to be {expextedTypes}, not <{type(argTuple[1]).__name__}>')
     
     def __checkValues(self, *args):
         for argTuple in args:
             expectedValues = str([i for i in argTuple[2]]).replace('[', '').replace(']', '')
             
-            if argTuple[1].upper() not in argTuple[2]:
+            if argTuple[1] not in argTuple[2]:
                 raise ValueError(f'Argument "{argTuple[0]}" expected to be {expectedValues}, not "{argTuple[1]}"')
 
 
     # USER METHODS
     def getEnvironments(self) -> dict: # getEnvironments. Returns a Dictionary
         """
         Show QuantumPath available environments.
@@ -295,15 +296,15 @@
                 username = qpathcredentials[self.activeEnvironment[1] + '-credentials']['username']
                 password = qpathcredentials[self.activeEnvironment[1] + '-credentials']['password']
 
             except:
                 raise self.ConfigFileError('Error reading username or password in config file')
             
         elif not username or not password:
-            raise TypeError('QSOAPlatform.authenticate() takes from 1 to 3 positional arguments')
+            raise ValueError('QSOAPlatform.authenticate() takes from 1 to 3 positional arguments')
 
         else:
             try:
                 base64_bytes = password.encode('ascii')
                 password = str(self.base64.b64decode(base64_bytes).decode('ascii'))
             
             except:
@@ -359,15 +360,15 @@
                 username = qpathcredentials[self.activeEnvironment[1] + '-credentials']['username']
                 password = qpathcredentials[self.activeEnvironment[1] + '-credentials']['password']
             
             except:
                 raise self.ConfigFileError('Error reading username or password in config file')
 
         elif not username or not password:
-            raise TypeError('QSOAPlatform.authenticate() takes from 1 to 3 positional arguments')
+            raise ValueError('QSOAPlatform.authenticate() takes from 1 to 3 positional arguments')
 
         self.context = self.Context(username, password, url)
 
         return True
 
 
     def echostatus(self) -> bool: # echostatus. Returns a Boolean
@@ -440,14 +441,38 @@
         
         else:
             raise self.AuthenticationError('User not authenticated')
 
         return version
 
 
+    def getLicenceInfo(self) -> dict: # getLicenceInfo. Returns a Dictionary
+        """
+        Returns QuantumPath account licence.
+
+        Prerequisites
+        ----------
+        - User already authenticated.
+
+        Output
+        ----------
+        dict
+        """
+
+        if self.echostatus():
+            url = self.environments[self.activeEnvironment[0]][self.activeEnvironment[1]] + self.connectionPoints['getLicenceInfo']
+
+            licence = apiConnection(url, self.context.getHeader(), 'json')
+        
+        else:
+            raise self.AuthenticationError('User not authenticated')
+
+        return licence
+
+
     def getQuantumSolutionList(self) -> dict: # getQuantumSolutionList. Returns a Dictionary
         """
         Show the list of solutions available to the user along with their IDs.
 
         Prerequisites
         ----------
         - User already authenticated.
@@ -856,15 +881,15 @@
             self.__checkInputTypes(
                 ('executionToken', args[0], (str,)),
                 ('idSolution', args[1], (int,)),
                 ('idFlow', args[2], (int,))
             )
         
         else:
-            raise TypeError('QSOAPlatform.authenticate() takes from 1 to 4 positional arguments')
+            raise ValueError('QSOAPlatform.authenticate() takes from 1 to 4 positional arguments')
         
 
         if self.echostatus():
             if len(args) == 1:
                 executionToken = args[0].getExecutionToken()
                 idSolution = args[0].getIdSolution()
                 idFlow = args[0].getIdFlow()
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Application.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Asset.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/CircuitGates.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/CircuitGates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,881 +1,1024 @@
 class CircuitGates:
     """
     Create Circuit Gates.
     """
 
     # CONSTRUCTOR
     def __init__(self):
-        self.classicRegisters = set()
+        """
+        CircuitGates object constructor.
+
+        Prerequisites
+        ----------
+        None.
+
+        Output
+        ----------
+        CircuitGates obj
+        """
+
         self.__circuitBody = [[]]
+        self.__qubitStates = []
+        self.__numerOfQubits = 0
+        self.__defaultQubitState = '0'
+        self.__validQubitStates = ['0', '1', '+', '-', 'i', '-i']
 
 
     # GETTERS
     def getCircuitBody(self) -> list:
         """
         Get Circuit Body.
 
+        Prerequisites
+        ----------
+        - Created circuit.
+
         Output
         ----------
         list
         """
 
         return self.__circuitBody
-    
+
+
+    def getQubitStates(self) -> list:
+        """
+        Get Circuit Qubit states.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Output
+        ----------
+        list
+        """
+
+        return self.__qubitStates
+
+
+    def getNumberOfQubits(self) -> int:
+        """
+        Get number of qubits used in circuit.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Output
+        ----------
+        int
+        """
+
+        return self.__numerOfQubits
+
+
+    def getDefaultQubitState(self) -> str:
+        """
+        Get Default Qubit state.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+        
+        Output
+        ----------
+        str
+        """
+        
+        return self.__defaultQubitState
+
+
     def getParsedBody(self) -> str:
+        """
+        Get Circuit Body VL.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Output
+        ----------
+        str
+        """
+
         stringBody = str(self.__circuitBody).replace("'", '"').replace(' ', '')
-        parsedtBody = 'circuit={"cols":' + stringBody + '}'
+        stringQubitStates = str(self.__qubitStates).replace("'", '"').replace(' ', '')
+        parsedtBody = 'circuit={"cols":' + stringBody + ', "init":' + stringQubitStates + '}'
 
         return parsedtBody
-    
-    def getClassicRegisters(self) -> set:
-        return self.classicRegisters
 
 
+    # SETTERS
+    def setDefaultQubitState(self, qubitState: str):
+        """
+        Set Default Qubit state.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Parameters
+        ----------
+        qubitState : str
+            Set default qubit state. It can be 0, 1, +, -, i or -i.
+
+        Output
+        ----------
+        str
+        """
+        self.__checkInputTypes(
+            ('qubitState', qubitState, (str,))
+        )
+
+        if qubitState in self.__validQubitStates:
+            self.__defaultQubitState = qubitState # set new default qubit state
+        else:
+            raise ValueError(f'Not valid quibt state. Default state is still |{self.__defaultQubitState}>')
+
+        return self.__qubitStates
+    
+
     # INTERN FUNCTIONS
     def __checkInputTypes(self, *args):
         for argTuple in args:
             expextedTypes = str([i.__name__ for i in argTuple[2]]).replace("['", "<").replace(" '", " <").replace("']", ">").replace("',", ">,")
 
             if type(argTuple[1]) not in argTuple[2]:
-                raise ValueError(f'Argument "{argTuple[0]}" expected to be {expextedTypes}, not <{type(argTuple[1]).__name__}>')
-    
-    def __checkAllItemsSameType(self, itemsList: list):
-        if not all(isinstance(n, int) for n in itemsList):
-            raise ValueError(f'Argument "position" expected to be <int>')
+                raise TypeError(f'Argument "{argTuple[0]}" expected to be {expextedTypes}, not <{type(argTuple[1]).__name__}>')
     
-    def __addMeasure(self, position, gate, circuitBody, classicRegisters):
-        if circuitBody[0] == []: # if circuit is empty
-            column = 0
-
-        else: # if circuit is not empty
-            column = -1
-            circuitBody.append([])
-
-
-        while len(circuitBody[column]) != position: # fill with 1 the positions until the gate position
-            circuitBody[column].append(1)
+    def __checkValues(self, *args):
+        for argTuple in args:
+            expectedValues = str([i for i in argTuple[2]]).replace('[', '').replace(']', '')
             
-        circuitBody[column].append(gate) # add the gate
-        classicRegisters.add(position) # transform quantum register to classic register
+            if argTuple[1] not in argTuple[2]:
+                raise ValueError(f'Argument "{argTuple[0]}" expected to be {expectedValues}, not "{argTuple[1]}"')
     
-    def __addSimpleGate(self, position, gate, circuitBody, classicRegisters = {}):
-        if position not in classicRegisters:
 
-            numColumn = len(circuitBody) - 1 # column indexes
-            lastColumn = -1 # last column with gate
+    def __addSimpleGate(self, position, gate, circuitBody):
+        numColumn = len(circuitBody) - 1 # column index
+        lastColumn = -1 # last column with gate
 
-            while numColumn >= 0: # while there are columns
+        # SEARCH LAST COLUMN TO ADD
+        while numColumn >= 0: # while there are columns
 
-                if 'CTRL' in circuitBody[numColumn] or 'Swap' in circuitBody[numColumn]: # if column have a multiple gate
-                    break
+            if 'CTRL' in circuitBody[numColumn] or 'Swap' in circuitBody[numColumn]: # column have a multiple gate
+                break
 
-                elif len(circuitBody[numColumn]) - 1 < position: # column is smaller than the gate position
+            elif len(circuitBody[numColumn]) - 1 < position: # column is smaller than the gate position
+                lastColumn = numColumn # column available to add the gate
+            
+            else: # column is greater than the gate position
+
+                if circuitBody[numColumn][position] == 1: # position is 1
                     lastColumn = numColumn # column available to add the gate
                 
-                else: # column is greater than the gate position
-
-                    if circuitBody[numColumn][position] == 1: # position is 1
-                        lastColumn = numColumn # column available to add the gate
-                    
-                    else: # column have a gate, so is not available to add the gate
-                        break
+                else: # column have a gate, so is not available to add the gate
+                    break
 
-                numColumn -= 1 # check previous column
-            
+            numColumn -= 1 # check previous column
 
-            if lastColumn != -1: # add the gate in an existing column
+        # ADD GATE
+        if lastColumn != -1: # add the gate in an existing column
 
-                if len(circuitBody[lastColumn]) - 1 < position: # column is smaller than the gate position
+            if len(circuitBody[lastColumn]) - 1 < position: # column is smaller than the gate position
 
-                    while len(circuitBody[lastColumn]) != position: # fill with 1 the positions until the gate position
-                        circuitBody[lastColumn].append(1)
-                    
-                    circuitBody[lastColumn].append(gate) # add the gate
+                while len(circuitBody[lastColumn]) != position: # fill with 1 the positions until the gate position
+                    circuitBody[lastColumn].append(1)
                 
-                else: # column is larger than the gate position
-                    circuitBody[lastColumn][position] = gate # replace 1 by the gate
+                circuitBody[lastColumn].append(gate) # add the gate
             
-            else: # add a new column
-                circuitBody.append([])
+            else: # column is larger than the gate position
+                circuitBody[lastColumn][position] = gate # replace 1 by the gate
+        
+        else: # add a new column
+            circuitBody.append([])
 
-                while len(circuitBody[lastColumn]) != position: # fill with 1 the positions until the gate position
-                    circuitBody[-1].append(1)
-                    
-                circuitBody[-1].append(gate) # add the gate
-    
-    def __addMultipleGate(self, positions, circuitBody, classicRegisters = {}):
-        # swap --> add gate
-        # control swap with classic register in swap --> not add gate
-        # control gate without classic register in gate --> add gate
-        # control gate with classic register in gate --> not add gate
-
-        addGate = True
-        control = False
-
-        for gate in positions: # check all gates
-            if 'CTRL' in gate: # if control in any position
-                control = True
-                break
+            while len(circuitBody[lastColumn]) != position: # fill with 1 the positions until the gate position
+                circuitBody[-1].append(1)
+                
+            circuitBody[-1].append(gate) # add the gate
 
-        if control: # if is a controlled gate
-            for gate in positions: # check all gates
-                if 'CTRL' not in gate: # is a gate position, not a control
-                    if gate[0] in classicRegisters: # gate position is a classic register
-                        addGate = False
-                        break
 
-        if addGate:
-            positions = sorted(positions)
-            
-            if circuitBody[0] == []: # if circuit is empty
-                column = 0
+    def __addMultipleGate(self, positions, circuitBody):
+        positions = sorted(positions)
 
-            else: # if circuit is not empty
-                column = -1
-                circuitBody.append([])
+        # SEARCH LAST COLUMN TO ADD
+        if circuitBody[0] == []: # circuit is empty
+            lastColumn = 0
 
-            for position in positions:
+        else: # if circuit is not empty
+            lastColumn = -1
+            circuitBody.append([])
+        
+        # ADD GATE
+        for position in positions:
 
-                while len(circuitBody[column]) != position[0]: # fill with 1 the positions until the gate position
-                    circuitBody[column].append(1)
-                
-                circuitBody[column].append(position[1]) # add the gate
+            while len(circuitBody[lastColumn]) != position[0]: # fill with 1 the positions until the gate position
+                circuitBody[lastColumn].append(1)
+            
+            circuitBody[lastColumn].append(position[1]) # add the gate
 
-            if 'Swap' in positions[0]: # if the multiple gate is a swap
 
-                if positions[0][0] in classicRegisters and positions[1][0] not in classicRegisters: # swap quantum regiter and classic register
-                    classicRegisters.remove(positions[0][0])
-                    classicRegisters.add(positions[1][0])
-                
-                elif positions[1][0] in classicRegisters and positions[0][0] not in classicRegisters: # swap quantum regiter and classic register
-                    classicRegisters.remove(positions[1][0])
-                    classicRegisters.add(positions[0][0])
-    
     def __definePositions(self, position, gate: str, circuitBody: list) -> list:
         positions = list()
 
         if isinstance(position, int): # gate in one position
             positions.append((position, gate))
-
+        
         elif isinstance(position, list): # gate in multiple positions
-            self.__checkAllItemsSameType(position)
-
             for i in position:
                 positions.append((i, gate)) # add all controls
-
+        
         elif position is None:
             lenCircuitBody = list()
 
             for column in circuitBody:
                 lenCircuitBody.append(len(column))
 
             times = max(lenCircuitBody)
 
             for i in range(times):
                 positions.append((i, gate))
             
         return positions
 
 
+    def __updateQubits(self):
+        new_numerOfQubits = max(len(x) for x in self.__circuitBody) # new number of qubits
+
+        if new_numerOfQubits > self.__numerOfQubits:
+            while len(self.__qubitStates) < new_numerOfQubits:
+                self.__qubitStates.append(self.__defaultQubitState) # add new qubit states
+        
+        self.__numerOfQubits = new_numerOfQubits
+    
+
     # METHODS
-    def x(self, position: int = None, add: bool = True) -> list: # Not gate
+    def initializeQubitStates(self, qubitStates: list):
         """
-        Add Pauli X gate.
+        Initialize Qubit states.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
-        position : int
-            Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
-        add : bool
-            Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        qbitStates : list
+            List of strings setting up the qubit states. It must be equal than number of qubits. There can be 0, 1, +, -, i or -i.
         """
-        if position:
-            self.__checkInputTypes(
-                ('position', position, (int, list))
-            )
         self.__checkInputTypes(
-            ('add', add, (bool,))
+            ('qubitStates', qubitStates, (list,))
         )
-        
-
-        gateSymbol = 'X'
-
-        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
-        if add:
-            for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        for qubitState in qubitStates:
+            self.__checkInputTypes(('qubitStates', qubitState, (str,)))
+            self.__checkValues(('qubitStates', qubitState, self.__validQubitStates))
         
-        return positions
+        if len(qubitStates) != self.__numerOfQubits:
+            raise ValueError(f'Incorrect number of qubit states. Input states are {len(qubitStates)} and should be {self.__numerOfQubits}')
 
+        self.__qubitStates = qubitStates
 
-    def y(self, position: int = None, add: bool = True) -> list: # pauli y gate
+
+    def h(self, position: int = None, add: bool = True) -> list: # hadamard gate
         """
-        Add Pauli Y gate.
+        Add Hadamard gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'Y'
+        gateSymbol = 'H'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+            
+        self.__updateQubits()
         
         return positions
-    
 
-    def z(self, position: int = None, add: bool = True) -> list: # pauli z gate
+
+    def x(self, position: int = None, add: bool = True) -> list: # not gate
         """
-        Add Pauli Z gate.
+        Add Pauli X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
-
-
-        gateSymbol = 'Z'
+        
+        gateSymbol = 'X'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
+        self.__updateQubits()
+        
         return positions
     
 
-    def s(self, position: int = None, add: bool = True) -> list: # square root of z, s gate
+    def y(self, position: int = None, add: bool = True) -> list: # pauli y gate
         """
-        Add Square root of Z, S gate.
+        Add Pauli Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'S'
+        gateSymbol = 'Y'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
+        self.__updateQubits()
+        
         return positions
-    
 
-    def sdg(self, position: int = None, add: bool = True) -> list: # s dagger gate
+
+    def z(self, position: int = None, add: bool = True) -> list: # pauli z gate
         """
-        Add S Dagger gate.
+        Add Pauli Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'I_S'
+        gateSymbol = 'Z'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
+        self.__updateQubits()
+        
         return positions
-    
 
-    def t(self, position: int = None, add: bool = True) -> list: # fourth root of z, t gate
+
+    def s(self, position: int = None, add: bool = True) -> list: # square root of z, s gate
         """
-        Add Fourt root of Z, T gate.
+        Add Square root of Z, S gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'T'
+        gateSymbol = 'S'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
+        self.__updateQubits()
+        
         return positions
-    
 
-    def tdg(self, position: int = None, add: bool = True) -> list: # t dagger gate
+
+    def i_s(self, position: int = None, add: bool = True) -> list: # Adjoint square root z gate
         """
-        Add T Dagger gate.
+        Add Adjoint square root Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'I_T'
+        gateSymbol = 'I_S'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
-        return positions
-    
-
-    def barrier(self, position: int = None): # barrier
-        """
-        Add Barrier.
-
-        Prerequisites
-        ----------
-        - Created circuit.
-
-        Parameters
-        ----------
-        position : int
-            Optional argument. Qubit position to add the barrier. In the case that the position is not indicated, the barrier will be added in all qubits. It can also be a list of positions.
-        """
-        if position:
-            self.__checkInputTypes(
-                ('position', position, (int, list))
-            )
-        
-
-        gateSymbol = 'SPACER'
-
-        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
+        self.__updateQubits()
         
-        if position is None:
-            self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
-        
-        else:
-            for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        return positions
 
 
-    def p(self, position: int = None, argument = 'pi', add: bool = True) -> list: # phase gate
+    def sx(self, position: int = None, add: bool = True) -> list: # square root of not gate
         """
-        Add Phase gate.
+        Add Square root of X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
-        argument: string
-            Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
-            ('argument', argument, (str, int)),
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = {'id': 'P', 'arg': str(argument)}
+        gateSymbol = 'SX'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
+        self.__updateQubits()
+        
         return positions
-    
 
-    def rz(self, position: int = None, argument = 'pi', add: bool = True) -> list: # retation z gate
+
+    def i_sx(self, position: int = None, add: bool = True) -> list: # adjoint square root X gate
         """
-        Add Rotation Z gate.
+        Add Adjoint square root X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
-        argument: string
-            Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
-            ('argument', argument, (str, int)),
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = {'id': 'RZ', 'arg': str(argument)}
+        gateSymbol = 'I_SX'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
-        return positions
-
-
-    def measure(self, position: int = None) -> list: # measure
-        """
-        Add Measure.
-
-        Prerequisites
-        ----------
-        - Created circuit.
-
-        Parameters
-        ----------
-        position : int
-            Optional argument. Qubit position to add the measurement. In the case that the position is not indicated, the measurement will be added in all qubits. It can also be a list of positions.
-        """
-        if position:
-            self.__checkInputTypes(
-                ('position', position, (int, list))
-            )
-
-        
-        gateSymbol = 'Measure'
-        
-        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
-
-        for gate in positions: # to all gates
-            self.__addMeasure(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+        self.__updateQubits()
         
         return positions
 
 
-    def h(self, position: int = None, add: bool = True) -> list: # hadamard gate
+    def sy(self, position: int = None, add: bool = True) -> list: # square root of y gate
         """
-        Add Hadamard gate.
+        Add Square root of Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'H'
+        gateSymbol = 'SY'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
 
-    def sx(self, position: int = None, add: bool = True) -> list: # square root of not gate
+
+    def i_sy(self, position: int = None, add: bool = True) -> list: # adjoint square root y gate
         """
-        Add Square root of X gate.
+        Add Adjoint square root Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'SX'
+        gateSymbol = 'I_SY'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
 
 
-    def sxdg(self, position: int = None, add: bool = True) -> list: # square root of not dagger gate
+    def t(self, position: int = None, add: bool = True) -> list: # four root of z, t gate
         """
-        Add Square root of X Dagger gate.
+        Add Four root of Z, T gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-        gateSymbol = 'I_SX'
+        gateSymbol = 'T'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
 
-    def sy(self, position: int = None, add: bool = True) -> list: # square root of y gate
+
+    def i_t(self, position: int = None, add: bool = True) -> list: # adjoint four root z gate
         """
-        Add Square root of Y gate.
+        Add Adjoint four root Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'SY'
+        gateSymbol = 'I_T'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
 
 
-    def sydg(self, position: int = None, add: bool = True) -> list: # square root of y dagger
+    def tx(self, position: int = None, add: bool = True) -> list: # four root of x gate
         """
-        Add Square root of Y Dagger gate.
+        Add four root of X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'I_SY'
+        gateSymbol = 'TX'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
 
-    def tx(self, position: int = None, add: bool = True) -> list: # fourth root of x gate
+
+    def i_tx(self, position: int = None, add: bool = True) -> list: # adjoint four root X gate
         """
-        Add Fourth root of X gate.
+        Add Adjoint four root X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'TX'
-
+        gateSymbol = 'I_TX'
+        
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
 
 
-    def txdg(self, position: int = None, add: bool = True) -> list: # fourth root of x dagger gate
+    def ty(self, position: int = None, add: bool = True) -> list: # four root of y gate
         """
-        Add Fourth root of X Dagger gate.
+        Add four root of Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
+        gateSymbol = 'TY'
 
-        gateSymbol = 'I_TX'
-        
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
 
-    def ty(self, position: int = None, add: bool = True) -> list: # fourth root of y gate
+
+    def i_ty(self, position: int = None, add: bool = True) -> list: # adjoint four root y gate
         """
-        Add Fourth root of Y gate.
+        Add Adjoint four root Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'TY'
+        gateSymbol = 'I_TY'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
 
-    def tydg(self, position: int = None, add: bool = True) -> list: # fourth root of y dagger gate
+
+    def p(self, position: int = None, argument = 'pi', add: bool = True) -> list: # phase gate
         """
-        Add Fourth root of Y Dagger gate.
+        Add Phase gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
+        argument: string
+            Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
+            ('argument', argument, (str, int)),
             ('add', add, (bool,))
         )
 
-
-        gateSymbol = 'I_TY'
+        gateSymbol = {'id': 'P', 'arg': str(argument)}
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
+
 
     def rx(self, position: int = None, argument = 'pi', add: bool = True) -> list: # rotation x gate
         """
         Add Rotation X gate.
 
         Prerequisites
         ----------
@@ -885,35 +1028,43 @@
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         argument: string
             Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('argument', argument, (str, int)),
             ('add', add, (bool,))
         )
 
-
         gateSymbol = {'id': 'RX', 'arg': str(argument)}
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
+
 
     def ry(self, position: int = None, argument = 'pi', add: bool = True) -> list: # rotation y gate
         """
         Add Rotation Y gate.
 
         Prerequisites
         ----------
@@ -923,91 +1074,89 @@
         ----------
         position : int
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         argument: string
             Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         if position:
             self.__checkInputTypes(
                 ('position', position, (int, list))
             )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
             ('argument', argument, (str, int)),
             ('add', add, (bool,))
         )
 
-
         gateSymbol = {'id': 'RY', 'arg': str(argument)}
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         if add:
             for gate in positions: # to all gates
-                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody, self.classicRegisters) # add to circuit
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
 
-    def control(self, position: int, circuit: list) -> list: # control
+
+    def rz(self, position: int = None, argument = 'pi', add: bool = True) -> list: # rotation z gate
         """
-        Add Control.
+        Add Rotation Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
-            Mandatory argument. Qubit position to add the control.
-        circuit : list
-            Gate or set of elements to add a control.
+            Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
+        argument: string
+            Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
+        add : bool
+            Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
+        if position:
+            self.__checkInputTypes(
+                ('position', position, (int, list))
+            )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         self.__checkInputTypes(
-            ('position', position, (int, list)),
-            ('circuit', circuit, (list,))
+            ('argument', argument, (str, int)),
+            ('add', add, (bool,))
         )
 
+        gateSymbol = {'id': 'RZ', 'arg': str(argument)}
 
-        correctPosition = True
-
-        for gate in circuit:
-            if position in gate:
-                correctPosition = False
-                break
-
-        if correctPosition:
-            circuit.append((position, 'CTRL'))
-
-        return circuit
-    
-
-    def addCreatedGate(self, gate: list): # add created gate
-        """
-        Add Created gate.
-
-        Prerequisites
-        ----------
-        - Created circuit.
-        - Created gate.
-
-        Parameters
-        ----------
-        gate : list
-            Created gate to add to the circuit.
-        """
-        self.__checkInputTypes(
-            ('gate', gate, (list,))
-        )
+        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
+        if add:
+            for gate in positions: # to all gates
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
+        
+        return positions
 
-        self.__addMultipleGate(gate, self.__circuitBody, self.classicRegisters) # add to circuit
-    
 
     def swap(self, position1: int, position2: int, add: bool = True) -> list: # swap gate
         """
         Add Rotation Swap gates.
 
         Prerequisites
         ----------
@@ -1017,63 +1166,74 @@
         ----------
         position1 : int
             Mandatory argument. First qubit position to add the swap.
         position2 : int
             Mandatory argument. Second qubit position to add the swap.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         self.__checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('add', add, (bool,)),
         )
 
         positions = [
             (position1, 'Swap'),
             (position2, 'Swap')
         ]
 
         if add:
-            self.__addMultipleGate(positions, self.__circuitBody, self.classicRegisters) # add to circuit
+            self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
         
-        return positions
+        self.__updateQubits()
         
+        return positions
+
 
     def ch(self, position1: int, position2: int, add: bool = True) -> list: # control hadamard gate
         """
         Add Rotation Control Hadamard gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position1 : int
-            Mandatory argument. First qubit position to add the swap.
+            Mandatory argument. First qubit position to add the control.
         position2 : int
-            Mandatory argument. Second qubit position to add the swap.
+            Mandatory argument. Second qubit position to add the hadamard gate.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         self.__checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('add', add, (bool,)),
         )
 
-
         positions = [
             (position1, 'CTRL'),
             (position2, 'H')
         ]
 
         if add:
-            self.__addMultipleGate(positions, self.__circuitBody, self.classicRegisters) # add to circuit
+            self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
 
 
     def cx(self, position1: int, position2: int, add: bool = True) -> list: # control not gate
         """
         Add Control X gate.
@@ -1081,107 +1241,336 @@
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position1 : int
-            Mandatory argument. First qubit position to add the swap.
+            Mandatory argument. First qubit position to add the control.
         position2 : int
-            Mandatory argument. Second qubit position to add the swap.
+            Mandatory argument. Second qubit position to add the X gate.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         self.__checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('add', add, (bool,)),
         )
 
-
         positions = [
             (position1, 'CTRL'),
             (position2, 'X')
         ]
 
         if add:
-            self.__addMultipleGate(positions, self.__circuitBody, self.classicRegisters) # add to circuit
+            self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
     
 
     def ccx(self, position1: int, position2: int, position3: int, add = True) -> list: # toffoli gate
         """
-        Add Rotation Control Control Hadamard gate.
+        Add Toffoli gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position1 : int
-            Mandatory argument. First qubit position to add the swap.
+            Mandatory argument. First qubit position to add the control.
         position2 : int
-            Mandatory argument. Second qubit position to add the swap.
+            Mandatory argument. Second qubit position to add the control.
         position3 : int
-            Mandatory argument. Second qubit position to add the swap.
+            Mandatory argument. Third qubit position to add the X gate.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         self.__checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('position3', position3, (int,)),
             ('add', add, (bool,)),
         )
 
-
         positions = [
             (position1, 'CTRL'),
             (position2, 'CTRL'),
             (position3, 'X')
         ]
 
         if add:
-            self.__addMultipleGate(positions, self.__circuitBody, self.classicRegisters) # add to circuit
+            self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return positions
-    
+
+
+    def measure(self, position: int = None) -> list: # measure
+        """
+        Add Measure.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Parameters
+        ----------
+        position : int
+            Optional argument. Qubit position to add the measurement. In the case that the position is not indicated, the measurement will be added in all qubits. It can also be a list of positions.
+        
+        Output
+        ----------
+        list
+        """
+        if position:
+            self.__checkInputTypes(
+                ('position', position, (int, list))
+            )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
+
+        gateSymbol = 'Measure'
+        
+        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
+
+        self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
+
+        self.__updateQubits()
+        
+        return positions
+
+
+    def barrier(self, position: int = None): # barrier
+        """
+        Add Barrier.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Parameters
+        ----------
+        position : int
+            Optional argument. Qubit position to add the barrier. In the case that the position is not indicated, the barrier will be added in all qubits. It can also be a list of positions.
+        """
+        if position:
+            self.__checkInputTypes(
+                ('position', position, (int, list))
+            )
+            if isinstance(position, list):
+                for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
+
+        gateSymbol = 'SPACER'
+
+        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
+        
+        if position is None:
+            self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
+        
+        else:
+            for gate in positions: # to all gates
+                self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
+
+
+    def beginRepeat(self, position: int, repetitions: int) -> list: # begin repeat
+        """
+        Add Begin Repeat.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Parameters
+        ----------
+        position : int
+            Qubit position to add the begin repetition. It can also be a list of positions.
+        repetitions: int
+            Number of repetitions.
+        
+        Output
+        ----------
+        list
+        """
+        self.__checkInputTypes(
+            ('position', position, (int, list))
+        )
+        if isinstance(position, list):
+            for p in position:
+                self.__checkInputTypes(('position', p, (int,)))
+        self.__checkInputTypes(
+            ('repetitions', repetitions, (int,))
+        )
+
+        gateSymbol = {'id': 'BEGIN_R', 'arg': str(repetitions)}
+        
+        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
+
+        self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
+
+        self.__updateQubits()
+        
+        return positions
+
+
+    def endRepeat(self, position: int) -> list: # begin repeat
+        """
+        Add End Repeat.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Parameters
+        ----------
+        position : int
+            Qubit position to add the end repetition. It can also be a list of positions.
+        
+        Output
+        ----------
+        list
+        """
+        self.__checkInputTypes(
+            ('position', position, (int, list))
+        )
+        if isinstance(position, list):
+            for p in position:
+                self.__checkInputTypes(('position', p, (int,)))
+
+        gateSymbol = 'END_R'
+        
+        positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
+
+        self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
+
+        self.__updateQubits()
+        
+        return positions
+
+
+    def control(self, position: int, circuit: list) -> list: # control
+        """
+        Add Control.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+
+        Parameters
+        ----------
+        position : int
+            Mandatory argument. Qubit position to add the control.
+        circuit : list
+            Gate or set of elements to add a control.
+        
+        Output
+        ----------
+        list
+        """
+        self.__checkInputTypes(
+            ('position', position, (int, list)),
+            ('circuit', circuit, (list,))
+        )
+        if isinstance(position, list):
+            for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
+
+        correctPosition = True
+
+        for gate in circuit:
+            if position in gate:
+                correctPosition = False
+                break
+
+        if correctPosition:
+            circuit.append((position, 'CTRL'))
+
+        self.__updateQubits()
+
+        return circuit
+
+
+    def addCreatedGate(self, gate: list): # add created gate
+        """
+        Add Created gate.
+
+        Prerequisites
+        ----------
+        - Created circuit.
+        - Created gate.
+
+        Parameters
+        ----------
+        gate : list
+            Created gate to add to the circuit.
+        """
+        self.__checkInputTypes(
+            ('gate', gate, (list,))
+        )
+
+        self.__addMultipleGate(gate, self.__circuitBody) # add to circuit
+
+        self.__updateQubits()
+
 
     def mcg(self, position: int, circuit: list, add: bool = True) -> list: # multi control gate
         """
         Add Multi Control gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int
             Qubit position or list of positions to add the control.
-        gate : list
+        circuit : list
             Gate or set of elements to add a control.
         add : bool
             Optional argument, True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
+        
+        Output
+        ----------
+        list
         """
         self.__checkInputTypes(
             ('position', position, (int, list)),
             ('circuit', circuit, (list,)),
             ('add', add, (bool,)),
         )
+        if isinstance(position, list):
+            for p in position:
+                    self.__checkInputTypes(('position', p, (int,)))
         
-
         gateSymbol = 'CTRL'
 
         if isinstance(position, int): # one postion
             circuit.append((position, gateSymbol))
 
         elif isinstance(position, list): # multiple positions
             for i in position:
                 circuit.append((i, gateSymbol)) # add all controls
 
         if add:
-            self.__addMultipleGate(circuit, self.__circuitBody, self.classicRegisters) # add to circuit
+            self.__addMultipleGate(circuit, self.__circuitBody) # add to circuit
+        
+        self.__updateQubits()
         
         return circuit
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Context.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Context.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/DeviceItem.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/Execution.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/__init__.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK/classes/apiConnection.py` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK/classes/apiConnection.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
         elif outputType == 'boolean':
             desMessage = bool(util.strtobool(message.text))
 
         elif outputType == 'json':
             desMessage = json.loads(message.content)
 
+            if isinstance(desMessage, str):
+                desMessage = json.loads(desMessage)
+
     else:
         raise APIConnectionError(f'Error {message.status_code} {message.reason}. {message.text}')
 
     return desMessage
 
 
 def apiConnection(*args): # manage api calls
@@ -27,14 +30,11 @@
     elif len(args) == 3: # normal get calls
         response = deserialize(requests.get(args[0], headers=args[1]), args[2])
     
     elif len(args) == 4: # create context
         response = deserialize(requests.post(args[0], data=args[1]), args[2])
     
     elif len(args) == 5: # post asset
-        # args[1].update({'Content-Type': 'application/json'})
         args[1].update({'Content-type': 'application/json; charset=utf-8'})
-        
-        # response = deserialize(requests.post(args[0], headers=args[1], data=args[2]), args[3])
         response = deserialize(requests.post(args[0], headers=args[1], data=args[2].encode('utf-8')), args[3])
     
     return response
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.3.2
+Version: 1.4
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.4/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 QuantumPathQSOAPySDK/classes/QuantumExecutionHistoryEntry.py
 QuantumPathQSOAPySDK/classes/SolutionItem.py
 QuantumPathQSOAPySDK/classes/__init__.py
 QuantumPathQSOAPySDK/classes/apiConnection.py
 test/test.py
 test/test_CircuitAnnealing.py
 test/test_CircuitFlow.py
-test/test_CircuitGates_MultipleGates.py
-test/test_CircuitGates_SimpleGates.py
+test/test_CircuitGates.py
 test/test_QSOAPlatform.py
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/setup.py` & `QuantumPathQSOAPySDK-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.3.2',
+  version='1.4',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.3.2/test/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.4/test/test_CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/test/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.4/test/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.3.2/test/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.4/test/test_QSOAPlatform.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         time.sleep(1)
         execution = qsoa.getQuantumExecutionResponse(application)
 
 
 ##################_____GET ENVIRONMENTS_____##################
 class Test_GetEnvironments(unittest.TestCase):
 
+    # GET ENVIRONMENTS
     def test_getEnvironments(self):
         qsoa = QSOAPlatform()
 
         environments = qsoa.getEnvironments()
 
         self.assertIsInstance(environments, dict)
         self.assertEqual(environments['default-environments'], {
@@ -47,14 +48,15 @@
             'lab': 'https://qsoa.quantumsoftt.com:10443/api/'
         })
 
 
 ##################_____GET ACTIVE ENVIRONMENT_____##################
 class Test_GetActiveEnvironment(unittest.TestCase):
 
+    # GET ACTIVE ENVIRONMENT
     def test_getActiveEnvironment(self):
         qsoa = QSOAPlatform()
 
         qsoa.setActiveEnvironment('pro')
         activeEnvironment = qsoa.getActiveEnvironment()
 
         self.assertIsInstance(activeEnvironment, tuple)
@@ -75,24 +77,26 @@
     
     # BAD ARGUMENT TYPE environmentName
     def test_setActiveEnvironment_badArgumentType_environmentName(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.setActiveEnvironment(0)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ENVIRONMENT
     def test_setActiveEnvironment_badEnvironment(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.setActiveEnvironment('badEnvironment')
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
 
 ##################_____ECHOPING_____##################
 class Test_Echoping(unittest.TestCase):
@@ -139,65 +143,70 @@
         qsoa = QSOAPlatform()
 
         username = 'username'
         password = 'cGFzc3dvcmQ=' # password encoded in Base64
 
         try:
             qsoa.authenticate(username, password)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT QUANTITY
     def test_authenticate_badArgumentQuantity(self):
         qsoa = QSOAPlatform()
 
         username = 'username'
 
         try:
             qsoa.authenticate(username)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'TypeError')
+            self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE username
     def test_authenticate_badArgumentType_username(self):
         qsoa = QSOAPlatform()
 
         username = 99
         password = 'password'
 
         try:
             qsoa.authenticate(username, password)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE password
     def test_authenticate_badArgumentType_password(self):
         qsoa = QSOAPlatform()
 
         username = 'username'
         password = 99
 
         try:
             qsoa.authenticate(username, password)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT FORMAT password
     def test_authenticate_badArgumentFormat_password(self):
         qsoa = QSOAPlatform()
 
         username = 'username'
         password = 'password'
 
         try:
             qsoa.authenticate(username, password)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'Base64Error')
 
 
 ##################_____AUTHENTICATEEX_____##################
 class Test_AuthenticateEx(unittest.TestCase):
@@ -232,55 +241,59 @@
         qsoa = QSOAPlatform()
 
         username = 'username'
         password = '5e884898da28047151d0e56f8dc6292773603d0d6aabbdd62a11ef721d1542d8' # password encrypted in SHA-256
 
         try:
             qsoa.authenticateEx(username, password)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT QUANTITY
     def test_authenticateEx_badArgumentQuantity(self):
         qsoa = QSOAPlatform()
 
         username = 'username'
 
         try:
             qsoa.authenticateEx(username)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'TypeError')
+            self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE username
     def test_authenticateEx_badArgumentType_username(self):
         qsoa = QSOAPlatform()
 
         username = 99
         password = 'password'
 
         try:
             qsoa.authenticateEx(username, password)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE password
     def test_authenticateEx_badArgumentType_password(self):
         qsoa = QSOAPlatform()
 
         username = 'username'
         password = 99
 
         try:
             qsoa.authenticateEx(username, password)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
 
 ##################_____QSOAPLATFORM_____##################
 class Test_QSOAPlatform(unittest.TestCase):
 
     # NOT AUTHENTICATE
     def test_QSOAPlatform_notAuthenticate(self):
@@ -318,54 +331,59 @@
     # AUTHENTICATE USER MANUALLY BAD CREDENTIALS
     def test_QSOAPlatform_manually_badCredentials(self):
         username = 'username'
         password = '5e884898da28047151d0e56f8dc6292773603d0d6aabbdd62a11ef721d1542d8' # password encrypted in SHA-256
 
         try:
             QSOAPlatform(username, password)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT QUANTITY
     def test_QSOAPlatform_badArgumentQuantity(self):
         username = 'username'
 
         try:
             QSOAPlatform(username)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'TypeError')
+            self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE username
     def test_QSOAPlatform_badArgumentType_username(self):
         username = 99
         password = 'password'
 
         try:
             QSOAPlatform(username, password)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE password
     def test_QSOAPlatform_badArgumentType_password(self):
         username = 'username'
         password = 99
 
         try:
             QSOAPlatform(username, password)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE configFile
     def test_QSOAPlatform_badArgumentType_configFile(self):
         try:
             QSOAPlatform(configFile=99)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
 
 ##################_____ECHOSTATUS_____##################
 class Test_Echostatus(unittest.TestCase):
@@ -392,14 +410,15 @@
 
     # NOT LOGGED IN
     def test_echouser_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.echouser()
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET VERSION_____##################
 class Test_GetVersion(unittest.TestCase):
@@ -414,14 +433,38 @@
 
     # NOT LOGGED IN
     def test_getVersion_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getVersion()
+            raise Exception
+
+        except Exception as e:
+            self.assertEqual(type(e).__name__, 'AuthenticationError')
+
+
+##################_____GET LICENCE INFO_____##################
+class Test_LicenceInfo(unittest.TestCase):
+
+    # GET LICENCE INFO
+    def test_getLlicenceInfo(self):
+        qsoa = QSOAPlatform(configFile=True)
+
+        version = qsoa.getLicenceInfo()
+
+        self.assertIsInstance(version, dict)
+
+    # NOT LOGGED IN
+    def test_getLlicenceInfo_notloggedIn(self):
+        qsoa = QSOAPlatform()
+
+        try:
+            qsoa.getLicenceInfo()
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM SOLUTION LIST_____##################
 class Test_GetQuantumSolutionList(unittest.TestCase):
@@ -436,14 +479,15 @@
 
     # NOT LOGGED IN
     def test_getQuantumSolutionList_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumSolutionList()
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM SOLUTIONS_____##################
 class Test_GetQuantumSolutions(unittest.TestCase):
@@ -461,14 +505,15 @@
 
     # NOT LOGGED IN
     def test_getQuantumSolutions_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumSolutions()
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM SOLUTION NAME_____##################
 class Test_GetQuantumSolutionName(unittest.TestCase):
@@ -485,36 +530,39 @@
     def test_getQuantumSolutionName_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getQuantumSolutionName(idSolution)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'NonExistentItemError')
+            self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getQuantumSolutionName_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumSolutionName(idSolution)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumSolutionName_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumSolutionName(idSolution_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM DEVICE LIST_____##################
 class Test_GetQuantumDeviceList(unittest.TestCase):
@@ -531,36 +579,39 @@
     def test_getQuantumDeviceList_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getQuantumDeviceList(idSolution)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getQuantumDeviceList_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumDeviceList(idSolution)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumDeviceList_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumDeviceList(idSolution_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM DEVICES_____##################
 class Test_GetQuantumDevices(unittest.TestCase):
@@ -580,36 +631,39 @@
     def test_getQuantumDevices_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getQuantumDevices(idSolution)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getQuantumDevices_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumDevices(idSolution)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # NOT LOGGED IN
     def test_getQuantumDevices_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumDevices(idSolution_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM DEVICE NAME_____##################
 class Test_GetQuantumDeviceName(unittest.TestCase):
@@ -626,60 +680,65 @@
     def test_getQuantumDeviceName_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getQuantumDeviceName(idSolution, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
     
     # BAD ARGUMENT idDevice
     def test_getQuantumDeviceName_badArgument_idDevice(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idDevice = 99
 
         try:
             qsoa.getQuantumDeviceName(idSolution_gates, idDevice)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'NonExistentItemError')
+            self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getQuantumDeviceName_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumDeviceName(idSolution, idDevice_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idDevice
     def test_getQuantumDeviceName_badArgumentType_idDevice(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idDevice = 'id'
 
         try:
             qsoa.getQuantumDeviceName(idSolution_gates, idDevice)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumDeviceName_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumDeviceName(idSolution_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM FLOW LIST_____##################
 class Test_GetQuantumFlowList(unittest.TestCase):
@@ -696,36 +755,39 @@
     def test_getQuantumFlowList_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getQuantumFlowList(idSolution)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getQuantumFlowList_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumFlowList(idSolution)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumFlowList_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumFlowList(idSolution_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM FLOWS_____##################
 class Test_GetQuantumDevices(unittest.TestCase):
@@ -745,36 +807,39 @@
     def test_getQuantumFlows_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getQuantumFlows(idSolution)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getQuantumFlows_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumFlows(idSolution)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumFlows_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumFlows(idSolution_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM FLOW NAME_____##################
 class Test_GetQuantumFlowName(unittest.TestCase):
@@ -791,60 +856,65 @@
     def test_getQuantumFlowName_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getQuantumFlowName(idSolution, idFlow_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
     
     # BAD ARGUMENT idFlow
     def test_getQuantumFlowName_badArgument_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = 99
 
         try:
             qsoa.getQuantumFlowName(idSolution_gates, idFlow)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'NonExistentItemError')
+            self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getQuantumFlowName_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumFlowName(idSolution, idFlow_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idFlow
     def test_getQuantumFlowName_badArgumentType_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = 'id'
 
         try:
             qsoa.getQuantumFlowName(idSolution_gates, idFlow)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumFlowName_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumFlowName(idSolution_gates, idFlow_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____RUN QUANTUM APPLICATION_____##################
 class Test_RunQuantumApplication(unittest.TestCase):
@@ -862,96 +932,104 @@
     def test_runQuantumApplication_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
     
     # BAD ARGUMENT idFlow
     def test_runQuantumApplication_badArgument_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = 99
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution_gates, idFlow, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT idDevice
     def test_runQuantumApplication_badArgument_idDevice(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idDevice = 99
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution_gates, idFlow_gates, idDevice)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE applicationName
     def test_runQuantumApplication_badArgumentType_applicationName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         applicationName = 99
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution_gates, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_runQuantumApplication_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
     
     # BAD ARGUMENT TYPE idFlow
     def test_runQuantumApplication_badArgumentType_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = '99'
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution_gates, idFlow, idDevice_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idDevice
     def test_runQuantumApplication_badArgumentType_idDevice(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idDevice = '99'
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution_gates, idFlow_gates, idDevice)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_runQuantumApplication_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.runQuantumApplication(applicationName, idSolution_gates, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____RUN QUANTUM EXECUTION RESPONSE_____##################
 class Test_RunQuantumExecutionResponse(unittest.TestCase):
@@ -1009,60 +1087,65 @@
     def test_getQuantumExecutionResponse_applicationObject_badArgumentType_application(self):
         qsoa = QSOAPlatform(configFile=True)
 
         application = 99
 
         try:
             qsoa.getQuantumExecutionResponse(application)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # MANUALLY BAD ARGUMENT TYPE executionToken
     def test_getQuantumExecutionResponse_manually_badArgumentType_executionToken(self):
         qsoa = QSOAPlatform(configFile=True)
 
         executionToken = 99
 
         try:
             qsoa.getQuantumExecutionResponse(executionToken, idSolution_gates, idFlow_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # MANUALLY BAD ARGUMENT TYPE idSolution
     def test_getQuantumExecutionResponse_manually_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = '99'
 
         try:
             qsoa.getQuantumExecutionResponse(executionToken_gates, idSolution, idFlow_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # MANUALLY BAD ARGUMENT TYPE idFlow
     def test_getQuantumExecutionResponse_manually_badArgumentType_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = '99'
 
         try:
             qsoa.getQuantumExecutionResponse(executionToken_gates, idSolution_gates, idFlow)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumExecutionResponse_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumExecutionResponse(executionToken_gates, idSolution_gates, idFlow_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____REPRESENT RESULTS_____##################
 class Test_RepresentResults(unittest.TestCase):
@@ -1116,63 +1199,68 @@
         qsoa = QSOAPlatform(configFile=True)
 
         executionToken = 'be2b3021-d294-472e-8265-3b39583ad172'
         execution = qsoa.getQuantumExecutionResponse(executionToken, idSolution_gates, idFlow_gates)
 
         try:
             qsoa.representResults(execution)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ExecutionObjectError')
 
     # BAD ARGUMENT resultIndex
     def test_representResults_badArgument_resultIndex(self):
         qsoa = QSOAPlatform(configFile=True)
 
         execution = qsoa.getQuantumExecutionResponse(executionToken_gates, idSolution_gates, idFlow_gates)
 
         try:
             qsoa.representResults(execution, 1)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'IndexError')
 
     # BAD ARGUMENT TYPE execution
     def test_representResults_badArgumentType_execution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         execution = 99
 
         try:
             qsoa.representResults(execution)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE resultIndex
     def test_representResults_badArgumentType_resultIndex(self):
         qsoa = QSOAPlatform(configFile=True)
 
         execution = qsoa.getQuantumExecutionResponse(executionToken_gates, idSolution_gates, idFlow_gates)
         resultIndex = '99'
 
         try:
             qsoa.representResults(execution, resultIndex)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_representResults_notloggedIn(self):
         qsoa = QSOAPlatform(configFile=True)
         execution = qsoa.getQuantumExecutionResponse(executionToken_gates, idSolution_gates, idFlow_gates)
         qsoa = QSOAPlatform()
 
         try:
             qsoa.representResults(execution)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET ASSET CATALOG_____##################
 class Test_GetAssetCatalog(unittest.TestCase):
@@ -1192,84 +1280,91 @@
     def test_getAssetCatalog_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.getAssetCatalog(idSolution, assetType_circuit, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetType
     def test_getAssetCatalog_badArgument_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 'assetType'
 
         try:
             qsoa.getAssetCatalog(idSolution_gates, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT assetLevel
     def test_getAssetCatalog_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 'assetLevel'
 
         try:
             qsoa.getAssetCatalog(idSolution_gates, assetType_circuit, assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_getAssetCatalog_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getAssetCatalog(idSolution, assetType_circuit, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetType
     def test_getAssetCatalog_badArgumentType_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 99
 
         try:
             qsoa.getAssetCatalog(idSolution_gates, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetLevel
     def test_getAssetCatalog_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 99
 
         try:
             qsoa.getAssetCatalog(idSolution_gates, assetType_circuit, assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getAssetCatalog_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getAssetCatalog(idSolution_gates, assetType_circuit, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET ASSET_____##################
 class Test_GetAsset(unittest.TestCase):
@@ -1289,84 +1384,91 @@
     def test_getAsset_badArgument_idAsset(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idAsset = 99
 
         try:
             qsoa.getAsset(idAsset, assetType_circuit, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetType
     def test_getAsset_badArgument_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 'assetType'
 
         try:
             qsoa.getAsset(idAsset, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT assetLevel
     def test_getAsset_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 'assetLevel'
 
         try:
             qsoa.getAsset(idAsset, assetType_circuit, assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE idAsset
     def test_getAsset_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idAsset = 'id'
 
         try:
             qsoa.getAsset(idAsset, assetType_circuit, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetType
     def test_getAsset_badArgumentType_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 99
 
         try:
             qsoa.getAsset(idAsset, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetLevel
     def test_getAsset_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 99
 
         try:
             qsoa.getAsset(idAsset, assetType_circuit, assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getAsset_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getAsset(idAsset, assetType_circuit, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____CREATE ASSET_____##################
 class Test_CreateAsset(unittest.TestCase):
@@ -1419,158 +1521,171 @@
         qsoa = QSOAPlatform(configFile=True)
 
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl))
 
     # BAD ARGUMENT idSolution
     def test_createAsset_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.createAsset(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetNamespace
     def test_createAsset_badArgument_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 'asset_namepace'
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetType
     def test_createAsset_badArgument_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 'assetType'
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT assetLevel
     def test_createAsset_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 'assetLevel'
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_createAsset_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.createAsset(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetName
     def test_createAsset_badArgumentType_assetName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetName = 99
 
         try:
             qsoa.createAsset(idSolution_gates, assetName, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetNamespace
     def test_createAsset_badArgumentType_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 99
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetDescription
     def test_createAsset_badArgumentType_assetDescription(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetDescription = 99
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetBody
     def test_createAsset_badArgumentType_assetBody(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetBody = 99
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetType
     def test_createAsset_badArgumentType_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 99
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetLevel
     def test_createAsset_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 99
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_createAsset_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____CREATE ASSET FLOW_____##################
 class Test_CreateAssetFlow(unittest.TestCase):
@@ -1617,158 +1732,171 @@
     def test_createAssetFlow_existingAsset(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(qsoa.getAsset(assetManagementData.getIdAsset(), assetType_flow, assetLevel_vl))
 
     # BAD ARGUMENT idSolution
     def test_createAssetFlow_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.createAssetFlow(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetNamespace
     def test_createAssetFlow_badArgument_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 'asset_namepace'
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetLevel
     def test_createAssetFlow_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 'assetLevel'
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
     
     # BAD ARGUMENT publish
     def test_createAssetFlow_badArgument_publish(self):
         qsoa = QSOAPlatform(configFile=True)
 
         publish = 99
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl, publish)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_createAssetFlow_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.createAssetFlow(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody,assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetName
     def test_createAssetFlow_badArgumentType_assetName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetName = 99
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetNamespace
     def test_createAssetFlow_badArgumentType_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 99
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetDescription
     def test_createAssetFlow_badArgumentType_assetDescription(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetDescription = 99
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetBody
     def test_createAssetFlow_badArgumentType_assetBody(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetBody = 99
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetLevel
     def test_createAssetFlow_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 99
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE publish
     def test_createAssetFlow_badArgumentType_publish(self):
         qsoa = QSOAPlatform(configFile=True)
 
         publish = 99
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl, publish)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_createAssetFlow_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.createAssetFlow(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____PUBLISH FLOW_____##################
 
@@ -1790,53 +1918,57 @@
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = 99
         publish = True
 
         try:
             qsoa.publishFlow(idFlow, publish)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE idFlow
     def test_publishFlow_badArgumentType_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = '99'
         publish = True
 
         try:
             qsoa.publishFlow(idFlow, publish)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE publish
     def test_publishFlow_badArgumentType_publish(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = 596
         publish = 99
 
         try:
             qsoa.publishFlow(idFlow, publish)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_publishFlow_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         idFlow = 596
         publish = True
 
         try:
             qsoa.publishFlow(idFlow, publish)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____UPDATE ASSET_____##################
 class Test_UpdateAsset(unittest.TestCase):
@@ -1873,14 +2005,16 @@
 
         assetManagementData1 = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         assetManagementData2 = qsoa.createAsset(idSolution_gates, assetName_circuit+'2', assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData2.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         try:
             qsoa.updateAsset(asset, assetName_circuit)
+            raise Exception
+        
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(qsoa.getAsset(assetManagementData1.getIdAsset(), assetType_circuit, assetLevel_vl))
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT QUANTITY
@@ -1890,31 +2024,33 @@
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT assetNamespace
     def test_updateAsset_badArgument_username(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetNamespace = 'new_assetNamespace'
 
         try:
             qsoa.updateAsset(asset, assetNamespace=new_assetNamespace)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT assetType
@@ -1925,17 +2061,18 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetType = 'new_assetType'
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=new_assetType)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT assetLevel
     def test_updateAsset_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
@@ -1943,97 +2080,103 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetLevel = 'new_assetLevel'
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=assetType_gates, assetLevel=new_assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE asset
     def test_updateAsset_badArgumentType_asset(self):
         qsoa = QSOAPlatform(configFile=True)
 
         asset = 99
 
         try:
             qsoa.updateAsset(asset)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetName
     def test_updateAsset_badArgumentType_assetName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetName = 99
 
         try:
             qsoa.updateAsset(asset, assetName=new_assetName)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetNamespace
     def test_updateAsset_badArgumentType_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetNamespace = 99
 
         try:
             qsoa.updateAsset(asset, assetNamespace=new_assetNamespace)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetDescription
     def test_updateAsset_badArgumentType_assetDescription(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetDescription = 99
 
         try:
             qsoa.updateAsset(asset, assetDescription=new_assetDescription)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetBody
     def test_updateAsset_badArgumentType_assetBody(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 99
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetType
     def test_updateAsset_badArgumentType_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
@@ -2041,17 +2184,18 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetType = 99
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=new_assetType)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetLevel
     def test_updateAsset_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
@@ -2059,31 +2203,33 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetLevel = 99
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=assetType_gates, assetLevel=new_assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # NOT LOGGED IN
     def test_updateAsset_notloggedIn(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         qsoa = QSOAPlatform()
 
         try:
             qsoa.updateAsset(asset)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
         
         qsoa = QSOAPlatform(configFile=True)
         qsoa.deleteAsset(asset)
 
@@ -2107,38 +2253,41 @@
     def test_getAssetManagementResult_badArgument_lifecycleToken(self):
         qsoa = QSOAPlatform(configFile=True)
 
         lifecycleToken = 'lifecycleToken'
 
         try:
             qsoa.getAssetManagementResult(lifecycleToken)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE lifecycleToken
     def test_getAssetManagementResult_badArgumentType_lifecycleToken(self):
         qsoa = QSOAPlatform(configFile=True)
 
         lifecycleToken = 99
 
         try:
             qsoa.getAssetManagementResult(lifecycleToken)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getAssetManagementResult_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         lifecycleToken = 'lifecycleToken'
 
         try:
             qsoa.getAssetManagementResult(lifecycleToken)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____DELETE ASSET_____##################
 class Test_DeleteAsset(unittest.TestCase):
@@ -2174,14 +2323,15 @@
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         idAsset = 99
 
         try:
             qsoa.deleteAsset(idAsset, assetType_circuit)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT assetType
@@ -2192,14 +2342,15 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         idAsset = asset.getId()
         assetType = 'assetType'
 
         try:
             qsoa.deleteAsset(idAsset, assetType)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE asset
@@ -2208,34 +2359,36 @@
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
 
         asset = 99
 
         try:
             qsoa.deleteAsset(asset)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl))
 
     # BAD ARGUMENT TYPE idAsset
     def test_deleteAsset_badArgumentType_idAsset(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         idAsset = 'id'
 
         try:
             qsoa.deleteAsset(idAsset, assetType_circuit)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetType
     def test_deleteAsset_badArgumentType_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
@@ -2243,31 +2396,33 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         idAsset = asset.getId()
         assetType = 99
 
         try:
             qsoa.deleteAsset(idAsset, assetType)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # NOT LOGGED IN
     def test_deleteAsset_notloggedIn(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         qsoa = QSOAPlatform()
 
         try:
             qsoa.deleteAsset(asset)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
         
         qsoa = QSOAPlatform(configFile=True)
         qsoa.deleteAsset(asset)
 
@@ -2290,96 +2445,104 @@
     def test_getQuantumExecutionHistoric_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.getQuantumExecutionHistoric(idSolution=idSolution)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idFlow
     def test_getQuantumExecutionHistoric_badArgumentType_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = 'id'
 
         try:
             qsoa.getQuantumExecutionHistoric(idFlow=idFlow)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idDevice
     def test_getQuantumExecutionHistoric_badArgumentType_idDevice(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idDevice = 'id'
 
         try:
             qsoa.getQuantumExecutionHistoric(idDevice=idDevice)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE dateFrom
     def test_getQuantumExecutionHistoric_badArgumentType_dateFrom(self):
         qsoa = QSOAPlatform(configFile=True)
 
         dateFrom = 99
 
         try:
             qsoa.getQuantumExecutionHistoric(dateFrom=dateFrom)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE isSimulator
     def test_getQuantumExecutionHistoric_badArgumentType_isSimulator(self):
         qsoa = QSOAPlatform(configFile=True)
 
         isSimulator = 99
 
         try:
             qsoa.getQuantumExecutionHistoric(isSimulator=isSimulator)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE top
     def test_getQuantumExecutionHistoric_badArgumentType_top(self):
         qsoa = QSOAPlatform(configFile=True)
 
         top = 'top'
 
         try:
             qsoa.getQuantumExecutionHistoric(top=top)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE resultType
     def test_getQuantumExecutionHistoric_badArgumentType_resultType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         resultType = 99
 
         try:
             qsoa.getQuantumExecutionHistoric(resultType=resultType)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumExecutionHistoric_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumExecutionHistoric(idSolution_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____GET QUANTUM EXECUTION HISTORIC RESULT_____##################
 class Test_GetQuantumExecutionHistoricResult(unittest.TestCase):
@@ -2399,29 +2562,31 @@
     def test_getQuantumExecutionHistoricResult_badArgumentType_idResult(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idResult = 'id'
 
         try:
             qsoa.getQuantumExecutionHistoricResult(idResult)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_getQuantumExecutionHistoricResult_notloggedIn(self):
         qsoa = QSOAPlatform(configFile=True)
 
         quantumExecutionHistoryEntryList = qsoa.getQuantumExecutionHistoric(idSolution_gates)
         idResult = quantumExecutionHistoryEntryList[0].getIdResult()
 
         qsoa = QSOAPlatform()
 
         try:
             qsoa.getQuantumExecutionHistoricResult(idResult)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____RUN QUANTUM APPLICATION SYNC_____##################
 class Test_RunQuantumApplicationSync(unittest.TestCase):
@@ -2438,96 +2603,104 @@
     def test_runQuantumApplicationSync_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
     
     # BAD ARGUMENT idFlow
     def test_runQuantumApplicationSync_badArgument_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = 99
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution_gates, idFlow, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT idDevice
     def test_runQuantumApplicationSync_badArgument_idDevice(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idDevice = 99
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution_gates, idFlow_gates, idDevice)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT TYPE applicationName
     def test_runQuantumApplicationSync_badArgumentType_applicationName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         applicationName = 99
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution_gates, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_runQuantumApplicationSync_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
     
     # BAD ARGUMENT TYPE idFlow
     def test_runQuantumApplicationSync_badArgumentType_idFlow(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idFlow = '99'
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution_gates, idFlow, idDevice_gates)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idDevice
     def test_runQuantumApplicationSync_badArgumentType_idDevice(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idDevice = '99'
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution_gates, idFlow_gates, idDevice)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_runQuantumApplicationSync_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.runQuantumApplicationSync(applicationName, idSolution_gates, idFlow_gates, idDevice_gates)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____CREATE ASSET SYNC_____##################
 class Test_CreateAssetSync(unittest.TestCase):
@@ -2580,158 +2753,171 @@
         qsoa = QSOAPlatform(configFile=True)
 
 
         assetManagementData = qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl))
 
     # BAD ARGUMENT idSolution
     def test_createAssetSync_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.createAssetSync(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetNamespace
     def test_createAssetSync_badArgument_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 'asset_namepace'
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetType
     def test_createAssetSync_badArgument_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 'assetType'
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT assetLevel
     def test_createAssetSync_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 'assetLevel'
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_createAssetSync_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.createAssetSync(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetName
     def test_createAssetSync_badArgumentType_assetName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetName = 99
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetNamespace
     def test_createAssetSync_badArgumentType_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 99
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetDescription
     def test_createAssetSync_badArgumentType_assetDescription(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetDescription = 99
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetBody
     def test_createAssetSync_badArgumentType_assetBody(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetBody = 99
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetType
     def test_createAssetSync_badArgumentType_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetType = 99
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetLevel
     def test_createAssetSync_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 99
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_createAssetSync_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.createAssetSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____CREATE ASSET FLOW SYNC_____##################
 class Test_CreateAssetFlowSync(unittest.TestCase):
@@ -2778,158 +2964,171 @@
     def test_createAssetFlowSync_existingAsset(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(qsoa.getAsset(assetManagementData.getIdAsset(), assetType_flow, assetLevel_vl))
 
     # BAD ARGUMENT idSolution
     def test_createAssetFlowSync_badArgument_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetNamespace
     def test_createAssetFlowSync_badArgument_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 'asset_namepace'
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
 
     # BAD ARGUMENT assetLevel
     def test_createAssetFlowSync_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 'assetLevel'
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
     
     # BAD ARGUMENT publish
     def test_createAssetFlowSync_badArgument_publish(self):
         qsoa = QSOAPlatform(configFile=True)
 
         publish = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl, publish)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE idSolution
     def test_createAssetFlowSync_badArgumentType_idSolution(self):
         qsoa = QSOAPlatform(configFile=True)
 
         idSolution = 'id'
 
         try:
             qsoa.createAssetFlowSync(idSolution, assetName_circuit, assetNamespace, assetDescription, assetBody,assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetName
     def test_createAssetFlowSync_badArgumentType_assetName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetName = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetNamespace
     def test_createAssetFlowSync_badArgumentType_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetNamespace = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetDescription
     def test_createAssetFlowSync_badArgumentType_assetDescription(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetDescription = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetBody
     def test_createAssetFlowSync_badArgumentType_assetBody(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetBody = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetLevel
     def test_createAssetFlowSync_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetLevel = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE publish
     def test_createAssetFlowSync_badArgumentType_publish(self):
         qsoa = QSOAPlatform(configFile=True)
 
         publish = 99
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl, publish)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # NOT LOGGED IN
     def test_createAssetFlowSync_notloggedIn(self):
         qsoa = QSOAPlatform()
 
         try:
             qsoa.createAssetFlowSync(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetLevel_vl)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 
 ##################_____UPDATE ASSET SYNC_____##################
 class Test_UpdateAssetSync(unittest.TestCase):
@@ -2966,14 +3165,16 @@
 
         assetManagementData1 = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         assetManagementData2 = qsoa.createAsset(idSolution_gates, assetName_circuit+'2', assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData2.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         try:
             qsoa.updateAssetSync(asset, assetName_circuit)
+            raise Exception
+        
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(qsoa.getAsset(assetManagementData1.getIdAsset(), assetType_circuit, assetLevel_vl))
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT QUANTITY
@@ -2983,31 +3184,33 @@
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
 
         try:
             qsoa.updateAssetSync(asset, assetBody=new_assetBody)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT assetNamespace
     def test_updateAsset_badArgument_username(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetNamespace = 'new_assetNamespace'
 
         try:
             qsoa.updateAsset(asset, assetNamespace=new_assetNamespace)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'APIConnectionError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT assetType
@@ -3018,17 +3221,18 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetType = 'new_assetType'
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=new_assetType)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT assetLevel
     def test_updateAsset_badArgument_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
@@ -3036,97 +3240,103 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetLevel = 'new_assetLevel'
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=assetType_gates, assetLevel=new_assetLevel)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'ValueError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE asset
     def test_updateAsset_badArgumentType_asset(self):
         qsoa = QSOAPlatform(configFile=True)
 
         asset = 99
 
         try:
             qsoa.updateAsset(asset)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
 
     # BAD ARGUMENT TYPE assetName
     def test_updateAsset_badArgumentType_assetName(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetName = 99
 
         try:
             qsoa.updateAsset(asset, assetName=new_assetName)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetNamespace
     def test_updateAsset_badArgumentType_assetNamespace(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetNamespace = 99
 
         try:
             qsoa.updateAsset(asset, assetNamespace=new_assetNamespace)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetDescription
     def test_updateAsset_badArgumentType_assetDescription(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetDescription = 99
 
         try:
             qsoa.updateAsset(asset, assetDescription=new_assetDescription)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetBody
     def test_updateAsset_badArgumentType_assetBody(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 99
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetType
     def test_updateAsset_badArgumentType_assetType(self):
         qsoa = QSOAPlatform(configFile=True)
 
@@ -3134,17 +3344,18 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetType = 99
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=new_assetType)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # BAD ARGUMENT TYPE assetLevel
     def test_updateAsset_badArgumentType_assetLevel(self):
         qsoa = QSOAPlatform(configFile=True)
 
@@ -3152,31 +3363,33 @@
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         new_assetBody = 'circuit={"cols":[["H"]]}'
         new_assetLevel = 99
 
         try:
             qsoa.updateAsset(asset, assetBody=new_assetBody, assetType=assetType_gates, assetLevel=new_assetLevel)
+            raise Exception
 
         except Exception as e:
-            self.assertEqual(type(e).__name__, 'ValueError')
+            self.assertEqual(type(e).__name__, 'TypeError')
         
         qsoa.deleteAsset(asset)
 
     # NOT LOGGED IN
     def test_updateAsset_notloggedIn(self):
         qsoa = QSOAPlatform(configFile=True)
 
         assetManagementData = qsoa.createAsset(idSolution_gates, assetName_circuit, assetNamespace, assetDescription, assetBody, assetType_gates, assetLevel_vl)
         asset = qsoa.getAsset(assetManagementData.getIdAsset(), assetType_circuit, assetLevel_vl)
 
         qsoa = QSOAPlatform()
 
         try:
             qsoa.updateAsset(asset)
+            raise Exception
 
         except Exception as e:
             self.assertEqual(type(e).__name__, 'AuthenticationError')
         
         qsoa = QSOAPlatform(configFile=True)
         qsoa.deleteAsset(asset)
```

