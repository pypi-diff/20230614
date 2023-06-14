# Comparing `tmp/pyjoulescope_driver-1.3.8.tar.gz` & `tmp/pyjoulescope_driver-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoulescope_driver-1.3.8.tar", last modified: Tue May 16 19:16:28 2023, max compression
+gzip compressed data, was "pyjoulescope_driver-1.3.9.tar", last modified: Wed May 17 18:35:47 2023, max compression
```

## Comparing `pyjoulescope_driver-1.3.8.tar` & `pyjoulescope_driver-1.3.9.tar`

### file list

```diff
@@ -1,405 +1,405 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.696563 pyjoulescope_driver-1.3.8/
--rw-rw-rw-   0        0        0     8166 2023-05-16 18:51:22.000000 pyjoulescope_driver-1.3.8/CHANGELOG.md
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjoulescope_driver-1.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0      345 2022-11-19 20:38:00.000000 pyjoulescope_driver-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5170 2023-05-16 19:16:28.696563 pyjoulescope_driver-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3360 2023-01-03 21:53:29.000000 pyjoulescope_driver-1.3.8/README.md
--rw-rw-rw-   0        0        0     6268 2022-09-20 19:25:49.000000 pyjoulescope_driver-1.3.8/credits.html
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.498444 pyjoulescope_driver-1.3.8/include/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.502444 pyjoulescope_driver-1.3.8/include/jsdrv/
--rw-rw-rw-   0        0        0     2698 2022-11-08 21:41:45.000000 pyjoulescope_driver-1.3.8/include/jsdrv/cmacro_inc.h
--rw-rw-rw-   0        0        0     8332 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.8/include/jsdrv/cstr.h
--rw-rw-rw-   0        0        0     5878 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.8/include/jsdrv/error_code.h
--rw-rw-rw-   0        0        0     6817 2023-04-14 18:25:40.000000 pyjoulescope_driver-1.3.8/include/jsdrv/log.h
--rw-rw-rw-   0        0        0     2002 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include/jsdrv/meta.h
--rw-rw-rw-   0        0        0    13863 2023-05-16 17:50:16.000000 pyjoulescope_driver-1.3.8/include/jsdrv/time.h
--rw-rw-rw-   0        0        0     3827 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.8/include/jsdrv/topic.h
--rw-rw-rw-   0        0        0    12351 2022-08-01 20:41:48.000000 pyjoulescope_driver-1.3.8/include/jsdrv/union.h
--rw-rw-rw-   0        0        0     4083 2023-05-16 18:52:20.000000 pyjoulescope_driver-1.3.8/include/jsdrv/version.h
--rw-rw-rw-   0        0        0    29282 2023-04-14 12:30:28.000000 pyjoulescope_driver-1.3.8/include/jsdrv.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.502444 pyjoulescope_driver-1.3.8/include_private/
--rw-rw-rw-   0        0        0    13394 2022-10-27 14:05:41.000000 pyjoulescope_driver-1.3.8/include_private/js220_api.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.514967 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/
--rw-rw-rw-   0        0        0     1683 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/assert.h
--rw-rw-rw-   0        0        0     2116 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/backend.h
--rw-rw-rw-   0        0        0     2774 2023-04-12 17:01:55.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/buffer.h
--rw-rw-rw-   0        0        0     3987 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/buffer_signal.h
--rw-rw-rw-   0        0        0     7138 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/cdef.h
--rw-rw-rw-   0        0        0     5647 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/dbc.h
--rw-rw-rw-   0        0        0     1385 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/device.h
--rw-rw-rw-   0        0        0     1291 2022-07-28 13:15:21.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/devices.h
--rw-rw-rw-   0        0        0     1633 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/downsample.h
--rw-rw-rw-   0        0        0     1960 2022-09-19 13:38:02.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/event.h
--rw-rw-rw-   0        0        0     6987 2023-03-19 15:49:32.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/frontend.h
--rw-rw-rw-   0        0        0     1408 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js110_cal.h
--rw-rw-rw-   0        0        0     3046 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js110_sample_processor.h
--rw-rw-rw-   0        0        0     2858 2022-11-01 15:41:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js110_stats.h
--rw-rw-rw-   0        0        0     1647 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js220_i128.h
--rw-rw-rw-   0        0        0     1558 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js220_stats.h
--rw-rw-rw-   0        0        0     3780 2022-08-01 13:11:32.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/json.h
--rw-rw-rw-   0        0        0    14035 2022-09-18 11:31:10.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/list.h
--rw-rw-rw-   0        0        0     8973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/log.h
--rw-rw-rw-   0        0        0     1650 2022-09-19 12:36:34.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/msg_queue.h
--rw-rw-rw-   0        0        0     2561 2022-07-28 13:01:35.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/mutex.h
--rw-rw-rw-   0        0        0     5113 2023-05-16 18:29:34.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/platform.h
--rw-rw-rw-   0        0        0     4061 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/pubsub.h
--rw-rw-rw-   0        0        0     2799 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/sample_buffer_f32.h
--rw-rw-rw-   0        0        0     4561 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/statistics.h
--rw-rw-rw-   0        0        0     1979 2023-05-16 18:29:03.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/thread.h
--rw-rw-rw-   0        0        0     8210 2022-07-29 18:34:03.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/usb_spec.h
--rw-rw-rw-   0        0        0     1533 2022-10-09 18:53:30.000000 pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/windows.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.521501 pyjoulescope_driver-1.3.8/pyjoulescope_driver/
--rw-rw-rw-   0        0        0      964 2023-03-29 21:30:50.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-03-29 21:47:21.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/__main__.py
--rw-rw-rw-   0        0        0  1592784 2023-04-28 17:29:48.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/binding.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.530033 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/
--rw-rw-rw-   0        0        0     1006 2023-05-10 12:27:33.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-04-14 19:51:53.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/api_timeout.py
--rw-rw-rw-   0        0        0     1830 2023-01-25 14:57:14.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/gpi.py
--rw-rw-rw-   0        0        0     6545 2023-05-10 12:33:10.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/info.py
--rw-rw-rw-   0        0        0     4213 2022-10-30 15:18:19.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/program.py
--rw-rw-rw-   0        0        0     5031 2023-04-13 12:02:12.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/record.py
--rw-rw-rw-   0        0        0      932 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/scan.py
--rw-rw-rw-   0        0        0     2410 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/set_parameter.py
--rw-rw-rw-   0        0        0     2981 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/statistics.py
--rw-rw-rw-   0        0        0     3723 2023-04-14 13:21:57.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/threads.py
--rw-rw-rw-   0        0        0   610304 2023-05-16 19:16:27.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/img_alpha.img
--rw-rw-rw-   0        0        0   610304 2023-05-16 19:16:27.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/img_beta.img
--rw-rw-rw-   0        0        0   609280 2023-05-16 19:16:27.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/img_stable.img
--rw-rw-rw-   0        0        0    10359 2023-04-15 14:37:51.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/program.py
--rw-rw-rw-   0        0        0     8451 2023-04-28 18:34:52.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/record.py
--rw-rw-rw-   0        0        0     8980 2022-11-11 19:24:16.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/release.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.531034 pyjoulescope_driver-1.3.8/pyjoulescope_driver/test/
--rw-rw-rw-   0        0        0        0 2022-10-09 12:38:26.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/test/__init__.py
--rw-rw-rw-   0        0        0     1901 2022-10-09 17:17:09.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/test/test_release.py
--rw-rw-rw-   0        0        0     2304 2023-03-29 16:02:01.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/test/test_time64.py
--rw-rw-rw-   0        0        0     4660 2023-03-29 16:00:59.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/time64.py
--rw-rw-rw-   0        0        0     1063 2023-05-16 18:52:20.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver/version.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.525004 pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/
--rw-rw-rw-   0        0        0     5170 2023-05-16 19:16:28.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13694 2023-05-16 19:16:28.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:16:28.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-16 19:16:28.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       69 2023-05-16 19:16:28.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-16 19:16:28.000000 pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1076 2023-04-28 13:51:47.000000 pyjoulescope_driver-1.3.8/pyproject.toml
--rw-rw-rw-   0        0        0      117 2023-05-16 19:16:28.696563 pyjoulescope_driver-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0    10352 2023-05-09 12:46:24.000000 pyjoulescope_driver-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.544124 pyjoulescope_driver-1.3.8/src/
--rw-rw-rw-   0        0        0     2821 2023-05-16 19:02:12.000000 pyjoulescope_driver-1.3.8/src/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.546157 pyjoulescope_driver-1.3.8/src/backend/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.547688 pyjoulescope_driver-1.3.8/src/backend/libusb/
--rw-rw-rw-   0        0        0    30330 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.8/src/backend/libusb/backend.c
--rw-rw-rw-   0        0        0     4580 2022-09-19 12:40:12.000000 pyjoulescope_driver-1.3.8/src/backend/libusb/msg_queue.c
--rw-rw-rw-   0        0        0     5503 2023-04-14 20:55:21.000000 pyjoulescope_driver-1.3.8/src/backend/posix.c
--rw-rw-rw-   0        0        0     6886 2023-04-14 20:54:20.000000 pyjoulescope_driver-1.3.8/src/backend/windows.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.548692 pyjoulescope_driver-1.3.8/src/backend/winusb/
--rw-rw-rw-   0        0        0    38641 2023-04-04 15:07:16.000000 pyjoulescope_driver-1.3.8/src/backend/winusb/backend.c
--rw-rw-rw-   0        0        0     7713 2022-09-18 12:51:07.000000 pyjoulescope_driver-1.3.8/src/backend/winusb/device_change_notifier.c
--rw-rw-rw-   0        0        0     2798 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/src/backend/winusb/device_change_notifier.h
--rw-rw-rw-   0        0        0     4807 2023-03-19 16:29:53.000000 pyjoulescope_driver-1.3.8/src/backend/winusb/msg_queue.c
--rw-rw-rw-   0        0        0    25694 2023-04-21 20:34:16.000000 pyjoulescope_driver-1.3.8/src/buffer.c
--rw-rw-rw-   0        0        0    32686 2023-04-28 18:46:11.000000 pyjoulescope_driver-1.3.8/src/buffer_signal.c
--rw-rw-rw-   0        0        0    11771 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/src/cstr.c
--rw-rw-rw-   0        0        0     1671 2022-09-19 11:52:36.000000 pyjoulescope_driver-1.3.8/src/devices.c
--rw-rw-rw-   0        0        0     8709 2022-10-24 15:34:41.000000 pyjoulescope_driver-1.3.8/src/downsample.c
--rw-rw-rw-   0        0        0     5925 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.8/src/emu.c
--rw-rw-rw-   0        0        0     4649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/src/emulated.c
--rw-rw-rw-   0        0        0     4817 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.8/src/error_code.c
--rw-rw-rw-   0        0        0     9335 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/src/js110_api.h
--rw-rw-rw-   0        0        0     3972 2022-09-18 11:26:57.000000 pyjoulescope_driver-1.3.8/src/js110_cal.c
--rw-rw-rw-   0        0        0     9038 2022-11-01 14:07:47.000000 pyjoulescope_driver-1.3.8/src/js110_sample_processor.c
--rw-rw-rw-   0        0        0     4551 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.8/src/js110_stats.c
--rw-rw-rw-   0        0        0    52738 2023-04-27 16:54:44.000000 pyjoulescope_driver-1.3.8/src/js110_usb.c
--rw-rw-rw-   0        0        0     5162 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.8/src/js220_i128.c
--rw-rw-rw-   0        0        0     1188 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.8/src/js220_params.c
--rw-rw-rw-   0        0        0     2893 2022-10-05 01:35:24.000000 pyjoulescope_driver-1.3.8/src/js220_stats.c
--rw-rw-rw-   0        0        0    62976 2023-04-20 12:52:32.000000 pyjoulescope_driver-1.3.8/src/js220_usb.c
--rw-rw-rw-   0        0        0    37782 2023-04-14 12:55:05.000000 pyjoulescope_driver-1.3.8/src/jsdrv.c
--rw-rw-rw-   0        0        0    10974 2022-08-01 18:37:59.000000 pyjoulescope_driver-1.3.8/src/json.c
--rw-rw-rw-   0        0        0    16499 2023-04-14 20:57:15.000000 pyjoulescope_driver-1.3.8/src/log.c
--rw-rw-rw-   0        0        0    10627 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.8/src/meta.c
--rw-rw-rw-   0        0        0    24211 2023-03-19 15:32:24.000000 pyjoulescope_driver-1.3.8/src/pubsub.c
--rw-rw-rw-   0        0        0     4944 2022-10-07 12:24:15.000000 pyjoulescope_driver-1.3.8/src/sample_buffer_f32.c
--rw-rw-rw-   0        0        0     5262 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.8/src/statistics.c
--rw-rw-rw-   0        0        0     2814 2023-03-09 19:53:59.000000 pyjoulescope_driver-1.3.8/src/time.c
--rw-rw-rw-   0        0        0     3763 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.8/src/topic.c
--rw-rw-rw-   0        0        0    12780 2022-09-18 11:32:07.000000 pyjoulescope_driver-1.3.8/src/union.c
--rw-rw-rw-   0        0        0     1001 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/src/version.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.549692 pyjoulescope_driver-1.3.8/third-party/
--rw-rw-rw-   0        0        0      810 2022-09-20 18:21:09.000000 pyjoulescope_driver-1.3.8/third-party/CMakeLists.txt
--rw-rw-rw-   0        0        0      364 2022-08-01 20:40:07.000000 pyjoulescope_driver-1.3.8/third-party/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.560232 pyjoulescope_driver-1.3.8/third-party/cmocka/
--rw-rw-rw-   0        0        0       18 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/.clang_complete
--rw-rw-rw-   0        0        0     9611 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     3508 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/.ycm_extra_conf.py
--rw-rw-rw-   0        0        0     1209 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/5.patch
--rw-rw-rw-   0        0        0     3601 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/CMakeLists.txt
--rw-rw-rw-   0        0        0     1845 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/CPackConfig.cmake
--rw-rw-rw-   0        0        0      284 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/CTestConfig.cmake
--rw-rw-rw-   0        0        0     5331 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/CompilerChecks.cmake
--rw-rw-rw-   0        0        0     4648 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/ConfigureChecks.cmake
--rw-rw-rw-   0        0        0      431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/DefineOptions.cmake
--rw-rw-rw-   0        0        0     3217 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/INSTALL.md
--rw-rw-rw-   0        0        0      658 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.562233 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.567758 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/
--rw-rw-rw-   0        0        0      866 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
--rw-rw-rw-   0        0        0     3360 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
--rw-rw-rw-   0        0        0     1952 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
--rw-rw-rw-   0        0        0      811 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
--rw-rw-rw-   0        0        0     3973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
--rw-rw-rw-   0        0        0      585 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
--rw-rw-rw-   0        0        0     1480 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/FindNSIS.cmake
--rw-rw-rw-   0        0        0      680 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
--rw-rw-rw-   0        0        0      656 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
--rw-rw-rw-   0        0        0     1145 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
--rw-rw-rw-   0        0        0       53 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmocka-build-tree-settings.cmake.in
--rw-rw-rw-   0        0        0      507 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmocka-config.cmake.in
--rw-rw-rw-   0        0        0      189 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/cmocka.pc.cmake
--rw-rw-rw-   0        0        0     5161 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/config.h.cmake
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.568761 pyjoulescope_driver-1.3.8/third-party/cmocka/coverity/
--rw-rw-rw-   0        0        0     3918 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/coverity/coverity_assert_model.c
--rw-rw-rw-   0        0        0      142 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/coverity/coverity_internal_model.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.570854 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/
--rw-rw-rw-   0        0        0     2206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/CMakeLists.txt
--rw-rw-rw-   0        0        0    26974 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/index.html
--rw-rw-rw-   0        0        0     5291 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/mainpage.dox
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.572853 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/
--rw-rw-rw-   0        0        0     1301 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/README.md
--rw-rw-rw-   0        0        0     2121 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/header.html
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.578891 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/
--rw-rw-rw-   0        0        0     6714 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/doc.svg
--rw-rw-rw-   0        0        0     3604 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/folderclosed.svg
--rw-rw-rw-   0        0        0     4299 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/folderopen.svg
--rw-rw-rw-   0        0        0     3955 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/mag_glass.svg
--rw-rw-rw-   0        0        0     3988 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
--rw-rw-rw-   0        0        0     3249 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
--rw-rw-rw-   0        0        0     3262 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
--rw-rw-rw-   0        0        0     7409 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
--rw-rw-rw-   0        0        0      483 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/sync_off.png
--rw-rw-rw-   0        0        0      488 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/sync_on.png
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.578891 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/js/
--rw-rw-rw-   0        0        0      977 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/js/striped_bg.js
--rw-rw-rw-   0        0        0    32455 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/that_style.css
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.588293 pyjoulescope_driver-1.3.8/third-party/cmocka/example/
--rw-rw-rw-   0        0        0     2562 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/CMakeLists.txt
--rw-rw-rw-   0        0        0     1755 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/allocate_module.c
--rw-rw-rw-   0        0        0     1640 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/allocate_module_test.c
--rw-rw-rw-   0        0        0     1254 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_macro.c
--rw-rw-rw-   0        0        0      144 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_macro.h
--rw-rw-rw-   0        0        0     1649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_macro_test.c
--rw-rw-rw-   0        0        0     1216 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_module.c
--rw-rw-rw-   0        0        0      692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_module.h
--rw-rw-rw-   0        0        0     1692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_module_test.c
--rw-rw-rw-   0        0        0     9746 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/calculator.c
--rw-rw-rw-   0        0        0    16244 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/calculator_test.c
--rw-rw-rw-   0        0        0     1439 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/database.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.588293 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/
--rw-rw-rw-   0        0        0      197 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.591803 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/
--rw-rw-rw-   0        0        0      620 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
--rw-rw-rw-   0        0        0     1431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/chef.c
--rw-rw-rw-   0        0        0      789 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/chef.h
--rw-rw-rw-   0        0        0     5222 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
--rw-rw-rw-   0        0        0       61 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.594803 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/
--rw-rw-rw-   0        0        0      685 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/CMakeLists.txt
--rw-rw-rw-   0        0        0     2033 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/README.md
--rw-rw-rw-   0        0        0     1882 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/proc_uptime.c
--rw-rw-rw-   0        0        0      793 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/proc_uptime.h
--rw-rw-rw-   0        0        0     5237 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/test_uptime.c
--rw-rw-rw-   0        0        0     3305 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/uptime.c
--rw-rw-rw-   0        0        0      415 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/example/simple_test.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.597310 pyjoulescope_driver-1.3.8/third-party/cmocka/include/
--rw-rw-rw-   0        0        0      465 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/include/CMakeLists.txt
--rw-rw-rw-   0        0        0    77952 2022-08-01 20:01:08.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmocka.h
--rw-rw-rw-   0        0        0     1893 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmocka_pbc.h
--rw-rw-rw-   0        0        0     4137 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmocka_private.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.598326 pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmockery/
--rw-rw-rw-   0        0        0       21 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmockery/cmockery.h
--rw-rw-rw-   0        0        0       25 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmockery/pbc.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.599329 pyjoulescope_driver-1.3.8/third-party/cmocka/src/
--rw-rw-rw-   0        0        0     3668 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/src/CMakeLists.txt
--rw-rw-rw-   0        0        0   119941 2022-09-18 17:05:56.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/src/cmocka.c
--rw-rw-rw-   0        0        0     1174 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/src/cmocka.def
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.614611 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/
--rw-rw-rw-   0        0        0     7657 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0     6215 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/cmocka_test.cmake
--rw-rw-rw-   0        0        0     2758 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/ctest-default.cmake
--rw-rw-rw-   0        0        0     1922 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_alloc.c
--rw-rw-rw-   0        0        0      818 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_assert_macros.c
--rw-rw-rw-   0        0        0      862 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_assert_macros_fail.c
--rw-rw-rw-   0        0        0     1550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_basics.c
--rw-rw-rw-   0        0        0      970 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_cmockery.c
--rw-rw-rw-   0        0        0      869 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_exception_handler.c
--rw-rw-rw-   0        0        0     1774 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_fixtures.c
--rw-rw-rw-   0        0        0     1206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_float_macros.c
--rw-rw-rw-   0        0        0      992 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_group_fixtures.c
--rw-rw-rw-   0        0        0      699 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_group_setup_assert.c
--rw-rw-rw-   0        0        0      696 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_group_setup_fail.c
--rw-rw-rw-   0        0        0     1757 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_groups.c
--rw-rw-rw-   0        0        0     2767 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_ordering.c
--rw-rw-rw-   0        0        0     2420 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_ordering_fail.c
--rw-rw-rw-   0        0        0     1577 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_returns.c
--rw-rw-rw-   0        0        0     1704 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_returns_fail.c
--rw-rw-rw-   0        0        0     1092 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_setup_fail.c
--rw-rw-rw-   0        0        0     1043 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_skip.c
--rw-rw-rw-   0        0        0     1362 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_skip_filter.c
--rw-rw-rw-   0        0        0     2280 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_strmatch.c
--rw-rw-rw-   0        0        0     1260 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_wildcard.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.621657 pyjoulescope_driver-1.3.8/third-party/libusb/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.621657 pyjoulescope_driver-1.3.8/third-party/libusb/.github/
--rw-rw-rw-   0        0        0      719 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.github/cifuzz.yml
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.623657 pyjoulescope_driver-1.3.8/third-party/libusb/.github/workflows/
--rw-rw-rw-   0        0        0     1188 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.github/workflows/linux.yml
--rw-rw-rw-   0        0        0     1023 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0      527 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.github/workflows/msys2.yml
--rw-rw-rw-   0        0        0      827 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.628683 pyjoulescope_driver-1.3.8/third-party/libusb/.private/
--rw-rw-rw-   0        0        0      202 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/README.txt
--rw-rw-rw-   0        0        0      548 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/appveyor_build.sh
--rw-rw-rw-   0        0        0     1424 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/bm.sh
--rw-rw-rw-   0        0        0     1109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/ci-build.sh
--rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/ci-container-build.sh
--rw-rw-rw-   0        0        0      959 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/post-rewrite.sh
--rw-rw-rw-   0        0        0     1995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/pre-commit.sh
--rw-rw-rw-   0        0        0     2545 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.private/wbs.txt
--rw-rw-rw-   0        0        0     1465 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/.travis.yml
--rw-rw-rw-   0        0        0     2523 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.8/third-party/libusb/CMakeLists.txt
--rw-rw-rw-   0        0        0     1972 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/INSTALL_WIN.txt
--rw-rw-rw-   0        0        0     1495 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Makefile.am
--rw-rw-rw-   0        0        0     1395 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/README-FORK.md
--rw-rw-rw-   0        0        0     1894 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/README.git
--rw-rw-rw-   0        0        0        6 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.632703 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/
--rw-rw-rw-   0        0        0     2409 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/common.xcconfig
--rw-rw-rw-   0        0        0      995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/config.h
--rw-rw-rw-   0        0        0     1135 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/debug.xcconfig
--rw-rw-rw-   0        0        0      988 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb.xcconfig
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.632703 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb.xcodeproj/
--rw-rw-rw-   0        0        0    62286 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
--rw-rw-rw-   0        0        0      963 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb_debug.xcconfig
--rw-rw-rw-   0        0        0      965 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb_release.xcconfig
--rw-rw-rw-   0        0        0     1208 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/release.xcconfig
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.633703 pyjoulescope_driver-1.3.8/third-party/libusb/android/
--rw-rw-rw-   0        0        0     2016 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/config.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.634703 pyjoulescope_driver-1.3.8/third-party/libusb/android/examples/
--rw-rw-rw-   0        0        0    11355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/examples/unrooted_android.c
--rw-rw-rw-   0        0        0     1156 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/examples/unrooted_android.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.637720 pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/
--rw-rw-rw-   0        0        0      997 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/Android.mk
--rw-rw-rw-   0        0        0     1370 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/Application.mk
--rw-rw-rw-   0        0        0     3425 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/examples.mk
--rw-rw-rw-   0        0        0     2056 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/libusb.mk
--rw-rw-rw-   0        0        0     1355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/tests.mk
--rw-rw-rw-   0        0        0     3820 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/appveyor.yml
--rw-rw-rw-   0        0        0      191 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/autogen.sh
--rw-rw-rw-   0        0        0      109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/bootstrap.sh
--rw-rw-rw-   0        0        0    16514 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/configure.ac
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.639740 pyjoulescope_driver-1.3.8/third-party/libusb/doc/
--rw-rw-rw-   0        0        0      685 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/doc/Makefile.in
--rw-rw-rw-   0        0        0   115647 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/doc/doxygen.cfg.in
--rw-rw-rw-   0        0        0     2923 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/doc/libusb.png
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.646518 pyjoulescope_driver-1.3.8/third-party/libusb/examples/
--rw-rw-rw-   0        0        0      416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/Makefile.am
--rw-rw-rw-   0        0        0    15812 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/dpfp.c
--rw-rw-rw-   0        0        0    24573 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/ezusb.c
--rw-rw-rw-   0        0        0     4247 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/ezusb.h
--rw-rw-rw-   0        0        0     9593 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/fxload.c
--rw-rw-rw-   0        0        0     3580 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/hotplugtest.c
--rw-rw-rw-   0        0        0     2081 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/listdevs.c
--rw-rw-rw-   0        0        0     6149 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/sam3u_benchmark.c
--rw-rw-rw-   0        0        0     9765 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/testlibusb.c
--rw-rw-rw-   0        0        0    40008 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/examples/xusb.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.494420 pyjoulescope_driver-1.3.8/third-party/libusb/include/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.646518 pyjoulescope_driver-1.3.8/third-party/libusb/include/linux/
--rw-rw-rw-   0        0        0     5104 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.8/third-party/libusb/include/linux/config.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.648539 pyjoulescope_driver-1.3.8/third-party/libusb/include/macos/
--rw-rw-rw-   0        0        0     5130 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/include/macos/config.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.656759 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/
--rw-rw-rw-   0        0        0     2539 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/Makefile.am
--rw-rw-rw-   0        0        0      780 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/Makefile.am.extra
--rw-rw-rw-   0        0        0    99186 2022-09-20 23:33:57.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/core.c
--rw-rw-rw-   0        0        0    37583 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/descriptor.c
--rw-rw-rw-   0        0        0    15552 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/hotplug.c
--rw-rw-rw-   0        0        0   113897 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/io.c
--rw-rw-rw-   0        0        0     8221 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusb-1.0.def
--rw-rw-rw-   0        0        0     1642 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusb-1.0.rc
--rw-rw-rw-   0        0        0    78746 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusb.h
--rw-rw-rw-   0        0        0    53532 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusbi.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.677071 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/
--rw-rw-rw-   0        0        0   103226 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/darwin_usb.c
--rw-rw-rw-   0        0        0     7071 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/darwin_usb.h
--rw-rw-rw-   0        0        0    24325 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/emscripten_webusb.cpp
--rw-rw-rw-   0        0        0     9581 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_posix.c
--rw-rw-rw-   0        0        0     1776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_posix.h
--rw-rw-rw-   0        0        0     6948 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_windows.c
--rw-rw-rw-   0        0        0     1520 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_windows.h
--rw-rw-rw-   0        0        0     7884 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_pollfs.cpp
--rw-rw-rw-   0        0        0     3386 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb.h
--rw-rw-rw-   0        0        0    16687 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb_backend.cpp
--rw-rw-rw-   0        0        0     7477 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb_raw.cpp
--rw-rw-rw-   0        0        0     4080 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb_raw.h
--rw-rw-rw-   0        0        0    10778 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_netlink.c
--rw-rw-rw-   0        0        0     8864 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_udev.c
--rw-rw-rw-   0        0        0    83335 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_usbfs.c
--rw-rw-rw-   0        0        0     6551 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_usbfs.h
--rw-rw-rw-   0        0        0    16279 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/netbsd_usb.c
--rw-rw-rw-   0        0        0     2996 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/null_usb.c
--rw-rw-rw-   0        0        0    18179 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/openbsd_usb.c
--rw-rw-rw-   0        0        0    45204 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/sunos_usb.c
--rw-rw-rw-   0        0        0     2254 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/sunos_usb.h
--rw-rw-rw-   0        0        0     3488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_posix.c
--rw-rw-rw-   0        0        0     3052 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_posix.h
--rw-rw-rw-   0        0        0     1416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_windows.c
--rw-rw-rw-   0        0        0     3280 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_windows.h
--rw-rw-rw-   0        0        0    30524 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_common.c
--rw-rw-rw-   0        0        0    14347 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_common.h
--rw-rw-rw-   0        0        0    24491 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_usbdk.c
--rw-rw-rw-   0        0        0     2926 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_usbdk.h
--rw-rw-rw-   0        0        0   171316 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_winusb.c
--rw-rw-rw-   0        0        0    24670 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_winusb.h
--rw-rw-rw-   0        0        0     8776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/strerror.c
--rw-rw-rw-   0        0        0    13160 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/sync.c
--rw-rw-rw-   0        0        0      449 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/version.h
--rw-rw-rw-   0        0        0       27 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb/version_nano.h
--rw-rw-rw-   0        0        0      323 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/libusb-1.0.pc.in
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.689539 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/
--rw-rw-rw-   0        0        0      136 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/.gitattributes
--rw-rw-rw-   0        0        0     2982 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Base.props
--rw-rw-rw-   0        0        0      287 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Configuration.Application.props
--rw-rw-rw-   0        0        0     2817 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Configuration.Base.props
--rw-rw-rw-   0        0        0      612 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Configuration.DynamicLibrary.props
--rw-rw-rw-   0        0        0      289 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Configuration.StaticLibrary.props
--rw-rw-rw-   0        0        0     1438 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/ProjectConfigurations.Base.props
--rw-rw-rw-   0        0        0      713 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/build_all.ps1
--rw-rw-rw-   0        0        0     2007 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/config.h
--rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/dpfp.vcxproj
--rw-rw-rw-   0        0        0     1659 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/dpfp_threaded.vcxproj
--rw-rw-rw-   0        0        0     2125 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/fxload.vcxproj
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.691560 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt/
--rw-rw-rw-   0        0        0    31341 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt/getopt.c
--rw-rw-rw-   0        0        0     6627 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt/getopt.h
--rw-rw-rw-   0        0        0     4708 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt/getopt1.c
--rw-rw-rw-   0        0        0     1522 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt.vcxproj
--rw-rw-rw-   0        0        0     1444 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/hotplugtest.vcxproj
--rw-rw-rw-   0        0        0    17271 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/libusb.sln
--rw-rw-rw-   0        0        0     2762 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/libusb_dll.vcxproj
--rw-rw-rw-   0        0        0     2336 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/libusb_static.vcxproj
--rw-rw-rw-   0        0        0     1441 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/listdevs.vcxproj
--rw-rw-rw-   0        0        0     1488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/sam3u_benchmark.vcxproj
--rw-rw-rw-   0        0        0     1579 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/stress.vcxproj
--rw-rw-rw-   0        0        0     1443 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/testlibusb.vcxproj
--rw-rw-rw-   0        0        0     1709 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/msvc/xusb.vcxproj
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.693563 pyjoulescope_driver-1.3.8/third-party/libusb/tests/
--rw-rw-rw-   0        0        0      623 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/tests/Makefile.am
--rw-rw-rw-   0        0        0     2490 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/tests/libusb_testlib.h
--rw-rw-rw-   0        0        0     4935 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/tests/stress.c
--rw-rw-rw-   0        0        0     4919 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/tests/testlib.c
--rw-rw-rw-   0        0        0    37223 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.8/third-party/libusb/tests/umockdev.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:16:28.695563 pyjoulescope_driver-1.3.8/third-party/tinyprintf/
--rw-rw-rw-   0        0        0      122 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/tinyprintf/CMakeLists.txt
--rw-rw-rw-   0        0        0    13188 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/tinyprintf/tinyprintf.c
--rw-rw-rw-   0        0        0     6550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/tinyprintf/tinyprintf.h
--rw-rw-rw-   0        0        0     1554 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.8/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.724287 pyjoulescope_driver-1.3.9/
+-rw-rw-rw-   0        0        0     8233 2023-05-17 14:59:07.000000 pyjoulescope_driver-1.3.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjoulescope_driver-1.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      345 2022-11-19 20:38:00.000000 pyjoulescope_driver-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5170 2023-05-17 18:35:47.724287 pyjoulescope_driver-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3360 2023-01-03 21:53:29.000000 pyjoulescope_driver-1.3.9/README.md
+-rw-rw-rw-   0        0        0     6268 2022-09-20 19:25:49.000000 pyjoulescope_driver-1.3.9/credits.html
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.549505 pyjoulescope_driver-1.3.9/include/
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.554042 pyjoulescope_driver-1.3.9/include/jsdrv/
+-rw-rw-rw-   0        0        0     2698 2022-11-08 21:41:45.000000 pyjoulescope_driver-1.3.9/include/jsdrv/cmacro_inc.h
+-rw-rw-rw-   0        0        0     8332 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.9/include/jsdrv/cstr.h
+-rw-rw-rw-   0        0        0     5878 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.9/include/jsdrv/error_code.h
+-rw-rw-rw-   0        0        0     6817 2023-04-14 18:25:40.000000 pyjoulescope_driver-1.3.9/include/jsdrv/log.h
+-rw-rw-rw-   0        0        0     2002 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include/jsdrv/meta.h
+-rw-rw-rw-   0        0        0    13863 2023-05-16 17:50:16.000000 pyjoulescope_driver-1.3.9/include/jsdrv/time.h
+-rw-rw-rw-   0        0        0     3827 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.9/include/jsdrv/topic.h
+-rw-rw-rw-   0        0        0    12351 2022-08-01 20:41:48.000000 pyjoulescope_driver-1.3.9/include/jsdrv/union.h
+-rw-rw-rw-   0        0        0     4083 2023-05-17 14:42:18.000000 pyjoulescope_driver-1.3.9/include/jsdrv/version.h
+-rw-rw-rw-   0        0        0    29282 2023-04-14 12:30:28.000000 pyjoulescope_driver-1.3.9/include/jsdrv.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.554042 pyjoulescope_driver-1.3.9/include_private/
+-rw-rw-rw-   0        0        0    13394 2022-10-27 14:05:41.000000 pyjoulescope_driver-1.3.9/include_private/js220_api.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.567884 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/
+-rw-rw-rw-   0        0        0     1683 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/assert.h
+-rw-rw-rw-   0        0        0     2116 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/backend.h
+-rw-rw-rw-   0        0        0     2774 2023-04-12 17:01:55.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/buffer.h
+-rw-rw-rw-   0        0        0     3987 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/buffer_signal.h
+-rw-rw-rw-   0        0        0     7138 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/cdef.h
+-rw-rw-rw-   0        0        0     5647 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/dbc.h
+-rw-rw-rw-   0        0        0     1385 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/device.h
+-rw-rw-rw-   0        0        0     1291 2022-07-28 13:15:21.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/devices.h
+-rw-rw-rw-   0        0        0     1633 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/downsample.h
+-rw-rw-rw-   0        0        0     1960 2022-09-19 13:38:02.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/event.h
+-rw-rw-rw-   0        0        0     6987 2023-03-19 15:49:32.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/frontend.h
+-rw-rw-rw-   0        0        0     1408 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js110_cal.h
+-rw-rw-rw-   0        0        0     3046 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js110_sample_processor.h
+-rw-rw-rw-   0        0        0     2858 2022-11-01 15:41:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js110_stats.h
+-rw-rw-rw-   0        0        0     1647 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js220_i128.h
+-rw-rw-rw-   0        0        0     1558 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js220_stats.h
+-rw-rw-rw-   0        0        0     3780 2022-08-01 13:11:32.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/json.h
+-rw-rw-rw-   0        0        0    14035 2022-09-18 11:31:10.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/list.h
+-rw-rw-rw-   0        0        0     8973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/log.h
+-rw-rw-rw-   0        0        0     1650 2022-09-19 12:36:34.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/msg_queue.h
+-rw-rw-rw-   0        0        0     2561 2022-07-28 13:01:35.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/mutex.h
+-rw-rw-rw-   0        0        0     5113 2023-05-16 18:29:34.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/platform.h
+-rw-rw-rw-   0        0        0     4061 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/pubsub.h
+-rw-rw-rw-   0        0        0     2799 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/sample_buffer_f32.h
+-rw-rw-rw-   0        0        0     4561 2023-05-16 18:13:07.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/statistics.h
+-rw-rw-rw-   0        0        0     1979 2023-05-16 18:29:03.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/thread.h
+-rw-rw-rw-   0        0        0     8210 2022-07-29 18:34:03.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/usb_spec.h
+-rw-rw-rw-   0        0        0     1533 2022-10-09 18:53:30.000000 pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/windows.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.574924 pyjoulescope_driver-1.3.9/pyjoulescope_driver/
+-rw-rw-rw-   0        0        0      964 2023-03-29 21:30:50.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-03-29 21:47:21.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/__main__.py
+-rw-rw-rw-   0        0        0  1592784 2023-04-28 17:29:48.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/binding.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.580942 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/
+-rw-rw-rw-   0        0        0     1006 2023-05-10 12:27:33.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-04-14 19:51:53.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/api_timeout.py
+-rw-rw-rw-   0        0        0     1830 2023-01-25 14:57:14.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/gpi.py
+-rw-rw-rw-   0        0        0     6545 2023-05-10 12:33:10.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/info.py
+-rw-rw-rw-   0        0        0     4213 2022-10-30 15:18:19.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/program.py
+-rw-rw-rw-   0        0        0     5031 2023-04-13 12:02:12.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/record.py
+-rw-rw-rw-   0        0        0      932 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/scan.py
+-rw-rw-rw-   0        0        0     2410 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/set_parameter.py
+-rw-rw-rw-   0        0        0     2981 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/statistics.py
+-rw-rw-rw-   0        0        0     3723 2023-04-14 13:21:57.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/threads.py
+-rw-rw-rw-   0        0        0   610304 2023-05-17 18:35:46.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/img_alpha.img
+-rw-rw-rw-   0        0        0   610304 2023-05-17 18:35:46.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/img_beta.img
+-rw-rw-rw-   0        0        0   609280 2023-05-17 18:35:46.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/img_stable.img
+-rw-rw-rw-   0        0        0    10359 2023-04-15 14:37:51.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/program.py
+-rw-rw-rw-   0        0        0     8451 2023-04-28 18:34:52.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/record.py
+-rw-rw-rw-   0        0        0     8980 2022-11-11 19:24:16.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/release.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.582451 pyjoulescope_driver-1.3.9/pyjoulescope_driver/test/
+-rw-rw-rw-   0        0        0        0 2022-10-09 12:38:26.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/test/__init__.py
+-rw-rw-rw-   0        0        0     1901 2022-10-09 17:17:09.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/test/test_release.py
+-rw-rw-rw-   0        0        0     2304 2023-03-29 16:02:01.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/test/test_time64.py
+-rw-rw-rw-   0        0        0     4660 2023-03-29 16:00:59.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/time64.py
+-rw-rw-rw-   0        0        0     1063 2023-05-17 14:42:18.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver/version.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.577440 pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/
+-rw-rw-rw-   0        0        0     5170 2023-05-17 18:35:47.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13694 2023-05-17 18:35:47.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 18:35:47.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-17 18:35:47.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       69 2023-05-17 18:35:47.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-17 18:35:47.000000 pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1076 2023-04-28 13:51:47.000000 pyjoulescope_driver-1.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0      117 2023-05-17 18:35:47.725294 pyjoulescope_driver-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0    10476 2023-05-17 14:40:20.000000 pyjoulescope_driver-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.597020 pyjoulescope_driver-1.3.9/src/
+-rw-rw-rw-   0        0        0     2821 2023-05-16 19:02:12.000000 pyjoulescope_driver-1.3.9/src/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.599025 pyjoulescope_driver-1.3.9/src/backend/
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.600530 pyjoulescope_driver-1.3.9/src/backend/libusb/
+-rw-rw-rw-   0        0        0    30330 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.9/src/backend/libusb/backend.c
+-rw-rw-rw-   0        0        0     4580 2022-09-19 12:40:12.000000 pyjoulescope_driver-1.3.9/src/backend/libusb/msg_queue.c
+-rw-rw-rw-   0        0        0     5503 2023-04-14 20:55:21.000000 pyjoulescope_driver-1.3.9/src/backend/posix.c
+-rw-rw-rw-   0        0        0     6886 2023-04-14 20:54:20.000000 pyjoulescope_driver-1.3.9/src/backend/windows.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.601535 pyjoulescope_driver-1.3.9/src/backend/winusb/
+-rw-rw-rw-   0        0        0    38641 2023-04-04 15:07:16.000000 pyjoulescope_driver-1.3.9/src/backend/winusb/backend.c
+-rw-rw-rw-   0        0        0     7713 2022-09-18 12:51:07.000000 pyjoulescope_driver-1.3.9/src/backend/winusb/device_change_notifier.c
+-rw-rw-rw-   0        0        0     2798 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/src/backend/winusb/device_change_notifier.h
+-rw-rw-rw-   0        0        0     4807 2023-03-19 16:29:53.000000 pyjoulescope_driver-1.3.9/src/backend/winusb/msg_queue.c
+-rw-rw-rw-   0        0        0    25694 2023-04-21 20:34:16.000000 pyjoulescope_driver-1.3.9/src/buffer.c
+-rw-rw-rw-   0        0        0    32686 2023-04-28 18:46:11.000000 pyjoulescope_driver-1.3.9/src/buffer_signal.c
+-rw-rw-rw-   0        0        0    11771 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/src/cstr.c
+-rw-rw-rw-   0        0        0     1671 2022-09-19 11:52:36.000000 pyjoulescope_driver-1.3.9/src/devices.c
+-rw-rw-rw-   0        0        0     8709 2022-10-24 15:34:41.000000 pyjoulescope_driver-1.3.9/src/downsample.c
+-rw-rw-rw-   0        0        0     5925 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.9/src/emu.c
+-rw-rw-rw-   0        0        0     4649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/src/emulated.c
+-rw-rw-rw-   0        0        0     4817 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.9/src/error_code.c
+-rw-rw-rw-   0        0        0     9335 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/src/js110_api.h
+-rw-rw-rw-   0        0        0     3972 2022-09-18 11:26:57.000000 pyjoulescope_driver-1.3.9/src/js110_cal.c
+-rw-rw-rw-   0        0        0     9038 2022-11-01 14:07:47.000000 pyjoulescope_driver-1.3.9/src/js110_sample_processor.c
+-rw-rw-rw-   0        0        0     4551 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.9/src/js110_stats.c
+-rw-rw-rw-   0        0        0    52738 2023-04-27 16:54:44.000000 pyjoulescope_driver-1.3.9/src/js110_usb.c
+-rw-rw-rw-   0        0        0     5162 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.9/src/js220_i128.c
+-rw-rw-rw-   0        0        0     1188 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.9/src/js220_params.c
+-rw-rw-rw-   0        0        0     2893 2022-10-05 01:35:24.000000 pyjoulescope_driver-1.3.9/src/js220_stats.c
+-rw-rw-rw-   0        0        0    62976 2023-04-20 12:52:32.000000 pyjoulescope_driver-1.3.9/src/js220_usb.c
+-rw-rw-rw-   0        0        0    37782 2023-04-14 12:55:05.000000 pyjoulescope_driver-1.3.9/src/jsdrv.c
+-rw-rw-rw-   0        0        0    10974 2022-08-01 18:37:59.000000 pyjoulescope_driver-1.3.9/src/json.c
+-rw-rw-rw-   0        0        0    16499 2023-04-14 20:57:15.000000 pyjoulescope_driver-1.3.9/src/log.c
+-rw-rw-rw-   0        0        0    10627 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.9/src/meta.c
+-rw-rw-rw-   0        0        0    24211 2023-03-19 15:32:24.000000 pyjoulescope_driver-1.3.9/src/pubsub.c
+-rw-rw-rw-   0        0        0     4944 2022-10-07 12:24:15.000000 pyjoulescope_driver-1.3.9/src/sample_buffer_f32.c
+-rw-rw-rw-   0        0        0     5262 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.9/src/statistics.c
+-rw-rw-rw-   0        0        0     2814 2023-03-09 19:53:59.000000 pyjoulescope_driver-1.3.9/src/time.c
+-rw-rw-rw-   0        0        0     3763 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.9/src/topic.c
+-rw-rw-rw-   0        0        0    12780 2022-09-18 11:32:07.000000 pyjoulescope_driver-1.3.9/src/union.c
+-rw-rw-rw-   0        0        0     1001 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/src/version.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.602541 pyjoulescope_driver-1.3.9/third-party/
+-rw-rw-rw-   0        0        0      810 2022-09-20 18:21:09.000000 pyjoulescope_driver-1.3.9/third-party/CMakeLists.txt
+-rw-rw-rw-   0        0        0      364 2022-08-01 20:40:07.000000 pyjoulescope_driver-1.3.9/third-party/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.610580 pyjoulescope_driver-1.3.9/third-party/cmocka/
+-rw-rw-rw-   0        0        0       18 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/.clang_complete
+-rw-rw-rw-   0        0        0     9611 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     3508 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/.ycm_extra_conf.py
+-rw-rw-rw-   0        0        0     1209 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/5.patch
+-rw-rw-rw-   0        0        0     3601 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1845 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/CPackConfig.cmake
+-rw-rw-rw-   0        0        0      284 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/CTestConfig.cmake
+-rw-rw-rw-   0        0        0     5331 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/CompilerChecks.cmake
+-rw-rw-rw-   0        0        0     4648 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/ConfigureChecks.cmake
+-rw-rw-rw-   0        0        0      431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/DefineOptions.cmake
+-rw-rw-rw-   0        0        0     3217 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/INSTALL.md
+-rw-rw-rw-   0        0        0      658 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.611586 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.614599 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/
+-rw-rw-rw-   0        0        0      866 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
+-rw-rw-rw-   0        0        0     3360 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
+-rw-rw-rw-   0        0        0     1952 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
+-rw-rw-rw-   0        0        0      811 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
+-rw-rw-rw-   0        0        0     3973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
+-rw-rw-rw-   0        0        0      585 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
+-rw-rw-rw-   0        0        0     1480 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/FindNSIS.cmake
+-rw-rw-rw-   0        0        0      680 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
+-rw-rw-rw-   0        0        0      656 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
+-rw-rw-rw-   0        0        0     1145 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
+-rw-rw-rw-   0        0        0       53 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmocka-build-tree-settings.cmake.in
+-rw-rw-rw-   0        0        0      507 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmocka-config.cmake.in
+-rw-rw-rw-   0        0        0      189 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/cmocka.pc.cmake
+-rw-rw-rw-   0        0        0     5161 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/config.h.cmake
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.615608 pyjoulescope_driver-1.3.9/third-party/cmocka/coverity/
+-rw-rw-rw-   0        0        0     3918 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/coverity/coverity_assert_model.c
+-rw-rw-rw-   0        0        0      142 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/coverity/coverity_internal_model.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.617114 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/
+-rw-rw-rw-   0        0        0     2206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/CMakeLists.txt
+-rw-rw-rw-   0        0        0    26974 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/index.html
+-rw-rw-rw-   0        0        0     5291 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/mainpage.dox
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.619120 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/
+-rw-rw-rw-   0        0        0     1301 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/README.md
+-rw-rw-rw-   0        0        0     2121 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/header.html
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.623644 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/
+-rw-rw-rw-   0        0        0     6714 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/doc.svg
+-rw-rw-rw-   0        0        0     3604 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/folderclosed.svg
+-rw-rw-rw-   0        0        0     4299 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/folderopen.svg
+-rw-rw-rw-   0        0        0     3955 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/mag_glass.svg
+-rw-rw-rw-   0        0        0     3988 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
+-rw-rw-rw-   0        0        0     3249 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
+-rw-rw-rw-   0        0        0     3262 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
+-rw-rw-rw-   0        0        0     7409 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
+-rw-rw-rw-   0        0        0      483 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/sync_off.png
+-rw-rw-rw-   0        0        0      488 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/sync_on.png
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.623644 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/js/
+-rw-rw-rw-   0        0        0      977 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/js/striped_bg.js
+-rw-rw-rw-   0        0        0    32455 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/that_style.css
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.630684 pyjoulescope_driver-1.3.9/third-party/cmocka/example/
+-rw-rw-rw-   0        0        0     2562 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1755 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/allocate_module.c
+-rw-rw-rw-   0        0        0     1640 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/allocate_module_test.c
+-rw-rw-rw-   0        0        0     1254 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_macro.c
+-rw-rw-rw-   0        0        0      144 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_macro.h
+-rw-rw-rw-   0        0        0     1649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_macro_test.c
+-rw-rw-rw-   0        0        0     1216 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_module.c
+-rw-rw-rw-   0        0        0      692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_module.h
+-rw-rw-rw-   0        0        0     1692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_module_test.c
+-rw-rw-rw-   0        0        0     9746 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/calculator.c
+-rw-rw-rw-   0        0        0    16244 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/calculator_test.c
+-rw-rw-rw-   0        0        0     1439 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/database.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.630684 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/
+-rw-rw-rw-   0        0        0      197 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.633787 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/
+-rw-rw-rw-   0        0        0      620 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/chef.c
+-rw-rw-rw-   0        0        0      789 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/chef.h
+-rw-rw-rw-   0        0        0     5222 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
+-rw-rw-rw-   0        0        0       61 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.636935 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/
+-rw-rw-rw-   0        0        0      685 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/CMakeLists.txt
+-rw-rw-rw-   0        0        0     2033 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/README.md
+-rw-rw-rw-   0        0        0     1882 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/proc_uptime.c
+-rw-rw-rw-   0        0        0      793 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/proc_uptime.h
+-rw-rw-rw-   0        0        0     5237 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/test_uptime.c
+-rw-rw-rw-   0        0        0     3305 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/uptime.c
+-rw-rw-rw-   0        0        0      415 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/example/simple_test.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.638605 pyjoulescope_driver-1.3.9/third-party/cmocka/include/
+-rw-rw-rw-   0        0        0      465 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/include/CMakeLists.txt
+-rw-rw-rw-   0        0        0    77952 2022-08-01 20:01:08.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmocka.h
+-rw-rw-rw-   0        0        0     1893 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmocka_pbc.h
+-rw-rw-rw-   0        0        0     4137 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmocka_private.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.639603 pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmockery/
+-rw-rw-rw-   0        0        0       21 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmockery/cmockery.h
+-rw-rw-rw-   0        0        0       25 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmockery/pbc.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.641108 pyjoulescope_driver-1.3.9/third-party/cmocka/src/
+-rw-rw-rw-   0        0        0     3668 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/src/CMakeLists.txt
+-rw-rw-rw-   0        0        0   119941 2022-09-18 17:05:56.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/src/cmocka.c
+-rw-rw-rw-   0        0        0     1174 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/src/cmocka.def
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.655416 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/
+-rw-rw-rw-   0        0        0     7657 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0     6215 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/cmocka_test.cmake
+-rw-rw-rw-   0        0        0     2758 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/ctest-default.cmake
+-rw-rw-rw-   0        0        0     1922 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_alloc.c
+-rw-rw-rw-   0        0        0      818 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_assert_macros.c
+-rw-rw-rw-   0        0        0      862 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_assert_macros_fail.c
+-rw-rw-rw-   0        0        0     1550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_basics.c
+-rw-rw-rw-   0        0        0      970 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_cmockery.c
+-rw-rw-rw-   0        0        0      869 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_exception_handler.c
+-rw-rw-rw-   0        0        0     1774 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_fixtures.c
+-rw-rw-rw-   0        0        0     1206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_float_macros.c
+-rw-rw-rw-   0        0        0      992 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_group_fixtures.c
+-rw-rw-rw-   0        0        0      699 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_group_setup_assert.c
+-rw-rw-rw-   0        0        0      696 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_group_setup_fail.c
+-rw-rw-rw-   0        0        0     1757 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_groups.c
+-rw-rw-rw-   0        0        0     2767 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_ordering.c
+-rw-rw-rw-   0        0        0     2420 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_ordering_fail.c
+-rw-rw-rw-   0        0        0     1577 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_returns.c
+-rw-rw-rw-   0        0        0     1704 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_returns_fail.c
+-rw-rw-rw-   0        0        0     1092 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_setup_fail.c
+-rw-rw-rw-   0        0        0     1043 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_skip.c
+-rw-rw-rw-   0        0        0     1362 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_skip_filter.c
+-rw-rw-rw-   0        0        0     2280 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_strmatch.c
+-rw-rw-rw-   0        0        0     1260 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_wildcard.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.662958 pyjoulescope_driver-1.3.9/third-party/libusb/
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.663467 pyjoulescope_driver-1.3.9/third-party/libusb/.github/
+-rw-rw-rw-   0        0        0      719 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.github/cifuzz.yml
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.664470 pyjoulescope_driver-1.3.9/third-party/libusb/.github/workflows/
+-rw-rw-rw-   0        0        0     1188 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.github/workflows/linux.yml
+-rw-rw-rw-   0        0        0     1023 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0      527 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.github/workflows/msys2.yml
+-rw-rw-rw-   0        0        0      827 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.668995 pyjoulescope_driver-1.3.9/third-party/libusb/.private/
+-rw-rw-rw-   0        0        0      202 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/README.txt
+-rw-rw-rw-   0        0        0      548 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/appveyor_build.sh
+-rw-rw-rw-   0        0        0     1424 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/bm.sh
+-rw-rw-rw-   0        0        0     1109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/ci-build.sh
+-rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/ci-container-build.sh
+-rw-rw-rw-   0        0        0      959 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/post-rewrite.sh
+-rw-rw-rw-   0        0        0     1995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/pre-commit.sh
+-rw-rw-rw-   0        0        0     2545 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.private/wbs.txt
+-rw-rw-rw-   0        0        0     1465 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/.travis.yml
+-rw-rw-rw-   0        0        0     2523 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.9/third-party/libusb/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1972 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/INSTALL_WIN.txt
+-rw-rw-rw-   0        0        0     1495 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Makefile.am
+-rw-rw-rw-   0        0        0     1395 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/README-FORK.md
+-rw-rw-rw-   0        0        0     1894 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/README.git
+-rw-rw-rw-   0        0        0        6 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.672504 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/
+-rw-rw-rw-   0        0        0     2409 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/common.xcconfig
+-rw-rw-rw-   0        0        0      995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/config.h
+-rw-rw-rw-   0        0        0     1135 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/debug.xcconfig
+-rw-rw-rw-   0        0        0      988 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb.xcconfig
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.673009 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb.xcodeproj/
+-rw-rw-rw-   0        0        0    62286 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
+-rw-rw-rw-   0        0        0      963 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb_debug.xcconfig
+-rw-rw-rw-   0        0        0      965 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb_release.xcconfig
+-rw-rw-rw-   0        0        0     1208 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/release.xcconfig
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.673513 pyjoulescope_driver-1.3.9/third-party/libusb/android/
+-rw-rw-rw-   0        0        0     2016 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/config.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.674518 pyjoulescope_driver-1.3.9/third-party/libusb/android/examples/
+-rw-rw-rw-   0        0        0    11355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/examples/unrooted_android.c
+-rw-rw-rw-   0        0        0     1156 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/examples/unrooted_android.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.677137 pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/
+-rw-rw-rw-   0        0        0      997 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/Android.mk
+-rw-rw-rw-   0        0        0     1370 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/Application.mk
+-rw-rw-rw-   0        0        0     3425 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/examples.mk
+-rw-rw-rw-   0        0        0     2056 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/libusb.mk
+-rw-rw-rw-   0        0        0     1355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/tests.mk
+-rw-rw-rw-   0        0        0     3820 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/appveyor.yml
+-rw-rw-rw-   0        0        0      191 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/autogen.sh
+-rw-rw-rw-   0        0        0      109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/bootstrap.sh
+-rw-rw-rw-   0        0        0    16514 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/configure.ac
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.678316 pyjoulescope_driver-1.3.9/third-party/libusb/doc/
+-rw-rw-rw-   0        0        0      685 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/doc/Makefile.in
+-rw-rw-rw-   0        0        0   115647 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/doc/doxygen.cfg.in
+-rw-rw-rw-   0        0        0     2923 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/doc/libusb.png
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.683034 pyjoulescope_driver-1.3.9/third-party/libusb/examples/
+-rw-rw-rw-   0        0        0      416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/Makefile.am
+-rw-rw-rw-   0        0        0    15812 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/dpfp.c
+-rw-rw-rw-   0        0        0    24573 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/ezusb.c
+-rw-rw-rw-   0        0        0     4247 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/ezusb.h
+-rw-rw-rw-   0        0        0     9593 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/fxload.c
+-rw-rw-rw-   0        0        0     3580 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/hotplugtest.c
+-rw-rw-rw-   0        0        0     2081 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/listdevs.c
+-rw-rw-rw-   0        0        0     6149 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/sam3u_benchmark.c
+-rw-rw-rw-   0        0        0     9765 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/testlibusb.c
+-rw-rw-rw-   0        0        0    40008 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/examples/xusb.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.544995 pyjoulescope_driver-1.3.9/third-party/libusb/include/
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.683610 pyjoulescope_driver-1.3.9/third-party/libusb/include/linux/
+-rw-rw-rw-   0        0        0     5104 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.9/third-party/libusb/include/linux/config.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.683610 pyjoulescope_driver-1.3.9/third-party/libusb/include/macos/
+-rw-rw-rw-   0        0        0     5130 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/include/macos/config.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.690640 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/
+-rw-rw-rw-   0        0        0     2539 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/Makefile.am
+-rw-rw-rw-   0        0        0      780 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/Makefile.am.extra
+-rw-rw-rw-   0        0        0    99186 2022-09-20 23:33:57.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/core.c
+-rw-rw-rw-   0        0        0    37583 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/descriptor.c
+-rw-rw-rw-   0        0        0    15552 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/hotplug.c
+-rw-rw-rw-   0        0        0   113897 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/io.c
+-rw-rw-rw-   0        0        0     8221 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusb-1.0.def
+-rw-rw-rw-   0        0        0     1642 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusb-1.0.rc
+-rw-rw-rw-   0        0        0    78746 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusb.h
+-rw-rw-rw-   0        0        0    53532 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusbi.h
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.707183 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/
+-rw-rw-rw-   0        0        0   103226 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/darwin_usb.c
+-rw-rw-rw-   0        0        0     7071 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/darwin_usb.h
+-rw-rw-rw-   0        0        0    24325 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/emscripten_webusb.cpp
+-rw-rw-rw-   0        0        0     9581 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_posix.c
+-rw-rw-rw-   0        0        0     1776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_posix.h
+-rw-rw-rw-   0        0        0     6948 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_windows.c
+-rw-rw-rw-   0        0        0     1520 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_windows.h
+-rw-rw-rw-   0        0        0     7884 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_pollfs.cpp
+-rw-rw-rw-   0        0        0     3386 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb.h
+-rw-rw-rw-   0        0        0    16687 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb_backend.cpp
+-rw-rw-rw-   0        0        0     7477 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb_raw.cpp
+-rw-rw-rw-   0        0        0     4080 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb_raw.h
+-rw-rw-rw-   0        0        0    10778 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_netlink.c
+-rw-rw-rw-   0        0        0     8864 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_udev.c
+-rw-rw-rw-   0        0        0    83335 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_usbfs.c
+-rw-rw-rw-   0        0        0     6551 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_usbfs.h
+-rw-rw-rw-   0        0        0    16279 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/netbsd_usb.c
+-rw-rw-rw-   0        0        0     2996 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/null_usb.c
+-rw-rw-rw-   0        0        0    18179 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/openbsd_usb.c
+-rw-rw-rw-   0        0        0    45204 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/sunos_usb.c
+-rw-rw-rw-   0        0        0     2254 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/sunos_usb.h
+-rw-rw-rw-   0        0        0     3488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_posix.c
+-rw-rw-rw-   0        0        0     3052 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_posix.h
+-rw-rw-rw-   0        0        0     1416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_windows.c
+-rw-rw-rw-   0        0        0     3280 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_windows.h
+-rw-rw-rw-   0        0        0    30524 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_common.c
+-rw-rw-rw-   0        0        0    14347 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_common.h
+-rw-rw-rw-   0        0        0    24491 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_usbdk.c
+-rw-rw-rw-   0        0        0     2926 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_usbdk.h
+-rw-rw-rw-   0        0        0   171316 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_winusb.c
+-rw-rw-rw-   0        0        0    24670 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_winusb.h
+-rw-rw-rw-   0        0        0     8776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/strerror.c
+-rw-rw-rw-   0        0        0    13160 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/sync.c
+-rw-rw-rw-   0        0        0      449 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/version.h
+-rw-rw-rw-   0        0        0       27 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb/version_nano.h
+-rw-rw-rw-   0        0        0      323 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/libusb-1.0.pc.in
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.718740 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/
+-rw-rw-rw-   0        0        0      136 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/.gitattributes
+-rw-rw-rw-   0        0        0     2982 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Base.props
+-rw-rw-rw-   0        0        0      287 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Configuration.Application.props
+-rw-rw-rw-   0        0        0     2817 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Configuration.Base.props
+-rw-rw-rw-   0        0        0      612 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Configuration.DynamicLibrary.props
+-rw-rw-rw-   0        0        0      289 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Configuration.StaticLibrary.props
+-rw-rw-rw-   0        0        0     1438 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/ProjectConfigurations.Base.props
+-rw-rw-rw-   0        0        0      713 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/build_all.ps1
+-rw-rw-rw-   0        0        0     2007 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/config.h
+-rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/dpfp.vcxproj
+-rw-rw-rw-   0        0        0     1659 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/dpfp_threaded.vcxproj
+-rw-rw-rw-   0        0        0     2125 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/fxload.vcxproj
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.720253 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt/
+-rw-rw-rw-   0        0        0    31341 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt/getopt.c
+-rw-rw-rw-   0        0        0     6627 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt/getopt.h
+-rw-rw-rw-   0        0        0     4708 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt/getopt1.c
+-rw-rw-rw-   0        0        0     1522 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt.vcxproj
+-rw-rw-rw-   0        0        0     1444 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/hotplugtest.vcxproj
+-rw-rw-rw-   0        0        0    17271 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/libusb.sln
+-rw-rw-rw-   0        0        0     2762 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/libusb_dll.vcxproj
+-rw-rw-rw-   0        0        0     2336 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/libusb_static.vcxproj
+-rw-rw-rw-   0        0        0     1441 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/listdevs.vcxproj
+-rw-rw-rw-   0        0        0     1488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/sam3u_benchmark.vcxproj
+-rw-rw-rw-   0        0        0     1579 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/stress.vcxproj
+-rw-rw-rw-   0        0        0     1443 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/testlibusb.vcxproj
+-rw-rw-rw-   0        0        0     1709 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/msvc/xusb.vcxproj
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.722758 pyjoulescope_driver-1.3.9/third-party/libusb/tests/
+-rw-rw-rw-   0        0        0      623 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/tests/Makefile.am
+-rw-rw-rw-   0        0        0     2490 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/tests/libusb_testlib.h
+-rw-rw-rw-   0        0        0     4935 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/tests/stress.c
+-rw-rw-rw-   0        0        0     4919 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/tests/testlib.c
+-rw-rw-rw-   0        0        0    37223 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.9/third-party/libusb/tests/umockdev.c
+drwxrwxrwx   0        0        0        0 2023-05-17 18:35:47.724287 pyjoulescope_driver-1.3.9/third-party/tinyprintf/
+-rw-rw-rw-   0        0        0      122 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/tinyprintf/CMakeLists.txt
+-rw-rw-rw-   0        0        0    13188 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/tinyprintf/tinyprintf.c
+-rw-rw-rw-   0        0        0     6550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/tinyprintf/tinyprintf.h
+-rw-rw-rw-   0        0        0     1554 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.9/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
```

### Comparing `pyjoulescope_driver-1.3.8/CHANGELOG.md` & `pyjoulescope_driver-1.3.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the Joulescope driver.
 
 
+## 1.3.9
+
+2023 May 17
+
+* Fixed installation on Ubuntu #6.
+
+
 ## 1.3.8
 
 2023 May 16
 
 * Updated info entry point.
 * Added automatic include path for jsdrv static CMake builds.
 * Added support for building a shared library.
```

### Comparing `pyjoulescope_driver-1.3.8/LICENSE.txt` & `pyjoulescope_driver-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/PKG-INFO` & `pyjoulescope_driver-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope_driver
-Version: 1.3.8
+Version: 1.3.9
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.3.8/README.md` & `pyjoulescope_driver-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/credits.html` & `pyjoulescope_driver-1.3.9/credits.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/cmacro_inc.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/cmacro_inc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/cstr.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/cstr.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/error_code.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/error_code.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/log.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/log.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/meta.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/meta.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/time.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/time.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/topic.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/topic.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/union.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/union.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv/version.h` & `pyjoulescope_driver-1.3.9/include/jsdrv/version.h`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 #define JSDRV_VERSION_MINOR 3
 
 /**
  * @brief The Joulescope driver patch version.
  *
  * Changes in the patch version indicate bug fixes and improvements.
  */
-#define JSDRV_VERSION_PATCH 8
+#define JSDRV_VERSION_PATCH 9
 
 /**
  * \brief The maximum version string length.
  *
  * The actual length is 14 bytes (MMM.mmm.ppppp\\x00), but round up
  * to simplify packing.
  */
```

### Comparing `pyjoulescope_driver-1.3.8/include/jsdrv.h` & `pyjoulescope_driver-1.3.9/include/jsdrv.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/js220_api.h` & `pyjoulescope_driver-1.3.9/include_private/js220_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/assert.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/assert.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/backend.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/backend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/buffer.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/buffer.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/buffer_signal.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/buffer_signal.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/cdef.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/dbc.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/dbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/device.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/device.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/devices.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/devices.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/downsample.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/downsample.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/event.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/event.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/frontend.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/frontend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js110_cal.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js110_cal.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js110_sample_processor.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js110_sample_processor.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js110_stats.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js110_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js220_i128.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js220_i128.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/js220_stats.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/js220_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/json.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/json.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/list.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/list.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/log.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/log.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/msg_queue.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/msg_queue.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/mutex.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/mutex.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/platform.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/platform.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/pubsub.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/pubsub.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/sample_buffer_f32.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/sample_buffer_f32.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/statistics.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/thread.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/thread.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/usb_spec.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/usb_spec.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/include_private/jsdrv_prv/windows.h` & `pyjoulescope_driver-1.3.9/include_private/jsdrv_prv/windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/__init__.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/__main__.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/binding.c` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/binding.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/__init__.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/api_timeout.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/api_timeout.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/gpi.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/gpi.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/info.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/program.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/record.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/record.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/scan.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/set_parameter.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/set_parameter.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/statistics.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/entry_points/threads.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/entry_points/threads.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/img_alpha.img` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/img_alpha.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/img_beta.img` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/img_beta.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/img_stable.img` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/img_stable.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/program.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/record.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/record.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/release.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/test/test_release.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/test/test_release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/test/test_time64.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/test/test_time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/time64.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver/version.py` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 
 __title__ = "pyjoulescope_driver"
 __description__ = 'Joulescope™ driver'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/PKG-INFO` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope-driver
-Version: 1.3.8
+Version: 1.3.9
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.3.8/pyjoulescope_driver.egg-info/SOURCES.txt` & `pyjoulescope_driver-1.3.9/pyjoulescope_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/pyproject.toml` & `pyjoulescope_driver-1.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/setup.py` & `pyjoulescope_driver-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 from setuptools import Command
 from setuptools.errors import ExecError
 from setuptools.command.build_py import build_py
 import numpy as np
 import os
 import platform
 os.environ['pyjoulescope_driver_setup'] = '1'
-from pyjoulescope_driver.release import releases_get_from_network
+
+try:
+    from pyjoulescope_driver.release import releases_get_from_network
+except ImportError:
+    releases_get_from_network = None
 
 
 MYPATH = os.path.dirname(os.path.abspath(__file__))
 VERSION_PATH = os.path.join(MYPATH, 'pyjoulescope_driver', 'version.py')
 C_INCS = [
     os.path.join(MYPATH, 'include'),
     os.path.join(MYPATH, 'include_private'),
@@ -169,15 +173,16 @@
     long_description = f.read()
 
 
 class BuildPyCommand(build_py):
     """Custom build command."""
 
     def run(self):
-        releases_get_from_network(force_download=True, dist_save=True)
+        if callable(releases_get_from_network):
+            releases_get_from_network(force_download=True, dist_save=True)
         build_py.run(self)
 
 
 class CustomBuildDocs(Command):
     """Custom command to build docs locally."""
 
     description = 'Build docs.'
```

### Comparing `pyjoulescope_driver-1.3.8/src/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/libusb/backend.c` & `pyjoulescope_driver-1.3.9/src/backend/libusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/libusb/msg_queue.c` & `pyjoulescope_driver-1.3.9/src/backend/libusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/posix.c` & `pyjoulescope_driver-1.3.9/src/backend/posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/windows.c` & `pyjoulescope_driver-1.3.9/src/backend/windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/winusb/backend.c` & `pyjoulescope_driver-1.3.9/src/backend/winusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/winusb/device_change_notifier.c` & `pyjoulescope_driver-1.3.9/src/backend/winusb/device_change_notifier.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/winusb/device_change_notifier.h` & `pyjoulescope_driver-1.3.9/src/backend/winusb/device_change_notifier.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/backend/winusb/msg_queue.c` & `pyjoulescope_driver-1.3.9/src/backend/winusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/buffer.c` & `pyjoulescope_driver-1.3.9/src/buffer.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/buffer_signal.c` & `pyjoulescope_driver-1.3.9/src/buffer_signal.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/cstr.c` & `pyjoulescope_driver-1.3.9/src/cstr.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/devices.c` & `pyjoulescope_driver-1.3.9/src/devices.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/downsample.c` & `pyjoulescope_driver-1.3.9/src/downsample.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/emu.c` & `pyjoulescope_driver-1.3.9/src/emu.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/emulated.c` & `pyjoulescope_driver-1.3.9/src/emulated.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/error_code.c` & `pyjoulescope_driver-1.3.9/src/error_code.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js110_api.h` & `pyjoulescope_driver-1.3.9/src/js110_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js110_cal.c` & `pyjoulescope_driver-1.3.9/src/js110_cal.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js110_sample_processor.c` & `pyjoulescope_driver-1.3.9/src/js110_sample_processor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js110_stats.c` & `pyjoulescope_driver-1.3.9/src/js110_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js110_usb.c` & `pyjoulescope_driver-1.3.9/src/js110_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js220_i128.c` & `pyjoulescope_driver-1.3.9/src/js220_i128.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js220_params.c` & `pyjoulescope_driver-1.3.9/src/js220_params.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js220_stats.c` & `pyjoulescope_driver-1.3.9/src/js220_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/js220_usb.c` & `pyjoulescope_driver-1.3.9/src/js220_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/jsdrv.c` & `pyjoulescope_driver-1.3.9/src/jsdrv.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/json.c` & `pyjoulescope_driver-1.3.9/src/json.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/log.c` & `pyjoulescope_driver-1.3.9/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/meta.c` & `pyjoulescope_driver-1.3.9/src/meta.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/pubsub.c` & `pyjoulescope_driver-1.3.9/src/pubsub.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/sample_buffer_f32.c` & `pyjoulescope_driver-1.3.9/src/sample_buffer_f32.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/statistics.c` & `pyjoulescope_driver-1.3.9/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/time.c` & `pyjoulescope_driver-1.3.9/src/time.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/topic.c` & `pyjoulescope_driver-1.3.9/src/topic.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/union.c` & `pyjoulescope_driver-1.3.9/src/union.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/src/version.c` & `pyjoulescope_driver-1.3.9/src/version.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/.gitlab-ci.yml` & `pyjoulescope_driver-1.3.9/third-party/cmocka/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/.ycm_extra_conf.py` & `pyjoulescope_driver-1.3.9/third-party/cmocka/.ycm_extra_conf.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/5.patch` & `pyjoulescope_driver-1.3.9/third-party/cmocka/5.patch`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/cmocka/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/CPackConfig.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/CPackConfig.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/CompilerChecks.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/CompilerChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/ConfigureChecks.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/ConfigureChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/INSTALL.md` & `pyjoulescope_driver-1.3.9/third-party/cmocka/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/README.md` & `pyjoulescope_driver-1.3.9/third-party/cmocka/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/FindNSIS.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/FindNSIS.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/cmake/Toolchain-cross-m32.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/cmake/Toolchain-cross-m32.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/config.h.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/coverity/coverity_assert_model.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/coverity/coverity_assert_model.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/index.html` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/mainpage.dox` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/mainpage.dox`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/README.md` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/header.html` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/header.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/doc.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/doc.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/folderclosed.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/folderclosed.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/folderopen.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/folderopen.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/mag_glass.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/mag_glass.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/nav_edge_left.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/nav_edge_left.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/nav_edge_right.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/nav_edge_right.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/img/splitbar_handle.svg` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/img/splitbar_handle.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/js/striped_bg.js` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/js/striped_bg.js`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/doc/that_style/that_style.css` & `pyjoulescope_driver-1.3.9/third-party/cmocka/doc/that_style/that_style.css`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/allocate_module.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/allocate_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/allocate_module_test.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/allocate_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_macro.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_macro.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_macro_test.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_macro_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_module.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_module.h` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_module.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/assert_module_test.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/assert_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/calculator.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/calculator.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/calculator_test.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/calculator_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/database.h` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/database.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/chef.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/chef.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/chef.h` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/chef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/README.md` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/proc_uptime.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/proc_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/proc_uptime.h` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/proc_uptime.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/test_uptime.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/test_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/example/mock/uptime/uptime.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/example/mock/uptime/uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmocka.h` & `pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmocka.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmocka_pbc.h` & `pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmocka_pbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/include/cmocka_private.h` & `pyjoulescope_driver-1.3.9/third-party/cmocka/include/cmocka_private.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/src/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/cmocka/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/src/cmocka.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/src/cmocka.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/src/cmocka.def` & `pyjoulescope_driver-1.3.9/third-party/cmocka/src/cmocka.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/cmocka_test.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/cmocka_test.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/ctest-default.cmake` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/ctest-default.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_alloc.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_alloc.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_assert_macros.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_assert_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_assert_macros_fail.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_assert_macros_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_basics.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_basics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_cmockery.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_cmockery.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_exception_handler.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_exception_handler.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_fixtures.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_float_macros.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_float_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_group_fixtures.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_group_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_group_setup_assert.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_group_setup_assert.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_group_setup_fail.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_group_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_groups.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_groups.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_ordering.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_ordering.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_ordering_fail.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_ordering_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_returns.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_returns.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_returns_fail.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_returns_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_setup_fail.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_skip.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_skip.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_skip_filter.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_skip_filter.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_strmatch.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_strmatch.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/cmocka/tests/test_wildcard.c` & `pyjoulescope_driver-1.3.9/third-party/cmocka/tests/test_wildcard.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.github/cifuzz.yml` & `pyjoulescope_driver-1.3.9/third-party/libusb/.github/cifuzz.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.github/workflows/linux.yml` & `pyjoulescope_driver-1.3.9/third-party/libusb/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.github/workflows/macos.yml` & `pyjoulescope_driver-1.3.9/third-party/libusb/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.github/workflows/msys2.yml` & `pyjoulescope_driver-1.3.9/third-party/libusb/.github/workflows/msys2.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.gitignore` & `pyjoulescope_driver-1.3.9/third-party/libusb/.gitignore`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.private/appveyor_build.sh` & `pyjoulescope_driver-1.3.9/third-party/libusb/.private/appveyor_build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.private/bm.sh` & `pyjoulescope_driver-1.3.9/third-party/libusb/.private/bm.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.private/ci-build.sh` & `pyjoulescope_driver-1.3.9/third-party/libusb/.private/ci-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.private/ci-container-build.sh` & `pyjoulescope_driver-1.3.9/third-party/libusb/.private/ci-container-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.private/post-rewrite.sh` & `pyjoulescope_driver-1.3.9/third-party/libusb/.private/post-rewrite.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.private/pre-commit.sh` & `pyjoulescope_driver-1.3.9/third-party/libusb/.private/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.private/wbs.txt` & `pyjoulescope_driver-1.3.9/third-party/libusb/.private/wbs.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/.travis.yml` & `pyjoulescope_driver-1.3.9/third-party/libusb/.travis.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/CMakeLists.txt` & `pyjoulescope_driver-1.3.9/third-party/libusb/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/INSTALL_WIN.txt` & `pyjoulescope_driver-1.3.9/third-party/libusb/INSTALL_WIN.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Makefile.am` & `pyjoulescope_driver-1.3.9/third-party/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/README-FORK.md` & `pyjoulescope_driver-1.3.9/third-party/libusb/README-FORK.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/README.git` & `pyjoulescope_driver-1.3.9/third-party/libusb/README.git`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/common.xcconfig` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/common.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/config.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/debug.xcconfig` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb.xcconfig` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb_debug.xcconfig` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb_debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/libusb_release.xcconfig` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/libusb_release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/Xcode/release.xcconfig` & `pyjoulescope_driver-1.3.9/third-party/libusb/Xcode/release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/config.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/examples/unrooted_android.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/examples/unrooted_android.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/examples/unrooted_android.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/examples/unrooted_android.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/Android.mk` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/Android.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/Application.mk` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/Application.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/examples.mk` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/examples.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/libusb.mk` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/libusb.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/android/jni/tests.mk` & `pyjoulescope_driver-1.3.9/third-party/libusb/android/jni/tests.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/appveyor.yml` & `pyjoulescope_driver-1.3.9/third-party/libusb/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/configure.ac` & `pyjoulescope_driver-1.3.9/third-party/libusb/configure.ac`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/doc/Makefile.in` & `pyjoulescope_driver-1.3.9/third-party/libusb/doc/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/doc/doxygen.cfg.in` & `pyjoulescope_driver-1.3.9/third-party/libusb/doc/doxygen.cfg.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/doc/libusb.png` & `pyjoulescope_driver-1.3.9/third-party/libusb/doc/libusb.png`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/dpfp.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/dpfp.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/ezusb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/ezusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/ezusb.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/ezusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/fxload.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/fxload.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/hotplugtest.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/hotplugtest.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/listdevs.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/listdevs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/sam3u_benchmark.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/sam3u_benchmark.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/testlibusb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/testlibusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/examples/xusb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/examples/xusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/include/linux/config.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/include/linux/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/include/macos/config.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/include/macos/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/Makefile.am` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/Makefile.am.extra` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/Makefile.am.extra`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/core.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/core.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/descriptor.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/descriptor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/hotplug.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/hotplug.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/io.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/io.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusb-1.0.def` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusb-1.0.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusb-1.0.rc` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusb-1.0.rc`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusb.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/libusbi.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/libusbi.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/darwin_usb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/darwin_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/darwin_usb.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/darwin_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/emscripten_webusb.cpp` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/emscripten_webusb.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_posix.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_posix.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_windows.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/events_windows.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/events_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_pollfs.cpp` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_pollfs.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb_backend.cpp` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb_backend.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb_raw.cpp` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb_raw.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/haiku_usb_raw.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/haiku_usb_raw.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_netlink.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_netlink.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_udev.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_udev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_usbfs.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_usbfs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/linux_usbfs.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/linux_usbfs.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/netbsd_usb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/netbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/null_usb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/null_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/openbsd_usb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/openbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/sunos_usb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/sunos_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/sunos_usb.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/sunos_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_posix.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_posix.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_windows.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/threads_windows.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/threads_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_common.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_common.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_common.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_common.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_usbdk.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_usbdk.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_usbdk.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_usbdk.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_winusb.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_winusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/os/windows_winusb.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/os/windows_winusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/strerror.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/strerror.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/libusb/sync.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/libusb/sync.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Base.props` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Configuration.Base.props` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Configuration.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/Configuration.DynamicLibrary.props` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/Configuration.DynamicLibrary.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/ProjectConfigurations.Base.props` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/ProjectConfigurations.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/build_all.ps1` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/build_all.ps1`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/config.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/dpfp.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/dpfp.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/dpfp_threaded.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/dpfp_threaded.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/fxload.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/fxload.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt/getopt.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt/getopt.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt/getopt.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt/getopt.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt/getopt1.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt/getopt1.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/getopt.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/getopt.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/hotplugtest.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/hotplugtest.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/libusb.sln` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/libusb.sln`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/libusb_dll.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/libusb_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/libusb_static.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/libusb_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/listdevs.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/listdevs.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/sam3u_benchmark.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/sam3u_benchmark.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/stress.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/stress.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/testlibusb.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/testlibusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/msvc/xusb.vcxproj` & `pyjoulescope_driver-1.3.9/third-party/libusb/msvc/xusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/tests/Makefile.am` & `pyjoulescope_driver-1.3.9/third-party/libusb/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/tests/libusb_testlib.h` & `pyjoulescope_driver-1.3.9/third-party/libusb/tests/libusb_testlib.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/tests/stress.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/tests/stress.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/tests/testlib.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/tests/testlib.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/libusb/tests/umockdev.c` & `pyjoulescope_driver-1.3.9/third-party/libusb/tests/umockdev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/tinyprintf/tinyprintf.c` & `pyjoulescope_driver-1.3.9/third-party/tinyprintf/tinyprintf.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/tinyprintf/tinyprintf.h` & `pyjoulescope_driver-1.3.9/third-party/tinyprintf/tinyprintf.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.8/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new` & `pyjoulescope_driver-1.3.9/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new`

 * *Files identical despite different names*

