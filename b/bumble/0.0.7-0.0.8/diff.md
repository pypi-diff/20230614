# Comparing `tmp/bumble-0.0.7.tar.gz` & `tmp/bumble-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/boccongibod/Workspace/bumble/dist/tmph0_yv_11/bumble-0.0.7.tar", last modified: Tue Aug  2 01:09:47 2022, max compression
+gzip compressed data, was "/Users/boccongibod/Temp/bumble/dist/tmp3ks2wxdr/bumble-0.0.8.tar", last modified: Thu Aug  4 21:00:51 2022, max compression
```

## Comparing `bumble-0.0.7.tar` & `bumble-0.0.8.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:47.018878 bumble-0.0.7/
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.842675 bumble-0.0.7/.github/
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.855735 bumble-0.0.7/.github/workflows/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2724 2022-05-19 17:50:11.000000 bumble-0.0.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      857 2022-08-02 00:34:44.000000 bumble-0.0.7/.github/workflows/python-build-test.yml
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1271 2022-08-02 00:34:44.000000 bumble-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      163 2022-07-23 16:39:25.000000 bumble-0.0.7/.gitignore
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1103 2022-05-17 02:35:55.000000 bumble-0.0.7/CONTRIBUTING.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    11357 2022-05-17 02:35:55.000000 bumble-0.0.7/LICENSE
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      330 2022-08-02 01:09:47.019097 bumble-0.0.7/PKG-INFO
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2309 2022-08-01 23:40:44.000000 bumble-0.0.7/README.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.862461 bumble-0.0.7/apps/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1771 2022-05-17 02:35:55.000000 bumble-0.0.7/apps/README.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)        0 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/__init__.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    23794 2022-08-01 23:40:44.000000 bumble-0.0.7/apps/console.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4055 2022-07-27 01:01:05.000000 bumble-0.0.7/apps/controller_info.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2239 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/controllers.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4104 2022-07-23 16:39:25.000000 bumble-0.0.7/apps/gatt_dump.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8564 2022-07-25 05:15:40.000000 bumble-0.0.7/apps/gg_bridge.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3764 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/hci_bridge.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.863813 bumble-0.0.7/apps/link_relay/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)        0 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/link_relay/__init__.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     9920 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/link_relay/link_relay.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      311 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/link_relay/logging.yml
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    13331 2022-07-23 16:39:25.000000 bumble-0.0.7/apps/pair.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     6401 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/scan.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4226 2022-07-23 16:39:25.000000 bumble-0.0.7/apps/show.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2098 2022-05-17 02:27:37.000000 bumble-0.0.7/apps/unbond.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.885072 bumble-0.0.7/bumble/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)        0 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/__init__.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    19407 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/a2dp.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    25388 2022-07-23 16:39:25.000000 bumble-0.0.7/bumble/att.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    68956 2022-07-25 05:15:40.000000 bumble-0.0.7/bumble/avdtp.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3023 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/bridge.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    96008 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/company_ids.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    35218 2022-07-27 01:01:05.000000 bumble-0.0.7/bumble/controller.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    45293 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/core.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8018 2022-07-23 16:39:25.000000 bumble-0.0.7/bumble/crypto.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    62396 2022-08-01 23:40:44.000000 bumble-0.0.7/bumble/device.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2113 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/gap.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    22070 2022-08-01 23:40:44.000000 bumble-0.0.7/bumble/gatt.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    29541 2022-07-25 05:15:40.000000 bumble-0.0.7/bumble/gatt_client.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    28951 2022-08-01 23:40:44.000000 bumble-0.0.7/bumble/gatt_server.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)   176395 2022-08-01 23:40:44.000000 bumble-0.0.7/bumble/hci.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     8032 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/helpers.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3253 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/hfp.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    28038 2022-07-27 01:01:05.000000 bumble-0.0.7/bumble/host.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     8917 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/keys.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    44053 2022-07-25 05:15:40.000000 bumble-0.0.7/bumble/l2cap.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    15022 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/link.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.891895 bumble-0.0.7/bumble/profiles/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      581 2022-07-23 16:39:25.000000 bumble-0.0.7/bumble/profiles/__init__.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2251 2022-07-23 16:39:25.000000 bumble-0.0.7/bumble/profiles/battery_service.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5451 2022-07-23 16:39:25.000000 bumble-0.0.7/bumble/profiles/device_information_service.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8370 2022-07-27 01:01:05.000000 bumble-0.0.7/bumble/profiles/heart_rate_service.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    29494 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/rfcomm.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    41414 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/sdp.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    62253 2022-07-27 01:01:05.000000 bumble-0.0.7/bumble/smp.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.903730 bumble-0.0.7/bumble/transport/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3977 2022-07-13 15:49:58.000000 bumble-0.0.7/bumble/transport/__init__.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     4081 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/android_emulator.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    10775 2022-07-25 05:15:40.000000 bumble-0.0.7/bumble/transport/common.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2636 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/emulated_bluetooth_packets_pb2.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2662 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/emulated_bluetooth_pb2.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     9359 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/emulated_bluetooth_pb2_grpc.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2076 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/emulated_bluetooth_vhci_pb2.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     4660 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/emulated_bluetooth_vhci_pb2_grpc.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2024 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/file.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     5698 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/hci_socket.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2711 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/pty.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    11230 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/pyusb.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2438 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/serial.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1859 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/tcp_client.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3145 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/tcp_server.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2205 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/udp.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    13394 2022-07-23 16:39:25.000000 bumble-0.0.7/bumble/transport/usb.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2117 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/vhci.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1683 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/ws_client.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3194 2022-05-17 02:27:37.000000 bumble-0.0.7/bumble/transport/ws_server.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5080 2022-07-25 05:15:40.000000 bumble-0.0.7/bumble/utils.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.888968 bumble-0.0.7/bumble.egg-info/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      330 2022-08-02 01:09:46.000000 bumble-0.0.7/bumble.egg-info/PKG-INFO
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     6011 2022-08-02 01:09:46.000000 bumble-0.0.7/bumble.egg-info/SOURCES.txt
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)        1 2022-08-02 01:09:46.000000 bumble-0.0.7/bumble.egg-info/dependency_links.txt
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      361 2022-08-02 01:09:46.000000 bumble-0.0.7/bumble.egg-info/entry_points.txt
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      444 2022-08-02 01:09:46.000000 bumble-0.0.7/bumble.egg-info/requires.txt
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)        7 2022-08-02 01:09:46.000000 bumble-0.0.7/bumble.egg-info/top_level.txt
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.904345 bumble-0.0.7/docs/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1035 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/README.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.908977 bumble-0.0.7/docs/images/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    24591 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo.png
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3942 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo.svg
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.913428 bumble-0.0.7/docs/images/logo.vectornator/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    20743 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo.vectornator/Artboard0.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      580 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo.vectornator/Document.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      148 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo.vectornator/Manifest.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    42419 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo.vectornator/Thumbnail.png
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)   656936 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo.vectornator/UndoHistory.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    49038 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo_framed.png
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     4205 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo_framed.svg
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.920361 bumble-0.0.7/docs/images/logo_framed.vectornator/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    23333 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo_framed.vectornator/Artboard0.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      580 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo_framed.vectornator/Document.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      148 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo_framed.vectornator/Manifest.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    59364 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo_framed.vectornator/Thumbnail.png
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)   621306 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/images/logo_framed.vectornator/UndoHistory.json
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.925191 bumble-0.0.7/docs/mkdocs/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2516 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/mkdocs.yml
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      165 2022-05-17 03:05:24.000000 bumble-0.0.7/docs/mkdocs/requirements.txt
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.926419 bumble-0.0.7/docs/mkdocs/src/
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.928303 bumble-0.0.7/docs/mkdocs/src/api/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       25 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/api/examples.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       39 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/api/guide.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      251 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/api/reference.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.933819 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1002 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/console.md
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)       30 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/gatt_dump.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       37 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/gg_bridge.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1341 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/hci_bridge.md
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)      777 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/index.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1777 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/link_relay.md
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)       20 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/pair.md
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)       20 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/show.md
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)       24 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/apps_and_tools/unbond.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.939386 bumble-0.0.7/docs/mkdocs/src/components/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       21 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/components/controller.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)        9 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/components/gatt.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)        9 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/components/host.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       33 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/components/security_manager.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.940047 bumble-0.0.7/docs/mkdocs/src/development/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1525 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/development/python_environments.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.942943 bumble-0.0.7/docs/mkdocs/src/examples/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3154 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/examples/index.md
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4113 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/getting_started.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.943628 bumble-0.0.7/docs/mkdocs/src/hardware/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2254 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/hardware/index.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.959408 bumble-0.0.7/docs/mkdocs/src/images/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)   116095 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/images/bumble_layers.svg
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)   450055 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/images/console_screenshot.png
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    15406 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/images/favicon.ico
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    24591 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/images/logo.png
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    49038 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/images/logo_framed.png
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     8979 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/index.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.963153 bumble-0.0.7/docs/mkdocs/src/platforms/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4169 2022-07-23 16:39:25.000000 bumble-0.0.7/docs/mkdocs/src/platforms/android.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      639 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/platforms/index.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     5980 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/platforms/linux.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      474 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/platforms/macos.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1252 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/platforms/windows.md
--rwxr-xr-x   0 boccongibod (369378) primarygroup (89939)    67769 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/platforms/winusb_driver.png
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.972159 bumble-0.0.7/docs/mkdocs/src/transports/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1003 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/android_emulator.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      365 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/file.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      770 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/hci_socket.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1935 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/index.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      544 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/pty.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      427 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/serial.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      317 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/tcp_client.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      449 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/tcp_server.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      435 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/udp.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1213 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/usb.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      556 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/vhci.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      435 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/ws_client.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      435 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/transports/ws_server.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.976706 bumble-0.0.7/docs/mkdocs/src/use_cases/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      853 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/use_cases/index.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      794 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_1.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      789 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_2.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      737 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_3.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      672 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_4.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1226 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_5.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      939 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_6.md
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.846680 bumble-0.0.7/docs/mkdocs/theme/
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:46.977565 bumble-0.0.7/docs/mkdocs/theme/partials/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2197 2022-05-17 02:27:37.000000 bumble-0.0.7/docs/mkdocs/theme/partials/footer.html
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      152 2022-05-17 02:35:55.000000 bumble-0.0.7/environment.yml
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:47.009309 bumble-0.0.7/examples/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     4054 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/README.md
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       97 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/a2dp_sink1.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2699 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/async_runner.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2675 2022-08-01 23:40:44.000000 bumble-0.0.7/examples/battery_client.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2521 2022-07-27 01:01:05.000000 bumble-0.0.7/examples/battery_server.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       89 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/classic1.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       54 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/classic2.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      174 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/device1.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      263 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/device2.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       62 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/device3.json
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4060 2022-07-23 16:39:25.000000 bumble-0.0.7/examples/device_information_client.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2575 2022-07-23 16:39:25.000000 bumble-0.0.7/examples/device_information_server.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2826 2022-08-01 23:40:44.000000 bumble-0.0.7/examples/heart_rate_client.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3921 2022-07-27 01:01:05.000000 bumble-0.0.7/examples/heart_rate_server.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       63 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/hfp_gateway.json
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2487 2022-07-13 15:49:58.000000 bumble-0.0.7/examples/hfp_handsfree.html
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)       68 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/hfp_handsfree.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2315 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/keyboard.html
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      103 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/keyboard.json
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)    14712 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/keyboard.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     7516 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_a2dp_info.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     5824 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_a2dp_sink.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     6737 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_a2dp_source.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1833 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_advertiser.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3616 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_classic_connect.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     3825 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_classic_discoverable.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2706 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_classic_discovery.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2159 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_connect_and_encrypt.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3227 2022-07-23 16:39:25.000000 bumble-0.0.7/examples/run_controller.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2893 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_controller_with_scanner.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3654 2022-07-23 16:39:25.000000 bumble-0.0.7/examples/run_gatt_client.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4135 2022-07-23 16:39:25.000000 bumble-0.0.7/examples/run_gatt_client_and_server.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     5321 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_gatt_server.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     9271 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_hfp_gateway.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5713 2022-07-13 15:49:58.000000 bumble-0.0.7/examples/run_hfp_handsfree.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4485 2022-07-25 05:15:40.000000 bumble-0.0.7/examples/run_notifier.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8601 2022-07-25 05:15:40.000000 bumble-0.0.7/examples/run_rfcomm_client.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     4259 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_rfcomm_server.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2768 2022-05-17 02:27:37.000000 bumble-0.0.7/examples/run_scanner.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      703 2022-05-17 02:35:55.000000 bumble-0.0.7/noxfile.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      140 2022-06-11 19:26:05.000000 bumble-0.0.7/pyproject.toml
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1601 2022-08-02 01:09:47.019926 bumble-0.0.7/setup.cfg
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)      619 2022-05-17 02:35:55.000000 bumble-0.0.7/setup.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1424 2022-05-17 02:35:55.000000 bumble-0.0.7/tasks.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:47.016303 bumble-0.0.7/tests/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     8958 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/a2dp_test.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     4369 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/avdtp_test.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1926 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/core_test.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    15634 2022-07-23 16:39:25.000000 bumble-0.0.7/tests/gatt_test.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1944 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/hci_data_001.bin
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    14601 2022-07-27 01:01:05.000000 bumble-0.0.7/tests/hci_test.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1625 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/import_test.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)       48 2022-07-23 16:39:25.000000 bumble-0.0.7/tests/pytest.ini
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1713 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/rfcomm_test.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     4439 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/sdp_test.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)    12394 2022-08-01 23:40:44.000000 bumble-0.0.7/tests/self_test.py
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8093 2022-07-23 16:39:25.000000 bumble-0.0.7/tests/smp_test.py
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     2349 2022-05-17 02:27:37.000000 bumble-0.0.7/tests/transport_test.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:47.016909 bumble-0.0.7/utils/
--rw-rw-r--   0 boccongibod (369378) primarygroup (89939)     1719 2022-05-17 02:27:37.000000 bumble-0.0.7/utils/generate_company_id_list.py
-drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-02 01:09:47.018197 bumble-0.0.7/web/
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4387 2022-07-13 15:49:58.000000 bumble-0.0.7/web/index.html
--rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2227 2022-07-13 15:49:58.000000 bumble-0.0.7/web/scanner.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.200266 bumble-0.0.8/
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:50.983497 bumble-0.0.8/.github/
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.017861 bumble-0.0.8/.github/workflows/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2724 2022-08-04 20:58:19.000000 bumble-0.0.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      857 2022-08-04 20:58:19.000000 bumble-0.0.8/.github/workflows/python-build-test.yml
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1036 2022-08-04 20:59:56.000000 bumble-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      163 2022-08-04 20:58:19.000000 bumble-0.0.8/.gitignore
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1103 2022-08-04 20:58:19.000000 bumble-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    11357 2022-08-04 20:58:19.000000 bumble-0.0.8/LICENSE
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2680 2022-08-04 21:00:51.200707 bumble-0.0.8/PKG-INFO
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2309 2022-08-04 20:58:19.000000 bumble-0.0.8/README.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.025740 bumble-0.0.8/apps/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1771 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/README.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/__init__.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    23794 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/console.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4055 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/controller_info.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2239 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/controllers.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4104 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/gatt_dump.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8564 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/gg_bridge.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3764 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/hci_bridge.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.027512 bumble-0.0.8/apps/link_relay/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/link_relay/__init__.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     9920 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/link_relay/link_relay.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      311 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/link_relay/logging.yml
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    13331 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/pair.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     6401 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/scan.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4226 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/show.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2098 2022-08-04 20:58:19.000000 bumble-0.0.8/apps/unbond.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.056465 bumble-0.0.8/bumble/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/__init__.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    19407 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/a2dp.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    25388 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/att.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    68956 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/avdtp.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3023 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/bridge.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    96008 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/company_ids.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    35218 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/controller.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    45293 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/core.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8018 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/crypto.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    62396 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/device.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2113 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/gap.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    22451 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/gatt.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    29541 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/gatt_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    28955 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/gatt_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)   176452 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/hci.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8032 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/helpers.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3253 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/hfp.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    28038 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/host.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8917 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/keys.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    44053 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/l2cap.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    15022 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/link.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.063073 bumble-0.0.8/bumble/profiles/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      581 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/profiles/__init__.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2251 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/profiles/battery_service.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5451 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/profiles/device_information_service.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8370 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/profiles/heart_rate_service.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    29494 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/rfcomm.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    41414 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/sdp.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    62253 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/smp.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.077924 bumble-0.0.8/bumble/transport/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3977 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/__init__.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4081 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/android_emulator.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    10775 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/common.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2636 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/emulated_bluetooth_packets_pb2.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2662 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/emulated_bluetooth_pb2.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     9359 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/emulated_bluetooth_pb2_grpc.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2076 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/emulated_bluetooth_vhci_pb2.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4660 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/emulated_bluetooth_vhci_pb2_grpc.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2024 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/file.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5698 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/hci_socket.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2711 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/pty.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    11230 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/pyusb.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2438 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/serial.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1859 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/tcp_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3145 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/tcp_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2205 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/udp.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    13394 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/usb.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2117 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/vhci.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1683 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/ws_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3194 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/transport/ws_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5080 2022-08-04 20:58:19.000000 bumble-0.0.8/bumble/utils.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.060124 bumble-0.0.8/bumble.egg-info/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2680 2022-08-04 21:00:50.000000 bumble-0.0.8/bumble.egg-info/PKG-INFO
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     6011 2022-08-04 21:00:50.000000 bumble-0.0.8/bumble.egg-info/SOURCES.txt
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)        1 2022-08-04 21:00:50.000000 bumble-0.0.8/bumble.egg-info/dependency_links.txt
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      361 2022-08-04 21:00:50.000000 bumble-0.0.8/bumble.egg-info/entry_points.txt
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      444 2022-08-04 21:00:50.000000 bumble-0.0.8/bumble.egg-info/requires.txt
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)        7 2022-08-04 21:00:50.000000 bumble-0.0.8/bumble.egg-info/top_level.txt
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.078653 bumble-0.0.8/docs/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1035 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/README.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.084449 bumble-0.0.8/docs/images/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    24591 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo.png
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3942 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo.svg
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.090594 bumble-0.0.8/docs/images/logo.vectornator/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    20743 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo.vectornator/Artboard0.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      580 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo.vectornator/Document.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      148 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo.vectornator/Manifest.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    42419 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo.vectornator/Thumbnail.png
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)   656936 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo.vectornator/UndoHistory.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    49038 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo_framed.png
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4205 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo_framed.svg
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.098890 bumble-0.0.8/docs/images/logo_framed.vectornator/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    23333 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo_framed.vectornator/Artboard0.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      580 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo_framed.vectornator/Document.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      148 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo_framed.vectornator/Manifest.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    59364 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo_framed.vectornator/Thumbnail.png
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)   621306 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/images/logo_framed.vectornator/UndoHistory.json
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.104873 bumble-0.0.8/docs/mkdocs/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2516 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/mkdocs.yml
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      165 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/requirements.txt
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.106371 bumble-0.0.8/docs/mkdocs/src/
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.108699 bumble-0.0.8/docs/mkdocs/src/api/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       25 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/api/examples.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       39 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/api/guide.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      251 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/api/reference.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.118016 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1002 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/console.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       30 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/gatt_dump.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       37 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/gg_bridge.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1341 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/hci_bridge.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      777 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/index.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1777 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/link_relay.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       20 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/pair.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       20 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/show.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       24 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/apps_and_tools/unbond.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.121165 bumble-0.0.8/docs/mkdocs/src/components/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       21 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/components/controller.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)        9 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/components/gatt.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)        9 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/components/host.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       33 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/components/security_manager.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.121889 bumble-0.0.8/docs/mkdocs/src/development/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1525 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/development/python_environments.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.122622 bumble-0.0.8/docs/mkdocs/src/examples/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3154 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/examples/index.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4113 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/getting_started.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.124510 bumble-0.0.8/docs/mkdocs/src/hardware/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2254 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/hardware/index.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.133907 bumble-0.0.8/docs/mkdocs/src/images/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)   116095 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/images/bumble_layers.svg
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)   450055 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/images/console_screenshot.png
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    15406 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/images/favicon.ico
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    24591 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/images/logo.png
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    49038 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/images/logo_framed.png
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8979 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/index.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.140308 bumble-0.0.8/docs/mkdocs/src/platforms/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4169 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/platforms/android.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      639 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/platforms/index.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5980 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/platforms/linux.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      474 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/platforms/macos.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1252 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/platforms/windows.md
+-rwxr-xr-x   0 boccongibod (369378) primarygroup (89939)    67769 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/platforms/winusb_driver.png
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.151044 bumble-0.0.8/docs/mkdocs/src/transports/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1003 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/android_emulator.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      365 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/file.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      770 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/hci_socket.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1935 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/index.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      544 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/pty.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      427 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/serial.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      317 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/tcp_client.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      449 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/tcp_server.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      435 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/udp.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1213 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/usb.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      556 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/vhci.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      435 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/ws_client.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      435 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/transports/ws_server.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.159275 bumble-0.0.8/docs/mkdocs/src/use_cases/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      853 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/use_cases/index.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      794 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_1.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      789 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_2.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      737 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_3.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      672 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_4.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1226 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_5.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      939 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_6.md
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:50.987687 bumble-0.0.8/docs/mkdocs/theme/
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.160217 bumble-0.0.8/docs/mkdocs/theme/partials/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2197 2022-08-04 20:58:19.000000 bumble-0.0.8/docs/mkdocs/theme/partials/footer.html
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      152 2022-08-04 20:58:19.000000 bumble-0.0.8/environment.yml
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.187779 bumble-0.0.8/examples/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4054 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/README.md
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       97 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/a2dp_sink1.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2699 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/async_runner.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2675 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/battery_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2521 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/battery_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       89 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/classic1.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       54 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/classic2.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      174 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/device1.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      263 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/device2.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       62 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/device3.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4060 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/device_information_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2575 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/device_information_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2826 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/heart_rate_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3921 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/heart_rate_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       63 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/hfp_gateway.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2487 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/hfp_handsfree.html
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       68 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/hfp_handsfree.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2315 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/keyboard.html
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      103 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/keyboard.json
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    14712 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/keyboard.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     7516 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_a2dp_info.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5824 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_a2dp_sink.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     6737 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_a2dp_source.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1833 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_advertiser.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3616 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_classic_connect.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3825 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_classic_discoverable.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2706 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_classic_discovery.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2159 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_connect_and_encrypt.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3227 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_controller.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2893 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_controller_with_scanner.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     3654 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_gatt_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4135 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_gatt_client_and_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5321 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_gatt_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     9271 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_hfp_gateway.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     5713 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_hfp_handsfree.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4485 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_notifier.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8601 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_rfcomm_client.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4259 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_rfcomm_server.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2768 2022-08-04 20:58:19.000000 bumble-0.0.8/examples/run_scanner.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      703 2022-08-04 20:58:19.000000 bumble-0.0.8/noxfile.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      140 2022-08-04 20:58:19.000000 bumble-0.0.8/pyproject.toml
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1682 2022-08-04 21:00:51.202604 bumble-0.0.8/setup.cfg
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)      619 2022-08-04 20:58:19.000000 bumble-0.0.8/setup.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1424 2022-08-04 20:58:19.000000 bumble-0.0.8/tasks.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.197283 bumble-0.0.8/tests/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8958 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/a2dp_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4369 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/avdtp_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1926 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/core_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    15634 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/gatt_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1944 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/hci_data_001.bin
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    14601 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/hci_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1625 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/import_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)       48 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/pytest.ini
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1713 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/rfcomm_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4439 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/sdp_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)    13766 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/self_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     8093 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/smp_test.py
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2349 2022-08-04 20:58:19.000000 bumble-0.0.8/tests/transport_test.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.198016 bumble-0.0.8/utils/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     1719 2022-08-04 20:58:19.000000 bumble-0.0.8/utils/generate_company_id_list.py
+drwxr-xr-x   0 boccongibod (369378) primarygroup (89939)        0 2022-08-04 21:00:51.199557 bumble-0.0.8/web/
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     4387 2022-08-04 20:58:19.000000 bumble-0.0.8/web/index.html
+-rw-r--r--   0 boccongibod (369378) primarygroup (89939)     2227 2022-08-04 20:58:19.000000 bumble-0.0.8/web/scanner.py
```

### Comparing `bumble-0.0.7/.github/workflows/codeql-analysis.yml` & `bumble-0.0.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/.github/workflows/python-build-test.yml` & `bumble-0.0.8/.github/workflows/python-build-test.yml`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/.github/workflows/python-publish.yml` & `bumble-0.0.8/.github/workflows/python-publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -27,19 +27,13 @@
         python-version: '3.10'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
     - name: Build package
       run: python -m build
-    - name: Publish package to Test PyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: __token__
-        password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-        repository_url: https://test.pypi.org/legacy/
     - name: Publish package to PyPI
       if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `bumble-0.0.7/CONTRIBUTING.md` & `bumble-0.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/LICENSE` & `bumble-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/README.md` & `bumble-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/README.md` & `bumble-0.0.8/apps/README.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/console.py` & `bumble-0.0.8/apps/console.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/controller_info.py` & `bumble-0.0.8/apps/controller_info.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/controllers.py` & `bumble-0.0.8/apps/controllers.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/gatt_dump.py` & `bumble-0.0.8/apps/gatt_dump.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/gg_bridge.py` & `bumble-0.0.8/apps/gg_bridge.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/hci_bridge.py` & `bumble-0.0.8/apps/hci_bridge.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/link_relay/link_relay.py` & `bumble-0.0.8/apps/link_relay/link_relay.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/pair.py` & `bumble-0.0.8/apps/pair.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/scan.py` & `bumble-0.0.8/apps/scan.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/show.py` & `bumble-0.0.8/apps/show.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/apps/unbond.py` & `bumble-0.0.8/apps/unbond.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/a2dp.py` & `bumble-0.0.8/bumble/a2dp.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/att.py` & `bumble-0.0.8/bumble/att.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/avdtp.py` & `bumble-0.0.8/bumble/avdtp.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/bridge.py` & `bumble-0.0.8/bumble/bridge.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/company_ids.py` & `bumble-0.0.8/bumble/company_ids.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/controller.py` & `bumble-0.0.8/bumble/controller.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/core.py` & `bumble-0.0.8/bumble/core.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/crypto.py` & `bumble-0.0.8/bumble/crypto.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/device.py` & `bumble-0.0.8/bumble/device.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/gap.py` & `bumble-0.0.8/bumble/gap.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/gatt.py` & `bumble-0.0.8/bumble/gatt.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,20 @@
 
         if hasattr(self.wrapped_characteristic, 'subscribe'):
             self.subscribe = self.wrapped_subscribe
 
     def __getattr__(self, name):
         return getattr(self.wrapped_characteristic, name)
 
+    def __setattr__(self, name, value):
+        if name in {'wrapped_characteristic', 'read_value', 'write_value', 'subscribe'}:
+            super().__setattr__(name, value)
+        else:
+            setattr(self.wrapped_characteristic, name, value)
+
     def read_encoded_value(self, connection):
         return self.encode_value(self.wrapped_characteristic.read_value(connection))
 
     def write_encoded_value(self, connection, value):
         return self.wrapped_characteristic.write_value(connection, self.decode_value(value))
 
     async def read_decoded_value(self):
@@ -339,14 +345,18 @@
         return value
 
     def wrapped_subscribe(self, subscriber=None):
         return self.wrapped_characteristic.subscribe(
             None if subscriber is None else lambda value: subscriber(self.decode_value(value))
         )
 
+    def __str__(self):
+        wrapped = str(self.wrapped_characteristic)
+        return f'{self.__class__.__name__}({wrapped})'
+
 
 # -----------------------------------------------------------------------------
 class DelegatedCharacteristicAdapter(CharacteristicAdapter):
     '''
     Adapter that converts bytes values using an encode and a decode function.
     '''
     def __init__(self, characteristic, encode=None, decode=None):
```

### Comparing `bumble-0.0.7/bumble/gatt_client.py` & `bumble-0.0.8/bumble/gatt_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/gatt_server.py` & `bumble-0.0.8/bumble/gatt_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,21 +541,21 @@
 
         if attribute := self.get_attribute(request.attribute_handle):
             # TODO: check permissions
             mtu = self.get_mtu(connection)
             value = attribute.read_value(connection)
             if request.value_offset > len(value):
                 response = ATT_Error_Response(
-                    request_opcode_in_error = request.op_code,
+                    request_opcode_in_error   = request.op_code,
                     attribute_handle_in_error = request.attribute_handle,
                     error_code                = ATT_INVALID_OFFSET_ERROR
                 )
             elif len(value) <= mtu - 1:
                 response = ATT_Error_Response(
-                    request_opcode_in_error = request.op_code,
+                    request_opcode_in_error   = request.op_code,
                     attribute_handle_in_error = request.attribute_handle,
                     error_code                = ATT_ATTRIBUTE_NOT_LONG_ERROR
                 )
             else:
                 part_size = min(mtu - 1, len(value) - request.value_offset)
                 response = ATT_Read_Blob_Response(
                     part_attribute_value = value[request.value_offset:request.value_offset + part_size]
```

### Comparing `bumble-0.0.7/bumble/hci.py` & `bumble-0.0.8/bumble/hci.py`

 * *Files 0% similar despite different names*

```diff
@@ -3272,14 +3272,17 @@
         self.event_code = event_code
         self.parameters = parameters
 
     def to_bytes(self):
         parameters = b'' if self.parameters is None else self.parameters
         return bytes([HCI_EVENT_PACKET, self.event_code, len(parameters)]) + parameters
 
+    def __bytes__(self):
+        return self.to_bytes()
+
     def __str__(self):
         result = color(self.name, 'magenta')
         if fields := getattr(self, 'fields', None):
             result += ':\n' + HCI_Object.format_fields(self.__dict__, fields, '  ')
         else:
             if self.parameters:
                 result += f': {self.parameters.hex()}'
```

### Comparing `bumble-0.0.7/bumble/helpers.py` & `bumble-0.0.8/bumble/helpers.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/hfp.py` & `bumble-0.0.8/bumble/hfp.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/host.py` & `bumble-0.0.8/bumble/host.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/keys.py` & `bumble-0.0.8/bumble/keys.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/l2cap.py` & `bumble-0.0.8/bumble/l2cap.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/link.py` & `bumble-0.0.8/bumble/link.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/profiles/__init__.py` & `bumble-0.0.8/bumble/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/profiles/battery_service.py` & `bumble-0.0.8/bumble/profiles/battery_service.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/profiles/device_information_service.py` & `bumble-0.0.8/bumble/profiles/device_information_service.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/profiles/heart_rate_service.py` & `bumble-0.0.8/bumble/profiles/heart_rate_service.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/rfcomm.py` & `bumble-0.0.8/bumble/rfcomm.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/sdp.py` & `bumble-0.0.8/bumble/sdp.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/smp.py` & `bumble-0.0.8/bumble/smp.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/__init__.py` & `bumble-0.0.8/bumble/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/android_emulator.py` & `bumble-0.0.8/bumble/transport/android_emulator.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/common.py` & `bumble-0.0.8/bumble/transport/common.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/emulated_bluetooth_packets_pb2.py` & `bumble-0.0.8/bumble/transport/emulated_bluetooth_packets_pb2.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/emulated_bluetooth_pb2.py` & `bumble-0.0.8/bumble/transport/emulated_bluetooth_pb2.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/emulated_bluetooth_pb2_grpc.py` & `bumble-0.0.8/bumble/transport/emulated_bluetooth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/emulated_bluetooth_vhci_pb2.py` & `bumble-0.0.8/bumble/transport/emulated_bluetooth_vhci_pb2.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/emulated_bluetooth_vhci_pb2_grpc.py` & `bumble-0.0.8/bumble/transport/emulated_bluetooth_vhci_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/file.py` & `bumble-0.0.8/bumble/transport/file.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/hci_socket.py` & `bumble-0.0.8/bumble/transport/hci_socket.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/pty.py` & `bumble-0.0.8/bumble/transport/pty.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/pyusb.py` & `bumble-0.0.8/bumble/transport/pyusb.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/serial.py` & `bumble-0.0.8/bumble/transport/serial.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/tcp_client.py` & `bumble-0.0.8/bumble/transport/tcp_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/tcp_server.py` & `bumble-0.0.8/bumble/transport/tcp_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/udp.py` & `bumble-0.0.8/bumble/transport/udp.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/usb.py` & `bumble-0.0.8/bumble/transport/usb.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/vhci.py` & `bumble-0.0.8/bumble/transport/vhci.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/ws_client.py` & `bumble-0.0.8/bumble/transport/ws_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/transport/ws_server.py` & `bumble-0.0.8/bumble/transport/ws_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble/utils.py` & `bumble-0.0.8/bumble/utils.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/bumble.egg-info/SOURCES.txt` & `bumble-0.0.8/bumble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/README.md` & `bumble-0.0.8/docs/README.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo.png` & `bumble-0.0.8/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo.svg` & `bumble-0.0.8/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo.vectornator/Artboard0.json` & `bumble-0.0.8/docs/images/logo.vectornator/Artboard0.json`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo.vectornator/Document.json` & `bumble-0.0.8/docs/images/logo.vectornator/Document.json`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo.vectornator/Thumbnail.png` & `bumble-0.0.8/docs/images/logo.vectornator/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo.vectornator/UndoHistory.json` & `bumble-0.0.8/docs/images/logo.vectornator/UndoHistory.json`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo_framed.png` & `bumble-0.0.8/docs/images/logo_framed.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo_framed.svg` & `bumble-0.0.8/docs/images/logo_framed.svg`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo_framed.vectornator/Artboard0.json` & `bumble-0.0.8/docs/images/logo_framed.vectornator/Artboard0.json`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo_framed.vectornator/Document.json` & `bumble-0.0.8/docs/images/logo_framed.vectornator/Document.json`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo_framed.vectornator/Thumbnail.png` & `bumble-0.0.8/docs/images/logo_framed.vectornator/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/images/logo_framed.vectornator/UndoHistory.json` & `bumble-0.0.8/docs/images/logo_framed.vectornator/UndoHistory.json`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/mkdocs.yml` & `bumble-0.0.8/docs/mkdocs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/apps_and_tools/console.md` & `bumble-0.0.8/docs/mkdocs/src/apps_and_tools/console.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/apps_and_tools/hci_bridge.md` & `bumble-0.0.8/docs/mkdocs/src/apps_and_tools/hci_bridge.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/apps_and_tools/index.md` & `bumble-0.0.8/docs/mkdocs/src/apps_and_tools/index.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/apps_and_tools/link_relay.md` & `bumble-0.0.8/docs/mkdocs/src/apps_and_tools/link_relay.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/development/python_environments.md` & `bumble-0.0.8/docs/mkdocs/src/development/python_environments.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/examples/index.md` & `bumble-0.0.8/docs/mkdocs/src/examples/index.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/getting_started.md` & `bumble-0.0.8/docs/mkdocs/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/hardware/index.md` & `bumble-0.0.8/docs/mkdocs/src/hardware/index.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/images/bumble_layers.svg` & `bumble-0.0.8/docs/mkdocs/src/images/bumble_layers.svg`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/images/console_screenshot.png` & `bumble-0.0.8/docs/mkdocs/src/images/console_screenshot.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/images/favicon.ico` & `bumble-0.0.8/docs/mkdocs/src/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/images/logo.png` & `bumble-0.0.8/docs/mkdocs/src/images/logo.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/images/logo_framed.png` & `bumble-0.0.8/docs/mkdocs/src/images/logo_framed.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/index.md` & `bumble-0.0.8/docs/mkdocs/src/index.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/platforms/android.md` & `bumble-0.0.8/docs/mkdocs/src/platforms/android.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/platforms/index.md` & `bumble-0.0.8/docs/mkdocs/src/platforms/index.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/platforms/linux.md` & `bumble-0.0.8/docs/mkdocs/src/platforms/linux.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/platforms/windows.md` & `bumble-0.0.8/docs/mkdocs/src/platforms/windows.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/platforms/winusb_driver.png` & `bumble-0.0.8/docs/mkdocs/src/platforms/winusb_driver.png`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/transports/android_emulator.md` & `bumble-0.0.8/docs/mkdocs/src/transports/android_emulator.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/transports/hci_socket.md` & `bumble-0.0.8/docs/mkdocs/src/transports/hci_socket.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/transports/index.md` & `bumble-0.0.8/docs/mkdocs/src/transports/index.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/transports/pty.md` & `bumble-0.0.8/docs/mkdocs/src/transports/pty.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/transports/usb.md` & `bumble-0.0.8/docs/mkdocs/src/transports/usb.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/transports/vhci.md` & `bumble-0.0.8/docs/mkdocs/src/transports/vhci.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/use_cases/index.md` & `bumble-0.0.8/docs/mkdocs/src/use_cases/index.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_1.md` & `bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_1.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_2.md` & `bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_2.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_3.md` & `bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_3.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_4.md` & `bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_4.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_5.md` & `bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_5.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/src/use_cases/use_case_6.md` & `bumble-0.0.8/docs/mkdocs/src/use_cases/use_case_6.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/docs/mkdocs/theme/partials/footer.html` & `bumble-0.0.8/docs/mkdocs/theme/partials/footer.html`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/README.md` & `bumble-0.0.8/examples/README.md`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/async_runner.py` & `bumble-0.0.8/examples/async_runner.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/battery_client.py` & `bumble-0.0.8/examples/battery_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/battery_server.py` & `bumble-0.0.8/examples/battery_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/device_information_client.py` & `bumble-0.0.8/examples/device_information_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/device_information_server.py` & `bumble-0.0.8/examples/device_information_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/heart_rate_client.py` & `bumble-0.0.8/examples/heart_rate_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/heart_rate_server.py` & `bumble-0.0.8/examples/heart_rate_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/hfp_handsfree.html` & `bumble-0.0.8/examples/hfp_handsfree.html`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/keyboard.html` & `bumble-0.0.8/examples/keyboard.html`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/keyboard.py` & `bumble-0.0.8/examples/keyboard.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_a2dp_info.py` & `bumble-0.0.8/examples/run_a2dp_info.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_a2dp_sink.py` & `bumble-0.0.8/examples/run_a2dp_sink.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_a2dp_source.py` & `bumble-0.0.8/examples/run_a2dp_source.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_advertiser.py` & `bumble-0.0.8/examples/run_advertiser.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_classic_connect.py` & `bumble-0.0.8/examples/run_classic_connect.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_classic_discoverable.py` & `bumble-0.0.8/examples/run_classic_discoverable.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_classic_discovery.py` & `bumble-0.0.8/examples/run_classic_discovery.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_connect_and_encrypt.py` & `bumble-0.0.8/examples/run_connect_and_encrypt.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_controller.py` & `bumble-0.0.8/examples/run_controller.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_controller_with_scanner.py` & `bumble-0.0.8/examples/run_controller_with_scanner.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_gatt_client.py` & `bumble-0.0.8/examples/run_gatt_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_gatt_client_and_server.py` & `bumble-0.0.8/examples/run_gatt_client_and_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_gatt_server.py` & `bumble-0.0.8/examples/run_gatt_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_hfp_gateway.py` & `bumble-0.0.8/examples/run_hfp_gateway.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_hfp_handsfree.py` & `bumble-0.0.8/examples/run_hfp_handsfree.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_notifier.py` & `bumble-0.0.8/examples/run_notifier.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_rfcomm_client.py` & `bumble-0.0.8/examples/run_rfcomm_client.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_rfcomm_server.py` & `bumble-0.0.8/examples/run_rfcomm_server.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/examples/run_scanner.py` & `bumble-0.0.8/examples/run_scanner.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/noxfile.py` & `bumble-0.0.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/setup.cfg` & `bumble-0.0.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [metadata]
 name = bumble
 use_scm_version = True
 description = Bluetooth Stack for Apps, Emulation, Test and Experimentation
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = Google
 author_email = tbd@tbd.com
 url = https://github.com/google/bumble
 
 [options]
 python_requires = >=3.8
 packages = bumble, bumble.transport, bumble.apps, bumble.apps.link_relay
```

### Comparing `bumble-0.0.7/setup.py` & `bumble-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tasks.py` & `bumble-0.0.8/tasks.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/a2dp_test.py` & `bumble-0.0.8/tests/a2dp_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/avdtp_test.py` & `bumble-0.0.8/tests/avdtp_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/core_test.py` & `bumble-0.0.8/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/gatt_test.py` & `bumble-0.0.8/tests/gatt_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/hci_data_001.bin` & `bumble-0.0.8/tests/hci_data_001.bin`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/hci_test.py` & `bumble-0.0.8/tests/hci_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/import_test.py` & `bumble-0.0.8/tests/import_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/rfcomm_test.py` & `bumble-0.0.8/tests/rfcomm_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/sdp_test.py` & `bumble-0.0.8/tests/sdp_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/self_test.py` & `bumble-0.0.8/tests/self_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,14 +160,52 @@
     assert(c.uuid == c1.uuid)
     result = await peer.read_value(c)
     assert(result is not None)
     assert(result == c1.value)
 
 
 # -----------------------------------------------------------------------------
+@pytest.mark.asyncio
+async def test_self_gatt_long_read():
+    # Create two devices, each with a controller, attached to the same link
+    two_devices = TwoDevices()
+
+    # Add some GATT characteristics to device 1
+    characteristics = [
+        Characteristic(
+            f'3A143AD7-D4A7-436B-97D6-5B62C315{i:04X}',
+            Characteristic.READ,
+            Characteristic.READABLE,
+            bytes([x & 255 for x in range(i)])
+        )
+        for i in range(0, 513)
+    ]
+
+    service = Service('8140E247-04F0-42C1-BC34-534C344DAFCA', characteristics)
+    two_devices.devices[1].add_service(service)
+
+    # Start
+    await two_devices.devices[0].power_on()
+    await two_devices.devices[1].power_on()
+
+    # Connect the two devices
+    connection = await two_devices.devices[0].connect(two_devices.devices[1].random_address)
+    peer = Peer(connection)
+
+    result = await peer.discover_service(service.uuid)
+    assert(len(result) == 1)
+    found_service = result[0]
+    found_characteristics = await found_service.discover_characteristics()
+    assert(len(found_characteristics) == 513)
+    for (i, characteristic) in enumerate(found_characteristics):
+        value = await characteristic.read_value()
+        assert(value == characteristics[i].value)
+
+
+# -----------------------------------------------------------------------------
 async def _test_self_smp_with_configs(pairing_config1, pairing_config2):
     # Create two devices, each with a controller, attached to the same link
     two_devices = TwoDevices()
 
     # Start
     await two_devices.devices[0].power_on()
     await two_devices.devices[1].power_on()
@@ -270,15 +308,15 @@
             if pairing_config2:
                 pairing_config2.delegate.reset()
             if pairing_config1 and pairing_config2:
                 pairing_config1.delegate.peer_delegate = pairing_config2.delegate
                 pairing_config2.delegate.peer_delegate = pairing_config1.delegate
 
             await _test_self_smp_with_configs(pairing_config1, pairing_config2)
-            
+
 
 
 # -----------------------------------------------------------------------------
 @pytest.mark.asyncio
 async def test_self_smp_reject():
     class RejectingDelegate(PairingDelegate):
         def __init__(self):
@@ -319,14 +357,15 @@
     assert(not paired)
 
 
 # -----------------------------------------------------------------------------
 async def run_test_self():
     await test_self_connection()
     await test_self_gatt()
+    await test_self_gatt_long_read()
     await test_self_smp()
     await test_self_smp_reject()
     await test_self_smp_wrong_pin()
 
 # -----------------------------------------------------------------------------
 if __name__ == '__main__':
     logging.basicConfig(level = os.environ.get('BUMBLE_LOGLEVEL', 'INFO').upper())
```

### Comparing `bumble-0.0.7/tests/smp_test.py` & `bumble-0.0.8/tests/smp_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/tests/transport_test.py` & `bumble-0.0.8/tests/transport_test.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/utils/generate_company_id_list.py` & `bumble-0.0.8/utils/generate_company_id_list.py`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/web/index.html` & `bumble-0.0.8/web/index.html`

 * *Files identical despite different names*

### Comparing `bumble-0.0.7/web/scanner.py` & `bumble-0.0.8/web/scanner.py`

 * *Files identical despite different names*

