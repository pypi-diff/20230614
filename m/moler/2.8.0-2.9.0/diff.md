# Comparing `tmp/moler-2.8.0.tar.gz` & `tmp/moler-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moler-2.8.0.tar", last modified: Tue Feb 21 07:37:10 2023, max compression
+gzip compressed data, was "moler-2.9.0.tar", last modified: Wed Apr 19 08:39:41 2023, max compression
```

## Comparing `moler-2.8.0.tar` & `moler-2.9.0.tar`

### file list

```diff
@@ -1,362 +1,363 @@
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/test/
--rw-r--r--   0 ute       (1000) ute       (1000)     8697 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_connection_configuration.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5290 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_connection_factory.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/test/device/
--rw-r--r--   0 ute       (1000) ute       (1000)     1239 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_SM_at_remote.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1707 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_SM_scpi.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2087 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_SM_juniper_ex.py
--rw-r--r--   0 ute       (1000) ute       (1000)    34004 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_device_configuration.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1751 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_SM_adb_remote.py
--rw-r--r--   0 ute       (1000) ute       (1000)      712 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_SM_unix_local.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1646 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_SM_pdu_aten.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9050 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_SM_unix_remote.py
--rw-r--r--   0 ute       (1000) ute       (1000)        0 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4699 2022-09-22 09:02:42.000000 moler-2.8.0/test/device/test_device.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/test/integration/
--rw-r--r--   0 ute       (1000) ute       (1000)     5898 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_io_tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1030 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_io_raw_subprocess.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3536 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_thread_based_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1938 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_io_device_unix_on_terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8505 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3836 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_connection_observer_with_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)    43199 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_io_raw_ssh.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2893 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_io_raw_terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5832 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_many_commands_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)    15070 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_devices_SM.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4299 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_connection_observer_with_external-io.py
--rw-r--r--   0 ute       (1000) ute       (1000)    15097 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/py3test_io_tcp_async_in_thread.py
--rw-r--r--   0 ute       (1000) ute       (1000)    37252 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/py3test_runners.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6580 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/py3test_io_tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)        0 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10265 2022-09-22 09:02:42.000000 moler-2.8.0/test/integration/test_io_raw_memory.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9533 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_publisher.py
--rw-r--r--   0 ute       (1000) ute       (1000)    24545 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_connection_observer.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8337 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_event.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3926 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_util_loghelper.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2845 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_table_read_parser.py
--rw-r--r--   0 ute       (1000) ute       (1000)    15348 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_loggers.py
--rw-r--r--   0 ute       (1000) ute       (1000)      464 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_moler_sleep.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11825 2023-02-21 06:54:25.000000 moler-2.8.0/test/test_helpers.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4184 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_scheduler.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/test/events/
--rw-r--r--   0 ute       (1000) ute       (1000)      140 2022-09-22 09:02:42.000000 moler-2.8.0/test/events/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/test/events/unix/
--rw-r--r--   0 ute       (1000) ute       (1000)     2052 2022-09-22 09:02:42.000000 moler-2.8.0/test/events/unix/test_event_wait4prompts.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3695 2022-09-22 09:02:42.000000 moler-2.8.0/test/events/unix/test_event_ping_no_response.py
--rw-r--r--   0 ute       (1000) ute       (1000)      140 2022-09-22 09:02:42.000000 moler-2.8.0/test/events/unix/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3239 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_event_awaiter.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10233 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_cmds_events_doc.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20235 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10804 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_command.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18472 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_moler_test.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8152 2022-09-22 09:02:42.000000 moler-2.8.0/test/test_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2833 2023-02-21 07:31:31.000000 moler-2.8.0/setup.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler.egg-info/
--rw-r--r--   0 ute       (1000) ute       (1000)        1 2023-02-21 07:37:08.000000 moler-2.8.0/moler.egg-info/dependency_links.txt
--rw-r--r--   0 ute       (1000) ute       (1000)     9451 2023-02-21 07:37:08.000000 moler-2.8.0/moler.egg-info/SOURCES.txt
--rw-r--r--   0 ute       (1000) ute       (1000)    31142 2023-02-21 07:37:08.000000 moler-2.8.0/moler.egg-info/PKG-INFO
--rw-r--r--   0 ute       (1000) ute       (1000)      481 2023-02-21 07:37:08.000000 moler-2.8.0/moler.egg-info/requires.txt
--rw-r--r--   0 ute       (1000) ute       (1000)       11 2023-02-21 07:37:08.000000 moler-2.8.0/moler.egg-info/top_level.txt
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/
--rw-r--r--   0 ute       (1000) ute       (1000)     5311 2022-09-22 09:02:42.000000 moler-2.8.0/moler/event.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6333 2022-11-15 13:25:06.000000 moler-2.8.0/moler/exceptions.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19981 2022-09-22 09:02:42.000000 moler-2.8.0/moler/runner_single_thread.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/device/
--rw-r--r--   0 ute       (1000) ute       (1000)    15980 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/adbremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2065 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/state_machine.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9792 2022-10-03 06:57:25.000000 moler-2.8.0/moler/device/unixlocal.py
--rw-r--r--   0 ute       (1000) ute       (1000)    22403 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/adbremote2.py
--rw-r--r--   0 ute       (1000) ute       (1000)    14312 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/junipergeneric.py
--rw-r--r--   0 ute       (1000) ute       (1000)    16857 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/proxy_pc2.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7148 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/abstract_device.py
--rw-r--r--   0 ute       (1000) ute       (1000)    45451 2022-11-15 13:25:06.000000 moler-2.8.0/moler/device/textualdevice.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10797 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/proxy_pc.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20174 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/device.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10499 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/atremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12221 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/pdu_aten.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1591 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/juniper_ex.py
--rw-r--r--   0 ute       (1000) ute       (1000)      425 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11861 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/scpi.py
--rw-r--r--   0 ute       (1000) ute       (1000)    24734 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/unixremote2.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19608 2022-09-22 09:02:42.000000 moler-2.8.0/moler/device/unixremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    50330 2022-09-22 09:02:41.000000 moler-2.8.0/moler/asyncio_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5728 2022-09-22 09:02:42.000000 moler-2.8.0/moler/moler_connection_for_single_thread_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6714 2022-09-22 09:02:42.000000 moler-2.8.0/moler/scheduler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3351 2022-09-22 09:02:42.000000 moler-2.8.0/moler/instance_loader.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/util/
--rw-r--r--   0 ute       (1000) ute       (1000)     4427 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/converterhelper.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2479 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/compressed_rotating_file_handler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9734 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/moler_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2946 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/loghelper.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1584 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/connection_observer_life_status.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1509 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/connection_observer.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12527 2022-11-15 13:25:06.000000 moler-2.8.0/moler/util/devices_SM.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9815 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/moler_test.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1950 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/tracked_thread.py
--rw-r--r--   0 ute       (1000) ute       (1000)      138 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1309 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/compressed_timed_rotating_file_handler.py
--rwxr-xr-x   0 ute       (1000) ute       (1000)    14622 2022-09-22 09:02:42.000000 moler-2.8.0/moler/util/cmds_events_doc.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3954 2022-09-22 09:02:42.000000 moler-2.8.0/moler/runner_factory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12699 2022-09-22 09:02:42.000000 moler-2.8.0/moler/helpers.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4871 2023-02-21 06:54:25.000000 moler-2.8.0/moler/observer_thread_wrapper.py
--rw-r--r--   0 ute       (1000) ute       (1000)    37032 2023-02-21 06:54:25.000000 moler-2.8.0/moler/runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8703 2022-09-22 09:02:41.000000 moler-2.8.0/moler/command_scheduler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2516 2022-09-22 09:02:41.000000 moler-2.8.0/moler/command.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17880 2023-02-21 06:54:25.000000 moler-2.8.0/moler/connection_observer.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1594 2022-09-22 09:02:41.000000 moler-2.8.0/moler/connection.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/parser/
--rw-r--r--   0 ute       (1000) ute       (1000)    16963 2022-09-22 09:02:42.000000 moler-2.8.0/moler/parser/table_text.py
--rw-r--r--   0 ute       (1000) ute       (1000)      141 2022-09-22 09:02:42.000000 moler-2.8.0/moler/parser/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5483 2022-09-22 09:02:42.000000 moler-2.8.0/moler/publisher.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8914 2022-09-22 09:02:41.000000 moler-2.8.0/moler/connection_factory.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/io/
--rw-r--r--   0 ute       (1000) ute       (1000)     7219 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/io_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2158 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/io_exceptions.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/io/raw/
--rw-r--r--   0 ute       (1000) ute       (1000)     7388 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/raw/terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7617 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/raw/tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9878 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/raw/tcpserverpiped.py
--rw-r--r--   0 ute       (1000) ute       (1000)      804 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/raw/subprocess.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9809 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/raw/memory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    23077 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/raw/sshshell.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1328 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/raw/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      499 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/io/asyncio/
--rw-r--r--   0 ute       (1000) ute       (1000)    14912 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/asyncio/terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6001 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/asyncio/tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)      515 2022-09-22 09:02:42.000000 moler-2.8.0/moler/io/asyncio/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/events/
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/events/shared/
--rw-r--r--   0 ute       (1000) ute       (1000)     5585 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/shared/wait4.py
--rw-r--r--   0 ute       (1000) ute       (1000)      673 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/shared/genericshared_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2236 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/shared/password_prompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1241 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/shared/genericshared_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      180 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/shared/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/events/juniper/
--rw-r--r--   0 ute       (1000) ute       (1000)      324 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/juniper/genericshared_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      898 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/juniper/genericshared_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      193 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/juniper/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/events/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)      892 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/scpi/genericscpi_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      325 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/scpi/genericscpi_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      186 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/scpi/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/events/pdu_aten/
--rw-r--r--   0 ute       (1000) ute       (1000)      190 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/pdu_aten/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7188 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5986 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      134 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/events/unix/
--rw-r--r--   0 ute       (1000) ute       (1000)     2814 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/last_login.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1243 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/genericunix_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2302 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/ping_response.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2236 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/failed_login_counter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1463 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/wait4prompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)      675 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/genericunix_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1319 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/shutdown.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4736 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/ping_no_response.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3756 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/wait4prompts.py
--rw-r--r--   0 ute       (1000) ute       (1000)      997 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/last_failed_login.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2191 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/advise_to_change_your_password.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4570 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/u_boot_crtm.py
--rw-r--r--   0 ute       (1000) ute       (1000)      188 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3599 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/private_system.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1756 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/unix/warning_default_password.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/events/juniper_ex/
--rw-r--r--   0 ute       (1000) ute       (1000)      903 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      336 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/juniper_ex/genericjuniper_ex_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      195 2022-09-22 09:02:42.000000 moler-2.8.0/moler/events/juniper_ex/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1672 2022-09-22 09:02:42.000000 moler-2.8.0/moler/observable_connection.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/at/
--rw-r--r--   0 ute       (1000) ute       (1000)     2792 2023-01-04 09:28:39.000000 moler-2.8.0/moler/cmd/at/get_functionality_level.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3630 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/cu.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3294 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_revision_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5957 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_imei.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2251 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/set_mode.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3125 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_manufacturer_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4365 2022-11-15 13:25:06.000000 moler-2.8.0/moler/cmd/at/run_script.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3385 2023-01-04 09:28:39.000000 moler-2.8.0/moler/cmd/at/set_functionality_level.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4976 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_apns.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1553 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/attach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1526 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/detach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2816 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/exit_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3804 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/genericat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1588 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/at.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3133 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_ip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2654 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_imsi.py
--rw-r--r--   0 ute       (1000) ute       (1000)      369 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3590 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/plink_serial.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3062 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_attach_state.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1878 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/enable_echo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5058 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/get_product_info.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2629 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/at/set_apn.py
--rw-r--r--   0 ute       (1000) ute       (1000)    23965 2023-02-21 06:54:25.000000 moler-2.8.0/moler/cmd/commandtextualgeneric.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/juniper/
--rw-r--r--   0 ute       (1000) ute       (1000)      938 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper/genericjuniper.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/juniper/configure/
--rw-r--r--   0 ute       (1000) ute       (1000)     2616 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper/configure/exit_configure.py
--rw-r--r--   0 ute       (1000) ute       (1000)      205 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper/configure/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      195 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/juniper/cli/
--rw-r--r--   0 ute       (1000) ute       (1000)     2571 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper/cli/configure.py
--rw-r--r--   0 ute       (1000) ute       (1000)      199 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper/cli/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/cmd/scpi/
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/cmd/scpi/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)     1598 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/scpi/read.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1364 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/scpi/idn.py
--rw-r--r--   0 ute       (1000) ute       (1000)      415 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/scpi/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1929 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/scpi/run_command.py
--rw-r--r--   0 ute       (1000) ute       (1000)      969 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/scpi/genericscpistate.py
--rw-r--r--   0 ute       (1000) ute       (1000)      202 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/scpi/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      370 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/genricscpi.py
--rw-r--r--   0 ute       (1000) ute       (1000)      188 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/scpi/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/pdu_aten/
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/
--rw-r--r--   0 ute       (1000) ute       (1000)     2879 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/read_status.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1890 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/sw.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2303 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/generic_pdu.py
--rw-r--r--   0 ute       (1000) ute       (1000)      415 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2933 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/read_meter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1589 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/quit.py
--rw-r--r--   0 ute       (1000) ute       (1000)      205 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/pdu/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      904 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/generic_pdu_aten.py
--rw-r--r--   0 ute       (1000) ute       (1000)      192 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/pdu_aten/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10313 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/commandchangingprompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4263 2023-02-21 06:54:25.000000 moler-2.8.0/moler/cmd/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/adb/
--rw-r--r--   0 ute       (1000) ute       (1000)     5676 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/adb/adb_shell.py
--rw-r--r--   0 ute       (1000) ute       (1000)      331 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/adb/generic_adb_command.py
--rw-r--r--   0 ute       (1000) ute       (1000)      191 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/adb/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/cmd/unix/
--rw-r--r--   0 ute       (1000) ute       (1000)    40767 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/wget.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12524 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/scp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4636 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/head.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2619 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/pwd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5740 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/gunzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3472 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/cut.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2626 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/chown.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2015 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/chgrp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7087 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/su.py
--rw-r--r--   0 ute       (1000) ute       (1000)    58711 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/iperf.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10461 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/sftp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3424 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/userdel.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17031 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ping.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11679 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/nping.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6441 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ip_link.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1473 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/adb_root.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10395 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/unzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4078 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/sed.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3048 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/reboot.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7766 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/traceroute.py
--rw-r--r--   0 ute       (1000) ute       (1000)    21236 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/netstat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2793 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ctrl_c.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6767 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/socat.py
--rw-r--r--   0 ute       (1000) ute       (1000)      432 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/logout.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12200 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ss.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3352 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/cd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1884 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/mkdir.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8277 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/openssl_x509_text_in.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4249 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/run_script.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18977 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2527 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/history.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3769 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4920 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/sshkeygen.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3565 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/sysctl.py
--rw-r--r--   0 ute       (1000) ute       (1000)    16399 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ls.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3119 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/which.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1077 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/enter.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20321 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/sudo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3678 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/devmem.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3773 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/hexdump.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1701 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/md5sum.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1772 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/rm.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5324 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/date.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5486 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/cat.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18527 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/lxc_ls.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5652 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/mpstat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6948 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ip_addr.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2043 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/mv.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6530 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/export.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4412 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/dmesg.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4737 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/gzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7006 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/lxc_info.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9047 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ip_neigh.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2106 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/kill.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2623 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/killall.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9989 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/w.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4955 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/mount.py
--rw-r--r--   0 ute       (1000) ute       (1000)    40235 2023-01-10 12:45:16.000000 moler-2.8.0/moler/cmd/unix/nmap.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1598 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/exit.py
--rw-r--r--   0 ute       (1000) ute       (1000)      934 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/tar.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1949 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/zip.py
--rw-r--r--   0 ute       (1000) ute       (1000)    44569 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ssh.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1950 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/adb_forward.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8154 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/find.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1139 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/sync.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4950 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7261 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/uptime.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20423 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ifconfig.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6034 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/lxc_attach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2684 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/uname.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1692 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/cp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5682 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/tail_latest_file.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1418 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/hostname.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17165 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/systemctl.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3783 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/run_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19975 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ip_route.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1201 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/bash.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4773 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/shasum.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1215 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/whoami.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3081 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/tee.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7889 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/route.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2279 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/chmod.py
--rw-r--r--   0 ute       (1000) ute       (1000)   115934 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/iperf2.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4264 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/du.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8662 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/service.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11822 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/generictelnetssh.py
--rw-r--r--   0 ute       (1000) ute       (1000)      194 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7597 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/nft.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1875 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/unxz.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2304 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/tail.py
--rw-r--r--   0 ute       (1000) ute       (1000)    89392 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/iptables.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9181 2022-12-22 09:28:26.000000 moler-2.8.0/moler/cmd/unix/passwd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1554 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ln.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3009 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/genericunix.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6135 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/env.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10563 2023-01-10 15:01:34.000000 moler-2.8.0/moler/cmd/unix/ethtool.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2799 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/useradd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9084 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/grep.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17423 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ipsec.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6248 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ntpq.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8529 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/lsof.py
--rw-r--r--   0 ute       (1000) ute       (1000)    24457 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/tcpdump.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5318 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/df.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11003 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/tshark.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3841 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/openssl_s_client.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4671 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/adb_devices.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7838 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/hciconfig.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1384 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/pkill.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17638 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/top.py
--rw-r--r--   0 ute       (1000) ute       (1000)    15745 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/ps.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4177 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/unix/echo.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/juniper_ex/
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/juniper_ex/configure/
--rw-r--r--   0 ute       (1000) ute       (1000)      207 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper_ex/configure/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      197 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper_ex/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      359 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper_ex/genericjuniperex.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:09.000000 moler-2.8.0/moler/cmd/juniper_ex/cli/
--rw-r--r--   0 ute       (1000) ute       (1000)      201 2022-09-22 09:02:41.000000 moler-2.8.0/moler/cmd/juniper_ex/cli/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      143 2022-09-22 09:02:41.000000 moler-2.8.0/moler/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8547 2022-09-22 09:02:42.000000 moler-2.8.0/moler/threaded_moler_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2439 2022-09-22 09:02:42.000000 moler-2.8.0/moler/event_awaiter.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10727 2022-09-22 09:02:41.000000 moler-2.8.0/moler/abstract_moler_connection.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-02-21 07:37:10.000000 moler-2.8.0/moler/config/
--rw-r--r--   0 ute       (1000) ute       (1000)     1421 2022-09-22 09:02:41.000000 moler-2.8.0/moler/config/devices.py
--rw-r--r--   0 ute       (1000) ute       (1000)    31702 2022-09-22 09:02:41.000000 moler-2.8.0/moler/config/loggers.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1566 2022-09-22 09:02:41.000000 moler-2.8.0/moler/config/runners.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11854 2022-09-22 09:02:41.000000 moler-2.8.0/moler/config/connections.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11562 2022-09-22 09:02:41.000000 moler-2.8.0/moler/config/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    25315 2023-02-21 07:31:31.000000 moler-2.8.0/README.md
--rw-r--r--   0 ute       (1000) ute       (1000)    31142 2023-02-21 07:37:10.000000 moler-2.8.0/PKG-INFO
--rw-r--r--   0 ute       (1000) ute       (1000)      165 2023-02-21 07:37:10.000000 moler-2.8.0/setup.cfg
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.960336 moler-2.9.0/
+-rw-r--r--   0 ute       (1000) ute       (1000)     1505 2022-09-22 09:02:41.000000 moler-2.9.0/LICENSE
+-rw-r--r--   0 ute       (1000) ute       (1000)    26669 2023-04-19 08:39:41.960336 moler-2.9.0/PKG-INFO
+-rw-r--r--   0 ute       (1000) ute       (1000)    25315 2023-04-19 08:38:18.000000 moler-2.9.0/README.md
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.020333 moler-2.9.0/moler/
+-rw-r--r--   0 ute       (1000) ute       (1000)      143 2022-09-22 09:02:41.000000 moler-2.9.0/moler/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10727 2022-09-22 09:02:41.000000 moler-2.9.0/moler/abstract_moler_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    50330 2022-09-22 09:02:41.000000 moler-2.9.0/moler/asyncio_runner.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.044333 moler-2.9.0/moler/cmd/
+-rw-r--r--   0 ute       (1000) ute       (1000)     4263 2023-02-21 06:54:25.000000 moler-2.9.0/moler/cmd/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.064333 moler-2.9.0/moler/cmd/adb/
+-rw-r--r--   0 ute       (1000) ute       (1000)      191 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/adb/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5676 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/adb/adb_shell.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      331 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/adb/generic_adb_command.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.164333 moler-2.9.0/moler/cmd/at/
+-rw-r--r--   0 ute       (1000) ute       (1000)      369 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1588 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/at.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1553 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/attach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3630 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/cu.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1526 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/detach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1878 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/enable_echo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2816 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/exit_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3804 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/genericat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4976 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_apns.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3062 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_attach_state.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2792 2023-01-04 09:28:39.000000 moler-2.9.0/moler/cmd/at/get_functionality_level.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5957 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_imei.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2654 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_imsi.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3133 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_ip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3125 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_manufacturer_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5058 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_product_info.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3294 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/get_revision_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3590 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/plink_serial.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4365 2022-11-15 13:25:06.000000 moler-2.9.0/moler/cmd/at/run_script.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2629 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/set_apn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3385 2023-01-04 09:28:39.000000 moler-2.9.0/moler/cmd/at/set_functionality_level.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2251 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/at/set_mode.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10507 2023-04-19 08:35:33.000000 moler-2.9.0/moler/cmd/commandchangingprompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    22630 2023-04-19 08:35:33.000000 moler-2.9.0/moler/cmd/commandtextualgeneric.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.164333 moler-2.9.0/moler/cmd/juniper/
+-rw-r--r--   0 ute       (1000) ute       (1000)      195 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.172333 moler-2.9.0/moler/cmd/juniper/cli/
+-rw-r--r--   0 ute       (1000) ute       (1000)      199 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper/cli/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2571 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper/cli/configure.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.176333 moler-2.9.0/moler/cmd/juniper/configure/
+-rw-r--r--   0 ute       (1000) ute       (1000)      205 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper/configure/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2616 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper/configure/exit_configure.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      938 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper/genericjuniper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.176333 moler-2.9.0/moler/cmd/juniper_ex/
+-rw-r--r--   0 ute       (1000) ute       (1000)      197 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper_ex/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.176333 moler-2.9.0/moler/cmd/juniper_ex/cli/
+-rw-r--r--   0 ute       (1000) ute       (1000)      201 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper_ex/cli/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.180333 moler-2.9.0/moler/cmd/juniper_ex/configure/
+-rw-r--r--   0 ute       (1000) ute       (1000)      207 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper_ex/configure/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      359 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/juniper_ex/genericjuniperex.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.180333 moler-2.9.0/moler/cmd/pdu_aten/
+-rw-r--r--   0 ute       (1000) ute       (1000)      192 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      904 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/generic_pdu_aten.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.188333 moler-2.9.0/moler/cmd/pdu_aten/pdu/
+-rw-r--r--   0 ute       (1000) ute       (1000)      205 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/pdu/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      415 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/pdu/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2303 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/pdu/generic_pdu.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1589 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/pdu/quit.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2933 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/pdu/read_meter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2879 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/pdu/read_status.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1890 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/pdu_aten/pdu/sw.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.196333 moler-2.9.0/moler/cmd/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      188 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      370 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/genricscpi.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.200333 moler-2.9.0/moler/cmd/scpi/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      202 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      415 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/scpi/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      969 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/scpi/genericscpistate.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1364 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/scpi/idn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1598 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/scpi/read.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1929 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/scpi/scpi/run_command.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.484334 moler-2.9.0/moler/cmd/unix/
+-rw-r--r--   0 ute       (1000) ute       (1000)      194 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4671 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/adb_devices.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1950 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/adb_forward.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1473 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/adb_root.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1201 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/bash.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5486 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/cat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3352 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/cd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2015 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/chgrp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2279 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/chmod.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2626 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/chown.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1692 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/cp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2793 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ctrl_c.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3472 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/cut.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5324 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/date.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3678 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/devmem.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5318 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/df.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4412 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/dmesg.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4264 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/du.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4177 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/echo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1077 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/enter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6135 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/env.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10563 2023-01-10 15:01:34.000000 moler-2.9.0/moler/cmd/unix/ethtool.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1598 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/exit.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3769 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6530 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/export.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8154 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/find.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11822 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/generictelnetssh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3009 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/genericunix.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9084 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/grep.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5740 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/gunzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4737 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/gzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7838 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/hciconfig.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4636 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/head.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3773 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/hexdump.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2527 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/history.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1418 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/hostname.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4950 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20423 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ifconfig.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6948 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ip_addr.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6441 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ip_link.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9047 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ip_neigh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19975 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ip_route.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    58711 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/iperf.py
+-rw-r--r--   0 ute       (1000) ute       (1000)   115934 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/iperf2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17423 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ipsec.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    89392 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/iptables.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2106 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/kill.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2623 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/killall.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1554 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ln.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      432 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/logout.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    16399 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ls.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8529 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/lsof.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6034 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/lxc_attach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7006 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/lxc_info.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18527 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/lxc_ls.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1701 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/md5sum.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1884 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/mkdir.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4955 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/mount.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5652 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/mpstat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2043 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/mv.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    21236 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/netstat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7597 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/nft.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    40235 2023-01-10 12:45:16.000000 moler-2.9.0/moler/cmd/unix/nmap.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11679 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/nping.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6248 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ntpq.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3841 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/openssl_s_client.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8277 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/openssl_x509_text_in.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9181 2022-12-22 09:28:26.000000 moler-2.9.0/moler/cmd/unix/passwd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17031 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ping.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1384 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/pkill.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    15745 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ps.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2619 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/pwd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3048 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/reboot.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1772 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/rm.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7889 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/route.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4249 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/run_script.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3783 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/run_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12524 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/scp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4078 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/sed.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8662 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/service.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10461 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/sftp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4773 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/shasum.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6767 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/socat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12200 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ss.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    44569 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/ssh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4920 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/sshkeygen.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7087 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/su.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20321 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/sudo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1139 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/sync.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3565 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/sysctl.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17165 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/systemctl.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2304 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/tail.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5682 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/tail_latest_file.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      934 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/tar.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    24457 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/tcpdump.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3081 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/tee.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18977 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17638 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/top.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7766 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/traceroute.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11003 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/tshark.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2684 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/uname.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1875 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/unxz.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10395 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/unzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7261 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/uptime.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2799 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/useradd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3424 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/userdel.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9989 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/w.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    40767 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/wget.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3119 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/which.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1215 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/whoami.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1949 2022-09-22 09:02:41.000000 moler-2.9.0/moler/cmd/unix/zip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2516 2022-09-22 09:02:41.000000 moler-2.9.0/moler/command.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8703 2022-09-22 09:02:41.000000 moler-2.9.0/moler/command_scheduler.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.492334 moler-2.9.0/moler/config/
+-rw-r--r--   0 ute       (1000) ute       (1000)    11562 2022-09-22 09:02:41.000000 moler-2.9.0/moler/config/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11854 2022-09-22 09:02:41.000000 moler-2.9.0/moler/config/connections.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1421 2022-09-22 09:02:41.000000 moler-2.9.0/moler/config/devices.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    31702 2022-09-22 09:02:41.000000 moler-2.9.0/moler/config/loggers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1566 2022-09-22 09:02:41.000000 moler-2.9.0/moler/config/runners.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1594 2022-09-22 09:02:41.000000 moler-2.9.0/moler/connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8914 2022-09-22 09:02:41.000000 moler-2.9.0/moler/connection_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18244 2023-04-19 08:35:33.000000 moler-2.9.0/moler/connection_observer.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.568334 moler-2.9.0/moler/device/
+-rw-r--r--   0 ute       (1000) ute       (1000)      425 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7148 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/abstract_device.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    15980 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/adbremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    22403 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/adbremote2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10499 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/atremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20174 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/device.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1591 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/juniper_ex.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    14312 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/junipergeneric.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12221 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/pdu_aten.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10797 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/proxy_pc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17097 2023-04-19 08:35:33.000000 moler-2.9.0/moler/device/proxy_pc2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11861 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/scpi.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2065 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/state_machine.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    45451 2022-11-15 13:25:06.000000 moler-2.9.0/moler/device/textualdevice.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9792 2022-10-03 06:57:25.000000 moler-2.9.0/moler/device/unixlocal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19608 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/unixremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    24734 2022-09-22 09:02:42.000000 moler-2.9.0/moler/device/unixremote2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5311 2022-09-22 09:02:42.000000 moler-2.9.0/moler/event.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2439 2022-09-22 09:02:42.000000 moler-2.9.0/moler/event_awaiter.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.576335 moler-2.9.0/moler/events/
+-rw-r--r--   0 ute       (1000) ute       (1000)      134 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.588335 moler-2.9.0/moler/events/juniper/
+-rw-r--r--   0 ute       (1000) ute       (1000)      193 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/juniper/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      898 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/juniper/genericshared_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      324 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/juniper/genericshared_textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.600335 moler-2.9.0/moler/events/juniper_ex/
+-rw-r--r--   0 ute       (1000) ute       (1000)      195 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/juniper_ex/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      903 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      336 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/juniper_ex/genericjuniper_ex_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7188 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/lineevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.608335 moler-2.9.0/moler/events/pdu_aten/
+-rw-r--r--   0 ute       (1000) ute       (1000)      190 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/pdu_aten/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.608335 moler-2.9.0/moler/events/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      186 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      892 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/scpi/genericscpi_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      325 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/scpi/genericscpi_textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.640335 moler-2.9.0/moler/events/shared/
+-rw-r--r--   0 ute       (1000) ute       (1000)      180 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/shared/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1241 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/shared/genericshared_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      673 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/shared/genericshared_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2236 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/shared/password_prompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5585 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/shared/wait4.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5986 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.712335 moler-2.9.0/moler/events/unix/
+-rw-r--r--   0 ute       (1000) ute       (1000)      188 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2191 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/advise_to_change_your_password.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2236 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/failed_login_counter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1243 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/genericunix_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      675 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/genericunix_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      997 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/last_failed_login.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2814 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/last_login.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4736 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/ping_no_response.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2302 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/ping_response.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3599 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/private_system.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1319 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/shutdown.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4570 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/u_boot_crtm.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1463 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/wait4prompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4247 2023-04-19 08:35:33.000000 moler-2.9.0/moler/events/unix/wait4prompts.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1756 2022-09-22 09:02:42.000000 moler-2.9.0/moler/events/unix/warning_default_password.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6333 2022-11-15 13:25:06.000000 moler-2.9.0/moler/exceptions.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12699 2022-09-22 09:02:42.000000 moler-2.9.0/moler/helpers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3351 2022-09-22 09:02:42.000000 moler-2.9.0/moler/instance_loader.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.724335 moler-2.9.0/moler/io/
+-rw-r--r--   0 ute       (1000) ute       (1000)      499 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.740335 moler-2.9.0/moler/io/asyncio/
+-rw-r--r--   0 ute       (1000) ute       (1000)      515 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/asyncio/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6001 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/asyncio/tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    14912 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/asyncio/terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7219 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/io_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2158 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/io_exceptions.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.756335 moler-2.9.0/moler/io/raw/
+-rw-r--r--   0 ute       (1000) ute       (1000)     1328 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/raw/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9809 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/raw/memory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    23077 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/raw/sshshell.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      804 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/raw/subprocess.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7617 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/raw/tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9878 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/raw/tcpserverpiped.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7388 2022-09-22 09:02:42.000000 moler-2.9.0/moler/io/raw/terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5728 2022-09-22 09:02:42.000000 moler-2.9.0/moler/moler_connection_for_single_thread_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1672 2022-09-22 09:02:42.000000 moler-2.9.0/moler/observable_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4871 2023-02-21 06:54:25.000000 moler-2.9.0/moler/observer_thread_wrapper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.756335 moler-2.9.0/moler/parser/
+-rw-r--r--   0 ute       (1000) ute       (1000)      141 2022-09-22 09:02:42.000000 moler-2.9.0/moler/parser/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    16963 2022-09-22 09:02:42.000000 moler-2.9.0/moler/parser/table_text.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5483 2022-09-22 09:02:42.000000 moler-2.9.0/moler/publisher.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    37032 2023-02-21 06:54:25.000000 moler-2.9.0/moler/runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3954 2022-09-22 09:02:42.000000 moler-2.9.0/moler/runner_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19981 2022-09-22 09:02:42.000000 moler-2.9.0/moler/runner_single_thread.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6714 2022-09-22 09:02:42.000000 moler-2.9.0/moler/scheduler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8547 2022-09-22 09:02:42.000000 moler-2.9.0/moler/threaded_moler_connection.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.780335 moler-2.9.0/moler/util/
+-rw-r--r--   0 ute       (1000) ute       (1000)      138 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/__init__.py
+-rwxr-xr-x   0 ute       (1000) ute       (1000)    14622 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/cmds_events_doc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2479 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/compressed_rotating_file_handler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1309 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/compressed_timed_rotating_file_handler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1509 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/connection_observer.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1584 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/connection_observer_life_status.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4427 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/converterhelper.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12527 2023-04-19 08:35:33.000000 moler-2.9.0/moler/util/devices_SM.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2946 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/loghelper.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9734 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/moler_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9815 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/moler_test.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1950 2022-09-22 09:02:42.000000 moler-2.9.0/moler/util/tracked_thread.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.028333 moler-2.9.0/moler.egg-info/
+-rw-r--r--   0 ute       (1000) ute       (1000)    26669 2023-04-19 08:39:40.000000 moler-2.9.0/moler.egg-info/PKG-INFO
+-rw-r--r--   0 ute       (1000) ute       (1000)     9459 2023-04-19 08:39:40.000000 moler-2.9.0/moler.egg-info/SOURCES.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)        1 2023-04-19 08:39:40.000000 moler-2.9.0/moler.egg-info/dependency_links.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)      481 2023-04-19 08:39:40.000000 moler-2.9.0/moler.egg-info/requires.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)       11 2023-04-19 08:39:40.000000 moler-2.9.0/moler.egg-info/top_level.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)      165 2023-04-19 08:39:41.960336 moler-2.9.0/setup.cfg
+-rw-r--r--   0 ute       (1000) ute       (1000)     2833 2023-04-19 08:38:18.000000 moler-2.9.0/setup.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.888336 moler-2.9.0/test/
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.908336 moler-2.9.0/test/device/
+-rw-r--r--   0 ute       (1000) ute       (1000)        0 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1751 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_SM_adb_remote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1239 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_SM_at_remote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2087 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_SM_juniper_ex.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1646 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_SM_pdu_aten.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1707 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_SM_scpi.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      712 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_SM_unix_local.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9050 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_SM_unix_remote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4699 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_device.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    34004 2022-09-22 09:02:42.000000 moler-2.9.0/test/device/test_device_configuration.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.928336 moler-2.9.0/test/events/
+-rw-r--r--   0 ute       (1000) ute       (1000)      140 2022-09-22 09:02:42.000000 moler-2.9.0/test/events/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.932336 moler-2.9.0/test/events/unix/
+-rw-r--r--   0 ute       (1000) ute       (1000)      140 2022-09-22 09:02:42.000000 moler-2.9.0/test/events/unix/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3695 2022-09-22 09:02:42.000000 moler-2.9.0/test/events/unix/test_event_ping_no_response.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2817 2023-04-19 08:35:33.000000 moler-2.9.0/test/events/unix/test_event_wait4prompts.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2023-04-19 08:39:41.960336 moler-2.9.0/test/integration/
+-rw-r--r--   0 ute       (1000) ute       (1000)        0 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6580 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/py3test_io_tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    15097 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/py3test_io_tcp_async_in_thread.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    37252 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/py3test_runners.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4299 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_connection_observer_with_external-io.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3836 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_connection_observer_with_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    15070 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_devices_SM.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1938 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_io_device_unix_on_terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10265 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_io_raw_memory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    43236 2023-04-19 08:35:33.000000 moler-2.9.0/test/integration/test_io_raw_ssh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1030 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_io_raw_subprocess.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2893 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_io_raw_terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5898 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_io_tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5832 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_many_commands_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8505 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3536 2022-09-22 09:02:42.000000 moler-2.9.0/test/integration/test_thread_based_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10233 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_cmds_events_doc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10804 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_command.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20235 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8697 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_connection_configuration.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5290 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_connection_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    24545 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_connection_observer.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8337 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_event.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3239 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_event_awaiter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11825 2023-02-21 06:54:25.000000 moler-2.9.0/test/test_helpers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    15348 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_loggers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      464 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_moler_sleep.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18472 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_moler_test.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9533 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_publisher.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8152 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4184 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_scheduler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2845 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_table_read_parser.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3926 2022-09-22 09:02:42.000000 moler-2.9.0/test/test_util_loghelper.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `moler-2.8.0/test/test_connection_configuration.py` & `moler-2.9.0/test/test_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_connection_factory.py` & `moler-2.9.0/test/test_connection_factory.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_SM_at_remote.py` & `moler-2.9.0/test/device/test_SM_at_remote.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_SM_scpi.py` & `moler-2.9.0/test/device/test_SM_scpi.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_SM_juniper_ex.py` & `moler-2.9.0/test/device/test_SM_juniper_ex.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_device_configuration.py` & `moler-2.9.0/test/device/test_device_configuration.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_SM_adb_remote.py` & `moler-2.9.0/test/device/test_SM_adb_remote.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_SM_unix_local.py` & `moler-2.9.0/test/device/test_SM_unix_local.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_SM_pdu_aten.py` & `moler-2.9.0/test/device/test_SM_pdu_aten.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_SM_unix_remote.py` & `moler-2.9.0/test/device/test_SM_unix_remote.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/device/test_device.py` & `moler-2.9.0/test/device/test_device.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_io_tcp.py` & `moler-2.9.0/test/integration/test_io_tcp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_io_raw_subprocess.py` & `moler-2.9.0/test/integration/test_io_raw_subprocess.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_thread_based_runner.py` & `moler-2.9.0/test/integration/test_thread_based_runner.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_io_device_unix_on_terminal.py` & `moler-2.9.0/test/integration/test_io_device_unix_on_terminal.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_serial_proxy.py` & `moler-2.9.0/test/integration/test_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_connection_observer_with_runner.py` & `moler-2.9.0/test/integration/test_connection_observer_with_runner.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_io_raw_ssh.py` & `moler-2.9.0/test/integration/test_io_raw_ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,15 +481,16 @@
     from moler.io.io_exceptions import ConnectionTimeout
     connection = sshshell_connection
     with connection.open():
         with pytest.raises(ConnectionTimeout) as exc:
             big_data = "123456789 " * 10000
             request = "echo {}\n".format(big_data)
             bytes2send = request.encode("utf-8")
-            connection.send(bytes2send, timeout=0.001)
+            for x in range(10):
+                connection.send(bytes2send, timeout=0.0005)
         assert "Timeout (> 0.001 sec) on ssh://molerssh@localhost:22" in str(exc.value)
 
 
 def test_send_can_push_remaining_data_within_timeout(sshshell_connection):
     connection = sshshell_connection
     with connection.open():
         big_data = "123456789 " * 10000
```

### Comparing `moler-2.8.0/test/integration/test_io_raw_terminal.py` & `moler-2.9.0/test/integration/test_io_raw_terminal.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_many_commands_connection.py` & `moler-2.9.0/test/integration/test_many_commands_connection.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_devices_SM.py` & `moler-2.9.0/test/integration/test_devices_SM.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_connection_observer_with_external-io.py` & `moler-2.9.0/test/integration/test_connection_observer_with_external-io.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/py3test_io_tcp_async_in_thread.py` & `moler-2.9.0/test/integration/py3test_io_tcp_async_in_thread.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/py3test_runners.py` & `moler-2.9.0/test/integration/py3test_runners.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/py3test_io_tcp.py` & `moler-2.9.0/test/integration/py3test_io_tcp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/integration/test_io_raw_memory.py` & `moler-2.9.0/test/integration/test_io_raw_memory.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_publisher.py` & `moler-2.9.0/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_connection_observer.py` & `moler-2.9.0/test/test_connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_event.py` & `moler-2.9.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_util_loghelper.py` & `moler-2.9.0/test/test_util_loghelper.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_table_read_parser.py` & `moler-2.9.0/test/test_table_read_parser.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_loggers.py` & `moler-2.9.0/test/test_loggers.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_helpers.py` & `moler-2.9.0/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_scheduler.py` & `moler-2.9.0/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/events/unix/test_event_wait4prompts.py` & `moler-2.9.0/test/events/unix/test_event_wait4prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 __author__ = 'Marcin Usielski'
-__copyright__ = 'Copyright (C) 2021, Nokia'
+__copyright__ = 'Copyright (C) 2021-2023, Nokia'
 __email__ = 'marcin.usielski@nokia.com'
 
 
 from moler.events.unix.wait4prompts import Wait4prompts
 import datetime
 import re
 
@@ -19,14 +19,29 @@
     buffer_connection.moler_connection.data_received(output.encode("utf-8"), datetime.datetime.now())
     ret = event.await_done(timeout=0.5)[0]
     assert event.done() is True
     assert 'list_matched' in ret
     assert 1 == len(ret['list_matched'])
 
 
+def test_event_wait4prompts_change_prompts(buffer_connection):
+    prompts = {re.compile(r'host:.*#'): "UNIX_LOCAL", re.compile(r'user@server.*#'): "USER"}
+    output = "user@hoost:/home/#"
+    event = Wait4prompts(connection=buffer_connection.moler_connection, till_occurs_times=1, prompts=prompts)
+    event.check_against_all_prompts = True
+    event.start()
+    new_prompts = {re.compile(r'hoost:.*#'): "UNIX_LOCAL", re.compile(r'user@server.*#'): "USER"}
+    event.change_prompts(prompts=new_prompts)
+    buffer_connection.moler_connection.data_received(output.encode("utf-8"), datetime.datetime.now())
+    ret = event.await_done(timeout=0.5)[0]
+    assert event.done() is True
+    assert 'list_matched' in ret
+    assert 1 == len(ret['list_matched'])
+
+
 def test_event_wait4prompts_wrong_2_prompts_from_1_line(buffer_connection):
     prompts = {re.compile(r'host:.*#'): "UNIX_LOCAL", re.compile(r'user@.*#'): "USER"}
     output = "user@host:/home/#"
     event = Wait4prompts(connection=buffer_connection.moler_connection, till_occurs_times=1, prompts=prompts)
     event.check_against_all_prompts = True
     event.start()
     buffer_connection.moler_connection.data_received(output.encode("utf-8"), datetime.datetime.now())
@@ -42,7 +57,9 @@
     event = Wait4prompts(connection=buffer_connection.moler_connection, till_occurs_times=1, prompts=prompts)
     event.check_against_all_prompts = False
     event.start()
     buffer_connection.moler_connection.data_received(output.encode("utf-8"), datetime.datetime.now())
     ret = event.await_done(timeout=0.5)[0]
     assert event.done() is True
     assert 'list_matched' not in ret
+
+
```

### Comparing `moler-2.8.0/test/events/unix/test_event_ping_no_response.py` & `moler-2.9.0/test/events/unix/test_event_ping_no_response.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_event_awaiter.py` & `moler-2.9.0/test/test_event_awaiter.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_cmds_events_doc.py` & `moler-2.9.0/test/test_cmds_events_doc.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_connection.py` & `moler-2.9.0/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_command.py` & `moler-2.9.0/test/test_command.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_moler_test.py` & `moler-2.9.0/test/test_moler_test.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/test/test_runner.py` & `moler-2.9.0/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/setup.py` & `moler-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 with io.open(join(here, 'requirements.txt'), encoding='utf-8') as f:
     requires = f.read().splitlines()
 
 setup(
     name='moler',  # Required
-    version='2.8.0',  # Required
+    version='2.9.0',  # Required
     description='Moler is library to help in building automated tests',  # Required
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/nokia/moler',  # Optional
     author='Nokia',  # Optional
     license='BSD 3-Clause',
     classifiers=[  # Optional
```

### Comparing `moler-2.8.0/moler.egg-info/SOURCES.txt` & `moler-2.9.0/moler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 moler/__init__.py
 moler/abstract_moler_connection.py
 moler/asyncio_runner.py
 moler/command.py
```

### Comparing `moler-2.8.0/moler.egg-info/PKG-INFO` & `moler-2.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,577 +1,17 @@
 Metadata-Version: 2.1
 Name: moler
-Version: 2.8.0
+Version: 2.9.0
 Summary: Moler is library to help in building automated tests
 Home-page: https://github.com/nokia/moler
 Author: Nokia
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/nokia/moler/issues
 Project-URL: Source, https://github.com/nokia/moler
-Description: [![image](https://img.shields.io/badge/pypi-v2.8.0-blue.svg)](https://pypi.org/project/moler/)
-        [![image](https://img.shields.io/badge/python-2.7%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/moler/)
-        [![Build Status](https://travis-ci.org/nokia/moler.svg?branch=master)](https://travis-ci.org/nokia/moler)
-        [![Coverage Status](https://coveralls.io/repos/github/nokia/moler/badge.svg?branch=master)](https://coveralls.io/github/nokia/moler?branch=master)
-        [![BCH compliance](https://bettercodehub.com/edge/badge/nokia/moler?branch=master)](https://bettercodehub.com/)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/355afc9110f34d549b7c08c33961827c)](https://www.codacy.com/app/mplichta/moler?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nokia/moler&amp;utm_campaign=Badge_Grade)
-        [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
-        
-        # Table of Contents
-        1. [Changelog](#changelog)
-        2. [Moler info](#moler)
-        3. [Moler usage examples](#moler-usage-examples)
-        4. [API design reasoning](#api-design-reasoning)
-        5. [Designed API](#designed-api)
-        
-        # Changelog
-        View our [chronological list](./CHANGELOG.md) of user-facing changes, large and small, made to the Moler project.
-        
-        ![moler logo](https://i.imgur.com/mkPutdC.png)
-        # Moler
-        Moler ([name origin](https://github.com/nokia/moler/wiki#moler-name-origin)) is Python library
-        that provides "bricks" for building  automated tests.
-        All these "bricks" have clearly defined responsibilities, have similar API,
-        follow same construction pattern (so new ones are easy to create).
-        
-        Here they are:
-        * Commands as self-reliant object
-          * to allow for command triggering and parsing encapsulated in single object (lower maintenance cost)
-        * Event observers & callbacks (alarms are events example)
-          * to allow for online reaction (not offline postprocessing)
-        * Run observers/commands in the background
-          * to allow for test logic decomposition into multiple commands running in parallel
-          * to allow for handling unexpected system behavior (reboots, alarms)
-        * State machines -> automatic auto-connecting after dropped connection
-          * to increase framework auto-recovery and help in troubleshooting "what went wrong"
-        * Automatic logging of all connections towards devices used by tests
-          * to decrease investigation time by having logs focused on different parts of system under test
-        
-        # Moler usage examples
-        Let's see Moler in action. Here is hypothetical use case: "find PIDs of all python processes":
-        
-        ```python
-        
-            from moler.config import load_config
-            from moler.device.device import DeviceFactory
-        
-            load_config(config='my_devices.yml')                    # description of available devices
-            my_unix = DeviceFactory.get_device(name='MyMachine')    # take specific device out of available ones
-            ps_cmd = my_unix.get_cmd(cmd_name="ps",                 # take command of that device
-                                     cmd_params={"options": "-ef"})
-        
-            processes_info = ps_cmd()                               # run the command, it returns result
-            for proc_info in processes_info:
-                if 'python' in proc_info['CMD']:
-                    print("PID: {info[PID]} CMD: {info[CMD]}".format(info=proc_info))
-        ```
-        
-        * To have command we ask device "give me such command".
-        * To run command we just call it as function (command object is callable)
-        * What command returns is usually dict or list of dicts - easy to process
-        
-        Above code displays:
-        
-        ```bash
-        
-            PID: 1817 CMD: /usr/bin/python /usr/share/system-config-printer/applet.py
-            PID: 21825 CMD: /usr/bin/python /home/gl/moler/examples/command/unix_ps.py
-        ```
-        
-        How does it know what `'MyMachine'` means? Code loads definition from `my_devices.yml` configuration file:
-        
-        ```yaml
-        
-            DEVICES:
-        
-              MyMachine:
-                DEVICE_CLASS: moler.device.unixlocal.UnixLocal
-        
-              RebexTestMachine:
-                DEVICE_CLASS: moler.device.unixremote.UnixRemote
-                CONNECTION_HOPS:
-                  UNIX_LOCAL:                # from state
-                    UNIX_REMOTE:             # to state
-                      execute_command: ssh   # via command
-                      command_params:        # with params
-                        expected_prompt: demo@
-                        host: test.rebex.net
-                        login: demo
-                        password: password
-                        set_timeout: False   # remote doesn't support: export TMOUT
-        ```
-        
-        We have remote machine in our config. Let's check if there is 'readme.txt' file
-        on that machine (and some info about the file):
-        
-        ```python
-        
-            remote_unix = DeviceFactory.get_device(name='RebexTestMachine')  # it starts in local shell
-            remote_unix.goto_state(state="UNIX_REMOTE")                      # make it go to remote shell
-        
-            ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
-        
-            remote_files = ls_cmd()
-        
-            if 'readme.txt' in remote_files['files']:
-                print("readme.txt file:")
-                readme_file_info = remote_files['files']['readme.txt']
-                for attr in readme_file_info:
-                    print("  {:<18}: {}".format(attr, readme_file_info[attr]))
-        ```
-        
-        As you may noticed device is state machine. State transitions are defined inside
-        configuration file under `CONNECTION_HOPS`. Please note, that it is only config file who
-        knows "I need to use ssh to be on remote" - client code just says "go to remote".
-        Thanks to that you can exchange "how to reach remote" without any change in main code.
-        
-        Above code displays:
-        
-        ```bash
-        
-            readme.txt file:
-              permissions       : -rw-------
-              hard_links_count  : 1
-              owner             : demo
-              group             : users
-              size_raw          : 403
-              size_bytes        : 403
-              date              : Apr 08  2014
-              name              : readme.txt
-        ```
-        
-        How about doing multiple things in parallel. Let's ping google
-        while asking test.rebex.net about readme.txt file:
-        
-        ```python
-        my_unix = DeviceFactory.get_device(name='MyMachine')
-        host = 'www.google.com'
-        ping_cmd = my_unix.get_cmd(cmd_name="ping", cmd_params={"destination": host, "options": "-w 6"})
-        
-        remote_unix = DeviceFactory.get_device(name='RebexTestMachine')
-        remote_unix.goto_state(state="UNIX_REMOTE")
-        ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
-        
-        print("Start pinging {} ...".format(host))
-        ping_cmd.start()                                # run command in background
-        print("Let's check readme.txt at {} while pinging {} ...".format(remote_unix.name, host))
-        
-        remote_files = ls_cmd()                         # foreground "run in the meantime"
-        file_info = remote_files['files']['readme.txt']
-        print("readme.txt file: owner={fi[owner]}, size={fi[size_bytes]}".format(fi=file_info))
-        
-        ping_stats = ping_cmd.await_done(timeout=6)     # await background command
-        print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
-                                                  ping_stats['packet_loss'],
-                                                  'time_avg',
-                                                  ping_stats['time_avg'],
-                                                  ping_stats['time_unit']))
-        ```
-        
-        ```log
-        Start pinging www.google.com ...
-        Let's check readme.txt at RebexTestMachine while pinging www.google.com ...
-        readme.txt file: owner=demo, size=403
-        ping www.google.com: packet_loss=0, time_avg=35.251 [ms]
-        ```
-        
-        Besides being callable command-object works as "Future" (result promise).
-        You can start it in background and later await till it is done to grab result.
-        
-        If we enhance our configuration with logging related info:
-        
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-        ```
-        
-        then above code will automatically create Molers' main log (`moler.log`)
-        which shows activity on all devices:
-        
-        ```log
-        22:30:19.723 INFO       moler               |More logs in: ./logs
-        22:30:19.747 INFO       MyMachine           |Connection to: 'MyMachine' has been opened.
-        22:30:19.748 INFO       MyMachine           |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.866 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:19.901 INFO       RebexTestMachine    |Connection to: 'RebexTestMachine' has been opened.
-        22:30:19.901 INFO       RebexTestMachine    |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.919 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
-        22:30:19.920 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:19.921 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
-        22:30:19.921 INFO       RebexTestMachine    |TERM=xterm-mono ssh -l demo test.rebex.net
-        22:30:20.763 INFO       RebexTestMachine    |*********
-        22:30:20.909 INFO       RebexTestMachine    |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
-        22:30:20.917 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh' finished.
-        22:30:20.919 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
-        22:30:20.920 INFO       MyMachine           |ping www.google.com -w 6
-        22:30:20.920 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
-        22:30:20.922 INFO       RebexTestMachine    |ls -l
-        22:30:20.985 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls' finished.
-        22:30:26.968 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping' finished.
-        22:30:26.992 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        22:30:27.011 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
-        22:30:27.032 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        
-        ```
-        
-        As you may noticed main log shows code progress from high-level view - data
-        on connections are not visible, just activity of commands running on devices.
-        
-        If you want to see in details what has happened on each device - you have it in device logs.
-        Moler creates log per each device
-        `moler.RebexTestMachine.log`:
-        
-        ```log
-        22:30:19.901  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.902 <|
-        22:30:19.919  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
-        22:30:19.920  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:19.921  |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
-        22:30:19.921 >|TERM=xterm-mono ssh -l demo test.rebex.net
-        
-        22:30:19.924 <|TERM=xterm-mono ssh -l demo test.rebex.net
-        
-        22:30:20.762 <|Password:
-        22:30:20.763 >|*********
-        22:30:20.763 <|
-        
-        22:30:20.908 <|Welcome to Rebex Virtual Shell!
-                      |For a list of supported commands, type 'help'.
-                      |demo@ETNA:/$
-        22:30:20.909  |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
-        22:30:20.917  |Command 'moler.cmd.unix.ssh.Ssh' finished.
-        22:30:20.920  |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
-        22:30:20.922 >|ls -l
-        
-        22:30:20.974 <|ls -l
-        
-        22:30:20.978 <|drwx------ 2 demo users          0 Jul 26  2017 .
-        
-        22:30:20.979 <|drwx------ 2 demo users          0 Jul 26  2017 ..
-                      |drwx------ 2 demo users          0 Dec 03  2015 aspnet_client
-                      |drwx------ 2 demo users          0 Oct 27  2015 pub
-                      |-rw------- 1 demo users        403 Apr 08  2014 readme.txt
-                      |demo@ETNA:/$
-        22:30:20.985  |Command 'moler.cmd.unix.ls.Ls' finished.
-        22:30:26.992  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        22:30:27.011  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
-        ```
-        
-        and `moler.MyMachine.log`:
-        
-        ```log
-        22:30:19.748  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.748 <|
-        22:30:19.866  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:20.919  |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
-        22:30:20.920 >|ping www.google.com -w 6
-        
-        22:30:20.921 <|ping www.google.com -w 6
-        
-        22:30:20.959 <|PING www.google.com (216.58.215.68) 56(84) bytes of data.
-        22:30:20.960 <|
-        
-        22:30:21.000 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=1 ttl=51 time=40.1 ms
-        22:30:21.001 <|
-        
-        22:30:21.992 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=2 ttl=51 time=31.0 ms
-        
-        22:30:22.999 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=3 ttl=51 time=36.5 ms
-        
-        22:30:23.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=4 ttl=51 time=31.4 ms
-        
-        22:30:24.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=5 ttl=51 time=29.8 ms
-        
-        22:30:26.010 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=6 ttl=51 time=42.4 ms
-        
-        22:30:26.960 <|
-                      |--- www.google.com ping statistics ---
-                      |6 packets transmitted, 6 received, 0% packet loss, time 5007ms
-                      |rtt min/avg/max/mdev = 29.888/35.251/42.405/4.786 ms
-                      |moler_bash#
-        22:30:26.968  |Command 'moler.cmd.unix.ping.Ping' finished.
-        22:30:27.032  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        ```
-        
-        If the log files are too large you can split files.
-        
-        The log files can be split by size. For example let's assume we want split log files by 5 MB (5242880 bytes) and we want
-        to keep maximum 999 files:
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: size
-                INTERVAL: 5242880
-                BACKUP_COUNT: 999  # Default value
-              
-        
-        ```
-        
-        The log files can be split by time. For example let's assume we want split log files every 30 minutes (1800 seconds)
-         and we want to keep maximum 999 files (default value):
-         
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: time
-                INTERVAL: 1800
-                BACKUP_COUNT: 999  # Default value
-        ```
-        
-        For space saving Moler can compress the logs after rotation. The external tool is used. Let's use the above examples
-        to show how to compress logs:
-        
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: size
-                INTERVAL: 5242880
-                BACKUP_COUNT: 999  # Default value
-                COMPRESS_AFTER_ROTATION: True  # Default is False
-                COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value
-                COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
-        
-        
-        ```
-        
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: time
-                INTERVAL: 1800
-                BACKUP_COUNT: 999  # Default value
-                COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value      
-                COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
-        ```
-        
-        In a script we can also disable logging from device. Please use it very carefully. Investigation any issue may be
-         impossible if we don't have full logs.
-         
-        ```python
-        my_unix = DeviceFactory.get_device(name='MyMachine')
-        
-        my_unix.disbale_logging()  # to disable logging on device
-        
-        my_unix.enable_logging()  # to enable logging on device
-        ```
-        
-        In a script you can add suffix to all log files or only to files for specific devices. with disable logging from device. 
-         
-        ```python
-        from moler.config.loggers import change_logging_suffix
-        change_logging_suffix(".suffix1")  # all log files with suffix
-        change_logging_suffix(None)  # all log files without suffx
-        
-        my_unix = DeviceFactory.get_device(name='MyMachine')
-        
-        my_unix.set_logging_suffix("device_suffix")  # to add suffix to filename with logs
-        
-        my_unix.set_suffix(None)  # to remove suffix from filename with logs
-        ```
-        
-        Previous examples ask device to create command. We can also create command ourselves
-        giving it connection to operate on:
-        
-        ```python
-        
-            import time
-            from moler.cmd.unix.ping import Ping
-            from moler.connection_factory import get_connection
-        
-            host = 'www.google.com'
-            terminal = get_connection(io_type='terminal', variant='threaded')  # take connection
-            with terminal.open():
-                ping_cmd = Ping(connection=terminal.moler_connection,
-                                destination=host, options="-w 6")
-                print("Start pinging {} ...".format(host))
-                ping_cmd.start()
-                print("Doing other stuff while pinging {} ...".format(host))
-                time.sleep(3)
-                ping_stats = ping_cmd.await_done(timeout=4)
-                print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
-                                                          ping_stats['packet_loss'],
-                                                          'time_avg',
-                                                          ping_stats['time_avg'],
-                                                          ping_stats['time_unit']))
-        ```
-        
-        Please note also that connection is context manager doing open/close actions.
-        
-        
-        ```bash
-        
-            Start pinging www.google.com ...
-            Doing other stuff while pinging www.google.com ...
-            ping www.google.com: packet_loss=0, time_avg=50.000 [ms]
-        ```
-        
-        ## Reuse freedom
-        Library gives you freedom which part you want to reuse. We are fan's of "take what you need only".
-        * You may use configuration files or configure things by Python calls.
-        
-           ```python
-           load_config(config={'DEVICES': {'MyMachine': {'DEVICE_CLASS': 'moler.device.unixlocal.UnixLocal'}}})
-           ```
-        * You may use devices or create commands manually
-        * You can take connection or build it yourself:
-        
-           ```python
-           from moler.threaded_moler_connection import ThreadedMolerConnection
-           from moler.io.raw.terminal import ThreadedTerminal
-        
-           terminal_connection = ThreadedTerminal(moler_connection=ThreadedMolerConnection())
-           ```
-        * You can even install your own implementation in place of default implementation per connection type
-        
-        # API design reasoning
-        The main goal of command is its usage simplicity: just run it and give me back its result.
-        
-        Command hides from its caller:
-        * a way how it realizes "runs"
-        * how it gets data of output to be parsed
-        * how it parses that data
-        
-        Command shows to its caller:
-        * API to start/stop it or await for its completion
-        * API to query for its result or result readiness
-        
-        Command works as [Futures and promises](https://en.wikipedia.org/wiki/Futures_and_promises)
-        
-        After starting, we await for its result which is parsed out command output provided usually as dict.
-        Running that command and parsing its output may take some time, so till that point result computation is yet incomplete.
-        
-        ## Command as future
-        * it starts some command on device/shell over connection
-          (as future-function starts it's execution)
-        * it parses data incoming over such connection
-          (as future-function does it's processing)
-        * it stores result of that parsing
-          (as future-function concludes in calculation result)
-        * it provides means to return that result
-          (as future-function does via 'return' or 'yield' statement)
-        * it's result is not ready "just-after" calling command
-          (as it is with future in contrast to function)
-        
-        So command should have future API.
-        
-        Quote from **_"Professional Python"_** by **Luke Sneeringer**:
-        > The Future is a standalone object. It is independent of the actual function that is running.
-        > It does nothing but store the state and result information.
-        
-        Command differs in that it is both:
-        * function-like object performing computation
-        * future-like object storing result of that computation.
-        
-        ## Command vs. Connection-observer
-        Command is just "active version" of connection observer.
-        
-        Connection observer is passive since it just observes connection for some data;
-        data that may just asynchronously appear (alarms, reboots or anything you want).
-        Intention here is split of responsibility: one observer is looking for alarms,
-        another one for reboots.
-        
-        Command is active since it actively triggers some output on connection
-        by sending command-string over that connection. So, it activates some action
-        on device-behind-connection. That action is "command" in device terminology.
-        Like `ping` on bash console/device. And it produces that "command" output.
-        That output is what Moler's Command as connection-observer is looking for.
-        
-        ## Most well known Python's futures
-        * [concurrent.futures.Future](https://docs.python.org/3/library/concurrent.futures.html)
-        * [asyncio.Future](https://docs.python.org/3/library/asyncio-task.html#future)
-        
-        | API                     | concurrent.futures.Future                   | asyncio.Future                                      |
-        | :---------------------- | :------------------------------------------ | :-------------------------------------------------- |
-        | storing result          | :white_check_mark: `set_result()`           | :white_check_mark: `set_result()`                   |
-        | result retrieval        | :white_check_mark: `result()`               | :white_check_mark: `result()`                       |
-        | storing failure cause   | :white_check_mark: `set_exception()`        | :white_check_mark: `set_exception()`                |
-        | failure cause retrieval | :white_check_mark: `exception()`            | :white_check_mark: `exception()`                    |
-        | stopping                | :white_check_mark: `cancel()`               | :white_check_mark: `cancel()`                       |
-        | check if stopped        | :white_check_mark: `cancelled()`            | :white_check_mark: `cancelled()`                    |
-        | check if running        | :white_check_mark: `running()`              | :no_entry_sign: `(but AbstractEventLoop.running())` |
-        | check if completed      | :white_check_mark: `done()`                 | :white_check_mark: `done()`                         |
-        | subscribe completion    | :white_check_mark: `add_done_callback()`    | :white_check_mark: `add_done_callback()`            |
-        | unsubscribe completion  | :no_entry_sign:                             | :white_check_mark: `remove_done_callback()`         |
-        
-        Starting callable to be run "as future" is done by entities external to future-object
-        
-        | API              | concurrent.futures<br>start via Executor objects (thread/proc) | asyncio<br>start via module-lvl functions or ev-loop |
-        | ---------------- | ---------------------------------------- | ---------------------------------------------- |
-        | start callable   | submit(fn, *args, **kwargs)<br>Schedules callable to be executed as<br>fn(*args **kwargs) -> Future | ensure_future(coro_or_future) -> Task<br>future = run_coroutine_threadsafe(coro, loop) |
-        | start same callable<br>on data iterator | map(fn, *iterables, timeout) -> iterator | join_future = asyncio.gather(*map(f, iterable))<br>loop.run_until_complete(join_future)|
-        
-        Awaiting completion of future is done by entities external to future-object
-        
-        | API               | concurrent.futures<br>awaiting by module level functions | asyncio<br>awaiting by module-lvl functions or ev-loop |
-        | ----------------- | ------------------------------------------ | -------------------------------------------- |
-        | await completion  |  done, not_done = wait(futures, timeout) -> futures | done, not_done = await wait(futures)<br>results = await gather(futures)<br>result = await future<br>result = yield from future<br>result = await coroutine<br>result = yield from coroutine<br>result = yield from wait_for(future, timeout)<br>loop.run_until_complete(future) -> blocking run |
-        | process as they<br>complete | for done in as_completed(futures, timeout) -> futures | for done in as_completed(futures, timeout) -> futures |
-        
-        ## Fundamental difference of command
-        Contrary to **concurrent.futures** and **asyncio** we don't want command to be run by some external entity.
-        We want it to be self-executable for usage simplicity.
-        We want to take command and just say to it:
-        * **"run"** or **"run in background"**
-        * and not **"Hi, external runner, would you run/run-background that command for me"**
-        
-        # Designed API
-        1. create command object
-        ``` python
-        command = Command()
-        ```
-        
-        2. run it synchronously/blocking and get result in one shot behaves like function call since Command is callable.
-        
-        Run-as-callable gives big advantage since it fits well in python ecosystem.
-        ``` python
-        result = command()
-        ```
-        function example:
-        ``` python
-        map(ping_cmd, all_machines_to_validate_reachability)
-        ```
-        
-        3. run it asynchronously/nonblocking
-        ``` python
-        command_as_future = command.start()
-        ```
-        
-        4. shift from background to foreground
-        
-        **asyncio:** variant looks like:
-        ``` python
-        result = await future
-        done_futures, pending = yield from asyncio.wait(futures)
-        result = yield from asyncio.wait_for(future, 60.0)
-        ```
-        and **concurrent.futures** variant looks like:
-        ``` python
-        done_futures, pending = wait(futures)
-        ```
-        Moler's API maps to above well-known API
-        ``` python
-        result = command.await_done(timeout)
-        ```
-        * it is "internal" to command "Hi command, that is what I want from you" (above APIs say "Hi you there, that is what I want you to do with command")
-        * it directly (Zen of Python) shows what we are awaiting for
-        * timeout is required parameter (not as in concurrent.futures) since we don't expect endless execution of command (user must know what is worst case timeout to await command completion)
-        
-        # Video introduction
-        You can [watch videos how to use Moler on YouTube](https://www.youtube.com/channel/UCgToo2qq8kLMyEgzd4btM9g). 
-        
 Keywords: testing development
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
@@ -585,7 +25,567 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![image](https://img.shields.io/badge/pypi-v2.9.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/python-2.7%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/moler/)
+[![Build Status](https://travis-ci.org/nokia/moler.svg?branch=master)](https://travis-ci.org/nokia/moler)
+[![Coverage Status](https://coveralls.io/repos/github/nokia/moler/badge.svg?branch=master)](https://coveralls.io/github/nokia/moler?branch=master)
+[![BCH compliance](https://bettercodehub.com/edge/badge/nokia/moler?branch=master)](https://bettercodehub.com/)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/355afc9110f34d549b7c08c33961827c)](https://www.codacy.com/app/mplichta/moler?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nokia/moler&amp;utm_campaign=Badge_Grade)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
+
+# Table of Contents
+1. [Changelog](#changelog)
+2. [Moler info](#moler)
+3. [Moler usage examples](#moler-usage-examples)
+4. [API design reasoning](#api-design-reasoning)
+5. [Designed API](#designed-api)
+
+# Changelog
+View our [chronological list](./CHANGELOG.md) of user-facing changes, large and small, made to the Moler project.
+
+![moler logo](https://i.imgur.com/mkPutdC.png)
+# Moler
+Moler ([name origin](https://github.com/nokia/moler/wiki#moler-name-origin)) is Python library
+that provides "bricks" for building  automated tests.
+All these "bricks" have clearly defined responsibilities, have similar API,
+follow same construction pattern (so new ones are easy to create).
+
+Here they are:
+* Commands as self-reliant object
+  * to allow for command triggering and parsing encapsulated in single object (lower maintenance cost)
+* Event observers & callbacks (alarms are events example)
+  * to allow for online reaction (not offline postprocessing)
+* Run observers/commands in the background
+  * to allow for test logic decomposition into multiple commands running in parallel
+  * to allow for handling unexpected system behavior (reboots, alarms)
+* State machines -> automatic auto-connecting after dropped connection
+  * to increase framework auto-recovery and help in troubleshooting "what went wrong"
+* Automatic logging of all connections towards devices used by tests
+  * to decrease investigation time by having logs focused on different parts of system under test
+
+# Moler usage examples
+Let's see Moler in action. Here is hypothetical use case: "find PIDs of all python processes":
+
+```python
+
+    from moler.config import load_config
+    from moler.device.device import DeviceFactory
+
+    load_config(config='my_devices.yml')                    # description of available devices
+    my_unix = DeviceFactory.get_device(name='MyMachine')    # take specific device out of available ones
+    ps_cmd = my_unix.get_cmd(cmd_name="ps",                 # take command of that device
+                             cmd_params={"options": "-ef"})
+
+    processes_info = ps_cmd()                               # run the command, it returns result
+    for proc_info in processes_info:
+        if 'python' in proc_info['CMD']:
+            print("PID: {info[PID]} CMD: {info[CMD]}".format(info=proc_info))
+```
+
+* To have command we ask device "give me such command".
+* To run command we just call it as function (command object is callable)
+* What command returns is usually dict or list of dicts - easy to process
+
+Above code displays:
+
+```bash
+
+    PID: 1817 CMD: /usr/bin/python /usr/share/system-config-printer/applet.py
+    PID: 21825 CMD: /usr/bin/python /home/gl/moler/examples/command/unix_ps.py
+```
+
+How does it know what `'MyMachine'` means? Code loads definition from `my_devices.yml` configuration file:
+
+```yaml
+
+    DEVICES:
+
+      MyMachine:
+        DEVICE_CLASS: moler.device.unixlocal.UnixLocal
+
+      RebexTestMachine:
+        DEVICE_CLASS: moler.device.unixremote.UnixRemote
+        CONNECTION_HOPS:
+          UNIX_LOCAL:                # from state
+            UNIX_REMOTE:             # to state
+              execute_command: ssh   # via command
+              command_params:        # with params
+                expected_prompt: demo@
+                host: test.rebex.net
+                login: demo
+                password: password
+                set_timeout: False   # remote doesn't support: export TMOUT
+```
+
+We have remote machine in our config. Let's check if there is 'readme.txt' file
+on that machine (and some info about the file):
+
+```python
+
+    remote_unix = DeviceFactory.get_device(name='RebexTestMachine')  # it starts in local shell
+    remote_unix.goto_state(state="UNIX_REMOTE")                      # make it go to remote shell
+
+    ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
+
+    remote_files = ls_cmd()
+
+    if 'readme.txt' in remote_files['files']:
+        print("readme.txt file:")
+        readme_file_info = remote_files['files']['readme.txt']
+        for attr in readme_file_info:
+            print("  {:<18}: {}".format(attr, readme_file_info[attr]))
+```
+
+As you may noticed device is state machine. State transitions are defined inside
+configuration file under `CONNECTION_HOPS`. Please note, that it is only config file who
+knows "I need to use ssh to be on remote" - client code just says "go to remote".
+Thanks to that you can exchange "how to reach remote" without any change in main code.
+
+Above code displays:
+
+```bash
+
+    readme.txt file:
+      permissions       : -rw-------
+      hard_links_count  : 1
+      owner             : demo
+      group             : users
+      size_raw          : 403
+      size_bytes        : 403
+      date              : Apr 08  2014
+      name              : readme.txt
+```
+
+How about doing multiple things in parallel. Let's ping google
+while asking test.rebex.net about readme.txt file:
+
+```python
+my_unix = DeviceFactory.get_device(name='MyMachine')
+host = 'www.google.com'
+ping_cmd = my_unix.get_cmd(cmd_name="ping", cmd_params={"destination": host, "options": "-w 6"})
+
+remote_unix = DeviceFactory.get_device(name='RebexTestMachine')
+remote_unix.goto_state(state="UNIX_REMOTE")
+ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
+
+print("Start pinging {} ...".format(host))
+ping_cmd.start()                                # run command in background
+print("Let's check readme.txt at {} while pinging {} ...".format(remote_unix.name, host))
+
+remote_files = ls_cmd()                         # foreground "run in the meantime"
+file_info = remote_files['files']['readme.txt']
+print("readme.txt file: owner={fi[owner]}, size={fi[size_bytes]}".format(fi=file_info))
+
+ping_stats = ping_cmd.await_done(timeout=6)     # await background command
+print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
+                                          ping_stats['packet_loss'],
+                                          'time_avg',
+                                          ping_stats['time_avg'],
+                                          ping_stats['time_unit']))
+```
+
+```log
+Start pinging www.google.com ...
+Let's check readme.txt at RebexTestMachine while pinging www.google.com ...
+readme.txt file: owner=demo, size=403
+ping www.google.com: packet_loss=0, time_avg=35.251 [ms]
+```
+
+Besides being callable command-object works as "Future" (result promise).
+You can start it in background and later await till it is done to grab result.
+
+If we enhance our configuration with logging related info:
+
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+```
+
+then above code will automatically create Molers' main log (`moler.log`)
+which shows activity on all devices:
+
+```log
+22:30:19.723 INFO       moler               |More logs in: ./logs
+22:30:19.747 INFO       MyMachine           |Connection to: 'MyMachine' has been opened.
+22:30:19.748 INFO       MyMachine           |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.866 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:19.901 INFO       RebexTestMachine    |Connection to: 'RebexTestMachine' has been opened.
+22:30:19.901 INFO       RebexTestMachine    |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.919 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
+22:30:19.920 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:19.921 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
+22:30:19.921 INFO       RebexTestMachine    |TERM=xterm-mono ssh -l demo test.rebex.net
+22:30:20.763 INFO       RebexTestMachine    |*********
+22:30:20.909 INFO       RebexTestMachine    |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
+22:30:20.917 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh' finished.
+22:30:20.919 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
+22:30:20.920 INFO       MyMachine           |ping www.google.com -w 6
+22:30:20.920 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
+22:30:20.922 INFO       RebexTestMachine    |ls -l
+22:30:20.985 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls' finished.
+22:30:26.968 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping' finished.
+22:30:26.992 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+22:30:27.011 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
+22:30:27.032 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+
+```
+
+As you may noticed main log shows code progress from high-level view - data
+on connections are not visible, just activity of commands running on devices.
+
+If you want to see in details what has happened on each device - you have it in device logs.
+Moler creates log per each device
+`moler.RebexTestMachine.log`:
+
+```log
+22:30:19.901  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.902 <|
+22:30:19.919  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
+22:30:19.920  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:19.921  |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
+22:30:19.921 >|TERM=xterm-mono ssh -l demo test.rebex.net
+
+22:30:19.924 <|TERM=xterm-mono ssh -l demo test.rebex.net
+
+22:30:20.762 <|Password:
+22:30:20.763 >|*********
+22:30:20.763 <|
+
+22:30:20.908 <|Welcome to Rebex Virtual Shell!
+              |For a list of supported commands, type 'help'.
+              |demo@ETNA:/$
+22:30:20.909  |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
+22:30:20.917  |Command 'moler.cmd.unix.ssh.Ssh' finished.
+22:30:20.920  |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
+22:30:20.922 >|ls -l
+
+22:30:20.974 <|ls -l
+
+22:30:20.978 <|drwx------ 2 demo users          0 Jul 26  2017 .
+
+22:30:20.979 <|drwx------ 2 demo users          0 Jul 26  2017 ..
+              |drwx------ 2 demo users          0 Dec 03  2015 aspnet_client
+              |drwx------ 2 demo users          0 Oct 27  2015 pub
+              |-rw------- 1 demo users        403 Apr 08  2014 readme.txt
+              |demo@ETNA:/$
+22:30:20.985  |Command 'moler.cmd.unix.ls.Ls' finished.
+22:30:26.992  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+22:30:27.011  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
+```
+
+and `moler.MyMachine.log`:
+
+```log
+22:30:19.748  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.748 <|
+22:30:19.866  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:20.919  |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
+22:30:20.920 >|ping www.google.com -w 6
+
+22:30:20.921 <|ping www.google.com -w 6
+
+22:30:20.959 <|PING www.google.com (216.58.215.68) 56(84) bytes of data.
+22:30:20.960 <|
+
+22:30:21.000 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=1 ttl=51 time=40.1 ms
+22:30:21.001 <|
+
+22:30:21.992 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=2 ttl=51 time=31.0 ms
+
+22:30:22.999 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=3 ttl=51 time=36.5 ms
+
+22:30:23.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=4 ttl=51 time=31.4 ms
+
+22:30:24.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=5 ttl=51 time=29.8 ms
+
+22:30:26.010 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=6 ttl=51 time=42.4 ms
+
+22:30:26.960 <|
+              |--- www.google.com ping statistics ---
+              |6 packets transmitted, 6 received, 0% packet loss, time 5007ms
+              |rtt min/avg/max/mdev = 29.888/35.251/42.405/4.786 ms
+              |moler_bash#
+22:30:26.968  |Command 'moler.cmd.unix.ping.Ping' finished.
+22:30:27.032  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+```
+
+If the log files are too large you can split files.
+
+The log files can be split by size. For example let's assume we want split log files by 5 MB (5242880 bytes) and we want
+to keep maximum 999 files:
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: size
+        INTERVAL: 5242880
+        BACKUP_COUNT: 999  # Default value
+      
+
+```
+
+The log files can be split by time. For example let's assume we want split log files every 30 minutes (1800 seconds)
+ and we want to keep maximum 999 files (default value):
+ 
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: time
+        INTERVAL: 1800
+        BACKUP_COUNT: 999  # Default value
+```
+
+For space saving Moler can compress the logs after rotation. The external tool is used. Let's use the above examples
+to show how to compress logs:
+
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: size
+        INTERVAL: 5242880
+        BACKUP_COUNT: 999  # Default value
+        COMPRESS_AFTER_ROTATION: True  # Default is False
+        COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value
+        COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
+
+
+```
+
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: time
+        INTERVAL: 1800
+        BACKUP_COUNT: 999  # Default value
+        COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value      
+        COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
+```
+
+In a script we can also disable logging from device. Please use it very carefully. Investigation any issue may be
+ impossible if we don't have full logs.
+ 
+```python
+my_unix = DeviceFactory.get_device(name='MyMachine')
+
+my_unix.disbale_logging()  # to disable logging on device
+
+my_unix.enable_logging()  # to enable logging on device
+```
+
+In a script you can add suffix to all log files or only to files for specific devices. with disable logging from device. 
+ 
+```python
+from moler.config.loggers import change_logging_suffix
+change_logging_suffix(".suffix1")  # all log files with suffix
+change_logging_suffix(None)  # all log files without suffx
+
+my_unix = DeviceFactory.get_device(name='MyMachine')
+
+my_unix.set_logging_suffix("device_suffix")  # to add suffix to filename with logs
+
+my_unix.set_suffix(None)  # to remove suffix from filename with logs
+```
+
+Previous examples ask device to create command. We can also create command ourselves
+giving it connection to operate on:
+
+```python
+
+    import time
+    from moler.cmd.unix.ping import Ping
+    from moler.connection_factory import get_connection
+
+    host = 'www.google.com'
+    terminal = get_connection(io_type='terminal', variant='threaded')  # take connection
+    with terminal.open():
+        ping_cmd = Ping(connection=terminal.moler_connection,
+                        destination=host, options="-w 6")
+        print("Start pinging {} ...".format(host))
+        ping_cmd.start()
+        print("Doing other stuff while pinging {} ...".format(host))
+        time.sleep(3)
+        ping_stats = ping_cmd.await_done(timeout=4)
+        print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
+                                                  ping_stats['packet_loss'],
+                                                  'time_avg',
+                                                  ping_stats['time_avg'],
+                                                  ping_stats['time_unit']))
+```
+
+Please note also that connection is context manager doing open/close actions.
+
+
+```bash
+
+    Start pinging www.google.com ...
+    Doing other stuff while pinging www.google.com ...
+    ping www.google.com: packet_loss=0, time_avg=50.000 [ms]
+```
+
+## Reuse freedom
+Library gives you freedom which part you want to reuse. We are fan's of "take what you need only".
+* You may use configuration files or configure things by Python calls.
+
+   ```python
+   load_config(config={'DEVICES': {'MyMachine': {'DEVICE_CLASS': 'moler.device.unixlocal.UnixLocal'}}})
+   ```
+* You may use devices or create commands manually
+* You can take connection or build it yourself:
+
+   ```python
+   from moler.threaded_moler_connection import ThreadedMolerConnection
+   from moler.io.raw.terminal import ThreadedTerminal
+
+   terminal_connection = ThreadedTerminal(moler_connection=ThreadedMolerConnection())
+   ```
+* You can even install your own implementation in place of default implementation per connection type
+
+# API design reasoning
+The main goal of command is its usage simplicity: just run it and give me back its result.
+
+Command hides from its caller:
+* a way how it realizes "runs"
+* how it gets data of output to be parsed
+* how it parses that data
+
+Command shows to its caller:
+* API to start/stop it or await for its completion
+* API to query for its result or result readiness
+
+Command works as [Futures and promises](https://en.wikipedia.org/wiki/Futures_and_promises)
+
+After starting, we await for its result which is parsed out command output provided usually as dict.
+Running that command and parsing its output may take some time, so till that point result computation is yet incomplete.
+
+## Command as future
+* it starts some command on device/shell over connection
+  (as future-function starts it's execution)
+* it parses data incoming over such connection
+  (as future-function does it's processing)
+* it stores result of that parsing
+  (as future-function concludes in calculation result)
+* it provides means to return that result
+  (as future-function does via 'return' or 'yield' statement)
+* it's result is not ready "just-after" calling command
+  (as it is with future in contrast to function)
+
+So command should have future API.
+
+Quote from **_"Professional Python"_** by **Luke Sneeringer**:
+> The Future is a standalone object. It is independent of the actual function that is running.
+> It does nothing but store the state and result information.
+
+Command differs in that it is both:
+* function-like object performing computation
+* future-like object storing result of that computation.
+
+## Command vs. Connection-observer
+Command is just "active version" of connection observer.
+
+Connection observer is passive since it just observes connection for some data;
+data that may just asynchronously appear (alarms, reboots or anything you want).
+Intention here is split of responsibility: one observer is looking for alarms,
+another one for reboots.
+
+Command is active since it actively triggers some output on connection
+by sending command-string over that connection. So, it activates some action
+on device-behind-connection. That action is "command" in device terminology.
+Like `ping` on bash console/device. And it produces that "command" output.
+That output is what Moler's Command as connection-observer is looking for.
+
+## Most well known Python's futures
+* [concurrent.futures.Future](https://docs.python.org/3/library/concurrent.futures.html)
+* [asyncio.Future](https://docs.python.org/3/library/asyncio-task.html#future)
+
+| API                     | concurrent.futures.Future                   | asyncio.Future                                      |
+| :---------------------- | :------------------------------------------ | :-------------------------------------------------- |
+| storing result          | :white_check_mark: `set_result()`           | :white_check_mark: `set_result()`                   |
+| result retrieval        | :white_check_mark: `result()`               | :white_check_mark: `result()`                       |
+| storing failure cause   | :white_check_mark: `set_exception()`        | :white_check_mark: `set_exception()`                |
+| failure cause retrieval | :white_check_mark: `exception()`            | :white_check_mark: `exception()`                    |
+| stopping                | :white_check_mark: `cancel()`               | :white_check_mark: `cancel()`                       |
+| check if stopped        | :white_check_mark: `cancelled()`            | :white_check_mark: `cancelled()`                    |
+| check if running        | :white_check_mark: `running()`              | :no_entry_sign: `(but AbstractEventLoop.running())` |
+| check if completed      | :white_check_mark: `done()`                 | :white_check_mark: `done()`                         |
+| subscribe completion    | :white_check_mark: `add_done_callback()`    | :white_check_mark: `add_done_callback()`            |
+| unsubscribe completion  | :no_entry_sign:                             | :white_check_mark: `remove_done_callback()`         |
+
+Starting callable to be run "as future" is done by entities external to future-object
+
+| API              | concurrent.futures<br>start via Executor objects (thread/proc) | asyncio<br>start via module-lvl functions or ev-loop |
+| ---------------- | ---------------------------------------- | ---------------------------------------------- |
+| start callable   | submit(fn, *args, **kwargs)<br>Schedules callable to be executed as<br>fn(*args **kwargs) -> Future | ensure_future(coro_or_future) -> Task<br>future = run_coroutine_threadsafe(coro, loop) |
+| start same callable<br>on data iterator | map(fn, *iterables, timeout) -> iterator | join_future = asyncio.gather(*map(f, iterable))<br>loop.run_until_complete(join_future)|
+
+Awaiting completion of future is done by entities external to future-object
+
+| API               | concurrent.futures<br>awaiting by module level functions | asyncio<br>awaiting by module-lvl functions or ev-loop |
+| ----------------- | ------------------------------------------ | -------------------------------------------- |
+| await completion  |  done, not_done = wait(futures, timeout) -> futures | done, not_done = await wait(futures)<br>results = await gather(futures)<br>result = await future<br>result = yield from future<br>result = await coroutine<br>result = yield from coroutine<br>result = yield from wait_for(future, timeout)<br>loop.run_until_complete(future) -> blocking run |
+| process as they<br>complete | for done in as_completed(futures, timeout) -> futures | for done in as_completed(futures, timeout) -> futures |
+
+## Fundamental difference of command
+Contrary to **concurrent.futures** and **asyncio** we don't want command to be run by some external entity.
+We want it to be self-executable for usage simplicity.
+We want to take command and just say to it:
+* **"run"** or **"run in background"**
+* and not **"Hi, external runner, would you run/run-background that command for me"**
+
+# Designed API
+1. create command object
+``` python
+command = Command()
+```
+
+2. run it synchronously/blocking and get result in one shot behaves like function call since Command is callable.
+
+Run-as-callable gives big advantage since it fits well in python ecosystem.
+``` python
+result = command()
+```
+function example:
+``` python
+map(ping_cmd, all_machines_to_validate_reachability)
+```
+
+3. run it asynchronously/nonblocking
+``` python
+command_as_future = command.start()
+```
+
+4. shift from background to foreground
+
+**asyncio:** variant looks like:
+``` python
+result = await future
+done_futures, pending = yield from asyncio.wait(futures)
+result = yield from asyncio.wait_for(future, 60.0)
+```
+and **concurrent.futures** variant looks like:
+``` python
+done_futures, pending = wait(futures)
+```
+Moler's API maps to above well-known API
+``` python
+result = command.await_done(timeout)
+```
+* it is "internal" to command "Hi command, that is what I want from you" (above APIs say "Hi you there, that is what I want you to do with command")
+* it directly (Zen of Python) shows what we are awaiting for
+* timeout is required parameter (not as in concurrent.futures) since we don't expect endless execution of command (user must know what is worst case timeout to await command completion)
+
+# Video introduction
+You can [watch videos how to use Moler on YouTube](https://www.youtube.com/channel/UCgToo2qq8kLMyEgzd4btM9g).
```

### Comparing `moler-2.8.0/moler/event.py` & `moler-2.9.0/moler/event.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/exceptions.py` & `moler-2.9.0/moler/exceptions.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/runner_single_thread.py` & `moler-2.9.0/moler/runner_single_thread.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/adbremote.py` & `moler-2.9.0/moler/device/adbremote.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/state_machine.py` & `moler-2.9.0/moler/device/state_machine.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/unixlocal.py` & `moler-2.9.0/moler/device/unixlocal.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/adbremote2.py` & `moler-2.9.0/moler/device/adbremote2.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/junipergeneric.py` & `moler-2.9.0/moler/device/junipergeneric.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/proxy_pc2.py` & `moler-2.9.0/moler/device/proxy_pc2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Moler's device has 2 main responsibilities:
 - be the factory that returns commands of that device
 - be the state machine that controls which commands may run in given state
 """
 
 __author__ = 'Michal Ernst, Grzegorz Latuszek'
-__copyright__ = 'Copyright (C) 2018-2020, Nokia'
+__copyright__ = 'Copyright (C) 2018-2023, Nokia'
 __email__ = 'michal.ernst@nokia.com, grzegorz.latuszek@nokia.com'
 import six
 import abc
 import platform
 
 from moler.device.textualdevice import TextualDevice
 from moler.device.unixlocal import UnixLocal
@@ -75,15 +75,15 @@
         self._after_open_prompt_detector = None
         self._warn_about_temporary_life_of_class()
 
     def _warn_about_temporary_life_of_class(self):
         what = "experimental/temporary implementation of device utilizing sshshell connection"
         temporary_classname = self.__class__.__name__
         target_classname = temporary_classname[:-1]
-        merge_info = "It's functionality will be merged"
+        merge_info = "Its functionality will be merged"
         future_change = "{} into {} device in Moler 2.0.0 and {} will be removed".format(merge_info,
                                                                                          target_classname,
                                                                                          temporary_classname)
         warn_msg = "Class {} is an {}. {}.".format(temporary_classname, what, future_change)
         self.logger.warning(warn_msg)
 
     def _should_use_proxy_pc(self, sm_params, proxy):
@@ -253,22 +253,26 @@
         self._after_open_prompt_detector = Wait4(detect_patterns=[r'^(.+)echo DETECTING PROMPT'],
                                                  connection=self.io_connection.moler_connection,
                                                  till_occurs_times=1)
         detector = self._after_open_prompt_detector
         detector.add_event_occurred_callback(callback=set_callback,
                                              callback_params={"event": detector})
         self.io_connection.moler_connection.sendline("echo DETECTING PROMPT")
-        self._after_open_prompt_detector.start(timeout=self._prompt_detector_timeout)
+        detector.start(timeout=self._prompt_detector_timeout)
+        # detector.await_done(timeout=self._prompt_detector_timeout)
 
     def _set_after_open_prompt(self, event):
         occurrence = event.get_last_occurrence()
-        prompt = occurrence['groups'][0]
+        prompt = occurrence['groups'][0].rstrip()
         state = self._get_current_state()
         with self._state_prompts_lock:
-            self._state_prompts[state] = prompt.rstrip()
+            self._state_prompts[state] = prompt
+            self._prepare_reverse_state_prompts_dict()
+            if self._prompts_event is not None:
+                self._prompts_event.change_prompts(prompts=self._reverse_state_prompts_dict)
 
     def _prepare_state_prompts(self):
         """
         Prepare textual prompt for each state.
         :return: Nothing.
         """
         if self._use_local_unix_state:
```

### Comparing `moler-2.8.0/moler/device/abstract_device.py` & `moler-2.9.0/moler/device/abstract_device.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/textualdevice.py` & `moler-2.9.0/moler/device/textualdevice.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/proxy_pc.py` & `moler-2.9.0/moler/device/proxy_pc.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/device.py` & `moler-2.9.0/moler/device/device.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/atremote.py` & `moler-2.9.0/moler/device/atremote.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/pdu_aten.py` & `moler-2.9.0/moler/device/pdu_aten.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/juniper_ex.py` & `moler-2.9.0/moler/device/juniper_ex.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/scpi.py` & `moler-2.9.0/moler/device/scpi.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/unixremote2.py` & `moler-2.9.0/moler/device/unixremote2.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/device/unixremote.py` & `moler-2.9.0/moler/device/unixremote.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/asyncio_runner.py` & `moler-2.9.0/moler/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/moler_connection_for_single_thread_runner.py` & `moler-2.9.0/moler/moler_connection_for_single_thread_runner.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/scheduler.py` & `moler-2.9.0/moler/scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/instance_loader.py` & `moler-2.9.0/moler/instance_loader.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/converterhelper.py` & `moler-2.9.0/moler/util/converterhelper.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/compressed_rotating_file_handler.py` & `moler-2.9.0/moler/util/compressed_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/moler_serial_proxy.py` & `moler-2.9.0/moler/util/moler_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/loghelper.py` & `moler-2.9.0/moler/util/loghelper.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/connection_observer_life_status.py` & `moler-2.9.0/moler/util/connection_observer_life_status.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/connection_observer.py` & `moler-2.9.0/moler/util/connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/devices_SM.py` & `moler-2.9.0/moler/util/devices_SM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Perform devices SM autotest.
 """
 
 __author__ = 'Michal Ernst, Marcin Usielski'
-__copyright__ = 'Copyright (C) 2019-2022, Nokia'
+__copyright__ = 'Copyright (C) 2019-2023, Nokia'
 __email__ = 'michal.ernst@nokia.com, marcin.usielski@nokia.com'
 
 import os
 import random
 import time
 import math
 import threading
@@ -219,15 +219,15 @@
         except KeyError as exc:
             if self.send_last_prompt_on_error and (cmd_data_string == "\x03"):  # ctrl+c
                 self.inject([self.input_bytes + self._last_prompt])
                 return
             try:
                 available_outputs = self.data[self.device.state].keys()
             except (KeyError, AttributeError):
-                available_outputs = "No output for state '{}'. Data: '{}'.".format(self.device.stata, self.data)
+                available_outputs = "No output for state '{}'. Data: '{}'.".format(self.device.state, self.data)
             raise MolerException(
                 "No output for cmd: '{}' in state '{}'!\n"
                 "Available outputs for the state: '{}'.\n"
                 "Please update your device_output dict!\n"
                 "{}".format(cmd_data_string, self.device.state, available_outputs, exc)
             )
```

### Comparing `moler-2.8.0/moler/util/moler_test.py` & `moler-2.9.0/moler/util/moler_test.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/tracked_thread.py` & `moler-2.9.0/moler/util/tracked_thread.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/compressed_timed_rotating_file_handler.py` & `moler-2.9.0/moler/util/compressed_timed_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/util/cmds_events_doc.py` & `moler-2.9.0/moler/util/cmds_events_doc.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/runner_factory.py` & `moler-2.9.0/moler/runner_factory.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/helpers.py` & `moler-2.9.0/moler/helpers.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/observer_thread_wrapper.py` & `moler-2.9.0/moler/observer_thread_wrapper.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/runner.py` & `moler-2.9.0/moler/runner.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/command_scheduler.py` & `moler-2.9.0/moler/command_scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/command.py` & `moler-2.9.0/moler/command.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/connection_observer.py` & `moler-2.9.0/moler/connection_observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,15 +352,21 @@
             raise NoResultSinceCancelCalled(self)
         if not self.done():
             raise ResultNotAvailableYet(self)
         return self._result
 
     def on_timeout(self):
         """Callback called when observer times out"""
-        pass
+        msg = ""
+        for attribute_name in sorted(self.__dict__.keys()):
+            if msg:
+                msg = "{}, '{}':'{}'".format(msg, attribute_name, self.__dict__[attribute_name])
+            else:
+                msg = "Timeout when '{}':'{}'".format(attribute_name, self.__dict__[attribute_name])
+        self._log(lvl=logging.INFO, msg=msg, levels_to_go_up=2)
 
     def is_command(self):
         """
         :return: True if instance of ConnectionObserver is a command. False if not a command.
         """
         return False
```

### Comparing `moler-2.8.0/moler/connection.py` & `moler-2.9.0/moler/connection.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/parser/table_text.py` & `moler-2.9.0/moler/parser/table_text.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/publisher.py` & `moler-2.9.0/moler/publisher.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/connection_factory.py` & `moler-2.9.0/moler/connection_factory.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/io_connection.py` & `moler-2.9.0/moler/io/io_connection.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/io_exceptions.py` & `moler-2.9.0/moler/io/io_exceptions.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/raw/terminal.py` & `moler-2.9.0/moler/io/raw/terminal.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/raw/tcp.py` & `moler-2.9.0/moler/io/raw/tcp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/raw/tcpserverpiped.py` & `moler-2.9.0/moler/io/raw/tcpserverpiped.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/raw/subprocess.py` & `moler-2.9.0/moler/io/raw/subprocess.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/raw/memory.py` & `moler-2.9.0/moler/io/raw/memory.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/raw/sshshell.py` & `moler-2.9.0/moler/io/raw/sshshell.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/raw/__init__.py` & `moler-2.9.0/moler/io/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/asyncio/terminal.py` & `moler-2.9.0/moler/io/asyncio/terminal.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/asyncio/tcp.py` & `moler-2.9.0/moler/io/asyncio/tcp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/io/asyncio/__init__.py` & `moler-2.9.0/moler/io/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/shared/wait4.py` & `moler-2.9.0/moler/events/shared/wait4.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/shared/genericshared_textualevent.py` & `moler-2.9.0/moler/events/shared/genericshared_textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/shared/password_prompt.py` & `moler-2.9.0/moler/events/shared/password_prompt.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/shared/genericshared_lineevent.py` & `moler-2.9.0/moler/events/shared/genericshared_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/juniper/genericshared_lineevent.py` & `moler-2.9.0/moler/events/juniper/genericshared_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/scpi/genericscpi_lineevent.py` & `moler-2.9.0/moler/events/scpi/genericscpi_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/lineevent.py` & `moler-2.9.0/moler/events/lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/textualevent.py` & `moler-2.9.0/moler/events/textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/last_login.py` & `moler-2.9.0/moler/events/unix/last_login.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/genericunix_lineevent.py` & `moler-2.9.0/moler/events/unix/genericunix_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/ping_response.py` & `moler-2.9.0/moler/events/unix/ping_response.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/failed_login_counter.py` & `moler-2.9.0/moler/events/unix/failed_login_counter.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/wait4prompt.py` & `moler-2.9.0/moler/events/unix/wait4prompt.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/genericunix_textualevent.py` & `moler-2.9.0/moler/events/unix/genericunix_textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/shutdown.py` & `moler-2.9.0/moler/events/unix/shutdown.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/ping_no_response.py` & `moler-2.9.0/moler/events/unix/ping_no_response.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/wait4prompts.py` & `moler-2.9.0/moler/events/unix/wait4prompts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 __author__ = 'Michal Ernst, Marcin Usielski'
-__copyright__ = 'Copyright (C) 2019-2021, Nokia'
+__copyright__ = 'Copyright (C) 2019-2023, Nokia'
 __email__ = 'michal.ernst@nokia.com, marcin.usielski@nokia.com'
 
 import datetime
 import re
 
 from moler.events.unix.genericunix_textualevent import GenericUnixTextualEvent
 from moler.exceptions import ParsingDone
@@ -18,28 +18,41 @@
         Event for waiting for prompt
         :param connection: moler connection to device, terminal when command is executed
         :param prompts: prompts->state regex dict. Key is regex, value is state.
         :param till_occurs_times: number of event occurrence
         :param runner: Runner to run event
         """
         super(Wait4prompts, self).__init__(connection=connection, runner=runner, till_occurs_times=till_occurs_times)
-        self.compiled_prompts_regex = self._compile_prompts_patterns(prompts)
+        self.compiled_prompts_regex = None  # Dict, key is a compiled regex, value is state name
+        self._prompts_list = None  # List of compiled regexps
+        self._set_prompts(prompts=prompts)
+
         self.process_full_lines_only = False
         self.check_against_all_prompts = False
         self._ret_list_matched = list()
 
     def on_new_line(self, line, is_full_line):
         try:
             self._parse_prompts(line)
         except ParsingDone:
             pass
 
+    def change_prompts(self, prompts):
+        self.pause()
+        self._set_prompts(prompts=prompts)
+        self.resume()
+        self.logger.info("Changed prompts into '{}'.".format(prompts))
+
+    def _set_prompts(self, prompts):
+        self.compiled_prompts_regex = self._compile_prompts_patterns(prompts=prompts)
+        self._prompts_list = sorted(self.compiled_prompts_regex.keys(), key=attrgetter('pattern'))
+
     def _parse_prompts(self, line):
         current_ret = None
-        for prompt_regex in sorted(self.compiled_prompts_regex.keys(), key=attrgetter('pattern')):
+        for prompt_regex in self._prompts_list:
             if self._regex_helper.search_compiled(prompt_regex, line):
                 current_ret = {
                     'line': line,
                     'prompt_regex': prompt_regex.pattern,
                     'state': self.compiled_prompts_regex[prompt_regex],
                     'time': datetime.datetime.now()
                 }
@@ -50,22 +63,22 @@
         if current_ret:
             if self.check_against_all_prompts:
                 current_ret['list_matched'] = self._ret_list_matched
                 self._ret_list_matched = list()
             self.event_occurred(event_data=current_ret)
             raise ParsingDone()
 
-    def _compile_prompts_patterns(self, patterns):
+    def _compile_prompts_patterns(self, prompts):
         compiled_patterns = dict()
-        for pattern in patterns.keys():
+        for pattern in prompts.keys():
             if not hasattr(pattern, "match"):  # Not compiled regexp
                 compiled_pattern = re.compile(pattern)
             else:
                 compiled_pattern = pattern
-            compiled_patterns[compiled_pattern] = patterns[pattern]
+            compiled_patterns[compiled_pattern] = prompts[pattern]
         return compiled_patterns
 
 
 EVENT_OUTPUT = """
 user@host01:~> TERM=xterm-mono telnet -4 host.domain.net 1500
 Login:
 Login:user
```

### Comparing `moler-2.8.0/moler/events/unix/last_failed_login.py` & `moler-2.9.0/moler/events/unix/last_failed_login.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/advise_to_change_your_password.py` & `moler-2.9.0/moler/events/unix/advise_to_change_your_password.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/u_boot_crtm.py` & `moler-2.9.0/moler/events/unix/u_boot_crtm.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/private_system.py` & `moler-2.9.0/moler/events/unix/private_system.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/unix/warning_default_password.py` & `moler-2.9.0/moler/events/unix/warning_default_password.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py` & `moler-2.9.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/observable_connection.py` & `moler-2.9.0/moler/observable_connection.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_functionality_level.py` & `moler-2.9.0/moler/cmd/at/get_functionality_level.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/cu.py` & `moler-2.9.0/moler/cmd/at/cu.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_revision_id.py` & `moler-2.9.0/moler/cmd/at/get_revision_id.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_imei.py` & `moler-2.9.0/moler/cmd/at/get_imei.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/set_mode.py` & `moler-2.9.0/moler/cmd/at/set_mode.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_manufacturer_id.py` & `moler-2.9.0/moler/cmd/at/get_manufacturer_id.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/run_script.py` & `moler-2.9.0/moler/cmd/at/run_script.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/set_functionality_level.py` & `moler-2.9.0/moler/cmd/at/set_functionality_level.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_apns.py` & `moler-2.9.0/moler/cmd/at/get_apns.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/attach.py` & `moler-2.9.0/moler/cmd/at/attach.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/detach.py` & `moler-2.9.0/moler/cmd/at/detach.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/exit_serial_proxy.py` & `moler-2.9.0/moler/cmd/at/exit_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/genericat.py` & `moler-2.9.0/moler/cmd/at/genericat.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/at.py` & `moler-2.9.0/moler/cmd/at/at.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_ip.py` & `moler-2.9.0/moler/cmd/at/get_ip.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_imsi.py` & `moler-2.9.0/moler/cmd/at/get_imsi.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/plink_serial.py` & `moler-2.9.0/moler/cmd/at/plink_serial.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_attach_state.py` & `moler-2.9.0/moler/cmd/at/get_attach_state.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/enable_echo.py` & `moler-2.9.0/moler/cmd/at/enable_echo.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/get_product_info.py` & `moler-2.9.0/moler/cmd/at/get_product_info.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/at/set_apn.py` & `moler-2.9.0/moler/cmd/at/set_apn.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/commandtextualgeneric.py` & `moler-2.9.0/moler/cmd/commandtextualgeneric.py`

 * *Files 4% similar despite different names*

```diff
@@ -457,31 +457,15 @@
         """
         Callback called by framework when timeout occurs.
 
         :return: None.
         """
         if self.break_on_timeout:
             self.break_cmd()
-        last_chunk = self._last_chunk
-        if last_chunk is not None:
-            try:
-                last_chunk = u"" + self._last_chunk
-            except Exception as ex:  # pragma: no cover
-                last_chunk = "{}/{}".format(ex, repr(ex))  # pragma: no cover
-        msg = ("Timeout when command_string='{}', _cmd_escaped='{}', _cmd_output_started='{}', ret_required='{}', "
-               "break_on_timeout='{}', _last_not_full_line='{}', _re_prompt='{}', do_not_process_after_done='{}', "
-               "newline_after_command_string='{}', wait_for_prompt_on_exception='{}', _stored_exception='{}', "
-               "current_ret='{}', _newline_chars='{}', _concatenate_before_command_starts='{}', "
-               "_command_string_right_index='{}', _command_string_left_index='{}', _last_chunk='{}'.").format(
-            self.__command_string, self._cmd_escaped.pattern, self._cmd_output_started, self.ret_required,
-            self.break_on_timeout, self._last_not_full_line, self._re_prompt.pattern, self.do_not_process_after_done,
-            self.newline_after_command_string, self.wait_for_prompt_on_exception, self._stored_exception,
-            self.current_ret, self._newline_chars, self._concatenate_before_command_starts,
-            self._max_index_from_beginning, self._max_index_from_end, last_chunk)
-        self._log(lvl=logging.INFO, msg=msg, levels_to_go_up=2)
+        return super(CommandTextualGeneric, self).on_timeout()
 
     def has_any_result(self):
         """
         Checks if any result was already set by command.
 
         :return: True if current_ret has collected any data. Otherwise False.
         """
```

### Comparing `moler-2.8.0/moler/cmd/juniper/genericjuniper.py` & `moler-2.9.0/moler/cmd/juniper/genericjuniper.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/juniper/configure/exit_configure.py` & `moler-2.9.0/moler/cmd/juniper/configure/exit_configure.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/juniper/cli/configure.py` & `moler-2.9.0/moler/cmd/juniper/cli/configure.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/scpi/scpi/read.py` & `moler-2.9.0/moler/cmd/scpi/scpi/read.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/scpi/scpi/idn.py` & `moler-2.9.0/moler/cmd/scpi/scpi/idn.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/scpi/scpi/run_command.py` & `moler-2.9.0/moler/cmd/scpi/scpi/run_command.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/scpi/scpi/genericscpistate.py` & `moler-2.9.0/moler/cmd/scpi/scpi/genericscpistate.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/pdu_aten/pdu/read_status.py` & `moler-2.9.0/moler/cmd/pdu_aten/pdu/read_status.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/pdu_aten/pdu/sw.py` & `moler-2.9.0/moler/cmd/pdu_aten/pdu/sw.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/pdu_aten/pdu/generic_pdu.py` & `moler-2.9.0/moler/cmd/pdu_aten/pdu/generic_pdu.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/pdu_aten/pdu/read_meter.py` & `moler-2.9.0/moler/cmd/pdu_aten/pdu/read_meter.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/pdu_aten/pdu/quit.py` & `moler-2.9.0/moler/cmd/pdu_aten/pdu/quit.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/pdu_aten/generic_pdu_aten.py` & `moler-2.9.0/moler/cmd/pdu_aten/generic_pdu_aten.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/commandchangingprompt.py` & `moler-2.9.0/moler/cmd/commandchangingprompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Generic command class for commands change prompt
 """
 
 __author__ = 'Marcin Usielski'
-__copyright__ = 'Copyright (C) 2019-2022, Nokia'
+__copyright__ = 'Copyright (C) 2019-2023, Nokia'
 __email__ = 'marcin.usielski@nokia.com'
 
 import abc
 import six
 
 from moler.cmd.commandtextualgeneric import CommandTextualGeneric
 from moler.exceptions import ParsingDone
@@ -61,16 +61,18 @@
 
         self._re_expected_prompt_without_anchors = regexp_without_anchors(self._re_expected_prompt)
         self._re_prompt_after_login_without_anchors = regexp_without_anchors(self._re_prompt_after_login)
 
     def __str__(self):
         base_str = super(CommandChangingPrompt, self).__str__()
         expected_prompt = self._re_expected_prompt.pattern
+        prompt_after_login = self._re_prompt_after_login.pattern
         # having expected prompt visible simplifies troubleshooting
-        return "{}, expected_prompt_regex:r'{}')".format(base_str[:-1], expected_prompt)
+        return "{}, expected_prompt_regex:r'{}', prompt_after_login:r'{}')".format(base_str[:-1], expected_prompt,
+                                                                                   prompt_after_login)
 
     def on_new_line(self, line, is_full_line):
         """
         Parses the output of the command.
 
         :param line: Line to process, can be only part of line. New line chars are removed from line.
         :param is_full_line: True if line had new line chars, False otherwise
```

### Comparing `moler-2.8.0/moler/cmd/__init__.py` & `moler-2.9.0/moler/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/adb/adb_shell.py` & `moler-2.9.0/moler/cmd/adb/adb_shell.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/wget.py` & `moler-2.9.0/moler/cmd/unix/wget.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/scp.py` & `moler-2.9.0/moler/cmd/unix/scp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/head.py` & `moler-2.9.0/moler/cmd/unix/head.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/pwd.py` & `moler-2.9.0/moler/cmd/unix/pwd.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/gunzip.py` & `moler-2.9.0/moler/cmd/unix/gunzip.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/cut.py` & `moler-2.9.0/moler/cmd/unix/cut.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/chown.py` & `moler-2.9.0/moler/cmd/unix/chown.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/chgrp.py` & `moler-2.9.0/moler/cmd/unix/chgrp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/su.py` & `moler-2.9.0/moler/cmd/unix/su.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/iperf.py` & `moler-2.9.0/moler/cmd/unix/iperf.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/sftp.py` & `moler-2.9.0/moler/cmd/unix/sftp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/userdel.py` & `moler-2.9.0/moler/cmd/unix/userdel.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ping.py` & `moler-2.9.0/moler/cmd/unix/ping.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/nping.py` & `moler-2.9.0/moler/cmd/unix/nping.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ip_link.py` & `moler-2.9.0/moler/cmd/unix/ip_link.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/adb_root.py` & `moler-2.9.0/moler/cmd/unix/adb_root.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/unzip.py` & `moler-2.9.0/moler/cmd/unix/unzip.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/sed.py` & `moler-2.9.0/moler/cmd/unix/sed.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/reboot.py` & `moler-2.9.0/moler/cmd/unix/reboot.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/traceroute.py` & `moler-2.9.0/moler/cmd/unix/traceroute.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/netstat.py` & `moler-2.9.0/moler/cmd/unix/netstat.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ctrl_c.py` & `moler-2.9.0/moler/cmd/unix/ctrl_c.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/socat.py` & `moler-2.9.0/moler/cmd/unix/socat.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ss.py` & `moler-2.9.0/moler/cmd/unix/ss.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/cd.py` & `moler-2.9.0/moler/cmd/unix/cd.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/mkdir.py` & `moler-2.9.0/moler/cmd/unix/mkdir.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/openssl_x509_text_in.py` & `moler-2.9.0/moler/cmd/unix/openssl_x509_text_in.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/run_script.py` & `moler-2.9.0/moler/cmd/unix/run_script.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/telnet.py` & `moler-2.9.0/moler/cmd/unix/telnet.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/history.py` & `moler-2.9.0/moler/cmd/unix/history.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/exit_telnet.py` & `moler-2.9.0/moler/cmd/unix/exit_telnet.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/sshkeygen.py` & `moler-2.9.0/moler/cmd/unix/sshkeygen.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/sysctl.py` & `moler-2.9.0/moler/cmd/unix/sysctl.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ls.py` & `moler-2.9.0/moler/cmd/unix/ls.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/which.py` & `moler-2.9.0/moler/cmd/unix/which.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/enter.py` & `moler-2.9.0/moler/cmd/unix/enter.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/sudo.py` & `moler-2.9.0/moler/cmd/unix/sudo.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/devmem.py` & `moler-2.9.0/moler/cmd/unix/devmem.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/hexdump.py` & `moler-2.9.0/moler/cmd/unix/hexdump.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/md5sum.py` & `moler-2.9.0/moler/cmd/unix/md5sum.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/rm.py` & `moler-2.9.0/moler/cmd/unix/rm.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/date.py` & `moler-2.9.0/moler/cmd/unix/date.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/cat.py` & `moler-2.9.0/moler/cmd/unix/cat.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/lxc_ls.py` & `moler-2.9.0/moler/cmd/unix/lxc_ls.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/mpstat.py` & `moler-2.9.0/moler/cmd/unix/mpstat.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ip_addr.py` & `moler-2.9.0/moler/cmd/unix/ip_addr.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/mv.py` & `moler-2.9.0/moler/cmd/unix/mv.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/export.py` & `moler-2.9.0/moler/cmd/unix/export.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/dmesg.py` & `moler-2.9.0/moler/cmd/unix/dmesg.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/gzip.py` & `moler-2.9.0/moler/cmd/unix/gzip.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/lxc_info.py` & `moler-2.9.0/moler/cmd/unix/lxc_info.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ip_neigh.py` & `moler-2.9.0/moler/cmd/unix/ip_neigh.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/kill.py` & `moler-2.9.0/moler/cmd/unix/kill.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/killall.py` & `moler-2.9.0/moler/cmd/unix/killall.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/w.py` & `moler-2.9.0/moler/cmd/unix/w.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/mount.py` & `moler-2.9.0/moler/cmd/unix/mount.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/nmap.py` & `moler-2.9.0/moler/cmd/unix/nmap.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/exit.py` & `moler-2.9.0/moler/cmd/unix/exit.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/tar.py` & `moler-2.9.0/moler/cmd/unix/tar.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/zip.py` & `moler-2.9.0/moler/cmd/unix/zip.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ssh.py` & `moler-2.9.0/moler/cmd/unix/ssh.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/adb_forward.py` & `moler-2.9.0/moler/cmd/unix/adb_forward.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/find.py` & `moler-2.9.0/moler/cmd/unix/find.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/sync.py` & `moler-2.9.0/moler/cmd/unix/sync.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/id.py` & `moler-2.9.0/moler/cmd/unix/id.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/uptime.py` & `moler-2.9.0/moler/cmd/unix/uptime.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ifconfig.py` & `moler-2.9.0/moler/cmd/unix/ifconfig.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/lxc_attach.py` & `moler-2.9.0/moler/cmd/unix/lxc_attach.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/uname.py` & `moler-2.9.0/moler/cmd/unix/uname.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/cp.py` & `moler-2.9.0/moler/cmd/unix/cp.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/tail_latest_file.py` & `moler-2.9.0/moler/cmd/unix/tail_latest_file.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/hostname.py` & `moler-2.9.0/moler/cmd/unix/hostname.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/systemctl.py` & `moler-2.9.0/moler/cmd/unix/systemctl.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/run_serial_proxy.py` & `moler-2.9.0/moler/cmd/unix/run_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ip_route.py` & `moler-2.9.0/moler/cmd/unix/ip_route.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/bash.py` & `moler-2.9.0/moler/cmd/unix/bash.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/shasum.py` & `moler-2.9.0/moler/cmd/unix/shasum.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/whoami.py` & `moler-2.9.0/moler/cmd/unix/whoami.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/tee.py` & `moler-2.9.0/moler/cmd/unix/tee.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/route.py` & `moler-2.9.0/moler/cmd/unix/route.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/chmod.py` & `moler-2.9.0/moler/cmd/unix/chmod.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/iperf2.py` & `moler-2.9.0/moler/cmd/unix/iperf2.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/du.py` & `moler-2.9.0/moler/cmd/unix/du.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/service.py` & `moler-2.9.0/moler/cmd/unix/service.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/generictelnetssh.py` & `moler-2.9.0/moler/cmd/unix/generictelnetssh.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/nft.py` & `moler-2.9.0/moler/cmd/unix/nft.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/unxz.py` & `moler-2.9.0/moler/cmd/unix/unxz.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/tail.py` & `moler-2.9.0/moler/cmd/unix/tail.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/iptables.py` & `moler-2.9.0/moler/cmd/unix/iptables.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/passwd.py` & `moler-2.9.0/moler/cmd/unix/passwd.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ln.py` & `moler-2.9.0/moler/cmd/unix/ln.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/genericunix.py` & `moler-2.9.0/moler/cmd/unix/genericunix.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/env.py` & `moler-2.9.0/moler/cmd/unix/env.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ethtool.py` & `moler-2.9.0/moler/cmd/unix/ethtool.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/useradd.py` & `moler-2.9.0/moler/cmd/unix/useradd.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/grep.py` & `moler-2.9.0/moler/cmd/unix/grep.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ipsec.py` & `moler-2.9.0/moler/cmd/unix/ipsec.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ntpq.py` & `moler-2.9.0/moler/cmd/unix/ntpq.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/lsof.py` & `moler-2.9.0/moler/cmd/unix/lsof.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/tcpdump.py` & `moler-2.9.0/moler/cmd/unix/tcpdump.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/df.py` & `moler-2.9.0/moler/cmd/unix/df.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/tshark.py` & `moler-2.9.0/moler/cmd/unix/tshark.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/openssl_s_client.py` & `moler-2.9.0/moler/cmd/unix/openssl_s_client.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/adb_devices.py` & `moler-2.9.0/moler/cmd/unix/adb_devices.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/hciconfig.py` & `moler-2.9.0/moler/cmd/unix/hciconfig.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/pkill.py` & `moler-2.9.0/moler/cmd/unix/pkill.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/top.py` & `moler-2.9.0/moler/cmd/unix/top.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/ps.py` & `moler-2.9.0/moler/cmd/unix/ps.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/cmd/unix/echo.py` & `moler-2.9.0/moler/cmd/unix/echo.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/threaded_moler_connection.py` & `moler-2.9.0/moler/threaded_moler_connection.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/event_awaiter.py` & `moler-2.9.0/moler/event_awaiter.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/abstract_moler_connection.py` & `moler-2.9.0/moler/abstract_moler_connection.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/config/devices.py` & `moler-2.9.0/moler/config/devices.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/config/loggers.py` & `moler-2.9.0/moler/config/loggers.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/config/runners.py` & `moler-2.9.0/moler/config/runners.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/config/connections.py` & `moler-2.9.0/moler/config/connections.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/moler/config/__init__.py` & `moler-2.9.0/moler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-2.8.0/README.md` & `moler-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![image](https://img.shields.io/badge/pypi-v2.8.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/pypi-v2.9.0-blue.svg)](https://pypi.org/project/moler/)
 [![image](https://img.shields.io/badge/python-2.7%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/moler/)
 [![Build Status](https://travis-ci.org/nokia/moler.svg?branch=master)](https://travis-ci.org/nokia/moler)
 [![Coverage Status](https://coveralls.io/repos/github/nokia/moler/badge.svg?branch=master)](https://coveralls.io/github/nokia/moler?branch=master)
 [![BCH compliance](https://bettercodehub.com/edge/badge/nokia/moler?branch=master)](https://bettercodehub.com/)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/355afc9110f34d549b7c08c33961827c)](https://www.codacy.com/app/mplichta/moler?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nokia/moler&amp;utm_campaign=Badge_Grade)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
```

### Comparing `moler-2.8.0/PKG-INFO` & `moler-2.9.0/moler.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,577 +1,17 @@
 Metadata-Version: 2.1
 Name: moler
-Version: 2.8.0
+Version: 2.9.0
 Summary: Moler is library to help in building automated tests
 Home-page: https://github.com/nokia/moler
 Author: Nokia
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/nokia/moler/issues
 Project-URL: Source, https://github.com/nokia/moler
-Description: [![image](https://img.shields.io/badge/pypi-v2.8.0-blue.svg)](https://pypi.org/project/moler/)
-        [![image](https://img.shields.io/badge/python-2.7%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/moler/)
-        [![Build Status](https://travis-ci.org/nokia/moler.svg?branch=master)](https://travis-ci.org/nokia/moler)
-        [![Coverage Status](https://coveralls.io/repos/github/nokia/moler/badge.svg?branch=master)](https://coveralls.io/github/nokia/moler?branch=master)
-        [![BCH compliance](https://bettercodehub.com/edge/badge/nokia/moler?branch=master)](https://bettercodehub.com/)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/355afc9110f34d549b7c08c33961827c)](https://www.codacy.com/app/mplichta/moler?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nokia/moler&amp;utm_campaign=Badge_Grade)
-        [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
-        
-        # Table of Contents
-        1. [Changelog](#changelog)
-        2. [Moler info](#moler)
-        3. [Moler usage examples](#moler-usage-examples)
-        4. [API design reasoning](#api-design-reasoning)
-        5. [Designed API](#designed-api)
-        
-        # Changelog
-        View our [chronological list](./CHANGELOG.md) of user-facing changes, large and small, made to the Moler project.
-        
-        ![moler logo](https://i.imgur.com/mkPutdC.png)
-        # Moler
-        Moler ([name origin](https://github.com/nokia/moler/wiki#moler-name-origin)) is Python library
-        that provides "bricks" for building  automated tests.
-        All these "bricks" have clearly defined responsibilities, have similar API,
-        follow same construction pattern (so new ones are easy to create).
-        
-        Here they are:
-        * Commands as self-reliant object
-          * to allow for command triggering and parsing encapsulated in single object (lower maintenance cost)
-        * Event observers & callbacks (alarms are events example)
-          * to allow for online reaction (not offline postprocessing)
-        * Run observers/commands in the background
-          * to allow for test logic decomposition into multiple commands running in parallel
-          * to allow for handling unexpected system behavior (reboots, alarms)
-        * State machines -> automatic auto-connecting after dropped connection
-          * to increase framework auto-recovery and help in troubleshooting "what went wrong"
-        * Automatic logging of all connections towards devices used by tests
-          * to decrease investigation time by having logs focused on different parts of system under test
-        
-        # Moler usage examples
-        Let's see Moler in action. Here is hypothetical use case: "find PIDs of all python processes":
-        
-        ```python
-        
-            from moler.config import load_config
-            from moler.device.device import DeviceFactory
-        
-            load_config(config='my_devices.yml')                    # description of available devices
-            my_unix = DeviceFactory.get_device(name='MyMachine')    # take specific device out of available ones
-            ps_cmd = my_unix.get_cmd(cmd_name="ps",                 # take command of that device
-                                     cmd_params={"options": "-ef"})
-        
-            processes_info = ps_cmd()                               # run the command, it returns result
-            for proc_info in processes_info:
-                if 'python' in proc_info['CMD']:
-                    print("PID: {info[PID]} CMD: {info[CMD]}".format(info=proc_info))
-        ```
-        
-        * To have command we ask device "give me such command".
-        * To run command we just call it as function (command object is callable)
-        * What command returns is usually dict or list of dicts - easy to process
-        
-        Above code displays:
-        
-        ```bash
-        
-            PID: 1817 CMD: /usr/bin/python /usr/share/system-config-printer/applet.py
-            PID: 21825 CMD: /usr/bin/python /home/gl/moler/examples/command/unix_ps.py
-        ```
-        
-        How does it know what `'MyMachine'` means? Code loads definition from `my_devices.yml` configuration file:
-        
-        ```yaml
-        
-            DEVICES:
-        
-              MyMachine:
-                DEVICE_CLASS: moler.device.unixlocal.UnixLocal
-        
-              RebexTestMachine:
-                DEVICE_CLASS: moler.device.unixremote.UnixRemote
-                CONNECTION_HOPS:
-                  UNIX_LOCAL:                # from state
-                    UNIX_REMOTE:             # to state
-                      execute_command: ssh   # via command
-                      command_params:        # with params
-                        expected_prompt: demo@
-                        host: test.rebex.net
-                        login: demo
-                        password: password
-                        set_timeout: False   # remote doesn't support: export TMOUT
-        ```
-        
-        We have remote machine in our config. Let's check if there is 'readme.txt' file
-        on that machine (and some info about the file):
-        
-        ```python
-        
-            remote_unix = DeviceFactory.get_device(name='RebexTestMachine')  # it starts in local shell
-            remote_unix.goto_state(state="UNIX_REMOTE")                      # make it go to remote shell
-        
-            ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
-        
-            remote_files = ls_cmd()
-        
-            if 'readme.txt' in remote_files['files']:
-                print("readme.txt file:")
-                readme_file_info = remote_files['files']['readme.txt']
-                for attr in readme_file_info:
-                    print("  {:<18}: {}".format(attr, readme_file_info[attr]))
-        ```
-        
-        As you may noticed device is state machine. State transitions are defined inside
-        configuration file under `CONNECTION_HOPS`. Please note, that it is only config file who
-        knows "I need to use ssh to be on remote" - client code just says "go to remote".
-        Thanks to that you can exchange "how to reach remote" without any change in main code.
-        
-        Above code displays:
-        
-        ```bash
-        
-            readme.txt file:
-              permissions       : -rw-------
-              hard_links_count  : 1
-              owner             : demo
-              group             : users
-              size_raw          : 403
-              size_bytes        : 403
-              date              : Apr 08  2014
-              name              : readme.txt
-        ```
-        
-        How about doing multiple things in parallel. Let's ping google
-        while asking test.rebex.net about readme.txt file:
-        
-        ```python
-        my_unix = DeviceFactory.get_device(name='MyMachine')
-        host = 'www.google.com'
-        ping_cmd = my_unix.get_cmd(cmd_name="ping", cmd_params={"destination": host, "options": "-w 6"})
-        
-        remote_unix = DeviceFactory.get_device(name='RebexTestMachine')
-        remote_unix.goto_state(state="UNIX_REMOTE")
-        ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
-        
-        print("Start pinging {} ...".format(host))
-        ping_cmd.start()                                # run command in background
-        print("Let's check readme.txt at {} while pinging {} ...".format(remote_unix.name, host))
-        
-        remote_files = ls_cmd()                         # foreground "run in the meantime"
-        file_info = remote_files['files']['readme.txt']
-        print("readme.txt file: owner={fi[owner]}, size={fi[size_bytes]}".format(fi=file_info))
-        
-        ping_stats = ping_cmd.await_done(timeout=6)     # await background command
-        print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
-                                                  ping_stats['packet_loss'],
-                                                  'time_avg',
-                                                  ping_stats['time_avg'],
-                                                  ping_stats['time_unit']))
-        ```
-        
-        ```log
-        Start pinging www.google.com ...
-        Let's check readme.txt at RebexTestMachine while pinging www.google.com ...
-        readme.txt file: owner=demo, size=403
-        ping www.google.com: packet_loss=0, time_avg=35.251 [ms]
-        ```
-        
-        Besides being callable command-object works as "Future" (result promise).
-        You can start it in background and later await till it is done to grab result.
-        
-        If we enhance our configuration with logging related info:
-        
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-        ```
-        
-        then above code will automatically create Molers' main log (`moler.log`)
-        which shows activity on all devices:
-        
-        ```log
-        22:30:19.723 INFO       moler               |More logs in: ./logs
-        22:30:19.747 INFO       MyMachine           |Connection to: 'MyMachine' has been opened.
-        22:30:19.748 INFO       MyMachine           |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.866 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:19.901 INFO       RebexTestMachine    |Connection to: 'RebexTestMachine' has been opened.
-        22:30:19.901 INFO       RebexTestMachine    |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.919 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
-        22:30:19.920 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:19.921 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
-        22:30:19.921 INFO       RebexTestMachine    |TERM=xterm-mono ssh -l demo test.rebex.net
-        22:30:20.763 INFO       RebexTestMachine    |*********
-        22:30:20.909 INFO       RebexTestMachine    |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
-        22:30:20.917 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh' finished.
-        22:30:20.919 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
-        22:30:20.920 INFO       MyMachine           |ping www.google.com -w 6
-        22:30:20.920 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
-        22:30:20.922 INFO       RebexTestMachine    |ls -l
-        22:30:20.985 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls' finished.
-        22:30:26.968 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping' finished.
-        22:30:26.992 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        22:30:27.011 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
-        22:30:27.032 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        
-        ```
-        
-        As you may noticed main log shows code progress from high-level view - data
-        on connections are not visible, just activity of commands running on devices.
-        
-        If you want to see in details what has happened on each device - you have it in device logs.
-        Moler creates log per each device
-        `moler.RebexTestMachine.log`:
-        
-        ```log
-        22:30:19.901  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.902 <|
-        22:30:19.919  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
-        22:30:19.920  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:19.921  |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
-        22:30:19.921 >|TERM=xterm-mono ssh -l demo test.rebex.net
-        
-        22:30:19.924 <|TERM=xterm-mono ssh -l demo test.rebex.net
-        
-        22:30:20.762 <|Password:
-        22:30:20.763 >|*********
-        22:30:20.763 <|
-        
-        22:30:20.908 <|Welcome to Rebex Virtual Shell!
-                      |For a list of supported commands, type 'help'.
-                      |demo@ETNA:/$
-        22:30:20.909  |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
-        22:30:20.917  |Command 'moler.cmd.unix.ssh.Ssh' finished.
-        22:30:20.920  |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
-        22:30:20.922 >|ls -l
-        
-        22:30:20.974 <|ls -l
-        
-        22:30:20.978 <|drwx------ 2 demo users          0 Jul 26  2017 .
-        
-        22:30:20.979 <|drwx------ 2 demo users          0 Jul 26  2017 ..
-                      |drwx------ 2 demo users          0 Dec 03  2015 aspnet_client
-                      |drwx------ 2 demo users          0 Oct 27  2015 pub
-                      |-rw------- 1 demo users        403 Apr 08  2014 readme.txt
-                      |demo@ETNA:/$
-        22:30:20.985  |Command 'moler.cmd.unix.ls.Ls' finished.
-        22:30:26.992  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        22:30:27.011  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
-        ```
-        
-        and `moler.MyMachine.log`:
-        
-        ```log
-        22:30:19.748  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
-        22:30:19.748 <|
-        22:30:19.866  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
-        22:30:20.919  |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
-        22:30:20.920 >|ping www.google.com -w 6
-        
-        22:30:20.921 <|ping www.google.com -w 6
-        
-        22:30:20.959 <|PING www.google.com (216.58.215.68) 56(84) bytes of data.
-        22:30:20.960 <|
-        
-        22:30:21.000 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=1 ttl=51 time=40.1 ms
-        22:30:21.001 <|
-        
-        22:30:21.992 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=2 ttl=51 time=31.0 ms
-        
-        22:30:22.999 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=3 ttl=51 time=36.5 ms
-        
-        22:30:23.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=4 ttl=51 time=31.4 ms
-        
-        22:30:24.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=5 ttl=51 time=29.8 ms
-        
-        22:30:26.010 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=6 ttl=51 time=42.4 ms
-        
-        22:30:26.960 <|
-                      |--- www.google.com ping statistics ---
-                      |6 packets transmitted, 6 received, 0% packet loss, time 5007ms
-                      |rtt min/avg/max/mdev = 29.888/35.251/42.405/4.786 ms
-                      |moler_bash#
-        22:30:26.968  |Command 'moler.cmd.unix.ping.Ping' finished.
-        22:30:27.032  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
-        ```
-        
-        If the log files are too large you can split files.
-        
-        The log files can be split by size. For example let's assume we want split log files by 5 MB (5242880 bytes) and we want
-        to keep maximum 999 files:
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: size
-                INTERVAL: 5242880
-                BACKUP_COUNT: 999  # Default value
-              
-        
-        ```
-        
-        The log files can be split by time. For example let's assume we want split log files every 30 minutes (1800 seconds)
-         and we want to keep maximum 999 files (default value):
-         
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: time
-                INTERVAL: 1800
-                BACKUP_COUNT: 999  # Default value
-        ```
-        
-        For space saving Moler can compress the logs after rotation. The external tool is used. Let's use the above examples
-        to show how to compress logs:
-        
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: size
-                INTERVAL: 5242880
-                BACKUP_COUNT: 999  # Default value
-                COMPRESS_AFTER_ROTATION: True  # Default is False
-                COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value
-                COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
-        
-        
-        ```
-        
-        ```yaml
-            LOGGER:
-              PATH: ./logs
-              DATE_FORMAT: "%H:%M:%S"
-              LOG_ROTATION:
-                KIND: time
-                INTERVAL: 1800
-                BACKUP_COUNT: 999  # Default value
-                COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value      
-                COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
-        ```
-        
-        In a script we can also disable logging from device. Please use it very carefully. Investigation any issue may be
-         impossible if we don't have full logs.
-         
-        ```python
-        my_unix = DeviceFactory.get_device(name='MyMachine')
-        
-        my_unix.disbale_logging()  # to disable logging on device
-        
-        my_unix.enable_logging()  # to enable logging on device
-        ```
-        
-        In a script you can add suffix to all log files or only to files for specific devices. with disable logging from device. 
-         
-        ```python
-        from moler.config.loggers import change_logging_suffix
-        change_logging_suffix(".suffix1")  # all log files with suffix
-        change_logging_suffix(None)  # all log files without suffx
-        
-        my_unix = DeviceFactory.get_device(name='MyMachine')
-        
-        my_unix.set_logging_suffix("device_suffix")  # to add suffix to filename with logs
-        
-        my_unix.set_suffix(None)  # to remove suffix from filename with logs
-        ```
-        
-        Previous examples ask device to create command. We can also create command ourselves
-        giving it connection to operate on:
-        
-        ```python
-        
-            import time
-            from moler.cmd.unix.ping import Ping
-            from moler.connection_factory import get_connection
-        
-            host = 'www.google.com'
-            terminal = get_connection(io_type='terminal', variant='threaded')  # take connection
-            with terminal.open():
-                ping_cmd = Ping(connection=terminal.moler_connection,
-                                destination=host, options="-w 6")
-                print("Start pinging {} ...".format(host))
-                ping_cmd.start()
-                print("Doing other stuff while pinging {} ...".format(host))
-                time.sleep(3)
-                ping_stats = ping_cmd.await_done(timeout=4)
-                print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
-                                                          ping_stats['packet_loss'],
-                                                          'time_avg',
-                                                          ping_stats['time_avg'],
-                                                          ping_stats['time_unit']))
-        ```
-        
-        Please note also that connection is context manager doing open/close actions.
-        
-        
-        ```bash
-        
-            Start pinging www.google.com ...
-            Doing other stuff while pinging www.google.com ...
-            ping www.google.com: packet_loss=0, time_avg=50.000 [ms]
-        ```
-        
-        ## Reuse freedom
-        Library gives you freedom which part you want to reuse. We are fan's of "take what you need only".
-        * You may use configuration files or configure things by Python calls.
-        
-           ```python
-           load_config(config={'DEVICES': {'MyMachine': {'DEVICE_CLASS': 'moler.device.unixlocal.UnixLocal'}}})
-           ```
-        * You may use devices or create commands manually
-        * You can take connection or build it yourself:
-        
-           ```python
-           from moler.threaded_moler_connection import ThreadedMolerConnection
-           from moler.io.raw.terminal import ThreadedTerminal
-        
-           terminal_connection = ThreadedTerminal(moler_connection=ThreadedMolerConnection())
-           ```
-        * You can even install your own implementation in place of default implementation per connection type
-        
-        # API design reasoning
-        The main goal of command is its usage simplicity: just run it and give me back its result.
-        
-        Command hides from its caller:
-        * a way how it realizes "runs"
-        * how it gets data of output to be parsed
-        * how it parses that data
-        
-        Command shows to its caller:
-        * API to start/stop it or await for its completion
-        * API to query for its result or result readiness
-        
-        Command works as [Futures and promises](https://en.wikipedia.org/wiki/Futures_and_promises)
-        
-        After starting, we await for its result which is parsed out command output provided usually as dict.
-        Running that command and parsing its output may take some time, so till that point result computation is yet incomplete.
-        
-        ## Command as future
-        * it starts some command on device/shell over connection
-          (as future-function starts it's execution)
-        * it parses data incoming over such connection
-          (as future-function does it's processing)
-        * it stores result of that parsing
-          (as future-function concludes in calculation result)
-        * it provides means to return that result
-          (as future-function does via 'return' or 'yield' statement)
-        * it's result is not ready "just-after" calling command
-          (as it is with future in contrast to function)
-        
-        So command should have future API.
-        
-        Quote from **_"Professional Python"_** by **Luke Sneeringer**:
-        > The Future is a standalone object. It is independent of the actual function that is running.
-        > It does nothing but store the state and result information.
-        
-        Command differs in that it is both:
-        * function-like object performing computation
-        * future-like object storing result of that computation.
-        
-        ## Command vs. Connection-observer
-        Command is just "active version" of connection observer.
-        
-        Connection observer is passive since it just observes connection for some data;
-        data that may just asynchronously appear (alarms, reboots or anything you want).
-        Intention here is split of responsibility: one observer is looking for alarms,
-        another one for reboots.
-        
-        Command is active since it actively triggers some output on connection
-        by sending command-string over that connection. So, it activates some action
-        on device-behind-connection. That action is "command" in device terminology.
-        Like `ping` on bash console/device. And it produces that "command" output.
-        That output is what Moler's Command as connection-observer is looking for.
-        
-        ## Most well known Python's futures
-        * [concurrent.futures.Future](https://docs.python.org/3/library/concurrent.futures.html)
-        * [asyncio.Future](https://docs.python.org/3/library/asyncio-task.html#future)
-        
-        | API                     | concurrent.futures.Future                   | asyncio.Future                                      |
-        | :---------------------- | :------------------------------------------ | :-------------------------------------------------- |
-        | storing result          | :white_check_mark: `set_result()`           | :white_check_mark: `set_result()`                   |
-        | result retrieval        | :white_check_mark: `result()`               | :white_check_mark: `result()`                       |
-        | storing failure cause   | :white_check_mark: `set_exception()`        | :white_check_mark: `set_exception()`                |
-        | failure cause retrieval | :white_check_mark: `exception()`            | :white_check_mark: `exception()`                    |
-        | stopping                | :white_check_mark: `cancel()`               | :white_check_mark: `cancel()`                       |
-        | check if stopped        | :white_check_mark: `cancelled()`            | :white_check_mark: `cancelled()`                    |
-        | check if running        | :white_check_mark: `running()`              | :no_entry_sign: `(but AbstractEventLoop.running())` |
-        | check if completed      | :white_check_mark: `done()`                 | :white_check_mark: `done()`                         |
-        | subscribe completion    | :white_check_mark: `add_done_callback()`    | :white_check_mark: `add_done_callback()`            |
-        | unsubscribe completion  | :no_entry_sign:                             | :white_check_mark: `remove_done_callback()`         |
-        
-        Starting callable to be run "as future" is done by entities external to future-object
-        
-        | API              | concurrent.futures<br>start via Executor objects (thread/proc) | asyncio<br>start via module-lvl functions or ev-loop |
-        | ---------------- | ---------------------------------------- | ---------------------------------------------- |
-        | start callable   | submit(fn, *args, **kwargs)<br>Schedules callable to be executed as<br>fn(*args **kwargs) -> Future | ensure_future(coro_or_future) -> Task<br>future = run_coroutine_threadsafe(coro, loop) |
-        | start same callable<br>on data iterator | map(fn, *iterables, timeout) -> iterator | join_future = asyncio.gather(*map(f, iterable))<br>loop.run_until_complete(join_future)|
-        
-        Awaiting completion of future is done by entities external to future-object
-        
-        | API               | concurrent.futures<br>awaiting by module level functions | asyncio<br>awaiting by module-lvl functions or ev-loop |
-        | ----------------- | ------------------------------------------ | -------------------------------------------- |
-        | await completion  |  done, not_done = wait(futures, timeout) -> futures | done, not_done = await wait(futures)<br>results = await gather(futures)<br>result = await future<br>result = yield from future<br>result = await coroutine<br>result = yield from coroutine<br>result = yield from wait_for(future, timeout)<br>loop.run_until_complete(future) -> blocking run |
-        | process as they<br>complete | for done in as_completed(futures, timeout) -> futures | for done in as_completed(futures, timeout) -> futures |
-        
-        ## Fundamental difference of command
-        Contrary to **concurrent.futures** and **asyncio** we don't want command to be run by some external entity.
-        We want it to be self-executable for usage simplicity.
-        We want to take command and just say to it:
-        * **"run"** or **"run in background"**
-        * and not **"Hi, external runner, would you run/run-background that command for me"**
-        
-        # Designed API
-        1. create command object
-        ``` python
-        command = Command()
-        ```
-        
-        2. run it synchronously/blocking and get result in one shot behaves like function call since Command is callable.
-        
-        Run-as-callable gives big advantage since it fits well in python ecosystem.
-        ``` python
-        result = command()
-        ```
-        function example:
-        ``` python
-        map(ping_cmd, all_machines_to_validate_reachability)
-        ```
-        
-        3. run it asynchronously/nonblocking
-        ``` python
-        command_as_future = command.start()
-        ```
-        
-        4. shift from background to foreground
-        
-        **asyncio:** variant looks like:
-        ``` python
-        result = await future
-        done_futures, pending = yield from asyncio.wait(futures)
-        result = yield from asyncio.wait_for(future, 60.0)
-        ```
-        and **concurrent.futures** variant looks like:
-        ``` python
-        done_futures, pending = wait(futures)
-        ```
-        Moler's API maps to above well-known API
-        ``` python
-        result = command.await_done(timeout)
-        ```
-        * it is "internal" to command "Hi command, that is what I want from you" (above APIs say "Hi you there, that is what I want you to do with command")
-        * it directly (Zen of Python) shows what we are awaiting for
-        * timeout is required parameter (not as in concurrent.futures) since we don't expect endless execution of command (user must know what is worst case timeout to await command completion)
-        
-        # Video introduction
-        You can [watch videos how to use Moler on YouTube](https://www.youtube.com/channel/UCgToo2qq8kLMyEgzd4btM9g). 
-        
 Keywords: testing development
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
@@ -585,7 +25,567 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![image](https://img.shields.io/badge/pypi-v2.9.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/python-2.7%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/moler/)
+[![Build Status](https://travis-ci.org/nokia/moler.svg?branch=master)](https://travis-ci.org/nokia/moler)
+[![Coverage Status](https://coveralls.io/repos/github/nokia/moler/badge.svg?branch=master)](https://coveralls.io/github/nokia/moler?branch=master)
+[![BCH compliance](https://bettercodehub.com/edge/badge/nokia/moler?branch=master)](https://bettercodehub.com/)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/355afc9110f34d549b7c08c33961827c)](https://www.codacy.com/app/mplichta/moler?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nokia/moler&amp;utm_campaign=Badge_Grade)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
+
+# Table of Contents
+1. [Changelog](#changelog)
+2. [Moler info](#moler)
+3. [Moler usage examples](#moler-usage-examples)
+4. [API design reasoning](#api-design-reasoning)
+5. [Designed API](#designed-api)
+
+# Changelog
+View our [chronological list](./CHANGELOG.md) of user-facing changes, large and small, made to the Moler project.
+
+![moler logo](https://i.imgur.com/mkPutdC.png)
+# Moler
+Moler ([name origin](https://github.com/nokia/moler/wiki#moler-name-origin)) is Python library
+that provides "bricks" for building  automated tests.
+All these "bricks" have clearly defined responsibilities, have similar API,
+follow same construction pattern (so new ones are easy to create).
+
+Here they are:
+* Commands as self-reliant object
+  * to allow for command triggering and parsing encapsulated in single object (lower maintenance cost)
+* Event observers & callbacks (alarms are events example)
+  * to allow for online reaction (not offline postprocessing)
+* Run observers/commands in the background
+  * to allow for test logic decomposition into multiple commands running in parallel
+  * to allow for handling unexpected system behavior (reboots, alarms)
+* State machines -> automatic auto-connecting after dropped connection
+  * to increase framework auto-recovery and help in troubleshooting "what went wrong"
+* Automatic logging of all connections towards devices used by tests
+  * to decrease investigation time by having logs focused on different parts of system under test
+
+# Moler usage examples
+Let's see Moler in action. Here is hypothetical use case: "find PIDs of all python processes":
+
+```python
+
+    from moler.config import load_config
+    from moler.device.device import DeviceFactory
+
+    load_config(config='my_devices.yml')                    # description of available devices
+    my_unix = DeviceFactory.get_device(name='MyMachine')    # take specific device out of available ones
+    ps_cmd = my_unix.get_cmd(cmd_name="ps",                 # take command of that device
+                             cmd_params={"options": "-ef"})
+
+    processes_info = ps_cmd()                               # run the command, it returns result
+    for proc_info in processes_info:
+        if 'python' in proc_info['CMD']:
+            print("PID: {info[PID]} CMD: {info[CMD]}".format(info=proc_info))
+```
+
+* To have command we ask device "give me such command".
+* To run command we just call it as function (command object is callable)
+* What command returns is usually dict or list of dicts - easy to process
+
+Above code displays:
+
+```bash
+
+    PID: 1817 CMD: /usr/bin/python /usr/share/system-config-printer/applet.py
+    PID: 21825 CMD: /usr/bin/python /home/gl/moler/examples/command/unix_ps.py
+```
+
+How does it know what `'MyMachine'` means? Code loads definition from `my_devices.yml` configuration file:
+
+```yaml
+
+    DEVICES:
+
+      MyMachine:
+        DEVICE_CLASS: moler.device.unixlocal.UnixLocal
+
+      RebexTestMachine:
+        DEVICE_CLASS: moler.device.unixremote.UnixRemote
+        CONNECTION_HOPS:
+          UNIX_LOCAL:                # from state
+            UNIX_REMOTE:             # to state
+              execute_command: ssh   # via command
+              command_params:        # with params
+                expected_prompt: demo@
+                host: test.rebex.net
+                login: demo
+                password: password
+                set_timeout: False   # remote doesn't support: export TMOUT
+```
+
+We have remote machine in our config. Let's check if there is 'readme.txt' file
+on that machine (and some info about the file):
+
+```python
+
+    remote_unix = DeviceFactory.get_device(name='RebexTestMachine')  # it starts in local shell
+    remote_unix.goto_state(state="UNIX_REMOTE")                      # make it go to remote shell
+
+    ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
+
+    remote_files = ls_cmd()
+
+    if 'readme.txt' in remote_files['files']:
+        print("readme.txt file:")
+        readme_file_info = remote_files['files']['readme.txt']
+        for attr in readme_file_info:
+            print("  {:<18}: {}".format(attr, readme_file_info[attr]))
+```
+
+As you may noticed device is state machine. State transitions are defined inside
+configuration file under `CONNECTION_HOPS`. Please note, that it is only config file who
+knows "I need to use ssh to be on remote" - client code just says "go to remote".
+Thanks to that you can exchange "how to reach remote" without any change in main code.
+
+Above code displays:
+
+```bash
+
+    readme.txt file:
+      permissions       : -rw-------
+      hard_links_count  : 1
+      owner             : demo
+      group             : users
+      size_raw          : 403
+      size_bytes        : 403
+      date              : Apr 08  2014
+      name              : readme.txt
+```
+
+How about doing multiple things in parallel. Let's ping google
+while asking test.rebex.net about readme.txt file:
+
+```python
+my_unix = DeviceFactory.get_device(name='MyMachine')
+host = 'www.google.com'
+ping_cmd = my_unix.get_cmd(cmd_name="ping", cmd_params={"destination": host, "options": "-w 6"})
+
+remote_unix = DeviceFactory.get_device(name='RebexTestMachine')
+remote_unix.goto_state(state="UNIX_REMOTE")
+ls_cmd = remote_unix.get_cmd(cmd_name="ls", cmd_params={"options": "-l"})
+
+print("Start pinging {} ...".format(host))
+ping_cmd.start()                                # run command in background
+print("Let's check readme.txt at {} while pinging {} ...".format(remote_unix.name, host))
+
+remote_files = ls_cmd()                         # foreground "run in the meantime"
+file_info = remote_files['files']['readme.txt']
+print("readme.txt file: owner={fi[owner]}, size={fi[size_bytes]}".format(fi=file_info))
+
+ping_stats = ping_cmd.await_done(timeout=6)     # await background command
+print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
+                                          ping_stats['packet_loss'],
+                                          'time_avg',
+                                          ping_stats['time_avg'],
+                                          ping_stats['time_unit']))
+```
+
+```log
+Start pinging www.google.com ...
+Let's check readme.txt at RebexTestMachine while pinging www.google.com ...
+readme.txt file: owner=demo, size=403
+ping www.google.com: packet_loss=0, time_avg=35.251 [ms]
+```
+
+Besides being callable command-object works as "Future" (result promise).
+You can start it in background and later await till it is done to grab result.
+
+If we enhance our configuration with logging related info:
+
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+```
+
+then above code will automatically create Molers' main log (`moler.log`)
+which shows activity on all devices:
+
+```log
+22:30:19.723 INFO       moler               |More logs in: ./logs
+22:30:19.747 INFO       MyMachine           |Connection to: 'MyMachine' has been opened.
+22:30:19.748 INFO       MyMachine           |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.866 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:19.901 INFO       RebexTestMachine    |Connection to: 'RebexTestMachine' has been opened.
+22:30:19.901 INFO       RebexTestMachine    |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.919 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
+22:30:19.920 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:19.921 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
+22:30:19.921 INFO       RebexTestMachine    |TERM=xterm-mono ssh -l demo test.rebex.net
+22:30:20.763 INFO       RebexTestMachine    |*********
+22:30:20.909 INFO       RebexTestMachine    |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
+22:30:20.917 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ssh.Ssh' finished.
+22:30:20.919 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
+22:30:20.920 INFO       MyMachine           |ping www.google.com -w 6
+22:30:20.920 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
+22:30:20.922 INFO       RebexTestMachine    |ls -l
+22:30:20.985 INFO       RebexTestMachine    |Command 'moler.cmd.unix.ls.Ls' finished.
+22:30:26.968 INFO       MyMachine           |Command 'moler.cmd.unix.ping.Ping' finished.
+22:30:26.992 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+22:30:27.011 INFO       RebexTestMachine    |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
+22:30:27.032 INFO       MyMachine           |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+
+```
+
+As you may noticed main log shows code progress from high-level view - data
+on connections are not visible, just activity of commands running on devices.
+
+If you want to see in details what has happened on each device - you have it in device logs.
+Moler creates log per each device
+`moler.RebexTestMachine.log`:
+
+```log
+22:30:19.901  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.902 <|
+22:30:19.919  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('demo@')]' started.
+22:30:19.920  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:19.921  |Command 'moler.cmd.unix.ssh.Ssh':'TERM=xterm-mono ssh -l demo test.rebex.net' started.
+22:30:19.921 >|TERM=xterm-mono ssh -l demo test.rebex.net
+
+22:30:19.924 <|TERM=xterm-mono ssh -l demo test.rebex.net
+
+22:30:20.762 <|Password:
+22:30:20.763 >|*********
+22:30:20.763 <|
+
+22:30:20.908 <|Welcome to Rebex Virtual Shell!
+              |For a list of supported commands, type 'help'.
+              |demo@ETNA:/$
+22:30:20.909  |Changed state from 'UNIX_LOCAL' into 'UNIX_REMOTE'
+22:30:20.917  |Command 'moler.cmd.unix.ssh.Ssh' finished.
+22:30:20.920  |Command 'moler.cmd.unix.ls.Ls':'ls -l' started.
+22:30:20.922 >|ls -l
+
+22:30:20.974 <|ls -l
+
+22:30:20.978 <|drwx------ 2 demo users          0 Jul 26  2017 .
+
+22:30:20.979 <|drwx------ 2 demo users          0 Jul 26  2017 ..
+              |drwx------ 2 demo users          0 Dec 03  2015 aspnet_client
+              |drwx------ 2 demo users          0 Oct 27  2015 pub
+              |-rw------- 1 demo users        403 Apr 08  2014 readme.txt
+              |demo@ETNA:/$
+22:30:20.985  |Command 'moler.cmd.unix.ls.Ls' finished.
+22:30:26.992  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+22:30:27.011  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('demo@')]' finished.
+```
+
+and `moler.MyMachine.log`:
+
+```log
+22:30:19.748  |Changed state from 'NOT_CONNECTED' into 'UNIX_LOCAL'
+22:30:19.748 <|
+22:30:19.866  |Event 'moler.events.unix.wait4prompt.Wait4prompt':'[re.compile('^moler_bash#')]' started.
+22:30:20.919  |Command 'moler.cmd.unix.ping.Ping':'ping www.google.com -w 6' started.
+22:30:20.920 >|ping www.google.com -w 6
+
+22:30:20.921 <|ping www.google.com -w 6
+
+22:30:20.959 <|PING www.google.com (216.58.215.68) 56(84) bytes of data.
+22:30:20.960 <|
+
+22:30:21.000 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=1 ttl=51 time=40.1 ms
+22:30:21.001 <|
+
+22:30:21.992 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=2 ttl=51 time=31.0 ms
+
+22:30:22.999 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=3 ttl=51 time=36.5 ms
+
+22:30:23.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=4 ttl=51 time=31.4 ms
+
+22:30:24.996 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=5 ttl=51 time=29.8 ms
+
+22:30:26.010 <|64 bytes from waw02s16-in-f4.1e100.net (216.58.215.68): icmp_seq=6 ttl=51 time=42.4 ms
+
+22:30:26.960 <|
+              |--- www.google.com ping statistics ---
+              |6 packets transmitted, 6 received, 0% packet loss, time 5007ms
+              |rtt min/avg/max/mdev = 29.888/35.251/42.405/4.786 ms
+              |moler_bash#
+22:30:26.968  |Command 'moler.cmd.unix.ping.Ping' finished.
+22:30:27.032  |Event 'moler.events.unix.wait4prompt.Wait4prompt': '[re.compile('^moler_bash#')]' finished.
+```
+
+If the log files are too large you can split files.
+
+The log files can be split by size. For example let's assume we want split log files by 5 MB (5242880 bytes) and we want
+to keep maximum 999 files:
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: size
+        INTERVAL: 5242880
+        BACKUP_COUNT: 999  # Default value
+      
+
+```
+
+The log files can be split by time. For example let's assume we want split log files every 30 minutes (1800 seconds)
+ and we want to keep maximum 999 files (default value):
+ 
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: time
+        INTERVAL: 1800
+        BACKUP_COUNT: 999  # Default value
+```
+
+For space saving Moler can compress the logs after rotation. The external tool is used. Let's use the above examples
+to show how to compress logs:
+
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: size
+        INTERVAL: 5242880
+        BACKUP_COUNT: 999  # Default value
+        COMPRESS_AFTER_ROTATION: True  # Default is False
+        COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value
+        COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
+
+
+```
+
+```yaml
+    LOGGER:
+      PATH: ./logs
+      DATE_FORMAT: "%H:%M:%S"
+      LOG_ROTATION:
+        KIND: time
+        INTERVAL: 1800
+        BACKUP_COUNT: 999  # Default value
+        COMPRESS_COMMAND: "zip -9mq {compressed} {log_input}"  # Default value      
+        COMPRESSED_FILE_EXTENSION: ".zip"  # Default value
+```
+
+In a script we can also disable logging from device. Please use it very carefully. Investigation any issue may be
+ impossible if we don't have full logs.
+ 
+```python
+my_unix = DeviceFactory.get_device(name='MyMachine')
+
+my_unix.disbale_logging()  # to disable logging on device
+
+my_unix.enable_logging()  # to enable logging on device
+```
+
+In a script you can add suffix to all log files or only to files for specific devices. with disable logging from device. 
+ 
+```python
+from moler.config.loggers import change_logging_suffix
+change_logging_suffix(".suffix1")  # all log files with suffix
+change_logging_suffix(None)  # all log files without suffx
+
+my_unix = DeviceFactory.get_device(name='MyMachine')
+
+my_unix.set_logging_suffix("device_suffix")  # to add suffix to filename with logs
+
+my_unix.set_suffix(None)  # to remove suffix from filename with logs
+```
+
+Previous examples ask device to create command. We can also create command ourselves
+giving it connection to operate on:
+
+```python
+
+    import time
+    from moler.cmd.unix.ping import Ping
+    from moler.connection_factory import get_connection
+
+    host = 'www.google.com'
+    terminal = get_connection(io_type='terminal', variant='threaded')  # take connection
+    with terminal.open():
+        ping_cmd = Ping(connection=terminal.moler_connection,
+                        destination=host, options="-w 6")
+        print("Start pinging {} ...".format(host))
+        ping_cmd.start()
+        print("Doing other stuff while pinging {} ...".format(host))
+        time.sleep(3)
+        ping_stats = ping_cmd.await_done(timeout=4)
+        print("ping {}: {}={}, {}={} [{}]".format(host,'packet_loss',
+                                                  ping_stats['packet_loss'],
+                                                  'time_avg',
+                                                  ping_stats['time_avg'],
+                                                  ping_stats['time_unit']))
+```
+
+Please note also that connection is context manager doing open/close actions.
+
+
+```bash
+
+    Start pinging www.google.com ...
+    Doing other stuff while pinging www.google.com ...
+    ping www.google.com: packet_loss=0, time_avg=50.000 [ms]
+```
+
+## Reuse freedom
+Library gives you freedom which part you want to reuse. We are fan's of "take what you need only".
+* You may use configuration files or configure things by Python calls.
+
+   ```python
+   load_config(config={'DEVICES': {'MyMachine': {'DEVICE_CLASS': 'moler.device.unixlocal.UnixLocal'}}})
+   ```
+* You may use devices or create commands manually
+* You can take connection or build it yourself:
+
+   ```python
+   from moler.threaded_moler_connection import ThreadedMolerConnection
+   from moler.io.raw.terminal import ThreadedTerminal
+
+   terminal_connection = ThreadedTerminal(moler_connection=ThreadedMolerConnection())
+   ```
+* You can even install your own implementation in place of default implementation per connection type
+
+# API design reasoning
+The main goal of command is its usage simplicity: just run it and give me back its result.
+
+Command hides from its caller:
+* a way how it realizes "runs"
+* how it gets data of output to be parsed
+* how it parses that data
+
+Command shows to its caller:
+* API to start/stop it or await for its completion
+* API to query for its result or result readiness
+
+Command works as [Futures and promises](https://en.wikipedia.org/wiki/Futures_and_promises)
+
+After starting, we await for its result which is parsed out command output provided usually as dict.
+Running that command and parsing its output may take some time, so till that point result computation is yet incomplete.
+
+## Command as future
+* it starts some command on device/shell over connection
+  (as future-function starts it's execution)
+* it parses data incoming over such connection
+  (as future-function does it's processing)
+* it stores result of that parsing
+  (as future-function concludes in calculation result)
+* it provides means to return that result
+  (as future-function does via 'return' or 'yield' statement)
+* it's result is not ready "just-after" calling command
+  (as it is with future in contrast to function)
+
+So command should have future API.
+
+Quote from **_"Professional Python"_** by **Luke Sneeringer**:
+> The Future is a standalone object. It is independent of the actual function that is running.
+> It does nothing but store the state and result information.
+
+Command differs in that it is both:
+* function-like object performing computation
+* future-like object storing result of that computation.
+
+## Command vs. Connection-observer
+Command is just "active version" of connection observer.
+
+Connection observer is passive since it just observes connection for some data;
+data that may just asynchronously appear (alarms, reboots or anything you want).
+Intention here is split of responsibility: one observer is looking for alarms,
+another one for reboots.
+
+Command is active since it actively triggers some output on connection
+by sending command-string over that connection. So, it activates some action
+on device-behind-connection. That action is "command" in device terminology.
+Like `ping` on bash console/device. And it produces that "command" output.
+That output is what Moler's Command as connection-observer is looking for.
+
+## Most well known Python's futures
+* [concurrent.futures.Future](https://docs.python.org/3/library/concurrent.futures.html)
+* [asyncio.Future](https://docs.python.org/3/library/asyncio-task.html#future)
+
+| API                     | concurrent.futures.Future                   | asyncio.Future                                      |
+| :---------------------- | :------------------------------------------ | :-------------------------------------------------- |
+| storing result          | :white_check_mark: `set_result()`           | :white_check_mark: `set_result()`                   |
+| result retrieval        | :white_check_mark: `result()`               | :white_check_mark: `result()`                       |
+| storing failure cause   | :white_check_mark: `set_exception()`        | :white_check_mark: `set_exception()`                |
+| failure cause retrieval | :white_check_mark: `exception()`            | :white_check_mark: `exception()`                    |
+| stopping                | :white_check_mark: `cancel()`               | :white_check_mark: `cancel()`                       |
+| check if stopped        | :white_check_mark: `cancelled()`            | :white_check_mark: `cancelled()`                    |
+| check if running        | :white_check_mark: `running()`              | :no_entry_sign: `(but AbstractEventLoop.running())` |
+| check if completed      | :white_check_mark: `done()`                 | :white_check_mark: `done()`                         |
+| subscribe completion    | :white_check_mark: `add_done_callback()`    | :white_check_mark: `add_done_callback()`            |
+| unsubscribe completion  | :no_entry_sign:                             | :white_check_mark: `remove_done_callback()`         |
+
+Starting callable to be run "as future" is done by entities external to future-object
+
+| API              | concurrent.futures<br>start via Executor objects (thread/proc) | asyncio<br>start via module-lvl functions or ev-loop |
+| ---------------- | ---------------------------------------- | ---------------------------------------------- |
+| start callable   | submit(fn, *args, **kwargs)<br>Schedules callable to be executed as<br>fn(*args **kwargs) -> Future | ensure_future(coro_or_future) -> Task<br>future = run_coroutine_threadsafe(coro, loop) |
+| start same callable<br>on data iterator | map(fn, *iterables, timeout) -> iterator | join_future = asyncio.gather(*map(f, iterable))<br>loop.run_until_complete(join_future)|
+
+Awaiting completion of future is done by entities external to future-object
+
+| API               | concurrent.futures<br>awaiting by module level functions | asyncio<br>awaiting by module-lvl functions or ev-loop |
+| ----------------- | ------------------------------------------ | -------------------------------------------- |
+| await completion  |  done, not_done = wait(futures, timeout) -> futures | done, not_done = await wait(futures)<br>results = await gather(futures)<br>result = await future<br>result = yield from future<br>result = await coroutine<br>result = yield from coroutine<br>result = yield from wait_for(future, timeout)<br>loop.run_until_complete(future) -> blocking run |
+| process as they<br>complete | for done in as_completed(futures, timeout) -> futures | for done in as_completed(futures, timeout) -> futures |
+
+## Fundamental difference of command
+Contrary to **concurrent.futures** and **asyncio** we don't want command to be run by some external entity.
+We want it to be self-executable for usage simplicity.
+We want to take command and just say to it:
+* **"run"** or **"run in background"**
+* and not **"Hi, external runner, would you run/run-background that command for me"**
+
+# Designed API
+1. create command object
+``` python
+command = Command()
+```
+
+2. run it synchronously/blocking and get result in one shot behaves like function call since Command is callable.
+
+Run-as-callable gives big advantage since it fits well in python ecosystem.
+``` python
+result = command()
+```
+function example:
+``` python
+map(ping_cmd, all_machines_to_validate_reachability)
+```
+
+3. run it asynchronously/nonblocking
+``` python
+command_as_future = command.start()
+```
+
+4. shift from background to foreground
+
+**asyncio:** variant looks like:
+``` python
+result = await future
+done_futures, pending = yield from asyncio.wait(futures)
+result = yield from asyncio.wait_for(future, 60.0)
+```
+and **concurrent.futures** variant looks like:
+``` python
+done_futures, pending = wait(futures)
+```
+Moler's API maps to above well-known API
+``` python
+result = command.await_done(timeout)
+```
+* it is "internal" to command "Hi command, that is what I want from you" (above APIs say "Hi you there, that is what I want you to do with command")
+* it directly (Zen of Python) shows what we are awaiting for
+* timeout is required parameter (not as in concurrent.futures) since we don't expect endless execution of command (user must know what is worst case timeout to await command completion)
+
+# Video introduction
+You can [watch videos how to use Moler on YouTube](https://www.youtube.com/channel/UCgToo2qq8kLMyEgzd4btM9g).
```

