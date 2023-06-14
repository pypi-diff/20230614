# Comparing `tmp/knifes-0.8.8.tar.gz` & `tmp/knifes-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knifes-0.8.8.tar", last modified: Thu Nov  3 11:10:57 2022, max compression
+gzip compressed data, was "knifes-0.8.9.tar", last modified: Thu Nov  3 11:19:21 2022, max compression
```

## Comparing `knifes-0.8.8.tar` & `knifes-0.8.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:10:57.984531 knifes-0.8.8/
--rw-r--r--   0 hwei       (501) staff       (20)      765 2022-11-03 11:10:57.984400 knifes-0.8.8/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.8/README.md
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:10:57.983707 knifes-0.8.8/knifes/
--rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.8/knifes/__init__.py
--rw-r--r--   0 hwei       (501) staff       (20)      134 2022-08-09 07:31:37.000000 knifes-0.8.8/knifes/_settings.py
--rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.8/knifes/aes.py
--rw-r--r--   0 hwei       (501) staff       (20)      606 2022-08-09 10:00:32.000000 knifes-0.8.8/knifes/alarm.py
--rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.8/knifes/auth.py
--rw-r--r--   0 hwei       (501) staff       (20)      487 2022-02-16 01:56:36.000000 knifes-0.8.8/knifes/constants.py
--rw-r--r--   0 hwei       (501) staff       (20)     6160 2022-08-31 09:51:36.000000 knifes-0.8.8/knifes/decorators.py
--rw-r--r--   0 hwei       (501) staff       (20)     5192 2022-11-03 11:09:52.000000 knifes-0.8.8/knifes/deploy.py
--rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.8/knifes/digests.py
--rw-r--r--   0 hwei       (501) staff       (20)      368 2022-09-25 02:42:32.000000 knifes-0.8.8/knifes/envconfig.py
--rw-r--r--   0 hwei       (501) staff       (20)      200 2022-01-21 03:14:54.000000 knifes-0.8.8/knifes/file.py
--rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.8/knifes/jsons.py
--rw-r--r--   0 hwei       (501) staff       (20)      559 2022-09-25 02:41:33.000000 knifes-0.8.8/knifes/logging.py
--rw-r--r--   0 hwei       (501) staff       (20)      849 2022-07-04 09:50:15.000000 knifes-0.8.8/knifes/misc.py
--rw-r--r--   0 hwei       (501) staff       (20)      866 2022-01-21 03:14:54.000000 knifes-0.8.8/knifes/randoms.py
--rw-r--r--   0 hwei       (501) staff       (20)     1792 2022-02-12 10:43:59.000000 knifes-0.8.8/knifes/results.py
--rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.8/knifes/roar.py
--rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.8/knifes/shell.py
--rw-r--r--   0 hwei       (501) staff       (20)     1563 2022-08-09 10:02:01.000000 knifes-0.8.8/knifes/sms.py
--rw-r--r--   0 hwei       (501) staff       (20)      994 2022-10-25 10:02:34.000000 knifes-0.8.8/knifes/strings.py
--rw-r--r--   0 hwei       (501) staff       (20)     1154 2022-01-21 03:14:54.000000 knifes-0.8.8/knifes/times.py
--rw-r--r--   0 hwei       (501) staff       (20)     2714 2022-10-22 06:06:43.000000 knifes-0.8.8/knifes/urls.py
--rw-r--r--   0 hwei       (501) staff       (20)     4333 2022-01-21 03:14:54.000000 knifes-0.8.8/knifes/useragent.py
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:10:57.984248 knifes-0.8.8/knifes.egg-info/
--rw-r--r--   0 hwei       (501) staff       (20)      765 2022-11-03 11:10:57.000000 knifes-0.8.8/knifes.egg-info/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      576 2022-11-03 11:10:57.000000 knifes-0.8.8/knifes.egg-info/SOURCES.txt
--rw-r--r--   0 hwei       (501) staff       (20)        1 2022-11-03 11:10:57.000000 knifes-0.8.8/knifes.egg-info/dependency_links.txt
--rw-r--r--   0 hwei       (501) staff       (20)       27 2022-11-03 11:10:57.000000 knifes-0.8.8/knifes.egg-info/requires.txt
--rw-r--r--   0 hwei       (501) staff       (20)        7 2022-11-03 11:10:57.000000 knifes-0.8.8/knifes.egg-info/top_level.txt
--rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.8/pyproject.toml
--rw-r--r--   0 hwei       (501) staff       (20)       38 2022-11-03 11:10:57.984574 knifes-0.8.8/setup.cfg
--rw-r--r--   0 hwei       (501) staff       (20)      900 2022-11-03 11:10:45.000000 knifes-0.8.8/setup.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:19:21.636872 knifes-0.8.9/
+-rw-r--r--   0 hwei       (501) staff       (20)      765 2022-11-03 11:19:21.636726 knifes-0.8.9/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.9/README.md
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:19:21.635679 knifes-0.8.9/knifes/
+-rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/__init__.py
+-rw-r--r--   0 hwei       (501) staff       (20)      134 2022-08-09 07:31:37.000000 knifes-0.8.9/knifes/_settings.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.9/knifes/aes.py
+-rw-r--r--   0 hwei       (501) staff       (20)      606 2022-08-09 10:00:32.000000 knifes-0.8.9/knifes/alarm.py
+-rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/auth.py
+-rw-r--r--   0 hwei       (501) staff       (20)      487 2022-02-16 01:56:36.000000 knifes-0.8.9/knifes/constants.py
+-rw-r--r--   0 hwei       (501) staff       (20)     6160 2022-08-31 09:51:36.000000 knifes-0.8.9/knifes/decorators.py
+-rw-r--r--   0 hwei       (501) staff       (20)     5201 2022-11-03 11:18:34.000000 knifes-0.8.9/knifes/deploy.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.9/knifes/digests.py
+-rw-r--r--   0 hwei       (501) staff       (20)      368 2022-09-25 02:42:32.000000 knifes-0.8.9/knifes/envconfig.py
+-rw-r--r--   0 hwei       (501) staff       (20)      200 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/file.py
+-rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.9/knifes/jsons.py
+-rw-r--r--   0 hwei       (501) staff       (20)      559 2022-09-25 02:41:33.000000 knifes-0.8.9/knifes/logging.py
+-rw-r--r--   0 hwei       (501) staff       (20)      849 2022-07-04 09:50:15.000000 knifes-0.8.9/knifes/misc.py
+-rw-r--r--   0 hwei       (501) staff       (20)      866 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/randoms.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1792 2022-02-12 10:43:59.000000 knifes-0.8.9/knifes/results.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.9/knifes/roar.py
+-rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/shell.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1563 2022-08-09 10:02:01.000000 knifes-0.8.9/knifes/sms.py
+-rw-r--r--   0 hwei       (501) staff       (20)      994 2022-10-25 10:02:34.000000 knifes-0.8.9/knifes/strings.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1154 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/times.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2714 2022-10-22 06:06:43.000000 knifes-0.8.9/knifes/urls.py
+-rw-r--r--   0 hwei       (501) staff       (20)     4333 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/useragent.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:19:21.636540 knifes-0.8.9/knifes.egg-info/
+-rw-r--r--   0 hwei       (501) staff       (20)      765 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      576 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/SOURCES.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        1 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/dependency_links.txt
+-rw-r--r--   0 hwei       (501) staff       (20)       27 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/requires.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        7 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/top_level.txt
+-rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.9/pyproject.toml
+-rw-r--r--   0 hwei       (501) staff       (20)       38 2022-11-03 11:19:21.636925 knifes-0.8.9/setup.cfg
+-rw-r--r--   0 hwei       (501) staff       (20)      900 2022-11-03 11:19:10.000000 knifes-0.8.9/setup.py
```

### Comparing `knifes-0.8.8/knifes/aes.py` & `knifes-0.8.9/knifes/aes.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/alarm.py` & `knifes-0.8.9/knifes/alarm.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/auth.py` & `knifes-0.8.9/knifes/auth.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/decorators.py` & `knifes-0.8.9/knifes/decorators.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/deploy.py` & `knifes-0.8.9/knifes/deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,33 +104,33 @@
     调用前先在project目录下创建venv环境,如:
     /root/.pyenv/versions/3.7.2/bin/python -m venv venv
     
     gunicorn >= 20.1.0
     在conf文件中配置wsgi_app
     根据app_name加载相应的配置文件
     """
-    install_modules(project_dir)
-
     cmd = f'{project_dir}venv/bin/gunicorn -c {project_dir}gunicorn_{app_name}_conf.py'
     # 判断是否已启动
     succ, err = exec_shell("pgrep -f '{}'".format(cmd))
     if succ:
         print_err('当前已启动！请通过reload命令重启')
         return
 
+    install_modules(project_dir)
+
     ret = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     if ret.returncode != 0:  # 执行失败
         print_err(ret.stderr.decode())
         raise SystemExit
 
     time.sleep(1)
     read_last_log(log_dir, 6)
 
     # 配置开机启动
-    autostart_at_boot(project_dir, app_name)
+    autostart_at_boot(project_dir, log_dir, app_name)
 
 
 def reload_gunicorn(project_dir, log_dir):
     install_modules(project_dir)
 
     pid_file = f'{log_dir}pid.pid'
     pid = read_file(pid_file).strip()
```

### Comparing `knifes-0.8.8/knifes/digests.py` & `knifes-0.8.9/knifes/digests.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/jsons.py` & `knifes-0.8.9/knifes/jsons.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/logging.py` & `knifes-0.8.9/knifes/logging.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/misc.py` & `knifes-0.8.9/knifes/misc.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/randoms.py` & `knifes-0.8.9/knifes/randoms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/results.py` & `knifes-0.8.9/knifes/results.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/roar.py` & `knifes-0.8.9/knifes/roar.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/sms.py` & `knifes-0.8.9/knifes/sms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/strings.py` & `knifes-0.8.9/knifes/strings.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/times.py` & `knifes-0.8.9/knifes/times.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/urls.py` & `knifes-0.8.9/knifes/urls.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes/useragent.py` & `knifes-0.8.9/knifes/useragent.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/knifes.egg-info/SOURCES.txt` & `knifes-0.8.9/knifes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knifes-0.8.8/setup.py` & `knifes-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knifes",
-    version="0.8.8",
+    version="0.8.9",
     author="knifes",
     author_email="author@example.com",
     description="Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     classifiers=[
```

