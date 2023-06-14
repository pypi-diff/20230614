# Comparing `tmp/NuPlone-2.1.4.tar.gz` & `tmp/NuPlone-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuPlone-2.1.4.tar", last modified: Wed Jan  4 13:07:46 2023, max compression
+gzip compressed data, was "NuPlone-2.2.0.tar", last modified: Wed Jun 14 14:57:41 2023, max compression
```

## Comparing `NuPlone-2.1.4.tar` & `NuPlone-2.2.0.tar`

### file list

```diff
@@ -1,400 +1,400 @@
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.429804 NuPlone-2.1.4/
--rw-r--r--   0 thet      (1000) thet      (1000)      265 2023-01-04 13:07:45.000000 NuPlone-2.1.4/MANIFEST.in
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.381803 NuPlone-2.1.4/NuPlone.egg-info/
--rw-r--r--   0 thet      (1000) thet      (1000)    18783 2023-01-04 13:07:46.000000 NuPlone-2.1.4/NuPlone.egg-info/PKG-INFO
--rw-r--r--   0 thet      (1000) thet      (1000)    17936 2023-01-04 13:07:46.000000 NuPlone-2.1.4/NuPlone.egg-info/SOURCES.txt
--rw-r--r--   0 thet      (1000) thet      (1000)        1 2023-01-04 13:07:46.000000 NuPlone-2.1.4/NuPlone.egg-info/dependency_links.txt
--rw-r--r--   0 thet      (1000) thet      (1000)       11 2023-01-04 13:07:46.000000 NuPlone-2.1.4/NuPlone.egg-info/namespace_packages.txt
--rw-r--r--   0 thet      (1000) thet      (1000)        1 2023-01-04 13:07:46.000000 NuPlone-2.1.4/NuPlone.egg-info/not-zip-safe
--rw-r--r--   0 thet      (1000) thet      (1000)      278 2023-01-04 13:07:46.000000 NuPlone-2.1.4/NuPlone.egg-info/requires.txt
--rw-r--r--   0 thet      (1000) thet      (1000)       11 2023-01-04 13:07:46.000000 NuPlone-2.1.4/NuPlone.egg-info/top_level.txt
--rw-r--r--   0 thet      (1000) thet      (1000)    18783 2023-01-04 13:07:46.429804 NuPlone-2.1.4/PKG-INFO
--rw-r--r--   0 thet      (1000) thet      (1000)     1940 2023-01-04 13:07:45.000000 NuPlone-2.1.4/README.rst
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.381803 NuPlone-2.1.4/docs/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.381803 NuPlone-2.1.4/docs/.static/
--rw-r--r--   0 thet      (1000) thet      (1000)      674 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/.static/logo.png
--rw-r--r--   0 thet      (1000) thet      (1000)     1126 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/.static/plone.css
--rw-r--r--   0 thet      (1000) thet      (1000)     2288 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/Makefile
--rw-r--r--   0 thet      (1000) thet      (1000)    11382 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/changes.rst
--rw-r--r--   0 thet      (1000) thet      (1000)     5902 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/conf.py
--rw-r--r--   0 thet      (1000) thet      (1000)     2995 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/defence.rst
--rw-r--r--   0 thet      (1000) thet      (1000)      383 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/index.rst
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/docs/mapal/
--rw-r--r--   0 thet      (1000) thet      (1000)     1724 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/mapal/index.rst
--rw-r--r--   0 thet      (1000) thet      (1000)     4495 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/mapal/javascript.rst
--rw-r--r--   0 thet      (1000) thet      (1000)     7731 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/mapal/markup.rst
--rw-r--r--   0 thet      (1000) thet      (1000)    18487 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/mapal/pizza-other.png
--rw-r--r--   0 thet      (1000) thet      (1000)    13546 2023-01-04 13:07:45.000000 NuPlone-2.1.4/docs/mapal/pizza-unknown.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/
--rw-r--r--   0 thet      (1000) thet      (1000)       56 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/__init__.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/
--rw-r--r--   0 thet      (1000) thet      (1000)       92 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/__init__.py
--rw-r--r--   0 thet      (1000) thet      (1000)      812 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/auth.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/browser/
--rw-r--r--   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/__init__.py
--rw-r--r--   0 thet      (1000) thet      (1000)     2604 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/configure.zcml
--rw-r--r--   0 thet      (1000) thet      (1000)     3876 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/contact.py
--rw-r--r--   0 thet      (1000) thet      (1000)      414 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/helper.py
--rw-r--r--   0 thet      (1000) thet      (1000)     2760 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/login.py
--rw-r--r--   0 thet      (1000) thet      (1000)      795 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/ordering.py
--rw-r--r--   0 thet      (1000) thet      (1000)     7417 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/pwreminder.py
--rw-r--r--   0 thet      (1000) thet      (1000)     3123 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/settings.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/browser/templates/
--rw-r--r--   0 thet      (1000) thet      (1000)     1518 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/templates/editlink.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     2564 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/templates/login.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      908 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/templates/pwreset-email.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      621 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/browser/wysiwyg.py
--rw-r--r--   0 thet      (1000) thet      (1000)      852 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/configure.zcml
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/locales/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/bg/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/locales/bg/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    20049 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/bg/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/ca/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/locales/ca/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17522 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/ca/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/cs/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/locales/cs/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17519 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/cs/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/de/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/locales/de/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17810 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/de/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/el/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/locales/el/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    20535 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/el/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/es/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.385803 NuPlone-2.1.4/plonetheme/nuplone/locales/es/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17396 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/es/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/fi/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/fi/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17184 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/fi/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/fr/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/fr/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17590 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/fr/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/hr/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/hr/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    14408 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/hr/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/hu/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/hu/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17502 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/hu/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/is/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/is/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17666 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/is/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/it/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/it/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17293 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/it/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/lt/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/lt/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17334 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/lt/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/lv/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/lv/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17605 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/lv/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/mt/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/mt/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17238 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/mt/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/nl/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/nl/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17020 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/nl/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/nl_BE/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/nl_BE/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17456 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/nl_BE/LC_MESSAGES/nuplone.po
--rw-r--r--   0 thet      (1000) thet      (1000)    14383 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/nuplone.pot
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/pt/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/pt/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17277 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/pt/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/sk/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/sk/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17301 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/sk/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/sl/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/sl/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    17163 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/sl/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/locales/sv/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/locales/sv/LC_MESSAGES/
--rw-r--r--   0 thet      (1000) thet      (1000)    14227 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/locales/sv/LC_MESSAGES/nuplone.po
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.377803 NuPlone-2.1.4/plonetheme/nuplone/profiles/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/profiles/default/
--rw-r--r--   0 thet      (1000) thet      (1000)       68 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/profiles/default/metadata.xml
--rw-r--r--   0 thet      (1000) thet      (1000)       23 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/profiles/default/plonetheme.nuplone.txt
--rw-r--r--   0 thet      (1000) thet      (1000)      128 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/profiles/default/skins.xml
--rw-r--r--   0 thet      (1000) thet      (1000)     1059 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/setuphandlers.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.389803 NuPlone-2.1.4/plonetheme/nuplone/skin/
--rw-r--r--   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/__init__.py
--rw-r--r--   0 thet      (1000) thet      (1000)     4238 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/actions.py
--rw-r--r--   0 thet      (1000) thet      (1000)     4061 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/configure.zcml
--rw-r--r--   0 thet      (1000) thet      (1000)     1346 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/error.py
--rw-r--r--   0 thet      (1000) thet      (1000)      206 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/interfaces.py
--rw-r--r--   0 thet      (1000) thet      (1000)     1130 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/language.py
--rw-r--r--   0 thet      (1000) thet      (1000)     4605 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/sitemenu.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.393803 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/
--rw-r--r--   0 thet      (1000) thet      (1000)     1320 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/delete.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1167 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/dexterity.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      702 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/error_generic.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      784 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/error_notfound.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     2498 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/error_unauthorized.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      414 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/frontpage.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     2375 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/layout.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     3803 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/sitemenu.pt
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.381803 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.393803 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/
--rw-r--r--   0 thet      (1000) thet      (1000)    18366 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/ABADIMT0.eot
--rw-r--r--   0 thet      (1000) thet      (1000)    30812 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/Abadi-MT-Std-Condensed Light.otf
--rw-r--r--   0 thet      (1000) thet      (1000)      192 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/Makefile
--rw-r--r--   0 thet      (1000) thet      (1000)     3850 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/body.png
--rw-r--r--   0 thet      (1000) thet      (1000)      176 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/button-default.png
--rw-r--r--   0 thet      (1000) thet      (1000)     2849 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/button-warning.png
--rw-r--r--   0 thet      (1000) thet      (1000)    37967 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/flags.jpg
--rw-r--r--   0 thet      (1000) thet      (1000)     3220 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/graph-bars.png
--rw-r--r--   0 thet      (1000) thet      (1000)    69813 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/header.png
--rw-r--r--   0 thet      (1000) thet      (1000)     3934 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/icons.png
--rw-r--r--   0 thet      (1000) thet      (1000)      471 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/ie-globalNavigation.png
--rw-r--r--   0 thet      (1000) thet      (1000)     4764 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/ie-steps-deep.png
--rw-r--r--   0 thet      (1000) thet      (1000)     4777 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/ie-steps-deeper.png
--rw-r--r--   0 thet      (1000) thet      (1000)     6436 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/logo.png
--rw-r--r--   0 thet      (1000) thet      (1000)      652 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/marker.png
--rw-r--r--   0 thet      (1000) thet      (1000)     2020 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/mask.png
--rw-r--r--   0 thet      (1000) thet      (1000)      883 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/microns.gif
--rw-r--r--   0 thet      (1000) thet      (1000)     4270 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/microns.png
--rw-r--r--   0 thet      (1000) thet      (1000)     4712 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/riskBadge-high.png
--rw-r--r--   0 thet      (1000) thet      (1000)    57847 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/screen.css
--rw-r--r--   0 thet      (1000) thet      (1000)    45534 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/screen.min.css
--rw-r--r--   0 thet      (1000) thet      (1000)      634 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/steps.png
--rw-r--r--   0 thet      (1000) thet      (1000)    14730 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-deCornae.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.397803 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/
--rw-r--r--   0 thet      (1000) thet      (1000)      916 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-active.png
--rw-r--r--   0 thet      (1000) thet      (1000)      395 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-dimmed.png
--rw-r--r--   0 thet      (1000) thet      (1000)      753 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-inactive.png
--rw-r--r--   0 thet      (1000) thet      (1000)     1035 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-active.png
--rw-r--r--   0 thet      (1000) thet      (1000)      449 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-dimmed.png
--rw-r--r--   0 thet      (1000) thet      (1000)     1002 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-inactive.png
--rw-r--r--   0 thet      (1000) thet      (1000)      835 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-active.png
--rw-r--r--   0 thet      (1000) thet      (1000)      536 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-dimmed.png
--rw-r--r--   0 thet      (1000) thet      (1000)      823 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-inactive.png
--rw-r--r--   0 thet      (1000) thet      (1000)      818 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-active.png
--rw-r--r--   0 thet      (1000) thet      (1000)      360 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-dimmed.png
--rw-r--r--   0 thet      (1000) thet      (1000)      753 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-inactive.png
--rw-r--r--   0 thet      (1000) thet      (1000)      558 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-active.png
--rw-r--r--   0 thet      (1000) thet      (1000)      308 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-dimmed.png
--rw-r--r--   0 thet      (1000) thet      (1000)      537 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-inactive.png
--rw-r--r--   0 thet      (1000) thet      (1000)      758 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-active-left.png
--rw-r--r--   0 thet      (1000) thet      (1000)      557 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector-left.png
--rw-r--r--   0 thet      (1000) thet      (1000)      805 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector.png
--rw-r--r--   0 thet      (1000) thet      (1000)      758 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current-left.png
--rw-r--r--   0 thet      (1000) thet      (1000)     1063 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current.png
--rw-r--r--   0 thet      (1000) thet      (1000)      840 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-right.png
--rw-r--r--   0 thet      (1000) thet      (1000)      210 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tabs.png
--rw-r--r--   0 thet      (1000) thet      (1000)    13575 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-mobile.png
--rw-r--r--   0 thet      (1000) thet      (1000)    14519 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs.png
--rw-r--r--   0 thet      (1000) thet      (1000)    11733 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/wheel.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.397803 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/
--rw-r--r--   0 thet      (1000) thet      (1000)    22872 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/base.css
--rw-r--r--   0 thet      (1000) thet      (1000)    19155 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/body.jpg
--rw-r--r--   0 thet      (1000) thet      (1000)     8598 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask-inverted.png
--rw-r--r--   0 thet      (1000) thet      (1000)    75485 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.gif
--rw-r--r--   0 thet      (1000) thet      (1000)    69657 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.png
--rw-r--r--   0 thet      (1000) thet      (1000)    71607 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/flags.jpg
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.405804 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/
--rw-r--r--   0 thet      (1000) thet      (1000)    18204 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ABADIMT0.eot
--rw-r--r--   0 thet      (1000) thet      (1000)    30812 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/Abadi-MT-Std-Condensed-Light.otf
--rw-r--r--   0 thet      (1000) thet      (1000)   242920 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ITCPortagoCom.ttf
--rw-r--r--   0 thet      (1000) thet      (1000)   224908 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/OctaneLTCom-Regular.ttf
--rwxr-xr-x   0 thet      (1000) thet      (1000)    62580 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.eot
--rwxr-xr-x   0 thet      (1000) thet      (1000)    33880 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.woff
--rwxr-xr-x   0 thet      (1000) thet      (1000)   102525 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina-cufon.js
--rwxr-xr-x   0 thet      (1000) thet      (1000)    27296 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.eot
--rwxr-xr-x   0 thet      (1000) thet      (1000)    47135 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.svg
--rwxr-xr-x   0 thet      (1000) thet      (1000)    27088 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.ttf
--rwxr-xr-x   0 thet      (1000) thet      (1000)    17472 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.woff
--rw-r--r--   0 thet      (1000) thet      (1000)    45176 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/armalite.ttf
--rw-r--r--   0 thet      (1000) thet      (1000)    11412 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.eot
--rw-r--r--   0 thet      (1000) thet      (1000)    23120 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.ttf
--rw-r--r--   0 thet      (1000) thet      (1000)    11451 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.eot
--rw-r--r--   0 thet      (1000) thet      (1000)    16360 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.ttf
--rwxr-xr-x   0 thet      (1000) thet      (1000)   175526 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/itcportagocom.eot
--rw-r--r--   0 thet      (1000) thet      (1000)    23740 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/xero4.ttf
--rw-r--r--   0 thet      (1000) thet      (1000)     3504 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/header.png
--rw-r--r--   0 thet      (1000) thet      (1000)      652 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/marker.png
--rw-r--r--   0 thet      (1000) thet      (1000)     2020 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/mask.png
--rw-r--r--   0 thet      (1000) thet      (1000)     2473 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/osha-logo.png
--rw-r--r--   0 thet      (1000) thet      (1000)      171 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/pattern-published.png
--rw-r--r--   0 thet      (1000) thet      (1000)    11733 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/wheel.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.409804 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/
--rw-r--r--   0 thet      (1000) thet      (1000)    30385 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/base.css
--rw-r--r--   0 thet      (1000) thet      (1000)      326 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/button.png
--rw-r--r--   0 thet      (1000) thet      (1000)      161 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/editorBarButton.png
--rw-r--r--   0 thet      (1000) thet      (1000)      655 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/editorBarToggle.png
--rw-r--r--   0 thet      (1000) thet      (1000)      339 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconAbbreviation.png
--rw-r--r--   0 thet      (1000) thet      (1000)      315 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconAcronym.png
--rw-r--r--   0 thet      (1000) thet      (1000)      388 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconBehaviour.png
--rw-r--r--   0 thet      (1000) thet      (1000)      259 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconBlockquote.png
--rw-r--r--   0 thet      (1000) thet      (1000)      295 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconCitation.png
--rw-r--r--   0 thet      (1000) thet      (1000)      305 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconCite.png
--rw-r--r--   0 thet      (1000) thet      (1000)      158 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconColumn.png
--rw-r--r--   0 thet      (1000) thet      (1000)      140 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconCopy.png
--rw-r--r--   0 thet      (1000) thet      (1000)      410 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconCut.png
--rw-r--r--   0 thet      (1000) thet      (1000)      373 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconDOM.png
--rw-r--r--   0 thet      (1000) thet      (1000)      344 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconDelete.png
--rw-r--r--   0 thet      (1000) thet      (1000)      355 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconEdit.png
--rw-r--r--   0 thet      (1000) thet      (1000)      253 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconEmphasised.png
--rw-r--r--   0 thet      (1000) thet      (1000)      207 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconFilm.png
--rw-r--r--   0 thet      (1000) thet      (1000)      389 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconFindReplace.png
--rw-r--r--   0 thet      (1000) thet      (1000)      436 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconForm.png
--rw-r--r--   0 thet      (1000) thet      (1000)      174 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconGroup.png
--rw-r--r--   0 thet      (1000) thet      (1000)     3149 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconImage.png
--rw-r--r--   0 thet      (1000) thet      (1000)      170 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconIndent.png
--rw-r--r--   0 thet      (1000) thet      (1000)      389 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconInsert.png
--rw-r--r--   0 thet      (1000) thet      (1000)      424 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconLayout.png
--rw-r--r--   0 thet      (1000) thet      (1000)      346 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconLink.png
--rw-r--r--   0 thet      (1000) thet      (1000)      308 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconNavigation.png
--rw-r--r--   0 thet      (1000) thet      (1000)      534 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconNonBreakingSpace.png
--rw-r--r--   0 thet      (1000) thet      (1000)     2958 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconOrderedList.png
--rw-r--r--   0 thet      (1000) thet      (1000)      168 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconOutdent.png
--rw-r--r--   0 thet      (1000) thet      (1000)      351 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconParagraph.png
--rw-r--r--   0 thet      (1000) thet      (1000)      140 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconPaste.png
--rw-r--r--   0 thet      (1000) thet      (1000)      313 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconPasteWord.png
--rw-r--r--   0 thet      (1000) thet      (1000)      403 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconPreview.png
--rw-r--r--   0 thet      (1000) thet      (1000)      261 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconRemoveStyle.png
--rw-r--r--   0 thet      (1000) thet      (1000)      290 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconSeparator.png
--rw-r--r--   0 thet      (1000) thet      (1000)      315 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconStrong.png
--rw-r--r--   0 thet      (1000) thet      (1000)      323 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconSubscript.png
--rw-r--r--   0 thet      (1000) thet      (1000)      330 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconSuperscript.png
--rw-r--r--   0 thet      (1000) thet      (1000)      178 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconTable.png
--rw-r--r--   0 thet      (1000) thet      (1000)      435 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconTerminator.png
--rw-r--r--   0 thet      (1000) thet      (1000)      349 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconText.png
--rw-r--r--   0 thet      (1000) thet      (1000)      391 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconUnlink.png
--rw-r--r--   0 thet      (1000) thet      (1000)     2891 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconUnorderedList.png
--rw-r--r--   0 thet      (1000) thet      (1000)    58863 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/icons-bar.png
--rw-r--r--   0 thet      (1000) thet      (1000)     3250 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/icons.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.409804 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/
--rw-r--r--   0 thet      (1000) thet      (1000)    70228 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/base.css
--rw-r--r--   0 thet      (1000) thet      (1000)      470 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/dragHandle.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.409804 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/fonts/
--rw-r--r--   0 thet      (1000) thet      (1000)    18204 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/fonts/ABADIMT0.eot
--rw-r--r--   0 thet      (1000) thet      (1000)    45244 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/icons.png
--rw-r--r--   0 thet      (1000) thet      (1000)    16868 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/infoPanel.png
--rw-r--r--   0 thet      (1000) thet      (1000)     2511 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/logo.png
--rw-r--r--   0 thet      (1000) thet      (1000)      441 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/siteMenu-top.png
--rw-r--r--   0 thet      (1000) thet      (1000)      218 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/twistie.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.413804 NuPlone-2.1.4/plonetheme/nuplone/skin/tests/
--rw-r--r--   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/tests/__init__.py
--rw-r--r--   0 thet      (1000) thet      (1000)     5701 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/tests/test_adapter.py
--rw-r--r--   0 thet      (1000) thet      (1000)      978 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/tests/test_pwreminder.py
--rw-r--r--   0 thet      (1000) thet      (1000)     4855 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/tests/test_sitemenu.py
--rw-r--r--   0 thet      (1000) thet      (1000)     2372 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/skin/tools.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.381803 NuPlone-2.1.4/plonetheme/nuplone/static/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.417804 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/
--rw-r--r--   0 thet      (1000) thet      (1000)     7090 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/10a90e5b4dae60a0543c.png
--rw-r--r--   0 thet      (1000) thet      (1000)     4618 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/179bd5aaea5c09a81ce7.png
--rw-r--r--   0 thet      (1000) thet      (1000)     7074 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/364b30f1e5d0687013c7.png
--rw-r--r--   0 thet      (1000) thet      (1000)     4618 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/70aafb8ff880c9e56337.png
--rw-r--r--   0 thet      (1000) thet      (1000)     6487 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/79819eb79cf7bb39ee83.png
--rw-r--r--   0 thet      (1000) thet      (1000)   196021 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)   953948 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     7111 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/cafe1bc324140ea6562e.png
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.425804 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/
--rw-r--r--   0 thet      (1000) thet      (1000)     1418 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     4800 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1178 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     3897 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1429 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     4597 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1143 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     3088 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     2854 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     8798 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     6801 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)    22816 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1057 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     3422 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     2526 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     7652 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)      800 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     2573 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1024 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     2876 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     2562 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     7857 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)   266969 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)   856701 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     3202 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     8596 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1177 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     3812 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     2592 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     4921 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     2131 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     5179 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1233 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     3811 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1203 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     4335 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     1687 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     3957 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)     3071 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)     5451 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)   649724 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/oira.cms.min.js
--rw-r--r--   0 thet      (1000) thet      (1000)  1976442 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/oira.cms.min.js.map
--rw-r--r--   0 thet      (1000) thet      (1000)      419 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/static/bundle/polyfills-loader.js
--rw-r--r--   0 thet      (1000) thet      (1000)      783 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/testing.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.425804 NuPlone-2.1.4/plonetheme/nuplone/tiles/
--rw-r--r--   0 thet      (1000) thet      (1000)       48 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/__init__.py
--rw-r--r--   0 thet      (1000) thet      (1000)     1220 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/analytics.py
--rw-r--r--   0 thet      (1000) thet      (1000)     1815 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/configure.zcml
--rw-r--r--   0 thet      (1000) thet      (1000)     2266 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/group.py
--rw-r--r--   0 thet      (1000) thet      (1000)      718 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/language.py
--rw-r--r--   0 thet      (1000) thet      (1000)      466 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/messages.py
--rw-r--r--   0 thet      (1000) thet      (1000)     6915 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/navigation.py
--rw-r--r--   0 thet      (1000) thet      (1000)      301 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/static.py
--rw-r--r--   0 thet      (1000) thet      (1000)     2062 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/tabs.py
--rw-r--r--   0 thet      (1000) thet      (1000)      754 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/tales.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.425804 NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/
--rw-r--r--   0 thet      (1000) thet      (1000)     1009 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/analytics.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      333 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/group.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      899 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/language.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      397 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/messages.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      949 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/navigation.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      989 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/tabs.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1694 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/tiles/tile.py
--rw-r--r--   0 thet      (1000) thet      (1000)     6537 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/utils.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.429804 NuPlone-2.1.4/plonetheme/nuplone/z3cform/
--rw-r--r--   0 thet      (1000) thet      (1000)      202 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/__init__.py
--rw-r--r--   0 thet      (1000) thet      (1000)     5116 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/configure.zcml
--rw-r--r--   0 thet      (1000) thet      (1000)     5203 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/directives.py
--rw-r--r--   0 thet      (1000) thet      (1000)      503 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/form.py
--rw-r--r--   0 thet      (1000) thet      (1000)      170 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/interfaces.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.429804 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/
--rw-r--r--   0 thet      (1000) thet      (1000)     1126 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/checkbox_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1154 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/checkboxlist_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1539 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/date_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1538 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/datetime_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      197 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/error.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1996 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/form.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      674 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/layout.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      888 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/multi_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1258 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/namedfile_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1386 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/namedimage_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      805 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/object_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     5461 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/orderedselect_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      910 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/password_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1177 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/passwordconfirm_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1098 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/radio_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1091 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/select_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      255 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/submit_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1052 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/text_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      957 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/textarea_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      974 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/textlines_display.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      908 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/textlines_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     2088 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/wrappedform.pt
--rw-r--r--   0 thet      (1000) thet      (1000)     1209 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/wysiwyg_input.pt
--rw-r--r--   0 thet      (1000) thet      (1000)      991 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates.py
--rw-r--r--   0 thet      (1000) thet      (1000)      362 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/utils.py
--rw-r--r--   0 thet      (1000) thet      (1000)     4563 2023-01-04 13:07:45.000000 NuPlone-2.1.4/plonetheme/nuplone/z3cform/widget.py
--rw-r--r--   0 thet      (1000) thet      (1000)      235 2023-01-04 13:07:45.000000 NuPlone-2.1.4/pyproject.toml
--rw-r--r--   0 thet      (1000) thet      (1000)       62 2023-01-04 13:07:45.000000 NuPlone-2.1.4/requirements.txt
--rw-r--r--   0 thet      (1000) thet      (1000)       95 2023-01-04 13:07:46.433804 NuPlone-2.1.4/setup.cfg
--rw-r--r--   0 thet      (1000) thet      (1000)     1832 2023-01-04 13:07:45.000000 NuPlone-2.1.4/setup.py
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.381803 NuPlone-2.1.4/src/
-drwxr-xr-x   0 thet      (1000) thet      (1000)        0 2023-01-04 13:07:46.429804 NuPlone-2.1.4/src/nuplone_components/
--rw-r--r--   0 thet      (1000) thet      (1000)    18867 2023-01-04 13:07:45.000000 NuPlone-2.1.4/src/nuplone_components/behaviour.js
--rw-r--r--   0 thet      (1000) thet      (1000)     4068 2023-01-04 13:07:45.000000 NuPlone-2.1.4/src/nuplone_components/editlink.js
--rw-r--r--   0 thet      (1000) thet      (1000)      321 2023-01-04 13:07:45.000000 NuPlone-2.1.4/src/nuplone_components/ordering.js
--rw-r--r--   0 thet      (1000) thet      (1000)     8950 2023-01-04 13:07:45.000000 NuPlone-2.1.4/src/nuplone_components/z3cform.js
--rw-r--r--   0 thet      (1000) thet      (1000)      304 2023-01-04 13:07:45.000000 NuPlone-2.1.4/versions.cfg
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.978391 NuPlone-2.2.0/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      265 2023-06-14 14:57:41.000000 NuPlone-2.2.0/MANIFEST.in
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/NuPlone.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14476 2023-06-14 14:57:41.000000 NuPlone-2.2.0/NuPlone.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17936 2023-06-14 14:57:41.000000 NuPlone-2.2.0/NuPlone.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-14 14:57:41.000000 NuPlone-2.2.0/NuPlone.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2023-06-14 14:57:41.000000 NuPlone-2.2.0/NuPlone.egg-info/namespace_packages.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-14 14:57:41.000000 NuPlone-2.2.0/NuPlone.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      278 2023-06-14 14:57:41.000000 NuPlone-2.2.0/NuPlone.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2023-06-14 14:57:41.000000 NuPlone-2.2.0/NuPlone.egg-info/top_level.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14476 2023-06-14 14:57:41.978391 NuPlone-2.2.0/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1940 2023-06-14 14:57:41.000000 NuPlone-2.2.0/README.rst
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/docs/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/docs/.static/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      674 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/.static/logo.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1126 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/.static/plone.css
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2288 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11452 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/changes.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5878 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/conf.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2995 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/defence.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)      383 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/index.rst
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/docs/mapal/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1724 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/mapal/index.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4495 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/mapal/javascript.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7731 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/mapal/markup.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)    18487 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/mapal/pizza-other.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13546 2023-06-14 14:57:41.000000 NuPlone-2.2.0/docs/mapal/pizza-unknown.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/plonetheme/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       56 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/plonetheme/nuplone/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       92 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      807 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/auth.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/browser/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2604 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3856 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/contact.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      414 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/helper.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2757 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/login.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      778 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/ordering.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7385 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/pwreminder.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3106 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/settings.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/browser/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1518 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/templates/editlink.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2564 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/templates/login.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      908 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/templates/pwreset-email.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      620 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/browser/wysiwyg.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      852 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/configure.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/bg/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/bg/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    20049 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/bg/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/ca/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/ca/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17522 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/ca/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/cs/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/cs/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17519 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/cs/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/de/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/de/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17810 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/de/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/el/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/el/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    20535 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/el/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/es/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17396 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/es/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/fi/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/fi/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17184 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/fi/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/fr/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17590 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/fr/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/hr/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/hr/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14408 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/hr/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/hu/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/hu/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17502 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/hu/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/is/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/is/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17666 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/is/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/it/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17293 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/it/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/lt/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/lt/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17334 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/lt/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/lv/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/lv/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17605 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/lv/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/mt/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/mt/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17238 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/mt/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/nl/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17020 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/nl/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/nl_BE/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/nl_BE/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17456 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/nl_BE/LC_MESSAGES/nuplone.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14383 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/nuplone.pot
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/pt/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/pt/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17277 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/pt/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/sk/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/sk/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17301 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/sk/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/sl/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/sl/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17163 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/sl/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/locales/sv/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/locales/sv/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14227 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/locales/sv/LC_MESSAGES/nuplone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/profiles/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/profiles/default/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       68 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/profiles/default/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       23 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/profiles/default/plonetheme.nuplone.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      128 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/profiles/default/skins.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1044 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/setuphandlers.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.950391 NuPlone-2.2.0/plonetheme/nuplone/skin/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4226 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/actions.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4061 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1317 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/error.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      206 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/interfaces.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1130 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/language.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4590 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/sitemenu.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.954391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1320 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/delete.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1167 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/dexterity.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      702 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/error_generic.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      784 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/error_notfound.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2498 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/error_unauthorized.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      414 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/frontpage.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2375 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/layout.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3803 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/sitemenu.pt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.942391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.954391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    18366 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/ABADIMT0.eot
+-rw-rw-r--   0 ale       (1000) ale       (1000)    30812 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/Abadi-MT-Std-Condensed Light.otf
+-rw-rw-r--   0 ale       (1000) ale       (1000)      192 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3850 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/body.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      176 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/button-default.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2849 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/button-warning.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    37967 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/flags.jpg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3220 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/graph-bars.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    69813 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/header.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3934 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/icons.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      471 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/ie-globalNavigation.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4764 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/ie-steps-deep.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4777 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/ie-steps-deeper.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6436 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/logo.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      652 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/marker.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2020 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/mask.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      883 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/microns.gif
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4270 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/microns.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4712 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/riskBadge-high.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    57847 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/screen.css
+-rw-rw-r--   0 ale       (1000) ale       (1000)    45534 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/screen.min.css
+-rw-rw-r--   0 ale       (1000) ale       (1000)      634 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/steps.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14730 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-deCornae.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.958391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      916 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-active.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      395 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-dimmed.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      753 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-inactive.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1035 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-active.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      449 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-dimmed.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1002 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-inactive.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      835 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-active.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      536 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-dimmed.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      823 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-inactive.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      818 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-active.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      360 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-dimmed.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      753 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-inactive.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      558 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-active.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      308 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-dimmed.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      537 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-inactive.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      758 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-active-left.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      557 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector-left.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      805 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      758 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current-left.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1063 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      840 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-right.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      210 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tabs.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13575 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-mobile.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14519 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11733 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/wheel.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.958391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    22872 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/base.css
+-rw-rw-r--   0 ale       (1000) ale       (1000)    19155 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/body.jpg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8598 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask-inverted.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    75485 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.gif
+-rw-rw-r--   0 ale       (1000) ale       (1000)    69657 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    71607 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/flags.jpg
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.958391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    18204 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ABADIMT0.eot
+-rw-rw-r--   0 ale       (1000) ale       (1000)    30812 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/Abadi-MT-Std-Condensed-Light.otf
+-rw-rw-r--   0 ale       (1000) ale       (1000)   242920 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ITCPortagoCom.ttf
+-rw-rw-r--   0 ale       (1000) ale       (1000)   224908 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/OctaneLTCom-Regular.ttf
+-rwxrwxr-x   0 ale       (1000) ale       (1000)    62580 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.eot
+-rwxrwxr-x   0 ale       (1000) ale       (1000)    33880 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.woff
+-rwxrwxr-x   0 ale       (1000) ale       (1000)   102525 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina-cufon.js
+-rwxrwxr-x   0 ale       (1000) ale       (1000)    27296 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.eot
+-rwxrwxr-x   0 ale       (1000) ale       (1000)    47135 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.svg
+-rwxrwxr-x   0 ale       (1000) ale       (1000)    27088 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.ttf
+-rwxrwxr-x   0 ale       (1000) ale       (1000)    17472 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.woff
+-rw-rw-r--   0 ale       (1000) ale       (1000)    45176 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/armalite.ttf
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11412 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.eot
+-rw-rw-r--   0 ale       (1000) ale       (1000)    23120 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.ttf
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11451 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.eot
+-rw-rw-r--   0 ale       (1000) ale       (1000)    16360 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.ttf
+-rwxrwxr-x   0 ale       (1000) ale       (1000)   175526 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/itcportagocom.eot
+-rw-rw-r--   0 ale       (1000) ale       (1000)    23740 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/xero4.ttf
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3504 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/header.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      652 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/marker.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2020 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/mask.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2473 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/osha-logo.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      171 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/pattern-published.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11733 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/wheel.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.962391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    30385 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/base.css
+-rw-rw-r--   0 ale       (1000) ale       (1000)      326 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/button.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      161 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/editorBarButton.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      655 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/editorBarToggle.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      339 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconAbbreviation.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      315 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconAcronym.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      388 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconBehaviour.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      259 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconBlockquote.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      295 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconCitation.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      305 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconCite.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      158 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconColumn.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      140 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconCopy.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      410 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconCut.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      373 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconDOM.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      344 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconDelete.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      355 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconEdit.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      253 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconEmphasised.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      207 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconFilm.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      389 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconFindReplace.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      436 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconForm.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      174 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconGroup.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3149 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconImage.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      170 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconIndent.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      389 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconInsert.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      424 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconLayout.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      346 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconLink.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      308 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconNavigation.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      534 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconNonBreakingSpace.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2958 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconOrderedList.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      168 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconOutdent.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      351 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconParagraph.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      140 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconPaste.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      313 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconPasteWord.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      403 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconPreview.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      261 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconRemoveStyle.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      290 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconSeparator.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      315 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconStrong.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      323 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconSubscript.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      330 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconSuperscript.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      178 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconTable.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      435 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconTerminator.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      349 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconText.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      391 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconUnlink.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2891 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconUnorderedList.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    58863 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/icons-bar.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3250 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/icons.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.966391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    70228 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/base.css
+-rw-rw-r--   0 ale       (1000) ale       (1000)      470 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/dragHandle.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.966391 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/fonts/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    18204 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/fonts/ABADIMT0.eot
+-rw-rw-r--   0 ale       (1000) ale       (1000)    45244 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/icons.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)    16868 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/infoPanel.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2511 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/logo.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      441 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/siteMenu-top.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)      218 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/twistie.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.966391 NuPlone-2.2.0/plonetheme/nuplone/skin/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/tests/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5576 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/tests/test_adapter.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1452 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/tests/test_pwreminder.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3746 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/tests/test_sitemenu.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2357 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/skin/tools.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/plonetheme/nuplone/static/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.970391 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7090 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/10a90e5b4dae60a0543c.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4618 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/179bd5aaea5c09a81ce7.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7074 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/364b30f1e5d0687013c7.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4618 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/70aafb8ff880c9e56337.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6487 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/79819eb79cf7bb39ee83.png
+-rw-rw-r--   0 ale       (1000) ale       (1000)   196021 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)   953948 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7111 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/cafe1bc324140ea6562e.png
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.974391 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1418 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4800 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1178 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3897 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1429 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4597 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1143 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3088 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2854 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8798 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6801 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)    22816 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1057 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3422 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2526 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7652 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)      800 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2573 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1024 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2876 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2562 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7857 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)   266969 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)   856701 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3202 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8596 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1177 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3812 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2592 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4921 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2131 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5179 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1233 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3811 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1203 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4335 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1687 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3957 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3071 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5451 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)   649724 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/oira.cms.min.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)  1976442 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/oira.cms.min.js.map
+-rw-rw-r--   0 ale       (1000) ale       (1000)      419 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/static/bundle/polyfills-loader.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)      768 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/testing.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.974391 NuPlone-2.2.0/plonetheme/nuplone/tiles/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       48 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1220 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/analytics.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1815 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2258 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/group.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      718 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/language.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      466 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/messages.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6846 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/navigation.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      301 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/static.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2047 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/tabs.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      734 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/tales.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.974391 NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1009 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/analytics.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      333 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/group.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      899 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/language.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      397 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/messages.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      949 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/navigation.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      989 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/tabs.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1670 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/tiles/tile.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6478 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/utils.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.974391 NuPlone-2.2.0/plonetheme/nuplone/z3cform/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      202 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5116 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5115 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/directives.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      476 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/form.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      170 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/interfaces.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.978391 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1126 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/checkbox_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1154 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/checkboxlist_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1539 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/date_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1538 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/datetime_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      197 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/error.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1996 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/form.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      674 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/layout.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      888 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/multi_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1258 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/namedfile_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1386 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/namedimage_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      805 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/object_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5461 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/orderedselect_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      910 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/password_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1177 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/passwordconfirm_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1098 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/radio_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1091 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/select_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      255 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/submit_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1052 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/text_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      957 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/textarea_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      974 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/textlines_display.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      908 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/textlines_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2088 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/wrappedform.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1209 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/wysiwyg_input.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      991 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      362 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/utils.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4487 2023-06-14 14:57:41.000000 NuPlone-2.2.0/plonetheme/nuplone/z3cform/widget.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      235 2023-06-14 14:57:41.000000 NuPlone-2.2.0/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       24 2023-06-14 14:57:41.000000 NuPlone-2.2.0/requirements.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       95 2023-06-14 14:57:41.978391 NuPlone-2.2.0/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2017 2023-06-14 14:57:41.000000 NuPlone-2.2.0/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.946391 NuPlone-2.2.0/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-14 14:57:41.978391 NuPlone-2.2.0/src/nuplone_components/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    18867 2023-06-14 14:57:41.000000 NuPlone-2.2.0/src/nuplone_components/behaviour.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4068 2023-06-14 14:57:41.000000 NuPlone-2.2.0/src/nuplone_components/editlink.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)      321 2023-06-14 14:57:41.000000 NuPlone-2.2.0/src/nuplone_components/ordering.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8950 2023-06-14 14:57:41.000000 NuPlone-2.2.0/src/nuplone_components/z3cform.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)       89 2023-06-14 14:57:41.000000 NuPlone-2.2.0/versions.cfg
```

### Comparing `NuPlone-2.1.4/NuPlone.egg-info/SOURCES.txt` & `NuPlone-2.2.0/NuPlone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/README.rst` & `NuPlone-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/.static/logo.png` & `NuPlone-2.2.0/docs/.static/logo.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/.static/plone.css` & `NuPlone-2.2.0/docs/.static/plone.css`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/Makefile` & `NuPlone-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/changes.rst` & `NuPlone-2.2.0/docs/changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.2.0 (2023-06-14)
+------------------
+
+- Support Plone 6
+  [ale-rt]
+
+
 2.1.4 (2023-01-04)
 ------------------
 
 - Sitemenu: Add a helper method to add submenus to existing categories.
   [thet]
 - Update pre-commit config.
   [thet]
```

### Comparing `NuPlone-2.1.4/docs/conf.py` & `NuPlone-2.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # repoze.atemplate documentation build configuration file
 #
 # This file is execfile()d with the current directory set to its containing
 # dir.
 #
 # The contents of this file are pickled, so don't put values in the
```

### Comparing `NuPlone-2.1.4/docs/defence.rst` & `NuPlone-2.2.0/docs/defence.rst`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/mapal/index.rst` & `NuPlone-2.2.0/docs/mapal/index.rst`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/mapal/javascript.rst` & `NuPlone-2.2.0/docs/mapal/javascript.rst`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/mapal/markup.rst` & `NuPlone-2.2.0/docs/mapal/markup.rst`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/mapal/pizza-other.png` & `NuPlone-2.2.0/docs/mapal/pizza-other.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/docs/mapal/pizza-unknown.png` & `NuPlone-2.2.0/docs/mapal/pizza-unknown.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/auth.py` & `NuPlone-2.2.0/plonetheme/nuplone/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from Products.PluggableAuthService.interfaces.plugins import IChallengePlugin
 from Products.PluggableAuthService.plugins.BasePlugin import BasePlugin
 from zope.interface import implementer
 
 
 @implementer(IChallengePlugin)
 class LoginChallenger(BasePlugin):
-    """Simple login challenger which does nothing, allowing the
-    Unauthorized exception view to be used instead.
-    """
+    """Simple login challenger which does nothing, allowing the Unauthorized
+    exception view to be used instead."""
 
     meta_type = "NuPlone Login Challenger"
     id = "nuplone-challenger"
 
     def challenge(self, request, response):
         if not NuPloneSkin.providedBy(request):
             return False
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/configure.zcml` & `NuPlone-2.2.0/plonetheme/nuplone/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/contact.py` & `NuPlone-2.2.0/plonetheme/nuplone/browser/contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from Products.statusmessages.interfaces import IStatusMessage
 from z3c.form import form
 from z3c.form.button import buttonAndHandler
 from zope import schema
 from zope.i18n import translate
 
 import logging
-import socket
 
 
 log = logging.getLogger(__name__)
 
 TextSpan7 = FieldWidgetFactory("z3c.form.browser.text.TextFieldWidget", klass="span-7")
 TextLines4Rows = FieldWidgetFactory(
     "z3c.form.browser.textlines.TextLinesFieldWidget", rows=4
@@ -45,15 +44,14 @@
     message = schema.Text(
         title=_("label_contact_text", default="Your message"), required=True
     )
     directives.widget(message="plonetheme.nuplone.browser.contact.TextLines4Rows")
 
 
 class ContactForm(AutoExtensibleForm, form.Form):
-
     ignoreContext = True
     schema = IContact
     label = _("header_contact", default="Contact")
     default_fieldset_label = None
 
     @property
     def email_from_name(self):
@@ -97,15 +95,15 @@
                 _(
                     "error_contactmail",
                     "An error occured while processing your contact request. Please try again later.",  # noqa: E501
                 ),
                 "error",
             )
             return
-        except socket.error as e:
+        except OSError as e:
             log.error(
                 "Socket error sending contact form for %s: %s", data["email"], e[1]
             )
             flash(
                 _(
                     "error_contactmail",
                     "An error occured while processing your contact request. Please try again later.",  # noqa: E501
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/login.py` & `NuPlone-2.2.0/plonetheme/nuplone/browser/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 
 log = logging.getLogger(__name__)
 
 
 class Login(BrowserView):
     def homeUrl(self, user):
-        """Return a suitable `home' for a user if came_from is unset or invalid."""
+        """Return a suitable `home' for a user if came_from is unset or
+        invalid."""
         put = getToolByName(self.context, "portal_url")
         return put.getPortalObject().absolute_url()
 
     def update(self):
         user = getSecurityManager().getUser()
         self.came_from = self.request.get("came_from")
         if not self.came_from:
@@ -47,15 +48,15 @@
             next = self.came_from or self.homeUrl(user)
             self.request.response.redirect(next)
 
         self.failed = self.anonymous and "login_attempt" in self.request
 
     def __call__(self):
         self.update()
-        return super(Login, self).__call__()
+        return super().__call__()
 
 
 class Logout(BrowserView):
     def __call__(self):
         flash = IStatusMessage(self.request).addStatusMessage
         if not isAnonymous():
             mt = getToolByName(self.context, "portal_membership")
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/pwreminder.py` & `NuPlone-2.2.0/plonetheme/nuplone/browser/pwreminder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from Acquisition import aq_inner
 from plone import api
 from plone.autoform.form import AutoExtensibleForm
 from plone.supermodel import model
 from plonetheme.nuplone import MessageFactory as _
 from plonetheme.nuplone.utils import createEmailTo
 from Products.CMFCore.utils import getToolByName
@@ -13,15 +12,14 @@
 from Products.statusmessages.interfaces import IStatusMessage
 from z3c.form import form
 from z3c.form.button import buttonAndHandler
 from zope import schema
 from zope.i18n import translate
 
 import logging
-import socket
 
 
 log = logging.getLogger(__name__)
 
 
 class IRequestPasswordReset(model.Schema):
     login = schema.TextLine(title=_("label_login", default="Login"), required=True)
@@ -32,15 +30,14 @@
 
     password = schema.Password(
         title=_("label_password", default="Password"), required=True
     )
 
 
 class RequestPasswordForm(AutoExtensibleForm, form.Form):
-
     email_template = ViewPageTemplateFile("templates/pwreset-email.pt")
 
     ignoreContext = True
     schema = IRequestPasswordReset
     label = _("header_password_reset_request", default="Reset password")
     default_fieldset_label = None
     description = _(
@@ -87,15 +84,15 @@
                 "error",
             )
             return
 
         ppr = getToolByName(self.context, "portal_password_reset")
         reset = ppr.requestReset(user.getId())
         portal_url = aq_inner(self.context).absolute_url()
-        reset_url = "%s/@@reset-password/%s" % (portal_url, reset["randomstring"])
+        reset_url = "{}/@@reset-password/{}".format(portal_url, reset["randomstring"])
 
         data["site"] = self.context.title
         subject = _(
             "password_reset_subject",
             default="Password reset for ${site}",
             mapping=data,
         )
@@ -124,15 +121,15 @@
                 _(
                     "error_contactmail",
                     "An error occured while processing your contact request. Please try again later.",  # noqa: E501
                 ),
                 "error",
             )
             return
-        except socket.error as e:
+        except OSError as e:
             log.error(
                 "Socket error sending password reset form to: %s", email_address, e[1]
             )
             flash(
                 _(
                     "error_contactmail",
                     "An error occured while processing your contact request. Please try again later.",  # noqa: E501
@@ -148,15 +145,14 @@
             ),
             "success",
         )
         self.request.response.redirect(portal_url)
 
 
 class PasswordReset(AutoExtensibleForm, form.Form):
-
     randomstring = None
 
     ignoreContext = True
     schema = IPasswordReset
     label = _("header_password_reset", default="Reset password")
     description = _(
         "intro_password_reset",
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/settings.py` & `NuPlone-2.2.0/plonetheme/nuplone/browser/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     password = schema.Password(
         title=_("label_password", default="Password"), required=True
     )
 
 
 @adapter(IPropertiedUser, IField)
 @implementer(IDataManager)
-class UserPropertyDataManager(object):
+class UserPropertyDataManager:
     def __init__(self, user, field):
         self.user = user
         self.field = field
         self.propname = field.__name__
         for sheet_id in user.listPropertysheets():
             sheet = user.getPropertysheet(sheet_id)
             if sheet.hasProperty(self.propname):
@@ -61,15 +61,15 @@
 
     def canWrite(self):
         return self.propname is not None
 
 
 @adapter(IPropertiedUser, IPassword)
 @implementer(IDataManager)
-class UserPasswordDataManager(object):
+class UserPasswordDataManager:
     def __init__(self, user, field):
         self.user = user
         self.field = field
 
     def get(self):
         raise AttributeError(self.field.__name__)
 
@@ -95,12 +95,11 @@
         return False
 
     def canWrite(self):
         return True
 
 
 class Settings(AutoExtensibleForm, form.EditForm):
-
     schema = ISettings
 
     def getContent(self):
         return getSecurityManager().getUser()
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/templates/editlink.pt` & `NuPlone-2.2.0/plonetheme/nuplone/browser/templates/editlink.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/templates/login.pt` & `NuPlone-2.2.0/plonetheme/nuplone/browser/templates/login.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/templates/pwreset-email.pt` & `NuPlone-2.2.0/plonetheme/nuplone/browser/templates/pwreset-email.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/browser/wysiwyg.py` & `NuPlone-2.2.0/plonetheme/nuplone/browser/wysiwyg.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,10 +12,9 @@
 
     new_window = schema.Bool(
         title=_("label_new_window", default="Open link in new window"), default=True
     )
 
 
 class EditLink(AutoExtensibleForm, form.EditForm):
-
     ignoreContext = True
     schema = ExternalLinkSchema
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/configure.zcml` & `NuPlone-2.2.0/plonetheme/nuplone/configure.zcml`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/bg/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/bg/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/ca/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/ca/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/cs/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/cs/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/de/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/de/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/el/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/el/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/es/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/es/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/fi/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/fi/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/fr/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/fr/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/hr/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/hr/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/hu/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/hu/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/is/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/is/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/it/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/it/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/lt/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/lt/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/lv/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/lv/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/mt/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/mt/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/nl/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/nl/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/nl_BE/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/nl_BE/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/nuplone.pot` & `NuPlone-2.2.0/plonetheme/nuplone/locales/nuplone.pot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/pt/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/pt/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/sk/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/sk/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/sl/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/sl/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/locales/sv/LC_MESSAGES/nuplone.po` & `NuPlone-2.2.0/plonetheme/nuplone/locales/sv/LC_MESSAGES/nuplone.po`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/setuphandlers.py` & `NuPlone-2.2.0/plonetheme/nuplone/setuphandlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from plone import api
 from plonetheme.nuplone.auth import LoginChallenger
 
 import logging
 
 
 log = logging.getLogger(__name__)
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/actions.py` & `NuPlone-2.2.0/plonetheme/nuplone/skin/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,8 +119,8 @@
         container = aq_parent(context)
 
         if not self.verify(container, context):
             return
 
         if self.request.method == "POST":
             return self.post()
-        return super(Delete, self).__call__()
+        return super().__call__()
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/configure.zcml` & `NuPlone-2.2.0/plonetheme/nuplone/skin/configure.zcml`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/error.py` & `NuPlone-2.2.0/plonetheme/nuplone/skin/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         if IBrowserView.providedBy(context):
             # NotFound errors can have extra aq wrapping
             self.context = context = aq_parent(context)
         log.debug("%r -> %r", self.exception, context)
 
     def __call__(self):
         self.update()
-        return super(Error, self).__call__()
+        return super().__call__()
 
 
 class Unauthorized(Error):
     def authenticate(self):
         """Try to authenticate the user manually, since ZPublisher dropped the
         user when it failed to validate access."""
         for parent in aq_chain(aq_inner(self.context)):
@@ -35,9 +35,9 @@
                 uf = parent.acl_users
                 try:
                     return uf.validate(self.request, None, roles=["Anonymous"])
                 except zExceptions.Unauthorized:
                     pass
 
     def update(self):
-        super(Unauthorized, self).update()
+        super().update()
         self.authenticate()
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/language.py` & `NuPlone-2.2.0/plonetheme/nuplone/skin/language.py`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/sitemenu.py` & `NuPlone-2.2.0/plonetheme/nuplone/skin/sitemenu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from Acquisition import aq_inner
 from OFS.interfaces import ICopyContainer
 from plone import api
 from plone.memoize.view import memoize_contextless
 from plone.protect.utils import addTokenToUrl
 from plonetheme.nuplone import MessageFactory as _
 from plonetheme.nuplone.utils import getFactoriesInContext
@@ -53,14 +52,15 @@
         if children:
             return menu
         else:
             return None
 
     def factories(self):
         """Helper method to generate the menu items for creating new content.
+
         If no content can be created None is returned.
         """
         menu = {"title": _("menu_add_new", default="Add new")}
         children = menu["children"] = []
         actions = getFactoriesInContext(self.context)
         actions.sort(key=lambda x: x.title)
         for action in actions:
@@ -92,15 +92,14 @@
         ec = pa._getExprContext(context)
         actions = [ActionInfo(action, ec) for action in actions]
 
         menu = {"title": _("menu_organise", default="Organise")}
         children = menu["children"] = []
         for a in actions:
             if a["visible"] and a["allowed"] and a["available"] and not is_root:
-
                 if a["id"] == "copy" and context.cb_isCopyable():
                     children.append(
                         {
                             "title": _("menu_copy", default="Copy"),
                             "url": "%s/@@copy" % context_url,
                         }
                     )
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/delete.pt` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/delete.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/dexterity.pt` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/dexterity.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/error_generic.pt` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/error_generic.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/error_notfound.pt` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/error_notfound.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/error_unauthorized.pt` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/error_unauthorized.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/layout.pt` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/sitemenu.pt` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/sitemenu.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/ABADIMT0.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/ABADIMT0.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/Abadi-MT-Std-Condensed Light.otf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/Abadi-MT-Std-Condensed Light.otf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/body.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/body.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/button-warning.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/button-warning.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/flags.jpg` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/flags.jpg`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/graph-bars.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/graph-bars.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/header.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/header.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/icons.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/icons.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/ie-steps-deep.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/ie-steps-deep.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/ie-steps-deeper.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/ie-steps-deeper.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/logo.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/logo.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/marker.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/marker.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/mask.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/mask.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/microns.gif` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/microns.gif`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/microns.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/microns.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/riskBadge-high.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/riskBadge-high.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/screen.css` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/screen.css`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/screen.min.css` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/screen.min.css`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/steps.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/steps.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-deCornae.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-deCornae.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-active.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-active.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-inactive.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-1-inactive.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-active.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-active.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-inactive.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-2-inactive.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-active.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-active.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-dimmed.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-dimmed.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-inactive.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-3-inactive.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-active.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-active.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-inactive.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-4-inactive.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-active.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-active.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-inactive.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/step-5-inactive.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-active-left.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-active-left.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector-left.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector-left.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-connector.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current-left.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current-left.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-current.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-right.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-ie6/tab-right.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs-mobile.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs-mobile.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/tabs.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/tabs.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/client/wheel.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/client/wheel.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/base.css` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/base.css`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/body.jpg` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/body.jpg`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask-inverted.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask-inverted.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.gif` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.gif`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/colour-preview-mask.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/flags.jpg` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/flags.jpg`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ABADIMT0.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ABADIMT0.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/Abadi-MT-Std-Condensed-Light.otf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/Abadi-MT-Std-Condensed-Light.otf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ITCPortagoCom.ttf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/ITCPortagoCom.ttf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/OctaneLTCom-Regular.ttf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/OctaneLTCom-Regular.ttf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.woff` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/abadimtstdcondensed_light.woff`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina-cufon.js` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina-cufon.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.svg` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.svg`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.ttf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.ttf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.woff` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/angelina.woff`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/armalite.ttf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/armalite.ttf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.ttf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/boston.ttf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.ttf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/carbon.ttf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/itcportagocom.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/itcportagocom.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/fonts/xero4.ttf` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/fonts/xero4.ttf`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/header.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/header.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/marker.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/marker.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/mask.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/mask.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/osha-logo.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/osha-logo.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/euphorie/wheel.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/euphorie/wheel.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/base.css` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/base.css`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/editorBarToggle.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/editorBarToggle.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconImage.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconImage.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconNonBreakingSpace.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconNonBreakingSpace.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconOrderedList.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconOrderedList.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/iconUnorderedList.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/iconUnorderedList.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/icons-bar.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/icons-bar.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/form/icons.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/form/icons.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/base.css` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/base.css`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/fonts/ABADIMT0.eot` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/fonts/ABADIMT0.eot`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/icons.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/icons.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/infoPanel.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/infoPanel.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/templates/style/main/logo.png` & `NuPlone-2.2.0/plonetheme/nuplone/skin/templates/style/main/logo.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/tests/test_adapter.py` & `NuPlone-2.2.0/plonetheme/nuplone/skin/tests/test_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-# -*- coding: UTF-8 -*-
-""" StatusMessage adapter tests.
-"""
+"""StatusMessage adapter tests."""
 from plonetheme.nuplone.testing import NUPLONE_INTEGRATION_TESTING
 from Products.statusmessages.interfaces import IStatusMessage
 from unittest import TestCase
 
-import six
-
 
 class TestHTMLStatusMessages(TestCase):
     layer = NUPLONE_INTEGRATION_TESTING
 
     def testAdapter(self):
-        """Test status messages
-        First some boilerplate.
-        """
+        """Test status messages First some boilerplate."""
         request = self.layer["request"].clone()
 
         # Now lets make sure we can actually adapt the request.
         status = IStatusMessage(request)
         self.assertTrue(IStatusMessage.providedBy(status))
 
         # Make sure there's no stored message.
@@ -99,76 +93,76 @@
 
         # And check the results again
         messages = status.show()
         self.assertEqual(len(messages), 1)
         test = messages[0]
         self.assertEqual(test.type, "success")
         self.assertEqual(test.message, "test")
-        self.assertIsInstance(test.message, six.text_type)
+        self.assertIsInstance(test.message, str)
 
         # Add two HTML messages
         status.add("test", type="info")
         status.add("test1", "warn")
 
         # And check the results again
         messages = status.show()
         self.assertEqual(len(messages), 2)
         test = messages[1]
         self.assertEqual(test.message, "test1")
-        self.assertIsInstance(test.message, six.text_type)
+        self.assertIsInstance(test.message, str)
         self.assertEqual(test.type, "warn")
 
         # add two identical messages
         status.add("test", type="info")
         status.add("test", type="info")
 
         # And check the results again
         messages = status.show()
         self.assertEqual(len(messages), 1)
         test = messages[0]
         self.assertEqual(test.message, "test")
-        self.assertIsInstance(test.message, six.text_type)
+        self.assertIsInstance(test.message, str)
         self.assertEqual(test.type, "info")
 
         # Make sure messages are removed again
         self.assertEqual(len(status.show()), 0)
 
         # Test incredibly long messages:
         status.add("m" * 0x400, type="t" * 0x20)
 
         # And check the results again
         messages = status.show()
         self.assertEqual(len(messages), 1)
 
         test = messages[0]
-        self.assertIsInstance(test.message, six.text_type)
+        self.assertIsInstance(test.message, str)
         assert test.message == "%s" % ("m" * 0x3FF)
         assert test.type == "t" * 0x1F
 
         # Add two mixed messages
         status.add("test", type="info")
         status.add("test1", "warn")
 
         # And check the results again
         messages = status.show()
         self.assertEqual(len(messages), 2)
         test = messages[0]
         self.assertEqual(test.message, "test")
-        self.assertIsInstance(test.message, six.text_type)
+        self.assertIsInstance(test.message, str)
         self.assertEqual(test.type, "info")
 
         test = messages[1]
         self.assertEqual(test.message, "test1")
-        self.assertIsInstance(test.message, six.text_type)
+        self.assertIsInstance(test.message, str)
         self.assertEqual(test.type, "warn")
 
         # Add a more complicated html message
         status.add('You can go <a href="http://plone.org">here</a>.', type="success")
         messages = status.show()
         self.assertEqual(len(messages), 1)
         test = messages[0]
         self.assertEqual(test.type, "success")
         self.assertEqual(
             test.message,
             'You can go <a href="http://plone.org">here</a>.',  # noqa: E501
         )
-        self.assertIsInstance(test.message, six.text_type)
+        self.assertIsInstance(test.message, str)
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/tests/test_pwreminder.py` & `NuPlone-2.2.0/plonetheme/nuplone/skin/tests/test_pwreminder.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,19 +11,29 @@
         browser = Browser(self.layer["app"])
         browser.open("%s/reset-password" % self.layer["portal"].absolute_url())
         browser.getForm("form").submit()
 
     def testInvalidKey(self):
         from zExceptions import NotFound
 
-        browser = Browser(self.layer["app"])
-        browser.handleErrors = False
-        url = "%s/reset-password/bogus" % self.layer["portal"].absolute_url()
-        self.assertRaises(NotFound, browser.open, url)
+        # The browser tests was replaced because of this issue:
+        # - https://github.com/plone/plone.testing/issues/83
+        #
+        # browser = Browser(self.layer["app"])
+        # browser.handleErrors = False
+        # url = "%s/reset-password/bogus" % self.layer["portal"].absolute_url()
+        with self.assertRaises(NotFound):
+            self.layer["portal"].restrictedTraverse("reset-password/bogus")
+            # browser.open(url)
 
     def testDoubleKeys(self):
         from zExceptions import NotFound
 
-        browser = Browser(self.layer["app"])
-        browser.handleErrors = False
-        url = "%s/reset-password/one/two" % self.layer["portal"].absolute_url()
-        self.assertRaises(NotFound, browser.open, url)
+        # The browser tests was replaced because of this issue:
+        # - https://github.com/plone/plone.testing/issues/83
+        #
+        # browser = Browser(self.layer["app"])
+        # browser.handleErrors = False
+        # url = "%s/reset-password/one/two" % self.layer["portal"].absolute_url()
+        with self.assertRaises(NotFound):
+            self.layer["portal"].restrictedTraverse("reset-password/one/two")
+            # browser.open(url)
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/skin/tools.py` & `NuPlone-2.2.0/plonetheme/nuplone/skin/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from AccessControl import getSecurityManager
 from Acquisition import aq_inner
 from plone import api
 from plone.memoize.view import memoize
 from plonetheme.nuplone import utils
 from Products.Five import BrowserView
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/10a90e5b4dae60a0543c.png` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/10a90e5b4dae60a0543c.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/179bd5aaea5c09a81ce7.png` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/179bd5aaea5c09a81ce7.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/364b30f1e5d0687013c7.png` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/364b30f1e5d0687013c7.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/70aafb8ff880c9e56337.png` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/70aafb8ff880c9e56337.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/79819eb79cf7bb39ee83.png` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/79819eb79cf7bb39ee83.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/bundle-polyfills.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/cafe1bc324140ea6562e.png` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/cafe1bc324140ea6562e.png`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/0.6cd4bd8c9badab61e723.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/10.d3b9daf3777a30698a00.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/105.97839df18a1eeb8afda4.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/185.75309d0f2aaac3951ba7.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/192.d30d22e53eef6912d1d3.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/212.6f700803cc744806f3ba.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/213.a24118cf28e2543d8b8c.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/306.6385c1b15fd80fbec1ec.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/383.59451bfe6594a5fc7d7a.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/399.0a533a588aa6f97bc0ce.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/482.cee2a3e4ce58de143547.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/550.ef690a33152a657ff0c8.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/591.7ad59dcd87be54cf1b7f.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/665.ffdbd9f6ed646a399ac6.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/765.5cc7dd7a3ce2a5af6f16.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/827.f862ea928a93cedd300d.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/830.e910cc96eb9ff827ea27.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/882.6b2ae75a9cadf6be92d4.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/883.292258a70c71e1e6ead0.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/chunks/920.626b78b07ce9d1b9cc2c.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/oira.cms.min.js` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/oira.cms.min.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/static/bundle/oira.cms.min.js.map` & `NuPlone-2.2.0/plonetheme/nuplone/static/bundle/oira.cms.min.js.map`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/testing.py` & `NuPlone-2.2.0/plonetheme/nuplone/testing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneWithPackageLayer
 
 import plonetheme.nuplone
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/analytics.py` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/analytics.py`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/configure.zcml` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/group.py` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,9 +59,9 @@
             if config.get("id"):
                 prefix.append(' id="%s"' % config["id"])
             if config.get("class"):
                 prefix.append(' class="%s"' % config["class"])
             prefix.append(">")
             prefix = "".join(prefix)
             postfix = "</%s>" % wrapper
-            result = "%s%s%s" % (prefix, result, postfix)
+            result = f"{prefix}{result}{postfix}"
         return result
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/language.py` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/language.py`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/navigation.py` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from plone import api
 from plone.i18n.normalizer.interfaces import IIDNormalizer
 from plone.tiles import Tile
 from plonetheme.nuplone.utils import getNavigationRoot
 from Products.CMFCore.utils import getToolByName
@@ -20,15 +19,15 @@
 class INavtreeFactory(Interface):
     """Marker interface for catalog builder functions."""
 
     def __call__(context, request):
         """Return a CatalogNavTree instance."""
 
 
-class CatalogNavTree(object):
+class CatalogNavTree:
     def __init__(self, context, request):
         self.build(context, request)
 
     def build(self, context, request):
         context = aq_inner(context)
 
         # If we are at a default page use the folder as context for the navtree
@@ -92,18 +91,17 @@
                 parentNode["children"].append(node)
             node["parent"] = parentNode
 
         self.tree = cache
         self.root = cache[navrootPath]
 
     def __iter__(self):
-        """Breadth-first iterator for navtree nodes which allows
-        modifications of the tree during iteration. Modifications
-        are given by passing a command to the next() method of the
-        generator. For example:
+        """Breadth-first iterator for navtree nodes which allows modifications
+        of the tree during iteration. Modifications are given by passing a
+        command to the next() method of the generator. For example:
 
         >>> tree=CatalogNavTree(context, request)
         >>> g=tree.iter()
         >>> value=next(g)
         >>> try:
         ...     while True:
         ...        if value.portal_type=="Collection":
@@ -136,29 +134,27 @@
                 queue.append(child)
 
     iter = __iter__
 
 
 @implementer(INavtreeFactory)
 @adapter(Interface, Interface)
-class TreeFactory(object):
+class TreeFactory:
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def __call__(self):
         return CatalogNavTree(self.context, self.request)
 
 
 class NavigationTile(Tile):
     def update(self):
         portal_types = getToolByName(self.context, "portal_types")
-        type_titles = dict(
-            [(fti.getId(), fti.Title()) for fti in portal_types.listTypeInfo()]
-        )
+        type_titles = {fti.getId(): fti.Title() for fti in portal_types.listTypeInfo()}
 
         use_view_types = api.portal.get_registry_record(
             "plone.types_use_view_action_in_listings", default=[]
         )
         normalize = getUtility(IIDNormalizer).normalize
         treefactory = getMultiAdapter((self.context, self.request), INavtreeFactory)
         tree = treefactory()
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/tabs.py` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from Acquisition import aq_inner
 from plone import api
 from plone.tiles import Tile
 from plonetheme.nuplone.utils import getNavigationRoot
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.utils import typesToList
 from zExceptions import NotFound
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/tales.py` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/tales.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 log = logging.getLogger(__name__)
 
 
 class TileExpression(StringExpr):
     def __call__(self, econtext):
-        name = super(TileExpression, self).__call__(econtext)
+        name = super().__call__(econtext)
         context = econtext.vars["context"]
         request = econtext.vars["request"]
 
         tile = getTile(context, request, name)
         if tile is None:  # XXX Use custom exception?
             log.warning("Request for unknown tile %s", name)
             return ""
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/analytics.pt` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/analytics.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/language.pt` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/language.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/navigation.pt` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/navigation.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/templates/tabs.pt` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/templates/tabs.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/tiles/tile.py` & `NuPlone-2.2.0/plonetheme/nuplone/tiles/tile.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,38 +21,38 @@
 @implementer(IAppConfigTile)
 class AppConfigTile(Tile):
     pass
 
 
 @implementer(ITileDataManager)
 @adapter(IAppConfigTile)
-class AppConfigTileDataManager(object):
+class AppConfigTileDataManager:
     def __init__(self, tile):
         self.tile = tile
 
     def get(self):
         try:
             return json.loads(
                 api.portal.get_registry_record(
-                    "plonetheme.nuplone.appconfigtile_{}".format(self.tile.id),
+                    f"plonetheme.nuplone.appconfigtile_{self.tile.id}",
                     default="{}",
                 )
             )
         except Exception:
             log.exception("Cannot get configuration for %r", self.tile.id)
             return {}
 
     def set(self, data):
         raise NotImplementedError
 
 
 def getTile(context, request, name):
     config = json.loads(
         api.portal.get_registry_record(
-            "plonetheme.nuplone.appconfigtile_{}".format(name), default="{}"
+            f"plonetheme.nuplone.appconfigtile_{name}", default="{}"
         )
         or "{}"
     )
     type = config.get("type", name)
     tile = queryMultiAdapter((context, request), Interface, name=type)
     if tile is None:
         log.warning(
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/utils.py` & `NuPlone-2.2.0/plonetheme/nuplone/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from AccessControl import getSecurityManager
 from Acquisition import aq_chain
 from Acquisition import aq_inner
 from email.header import Header
 from email.mime.text import MIMEText
 from plone.app.layout.navigation.interfaces import INavigationRoot
 from plonetheme.nuplone import MessageFactory as _
@@ -11,15 +10,14 @@
 from Products.CMFPlone.interfaces import IPloneSiteRoot
 from z3c.form.interfaces import IAddForm
 from z3c.form.interfaces import IEditForm
 
 import collections
 import email.utils as emailutils
 import logging
-import six
 
 
 log = logging.getLogger(__name__)
 
 
 def getPortal(context):
     for obj in aq_chain(aq_inner(context)):
@@ -41,18 +39,20 @@
 def isAnonymous(user=None):
     if user is None:
         user = getSecurityManager().getUser()
     return user is None or user.getUserName() == "Anonymous User"
 
 
 def viewType(context, request):
-    """Determine what type of view the user is looking at. This returns
-    one of three options: ``view`` for normal object views, ``add``
-    for add forms, ``edit`` for edit forms, and ``other`` for all other
-    types."""
+    """Determine what type of view the user is looking at.
+
+    This returns one of three options: ``view`` for normal object views,
+    ``add`` for add forms, ``edit`` for edit forms, and ``other`` for
+    all other types.
+    """
 
     view = request.other.get("PUBLISHED")
     if view is not None:
         if IAddForm.providedBy(view):
             return "add"
         if IEditForm.providedBy(view):
             return "edit"
@@ -78,25 +78,25 @@
     except AttributeError:
         # object has no absolute_url (None or Not Found)
         pass
 
     return "other"
 
 
-class SimpleLiteral(six.text_type):
+class SimpleLiteral(str):
     def __html__(self):
-        return six.text_type(self)
+        return str(self)
 
 
 def setLanguage(request, context, lang=None):
-    """Switch Plone to another language. If no language is given via the
-    `lang` parameter the language is taken from a `language`
-    request parameter. If a dialect was chosen but is not available the main
-    language is used instead. If the main language is also not available
-    nothing is done and ``False`` is returned.
+    """Switch Plone to another language. If no language is given via the `lang`
+    parameter the language is taken from a `language` request parameter. If a
+    dialect was chosen but is not available the main language is used instead.
+    If the main language is also not available nothing is done and ``False`` is
+    returned.
 
     It is safe to call this method before rendering a template: it will
     immediately switch the current language. That means there is no need
     to trigger a redirect to force a new HTTP request.
     """
     if lang is None:
         lang = request.form.get("language")
@@ -124,16 +124,16 @@
     return True
 
 
 FactoryInfo = collections.namedtuple("FactoryInfo", "id title description url")
 
 
 def getFactoriesInContext(context):
-    """Return a list of all factories available to the current user at
-    the given location."""
+    """Return a list of all factories available to the current user at the
+    given location."""
     context = aq_inner(context)
     ftis = context.allowedContentTypes()
     if not ftis:
         return []
 
     tt = getToolByName(context, "portal_types")
     ec = tt._getExprContext(context)
@@ -155,19 +155,20 @@
     sender_email,
     recipient_name,
     recipient_email,
     subject,
     body,
     format="plain",
 ):
-    """Create an :obj:`email.MIMEText.MIMEtext` instance for an email. This
-    method will take care of adding addings a date header and message ID
-    to the email, as well as quoting of non-ASCII content.
+    """Create an :obj:`email.MIMEText.MIMEtext` instance for an email.
+
+    This method will take care of adding addings a date header and
+    message ID to the email, as well as quoting of non-ASCII content.
     """
-    if isinstance(body, six.text_type):
+    if isinstance(body, str):
         mail = MIMEText(body.encode("utf-8"), format, "utf-8")
     else:
         mail = MIMEText(body, format)
 
     if sender_name:
         mail["From"] = emailutils.formataddr((sender_name, sender_email))
     else:
@@ -181,29 +182,27 @@
     mail.set_param("charset", "utf-8")
 
     return mail
 
 
 def formatDate(request, date, length="long"):
     """Wrapper aound the zope.i18n date formatter which does not abort on
-    pre-1900 dates.
-    """
+    pre-1900 dates."""
     if date.year < 1900:
         return _("date_to_early", default="<pre-1900-date>")
     return request.locale.dates.getFormatter("date", length).format(date)
 
 
 def formatTime(request, time, length=None):
     return request.locale.dates.getFormatter("time", length).format(time)
 
 
 def formatDatetime(request, timestamp, length="long"):
     """Wrapper aound the zope.i18n datetime formatter which does not abort on
-    pre-1900 dates.
-    """
+    pre-1900 dates."""
     if timestamp.year < 1900:
         return _("date_to_early", default="<pre-1900-date>")
     if length == "long":
         return _(
             "format_datetime",
             default="${date} at ${time}",
             mapping=dict(
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/configure.zcml` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/configure.zcml`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/directives.py` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/directives.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         if action not in ["show", "enable"]:
             raise ValueError("Invalid action given")
         return [Dependency(field, name, op, value, action)]
 
 
 @adapter(Interface, Interface, AutoExtensibleForm)
 @implementer(plone.z3cform.fieldsets.interfaces.IFormExtender)
-class FormDependencyExtender(object):
-
+class FormDependencyExtender:
     order = 0
 
     def __init__(self, context, request, form):
         self.context = context
         self.request = request
         self.form = form
 
@@ -68,24 +67,24 @@
             dependencies.setdefault(directive.name, []).append(directive)
 
         todo = collections.deque([self.form])
         while todo:
             group = todo.pop()
             if hasattr(group, "groups"):
                 todo.extendleft(group.groups)
-            for (name, field) in group.fields.items():
+            for name, field in group.fields.items():
                 depends = dependencies.get(name, None)
                 if depends is None:
                     continue
                 field.field._dependencies = depends
 
 
 @adapter(IWidget, Interface)
 @implementer(IBrowserView)
-class WidgetDependencyView(object):
+class WidgetDependencyView:
     def __init__(self, widget, request):
         self.widget = widget
         self.request = request
 
     def __call__(self):
         dependencies = getattr(self.widget.field, "_dependencies", None)
         if not dependencies:
@@ -95,46 +94,43 @@
         widgets = self.widget.__parent__
         for dependency in dependencies:
             widget = widgets[dependency.field]
             name = widget.name
             if isinstance(widget, CheckBoxWidget):
                 name = "%s:list" % name
             if dependency.op in ["on", "off"]:
-                classes.append("dependsOn-%s-%s" % (name, dependency.op))
+                classes.append(f"dependsOn-{name}-{dependency.op}")
             elif dependency.op == "==":
-                classes.append("dependsOn-%s-equals-%s" % (name, dependency.value))
+                classes.append(f"dependsOn-{name}-equals-{dependency.value}")
             elif dependency.op == "!=":
-                classes.append("dependsOn-%s-notEquals-%s" % (name, dependency.value))
+                classes.append(f"dependsOn-{name}-notEquals-{dependency.value}")
 
             classes.append("dependsAction-%s" % dependency.action)
 
         return " ".join(classes) if classes else None
 
 
 @adapter(Interface, Interface, AutoExtensibleForm)
 @implementer(plone.z3cform.fieldsets.interfaces.IFormExtender)
-class FormLayoutExtender(object):
-
+class FormLayoutExtender:
     order = 10
 
     def __init__(self, context, request, form):
         self.context = context
         self.request = request
         self.form = form
 
     def update(self):
         fieldsets = mergedTaggedValueList(self.form.schema, FIELDSETS_KEY)
         if not isinstance(self.form.groups, list):
             self.form.groups = list(self.form.groups)
-        groups = dict(
-            [
-                (group.__name__, (index, group))
-                for (index, group) in enumerate(self.form.groups)
-            ]
-        )
+        groups = {
+            group.__name__: (index, group)
+            for (index, group) in enumerate(self.form.groups)
+        }
         for fieldset in fieldsets:
             layout = getattr(fieldset, "layout", None)
             if layout is None:
                 continue
             if fieldset.__name__ not in groups:
                 continue
             (index, group) = groups[fieldset.__name__]
```

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/checkbox_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/checkboxlist_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/checkboxlist_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/date_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/date_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/datetime_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/datetime_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/form.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/form.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/layout.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/multi_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/multi_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/namedfile_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/namedfile_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/namedimage_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/namedimage_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/object_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/object_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/orderedselect_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/orderedselect_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/password_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/password_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/passwordconfirm_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/passwordconfirm_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/radio_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/radio_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/select_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/select_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/text_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/text_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/textarea_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/textarea_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/textlines_display.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/textlines_display.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/textlines_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/textlines_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/wrappedform.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/wrappedform.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates/wysiwyg_input.pt` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates/wysiwyg_input.pt`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/templates.py` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/templates.py`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/plonetheme/nuplone/z3cform/widget.py` & `NuPlone-2.2.0/plonetheme/nuplone/z3cform/widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     self.value is still a list since this widget uses the
     SequenceDataConverter. Apparently z3c.form does this since it has no
     concept of a single-valued field which takes its value from a
     vocabulary.
     """
 
     def update(self):
-        super(SingleRadioWidget, self).update()
+        super().update()
         for item in self.items:
             item["name"] = item["name"].split(":list", 1)[0]
 
 
 @adapter(IChoice, INuPloneFormLayer)
 @implementer(IFieldWidget)
 def ChoiceWidgetFactory(field, request):
@@ -60,15 +60,15 @@
         if self.value != self.field.missing_value:
             try:
                 blob = getattr(self.value, "_blob", None)
                 if blob:
                     blob.__repr__()
             except POSKeyError:
                 return False
-        return super(NicerNamedImageWidget, self).allow_nochange
+        return super().allow_nochange
 
     def extract(self, default=NOVALUE):
         action = self.request.get("%s.action" % self.name, None)
         if action == "remove":
             return None
 
         value = FileWidget.extract(self, default)
@@ -103,15 +103,15 @@
         if self.value != self.field.missing_value:
             try:
                 blob = getattr(self.value, "_blob", None)
                 if blob:
                     blob.__repr__()
             except POSKeyError:
                 return False
-        return super(NicerNamedFileWidget, self).allow_nochange
+        return super().allow_nochange
 
     def extract(self, default=NOVALUE):
         action = self.request.get("%s.action" % self.name, None)
         if action == "remove":
             return None
 
         value = FileWidget.extract(self, default)
```

### Comparing `NuPlone-2.1.4/setup.py` & `NuPlone-2.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-# coding=utf-8
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "2.1.4"
+version = "2.2.0"
 
 setup(
     name="NuPlone",
     version=version,
     description="A new user interface for Plone",
     long_description=open("README.rst").read()
     + "\n"
     + open(os.path.join("docs", "changes.rst")).read(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Framework :: Zope",
         "Framework :: Zope :: 4",
+        "Framework :: Zope :: 5",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="web zope plone theme",
     author="Cornelis Kolbach, Wichert Akkerman and Syslab.com",
     author_email="info@syslab.com",
     url="https://github.com/euphorie/NuPlone",
     license="GPL",
     packages=find_packages(exclude=["ez_setup"]),
     namespace_packages=["plonetheme"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.7",
     install_requires=[
         "setuptools",
         "Plone >=5.2",
         "Products.statusmessages",
         "plone.api",
         "plone.app.z3cform",
         "plone.autoform",
```

### Comparing `NuPlone-2.1.4/src/nuplone_components/behaviour.js` & `NuPlone-2.2.0/src/nuplone_components/behaviour.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/src/nuplone_components/editlink.js` & `NuPlone-2.2.0/src/nuplone_components/editlink.js`

 * *Files identical despite different names*

### Comparing `NuPlone-2.1.4/src/nuplone_components/z3cform.js` & `NuPlone-2.2.0/src/nuplone_components/z3cform.js`

 * *Files identical despite different names*

