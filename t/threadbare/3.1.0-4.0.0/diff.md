# Comparing `tmp/threadbare-3.1.0.tar.gz` & `tmp/threadbare-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadbare-3.1.0.tar", last modified: Tue Jun  6 04:32:32 2023, max compression
+gzip compressed data, was "threadbare-4.0.0.tar", last modified: Wed Jun 14 02:10:14 2023, max compression
```

## Comparing `threadbare-3.1.0.tar` & `threadbare-4.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.886560 threadbare-3.1.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    35147 2023-06-06 04:32:01.000000 threadbare-3.1.0/LICENCE.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2023-06-06 04:32:32.886560 threadbare-3.1.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5296 2023-06-06 04:32:01.000000 threadbare-3.1.0/README.md
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-06-06 04:32:32.886560 threadbare-3.1.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      764 2023-06-06 04:32:01.000000 threadbare-3.1.0/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.882560 threadbare-3.1.0/tests/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     2030 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_common.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    12453 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_execute.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    23949 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_operations.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     6438 2023-06-06 04:32:01.000000 threadbare-3.1.0/tests/test_state.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.882560 threadbare-3.1.0/threadbare/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     3274 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/common.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    10351 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/execute.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    38946 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/operations.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     3953 2023-06-06 04:32:01.000000 threadbare-3.1.0/threadbare/state.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-06 04:32:32.886560 threadbare-3.1.0/threadbare.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      398 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       11 2023-06-06 04:32:32.000000 threadbare-3.1.0/threadbare.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-14 02:10:14.827000 threadbare-4.0.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    34523 2023-06-14 02:09:32.000000 threadbare-4.0.0/LICENCE.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2023-06-14 02:10:14.827000 threadbare-4.0.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5457 2023-06-14 02:09:32.000000 threadbare-4.0.0/README.md
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-06-14 02:10:14.827000 threadbare-4.0.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      765 2023-06-14 02:09:32.000000 threadbare-4.0.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-14 02:10:14.799000 threadbare-4.0.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     2030 2023-06-14 02:09:32.000000 threadbare-4.0.0/tests/test_common.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    12453 2023-06-14 02:09:32.000000 threadbare-4.0.0/tests/test_execute.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    23423 2023-06-14 02:09:32.000000 threadbare-4.0.0/tests/test_operations.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     6438 2023-06-14 02:09:32.000000 threadbare-4.0.0/tests/test_state.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-14 02:10:14.799000 threadbare-4.0.0/threadbare/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      847 2023-06-14 02:09:32.000000 threadbare-4.0.0/threadbare/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     3274 2023-06-14 02:09:32.000000 threadbare-4.0.0/threadbare/common.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    10351 2023-06-14 02:09:32.000000 threadbare-4.0.0/threadbare/execute.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    36754 2023-06-14 02:09:32.000000 threadbare-4.0.0/threadbare/operations.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     3953 2023-06-14 02:09:32.000000 threadbare-4.0.0/threadbare/state.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-14 02:10:14.827000 threadbare-4.0.0/threadbare.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      604 2023-06-14 02:10:14.000000 threadbare-4.0.0/threadbare.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      398 2023-06-14 02:10:14.000000 threadbare-4.0.0/threadbare.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-06-14 02:10:14.000000 threadbare-4.0.0/threadbare.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       21 2023-06-14 02:10:14.000000 threadbare-4.0.0/threadbare.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       11 2023-06-14 02:10:14.000000 threadbare-4.0.0/threadbare.egg-info/top_level.txt
```

### Comparing `threadbare-3.1.0/LICENCE.txt` & `threadbare-4.0.0/LICENCE.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
+our General Public Licenses are intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+software for all its users.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+  "This License" refers to version 3 of the GNU Affero General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -545,43 +533,53 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
+under version 3 of the GNU General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
+Program specifies that a certain numbered version of the GNU Affero General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
+GNU Affero General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
+versions of the GNU Affero General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -631,44 +629,33 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
+    it under the terms of the GNU Affero General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    GNU Affero General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

### Comparing `threadbare-3.1.0/PKG-INFO` & `threadbare-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: threadbare
-Version: 3.1.0
+Version: 4.0.0
 Summary: A Fabric and Paramiko replacement library
 Home-page: https://github.com/elifesciences/threadbare
 Maintainer: Luke
 Maintainer-email: lsh-0@users.noreply.github.com
-License: GPLv3
+License: AGPLv3
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 A partial replacement of the Fabric and Paramiko libraries using ParallelSSH.
```

### Comparing `threadbare-3.1.0/README.md` & `threadbare-4.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 ```python
 from threadbare.state import settings
 from threadbare.operations import remote
 with settings(host_string='my.server', warn_only=True):
     remote("echo 'hello world!'")
 ```
 
+See [example.py](./example.py) for more.
+
 ## local tests
 
 Run the [test suite](./test.sh) with `./test.sh`
 
 Individual tests can be run with `./test.sh example.py::test_fn_name`
 
 ## remote tests
@@ -136,7 +138,12 @@
 mechanism for manipulating global state. 
 
 * changes to global state within the worker function does not propagate back to the parent
 * SSH connections cannot be passed to child processes so new connections are made within the child process if necessary
 * child processes cannot prompt for input. They have no access to stdin.
 * child processes may die or throw exceptions that can't be properly handled in the parent
 
+## Licence
+
+Copyright © 2019-2023 eLife Sciences
+
+Distributed under the GNU Affero General Public Licence, version 3.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `threadbare-3.1.0/setup.py` & `threadbare-4.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='threadbare',
-    version='3.1.0',
+    version='4.0.0',
     description='A Fabric and Paramiko replacement library',
     long_description="A partial replacement of the Fabric and Paramiko libraries using ParallelSSH.",
     long_description_content_type="text/markdown",
     url="https://github.com/elifesciences/threadbare",
     maintainer="Luke",
     maintainer_email="lsh-0@users.noreply.github.com",
-    install_requires=["parallel-ssh>=1.9.1"],
+    install_requires=["parallel-ssh>=2.12.0"],
     packages=["threadbare"],
     classifiers=[
         "Intended Audience :: System Administrators",
         "Programming Language :: Python :: 3",
         "Operating System :: POSIX",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
     ],
-    license="GPLv3"
+    license="AGPLv3"
 )
```

### Comparing `threadbare-3.1.0/tests/test_common.py` & `threadbare-4.0.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.1.0/tests/test_execute.py` & `threadbare-4.0.0/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.1.0/tests/test_operations.py` & `threadbare-4.0.0/tests/test_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import unittest.mock as mock
 from unittest.mock import patch
 from io import StringIO
 import pytest
 from threadbare import operations, state
 from threadbare.common import merge, cwd, PromptedException
-from pssh import exceptions as pssh_exceptions
 
 # remote
 
 HOST = "testhost"
 USER = "testuser"
 PORT = 666
 PEM = "/home/testuser/.ssh/id_rsa"
@@ -232,46 +231,30 @@
                 "stderr": [],
             }
             operations.remote(**merge(base, given_kwargs))
             mockobj.assert_called_with(**merge(base, expected_kwargs))
 
 
 def test_remote_command_exception():
+    """exceptions from the parallel-ssh client are passed through.
+    previously they were caught and wrapped in an `operations.NetworkError`."""
     kwargs = {
         "host_string": HOST,
         "port": PORT,
         "user": USER,
         "key_filename": PEM,
         "command": "echo hello",
     }
     m = mock.MagicMock()
-    m.run_command = mock.Mock(side_effect=ValueError("earthshatteringkaboom"))
+    m.run_command = mock.Mock(side_effect=ConnectionRefusedError("whom?"))
     with patch("threadbare.operations.SSHClient", return_value=m):
-        with pytest.raises(operations.NetworkError):
+        with pytest.raises(ConnectionRefusedError):
             operations.remote(**kwargs)
 
 
-def test_remote_command_timeout_exception():
-    kwargs = {
-        "host_string": HOST,
-        "port": PORT,
-        "user": USER,
-        "key_filename": PEM,
-        "command": "echo hello",
-    }
-    m = mock.MagicMock()
-    m.run_command = mock.Mock(side_effect=pssh_exceptions.Timeout("foobar"))
-    with patch("threadbare.operations.SSHClient", return_value=m):
-        with pytest.raises(operations.NetworkError) as err:
-            operations.remote(**kwargs)
-        err = err.value
-        assert type(err.wrapped) == pssh_exceptions.Timeout
-        assert str(err) == "Timed out trying to connect. foobar"
-
-
 # local
 
 
 def test_lcd():
     "changes the local working directory"
     cur_cwd = cwd()
     new_cwd = "/tmp"
```

### Comparing `threadbare-3.1.0/tests/test_state.py` & `threadbare-4.0.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.1.0/threadbare/__init__.py` & `threadbare-4.0.0/threadbare/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from gevent import monkey
 
 monkey.patch_all()
 
 import os  # NOQA: E402
 
 if os.path.exists("README.md"):
-    data = open("README.md").read()
-    __doc__ = str(data)
+    with open("README.md") as fh:
+        __doc__ = str(fh.read())
 
 from . import state, operations, execute  # NOQA: E402
 
 assert state and operations and execute  # quieten pyflakes
 
 import logging  # NOQA: E402
```

### Comparing `threadbare-3.1.0/threadbare/common.py` & `threadbare-4.0.0/threadbare/common.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.1.0/threadbare/execute.py` & `threadbare-4.0.0/threadbare/execute.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.1.0/threadbare/operations.py` & `threadbare-4.0.0/threadbare/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,50 +32,24 @@
     def __deepcopy__(self, memo):
         # do not copy.deepcopy ourselves or the pssh SSHClient object, just
         # return a reference to the object (self)
         # - https://docs.python.org/3/library/copy.html
         return self
 
 
-class NetworkError(BaseException):
-    """generic 'died while doing something ssh-related' catch-all exception class.
-    calling str() on this exception will return the results of calling str() on the
-    wrapped exception."""
-
-    def __init__(self, wrapped_exception_inst):
-        self.wrapped = wrapped_exception_inst
-
-    def __str__(self):
-        # for cases where we want the convenient:
-        #   `raise NetworkError("some network problem")`
-        if isinstance(self.wrapped, str):
-            return self.wrapped
-
-        # we have the opportunity here to tweak the error messages to make them
-        # similar to their equivalents in Fabric.
-        # original error messages are still available via `str(excinst.wrapped)`
-        space = " "
-        custom_error_prefixes = {
-            # builder: https://github.com/elifesciences/builder/blob/master/src/buildercore/core.py#L345-L347
-            # pssh: https://github.com/ParallelSSH/parallel-ssh/blob/8b7bb4bcb94d913c3b7da77db592f84486c53b90/pssh/clients/native/parallel.py#L272-L274
-            pssh.exceptions.Timeout: "Timed out trying to connect.",
-            # builder: https://github.com/elifesciences/builder/blob/master/src/buildercore/core.py#L348-L350
-            # fabric: https://github.com/mathiasertl/fabric/blob/master/fabric/network.py#L601-L605
-            # pssh: https://github.com/ParallelSSH/parallel-ssh/blob/2e9668cf4b58b38316b1d515810d7e6c595c76f3/pssh/exceptions.py
-            pssh.exceptions.SSHException: "Low level socket error connecting to host.",
-            pssh.exceptions.SessionError: "Low level socket error connecting to host.",
-            # lsh@2023-05-08: changed in pssh 2.9.0 and deprecated, pssh uses the builtin now.
-            pssh.exceptions.ConnectionErrorException: "Low level socket error connecting to host.",
-            ConnectionError: "Low level socket error connecting to host.",
-            # lsh@2023-05-08: introduced in pssh 2.9.0, we have to capture this and retry it ourselves.
-            ConnectionRefusedError: "Low level socket error connecting to host.",
-        }
-        new_error = custom_error_prefixes.get(type(self.wrapped)) or ""
-        original_error = str(self.wrapped)
-        return new_error + space + original_error
+class NetworkError(Exception):
+    "generic 'died while doing something network-related' catch-all exception class."
+    pass
+
+
+class WrappedNetworkError(NetworkError):
+    "groups several exceptions into a single WrappedNetworkError"
+
+    def __init__(self, exc):
+        self.wrapped = exc
 
 
 def pem_key():
     """returns the first private key found in a list of common private keys.
     if none of the keys exist, the default (first) key will be returned."""
     id_list = ["id_rsa", "id_dsa", "identity", "id_ecdsa"]
     id_list = [os.path.expanduser("~/.ssh/" + idstr) for idstr in id_list]
@@ -207,41 +181,36 @@
     )
 
     shell = False  # handled ourselves
     sudo = False  # handled ourselves
     user = None  # user to sudo to
     encoding = "utf-8"  # used everywhere
 
-    try:
-        # https://parallel-ssh.readthedocs.io/en/latest/native_single.html#pssh.clients.native.single.SSHClient.run_command
-        # https://github.com/ParallelSSH/parallel-ssh/blob/master/pssh/output.py
-        host_output = client.run_command(
-            command, sudo, user, use_pty, shell, encoding, timeout
-        )
+    # https://parallel-ssh.readthedocs.io/en/latest/native_single.html#pssh.clients.native.single.SSHClient.run_command
+    # https://github.com/ParallelSSH/parallel-ssh/blob/master/pssh/output.py
+    host_output = client.run_command(
+        command, sudo, user, use_pty, shell, encoding, timeout
+    )
 
-        host_string = host_output.host
-        stdout = host_output.stdout
-        stderr = host_output.stderr
-
-        def get_exit_code():
-            client.wait_finished(host_output)
-            return host_output.exit_code
-
-        return {
-            # defer executing as it consumes output entirely before returning. this
-            # removes our chance to display/transform output as it is streamed to us
-            "return_code": get_exit_code,
-            "command": command,
-            "stdout": stdout,
-            "stderr": stderr,
-        }
-    except BaseException as ex:
-        # *probably* a network error:
-        # - https://github.com/ParallelSSH/parallel-ssh/blob/master/pssh/exceptions.py
-        raise NetworkError(ex)
+    host_string = host_output.host
+    stdout = host_output.stdout
+    stderr = host_output.stderr
+
+    def get_exit_code():
+        client.wait_finished(host_output)
+        return host_output.exit_code
+
+    return {
+        # defer executing as it consumes output entirely before returning. this
+        # removes our chance to display/transform output as it is streamed to us
+        "return_code": get_exit_code,
+        "command": command,
+        "stdout": stdout,
+        "stderr": stderr,
+    }
 
 
 def _print_line(output_pipe, line, **kwargs):
     """writes the given `line` (string) to the given `output_pipe` (file-like object)
     if `quiet` is True, `line` is *not* written to `output_pipe`.
     if `discard_output` is True, `line` is *not* returned and output does *not* accumulate in memory."""
 
@@ -275,15 +244,15 @@
         }
 
         # render template and write to given pipe
         template = final_kwargs["line_template"]
 
         if not final_kwargs["display_prefix"]:
             try:
-                template = template[template.index("{line}"):]
+                template = template[template.index("{line}") :]
             except ValueError:  # "substring not found"
                 msg = "'display_prefix' option ignored: '{line}' not found in 'line_template' setting"
                 LOG.warning(msg)
 
         output_pipe.write(template.format(**template_kwargs))
 
     if not final_kwargs["discard_output"]:
@@ -823,15 +792,15 @@
 
     try:
         transfer_fn(remote_tempfile, local_path)
         return local_path
 
     except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
         # permissions or network issues may cause these
-        raise NetworkError(exc)
+        raise WrappedNetworkError(exc)
 
     finally:
         remote_sudo('rm -f "%s"' % remote_tempfile, **kwargs)
 
 
 # https://github.com/mathiasertl/fabric/blob/master/fabric/operations.py#L419
 # use_sudo hack: https://github.com/mathiasertl/fabric/blob/master/fabric/operations.py#L453-L458
@@ -878,19 +847,20 @@
             client = _ssh_client(**kwargs)
             transfer_fn = _transfer_fn(client, "download", **kwargs)
 
             try:
                 transfer_fn(remote_path, local_path)
             except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
                 # permissions or network issues may cause these
-                raise NetworkError(exc)
+                raise WrappedNetworkError(exc)
 
         if temp_file:
             flags = "r" if isinstance(data_buffer, io.StringIO) else "rb"
-            data = open(local_path, flags).read()
+            with open(local_path, flags) as fh:
+                data = fh.read()
             data_buffer.write(data)
             # deletes the *temporary file*. `temp_file` is a file descriptor
             os.unlink(local_path)
             return data_buffer
 
         return local_path
 
@@ -924,15 +894,15 @@
         remote_sudo(move_file_into_place, **kwargs)
         ensure(
             remote_file_exists(remote_path, use_sudo=True, **kwargs),
             "remote path does not exist: %s" % (remote_path),
         )
     except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
         # permissions or network issues may cause these
-        raise NetworkError(exc)
+        raise WrappedNetworkError(exc)
 
 
 def _write_bytes_to_temporary_file(local_path):
     """if `local_path` is a file-like object, write the contents to an *actual* file and
     return a pair of new local filename and a function that removes the temporary file when called."""
     if hasattr(local_path, "read"):
         # `local_path` is a file-like object
@@ -973,8 +943,8 @@
         client = _ssh_client(**kwargs)
 
         try:
             transfer_fn = _transfer_fn(client, "upload", **kwargs)
             transfer_fn(local_path, remote_path)
         except (pssh.exceptions.SFTPError, pssh.exceptions.SCPError) as exc:
             # permissions or network issues may cause these
-            raise NetworkError(exc)
+            raise WrappedNetworkError(exc)
```

### Comparing `threadbare-3.1.0/threadbare/state.py` & `threadbare-4.0.0/threadbare/state.py`

 * *Files identical despite different names*

### Comparing `threadbare-3.1.0/threadbare.egg-info/PKG-INFO` & `threadbare-4.0.0/threadbare.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: threadbare
-Version: 3.1.0
+Version: 4.0.0
 Summary: A Fabric and Paramiko replacement library
 Home-page: https://github.com/elifesciences/threadbare
 Maintainer: Luke
 Maintainer-email: lsh-0@users.noreply.github.com
-License: GPLv3
+License: AGPLv3
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 A partial replacement of the Fabric and Paramiko libraries using ParallelSSH.
```

