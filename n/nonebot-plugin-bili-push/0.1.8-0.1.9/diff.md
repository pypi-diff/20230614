# Comparing `tmp/nonebot_plugin_bili_push-0.1.8.tar.gz` & `tmp/nonebot_plugin_bili_push-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bili_push-0.1.8.tar", last modified: Wed Jun 14 06:38:30 2023, max compression
+gzip compressed data, was "nonebot_plugin_bili_push-0.1.9.tar", last modified: Wed Jun 14 13:16:03 2023, max compression
```

## Comparing `nonebot_plugin_bili_push-0.1.8.tar` & `nonebot_plugin_bili_push-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:38:30.748955 nonebot_plugin_bili_push-0.1.8/
--rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      268 2023-06-14 06:38:30.747956 nonebot_plugin_bili_push-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1694 2023-06-14 03:27:08.000000 nonebot_plugin_bili_push-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:38:30.736955 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push/
--rw-rw-rw-   0        0        0    98887 2023-06-14 06:16:44.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:38:30.745954 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/
--rw-rw-rw-   0        0        0      268 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-14 06:38:30.000000 nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:38:30.749954 nonebot_plugin_bili_push-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-06-14 06:38:18.000000 nonebot_plugin_bili_push-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:16:03.575147 nonebot_plugin_bili_push-0.1.9/
+-rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      268 2023-06-14 13:16:03.574145 nonebot_plugin_bili_push-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2023-06-14 09:01:11.000000 nonebot_plugin_bili_push-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 13:16:03.562143 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push/
+-rw-rw-rw-   0        0        0    99347 2023-06-14 12:59:20.000000 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:16:03.572145 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-06-14 13:16:03.000000 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-14 13:16:03.000000 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:16:03.000000 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-06-14 13:16:03.000000 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-14 13:16:03.000000 nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 13:16:03.575147 nonebot_plugin_bili_push-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-06-14 13:15:41.000000 nonebot_plugin_bili_push-0.1.9/setup.py
```

### Comparing `nonebot_plugin_bili_push-0.1.8/LICENSE` & `nonebot_plugin_bili_push-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.8/README.md` & `nonebot_plugin_bili_push-0.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 
 ## 安装
 （以下方法三选一）
 
 一.命令行安装：
 
     nb plugin install nonebot-plugin-bili-push
- 二.使用插件文件安装：（不推荐）
- 1.下载插件文件，放到plugins文件夹。
+ 二.使用插件文件安装：（不推荐） 
+ 
+1.下载插件文件，放到plugins文件夹。
+
 2.修改pyproject.toml使其可以加载插件
 
 三.pip安装：（不推荐）
 1.执行此命令
 
     pip install nonebot-plugin-bili-push
 2.修改pyproject.toml使其可以加载插件
 
     plugins = [”nonebot-plugin-bili-push“]
  
 ## 配置
 在 nonebot2 项目的`.env`文件中选填配置
+
 配置管理员账户，只有管理员才能添加订阅
 
     SUPERUSERS=["12345678"] # 配置 NoneBot 超级用户
 插件数据存放位置，默认为 “./”。
 
     bilipush_basepath="./"
 ## 参考内容
```

### Comparing `nonebot_plugin_bili_push-0.1.8/nonebot_plugin_bili_push/__init__.py` & `nonebot_plugin_bili_push-0.1.9/nonebot_plugin_bili_push/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,20 +95,33 @@
 half_text = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U",
              "V", "W", "X", "Y", "Z", "a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p",
              "q", "r", "s", "t", "u", "v", "w", "x", "y", "z", "1", "2", "3", "4", "5", "6", "7", "8", "9", "0", ",",
              ".", "/", "\\", "[", "]", "(", ")", "!", "+", "-", "*", "！", "？", "。", "，", "{", "}", "、", "‘", "“",
              '"', "'", "！", " "]
 
 
+def get_file_path(file_name):
+    file_path = basepath + "cache/file/"
+    if not os.path.exists(file_path):
+        os.makedirs(file_path)
+    file_path += file_name
+    if not os.path.exists(file_path):
+        # 如果文件未缓存，则缓存下来
+        url = apiurl + "/file/" + file_name
+        with open(file_path, "wb") as f, requests.get(url) as res:
+            f.write(res.content)
+    return file_path
+
+
 def get_emoji(emoji):
     cachepath = basepath + "cache/emoji/"
     if not os.path.exists(cachepath):
         os.makedirs(cachepath)
     cachepath = cachepath + emoji + ".png"
-    if not cachepath.exists():
+    if not os.path.exists(cachepath):
         if use_api:
             url = apiurl + "/api/emoji?imageid=" + emoji
             try:
                 return_image = requests.get(url)
                 return_image = Image.open(BytesIO(return_image.content))
                 return_image.save(cachepath)
             except:
@@ -287,15 +300,15 @@
 
     return image_background
 
 
 def draw_text(text: str,
               size: int,
               textlen: int = 20,
-              fontfile: str = "./font/腾祥嘉丽中圆.ttf",
+              fontfile: str = get_file_path("腾祥嘉丽中圆.ttf"),
               biliemoji_infos=None,
               draw_qqemoji=False,
               calculate=False
               ):
     """
     - 文字转图片
 
@@ -453,15 +466,15 @@
         bilidata = json.loads(bilidata)
         try:
             emoji_infos = data["display"]["emoji_info"]["emoji_details"]
         except:
             emoji_infos = []
 
         fortsize = 30
-        fontfile = './font/腾祥嘉丽中圆.ttf'
+        fontfile = get_file_path("腾祥嘉丽中圆.ttf")
         font = ImageFont.truetype(font=fontfile, size=fortsize)
 
         # 转发动态
         if bilitype == 1:
             card_message = bilidata["item"]["content"]
             origin_data = bilidata["origin"]
             origin_data = json.loads(origin_data)
@@ -1072,14 +1085,15 @@
                     returnpath = cachepath + 'bili动态/'
                     if not os.path.exists(returnpath):
                         os.makedirs(returnpath)
                     returnpath = returnpath + date + '_' + timenow + '_' + qq + '.png'
                     draw_image.save(returnpath)
                     print("bili-push_绘图成功")
                     code = 2
+
         # 图文动态
         elif bilitype == 2:
             card_message = bilidata["item"]["description"]
             card_images = bilidata["item"]["pictures"]
             images = []
             for card_image in card_images:
                 image_url = card_image["img_src"]
```

### Comparing `nonebot_plugin_bili_push-0.1.8/setup.py` & `nonebot_plugin_bili_push-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         'nonebot_adapter_onebot>=2.2.3',
         'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_bili_push',
-      version='0.1.8',
+      version='0.1.9',
       description='nonebot2 plugin',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_bili_push',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
```

