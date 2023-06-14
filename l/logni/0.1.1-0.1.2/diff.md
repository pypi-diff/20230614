# Comparing `tmp/logni-0.1.1.tar.gz` & `tmp/logni-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logni-0.1.1.tar", last modified: Fri Oct 11 10:20:30 2019, max compression
+gzip compressed data, was "logni-0.1.2.tar", last modified: Wed Jun 14 11:34:06 2023, max compression
```

## Comparing `logni-0.1.1.tar` & `logni-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2019-10-11 10:20:30.000000 logni-0.1.1/
--rw-r--r--   0 erik      (1000) erik      (1000)     2116 2019-10-10 10:22:56.000000 logni-0.1.1/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2019-10-11 10:20:30.000000 logni-0.1.1/logni.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     3501 2019-10-11 10:20:30.000000 logni-0.1.1/logni.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      159 2019-10-11 10:20:30.000000 logni-0.1.1/logni.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        6 2019-10-11 10:20:30.000000 logni-0.1.1/logni.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2019-10-11 10:20:30.000000 logni-0.1.1/logni.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       79 2019-10-11 10:20:30.000000 logni-0.1.1/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     3501 2019-10-11 10:20:30.000000 logni-0.1.1/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1269 2019-10-11 10:20:24.000000 logni-0.1.1/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2019-10-11 10:20:30.000000 logni-0.1.1/logni/
--rw-r--r--   0 erik      (1000) erik      (1000)     8954 2019-10-10 10:12:56.000000 logni-0.1.1/logni/logni.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-14 11:34:06.161782 logni-0.1.2/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4386 2023-06-14 11:34:06.161782 logni-0.1.2/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     2855 2021-12-29 19:26:16.000000 logni-0.1.2/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-14 11:34:06.161782 logni-0.1.2/logni/
+-rw-r--r--   0 erik      (1000) erik      (1000)      359 2022-03-08 08:38:16.000000 logni-0.1.2/logni/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      333 2022-03-08 08:40:10.000000 logni-0.1.2/logni/cfgni.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1285 2022-03-08 09:49:17.000000 logni-0.1.2/logni/consolestream.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1221 2021-12-29 18:05:57.000000 logni-0.1.2/logni/filestream.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9937 2022-03-08 08:54:31.000000 logni-0.1.2/logni/logni.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1736 2021-12-29 17:55:24.000000 logni-0.1.2/logni/utilni.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-14 11:34:06.161782 logni-0.1.2/logni.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4386 2023-06-14 11:34:06.000000 logni-0.1.2/logni.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      251 2023-06-14 11:34:06.000000 logni-0.1.2/logni.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-06-14 11:34:06.000000 logni-0.1.2/logni.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        6 2023-06-14 11:34:06.000000 logni-0.1.2/logni.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       79 2023-06-14 11:34:06.161782 logni-0.1.2/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1228 2023-06-14 11:33:15.000000 logni-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `logni-0.1.1/logni.egg-info/PKG-INFO` & `logni-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,89 @@
 Metadata-Version: 2.1
 Name: logni
-Version: 0.1.1
+Version: 0.1.2
 Summary: python library for event logging and application states
 Home-page: https://github.com/erikni/logni.py
 Author: Erik Brozek
 Author-email: erik@brozek.name
 License: MIT
 Download-URL: https://github.com/erik/logni.py/archive/master.zip
-Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/441b9bb67c0f4956b5d4bcfbe76e00c6)](https://www.codacy.com/manual/erikni/logni.py?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=erikni/logni.py&amp;utm_campaign=Badge_Grade)
+Description: [![PyPI Version](https://shields.mitmproxy.org/pypi/v/logni.svg)](https://pypi.org/project/logni/)
+        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/441b9bb67c0f4956b5d4bcfbe76e00c6)](https://www.codacy.com/manual/erikni/logni.py?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=erikni/logni.py&amp;utm_campaign=Badge_Grade)
         [![Github Releases](https://img.shields.io/github/downloads/atom/atom/latest/total.svg)](https://github.com/erikni/logni.py/releases)
         [![Build Status](https://api.travis-ci.org/erikni/logni.py.svg?branch=develop)](http://travis-ci.org/erikni/logni.py)
         [![Maintainability](https://api.codeclimate.com/v1/badges/27cb403386b704028bb5/maintainability)](https://codeclimate.com/github/erikni/logni.py/maintainability)
+        [![Known Vulnerabilities](https://snyk.io//test/github/erikni/logni.py/badge.svg?targetFile=requirements.txt)](https://snyk.io//test/github/erikni/logni.py?targetFile=requirements.txt)
         [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENCE)
         
         # logni.py
         logni is a python library for event logging and application states
         
         ## How to install?
-        - git (github)
-        - pip (python packages -> todo)
+        - git (github) #1
+        - wget (github) #2
+        - pip (python packages) #3
         
         
-        Install from Github
+        Install from Github #1
         ```
         $ git clone https://github.com/erikni/logni.py.git
         $ cd logni.py
-        $ pip install -r requirements.txt
-        $ python src/logni.py
+        $ sudo pip3 install -r requirements.txt
+        $ python3 test/example/basic_example.py
+        ```
+        
+        Install from Github #2
+        ```
+        $ sudo wget -O - https://raw.githubusercontent.com/erikni/logni.py/master/setup.sh | bash
+        ```
+        
+        Install with PIP (Python Package Installer) #3
+        ```
+        $ pip3 install logni
+        $ python3 /usr/local/lib/python3/dist-packages/logni/logni.py
         ```
         
         ## Example
         
         ```
-        $ python
+        $ python3
         
-        >>> import logni
-        >>> log = logni.Logni()
+        >>> from logni import log
         
         >>> log.mask('ALL')
-        >>> log.stderr(1)
+        >>> log.console(1)
         
-        $ log.critical('critical message')
+        >>> log.critical('critical message')
         2016/04/01 22:08:18 [15489] F4: critical message [7e995d1a] {logni.py:fatal():161}
         
-        $ log.error('error message #%s', time.time(), priority=4)
+        >>> log.error('error message #%s', time.time(), priority=4)
         2016/04/01 22:08:18 [15489] E4: error message #1459541298.29 [58138001] {logni.py:error():164}
         
-        $ log.warn('warning message #%s', time.time(), priority=3)
+        >>> log.warn('warning message #%s', time.time(), priority=3)
         2016/04/01 22:08:18 [15489] W3: warning message #1459541298.29 [91b483ab] {logni.py:warn():167}
         
-        $ log.info('info message #%s', time.time(), priority=2)
+        >>> log.info('info message #%s', time.time(), priority=2)
         2016/04/01 22:08:18 [15489] I2: info message #1459541298.29 [eaf58c15] {logni.py:info():170}
         
-        $ log.debug('debug message #%s', time.time(), priority=1)
+        >>> log.debug('debug message #%s', time.time(), priority=1)
         2016/04/01 22:08:18 [15489] D1: debug message #1459541298.29 [37e911b8] {logni.py:debug():173}
         ```
         
+        ## Support
+        
+        Logni support python >= 3.6
+        
+        ## Roadmap
+        
+        Current roadmap:
+        
+        * new integration (rollbar, logentries, sentry, ... )
+        * performance improvement.
+        
         ## Test
         
         [test/unit](https://github.com/erikni/logni.py/tree/develop/test/unit)
         
         ## Contribution
         
         [Pull Requests](https://github.com/erikni/logni.py/pulls) are very welcome.
@@ -67,18 +91,17 @@
         # Licence
         
         [GNU General Public License v3.0](LICENSE)
         
 Keywords: logging,logging-library,logger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Logging
-Requires-Python: >=2.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `logni-0.1.1/PKG-INFO` & `logni-0.1.2/logni.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,89 @@
 Metadata-Version: 2.1
 Name: logni
-Version: 0.1.1
+Version: 0.1.2
 Summary: python library for event logging and application states
 Home-page: https://github.com/erikni/logni.py
 Author: Erik Brozek
 Author-email: erik@brozek.name
 License: MIT
 Download-URL: https://github.com/erik/logni.py/archive/master.zip
-Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/441b9bb67c0f4956b5d4bcfbe76e00c6)](https://www.codacy.com/manual/erikni/logni.py?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=erikni/logni.py&amp;utm_campaign=Badge_Grade)
+Description: [![PyPI Version](https://shields.mitmproxy.org/pypi/v/logni.svg)](https://pypi.org/project/logni/)
+        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/441b9bb67c0f4956b5d4bcfbe76e00c6)](https://www.codacy.com/manual/erikni/logni.py?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=erikni/logni.py&amp;utm_campaign=Badge_Grade)
         [![Github Releases](https://img.shields.io/github/downloads/atom/atom/latest/total.svg)](https://github.com/erikni/logni.py/releases)
         [![Build Status](https://api.travis-ci.org/erikni/logni.py.svg?branch=develop)](http://travis-ci.org/erikni/logni.py)
         [![Maintainability](https://api.codeclimate.com/v1/badges/27cb403386b704028bb5/maintainability)](https://codeclimate.com/github/erikni/logni.py/maintainability)
+        [![Known Vulnerabilities](https://snyk.io//test/github/erikni/logni.py/badge.svg?targetFile=requirements.txt)](https://snyk.io//test/github/erikni/logni.py?targetFile=requirements.txt)
         [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENCE)
         
         # logni.py
         logni is a python library for event logging and application states
         
         ## How to install?
-        - git (github)
-        - pip (python packages -> todo)
+        - git (github) #1
+        - wget (github) #2
+        - pip (python packages) #3
         
         
-        Install from Github
+        Install from Github #1
         ```
         $ git clone https://github.com/erikni/logni.py.git
         $ cd logni.py
-        $ pip install -r requirements.txt
-        $ python src/logni.py
+        $ sudo pip3 install -r requirements.txt
+        $ python3 test/example/basic_example.py
+        ```
+        
+        Install from Github #2
+        ```
+        $ sudo wget -O - https://raw.githubusercontent.com/erikni/logni.py/master/setup.sh | bash
+        ```
+        
+        Install with PIP (Python Package Installer) #3
+        ```
+        $ pip3 install logni
+        $ python3 /usr/local/lib/python3/dist-packages/logni/logni.py
         ```
         
         ## Example
         
         ```
-        $ python
+        $ python3
         
-        >>> import logni
-        >>> log = logni.Logni()
+        >>> from logni import log
         
         >>> log.mask('ALL')
-        >>> log.stderr(1)
+        >>> log.console(1)
         
-        $ log.critical('critical message')
+        >>> log.critical('critical message')
         2016/04/01 22:08:18 [15489] F4: critical message [7e995d1a] {logni.py:fatal():161}
         
-        $ log.error('error message #%s', time.time(), priority=4)
+        >>> log.error('error message #%s', time.time(), priority=4)
         2016/04/01 22:08:18 [15489] E4: error message #1459541298.29 [58138001] {logni.py:error():164}
         
-        $ log.warn('warning message #%s', time.time(), priority=3)
+        >>> log.warn('warning message #%s', time.time(), priority=3)
         2016/04/01 22:08:18 [15489] W3: warning message #1459541298.29 [91b483ab] {logni.py:warn():167}
         
-        $ log.info('info message #%s', time.time(), priority=2)
+        >>> log.info('info message #%s', time.time(), priority=2)
         2016/04/01 22:08:18 [15489] I2: info message #1459541298.29 [eaf58c15] {logni.py:info():170}
         
-        $ log.debug('debug message #%s', time.time(), priority=1)
+        >>> log.debug('debug message #%s', time.time(), priority=1)
         2016/04/01 22:08:18 [15489] D1: debug message #1459541298.29 [37e911b8] {logni.py:debug():173}
         ```
         
+        ## Support
+        
+        Logni support python >= 3.6
+        
+        ## Roadmap
+        
+        Current roadmap:
+        
+        * new integration (rollbar, logentries, sentry, ... )
+        * performance improvement.
+        
         ## Test
         
         [test/unit](https://github.com/erikni/logni.py/tree/develop/test/unit)
         
         ## Contribution
         
         [Pull Requests](https://github.com/erikni/logni.py/pulls) are very welcome.
@@ -67,18 +91,17 @@
         # Licence
         
         [GNU General Public License v3.0](LICENSE)
         
 Keywords: logging,logging-library,logger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Logging
-Requires-Python: >=2.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `logni-0.1.1/setup.py` & `logni-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 python setup
 """
 
 import sys
 import setuptools
 
 
-if sys.version_info < (2, 7):
-	sys.exit("Python 2.7 or newer is required for logni.py")
+if sys.version_info < (3, 6):
+	sys.exit("Python 3.7 or newer is required for logni.py")
 
 
 def readme():
 	""" readme """
 
 	return open('README.md', 'r').read()
 
@@ -20,29 +20,28 @@
 def version():
 	""" version """
 
 	return open('version.properties', 'r').read()
 
 
 setuptools.setup(name='logni',\
-  version='0.1.1',\
+  version='0.1.2',\
   author='Erik Brozek',\
   author_email='erik@brozek.name',\
   description='python library for event logging and application states',\
   long_description=readme(),\
   long_description_content_type='text/markdown',\
   url='https://github.com/erikni/logni.py',\
   download_url='https://github.com/erik/logni.py/archive/master.zip',\
   packages=['logni'],\
   classifiers=['Development Status :: 4 - Beta',\
-    'Programming Language :: Python :: 2',\
-    'Programming Language :: Python :: 2.7',\
     'Programming Language :: Python :: 3',\
-    'Programming Language :: Python :: 3.5',\
-    'Programming Language :: Python :: 3.6',\
     'Programming Language :: Python :: 3.7',\
     'Programming Language :: Python :: 3.8',\
+    'Programming Language :: Python :: 3.9',\
+    'Programming Language :: Python :: 3.10',\
+    'Programming Language :: Python :: 3.11',\
     'License :: OSI Approved :: MIT License',\
     'Topic :: System :: Logging'],\
-  python_requires='>=2.7',\
-  keywords=['logging', 'logging-library', 'logger'],
+  python_requires='>=3.7',\
+  keywords=['logging', 'logging-library', 'logger'],\
   license='MIT')
```

### Comparing `logni-0.1.1/logni/logni.py` & `logni-0.1.2/logni/logni.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,400 +11,437 @@
  an express grant of patent rights.
 
  see all: https://github.com/erikni/logni.py/blob/master/LICENSE
 
  ---
 
  logni is python library for event logging and application states
+
+ Example:
+
+ log = logni.Logni({'debugMode':True, 'mask':'ALL', 'console':True})
+
+ log.info('informational message with priority=4')
+ log.info('informational message with priority=3', priority=3)
+
+ log.debug('debug message [ts=%s] with priority=2', time.time(), priority=2)
+ log.error('error message with priority=1', priority=1)
+ log.warn('warning message with priority=1', priority=1)
 """
 
+# pylint: disable=cyclic-import
+import sys
 import time
 import random
 import traceback
 import os
 import os.path
-import sys
+import functools
+import logni
 
 MAX_LEN = 10000
+CHARSET = 'utf8'
+TIME_FORMAT = '%Y/%m/%d %H:%M:%S'
 
+class Logni():
+	""" Logni object """
 
-class Logni(object):
-	""" logni object """
+	# global
+	__config = {\
+		'debugMode': False,
+		'charset': CHARSET,
+		'color': False,
+		'console': True,
+		'log_file': None,
+		'env': '',
+		'flush': True,
+		'name': 'LOG',
+		'mask': 'ALL',
+		'maxLen': MAX_LEN,
+		'strip': True,
+		'stackOffset': 1,
+		'stackDepth': 2,
+		'timeFormat': TIME_FORMAT,
+		'revision': ''}
 
-	def __init__(self, config=None):
-		""" init """
 
-		# global
-		self.__config = {\
-			'debugMode': False,
-			'charset': 'utf8',
-			'color': 0,
-			'console': 0,
-			'env': '',
-			'flush': 1,
-			'mask': 'ALL',
-			'maxLen': MAX_LEN,
-			'strip': 0,
-			'stackOffset': 0,
-			'stackDepth': 1,
-			'timeFormat': '%Y/%m/%d %H:%M:%S',
-			'revision': ''}
+	def __init__(self, config=None):
+		""" Init
 
-		self.__file = None
+		@param config """
 
+		self.cfg = logni.Cfgni()
 		if not config:
 			config = {}
 
-		for cfgName in config:
-			self.__config[cfgName] = config[cfgName]
-
-		# colors: https://getbootstrap.com/docs/4.1/components/alerts/
-		# self.__logniColors = {\
-		#	'primary':"#004085", # blue light
-		#	'secondary':"#383d41", # seda
-		#	'success':"#155724", # green light
-		#	'danger':"#721c24", # ping light
-		#	'warning':"#856404", # yellow light
-		#	'info':"#0c5460", # blue-green light
-		#	'light':"#818182", # svetle seda
-		#	'dark':"#1b1e21"} # tmave seda
+		# environment variable values
+		for env_name in ('mask', 'console', 'name', 'file'):
+			if os.environ.get('LOGNI_%s' % env_name.upper()):
+				config[env_name] = os.environ['LOGNI_%s' % env_name.upper()]
+
+		# config
+		for cfg_name in config:
+			self.__config[cfg_name] = config[cfg_name]
+
+		# init
+		self.__name = self.__config.get('name', 'LOG').upper()
+		self.__util = logni.Util(self.__config)
+		self.__file = logni.FileStream(self.__config)
+		self.__console = logni.ConsoleStream(self.__config)
 
 		# severity
-		self.__logniMaskSeverity = {}
-		self.__logniSeverityColors = { \
-			'DEBUG': "light",
-			'INFO': "primary",
-			'WARN': "warning",
-			'ERROR': "danger",
-			'CRITICAL': "danger"}
-
-		self.__logniMaskSeverityFull = ["DEBUG", "INFO", "WARN", "ERROR", "CRITICAL"]
-
-		# severity (sortname)
-		self.__logniMaskSeverityShort = []
-		for severityName in self.__logniMaskSeverityFull:
-			_short = severityName[:1]
+		self.__logni_mask_severity = {}
+		self.__logni_mask_severity_full = [\
+			self.cfg.SEVERITY_DEBUG,\
+			self.cfg.SEVERITY_INFO,\
+			self.cfg.SEVERITY_WARN,\
+			self.cfg.SEVERITY_ERROR,\
+			self.cfg.SEVERITY_CRITICAL]
+
+		# severity (shortname)
+		self.__logni_mask_severity_short = []
+		for severity_name in self.__logni_mask_severity_full:
+			_short = severity_name[:1]
 
-			self.__logniMaskSeverityShort.append(_short)
-			self.__logniMaskSeverity[_short] = self.__setPriority(5)
+			self.__logni_mask_severity_short.append(_short)
+			self.__logni_mask_severity[_short] = self.__util.set_priority(5)
 
 		# default
-		self.mask('ALL')
-		self.console(True)
+		self.mask(self.__config.get('mask', 'ALL'))
+		self.console(self.__config.get('console', True))
 
-		if config.get('mask'):
-			self.mask(config['mask'])
 
+	def file(self, log_file):
+		""" File output
 
-	def file(self, logFile):
-		""" file """
+		@param log_file
 
-		self.__debug('file=%s', logFile)
+		@return exitcode """
 
-		# err: file not found
-		if not os.path.isfile(logFile):
-			self.__debug('file="%s": not found"', logFile)
-			return 1
+		self.__config['log_file'] = log_file
 
-		# err: read file
-		try:
-			self.__file = open(logFile, 'ab')
-		except BaseException as emsg:
-			self.__debug('file="%s": err="%s"', (logFile, emsg))
-			return 1
+		return self.__file.file(log_file)
 
-		return 0
 
+	def console(self, console=False):
+		""" Console (stderr) output
 
-	def __setMask(self, mask='ALL'):
-		""" set mask """
+		@param console
 
-		maskPriority = {'ALL': 1, 'OFF': 5}
-		priority = maskPriority.get(mask)
-		if not priority:
-			return 1
+		@return exitcode """
 
-		for severityShort in self.__logniMaskSeverityShort:
-			self.__logniMaskSeverity[severityShort] = self.__setPriority(priority)
+		self.__config['console'] = console
+		self.__util.debug('console=%s', console)
 
-		self.__debug('mask.__setMask: self.__logniMaskSeverityShort=%s', self.__logniMaskSeverityShort)
-		self.__debug('mask.__setMask: self.__logniMaskSeverity=%s', self.__logniMaskSeverity)
+		return self.__console.console(console)
 
-		return 0
+	stderr = console
 
 
-	def mask(self, mask='ALL'):
-		""" mask """
+	def name(self, name):
+		""" Set name """
 
-		self.__debug('mask=%s', mask)
+		if not name:
+			return False
 
-		# default mask=ALL
-		if not mask:
-			mask = 'ALL'
-			self.__debug('mask=ALL')
+		self.__config['name'] = name
+		self.__util.debug('name=%s', name)
+		self.__name = name.upper()
 
+		return True
 
-		# log mask = ALL | OFF
-		if self.__setMask(mask) == 0:
-			return 0
 
-		# len is wrong
-		lenMask = len(mask)
-		if lenMask not in (2, 4, 6, 8, 10):
-			self.__debug('mask=%s: error len=%s', (mask, lenMask))
-			return 1
+	def __set_mask(self, mask='ALL'):
+		""" Set ALL | OFF / NOTSET mask
 
-		# set default MASK=0FF
-		self.__setMask('OFF')
+		@param mask
 
-		# set severity
-		for no in range(0, lenMask, 2):
+		@return exitcode """
 
-			_len = mask[no]
-			_priority = self.__setPriority(mask[no+1])
+		mask_priority = {'ALL': 1, 'OFF': 5, 'NOTSET': 5}
+		priority = mask_priority.get(mask)
+		if not priority:
+			return False
 
-			self.__logniMaskSeverity[_len] = _priority
-			self.__debug('mask: len=%s, priority=%s', (_len, _priority))
+		for severity_short in self.__logni_mask_severity_short:
+			self.__logni_mask_severity[severity_short] = self.__util.set_priority(priority)
 
-			del _len, _priority
+		self.__util.debug('__set_mask: self.__logni_mask_severity_short=%s',\
+			self.__logni_mask_severity_short)
+		self.__util.debug('__set_mask: self.__logni_mask_severity=%s',\
+			self.__logni_mask_severity)
 
-		self.__debug('mask: self.__logniMaskSeverity=%s', self.__logniMaskSeverity)
-		self.__config['mask'] = mask
+		return True
 
-		return 0
 
+	def mask(self, mask='ALL'):
+		""" Set mask
 
-	def console(self, console=0):
-		""" stderr / console """
+		@param mask
 
-		self.__config['console'] = console
-		self.__debug('console=%s', console)
+		@return exitcode """
 
-	stderr = console
+		self.__util.debug('mask=%s', mask)
 
+		# default mask=ALL
+		if not mask:
+			mask = 'ALL'
+			self.__util.debug('mask=ALL')
 
-	def maxLen(self, maxLen=MAX_LEN):
-		""" stderr / console """
 
-		self.__config['maxLen'] = maxLen
-		self.__debug('maxLen=%s', maxLen)
+		# log mask = ALL | OFF
+		if self.__set_mask(mask):
+			return True
 
+		# len is wrong
+		len_mask = len(mask)
+		if len_mask not in (2, 4, 6, 8, 10):
+			self.__util.debug('mask=%s: error len=%s', (mask, len_mask))
+			return False
 
-	def __setPriority(self, priority=4):
-		""" set priority """
+		# set default MASK=0FF
+		self.__set_mask('OFF')
 
-		self.__debug('__setPriority: priority=%s', priority)
+		# set severity
+		for pos_no in range(0, len_mask, 2):
 
-		if not priority:
-			return 1
+			_len = mask[pos_no]
+			_priority = self.__util.set_priority(mask[pos_no+1])
 
-		priority = abs(int(priority))
+			self.__logni_mask_severity[_len] = _priority
+			self.__util.debug('mask: len=%s, priority=%s', (_len, _priority))
 
-		# priority
-		if priority not in range(1, 5+1):
-			priority = 5
+			del _len, _priority
 
-		return priority
+		self.__util.debug('mask: self.__logni_mask_severity=%s', self.__logni_mask_severity)
+		self.__config['mask'] = mask
+
+		return True
 
 
 	# log use?
-	def __logUse(self, severity='', priority=1):
-		""" use log ? """
+	def __log_use(self, severity='', priority=1):
+		""" Use log?
+
+		@param severity
+		@param priority
 
-		self.__debug('log.__logUse: severity=%s, priority=%s', (severity, priority))
+		@return exitcode """
 
-		priority = self.__setPriority(priority)
+		self.__util.debug('__log_use: severity=%s, priority=%s', (severity, priority))
+
+		priority = self.__util.set_priority(priority)
 
 		# if mask=ALL
 		if self.__config['mask'] == 'ALL':
-			self.__debug('log.__logUse: severity=%s, msg priority=%s >= mask=ALL -> msg log is VISIBLE',\
+			self.__util.debug('__log_use: severity=%s, msg priority=%s ' + \
+				'>= mask=ALL -> msg log is VISIBLE',\
 				(severity, priority))
-			return 0
+			return True
 
-		if severity[0] not in self.__logniMaskSeverity:
-			self.__debug('log.__logUse: severity=%s not exist', severity)
-			return 1
+		if severity[0] not in self.__logni_mask_severity:
+			self.__util.debug('__log_use: severity=%s not exist', severity)
+			return False
 
 		# message hidden
-		_priority = self.__logniMaskSeverity[severity[0]]
+		_priority = self.__logni_mask_severity[severity[0]]
 		if priority < _priority:
-			self.__debug('log.__logUse: severity=%s, msg priority=%s < ' + \
+			self.__util.debug('__log_use: severity=%s, msg priority=%s < ' + \
 				'mask priority=%s -> msg log is HIDDEN',\
 				(severity, priority, _priority))
-			return 1
+			return False
 
 		# message visible
-		self.__debug('log.__logUse: severity=%s, msg priority=%s >= ' + \
+		self.__util.debug('__log_use: severity=%s, msg priority=%s >= ' + \
 			'mask priority=%s -> msg log is VISIBLE',\
 			(severity, priority, _priority))
 
-		return 0
-
-
-	# maxlen
-	def __logMaxLen(self, msg):
-		""" max length """
-
-		# maxlen
-		msgLen = len(msg)
-		if msgLen < self.__config['maxLen']:
-			return msg
+		return True
 
-		msg = msg[:self.__config['maxLen']] + ' ...'
-		self.__debug('log: msgLen=%s > global maxLen=%s -> because msg short',\
-			(msgLen, self.__config['maxLen']))
 
-		return msg
+	def log(self, severity, msg='', params=(), priority=1):
+		""" Log message
 
+		@param msg
+		@param params
+		@param severity
+		@param priority
 
-	def log(self, msg, params=(), **kw):
-		""" log message """
-
-		severity, priority = kw.iteritems().next()
-		self.__debug('log: severity=%s, priority=%s', (severity, priority))
-
-		return self.__log(msg, params, severity, priority)
-
-
-	def __log(self, msg, params=(), severity='DEBUG', priority=1):
-		""" log message """
+		@return struct """
 
 		# priority
-		priority = self.__setPriority(priority)
+		priority = self.__util.set_priority(priority)
 
 		# log use?
-		if self.__logUse(severity, priority) == 1:
-			return {'msg':msg, 'severity':severity, 'priority':priority, 'use':0}
+		if not self.__log_use(severity, priority):
+			return {'msg':msg, 'severity':severity, 'priority':priority, 'use':False}
 
 		try:
 			msg = msg % params
 		except BaseException as emsg:
 			msg = '!! %s %s <%s>' % (msg, params, emsg)
 
-		# todo: unicode test
+		# unicode test
 		# if isinstance(msg, types.UnicodeType):
 		# msg = msg.encode(self.__config['charset'], 'ignore')
 
 		# strip message
 		if self.__config['strip']:
 			msg = msg.replace('\n', ' ').strip()
 
 		# max len
-		msg = self.__logMaxLen(msg)
+		msg = self.__util.log_max_len(msg)
 
 		# stack
-		stackList = []
+		stack_list = []
 		offset = self.__config['stackOffset'] + 1
 		limit = self.__config['stackDepth'] + offset
 		for tes in traceback.extract_stack(limit=limit)[:-offset]:
-			stackList.append('%s:%s():%s' % (tes[0].split('/')[-1], tes[2], tes[1]))
+			stack_list.append('%s:%s():%s' % (tes[0].split('/')[-1], tes[2], tes[1]))
 
 		# log message
 		xrand = '%x' % random.SystemRandom().randint(1, 4294967295)
-		logMessage = "%s [%s] %s: %s [%s] {%s}\n" % \
+		log_message = "%s [%s] %s %s: %s [%s] {%s}" % \
 			(time.strftime(self.__config['timeFormat'], time.localtime()),\
 			os.getpid(),\
+			self.__name,\
 			'%s%s' % (severity[0], priority),\
 			msg, xrand,\
-			','.join(stackList))
+			','.join(stack_list))
 
 		# log to file / console
-		self.__log2File(logMessage)
-		self.__log2Console(logMessage)
+		self.__file.log(log_message)
+		self.__console.log(log_message, severity)
 
-		return {'msg':msg, 'severity':severity, 'priority':priority, 'use':1}
+		return {'msg':msg, 'severity':severity, 'priority':priority, 'use':True, 'hash':xrand}
 
+	# ---
 
-	def __log2File(self, logMessage):
-		""" log to file """
+	def traceback(self, exc, priority=1):
+		""" Traceback exception """
 
-		# file descriptor
-		if not self.__file:
-			return 0
+		try:
+			exc_type = exc.__class__
+			exc_tb = exc.__traceback__
+			exc_value = exc
+		except BaseException as base_err:
+			exc_type, exc_value, exc_tb = sys.exc_info()
+			del base_err
 
-		self.__file.write(logMessage)
+		tbt = traceback.TracebackException(exc_type, exc_value, exc_tb)
+		msg = '\\n'.join(tbt.format())
 
-		if self.__config['flush']:
-			self.__file.flush()
+		return self.log(self.cfg.SEVERITY_CRITICAL, msg, (), priority)
 
-		return 0
 
+	def critical(self, msg, params=(), priority=1):
+		""" Critical: critical / fatal message
 
-	def __log2Console(self, logMessage):
-		""" log to console / stderr """
+		@param msg
+		@param params
+		@param priority
 
-		# stderr / console
-		if not self.__config['console']:
-			return 0
+		@return struct """
 
-		sys.stderr.write(logMessage)
+		return self.log(self.cfg.SEVERITY_CRITICAL, msg, params, priority)
 
-		if self.__config['flush']:
-			sys.stderr.flush()
+	fatal = critical
 
-		return 0
 
+	def error(self, msg, params=(), priority=1):
+		""" Error: error message
 
-	# ---
+		@param msg
+		@param params
+		@param priority
 
-	def critical(self, msg, params=(), priority=4):
-		""" critical / fatal message """
+		@return struct """
 
-		return self.__log(msg, params, 'CRITICAL', priority)
+		return self.log(self.cfg.SEVERITY_ERROR, msg, params, priority)
 
-	fatal = critical
+	err = error
 
 
-	def error(self, msg, params=(), priority=4):
-		""" err / error message """
+	def warn(self, msg, params=(), priority=1):
+		""" Warn: warning message
 
-		return self.__log(msg, params, 'ERR', priority)
+		@param msg
+		@param params
+		@param priority
 
-	err = error
+		@return struct """
 
+		return self.log(self.cfg.SEVERITY_WARN, msg, params, priority)
 
-	def warn(self, msg, params=(), priority=4):
-		""" warn / warning message """
+	warning = warn
 
-		return self.__log(msg, params, 'WARN', priority)
 
-	warning = warn
+	def info(self, msg, params=(), priority=1):
+		""" Info: informational messages
 
+		@param msg
+		@param params
+		@param priority
 
-	def info(self, msg, params=(), priority=4):
-		""" info / informational message """
+		@return struct """
 
-		return self.__log(msg, params, 'INFO', priority)
+		return self.log(self.cfg.SEVERITY_INFO, msg, params, priority)
 
 	informational = info
 
 
-	def debug(self, msg, params=(), priority=4):
-		""" dbg / debug message """
+	def debug(self, msg, params=(), priority=1):
+		""" Debug: debug-level messages
+
+		@param msg
+		@param params
+		@param priority
 
-		return self.__log(msg, params, 'DEBUG', priority)
+		@return struct """
+
+		return self.log(self.cfg.SEVERITY_DEBUG, msg, params, priority)
 
 	dbg = debug
 
 
-	# ----
+	def emergency(self, msg, params=()):
+		""" Emergency: system is unusable
+
+		critical(msg, priority=4) """
+
+		return self.critical(msg, params, priority=4)
+
+
+	def alert(self, msg, params=()):
+		""" Alert: action must be taken immediately
+
+		error(msg, priority=3) """
+
+		return self.error(msg, params, priority=3)
+
+
+	def notice(self, msg, params=()):
+		""" Notice: normal but significant condition
+
+		info(msg, priority=1) """
+
+		return self.info(msg, params, priority=1)
+
 
-	def __debug(self, msg, val=()):
-		""" debug mode log """
+	def timer(self, func):
+		""" Timer: print the runtime of the decorated function """
 
-		if not self.__config['debugMode']:
-			return 1
+		@functools.wraps(func)
+		def log_wrapper_timer(*args, **kwargs):
+			""" log wrapper timer """
 
-		tf = time.strftime(self.__config['timeFormat'], time.localtime())
-		getpid = os.getpid()
-		msgVal = msg % val
+			start_time = time.time()
+			ret = func(*args, **kwargs)
+			run_time = int((time.time() - start_time) * 1000)
 
-		if val:
-			msgVal = msg % val
-			sys.stderr.write('%s [%s] DEBUG: %s\n' % (tf, getpid, msgVal))
-			return 0
+			self.info('func %s() in %sms', (func.__name__, run_time), priority=1)
 
-		sys.stderr.write('%s [%s] DEBUG: %s\n' % (tf, getpid, msg))
-		return 0
+			return ret
 
+		return log_wrapper_timer
 
 # run: python test/example/example.py
```

