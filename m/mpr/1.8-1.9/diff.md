# Comparing `tmp/mpr-1.8.tar.gz` & `tmp/mpr-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpr-1.8.tar", last modified: Wed Aug 31 05:06:31 2022, max compression
+gzip compressed data, was "mpr-1.9.tar", last modified: Mon Oct 10 05:54:18 2022, max compression
```

## Comparing `mpr-1.8.tar` & `mpr-1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-08-31 05:06:31.483013 mpr-1.8/
--rw-r--r--   0 mark      (1000) mark      (1000)    22012 2022-08-31 05:06:31.483013 mpr-1.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    21595 2022-08-31 04:46:39.000000 mpr-1.8/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-08-31 05:06:31.483013 mpr-1.8/mpr.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    22012 2022-08-31 05:06:31.000000 mpr-1.8/mpr.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      163 2022-08-31 05:06:31.000000 mpr-1.8/mpr.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-08-31 05:06:31.000000 mpr-1.8/mpr.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       33 2022-08-31 05:06:31.000000 mpr-1.8/mpr.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        4 2022-08-31 05:06:31.000000 mpr-1.8/mpr.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)    15258 2022-08-31 04:57:18.000000 mpr-1.8/mpr.py
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2022-08-31 05:06:31.483013 mpr-1.8/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)      956 2022-08-31 05:05:25.000000 mpr-1.8/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-10 05:54:18.630303 mpr-1.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)    22281 2022-10-10 05:54:18.630303 mpr-1.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    21864 2022-10-10 05:47:05.000000 mpr-1.9/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-10 05:54:18.630303 mpr-1.9/mpr.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    22281 2022-10-10 05:54:18.000000 mpr-1.9/mpr.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      163 2022-10-10 05:54:18.000000 mpr-1.9/mpr.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-10-10 05:54:18.000000 mpr-1.9/mpr.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       33 2022-10-10 05:54:18.000000 mpr-1.9/mpr.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        4 2022-10-10 05:54:18.000000 mpr-1.9/mpr.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)    16565 2022-10-10 05:50:11.000000 mpr-1.9/mpr.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2022-10-10 05:54:18.630303 mpr-1.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)      956 2022-10-10 05:52:54.000000 mpr-1.9/setup.py
```

### Comparing `mpr-1.8/PKG-INFO` & `mpr-1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: mpr
-Version: 1.8
-Summary: Wrapper for MicroPython mpremote tool
-Home-page: https://github.com/bulletmark/mpr
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
-License: GPLv3
-Keywords: micropython mpremote webrepl ampy rshell mpfshell upyloader upydev thonny
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 ## MPR - Wrapper for MicroPython mpremote tool
 [![PyPi](https://img.shields.io/pypi/v/mpr)](https://pypi.org/project/mpr/)
 [![AUR](https://img.shields.io/aur/version/mpr)](https://aur.archlinux.org/packages/mpr/)
 
 The [mpremote][mpremote] command line tool is used to interact with a
 [MicroPython][upy] device over a USB/serial connection. It's an official
 part of [MicroPython][upy], well featured, and it works more reliably
@@ -27,23 +14,23 @@
 help for all commands so they can easily see usage and expected
 arguments (e.g. like [git](https://git-scm.com/) provides).
 
 So [mpr][mpr] presents an alternative "git-like" interface which wraps
 [mpremote][mpremote] and behaves like a conventional Linux command line
 tool where only a single command is accepted (although note there are
 global options to connect an explicit device and/or mount a local
-directory before that command). Unlike [mpremote][mpremote], multiple
-file/directory arguments can be specified for a command, allowing you to
-exploit your shell wildcard abilities. Full in-built usage help is
-available for the tool, and each of it's commands (see [Usage](#usage)
-section below). It also provides a novel shortcut mechanism to [infer
-target device directories](#directorypath-inference) based on where on
-your local PC you are copying files from or to. There are a few other
-nice [features](#compatibility-notes). The following session shows small
-examples of [mpr][mpr] in use.
+directory before that command). Unlike [mpremote][mpremote], [mpr][mpr]
+always allows you to exploit your shell wildcard abilities to pass
+multiple file/directory arguments to commands. Full in-built usage help
+is available for the tool, and each of it's commands (see
+[Usage](#usage) section below). It also provides a novel shortcut
+mechanism to [infer target device directories](#directorypath-inference)
+based on where on your local PC you are copying files from or to. There
+are a few other nice [features](#compatibility-notes). The following
+session shows small examples of [mpr][mpr] in use.
 
 ```
 $ tree
 ./
 ├── Makefile
 ├── boot.py
 ├── main.py
@@ -122,20 +109,20 @@
 ```
 $ cd mpr # i.e. to git source dir above
 $ git pull
 $ sudo pip3 install -U .
 ```
 ## Usage
 
-Type `mpr` or `mpr -h` to view the following usage summary:
+Type `mpr` or `mpr -h` to view the usage summary:
 
 ```
 usage: mpr [-h] [-d DEVICE] [-m MOUNT] [-M MOUNT_UNSAFE_LINKS] [-x] [-b]
               [-p PATH_TO_MPREMOTE] [-c] [-v]
-              {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,bootloader,df,setrtc,version,config,cf}
+              {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,mip,m,bootloader,df,setrtc,version,config,cf}
               ...
 
 This is a command line tool to wrap the MicroPython mpremote tool and provide
 a more conventional command line interface. Multiple arguments can be
 specified for commands and inbuilt usage help is provided for all commands.
 
 options:
@@ -152,15 +139,15 @@
   -b, --reboot          do hard reboot after command
   -p PATH_TO_MPREMOTE, --path-to-mpremote PATH_TO_MPREMOTE
                         path to mpremote program, default = "mpremote"
   -c, --completion      output shell TAB completion code
   -v, --verbose         print executed commands (for debug)
 
 Commands:
-  {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,bootloader,df,setrtc,version,config,cf}
+  {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,mip,m,bootloader,df,setrtc,version,config,cf}
     get (g)             Copy one or more files from device to local directory.
     put (p)             Copy one or more local files to directory on device.
     copy (c)            Copy one of more remote files to a directory on
                         device.
     ls                  List directory on device.
     mkdir (mkd)         Create the given directory[s] on device.
     rmdir (rmd)         Remove the given directory[s] on device.
@@ -170,14 +157,15 @@
     reset (x)           Soft reset the device.
     reboot (b)          Hard reboot the device.
     repl (r)            Enter REPL on device.
     list (l, devs)      List currently connected devices.
     run                 Run the given local scripts on device.
     eval                Evaluate and print the given strings on device.
     exec                Execute the given strings on device.
+    mip (m)             Use mip to install packages on device.
     bootloader          Enter bootloader on device.
     df                  Show flash usage on device.
     setrtc              Set the Real Time Clock (RTC) on device.
     version             Show version of mpremote tool.
     config (cf)         Open the mpr configuration file with your editor.
 
 Type "mpr <command> -h" to see specific help/usage for any of the above
@@ -328,15 +316,15 @@
 
 ### Command `edit`
 
 ```
 usage: mpr edit [-h] file [file ...]
 
 Edit the given file[s] on device. Copies the file from device, opens your
-editor on that local file, then copies it back if changed.
+editor on that local file, then copies it back.
 
 positional arguments:
   file        name of file[s]
 
 options:
   -h, --help  show this help message and exit
 
@@ -449,14 +437,38 @@
 
 options:
   -h, --help  show this help message and exit
 
 aliases: <none>
 ```
 
+### Command `mip`
+
+```
+usage: mpr mip [-h] [-n] [-t TARGET] [-i INDEX]
+                  command package [package ...]
+
+Use mip to install packages on device.
+
+positional arguments:
+  command               mip command, e.g. "install"
+  package               package specifications, e.g. "name", "name@version",
+                        "github.org/repo", "github.org/repo@branch"
+
+options:
+  -h, --help            show this help message and exit
+  -n, --no-mpy          do not download the compiled .mpy files
+  -t TARGET, --target TARGET
+                        destination directory on device
+  -i INDEX, --index INDEX
+                        package index to use, default="micropython-lib"
+
+aliases: m
+```
+
 ### Command `bootloader`
 
 ```
 usage: mpr bootloader [-h]
 
 Enter bootloader on device.
 
@@ -558,28 +570,14 @@
 -l` to print out the standard mpremote device mnemonics and names which
 can be used.
 
 The `cp` command in mpremote is implemented with explicit `get` and
 `put` commands in mpr so there is no need for the user to use a `:` char
 to infer direction.
 
-With mpremote all commands that take an argument only accept a single
-argument whereas with mpr all commands can accept multiple arguments
-(which mpr implements internally by executing mpremote multiple times).
-Most specifically, this allow you to exploit wildcard file selection
-with your shell. E.g to copy all the Python files from your local
-directory you simply do:
-
-```
-$ mpr put *.py /
-```
-
-With mpremote, you would have to do the above with individual commands,
-one for each file.
-
 mpr provides shortcut aliases for the most commonly used longer
 commands, e.g. `r` for `repl`, `p` for `put`, and `g` for `get`. See the
 main help/usage for a list of all commands and their aliases. So the
 above command can be tersely typed as:
 
 ```
 $ mpr p *.py /
@@ -622,15 +620,15 @@
 There are some undocumented features in mpremote which have been added
 to mpr as they are discovered.
 
 1. The `reboot` command can accept an optional millisecs delay.
 2. The `put` command (`cp` in mpremote) can copy a specified local
    directory recursively to root (`/`) on the device.
 
-## Default Arguments
+## Default Options
 
 You can set default starting options for your user in
 `~/.config/mpr.conf`. E.g. use this to set a default
 `--path-to-mpremote` setting so it does not have to be specified each
 time. Blank lines and anything after a `#` on any line is ignored.
 
 E.g. create `~/.config/mpr.conf` with contents:
@@ -737,16 +735,16 @@
 
 The mpr option `--path-to-mpremote` defaults to `mpremote` which will
 normally be found by your shell in a standard location (e.g.
 `/usr/bin/mpremote`) but if you have the MicroPython source installed
 somewhere then you don't need to formally install mpremote and can
 instead just set e.g. `--path-to-mpremote
 /opt/micropython/tools/mpremote/mpremote.py` in your
-`~/.config/mpr.conf` as a [default argument](#default-arguments) as
-described in a previous [section](#default-arguments).
+`~/.config/mpr.conf` as a [default option](#default-options) as
+described in a previous [section](#default-options).
 
 ## Shell Tab Completion
 
 If you install the Python 3 [argcomplete](https://kislyuk.github.io/argcomplete/) package:
 
 ```
 $ sudo pip3 install -U argcomplete
```

### Comparing `mpr-1.8/README.md` & `mpr-1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: mpr
+Version: 1.9
+Summary: Wrapper for MicroPython mpremote tool
+Home-page: https://github.com/bulletmark/mpr
+Author: Mark Blakeney
+Author-email: mark.blakeney@bullet-systems.net
+License: GPLv3
+Keywords: micropython mpremote webrepl ampy rshell mpfshell upyloader upydev thonny
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 ## MPR - Wrapper for MicroPython mpremote tool
 [![PyPi](https://img.shields.io/pypi/v/mpr)](https://pypi.org/project/mpr/)
 [![AUR](https://img.shields.io/aur/version/mpr)](https://aur.archlinux.org/packages/mpr/)
 
 The [mpremote][mpremote] command line tool is used to interact with a
 [MicroPython][upy] device over a USB/serial connection. It's an official
 part of [MicroPython][upy], well featured, and it works more reliably
@@ -14,23 +27,23 @@
 help for all commands so they can easily see usage and expected
 arguments (e.g. like [git](https://git-scm.com/) provides).
 
 So [mpr][mpr] presents an alternative "git-like" interface which wraps
 [mpremote][mpremote] and behaves like a conventional Linux command line
 tool where only a single command is accepted (although note there are
 global options to connect an explicit device and/or mount a local
-directory before that command). Unlike [mpremote][mpremote], multiple
-file/directory arguments can be specified for a command, allowing you to
-exploit your shell wildcard abilities. Full in-built usage help is
-available for the tool, and each of it's commands (see [Usage](#usage)
-section below). It also provides a novel shortcut mechanism to [infer
-target device directories](#directorypath-inference) based on where on
-your local PC you are copying files from or to. There are a few other
-nice [features](#compatibility-notes). The following session shows small
-examples of [mpr][mpr] in use.
+directory before that command). Unlike [mpremote][mpremote], [mpr][mpr]
+always allows you to exploit your shell wildcard abilities to pass
+multiple file/directory arguments to commands. Full in-built usage help
+is available for the tool, and each of it's commands (see
+[Usage](#usage) section below). It also provides a novel shortcut
+mechanism to [infer target device directories](#directorypath-inference)
+based on where on your local PC you are copying files from or to. There
+are a few other nice [features](#compatibility-notes). The following
+session shows small examples of [mpr][mpr] in use.
 
 ```
 $ tree
 ./
 ├── Makefile
 ├── boot.py
 ├── main.py
@@ -109,20 +122,20 @@
 ```
 $ cd mpr # i.e. to git source dir above
 $ git pull
 $ sudo pip3 install -U .
 ```
 ## Usage
 
-Type `mpr` or `mpr -h` to view the following usage summary:
+Type `mpr` or `mpr -h` to view the usage summary:
 
 ```
 usage: mpr [-h] [-d DEVICE] [-m MOUNT] [-M MOUNT_UNSAFE_LINKS] [-x] [-b]
               [-p PATH_TO_MPREMOTE] [-c] [-v]
-              {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,bootloader,df,setrtc,version,config,cf}
+              {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,mip,m,bootloader,df,setrtc,version,config,cf}
               ...
 
 This is a command line tool to wrap the MicroPython mpremote tool and provide
 a more conventional command line interface. Multiple arguments can be
 specified for commands and inbuilt usage help is provided for all commands.
 
 options:
@@ -139,15 +152,15 @@
   -b, --reboot          do hard reboot after command
   -p PATH_TO_MPREMOTE, --path-to-mpremote PATH_TO_MPREMOTE
                         path to mpremote program, default = "mpremote"
   -c, --completion      output shell TAB completion code
   -v, --verbose         print executed commands (for debug)
 
 Commands:
-  {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,bootloader,df,setrtc,version,config,cf}
+  {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,mip,m,bootloader,df,setrtc,version,config,cf}
     get (g)             Copy one or more files from device to local directory.
     put (p)             Copy one or more local files to directory on device.
     copy (c)            Copy one of more remote files to a directory on
                         device.
     ls                  List directory on device.
     mkdir (mkd)         Create the given directory[s] on device.
     rmdir (rmd)         Remove the given directory[s] on device.
@@ -157,14 +170,15 @@
     reset (x)           Soft reset the device.
     reboot (b)          Hard reboot the device.
     repl (r)            Enter REPL on device.
     list (l, devs)      List currently connected devices.
     run                 Run the given local scripts on device.
     eval                Evaluate and print the given strings on device.
     exec                Execute the given strings on device.
+    mip (m)             Use mip to install packages on device.
     bootloader          Enter bootloader on device.
     df                  Show flash usage on device.
     setrtc              Set the Real Time Clock (RTC) on device.
     version             Show version of mpremote tool.
     config (cf)         Open the mpr configuration file with your editor.
 
 Type "mpr <command> -h" to see specific help/usage for any of the above
@@ -315,15 +329,15 @@
 
 ### Command `edit`
 
 ```
 usage: mpr edit [-h] file [file ...]
 
 Edit the given file[s] on device. Copies the file from device, opens your
-editor on that local file, then copies it back if changed.
+editor on that local file, then copies it back.
 
 positional arguments:
   file        name of file[s]
 
 options:
   -h, --help  show this help message and exit
 
@@ -436,14 +450,38 @@
 
 options:
   -h, --help  show this help message and exit
 
 aliases: <none>
 ```
 
+### Command `mip`
+
+```
+usage: mpr mip [-h] [-n] [-t TARGET] [-i INDEX]
+                  command package [package ...]
+
+Use mip to install packages on device.
+
+positional arguments:
+  command               mip command, e.g. "install"
+  package               package specifications, e.g. "name", "name@version",
+                        "github.org/repo", "github.org/repo@branch"
+
+options:
+  -h, --help            show this help message and exit
+  -n, --no-mpy          do not download the compiled .mpy files
+  -t TARGET, --target TARGET
+                        destination directory on device
+  -i INDEX, --index INDEX
+                        package index to use, default="micropython-lib"
+
+aliases: m
+```
+
 ### Command `bootloader`
 
 ```
 usage: mpr bootloader [-h]
 
 Enter bootloader on device.
 
@@ -545,28 +583,14 @@
 -l` to print out the standard mpremote device mnemonics and names which
 can be used.
 
 The `cp` command in mpremote is implemented with explicit `get` and
 `put` commands in mpr so there is no need for the user to use a `:` char
 to infer direction.
 
-With mpremote all commands that take an argument only accept a single
-argument whereas with mpr all commands can accept multiple arguments
-(which mpr implements internally by executing mpremote multiple times).
-Most specifically, this allow you to exploit wildcard file selection
-with your shell. E.g to copy all the Python files from your local
-directory you simply do:
-
-```
-$ mpr put *.py /
-```
-
-With mpremote, you would have to do the above with individual commands,
-one for each file.
-
 mpr provides shortcut aliases for the most commonly used longer
 commands, e.g. `r` for `repl`, `p` for `put`, and `g` for `get`. See the
 main help/usage for a list of all commands and their aliases. So the
 above command can be tersely typed as:
 
 ```
 $ mpr p *.py /
@@ -609,15 +633,15 @@
 There are some undocumented features in mpremote which have been added
 to mpr as they are discovered.
 
 1. The `reboot` command can accept an optional millisecs delay.
 2. The `put` command (`cp` in mpremote) can copy a specified local
    directory recursively to root (`/`) on the device.
 
-## Default Arguments
+## Default Options
 
 You can set default starting options for your user in
 `~/.config/mpr.conf`. E.g. use this to set a default
 `--path-to-mpremote` setting so it does not have to be specified each
 time. Blank lines and anything after a `#` on any line is ignored.
 
 E.g. create `~/.config/mpr.conf` with contents:
@@ -724,16 +748,16 @@
 
 The mpr option `--path-to-mpremote` defaults to `mpremote` which will
 normally be found by your shell in a standard location (e.g.
 `/usr/bin/mpremote`) but if you have the MicroPython source installed
 somewhere then you don't need to formally install mpremote and can
 instead just set e.g. `--path-to-mpremote
 /opt/micropython/tools/mpremote/mpremote.py` in your
-`~/.config/mpr.conf` as a [default argument](#default-arguments) as
-described in a previous [section](#default-arguments).
+`~/.config/mpr.conf` as a [default option](#default-options) as
+described in a previous [section](#default-options).
 
 ## Shell Tab Completion
 
 If you install the Python 3 [argcomplete](https://kislyuk.github.io/argcomplete/) package:
 
 ```
 $ sudo pip3 install -U argcomplete
```

### Comparing `mpr-1.8/mpr.egg-info/PKG-INFO` & `mpr-1.9/mpr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpr
-Version: 1.8
+Version: 1.9
 Summary: Wrapper for MicroPython mpremote tool
 Home-page: https://github.com/bulletmark/mpr
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: micropython mpremote webrepl ampy rshell mpfshell upyloader upydev thonny
 Classifier: Programming Language :: Python :: 3
@@ -27,23 +27,23 @@
 help for all commands so they can easily see usage and expected
 arguments (e.g. like [git](https://git-scm.com/) provides).
 
 So [mpr][mpr] presents an alternative "git-like" interface which wraps
 [mpremote][mpremote] and behaves like a conventional Linux command line
 tool where only a single command is accepted (although note there are
 global options to connect an explicit device and/or mount a local
-directory before that command). Unlike [mpremote][mpremote], multiple
-file/directory arguments can be specified for a command, allowing you to
-exploit your shell wildcard abilities. Full in-built usage help is
-available for the tool, and each of it's commands (see [Usage](#usage)
-section below). It also provides a novel shortcut mechanism to [infer
-target device directories](#directorypath-inference) based on where on
-your local PC you are copying files from or to. There are a few other
-nice [features](#compatibility-notes). The following session shows small
-examples of [mpr][mpr] in use.
+directory before that command). Unlike [mpremote][mpremote], [mpr][mpr]
+always allows you to exploit your shell wildcard abilities to pass
+multiple file/directory arguments to commands. Full in-built usage help
+is available for the tool, and each of it's commands (see
+[Usage](#usage) section below). It also provides a novel shortcut
+mechanism to [infer target device directories](#directorypath-inference)
+based on where on your local PC you are copying files from or to. There
+are a few other nice [features](#compatibility-notes). The following
+session shows small examples of [mpr][mpr] in use.
 
 ```
 $ tree
 ./
 ├── Makefile
 ├── boot.py
 ├── main.py
@@ -122,20 +122,20 @@
 ```
 $ cd mpr # i.e. to git source dir above
 $ git pull
 $ sudo pip3 install -U .
 ```
 ## Usage
 
-Type `mpr` or `mpr -h` to view the following usage summary:
+Type `mpr` or `mpr -h` to view the usage summary:
 
 ```
 usage: mpr [-h] [-d DEVICE] [-m MOUNT] [-M MOUNT_UNSAFE_LINKS] [-x] [-b]
               [-p PATH_TO_MPREMOTE] [-c] [-v]
-              {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,bootloader,df,setrtc,version,config,cf}
+              {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,mip,m,bootloader,df,setrtc,version,config,cf}
               ...
 
 This is a command line tool to wrap the MicroPython mpremote tool and provide
 a more conventional command line interface. Multiple arguments can be
 specified for commands and inbuilt usage help is provided for all commands.
 
 options:
@@ -152,15 +152,15 @@
   -b, --reboot          do hard reboot after command
   -p PATH_TO_MPREMOTE, --path-to-mpremote PATH_TO_MPREMOTE
                         path to mpremote program, default = "mpremote"
   -c, --completion      output shell TAB completion code
   -v, --verbose         print executed commands (for debug)
 
 Commands:
-  {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,bootloader,df,setrtc,version,config,cf}
+  {get,g,put,p,copy,c,ls,mkdir,mkd,rmdir,rmd,rm,touch,edit,e,reset,x,reboot,b,repl,r,list,l,devs,run,eval,exec,mip,m,bootloader,df,setrtc,version,config,cf}
     get (g)             Copy one or more files from device to local directory.
     put (p)             Copy one or more local files to directory on device.
     copy (c)            Copy one of more remote files to a directory on
                         device.
     ls                  List directory on device.
     mkdir (mkd)         Create the given directory[s] on device.
     rmdir (rmd)         Remove the given directory[s] on device.
@@ -170,14 +170,15 @@
     reset (x)           Soft reset the device.
     reboot (b)          Hard reboot the device.
     repl (r)            Enter REPL on device.
     list (l, devs)      List currently connected devices.
     run                 Run the given local scripts on device.
     eval                Evaluate and print the given strings on device.
     exec                Execute the given strings on device.
+    mip (m)             Use mip to install packages on device.
     bootloader          Enter bootloader on device.
     df                  Show flash usage on device.
     setrtc              Set the Real Time Clock (RTC) on device.
     version             Show version of mpremote tool.
     config (cf)         Open the mpr configuration file with your editor.
 
 Type "mpr <command> -h" to see specific help/usage for any of the above
@@ -328,15 +329,15 @@
 
 ### Command `edit`
 
 ```
 usage: mpr edit [-h] file [file ...]
 
 Edit the given file[s] on device. Copies the file from device, opens your
-editor on that local file, then copies it back if changed.
+editor on that local file, then copies it back.
 
 positional arguments:
   file        name of file[s]
 
 options:
   -h, --help  show this help message and exit
 
@@ -449,14 +450,38 @@
 
 options:
   -h, --help  show this help message and exit
 
 aliases: <none>
 ```
 
+### Command `mip`
+
+```
+usage: mpr mip [-h] [-n] [-t TARGET] [-i INDEX]
+                  command package [package ...]
+
+Use mip to install packages on device.
+
+positional arguments:
+  command               mip command, e.g. "install"
+  package               package specifications, e.g. "name", "name@version",
+                        "github.org/repo", "github.org/repo@branch"
+
+options:
+  -h, --help            show this help message and exit
+  -n, --no-mpy          do not download the compiled .mpy files
+  -t TARGET, --target TARGET
+                        destination directory on device
+  -i INDEX, --index INDEX
+                        package index to use, default="micropython-lib"
+
+aliases: m
+```
+
 ### Command `bootloader`
 
 ```
 usage: mpr bootloader [-h]
 
 Enter bootloader on device.
 
@@ -558,28 +583,14 @@
 -l` to print out the standard mpremote device mnemonics and names which
 can be used.
 
 The `cp` command in mpremote is implemented with explicit `get` and
 `put` commands in mpr so there is no need for the user to use a `:` char
 to infer direction.
 
-With mpremote all commands that take an argument only accept a single
-argument whereas with mpr all commands can accept multiple arguments
-(which mpr implements internally by executing mpremote multiple times).
-Most specifically, this allow you to exploit wildcard file selection
-with your shell. E.g to copy all the Python files from your local
-directory you simply do:
-
-```
-$ mpr put *.py /
-```
-
-With mpremote, you would have to do the above with individual commands,
-one for each file.
-
 mpr provides shortcut aliases for the most commonly used longer
 commands, e.g. `r` for `repl`, `p` for `put`, and `g` for `get`. See the
 main help/usage for a list of all commands and their aliases. So the
 above command can be tersely typed as:
 
 ```
 $ mpr p *.py /
@@ -622,15 +633,15 @@
 There are some undocumented features in mpremote which have been added
 to mpr as they are discovered.
 
 1. The `reboot` command can accept an optional millisecs delay.
 2. The `put` command (`cp` in mpremote) can copy a specified local
    directory recursively to root (`/`) on the device.
 
-## Default Arguments
+## Default Options
 
 You can set default starting options for your user in
 `~/.config/mpr.conf`. E.g. use this to set a default
 `--path-to-mpremote` setting so it does not have to be specified each
 time. Blank lines and anything after a `#` on any line is ignored.
 
 E.g. create `~/.config/mpr.conf` with contents:
@@ -737,16 +748,16 @@
 
 The mpr option `--path-to-mpremote` defaults to `mpremote` which will
 normally be found by your shell in a standard location (e.g.
 `/usr/bin/mpremote`) but if you have the MicroPython source installed
 somewhere then you don't need to formally install mpremote and can
 instead just set e.g. `--path-to-mpremote
 /opt/micropython/tools/mpremote/mpremote.py` in your
-`~/.config/mpr.conf` as a [default argument](#default-arguments) as
-described in a previous [section](#default-arguments).
+`~/.config/mpr.conf` as a [default option](#default-options) as
+described in a previous [section](#default-options).
 
 ## Shell Tab Completion
 
 If you install the Python 3 [argcomplete](https://kislyuk.github.io/argcomplete/) package:
 
 ```
 $ sudo pip3 install -U argcomplete
```

### Comparing `mpr-1.8/mpr.py` & `mpr-1.9/mpr.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 else:
     completion = True
 
 PROG = Path(__file__).stem
 CNFFILE = Path(os.getenv('XDG_CONFIG_HOME', '~/.config'), f'{PROG}.conf')
 CWD = Path.cwd()
 commands = []
+options = {}
+aliases_all = set()
 cnffile = None
 
 def get_editor():
     'Return editor for this user'
     return os.getenv('VISUAL') or os.getenv('EDITOR') or 'vi'
 
 def infer_root(path, *, dest=False):
@@ -118,14 +120,35 @@
     res = subprocess.run(cmd, stderr=out, stdout=out, shell=True)
     if res.returncode != 0:
         doexit(args, res.returncode)
     return res.stdout
 
 mpcmd.cmdtext = None
 
+def mpcmd_wrap(args):
+    'Extract args/options and send to device'
+    opts = options[args.cmdname]
+    arglist = [args.cmdname]
+    for opt in opts._actions:
+        arg = args.__dict__.get(opt.dest)
+        if arg is None:
+            continue
+        if opt.const:
+            if arg == opt.default:
+                continue
+            arg = None
+
+        if opt.option_strings:
+            arglist.append(opt.option_strings[-1])
+
+        if arg is not None:
+            arglist.append(' '.join(arg) if isinstance(arg, list) else arg)
+
+    mpcmd(args, ' '.join(arglist))
+
 def main():
     'Main code'
     global cnffile
 
     # Parse arguments
     opt = argparse.ArgumentParser(description=__doc__,
             epilog=f'Type "{PROG} <command> -h" to see specific help/usage '
@@ -164,20 +187,26 @@
             desc = cls.doc.strip()
         elif cls.__doc__:
             desc = cls.__doc__.strip()
         else:
             sys.exit(f'Must define a docstring for command class "{name}".')
 
         title = desc.splitlines()[0]
-        assert title[-1] == '.', f'Title "{title}" should include full stop.'
+        if title[-1] != '.':
+            sys.exit(f'Title "{title}" should include full stop.')
 
+        # Code check to ensure we have not defined duplicate aliases
         aliases = cls.aliases if hasattr(cls, 'aliases') else []
+        for a in aliases:
+            if a in aliases_all:
+                sys.exit(f'command {name}: duplicate alias: {a}')
+            aliases_all.add(a)
 
-        cmdopt = cmd.add_parser(name, description=desc, help=title,
-                aliases=aliases)
+        options[name] = cmdopt = cmd.add_parser(name, description=desc,
+                                help=title, aliases=aliases)
 
         # Set up this commands own arguments, if it has any
         if hasattr(cls, 'init'):
             cls.init(cmdopt)
 
         # Set the function to call
         cmdopt.set_defaults(func=cls.run)
@@ -380,33 +409,31 @@
 class _touch(COMMAND):
     'Touch the given file[s] on device.'
 
     def init(opt):
         opt.add_argument('file', nargs='+', help='name of file[s]')
 
     def run(args):
-        files = ' '.join(args.file)
-        mpcmd(args, f'touch {files}')
+        mpcmd_wrap(args)
 
 @command
 class _edit(COMMAND):
     '''
     Edit the given file[s] on device.
 
     Copies the file from device, opens your editor on that local file,
-    then copies it back if changed.
+    then copies it back.
     '''
     aliases = ['e']
 
     def init(opt):
         opt.add_argument('file', nargs='+', help='name of file[s]')
 
     def run(args):
-        files = ' '.join(args.file)
-        mpcmd(args, f'edit {files}')
+        mpcmd_wrap(args)
 
 @command
 class _reset(COMMAND):
     'Soft reset the device.'
     aliases = ['x']
 
     def run(args):
@@ -437,22 +464,15 @@
                 help='capture output of the REPL session to given file')
         opt.add_argument('-x', '--inject-code',
                 help='characters to inject at the REPL when Ctrl-J is pressed')
         opt.add_argument('-i', '--inject-file',
                 help='file to inject at the REPL when Ctrl-K is pressed')
 
     def run(args):
-        arglist = ['repl']
-        for opt in ('capture', 'inject_code', 'inject_file'):
-            arg = args.__dict__.get(opt)
-            if arg:
-                opt = opt.replace('_', '-')
-                arglist.append(f'--{opt} "{arg}"')
-
-        mpcmd(args, ' '.join(arglist))
+        mpcmd_wrap(args)
 
 @command
 class _list(COMMAND):
     'List currently connected devices.'
     aliases = ['l', 'devs']
 
     def run(args):
@@ -491,14 +511,35 @@
                 help='string to execute')
 
     def run(args):
         for string in args.string:
             mpcmd(args, f'exec "{string}"')
 
 @command
+class _mip(COMMAND):
+    'Run mip to install packages on device.'
+    aliases = ['m']
+
+    def init(opt):
+        opt.add_argument('-n', '--no-mpy', action='store_true',
+                help='download .py files, not compiled .mpy files')
+        opt.add_argument('-t', '--target',
+                help='destination directory on device')
+        opt.add_argument('-i', '--index',
+                help='package index to use, default="micropython-lib"')
+        opt.add_argument('command',
+                help='mip command, e.g. "install"')
+        opt.add_argument('package', nargs='+',
+                help='package specifications, e.g. "name", "name@version", '
+                         '"github.org/repo", "github.org/repo@branch"')
+
+    def run(args):
+        mpcmd_wrap(args)
+
+@command
 class _bootloader(COMMAND):
     'Enter bootloader on device.'
 
 @command
 class _df(COMMAND):
     'Show flash usage on device.'
```

### Comparing `mpr-1.8/setup.py` & `mpr-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 name = 'mpr'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 
 setup(
     name=name,
-    version='1.8',
+    version='1.9',
     description='Wrapper for MicroPython mpremote tool',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/bulletmark/{name}',
     author='Mark Blakeney',
     author_email='mark.blakeney@bullet-systems.net',
     keywords='micropython mpremote webrepl ampy rshell '
```

