# Comparing `tmp/hagrid-0.3.8.tar.gz` & `tmp/hagrid-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.8.tar", last modified: Fri May  5 03:25:15 2023, max compression
+gzip compressed data, was "hagrid-0.3.9.tar", last modified: Fri May 12 03:18:06 2023, max compression
```

## Comparing `hagrid-0.3.8.tar` & `hagrid-0.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 03:25:15.429014 hagrid-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-05-05 03:22:19.000000 hagrid-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)   134867 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-05 03:24:13.000000 hagrid-0.3.8/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 03:22:38.000000 hagrid-0.3.8/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:25:15.429014 hagrid-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-05 03:22:38.000000 hagrid-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:22:19.000000 hagrid-0.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:22:19.000000 hagrid-0.3.8/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-05 03:22:19.000000 hagrid-0.3.8/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:18:06.061047 hagrid-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-12 03:18:06.061047 hagrid-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-05-12 03:15:14.000000 hagrid-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:18:06.057047 hagrid-0.3.9/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134898 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-12 03:17:08.000000 hagrid-0.3.9/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 03:15:32.000000 hagrid-0.3.9/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-12 03:15:14.000000 hagrid-0.3.9/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:18:06.057047 hagrid-0.3.9/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-12 03:18:06.000000 hagrid-0.3.9/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-12 03:18:06.000000 hagrid-0.3.9/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 03:18:06.000000 hagrid-0.3.9/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 03:18:06.000000 hagrid-0.3.9/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-12 03:18:06.000000 hagrid-0.3.9/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 03:18:06.000000 hagrid-0.3.9/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 03:18:06.061047 hagrid-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-12 03:15:32.000000 hagrid-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:18:06.057047 hagrid-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:15:14.000000 hagrid-0.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:18:06.061047 hagrid-0.3.9/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:15:14.000000 hagrid-0.3.9/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-12 03:15:14.000000 hagrid-0.3.9/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.8/README.md` & `hagrid-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/__init__.py` & `hagrid-0.3.9/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/art.py` & `hagrid-0.3.9/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/auth.py` & `hagrid-0.3.9/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/azure.py` & `hagrid-0.3.9/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/cache.py` & `hagrid-0.3.9/hagrid/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "gcp_key_path": "~/.ssh/google_compute_engine",
     "gcp_repo": DEFAULT_REPO,
     "gcp_branch": STABLE_BRANCH,
     "install_wizard_complete": False,
     "aws_region": "us-east-1",
     "aws_security_group_name": "openmined_sg",
     "aws_security_group_cidr": "0.0.0.0/0",
-    "aws_image_id": "ami-09cd747c78a9add63",  # Ubuntu Server 20.04 LTS (HVM), SSD Volume Type
+    "aws_image_id": "ami-05de688637f3e33ee",  # Ubuntu Server 22.04 LTS (HVM), SSD Volume Type
     "aws_ec2_instance_type": "t2.xlarge",
     "aws_ec2_instance_username": "ubuntu",  # For Ubuntu AMI, the default user name is ubuntu
     "aws_repo": DEFAULT_REPO,
     "aws_branch": STABLE_BRANCH,
 }
```

### Comparing `hagrid-0.3.8/hagrid/cli.py` & `hagrid-0.3.9/hagrid/cli.py`

 * *Files identical despite different names*

```diff
@@ -97,15 +97,15 @@
 fix_windows_virtualenv_api(VirtualEnvironment)
 
 
 def get_azure_image(short_name: str) -> str:
     prebuild_070 = (
         "madhavajay1632269232059:openmined_mj_grid_domain_ubuntu_1:domain_070:latest"
     )
-    fresh_ubuntu = "Canonical:0001-com-ubuntu-server-focal:20_04-lts:latest"
+    fresh_ubuntu = "Canonical:0001-com-ubuntu-server-jammy:22_04-lts-gen2:latest"
     if short_name == "default":
         return fresh_ubuntu
     elif short_name == "domain_0.7.0":
         return prebuild_070
     raise Exception(f"Image name doesn't exist: {short_name}. Try: default or 0.7.0")
 
 
@@ -1935,15 +1935,15 @@
             generate_sec_random_password(length=48, special_chars=False)
         ),
         "ENABLE_OBLV": str(enable_oblv).lower(),
     }
 
     if "trace" in kwargs and kwargs["trace"] is True:
         envs["TRACE"] = "True"
-        envs["JAEGER_HOST"] = "docker-host"
+        envs["JAEGER_HOST"] = "host.docker.internal"
         envs["JAEGER_PORT"] = int(
             find_available_port(host="localhost", port=14268, search=True)
         )
 
     if "platform" in kwargs and kwargs["platform"] is not None:
         envs["DOCKER_DEFAULT_PLATFORM"] = docker_platform
 
@@ -2580,15 +2580,15 @@
         "https://www.googleapis.com/auth/logging.write",
         "https://www.googleapis.com/auth/monitoring.write",
         "https://www.googleapis.com/auth/servicecontrol",
         "https://www.googleapis.com/auth/service.management.readonly",
         "https://www.googleapis.com/auth/trace.append",
     ]
     tags = "http-server,https-server"
-    disk_image = "projects/ubuntu-os-cloud/global/images/ubuntu-2004-focal-v20220308"
+    disk_image = "projects/ubuntu-os-cloud/global/images/ubuntu-2204-jammy-v20230429"
     disk = (
         f"auto-delete=yes,boot=yes,device-name={vm_name},image={disk_image},"
         + f"mode=rw,size={disk_size_gb},type=pd-ssd"
     )
     security_flags = (
         "--no-shielded-secure-boot --shielded-vtpm "
         + "--shielded-integrity-monitoring --reservation-affinity=any"
@@ -2991,15 +2991,15 @@
         path = grid_path + "/worker"
         env_var = ";export $(cat ../.env | sed 's/#.*//g' | xargs);"
 
     cmd = ""
     cmd += "docker compose"
     cmd += ' --file "docker-compose.yml"'
     cmd += ' --project-name "' + snake_name + '"'
-    cmd += " down"
+    cmd += " down --remove-orphans"
 
     cmd = "cd " + path + env_var + cmd
     return cmd
 
 
 @click.command(
     help="Stop a running PyGrid domain/network node.",
```

### Comparing `hagrid-0.3.8/hagrid/deps.py` & `hagrid-0.3.9/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/grammar.py` & `hagrid-0.3.9/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/land.py` & `hagrid-0.3.9/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/launch.py` & `hagrid-0.3.9/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/lib.py` & `hagrid-0.3.9/hagrid/lib.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/manifest_template.yml` & `hagrid-0.3.9/hagrid/manifest_template.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.8
-syft_version: 0.8.1-beta.0
-dockerTag: 0.8.1-beta.0
+hagrid_version: 0.3.9
+syft_version: 0.8.1-beta.1
+dockerTag: 0.8.1-beta.1
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: d80af183671ff8e27ed7b070f963c93039135fa8
+hash: ea689a53f6c4444f896d071f5aa37f72d3fdfdd1
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
       - rabbitmq/rabbitmq.conf
       - redis/redis.conf
```

### Comparing `hagrid-0.3.8/hagrid/mode.py` & `hagrid-0.3.9/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/names.py` & `hagrid-0.3.9/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/orchestra.py` & `hagrid-0.3.9/hagrid/orchestra.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/parse_template.py` & `hagrid-0.3.9/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/quickstart_ui.py` & `hagrid-0.3.9/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/rand_sec.py` & `hagrid-0.3.9/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/style.py` & `hagrid-0.3.9/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/util.py` & `hagrid-0.3.9/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/win_bootstrap.py` & `hagrid-0.3.9/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid/wizard_ui.py` & `hagrid-0.3.9/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.9/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.8/setup.py` & `hagrid-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=7.1",
     "cryptography>=37.0.2",
```

### Comparing `hagrid-0.3.8/tests/hagrid/cli_test.py` & `hagrid-0.3.9/tests/hagrid/cli_test.py`

 * *Files identical despite different names*

