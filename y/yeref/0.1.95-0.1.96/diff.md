# Comparing `tmp/yeref-0.1.95.tar.gz` & `tmp/yeref-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.95.tar", last modified: Tue Jun 13 14:48:24 2023, max compression
+gzip compressed data, was "yeref-0.1.96.tar", last modified: Wed Jun 14 09:34:39 2023, max compression
```

## Comparing `yeref-0.1.95.tar` & `yeref-0.1.96.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:48:24.297967 yeref-0.1.95/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:48:24.298116 yeref-0.1.95/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-13 14:48:24.298731 yeref-0.1.95/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-13 14:48:09.000000 yeref-0.1.95/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:48:24.291248 yeref-0.1.95/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.95/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   551904 2023-06-13 14:47:58.000000 yeref-0.1.95/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210914 2023-06-13 13:35:20.000000 yeref-0.1.95/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:48:24.297587 yeref-0.1.95/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:48:24.000000 yeref-0.1.95/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-13 14:48:24.000000 yeref-0.1.95/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-13 14:48:24.000000 yeref-0.1.95/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-13 14:48:24.000000 yeref-0.1.95/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-14 09:34:39.390853 yeref-0.1.96/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-14 09:34:39.391090 yeref-0.1.96/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-14 09:34:39.392052 yeref-0.1.96/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-14 09:34:35.000000 yeref-0.1.96/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-14 09:34:39.383451 yeref-0.1.96/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.96/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   551845 2023-06-14 09:17:40.000000 yeref-0.1.96/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210936 2023-06-14 09:33:51.000000 yeref-0.1.96/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-14 09:34:39.390151 yeref-0.1.96/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.95/setup.py` & `yeref-0.1.96/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.95',
+      version='0.1.96',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.92-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.96-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.95/yeref/l_.py` & `yeref-0.1.96/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -2002,15 +2002,15 @@
     'en': "👩🏽‍💻 <b>Attach</b> .jpg/.png/.gif/.mp4 content to create a link",
     'es': "👩🏽‍💻 <b>Adjunte</b> contenido .jpg/.png/.gif/.mp4 para crear un enlace",
     'fr': "👩🏽‍💻 <b>Joignez</b> du contenu .jpg/.png/.gif/.mp4 pour créer un lien",
     'zh': "👩🏽‍💻<b>附加</b>.jpg/.png/.gif/.mp4 内容以创建链接",
     'ar': "👩🏽‍💻 <b>أرفق</b> محتوى .jpg / .png / .gif / .mp4 لإنشاء ارتباط",
 }
 l_telegraph_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> получения ссылки (попробуй позже ии загрузи другой файл)",
+    'ru': "👩🏽‍💻 <b>Ошибка</b> получения ссылки (попробуй позже или загрузи другой файл)",
     'en': "👩🏽‍💻 <b>Failed</b> to get link (try later and upload another file)",
     'es': "👩🏽‍💻 <b>No se pudo</b> obtener el enlace (intente más tarde y cargue otro archivo)",
     'fr': "👩🏽‍💻 <b>Échec</b> de l'obtention du lien (essayez plus tard et téléchargez un autre fichier)",
     'zh': "👩🏽‍💻 获取链接<b>失败</b>（稍后再试并上传另一个文件）",
     'ar': "👩🏽‍💻 <b>فشل</b> الحصول على الرابط (حاول لاحقًا وقم بتحميل ملف آخر)",
 }
 l_json_text = {
@@ -2439,15 +2439,15 @@
     'en': "🕵️ Competitors",
     'es': "🕵️ Competidores",
     'fr': "🕵️ Concurrents",
     'zh': "🕵️ 参赛者",
     'ar': "🕵️ المنافسون",
 }
 l_find_bot = {
-    'ru': "🫥 Tg-боты",
+    'ru': "🫥 Боты",
     'en': "🫥 Tg bots",
     'es': "🫥Tg bots",
     'fr': "🫥 Robots Tg",
     'zh': "🫥 Tg 机器人",
     'ar': "🫥 Tg bots",
 }
 
@@ -2716,48 +2716,48 @@
     'en': "🔎 Add your channel/group/user/bot to the database with the command: /add ССЫЛКА\n\n👩🏽‍💻 Conditions: availability of an avatar and @username /link (+ for channel/group > 100 members + last message < 100 days ago + for the bot and the user, the presence of a description)",
     'es': "🔎 Agregue su canal/grupo/usuario/bot a la base de datos con el comando: /add ССЫЛКА\n\n👩🏽‍💻 Condiciones: disponibilidad de un avatar y @username /link (+ para canal/grupo > 100 miembros + último mensaje < hace 100 días + para el bot y el usuario, la presencia de una descripción)",
     'fr': "🔎 Ajoutez votre chaîne/groupe/utilisateur/bot à la base de données avec la commande : /add ССЫЛКА\n\n👩🏽‍💻 Conditions : disponibilité d'un avatar et @username /link (+ pour chaîne/groupe > 100 membres + dernier message il y a < 100 jours + pour le bot et l'utilisateur, la présence d'une description)",
     'zh': "🔎 使用以下命令将您的频道/组/用户/机器人添加到数据库： /add ССЫЛКА\n\n👩🏽‍💻 条件：头像和@username /link 的可用性（+ 对于频道/组 > 100 个成员 + 最后一个消息 < 100 天前 + 对于机器人和用户，存在描述）",
     'ar': "🔎 أضف قناتك / مجموعتك / مستخدم / بوت إلى قاعدة البيانات بالأمر: /add ССЫЛКА\n\n👩🏽‍💻 الشروط: توفر الصورة الرمزية و @username / الرابط (+ للقناة / المجموعة> 100 عضو + الأخير رسالة <100 يوم مضت + للبوت والمستخدم ، وجود وصف)",
 }
 l_add_join_err = {
-    'ru': "🚫 <b>Добавить</b> в базу {0} не удалось, необходимо открыть свободный доступ для присоединения",
+    'ru': "👩🏽‍💻 <b>Ошибка</b> (вставь корректную ссылку или повтори позже)",
     'en': "🚫 Failed to add {0} to the database, you need to open free access to join",
     'es': "🚫 No se pudo agregar {0} a la base de datos, debe abrir el acceso gratuito para unirse",
     'fr': "🚫 Échec de l'ajout de {0} à la base de données, vous devez ouvrir un accès gratuit pour rejoindre",
     'zh': "🚫 添加{0}到数据库失败，需要开通免费权限才能加入",
     'ar': "🚫 فشل إضافة {0} إلى قاعدة البيانات ، تحتاج إلى فتح وصول مجاني للانضمام",
 }
 
 l_add_chn_fail = {
-    'ru': "🚫 <b>Канал</b> {0} - не добавлен в базу\n\n{1} аватар\n{2} >100 подписчиков\n{3} последний пост <100 дней назад",
+    'ru': "🚫 <b>Канал</b> {0} не добавлен в базу\n\n{1} аватар\n{2} >{4} подписчиков\n{3} последний пост <{5} дней назад",
     'en': "🚫 Channel {0} - not added to the database\n\n{1} avatar\n{2} >100 subscribers\n{3} last post <100 days ago",
     'es': "🚫 Canal {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 suscriptores\n{3} última publicación <100 días atrás",
     'fr': "🚫 Chaîne {0} - non ajoutée à la base de données\n\n{1} avatar\n{2} >100 abonnés\n{3} dernier message il y a <100 jours",
     'zh': "🚫 频道 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 个订阅者\n{3} 上次发布 <100 天前",
     'ar': "🚫 القناة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 مشترك\n{3} آخر مشاركة قبل أقل من 100 يوم",
 }
 l_add_grp_fail = {
-    'ru': "🚫 <b>Группа</b> {0} - не добавлена в базу\n\n{1} аватар\n{2} >100 участников\n{3} последний пост <100 дней назад",
+    'ru': "🚫 <b>Группа</b> {0} не добавлена в базу\n\n{1} аватар\n{2} >{4} участников\n{3} последний пост <{5} дней назад",
     'en': "🚫 Group {0} - not added to the database\n\n{1} avatar\n{2} >100 members\n{3} last post <100 days ago",
     'es': "🚫 Grupo {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 miembros\n{3} última publicación <100 días atrás",
     'fr': "🚫 Groupe {0} - non ajouté à la base de données\n\n{1} avatar\n{2} >100 membres\n{3} dernier message il y a <100 jours",
     'zh': "🚫 组 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 名成员\n{3} 上次发帖 <100 天前",
     'ar': "🚫 المجموعة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 عضو\n{3} آخر مشاركة منذ أقل من 100 يوم",
 }
 l_add_usr_fail = {
-    'ru': "🚫 <b>Пользователь</b> {0} - не добавлен в базу\n\n{1} аватар\n{2} @username\n{3} био",
+    'ru': "🚫 <b>Пользователь</b> {0} не добавлен в базу\n\n{1} аватар\n{2} @username\n{3} био",
     'en': "🚫 User {0} - not added to database\n\n{1} avatar\n{2} @username\n{3} bio",
     'es': "🚫 Usuario {0}: no agregado a la base de datos\n\n{1} avatar\n{2} @username\n{3} biografía",
     'fr': "🚫 Utilisateur {0} - non ajouté à la base de données\n\n{1} avatar\n{2} @username\n{3} bio",
     'zh': "🚫 用户 {0} - 未添加到数据库\n\n{1} 头像\n{2} @username\n{3} 简介",
     'ar': "🚫 المستخدم {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} @username\n{3} السيرة الذاتية",
 }
 l_add_bot_fail = {
-    'ru': "🚫 <b>Бот</b> {0} - не добавлен в базу\n\n{1} аватар\n{2} описание",
+    'ru': "🚫 <b>Бот</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание",
     'en': "🚫 Bot {0} - not added to the database\n\n{1} avatar\n{2} description",
     'es': "🚫 Bot {0} - no agregado a la base de datos\n\n{1} avatar\n{2} descripción",
     'fr': "🚫 Bot {0} - non ajouté à la base de données\n\n{1} description de l'avatar\n{2}",
     'zh': "🚫 机器人 {0} - 未添加到数据库\n\n{1} 头像\n{2} 描述",
     'ar': "🚫 بوت {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} الوصف",
 }
```

### Comparing `yeref-0.1.95/yeref/yeref.py` & `yeref-0.1.96/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -3231,25 +3231,25 @@
         max_dt = datetime.datetime(2020, 1, 1)
         arr = [it for it in os.listdir(EXTRA_D) if it.startswith('debug.') and it != 'debug.log']
 
         for item in arr:
             parts = item.split('.')
             if len(parts) <= 2: continue
             parts_dt = parts[1].split('_')
-            cur_dt = datetime.datetime.strptime(f"{parts_dt[0]}_{parts_dt[1]}", '%d-%m-%Y_%H-%M-%S')
+            cur_dt = datetime.datetime.strptime(f"{parts_dt[0]}_{parts_dt[1]}", '%Y-%m-%d_%H-%M-%S')
 
             if cur_dt > max_dt:
                 max_dt = cur_dt
 
         for item in arr:
             file_item = os.path.join(EXTRA_D, item)
             parts = item.split('.')
             if len(parts) <= 2: continue
             parts_dt = parts[1].split('_')
-            cur_dt = datetime.datetime.strptime(f"{parts_dt[0]}_{parts_dt[1]}", '%d-%m-%Y_%H-%M-%S')
+            cur_dt = datetime.datetime.strptime(f"{parts_dt[0]}_{parts_dt[1]}", '%Y-%m-%d_%H-%M-%S')
 
             if cur_dt < max_dt and os.path.exists(file_item):
                 os.remove(file_item)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
@@ -4759,24 +4759,24 @@
 
 
 # region payment
 async def update_subscribe(bot, BASE_D):
     try:
         dt_ = datetime.datetime.utcnow()
         if not (dt_.hour % 2 == 0 and dt_.minute % 2 == 0 and dt_.second % 2 == 0): return
-        sql = "SELECT USER_TID, USER_LZ, USER_DTPAID FROM USER WHERE USER_ISPAID=1"
+        sql = "SELECT USER_TID, USER_LZ, USER_DTPAID, USER_ISPAID FROM USER"
         data = await db_select(sql, (), BASE_D)
 
         for item in data:
             try:
-                await asyncio.sleep(round(random.uniform(0, 1), 2))
-                USER_TID, USER_LZ, USER_DTPAID = item
+                await asyncio.sleep(round(random.uniform(1, 2), 2))
+                USER_TID, USER_LZ, USER_DTPAID, USER_ISPAID = item
                 get_ = await bot.get_chat(chat_id=USER_TID)
 
-                if USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
+                if USER_ISPAID and USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
                     chan_private_donate = channel_library_ru if USER_LZ == 'ru' else channel_library_en
                     extra_bot = Bot(token=BOT_TOKEN_E18B)
                     get_chat_member_ = await extra_bot.get_chat_member(chat_id=chan_private_donate, user_id=USER_TID)
                     await extra_bot.session.close()
 
                     if get_chat_member_.status in ['member', 'administrator', 'creator']:
                         USER_DTPAID = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S')
```

