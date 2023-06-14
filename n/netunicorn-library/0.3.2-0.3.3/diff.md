# Comparing `tmp/netunicorn-library-0.3.2.tar.gz` & `tmp/netunicorn-library-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-library-0.3.2.tar", last modified: Sat Jun 10 04:38:42 2023, max compression
+gzip compressed data, was "netunicorn-library-0.3.3.tar", last modified: Wed Jun 14 05:02:46 2023, max compression
```

## Comparing `netunicorn-library-0.3.2.tar` & `netunicorn-library-0.3.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.255766 netunicorn-library-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.255766 netunicorn-library-0.3.2/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.255766 netunicorn-library-0.3.2/src/netunicorn/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.255766 netunicorn-library-0.3.2/src/netunicorn/library/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/pipelines/measurements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/pipelines/measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/capture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/capture/tcpdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/letsencrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/letsencrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/letsencrypt/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/measurements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/measurements/ookla_speedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/measurements/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/arp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/arp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/arp/spoof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/cve202141773/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/heartbleed/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/icmp/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/icmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/icmp/redirection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/land/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/land/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/land/landattack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/log4j/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.259767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/loris/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/loris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mac/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mac/flooder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/qoe_youtube/
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/qoe_youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/qoe_youtube/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/upload/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/upload/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/utils/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-10 04:38:28.000000 netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:38:42.263767 netunicorn-library-0.3.2/src/netunicorn_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-10 04:38:42.000000 netunicorn-library-0.3.2/src/netunicorn_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-10 04:38:42.000000 netunicorn-library-0.3.2/src/netunicorn_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 04:38:42.000000 netunicorn-library-0.3.2/src/netunicorn_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-10 04:38:42.000000 netunicorn-library-0.3.2/src/netunicorn_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-10 04:38:42.000000 netunicorn-library-0.3.2/src/netunicorn_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.702647 netunicorn-library-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 05:02:46.702647 netunicorn-library-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 05:02:46.702647 netunicorn-library-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.694647 netunicorn-library-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.694647 netunicorn-library-0.3.3/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.694647 netunicorn-library-0.3.3/src/netunicorn/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.694647 netunicorn-library-0.3.3/src/netunicorn/library/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/pipelines/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/pipelines/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/capture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/capture/tcpdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/letsencrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/letsencrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/letsencrypt/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/measurements/ookla_speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/measurements/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/arp/spoof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/cve202141773/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/heartbleed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/icmp/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/icmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/icmp/redirection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/land/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/land/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/land/landattack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/log4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/loris/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/loris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mac/flooder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.698647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/qoe_youtube/
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/qoe_youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/qoe_youtube/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.702647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/upload/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/upload/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.702647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/utils/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.702647 netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-14 05:02:35.000000 netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:02:46.702647 netunicorn-library-0.3.3/src/netunicorn_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 05:02:46.000000 netunicorn-library-0.3.3/src/netunicorn_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-14 05:02:46.000000 netunicorn-library-0.3.3/src/netunicorn_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:02:46.000000 netunicorn-library-0.3.3/src/netunicorn_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 05:02:46.000000 netunicorn-library-0.3.3/src/netunicorn_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 05:02:46.000000 netunicorn-library-0.3.3/src/netunicorn_library.egg-info/top_level.txt
```

### Comparing `netunicorn-library-0.3.2/pyproject.toml` & `netunicorn-library-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-library"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn contrib library"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
@@ -17,8 +17,8 @@
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "netunicorn-base >= 0.3.1",
 ]
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
```

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py` & `netunicorn-library-0.3.3/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/basic.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/basic.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/capture/tcpdump.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/capture/tcpdump.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         raise NotImplementedError(
             f'StopCapture is not implemented for {node.architecture}'
         )
 
 
 class StopNamedCaptureLinuxImplementation(Task):
-    requirements = ["sudo apt-get update", "sudo apt-get install -y tcpdump"]
+    requirements = ["sudo apt-get update", "sudo apt-get install -y tcpdump", "sudo apt-get install -y procps"]
 
     def __init__(self, capture_task_name: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.capture_task_name = capture_task_name
 
     def run(self):
         signal.signal(signal.SIGCHLD, signal.SIG_IGN)
```

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/flags.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/flags.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/letsencrypt/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/letsencrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/letsencrypt/tasks.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/letsencrypt/tasks.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/measurements/ookla_speedtest.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/measurements/ookla_speedtest.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/measurements/ping.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/measurements/ping.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,21 +27,22 @@
     unit_rtt: str
     unparsed_output: List[str]
     raw_output: str
 
 
 class Ping(TaskDispatcher):
     def __init__(self, address: str, count: int = 1, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.address = address
         self.count = count
-        super().__init__(*args, **kwargs)
+        self.linux_implementation = PingLinuxImplementation(self.address, self.count)
 
     def dispatch(self, node: Node) -> Task:
         if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
-            return PingLinuxImplementation(self.address, self.count)
+            return self.linux_implementation
         raise NotImplementedError(
             f'Ping is not implemented for architecture: {node.architecture}'
         )
 
 
 class PingLinuxImplementation(Task):
     requirements = ["sudo apt-get install -y inetutils-ping"]
```

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/arp/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/arp/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/land/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/land/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/loris/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/loris/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mail/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/qoe_youtube/__init__.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/qoe_youtube/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 from netunicorn.base import Failure, Success, Task, TaskDispatcher, is_successful
 
 
 class StartQoECollectionServer(TaskDispatcher):
     def __init__(
         self, data_folder: str = ".", interface: str = "0.0.0.0", port: int = 34543, *args, **kwargs,
     ):
+        super().__init__(*args, **kwargs)
         self.data_folder = data_folder
         self.interface = interface
         self.port = port
-        super().__init__(*args, **kwargs)
+        self.linux_implementation = StartQoECollectionServerLinuxImplementation(
+                self.data_folder, self.interface, self.port, name=self.name
+            )
 
     def dispatch(self, node: Node) -> Task:
         if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
-            return StartQoECollectionServerLinuxImplementation(
-                self.data_folder, self.interface, self.port, name=self.name
-            )
+            return self.linux_implementation
 
         raise NotImplementedError(
             f'StartQoECollectionServer is not implemented for {node.architecture}'
         )
 
 
 class StartQoECollectionServerLinuxImplementation(Task):
@@ -73,20 +74,23 @@
             f"using interface {self.interface}:{self.port}, process ID: {process.pid}",
             process.pid,
         )
 
 
 class StopQoECollectionServer(TaskDispatcher):
     def __init__(self, start_task_name: str, *args, **kwargs):
-        self.start_task_name = start_task_name
         super().__init__(*args, **kwargs)
+        self.start_task_name = start_task_name
+        self.linux_implementation = StopQoECollectionServerLinuxImplementation(
+            start_task_name=self.start_task_name, name=self.name
+        )
 
     def dispatch(self, node: Node) -> Task:
         if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
-            return StopQoECollectionServerLinuxImplementation(start_task_name=self.start_task_name, name=self.name)
+            return self.linux_implementation
 
         raise NotImplementedError(
             f'StopQoECollectionServer is not implemented for {node.architecture}'
         )
 
 
 class StopQoECollectionServerLinuxImplementation(Task):
@@ -119,27 +123,28 @@
         self.video_url = video_url
         self.duration = duration
         self.quality = quality
         self.qoe_server_address = qoe_server_address
         self.qoe_server_port = qoe_server_port
         self.report_time = report_time
         super().__init__(*args, **kwargs)
-
-    def dispatch(self, node: Node) -> Task:
-        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
-            return WatchYouTubeVideoLinuxImplementation(
+        self.linux_implementation = WatchYouTubeVideoLinuxImplementation(
                 self.video_url,
                 self.duration,
                 self.quality,
                 self.qoe_server_address,
                 self.qoe_server_port,
                 self.report_time,
                 name=self.name,
             )
 
+    def dispatch(self, node: Node) -> Task:
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
+            return self.linux_implementation
+
         raise NotImplementedError(
             f'WatchYouTubeVideo is not implemented for architecture: {node.architecture}'
         )
 
 
 class WatchYouTubeVideoLinuxImplementation(Task):
     requirements = [
```

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/qoe_youtube/watcher.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/qoe_youtube/watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/upload/fileio.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/upload/fileio.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/upload/webdav.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/upload/webdav.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/utils/sleep.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py` & `netunicorn-library-0.3.3/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.2/src/netunicorn_library.egg-info/SOURCES.txt` & `netunicorn-library-0.3.3/src/netunicorn_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

