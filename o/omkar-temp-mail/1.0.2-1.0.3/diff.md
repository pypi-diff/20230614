# Comparing `tmp/omkar-temp-mail-1.0.2.tar.gz` & `tmp/omkar-temp-mail-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omkar-temp-mail-1.0.2.tar", last modified: Wed Jun 14 06:58:38 2023, max compression
+gzip compressed data, was "omkar-temp-mail-1.0.3.tar", last modified: Wed Jun 14 07:01:59 2023, max compression
```

## Comparing `omkar-temp-mail-1.0.2.tar` & `omkar-temp-mail-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,2 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-14 06:58:38.050292 omkar-temp-mail-1.0.2/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      114 2023-06-14 06:56:59.000000 omkar-temp-mail-1.0.2/AUTHORS
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1068 2023-06-14 06:56:59.000000 omkar-temp-mail-1.0.2/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4238 2023-06-14 06:58:38.050292 omkar-temp-mail-1.0.2/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2604 2023-06-14 06:56:59.000000 omkar-temp-mail-1.0.2/README.rst
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-14 06:58:38.050292 omkar-temp-mail-1.0.2/omkar-temp-mail/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       31 2023-06-14 06:56:59.000000 omkar-temp-mail-1.0.2/omkar-temp-mail/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5234 2023-06-14 06:56:59.000000 omkar-temp-mail-1.0.2/omkar-temp-mail/temp_mail.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-14 06:58:38.050292 omkar-temp-mail-1.0.2/omkar_temp_mail.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4238 2023-06-14 06:58:37.000000 omkar-temp-mail-1.0.2/omkar_temp_mail.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      296 2023-06-14 06:58:37.000000 omkar-temp-mail-1.0.2/omkar_temp_mail.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-14 06:58:37.000000 omkar-temp-mail-1.0.2/omkar_temp_mail.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       32 2023-06-14 06:58:37.000000 omkar-temp-mail-1.0.2/omkar_temp_mail.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       16 2023-06-14 06:58:37.000000 omkar-temp-mail-1.0.2/omkar_temp_mail.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2023-06-14 06:58:38.054292 omkar-temp-mail-1.0.2/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2216 2023-06-14 06:56:59.000000 omkar-temp-mail-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:01:59.569862 omkar-temp-mail-1.0.3/
+-rw-rw-rw-   0        0        0     4720 2023-06-14 07:01:59.569862 omkar-temp-mail-1.0.3/PKG-INFO
```

### Comparing `omkar-temp-mail-1.0.2/PKG-INFO` & `omkar-temp-mail-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,112 @@
-Metadata-Version: 2.1
-Name: omkar-temp-mail
-Version: 1.0.2
-Summary: Use Omkar Temporary for receiving temporary emails
-Author: Chetan Jain
-Author-email: chetan@omkar.cloud
-Maintainer: Chetan Jain
-Maintainer-email: chetan@omkar.cloud
-License: MIT
-Project-URL: Documentation, https://github.com/omkarcloud/omkar-temp-mail
-Project-URL: Source, https://github.com/omkarcloud/omkar-temp-mail
-Project-URL: Tracker, https://github.com/omkarcloud/omkar-temp-mail/issues
-Keywords: temp-mail,disposable-email,temporary-email,tempmail,temporary-email,disposable-email-addresses,python,mail-api,mail ,10minutemail,10minute,free-mail
-Classifier: Framework :: Scrapy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-License-File: LICENSE
-License-File: AUTHORS
-
-Omkar Temp Mail
-===============
-
-Omkar Temporary Email offers a convenient solution for receiving
-temporary emails. It is particularly useful for automated tasks that
-require email verification during account creation.
-
-Getting Started
----------------
-
-To get started with Omkar Temp Mail install ``omkar-temp-mail`` using
-the following command:
-
-.. code:: bash
-
-   python -m pip install omkar-temp-mail
-
-Usage
------
-
-1. ``get_domains`` Returns a list of available domain options for
-   generating temporary email addresses.
-
-.. code:: python
-
-   from omkar_temp_mail import TempMail
-
-   domains = TempMail.get_domains()
-   print(domains) # prints ['1secmail.com', '1secmail.org', '1secmail.net', 'kzccv.com', 'qiott.com', 'wuuvo.com', 'icznn.com', 'ezztt.com']
-
-2. ``get_email_link(email)``
-
-Get’s the first link from the most recent email message received in the
-given email address.
-
-.. code:: python
-
-   from omkar_temp_mail import TempMail
-
-   email = "shyam@1secmail.com"
-   link = TempMail.get_email_link(email)
-   print(link) 
-
-3. ``get_body(email)``
-
-Get’s the content (text or HTML) from the most recent email message
-received in the given email address.
-
-.. code:: python
-
-   from omkar_temp_mail import TempMail
-
-   email = "shyam@1secmail.com"
-   body = TempMail.get_body(email)
-   print(body) 
-
-4. ``deleteMailbox(email)``
-
-Deletes the mailbox associated with the provided email address.
-
-.. code:: python
-
-   from omkar_temp_mail import TempMail
-
-   email = "shyam@1secmail.com"
-   TempMail.deleteMailbox(email)
-
-5. ``get_email_link_and_delete_mailbox(email)``
-
-Combines the functionality of ``get_email_link`` and
-``deleteMailbox(email)``. It first retrieves the first link from the
-most recent email and then deletes the mailbox, returning the link.
-
-.. code:: python
-
-   from omkar_temp_mail import TempMail
-
-   email = "shyam@1secmail.com"
-   link = TempMail.get_email_link_and_delete_mailbox(email)
-   print("Link:", link)
-
-If my code helped you in generating Temporary Email, please take a moment to `star the repository <https://github.com/omkarcloud/omkar-temp-mail>`__. Your act of starring will help developers in discovering our Repository and contribute towards helping fellow developers in their automation tasks. Dhanyawad 🙏! Vande Mataram!
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+Metadata-Version: 1.1
+Name: omkar-temp-mail
+Version: 1.0.3
+Summary: Use Omkar Temporary for receiving temporary emails
+Home-page: UNKNOWN
+Author: Chetan Jain
+Author-email: chetan@omkar.cloud
+License: MIT
+Description: Omkar Temp Mail
+        ===============
+        
+        Omkar Temporary Email offers a convenient solution for receiving
+        temporary emails. It is particularly useful for automated tasks that
+        require email verification during account creation.
+        
+        Getting Started
+        ---------------
+        
+        To get started with Omkar Temp Mail install ``omkar-temp-mail`` using
+        the following command:
+        
+        .. code:: bash
+        
+           python -m pip install omkar-temp-mail
+        
+        Usage
+        -----
+        
+        1. ``get_domains`` Returns a list of available domain options for
+           generating temporary email addresses.
+        
+        .. code:: python
+        
+           from omkar_temp_mail import TempMail
+        
+           domains = TempMail.get_domains()
+           print(domains) # prints ['1secmail.com', '1secmail.org', '1secmail.net', 'kzccv.com', 'qiott.com', 'wuuvo.com', 'icznn.com', 'ezztt.com']
+        
+        2. ``get_email_link(email)``
+        
+        Get’s the first link from the most recent email message received in the
+        given email address.
+        
+        .. code:: python
+        
+           from omkar_temp_mail import TempMail
+        
+           email = "shyam@1secmail.com"
+           link = TempMail.get_email_link(email)
+           print(link) 
+        
+        3. ``get_body(email)``
+        
+        Get’s the content (text or HTML) from the most recent email message
+        received in the given email address.
+        
+        .. code:: python
+        
+           from omkar_temp_mail import TempMail
+        
+           email = "shyam@1secmail.com"
+           body = TempMail.get_body(email)
+           print(body) 
+        
+        4. ``deleteMailbox(email)``
+        
+        Deletes the mailbox associated with the provided email address.
+        
+        .. code:: python
+        
+           from omkar_temp_mail import TempMail
+        
+           email = "shyam@1secmail.com"
+           TempMail.deleteMailbox(email)
+        
+        5. ``get_email_link_and_delete_mailbox(email)``
+        
+        Combines the functionality of ``get_email_link`` and
+        ``deleteMailbox(email)``. It first retrieves the first link from the
+        most recent email and then deletes the mailbox, returning the link.
+        
+        .. code:: python
+        
+           from omkar_temp_mail import TempMail
+        
+           email = "shyam@1secmail.com"
+           link = TempMail.get_email_link_and_delete_mailbox(email)
+           print("Link:", link)
+        
+        If my code helped you in generating Temporary Email, please take a moment to `star the repository <https://github.com/omkarcloud/omkar-temp-mail>`__. Your act of starring will help developers in discovering our Repository and contribute towards helping fellow developers in their automation tasks. Dhanyawad 🙏! Vande Mataram!
+        --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+        
+Keywords: temp-mail,disposable-email,temporary-email,tempmail,temporary-email,disposable-email-addresses,python,mail-api,mail ,10minutemail,10minute,free-mail
+Platform: UNKNOWN
+Classifier: Framework :: Scrapy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

