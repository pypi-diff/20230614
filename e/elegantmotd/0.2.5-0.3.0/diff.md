# Comparing `tmp/elegantmotd-0.2.5.tar.gz` & `tmp/elegantmotd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegantmotd-0.2.5.tar", max compression
+gzip compressed data, was "elegantmotd-0.3.0.tar", max compression
```

## Comparing `elegantmotd-0.2.5.tar` & `elegantmotd-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1607 2023-05-02 17:18:20.672993 elegantmotd-0.2.5/README.md
--rw-r--r--   0        0        0      760 2023-05-02 18:26:28.872815 elegantmotd-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:59:59.267653 elegantmotd-0.2.5/src/elegantmotd/__init__.py
--rw-r--r--   0        0        0      200 2023-05-02 17:18:20.672993 elegantmotd-0.2.5/src/elegantmotd/constants.py
--rw-r--r--   0        0        0      819 2023-05-02 18:18:23.387757 elegantmotd-0.2.5/src/elegantmotd/cpu.py
--rw-r--r--   0        0        0     1036 2023-05-02 18:07:36.104712 elegantmotd-0.2.5/src/elegantmotd/disk.py
--rw-r--r--   0        0        0      294 2023-05-02 18:07:36.120712 elegantmotd-0.2.5/src/elegantmotd/load.py
--rw-r--r--   0        0        0      365 2023-05-02 18:07:36.104712 elegantmotd-0.2.5/src/elegantmotd/loggedinusers.py
--rw-r--r--   0        0        0     1429 2023-05-02 18:07:36.132712 elegantmotd-0.2.5/src/elegantmotd/memory.py
--rw-r--r--   0        0        0     2126 2023-05-02 18:14:12.401738 elegantmotd-0.2.5/src/elegantmotd/motd.py
--rw-r--r--   0        0        0      500 2023-05-02 18:07:36.116712 elegantmotd-0.2.5/src/elegantmotd/network.py
--rw-r--r--   0        0        0      279 2023-05-02 18:18:23.387757 elegantmotd-0.2.5/src/elegantmotd/process.py
--rw-r--r--   0        0        0      286 2023-05-02 18:19:32.351205 elegantmotd-0.2.5/src/elegantmotd/sysinfo.py
--rw-r--r--   0        0        0     1414 2023-05-02 18:07:36.112712 elegantmotd-0.2.5/src/elegantmotd/temperature.py
--rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 elegantmotd-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1865 2023-06-13 22:17:42.539527 elegantmotd-0.3.0/README.md
+-rw-r--r--   0        0        0      782 2023-06-13 22:12:09.934290 elegantmotd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/__init__.py
+-rw-r--r--   0        0        0      200 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/constants.py
+-rw-r--r--   0        0        0      819 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/cpu.py
+-rw-r--r--   0        0        0     1036 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/disk.py
+-rw-r--r--   0        0        0      294 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/load.py
+-rw-r--r--   0        0        0      365 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/loggedinusers.py
+-rw-r--r--   0        0        0     1429 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/memory.py
+-rw-r--r--   0        0        0     2953 2023-06-13 22:14:46.492987 elegantmotd-0.3.0/src/elegantmotd/motd.py
+-rw-r--r--   0        0        0      500 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/network.py
+-rw-r--r--   0        0        0      279 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/process.py
+-rw-r--r--   0        0        0      286 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/sysinfo.py
+-rw-r--r--   0        0        0     1414 2023-06-13 21:39:48.262588 elegantmotd-0.3.0/src/elegantmotd/temperature.py
+-rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 elegantmotd-0.3.0/PKG-INFO
```

### Comparing `elegantmotd-0.2.5/README.md` & `elegantmotd-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,106 @@
+Metadata-Version: 2.1
+Name: elegantmotd
+Version: 0.3.0
+Summary: A visually appealing and informative Message of the Day (MOTD) generator for Linux systems.
+Home-page: https://github.com/emerick-biron/elegantmotd
+License: MIT
+Keywords: motd,system,information,console,dashboard
+Author: Emerick Biron
+Author-email: emerick.biron@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: art (>=5.9,<6.0)
+Requires-Dist: netifaces (>=0.11.0,<0.12.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Project-URL: Repository, https://github.com/emerick-biron/elegantmotd.git
+Description-Content-Type: text/markdown
+
 # ElegantMOTD
 
 ElegantMOTD is a Python-based Message of the Day (MOTD) generator for displaying system information in a visually
 appealing and informative manner. It works on Linux systems and provides details such as system load, disk usage, memory
 usage, swap usage, temperature, network interfaces, CPU usage, and more.
 
 ## Features
 
 - Rich, colorful text-based output.
 - Displays various system information.
 - Customizable display options.
 - Easy to use and integrate into your system.
 
 ## Installation
+
 - Clone this repository:
+
 ```bash
 git clone https://github.com/yourusername/elegantmotd.git
 cd elegantmotd
 ```
+
 - Create a virtual environment and activate it:
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 ```
 
 - Install the required dependencies:
+
 ```bash
 poetry build 
 ```
 
 ## Usage
 
 To display the Message of the Day, run the following command:
 
 ```bash
 elegantmotd
 ```
 
+## Live Updates
+
+If you want to enable live updates of the system information, you can use the `--watch`/`-w` option:
+
+```bash
+elegantmotd --watch
+```
+
+With the `--watch` option, the MOTD will be continuously updated with the latest system information.
+
 ## Output
 
 ![Output](resources/output.png)
 
 ## Customization
 
-You can customize the output by modifying the `motd.py` file and adding or removing system information modules as per your preference. The available modules are:
+You can customize the output by modifying the `motd.py` file and adding or removing system information modules as per
+your preference. The available modules are:
 
 - Load
 - Disk
 - Memory
 - Temperature
 - Process
 - LoggedInUsers
 - Network
 - CPU
 
-To add or remove a module, simply add or remove the corresponding import statement and the respective class instance from the `sysinfos` list in the `display()` function.
+To add or remove a module, simply add or remove the corresponding import statement and the respective class instance
+from the `sysinfos` list in the `display()` function.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
+
```

### Comparing `elegantmotd-0.2.5/pyproject.toml` & `elegantmotd-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elegantmotd"
-version = "0.2.5"
+version = "0.3.0"
 authors = ["Emerick Biron <emerick.biron@gmail.com>"]
 readme = "README.md"
 description = "A visually appealing and informative Message of the Day (MOTD) generator for Linux systems."
 homepage = "https://github.com/emerick-biron/elegantmotd"
 repository = "https://github.com/emerick-biron/elegantmotd.git"
 keywords = ["motd", "system", "information", "console", "dashboard"]
 license = "MIT"
@@ -12,14 +12,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "^13.3.4"
 psutil = "^5.9.5"
 netifaces = "^0.11.0"
 art = "^5.9"
+rich-click = "^1.6.1"
 
 [tool.poetry.scripts]
 elegantmotd="elegantmotd.motd:display"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `elegantmotd-0.2.5/src/elegantmotd/cpu.py` & `elegantmotd-0.3.0/src/elegantmotd/cpu.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.5/src/elegantmotd/disk.py` & `elegantmotd-0.3.0/src/elegantmotd/disk.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.5/src/elegantmotd/memory.py` & `elegantmotd-0.3.0/src/elegantmotd/memory.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.5/src/elegantmotd/motd.py` & `elegantmotd-0.3.0/src/elegantmotd/motd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 import platform
 import re
+import time
 from datetime import datetime, timezone
 
+import rich_click as click
 from art import text2art
 from rich.console import Console
+from rich.live import Live
+from rich.padding import Padding
 from rich.style import Style
 from rich.table import Table
 
 from .cpu import CPU
 from .disk import Disk
 from .load import Load
 from .loggedinusers import LoggedInUsers
@@ -36,37 +40,52 @@
     return platform.release()
 
 
 def get_architecture():
     return platform.machine()
 
 
-def display():
-    distro, codename = get_distro_info()
-    kernel = get_kernel_info()
-    architecture = get_architecture()
-
+@click.command(help="Display system information in a visually appealing manner.")
+@click.option("-w", "--watch", is_flag=True, show_default=False, default=False,
+              help="Enable live updates of the system information.")
+def display(watch: bool) -> None:
     console = Console()
-    console.print(f"💻 [blue bold]{distro} {codename} LTS (GNU/Linux {kernel} {architecture}) [/]💻")
-    console.print(f"[orange1 bold]{text2art(os.getlogin(), font='small')}[/]", end="")
+    try:
+        distro, codename = get_distro_info()
+        kernel = get_kernel_info()
+        architecture = get_architecture()
+
+        if watch:
+            console.clear()
+        console.print(f"💻 [blue bold]{distro} {codename} LTS (GNU/Linux {kernel} {architecture}) [/]💻")
+        console.print(f"[orange1 bold]{text2art(os.getlogin(), font='small')}[/]", end="")
+        padding = Padding(generate_table(), (0, 0, 1, 0))
+        if watch:
+            with Live(padding, refresh_per_second=1) as live:
+                while True:
+                    time.sleep(1)
+                    padding.renderable = generate_table()
+                    live.update(padding)
+        else:
+            console.print(padding)
+    except KeyboardInterrupt:
+        console.clear()
+
+
+def generate_table() -> Table:
     local_time = datetime.now(timezone.utc).astimezone()
     utc_offset = round(local_time.utcoffset().total_seconds() / 3600)
     table = Table(
         show_header=False,
         box=None,
         title_justify="left",
         title=f"  System information as of {local_time.strftime('%a. %d %B %Y %H:%M:%S')} UTC+{utc_offset}\n",
         title_style=Style(color="white", italic=False, bold=True, ),
         expand=True,
         leading=1,
         padding=(0, 2)
     )
-
     table.add_column("Info", style="bold CYAN")
     table.add_column("Value", style="bold WHITE")
-
     sysinfos = [Load(), Disk(), Memory(), Temperature(), Process(), LoggedInUsers(), Network(), CPU()]
-
     [table.add_row(f"{info}:", sysinfo.infos[info]) for sysinfo in sysinfos for info in sysinfo.infos]
-
-    console.print(table)
-    console.print()
+    return table
```

### Comparing `elegantmotd-0.2.5/src/elegantmotd/temperature.py` & `elegantmotd-0.3.0/src/elegantmotd/temperature.py`

 * *Files identical despite different names*

