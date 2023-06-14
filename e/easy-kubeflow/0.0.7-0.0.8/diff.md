# Comparing `tmp/easy-kubeflow-0.0.7.tar.gz` & `tmp/easy-kubeflow-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy-kubeflow-0.0.7.tar", last modified: Mon May 15 10:52:26 2023, max compression
+gzip compressed data, was "dist/easy-kubeflow-0.0.8.tar", last modified: Wed Jun 14 04:37:48 2023, max compression
```

## Comparing `easy-kubeflow-0.0.7.tar` & `easy-kubeflow-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/
--rw-r--r--   0 lwb        (501) staff       (20)      492 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/PKG-INFO
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/
--rw-r--r--   0 lwb        (501) staff       (20)      492 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/PKG-INFO
--rw-r--r--   0 lwb        (501) staff       (20)      476 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/SOURCES.txt
--rw-r--r--   0 lwb        (501) staff       (20)       52 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/requires.txt
--rw-r--r--   0 lwb        (501) staff       (20)       14 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/top_level.txt
--rw-r--r--   0 lwb        (501) staff       (20)        1 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow.egg-info/dependency_links.txt
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/
--rw-r--r--   0 lwb        (501) staff       (20)      122 2021-12-16 02:31:39.000000 easy-kubeflow-0.0.7/easy_kubeflow/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/pipelines/
--rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.0.7/easy_kubeflow/pipelines/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    21172 2023-05-15 10:39:18.000000 easy-kubeflow-0.0.7/easy_kubeflow/pipelines/pipelines_util.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/utils/
--rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.0.7/easy_kubeflow/utils/log_util.py
--rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.0.7/easy_kubeflow/utils/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/examples/
--rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.0.7/easy_kubeflow/examples/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/easy_kubeflow/_docker/
--rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.0.7/easy_kubeflow/_docker/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    22930 2022-12-05 06:17:57.000000 easy-kubeflow-0.0.7/easy_kubeflow/_docker/docker_util.py
--rw-r--r--   0 lwb        (501) staff       (20)     7231 2023-02-27 10:44:37.000000 easy-kubeflow-0.0.7/README.md
--rw-r--r--   0 lwb        (501) staff       (20)      836 2023-05-15 10:45:09.000000 easy-kubeflow-0.0.7/setup.py
--rw-r--r--   0 lwb        (501) staff       (20)       38 2023-05-15 10:52:26.000000 easy-kubeflow-0.0.7/setup.cfg
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/
+-rw-r--r--   0 lwb        (501) staff       (20)      492 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/PKG-INFO
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/
+-rw-r--r--   0 lwb        (501) staff       (20)      492 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/PKG-INFO
+-rw-r--r--   0 lwb        (501) staff       (20)      476 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/SOURCES.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       52 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/requires.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       14 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/top_level.txt
+-rw-r--r--   0 lwb        (501) staff       (20)        1 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/dependency_links.txt
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/
+-rw-r--r--   0 lwb        (501) staff       (20)      122 2021-12-16 02:31:39.000000 easy-kubeflow-0.0.8/easy_kubeflow/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/pipelines/
+-rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.0.8/easy_kubeflow/pipelines/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    21815 2023-06-14 03:54:58.000000 easy-kubeflow-0.0.8/easy_kubeflow/pipelines/pipelines_util.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/utils/
+-rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.0.8/easy_kubeflow/utils/log_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.0.8/easy_kubeflow/utils/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/examples/
+-rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.0.8/easy_kubeflow/examples/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/_docker/
+-rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.0.8/easy_kubeflow/_docker/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    22930 2022-12-05 06:17:57.000000 easy-kubeflow-0.0.8/easy_kubeflow/_docker/docker_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)     7231 2023-02-27 10:44:37.000000 easy-kubeflow-0.0.8/README.md
+-rw-r--r--   0 lwb        (501) staff       (20)      836 2023-06-14 04:37:35.000000 easy-kubeflow-0.0.8/setup.py
+-rw-r--r--   0 lwb        (501) staff       (20)       38 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/setup.cfg
```

### Comparing `easy-kubeflow-0.0.7/easy_kubeflow/pipelines/pipelines_util.py` & `easy-kubeflow-0.0.8/easy_kubeflow/pipelines/pipelines_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -417,26 +417,32 @@
             _logger.warning("Use default gpu limit: 0")
 
 
 # TODO: ReuseComponent use command
 class ReuseComponent(object):
     """definition for reuse pipelines component"""
 
-    def __init__(self, component_factory_func: Callable = None, arguments: Optional[dict] = None,
+    def __init__(self, component_factory_func: Callable = None,
+                 arguments: Optional[dict] = None,
+                 command: Optional[list] = None,
                  nfs_path: str = NFS_PATH,
                  nfs_master_host: str = NFS_MASTER_HOST):
         """
         Reuse component object
         :param component_factory_func: factory func to build reuse component op
+        :param command: [list] args to run component container, default None.
+                        the command to run in the container. If None, uses default CMD
+                        in defined in container.
         :param arguments: [dict] args to run reuse component container, default None
         :param nfs_path: default root path defined by cluster admin
         :param nfs_master_host: default host selected by cluster admin
         """
         self.uuid = str(uuid4())
         self.arguments = arguments
+        self.command = command
         self.factory_func = component_factory_func
         self.nfs_path = nfs_path
         self.nfs_master_host = nfs_master_host
         self.op = self.factory_func(**_uniform_data_path(self.arguments))
 
     @staticmethod
     def _uniform_name(name: str = None):
@@ -451,14 +457,15 @@
         default pipelines component containerOp
         :return: component containerOp
         """
         _logger.info("ReuseComponent op of `%s` init ..." % self._uniform_name(self.factory_func.__name__))
         _logger.info("Container mount path is: %s" % self.nfs_path)
         self._pull_image_policy()
         self._add_volume()
+        self._add_command(self.command)
         return self.op
 
     def udf_op(self, request_cpu: Optional[str] = None, request_mem: Optional[str] = None,
                request_gpu: Optional[str] = None,
                strategies: Optional[list] = None) -> 'dsl.ContainerOp':
         """
         user define pipelines component containerOp
@@ -491,14 +498,24 @@
     def _pull_image_policy(self, policy: str = 'Always'):
         """
         default image pull policy: `Always`
         """
         self.op.container.image_pull_policy = policy
         _logger.info("Use image pull policy: %s" % policy)
 
+    def _add_command(self, command: list = None):
+        """
+        default command: None
+        """
+        if command:
+            self.op.container.command = command
+            _logger.info("Use command: %s" % command)
+        else:
+            _logger.warning("Use default command")
+
     def _add_volume(self):
         """add nfs volume, volume and mount volume has the same path"""
         self.op.add_volume(
             k8s_client.V1Volume(name=self.uuid + '-pv',
                                 nfs=k8s_client.V1NFSVolumeSource(
                                     path=self.nfs_path,
                                     server=self.nfs_master_host
```

### Comparing `easy-kubeflow-0.0.7/easy_kubeflow/utils/log_util.py` & `easy-kubeflow-0.0.8/easy_kubeflow/utils/log_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.7/easy_kubeflow/_docker/docker_util.py` & `easy-kubeflow-0.0.8/easy_kubeflow/_docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.7/README.md` & `easy-kubeflow-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.7/setup.py` & `easy-kubeflow-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = None
 
 setuptools.setup(
     name="easy-kubeflow",  # Replace with your own name
-    version="0.0.7",
+    version="0.0.8",
     author="CrazyBean",
     author_email="liuweibin@stonewise.cn",
     description="sdk help users for a better use of kubeflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://service.stonewise.cn:8029/liuweibin/easy-kubeflow.git",
     install_requires=[
```

