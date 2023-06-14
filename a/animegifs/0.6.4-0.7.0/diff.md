# Comparing `tmp/animegifs-0.6.4.tar.gz` & `tmp/animegifs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.6.4.tar", last modified: Thu Jun  8 15:56:03 2023, max compression
+gzip compressed data, was "animegifs-0.7.0.tar", last modified: Wed Jun 14 16:36:10 2023, max compression
```

## Comparing `animegifs-0.6.4.tar` & `animegifs-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.451429 animegifs-0.6.4/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.4/LICENSE
--rw-rw-rw-   0        0        0     3869 2023-06-08 15:56:03.450428 animegifs-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-06-08 15:41:36.000000 animegifs-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.427427 animegifs-0.6.4/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.4/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3401 2023-06-08 14:53:25.000000 animegifs-0.6.4/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.448431 animegifs-0.6.4/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.4/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     2331 2023-06-08 15:47:16.000000 animegifs-0.6.4/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     2026 2023-06-08 14:53:25.000000 animegifs-0.6.4/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.438429 animegifs-0.6.4/animegifs.egg-info/
--rw-rw-rw-   0        0        0     3869 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 15:56:03.451429 animegifs-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1282 2023-06-08 14:59:43.000000 animegifs-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.506571 animegifs-0.7.0/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     4084 2023-06-14 16:36:10.505571 animegifs-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3289 2023-06-14 16:25:37.000000 animegifs-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.486569 animegifs-0.7.0/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.7.0/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3739 2023-06-14 16:29:46.000000 animegifs-0.7.0/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.503573 animegifs-0.7.0/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.7.0/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     2331 2023-06-08 15:47:16.000000 animegifs-0.7.0/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1157 2023-06-14 16:22:51.000000 animegifs-0.7.0/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.495570 animegifs-0.7.0/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     4084 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 16:36:10.506571 animegifs-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2023-06-14 16:30:12.000000 animegifs-0.7.0/setup.py
```

### Comparing `animegifs-0.6.4/LICENSE` & `animegifs-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.4/PKG-INFO` & `animegifs-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.6.4
+Version: 0.7.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Classifier: Programming Language :: Python :: 3.8
@@ -54,82 +54,83 @@
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
-**Category list:** 
+## Category list:
 
+**A**
 * Attack
-* Bite
-* Bloodsuck
-* Blush
-* Bonk
-* Brofist
-* Cry
-* Cuddle
-* Dance
-* Disgust
+
+**B**
+* Bite, Bloodsuck, Blush, Bonk, Brofist
+
+**C**
+* Cry, Cuddle
+
+**D**
+* Dance, Disgust
+
+**E**
 * Exploding
-* Facedesk
-* Facepalm
-* Flick
-* Flirt
-* Handhold
-* Happy
-* Harass
-* Highfive
-* Hug
-* Icecream
-* Insult
-* Kill
-* Kiss
-* Lick
-* Love
+
+**F**
+* Facedesk, Facepalm, Flick, Flirt
+
+**H**
+* Handhold, Happy, Harass, Highfive, Hug
+
+**I**
+* Icecream, Insult
+
+**K**
+* Kill, Kiss
+
+**L**
+* Lick, Love
+
+**M**
 * Marry
-* Nod
-* Nosebleed
-* Nuzzle
-* Pat
-* Peck
-* Poke
-* Popcorn
-* Pout
-* Punch
-* Punish
+
+**N**
+* Nod, Nosebleed, Nuzzle
+
+**P**
+* Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
+
+**R**
 * Run
-* Sad
-* Scared
-* Shoot
-* Shrug
-* Sip
-* Slap
-* Smirk
-* Sorry
-* Spank
-* Stare
-* Tease
-* Threat
-* Tickle
-* Tired
+
+**S**
+* Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
+
+**T**
+* Tease, Threat, Tickle, Tired
+
+**W**
 * Wave
+
+**Y**
 * Yawn
 
 **Special Category List**
 
-* Random
-* Steal-magic
+* Random, Steal-magic
+
+# Live API
+
+You can test out the API (and lib functionality) on my bot's website here: https://enkidu-app.github.io/animegifs
 
 # Troubleshooting and other
 
 If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
 Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
 I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
 
 # Copyright
 
 This repository doesn't include any copyrighted material. 
-If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, 
-email me at **grest0grest@gmail.com**. 
+If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, email me at **grest0grest@gmail.com**. 
 Please provide specific details about the copyrighted material and where it can be found.
 Once I confirm your claim, I'll take immediate action to remove the identified material.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.6.4 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.7.0 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
 anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
@@ -15,25 +15,28 @@
 anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
 #return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
 gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
 and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
 anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
 gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` **Category list:** * Attack * Bite * Bloodsuck * Blush *
-Bonk * Brofist * Cry * Cuddle * Dance * Disgust * Exploding * Facedesk *
-Facepalm * Flick * Flirt * Handhold * Happy * Harass * Highfive * Hug *
-Icecream * Insult * Kill * Kiss * Lick * Love * Marry * Nod * Nosebleed *
-Nuzzle * Pat * Peck * Poke * Popcorn * Pout * Punch * Punish * Run * Sad *
-Scared * Shoot * Shrug * Sip * Slap * Smirk * Sorry * Spank * Stare * Tease *
-Threat * Tickle * Tired * Wave * Yawn **Special Category List** * Random *
-Steal-magic # Troubleshooting and other If you encounter an error, please raise
-an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues.
-Alternatively, you can join my Discord server to request new categories,
-functions, provide feedback, or report any errors. I do also have a multi-
-function Discord bot. Feel free to check out the web dashboard here: https://
-enkidu-app.github.io. # Copyright This repository doesn't include any
-copyrighted material. If you happen to come across any copyrighted content
-within this repository (but hosted elsewhere) that you own or represent, email
-me at **grest0grest@gmail.com**. Please provide specific details about the
-copyrighted material and where it can be found. Once I confirm your claim, I'll
-take immediate action to remove the identified material.
+myanimelist page. ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
+Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
+Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
+Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
+Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
+Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, ,Shoot, Shrug,
+Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
+**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
+Live API You can test out the API (and lib functionality) on my bot's website
+here: https://enkidu-app.github.io/animegifs # Troubleshooting and other If you
+encounter an error, please raise an issue on the issue page: https://
+github.com/MarcoSa-2000/animegifs/issues. Alternatively, you can join my
+Discord server to request new categories, functions, provide feedback, or
+report any errors. I do also have a multi-function Discord bot. Feel free to
+check out the web dashboard here: https://enkidu-app.github.io. # Copyright
+This repository doesn't include any copyrighted material. If you happen to come
+across any copyrighted content within this repository (but hosted elsewhere)
+that you own or represent, email me at **grest0grest@gmail.com**. Please
+provide specific details about the copyrighted material and where it can be
+found. Once I confirm your claim, I'll take immediate action to remove the
+identified material.
```

### Comparing `animegifs-0.6.4/README.md` & `animegifs-0.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -34,82 +34,83 @@
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
-**Category list:** 
+## Category list:
 
+**A**
 * Attack
-* Bite
-* Bloodsuck
-* Blush
-* Bonk
-* Brofist
-* Cry
-* Cuddle
-* Dance
-* Disgust
+
+**B**
+* Bite, Bloodsuck, Blush, Bonk, Brofist
+
+**C**
+* Cry, Cuddle
+
+**D**
+* Dance, Disgust
+
+**E**
 * Exploding
-* Facedesk
-* Facepalm
-* Flick
-* Flirt
-* Handhold
-* Happy
-* Harass
-* Highfive
-* Hug
-* Icecream
-* Insult
-* Kill
-* Kiss
-* Lick
-* Love
+
+**F**
+* Facedesk, Facepalm, Flick, Flirt
+
+**H**
+* Handhold, Happy, Harass, Highfive, Hug
+
+**I**
+* Icecream, Insult
+
+**K**
+* Kill, Kiss
+
+**L**
+* Lick, Love
+
+**M**
 * Marry
-* Nod
-* Nosebleed
-* Nuzzle
-* Pat
-* Peck
-* Poke
-* Popcorn
-* Pout
-* Punch
-* Punish
+
+**N**
+* Nod, Nosebleed, Nuzzle
+
+**P**
+* Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
+
+**R**
 * Run
-* Sad
-* Scared
-* Shoot
-* Shrug
-* Sip
-* Slap
-* Smirk
-* Sorry
-* Spank
-* Stare
-* Tease
-* Threat
-* Tickle
-* Tired
+
+**S**
+* Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
+
+**T**
+* Tease, Threat, Tickle, Tired
+
+**W**
 * Wave
+
+**Y**
 * Yawn
 
 **Special Category List**
 
-* Random
-* Steal-magic
+* Random, Steal-magic
+
+# Live API
+
+You can test out the API (and lib functionality) on my bot's website here: https://enkidu-app.github.io/animegifs
 
 # Troubleshooting and other
 
 If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
 Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
 I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
 
 # Copyright
 
 This repository doesn't include any copyrighted material. 
-If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, 
-email me at **grest0grest@gmail.com**. 
+If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, email me at **grest0grest@gmail.com**. 
 Please provide specific details about the copyrighted material and where it can be found.
 Once I confirm your claim, I'll take immediate action to remove the identified material.
```

#### html2text {}

```diff
@@ -7,25 +7,28 @@
 anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
 #return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
 gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
 and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
 anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
 gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` **Category list:** * Attack * Bite * Bloodsuck * Blush *
-Bonk * Brofist * Cry * Cuddle * Dance * Disgust * Exploding * Facedesk *
-Facepalm * Flick * Flirt * Handhold * Happy * Harass * Highfive * Hug *
-Icecream * Insult * Kill * Kiss * Lick * Love * Marry * Nod * Nosebleed *
-Nuzzle * Pat * Peck * Poke * Popcorn * Pout * Punch * Punish * Run * Sad *
-Scared * Shoot * Shrug * Sip * Slap * Smirk * Sorry * Spank * Stare * Tease *
-Threat * Tickle * Tired * Wave * Yawn **Special Category List** * Random *
-Steal-magic # Troubleshooting and other If you encounter an error, please raise
-an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues.
-Alternatively, you can join my Discord server to request new categories,
-functions, provide feedback, or report any errors. I do also have a multi-
-function Discord bot. Feel free to check out the web dashboard here: https://
-enkidu-app.github.io. # Copyright This repository doesn't include any
-copyrighted material. If you happen to come across any copyrighted content
-within this repository (but hosted elsewhere) that you own or represent, email
-me at **grest0grest@gmail.com**. Please provide specific details about the
-copyrighted material and where it can be found. Once I confirm your claim, I'll
-take immediate action to remove the identified material.
+myanimelist page. ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
+Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
+Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
+Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
+Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
+Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, ,Shoot, Shrug,
+Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
+**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
+Live API You can test out the API (and lib functionality) on my bot's website
+here: https://enkidu-app.github.io/animegifs # Troubleshooting and other If you
+encounter an error, please raise an issue on the issue page: https://
+github.com/MarcoSa-2000/animegifs/issues. Alternatively, you can join my
+Discord server to request new categories, functions, provide feedback, or
+report any errors. I do also have a multi-function Discord bot. Feel free to
+check out the web dashboard here: https://enkidu-app.github.io. # Copyright
+This repository doesn't include any copyrighted material. If you happen to come
+across any copyrighted content within this repository (but hosted elsewhere)
+that you own or represent, email me at **grest0grest@gmail.com**. Please
+provide specific details about the copyrighted material and where it can be
+found. Once I confirm your claim, I'll take immediate action to remove the
+identified material.
```

### Comparing `animegifs-0.6.4/animegifs/animegifs.py` & `animegifs-0.7.0/animegifs/animegifs.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,26 @@
                 sorry, spank, stare, steal-magic, tease, threat, tickle, tired, wave, yawn.
 
         Returns:
             gif: gif (url) -> str
         """
         if type(category) is int:
             raise errors.CategoryIntegral(category)
-        if category.lower() in gifs.gifs_name_list:
+        if category.lower() in list(gifs.access().keys()) or category.lower() == 'random':
             if category.lower() == 'random':
                 gif_list = []
                 for key, gif_url in gifs.access().items():
                     for urls in gif_url:
                         gif_list.append(urls[0])
                 gif = gif_list
             else:
                 gifs_list = gifs.access()[category.lower()]
                 gif = [gif_url[0] for gif_url in gifs_list]
             gif = random.choice(gif)
-        elif category.lower() not in gifs.gifs_name_list:
+        elif category.lower() not in list(gifs.access().keys()):
             raise errors.CategoryError(category)
         else:
             raise errors.CategoryUnknown(category)
         return gif
 
     def get_mal(self, gif) -> str:
         """
@@ -73,15 +73,18 @@
         Returns:
             malid: malId -> int
         """
         for key, gif_url in gifs.access().items():
             for gif_name in gif_url:
                 if gif_name[0] == gif:
                     result = gif_name[1]
-                    malid = int(result)
+                    try:
+                        malid = int(result)
+                    except ValueError as exc:
+                        raise errors.MethodNotUpdated(gif) from exc
                     return malid
             else:
                 continue
 
     def get_animetitle(self, gif) -> str:
         """
         Return the title of the gif's anime.
@@ -92,11 +95,14 @@
         Returns:
             title: title -> str
         """
         for key, gif_url in gifs.access().items():
             for gif_name in gif_url:
                 if gif_name[0] == gif:
                     result = gif_name[1]
-                    title = Anime(int(result)).title
+                    try:
+                        title = Anime(int(result)).title
+                    except ValueError as exc:
+                        raise errors.MethodNotUpdated(gif) from exc
                     return title
             else:
                 continue
```

### Comparing `animegifs-0.6.4/animegifs/distutils/errors.py` & `animegifs-0.7.0/animegifs/distutils/errors.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.4/animegifs.egg-info/PKG-INFO` & `animegifs-0.7.0/animegifs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.6.4
+Version: 0.7.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Classifier: Programming Language :: Python :: 3.8
@@ -54,82 +54,83 @@
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
-**Category list:** 
+## Category list:
 
+**A**
 * Attack
-* Bite
-* Bloodsuck
-* Blush
-* Bonk
-* Brofist
-* Cry
-* Cuddle
-* Dance
-* Disgust
+
+**B**
+* Bite, Bloodsuck, Blush, Bonk, Brofist
+
+**C**
+* Cry, Cuddle
+
+**D**
+* Dance, Disgust
+
+**E**
 * Exploding
-* Facedesk
-* Facepalm
-* Flick
-* Flirt
-* Handhold
-* Happy
-* Harass
-* Highfive
-* Hug
-* Icecream
-* Insult
-* Kill
-* Kiss
-* Lick
-* Love
+
+**F**
+* Facedesk, Facepalm, Flick, Flirt
+
+**H**
+* Handhold, Happy, Harass, Highfive, Hug
+
+**I**
+* Icecream, Insult
+
+**K**
+* Kill, Kiss
+
+**L**
+* Lick, Love
+
+**M**
 * Marry
-* Nod
-* Nosebleed
-* Nuzzle
-* Pat
-* Peck
-* Poke
-* Popcorn
-* Pout
-* Punch
-* Punish
+
+**N**
+* Nod, Nosebleed, Nuzzle
+
+**P**
+* Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
+
+**R**
 * Run
-* Sad
-* Scared
-* Shoot
-* Shrug
-* Sip
-* Slap
-* Smirk
-* Sorry
-* Spank
-* Stare
-* Tease
-* Threat
-* Tickle
-* Tired
+
+**S**
+* Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
+
+**T**
+* Tease, Threat, Tickle, Tired
+
+**W**
 * Wave
+
+**Y**
 * Yawn
 
 **Special Category List**
 
-* Random
-* Steal-magic
+* Random, Steal-magic
+
+# Live API
+
+You can test out the API (and lib functionality) on my bot's website here: https://enkidu-app.github.io/animegifs
 
 # Troubleshooting and other
 
 If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
 Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
 I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
 
 # Copyright
 
 This repository doesn't include any copyrighted material. 
-If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, 
-email me at **grest0grest@gmail.com**. 
+If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, email me at **grest0grest@gmail.com**. 
 Please provide specific details about the copyrighted material and where it can be found.
 Once I confirm your claim, I'll take immediate action to remove the identified material.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.6.4 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.7.0 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
 anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
@@ -15,25 +15,28 @@
 anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
 #return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
 gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
 and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
 anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
 gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` **Category list:** * Attack * Bite * Bloodsuck * Blush *
-Bonk * Brofist * Cry * Cuddle * Dance * Disgust * Exploding * Facedesk *
-Facepalm * Flick * Flirt * Handhold * Happy * Harass * Highfive * Hug *
-Icecream * Insult * Kill * Kiss * Lick * Love * Marry * Nod * Nosebleed *
-Nuzzle * Pat * Peck * Poke * Popcorn * Pout * Punch * Punish * Run * Sad *
-Scared * Shoot * Shrug * Sip * Slap * Smirk * Sorry * Spank * Stare * Tease *
-Threat * Tickle * Tired * Wave * Yawn **Special Category List** * Random *
-Steal-magic # Troubleshooting and other If you encounter an error, please raise
-an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues.
-Alternatively, you can join my Discord server to request new categories,
-functions, provide feedback, or report any errors. I do also have a multi-
-function Discord bot. Feel free to check out the web dashboard here: https://
-enkidu-app.github.io. # Copyright This repository doesn't include any
-copyrighted material. If you happen to come across any copyrighted content
-within this repository (but hosted elsewhere) that you own or represent, email
-me at **grest0grest@gmail.com**. Please provide specific details about the
-copyrighted material and where it can be found. Once I confirm your claim, I'll
-take immediate action to remove the identified material.
+myanimelist page. ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
+Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
+Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
+Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
+Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
+Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, ,Shoot, Shrug,
+Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
+**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
+Live API You can test out the API (and lib functionality) on my bot's website
+here: https://enkidu-app.github.io/animegifs # Troubleshooting and other If you
+encounter an error, please raise an issue on the issue page: https://
+github.com/MarcoSa-2000/animegifs/issues. Alternatively, you can join my
+Discord server to request new categories, functions, provide feedback, or
+report any errors. I do also have a multi-function Discord bot. Feel free to
+check out the web dashboard here: https://enkidu-app.github.io. # Copyright
+This repository doesn't include any copyrighted material. If you happen to come
+across any copyrighted content within this repository (but hosted elsewhere)
+that you own or represent, email me at **grest0grest@gmail.com**. Please
+provide specific details about the copyrighted material and where it can be
+found. Once I confirm your claim, I'll take immediate action to remove the
+identified material.
```

### Comparing `animegifs-0.6.4/setup.py` & `animegifs-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.6.4'
+VERSION = '0.7.0'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
```

