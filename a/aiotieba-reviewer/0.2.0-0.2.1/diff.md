# Comparing `tmp/aiotieba-reviewer-0.2.0.tar.gz` & `tmp/aiotieba-reviewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotieba-reviewer-0.2.0.tar", last modified: Sat May 20 23:39:46 2023, max compression
+gzip compressed data, was "aiotieba-reviewer-0.2.1.tar", last modified: Wed Jun 14 02:11:46 2023, max compression
```

## Comparing `aiotieba-reviewer-0.2.0.tar` & `aiotieba-reviewer-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.486733 aiotieba-reviewer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-20 23:39:46.486733 aiotieba-reviewer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.478733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/perf_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/punish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/user_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/examples/cmd_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/examples/reviewer_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:39:46.486733 aiotieba-reviewer-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.592177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/perf_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/punish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.592177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/user_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.592177 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/examples/cmd_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/examples/reviewer_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/setup.cfg
```

### Comparing `aiotieba-reviewer-0.2.0/LICENSE` & `aiotieba-reviewer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/README.md` & `aiotieba-reviewer-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,43 +7,61 @@
 + 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
 + 支持针对多条相互关联的内容的审查
 + 支持二维码识别、相似图像查找
 + 支持用户黑白名单、图片黑白名单
 + 使用本地缓存避免重复检测，极大提升性能
 + 优先使用websocket接口，节省带宽
 
-## 安装 (beta)
+## 安装与更新
+
+### 安装 (git)
 
 ```shell
 git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
 cd ./aiotieba-reviewer
 pip install .
 ```
 
+### 更新 (git)
+
+```shell
+git pull
+```
+
+### 安装 (pip)
+
+```shell
+pip install aiotieba-reviewer
+```
+
+### 更新 (pip)
+
+```shell
+pip install -U aiotieba-reviewer
+```
+
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.05.20更新*
+*2023.06.14更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 4,988,625  |      719,584       |    1,314     |   58,553   |
-|     孙笑川     | 4,073,427  |      645,815       |    5,241     |  224,603   |
-|    原神内鬼    |  594,645   |      376,348       |     787      |   28,587   |
-|      憨批      |   17,165   |      125,894       |    3,699     |   62,855   |
-|      禾野      |  363,088   |      106,555       |     966      |   8,602    |
-|    lol半价     | 2,078,647  |       68,593       |     258      |   22,063   |
-|      宫漫      | 1,597,685  |       18,857       |      70      |   1,110    |
-|    天堂鸡汤    |  357,856   |       16,914       |     126      |   4,848    |
-|     vtuber     |  224,576   |       15,538       |     108      |   1,982    |
-|      嘉然      |   61,135   |       10,796       |      76      |    990     |
-|    元气骑士    |  273,274   |       4,298        |      49      |    500     |
-| vtuber自由讨论 |   17,214   |       1,053        |      1       |     13     |
+|    抗压背锅    | 5,067,645  |     1,201,056      |    2,613     |   76,863   |
+|     孙笑川     | 4,192,991  |      663,014       |    5,261     |  217,712   |
+|    原神内鬼    |  602,236   |      379,701       |     735      |   28,531   |
+|      憨批      |   23,131   |      155,320       |    4,012     |   71,069   |
+|    lol半价     | 2,087,686  |       64,620       |     201      |   19,142   |
+|    天堂鸡汤    |  364,725   |       13,804       |     100      |   3,870    |
+|     vtuber     |  225,520   |       11,981       |      77      |    916     |
+|      嘉然      |   61,259   |       8,672        |      60      |    832     |
+|    元气骑士    |  274,123   |       4,216        |      44      |    452     |
+| vtuber自由讨论 |   17,232   |        905         |      1       |     7      |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/client.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/database.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/database.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/executor.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/executor.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/imgproc.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/imgproc.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/perf_stat.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/perf_stat.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/punish.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/punish.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/checker.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/runner.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/producer.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/runner.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/entry.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/entry.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/checker.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/runner.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/producer.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/runner.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/checker.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/runner.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/producer.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/runner.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/user_checker.py` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/user_checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/SOURCES.txt` & `aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/examples/cmd_handler.py` & `aiotieba-reviewer-0.2.1/examples/cmd_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
 
         await self.__cmd_drop(ctx, 10)
 
         note = ctx.args[0] if len(ctx.args) > 0 else ctx.note
 
         await self.__cmd_set(ctx, -5, note, user_id=ctx.parent.author_id)
 
-    @check_and_log(need_permission=4, need_arg_num=0)
+    @check_and_log(need_permission=5, need_arg_num=0)
     async def cmd_avada_kedavra(self, ctx: Context) -> None:
         """
         索命咒
         删帖 清空发帖人主页显示的在当前吧的所有主题帖 加入脚本黑名单+封禁十天
         """
 
         await self.__cmd_drop(ctx, 10)
```

### Comparing `aiotieba-reviewer-0.2.0/examples/reviewer_example.py` & `aiotieba-reviewer-0.2.1/examples/reviewer_example.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.0/pyproject.toml` & `aiotieba-reviewer-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
-dependencies = ["aiotieba[img,speedup]<4.0,>=3.4.0", "aiomysql<0.2,>=0.1.0"]
+dependencies = ["aiotieba[img,speedup]<4.0,>=3.4.0", "aiomysql<0.3,>=0.1.0"]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.dynamic]
 version = { attr = "aiotieba_reviewer.__version__.__version__" }
```

