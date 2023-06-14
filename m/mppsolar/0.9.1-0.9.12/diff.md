# Comparing `tmp/mppsolar-0.9.1.tar.gz` & `tmp/mppsolar-0.9.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mppsolar-0.9.1.tar", last modified: Fri Nov 12 02:34:33 2021, max compression
+gzip compressed data, was "mppsolar-0.9.12.tar", last modified: Thu Apr  7 05:07:14 2022, max compression
```

## Comparing `mppsolar-0.9.1.tar` & `mppsolar-0.9.12.tar`

### file list

```diff
@@ -1,70 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.011857 mppsolar-0.9.1/
--rw-rw-r--   0 root         (0) root         (0)     1064 2020-11-25 04:12:34.000000 mppsolar-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2066 2021-11-12 02:34:33.011857 mppsolar-0.9.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1383 2021-06-17 01:51:29.000000 mppsolar-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.003857 mppsolar-0.9.1/mppsolar/
--rw-rw-r--   0 root         (0) root         (0)    14334 2021-10-28 02:28:38.000000 mppsolar-0.9.1/mppsolar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.003857 mppsolar-0.9.1/mppsolar/devices/
--rw-rw-r--   0 root         (0) root         (0)        0 2020-11-26 01:02:38.000000 mppsolar-0.9.1/mppsolar/devices/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13314 2021-11-02 04:28:22.000000 mppsolar-0.9.1/mppsolar/devices/device.py
--rw-rw-r--   0 root         (0) root         (0)      191 2021-02-15 03:10:45.000000 mppsolar-0.9.1/mppsolar/devices/jkbms.py
--rw-rw-r--   0 root         (0) root         (0)      197 2021-02-15 03:10:31.000000 mppsolar-0.9.1/mppsolar/devices/mppsolar.py
--rw-rw-r--   0 root         (0) root         (0)     3001 2021-10-28 02:24:12.000000 mppsolar-0.9.1/mppsolar/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.007857 mppsolar-0.9.1/mppsolar/io/
--rw-rw-r--   0 root         (0) root         (0)     4106 2021-10-28 06:36:29.000000 mppsolar-0.9.1/mppsolar/io/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1643 2021-10-28 07:24:00.000000 mppsolar-0.9.1/mppsolar/io/baseio.py
--rw-rw-r--   0 root         (0) root         (0)     1631 2021-06-28 04:03:53.000000 mppsolar-0.9.1/mppsolar/io/dalyserialio.py
--rw-rw-r--   0 root         (0) root         (0)     1504 2021-02-15 04:05:20.000000 mppsolar-0.9.1/mppsolar/io/esp32io.py
--rw-rw-r--   0 root         (0) root         (0)     2619 2021-05-21 03:12:49.000000 mppsolar-0.9.1/mppsolar/io/hidrawio.py
--rw-rw-r--   0 root         (0) root         (0)     1640 2021-05-21 03:13:06.000000 mppsolar-0.9.1/mppsolar/io/jkbledelegate.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2021-02-15 04:03:25.000000 mppsolar-0.9.1/mppsolar/io/jkbleio.py
--rw-rw-r--   0 root         (0) root         (0)     4050 2021-09-30 04:12:37.000000 mppsolar-0.9.1/mppsolar/io/mqttio.py
--rw-rw-r--   0 root         (0) root         (0)     1313 2021-05-21 03:13:45.000000 mppsolar-0.9.1/mppsolar/io/serialio.py
--rw-rw-r--   0 root         (0) root         (0)     2293 2021-05-21 03:13:53.000000 mppsolar-0.9.1/mppsolar/io/testio.py
--rw-rw-r--   0 root         (0) root         (0)     3204 2021-04-26 23:52:56.000000 mppsolar-0.9.1/mppsolar/io/vserialio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.007857 mppsolar-0.9.1/mppsolar/libs/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-01 19:47:05.000000 mppsolar-0.9.1/mppsolar/libs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2509 2021-10-18 04:12:57.000000 mppsolar-0.9.1/mppsolar/libs/mqttbroker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.007857 mppsolar-0.9.1/mppsolar/outputs/
--rw-rw-r--   0 root         (0) root         (0)     2093 2021-10-28 07:45:53.000000 mppsolar-0.9.1/mppsolar/outputs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      175 2021-02-15 04:01:55.000000 mppsolar-0.9.1/mppsolar/outputs/baseoutput.py
--rw-rw-r--   0 root         (0) root         (0)     2845 2021-03-18 02:54:35.000000 mppsolar-0.9.1/mppsolar/outputs/hass_mqtt.py
--rw-rw-r--   0 root         (0) root         (0)     2234 2021-04-05 22:30:21.000000 mppsolar-0.9.1/mppsolar/outputs/influx2_mqtt.py
--rw-rw-r--   0 root         (0) root         (0)     1966 2021-04-05 22:30:12.000000 mppsolar-0.9.1/mppsolar/outputs/influx_mqtt.py
--rw-rw-r--   0 root         (0) root         (0)     1387 2021-05-21 03:05:41.000000 mppsolar-0.9.1/mppsolar/outputs/json.py
--rw-rw-r--   0 root         (0) root         (0)     2101 2021-04-05 22:30:32.000000 mppsolar-0.9.1/mppsolar/outputs/json_mqtt.py
--rw-rw-r--   0 root         (0) root         (0)     3859 2021-10-28 07:58:08.000000 mppsolar-0.9.1/mppsolar/outputs/mqtt.py
--rw-rw-r--   0 root         (0) root         (0)     1022 2021-10-29 01:42:28.000000 mppsolar-0.9.1/mppsolar/outputs/raw.py
--rw-rw-r--   0 root         (0) root         (0)     1892 2021-05-21 03:04:54.000000 mppsolar-0.9.1/mppsolar/outputs/screen.py
--rw-rw-r--   0 root         (0) root         (0)     1989 2021-02-15 19:53:00.000000 mppsolar-0.9.1/mppsolar/outputs/tag_mqtt.py
--rw-rw-r--   0 root         (0) root         (0)     6134 2021-11-01 03:59:53.000000 mppsolar-0.9.1/mppsolar/powermon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.011857 mppsolar-0.9.1/mppsolar/protocols/
--rw-rw-r--   0 root         (0) root         (0)      910 2021-10-28 07:02:28.000000 mppsolar-0.9.1/mppsolar/protocols/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    21551 2021-11-02 03:57:17.000000 mppsolar-0.9.1/mppsolar/protocols/abstractprotocol.py
--rw-rw-r--   0 root         (0) root         (0)    13527 2021-06-27 22:08:14.000000 mppsolar-0.9.1/mppsolar/protocols/daly.py
--rw-rw-r--   0 root         (0) root         (0)      427 2021-06-02 05:45:36.000000 mppsolar-0.9.1/mppsolar/protocols/daly40.py
--rw-rw-r--   0 root         (0) root         (0)    13605 2021-08-18 02:01:55.000000 mppsolar-0.9.1/mppsolar/protocols/jk02.py
--rw-rw-r--   0 root         (0) root         (0)     7691 2021-08-03 21:32:30.000000 mppsolar-0.9.1/mppsolar/protocols/jk04.py
--rw-rw-r--   0 root         (0) root         (0)     5902 2021-06-16 02:35:36.000000 mppsolar-0.9.1/mppsolar/protocols/jk232.py
--rw-rw-r--   0 root         (0) root         (0)     5176 2021-06-16 03:24:10.000000 mppsolar-0.9.1/mppsolar/protocols/jk485.py
--rw-rw-r--   0 root         (0) root         (0)     7200 2021-08-18 02:21:20.000000 mppsolar-0.9.1/mppsolar/protocols/jkabstractprotocol.py
--rw-rw-r--   0 root         (0) root         (0)     6893 2021-06-16 20:31:12.000000 mppsolar-0.9.1/mppsolar/protocols/pi16.py
--rw-rw-r--   0 root         (0) root         (0)    30097 2021-09-30 21:14:39.000000 mppsolar-0.9.1/mppsolar/protocols/pi17.py
--rw-rw-r--   0 root         (0) root         (0)     5646 2021-09-30 06:17:03.000000 mppsolar-0.9.1/mppsolar/protocols/pi18.py
--rw-rw-r--   0 root         (0) root         (0)    36644 2021-09-30 06:51:23.000000 mppsolar-0.9.1/mppsolar/protocols/pi30.py
--rw-rw-r--   0 root         (0) root         (0)    34303 2021-08-03 23:07:16.000000 mppsolar-0.9.1/mppsolar/protocols/pi30max.py
--rw-rw-r--   0 root         (0) root         (0)    15179 2021-05-21 03:11:17.000000 mppsolar-0.9.1/mppsolar/protocols/pi30revo.py
--rw-rw-r--   0 root         (0) root         (0)    15502 2021-04-19 20:12:31.000000 mppsolar-0.9.1/mppsolar/protocols/pi41.py
--rw-rw-r--   0 root         (0) root         (0)     9335 2021-08-08 04:10:59.000000 mppsolar-0.9.1/mppsolar/protocols/protocol_helpers.py
--rw-rw-r--   0 root         (0) root         (0)    11472 2021-08-04 00:06:33.000000 mppsolar-0.9.1/mppsolar/protocols/ved.py
--rw-rw-r--   0 root         (0) root         (0)       88 2021-10-29 01:45:47.000000 mppsolar-0.9.1/mppsolar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 02:34:33.003857 mppsolar-0.9.1/mppsolar.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2066 2021-11-12 02:34:32.000000 mppsolar-0.9.1/mppsolar.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1601 2021-11-12 02:34:32.000000 mppsolar-0.9.1/mppsolar.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2021-11-12 02:34:32.000000 mppsolar-0.9.1/mppsolar.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      101 2021-11-12 02:34:32.000000 mppsolar-0.9.1/mppsolar.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       58 2021-11-12 02:34:32.000000 mppsolar-0.9.1/mppsolar.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2021-11-12 02:34:32.000000 mppsolar-0.9.1/mppsolar.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      104 2021-02-09 04:12:54.000000 mppsolar-0.9.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-12 02:34:33.011857 mppsolar-0.9.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3477 2021-10-06 04:31:21.000000 mppsolar-0.9.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.209878 mppsolar-0.9.12/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1064 2022-04-07 04:16:38.000000 mppsolar-0.9.12/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     2066 2022-04-07 05:07:14.209878 mppsolar-0.9.12/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1382 2022-04-07 04:30:24.000000 mppsolar-0.9.12/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.149877 mppsolar-0.9.12/mppsolar/
+-rw-r--r--   0 pi        (1000) pi        (1000)    14334 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.159877 mppsolar-0.9.12/mppsolar/devices/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/devices/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13314 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/devices/device.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      191 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/devices/jkbms.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      197 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/devices/mppsolar.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3001 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/helpers.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.169877 mppsolar-0.9.12/mppsolar/io/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4131 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1643 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/baseio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1631 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/dalyserialio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1504 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/esp32io.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2619 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/hidrawio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1640 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/jkbledelegate.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4669 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/jkbleio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4050 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/mqttio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1313 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/serialio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2293 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/testio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3204 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/io/vserialio.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.169877 mppsolar-0.9.12/mppsolar/libs/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/libs/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2683 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/libs/mqttbroker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.189878 mppsolar-0.9.12/mppsolar/outputs/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2079 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      175 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/baseoutput.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3015 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/domoticz_autodiscover.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3134 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/domoticz_mqtt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3140 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/hass_mqtt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2234 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/influx2_mqtt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1966 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/influx_mqtt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1387 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/json.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2257 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/json_mqtt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3883 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/mqtt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1022 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/raw.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1892 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/screen.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1989 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/outputs/tag_mqtt.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.189878 mppsolar-0.9.12/mppsolar/ports/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1173 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/ports/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1639 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/ports/port.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2393 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/ports/test.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6423 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/powermon.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.209878 mppsolar-0.9.12/mppsolar/protocols/
+-rw-r--r--   0 pi        (1000) pi        (1000)      910 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21551 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/abstractprotocol.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13527 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/daly.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      427 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/daly40.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13605 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/jk02.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7691 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/jk04.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5902 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/jk232.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5176 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/jk485.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7200 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/jkabstractprotocol.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6893 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/pi16.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    30097 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/pi17.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    15716 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/pi18.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    36644 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/pi30.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    34303 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/pi30max.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    15179 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/pi30revo.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    15502 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/pi41.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9335 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/protocol_helpers.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    11472 2022-04-07 04:16:38.000000 mppsolar-0.9.12/mppsolar/protocols/ved.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       59 2022-04-07 04:50:39.000000 mppsolar-0.9.12/mppsolar/version.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-04-07 05:07:14.159877 mppsolar-0.9.12/mppsolar.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2066 2022-04-07 05:07:08.000000 mppsolar-0.9.12/mppsolar.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1750 2022-04-07 05:07:14.000000 mppsolar-0.9.12/mppsolar.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-04-07 05:07:09.000000 mppsolar-0.9.12/mppsolar.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      100 2022-04-07 05:07:12.000000 mppsolar-0.9.12/mppsolar.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       71 2022-04-07 05:07:13.000000 mppsolar-0.9.12/mppsolar.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        9 2022-04-07 05:07:13.000000 mppsolar-0.9.12/mppsolar.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      104 2022-04-07 04:16:38.000000 mppsolar-0.9.12/pyproject.toml
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-04-07 05:07:14.209878 mppsolar-0.9.12/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)     3496 2022-04-07 04:58:27.000000 mppsolar-0.9.12/setup.py
```

### Comparing `mppsolar-0.9.1/LICENSE` & `mppsolar-0.9.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/PKG-INFO` & `mppsolar-0.9.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mppsolar
-Version: 0.9.1
+Version: 0.9.12
 Summary: Package to communicate with Solar inverters and BMSs
 Home-page: https://github.com/jblance/mpp-solar
 Author: John Blance
 Author-email: 
 License: MIT
 Keywords: hardware serial communication
 Platform: UNKNOWN
@@ -43,15 +43,15 @@
 
 ## Compute hardware support ##
 The python code is designed to run on Linux type python environments using python 3.6 or newer
 
 [Hardware that has been known to work](https://github.com/jblance/mpp-solar/blob/master/docs/hardware.md)
 
 ## Installation ##
-* to get the latest stable version: `sudo pip install mpp-solar`
+* to get the latest stable version: `sudo pip install mppsolar`
 * [more installation options](https://github.com/jblance/mpp-solar/blob/master/docs/installation.md)
 
 ## Usage ###
 `$ mpp-solar -h` or `$ jkbms -h` will display the available options
 
 [More detailed usage](https://github.com/jblance/mpp-solar/blob/master/docs/usage.md)
```

### Comparing `mppsolar-0.9.1/README.md` & `mppsolar-0.9.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ## Compute hardware support ##
 The python code is designed to run on Linux type python environments using python 3.6 or newer
 
 [Hardware that has been known to work](https://github.com/jblance/mpp-solar/blob/master/docs/hardware.md)
 
 ## Installation ##
-* to get the latest stable version: `sudo pip install mpp-solar`
+* to get the latest stable version: `sudo pip install mppsolar`
 * [more installation options](https://github.com/jblance/mpp-solar/blob/master/docs/installation.md)
 
 ## Usage ###
 `$ mpp-solar -h` or `$ jkbms -h` will display the available options
 
 [More detailed usage](https://github.com/jblance/mpp-solar/blob/master/docs/usage.md)
```

### Comparing `mppsolar-0.9.1/mppsolar/__init__.py` & `mppsolar-0.9.12/mppsolar/__init__.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/devices/device.py` & `mppsolar-0.9.12/mppsolar/devices/device.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/helpers.py` & `mppsolar-0.9.12/mppsolar/helpers.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/baseio.py` & `mppsolar-0.9.12/mppsolar/io/baseio.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/dalyserialio.py` & `mppsolar-0.9.12/mppsolar/io/dalyserialio.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/esp32io.py` & `mppsolar-0.9.12/mppsolar/io/esp32io.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/hidrawio.py` & `mppsolar-0.9.12/mppsolar/io/hidrawio.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/jkbledelegate.py` & `mppsolar-0.9.12/mppsolar/io/jkbledelegate.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/jkbleio.py` & `mppsolar-0.9.12/mppsolar/io/jkbleio.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .baseio import BaseIO
 from ..helpers import get_kwargs
 from .jkbledelegate import jkBleDelegate
 
 log = logging.getLogger("JkBleIO")
 
 getInfo = b"\xaa\x55\x90\xeb\x97\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x11"
+# getInfo = b"\xaa\x55\x90\xeb\x97\x00\xdf\x52\x88\x67\x9d\x0a\x09\x6b\x9a\xf6\x70\x9a\x17\xfd"
 
 
 class JkBleIO(BaseIO):
     def __init__(self, device_path) -> None:
         self._device = None
         self._device_path = device_path
         self.maxConnectionAttempts = 3
```

### Comparing `mppsolar-0.9.1/mppsolar/io/mqttio.py` & `mppsolar-0.9.12/mppsolar/io/mqttio.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/serialio.py` & `mppsolar-0.9.12/mppsolar/io/serialio.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/testio.py` & `mppsolar-0.9.12/mppsolar/io/testio.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/io/vserialio.py` & `mppsolar-0.9.12/mppsolar/io/vserialio.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/libs/mqttbroker.py` & `mppsolar-0.9.12/mppsolar/libs/mqttbroker.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,24 +42,29 @@
         self._isConnected = False
 
     def on_disconnect(self, client, userdata, rc):
         print(f"Disconnection returned result: {rc}")
         self._isConnected = False
 
     def connect(self):
+
         self.mqttc.on_connect = self.on_connect
         self.mqttc.on_disconnect = self.on_disconnect
-        self.mqttc.connect(self.name, self.port, keepalive=60)
+        # if a name is supplied, connect
+        if self.name:
+            self.mqttc.connect(self.name, self.port, keepalive=60)
 
     def start(self):
-        self.mqttc.loop_start()
+        if self._isConnected:
+            self.mqttc.loop_start()
 
     def stop(self):
         self.mqttc.loop_stop()
-        self.mqttc.disconnect
+        if self._isConnected:
+            self.mqttc.disconnect
 
     def set(self, variable, value):
         setattr(self, variable, value)
 
     def update(self, variable, value):
         # only override if value is not None
         if value is None:
@@ -71,16 +76,17 @@
 
         # check if connected, connect if not
         if not self._isConnected:
             log.debug("Not connected, connecting")
             self.connect
         # Register callback
         self.mqttc.on_message = callback
-        # Subscribe to command topic
-        self.mqttc.subscribe(topic, qos=0)
+        if self._isConnected:
+            # Subscribe to command topic
+            self.mqttc.subscribe(topic, qos=0)
 
 
 if __name__ == "__main__":
     broker = MqttBroker("brokername")
     print(broker)
     broker.name = "test1"
     print(broker)
```

### Comparing `mppsolar-0.9.1/mppsolar/outputs/__init__.py` & `mppsolar-0.9.12/mppsolar/outputs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             # perhaps raise a Powermon exception here??
             # maybe warn and keep going, only error if no outputs found?
             log.critical(f"No module found for output processor {output}")
     return ops
 
 
 def output_results(results, config, mqtt_broker):
-    outputs = get_outputs(config.get("CONFIG", "outputs"))
+    outputs = get_outputs(config["outputs"])
     for op in outputs:
         # maybe include the command and what the command is im the output
         # eg QDI run, Display Inverter Default Settings
         filter = config.get("CONFIG", "filter")
         log.debug(f"Using output filter: {filter}")
         op.output(
             data=dict(results),
```

### Comparing `mppsolar-0.9.1/mppsolar/outputs/hass_mqtt.py` & `mppsolar-0.9.12/mppsolar/outputs/hass_mqtt.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,15 +51,18 @@
                 #
                 # <discovery_prefix>/<component>/[<node_id>/]<object_id>/config
                 # topic "homeassistant/binary_sensor/garden/config"
                 # msg '{"name": "garden", "device_class": "motion", "state_topic": "homeassistant/binary_sensor/garden/state", "unit_of_measurement": "°C"}'
                 topic = f"homeassistant/sensor/mpp_{tag}_{key}/config"
                 topic = topic.replace(" ", "_")
                 name = f"{tag} {_key}"
-                payload = f'{{"name": "{name}", "state_topic": "homeassistant/sensor/mpp_{tag}_{key}/state", "unit_of_measurement": "{unit}", "unique_id": "mpp_{tag}_{key}"  }}'
+                if unit == "W":
+                    payload = f'{{"name": "{name}", "state_topic": "homeassistant/sensor/mpp_{tag}_{key}/state", "unit_of_measurement": "{unit}", "unique_id": "mpp_{tag}_{key}", "state_class": "measurement", "device_class": "power"  }}'
+                else:
+                    payload = f'{{"name": "{name}", "state_topic": "homeassistant/sensor/mpp_{tag}_{key}/state", "unit_of_measurement": "{unit}", "unique_id": "mpp_{tag}_{key}"  }}'
                 # msg = {"topic": topic, "payload": payload, "retain": True}
                 msg = {"topic": topic, "payload": payload}
                 msgs.append(msg)
                 #
                 # VALUE SETTING
                 #
                 # unit = data[key][1]
```

### Comparing `mppsolar-0.9.1/mppsolar/outputs/influx2_mqtt.py` & `mppsolar-0.9.12/mppsolar/outputs/influx2_mqtt.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/outputs/influx_mqtt.py` & `mppsolar-0.9.12/mppsolar/outputs/influx_mqtt.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/outputs/json.py` & `mppsolar-0.9.12/mppsolar/outputs/json.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/outputs/json_mqtt.py` & `mppsolar-0.9.12/mppsolar/outputs/json_mqtt.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,19 @@
     def __init__(self, *args, **kwargs) -> None:
         log.debug(f"__init__: kwargs {kwargs}")
 
     def build_msgs(self, *args, **kwargs):
         data = get_kwargs(kwargs, "data")
         tag = get_kwargs(kwargs, "tag")
         keep_case = get_kwargs(kwargs, "keep_case")
-        topic = get_kwargs(kwargs, "mqtt_topic", default="mpp-solar")
+        mqtt_broker = get_kwargs(kwargs, "mqtt_broker")
+        if mqtt_broker is not None:
+            topic = mqtt_broker.results_topic
+        else:
+            topic = get_kwargs(kwargs, "mqtt_topic", default="mpp-solar")
         filter = get_kwargs(kwargs, "filter")
         if filter is not None:
             filter = re.compile(filter)
         excl_filter = get_kwargs(kwargs, "excl_filter")
         if excl_filter is not None:
             excl_filter = re.compile(excl_filter)
```

### Comparing `mppsolar-0.9.1/mppsolar/outputs/mqtt.py` & `mppsolar-0.9.12/mppsolar/outputs/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def output(self, *args, **kwargs):
         log.info("Using output processor: mqtt")
         log.debug(f"kwargs {kwargs}")
         data = get_kwargs(kwargs, "data")
         if data is None:
             return
         mqtt_broker = get_kwargs(kwargs, "mqtt_broker")
-        if mqtt_broker is None:
+        if mqtt_broker is None or not mqtt_broker.name:
             return
         mqtt_port = mqtt_broker.port
         mqtt_user = mqtt_broker.username
         mqtt_pass = mqtt_broker.password
 
         filter = get_kwargs(kwargs, "filter")
         if filter is not None:
```

### Comparing `mppsolar-0.9.1/mppsolar/outputs/raw.py` & `mppsolar-0.9.12/mppsolar/outputs/raw.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/outputs/screen.py` & `mppsolar-0.9.12/mppsolar/outputs/screen.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/outputs/tag_mqtt.py` & `mppsolar-0.9.12/mppsolar/outputs/tag_mqtt.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/powermon.py` & `mppsolar-0.9.12/mppsolar/powermon.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,63 @@
 # !/usr/bin/python3
-import configparser
-import io
 import logging
 from argparse import ArgumentParser
 from collections import deque
 from time import sleep
 
-from mppsolar.io import get_port
+import yaml
+
 from mppsolar.libs.mqttbroker import MqttBroker
 from mppsolar.outputs import output_results
+from mppsolar.ports import get_port
 from mppsolar.protocols import get_protocol
 from mppsolar.version import __version__  # noqa: F401
 
+# from mppsolar.io import get_port
+
+
 # Set-up logger
 log = logging.getLogger("")
 FORMAT = "%(asctime)-15s:%(levelname)s:%(module)s:%(funcName)s@%(lineno)d: %(message)s"
 logging.basicConfig(format=FORMAT)
 
+
+class ConfigError(Exception):
+    pass
+
+
 sample_config = """
-    [CONFIG]
-    port = /dev/ttyUSB0
-    porttype = test
-    portbaud = 2400
-    protocol = PI30
-    mqttbroker_name = localhost
-    mqttbroker_port = 1883
-    mqttbroker_user =
-    mqttbroker_pass =
-    split_token = ,
-    commands = QPIGS,QPIRI
-    outputs = screen,mqtt
-    tag = sample
-    filter =
-    command_topic = test/command_topic
-    command_pause = 5
-    """
+  port:
+    path: /dev/ttyUSB0
+    type: test
+    baud: 2400
+  protocol: PI30
+  mqttbroker:
+    name: null
+    port: 1883
+    user: null
+    pass: null
+  adhoc_commands:
+    topic: test/command_topic
+    outputs:
+      - name: screen
+      - name: mqtt
+  commands:
+    - command: QPIGS
+      gap: 10s
+      outputs:
+      - name: screen
+      - name: mqtt
+    - command: QPIRI
+      gap: 1m
+      outputs:
+      - name: screen
+        tag: testtag
+        filter: volt
+"""
 
 ADHOC_COMMANDS = deque([])
 SPLIT_TOKEN = ","
 
 
 def mqtt_callback(client, userdata, msg):
     print(f"Received `{msg.payload}` on topic `{msg.topic}`")
@@ -51,17 +70,17 @@
     parser = ArgumentParser(description=description)
 
     parser.add_argument(
         "-C",
         "--configFile",
         nargs="?",
         type=str,
-        help="Full location of config file (default /etc/mpp-solar/powermon.conf)",
-        const=None,
-        default="/etc/mpp-solar/powermon.conf",
+        help="Full location of config file",
+        const="/etc/mpp-solar/powermon.yml",
+        default=None,
     )
     parser.add_argument("-v", "--version", action="store_true", help="Display the version")
     parser.add_argument(
         "--generateConfigFile",
         action="store_true",
         help="Print a new config file based on options supplied (including the existing config file)",
     )
@@ -99,93 +118,97 @@
     if args.version:
         print(description)
         return None
 
     # Build configuration from defaults, config file and command line overrides
     log.info(f"Using config file:{args.configFile}")
     # build config - start with defaults
-    config = configparser.ConfigParser()
-    config.read_string(sample_config)
+    config = yaml.safe_load(sample_config)
     # build config - update with details from config file
     if args.configFile is not None:
-        config.read(args.configFile)
+        with open("args.configFile", "r") as stream:
+            try:
+                config.update(yaml.safe_load(stream))
+            except yaml.YAMLError as exc:
+                print(exc)
     # build config - override with any command line arguments
     # TODO: command line overrides
 
     # if generateConfigFile is true then print config out
     if args.generateConfigFile:
-        # FIXME must be a better way
-        with io.StringIO() as ss:
-            config.write(ss)
-            ss.seek(0)  # rewind
-            print(ss.read())
+        print("# yaml config for powermon")
+        print("# default location /etc/mpp-solar/powermon.yml")
+        print(yaml.dump(config))
         return
 
     # debug dump config
-    for section in config.sections():
-        log.debug(f"config section [{section}]")
-        for key in config[section]:
-            print(f"{key} = {config[section][key]}")
-
-    # split token
-    SPLIT_TOKEN = config.get("CONFIG", "split_token")
+    log.debug(config)
 
     # Build mqtt broker
+    # TODO disable if not defined
     mqtt_broker = MqttBroker(
-        name=config.get("CONFIG", "mqttbroker_name"),
-        port=config.getint("CONFIG", "mqttbroker_port"),
-        username=config.get("CONFIG", "mqttbroker_user"),
-        password=config.get("CONFIG", "mqttbroker_pass"),
+        name=config["mqttbroker"]["name"],
+        port=config["mqttbroker"]["port"],
+        username=config["mqttbroker"]["user"],
+        password=config["mqttbroker"]["pass"],
     )
     log.debug(mqtt_broker)
+
     # sub to command topic
+    # TODO disable if not defined
+    # TODO disable if mqttbroker is null
     mqtt_broker.connect()
-    mqtt_broker.subscribe(config.get("CONFIG", "command_topic"), mqtt_callback)
+    mqtt_broker.subscribe(config["adhoc_commands"]["topic"], mqtt_callback)
     # connect to mqtt
     mqtt_broker.start()
 
     # get port
-    port = get_port(
-        port=config.get("CONFIG", "port"),
-        porttype=config.get("CONFIG", "porttype"),
-        baud=config.get("CONFIG", "portbaud"),
-    )
+    portconfig = config["port"].copy()
+    log.debug("portconfig", portconfig)
+    port = get_port(portconfig)
+    # port = get_port(porttype=porttype)
+    if not port:
+        log.error(f"No port for config '{portconfig}' found")
+        raise ConfigError(f"No port for config '{portconfig}' found")
 
     # get protocol handler
-    protocol = get_protocol(protocol=config.get("CONFIG", "protocol"))
+    protocol = get_protocol(protocol=config["protocol"])
 
     loop = True
-
     try:
         # connect to port
         port.connect()
         while loop:
             # loop through command list
-            for command in config.get("CONFIG", "commands").split(SPLIT_TOKEN):
+            for command in config["commands"]:
                 # process any adhoc commands first
-                print(f"{ADHOC_COMMANDS}")
+                log.debug(f"adhoc command list: {ADHOC_COMMANDS}")
                 while len(ADHOC_COMMANDS) > 0:
                     adhoc_command = ADHOC_COMMANDS.popleft().decode()  # FIXME: decode to str #
                     log.info(f"Processing command: {adhoc_command}")
                     results = port.process_command(command=adhoc_command, protocol=protocol)
                     log.debug(f"results {results}")
                     # send to output processor(s)
-                    output_results(results=results, config=config, mqtt_broker=mqtt_broker)
+                    # TODO sort outputs
+                    output_results(
+                        results=results, outputs=config["adhoc_commands"], mqtt_broker=mqtt_broker
+                    )
                 # process 'normal' commands
                 log.info(f"Processing command: {command}")
-                results = port.process_command(command=command, protocol=protocol)
+                results = port.process_command(command=command["command"], protocol=protocol)
                 log.debug(f"results {results}")
                 # send to output processor(s)
-                output_results(results=results, config=config, mqtt_broker=mqtt_broker)
+                output_results(results=results, outputs=command, mqtt_broker=mqtt_broker)
                 # pause
-                pause_time = config.getint("CONFIG", "command_pause")
+                pause_time = config["command_pause"]
                 log.debug(f"Sleeping for {pause_time}secs")
-            sleep(pause_time)
             if args.once:
                 loop = False
+            else:
+                sleep(pause_time)
     except KeyboardInterrupt:
         print("KeyboardInterrupt")
     finally:
         # Disconnect port
         port.disconnect()
         # Disconnect mqtt
         mqtt_broker.stop()
```

### Comparing `mppsolar-0.9.1/mppsolar/protocols/__init__.py` & `mppsolar-0.9.12/mppsolar/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/abstractprotocol.py` & `mppsolar-0.9.12/mppsolar/protocols/abstractprotocol.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/daly.py` & `mppsolar-0.9.12/mppsolar/protocols/daly.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/jk02.py` & `mppsolar-0.9.12/mppsolar/protocols/jk02.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/jk04.py` & `mppsolar-0.9.12/mppsolar/protocols/jk04.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/jk232.py` & `mppsolar-0.9.12/mppsolar/protocols/jk232.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/jk485.py` & `mppsolar-0.9.12/mppsolar/protocols/jk485.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/jkabstractprotocol.py` & `mppsolar-0.9.12/mppsolar/protocols/jkabstractprotocol.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/pi16.py` & `mppsolar-0.9.12/mppsolar/protocols/pi16.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/pi17.py` & `mppsolar-0.9.12/mppsolar/protocols/pi17.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/pi30.py` & `mppsolar-0.9.12/mppsolar/protocols/pi30.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/pi30max.py` & `mppsolar-0.9.12/mppsolar/protocols/pi30max.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/pi30revo.py` & `mppsolar-0.9.12/mppsolar/protocols/pi30revo.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/pi41.py` & `mppsolar-0.9.12/mppsolar/protocols/pi41.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/protocol_helpers.py` & `mppsolar-0.9.12/mppsolar/protocols/protocol_helpers.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar/protocols/ved.py` & `mppsolar-0.9.12/mppsolar/protocols/ved.py`

 * *Files identical despite different names*

### Comparing `mppsolar-0.9.1/mppsolar.egg-info/PKG-INFO` & `mppsolar-0.9.12/mppsolar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mppsolar
-Version: 0.9.1
+Version: 0.9.12
 Summary: Package to communicate with Solar inverters and BMSs
 Home-page: https://github.com/jblance/mpp-solar
 Author: John Blance
 Author-email: 
 License: MIT
 Keywords: hardware serial communication
 Platform: UNKNOWN
@@ -43,15 +43,15 @@
 
 ## Compute hardware support ##
 The python code is designed to run on Linux type python environments using python 3.6 or newer
 
 [Hardware that has been known to work](https://github.com/jblance/mpp-solar/blob/master/docs/hardware.md)
 
 ## Installation ##
-* to get the latest stable version: `sudo pip install mpp-solar`
+* to get the latest stable version: `sudo pip install mppsolar`
 * [more installation options](https://github.com/jblance/mpp-solar/blob/master/docs/installation.md)
 
 ## Usage ###
 `$ mpp-solar -h` or `$ jkbms -h` will display the available options
 
 [More detailed usage](https://github.com/jblance/mpp-solar/blob/master/docs/usage.md)
```

### Comparing `mppsolar-0.9.1/mppsolar.egg-info/SOURCES.txt` & `mppsolar-0.9.12/mppsolar.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,28 @@
 mppsolar/io/serialio.py
 mppsolar/io/testio.py
 mppsolar/io/vserialio.py
 mppsolar/libs/__init__.py
 mppsolar/libs/mqttbroker.py
 mppsolar/outputs/__init__.py
 mppsolar/outputs/baseoutput.py
+mppsolar/outputs/domoticz_autodiscover.py
+mppsolar/outputs/domoticz_mqtt.py
 mppsolar/outputs/hass_mqtt.py
 mppsolar/outputs/influx2_mqtt.py
 mppsolar/outputs/influx_mqtt.py
 mppsolar/outputs/json.py
 mppsolar/outputs/json_mqtt.py
 mppsolar/outputs/mqtt.py
 mppsolar/outputs/raw.py
 mppsolar/outputs/screen.py
 mppsolar/outputs/tag_mqtt.py
+mppsolar/ports/__init__.py
+mppsolar/ports/port.py
+mppsolar/ports/test.py
 mppsolar/protocols/__init__.py
 mppsolar/protocols/abstractprotocol.py
 mppsolar/protocols/daly.py
 mppsolar/protocols/daly40.py
 mppsolar/protocols/jk02.py
 mppsolar/protocols/jk04.py
 mppsolar/protocols/jk232.py
```

### Comparing `mppsolar-0.9.1/setup.py` & `mppsolar-0.9.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     install_requires=["pyserial", "paho-mqtt"],
     # install_requires=[],
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
-        "dev": ["check-manifest"],
+        "dev": ["check-manifest", "flake8", "build"],
         "test": ["coverage"],
     },
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
     entry_points={
         "console_scripts": [
```

