# Comparing `tmp/mighty_logger-0.5.1.tar.gz` & `tmp/mighty_logger-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.5.1.tar", last modified: Thu Jun  8 16:17:12 2023, max compression
+gzip compressed data, was "mighty_logger-0.6.0.tar", last modified: Wed Jun 14 15:04:27 2023, max compression
```

## Comparing `mighty_logger-0.5.1.tar` & `mighty_logger-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.349214 mighty_logger-0.5.1/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    10255 2023-06-08 16:17:12.350214 mighty_logger-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     9290 2023-06-08 12:57:30.000000 mighty_logger-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.268080 mighty_logger-0.5.1/mighty_logger/
--rw-rw-rw-   0        0        0      823 2023-06-08 16:11:27.000000 mighty_logger-0.5.1/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.304869 mighty_logger-0.5.1/mighty_logger/basic/
--rw-rw-rw-   0        0        0      857 2023-04-11 08:43:49.000000 mighty_logger-0.5.1/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     5454 2023-06-06 13:48:02.000000 mighty_logger-0.5.1/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1325 2023-04-12 11:19:28.000000 mighty_logger-0.5.1/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.5.1/mighty_logger/basic/patterns.py
--rw-rw-rw-   0        0        0     3125 2023-06-08 10:41:07.000000 mighty_logger-0.5.1/mighty_logger/basic/text_buffer_type.py
--rw-rw-rw-   0        0        0    47848 2023-06-08 10:41:07.000000 mighty_logger-0.5.1/mighty_logger/powerful_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.320295 mighty_logger-0.5.1/mighty_logger/src/
--rw-rw-rw-   0        0        0      935 2023-06-07 17:37:14.000000 mighty_logger-0.5.1/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     4570 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     8657 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/src/color_picker.py
--rw-rw-rw-   0        0        0      728 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/src/log_environment.py
--rw-rw-rw-   0        0        0     5640 2023-06-08 10:15:33.000000 mighty_logger-0.5.1/mighty_logger/src/status_variables.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.325296 mighty_logger-0.5.1/mighty_logger/text/
--rw-rw-rw-   0        0        0      789 2023-06-08 15:16:03.000000 mighty_logger-0.5.1/mighty_logger/text/__init__.py
--rw-rw-rw-   0        0        0     2373 2023-06-08 15:16:03.000000 mighty_logger-0.5.1/mighty_logger/text/icon_set.py
--rw-rw-rw-   0        0        0     4993 2023-06-08 14:51:35.000000 mighty_logger-0.5.1/mighty_logger/text/text_buffer.py
--rw-rw-rw-   0        0        0     4822 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/text/~animation.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.272078 mighty_logger-0.5.1/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0    10255 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      757 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 16:17:12.351217 mighty_logger-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2796 2023-06-08 16:11:27.000000 mighty_logger-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.348215 mighty_logger-0.5.1/test/
--rw-rw-rw-   0        0        0     1239 2023-06-08 14:24:28.000000 mighty_logger-0.5.1/test/test_console.py
--rw-rw-rw-   0        0        0     1184 2023-06-08 15:16:03.000000 mighty_logger-0.5.1/test/test_html.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.340353 mighty_logger-0.6.0/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0    10318 2023-06-14 15:04:27.340353 mighty_logger-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9350 2023-06-12 16:10:21.000000 mighty_logger-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.249337 mighty_logger-0.6.0/mighty_logger/
+-rw-rw-rw-   0        0        0      823 2023-06-12 12:55:27.000000 mighty_logger-0.6.0/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.300349 mighty_logger-0.6.0/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      857 2023-04-11 08:43:49.000000 mighty_logger-0.6.0/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     5371 2023-06-12 12:55:27.000000 mighty_logger-0.6.0/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1325 2023-04-12 11:19:28.000000 mighty_logger-0.6.0/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.6.0/mighty_logger/basic/patterns.py
+-rw-rw-rw-   0        0        0     4009 2023-06-12 12:55:27.000000 mighty_logger-0.6.0/mighty_logger/basic/text_buffer_type.py
+-rw-rw-rw-   0        0        0    70934 2023-06-12 14:16:59.000000 mighty_logger-0.6.0/mighty_logger/powerful_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.314351 mighty_logger-0.6.0/mighty_logger/src/
+-rw-rw-rw-   0        0        0      943 2023-06-11 13:34:59.000000 mighty_logger-0.6.0/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/color_picker.py
+-rw-rw-rw-   0        0        0     1293 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/log_enums.py
+-rw-rw-rw-   0        0        0     5647 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/status_variables.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.335354 mighty_logger-0.6.0/mighty_logger/text/
+-rw-rw-rw-   0        0        0      853 2023-06-10 14:12:03.000000 mighty_logger-0.6.0/mighty_logger/text/__init__.py
+-rw-rw-rw-   0        0        0     5947 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/text/animation.py
+-rw-rw-rw-   0        0        0     2872 2023-06-12 13:38:48.000000 mighty_logger-0.6.0/mighty_logger/text/icon_set.py
+-rw-rw-rw-   0        0        0     5806 2023-06-12 16:08:04.000000 mighty_logger-0.6.0/mighty_logger/text/text_buffer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.255339 mighty_logger-0.6.0/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0    10318 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 15:04:27.342354 mighty_logger-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     2796 2023-06-14 14:55:46.000000 mighty_logger-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.338353 mighty_logger-0.6.0/test/
+-rw-rw-rw-   0        0        0     2067 2023-06-14 12:00:28.000000 mighty_logger-0.6.0/test/test_console.py
+-rw-rw-rw-   0        0        0     2099 2023-06-14 12:02:42.000000 mighty_logger-0.6.0/test/test_html.py
```

### Comparing `mighty_logger-0.5.1/LICENSE` & `mighty_logger-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.1/PKG-INFO` & `mighty_logger-0.6.0/mighty_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mighty_logger
-Version: 0.5.1
+Name: mighty-logger
+Version: 0.6.0
 Summary: Powerful functional logger with support for qt programming
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
@@ -97,20 +97,21 @@
 
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
-- [ ] v0.6.0 - Progress update (added start of some log entries in threads (process))
+- [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [ ] v0.6.1 - Animation update (added animations in processes)
 - [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
 - [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
 - [ ] v0.7.2 - Search update (added search by log entry types)
 - [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
+- [ ] v0.8.0 - ? (???) in short, add export to csv
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
@@ -154,16 +155,18 @@
 if __name__ == "__main__":
     logger = Logger(program_name="Test", console_width=115)
     logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
 ```
 
 The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
 
-> <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span><br>
-> <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span><br>
+<pre>
+<span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
+<span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
+</pre>
 
 See the APPLYING.md file for more details.
 
 - [Content](#content)
 
 ## *Additional functionality*
```

### Comparing `mighty_logger-0.5.1/README.md` & `mighty_logger-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,21 @@
 
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
-- [ ] v0.6.0 - Progress update (added start of some log entries in threads (process))
+- [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [ ] v0.6.1 - Animation update (added animations in processes)
 - [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
 - [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
 - [ ] v0.7.2 - Search update (added search by log entry types)
 - [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
+- [ ] v0.8.0 - ? (???) in short, add export to csv
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
@@ -135,16 +136,18 @@
 if __name__ == "__main__":
     logger = Logger(program_name="Test", console_width=115)
     logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
 ```
 
 The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
 
-> <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span><br>
-> <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span><br>
+<pre>
+<span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
+<span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
+</pre>
 
 See the APPLYING.md file for more details.
 
 - [Content](#content)
 
 ## *Additional functionality*
```

### Comparing `mighty_logger-0.5.1/mighty_logger/__init__.py` & `mighty_logger-0.6.0/mighty_logger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .powerful_logger import Logger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.5.1/mighty_logger/basic/__init__.py` & `mighty_logger-0.6.0/mighty_logger/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.1/mighty_logger/basic/basic_logger.py` & `mighty_logger-0.6.0/mighty_logger/basic/basic_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 limitations under the License.
 """
 
 import datetime, platform, os, random
 
 from mighty_logger.basic.patterns import Singleton
 from mighty_logger.src.ansi_format import GetAnsiFormat
-from mighty_logger.src.log_environment import LogEnvironments
+from mighty_logger.src.log_enums import LogEnvironments
 
 class BasicLogger(Singleton):
 	def __init__(
-			self,
-			program_name: str,
+		self,
+		program_name: str,
 	) -> None:
 		self._program_name = program_name
 		self._settings: dict = {}
 		self._ID = random.randint(1000000, 9999999)
 
 	def _initialized_data(
-			self,
-			colors: list[str, str],
-			env: str
+		self,
+		colors: list[str, str],
+		env: str
 	) -> str:
 		"""
 		A method that assemble an entry of system initialized data.
 
 		:param colors: Color string list of initialized data
 		:return: a string with initialized data
 		"""
@@ -62,23 +62,23 @@
 					f":{platform.version()}" +
 					":{}:{}".format(*platform.architecture()) +
 					f":{platform.machine()}" +
 					f"{GetAnsiFormat('reset/on')}"
 			)
 
 	def _assemble_entry(
-			self,
-			colors: list[str, str, str, str, str, str],
-			animation: list,
-			icon: str,
-			status_message_text: str,
-			message_type: str,
-			message_text: str,
-			env: str,
-			local_settings: dict
+		self,
+		colors: list[str, str, str, str, str, str],
+		animation: str,
+		icon: str,
+		status_message_text: str,
+		message_type: str,
+		message_text: str,
+		env: str,
+		local_settings: dict
 	) -> str:
 		"""
 		A method that assemble an entry into a string and returns it.
 
 		:param colors: 6 colors that the method uses to assemble the string
 		:param animation: Animation of entry
 		:param icon: Type icon
@@ -98,32 +98,32 @@
 		status_type_entry = local_settings['status_type_local_entry'] if 'status_type_local_entry' in local_settings else self._settings['status_type_global_entry']
 		message_entry = local_settings['message_local_entry'] if 'message_local_entry' in local_settings else self._settings['message_global_entry']
 		if env == LogEnvironments.HTML:
 			return (
 					(f"<b>" if bold else "") +
 					(f"<i>" if italic else "") +
 					f"<span style='background-color: #{colors[5]};'>" +
-					f"<span style='color: #{colors[4]};'>-?entry> {animation[0]}</span>" +  # todo Must add animation
+					f"<span style='color: #{colors[4]};'>-?entry> {animation} </span>" +
 					(f"<span style='color: #{colors[0]};'>*{datetime.datetime.now()} </span>" if time_entry else "") +
-					f"<div style='display: inline-block; white-space: pre; tab-size: 4'>{icon}&#9;</div>" +
+					f"<div style='display: inline-block; white-space: pre; tab-size: 4'>{icon} </div>" +
 					(f"<span style='color: #{colors[1]};'>#STATUS: </span>" if status_entry else "") +
 					(f"<span style='color: #{colors[2]};'>{status_message_text} </span>" if status_message_entry else "") +
 					(f"<span style='color: #{colors[3]};'>{message_type} - </span>" if status_type_entry else "") +
 					(f"<span style='color: #{colors[4]};'>{message_text}</span></span>" if message_entry else "") +
 					(f"</i>" if italic else "") +
 					(f"</b>" if bold else "")
 			)
 		else:
 			return (
 					(f"{GetAnsiFormat('bold/on')}" if bold else "") +
 					(f"{GetAnsiFormat('italic/on')}" if italic else "") +
 					(f"{GetAnsiFormat('invert/on')}" if invert else "") +
 					f"{colors[5]}" +
-					f"{colors[4]}-?entry> {animation[0]}" +  # todo Must add animation
+					f"{colors[4]}-?entry> {animation} " +
 					(f"{colors[0]}*{datetime.datetime.now()} " if time_entry else "") +
-					f"{icon}\t" +
+					f"{icon} " +
 					(f"{colors[1]}#STATUS: " if status_entry else "") +
 					(f"{colors[2]}{status_message_text} " if status_message_entry else "") +
 					(f"{colors[3]}{message_type} - " if status_type_entry else "") +
 					(f"{colors[4]}{message_text}" if message_entry else "") +
 					f"{GetAnsiFormat('reset/on')}"
 			)
```

### Comparing `mighty_logger-0.5.1/mighty_logger/basic/exceptions.py` & `mighty_logger-0.6.0/mighty_logger/basic/exceptions.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.1/mighty_logger/basic/patterns.py` & `mighty_logger-0.6.0/mighty_logger/basic/patterns.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.1/mighty_logger/basic/text_buffer_type.py` & `mighty_logger-0.6.0/mighty_logger/basic/text_buffer_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -73,14 +73,32 @@
 
 		:param number_string: Position (number) of the string to be replaced (added)
 		:param message: A string that will replace the previous one by position
 		"""
 		raise NotImplementedError("Method replace() is not implemented in the base class.")
 
 	@abstractmethod
+	def pop(self, number_string: int = -1) -> str:
+		"""
+		Removes and returns the specified string from the buffer.
+
+		:param number_string: The string to be removed from the buffer
+		"""
+		raise NotImplementedError("Method remove() is not implemented in the base class.")
+
+	@abstractmethod
+	def remove(self, number_string: int = -1) -> None:
+		"""
+		Deletes without returning the specified string from the buffer.
+
+		:param number_string: The string to be removed from the buffer
+		"""
+		raise NotImplementedError("Method remove() is not implemented in the base class.")
+
+	@abstractmethod
 	def save(self, name_file: str = "buffer", clean: bool = True) -> None:
 		"""
 		Saves the text of the buffer to a file.
 
 		:param name_file: The name of the file where the buffer will be saved
 		:param clean: Saving should be done in Plain text?
 		"""
@@ -89,8 +107,16 @@
 	@abstractmethod
 	def update_console(self) -> None:
 		"""
 		Refreshes the console, erasing output text and outputting an updated buffer.
 		"""
 		raise NotImplementedError("Method update_console() is not implemented in the base class.")
 
+	@abstractmethod
+	def update_entry(self) -> None:
+		"""
+		Rewrites the last line of output after updating the last line of the buffer.
+		Used (mostly) by the Progress bar (that is Progress string).
+		"""
+		raise NotImplementedError("Method update_entry() is not implemented in the base class.")
+
 	# todo v0.7.0 abstractmethod remove(), clear(), -open_save() or load()-
```

### Comparing `mighty_logger-0.5.1/mighty_logger/src/__init__.py` & `mighty_logger-0.6.0/mighty_logger/src/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 	AnsiColor,\
 	Dec2Hex,\
 	Dec2Ansi,\
 	Hex2Dec,\
 	Hex2Ansi,\
 	Ansi2Dec,\
 	Ansi2Hex
-from .log_environment import LogEnvironments
+from .log_enums import LogEnvironments, TypesEntries
 from .status_variables import StatusMessagePatterns
```

### Comparing `mighty_logger-0.5.1/mighty_logger/src/ansi_format.py` & `mighty_logger-0.6.0/mighty_logger/src/ansi_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module with implementation of ANSI escape codes.
+A module with implementation of ANSI escape codes.
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mighty_logger-0.5.1/mighty_logger/src/color_picker.py` & `mighty_logger-0.6.0/mighty_logger/src/color_picker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module with implementation of colors and their formatter functions.
+A module with implementation of colors and their formatter functions.
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mighty_logger-0.5.1/mighty_logger/src/log_environment.py` & `mighty_logger-0.6.0/mighty_logger/text/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-A module with a list of environment options in which the modules work.
+A package with the implementation of text formats.
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -12,10 +12,10 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-class LogEnvironments:
-	CONSOLE = 'console',
-	HTML = 'html'
+from .animation import IndefiniteAnimations, DefiniteAnimations
+from .icon_set import IconSetType, EmptyIconSet, IconSet1, IconSet2, IconSet3, IconSet4
+from .text_buffer import BasicTextBuffer, TextBuffer
```

### Comparing `mighty_logger-0.5.1/mighty_logger/src/status_variables.py` & `mighty_logger-0.6.0/mighty_logger/src/status_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module with implementation of entry status messages.
+A module with implementation of entry status messages.
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -17,15 +17,15 @@
 """
 
 class StatusMessageType:
 	"""
 	Wrapper class for status message.
 	"""
 	def __init__(self, message: str):
-		self.__current_status_message = message
+		self.__current_status_message: str = message
 
 	@property
 	def current_status_message(self) -> str:
 		return self.__current_status_message
 
 class StatusMessagePatterns:
 	"""
```

### Comparing `mighty_logger-0.5.1/mighty_logger/text/icon_set.py` & `mighty_logger-0.6.0/mighty_logger/text/icon_set.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,20 @@
 	user = ''
 	message = ''
 	info = ''
 	notice = ''
 	warning = ''
 	error = ''
 	critical = ''
+	resolved = ''
+	unresolved = ''
+	initiation = ''
 	process = ''
+	achievement = ''
+	milestone = ''
 	success = ''
 	fail = ''
 
 class EmptyIconSet(IconSetType):
 	...
 
 class IconSet1(IconSetType):
@@ -53,15 +58,20 @@
 	user = '👤'
 	message = '💬'
 	info = 'ℹ️'
 	notice = '📌'
 	warning = '⚠️'
 	error = '❌'
 	critical = '🔥'
+	resolved = '✅'
+	unresolved = '❎'
+	initiation = '🚀'
 	process = '⏳'
+	achievement = '🏆'
+	milestone = '🔖'
 	success = '✔️'
 	fail = '❌'
 
 class IconSet2(IconSetType):
 	"""
 	Second icon set.
 	"""
@@ -74,15 +84,20 @@
 	user = '👥'
 	message = '📝'
 	info = '🔍'
 	notice = '📎'
 	warning = '⚡️'
 	error = '🚫'
 	critical = '🚨'
+	resolved = '❗'
+	unresolved = '❓'
+	initiation = '🚀'
 	process = '🔄'
+	achievement = '🏆'
+	milestone = '🔖'
 	success = '🎉'
 	fail = '🚫'
 
 class IconSet3(IconSetType):
 	"""
 	Third icon set.
 	"""
@@ -95,15 +110,20 @@
 	user = '🙋‍♂️'
 	message = '🗒️'
 	info = '📌'
 	notice = '🔖'
 	warning = '⛔️'
 	error = '💔'
 	critical = '⛔️'
+	resolved = '🟦'
+	unresolved = '🟥'
+	initiation = '🔥'
 	process = '⚙️'
+	achievement = '🌟'
+	milestone = '🎯'
 	success = '👍'
 	fail = '👎'
 
 class IconSet4(IconSetType):
 	"""
 	Fourth icon set.
 	"""
@@ -113,13 +133,18 @@
 	event = '🚨'
 	audit = '🔐'
 	metrics = '📄'
 	user = '🙋‍♀️'
 	message = '📨'
 	info = '🔔'
 	notice = '🚩'
-	warning = '🔺'
-	error = '🔴'
+	warning = '⚠️'
+	error = '🔺'
 	critical = '🚒'
+	resolved = '🟢'
+	unresolved = '🔴'
+	initiation = '🔧'
 	process = '🕰️'
+	achievement = '🎖️'
+	milestone = '🗺️'
 	success = '✅'
 	fail = '❎'
```

### Comparing `mighty_logger-0.5.1/mighty_logger/text/text_buffer.py` & `mighty_logger-0.6.0/mighty_logger/text/text_buffer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module with implementation of text buffers.
+A module with implementation of text buffers.
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -47,24 +47,38 @@
 	def replace(self, number_string: int, message: str) -> None:
 		if number_string < len(self._text_buffer):
 			self._text_buffer[number_string] = f"{message}"
 		else:
 			self._text_buffer.extend([""] * (number_string - len(self._text_buffer)))
 			self.append(message)
 
+	def pop(self, number_string: int = -1) -> str:
+		last = self._text_buffer.pop(number_string)
+		return last
+
+	def remove(self, number_string: int = -1) -> None:
+		self._text_buffer.pop(number_string)
+
 	def save(self, name_file: str = "buffer", clean: bool = True) -> None:
 		with open(name_file, "w", encoding="utf-8") as text_buffer_file:
 			if clean:
-				text_buffer_file.write(self._text_buffer[0] + '\n' + '\n<br>'.join(self._text_buffer[1:]))
+				text_buffer_file.write(
+					'<pre>' + self._text_buffer[0] + '\n' + '\n'.join(self._text_buffer[1:]) + '</pre>'
+				)
 			else:
-				text_buffer_file.write(self._text_buffer[0] + '\n' + '\n'.join(self._text_buffer[1:]))
+				text_buffer_file.write(
+					'<pre>' + self._text_buffer[0] + ''.join(self._text_buffer[1:]) + '</pre>'
+				)
 
 	def update_console(self) -> None:
 		super().update_console()
 
+	def update_entry(self) -> None:
+		super().update_console()
+
 class TextBuffer(Singleton, TextBufferType):
 	"""
 	A class with an advanced implementation of the console text buffer. It is not necessary to use it
 	only in the console, but almost all methods are reimplemented for more complex algorithms, taking
 	into account the width of the console (number of characters per line) and use ANSI escape codes
 	that are only found in the console.
 	"""
@@ -102,14 +116,23 @@
 			self.append(message)
 		else:
 			old_excess_console_strings = len(re.sub(r"\033\[.*?m", "", self._text_buffer[number_string])) // self.width
 			new_excess_console_strings = len(re.sub(r"\033\[.*?m", "", message)) // self.width
 			self._buffer_size += new_excess_console_strings - old_excess_console_strings
 			self._text_buffer[number_string] = f"{message}"
 
+	def pop(self, number_string: int = -1) -> str:
+		self._buffer_size -= 1
+		last = self._text_buffer.pop(number_string)
+		return last
+
+	def remove(self, number_string: int = -1) -> None:
+		self._buffer_size -= 1
+		self._text_buffer.pop(number_string)
+
 	def save(self, name_file: str = "buffer", clean: bool = True) -> None:
 		with open(name_file, "w", encoding="utf-8") as text_buffer_file:
 			if clean:
 				for item in self._text_buffer:
 					text_buffer_file.write("{}\n".format(re.sub(r"\033\[.*?m", "", item)))
 			else:
 				text_buffer_file.write('\n'.join(self._text_buffer))
@@ -119,7 +142,13 @@
 		if self._cursor_string == 0:
 			sys.stdout.write(f'\r\033[K')
 		else:
 			sys.stdout.write(f'\033[{self._cursor_string}A\r\033[J')
 		sys.stdout.write('\n'.join(self._text_buffer))
 		sys.stdout.flush()  # Clearing the output buffer so that the changes are displayed immediately
 		self._cursor_string = self._buffer_size - 1
+
+	def update_entry(self) -> None:
+		# todo Translate to thread in a future update
+		sys.stdout.write(f'\r')
+		sys.stdout.write(self._text_buffer[-1])
+		sys.stdout.flush()  # Clearing the output buffer so that the changes are displayed immediately
```

### Comparing `mighty_logger-0.5.1/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mighty-logger
-Version: 0.5.1
+Name: mighty_logger
+Version: 0.6.0
 Summary: Powerful functional logger with support for qt programming
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
@@ -97,20 +97,21 @@
 
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
-- [ ] v0.6.0 - Progress update (added start of some log entries in threads (process))
+- [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [ ] v0.6.1 - Animation update (added animations in processes)
 - [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
 - [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
 - [ ] v0.7.2 - Search update (added search by log entry types)
 - [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
+- [ ] v0.8.0 - ? (???) in short, add export to csv
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
@@ -154,16 +155,18 @@
 if __name__ == "__main__":
     logger = Logger(program_name="Test", console_width=115)
     logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
 ```
 
 The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
 
-> <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span><br>
-> <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span><br>
+<pre>
+<span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
+<span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
+</pre>
 
 See the APPLYING.md file for more details.
 
 - [Content](#content)
 
 ## *Additional functionality*
```

### Comparing `mighty_logger-0.5.1/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-0.6.0/mighty_logger.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 mighty_logger/basic/basic_logger.py
 mighty_logger/basic/exceptions.py
 mighty_logger/basic/patterns.py
 mighty_logger/basic/text_buffer_type.py
 mighty_logger/src/__init__.py
 mighty_logger/src/ansi_format.py
 mighty_logger/src/color_picker.py
-mighty_logger/src/log_environment.py
+mighty_logger/src/log_enums.py
 mighty_logger/src/status_variables.py
 mighty_logger/text/__init__.py
+mighty_logger/text/animation.py
 mighty_logger/text/icon_set.py
 mighty_logger/text/text_buffer.py
-mighty_logger/text/~animation.py
 test/test_console.py
 test/test_html.py
```

### Comparing `mighty_logger-0.5.1/setup.py` & `mighty_logger-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mighty_logger",
-    version="0.5.1",
+    version="0.6.0",
 
     author="Kalynovsky 'Nakamura Akira' Valentin",
     author_email="nakama3942@gmail.com",
 
     description="Powerful functional logger with support for qt programming",
     long_description=readme,
     long_description_content_type="text/markdown",
```

