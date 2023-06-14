# Comparing `tmp/ensta-2.2.tar.gz` & `tmp/ensta-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.2.tar", last modified: Tue Jun 13 18:06:46 2023, max compression
+gzip compressed data, was "ensta-2.3.tar", last modified: Wed Jun 14 16:39:03 2023, max compression
```

## Comparing `ensta-2.2.tar` & `ensta-2.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-13 18:06:24.000000 ensta-2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-13 18:06:46.049261 ensta-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-13 18:06:24.000000 ensta-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta/
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-13 18:06:24.000000 ensta-2.2/ensta/Guest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-06-13 18:06:24.000000 ensta-2.2/ensta/Host.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 18:06:24.000000 ensta-2.2/ensta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/FollowPerson.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/FollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/UnfollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-13 18:06:24.000000 ensta-2.2/ensta/lib/Commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-13 18:06:24.000000 ensta-2.2/ensta/lib/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 18:06:24.000000 ensta-2.2/ensta/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 18:06:46.053261 ensta-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-13 18:06:24.000000 ensta-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.365608 ensta-2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-14 16:38:51.000000 ensta-2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-14 16:39:03.365608 ensta-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-14 16:38:51.000000 ensta-2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.361608 ensta-2.3/ensta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-14 16:38:51.000000 ensta-2.3/ensta/Authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-14 16:38:51.000000 ensta-2.3/ensta/Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-06-14 16:38:51.000000 ensta-2.3/ensta/Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 16:38:51.000000 ensta-2.3/ensta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.365608 ensta-2.3/ensta/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/FollowPerson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/FollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/UnfollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.365608 ensta-2.3/ensta/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-14 16:38:51.000000 ensta-2.3/ensta/lib/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-14 16:38:51.000000 ensta-2.3/ensta/lib/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 16:38:51.000000 ensta-2.3/ensta/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.361608 ensta-2.3/ensta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 16:39:03.365608 ensta-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-14 16:38:51.000000 ensta-2.3/setup.py
```

### Comparing `ensta-2.2/LICENSE.txt` & `ensta-2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-2.2/PKG-INFO` & `ensta-2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.2
+Version: 2.3
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.2.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.3.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,42 +16,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 🤖 Ensta - Simple Instagram API
 [![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
+[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
 
-This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
+<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
 
-It supports three two of classes - *Guest* & *Host*.
+This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+Two type of classes are supported - ***Guest & Host***.
+
+[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
+
+## 📢 Announcement
+Users can now log in through their **Username** and **Password** to generate SessionId!
 
 ## Installation
-To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
+To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
-pip install ensta
+$ pip install ensta
 ```
 
-To upgrade to the latest version, run:
+To update the existing package, run:
 ```shell
-pip install ensta --upgrade
+$ pip install ensta --upgrade
 ```
 
 ## 🧔🏻‍♂️ Guest Mode
 This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
 - Check if username is available for registration
 - Fetch someone's profile data
 - Convert username to userid
 - Convert userid to username
 
-Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
 profile = guest.profile("cristiano")
 
@@ -60,70 +65,62 @@
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
 ```
 
 ## 🧔🏻‍♂️ Host Mode
-This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
+Host mode requires login through SessionID, which should be passed as an argument during initialization.
+It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
 
 These are the methods supported till now:
 - Check authentication status of the user
-- Send follow request to an account
-- Follow/unfollow accounts
+- Follow/unfollow users
 - Fetch someone's follower/following list
-- Toggle account privacy - 'Public' or 'Private'
+- Switch account type - 'Public' or 'Private'
 
-Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
 
 ```python
-from ensta import Host
+from ensta import Host, NewSessionID
 
-sessionid = "123456:abcdefg"  # Place your SessionId here
+sessionid = NewSessionID("username", "password")
 
 host = Host(sessionid)
 status = host.follow("cristiano")
 
 if status is None:
     print("Something went wrong.")
 else:
     if status.following:
         print("Following!")
     
     elif status.follow_requested:
         print("Requested to follow!")
 ```
 
-## Important
-Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
+> ### **Note:**
+> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
+>
+> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
+
+## 📋 Remember
+Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
 ```python
 from ensta import Guest
 
 guest = Guest()
 available = guest.username_availability("cristiano")
 
-if available is None:  # Operation failed
+if available is None:  # 'None' indicates failure
     print("Something went wrong.")
 else:
     print(available)
 ```
 
-## Session ID
-When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
-
-In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
-- Visit [Instagram.com](https://instagram.com) and log into your account.
-- Once you're logged in, open DevTools (Ctrl + Shift + I).
-- Switch to **Application** tab.
-- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
-- Once done, you will see the list of all cookies.
-- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
-
-An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
-
-## Donate ❤️
-If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
+## ❤️ Donate
+If you wish to help me in the development of Ensta, consider donating:
 
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
 
 ## Disclaimer
-This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
+This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
```

### Comparing `ensta-2.2/README.md` & `ensta-2.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 # 🤖 Ensta - Simple Instagram API
 [![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
+[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
 
-This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
+<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
 
-It supports three two of classes - *Guest* & *Host*.
+This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+Two type of classes are supported - ***Guest & Host***.
+
+[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
+
+## 📢 Announcement
+Users can now log in through their **Username** and **Password** to generate SessionId!
 
 ## Installation
-To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
+To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
-pip install ensta
+$ pip install ensta
 ```
 
-To upgrade to the latest version, run:
+To update the existing package, run:
 ```shell
-pip install ensta --upgrade
+$ pip install ensta --upgrade
 ```
 
 ## 🧔🏻‍♂️ Guest Mode
 This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
 - Check if username is available for registration
 - Fetch someone's profile data
 - Convert username to userid
 - Convert userid to username
 
-Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
 profile = guest.profile("cristiano")
 
@@ -41,70 +46,62 @@
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
 ```
 
 ## 🧔🏻‍♂️ Host Mode
-This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
+Host mode requires login through SessionID, which should be passed as an argument during initialization.
+It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
 
 These are the methods supported till now:
 - Check authentication status of the user
-- Send follow request to an account
-- Follow/unfollow accounts
+- Follow/unfollow users
 - Fetch someone's follower/following list
-- Toggle account privacy - 'Public' or 'Private'
+- Switch account type - 'Public' or 'Private'
 
-Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
 
 ```python
-from ensta import Host
+from ensta import Host, NewSessionID
 
-sessionid = "123456:abcdefg"  # Place your SessionId here
+sessionid = NewSessionID("username", "password")
 
 host = Host(sessionid)
 status = host.follow("cristiano")
 
 if status is None:
     print("Something went wrong.")
 else:
     if status.following:
         print("Following!")
     
     elif status.follow_requested:
         print("Requested to follow!")
 ```
 
-## Important
-Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
+> ### **Note:**
+> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
+>
+> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
+
+## 📋 Remember
+Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
 ```python
 from ensta import Guest
 
 guest = Guest()
 available = guest.username_availability("cristiano")
 
-if available is None:  # Operation failed
+if available is None:  # 'None' indicates failure
     print("Something went wrong.")
 else:
     print(available)
 ```
 
-## Session ID
-When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
-
-In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
-- Visit [Instagram.com](https://instagram.com) and log into your account.
-- Once you're logged in, open DevTools (Ctrl + Shift + I).
-- Switch to **Application** tab.
-- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
-- Once done, you will see the list of all cookies.
-- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
-
-An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
-
-## Donate ❤️
-If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
+## ❤️ Donate
+If you wish to help me in the development of Ensta, consider donating:
 
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
 
 ## Disclaimer
-This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
+This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
```

### Comparing `ensta-2.2/ensta/Guest.py` & `ensta-2.3/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-2.2/ensta/Host.py` & `ensta-2.3/ensta/Host.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     refresh_csrf_token,
     update_app_id,
     update_homepage_source,
     update_session,
     format_identifier
 )
 from .lib import (
-    AuthenticationError,
+    SessionError,
     NetworkError,
     IdentifierError,
-    CodeError
+    DevelopmentError
 )
 from .containers import (FollowedStatus, UnfollowedStatus, FollowPerson)
 from .containers.Profile import Profile
 
 USERNAME = 0
 UID = 1
 
@@ -43,15 +43,15 @@
             homepage_source=self.homepage_source,
             app_id=self.insta_app_id
         )
 
         self.request_session.cookies.set("sessionid", session_id)
 
         if not self.authenticated():
-            raise AuthenticationError("Either User ID or Session ID is not valid.")
+            raise SessionError("SessionID is incorrect or expired.")
 
     def update_homepage_source(self) -> None:
         temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
 
         if temp_homepage_source == "":
             raise NetworkError("Couldn't load instagram homepage.")
 
@@ -453,21 +453,21 @@
             else:
                 return False, None
 
         elif not is_username and required == UID:
             return True, identifier
 
         else:
-            raise CodeError("Identifier Conversion (Else Block)")
+            raise DevelopmentError("Identifier Conversion (Else Block)")
 
     def _set_account_privacy(self, privacy: str) -> bool:
         is_private = (privacy == "private")
 
         if privacy != "private" and privacy != "public":
-            raise CodeError("_set_account_privacy")
+            raise DevelopmentError("_set_account_privacy")
 
         refresh_csrf_token(self)
         body_json = {
             "is_private": is_private
         }
         request_headers = {
             "accept": "*/*",
```

### Comparing `ensta-2.2/ensta/containers/Profile.py` & `ensta-2.3/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-2.2/ensta/lib/Commons.py` & `ensta-2.3/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-2.2/ensta/lib/Exceptions.py` & `ensta-2.3/ensta/lib/Exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class AuthenticationError(Exception):
+class SessionError(Exception):
 
     def __init__(self, message):
         super().__init__(message)
 
 
 class NetworkError(Exception):
 
@@ -12,11 +12,23 @@
 
 class IdentifierError(Exception):
 
     def __init__(self, message):
         super().__init__(message)
 
 
-class CodeError(Exception):
+class DevelopmentError(Exception):
 
     def __init__(self, location: str = "Unknown"):
         super().__init__(f"There was an error while executing this function, maybe caused due to a bug in the code. Please submit this as an issue on GitHub.\nFound in: {location}")
+
+
+class AuthenticationError(Exception):
+
+    def __init__(self, message):
+        super().__init__(message)
+
+
+class ChallengeError(Exception):
+
+    def __init__(self, message):
+        super().__init__(message)
```

### Comparing `ensta-2.2/ensta.egg-info/PKG-INFO` & `ensta-2.3/ensta.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.2
+Version: 2.3
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.2.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.3.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,42 +16,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 🤖 Ensta - Simple Instagram API
 [![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+[![Downloads](https://static.pepy.tech/badge/ensta)](https://pepy.tech/project/ensta)
+[![Twitter Share](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
 
-This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
+<img style="border-radius: 10px" src="https://imgtr.ee/images/2023/06/14/Twfd4.png"/>
 
-It supports three two of classes - *Guest* & *Host*.
+This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+Two type of classes are supported - ***Guest & Host***.
+
+[<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
+
+## 📢 Announcement
+Users can now log in through their **Username** and **Password** to generate SessionId!
 
 ## Installation
-To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
+To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
-pip install ensta
+$ pip install ensta
 ```
 
-To upgrade to the latest version, run:
+To update the existing package, run:
 ```shell
-pip install ensta --upgrade
+$ pip install ensta --upgrade
 ```
 
 ## 🧔🏻‍♂️ Guest Mode
 This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
 - Check if username is available for registration
 - Fetch someone's profile data
 - Convert username to userid
 - Convert userid to username
 
-Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+Here's an example where an instance of *Guest Class* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
 profile = guest.profile("cristiano")
 
@@ -60,70 +65,62 @@
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
 ```
 
 ## 🧔🏻‍♂️ Host Mode
-This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
+Host mode requires login through SessionID, which should be passed as an argument during initialization.
+It can be used to take actions that require login. Additionally, users can manage their own profile through this class.
 
 These are the methods supported till now:
 - Check authentication status of the user
-- Send follow request to an account
-- Follow/unfollow accounts
+- Follow/unfollow users
 - Fetch someone's follower/following list
-- Toggle account privacy - 'Public' or 'Private'
+- Switch account type - 'Public' or 'Private'
 
-Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+Here's an example where an instance of *Host Class* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
 
 ```python
-from ensta import Host
+from ensta import Host, NewSessionID
 
-sessionid = "123456:abcdefg"  # Place your SessionId here
+sessionid = NewSessionID("username", "password")
 
 host = Host(sessionid)
 status = host.follow("cristiano")
 
 if status is None:
     print("Something went wrong.")
 else:
     if status.following:
         print("Following!")
     
     elif status.follow_requested:
         print("Requested to follow!")
 ```
 
-## Important
-Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
+> ### **Note:**
+> When you create a new sessionid through *NewSessionID()*, it's recommended to save it somewhere, and use the same sessionid (instead of creating a new one each time you need) until it expires or becomes invalid.
+>
+> This should be done to avoid unnecessary prolonged wait time while generating a new sessionid and also to prevent getting your account from getting flagged because of repetitive logins.
+
+## 📋 Remember
+Every function should return **None** on failure. So, it's recommended to add an *if statement* before using the actual data to avoid TypeErrors. Here's an example:
 ```python
 from ensta import Guest
 
 guest = Guest()
 available = guest.username_availability("cristiano")
 
-if available is None:  # Operation failed
+if available is None:  # 'None' indicates failure
     print("Something went wrong.")
 else:
     print(available)
 ```
 
-## Session ID
-When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
-
-In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
-- Visit [Instagram.com](https://instagram.com) and log into your account.
-- Once you're logged in, open DevTools (Ctrl + Shift + I).
-- Switch to **Application** tab.
-- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
-- Once done, you will see the list of all cookies.
-- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
-
-An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
-
-## Donate ❤️
-If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
+## ❤️ Donate
+If you wish to help me in the development of Ensta, consider donating:
 
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+[<img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="150"/>](https://buymeacoffee.com/diezo)
 
 ## Disclaimer
-This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
+This is a third-party package, and not approved by Instagram. It doesn't promote illegal activities or activities that violate [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/) such as spamming users, creating bot accounts, misusing data etc. You are solely responsible for all the actions you take using this package.
```

### Comparing `ensta-2.2/setup.py` & `ensta-2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="2.2",
+    version="2.3",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.2.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.3.tar.gz",
     keywords=["instagram-client", "instagram", "api-wrapper", "instagram-scraper", "instagram-api", "instagram-sdk", "instagram-photos", "instagram-api-python", "instabot", "instagram-stories", "instagram-bot", "instapy", "instagram-downloader", "instagram-account", "instagram-crawler", "instagram-private-api", "igtv", "instagram-automation", "reels", "instagram-feed"],
-    install_requires=["requests"],
+    install_requires=["requests", "selenium"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10"
```

