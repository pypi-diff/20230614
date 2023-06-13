# Comparing `tmp/Logic Circuits Evolution-1.0.0.tar.gz` & `tmp/Logic Circuits Evolution-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Logic Circuits Evolution-1.0.0.tar", last modified: Tue Jun 13 23:22:47 2023, max compression
+gzip compressed data, was "Logic Circuits Evolution-1.0.1.tar", last modified: Tue Jun 13 23:39:42 2023, max compression
```

## Comparing `Logic Circuits Evolution-1.0.0.tar` & `Logic Circuits Evolution-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 23:22:47.274803 Logic Circuits Evolution-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-13 23:22:47.236919 Logic Circuits Evolution-1.0.0/Logic_Circuits_Evolution/
--rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 Logic Circuits Evolution-1.0.0/Logic_Circuits_Evolution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 23:22:47.270793 Logic Circuits Evolution-1.0.0/Logic_Circuits_Evolution.egg-info/
--rw-rw-rw-   0        0        0      278 2023-06-13 23:22:46.000000 Logic Circuits Evolution-1.0.0/Logic_Circuits_Evolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-13 23:22:47.000000 Logic Circuits Evolution-1.0.0/Logic_Circuits_Evolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 23:22:46.000000 Logic Circuits Evolution-1.0.0/Logic_Circuits_Evolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 23:22:46.000000 Logic Circuits Evolution-1.0.0/Logic_Circuits_Evolution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      278 2023-06-13 23:22:47.272799 Logic Circuits Evolution-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-13 23:22:47.274803 Logic Circuits Evolution-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      329 2023-06-13 23:22:05.000000 Logic Circuits Evolution-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:39:42.801370 Logic Circuits Evolution-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-13 23:39:42.768910 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution/
+-rw-rw-rw-   0        0        0    19730 2023-06-13 23:39:06.000000 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:39:42.797839 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-06-13 23:39:42.000000 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-13 23:39:42.000000 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 23:39:42.000000 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 23:39:42.000000 Logic Circuits Evolution-1.0.1/Logic_Circuits_Evolution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      278 2023-06-13 23:39:42.799401 Logic Circuits Evolution-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-13 23:39:42.801370 Logic Circuits Evolution-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      329 2023-06-13 23:39:34.000000 Logic Circuits Evolution-1.0.1/setup.py
```

