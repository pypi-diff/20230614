# Comparing `tmp/github4api-1.1.4.tar.gz` & `tmp/github4api-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github4api-1.1.4.tar", last modified: Fri Jun  9 12:48:46 2023, max compression
+gzip compressed data, was "github4api-1.1.5.tar", last modified: Wed Jun 14 00:16:26 2023, max compression
```

## Comparing `github4api-1.1.4.tar` & `github4api-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.041315 github4api-1.1.4/
--rw-rw-rw-   0        0        0     1092 2023-06-08 18:05:26.000000 github4api-1.1.4/LICENSE
--rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8449 2023-06-09 12:48:46.041315 github4api-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     7423 2023-06-09 12:45:58.000000 github4api-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.028234 github4api-1.1.4/github4api/
--rw-rw-rw-   0        0        0      245 2023-06-08 18:44:02.000000 github4api-1.1.4/github4api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.035236 github4api-1.1.4/github4api/handlers/
--rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.4/github4api/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.036233 github4api-1.1.4/github4api/handlers/request_handler/
--rw-rw-rw-   0        0        0      941 2023-06-08 18:55:53.000000 github4api-1.1.4/github4api/handlers/request_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.037313 github4api-1.1.4/github4api/handlers/user_handler/
--rw-rw-rw-   0        0        0      792 2023-06-09 11:56:55.000000 github4api-1.1.4/github4api/handlers/user_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.038314 github4api-1.1.4/github4api/scraper/
--rw-rw-rw-   0        0        0     7007 2023-06-09 12:19:47.000000 github4api-1.1.4/github4api/scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.034234 github4api-1.1.4/github4api.egg-info/
--rw-rw-rw-   0        0        0     8449 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      424 2023-06-08 18:15:41.000000 github4api-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 12:48:46.041315 github4api-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-06-08 18:15:23.000000 github4api-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.039315 github4api-1.1.4/tests/
--rw-rw-rw-   0        0        0      585 2023-06-08 16:08:56.000000 github4api-1.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.929211 github4api-1.1.5/
+-rw-rw-rw-   0        0        0     1092 2023-06-08 18:05:26.000000 github4api-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9880 2023-06-14 00:16:26.929211 github4api-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8803 2023-06-14 00:15:03.000000 github4api-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.916211 github4api-1.1.5/github4api/
+-rw-rw-rw-   0        0        0      372 2023-06-13 23:43:00.000000 github4api-1.1.5/github4api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.922211 github4api-1.1.5/github4api/exceptions/
+-rw-rw-rw-   0        0        0      285 2023-06-13 23:42:53.000000 github4api-1.1.5/github4api/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.923211 github4api-1.1.5/github4api/handlers/
+-rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.5/github4api/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.924209 github4api-1.1.5/github4api/handlers/request_handler/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 22:34:53.000000 github4api-1.1.5/github4api/handlers/request_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.925211 github4api-1.1.5/github4api/handlers/user_handler/
+-rw-rw-rw-   0        0        0      976 2023-06-13 22:36:24.000000 github4api-1.1.5/github4api/handlers/user_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.926211 github4api-1.1.5/github4api/scraper/
+-rw-rw-rw-   0        0        0    11348 2023-06-14 00:06:30.000000 github4api-1.1.5/github4api/scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.921216 github4api-1.1.5/github4api.egg-info/
+-rw-rw-rw-   0        0        0     9880 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 00:16:26.000000 github4api-1.1.5/github4api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      424 2023-06-09 19:21:00.000000 github4api-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:16:26.929211 github4api-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-06-09 19:20:47.000000 github4api-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:16:26.928213 github4api-1.1.5/tests/
+-rw-rw-rw-   0        0        0      603 2023-06-09 19:43:12.000000 github4api-1.1.5/tests/__init__.py
```

### Comparing `github4api-1.1.4/LICENSE` & `github4api-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `github4api-1.1.4/PKG-INFO` & `github4api-1.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.4</b></p>
+<p align='center'><b>Version 1.1.5</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
@@ -182,15 +182,15 @@
 from github4api.handlers.request_handler import RequestHandler
 
 
 
 
 def main():
     request: RequestHandler = RequestHandler(
-        url=UserHandler(username='shervinbdndev').serialize(get_repos=True), # for accessing the repositories you should set get_repos param to True
+        url=UserHandler(username='shervinbdndev').serialize(),
     ).sendGetRequest(content=True)
     
     scraper: Scrape = Scrape(data=request)
     
     scraper.startApi(log=False)
 
     # Then your free to use the new method to get User's Repositories names
@@ -256,13 +256,64 @@
 
 
 if (__name__ == "__main__"):
     main()
 
 ```
 
+<br><br><br>
+
+# New Changes on Version 1.1.5
+
+## Now you can Access
+
+- ### User's Last Year Contributions
+- ### Check if User's Repository is Public Archive
+- ### Check if User has README.md
+- ### Get Repository's Used Languages
+- ### Get User's Unlocked Achievements
+
+
+```python
+
+
+from github4api.scraper import Scrape
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
+
+
+
+
+def main():
+    user: UserHandler = UserHandler(username='shervinbdndev').serialize() # user instance
+    
+    request: RequestHandler = RequestHandler(url=user).sendGetRequest(content=True) # send request by RequestHandler
+    
+    scraper: Scrape = Scrape(data=request)
+    
+    scraper.startApi(log=False)
+    
+    print(scraper.lastYearContributions) # last year contributions
+    
+    print(scraper.isRepositoryPublicArchive(username='shervinbdndev', repo_name='Quizino')) # check if repository is public archive => returns True or False
+    
+    print(scraper.userHasReadMe(username='shervinbdndev')) # check if user has README.md
+
+    print(scraper.repositoryUsedLanguages(username='shervinbdndev', repo_name='github4api')) # get repository's used languages (also you can select by index)
+
+    print(scraper.userAchievements(username='shervinbdndev')) # get user's achievements (also you can select by index)
+    
+
+
+
+if (__name__ == "__main__"):
+    main()
+
+
+```
+
 <br>
 
 <h1 align='left'>Enjoy :)</h1>
 
 <br>
 <h3><b>Package Uploaded in PYPI :<a href="https://pypi.org/project/github4api/">Here</a></b></h3>
```

### Comparing `github4api-1.1.4/README.md` & `github4api-1.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.4</b></p>
+<p align='center'><b>Version 1.1.5</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
@@ -160,15 +160,15 @@
 from github4api.handlers.request_handler import RequestHandler
 
 
 
 
 def main():
     request: RequestHandler = RequestHandler(
-        url=UserHandler(username='shervinbdndev').serialize(get_repos=True), # for accessing the repositories you should set get_repos param to True
+        url=UserHandler(username='shervinbdndev').serialize(),
     ).sendGetRequest(content=True)
     
     scraper: Scrape = Scrape(data=request)
     
     scraper.startApi(log=False)
 
     # Then your free to use the new method to get User's Repositories names
@@ -234,13 +234,64 @@
 
 
 if (__name__ == "__main__"):
     main()
 
 ```
 
+<br><br><br>
+
+# New Changes on Version 1.1.5
+
+## Now you can Access
+
+- ### User's Last Year Contributions
+- ### Check if User's Repository is Public Archive
+- ### Check if User has README.md
+- ### Get Repository's Used Languages
+- ### Get User's Unlocked Achievements
+
+
+```python
+
+
+from github4api.scraper import Scrape
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
+
+
+
+
+def main():
+    user: UserHandler = UserHandler(username='shervinbdndev').serialize() # user instance
+    
+    request: RequestHandler = RequestHandler(url=user).sendGetRequest(content=True) # send request by RequestHandler
+    
+    scraper: Scrape = Scrape(data=request)
+    
+    scraper.startApi(log=False)
+    
+    print(scraper.lastYearContributions) # last year contributions
+    
+    print(scraper.isRepositoryPublicArchive(username='shervinbdndev', repo_name='Quizino')) # check if repository is public archive => returns True or False
+    
+    print(scraper.userHasReadMe(username='shervinbdndev')) # check if user has README.md
+
+    print(scraper.repositoryUsedLanguages(username='shervinbdndev', repo_name='github4api')) # get repository's used languages (also you can select by index)
+
+    print(scraper.userAchievements(username='shervinbdndev')) # get user's achievements (also you can select by index)
+    
+
+
+
+if (__name__ == "__main__"):
+    main()
+
+
+```
+
 <br>
 
 <h1 align='left'>Enjoy :)</h1>
 
 <br>
 <h3><b>Package Uploaded in PYPI :<a href="https://pypi.org/project/github4api/">Here</a></b></h3>
```

### Comparing `github4api-1.1.4/github4api/handlers/request_handler/__init__.py` & `github4api-1.1.5/github4api/handlers/request_handler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,32 @@
 
 
 
 
 
 class RequestHandler:
     def __init__(self: Self, url: str) -> Literal[None]:
+        super(RequestHandler, self).__init__()
         self.__url = url
         self.__data = None
         
     @property
     def url(self: Self) -> str:
         return self.__url
         
-    def sendGetRequest(self: Self, content: bool = False) -> Union[int, bytes, Literal[None]]:
+    def sendGetRequest(self: Self, content: bool = False, status_code = False) -> Union[int, bytes, Literal[None]]:
         try:
             self.__data = requests.get(url=self.url)
             
         except* requests.ConnectionError as ce:
             raise ce.__doc__
         
         except* requests.RequestException as re:
             raise re.__doc__
         
         if (content):
             return self.__data.content
         
+        if (status_code):
+            return self.__data.status_code
+        
         return self.__data
```

### Comparing `github4api-1.1.4/github4api.egg-info/PKG-INFO` & `github4api-1.1.5/github4api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.4</b></p>
+<p align='center'><b>Version 1.1.5</b></p>
 <p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
@@ -182,15 +182,15 @@
 from github4api.handlers.request_handler import RequestHandler
 
 
 
 
 def main():
     request: RequestHandler = RequestHandler(
-        url=UserHandler(username='shervinbdndev').serialize(get_repos=True), # for accessing the repositories you should set get_repos param to True
+        url=UserHandler(username='shervinbdndev').serialize(),
     ).sendGetRequest(content=True)
     
     scraper: Scrape = Scrape(data=request)
     
     scraper.startApi(log=False)
 
     # Then your free to use the new method to get User's Repositories names
@@ -256,13 +256,64 @@
 
 
 if (__name__ == "__main__"):
     main()
 
 ```
 
+<br><br><br>
+
+# New Changes on Version 1.1.5
+
+## Now you can Access
+
+- ### User's Last Year Contributions
+- ### Check if User's Repository is Public Archive
+- ### Check if User has README.md
+- ### Get Repository's Used Languages
+- ### Get User's Unlocked Achievements
+
+
+```python
+
+
+from github4api.scraper import Scrape
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
+
+
+
+
+def main():
+    user: UserHandler = UserHandler(username='shervinbdndev').serialize() # user instance
+    
+    request: RequestHandler = RequestHandler(url=user).sendGetRequest(content=True) # send request by RequestHandler
+    
+    scraper: Scrape = Scrape(data=request)
+    
+    scraper.startApi(log=False)
+    
+    print(scraper.lastYearContributions) # last year contributions
+    
+    print(scraper.isRepositoryPublicArchive(username='shervinbdndev', repo_name='Quizino')) # check if repository is public archive => returns True or False
+    
+    print(scraper.userHasReadMe(username='shervinbdndev')) # check if user has README.md
+
+    print(scraper.repositoryUsedLanguages(username='shervinbdndev', repo_name='github4api')) # get repository's used languages (also you can select by index)
+
+    print(scraper.userAchievements(username='shervinbdndev')) # get user's achievements (also you can select by index)
+    
+
+
+
+if (__name__ == "__main__"):
+    main()
+
+
+```
+
 <br>
 
 <h1 align='left'>Enjoy :)</h1>
 
 <br>
 <h3><b>Package Uploaded in PYPI :<a href="https://pypi.org/project/github4api/">Here</a></b></h3>
```

### Comparing `github4api-1.1.4/setup.py` & `github4api-1.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with codecs.open(os.path.normpath(path=os.path.join(os.path.abspath(path=os.path.dirname(p=__file__)) , r"README.md")) , encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 setup(
     name="github4api",
-    version='1.1.4',
+    version='1.1.5',
     author="Shervin Badanara (shervinbdndev)",
     maintainer="Shervin Badanara",
     author_email="shervin2234@gmail.com",
     description='A python Package API for getting Github Users Information.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages() ,
```

### Comparing `github4api-1.1.4/tests/__init__.py` & `github4api-1.1.5/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from github4api.scraper import Scrape
-from github4api.user_handler import UserHandler
-from github4api.request_handler import RequestHandler
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
 
 
 
 
 def main():
     request: RequestHandler = RequestHandler(
         url=UserHandler(username='shervinbdndev').serialize(),
```

