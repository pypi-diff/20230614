# Comparing `tmp/pymlab-0.5.dev202212182151.tar.gz` & `tmp/pymlab-0.5.dev202306132244.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymlab-0.5.dev202212182151.tar", last modified: Sun Dec 18 21:51:40 2022, max compression
+gzip compressed data, was "pymlab-0.5.dev202306132244.tar", last modified: Tue Jun 13 22:44:02 2023, max compression
```

## Comparing `pymlab-0.5.dev202212182151.tar` & `pymlab-0.5.dev202306132244.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.740537 pymlab-0.5.dev202212182151/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2022-12-18 21:51:40.740537 pymlab-0.5.dev202212182151/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.736537 pymlab-0.5.dev202212182151/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/doc/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/doc/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/doc/pymlab.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/doc/pymlab.sensors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-18 21:51:40.740537 pymlab-0.5.dev202212182151/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1415 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.736537 pymlab-0.5.dev202212182151/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.736537 pymlab-0.5.dev202212182151/src/pymlab/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6675 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/iic_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.740537 pymlab-0.5.dev202212182151/src/pymlab/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/acount.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/adc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/altimet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      556 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/atmega.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/bus_translators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6149 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/clkgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    12425 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/gpio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3772 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/i2chub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/i2cio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/i2clcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/i2cpwm.py
--rw-r--r--   0 runner    (1001) docker     (123)    34609 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/iic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49035 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/imu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/lioncell.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/lts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/mag.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      744 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/rps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/sdp3x.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8435 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/sht.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6742 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/sps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/thermopile.py
--rw-r--r--   0 runner    (1001) docker     (123)    22027 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/sensors/windgauge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.740537 pymlab-0.5.dev202212182151/src/pymlab/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/tests/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.740537 pymlab-0.5.dev202212182151/src/pymlab/tests/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/tests/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/tests/sensors/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/pymlab/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 21:51:40.736537 pymlab-0.5.dev202212182151/src/pymlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2022-12-18 21:51:40.000000 pymlab-0.5.dev202212182151/src/pymlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2022-12-18 21:51:40.000000 pymlab-0.5.dev202212182151/src/pymlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 21:51:40.000000 pymlab-0.5.dev202212182151/src/pymlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-18 21:51:40.000000 pymlab-0.5.dev202212182151/src/pymlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-18 21:51:40.000000 pymlab-0.5.dev202212182151/src/pymlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-18 21:51:32.000000 pymlab-0.5.dev202212182151/src/quick_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.980701 pymlab-0.5.dev202306132244/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-13 22:44:02.980701 pymlab-0.5.dev202306132244/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.976701 pymlab-0.5.dev202306132244/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/doc/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/doc/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/doc/pymlab.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/doc/pymlab.sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 22:44:02.980701 pymlab-0.5.dev202306132244/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1415 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.976701 pymlab-0.5.dev202306132244/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.976701 pymlab-0.5.dev202306132244/src/pymlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6675 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/iic_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.980701 pymlab-0.5.dev202306132244/src/pymlab/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/acount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/altimet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/atmega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/bus_translators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6149 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/clkgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/gpio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3772 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/i2chub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/i2cio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/i2clcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/i2cpwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/iic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49035 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/imu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/lioncell.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/lts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/mag.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      744 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/rps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/sdp3x.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8435 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/sht.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6742 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/sps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/thermopile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/sensors/windgauge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.980701 pymlab-0.5.dev202306132244/src/pymlab/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/tests/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.980701 pymlab-0.5.dev202306132244/src/pymlab/tests/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/tests/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/tests/sensors/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/pymlab/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:44:02.976701 pymlab-0.5.dev202306132244/src/pymlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-13 22:44:02.000000 pymlab-0.5.dev202306132244/src/pymlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-13 22:44:02.000000 pymlab-0.5.dev202306132244/src/pymlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:44:02.000000 pymlab-0.5.dev202306132244/src/pymlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 22:44:02.000000 pymlab-0.5.dev202306132244/src/pymlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 22:44:02.000000 pymlab-0.5.dev202306132244/src/pymlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 22:43:56.000000 pymlab-0.5.dev202306132244/src/quick_test.py
```

### Comparing `pymlab-0.5.dev202212182151/LICENSE` & `pymlab-0.5.dev202306132244/LICENSE`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/PKG-INFO` & `pymlab-0.5.dev202306132244/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymlab
-Version: 0.5.dev202212182151
+Version: 0.5.dev202306132244
 Summary: Toolbox for interfacing I2C sensors.
 Home-page: https://github.com/MLAB-project/pymlab
 Download-URL: https://github.com/MLAB-project/pymlab/archive/refs/heads/master.zip
 Author: Jan Milík
 Author-email: milikjan@fit.cvut.cz
 License: Lesser General Public License v3
 Keywords: TWI,IIC,I2C,USB,sensors,drivers
```

### Comparing `pymlab-0.5.dev202212182151/README.md` & `pymlab-0.5.dev202306132244/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 Installation
 ------------
 
 ### Dependencies
     $ sudo apt-get install git python3-setuptools python3-smbus python3-six python3-pip python3-numpy python3-hidapi python3-smbus2
 
+Dependencies are also available on pip (useful on systems without native packages)
+    $ sudo python3 -m pip install smbus2
+
 The latest version of pymlab library use true I²C transfers instead of SMBus transfers. It is needed by some sensors. Namely by SHT31, SHT25 etc.  Therefore an updated version of i2c-tools and python-smbus module is needed for correct working of pymlab library and some examples.
 The latest version of python-smbus could be installed from [this fork of i2c-tools](https://github.com/MLAB-project/i2c-tools).
 
 ### Install in to Ubuntu python system
 
     $ git clone https://github.com/MLAB-project/pymlab
     $ cd pymlab/
```

### Comparing `pymlab-0.5.dev202212182151/doc/conf.py` & `pymlab-0.5.dev202306132244/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/doc/pymlab.rst` & `pymlab-0.5.dev202306132244/doc/pymlab.rst`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/doc/pymlab.sensors.rst` & `pymlab-0.5.dev202306132244/doc/pymlab.sensors.rst`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/setup.py` & `pymlab-0.5.dev202306132244/setup.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/__init__.py` & `pymlab-0.5.dev202306132244/src/pymlab/__init__.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/config.py` & `pymlab-0.5.dev202306132244/src/pymlab/config.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/iic_server.py` & `pymlab-0.5.dev202306132244/src/pymlab/iic_server.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/__init__.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/acount.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/acount.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/adc.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/adc.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/altimet.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/altimet.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/atmega.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/atmega.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/bus_translators.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/bus_translators.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/clkgen.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/clkgen.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/gpio.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/gpio.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/i2chub.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/i2chub.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/i2cio.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/i2cio.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/i2clcd.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/i2clcd.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/i2cpwm.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/i2cpwm.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/iic.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/iic.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/imu.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/imu.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/light.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/light.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/lightning.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/lightning.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/lioncell.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/lioncell.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/lts.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/lts.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/mag.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/mag.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/motor.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/motor.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/rps.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/rps.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/rtc.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/rtc.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/sdp3x.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/sdp3x.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/sht.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/sht.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/sps.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/sps.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/thermopile.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/thermopile.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/sensors/windgauge.py` & `pymlab-0.5.dev202306132244/src/pymlab/sensors/windgauge.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/tests/remote.py` & `pymlab-0.5.dev202306132244/src/pymlab/tests/remote.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/tests/sensors/config.py` & `pymlab-0.5.dev202306132244/src/pymlab/tests/sensors/config.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab/utils.py` & `pymlab-0.5.dev202306132244/src/pymlab/utils.py`

 * *Files identical despite different names*

### Comparing `pymlab-0.5.dev202212182151/src/pymlab.egg-info/PKG-INFO` & `pymlab-0.5.dev202306132244/src/pymlab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymlab
-Version: 0.5.dev202212182151
+Version: 0.5.dev202306132244
 Summary: Toolbox for interfacing I2C sensors.
 Home-page: https://github.com/MLAB-project/pymlab
 Download-URL: https://github.com/MLAB-project/pymlab/archive/refs/heads/master.zip
 Author: Jan Milík
 Author-email: milikjan@fit.cvut.cz
 License: Lesser General Public License v3
 Keywords: TWI,IIC,I2C,USB,sensors,drivers
```

### Comparing `pymlab-0.5.dev202212182151/src/pymlab.egg-info/SOURCES.txt` & `pymlab-0.5.dev202306132244/src/pymlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

