# Comparing `tmp/simple_aws_ec2-0.2.1.tar.gz` & `tmp/simple_aws_ec2-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_ec2-0.2.1.tar", last modified: Wed Jun 14 14:25:59 2023, max compression
+gzip compressed data, was "simple_aws_ec2-0.3.1.tar", last modified: Wed Jun 14 19:02:09 2023, max compression
```

## Comparing `simple_aws_ec2-0.2.1.tar` & `simple_aws_ec2-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.384306 simple_aws_ec2-0.2.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5098 2023-06-14 14:25:59.384151 simple_aws_ec2-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4036 2023-06-14 13:43:26.000000 simple_aws_ec2-0.2.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1606 2023-06-14 13:42:31.000000 simple_aws_ec2-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-14 14:25:59.384350 simple_aws_ec2-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.2.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.381888 simple_aws_ec2-0.2.1/simple_aws_ec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-14 14:25:25.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1034 2023-06-14 14:00:30.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.383211 simple_aws_ec2-0.2.1/simple_aws_ec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    18508 2023-06-14 13:50:05.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/ec2.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.383078 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5098 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.383838 simple_aws_ec2-0.2.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-05-03 16:04:16.000000 simple_aws_ec2-0.2.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6793 2023-06-14 13:58:57.000000 simple_aws_ec2-0.2.1/tests/test_ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:02:09.565534 simple_aws_ec2-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-14 19:02:09.565372 simple_aws_ec2-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5722 2023-06-14 19:01:43.000000 simple_aws_ec2-0.3.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1923 2023-06-14 18:54:50.000000 simple_aws_ec2-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-14 19:02:09.565585 simple_aws_ec2-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:02:09.562393 simple_aws_ec2-0.3.1/simple_aws_ec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.3.1/simple_aws_ec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-14 18:53:31.000000 simple_aws_ec2-0.3.1/simple_aws_ec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1186 2023-06-14 18:22:49.000000 simple_aws_ec2-0.3.1/simple_aws_ec2/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:02:09.563223 simple_aws_ec2-0.3.1/simple_aws_ec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.1/simple_aws_ec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    27950 2023-06-14 19:00:28.000000 simple_aws_ec2-0.3.1/simple_aws_ec2/ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:02:09.563093 simple_aws_ec2-0.3.1/simple_aws_ec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-14 19:02:09.000000 simple_aws_ec2-0.3.1/simple_aws_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-06-14 19:02:09.000000 simple_aws_ec2-0.3.1/simple_aws_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-14 19:02:09.000000 simple_aws_ec2-0.3.1/simple_aws_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-14 19:02:09.000000 simple_aws_ec2-0.3.1/simple_aws_ec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-14 19:02:09.000000 simple_aws_ec2-0.3.1/simple_aws_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:02:09.563723 simple_aws_ec2-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      693 2023-06-14 18:52:23.000000 simple_aws_ec2-0.3.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7061 2023-06-14 18:29:00.000000 simple_aws_ec2-0.3.1/tests/test_ec2.py
```

### Comparing `simple_aws_ec2-0.2.1/LICENSE.txt` & `simple_aws_ec2-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.2.1/PKG-INFO` & `simple_aws_ec2-0.3.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: simple_aws_ec2
-Version: 0.2.1
-Summary: Simple AWS EC2 devtool.
-Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.2.1#downloads
-Author: Sanhe Hu
-Author-email: husanhe@gmail.com
-Maintainer: Unknown
-License: MIT
-Platform: Windows
-Platform: MacOS
-Platform: Unix
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
 
 .. .. image:: https://readthedocs.org/projects/simple_aws_ec2/badge/?version=latest
     :target: https://simple_aws_ec2.readthedocs.io/index.html
     :alt: Documentation Status
 
 .. image:: https://github.com/MacHu-GWU/simple_aws_ec2-project/workflows/CI/badge.svg
     :target: https://github.com/MacHu-GWU/simple_aws_ec2-project/actions?query=workflow:CI
@@ -81,33 +50,36 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/simple_aws_ec2#files
 
 
 Welcome to ``simple_aws_ec2`` Documentation
 ==============================================================================
+Simple AWS EC2 dev tool.
+
+Requires Python3.7+
 
 Usage:
 
 .. code-block:: python
 
-    from simple_aws_ec2 import Ec2Instance
-    from boto_session_manager import BotoSesManager
+    import boto3
+    from simple_aws_ec2.api import Ec2Instance, Image
 
-    bsm = BotoSesManager()
+    ec2_client = boto3.client("ec2")
 
     # get ec2 by id
-    ec2_inst = Ec2Instance.from_id(bsm, "i-1a2b3c")
+    ec2_inst = Ec2Instance.from_id(ec2_client, "i-1a2b3c")
     # get ec2 by running code from inside of ec2
-    ec2_inst = EC2Instance.from_ec2_inside(bsm)
+    ec2_inst = EC2Instance.from_ec2_inside(ec2_client)
     # get ec2 by it's name, it returns a iter proxy that may have multiple ec2
-    ec2_inst = EC2Instance.from_ec2_name(bsm, "my-server").one_or_none()
+    ec2_inst = EC2Instance.from_ec2_name(ec2_client, "my-server").one_or_none()
     # get ec2 by tag key value pair, it returns a iter proxy that may have multiple ec2
-    ec2_inst = EC2Instance.from_tag_key_value(bsm, key="Env", value="prod").one_or_none()
-    ec2_inst = EC2Instance.query(bsm, filters=..., instnace_ids=...).all()
+    ec2_inst = EC2Instance.from_tag_key_value(ec2_client, key="Env", value="prod").one_or_none()
+    ec2_inst = EC2Instance.query(ec2_client, filters=..., instnace_ids=...).all()
 
     print(ec2_inst.id)
     print(ec2_inst.status)
     print(ec2_inst.public_ip)
     print(ec2_inst.private_ip)
     print(ec2_inst.vpc_id)
     print(ec2_inst.subnet_id)
@@ -124,14 +96,56 @@
     print(ec2_inst.is_shutting_down()
     print(ec2_inst.is_stopping()
     print(ec2_inst.is_terminated()
 
     print(ec2_inst.is_ready_to_start()
     print(ec2_inst.is_ready_to_stop()
 
+    # the following methods has to be called on a running ec2 instance
+    # it use the EC2 metadata api
+    # https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-data-retrieval.html
+    print(EC2Instance.get_ami_id())
+    print(EC2Instance.get_instance_id())
+    print(EC2Instance.get_instance_type())
+    print(EC2Instance.get_local_hostname())
+    print(EC2Instance.get_local_ipv4())
+    print(EC2Instance.get_public_hostname())
+    print(EC2Instance.get_public_ipv4())
+    print(EC2Instance.get_security_groups()
+
+    # AMI Image API
+    image = Image.from_id(ec2_client, "ami-1a2b3c")
+    image = Image.from_ec2_inside(ec2_client)
+
+    image_list = Image.query(ec2_client).all()
+
+    image_list = Image.query(ec2_client, owners=["self"]).all()
+
+    print(image.image_type_is_machine())
+    print(image.image_type_is_kernel())
+    print(image.image_type_is_ramdisk())
+    print(image.is_pending())
+    print(image.is_available())
+    print(image.is_invalid())
+    print(image.is_deregistered())
+    print(image.is_transient())
+    print(image.is_failed())
+    print(image.is_error())
+    print(image.image_root_device_type_is_ebs())
+    print(image.image_root_device_type_is_instance_store())
+    print(image.image_virtualization_type_is_hvm())
+    print(image.image_virtualization_type_is_paravirtual())
+    print(image.image_boot_mode_is_legacy_bios())
+    print(image.image_boot_mode_is_uefi())
+    print(image.image_boot_mode_is_uefi_preferred())
+
+    image = Image.from_image_name(ec2_client, "my-image").all()
+
+    image_list = Image.from_tag_key_value(ec2_client, key="Env", value="dev").all()
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``simple_aws_ec2`` is released on PyPI, so all you need is:
@@ -140,8 +154,8 @@
 
     $ pip install simple_aws_ec2
 
 To upgrade to latest version:
 
 .. code-block:: console
 
-    $ pip install --upgrade simple_aws_ec2
+    $ pip install --upgrade simple_aws_ec2
```

### Comparing `simple_aws_ec2-0.2.1/release-history.rst` & `simple_aws_ec2-0.3.1/release-history.rst`

 * *Files 7% similar despite different names*

```diff
@@ -11,32 +11,37 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2023-06-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add lots of EC2 instance attributes
+- add helper methods to call EC2 metadata API from EC2 instance inside.
+- add method :meth:`~simple_aws_ec2.ec2.Image.os_type` to guess the AMI OS type, and then get the user name.
+
+
 0.2.1 (2023-06-14)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Breaking change**
 
 - all method now take ec2_client as the first argument. no longer need ``boto_session_manager``.
 
 **Features and Improvements**
 
 - add :class:`~simple_aws_ec2.ec2.Image` class.
 
 **Minor Improvements**
 
 - :meth`~simple_aws_ec2.ec2.Ec2Instance.from_tag_key_value` now take list of values.
 
-**Bugfixes**
-
-**Miscellaneous**
-
 
 0.1.4 (2023-05-06)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that the :meth:`~simple_aws_ec2.ec2.Ec2Instance._yield_dict_from_describe_instances_response` method failed to yield instances objects.
```

### Comparing `simple_aws_ec2-0.2.1/requirements-doc.txt` & `simple_aws_ec2-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.2.1/setup.py` & `simple_aws_ec2-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.2.1/simple_aws_ec2/api.py` & `simple_aws_ec2-0.3.1/simple_aws_ec2/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # -*- coding: utf-8 -*-
 
 """
 Public API.
 
+- :class:`~simple_aws_ec2.ec2.CannotDetectOSTypeError`
 - :class:`~simple_aws_ec2.ec2.EC2InstanceStatusEnum`
 - :class:`~simple_aws_ec2.ec2.EC2InstanceArchitectureEnum`
 - :class:`~simple_aws_ec2.ec2.Ec2InstanceHypervisorEnum`
 - :class:`~simple_aws_ec2.ec2.Ec2Instance`
 - :class:`~simple_aws_ec2.ec2.Ec2InstanceIterProxy`
 - :class:`~simple_aws_ec2.ec2.ImageTypeEnum`
 - :class:`~simple_aws_ec2.ec2.ImageStateEnum`
 - :class:`~simple_aws_ec2.ec2.ImageRootDeviceTypeEnum`
 - :class:`~simple_aws_ec2.ec2.ImageVirtualizationTypeEnum`
 - :class:`~simple_aws_ec2.ec2.ImageBootModeEnum`
 - :class:`~simple_aws_ec2.ec2.ImageOwnerGroupEnum`
+- :class:`~simple_aws_ec2.ec2.ImageOSTypeEnum`
 - :class:`~simple_aws_ec2.ec2.Image`
 - :class:`~simple_aws_ec2.ec2.ImageIterProxy`
 """
 
 from .ec2 import (
+    CannotDetectOSTypeError,
     EC2InstanceStatusEnum,
     EC2InstanceArchitectureEnum,
     Ec2InstanceHypervisorEnum,
     Ec2Instance,
     Ec2InstanceIterProxy,
     ImageTypeEnum,
     ImageStateEnum,
     ImageRootDeviceTypeEnum,
     ImageVirtualizationTypeEnum,
     ImageBootModeEnum,
     ImageOwnerGroupEnum,
+    ImageOSTypeEnum,
     Image,
     ImageIterProxy,
 )
```

### Comparing `simple_aws_ec2-0.2.1/simple_aws_ec2/ec2.py` & `simple_aws_ec2-0.3.1/simple_aws_ec2/ec2.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,36 +3,47 @@
 """
 Abstract dataclass for EC2 instance.
 """
 
 import typing as T
 import enum
 import dataclasses
+from datetime import datetime
 from urllib import request
+
 from func_args import resolve_kwargs, NOTHING
 from iterproxy import IterProxy
 
 
+class CannotDetectOSTypeError(TypeError):
+    """
+    raised when unable to use the name and description to detect the OS type
+    of the AMI.
+    """
+
+    pass
+
+
 def get_response(url: str) -> str:  # pragma: no cover
     """
     Get the text response from the url.
     """
     with request.urlopen(url) as response:
         return response.read().decode("utf-8").strip()
 
 
-def get_instance_id() -> str:  # pragma: no cover
+def _get_metadata(name: str) -> str:  # pragma: no cover
     """
     Get the EC2 instance id from the AWS EC2 metadata API.
 
     Reference:
 
     - https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-data-retrieval.html
     """
-    url = "http://169.254.169.254/latest/meta-data/instance-id"
+    url = f"http://169.254.169.254/latest/meta-data/{name}"
     return get_response(url).strip()
 
 
 class EC2InstanceStatusEnum(str, enum.Enum):
     """
     EC2 instance status enumerations.
 
@@ -72,26 +83,44 @@
 class Ec2Instance:
     """
     Represent an EC2 instance.
     """
 
     id: str = dataclasses.field()
     status: str = dataclasses.field()
+    status_transition_reason: T.Optional[str] = dataclasses.field(default=None)
     public_ip: T.Optional[str] = dataclasses.field(default=None)
     private_ip: T.Optional[str] = dataclasses.field(default=None)
     public_dns_name: T.Optional[str] = dataclasses.field(default=None)
     private_dns_name: T.Optional[str] = dataclasses.field(default=None)
     vpc_id: T.Optional[str] = dataclasses.field(default=None)
     subnet_id: T.Optional[str] = dataclasses.field(default=None)
     security_groups: T.List[T.Dict[str, str]] = dataclasses.field(default_factory=list)
     image_id: T.Optional[str] = dataclasses.field(default=None)
+    platform: T.Optional[str] = dataclasses.field(default=None)
+    platform_details: T.Optional[str] = dataclasses.field(default=None)
     instance_type: T.Optional[str] = dataclasses.field(default=None)
+    launch_time: T.Optional[datetime] = dataclasses.field(default=None)
     key_name: T.Optional[str] = dataclasses.field(default=None)
     architecture: T.Optional[str] = dataclasses.field(default=None)
+    ebs_optimized: T.Optional[bool] = dataclasses.field(default=None)
+    ena_support: T.Optional[bool] = dataclasses.field(default=None)
     hypervisor: T.Optional[str] = dataclasses.field(default=None)
+    iam_instance_profile_arn: T.Optional[str] = dataclasses.field(default=None)
+    iam_instance_profile_id: T.Optional[str] = dataclasses.field(default=None)
+    instance_lifecycle: T.Optional[str] = dataclasses.field(default=None)
+    root_device_name: T.Optional[str] = dataclasses.field(default=None)
+    root_device_type: T.Optional[str] = dataclasses.field(default=None)
+    spot_instance_request_id: T.Optional[str] = dataclasses.field(default=None)
+    sriov_net_support: T.Optional[str] = dataclasses.field(default=None)
+    virtualization_type: T.Optional[str] = dataclasses.field(default=None)
+    boot_mode: T.Optional[str] = dataclasses.field(default=None)
+    usage_operation: T.Optional[str] = dataclasses.field(default=None)
+    usage_operation_update_time: T.Optional[datetime] = dataclasses.field(default=None)
+    current_instance_boot_mode: T.Optional[str] = dataclasses.field(default=None)
     ipv6_address: T.Optional[str] = dataclasses.field(default=None)
     tags: T.Dict[str, str] = dataclasses.field(default_factory=dict)
     data: T.Dict[str, T.Any] = dataclasses.field(default_factory=dict)
 
     @classmethod
     def from_dict(cls, dct: dict) -> "Ec2Instance":
         """
@@ -100,26 +129,44 @@
         Ref:
 
         - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/client/describe_instances.html
         """
         return cls(
             id=dct["InstanceId"],
             status=dct["State"]["Name"],
+            status_transition_reason=dct.get("StateTransitionReason"),
             public_ip=dct.get("PublicIpAddress"),
             private_ip=dct.get("PrivateIpAddress"),
             public_dns_name=dct.get("PublicDnsName"),
             private_dns_name=dct.get("PrivateDnsName"),
             vpc_id=dct.get("VpcId"),
             subnet_id=dct.get("SubnetId"),
             security_groups=dct.get("SecurityGroups", []),
             image_id=dct.get("ImageId"),
+            platform=dct.get("Platform"),
+            platform_details=dct.get("PlatformDetails"),
             instance_type=dct.get("InstanceType"),
+            launch_time=dct.get("LaunchTime"),
             key_name=dct.get("KeyName"),
             architecture=dct.get("Architecture"),
+            ebs_optimized=dct.get("EbsOptimized"),
+            ena_support=dct.get("EnaSupport"),
             hypervisor=dct.get("Hypervisor"),
+            iam_instance_profile_arn=dct.get("IamInstanceProfile", {}).get("Arn"),
+            iam_instance_profile_id=dct.get("IamInstanceProfile", {}).get("Id"),
+            instance_lifecycle=dct.get("InstanceLifecycle"),
+            root_device_name=dct.get("RootDeviceName"),
+            root_device_type=dct.get("RootDeviceType"),
+            spot_instance_request_id=dct.get("SpotInstanceRequestId"),
+            sriov_net_support=dct.get("SriovNetSupport"),
+            virtualization_type=dct.get("VirtualizationType"),
+            boot_mode=dct.get("BootMode"),
+            usage_operation=dct.get("UsageOperation"),
+            usage_operation_update_time=dct.get("UsageOperationUpdateTime"),
+            current_instance_boot_mode=dct.get("CurrentInstanceBootMode"),
             ipv6_address=dct.get("Ipv6Address"),
             tags={kv["Key"]: kv["Value"] for kv in dct.get("Tags", [])},
             data=dct,
         )
 
     def is_pending(self) -> bool:
         """ """
@@ -142,30 +189,38 @@
         return self.status == EC2InstanceStatusEnum.stopping.value
 
     def is_stopped(self) -> bool:
         """ """
         return self.status == EC2InstanceStatusEnum.stopped.value
 
     def is_ready_to_stop(self) -> bool:
-        """ """
+        """
+        Check if EC2 instance is ready to stop.
+        """
         return self.is_running() is True
 
     def is_ready_to_start(self) -> bool:
-        """ """
+        """
+        Check if EC2 instance is ready to start.
+        """
         return self.is_stopped() is True
 
     def start_instance(self, ec2_client):
-        """ """
+        """
+        Start instance.
+        """
         return ec2_client.start_instances(
             InstanceIds=[self.id],
             DryRun=False,
         )
 
     def stop_instance(self, ec2_client):
-        """ """
+        """
+        Stop instance.
+        """
         return ec2_client.stop_instances(
             InstanceIds=[self.id],
             DryRun=False,
         )
 
     # --------------------------------------------------------------------------
     # more constructor methods
@@ -209,44 +264,51 @@
                 yield from cls._yield_dict_from_describe_instances_response(response)
 
         return Ec2InstanceIterProxy(run())
 
     @classmethod
     def from_id(cls, ec2_client, inst_id: str) -> T.Optional["Ec2Instance"]:
         """
-        TODO: docstring
+        Get ec2 instance details by it's id.
         """
         return cls.query(
             ec2_client=ec2_client,
             instance_ids=[inst_id],
         ).one_or_none()
 
     @classmethod
     def from_ec2_inside(
         cls,
         ec2_client,
     ) -> T.Optional["Ec2Instance"]:  # pragma: no cover
         """
-        TODO: docstring
+        Use ec2 metadata API to get the instance id.
+
+        .. note::
+
+            This function should only be called on an EC2 instance
         """
-        instance_id = get_instance_id()
+        instance_id = cls.get_instance_id()
         return cls.query(
             ec2_client=ec2_client,
             instance_ids=[instance_id],
         ).one()
 
     @classmethod
     def from_tag_key_value(
         cls,
         ec2_client,
         key: str,
         value: T.Union[str, T.Iterable[str]],
     ) -> "Ec2InstanceIterProxy":
         """
-        TODO: docstring
+        Query EC2 Instance by tag key and values.
+
+        :param key: tag key
+        :param value: tag value or values
         """
         if isinstance(value, str):
             values = [value]
         else:
             values = list(value)
         return cls.query(
             ec2_client=ec2_client,
@@ -271,14 +333,50 @@
         return cls.query(
             ec2_client=ec2_client,
             filters=[
                 dict(Name=f"tag:Name", Values=names),
             ],
         )
 
+    # --------------------------------------------------------------------------
+    # Retrieve instance metadata
+    # these methods should only be used within EC2 instance
+    # --------------------------------------------------------------------------
+    @classmethod
+    def get_ami_id(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="ami-id")
+
+    @classmethod
+    def get_instance_id(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="instance-id")
+
+    @classmethod
+    def get_instance_type(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="instance-type")
+
+    @classmethod
+    def get_local_hostname(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="local-hostname")
+
+    @classmethod
+    def get_local_ipv4(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="local-ipv4")
+
+    @classmethod
+    def get_public_hostname(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="public-hostname")
+
+    @classmethod
+    def get_public_ipv4(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="public-ipv4")
+
+    @classmethod
+    def get_security_groups(cls) -> T.List[str]:  # pragma: no cover
+        return _get_metadata(name="security-groups").splitlines()
+
 
 class Ec2InstanceIterProxy(IterProxy[Ec2Instance]):
     """
     Advanced iterator proxy for :class:`Ec2Instance`.
     """
 
 
@@ -321,16 +419,57 @@
 
 class ImageOwnerGroupEnum(str, enum.Enum):
     self = "self"
     amazon = "amazon"
     aws_marketplace = "aws-marketplace"
 
 
+type_to_users: T.Dict[str, T.List[str]] = {
+    "AmazonLinux": ["ec2-user"],
+    "CentOS": ["centos", "ec2-user"],
+    "Debian": ["admin"],
+    "Fedora": ["fedora", "ec2-user"],
+    "RHEL": ["ec2-user", "root"],
+    "SUSE": ["ec2-user", "root"],
+    "Ubuntu": ["ubuntu"],
+    "Oracle": ["ec2-user"],
+    "Bitnami": ["bitnami"],
+    "Other": ["unknown"],
+}
+
+
+class ImageOSTypeEnum(str, enum.Enum):
+    """
+    Reference:
+
+    - Default user name for AMI: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connection-prereqs.html#connection-prereqs-get-info-about-instance
+    """
+
+    AmazonLinux = "AmazonLinux"
+    CentOS = "CentOS"
+    Debian = "Debian"
+    Fedora = "Fedora"
+    RHEL = "RHEL"
+    SUSE = "SUSE"
+    Ubuntu = "Ubuntu"
+    Oracle = "Oracle"
+    Bitnami = "Bitnami"
+    Other = "Other"
+
+    @property
+    def users(self) -> T.List[str]:
+        return type_to_users[self.value]
+
+
 @dataclasses.dataclass
 class Image:
+    """
+    Represent an AMI image.
+    """
+
     id: str = dataclasses.field()
     image_location: T.Optional[str] = dataclasses.field(default=None)
     image_type: T.Optional[str] = dataclasses.field(default=None)
     architecture: T.Optional[str] = dataclasses.field(default=None)
     creation_date: T.Optional[str] = dataclasses.field(default=None)
     public: T.Optional[bool] = dataclasses.field(default=None)
     kernel_id: T.Optional[str] = dataclasses.field(default=None)
@@ -357,15 +496,15 @@
     imds_support: T.Optional[str] = dataclasses.field(default=None)
     tags: T.Dict[str, str] = dataclasses.field(default_factory=dict)
     data: T.Dict[str, T.Any] = dataclasses.field(default_factory=dict)
 
     @classmethod
     def from_dict(cls, dct: dict) -> "Image":
         """
-        Create an EC2 instance object from the ``describe_instances`` API response.
+        Create an AMI Image object from the ``describe_images`` API response.
 
         Ref:
 
         - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/client/describe_images.html
         """
         return cls(
             id=dct["ImageId"],
@@ -442,16 +581,14 @@
 
     def image_root_device_type_is_ebs(self) -> bool:
         return self.root_device_type == ImageRootDeviceTypeEnum.ebs.value
 
     def image_root_device_type_is_instance_store(self) -> bool:
         return self.root_device_type == ImageRootDeviceTypeEnum.instance_store.value
 
-    # class ImageVirtualizationTypeEnum(str, enum.Enum):
-
     def image_virtualization_type_is_hvm(self) -> bool:
         return self.virtualization_type == ImageVirtualizationTypeEnum.hvm.value
 
     def image_virtualization_type_is_paravirtual(self) -> bool:
         return self.virtualization_type == ImageVirtualizationTypeEnum.paravirtual.value
 
     def image_boot_mode_is_legacy_bios(self) -> bool:
@@ -459,14 +596,109 @@
 
     def image_boot_mode_is_uefi(self) -> bool:
         return self.boot_mode == ImageBootModeEnum.uefi.value
 
     def image_boot_mode_is_uefi_preferred(self) -> bool:
         return self.boot_mode == ImageBootModeEnum.uefi_preferred.value
 
+    @property
+    def os_type(self) -> ImageOSTypeEnum:  # pragma: no cover
+        """
+        Try to use the image name and description to determine the OS type.
+
+        If the OS type cannot be determined, raise :class:`CannotDetectOSTypeError`.
+        """
+        if self.name.startswith("al"):
+            if self.description is not None:
+                if self.description.startswith("Amazon Linux"):
+                    return ImageOSTypeEnum.AmazonLinux
+        elif self.name.startswith("ubuntu"):
+            if self.description is not None:
+                if "Ubuntu" in self.description:
+                    return ImageOSTypeEnum.Ubuntu
+        elif self.name.startswith("RHEL"):
+            if self.description is not None:
+                if self.description.startswith("RHEL"):
+                    return ImageOSTypeEnum.RHEL
+        elif self.name.startswith("debian"):
+            if self.description is not None:
+                if self.description.startswith("Debian"):
+                    return ImageOSTypeEnum.Debian
+        elif self.name.startswith("suse"):
+            if self.description is not None:
+                if self.description.startswith("SUSE"):
+                    return ImageOSTypeEnum.SUSE
+        elif "fedora" in self.name.lower():
+            if self.description is not None:
+                if "fedora" in self.description.lower():
+                    return ImageOSTypeEnum.Fedora
+        elif "centos" in self.name.lower():
+            if self.description is not None:
+                if "centos" in self.description.lower():
+                    return ImageOSTypeEnum.CentOS
+        elif "oracle" in self.name.lower():
+            if self.description is not None:
+                if "oracle" in self.description.lower():
+                    return ImageOSTypeEnum.Oracle
+        elif "bitnami" in self.name.lower():
+            if self.description is not None:
+                if "bitnami" in self.description.lower():
+                    return ImageOSTypeEnum.Bitnami
+        else:
+            raise CannotDetectOSTypeError
+
+    def is_amazon_linux_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.AmazonLinux
+
+    def is_cent_os_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.CentOS
+
+    def is_debian_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.Debian
+
+    def is_fedora_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.Fedora
+
+    def is_rhel_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.RHEL
+
+    def is_suse_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.SUSE
+
+    def is_ubuntu_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.Ubuntu
+
+    def is_oracle_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.Oracle
+
+    def is_bitnami_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.Bitnami
+
+    def is_other_os(self) -> bool:  # pragma: no cover
+        """"""
+        return self.os_type is ImageOSTypeEnum.Other
+
+    @property
+    def users(self) -> T.List[str]:
+        """
+        Return the potential default user names for the Image. It try to use
+        the image name and description to determine the OS type.
+        If the OS type cannot be determined, raise :class:`CannotDetectOSTypeError`.
+        """
+        return self.os_type.users
+
     # --------------------------------------------------------------------------
     # more constructor methods
     # --------------------------------------------------------------------------
     @classmethod
     def _yield_dict_from_describe_images_response(
         cls,
         res: dict,
@@ -530,15 +762,18 @@
     def from_tag_key_value(
         cls,
         ec2_client,
         key: str,
         value: T.Union[str, T.Iterable[str]],
     ) -> "ImageIterProxy":
         """
-        TODO: docstring
+        Query AMI Image by tag key and values.
+
+        :param key: tag key
+        :param value: tag value or values
         """
         if isinstance(value, str):
             values = [value]
         else:
             values = list(value)
         return cls.query(
             ec2_client=ec2_client,
@@ -564,12 +799,27 @@
         return cls.query(
             ec2_client=ec2_client,
             filters=[
                 dict(Name="name", Values=names),
             ],
         )
 
+    @classmethod
+    def from_ec2_inside(
+        cls,
+        ec2_client,
+    ) -> T.Optional["Image"]:  # pragma: no cover
+        """
+        Use ec2 metadata API to get the instance id, then get the image details
+
+        .. note::
+
+            This function should only be called on an EC2 instance
+        """
+        ec2_inst = Ec2Instance.from_ec2_inside(ec2_client=ec2_client)
+        return cls.from_id(ec2_client=ec2_client, image_id=ec2_inst.image_id)
+
 
 class ImageIterProxy(IterProxy[Image]):
     """
     Advanced iterator proxy for :class:`Image`.
     """
```

### Comparing `simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/PKG-INFO` & `simple_aws_ec2-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: simple-aws-ec2
-Version: 0.2.1
+Name: simple_aws_ec2
+Version: 0.3.1
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -81,33 +81,36 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/simple_aws_ec2#files
 
 
 Welcome to ``simple_aws_ec2`` Documentation
 ==============================================================================
+Simple AWS EC2 dev tool.
+
+Requires Python3.7+
 
 Usage:
 
 .. code-block:: python
 
-    from simple_aws_ec2 import Ec2Instance
-    from boto_session_manager import BotoSesManager
+    import boto3
+    from simple_aws_ec2.api import Ec2Instance, Image
 
-    bsm = BotoSesManager()
+    ec2_client = boto3.client("ec2")
 
     # get ec2 by id
-    ec2_inst = Ec2Instance.from_id(bsm, "i-1a2b3c")
+    ec2_inst = Ec2Instance.from_id(ec2_client, "i-1a2b3c")
     # get ec2 by running code from inside of ec2
-    ec2_inst = EC2Instance.from_ec2_inside(bsm)
+    ec2_inst = EC2Instance.from_ec2_inside(ec2_client)
     # get ec2 by it's name, it returns a iter proxy that may have multiple ec2
-    ec2_inst = EC2Instance.from_ec2_name(bsm, "my-server").one_or_none()
+    ec2_inst = EC2Instance.from_ec2_name(ec2_client, "my-server").one_or_none()
     # get ec2 by tag key value pair, it returns a iter proxy that may have multiple ec2
-    ec2_inst = EC2Instance.from_tag_key_value(bsm, key="Env", value="prod").one_or_none()
-    ec2_inst = EC2Instance.query(bsm, filters=..., instnace_ids=...).all()
+    ec2_inst = EC2Instance.from_tag_key_value(ec2_client, key="Env", value="prod").one_or_none()
+    ec2_inst = EC2Instance.query(ec2_client, filters=..., instnace_ids=...).all()
 
     print(ec2_inst.id)
     print(ec2_inst.status)
     print(ec2_inst.public_ip)
     print(ec2_inst.private_ip)
     print(ec2_inst.vpc_id)
     print(ec2_inst.subnet_id)
@@ -124,14 +127,56 @@
     print(ec2_inst.is_shutting_down()
     print(ec2_inst.is_stopping()
     print(ec2_inst.is_terminated()
 
     print(ec2_inst.is_ready_to_start()
     print(ec2_inst.is_ready_to_stop()
 
+    # the following methods has to be called on a running ec2 instance
+    # it use the EC2 metadata api
+    # https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-data-retrieval.html
+    print(EC2Instance.get_ami_id())
+    print(EC2Instance.get_instance_id())
+    print(EC2Instance.get_instance_type())
+    print(EC2Instance.get_local_hostname())
+    print(EC2Instance.get_local_ipv4())
+    print(EC2Instance.get_public_hostname())
+    print(EC2Instance.get_public_ipv4())
+    print(EC2Instance.get_security_groups()
+
+    # AMI Image API
+    image = Image.from_id(ec2_client, "ami-1a2b3c")
+    image = Image.from_ec2_inside(ec2_client)
+
+    image_list = Image.query(ec2_client).all()
+
+    image_list = Image.query(ec2_client, owners=["self"]).all()
+
+    print(image.image_type_is_machine())
+    print(image.image_type_is_kernel())
+    print(image.image_type_is_ramdisk())
+    print(image.is_pending())
+    print(image.is_available())
+    print(image.is_invalid())
+    print(image.is_deregistered())
+    print(image.is_transient())
+    print(image.is_failed())
+    print(image.is_error())
+    print(image.image_root_device_type_is_ebs())
+    print(image.image_root_device_type_is_instance_store())
+    print(image.image_virtualization_type_is_hvm())
+    print(image.image_virtualization_type_is_paravirtual())
+    print(image.image_boot_mode_is_legacy_bios())
+    print(image.image_boot_mode_is_uefi())
+    print(image.image_boot_mode_is_uefi_preferred())
+
+    image = Image.from_image_name(ec2_client, "my-image").all()
+
+    image_list = Image.from_tag_key_value(ec2_client, key="Env", value="dev").all()
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``simple_aws_ec2`` is released on PyPI, so all you need is:
```

### Comparing `simple_aws_ec2-0.2.1/tests/test_ec2.py` & `simple_aws_ec2-0.3.1/tests/test_ec2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # -*- coding: utf-8 -*-
 
 import os
 import pytest
 import moto
 from boto_session_manager import BotoSesManager
 
-from simple_aws_ec2.ec2 import Ec2Instance, Image, ImageOwnerGroupEnum
+from simple_aws_ec2.ec2 import (
+    Ec2Instance,
+    Image,
+    ImageOwnerGroupEnum,
+    ImageOSTypeEnum,
+)
 
 
 class TestEc2:
     mock_ec2 = None
     bsm: BotoSesManager = None
 
     @classmethod
@@ -178,14 +183,20 @@
         ).all()
         for image_list in [image_list_1, image_list_2]:
             assert len(image_list) == 1
             image = image_list[0]
             assert image.id == self.image_id_1
             assert image.tags["Env"] == "dev"
 
+        image = Image.from_id(self.bsm.ec2_client, self.image_id_1)
+        image.name = "ubuntu"
+        image.description = "Ubuntu"
+        assert image.os_type is ImageOSTypeEnum.Ubuntu
+        assert "ubuntu" in image.users
+
     def test(self):
         self._test_ec2()
         self._test_ec2_start_and_stop()
         self._test_image()
 
 
 if __name__ == "__main__":
```

