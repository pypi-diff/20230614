# Comparing `tmp/boxjelly-0.3.2.tar.gz` & `tmp/boxjelly-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxjelly-0.3.2.tar", max compression
+gzip compressed data, was "boxjelly-0.3.3.tar", max compression
```

## Comparing `boxjelly-0.3.2.tar` & `boxjelly-0.3.3.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.947233 boxjelly-0.3.2/boxjelly/__init__.py
--rw-r--r--   0        0        0      593 2022-06-24 17:58:30.916629 boxjelly-0.3.2/boxjelly/assets/assets.qrc
--rw-r--r--   0        0        0    11346 2022-06-13 22:35:25.947233 boxjelly-0.3.2/boxjelly/assets/icons/boxjelly.svg
--rw-r--r--   0        0        0    11845 2022-06-13 22:35:25.947233 boxjelly-0.3.2/boxjelly/assets/icons/boxjelly_logo.svg
--rw-r--r--   0        0        0      802 2022-06-24 16:29:45.779955 boxjelly-0.3.2/boxjelly/assets/icons/delete.png
--rw-r--r--   0        0        0      559 2022-06-24 16:29:45.780955 boxjelly-0.3.2/boxjelly/assets/icons/merge.png
--rw-r--r--   0        0        0      723 2022-06-24 16:29:45.781955 boxjelly-0.3.2/boxjelly/assets/icons/redo.png
--rw-r--r--   0        0        0      642 2022-06-24 16:29:45.782955 boxjelly-0.3.2/boxjelly/assets/icons/rename.png
--rw-r--r--   0        0        0      411 2022-06-24 16:29:45.783955 boxjelly-0.3.2/boxjelly/assets/icons/seek_beginning.png
--rw-r--r--   0        0        0      432 2022-06-24 16:29:45.783955 boxjelly-0.3.2/boxjelly/assets/icons/seek_end.png
--rw-r--r--   0        0        0      528 2022-06-24 16:29:45.784955 boxjelly-0.3.2/boxjelly/assets/icons/split.png
--rw-r--r--   0        0        0      699 2022-06-24 16:29:45.785955 boxjelly-0.3.2/boxjelly/assets/icons/undo.png
--rw-r--r--   0        0        0    76791 2022-06-13 22:35:25.947233 boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_1024.png
--rw-r--r--   0        0        0     8507 2022-06-13 22:35:25.947233 boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_128.png
--rw-r--r--   0        0        0    17271 2022-06-13 22:35:25.947233 boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_256.png
--rw-r--r--   0        0        0    36237 2022-06-13 22:35:25.947233 boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_512.png
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.957255 boxjelly-0.3.2/boxjelly/commands/__init__.py
--rw-r--r--   0        0        0     8553 2022-06-24 17:01:21.967322 boxjelly-0.3.2/boxjelly/commands/TrackListCommand.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.957255 boxjelly-0.3.2/boxjelly/delegates/__init__.py
--rw-r--r--   0        0        0     1700 2022-06-22 19:45:05.166534 boxjelly-0.3.2/boxjelly/delegates/TrackHeadersDelegate.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.957255 boxjelly-0.3.2/boxjelly/lib/__init__.py
--rw-r--r--   0        0        0      418 2022-06-24 17:01:21.969323 boxjelly-0.3.2/boxjelly/lib/constants.py
--rw-r--r--   0        0        0    12073 2022-06-24 17:01:21.970322 boxjelly-0.3.2/boxjelly/lib/fileio.py
--rw-r--r--   0        0        0    26595 2022-06-24 17:58:30.917629 boxjelly-0.3.2/boxjelly/lib/resources.py
--rw-r--r--   0        0        0     2735 2022-06-24 16:27:08.379852 boxjelly-0.3.2/boxjelly/lib/settings.py
--rw-r--r--   0        0        0      869 2022-06-14 18:35:03.706395 boxjelly-0.3.2/boxjelly/lib/track.py
--rw-r--r--   0        0        0      420 2022-06-22 19:45:05.171535 boxjelly-0.3.2/boxjelly/lib/util.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.957255 boxjelly-0.3.2/boxjelly/models/__init__.py
--rw-r--r--   0        0        0    16492 2022-06-24 16:03:14.431370 boxjelly-0.3.2/boxjelly/models/TrackListModel.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.957255 boxjelly-0.3.2/boxjelly/scripts/__init__.py
--rw-r--r--   0        0        0     1947 2022-06-24 17:58:30.918629 boxjelly-0.3.2/boxjelly/scripts/run.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.967356 boxjelly-0.3.2/boxjelly/ui/__init__.py
--rw-r--r--   0        0        0     1351 2022-06-22 19:45:05.175533 boxjelly-0.3.2/boxjelly/ui/FileSelector.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.967356 boxjelly-0.3.2/boxjelly/ui/graphicsitems/__init__.py
--rw-r--r--   0        0        0     2771 2022-06-22 19:45:05.183534 boxjelly-0.3.2/boxjelly/ui/graphicsitems/TimelineTrack.py
--rw-r--r--   0        0        0    14639 2022-06-24 17:58:30.919629 boxjelly-0.3.2/boxjelly/ui/MainWindow.py
--rw-r--r--   0        0        0     1140 2022-06-22 19:45:05.177533 boxjelly-0.3.2/boxjelly/ui/MediaSelectionBox.py
--rw-r--r--   0        0        0     1450 2022-06-24 16:29:45.790955 boxjelly-0.3.2/boxjelly/ui/OpenDialog.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.967356 boxjelly-0.3.2/boxjelly/ui/settings/__init__.py
--rw-r--r--   0        0        0     3013 2022-06-24 17:01:21.975322 boxjelly-0.3.2/boxjelly/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.977377 boxjelly-0.3.2/boxjelly/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0      898 2022-06-22 19:45:05.185534 boxjelly-0.3.2/boxjelly/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0     4379 2022-06-24 16:03:14.438520 boxjelly-0.3.2/boxjelly/ui/settings/tabs/NetworkSettingsTab.py
--rw-r--r--   0        0        0     1156 2022-06-22 19:45:05.187533 boxjelly-0.3.2/boxjelly/ui/settings/tabs/VideoSettingsTab.py
--rw-r--r--   0        0        0     5481 2022-06-24 17:01:21.973322 boxjelly-0.3.2/boxjelly/ui/SourceWidgets.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.977377 boxjelly-0.3.2/boxjelly/ui/track/__init__.py
--rw-r--r--   0        0        0     4373 2022-06-24 17:01:21.977322 boxjelly-0.3.2/boxjelly/ui/track/Timeline.py
--rw-r--r--   0        0        0    10673 2022-06-24 17:01:21.978322 boxjelly-0.3.2/boxjelly/ui/track/TrackGraphicsView.py
--rw-r--r--   0        0        0      874 2022-06-22 19:45:05.191533 boxjelly-0.3.2/boxjelly/ui/track/TrackHeadersView.py
--rw-r--r--   0        0        0     2510 2022-06-22 19:45:05.192535 boxjelly-0.3.2/boxjelly/ui/track/TrackPanel.py
--rw-r--r--   0        0        0     1297 2022-06-24 17:01:21.974322 boxjelly-0.3.2/boxjelly/ui/TrackSelectionBox.py
--rw-r--r--   0        0        0        0 2022-06-13 22:35:25.977377 boxjelly-0.3.2/boxjelly/ui/video/__init__.py
--rw-r--r--   0        0        0     6074 2022-06-22 19:45:05.193534 boxjelly-0.3.2/boxjelly/ui/video/CthulhuVideoController.py
--rw-r--r--   0        0        0     1711 2022-06-22 19:45:05.182535 boxjelly-0.3.2/boxjelly/ui/WidgetComboBox.py
--rw-r--r--   0        0        0     1085 2022-06-13 19:36:19.654399 boxjelly-0.3.2/LICENSE
--rw-r--r--   0        0        0      537 2022-06-24 17:58:30.920630 boxjelly-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1279 2022-06-24 17:58:30.914629 boxjelly-0.3.2/README.md
--rw-r--r--   0        0        0     2455 2022-06-24 17:58:51.553697 boxjelly-0.3.2/setup.py
--rw-r--r--   0        0        0     1925 2022-06-24 17:58:51.553697 boxjelly-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-01-25 18:58:58.749648 boxjelly-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1226 2023-01-25 18:58:58.749648 boxjelly-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/__init__.py
+-rw-r--r--   0        0        0      580 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/assets.qrc
+-rw-r--r--   0        0        0    11165 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/boxjelly.svg
+-rw-r--r--   0        0        0    11651 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/boxjelly_logo.svg
+-rw-r--r--   0        0        0      802 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/delete.png
+-rw-r--r--   0        0        0      559 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/merge.png
+-rw-r--r--   0        0        0      723 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/redo.png
+-rw-r--r--   0        0        0      642 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/rename.png
+-rw-r--r--   0        0        0      411 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/seek_beginning.png
+-rw-r--r--   0        0        0      432 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/seek_end.png
+-rw-r--r--   0        0        0      528 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/split.png
+-rw-r--r--   0        0        0      699 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/icons/undo.png
+-rw-r--r--   0        0        0    76791 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_1024.png
+-rw-r--r--   0        0        0     8507 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_128.png
+-rw-r--r--   0        0        0    17271 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_256.png
+-rw-r--r--   0        0        0    36237 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_512.png
+-rw-r--r--   0        0        0     8339 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/commands/TrackListCommand.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/commands/__init__.py
+-rw-r--r--   0        0        0     1658 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/delegates/TrackHeadersDelegate.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/delegates/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/lib/__init__.py
+-rw-r--r--   0        0        0      398 2023-06-14 16:17:31.605023 boxjelly-0.3.3/boxjelly/lib/constants.py
+-rw-r--r--   0        0        0    11737 2023-06-14 16:17:31.605023 boxjelly-0.3.3/boxjelly/lib/fileio.py
+-rw-r--r--   0        0        0    26003 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/lib/resources.py
+-rw-r--r--   0        0        0     2656 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/lib/settings.py
+-rw-r--r--   0        0        0      823 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/lib/track.py
+-rw-r--r--   0        0        0      401 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/lib/util.py
+-rw-r--r--   0        0        0    16084 2023-01-25 19:16:30.221395 boxjelly-0.3.3/boxjelly/models/TrackListModel.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/scripts/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-14 16:17:31.605023 boxjelly-0.3.3/boxjelly/scripts/run.py
+-rw-r--r--   0        0        0     1311 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/FileSelector.py
+-rw-r--r--   0        0        0    14318 2023-06-14 16:17:31.609023 boxjelly-0.3.3/boxjelly/ui/MainWindow.py
+-rw-r--r--   0        0        0     1105 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/MediaSelectionBox.py
+-rw-r--r--   0        0        0     1407 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/OpenDialog.py
+-rw-r--r--   0        0        0     5305 2023-06-14 16:17:31.609023 boxjelly-0.3.3/boxjelly/ui/SourceWidgets.py
+-rw-r--r--   0        0        0     1261 2023-06-14 16:17:31.609023 boxjelly-0.3.3/boxjelly/ui/TrackSelectionBox.py
+-rw-r--r--   0        0        0     1654 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/WidgetComboBox.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/__init__.py
+-rw-r--r--   0        0        0     2689 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/graphicsitems/TimelineTrack.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/graphicsitems/__init__.py
+-rw-r--r--   0        0        0     2925 2023-06-14 16:17:31.609023 boxjelly-0.3.3/boxjelly/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/settings/__init__.py
+-rw-r--r--   0        0        0      861 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0     4288 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/settings/tabs/NetworkSettingsTab.py
+-rw-r--r--   0        0        0     1122 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/settings/tabs/VideoSettingsTab.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     4247 2023-06-14 18:33:58.292378 boxjelly-0.3.3/boxjelly/ui/track/Timeline.py
+-rw-r--r--   0        0        0    10447 2023-06-14 18:39:32.295021 boxjelly-0.3.3/boxjelly/ui/track/TrackGraphicsView.py
+-rw-r--r--   0        0        0      852 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/track/TrackHeadersView.py
+-rw-r--r--   0        0        0     2444 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/track/TrackPanel.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/track/__init__.py
+-rw-r--r--   0        0        0     5908 2023-06-14 16:44:21.634736 boxjelly-0.3.3/boxjelly/ui/video/CthulhuVideoController.py
+-rw-r--r--   0        0        0        0 2023-01-25 18:58:58.749648 boxjelly-0.3.3/boxjelly/ui/video/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-14 18:39:32.295021 boxjelly-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 boxjelly-0.3.3/PKG-INFO
```

### Comparing `boxjelly-0.3.2/boxjelly/assets/assets.qrc` & `boxjelly-0.3.3/boxjelly/assets/assets.qrc`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-00000000: 3c21 444f 4354 5950 4520 5243 433e 0d0a  <!DOCTYPE RCC>..
-00000010: 3c52 4343 2076 6572 7369 6f6e 3d22 312e  <RCC version="1.
-00000020: 3022 3e0d 0a20 2020 203c 7172 6573 6f75  0">..    <qresou
-00000030: 7263 6520 7072 6566 6978 3d22 2f69 636f  rce prefix="/ico
-00000040: 6e73 223e 0d0a 2020 2020 2020 2020 3c66  ns">..        <f
-00000050: 696c 6520 616c 6961 733d 226c 6f67 6f22  ile alias="logo"
-00000060: 3e69 636f 6e73 2f62 6f78 6a65 6c6c 795f  >icons/boxjelly_
-00000070: 6c6f 676f 2e73 7667 3c2f 6669 6c65 3e0d  logo.svg</file>.
-00000080: 0a20 2020 2020 2020 203c 6669 6c65 2061  .        <file a
-00000090: 6c69 6173 3d22 7265 6e61 6d65 223e 6963  lias="rename">ic
-000000a0: 6f6e 732f 7265 6e61 6d65 2e70 6e67 3c2f  ons/rename.png</
-000000b0: 6669 6c65 3e0d 0a20 2020 2020 2020 203c  file>..        <
-000000c0: 6669 6c65 2061 6c69 6173 3d22 7370 6c69  file alias="spli
-000000d0: 7422 3e69 636f 6e73 2f73 706c 6974 2e70  t">icons/split.p
-000000e0: 6e67 3c2f 6669 6c65 3e0d 0a20 2020 2020  ng</file>..     
-000000f0: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-00000100: 6d65 7267 6522 3e69 636f 6e73 2f6d 6572  merge">icons/mer
-00000110: 6765 2e70 6e67 3c2f 6669 6c65 3e0d 0a20  ge.png</file>.. 
-00000120: 2020 2020 2020 203c 6669 6c65 2061 6c69         <file ali
-00000130: 6173 3d22 6465 6c65 7465 223e 6963 6f6e  as="delete">icon
-00000140: 732f 6465 6c65 7465 2e70 6e67 3c2f 6669  s/delete.png</fi
-00000150: 6c65 3e0d 0a20 2020 2020 2020 203c 6669  le>..        <fi
-00000160: 6c65 2061 6c69 6173 3d22 7365 656b 5f62  le alias="seek_b
-00000170: 6567 696e 6e69 6e67 223e 6963 6f6e 732f  eginning">icons/
-00000180: 7365 656b 5f62 6567 696e 6e69 6e67 2e70  seek_beginning.p
-00000190: 6e67 3c2f 6669 6c65 3e0d 0a20 2020 2020  ng</file>..     
-000001a0: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-000001b0: 7365 656b 5f65 6e64 223e 6963 6f6e 732f  seek_end">icons/
-000001c0: 7365 656b 5f65 6e64 2e70 6e67 3c2f 6669  seek_end.png</fi
-000001d0: 6c65 3e0d 0a20 2020 2020 2020 203c 6669  le>..        <fi
-000001e0: 6c65 2061 6c69 6173 3d22 756e 646f 223e  le alias="undo">
-000001f0: 6963 6f6e 732f 756e 646f 2e70 6e67 3c2f  icons/undo.png</
-00000200: 6669 6c65 3e0d 0a20 2020 2020 2020 203c  file>..        <
-00000210: 6669 6c65 2061 6c69 6173 3d22 7265 646f  file alias="redo
-00000220: 223e 6963 6f6e 732f 7265 646f 2e70 6e67  ">icons/redo.png
-00000230: 3c2f 6669 6c65 3e0d 0a20 2020 203c 2f71  </file>..    </q
-00000240: 7265 736f 7572 6365 3e0d 0a3c 2f52 4343  resource>..</RCC
-00000250: 3e                                       >
+00000000: 3c21 444f 4354 5950 4520 5243 433e 0a3c  <!DOCTYPE RCC>.<
+00000010: 5243 4320 7665 7273 696f 6e3d 2231 2e30  RCC version="1.0
+00000020: 223e 0a20 2020 203c 7172 6573 6f75 7263  ">.    <qresourc
+00000030: 6520 7072 6566 6978 3d22 2f69 636f 6e73  e prefix="/icons
+00000040: 223e 0a20 2020 2020 2020 203c 6669 6c65  ">.        <file
+00000050: 2061 6c69 6173 3d22 6c6f 676f 223e 6963   alias="logo">ic
+00000060: 6f6e 732f 626f 786a 656c 6c79 5f6c 6f67  ons/boxjelly_log
+00000070: 6f2e 7376 673c 2f66 696c 653e 0a20 2020  o.svg</file>.   
+00000080: 2020 2020 203c 6669 6c65 2061 6c69 6173       <file alias
+00000090: 3d22 7265 6e61 6d65 223e 6963 6f6e 732f  ="rename">icons/
+000000a0: 7265 6e61 6d65 2e70 6e67 3c2f 6669 6c65  rename.png</file
+000000b0: 3e0a 2020 2020 2020 2020 3c66 696c 6520  >.        <file 
+000000c0: 616c 6961 733d 2273 706c 6974 223e 6963  alias="split">ic
+000000d0: 6f6e 732f 7370 6c69 742e 706e 673c 2f66  ons/split.png</f
+000000e0: 696c 653e 0a20 2020 2020 2020 203c 6669  ile>.        <fi
+000000f0: 6c65 2061 6c69 6173 3d22 6d65 7267 6522  le alias="merge"
+00000100: 3e69 636f 6e73 2f6d 6572 6765 2e70 6e67  >icons/merge.png
+00000110: 3c2f 6669 6c65 3e0a 2020 2020 2020 2020  </file>.        
+00000120: 3c66 696c 6520 616c 6961 733d 2264 656c  <file alias="del
+00000130: 6574 6522 3e69 636f 6e73 2f64 656c 6574  ete">icons/delet
+00000140: 652e 706e 673c 2f66 696c 653e 0a20 2020  e.png</file>.   
+00000150: 2020 2020 203c 6669 6c65 2061 6c69 6173       <file alias
+00000160: 3d22 7365 656b 5f62 6567 696e 6e69 6e67  ="seek_beginning
+00000170: 223e 6963 6f6e 732f 7365 656b 5f62 6567  ">icons/seek_beg
+00000180: 696e 6e69 6e67 2e70 6e67 3c2f 6669 6c65  inning.png</file
+00000190: 3e0a 2020 2020 2020 2020 3c66 696c 6520  >.        <file 
+000001a0: 616c 6961 733d 2273 6565 6b5f 656e 6422  alias="seek_end"
+000001b0: 3e69 636f 6e73 2f73 6565 6b5f 656e 642e  >icons/seek_end.
+000001c0: 706e 673c 2f66 696c 653e 0a20 2020 2020  png</file>.     
+000001d0: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
+000001e0: 756e 646f 223e 6963 6f6e 732f 756e 646f  undo">icons/undo
+000001f0: 2e70 6e67 3c2f 6669 6c65 3e0a 2020 2020  .png</file>.    
+00000200: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
+00000210: 2272 6564 6f22 3e69 636f 6e73 2f72 6564  "redo">icons/red
+00000220: 6f2e 706e 673c 2f66 696c 653e 0a20 2020  o.png</file>.   
+00000230: 203c 2f71 7265 736f 7572 6365 3e0a 3c2f   </qresource>.</
+00000240: 5243 433e                                RCC>
```

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/boxjelly.svg` & `boxjelly-0.3.3/boxjelly/assets/icons/boxjelly.svg`

 * *Files 17% similar despite different names*

```diff
@@ -1,710 +1,698 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0d0a 3c21 2d2d 2043 7265  "no"?>..<!-- Cre
-00000040: 6174 6564 2077 6974 6820 496e 6b73 6361  ated with Inksca
-00000050: 7065 2028 6874 7470 3a2f 2f77 7777 2e69  pe (http://www.i
-00000060: 6e6b 7363 6170 652e 6f72 672f 2920 2d2d  nkscape.org/) --
-00000070: 3e0d 0a0d 0a3c 7376 670d 0a20 2020 786d  >....<svg..   xm
-00000080: 6c6e 733a 6463 3d22 6874 7470 3a2f 2f70  lns:dc="http://p
-00000090: 7572 6c2e 6f72 672f 6463 2f65 6c65 6d65  url.org/dc/eleme
-000000a0: 6e74 732f 312e 312f 220d 0a20 2020 786d  nts/1.1/"..   xm
-000000b0: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
-000000c0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-000000d0: 7267 2f6e 7323 220d 0a20 2020 786d 6c6e  rg/ns#"..   xmln
-000000e0: 733a 7264 663d 2268 7474 703a 2f2f 7777  s:rdf="http://ww
-000000f0: 772e 7733 2e6f 7267 2f31 3939 392f 3032  w.w3.org/1999/02
-00000100: 2f32 322d 7264 662d 7379 6e74 6178 2d6e  /22-rdf-syntax-n
-00000110: 7323 220d 0a20 2020 786d 6c6e 733a 7376  s#"..   xmlns:sv
-00000120: 673d 2268 7474 703a 2f2f 7777 772e 7733  g="http://www.w3
-00000130: 2e6f 7267 2f32 3030 302f 7376 6722 0d0a  .org/2000/svg"..
-00000140: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
-00000150: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
-00000160: 2f73 7667 220d 0a20 2020 786d 6c6e 733a  /svg"..   xmlns:
-00000170: 736f 6469 706f 6469 3d22 6874 7470 3a2f  sodipodi="http:/
-00000180: 2f73 6f64 6970 6f64 692e 736f 7572 6365  /sodipodi.source
-00000190: 666f 7267 652e 6e65 742f 4454 442f 736f  forge.net/DTD/so
-000001a0: 6469 706f 6469 2d30 2e64 7464 220d 0a20  dipodi-0.dtd".. 
-000001b0: 2020 786d 6c6e 733a 696e 6b73 6361 7065    xmlns:inkscape
-000001c0: 3d22 6874 7470 3a2f 2f77 7777 2e69 6e6b  ="http://www.ink
-000001d0: 7363 6170 652e 6f72 672f 6e61 6d65 7370  scape.org/namesp
-000001e0: 6163 6573 2f69 6e6b 7363 6170 6522 0d0a  aces/inkscape"..
-000001f0: 2020 2077 6964 7468 3d22 3136 7078 220d     width="16px".
-00000200: 0a20 2020 6865 6967 6874 3d22 3136 7078  .   height="16px
-00000210: 220d 0a20 2020 7669 6577 426f 783d 2230  "..   viewBox="0
-00000220: 2030 2031 3620 3136 220d 0a20 2020 7665   0 16 16"..   ve
-00000230: 7273 696f 6e3d 2231 2e31 220d 0a20 2020  rsion="1.1"..   
-00000240: 6964 3d22 5356 4752 6f6f 7422 0d0a 2020  id="SVGRoot"..  
-00000250: 2069 6e6b 7363 6170 653a 7665 7273 696f   inkscape:versio
-00000260: 6e3d 2230 2e39 322e 3520 2832 3036 3065  n="0.92.5 (2060e
-00000270: 6331 6639 662c 2032 3032 302d 3034 2d30  c1f9f, 2020-04-0
-00000280: 3829 220d 0a20 2020 736f 6469 706f 6469  8)"..   sodipodi
-00000290: 3a64 6f63 6e61 6d65 3d22 626f 786a 656c  :docname="boxjel
-000002a0: 6c79 2d74 6869 636b 2e73 7667 223e 0d0a  ly-thick.svg">..
-000002b0: 2020 3c64 6566 730d 0a20 2020 2020 6964    <defs..     id
-000002c0: 3d22 6465 6673 3130 223e 0d0a 2020 2020  ="defs10">..    
-000002d0: 3c69 6e6b 7363 6170 653a 7061 7468 2d65  <inkscape:path-e
-000002e0: 6666 6563 740d 0a20 2020 2020 2020 6566  ffect..       ef
-000002f0: 6665 6374 3d22 7461 7065 725f 7374 726f  fect="taper_stro
-00000300: 6b65 220d 0a20 2020 2020 2020 6964 3d22  ke"..       id="
-00000310: 7061 7468 2d65 6666 6563 7435 3338 3122  path-effect5381"
-00000320: 0d0a 2020 2020 2020 2069 735f 7669 7369  ..       is_visi
-00000330: 626c 653d 2274 7275 6522 0d0a 2020 2020  ble="true"..    
-00000340: 2020 2073 7472 6f6b 655f 7769 6474 683d     stroke_width=
-00000350: 2230 2e39 220d 0a20 2020 2020 2020 6174  "0.9"..       at
-00000360: 7461 6368 5f73 7461 7274 3d22 3165 2d30  tach_start="1e-0
-00000370: 3722 0d0a 2020 2020 2020 2065 6e64 5f6f  7"..       end_o
-00000380: 6666 7365 743d 2230 2e39 3939 3939 220d  ffset="0.99999".
-00000390: 0a20 2020 2020 2020 736d 6f6f 7468 696e  .       smoothin
-000003a0: 673d 2231 2e31 220d 0a20 2020 2020 2020  g="1.1"..       
-000003b0: 6a6f 696e 7479 7065 3d22 6578 7472 6170  jointype="extrap
-000003c0: 6f6c 6174 6564 220d 0a20 2020 2020 2020  olated"..       
-000003d0: 6d69 7465 725f 6c69 6d69 743d 2231 3030  miter_limit="100
-000003e0: 2220 2f3e 0d0a 2020 2020 3c69 6e6b 7363  " />..    <inksc
-000003f0: 6170 653a 7061 7468 2d65 6666 6563 740d  ape:path-effect.
-00000400: 0a20 2020 2020 2020 6566 6665 6374 3d22  .       effect="
-00000410: 7461 7065 725f 7374 726f 6b65 220d 0a20  taper_stroke".. 
-00000420: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
-00000430: 6666 6563 7435 3338 312d 3322 0d0a 2020  ffect5381-3"..  
-00000440: 2020 2020 2069 735f 7669 7369 626c 653d       is_visible=
-00000450: 2274 7275 6522 0d0a 2020 2020 2020 2073  "true"..       s
-00000460: 7472 6f6b 655f 7769 6474 683d 2230 2e39  troke_width="0.9
-00000470: 220d 0a20 2020 2020 2020 6174 7461 6368  "..       attach
-00000480: 5f73 7461 7274 3d22 3165 2d30 3722 0d0a  _start="1e-07"..
-00000490: 2020 2020 2020 2065 6e64 5f6f 6666 7365         end_offse
-000004a0: 743d 2231 2e34 3232 3030 3934 220d 0a20  t="1.4220094".. 
-000004b0: 2020 2020 2020 736d 6f6f 7468 696e 673d        smoothing=
-000004c0: 2231 2e31 220d 0a20 2020 2020 2020 6a6f  "1.1"..       jo
-000004d0: 696e 7479 7065 3d22 6578 7472 6170 6f6c  intype="extrapol
-000004e0: 6174 6564 220d 0a20 2020 2020 2020 6d69  ated"..       mi
-000004f0: 7465 725f 6c69 6d69 743d 2231 3030 2220  ter_limit="100" 
-00000500: 2f3e 0d0a 2020 2020 3c69 6e6b 7363 6170  />..    <inkscap
-00000510: 653a 7061 7468 2d65 6666 6563 740d 0a20  e:path-effect.. 
-00000520: 2020 2020 2020 6566 6665 6374 3d22 7461        effect="ta
-00000530: 7065 725f 7374 726f 6b65 220d 0a20 2020  per_stroke"..   
-00000540: 2020 2020 6964 3d22 7061 7468 2d65 6666      id="path-eff
-00000550: 6563 7435 3338 312d 332d 3722 0d0a 2020  ect5381-3-7"..  
-00000560: 2020 2020 2069 735f 7669 7369 626c 653d       is_visible=
-00000570: 2274 7275 6522 0d0a 2020 2020 2020 2073  "true"..       s
-00000580: 7472 6f6b 655f 7769 6474 683d 2231 220d  troke_width="1".
-00000590: 0a20 2020 2020 2020 6174 7461 6368 5f73  .       attach_s
-000005a0: 7461 7274 3d22 3165 2d30 3722 0d0a 2020  tart="1e-07"..  
-000005b0: 2020 2020 2065 6e64 5f6f 6666 7365 743d       end_offset=
-000005c0: 2231 2e34 3232 3030 3934 220d 0a20 2020  "1.4220094"..   
-000005d0: 2020 2020 736d 6f6f 7468 696e 673d 2231      smoothing="1
-000005e0: 2e31 220d 0a20 2020 2020 2020 6a6f 696e  .1"..       join
-000005f0: 7479 7065 3d22 6578 7472 6170 6f6c 6174  type="extrapolat
-00000600: 6564 220d 0a20 2020 2020 2020 6d69 7465  ed"..       mite
-00000610: 725f 6c69 6d69 743d 2231 3030 2220 2f3e  r_limit="100" />
-00000620: 0d0a 2020 2020 3c69 6e6b 7363 6170 653a  ..    <inkscape:
-00000630: 7061 7468 2d65 6666 6563 740d 0a20 2020  path-effect..   
-00000640: 2020 2020 6566 6665 6374 3d22 7461 7065      effect="tape
-00000650: 725f 7374 726f 6b65 220d 0a20 2020 2020  r_stroke"..     
-00000660: 2020 6964 3d22 7061 7468 2d65 6666 6563    id="path-effec
-00000670: 7435 3338 312d 3222 0d0a 2020 2020 2020  t5381-2"..      
-00000680: 2069 735f 7669 7369 626c 653d 2274 7275   is_visible="tru
-00000690: 6522 0d0a 2020 2020 2020 2073 7472 6f6b  e"..       strok
-000006a0: 655f 7769 6474 683d 2231 220d 0a20 2020  e_width="1"..   
-000006b0: 2020 2020 6174 7461 6368 5f73 7461 7274      attach_start
-000006c0: 3d22 3165 2d30 3722 0d0a 2020 2020 2020  ="1e-07"..      
-000006d0: 2065 6e64 5f6f 6666 7365 743d 2230 2e39   end_offset="0.9
-000006e0: 3939 3939 220d 0a20 2020 2020 2020 736d  9999"..       sm
-000006f0: 6f6f 7468 696e 673d 2231 2e31 220d 0a20  oothing="1.1".. 
-00000700: 2020 2020 2020 6a6f 696e 7479 7065 3d22        jointype="
-00000710: 6578 7472 6170 6f6c 6174 6564 220d 0a20  extrapolated".. 
-00000720: 2020 2020 2020 6d69 7465 725f 6c69 6d69        miter_limi
-00000730: 743d 2231 3030 2220 2f3e 0d0a 2020 2020  t="100" />..    
-00000740: 3c69 6e6b 7363 6170 653a 7061 7468 2d65  <inkscape:path-e
-00000750: 6666 6563 740d 0a20 2020 2020 2020 6566  ffect..       ef
-00000760: 6665 6374 3d22 7461 7065 725f 7374 726f  fect="taper_stro
-00000770: 6b65 220d 0a20 2020 2020 2020 6964 3d22  ke"..       id="
-00000780: 7061 7468 2d65 6666 6563 7435 3338 312d  path-effect5381-
-00000790: 332d 3122 0d0a 2020 2020 2020 2069 735f  3-1"..       is_
-000007a0: 7669 7369 626c 653d 2274 7275 6522 0d0a  visible="true"..
-000007b0: 2020 2020 2020 2073 7472 6f6b 655f 7769         stroke_wi
-000007c0: 6474 683d 2230 2e39 220d 0a20 2020 2020  dth="0.9"..     
-000007d0: 2020 6174 7461 6368 5f73 7461 7274 3d22    attach_start="
-000007e0: 3165 2d30 3722 0d0a 2020 2020 2020 2065  1e-07"..       e
-000007f0: 6e64 5f6f 6666 7365 743d 2231 2e34 3232  nd_offset="1.422
-00000800: 3030 3934 220d 0a20 2020 2020 2020 736d  0094"..       sm
-00000810: 6f6f 7468 696e 673d 2231 2e31 220d 0a20  oothing="1.1".. 
-00000820: 2020 2020 2020 6a6f 696e 7479 7065 3d22        jointype="
-00000830: 6578 7472 6170 6f6c 6174 6564 220d 0a20  extrapolated".. 
-00000840: 2020 2020 2020 6d69 7465 725f 6c69 6d69        miter_limi
-00000850: 743d 2231 3030 2220 2f3e 0d0a 2020 2020  t="100" />..    
-00000860: 3c69 6e6b 7363 6170 653a 7061 7468 2d65  <inkscape:path-e
-00000870: 6666 6563 740d 0a20 2020 2020 2020 6566  ffect..       ef
-00000880: 6665 6374 3d22 7461 7065 725f 7374 726f  fect="taper_stro
-00000890: 6b65 220d 0a20 2020 2020 2020 6964 3d22  ke"..       id="
-000008a0: 7061 7468 2d65 6666 6563 7435 3338 312d  path-effect5381-
-000008b0: 3722 0d0a 2020 2020 2020 2069 735f 7669  7"..       is_vi
-000008c0: 7369 626c 653d 2274 7275 6522 0d0a 2020  sible="true"..  
-000008d0: 2020 2020 2073 7472 6f6b 655f 7769 6474       stroke_widt
-000008e0: 683d 2230 2e39 220d 0a20 2020 2020 2020  h="0.9"..       
-000008f0: 6174 7461 6368 5f73 7461 7274 3d22 3165  attach_start="1e
-00000900: 2d30 3722 0d0a 2020 2020 2020 2065 6e64  -07"..       end
-00000910: 5f6f 6666 7365 743d 2230 2e39 3939 3939  _offset="0.99999
-00000920: 220d 0a20 2020 2020 2020 736d 6f6f 7468  "..       smooth
-00000930: 696e 673d 2231 2e31 220d 0a20 2020 2020  ing="1.1"..     
-00000940: 2020 6a6f 696e 7479 7065 3d22 6578 7472    jointype="extr
-00000950: 6170 6f6c 6174 6564 220d 0a20 2020 2020  apolated"..     
-00000960: 2020 6d69 7465 725f 6c69 6d69 743d 2231    miter_limit="1
-00000970: 3030 2220 2f3e 0d0a 2020 2020 3c69 6e6b  00" />..    <ink
-00000980: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
-00000990: 740d 0a20 2020 2020 2020 6566 6665 6374  t..       effect
-000009a0: 3d22 7461 7065 725f 7374 726f 6b65 220d  ="taper_stroke".
-000009b0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-000009c0: 2d65 6666 6563 7435 3338 312d 332d 3922  -effect5381-3-9"
-000009d0: 0d0a 2020 2020 2020 2069 735f 7669 7369  ..       is_visi
-000009e0: 626c 653d 2274 7275 6522 0d0a 2020 2020  ble="true"..    
-000009f0: 2020 2073 7472 6f6b 655f 7769 6474 683d     stroke_width=
-00000a00: 2230 2e39 220d 0a20 2020 2020 2020 6174  "0.9"..       at
-00000a10: 7461 6368 5f73 7461 7274 3d22 3165 2d30  tach_start="1e-0
-00000a20: 3722 0d0a 2020 2020 2020 2065 6e64 5f6f  7"..       end_o
-00000a30: 6666 7365 743d 2231 2e34 3232 3030 3934  ffset="1.4220094
-00000a40: 220d 0a20 2020 2020 2020 736d 6f6f 7468  "..       smooth
-00000a50: 696e 673d 2231 2e31 220d 0a20 2020 2020  ing="1.1"..     
-00000a60: 2020 6a6f 696e 7479 7065 3d22 6578 7472    jointype="extr
-00000a70: 6170 6f6c 6174 6564 220d 0a20 2020 2020  apolated"..     
-00000a80: 2020 6d69 7465 725f 6c69 6d69 743d 2231    miter_limit="1
-00000a90: 3030 2220 2f3e 0d0a 2020 2020 3c69 6e6b  00" />..    <ink
-00000aa0: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
-00000ab0: 740d 0a20 2020 2020 2020 6566 6665 6374  t..       effect
-00000ac0: 3d22 7461 7065 725f 7374 726f 6b65 220d  ="taper_stroke".
-00000ad0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00000ae0: 2d65 6666 6563 7435 3338 312d 3622 0d0a  -effect5381-6"..
-00000af0: 2020 2020 2020 2069 735f 7669 7369 626c         is_visibl
-00000b00: 653d 2274 7275 6522 0d0a 2020 2020 2020  e="true"..      
-00000b10: 2073 7472 6f6b 655f 7769 6474 683d 2230   stroke_width="0
-00000b20: 2e39 220d 0a20 2020 2020 2020 6174 7461  .9"..       atta
-00000b30: 6368 5f73 7461 7274 3d22 3165 2d30 3722  ch_start="1e-07"
-00000b40: 0d0a 2020 2020 2020 2065 6e64 5f6f 6666  ..       end_off
-00000b50: 7365 743d 2230 2e39 3939 3939 220d 0a20  set="0.99999".. 
-00000b60: 2020 2020 2020 736d 6f6f 7468 696e 673d        smoothing=
-00000b70: 2231 2e31 220d 0a20 2020 2020 2020 6a6f  "1.1"..       jo
-00000b80: 696e 7479 7065 3d22 6578 7472 6170 6f6c  intype="extrapol
-00000b90: 6174 6564 220d 0a20 2020 2020 2020 6d69  ated"..       mi
-00000ba0: 7465 725f 6c69 6d69 743d 2231 3030 2220  ter_limit="100" 
-00000bb0: 2f3e 0d0a 2020 3c2f 6465 6673 3e0d 0a20  />..  </defs>.. 
-00000bc0: 203c 736f 6469 706f 6469 3a6e 616d 6564   <sodipodi:named
-00000bd0: 7669 6577 0d0a 2020 2020 2069 643d 2262  view..     id="b
-00000be0: 6173 6522 0d0a 2020 2020 2070 6167 6563  ase"..     pagec
-00000bf0: 6f6c 6f72 3d22 2366 6666 6666 6622 0d0a  olor="#ffffff"..
-00000c00: 2020 2020 2062 6f72 6465 7263 6f6c 6f72       bordercolor
-00000c10: 3d22 2336 3636 3636 3622 0d0a 2020 2020  ="#666666"..    
-00000c20: 2062 6f72 6465 726f 7061 6369 7479 3d22   borderopacity="
-00000c30: 312e 3022 0d0a 2020 2020 2069 6e6b 7363  1.0"..     inksc
-00000c40: 6170 653a 7061 6765 6f70 6163 6974 793d  ape:pageopacity=
-00000c50: 2230 2e30 220d 0a20 2020 2020 696e 6b73  "0.0"..     inks
-00000c60: 6361 7065 3a70 6167 6573 6861 646f 773d  cape:pageshadow=
-00000c70: 2232 220d 0a20 2020 2020 696e 6b73 6361  "2"..     inksca
-00000c80: 7065 3a7a 6f6f 6d3d 2234 352e 3235 3438  pe:zoom="45.2548
-00000c90: 3334 220d 0a20 2020 2020 696e 6b73 6361  34"..     inksca
-00000ca0: 7065 3a63 783d 2237 2e38 3735 3836 3635  pe:cx="7.8758665
-00000cb0: 220d 0a20 2020 2020 696e 6b73 6361 7065  "..     inkscape
-00000cc0: 3a63 793d 2238 2e33 3638 3537 3132 220d  :cy="8.3685712".
-00000cd0: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
-00000ce0: 6f63 756d 656e 742d 756e 6974 733d 2270  ocument-units="p
-00000cf0: 7822 0d0a 2020 2020 2069 6e6b 7363 6170  x"..     inkscap
-00000d00: 653a 6375 7272 656e 742d 6c61 7965 723d  e:current-layer=
-00000d10: 226c 6179 6572 3122 0d0a 2020 2020 2073  "layer1"..     s
-00000d20: 686f 7767 7269 643d 2266 616c 7365 220d  howgrid="false".
-00000d30: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-00000d40: 696e 646f 772d 7769 6474 683d 2232 3038  indow-width="208
-00000d50: 3022 0d0a 2020 2020 2069 6e6b 7363 6170  0"..     inkscap
-00000d60: 653a 7769 6e64 6f77 2d68 6569 6768 743d  e:window-height=
-00000d70: 2231 3232 3622 0d0a 2020 2020 2069 6e6b  "1226"..     ink
-00000d80: 7363 6170 653a 7769 6e64 6f77 2d78 3d22  scape:window-x="
-00000d90: 3838 3222 0d0a 2020 2020 2069 6e6b 7363  882"..     inksc
-00000da0: 6170 653a 7769 6e64 6f77 2d79 3d22 3022  ape:window-y="0"
-00000db0: 0d0a 2020 2020 2069 6e6b 7363 6170 653a  ..     inkscape:
-00000dc0: 7769 6e64 6f77 2d6d 6178 696d 697a 6564  window-maximized
-00000dd0: 3d22 3022 0d0a 2020 2020 2069 6e6b 7363  ="0"..     inksc
-00000de0: 6170 653a 6772 6964 2d62 626f 783d 2274  ape:grid-bbox="t
-00000df0: 7275 6522 0d0a 2020 2020 2069 6e6b 7363  rue"..     inksc
-00000e00: 6170 653a 736e 6170 2d6e 6f64 6573 3d22  ape:snap-nodes="
-00000e10: 6661 6c73 6522 202f 3e0d 0a20 203c 6d65  false" />..  <me
-00000e20: 7461 6461 7461 0d0a 2020 2020 2069 643d  tadata..     id=
-00000e30: 226d 6574 6164 6174 6131 3322 3e0d 0a20  "metadata13">.. 
-00000e40: 2020 203c 7264 663a 5244 463e 0d0a 2020     <rdf:RDF>..  
-00000e50: 2020 2020 3c63 633a 576f 726b 0d0a 2020      <cc:Work..  
-00000e60: 2020 2020 2020 2072 6466 3a61 626f 7574         rdf:about
-00000e70: 3d22 223e 0d0a 2020 2020 2020 2020 3c64  ="">..        <d
-00000e80: 633a 666f 726d 6174 3e69 6d61 6765 2f73  c:format>image/s
-00000e90: 7667 2b78 6d6c 3c2f 6463 3a66 6f72 6d61  vg+xml</dc:forma
-00000ea0: 743e 0d0a 2020 2020 2020 2020 3c64 633a  t>..        <dc:
-00000eb0: 7479 7065 0d0a 2020 2020 2020 2020 2020  type..          
-00000ec0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
-00000ed0: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
-00000ee0: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
-00000ef0: 496d 6167 6522 202f 3e0d 0a20 2020 2020  Image" />..     
-00000f00: 2020 203c 6463 3a74 6974 6c65 3e3c 2f64     <dc:title></d
-00000f10: 633a 7469 746c 653e 0d0a 2020 2020 2020  c:title>..      
-00000f20: 3c2f 6363 3a57 6f72 6b3e 0d0a 2020 2020  </cc:Work>..    
-00000f30: 3c2f 7264 663a 5244 463e 0d0a 2020 3c2f  </rdf:RDF>..  </
-00000f40: 6d65 7461 6461 7461 3e0d 0a20 203c 670d  metadata>..  <g.
-00000f50: 0a20 2020 2020 696e 6b73 6361 7065 3a6c  .     inkscape:l
-00000f60: 6162 656c 3d22 4c61 7965 7220 3122 0d0a  abel="Layer 1"..
-00000f70: 2020 2020 2069 6e6b 7363 6170 653a 6772       inkscape:gr
-00000f80: 6f75 706d 6f64 653d 226c 6179 6572 220d  oupmode="layer".
-00000f90: 0a20 2020 2020 6964 3d22 6c61 7965 7231  .     id="layer1
-00000fa0: 223e 0d0a 2020 2020 3c70 6174 680d 0a20  ">..    <path.. 
-00000fb0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00000fc0: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
-00000fd0: 3033 3338 303b 7374 726f 6b65 2d77 6964  03380;stroke-wid
-00000fe0: 7468 3a31 3b73 7472 6f6b 652d 6c69 6e65  th:1;stroke-line
-00000ff0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00001000: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00001010: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00001020: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00001030: 793a 3122 0d0a 2020 2020 2020 2064 3d22  y:1"..       d="
-00001040: 6d20 3131 2e32 3135 3730 362c 312e 3931  m 11.215706,1.91
-00001050: 3230 3036 3120 302e 3733 3434 3537 2c30  20061 0.734457,0
-00001060: 2e33 3137 3133 3135 2063 2030 2e38 3133  .3171315 c 0.813
-00001070: 3737 382c 302e 3335 3133 3832 3220 312e  778,0.3513822 1.
-00001080: 3939 3930 3432 2c31 2e33 3838 3333 3031  999042,1.3883301
-00001090: 2031 2e34 3937 3139 382c 322e 3138 3532   1.497198,2.1852
-000010a0: 3837 3120 4c20 3131 2e38 3431 3136 332c  871 L 11.841163,
-000010b0: 362e 3936 3531 3631 3120 4320 3131 2e33  6.9651611 C 11.3
-000010c0: 3339 3331 392c 372e 3736 3231 3138 3320  39319,7.7621183 
-000010d0: 3130 2e39 3336 3832 382c 382e 3332 3730  10.936828,8.3270
-000010e0: 3238 3620 392e 3537 3136 3732 382c 372e  286 9.5716728,7.
-000010f0: 3733 3735 3636 3820 4c20 382e 3833 3732  7375668 L 8.8372
-00001100: 3136 362c 372e 3432 3034 3335 3320 4320  166,7.4204353 C 
-00001110: 372e 3431 3438 3336 352c 362e 3830 3632  7.4148365,6.8062
-00001120: 3634 3520 372e 3730 3632 3430 352c 362e  645 7.7062405,6.
-00001130: 3130 3030 3237 3920 382e 3030 3133 3635  1000279 8.001365
-00001140: 342c 352e 3230 3536 3632 3420 4c20 382e  4,5.2056624 L 8.
-00001150: 3933 3735 3137 322c 322e 3336 3836 3837  9375172,2.368687
-00001160: 3320 4320 392e 3233 3236 3431 392c 312e  3 C 9.2326419,1.
-00001170: 3437 3433 3232 3420 3130 2e34 3031 3932  4743224 10.40192
-00001180: 382c 312e 3536 3036 3233 3720 3131 2e32  8,1.5606237 11.2
-00001190: 3135 3730 362c 312e 3931 3230 3036 3120  15706,1.9120061 
-000011a0: 5a22 0d0a 2020 2020 2020 2069 643d 2272  Z"..       id="r
-000011b0: 6563 7432 3035 220d 0a20 2020 2020 2020  ect205"..       
-000011c0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-000011d0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-000011e0: 0d0a 2020 2020 2020 2073 6f64 6970 6f64  ..       sodipod
-000011f0: 693a 6e6f 6465 7479 7065 733d 2273 7373  i:nodetypes="sss
-00001200: 7373 7373 7373 2220 2f3e 0d0a 2020 2020  ssssss" />..    
-00001210: 3c70 6174 680d 0a20 2020 2020 2020 7374  <path..       st
-00001220: 796c 653d 2266 696c 6c3a 2330 3033 3338  yle="fill:#00338
-00001230: 303b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  0;fill-rule:nonz
-00001240: 6572 6f3b 7374 726f 6b65 3a6e 6f6e 653b  ero;stroke:none;
-00001250: 7374 726f 6b65 2d77 6964 7468 3a31 7078  stroke-width:1px
-00001260: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00001270: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00001280: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00001290: 652d 6f70 6163 6974 793a 3122 0d0a 2020  e-opacity:1"..  
-000012a0: 2020 2020 2064 3d22 4d20 362e 3938 3635       d="M 6.9865
-000012b0: 3237 352c 372e 3934 3632 3236 3920 4320  275,7.9462269 C 
-000012c0: 362e 3735 3736 3839 372c 382e 3238 3138  6.7576897,8.2818
-000012d0: 3535 3520 362e 3238 3530 3433 392c 382e  555 6.2850439,8.
-000012e0: 3437 3935 3737 3720 352e 3831 3632 3430  4795777 5.816240
-000012f0: 322c 382e 3730 3534 3334 3520 352e 3538  2,8.7054345 5.58
-00001300: 3138 3338 342c 382e 3831 3833 3632 3920  18384,8.8183629 
-00001310: 352e 3333 3637 3639 2c38 2e39 3330 3534  5.336769,8.93054
-00001320: 3738 2035 2e31 3437 3233 3733 2c39 2e31  78 5.1472373,9.1
-00001330: 3933 3032 3433 2034 2e39 3537 3730 3535  930243 4.9577055
-00001340: 2c39 2e34 3535 3530 3039 2034 2e39 3532  ,9.4555009 4.952
-00001350: 3031 3037 2c39 2e38 3734 3235 3735 2035  0107,9.8742575 5
-00001360: 2e31 3136 3536 3237 2c31 302e 3139 3932  .1165627,10.1992
-00001370: 3333 2061 2031 2e30 3234 3630 3038 2c31  33 a 1.0246008,1
-00001380: 2e30 3234 3630 3038 2030 2030 2030 2030  .0246008 0 0 0 0
-00001390: 2e30 3036 3737 2c30 2e30 3133 3134 2031  .00677,0.01314 1
-000013a0: 2e38 3437 3037 3232 2c31 2e38 3437 3037  .8470722,1.84707
-000013b0: 3232 2030 2030 2031 2030 2e30 3034 3938  22 0 0 1 0.00498
-000013c0: 2c30 2e30 3038 3620 6320 302e 3136 3635  ,0.0086 c 0.1665
-000013d0: 3034 332c 302e 3238 3833 3934 2030 2e30  043,0.288394 0.0
-000013e0: 3833 3630 342c 302e 3332 3439 3220 2d30  83604,0.32492 -0
-000013f0: 2e31 3436 3935 3232 2c30 2e34 3633 3030  .1469522,0.46300
-00001400: 3120 2d30 2e32 3330 3535 3632 2c30 2e31  1 -0.2305562,0.1
-00001410: 3338 3038 3120 2d30 2e36 3236 3035 3131  38081 -0.6260511
-00001420: 2c30 2e31 3533 3232 3120 2d30 2e37 3738  ,0.153221 -0.778
-00001430: 3839 3032 2c30 2e30 3634 3938 2030 2c30  8902,0.06498 0,0
-00001440: 202d 332e 3631 652d 352c 2d32 2e31 652d   -3.61e-5,-2.1e-
-00001450: 3520 2d33 2e36 3165 2d35 2c2d 322e 3165  5 -3.61e-5,-2.1e
-00001460: 2d35 202d 302e 3336 3037 3230 392c 2d30  -5 -0.3607209,-0
-00001470: 2e31 3639 3530 3720 2d30 2e37 3133 3135  .169507 -0.71315
-00001480: 352c 2d30 2e31 3031 3633 3120 2d30 2e39  5,-0.101631 -0.9
-00001490: 3632 3134 3831 2c30 2e31 3033 3133 3120  621481,0.103131 
-000014a0: 2d30 2e32 3538 3231 3933 2c30 2e32 3431  -0.2582193,0.241
-000014b0: 3431 3620 2d30 2e34 3030 3738 3932 2c30  416 -0.4007892,0
-000014c0: 2e35 3031 3534 3720 2d30 2e34 3835 3838  .501547 -0.48588
-000014d0: 3031 2c30 2e36 3630 3032 3520 2d30 2e35  01,0.660025 -0.5
-000014e0: 3632 3933 3639 2c30 2e39 3332 3034 3920  629369,0.932049 
-000014f0: 2d30 2e38 3130 3433 3239 2c31 2e32 3536  -0.8104329,1.256
-00001500: 3435 3520 2d30 2e39 3234 3132 3335 2c31  455 -0.9241235,1
-00001510: 2e34 3435 3538 3620 2d30 2e31 3135 3332  .445586 -0.11532
-00001520: 3235 2c30 2e31 3931 3834 3620 2d30 2e30  25,0.191846 -0.0
-00001530: 3333 3933 312c 302e 3233 3233 3136 202d  33931,0.232316 -
-00001540: 302e 3033 3339 3331 2c30 2e32 3332 3331  0.033931,0.23231
-00001550: 3620 302c 3020 2d30 2e30 3039 3838 2c30  6 0,0 -0.00988,0
-00001560: 2e31 3136 3937 3320 302e 3233 3335 3434  .116973 0.233544
-00001570: 362c 302e 3036 3635 3820 302e 3234 3139  6,0.06658 0.2419
-00001580: 3437 392c 2d30 2e30 3530 3039 2030 2e37  479,-0.05009 0.7
-00001590: 3837 3936 3639 2c2d 302e 3239 3738 3532  879669,-0.297852
-000015a0: 2031 2e34 3438 3033 312c 2d31 2e32 3833   1.448031,-1.283
-000015b0: 3637 3620 302e 3132 3330 3131 362c 2d30  676 0.1230116,-0
-000015c0: 2e31 3637 3934 3120 302e 3234 3134 3237  .167941 0.241427
-000015d0: 372c 2d30 2e33 3731 3733 3820 302e 3334  7,-0.371738 0.34
-000015e0: 3535 3639 372c 2d30 2e34 3433 3637 3220  55697,-0.443672 
-000015f0: 2d30 2e30 3139 3032 332c 302e 3030 3636  -0.019023,0.0066
-00001600: 202d 302e 3030 3731 382c 2d30 2e30 3032   -0.00718,-0.002
-00001610: 3620 2d30 2e30 3731 3033 312c 2d38 2e35  6 -0.071031,-8.5
-00001620: 3265 2d34 2030 2c30 2034 2e36 652d 362c  2e-4 0,0 4.6e-6,
-00001630: 3265 2d36 2034 2e37 652d 362c 3265 2d36  2e-6 4.7e-6,2e-6
-00001640: 2030 2e35 3435 3439 3234 2c30 2e33 3134   0.5454924,0.314
-00001650: 3934 3120 312e 3139 3038 3735 322c 302e  941 1.1908752,0.
-00001660: 3232 3734 3239 2031 2e36 3931 3331 3334  227429 1.6913134
-00001670: 2c2d 302e 3037 3232 3920 4320 352e 3934  ,-0.07229 C 5.94
-00001680: 3133 3235 322c 3131 2e31 3538 3039 3220  13252,11.158092 
-00001690: 362e 3237 3835 312c 3130 2e34 3238 3436  6.27851,10.42846
-000016a0: 3920 352e 3931 3431 3837 392c 392e 3738  9 5.9141879,9.78
-000016b0: 3232 3438 3120 352e 3834 3738 3034 362c  22481 5.8478046,
-000016c0: 392e 3635 3238 3637 3620 352e 3836 3936  9.6528676 5.8696
-000016d0: 3435 322c 392e 3732 3939 3431 3520 352e  452,9.7299415 5.
-000016e0: 3837 3638 3934 332c 392e 3731 3939 3032  8768943,9.719902
-000016f0: 3520 352e 3838 3433 3330 312c 392e 3730  5 5.8843301,9.70
-00001700: 3936 3034 3920 362e 3030 3437 3132 312c  96049 6.0047121,
-00001710: 392e 3631 3336 3335 3920 362e 3230 3638  9.6136359 6.2068
-00001720: 3635 392c 392e 3531 3632 3433 3720 362e  659,9.5162437 6.
-00001730: 3631 3131 3733 372c 392e 3332 3134 3539  6111737,9.321459
-00001740: 3220 372e 3239 3630 3537 2c39 2e30 3839  2 7.296057,9.089
-00001750: 3837 3332 2037 2e37 3330 3133 3139 2c38  8732 7.7301319,8
-00001760: 2e34 3533 3233 3033 205a 220d 0a20 2020  .4532303 Z"..   
-00001770: 2020 2020 6964 3d22 7061 7468 3439 3335      id="path4935
-00001780: 220d 0a20 2020 2020 2020 696e 6b73 6361  "..       inksca
-00001790: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-000017a0: 7661 7475 7265 3d22 3022 0d0a 2020 2020  vature="0"..    
-000017b0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-000017c0: 7479 7065 733d 2263 6363 6322 0d0a 2020  types="cccc"..  
-000017d0: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
-000017e0: 7468 2d65 6666 6563 743d 2223 7061 7468  th-effect="#path
-000017f0: 2d65 6666 6563 7435 3338 3122 0d0a 2020  -effect5381"..  
-00001800: 2020 2020 2069 6e6b 7363 6170 653a 6f72       inkscape:or
-00001810: 6967 696e 616c 2d64 3d22 4d20 372e 3335  iginal-d="M 7.35
-00001820: 3833 3239 392c 382e 3139 3937 3238 3320  83299,8.1997283 
-00001830: 4320 362e 3639 3534 3137 332c 392e 3137  C 6.6954173,9.17
-00001840: 3230 3030 3120 352e 3034 3332 3731 342c  20001 5.0432714,
-00001850: 392e 3035 3833 3434 3920 352e 3531 3830  9.0583449 5.5180
-00001860: 3239 362c 392e 3939 3539 3438 3720 362e  296,9.9959487 6.
-00001870: 3035 3932 3331 2c31 302e 3933 3333 3337  059231,10.933337
-00001880: 2034 2e36 3735 3830 3733 2c31 312e 3534   4.6758073,11.54
-00001890: 3138 3233 2033 2e39 3737 3437 3537 2c31  1823 3.9774757,1
-000018a0: 312e 3133 3836 3431 2033 2e32 3938 3536  1.138641 3.29856
-000018b0: 3431 2c31 302e 3734 3636 3731 2033 2e30  41,10.746671 3.0
-000018c0: 3838 3830 3535 2c31 322e 3435 3537 3733  888055,12.455773
-000018d0: 2031 2e37 3839 3836 342c 3133 2e31 3933   1.789864,13.193
-000018e0: 3637 220d 0a20 2020 2020 2020 7472 616e  67"..       tran
-000018f0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00001900: 2830 2e34 3132 3037 3136 312c 2d31 2e34  (0.41207161,-1.4
-00001910: 3537 3234 3135 2922 202f 3e0d 0a20 2020  572415)" />..   
-00001920: 203c 7061 7468 0d0a 2020 2020 2020 2073   <path..       s
-00001930: 7479 6c65 3d22 6669 6c6c 3a23 3030 3333  tyle="fill:#0033
-00001940: 3830 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  80;fill-rule:non
-00001950: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
-00001960: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
-00001970: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00001980: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00001990: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-000019a0: 6b65 2d6f 7061 6369 7479 3a31 220d 0a20  ke-opacity:1".. 
-000019b0: 2020 2020 2020 643d 226d 2037 2e37 3235        d="m 7.725
-000019c0: 3932 3231 2c38 2e30 3334 3030 3035 2063  9221,8.0340005 c
-000019d0: 2030 2c30 2e36 3732 3932 3239 2030 2e30   0,0.6729229 0.0
-000019e0: 3738 3238 352c 312e 3331 3230 3436 3620  78285,1.3120466 
-000019f0: 302e 3032 3935 3237 2c31 2e36 3833 3530  0.029527,1.68350
-00001a00: 3834 202d 302e 3034 3837 3538 2c30 2e33  84 -0.048758,0.3
-00001a10: 3731 3436 3231 2030 2e30 3131 3630 332c  714621 0.011603,
-00001a20: 302e 3430 3432 3039 3120 2d30 2e34 3333  0.4042091 -0.433
-00001a30: 3137 3437 2c30 2e34 3034 3230 3931 202d  1747,0.4042091 -
-00001a40: 302e 3530 3935 3139 312c 3020 2d30 2e39  0.5095191,0 -0.9
-00001a50: 3330 3031 3937 2c30 2e31 3331 3034 3920  300197,0.131049 
-00001a60: 2d31 2e32 3037 3039 3432 2c30 2e34 3139  -1.2070942,0.419
-00001a70: 3231 3320 2d30 2e32 3737 3037 3435 2c30  213 -0.2770745,0
-00001a80: 2e32 3838 3136 3420 2d30 2e33 3530 3239  .288164 -0.35029
-00001a90: 3437 2c30 2e36 3737 3734 3520 2d30 2e33  47,0.677745 -0.3
-00001aa0: 3235 3438 3738 2c31 2e30 3231 3135 3520  254878,1.021155 
-00001ab0: 302e 3034 3938 372c 302e 3537 3037 3132  0.04987,0.570712
-00001ac0: 2030 2e32 3830 3635 3034 2c31 2e30 3338   0.2806504,1.038
-00001ad0: 3438 3320 302e 3438 3438 3137 352c 312e  483 0.4848175,1.
-00001ae0: 3336 3332 3536 2030 2e31 3536 3533 3338  363256 0.1565338
-00001af0: 2c30 2e32 3535 3130 3520 302e 3132 3234  ,0.255105 0.1224
-00001b00: 3734 392c 302e 3530 3131 3839 202d 302e  749,0.501189 -0.
-00001b10: 3030 3739 322c 302e 3535 3939 3231 202d  00792,0.559921 -
-00001b20: 302e 3633 3938 3836 2c30 2e35 3832 3837  0.639886,0.58287
-00001b30: 3520 2d31 2e31 3430 3037 3931 2c30 2e37  5 -1.1400791,0.7
-00001b40: 3933 3231 3220 2d31 2e32 3732 3636 3134  93212 -1.2726614
-00001b50: 2c30 2e39 3537 3137 3220 2d30 2e31 3332  ,0.957172 -0.132
-00001b60: 3033 3537 2c30 2e31 3633 3238 3420 2d30  0357,0.163284 -0
-00001b70: 2e30 3430 3630 342c 302e 3139 3138 3636  .040604,0.191866
-00001b80: 202d 302e 3034 3036 3034 2c30 2e31 3931   -0.040604,0.191
-00001b90: 3836 3620 302c 3020 2d30 2e30 3231 3334  866 0,0 -0.02134
-00001ba0: 352c 302e 3038 3437 3120 302e 3138 3035  5,0.08471 0.1805
-00001bb0: 3237 332c 302e 3037 3035 3820 2d30 2e30  273,0.07058 -0.0
-00001bc0: 3134 3335 372c 302e 3030 3120 302e 3833  14357,0.001 0.83
-00001bd0: 3831 3036 392c 2d30 2e30 3839 3720 312e  81069,-0.0897 1.
-00001be0: 3630 3533 3832 352c 2d30 2e36 3031 3036  6053825,-0.60106
-00001bf0: 3320 302e 3338 3933 3436 312c 2d30 2e33  3 0.3893461,-0.3
-00001c00: 3430 3037 3720 302e 3632 3634 3538 312c  40077 0.6264581,
-00001c10: 2d30 2e39 3732 3632 3920 302e 3239 3739  -0.972629 0.2979
-00001c20: 3733 322c 2d31 2e36 3036 3234 3120 2d30  732,-1.606241 -0
-00001c30: 2e31 3532 3037 3737 2c2d 302e 3239 3139  .1520777,-0.2919
-00001c40: 3538 202d 302e 3333 3337 3930 322c 2d30  58 -0.3337902,-0
-00001c50: 2e36 3630 3932 3220 2d30 2e33 3439 3834  .660922 -0.34984
-00001c60: 3935 2c2d 312e 3030 3033 3339 202d 302e  95,-1.000339 -0.
-00001c70: 3031 3333 3038 2c2d 302e 3138 3432 3239  013308,-0.184229
-00001c80: 2030 2e30 3139 3935 322c 2d30 2e32 3733   0.019952,-0.273
-00001c90: 3632 3120 302e 3037 3635 3834 2c2d 302e  621 0.076584,-0.
-00001ca0: 3333 3235 3220 302e 3035 3636 3332 2c2d  33252 0.056632,-
-00001cb0: 302e 3035 3839 2030 2e31 3937 3036 3439  0.0589 0.1970649
-00001cc0: 2c2d 302e 3134 3330 3033 2030 2e35 3538  ,-0.143003 0.558
-00001cd0: 3333 3732 2c2d 302e 3134 3330 3033 2030  3372,-0.143003 0
-00001ce0: 2e37 3631 3935 3136 2c30 2031 2e32 3439  .7619516,0 1.249
-00001cf0: 3133 3638 2c2d 302e 3630 3531 3539 2031  1368,-0.605159 1
-00001d00: 2e33 3235 3532 3032 2c2d 312e 3138 3730  .3255202,-1.1870
-00001d10: 3738 3920 302e 3037 3633 3834 2c2d 302e  789 0.076384,-0.
-00001d20: 3538 3139 3230 3420 2d30 2e30 3231 3837  5819204 -0.02187
-00001d30: 322c 2d31 2e32 3131 3635 3535 202d 302e  2,-1.2116555 -0.
-00001d40: 3032 3138 3732 2c2d 312e 3830 3036 3338  021872,-1.800638
-00001d50: 3620 7a22 0d0a 2020 2020 2020 2069 643d  6 z"..       id=
-00001d60: 2270 6174 6834 3933 352d 3622 0d0a 2020  "path4935-6"..  
-00001d70: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00001d80: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-00001d90: 653d 2230 220d 0a20 2020 2020 2020 736f  e="0"..       so
-00001da0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00001db0: 3d22 6363 6363 220d 0a20 2020 2020 2020  ="cccc"..       
-00001dc0: 696e 6b73 6361 7065 3a70 6174 682d 6566  inkscape:path-ef
-00001dd0: 6665 6374 3d22 2370 6174 682d 6566 6665  fect="#path-effe
-00001de0: 6374 3533 3831 2d33 220d 0a20 2020 2020  ct5381-3"..     
-00001df0: 2020 696e 6b73 6361 7065 3a6f 7269 6769    inkscape:origi
-00001e00: 6e61 6c2d 643d 226d 2038 2e31 3735 3932  nal-d="m 8.17592
-00001e10: 3231 2c38 2e30 3334 3030 3031 2063 2030  21,8.0340001 c 0
-00001e20: 2c31 2e32 3631 3930 3632 2030 2e33 3533  ,1.2619062 0.353
-00001e30: 3038 3038 2c32 2e35 3337 3731 3739 202d  0808,2.5377179 -
-00001e40: 302e 3835 3336 3438 322c 322e 3533 3737  0.8536482,2.5377
-00001e50: 3137 3920 2d31 2e35 3036 3538 342c 3020  179 -1.506584,0 
-00001e60: 2d31 2e31 3538 3133 3638 2c31 2e32 3838  -1.1581368,1.288
-00001e70: 3036 3120 2d30 2e36 3636 3431 382c 322e  061 -0.666418,2.
-00001e80: 3133 3937 3433 2030 2e35 3734 3933 3135  139743 0.5749315
-00001e90: 2c31 2e30 3535 3730 3320 2d30 2e34 3132  ,1.055703 -0.412
-00001ea0: 3336 3038 2c31 2e31 3839 3931 202d 312e  3608,1.18991 -1.
-00001eb0: 3731 3133 3032 332c 312e 3932 3738 3037  7113023,1.927807
-00001ec0: 220d 0a20 2020 2020 2020 7472 616e 7366  "..       transf
-00001ed0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2832  orm="translate(2
-00001ee0: 2e35 3634 3531 3735 2c2d 302e 3436 3035  .5645175,-0.4605
-00001ef0: 3337 3334 2922 202f 3e0d 0a20 2020 203c  3734)" />..    <
-00001f00: 7061 7468 0d0a 2020 2020 2020 2073 7479  path..       sty
-00001f10: 6c65 3d22 6669 6c6c 3a23 3030 3333 3830  le="fill:#003380
-00001f20: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
-00001f30: 726f 3b73 7472 6f6b 653a 6e6f 6e65 3b73  ro;stroke:none;s
-00001f40: 7472 6f6b 652d 7769 6474 683a 3170 783b  troke-width:1px;
-00001f50: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00001f60: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-00001f70: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00001f80: 2d6f 7061 6369 7479 3a31 220d 0a20 2020  -opacity:1"..   
-00001f90: 2020 2020 643d 226d 2037 2e37 3235 3932      d="m 7.72592
-00001fa0: 3231 2c38 2e30 3334 3030 3035 2063 2030  21,8.0340005 c 0
-00001fb0: 2c30 2e36 3732 3932 3239 2030 2e30 3738  ,0.6729229 0.078
-00001fc0: 3238 352c 312e 3331 3230 3436 3620 302e  285,1.3120466 0.
-00001fd0: 3032 3935 3237 2c31 2e36 3833 3530 3834  029527,1.6835084
-00001fe0: 202d 302e 3034 3837 3538 2c30 2e33 3731   -0.048758,0.371
-00001ff0: 3436 3231 2030 2e30 3131 3630 332c 302e  4621 0.011603,0.
-00002000: 3430 3432 3039 3120 2d30 2e34 3333 3137  4042091 -0.43317
-00002010: 3437 2c30 2e34 3034 3230 3931 202d 302e  47,0.4042091 -0.
-00002020: 3530 3935 3139 312c 3020 2d30 2e39 3330  5095191,0 -0.930
-00002030: 3031 3937 2c30 2e31 3331 3034 3920 2d31  0197,0.131049 -1
-00002040: 2e32 3037 3039 3432 2c30 2e34 3139 3231  .2070942,0.41921
-00002050: 3320 2d30 2e32 3737 3037 3435 2c30 2e32  3 -0.2770745,0.2
-00002060: 3838 3136 3420 2d30 2e33 3530 3239 3437  88164 -0.3502947
-00002070: 2c30 2e36 3737 3734 3520 2d30 2e33 3235  ,0.677745 -0.325
-00002080: 3438 3738 2c31 2e30 3231 3135 3520 302e  4878,1.021155 0.
-00002090: 3034 3938 372c 302e 3537 3037 3132 2030  04987,0.570712 0
-000020a0: 2e32 3830 3635 3034 2c31 2e30 3338 3438  .2806504,1.03848
-000020b0: 3320 302e 3438 3438 3137 352c 312e 3336  3 0.4848175,1.36
-000020c0: 3332 3536 2030 2e31 3536 3533 3338 2c30  3256 0.1565338,0
-000020d0: 2e32 3535 3130 3520 302e 3132 3234 3734  .255105 0.122474
-000020e0: 392c 302e 3530 3131 3839 202d 302e 3030  9,0.501189 -0.00
-000020f0: 3739 322c 302e 3535 3939 3231 202d 302e  792,0.559921 -0.
-00002100: 3633 3938 3836 2c30 2e35 3832 3837 3520  639886,0.582875 
-00002110: 2d31 2e31 3430 3037 3931 2c30 2e37 3933  -1.1400791,0.793
-00002120: 3231 3220 2d31 2e32 3732 3636 3134 2c30  212 -1.2726614,0
-00002130: 2e39 3537 3137 3220 2d30 2e31 3332 3033  .957172 -0.13203
-00002140: 3537 2c30 2e31 3633 3238 3420 2d30 2e30  57,0.163284 -0.0
-00002150: 3430 3630 342c 302e 3139 3138 3636 202d  40604,0.191866 -
-00002160: 302e 3034 3036 3034 2c30 2e31 3931 3836  0.040604,0.19186
-00002170: 3620 302c 3020 2d30 2e30 3231 3334 352c  6 0,0 -0.021345,
-00002180: 302e 3038 3437 3120 302e 3138 3035 3237  0.08471 0.180527
-00002190: 332c 302e 3037 3035 3820 2d30 2e30 3134  3,0.07058 -0.014
-000021a0: 3335 372c 302e 3030 3120 302e 3833 3831  357,0.001 0.8381
-000021b0: 3036 392c 2d30 2e30 3839 3720 312e 3630  069,-0.0897 1.60
-000021c0: 3533 3832 352c 2d30 2e36 3031 3036 3320  53825,-0.601063 
-000021d0: 302e 3338 3933 3436 312c 2d30 2e33 3430  0.3893461,-0.340
-000021e0: 3037 3720 302e 3632 3634 3538 312c 2d30  077 0.6264581,-0
-000021f0: 2e39 3732 3632 3920 302e 3239 3739 3733  .972629 0.297973
-00002200: 322c 2d31 2e36 3036 3234 3120 2d30 2e31  2,-1.606241 -0.1
-00002210: 3532 3037 3737 2c2d 302e 3239 3139 3538  520777,-0.291958
-00002220: 202d 302e 3333 3337 3930 322c 2d30 2e36   -0.3337902,-0.6
-00002230: 3630 3932 3220 2d30 2e33 3439 3834 3935  60922 -0.3498495
-00002240: 2c2d 312e 3030 3033 3339 202d 302e 3031  ,-1.000339 -0.01
-00002250: 3333 3038 2c2d 302e 3138 3432 3239 2030  3308,-0.184229 0
-00002260: 2e30 3139 3935 322c 2d30 2e32 3733 3632  .019952,-0.27362
-00002270: 3120 302e 3037 3635 3834 2c2d 302e 3333  1 0.076584,-0.33
-00002280: 3235 3220 302e 3035 3636 3332 2c2d 302e  252 0.056632,-0.
-00002290: 3035 3839 2030 2e31 3937 3036 3439 2c2d  0589 0.1970649,-
-000022a0: 302e 3134 3330 3033 2030 2e35 3538 3333  0.143003 0.55833
-000022b0: 3732 2c2d 302e 3134 3330 3033 2030 2e37  72,-0.143003 0.7
-000022c0: 3631 3935 3136 2c30 2031 2e32 3439 3133  619516,0 1.24913
-000022d0: 3638 2c2d 302e 3630 3531 3539 2031 2e33  68,-0.605159 1.3
-000022e0: 3235 3532 3032 2c2d 312e 3138 3730 3738  255202,-1.187078
-000022f0: 3920 302e 3037 3633 3834 2c2d 302e 3538  9 0.076384,-0.58
-00002300: 3139 3230 3420 2d30 2e30 3231 3837 322c  19204 -0.021872,
-00002310: 2d31 2e32 3131 3635 3535 202d 302e 3032  -1.2116555 -0.02
-00002320: 3138 3732 2c2d 312e 3830 3036 3338 3620  1872,-1.8006386 
-00002330: 7a22 0d0a 2020 2020 2020 2069 643d 2270  z"..       id="p
-00002340: 6174 6834 3933 352d 362d 3322 0d0a 2020  ath4935-6-3"..  
-00002350: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00002360: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-00002370: 653d 2230 220d 0a20 2020 2020 2020 736f  e="0"..       so
-00002380: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00002390: 3d22 6363 6363 220d 0a20 2020 2020 2020  ="cccc"..       
-000023a0: 696e 6b73 6361 7065 3a70 6174 682d 6566  inkscape:path-ef
-000023b0: 6665 6374 3d22 2370 6174 682d 6566 6665  fect="#path-effe
-000023c0: 6374 3533 3831 2d33 2d39 220d 0a20 2020  ct5381-3-9"..   
-000023d0: 2020 2020 696e 6b73 6361 7065 3a6f 7269      inkscape:ori
-000023e0: 6769 6e61 6c2d 643d 226d 2038 2e31 3735  ginal-d="m 8.175
-000023f0: 3932 3231 2c38 2e30 3334 3030 3031 2063  9221,8.0340001 c
-00002400: 2030 2c31 2e32 3631 3930 3632 2030 2e33   0,1.2619062 0.3
-00002410: 3533 3038 3038 2c32 2e35 3337 3731 3739  530808,2.5377179
-00002420: 202d 302e 3835 3336 3438 322c 322e 3533   -0.8536482,2.53
-00002430: 3737 3137 3920 2d31 2e35 3036 3538 342c  77179 -1.506584,
-00002440: 3020 2d31 2e31 3538 3133 3638 2c31 2e32  0 -1.1581368,1.2
-00002450: 3838 3036 3120 2d30 2e36 3636 3431 382c  88061 -0.666418,
-00002460: 322e 3133 3937 3433 2030 2e35 3734 3933  2.139743 0.57493
-00002470: 3135 2c31 2e30 3535 3730 3320 2d30 2e34  15,1.055703 -0.4
-00002480: 3132 3336 3038 2c31 2e31 3839 3931 202d  123608,1.18991 -
-00002490: 312e 3731 3133 3032 332c 312e 3932 3738  1.7113023,1.9278
-000024a0: 3037 220d 0a20 2020 2020 2020 7472 616e  07"..       tran
-000024b0: 7366 6f72 6d3d 226d 6174 7269 7828 302e  sform="matrix(0.
-000024c0: 3734 3533 3433 3931 2c2d 302e 3130 3037  74534391,-0.1007
-000024d0: 3430 372c 302e 3130 3037 3430 372c 302e  407,0.1007407,0.
-000024e0: 3734 3533 3433 3931 2c31 2e31 3639 3630  74534391,1.16960
-000024f0: 3139 2c31 2e35 3830 3434 3436 2922 202f  19,1.5804446)" /
-00002500: 3e0d 0a20 2020 203c 7061 7468 0d0a 2020  >..    <path..  
-00002510: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00002520: 3a23 3030 3333 3830 3b66 696c 6c2d 7275  :#003380;fill-ru
-00002530: 6c65 3a6e 6f6e 7a65 726f 3b73 7472 6f6b  le:nonzero;strok
-00002540: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00002550: 6474 683a 3170 783b 7374 726f 6b65 2d6c  dth:1px;stroke-l
-00002560: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-00002570: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-00002580: 723b 7374 726f 6b65 2d6f 7061 6369 7479  r;stroke-opacity
-00002590: 3a31 220d 0a20 2020 2020 2020 643d 224d  :1"..       d="M
-000025a0: 2036 2e39 3836 3532 3735 2c37 2e39 3436   6.9865275,7.946
-000025b0: 3232 3639 2043 2036 2e37 3537 3638 3937  2269 C 6.7576897
-000025c0: 2c38 2e32 3831 3835 3535 2036 2e32 3835  ,8.2818555 6.285
-000025d0: 3034 3339 2c38 2e34 3739 3537 3737 2035  0439,8.4795777 5
-000025e0: 2e38 3136 3234 3032 2c38 2e37 3035 3433  .8162402,8.70543
-000025f0: 3435 2035 2e35 3831 3833 3834 2c38 2e38  45 5.5818384,8.8
-00002600: 3138 3336 3239 2035 2e33 3336 3736 392c  183629 5.336769,
-00002610: 382e 3933 3035 3437 3820 352e 3134 3732  8.9305478 5.1472
-00002620: 3337 332c 392e 3139 3330 3234 3320 342e  373,9.1930243 4.
-00002630: 3935 3737 3035 352c 392e 3435 3535 3030  9577055,9.455500
-00002640: 3920 342e 3935 3230 3130 372c 392e 3837  9 4.9520107,9.87
-00002650: 3432 3537 3520 352e 3131 3635 3632 372c  42575 5.1165627,
-00002660: 3130 2e31 3939 3233 3320 6120 312e 3032  10.199233 a 1.02
-00002670: 3436 3030 382c 312e 3032 3436 3030 3820  46008,1.0246008 
-00002680: 3020 3020 3020 302e 3030 3637 372c 302e  0 0 0 0.00677,0.
-00002690: 3031 3331 3420 312e 3834 3730 3732 322c  01314 1.8470722,
-000026a0: 312e 3834 3730 3732 3220 3020 3020 3120  1.8470722 0 0 1 
-000026b0: 302e 3030 3439 382c 302e 3030 3836 2063  0.00498,0.0086 c
-000026c0: 2030 2e31 3636 3530 3433 2c30 2e32 3838   0.1665043,0.288
-000026d0: 3339 3420 302e 3038 3336 3034 2c30 2e33  394 0.083604,0.3
-000026e0: 3234 3932 202d 302e 3134 3639 3532 322c  2492 -0.1469522,
-000026f0: 302e 3436 3330 3031 202d 302e 3233 3035  0.463001 -0.2305
-00002700: 3536 322c 302e 3133 3830 3831 202d 302e  562,0.138081 -0.
-00002710: 3632 3630 3531 312c 302e 3135 3332 3231  6260511,0.153221
-00002720: 202d 302e 3737 3838 3930 322c 302e 3036   -0.7788902,0.06
-00002730: 3439 3820 302c 3020 2d33 2e36 3165 2d35  498 0,0 -3.61e-5
-00002740: 2c2d 322e 3165 2d35 202d 332e 3631 652d  ,-2.1e-5 -3.61e-
-00002750: 352c 2d32 2e31 652d 3520 2d30 2e33 3630  5,-2.1e-5 -0.360
-00002760: 3732 3039 2c2d 302e 3136 3935 3037 202d  7209,-0.169507 -
-00002770: 302e 3731 3331 3535 2c2d 302e 3130 3136  0.713155,-0.1016
-00002780: 3331 202d 302e 3936 3231 3438 312c 302e  31 -0.9621481,0.
-00002790: 3130 3331 3331 202d 302e 3235 3832 3139  103131 -0.258219
-000027a0: 332c 302e 3234 3134 3136 202d 302e 3430  3,0.241416 -0.40
-000027b0: 3037 3839 322c 302e 3530 3135 3437 202d  07892,0.501547 -
-000027c0: 302e 3438 3538 3830 312c 302e 3636 3030  0.4858801,0.6600
-000027d0: 3235 202d 302e 3536 3239 3336 392c 302e  25 -0.5629369,0.
-000027e0: 3933 3230 3439 202d 302e 3831 3034 3332  932049 -0.810432
-000027f0: 392c 312e 3235 3634 3535 202d 302e 3932  9,1.256455 -0.92
-00002800: 3431 3233 352c 312e 3434 3535 3836 202d  41235,1.445586 -
-00002810: 302e 3131 3533 3232 352c 302e 3139 3138  0.1153225,0.1918
-00002820: 3436 202d 302e 3033 3339 3331 2c30 2e32  46 -0.033931,0.2
-00002830: 3332 3331 3620 2d30 2e30 3333 3933 312c  32316 -0.033931,
-00002840: 302e 3233 3233 3136 2030 2c30 202d 302e  0.232316 0,0 -0.
-00002850: 3030 3938 382c 302e 3131 3639 3733 2030  00988,0.116973 0
-00002860: 2e32 3333 3534 3436 2c30 2e30 3636 3538  .2335446,0.06658
-00002870: 2030 2e32 3431 3934 3739 2c2d 302e 3035   0.2419479,-0.05
-00002880: 3030 3920 302e 3738 3739 3636 392c 2d30  009 0.7879669,-0
-00002890: 2e32 3937 3835 3220 312e 3434 3830 3331  .297852 1.448031
-000028a0: 2c2d 312e 3238 3336 3736 2030 2e31 3233  ,-1.283676 0.123
-000028b0: 3031 3136 2c2d 302e 3136 3739 3431 2030  0116,-0.167941 0
-000028c0: 2e32 3431 3432 3737 2c2d 302e 3337 3137  .2414277,-0.3717
-000028d0: 3338 2030 2e33 3435 3536 3937 2c2d 302e  38 0.3455697,-0.
-000028e0: 3434 3336 3732 202d 302e 3031 3930 3233  443672 -0.019023
-000028f0: 2c30 2e30 3036 3620 2d30 2e30 3037 3138  ,0.0066 -0.00718
-00002900: 2c2d 302e 3030 3236 202d 302e 3037 3130  ,-0.0026 -0.0710
-00002910: 3331 2c2d 382e 3532 652d 3420 302c 3020  31,-8.52e-4 0,0 
-00002920: 342e 3665 2d36 2c32 652d 3620 342e 3765  4.6e-6,2e-6 4.7e
-00002930: 2d36 2c32 652d 3620 302e 3534 3534 3932  -6,2e-6 0.545492
-00002940: 342c 302e 3331 3439 3431 2031 2e31 3930  4,0.314941 1.190
-00002950: 3837 3532 2c30 2e32 3237 3432 3920 312e  8752,0.227429 1.
-00002960: 3639 3133 3133 342c 2d30 2e30 3732 3239  6913134,-0.07229
-00002970: 2043 2035 2e39 3431 3332 3532 2c31 312e   C 5.9413252,11.
-00002980: 3135 3830 3932 2036 2e32 3738 3531 2c31  158092 6.27851,1
-00002990: 302e 3432 3834 3639 2035 2e39 3134 3138  0.428469 5.91418
-000029a0: 3739 2c39 2e37 3832 3234 3831 2035 2e38  79,9.7822481 5.8
-000029b0: 3437 3830 3436 2c39 2e36 3532 3836 3736  478046,9.6528676
-000029c0: 2035 2e38 3639 3634 3532 2c39 2e37 3239   5.8696452,9.729
-000029d0: 3934 3135 2035 2e38 3736 3839 3433 2c39  9415 5.8768943,9
-000029e0: 2e37 3139 3930 3235 2035 2e38 3834 3333  .7199025 5.88433
-000029f0: 3031 2c39 2e37 3039 3630 3439 2036 2e30  01,9.7096049 6.0
-00002a00: 3034 3731 3231 2c39 2e36 3133 3633 3539  047121,9.6136359
-00002a10: 2036 2e32 3036 3836 3539 2c39 2e35 3136   6.2068659,9.516
-00002a20: 3234 3337 2036 2e36 3131 3137 3337 2c39  2437 6.6111737,9
-00002a30: 2e33 3231 3435 3932 2037 2e32 3936 3035  .3214592 7.29605
-00002a40: 372c 392e 3038 3938 3733 3220 372e 3733  7,9.0898732 7.73
-00002a50: 3031 3331 392c 382e 3435 3332 3330 3320  01319,8.4532303 
-00002a60: 5a22 0d0a 2020 2020 2020 2069 643d 2270  Z"..       id="p
-00002a70: 6174 6834 3933 352d 3022 0d0a 2020 2020  ath4935-0"..    
-00002a80: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00002a90: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00002aa0: 2230 220d 0a20 2020 2020 2020 736f 6469  "0"..       sodi
-00002ab0: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-00002ac0: 6363 6363 220d 0a20 2020 2020 2020 696e  cccc"..       in
-00002ad0: 6b73 6361 7065 3a70 6174 682d 6566 6665  kscape:path-effe
-00002ae0: 6374 3d22 2370 6174 682d 6566 6665 6374  ct="#path-effect
-00002af0: 3533 3831 2d36 220d 0a20 2020 2020 2020  5381-6"..       
-00002b00: 696e 6b73 6361 7065 3a6f 7269 6769 6e61  inkscape:origina
-00002b10: 6c2d 643d 224d 2037 2e33 3538 3332 3939  l-d="M 7.3583299
-00002b20: 2c38 2e31 3939 3732 3833 2043 2036 2e36  ,8.1997283 C 6.6
-00002b30: 3935 3431 3733 2c39 2e31 3732 3030 3031  954173,9.1720001
-00002b40: 2035 2e30 3433 3237 3134 2c39 2e30 3538   5.0432714,9.058
-00002b50: 3334 3439 2035 2e35 3138 3032 3936 2c39  3449 5.5180296,9
-00002b60: 2e39 3935 3934 3837 2036 2e30 3539 3233  .9959487 6.05923
-00002b70: 312c 3130 2e39 3333 3333 3720 342e 3637  1,10.933337 4.67
-00002b80: 3538 3037 332c 3131 2e35 3431 3832 3320  58073,11.541823 
-00002b90: 332e 3937 3734 3735 372c 3131 2e31 3338  3.9774757,11.138
-00002ba0: 3634 3120 332e 3239 3835 3634 312c 3130  641 3.2985641,10
-00002bb0: 2e37 3436 3637 3120 332e 3038 3838 3035  .746671 3.088805
-00002bc0: 352c 3132 2e34 3535 3737 3320 312e 3738  5,12.455773 1.78
-00002bd0: 3938 3634 2c31 332e 3139 3336 3722 0d0a  9864,13.19367"..
-00002be0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00002bf0: 3d22 6d61 7472 6978 282d 302e 3732 3834  ="matrix(-0.7284
-00002c00: 3236 3239 2c2d 302e 3438 3334 3038 3631  2629,-0.48340861
-00002c10: 2c2d 302e 3438 3931 3232 3834 2c30 2e37  ,-0.48912284,0.7
-00002c20: 3139 3931 3633 372c 3230 2e37 3933 3332  1991637,20.79332
-00002c30: 342c 352e 3533 3236 3739 3229 2220 2f3e  4,5.5326792)" />
-00002c40: 0d0a 2020 3c2f 673e 0d0a 3c2f 7376 673e  ..  </g>..</svg>
-00002c50: 0d0a                                     ..
+00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
+00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
+00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
+00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
+00000070: 0a0a 3c73 7667 0a20 2020 786d 6c6e 733a  ..<svg.   xmlns:
+00000080: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
+00000090: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
+000000a0: 312e 312f 220a 2020 2078 6d6c 6e73 3a63  1.1/".   xmlns:c
+000000b0: 633d 2268 7474 703a 2f2f 6372 6561 7469  c="http://creati
+000000c0: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
+000000d0: 2322 0a20 2020 786d 6c6e 733a 7264 663d  #".   xmlns:rdf=
+000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+000000f0: 7267 2f31 3939 392f 3032 2f32 322d 7264  rg/1999/02/22-rd
+00000100: 662d 7379 6e74 6178 2d6e 7323 220a 2020  f-syntax-ns#".  
+00000110: 2078 6d6c 6e73 3a73 7667 3d22 6874 7470   xmlns:svg="http
+00000120: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000130: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
+00000140: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+00000150: 6f72 672f 3230 3030 2f73 7667 220a 2020  org/2000/svg".  
+00000160: 2078 6d6c 6e73 3a73 6f64 6970 6f64 693d   xmlns:sodipodi=
+00000170: 2268 7474 703a 2f2f 736f 6469 706f 6469  "http://sodipodi
+00000180: 2e73 6f75 7263 6566 6f72 6765 2e6e 6574  .sourceforge.net
+00000190: 2f44 5444 2f73 6f64 6970 6f64 692d 302e  /DTD/sodipodi-0.
+000001a0: 6474 6422 0a20 2020 786d 6c6e 733a 696e  dtd".   xmlns:in
+000001b0: 6b73 6361 7065 3d22 6874 7470 3a2f 2f77  kscape="http://w
+000001c0: 7777 2e69 6e6b 7363 6170 652e 6f72 672f  ww.inkscape.org/
+000001d0: 6e61 6d65 7370 6163 6573 2f69 6e6b 7363  namespaces/inksc
+000001e0: 6170 6522 0a20 2020 7769 6474 683d 2231  ape".   width="1
+000001f0: 3670 7822 0a20 2020 6865 6967 6874 3d22  6px".   height="
+00000200: 3136 7078 220a 2020 2076 6965 7742 6f78  16px".   viewBox
+00000210: 3d22 3020 3020 3136 2031 3622 0a20 2020  ="0 0 16 16".   
+00000220: 7665 7273 696f 6e3d 2231 2e31 220a 2020  version="1.1".  
+00000230: 2069 643d 2253 5647 526f 6f74 220a 2020   id="SVGRoot".  
+00000240: 2069 6e6b 7363 6170 653a 7665 7273 696f   inkscape:versio
+00000250: 6e3d 2230 2e39 322e 3520 2832 3036 3065  n="0.92.5 (2060e
+00000260: 6331 6639 662c 2032 3032 302d 3034 2d30  c1f9f, 2020-04-0
+00000270: 3829 220a 2020 2073 6f64 6970 6f64 693a  8)".   sodipodi:
+00000280: 646f 636e 616d 653d 2262 6f78 6a65 6c6c  docname="boxjell
+00000290: 792d 7468 6963 6b2e 7376 6722 3e0a 2020  y-thick.svg">.  
+000002a0: 3c64 6566 730a 2020 2020 2069 643d 2264  <defs.     id="d
+000002b0: 6566 7331 3022 3e0a 2020 2020 3c69 6e6b  efs10">.    <ink
+000002c0: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
+000002d0: 740a 2020 2020 2020 2065 6666 6563 743d  t.       effect=
+000002e0: 2274 6170 6572 5f73 7472 6f6b 6522 0a20  "taper_stroke". 
+000002f0: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
+00000300: 6666 6563 7435 3338 3122 0a20 2020 2020  ffect5381".     
+00000310: 2020 6973 5f76 6973 6962 6c65 3d22 7472    is_visible="tr
+00000320: 7565 220a 2020 2020 2020 2073 7472 6f6b  ue".       strok
+00000330: 655f 7769 6474 683d 2230 2e39 220a 2020  e_width="0.9".  
+00000340: 2020 2020 2061 7474 6163 685f 7374 6172       attach_star
+00000350: 743d 2231 652d 3037 220a 2020 2020 2020  t="1e-07".      
+00000360: 2065 6e64 5f6f 6666 7365 743d 2230 2e39   end_offset="0.9
+00000370: 3939 3939 220a 2020 2020 2020 2073 6d6f  9999".       smo
+00000380: 6f74 6869 6e67 3d22 312e 3122 0a20 2020  othing="1.1".   
+00000390: 2020 2020 6a6f 696e 7479 7065 3d22 6578      jointype="ex
+000003a0: 7472 6170 6f6c 6174 6564 220a 2020 2020  trapolated".    
+000003b0: 2020 206d 6974 6572 5f6c 696d 6974 3d22     miter_limit="
+000003c0: 3130 3022 202f 3e0a 2020 2020 3c69 6e6b  100" />.    <ink
+000003d0: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
+000003e0: 740a 2020 2020 2020 2065 6666 6563 743d  t.       effect=
+000003f0: 2274 6170 6572 5f73 7472 6f6b 6522 0a20  "taper_stroke". 
+00000400: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
+00000410: 6666 6563 7435 3338 312d 3322 0a20 2020  ffect5381-3".   
+00000420: 2020 2020 6973 5f76 6973 6962 6c65 3d22      is_visible="
+00000430: 7472 7565 220a 2020 2020 2020 2073 7472  true".       str
+00000440: 6f6b 655f 7769 6474 683d 2230 2e39 220a  oke_width="0.9".
+00000450: 2020 2020 2020 2061 7474 6163 685f 7374         attach_st
+00000460: 6172 743d 2231 652d 3037 220a 2020 2020  art="1e-07".    
+00000470: 2020 2065 6e64 5f6f 6666 7365 743d 2231     end_offset="1
+00000480: 2e34 3232 3030 3934 220a 2020 2020 2020  .4220094".      
+00000490: 2073 6d6f 6f74 6869 6e67 3d22 312e 3122   smoothing="1.1"
+000004a0: 0a20 2020 2020 2020 6a6f 696e 7479 7065  .       jointype
+000004b0: 3d22 6578 7472 6170 6f6c 6174 6564 220a  ="extrapolated".
+000004c0: 2020 2020 2020 206d 6974 6572 5f6c 696d         miter_lim
+000004d0: 6974 3d22 3130 3022 202f 3e0a 2020 2020  it="100" />.    
+000004e0: 3c69 6e6b 7363 6170 653a 7061 7468 2d65  <inkscape:path-e
+000004f0: 6666 6563 740a 2020 2020 2020 2065 6666  ffect.       eff
+00000500: 6563 743d 2274 6170 6572 5f73 7472 6f6b  ect="taper_strok
+00000510: 6522 0a20 2020 2020 2020 6964 3d22 7061  e".       id="pa
+00000520: 7468 2d65 6666 6563 7435 3338 312d 332d  th-effect5381-3-
+00000530: 3722 0a20 2020 2020 2020 6973 5f76 6973  7".       is_vis
+00000540: 6962 6c65 3d22 7472 7565 220a 2020 2020  ible="true".    
+00000550: 2020 2073 7472 6f6b 655f 7769 6474 683d     stroke_width=
+00000560: 2231 220a 2020 2020 2020 2061 7474 6163  "1".       attac
+00000570: 685f 7374 6172 743d 2231 652d 3037 220a  h_start="1e-07".
+00000580: 2020 2020 2020 2065 6e64 5f6f 6666 7365         end_offse
+00000590: 743d 2231 2e34 3232 3030 3934 220a 2020  t="1.4220094".  
+000005a0: 2020 2020 2073 6d6f 6f74 6869 6e67 3d22       smoothing="
+000005b0: 312e 3122 0a20 2020 2020 2020 6a6f 696e  1.1".       join
+000005c0: 7479 7065 3d22 6578 7472 6170 6f6c 6174  type="extrapolat
+000005d0: 6564 220a 2020 2020 2020 206d 6974 6572  ed".       miter
+000005e0: 5f6c 696d 6974 3d22 3130 3022 202f 3e0a  _limit="100" />.
+000005f0: 2020 2020 3c69 6e6b 7363 6170 653a 7061      <inkscape:pa
+00000600: 7468 2d65 6666 6563 740a 2020 2020 2020  th-effect.      
+00000610: 2065 6666 6563 743d 2274 6170 6572 5f73   effect="taper_s
+00000620: 7472 6f6b 6522 0a20 2020 2020 2020 6964  troke".       id
+00000630: 3d22 7061 7468 2d65 6666 6563 7435 3338  ="path-effect538
+00000640: 312d 3222 0a20 2020 2020 2020 6973 5f76  1-2".       is_v
+00000650: 6973 6962 6c65 3d22 7472 7565 220a 2020  isible="true".  
+00000660: 2020 2020 2073 7472 6f6b 655f 7769 6474       stroke_widt
+00000670: 683d 2231 220a 2020 2020 2020 2061 7474  h="1".       att
+00000680: 6163 685f 7374 6172 743d 2231 652d 3037  ach_start="1e-07
+00000690: 220a 2020 2020 2020 2065 6e64 5f6f 6666  ".       end_off
+000006a0: 7365 743d 2230 2e39 3939 3939 220a 2020  set="0.99999".  
+000006b0: 2020 2020 2073 6d6f 6f74 6869 6e67 3d22       smoothing="
+000006c0: 312e 3122 0a20 2020 2020 2020 6a6f 696e  1.1".       join
+000006d0: 7479 7065 3d22 6578 7472 6170 6f6c 6174  type="extrapolat
+000006e0: 6564 220a 2020 2020 2020 206d 6974 6572  ed".       miter
+000006f0: 5f6c 696d 6974 3d22 3130 3022 202f 3e0a  _limit="100" />.
+00000700: 2020 2020 3c69 6e6b 7363 6170 653a 7061      <inkscape:pa
+00000710: 7468 2d65 6666 6563 740a 2020 2020 2020  th-effect.      
+00000720: 2065 6666 6563 743d 2274 6170 6572 5f73   effect="taper_s
+00000730: 7472 6f6b 6522 0a20 2020 2020 2020 6964  troke".       id
+00000740: 3d22 7061 7468 2d65 6666 6563 7435 3338  ="path-effect538
+00000750: 312d 332d 3122 0a20 2020 2020 2020 6973  1-3-1".       is
+00000760: 5f76 6973 6962 6c65 3d22 7472 7565 220a  _visible="true".
+00000770: 2020 2020 2020 2073 7472 6f6b 655f 7769         stroke_wi
+00000780: 6474 683d 2230 2e39 220a 2020 2020 2020  dth="0.9".      
+00000790: 2061 7474 6163 685f 7374 6172 743d 2231   attach_start="1
+000007a0: 652d 3037 220a 2020 2020 2020 2065 6e64  e-07".       end
+000007b0: 5f6f 6666 7365 743d 2231 2e34 3232 3030  _offset="1.42200
+000007c0: 3934 220a 2020 2020 2020 2073 6d6f 6f74  94".       smoot
+000007d0: 6869 6e67 3d22 312e 3122 0a20 2020 2020  hing="1.1".     
+000007e0: 2020 6a6f 696e 7479 7065 3d22 6578 7472    jointype="extr
+000007f0: 6170 6f6c 6174 6564 220a 2020 2020 2020  apolated".      
+00000800: 206d 6974 6572 5f6c 696d 6974 3d22 3130   miter_limit="10
+00000810: 3022 202f 3e0a 2020 2020 3c69 6e6b 7363  0" />.    <inksc
+00000820: 6170 653a 7061 7468 2d65 6666 6563 740a  ape:path-effect.
+00000830: 2020 2020 2020 2065 6666 6563 743d 2274         effect="t
+00000840: 6170 6572 5f73 7472 6f6b 6522 0a20 2020  aper_stroke".   
+00000850: 2020 2020 6964 3d22 7061 7468 2d65 6666      id="path-eff
+00000860: 6563 7435 3338 312d 3722 0a20 2020 2020  ect5381-7".     
+00000870: 2020 6973 5f76 6973 6962 6c65 3d22 7472    is_visible="tr
+00000880: 7565 220a 2020 2020 2020 2073 7472 6f6b  ue".       strok
+00000890: 655f 7769 6474 683d 2230 2e39 220a 2020  e_width="0.9".  
+000008a0: 2020 2020 2061 7474 6163 685f 7374 6172       attach_star
+000008b0: 743d 2231 652d 3037 220a 2020 2020 2020  t="1e-07".      
+000008c0: 2065 6e64 5f6f 6666 7365 743d 2230 2e39   end_offset="0.9
+000008d0: 3939 3939 220a 2020 2020 2020 2073 6d6f  9999".       smo
+000008e0: 6f74 6869 6e67 3d22 312e 3122 0a20 2020  othing="1.1".   
+000008f0: 2020 2020 6a6f 696e 7479 7065 3d22 6578      jointype="ex
+00000900: 7472 6170 6f6c 6174 6564 220a 2020 2020  trapolated".    
+00000910: 2020 206d 6974 6572 5f6c 696d 6974 3d22     miter_limit="
+00000920: 3130 3022 202f 3e0a 2020 2020 3c69 6e6b  100" />.    <ink
+00000930: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
+00000940: 740a 2020 2020 2020 2065 6666 6563 743d  t.       effect=
+00000950: 2274 6170 6572 5f73 7472 6f6b 6522 0a20  "taper_stroke". 
+00000960: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
+00000970: 6666 6563 7435 3338 312d 332d 3922 0a20  ffect5381-3-9". 
+00000980: 2020 2020 2020 6973 5f76 6973 6962 6c65        is_visible
+00000990: 3d22 7472 7565 220a 2020 2020 2020 2073  ="true".       s
+000009a0: 7472 6f6b 655f 7769 6474 683d 2230 2e39  troke_width="0.9
+000009b0: 220a 2020 2020 2020 2061 7474 6163 685f  ".       attach_
+000009c0: 7374 6172 743d 2231 652d 3037 220a 2020  start="1e-07".  
+000009d0: 2020 2020 2065 6e64 5f6f 6666 7365 743d       end_offset=
+000009e0: 2231 2e34 3232 3030 3934 220a 2020 2020  "1.4220094".    
+000009f0: 2020 2073 6d6f 6f74 6869 6e67 3d22 312e     smoothing="1.
+00000a00: 3122 0a20 2020 2020 2020 6a6f 696e 7479  1".       jointy
+00000a10: 7065 3d22 6578 7472 6170 6f6c 6174 6564  pe="extrapolated
+00000a20: 220a 2020 2020 2020 206d 6974 6572 5f6c  ".       miter_l
+00000a30: 696d 6974 3d22 3130 3022 202f 3e0a 2020  imit="100" />.  
+00000a40: 2020 3c69 6e6b 7363 6170 653a 7061 7468    <inkscape:path
+00000a50: 2d65 6666 6563 740a 2020 2020 2020 2065  -effect.       e
+00000a60: 6666 6563 743d 2274 6170 6572 5f73 7472  ffect="taper_str
+00000a70: 6f6b 6522 0a20 2020 2020 2020 6964 3d22  oke".       id="
+00000a80: 7061 7468 2d65 6666 6563 7435 3338 312d  path-effect5381-
+00000a90: 3622 0a20 2020 2020 2020 6973 5f76 6973  6".       is_vis
+00000aa0: 6962 6c65 3d22 7472 7565 220a 2020 2020  ible="true".    
+00000ab0: 2020 2073 7472 6f6b 655f 7769 6474 683d     stroke_width=
+00000ac0: 2230 2e39 220a 2020 2020 2020 2061 7474  "0.9".       att
+00000ad0: 6163 685f 7374 6172 743d 2231 652d 3037  ach_start="1e-07
+00000ae0: 220a 2020 2020 2020 2065 6e64 5f6f 6666  ".       end_off
+00000af0: 7365 743d 2230 2e39 3939 3939 220a 2020  set="0.99999".  
+00000b00: 2020 2020 2073 6d6f 6f74 6869 6e67 3d22       smoothing="
+00000b10: 312e 3122 0a20 2020 2020 2020 6a6f 696e  1.1".       join
+00000b20: 7479 7065 3d22 6578 7472 6170 6f6c 6174  type="extrapolat
+00000b30: 6564 220a 2020 2020 2020 206d 6974 6572  ed".       miter
+00000b40: 5f6c 696d 6974 3d22 3130 3022 202f 3e0a  _limit="100" />.
+00000b50: 2020 3c2f 6465 6673 3e0a 2020 3c73 6f64    </defs>.  <sod
+00000b60: 6970 6f64 693a 6e61 6d65 6476 6965 770a  ipodi:namedview.
+00000b70: 2020 2020 2069 643d 2262 6173 6522 0a20       id="base". 
+00000b80: 2020 2020 7061 6765 636f 6c6f 723d 2223      pagecolor="#
+00000b90: 6666 6666 6666 220a 2020 2020 2062 6f72  ffffff".     bor
+00000ba0: 6465 7263 6f6c 6f72 3d22 2336 3636 3636  dercolor="#66666
+00000bb0: 3622 0a20 2020 2020 626f 7264 6572 6f70  6".     borderop
+00000bc0: 6163 6974 793d 2231 2e30 220a 2020 2020  acity="1.0".    
+00000bd0: 2069 6e6b 7363 6170 653a 7061 6765 6f70   inkscape:pageop
+00000be0: 6163 6974 793d 2230 2e30 220a 2020 2020  acity="0.0".    
+00000bf0: 2069 6e6b 7363 6170 653a 7061 6765 7368   inkscape:pagesh
+00000c00: 6164 6f77 3d22 3222 0a20 2020 2020 696e  adow="2".     in
+00000c10: 6b73 6361 7065 3a7a 6f6f 6d3d 2234 352e  kscape:zoom="45.
+00000c20: 3235 3438 3334 220a 2020 2020 2069 6e6b  254834".     ink
+00000c30: 7363 6170 653a 6378 3d22 372e 3837 3538  scape:cx="7.8758
+00000c40: 3636 3522 0a20 2020 2020 696e 6b73 6361  665".     inksca
+00000c50: 7065 3a63 793d 2238 2e33 3638 3537 3132  pe:cy="8.3685712
+00000c60: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000c70: 646f 6375 6d65 6e74 2d75 6e69 7473 3d22  document-units="
+00000c80: 7078 220a 2020 2020 2069 6e6b 7363 6170  px".     inkscap
+00000c90: 653a 6375 7272 656e 742d 6c61 7965 723d  e:current-layer=
+00000ca0: 226c 6179 6572 3122 0a20 2020 2020 7368  "layer1".     sh
+00000cb0: 6f77 6772 6964 3d22 6661 6c73 6522 0a20  owgrid="false". 
+00000cc0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
+00000cd0: 646f 772d 7769 6474 683d 2232 3038 3022  dow-width="2080"
+00000ce0: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
+00000cf0: 696e 646f 772d 6865 6967 6874 3d22 3132  indow-height="12
+00000d00: 3236 220a 2020 2020 2069 6e6b 7363 6170  26".     inkscap
+00000d10: 653a 7769 6e64 6f77 2d78 3d22 3838 3222  e:window-x="882"
+00000d20: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
+00000d30: 696e 646f 772d 793d 2230 220a 2020 2020  indow-y="0".    
+00000d40: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+00000d50: 2d6d 6178 696d 697a 6564 3d22 3022 0a20  -maximized="0". 
+00000d60: 2020 2020 696e 6b73 6361 7065 3a67 7269      inkscape:gri
+00000d70: 642d 6262 6f78 3d22 7472 7565 220a 2020  d-bbox="true".  
+00000d80: 2020 2069 6e6b 7363 6170 653a 736e 6170     inkscape:snap
+00000d90: 2d6e 6f64 6573 3d22 6661 6c73 6522 202f  -nodes="false" /
+00000da0: 3e0a 2020 3c6d 6574 6164 6174 610a 2020  >.  <metadata.  
+00000db0: 2020 2069 643d 226d 6574 6164 6174 6131     id="metadata1
+00000dc0: 3322 3e0a 2020 2020 3c72 6466 3a52 4446  3">.    <rdf:RDF
+00000dd0: 3e0a 2020 2020 2020 3c63 633a 576f 726b  >.      <cc:Work
+00000de0: 0a20 2020 2020 2020 2020 7264 663a 6162  .         rdf:ab
+00000df0: 6f75 743d 2222 3e0a 2020 2020 2020 2020  out="">.        
+00000e00: 3c64 633a 666f 726d 6174 3e69 6d61 6765  <dc:format>image
+00000e10: 2f73 7667 2b78 6d6c 3c2f 6463 3a66 6f72  /svg+xml</dc:for
+00000e20: 6d61 743e 0a20 2020 2020 2020 203c 6463  mat>.        <dc
+00000e30: 3a74 7970 650a 2020 2020 2020 2020 2020  :type.          
+00000e40: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
+00000e50: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
+00000e60: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
+00000e70: 496d 6167 6522 202f 3e0a 2020 2020 2020  Image" />.      
+00000e80: 2020 3c64 633a 7469 746c 653e 3c2f 6463    <dc:title></dc
+00000e90: 3a74 6974 6c65 3e0a 2020 2020 2020 3c2f  :title>.      </
+00000ea0: 6363 3a57 6f72 6b3e 0a20 2020 203c 2f72  cc:Work>.    </r
+00000eb0: 6466 3a52 4446 3e0a 2020 3c2f 6d65 7461  df:RDF>.  </meta
+00000ec0: 6461 7461 3e0a 2020 3c67 0a20 2020 2020  data>.  <g.     
+00000ed0: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
+00000ee0: 4c61 7965 7220 3122 0a20 2020 2020 696e  Layer 1".     in
+00000ef0: 6b73 6361 7065 3a67 726f 7570 6d6f 6465  kscape:groupmode
+00000f00: 3d22 6c61 7965 7222 0a20 2020 2020 6964  ="layer".     id
+00000f10: 3d22 6c61 7965 7231 223e 0a20 2020 203c  ="layer1">.    <
+00000f20: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+00000f30: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
+00000f40: 6f6b 653a 2330 3033 3338 303b 7374 726f  oke:#003380;stro
+00000f50: 6b65 2d77 6964 7468 3a31 3b73 7472 6f6b  ke-width:1;strok
+00000f60: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00000f70: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00000f80: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00000f90: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00000fa0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00000fb0: 2020 643d 226d 2031 312e 3231 3537 3036    d="m 11.215706
+00000fc0: 2c31 2e39 3132 3030 3631 2030 2e37 3334  ,1.9120061 0.734
+00000fd0: 3435 372c 302e 3331 3731 3331 3520 6320  457,0.3171315 c 
+00000fe0: 302e 3831 3337 3738 2c30 2e33 3531 3338  0.813778,0.35138
+00000ff0: 3232 2031 2e39 3939 3034 322c 312e 3338  22 1.999042,1.38
+00001000: 3833 3330 3120 312e 3439 3731 3938 2c32  83301 1.497198,2
+00001010: 2e31 3835 3238 3731 204c 2031 312e 3834  .1852871 L 11.84
+00001020: 3131 3633 2c36 2e39 3635 3136 3131 2043  1163,6.9651611 C
+00001030: 2031 312e 3333 3933 3139 2c37 2e37 3632   11.339319,7.762
+00001040: 3131 3833 2031 302e 3933 3638 3238 2c38  1183 10.936828,8
+00001050: 2e33 3237 3032 3836 2039 2e35 3731 3637  .3270286 9.57167
+00001060: 3238 2c37 2e37 3337 3536 3638 204c 2038  28,7.7375668 L 8
+00001070: 2e38 3337 3231 3636 2c37 2e34 3230 3433  .8372166,7.42043
+00001080: 3533 2043 2037 2e34 3134 3833 3635 2c36  53 C 7.4148365,6
+00001090: 2e38 3036 3236 3435 2037 2e37 3036 3234  .8062645 7.70624
+000010a0: 3035 2c36 2e31 3030 3032 3739 2038 2e30  05,6.1000279 8.0
+000010b0: 3031 3336 3534 2c35 2e32 3035 3636 3234  013654,5.2056624
+000010c0: 204c 2038 2e39 3337 3531 3732 2c32 2e33   L 8.9375172,2.3
+000010d0: 3638 3638 3733 2043 2039 2e32 3332 3634  686873 C 9.23264
+000010e0: 3139 2c31 2e34 3734 3332 3234 2031 302e  19,1.4743224 10.
+000010f0: 3430 3139 3238 2c31 2e35 3630 3632 3337  401928,1.5606237
+00001100: 2031 312e 3231 3537 3036 2c31 2e39 3132   11.215706,1.912
+00001110: 3030 3631 205a 220a 2020 2020 2020 2069  0061 Z".       i
+00001120: 643d 2272 6563 7432 3035 220a 2020 2020  d="rect205".    
+00001130: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00001140: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00001150: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
+00001160: 6f64 693a 6e6f 6465 7479 7065 733d 2273  odi:nodetypes="s
+00001170: 7373 7373 7373 7373 2220 2f3e 0a20 2020  ssssssss" />.   
+00001180: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+00001190: 796c 653d 2266 696c 6c3a 2330 3033 3338  yle="fill:#00338
+000011a0: 303b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  0;fill-rule:nonz
+000011b0: 6572 6f3b 7374 726f 6b65 3a6e 6f6e 653b  ero;stroke:none;
+000011c0: 7374 726f 6b65 2d77 6964 7468 3a31 7078  stroke-width:1px
+000011d0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+000011e0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+000011f0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00001200: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00001210: 2020 2020 643d 224d 2036 2e39 3836 3532      d="M 6.98652
+00001220: 3735 2c37 2e39 3436 3232 3639 2043 2036  75,7.9462269 C 6
+00001230: 2e37 3537 3638 3937 2c38 2e32 3831 3835  .7576897,8.28185
+00001240: 3535 2036 2e32 3835 3034 3339 2c38 2e34  55 6.2850439,8.4
+00001250: 3739 3537 3737 2035 2e38 3136 3234 3032  795777 5.8162402
+00001260: 2c38 2e37 3035 3433 3435 2035 2e35 3831  ,8.7054345 5.581
+00001270: 3833 3834 2c38 2e38 3138 3336 3239 2035  8384,8.8183629 5
+00001280: 2e33 3336 3736 392c 382e 3933 3035 3437  .336769,8.930547
+00001290: 3820 352e 3134 3732 3337 332c 392e 3139  8 5.1472373,9.19
+000012a0: 3330 3234 3320 342e 3935 3737 3035 352c  30243 4.9577055,
+000012b0: 392e 3435 3535 3030 3920 342e 3935 3230  9.4555009 4.9520
+000012c0: 3130 372c 392e 3837 3432 3537 3520 352e  107,9.8742575 5.
+000012d0: 3131 3635 3632 372c 3130 2e31 3939 3233  1165627,10.19923
+000012e0: 3320 6120 312e 3032 3436 3030 382c 312e  3 a 1.0246008,1.
+000012f0: 3032 3436 3030 3820 3020 3020 3020 302e  0246008 0 0 0 0.
+00001300: 3030 3637 372c 302e 3031 3331 3420 312e  00677,0.01314 1.
+00001310: 3834 3730 3732 322c 312e 3834 3730 3732  8470722,1.847072
+00001320: 3220 3020 3020 3120 302e 3030 3439 382c  2 0 0 1 0.00498,
+00001330: 302e 3030 3836 2063 2030 2e31 3636 3530  0.0086 c 0.16650
+00001340: 3433 2c30 2e32 3838 3339 3420 302e 3038  43,0.288394 0.08
+00001350: 3336 3034 2c30 2e33 3234 3932 202d 302e  3604,0.32492 -0.
+00001360: 3134 3639 3532 322c 302e 3436 3330 3031  1469522,0.463001
+00001370: 202d 302e 3233 3035 3536 322c 302e 3133   -0.2305562,0.13
+00001380: 3830 3831 202d 302e 3632 3630 3531 312c  8081 -0.6260511,
+00001390: 302e 3135 3332 3231 202d 302e 3737 3838  0.153221 -0.7788
+000013a0: 3930 322c 302e 3036 3439 3820 302c 3020  902,0.06498 0,0 
+000013b0: 2d33 2e36 3165 2d35 2c2d 322e 3165 2d35  -3.61e-5,-2.1e-5
+000013c0: 202d 332e 3631 652d 352c 2d32 2e31 652d   -3.61e-5,-2.1e-
+000013d0: 3520 2d30 2e33 3630 3732 3039 2c2d 302e  5 -0.3607209,-0.
+000013e0: 3136 3935 3037 202d 302e 3731 3331 3535  169507 -0.713155
+000013f0: 2c2d 302e 3130 3136 3331 202d 302e 3936  ,-0.101631 -0.96
+00001400: 3231 3438 312c 302e 3130 3331 3331 202d  21481,0.103131 -
+00001410: 302e 3235 3832 3139 332c 302e 3234 3134  0.2582193,0.2414
+00001420: 3136 202d 302e 3430 3037 3839 322c 302e  16 -0.4007892,0.
+00001430: 3530 3135 3437 202d 302e 3438 3538 3830  501547 -0.485880
+00001440: 312c 302e 3636 3030 3235 202d 302e 3536  1,0.660025 -0.56
+00001450: 3239 3336 392c 302e 3933 3230 3439 202d  29369,0.932049 -
+00001460: 302e 3831 3034 3332 392c 312e 3235 3634  0.8104329,1.2564
+00001470: 3535 202d 302e 3932 3431 3233 352c 312e  55 -0.9241235,1.
+00001480: 3434 3535 3836 202d 302e 3131 3533 3232  445586 -0.115322
+00001490: 352c 302e 3139 3138 3436 202d 302e 3033  5,0.191846 -0.03
+000014a0: 3339 3331 2c30 2e32 3332 3331 3620 2d30  3931,0.232316 -0
+000014b0: 2e30 3333 3933 312c 302e 3233 3233 3136  .033931,0.232316
+000014c0: 2030 2c30 202d 302e 3030 3938 382c 302e   0,0 -0.00988,0.
+000014d0: 3131 3639 3733 2030 2e32 3333 3534 3436  116973 0.2335446
+000014e0: 2c30 2e30 3636 3538 2030 2e32 3431 3934  ,0.06658 0.24194
+000014f0: 3739 2c2d 302e 3035 3030 3920 302e 3738  79,-0.05009 0.78
+00001500: 3739 3636 392c 2d30 2e32 3937 3835 3220  79669,-0.297852 
+00001510: 312e 3434 3830 3331 2c2d 312e 3238 3336  1.448031,-1.2836
+00001520: 3736 2030 2e31 3233 3031 3136 2c2d 302e  76 0.1230116,-0.
+00001530: 3136 3739 3431 2030 2e32 3431 3432 3737  167941 0.2414277
+00001540: 2c2d 302e 3337 3137 3338 2030 2e33 3435  ,-0.371738 0.345
+00001550: 3536 3937 2c2d 302e 3434 3336 3732 202d  5697,-0.443672 -
+00001560: 302e 3031 3930 3233 2c30 2e30 3036 3620  0.019023,0.0066 
+00001570: 2d30 2e30 3037 3138 2c2d 302e 3030 3236  -0.00718,-0.0026
+00001580: 202d 302e 3037 3130 3331 2c2d 382e 3532   -0.071031,-8.52
+00001590: 652d 3420 302c 3020 342e 3665 2d36 2c32  e-4 0,0 4.6e-6,2
+000015a0: 652d 3620 342e 3765 2d36 2c32 652d 3620  e-6 4.7e-6,2e-6 
+000015b0: 302e 3534 3534 3932 342c 302e 3331 3439  0.5454924,0.3149
+000015c0: 3431 2031 2e31 3930 3837 3532 2c30 2e32  41 1.1908752,0.2
+000015d0: 3237 3432 3920 312e 3639 3133 3133 342c  27429 1.6913134,
+000015e0: 2d30 2e30 3732 3239 2043 2035 2e39 3431  -0.07229 C 5.941
+000015f0: 3332 3532 2c31 312e 3135 3830 3932 2036  3252,11.158092 6
+00001600: 2e32 3738 3531 2c31 302e 3432 3834 3639  .27851,10.428469
+00001610: 2035 2e39 3134 3138 3739 2c39 2e37 3832   5.9141879,9.782
+00001620: 3234 3831 2035 2e38 3437 3830 3436 2c39  2481 5.8478046,9
+00001630: 2e36 3532 3836 3736 2035 2e38 3639 3634  .6528676 5.86964
+00001640: 3532 2c39 2e37 3239 3934 3135 2035 2e38  52,9.7299415 5.8
+00001650: 3736 3839 3433 2c39 2e37 3139 3930 3235  768943,9.7199025
+00001660: 2035 2e38 3834 3333 3031 2c39 2e37 3039   5.8843301,9.709
+00001670: 3630 3439 2036 2e30 3034 3731 3231 2c39  6049 6.0047121,9
+00001680: 2e36 3133 3633 3539 2036 2e32 3036 3836  .6136359 6.20686
+00001690: 3539 2c39 2e35 3136 3234 3337 2036 2e36  59,9.5162437 6.6
+000016a0: 3131 3137 3337 2c39 2e33 3231 3435 3932  111737,9.3214592
+000016b0: 2037 2e32 3936 3035 372c 392e 3038 3938   7.296057,9.0898
+000016c0: 3733 3220 372e 3733 3031 3331 392c 382e  732 7.7301319,8.
+000016d0: 3435 3332 3330 3320 5a22 0a20 2020 2020  4532303 Z".     
+000016e0: 2020 6964 3d22 7061 7468 3439 3335 220a    id="path4935".
+000016f0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00001700: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00001710: 7572 653d 2230 220a 2020 2020 2020 2073  ure="0".       s
+00001720: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00001730: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
+00001740: 696e 6b73 6361 7065 3a70 6174 682d 6566  inkscape:path-ef
+00001750: 6665 6374 3d22 2370 6174 682d 6566 6665  fect="#path-effe
+00001760: 6374 3533 3831 220a 2020 2020 2020 2069  ct5381".       i
+00001770: 6e6b 7363 6170 653a 6f72 6967 696e 616c  nkscape:original
+00001780: 2d64 3d22 4d20 372e 3335 3833 3239 392c  -d="M 7.3583299,
+00001790: 382e 3139 3937 3238 3320 4320 362e 3639  8.1997283 C 6.69
+000017a0: 3534 3137 332c 392e 3137 3230 3030 3120  54173,9.1720001 
+000017b0: 352e 3034 3332 3731 342c 392e 3035 3833  5.0432714,9.0583
+000017c0: 3434 3920 352e 3531 3830 3239 362c 392e  449 5.5180296,9.
+000017d0: 3939 3539 3438 3720 362e 3035 3932 3331  9959487 6.059231
+000017e0: 2c31 302e 3933 3333 3337 2034 2e36 3735  ,10.933337 4.675
+000017f0: 3830 3733 2c31 312e 3534 3138 3233 2033  8073,11.541823 3
+00001800: 2e39 3737 3437 3537 2c31 312e 3133 3836  .9774757,11.1386
+00001810: 3431 2033 2e32 3938 3536 3431 2c31 302e  41 3.2985641,10.
+00001820: 3734 3636 3731 2033 2e30 3838 3830 3535  746671 3.0888055
+00001830: 2c31 322e 3435 3537 3733 2031 2e37 3839  ,12.455773 1.789
+00001840: 3836 342c 3133 2e31 3933 3637 220a 2020  864,13.19367".  
+00001850: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+00001860: 7472 616e 736c 6174 6528 302e 3431 3230  translate(0.4120
+00001870: 3731 3631 2c2d 312e 3435 3732 3431 3529  7161,-1.4572415)
+00001880: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+00001890: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+000018a0: 6c3a 2330 3033 3338 303b 6669 6c6c 2d72  l:#003380;fill-r
+000018b0: 756c 653a 6e6f 6e7a 6572 6f3b 7374 726f  ule:nonzero;stro
+000018c0: 6b65 3a6e 6f6e 653b 7374 726f 6b65 2d77  ke:none;stroke-w
+000018d0: 6964 7468 3a31 7078 3b73 7472 6f6b 652d  idth:1px;stroke-
+000018e0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+000018f0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00001900: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
+00001910: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+00001920: 2037 2e37 3235 3932 3231 2c38 2e30 3334   7.7259221,8.034
+00001930: 3030 3035 2063 2030 2c30 2e36 3732 3932  0005 c 0,0.67292
+00001940: 3239 2030 2e30 3738 3238 352c 312e 3331  29 0.078285,1.31
+00001950: 3230 3436 3620 302e 3032 3935 3237 2c31  20466 0.029527,1
+00001960: 2e36 3833 3530 3834 202d 302e 3034 3837  .6835084 -0.0487
+00001970: 3538 2c30 2e33 3731 3436 3231 2030 2e30  58,0.3714621 0.0
+00001980: 3131 3630 332c 302e 3430 3432 3039 3120  11603,0.4042091 
+00001990: 2d30 2e34 3333 3137 3437 2c30 2e34 3034  -0.4331747,0.404
+000019a0: 3230 3931 202d 302e 3530 3935 3139 312c  2091 -0.5095191,
+000019b0: 3020 2d30 2e39 3330 3031 3937 2c30 2e31  0 -0.9300197,0.1
+000019c0: 3331 3034 3920 2d31 2e32 3037 3039 3432  31049 -1.2070942
+000019d0: 2c30 2e34 3139 3231 3320 2d30 2e32 3737  ,0.419213 -0.277
+000019e0: 3037 3435 2c30 2e32 3838 3136 3420 2d30  0745,0.288164 -0
+000019f0: 2e33 3530 3239 3437 2c30 2e36 3737 3734  .3502947,0.67774
+00001a00: 3520 2d30 2e33 3235 3438 3738 2c31 2e30  5 -0.3254878,1.0
+00001a10: 3231 3135 3520 302e 3034 3938 372c 302e  21155 0.04987,0.
+00001a20: 3537 3037 3132 2030 2e32 3830 3635 3034  570712 0.2806504
+00001a30: 2c31 2e30 3338 3438 3320 302e 3438 3438  ,1.038483 0.4848
+00001a40: 3137 352c 312e 3336 3332 3536 2030 2e31  175,1.363256 0.1
+00001a50: 3536 3533 3338 2c30 2e32 3535 3130 3520  565338,0.255105 
+00001a60: 302e 3132 3234 3734 392c 302e 3530 3131  0.1224749,0.5011
+00001a70: 3839 202d 302e 3030 3739 322c 302e 3535  89 -0.00792,0.55
+00001a80: 3939 3231 202d 302e 3633 3938 3836 2c30  9921 -0.639886,0
+00001a90: 2e35 3832 3837 3520 2d31 2e31 3430 3037  .582875 -1.14007
+00001aa0: 3931 2c30 2e37 3933 3231 3220 2d31 2e32  91,0.793212 -1.2
+00001ab0: 3732 3636 3134 2c30 2e39 3537 3137 3220  726614,0.957172 
+00001ac0: 2d30 2e31 3332 3033 3537 2c30 2e31 3633  -0.1320357,0.163
+00001ad0: 3238 3420 2d30 2e30 3430 3630 342c 302e  284 -0.040604,0.
+00001ae0: 3139 3138 3636 202d 302e 3034 3036 3034  191866 -0.040604
+00001af0: 2c30 2e31 3931 3836 3620 302c 3020 2d30  ,0.191866 0,0 -0
+00001b00: 2e30 3231 3334 352c 302e 3038 3437 3120  .021345,0.08471 
+00001b10: 302e 3138 3035 3237 332c 302e 3037 3035  0.1805273,0.0705
+00001b20: 3820 2d30 2e30 3134 3335 372c 302e 3030  8 -0.014357,0.00
+00001b30: 3120 302e 3833 3831 3036 392c 2d30 2e30  1 0.8381069,-0.0
+00001b40: 3839 3720 312e 3630 3533 3832 352c 2d30  897 1.6053825,-0
+00001b50: 2e36 3031 3036 3320 302e 3338 3933 3436  .601063 0.389346
+00001b60: 312c 2d30 2e33 3430 3037 3720 302e 3632  1,-0.340077 0.62
+00001b70: 3634 3538 312c 2d30 2e39 3732 3632 3920  64581,-0.972629 
+00001b80: 302e 3239 3739 3733 322c 2d31 2e36 3036  0.2979732,-1.606
+00001b90: 3234 3120 2d30 2e31 3532 3037 3737 2c2d  241 -0.1520777,-
+00001ba0: 302e 3239 3139 3538 202d 302e 3333 3337  0.291958 -0.3337
+00001bb0: 3930 322c 2d30 2e36 3630 3932 3220 2d30  902,-0.660922 -0
+00001bc0: 2e33 3439 3834 3935 2c2d 312e 3030 3033  .3498495,-1.0003
+00001bd0: 3339 202d 302e 3031 3333 3038 2c2d 302e  39 -0.013308,-0.
+00001be0: 3138 3432 3239 2030 2e30 3139 3935 322c  184229 0.019952,
+00001bf0: 2d30 2e32 3733 3632 3120 302e 3037 3635  -0.273621 0.0765
+00001c00: 3834 2c2d 302e 3333 3235 3220 302e 3035  84,-0.33252 0.05
+00001c10: 3636 3332 2c2d 302e 3035 3839 2030 2e31  6632,-0.0589 0.1
+00001c20: 3937 3036 3439 2c2d 302e 3134 3330 3033  970649,-0.143003
+00001c30: 2030 2e35 3538 3333 3732 2c2d 302e 3134   0.5583372,-0.14
+00001c40: 3330 3033 2030 2e37 3631 3935 3136 2c30  3003 0.7619516,0
+00001c50: 2031 2e32 3439 3133 3638 2c2d 302e 3630   1.2491368,-0.60
+00001c60: 3531 3539 2031 2e33 3235 3532 3032 2c2d  5159 1.3255202,-
+00001c70: 312e 3138 3730 3738 3920 302e 3037 3633  1.1870789 0.0763
+00001c80: 3834 2c2d 302e 3538 3139 3230 3420 2d30  84,-0.5819204 -0
+00001c90: 2e30 3231 3837 322c 2d31 2e32 3131 3635  .021872,-1.21165
+00001ca0: 3535 202d 302e 3032 3138 3732 2c2d 312e  55 -0.021872,-1.
+00001cb0: 3830 3036 3338 3620 7a22 0a20 2020 2020  8006386 z".     
+00001cc0: 2020 6964 3d22 7061 7468 3439 3335 2d36    id="path4935-6
+00001cd0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00001ce0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00001cf0: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+00001d00: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+00001d10: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
+00001d20: 2020 696e 6b73 6361 7065 3a70 6174 682d    inkscape:path-
+00001d30: 6566 6665 6374 3d22 2370 6174 682d 6566  effect="#path-ef
+00001d40: 6665 6374 3533 3831 2d33 220a 2020 2020  fect5381-3".    
+00001d50: 2020 2069 6e6b 7363 6170 653a 6f72 6967     inkscape:orig
+00001d60: 696e 616c 2d64 3d22 6d20 382e 3137 3539  inal-d="m 8.1759
+00001d70: 3232 312c 382e 3033 3430 3030 3120 6320  221,8.0340001 c 
+00001d80: 302c 312e 3236 3139 3036 3220 302e 3335  0,1.2619062 0.35
+00001d90: 3330 3830 382c 322e 3533 3737 3137 3920  30808,2.5377179 
+00001da0: 2d30 2e38 3533 3634 3832 2c32 2e35 3337  -0.8536482,2.537
+00001db0: 3731 3739 202d 312e 3530 3635 3834 2c30  7179 -1.506584,0
+00001dc0: 202d 312e 3135 3831 3336 382c 312e 3238   -1.1581368,1.28
+00001dd0: 3830 3631 202d 302e 3636 3634 3138 2c32  8061 -0.666418,2
+00001de0: 2e31 3339 3734 3320 302e 3537 3439 3331  .139743 0.574931
+00001df0: 352c 312e 3035 3537 3033 202d 302e 3431  5,1.055703 -0.41
+00001e00: 3233 3630 382c 312e 3138 3939 3120 2d31  23608,1.18991 -1
+00001e10: 2e37 3131 3330 3233 2c31 2e39 3237 3830  .7113023,1.92780
+00001e20: 3722 0a20 2020 2020 2020 7472 616e 7366  7".       transf
+00001e30: 6f72 6d3d 2274 7261 6e73 6c61 7465 2832  orm="translate(2
+00001e40: 2e35 3634 3531 3735 2c2d 302e 3436 3035  .5645175,-0.4605
+00001e50: 3337 3334 2922 202f 3e0a 2020 2020 3c70  3734)" />.    <p
+00001e60: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00001e70: 3d22 6669 6c6c 3a23 3030 3333 3830 3b66  ="fill:#003380;f
+00001e80: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
+00001e90: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
+00001ea0: 6f6b 652d 7769 6474 683a 3170 783b 7374  oke-width:1px;st
+00001eb0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00001ec0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00001ed0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+00001ee0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00001ef0: 2064 3d22 6d20 372e 3732 3539 3232 312c   d="m 7.7259221,
+00001f00: 382e 3033 3430 3030 3520 6320 302c 302e  8.0340005 c 0,0.
+00001f10: 3637 3239 3232 3920 302e 3037 3832 3835  6729229 0.078285
+00001f20: 2c31 2e33 3132 3034 3636 2030 2e30 3239  ,1.3120466 0.029
+00001f30: 3532 372c 312e 3638 3335 3038 3420 2d30  527,1.6835084 -0
+00001f40: 2e30 3438 3735 382c 302e 3337 3134 3632  .048758,0.371462
+00001f50: 3120 302e 3031 3136 3033 2c30 2e34 3034  1 0.011603,0.404
+00001f60: 3230 3931 202d 302e 3433 3331 3734 372c  2091 -0.4331747,
+00001f70: 302e 3430 3432 3039 3120 2d30 2e35 3039  0.4042091 -0.509
+00001f80: 3531 3931 2c30 202d 302e 3933 3030 3139  5191,0 -0.930019
+00001f90: 372c 302e 3133 3130 3439 202d 312e 3230  7,0.131049 -1.20
+00001fa0: 3730 3934 322c 302e 3431 3932 3133 202d  70942,0.419213 -
+00001fb0: 302e 3237 3730 3734 352c 302e 3238 3831  0.2770745,0.2881
+00001fc0: 3634 202d 302e 3335 3032 3934 372c 302e  64 -0.3502947,0.
+00001fd0: 3637 3737 3435 202d 302e 3332 3534 3837  677745 -0.325487
+00001fe0: 382c 312e 3032 3131 3535 2030 2e30 3439  8,1.021155 0.049
+00001ff0: 3837 2c30 2e35 3730 3731 3220 302e 3238  87,0.570712 0.28
+00002000: 3036 3530 342c 312e 3033 3834 3833 2030  06504,1.038483 0
+00002010: 2e34 3834 3831 3735 2c31 2e33 3633 3235  .4848175,1.36325
+00002020: 3620 302e 3135 3635 3333 382c 302e 3235  6 0.1565338,0.25
+00002030: 3531 3035 2030 2e31 3232 3437 3439 2c30  5105 0.1224749,0
+00002040: 2e35 3031 3138 3920 2d30 2e30 3037 3932  .501189 -0.00792
+00002050: 2c30 2e35 3539 3932 3120 2d30 2e36 3339  ,0.559921 -0.639
+00002060: 3838 362c 302e 3538 3238 3735 202d 312e  886,0.582875 -1.
+00002070: 3134 3030 3739 312c 302e 3739 3332 3132  1400791,0.793212
+00002080: 202d 312e 3237 3236 3631 342c 302e 3935   -1.2726614,0.95
+00002090: 3731 3732 202d 302e 3133 3230 3335 372c  7172 -0.1320357,
+000020a0: 302e 3136 3332 3834 202d 302e 3034 3036  0.163284 -0.0406
+000020b0: 3034 2c30 2e31 3931 3836 3620 2d30 2e30  04,0.191866 -0.0
+000020c0: 3430 3630 342c 302e 3139 3138 3636 2030  40604,0.191866 0
+000020d0: 2c30 202d 302e 3032 3133 3435 2c30 2e30  ,0 -0.021345,0.0
+000020e0: 3834 3731 2030 2e31 3830 3532 3733 2c30  8471 0.1805273,0
+000020f0: 2e30 3730 3538 202d 302e 3031 3433 3537  .07058 -0.014357
+00002100: 2c30 2e30 3031 2030 2e38 3338 3130 3639  ,0.001 0.8381069
+00002110: 2c2d 302e 3038 3937 2031 2e36 3035 3338  ,-0.0897 1.60538
+00002120: 3235 2c2d 302e 3630 3130 3633 2030 2e33  25,-0.601063 0.3
+00002130: 3839 3334 3631 2c2d 302e 3334 3030 3737  893461,-0.340077
+00002140: 2030 2e36 3236 3435 3831 2c2d 302e 3937   0.6264581,-0.97
+00002150: 3236 3239 2030 2e32 3937 3937 3332 2c2d  2629 0.2979732,-
+00002160: 312e 3630 3632 3431 202d 302e 3135 3230  1.606241 -0.1520
+00002170: 3737 372c 2d30 2e32 3931 3935 3820 2d30  777,-0.291958 -0
+00002180: 2e33 3333 3739 3032 2c2d 302e 3636 3039  .3337902,-0.6609
+00002190: 3232 202d 302e 3334 3938 3439 352c 2d31  22 -0.3498495,-1
+000021a0: 2e30 3030 3333 3920 2d30 2e30 3133 3330  .000339 -0.01330
+000021b0: 382c 2d30 2e31 3834 3232 3920 302e 3031  8,-0.184229 0.01
+000021c0: 3939 3532 2c2d 302e 3237 3336 3231 2030  9952,-0.273621 0
+000021d0: 2e30 3736 3538 342c 2d30 2e33 3332 3532  .076584,-0.33252
+000021e0: 2030 2e30 3536 3633 322c 2d30 2e30 3538   0.056632,-0.058
+000021f0: 3920 302e 3139 3730 3634 392c 2d30 2e31  9 0.1970649,-0.1
+00002200: 3433 3030 3320 302e 3535 3833 3337 322c  43003 0.5583372,
+00002210: 2d30 2e31 3433 3030 3320 302e 3736 3139  -0.143003 0.7619
+00002220: 3531 362c 3020 312e 3234 3931 3336 382c  516,0 1.2491368,
+00002230: 2d30 2e36 3035 3135 3920 312e 3332 3535  -0.605159 1.3255
+00002240: 3230 322c 2d31 2e31 3837 3037 3839 2030  202,-1.1870789 0
+00002250: 2e30 3736 3338 342c 2d30 2e35 3831 3932  .076384,-0.58192
+00002260: 3034 202d 302e 3032 3138 3732 2c2d 312e  04 -0.021872,-1.
+00002270: 3231 3136 3535 3520 2d30 2e30 3231 3837  2116555 -0.02187
+00002280: 322c 2d31 2e38 3030 3633 3836 207a 220a  2,-1.8006386 z".
+00002290: 2020 2020 2020 2069 643d 2270 6174 6834         id="path4
+000022a0: 3933 352d 362d 3322 0a20 2020 2020 2020  935-6-3".       
+000022b0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+000022c0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+000022d0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+000022e0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+000022f0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00002300: 653a 7061 7468 2d65 6666 6563 743d 2223  e:path-effect="#
+00002310: 7061 7468 2d65 6666 6563 7435 3338 312d  path-effect5381-
+00002320: 332d 3922 0a20 2020 2020 2020 696e 6b73  3-9".       inks
+00002330: 6361 7065 3a6f 7269 6769 6e61 6c2d 643d  cape:original-d=
+00002340: 226d 2038 2e31 3735 3932 3231 2c38 2e30  "m 8.1759221,8.0
+00002350: 3334 3030 3031 2063 2030 2c31 2e32 3631  340001 c 0,1.261
+00002360: 3930 3632 2030 2e33 3533 3038 3038 2c32  9062 0.3530808,2
+00002370: 2e35 3337 3731 3739 202d 302e 3835 3336  .5377179 -0.8536
+00002380: 3438 322c 322e 3533 3737 3137 3920 2d31  482,2.5377179 -1
+00002390: 2e35 3036 3538 342c 3020 2d31 2e31 3538  .506584,0 -1.158
+000023a0: 3133 3638 2c31 2e32 3838 3036 3120 2d30  1368,1.288061 -0
+000023b0: 2e36 3636 3431 382c 322e 3133 3937 3433  .666418,2.139743
+000023c0: 2030 2e35 3734 3933 3135 2c31 2e30 3535   0.5749315,1.055
+000023d0: 3730 3320 2d30 2e34 3132 3336 3038 2c31  703 -0.4123608,1
+000023e0: 2e31 3839 3931 202d 312e 3731 3133 3032  .18991 -1.711302
+000023f0: 332c 312e 3932 3738 3037 220a 2020 2020  3,1.927807".    
+00002400: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
+00002410: 7472 6978 2830 2e37 3435 3334 3339 312c  trix(0.74534391,
+00002420: 2d30 2e31 3030 3734 3037 2c30 2e31 3030  -0.1007407,0.100
+00002430: 3734 3037 2c30 2e37 3435 3334 3339 312c  7407,0.74534391,
+00002440: 312e 3136 3936 3031 392c 312e 3538 3034  1.1696019,1.5804
+00002450: 3434 3629 2220 2f3e 0a20 2020 203c 7061  446)" />.    <pa
+00002460: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+00002470: 2266 696c 6c3a 2330 3033 3338 303b 6669  "fill:#003380;fi
+00002480: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00002490: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
+000024a0: 6b65 2d77 6964 7468 3a31 7078 3b73 7472  ke-width:1px;str
+000024b0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+000024c0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+000024d0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+000024e0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+000024f0: 643d 224d 2036 2e39 3836 3532 3735 2c37  d="M 6.9865275,7
+00002500: 2e39 3436 3232 3639 2043 2036 2e37 3537  .9462269 C 6.757
+00002510: 3638 3937 2c38 2e32 3831 3835 3535 2036  6897,8.2818555 6
+00002520: 2e32 3835 3034 3339 2c38 2e34 3739 3537  .2850439,8.47957
+00002530: 3737 2035 2e38 3136 3234 3032 2c38 2e37  77 5.8162402,8.7
+00002540: 3035 3433 3435 2035 2e35 3831 3833 3834  054345 5.5818384
+00002550: 2c38 2e38 3138 3336 3239 2035 2e33 3336  ,8.8183629 5.336
+00002560: 3736 392c 382e 3933 3035 3437 3820 352e  769,8.9305478 5.
+00002570: 3134 3732 3337 332c 392e 3139 3330 3234  1472373,9.193024
+00002580: 3320 342e 3935 3737 3035 352c 392e 3435  3 4.9577055,9.45
+00002590: 3535 3030 3920 342e 3935 3230 3130 372c  55009 4.9520107,
+000025a0: 392e 3837 3432 3537 3520 352e 3131 3635  9.8742575 5.1165
+000025b0: 3632 372c 3130 2e31 3939 3233 3320 6120  627,10.199233 a 
+000025c0: 312e 3032 3436 3030 382c 312e 3032 3436  1.0246008,1.0246
+000025d0: 3030 3820 3020 3020 3020 302e 3030 3637  008 0 0 0 0.0067
+000025e0: 372c 302e 3031 3331 3420 312e 3834 3730  7,0.01314 1.8470
+000025f0: 3732 322c 312e 3834 3730 3732 3220 3020  722,1.8470722 0 
+00002600: 3020 3120 302e 3030 3439 382c 302e 3030  0 1 0.00498,0.00
+00002610: 3836 2063 2030 2e31 3636 3530 3433 2c30  86 c 0.1665043,0
+00002620: 2e32 3838 3339 3420 302e 3038 3336 3034  .288394 0.083604
+00002630: 2c30 2e33 3234 3932 202d 302e 3134 3639  ,0.32492 -0.1469
+00002640: 3532 322c 302e 3436 3330 3031 202d 302e  522,0.463001 -0.
+00002650: 3233 3035 3536 322c 302e 3133 3830 3831  2305562,0.138081
+00002660: 202d 302e 3632 3630 3531 312c 302e 3135   -0.6260511,0.15
+00002670: 3332 3231 202d 302e 3737 3838 3930 322c  3221 -0.7788902,
+00002680: 302e 3036 3439 3820 302c 3020 2d33 2e36  0.06498 0,0 -3.6
+00002690: 3165 2d35 2c2d 322e 3165 2d35 202d 332e  1e-5,-2.1e-5 -3.
+000026a0: 3631 652d 352c 2d32 2e31 652d 3520 2d30  61e-5,-2.1e-5 -0
+000026b0: 2e33 3630 3732 3039 2c2d 302e 3136 3935  .3607209,-0.1695
+000026c0: 3037 202d 302e 3731 3331 3535 2c2d 302e  07 -0.713155,-0.
+000026d0: 3130 3136 3331 202d 302e 3936 3231 3438  101631 -0.962148
+000026e0: 312c 302e 3130 3331 3331 202d 302e 3235  1,0.103131 -0.25
+000026f0: 3832 3139 332c 302e 3234 3134 3136 202d  82193,0.241416 -
+00002700: 302e 3430 3037 3839 322c 302e 3530 3135  0.4007892,0.5015
+00002710: 3437 202d 302e 3438 3538 3830 312c 302e  47 -0.4858801,0.
+00002720: 3636 3030 3235 202d 302e 3536 3239 3336  660025 -0.562936
+00002730: 392c 302e 3933 3230 3439 202d 302e 3831  9,0.932049 -0.81
+00002740: 3034 3332 392c 312e 3235 3634 3535 202d  04329,1.256455 -
+00002750: 302e 3932 3431 3233 352c 312e 3434 3535  0.9241235,1.4455
+00002760: 3836 202d 302e 3131 3533 3232 352c 302e  86 -0.1153225,0.
+00002770: 3139 3138 3436 202d 302e 3033 3339 3331  191846 -0.033931
+00002780: 2c30 2e32 3332 3331 3620 2d30 2e30 3333  ,0.232316 -0.033
+00002790: 3933 312c 302e 3233 3233 3136 2030 2c30  931,0.232316 0,0
+000027a0: 202d 302e 3030 3938 382c 302e 3131 3639   -0.00988,0.1169
+000027b0: 3733 2030 2e32 3333 3534 3436 2c30 2e30  73 0.2335446,0.0
+000027c0: 3636 3538 2030 2e32 3431 3934 3739 2c2d  6658 0.2419479,-
+000027d0: 302e 3035 3030 3920 302e 3738 3739 3636  0.05009 0.787966
+000027e0: 392c 2d30 2e32 3937 3835 3220 312e 3434  9,-0.297852 1.44
+000027f0: 3830 3331 2c2d 312e 3238 3336 3736 2030  8031,-1.283676 0
+00002800: 2e31 3233 3031 3136 2c2d 302e 3136 3739  .1230116,-0.1679
+00002810: 3431 2030 2e32 3431 3432 3737 2c2d 302e  41 0.2414277,-0.
+00002820: 3337 3137 3338 2030 2e33 3435 3536 3937  371738 0.3455697
+00002830: 2c2d 302e 3434 3336 3732 202d 302e 3031  ,-0.443672 -0.01
+00002840: 3930 3233 2c30 2e30 3036 3620 2d30 2e30  9023,0.0066 -0.0
+00002850: 3037 3138 2c2d 302e 3030 3236 202d 302e  0718,-0.0026 -0.
+00002860: 3037 3130 3331 2c2d 382e 3532 652d 3420  071031,-8.52e-4 
+00002870: 302c 3020 342e 3665 2d36 2c32 652d 3620  0,0 4.6e-6,2e-6 
+00002880: 342e 3765 2d36 2c32 652d 3620 302e 3534  4.7e-6,2e-6 0.54
+00002890: 3534 3932 342c 302e 3331 3439 3431 2031  54924,0.314941 1
+000028a0: 2e31 3930 3837 3532 2c30 2e32 3237 3432  .1908752,0.22742
+000028b0: 3920 312e 3639 3133 3133 342c 2d30 2e30  9 1.6913134,-0.0
+000028c0: 3732 3239 2043 2035 2e39 3431 3332 3532  7229 C 5.9413252
+000028d0: 2c31 312e 3135 3830 3932 2036 2e32 3738  ,11.158092 6.278
+000028e0: 3531 2c31 302e 3432 3834 3639 2035 2e39  51,10.428469 5.9
+000028f0: 3134 3138 3739 2c39 2e37 3832 3234 3831  141879,9.7822481
+00002900: 2035 2e38 3437 3830 3436 2c39 2e36 3532   5.8478046,9.652
+00002910: 3836 3736 2035 2e38 3639 3634 3532 2c39  8676 5.8696452,9
+00002920: 2e37 3239 3934 3135 2035 2e38 3736 3839  .7299415 5.87689
+00002930: 3433 2c39 2e37 3139 3930 3235 2035 2e38  43,9.7199025 5.8
+00002940: 3834 3333 3031 2c39 2e37 3039 3630 3439  843301,9.7096049
+00002950: 2036 2e30 3034 3731 3231 2c39 2e36 3133   6.0047121,9.613
+00002960: 3633 3539 2036 2e32 3036 3836 3539 2c39  6359 6.2068659,9
+00002970: 2e35 3136 3234 3337 2036 2e36 3131 3137  .5162437 6.61117
+00002980: 3337 2c39 2e33 3231 3435 3932 2037 2e32  37,9.3214592 7.2
+00002990: 3936 3035 372c 392e 3038 3938 3733 3220  96057,9.0898732 
+000029a0: 372e 3733 3031 3331 392c 382e 3435 3332  7.7301319,8.4532
+000029b0: 3330 3320 5a22 0a20 2020 2020 2020 6964  303 Z".       id
+000029c0: 3d22 7061 7468 3439 3335 2d30 220a 2020  ="path4935-0".  
+000029d0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+000029e0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+000029f0: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
+00002a00: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+00002a10: 2263 6363 6322 0a20 2020 2020 2020 696e  "cccc".       in
+00002a20: 6b73 6361 7065 3a70 6174 682d 6566 6665  kscape:path-effe
+00002a30: 6374 3d22 2370 6174 682d 6566 6665 6374  ct="#path-effect
+00002a40: 3533 3831 2d36 220a 2020 2020 2020 2069  5381-6".       i
+00002a50: 6e6b 7363 6170 653a 6f72 6967 696e 616c  nkscape:original
+00002a60: 2d64 3d22 4d20 372e 3335 3833 3239 392c  -d="M 7.3583299,
+00002a70: 382e 3139 3937 3238 3320 4320 362e 3639  8.1997283 C 6.69
+00002a80: 3534 3137 332c 392e 3137 3230 3030 3120  54173,9.1720001 
+00002a90: 352e 3034 3332 3731 342c 392e 3035 3833  5.0432714,9.0583
+00002aa0: 3434 3920 352e 3531 3830 3239 362c 392e  449 5.5180296,9.
+00002ab0: 3939 3539 3438 3720 362e 3035 3932 3331  9959487 6.059231
+00002ac0: 2c31 302e 3933 3333 3337 2034 2e36 3735  ,10.933337 4.675
+00002ad0: 3830 3733 2c31 312e 3534 3138 3233 2033  8073,11.541823 3
+00002ae0: 2e39 3737 3437 3537 2c31 312e 3133 3836  .9774757,11.1386
+00002af0: 3431 2033 2e32 3938 3536 3431 2c31 302e  41 3.2985641,10.
+00002b00: 3734 3636 3731 2033 2e30 3838 3830 3535  746671 3.0888055
+00002b10: 2c31 322e 3435 3537 3733 2031 2e37 3839  ,12.455773 1.789
+00002b20: 3836 342c 3133 2e31 3933 3637 220a 2020  864,13.19367".  
+00002b30: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+00002b40: 6d61 7472 6978 282d 302e 3732 3834 3236  matrix(-0.728426
+00002b50: 3239 2c2d 302e 3438 3334 3038 3631 2c2d  29,-0.48340861,-
+00002b60: 302e 3438 3931 3232 3834 2c30 2e37 3139  0.48912284,0.719
+00002b70: 3931 3633 372c 3230 2e37 3933 3332 342c  91637,20.793324,
+00002b80: 352e 3533 3236 3739 3229 2220 2f3e 0a20  5.5326792)" />. 
+00002b90: 203c 2f67 3e0a 3c2f 7376 673e 0a          </g>.</svg>.
```

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/boxjelly_logo.svg` & `boxjelly-0.3.3/boxjelly/assets/icons/boxjelly_logo.svg`

 * *Files 23% similar despite different names*

```diff
@@ -1,741 +1,729 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0d0a 3c21 2d2d 2043 7265  "no"?>..<!-- Cre
-00000040: 6174 6564 2077 6974 6820 496e 6b73 6361  ated with Inksca
-00000050: 7065 2028 6874 7470 3a2f 2f77 7777 2e69  pe (http://www.i
-00000060: 6e6b 7363 6170 652e 6f72 672f 2920 2d2d  nkscape.org/) --
-00000070: 3e0d 0a0d 0a3c 7376 670d 0a20 2020 786d  >....<svg..   xm
-00000080: 6c6e 733a 6463 3d22 6874 7470 3a2f 2f70  lns:dc="http://p
-00000090: 7572 6c2e 6f72 672f 6463 2f65 6c65 6d65  url.org/dc/eleme
-000000a0: 6e74 732f 312e 312f 220d 0a20 2020 786d  nts/1.1/"..   xm
-000000b0: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
-000000c0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-000000d0: 7267 2f6e 7323 220d 0a20 2020 786d 6c6e  rg/ns#"..   xmln
-000000e0: 733a 7264 663d 2268 7474 703a 2f2f 7777  s:rdf="http://ww
-000000f0: 772e 7733 2e6f 7267 2f31 3939 392f 3032  w.w3.org/1999/02
-00000100: 2f32 322d 7264 662d 7379 6e74 6178 2d6e  /22-rdf-syntax-n
-00000110: 7323 220d 0a20 2020 786d 6c6e 733a 7376  s#"..   xmlns:sv
-00000120: 673d 2268 7474 703a 2f2f 7777 772e 7733  g="http://www.w3
-00000130: 2e6f 7267 2f32 3030 302f 7376 6722 0d0a  .org/2000/svg"..
-00000140: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
-00000150: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
-00000160: 2f73 7667 220d 0a20 2020 786d 6c6e 733a  /svg"..   xmlns:
-00000170: 736f 6469 706f 6469 3d22 6874 7470 3a2f  sodipodi="http:/
-00000180: 2f73 6f64 6970 6f64 692e 736f 7572 6365  /sodipodi.source
-00000190: 666f 7267 652e 6e65 742f 4454 442f 736f  forge.net/DTD/so
-000001a0: 6469 706f 6469 2d30 2e64 7464 220d 0a20  dipodi-0.dtd".. 
-000001b0: 2020 786d 6c6e 733a 696e 6b73 6361 7065    xmlns:inkscape
-000001c0: 3d22 6874 7470 3a2f 2f77 7777 2e69 6e6b  ="http://www.ink
-000001d0: 7363 6170 652e 6f72 672f 6e61 6d65 7370  scape.org/namesp
-000001e0: 6163 6573 2f69 6e6b 7363 6170 6522 0d0a  aces/inkscape"..
-000001f0: 2020 2077 6964 7468 3d22 3136 7078 220d     width="16px".
-00000200: 0a20 2020 6865 6967 6874 3d22 3136 7078  .   height="16px
-00000210: 220d 0a20 2020 7669 6577 426f 783d 2230  "..   viewBox="0
-00000220: 2030 2031 3620 3136 220d 0a20 2020 7665   0 16 16"..   ve
-00000230: 7273 696f 6e3d 2231 2e31 220d 0a20 2020  rsion="1.1"..   
-00000240: 6964 3d22 5356 4752 6f6f 7422 0d0a 2020  id="SVGRoot"..  
-00000250: 2069 6e6b 7363 6170 653a 7665 7273 696f   inkscape:versio
-00000260: 6e3d 2230 2e39 322e 3520 2832 3036 3065  n="0.92.5 (2060e
-00000270: 6331 6639 662c 2032 3032 302d 3034 2d30  c1f9f, 2020-04-0
-00000280: 3829 220d 0a20 2020 736f 6469 706f 6469  8)"..   sodipodi
-00000290: 3a64 6f63 6e61 6d65 3d22 626f 786a 656c  :docname="boxjel
-000002a0: 6c79 2e73 7667 220d 0a20 2020 696e 6b73  ly.svg"..   inks
-000002b0: 6361 7065 3a6c 6162 656c 3d22 4261 636b  cape:label="Back
-000002c0: 6772 6f75 6e64 223e 0d0a 2020 3c64 6566  ground">..  <def
-000002d0: 730d 0a20 2020 2020 6964 3d22 6465 6673  s..     id="defs
-000002e0: 3130 223e 0d0a 2020 2020 3c69 6e6b 7363  10">..    <inksc
-000002f0: 6170 653a 7061 7468 2d65 6666 6563 740d  ape:path-effect.
-00000300: 0a20 2020 2020 2020 6566 6665 6374 3d22  .       effect="
-00000310: 7461 7065 725f 7374 726f 6b65 220d 0a20  taper_stroke".. 
-00000320: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
-00000330: 6666 6563 7435 3338 3122 0d0a 2020 2020  ffect5381"..    
-00000340: 2020 2069 735f 7669 7369 626c 653d 2274     is_visible="t
-00000350: 7275 6522 0d0a 2020 2020 2020 2073 7472  rue"..       str
-00000360: 6f6b 655f 7769 6474 683d 2230 2e39 220d  oke_width="0.9".
-00000370: 0a20 2020 2020 2020 6174 7461 6368 5f73  .       attach_s
-00000380: 7461 7274 3d22 3165 2d30 3722 0d0a 2020  tart="1e-07"..  
-00000390: 2020 2020 2065 6e64 5f6f 6666 7365 743d       end_offset=
-000003a0: 2230 2e39 3939 3939 220d 0a20 2020 2020  "0.99999"..     
-000003b0: 2020 736d 6f6f 7468 696e 673d 2231 2e31    smoothing="1.1
-000003c0: 220d 0a20 2020 2020 2020 6a6f 696e 7479  "..       jointy
-000003d0: 7065 3d22 6578 7472 6170 6f6c 6174 6564  pe="extrapolated
-000003e0: 220d 0a20 2020 2020 2020 6d69 7465 725f  "..       miter_
-000003f0: 6c69 6d69 743d 2231 3030 2220 2f3e 0d0a  limit="100" />..
-00000400: 2020 2020 3c69 6e6b 7363 6170 653a 7061      <inkscape:pa
-00000410: 7468 2d65 6666 6563 740d 0a20 2020 2020  th-effect..     
-00000420: 2020 6566 6665 6374 3d22 7461 7065 725f    effect="taper_
-00000430: 7374 726f 6b65 220d 0a20 2020 2020 2020  stroke"..       
-00000440: 6964 3d22 7061 7468 2d65 6666 6563 7435  id="path-effect5
-00000450: 3338 312d 3322 0d0a 2020 2020 2020 2069  381-3"..       i
-00000460: 735f 7669 7369 626c 653d 2274 7275 6522  s_visible="true"
-00000470: 0d0a 2020 2020 2020 2073 7472 6f6b 655f  ..       stroke_
-00000480: 7769 6474 683d 2230 2e39 220d 0a20 2020  width="0.9"..   
-00000490: 2020 2020 6174 7461 6368 5f73 7461 7274      attach_start
-000004a0: 3d22 3165 2d30 3722 0d0a 2020 2020 2020  ="1e-07"..      
-000004b0: 2065 6e64 5f6f 6666 7365 743d 2231 2e34   end_offset="1.4
-000004c0: 3232 3030 3934 220d 0a20 2020 2020 2020  220094"..       
-000004d0: 736d 6f6f 7468 696e 673d 2231 2e31 220d  smoothing="1.1".
-000004e0: 0a20 2020 2020 2020 6a6f 696e 7479 7065  .       jointype
-000004f0: 3d22 6578 7472 6170 6f6c 6174 6564 220d  ="extrapolated".
-00000500: 0a20 2020 2020 2020 6d69 7465 725f 6c69  .       miter_li
-00000510: 6d69 743d 2231 3030 2220 2f3e 0d0a 2020  mit="100" />..  
-00000520: 2020 3c69 6e6b 7363 6170 653a 7061 7468    <inkscape:path
-00000530: 2d65 6666 6563 740d 0a20 2020 2020 2020  -effect..       
-00000540: 6566 6665 6374 3d22 7461 7065 725f 7374  effect="taper_st
-00000550: 726f 6b65 220d 0a20 2020 2020 2020 6964  roke"..       id
-00000560: 3d22 7061 7468 2d65 6666 6563 7435 3338  ="path-effect538
-00000570: 312d 332d 3722 0d0a 2020 2020 2020 2069  1-3-7"..       i
-00000580: 735f 7669 7369 626c 653d 2274 7275 6522  s_visible="true"
-00000590: 0d0a 2020 2020 2020 2073 7472 6f6b 655f  ..       stroke_
-000005a0: 7769 6474 683d 2231 220d 0a20 2020 2020  width="1"..     
-000005b0: 2020 6174 7461 6368 5f73 7461 7274 3d22    attach_start="
-000005c0: 3165 2d30 3722 0d0a 2020 2020 2020 2065  1e-07"..       e
-000005d0: 6e64 5f6f 6666 7365 743d 2231 2e34 3232  nd_offset="1.422
-000005e0: 3030 3934 220d 0a20 2020 2020 2020 736d  0094"..       sm
-000005f0: 6f6f 7468 696e 673d 2231 2e31 220d 0a20  oothing="1.1".. 
-00000600: 2020 2020 2020 6a6f 696e 7479 7065 3d22        jointype="
-00000610: 6578 7472 6170 6f6c 6174 6564 220d 0a20  extrapolated".. 
-00000620: 2020 2020 2020 6d69 7465 725f 6c69 6d69        miter_limi
-00000630: 743d 2231 3030 2220 2f3e 0d0a 2020 2020  t="100" />..    
-00000640: 3c69 6e6b 7363 6170 653a 7061 7468 2d65  <inkscape:path-e
-00000650: 6666 6563 740d 0a20 2020 2020 2020 6566  ffect..       ef
-00000660: 6665 6374 3d22 7461 7065 725f 7374 726f  fect="taper_stro
-00000670: 6b65 220d 0a20 2020 2020 2020 6964 3d22  ke"..       id="
-00000680: 7061 7468 2d65 6666 6563 7435 3338 312d  path-effect5381-
-00000690: 3222 0d0a 2020 2020 2020 2069 735f 7669  2"..       is_vi
-000006a0: 7369 626c 653d 2274 7275 6522 0d0a 2020  sible="true"..  
-000006b0: 2020 2020 2073 7472 6f6b 655f 7769 6474       stroke_widt
-000006c0: 683d 2231 220d 0a20 2020 2020 2020 6174  h="1"..       at
-000006d0: 7461 6368 5f73 7461 7274 3d22 3165 2d30  tach_start="1e-0
-000006e0: 3722 0d0a 2020 2020 2020 2065 6e64 5f6f  7"..       end_o
-000006f0: 6666 7365 743d 2230 2e39 3939 3939 220d  ffset="0.99999".
-00000700: 0a20 2020 2020 2020 736d 6f6f 7468 696e  .       smoothin
-00000710: 673d 2231 2e31 220d 0a20 2020 2020 2020  g="1.1"..       
-00000720: 6a6f 696e 7479 7065 3d22 6578 7472 6170  jointype="extrap
-00000730: 6f6c 6174 6564 220d 0a20 2020 2020 2020  olated"..       
-00000740: 6d69 7465 725f 6c69 6d69 743d 2231 3030  miter_limit="100
-00000750: 2220 2f3e 0d0a 2020 2020 3c69 6e6b 7363  " />..    <inksc
-00000760: 6170 653a 7061 7468 2d65 6666 6563 740d  ape:path-effect.
-00000770: 0a20 2020 2020 2020 6566 6665 6374 3d22  .       effect="
-00000780: 7461 7065 725f 7374 726f 6b65 220d 0a20  taper_stroke".. 
-00000790: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
-000007a0: 6666 6563 7435 3338 312d 332d 3122 0d0a  ffect5381-3-1"..
-000007b0: 2020 2020 2020 2069 735f 7669 7369 626c         is_visibl
-000007c0: 653d 2274 7275 6522 0d0a 2020 2020 2020  e="true"..      
-000007d0: 2073 7472 6f6b 655f 7769 6474 683d 2230   stroke_width="0
-000007e0: 2e39 220d 0a20 2020 2020 2020 6174 7461  .9"..       atta
-000007f0: 6368 5f73 7461 7274 3d22 3165 2d30 3722  ch_start="1e-07"
-00000800: 0d0a 2020 2020 2020 2065 6e64 5f6f 6666  ..       end_off
-00000810: 7365 743d 2231 2e34 3232 3030 3934 220d  set="1.4220094".
-00000820: 0a20 2020 2020 2020 736d 6f6f 7468 696e  .       smoothin
-00000830: 673d 2231 2e31 220d 0a20 2020 2020 2020  g="1.1"..       
-00000840: 6a6f 696e 7479 7065 3d22 6578 7472 6170  jointype="extrap
-00000850: 6f6c 6174 6564 220d 0a20 2020 2020 2020  olated"..       
-00000860: 6d69 7465 725f 6c69 6d69 743d 2231 3030  miter_limit="100
-00000870: 2220 2f3e 0d0a 2020 2020 3c69 6e6b 7363  " />..    <inksc
-00000880: 6170 653a 7061 7468 2d65 6666 6563 740d  ape:path-effect.
-00000890: 0a20 2020 2020 2020 6566 6665 6374 3d22  .       effect="
-000008a0: 7461 7065 725f 7374 726f 6b65 220d 0a20  taper_stroke".. 
-000008b0: 2020 2020 2020 6964 3d22 7061 7468 2d65        id="path-e
-000008c0: 6666 6563 7435 3338 312d 3722 0d0a 2020  ffect5381-7"..  
-000008d0: 2020 2020 2069 735f 7669 7369 626c 653d       is_visible=
-000008e0: 2274 7275 6522 0d0a 2020 2020 2020 2073  "true"..       s
-000008f0: 7472 6f6b 655f 7769 6474 683d 2230 2e39  troke_width="0.9
-00000900: 220d 0a20 2020 2020 2020 6174 7461 6368  "..       attach
-00000910: 5f73 7461 7274 3d22 3165 2d30 3722 0d0a  _start="1e-07"..
-00000920: 2020 2020 2020 2065 6e64 5f6f 6666 7365         end_offse
-00000930: 743d 2230 2e39 3939 3939 220d 0a20 2020  t="0.99999"..   
-00000940: 2020 2020 736d 6f6f 7468 696e 673d 2231      smoothing="1
-00000950: 2e31 220d 0a20 2020 2020 2020 6a6f 696e  .1"..       join
-00000960: 7479 7065 3d22 6578 7472 6170 6f6c 6174  type="extrapolat
-00000970: 6564 220d 0a20 2020 2020 2020 6d69 7465  ed"..       mite
-00000980: 725f 6c69 6d69 743d 2231 3030 2220 2f3e  r_limit="100" />
-00000990: 0d0a 2020 2020 3c69 6e6b 7363 6170 653a  ..    <inkscape:
-000009a0: 7061 7468 2d65 6666 6563 740d 0a20 2020  path-effect..   
-000009b0: 2020 2020 6566 6665 6374 3d22 7461 7065      effect="tape
-000009c0: 725f 7374 726f 6b65 220d 0a20 2020 2020  r_stroke"..     
-000009d0: 2020 6964 3d22 7061 7468 2d65 6666 6563    id="path-effec
-000009e0: 7435 3338 312d 332d 3922 0d0a 2020 2020  t5381-3-9"..    
-000009f0: 2020 2069 735f 7669 7369 626c 653d 2274     is_visible="t
-00000a00: 7275 6522 0d0a 2020 2020 2020 2073 7472  rue"..       str
-00000a10: 6f6b 655f 7769 6474 683d 2230 2e39 220d  oke_width="0.9".
-00000a20: 0a20 2020 2020 2020 6174 7461 6368 5f73  .       attach_s
-00000a30: 7461 7274 3d22 3165 2d30 3722 0d0a 2020  tart="1e-07"..  
-00000a40: 2020 2020 2065 6e64 5f6f 6666 7365 743d       end_offset=
-00000a50: 2231 2e34 3232 3030 3934 220d 0a20 2020  "1.4220094"..   
-00000a60: 2020 2020 736d 6f6f 7468 696e 673d 2231      smoothing="1
-00000a70: 2e31 220d 0a20 2020 2020 2020 6a6f 696e  .1"..       join
-00000a80: 7479 7065 3d22 6578 7472 6170 6f6c 6174  type="extrapolat
-00000a90: 6564 220d 0a20 2020 2020 2020 6d69 7465  ed"..       mite
-00000aa0: 725f 6c69 6d69 743d 2231 3030 2220 2f3e  r_limit="100" />
-00000ab0: 0d0a 2020 2020 3c69 6e6b 7363 6170 653a  ..    <inkscape:
-00000ac0: 7061 7468 2d65 6666 6563 740d 0a20 2020  path-effect..   
-00000ad0: 2020 2020 6566 6665 6374 3d22 7461 7065      effect="tape
-00000ae0: 725f 7374 726f 6b65 220d 0a20 2020 2020  r_stroke"..     
-00000af0: 2020 6964 3d22 7061 7468 2d65 6666 6563    id="path-effec
-00000b00: 7435 3338 312d 3622 0d0a 2020 2020 2020  t5381-6"..      
-00000b10: 2069 735f 7669 7369 626c 653d 2274 7275   is_visible="tru
-00000b20: 6522 0d0a 2020 2020 2020 2073 7472 6f6b  e"..       strok
-00000b30: 655f 7769 6474 683d 2230 2e39 220d 0a20  e_width="0.9".. 
-00000b40: 2020 2020 2020 6174 7461 6368 5f73 7461        attach_sta
-00000b50: 7274 3d22 3165 2d30 3722 0d0a 2020 2020  rt="1e-07"..    
-00000b60: 2020 2065 6e64 5f6f 6666 7365 743d 2230     end_offset="0
-00000b70: 2e39 3939 3939 220d 0a20 2020 2020 2020  .99999"..       
-00000b80: 736d 6f6f 7468 696e 673d 2231 2e31 220d  smoothing="1.1".
-00000b90: 0a20 2020 2020 2020 6a6f 696e 7479 7065  .       jointype
-00000ba0: 3d22 6578 7472 6170 6f6c 6174 6564 220d  ="extrapolated".
-00000bb0: 0a20 2020 2020 2020 6d69 7465 725f 6c69  .       miter_li
-00000bc0: 6d69 743d 2231 3030 2220 2f3e 0d0a 2020  mit="100" />..  
-00000bd0: 3c2f 6465 6673 3e0d 0a20 203c 736f 6469  </defs>..  <sodi
-00000be0: 706f 6469 3a6e 616d 6564 7669 6577 0d0a  podi:namedview..
-00000bf0: 2020 2020 2069 643d 2262 6173 6522 0d0a       id="base"..
-00000c00: 2020 2020 2070 6167 6563 6f6c 6f72 3d22       pagecolor="
-00000c10: 2366 6666 6666 6622 0d0a 2020 2020 2062  #ffffff"..     b
-00000c20: 6f72 6465 7263 6f6c 6f72 3d22 2336 3636  ordercolor="#666
-00000c30: 3636 3622 0d0a 2020 2020 2062 6f72 6465  666"..     borde
-00000c40: 726f 7061 6369 7479 3d22 312e 3022 0d0a  ropacity="1.0"..
-00000c50: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
-00000c60: 6765 6f70 6163 6974 793d 2230 2e30 220d  geopacity="0.0".
-00000c70: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
-00000c80: 6167 6573 6861 646f 773d 2232 220d 0a20  ageshadow="2".. 
-00000c90: 2020 2020 696e 6b73 6361 7065 3a7a 6f6f      inkscape:zoo
-00000ca0: 6d3d 2234 352e 3235 3438 3334 220d 0a20  m="45.254834".. 
-00000cb0: 2020 2020 696e 6b73 6361 7065 3a63 783d      inkscape:cx=
-00000cc0: 2234 2e30 3830 3935 3537 220d 0a20 2020  "4.0809557"..   
-00000cd0: 2020 696e 6b73 6361 7065 3a63 793d 2238    inkscape:cy="8
-00000ce0: 2e35 3939 3335 3822 0d0a 2020 2020 2069  .599358"..     i
-00000cf0: 6e6b 7363 6170 653a 646f 6375 6d65 6e74  nkscape:document
-00000d00: 2d75 6e69 7473 3d22 7078 220d 0a20 2020  -units="px"..   
-00000d10: 2020 696e 6b73 6361 7065 3a63 7572 7265    inkscape:curre
-00000d20: 6e74 2d6c 6179 6572 3d22 6c61 7965 7231  nt-layer="layer1
-00000d30: 220d 0a20 2020 2020 7368 6f77 6772 6964  "..     showgrid
-00000d40: 3d22 6661 6c73 6522 0d0a 2020 2020 2069  ="false"..     i
-00000d50: 6e6b 7363 6170 653a 7769 6e64 6f77 2d77  nkscape:window-w
-00000d60: 6964 7468 3d22 3334 3430 220d 0a20 2020  idth="3440"..   
-00000d70: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-00000d80: 772d 6865 6967 6874 3d22 3133 3231 220d  w-height="1321".
-00000d90: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-00000da0: 696e 646f 772d 783d 2230 220d 0a20 2020  indow-x="0"..   
-00000db0: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-00000dc0: 772d 793d 2232 3422 0d0a 2020 2020 2069  w-y="24"..     i
-00000dd0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d6d  nkscape:window-m
-00000de0: 6178 696d 697a 6564 3d22 3122 0d0a 2020  aximized="1"..  
-00000df0: 2020 2069 6e6b 7363 6170 653a 6772 6964     inkscape:grid
-00000e00: 2d62 626f 783d 2274 7275 6522 0d0a 2020  -bbox="true"..  
-00000e10: 2020 2069 6e6b 7363 6170 653a 736e 6170     inkscape:snap
-00000e20: 2d6e 6f64 6573 3d22 7472 7565 2220 2f3e  -nodes="true" />
-00000e30: 0d0a 2020 3c6d 6574 6164 6174 610d 0a20  ..  <metadata.. 
-00000e40: 2020 2020 6964 3d22 6d65 7461 6461 7461      id="metadata
-00000e50: 3133 223e 0d0a 2020 2020 3c72 6466 3a52  13">..    <rdf:R
-00000e60: 4446 3e0d 0a20 2020 2020 203c 6363 3a57  DF>..      <cc:W
-00000e70: 6f72 6b0d 0a20 2020 2020 2020 2020 7264  ork..         rd
-00000e80: 663a 6162 6f75 743d 2222 3e0d 0a20 2020  f:about="">..   
-00000e90: 2020 2020 203c 6463 3a66 6f72 6d61 743e       <dc:format>
-00000ea0: 696d 6167 652f 7376 672b 786d 6c3c 2f64  image/svg+xml</d
-00000eb0: 633a 666f 726d 6174 3e0d 0a20 2020 2020  c:format>..     
-00000ec0: 2020 203c 6463 3a74 7970 650d 0a20 2020     <dc:type..   
-00000ed0: 2020 2020 2020 2020 7264 663a 7265 736f          rdf:reso
-00000ee0: 7572 6365 3d22 6874 7470 3a2f 2f70 7572  urce="http://pur
-00000ef0: 6c2e 6f72 672f 6463 2f64 636d 6974 7970  l.org/dc/dcmityp
-00000f00: 652f 5374 696c 6c49 6d61 6765 2220 2f3e  e/StillImage" />
-00000f10: 0d0a 2020 2020 2020 2020 3c64 633a 7469  ..        <dc:ti
-00000f20: 746c 6520 2f3e 0d0a 2020 2020 2020 3c2f  tle />..      </
-00000f30: 6363 3a57 6f72 6b3e 0d0a 2020 2020 3c2f  cc:Work>..    </
-00000f40: 7264 663a 5244 463e 0d0a 2020 3c2f 6d65  rdf:RDF>..  </me
-00000f50: 7461 6461 7461 3e0d 0a20 203c 656c 6c69  tadata>..  <elli
-00000f60: 7073 650d 0a20 2020 2020 7374 796c 653d  pse..     style=
-00000f70: 2266 696c 6c3a 2330 3034 3461 613b 6669  "fill:#0044aa;fi
-00000f80: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-00000f90: 6f6b 653a 2330 3033 3338 303b 7374 726f  oke:#003380;stro
-00000fa0: 6b65 2d77 6964 7468 3a31 2e30 3132 3335  ke-width:1.01235
-00000fb0: 3137 353b 7374 726f 6b65 2d6c 696e 6563  175;stroke-linec
-00000fc0: 6170 3a62 7574 743b 7374 726f 6b65 2d6d  ap:butt;stroke-m
-00000fd0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00000fe0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00000ff0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00001000: 3a31 220d 0a20 2020 2020 6964 3d22 7061  :1"..     id="pa
-00001010: 7468 3832 3822 0d0a 2020 2020 2063 783d  th828"..     cx=
-00001020: 2238 220d 0a20 2020 2020 6379 3d22 3822  "8"..     cy="8"
-00001030: 0d0a 2020 2020 2072 783d 2237 2e34 3933  ..     rx="7.493
-00001040: 3832 3435 220d 0a20 2020 2020 7279 3d22  8245"..     ry="
-00001050: 372e 3439 3338 3234 2220 2f3e 0d0a 2020  7.493824" />..  
-00001060: 3c67 0d0a 2020 2020 2069 6e6b 7363 6170  <g..     inkscap
-00001070: 653a 6c61 6265 6c3d 224a 656c 6c79 220d  e:label="Jelly".
-00001080: 0a20 2020 2020 6964 3d22 6c61 7965 7231  .     id="layer1
-00001090: 220d 0a20 2020 2020 7374 796c 653d 2264  "..     style="d
-000010a0: 6973 706c 6179 3a69 6e6c 696e 6522 0d0a  isplay:inline"..
-000010b0: 2020 2020 2069 6e6b 7363 6170 653a 6772       inkscape:gr
-000010c0: 6f75 706d 6f64 653d 226c 6179 6572 223e  oupmode="layer">
-000010d0: 0d0a 2020 2020 3c67 0d0a 2020 2020 2020  ..    <g..      
-000010e0: 2069 643d 2267 3834 3122 0d0a 2020 2020   id="g841"..    
-000010f0: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
-00001100: 7472 6978 2830 2e38 3834 3237 3135 332c  trix(0.88427153,
-00001110: 302c 302c 302e 3838 3432 3731 3533 2c30  0,0,0.88427153,0
-00001120: 2e32 3038 3135 3730 312c 302e 3734 3236  .20815701,0.7426
-00001130: 3739 3735 2922 3e0d 0a20 2020 2020 203c  7975)">..      <
-00001140: 7061 7468 0d0a 2020 2020 2020 2020 2073  path..         s
-00001150: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00001160: 733d 2273 7373 7373 7373 7373 220d 0a20  s="sssssssss".. 
-00001170: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00001180: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-00001190: 7475 7265 3d22 3022 0d0a 2020 2020 2020  ture="0"..      
-000011a0: 2020 2069 643d 2272 6563 7432 3035 220d     id="rect205".
-000011b0: 0a20 2020 2020 2020 2020 643d 226d 2031  .         d="m 1
-000011c0: 312e 3231 3537 3036 2c31 2e39 3132 3030  1.215706,1.91200
-000011d0: 3631 2030 2e37 3334 3435 372c 302e 3331  61 0.734457,0.31
-000011e0: 3731 3331 3520 6320 302e 3831 3337 3738  71315 c 0.813778
-000011f0: 2c30 2e33 3531 3338 3232 2031 2e39 3939  ,0.3513822 1.999
-00001200: 3034 322c 312e 3338 3833 3330 3120 312e  042,1.3883301 1.
-00001210: 3439 3731 3938 2c32 2e31 3835 3238 3731  497198,2.1852871
-00001220: 204c 2031 312e 3834 3131 3633 2c36 2e39   L 11.841163,6.9
-00001230: 3635 3136 3131 2043 2031 312e 3333 3933  651611 C 11.3393
-00001240: 3139 2c37 2e37 3632 3131 3833 2031 302e  19,7.7621183 10.
-00001250: 3933 3638 3238 2c38 2e33 3237 3032 3836  936828,8.3270286
-00001260: 2039 2e35 3731 3637 3238 2c37 2e37 3337   9.5716728,7.737
-00001270: 3536 3638 204c 2038 2e38 3337 3231 3636  5668 L 8.8372166
-00001280: 2c37 2e34 3230 3433 3533 2043 2037 2e34  ,7.4204353 C 7.4
-00001290: 3134 3833 3635 2c36 2e38 3036 3236 3435  148365,6.8062645
-000012a0: 2037 2e37 3036 3234 3035 2c36 2e31 3030   7.7062405,6.100
-000012b0: 3032 3739 2038 2e30 3031 3336 3534 2c35  0279 8.0013654,5
-000012c0: 2e32 3035 3636 3234 204c 2038 2e39 3337  .2056624 L 8.937
-000012d0: 3531 3732 2c32 2e33 3638 3638 3733 2043  5172,2.3686873 C
-000012e0: 2039 2e32 3332 3634 3139 2c31 2e34 3734   9.2326419,1.474
-000012f0: 3332 3234 2031 302e 3430 3139 3238 2c31  3224 10.401928,1
-00001300: 2e35 3630 3632 3337 2031 312e 3231 3537  .5606237 11.2157
-00001310: 3036 2c31 2e39 3132 3030 3631 205a 220d  06,1.9120061 Z".
-00001320: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00001330: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
-00001340: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00001350: 2d77 6964 7468 3a31 3b73 7472 6f6b 652d  -width:1;stroke-
-00001360: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00001370: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00001380: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00001390: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-000013a0: 6163 6974 793a 3122 202f 3e0d 0a20 2020  acity:1" />..   
-000013b0: 2020 203c 7061 7468 0d0a 2020 2020 2020     <path..      
-000013c0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-000013d0: 616e 736c 6174 6528 302e 3431 3230 3731  anslate(0.412071
-000013e0: 3631 2c2d 312e 3435 3732 3431 3529 220d  61,-1.4572415)".
-000013f0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00001400: 7065 3a6f 7269 6769 6e61 6c2d 643d 224d  pe:original-d="M
-00001410: 2037 2e33 3538 3332 3939 2c38 2e31 3939   7.3583299,8.199
-00001420: 3732 3833 2043 2036 2e36 3935 3431 3733  7283 C 6.6954173
-00001430: 2c39 2e31 3732 3030 3031 2035 2e30 3433  ,9.1720001 5.043
-00001440: 3237 3134 2c39 2e30 3538 3334 3439 2035  2714,9.0583449 5
-00001450: 2e35 3138 3032 3936 2c39 2e39 3935 3934  .5180296,9.99594
-00001460: 3837 2036 2e30 3539 3233 312c 3130 2e39  87 6.059231,10.9
-00001470: 3333 3333 3720 342e 3637 3538 3037 332c  33337 4.6758073,
-00001480: 3131 2e35 3431 3832 3320 332e 3937 3734  11.541823 3.9774
-00001490: 3735 372c 3131 2e31 3338 3634 3120 332e  757,11.138641 3.
-000014a0: 3239 3835 3634 312c 3130 2e37 3436 3637  2985641,10.74667
-000014b0: 3120 332e 3038 3838 3035 352c 3132 2e34  1 3.0888055,12.4
-000014c0: 3535 3737 3320 312e 3738 3938 3634 2c31  55773 1.789864,1
-000014d0: 332e 3139 3336 3722 0d0a 2020 2020 2020  3.19367"..      
-000014e0: 2020 2069 6e6b 7363 6170 653a 7061 7468     inkscape:path
-000014f0: 2d65 6666 6563 743d 2223 7061 7468 2d65  -effect="#path-e
-00001500: 6666 6563 7435 3338 3122 0d0a 2020 2020  ffect5381"..    
-00001510: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-00001520: 6465 7479 7065 733d 2263 6363 6322 0d0a  detypes="cccc"..
-00001530: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00001540: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00001550: 6174 7572 653d 2230 220d 0a20 2020 2020  ature="0"..     
-00001560: 2020 2020 6964 3d22 7061 7468 3439 3335      id="path4935
-00001570: 220d 0a20 2020 2020 2020 2020 643d 224d  "..         d="M
-00001580: 2036 2e39 3836 3532 3735 2c37 2e39 3436   6.9865275,7.946
-00001590: 3232 3639 2043 2036 2e37 3537 3638 3937  2269 C 6.7576897
-000015a0: 2c38 2e32 3831 3835 3535 2036 2e32 3835  ,8.2818555 6.285
-000015b0: 3034 3339 2c38 2e34 3739 3537 3737 2035  0439,8.4795777 5
-000015c0: 2e38 3136 3234 3032 2c38 2e37 3035 3433  .8162402,8.70543
-000015d0: 3435 2035 2e35 3831 3833 3834 2c38 2e38  45 5.5818384,8.8
-000015e0: 3138 3336 3239 2035 2e33 3336 3736 392c  183629 5.336769,
-000015f0: 382e 3933 3035 3437 3820 352e 3134 3732  8.9305478 5.1472
-00001600: 3337 332c 392e 3139 3330 3234 3320 342e  373,9.1930243 4.
-00001610: 3935 3737 3035 352c 392e 3435 3535 3030  9577055,9.455500
-00001620: 3920 342e 3935 3230 3130 372c 392e 3837  9 4.9520107,9.87
-00001630: 3432 3537 3520 352e 3131 3635 3632 372c  42575 5.1165627,
-00001640: 3130 2e31 3939 3233 3320 6120 312e 3032  10.199233 a 1.02
-00001650: 3436 3030 382c 312e 3032 3436 3030 3820  46008,1.0246008 
-00001660: 3020 3020 3020 302e 3030 3637 372c 302e  0 0 0 0.00677,0.
-00001670: 3031 3331 3420 312e 3834 3730 3732 322c  01314 1.8470722,
-00001680: 312e 3834 3730 3732 3220 3020 3020 3120  1.8470722 0 0 1 
-00001690: 302e 3030 3439 382c 302e 3030 3836 2063  0.00498,0.0086 c
-000016a0: 2030 2e31 3636 3530 3433 2c30 2e32 3838   0.1665043,0.288
-000016b0: 3339 3420 302e 3038 3336 3034 2c30 2e33  394 0.083604,0.3
-000016c0: 3234 3932 202d 302e 3134 3639 3532 322c  2492 -0.1469522,
-000016d0: 302e 3436 3330 3031 202d 302e 3233 3035  0.463001 -0.2305
-000016e0: 3536 322c 302e 3133 3830 3831 202d 302e  562,0.138081 -0.
-000016f0: 3632 3630 3531 312c 302e 3135 3332 3231  6260511,0.153221
-00001700: 202d 302e 3737 3838 3930 322c 302e 3036   -0.7788902,0.06
-00001710: 3439 3820 302c 3020 2d33 2e36 3165 2d35  498 0,0 -3.61e-5
-00001720: 2c2d 322e 3165 2d35 202d 332e 3631 652d  ,-2.1e-5 -3.61e-
-00001730: 352c 2d32 2e31 652d 3520 2d30 2e33 3630  5,-2.1e-5 -0.360
-00001740: 3732 3039 2c2d 302e 3136 3935 3037 202d  7209,-0.169507 -
-00001750: 302e 3731 3331 3535 2c2d 302e 3130 3136  0.713155,-0.1016
-00001760: 3331 202d 302e 3936 3231 3438 312c 302e  31 -0.9621481,0.
-00001770: 3130 3331 3331 202d 302e 3235 3832 3139  103131 -0.258219
-00001780: 332c 302e 3234 3134 3136 202d 302e 3430  3,0.241416 -0.40
-00001790: 3037 3839 322c 302e 3530 3135 3437 202d  07892,0.501547 -
-000017a0: 302e 3438 3538 3830 312c 302e 3636 3030  0.4858801,0.6600
-000017b0: 3235 202d 302e 3536 3239 3336 392c 302e  25 -0.5629369,0.
-000017c0: 3933 3230 3439 202d 302e 3831 3034 3332  932049 -0.810432
-000017d0: 392c 312e 3235 3634 3535 202d 302e 3932  9,1.256455 -0.92
-000017e0: 3431 3233 352c 312e 3434 3535 3836 202d  41235,1.445586 -
-000017f0: 302e 3131 3533 3232 352c 302e 3139 3138  0.1153225,0.1918
-00001800: 3436 202d 302e 3033 3339 3331 2c30 2e32  46 -0.033931,0.2
-00001810: 3332 3331 3620 2d30 2e30 3333 3933 312c  32316 -0.033931,
-00001820: 302e 3233 3233 3136 2030 2c30 202d 302e  0.232316 0,0 -0.
-00001830: 3030 3938 382c 302e 3131 3639 3733 2030  00988,0.116973 0
-00001840: 2e32 3333 3534 3436 2c30 2e30 3636 3538  .2335446,0.06658
-00001850: 2030 2e32 3431 3934 3739 2c2d 302e 3035   0.2419479,-0.05
-00001860: 3030 3920 302e 3738 3739 3636 392c 2d30  009 0.7879669,-0
-00001870: 2e32 3937 3835 3220 312e 3434 3830 3331  .297852 1.448031
-00001880: 2c2d 312e 3238 3336 3736 2030 2e31 3233  ,-1.283676 0.123
-00001890: 3031 3136 2c2d 302e 3136 3739 3431 2030  0116,-0.167941 0
-000018a0: 2e32 3431 3432 3737 2c2d 302e 3337 3137  .2414277,-0.3717
-000018b0: 3338 2030 2e33 3435 3536 3937 2c2d 302e  38 0.3455697,-0.
-000018c0: 3434 3336 3732 202d 302e 3031 3930 3233  443672 -0.019023
-000018d0: 2c30 2e30 3036 3620 2d30 2e30 3037 3138  ,0.0066 -0.00718
-000018e0: 2c2d 302e 3030 3236 202d 302e 3037 3130  ,-0.0026 -0.0710
-000018f0: 3331 2c2d 382e 3532 652d 3420 302c 3020  31,-8.52e-4 0,0 
-00001900: 342e 3665 2d36 2c32 652d 3620 342e 3765  4.6e-6,2e-6 4.7e
-00001910: 2d36 2c32 652d 3620 302e 3534 3534 3932  -6,2e-6 0.545492
-00001920: 342c 302e 3331 3439 3431 2031 2e31 3930  4,0.314941 1.190
-00001930: 3837 3532 2c30 2e32 3237 3432 3920 312e  8752,0.227429 1.
-00001940: 3639 3133 3133 342c 2d30 2e30 3732 3239  6913134,-0.07229
-00001950: 2043 2035 2e39 3431 3332 3532 2c31 312e   C 5.9413252,11.
-00001960: 3135 3830 3932 2036 2e32 3738 3531 2c31  158092 6.27851,1
-00001970: 302e 3432 3834 3639 2035 2e39 3134 3138  0.428469 5.91418
-00001980: 3739 2c39 2e37 3832 3234 3831 2035 2e38  79,9.7822481 5.8
-00001990: 3437 3830 3436 2c39 2e36 3532 3836 3736  478046,9.6528676
-000019a0: 2035 2e38 3639 3634 3532 2c39 2e37 3239   5.8696452,9.729
-000019b0: 3934 3135 2035 2e38 3736 3839 3433 2c39  9415 5.8768943,9
-000019c0: 2e37 3139 3930 3235 2035 2e38 3834 3333  .7199025 5.88433
-000019d0: 3031 2c39 2e37 3039 3630 3439 2036 2e30  01,9.7096049 6.0
-000019e0: 3034 3731 3231 2c39 2e36 3133 3633 3539  047121,9.6136359
-000019f0: 2036 2e32 3036 3836 3539 2c39 2e35 3136   6.2068659,9.516
-00001a00: 3234 3337 2036 2e36 3131 3137 3337 2c39  2437 6.6111737,9
-00001a10: 2e33 3231 3435 3932 2037 2e32 3936 3035  .3214592 7.29605
-00001a20: 372c 392e 3038 3938 3733 3220 372e 3733  7,9.0898732 7.73
-00001a30: 3031 3331 392c 382e 3435 3332 3330 3320  01319,8.4532303 
-00001a40: 5a22 0d0a 2020 2020 2020 2020 2073 7479  Z"..         sty
-00001a50: 6c65 3d22 6669 6c6c 3a23 6666 6666 6666  le="fill:#ffffff
-00001a60: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
-00001a70: 726f 3b73 7472 6f6b 653a 6e6f 6e65 3b73  ro;stroke:none;s
-00001a80: 7472 6f6b 652d 7769 6474 683a 3170 783b  troke-width:1px;
-00001a90: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00001aa0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-00001ab0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00001ac0: 2d6f 7061 6369 7479 3a31 2220 2f3e 0d0a  -opacity:1" />..
-00001ad0: 2020 2020 2020 3c70 6174 680d 0a20 2020        <path..   
-00001ae0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-00001af0: 2274 7261 6e73 6c61 7465 2832 2e35 3634  "translate(2.564
-00001b00: 3531 3735 2c2d 302e 3436 3035 3337 3334  5175,-0.46053734
-00001b10: 2922 0d0a 2020 2020 2020 2020 2069 6e6b  )"..         ink
-00001b20: 7363 6170 653a 6f72 6967 696e 616c 2d64  scape:original-d
-00001b30: 3d22 6d20 382e 3137 3539 3232 312c 382e  ="m 8.1759221,8.
-00001b40: 3033 3430 3030 3120 6320 302c 312e 3236  0340001 c 0,1.26
-00001b50: 3139 3036 3220 302e 3335 3330 3830 382c  19062 0.3530808,
-00001b60: 322e 3533 3737 3137 3920 2d30 2e38 3533  2.5377179 -0.853
-00001b70: 3634 3832 2c32 2e35 3337 3731 3739 202d  6482,2.5377179 -
-00001b80: 312e 3530 3635 3834 2c30 202d 312e 3135  1.506584,0 -1.15
-00001b90: 3831 3336 382c 312e 3238 3830 3631 202d  81368,1.288061 -
-00001ba0: 302e 3636 3634 3138 2c32 2e31 3339 3734  0.666418,2.13974
-00001bb0: 3320 302e 3537 3439 3331 352c 312e 3035  3 0.5749315,1.05
-00001bc0: 3537 3033 202d 302e 3431 3233 3630 382c  5703 -0.4123608,
-00001bd0: 312e 3138 3939 3120 2d31 2e37 3131 3330  1.18991 -1.71130
-00001be0: 3233 2c31 2e39 3237 3830 3722 0d0a 2020  23,1.927807"..  
-00001bf0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00001c00: 7061 7468 2d65 6666 6563 743d 2223 7061  path-effect="#pa
-00001c10: 7468 2d65 6666 6563 7435 3338 312d 3322  th-effect5381-3"
-00001c20: 0d0a 2020 2020 2020 2020 2073 6f64 6970  ..         sodip
-00001c30: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
-00001c40: 6363 6322 0d0a 2020 2020 2020 2020 2069  ccc"..         i
-00001c50: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-00001c60: 722d 6375 7276 6174 7572 653d 2230 220d  r-curvature="0".
-00001c70: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00001c80: 7468 3439 3335 2d36 220d 0a20 2020 2020  th4935-6"..     
-00001c90: 2020 2020 643d 226d 2037 2e37 3235 3932      d="m 7.72592
-00001ca0: 3231 2c38 2e30 3334 3030 3035 2063 2030  21,8.0340005 c 0
-00001cb0: 2c30 2e36 3732 3932 3239 2030 2e30 3738  ,0.6729229 0.078
-00001cc0: 3238 352c 312e 3331 3230 3436 3620 302e  285,1.3120466 0.
-00001cd0: 3032 3935 3237 2c31 2e36 3833 3530 3834  029527,1.6835084
-00001ce0: 202d 302e 3034 3837 3538 2c30 2e33 3731   -0.048758,0.371
-00001cf0: 3436 3231 2030 2e30 3131 3630 332c 302e  4621 0.011603,0.
-00001d00: 3430 3432 3039 3120 2d30 2e34 3333 3137  4042091 -0.43317
-00001d10: 3437 2c30 2e34 3034 3230 3931 202d 302e  47,0.4042091 -0.
-00001d20: 3530 3935 3139 312c 3020 2d30 2e39 3330  5095191,0 -0.930
-00001d30: 3031 3937 2c30 2e31 3331 3034 3920 2d31  0197,0.131049 -1
-00001d40: 2e32 3037 3039 3432 2c30 2e34 3139 3231  .2070942,0.41921
-00001d50: 3320 2d30 2e32 3737 3037 3435 2c30 2e32  3 -0.2770745,0.2
-00001d60: 3838 3136 3420 2d30 2e33 3530 3239 3437  88164 -0.3502947
-00001d70: 2c30 2e36 3737 3734 3520 2d30 2e33 3235  ,0.677745 -0.325
-00001d80: 3438 3738 2c31 2e30 3231 3135 3520 302e  4878,1.021155 0.
-00001d90: 3034 3938 372c 302e 3537 3037 3132 2030  04987,0.570712 0
-00001da0: 2e32 3830 3635 3034 2c31 2e30 3338 3438  .2806504,1.03848
-00001db0: 3320 302e 3438 3438 3137 352c 312e 3336  3 0.4848175,1.36
-00001dc0: 3332 3536 2030 2e31 3536 3533 3338 2c30  3256 0.1565338,0
-00001dd0: 2e32 3535 3130 3520 302e 3132 3234 3734  .255105 0.122474
-00001de0: 392c 302e 3530 3131 3839 202d 302e 3030  9,0.501189 -0.00
-00001df0: 3739 322c 302e 3535 3939 3231 202d 302e  792,0.559921 -0.
-00001e00: 3633 3938 3836 2c30 2e35 3832 3837 3520  639886,0.582875 
-00001e10: 2d31 2e31 3430 3037 3931 2c30 2e37 3933  -1.1400791,0.793
-00001e20: 3231 3220 2d31 2e32 3732 3636 3134 2c30  212 -1.2726614,0
-00001e30: 2e39 3537 3137 3220 2d30 2e31 3332 3033  .957172 -0.13203
-00001e40: 3537 2c30 2e31 3633 3238 3420 2d30 2e30  57,0.163284 -0.0
-00001e50: 3430 3630 342c 302e 3139 3138 3636 202d  40604,0.191866 -
-00001e60: 302e 3034 3036 3034 2c30 2e31 3931 3836  0.040604,0.19186
-00001e70: 3620 302c 3020 2d30 2e30 3231 3334 352c  6 0,0 -0.021345,
-00001e80: 302e 3038 3437 3120 302e 3138 3035 3237  0.08471 0.180527
-00001e90: 332c 302e 3037 3035 3820 2d30 2e30 3134  3,0.07058 -0.014
-00001ea0: 3335 372c 302e 3030 3120 302e 3833 3831  357,0.001 0.8381
-00001eb0: 3036 392c 2d30 2e30 3839 3720 312e 3630  069,-0.0897 1.60
-00001ec0: 3533 3832 352c 2d30 2e36 3031 3036 3320  53825,-0.601063 
-00001ed0: 302e 3338 3933 3436 312c 2d30 2e33 3430  0.3893461,-0.340
-00001ee0: 3037 3720 302e 3632 3634 3538 312c 2d30  077 0.6264581,-0
-00001ef0: 2e39 3732 3632 3920 302e 3239 3739 3733  .972629 0.297973
-00001f00: 322c 2d31 2e36 3036 3234 3120 2d30 2e31  2,-1.606241 -0.1
-00001f10: 3532 3037 3737 2c2d 302e 3239 3139 3538  520777,-0.291958
-00001f20: 202d 302e 3333 3337 3930 322c 2d30 2e36   -0.3337902,-0.6
-00001f30: 3630 3932 3220 2d30 2e33 3439 3834 3935  60922 -0.3498495
-00001f40: 2c2d 312e 3030 3033 3339 202d 302e 3031  ,-1.000339 -0.01
-00001f50: 3333 3038 2c2d 302e 3138 3432 3239 2030  3308,-0.184229 0
-00001f60: 2e30 3139 3935 322c 2d30 2e32 3733 3632  .019952,-0.27362
-00001f70: 3120 302e 3037 3635 3834 2c2d 302e 3333  1 0.076584,-0.33
-00001f80: 3235 3220 302e 3035 3636 3332 2c2d 302e  252 0.056632,-0.
-00001f90: 3035 3839 2030 2e31 3937 3036 3439 2c2d  0589 0.1970649,-
-00001fa0: 302e 3134 3330 3033 2030 2e35 3538 3333  0.143003 0.55833
-00001fb0: 3732 2c2d 302e 3134 3330 3033 2030 2e37  72,-0.143003 0.7
-00001fc0: 3631 3935 3136 2c30 2031 2e32 3439 3133  619516,0 1.24913
-00001fd0: 3638 2c2d 302e 3630 3531 3539 2031 2e33  68,-0.605159 1.3
-00001fe0: 3235 3532 3032 2c2d 312e 3138 3730 3738  255202,-1.187078
-00001ff0: 3920 302e 3037 3633 3834 2c2d 302e 3538  9 0.076384,-0.58
-00002000: 3139 3230 3420 2d30 2e30 3231 3837 322c  19204 -0.021872,
-00002010: 2d31 2e32 3131 3635 3535 202d 302e 3032  -1.2116555 -0.02
-00002020: 3138 3732 2c2d 312e 3830 3036 3338 3620  1872,-1.8006386 
-00002030: 7a22 0d0a 2020 2020 2020 2020 2073 7479  z"..         sty
-00002040: 6c65 3d22 6669 6c6c 3a23 6666 6666 6666  le="fill:#ffffff
-00002050: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
-00002060: 726f 3b73 7472 6f6b 653a 6e6f 6e65 3b73  ro;stroke:none;s
-00002070: 7472 6f6b 652d 7769 6474 683a 3170 783b  troke-width:1px;
-00002080: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00002090: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-000020a0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-000020b0: 2d6f 7061 6369 7479 3a31 2220 2f3e 0d0a  -opacity:1" />..
-000020c0: 2020 2020 2020 3c70 6174 680d 0a20 2020        <path..   
-000020d0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-000020e0: 226d 6174 7269 7828 302e 3734 3533 3433  "matrix(0.745343
-000020f0: 3931 2c2d 302e 3130 3037 3430 372c 302e  91,-0.1007407,0.
-00002100: 3130 3037 3430 372c 302e 3734 3533 3433  1007407,0.745343
-00002110: 3931 2c31 2e31 3639 3630 3139 2c31 2e35  91,1.1696019,1.5
-00002120: 3830 3434 3436 2922 0d0a 2020 2020 2020  804446)"..      
-00002130: 2020 2069 6e6b 7363 6170 653a 6f72 6967     inkscape:orig
-00002140: 696e 616c 2d64 3d22 6d20 382e 3137 3539  inal-d="m 8.1759
-00002150: 3232 312c 382e 3033 3430 3030 3120 6320  221,8.0340001 c 
-00002160: 302c 312e 3236 3139 3036 3220 302e 3335  0,1.2619062 0.35
-00002170: 3330 3830 382c 322e 3533 3737 3137 3920  30808,2.5377179 
-00002180: 2d30 2e38 3533 3634 3832 2c32 2e35 3337  -0.8536482,2.537
-00002190: 3731 3739 202d 312e 3530 3635 3834 2c30  7179 -1.506584,0
-000021a0: 202d 312e 3135 3831 3336 382c 312e 3238   -1.1581368,1.28
-000021b0: 3830 3631 202d 302e 3636 3634 3138 2c32  8061 -0.666418,2
-000021c0: 2e31 3339 3734 3320 302e 3537 3439 3331  .139743 0.574931
-000021d0: 352c 312e 3035 3537 3033 202d 302e 3431  5,1.055703 -0.41
-000021e0: 3233 3630 382c 312e 3138 3939 3120 2d31  23608,1.18991 -1
-000021f0: 2e37 3131 3330 3233 2c31 2e39 3237 3830  .7113023,1.92780
-00002200: 3722 0d0a 2020 2020 2020 2020 2069 6e6b  7"..         ink
-00002210: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
-00002220: 743d 2223 7061 7468 2d65 6666 6563 7435  t="#path-effect5
-00002230: 3338 312d 332d 3922 0d0a 2020 2020 2020  381-3-9"..      
-00002240: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00002250: 7479 7065 733d 2263 6363 6322 0d0a 2020  types="cccc"..  
-00002260: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00002270: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00002280: 7572 653d 2230 220d 0a20 2020 2020 2020  ure="0"..       
-00002290: 2020 6964 3d22 7061 7468 3439 3335 2d36    id="path4935-6
-000022a0: 2d33 220d 0a20 2020 2020 2020 2020 643d  -3"..         d=
-000022b0: 226d 2037 2e37 3235 3932 3231 2c38 2e30  "m 7.7259221,8.0
-000022c0: 3334 3030 3035 2063 2030 2c30 2e36 3732  340005 c 0,0.672
-000022d0: 3932 3239 2030 2e30 3738 3238 352c 312e  9229 0.078285,1.
-000022e0: 3331 3230 3436 3620 302e 3032 3935 3237  3120466 0.029527
-000022f0: 2c31 2e36 3833 3530 3834 202d 302e 3034  ,1.6835084 -0.04
-00002300: 3837 3538 2c30 2e33 3731 3436 3231 2030  8758,0.3714621 0
-00002310: 2e30 3131 3630 332c 302e 3430 3432 3039  .011603,0.404209
-00002320: 3120 2d30 2e34 3333 3137 3437 2c30 2e34  1 -0.4331747,0.4
-00002330: 3034 3230 3931 202d 302e 3530 3935 3139  042091 -0.509519
-00002340: 312c 3020 2d30 2e39 3330 3031 3937 2c30  1,0 -0.9300197,0
-00002350: 2e31 3331 3034 3920 2d31 2e32 3037 3039  .131049 -1.20709
-00002360: 3432 2c30 2e34 3139 3231 3320 2d30 2e32  42,0.419213 -0.2
-00002370: 3737 3037 3435 2c30 2e32 3838 3136 3420  770745,0.288164 
-00002380: 2d30 2e33 3530 3239 3437 2c30 2e36 3737  -0.3502947,0.677
-00002390: 3734 3520 2d30 2e33 3235 3438 3738 2c31  745 -0.3254878,1
-000023a0: 2e30 3231 3135 3520 302e 3034 3938 372c  .021155 0.04987,
-000023b0: 302e 3537 3037 3132 2030 2e32 3830 3635  0.570712 0.28065
-000023c0: 3034 2c31 2e30 3338 3438 3320 302e 3438  04,1.038483 0.48
-000023d0: 3438 3137 352c 312e 3336 3332 3536 2030  48175,1.363256 0
-000023e0: 2e31 3536 3533 3338 2c30 2e32 3535 3130  .1565338,0.25510
-000023f0: 3520 302e 3132 3234 3734 392c 302e 3530  5 0.1224749,0.50
-00002400: 3131 3839 202d 302e 3030 3739 322c 302e  1189 -0.00792,0.
-00002410: 3535 3939 3231 202d 302e 3633 3938 3836  559921 -0.639886
-00002420: 2c30 2e35 3832 3837 3520 2d31 2e31 3430  ,0.582875 -1.140
-00002430: 3037 3931 2c30 2e37 3933 3231 3220 2d31  0791,0.793212 -1
-00002440: 2e32 3732 3636 3134 2c30 2e39 3537 3137  .2726614,0.95717
-00002450: 3220 2d30 2e31 3332 3033 3537 2c30 2e31  2 -0.1320357,0.1
-00002460: 3633 3238 3420 2d30 2e30 3430 3630 342c  63284 -0.040604,
-00002470: 302e 3139 3138 3636 202d 302e 3034 3036  0.191866 -0.0406
-00002480: 3034 2c30 2e31 3931 3836 3620 302c 3020  04,0.191866 0,0 
-00002490: 2d30 2e30 3231 3334 352c 302e 3038 3437  -0.021345,0.0847
-000024a0: 3120 302e 3138 3035 3237 332c 302e 3037  1 0.1805273,0.07
-000024b0: 3035 3820 2d30 2e30 3134 3335 372c 302e  058 -0.014357,0.
-000024c0: 3030 3120 302e 3833 3831 3036 392c 2d30  001 0.8381069,-0
-000024d0: 2e30 3839 3720 312e 3630 3533 3832 352c  .0897 1.6053825,
-000024e0: 2d30 2e36 3031 3036 3320 302e 3338 3933  -0.601063 0.3893
-000024f0: 3436 312c 2d30 2e33 3430 3037 3720 302e  461,-0.340077 0.
-00002500: 3632 3634 3538 312c 2d30 2e39 3732 3632  6264581,-0.97262
-00002510: 3920 302e 3239 3739 3733 322c 2d31 2e36  9 0.2979732,-1.6
-00002520: 3036 3234 3120 2d30 2e31 3532 3037 3737  06241 -0.1520777
-00002530: 2c2d 302e 3239 3139 3538 202d 302e 3333  ,-0.291958 -0.33
-00002540: 3337 3930 322c 2d30 2e36 3630 3932 3220  37902,-0.660922 
-00002550: 2d30 2e33 3439 3834 3935 2c2d 312e 3030  -0.3498495,-1.00
-00002560: 3033 3339 202d 302e 3031 3333 3038 2c2d  0339 -0.013308,-
-00002570: 302e 3138 3432 3239 2030 2e30 3139 3935  0.184229 0.01995
-00002580: 322c 2d30 2e32 3733 3632 3120 302e 3037  2,-0.273621 0.07
-00002590: 3635 3834 2c2d 302e 3333 3235 3220 302e  6584,-0.33252 0.
-000025a0: 3035 3636 3332 2c2d 302e 3035 3839 2030  056632,-0.0589 0
-000025b0: 2e31 3937 3036 3439 2c2d 302e 3134 3330  .1970649,-0.1430
-000025c0: 3033 2030 2e35 3538 3333 3732 2c2d 302e  03 0.5583372,-0.
-000025d0: 3134 3330 3033 2030 2e37 3631 3935 3136  143003 0.7619516
-000025e0: 2c30 2031 2e32 3439 3133 3638 2c2d 302e  ,0 1.2491368,-0.
-000025f0: 3630 3531 3539 2031 2e33 3235 3532 3032  605159 1.3255202
-00002600: 2c2d 312e 3138 3730 3738 3920 302e 3037  ,-1.1870789 0.07
-00002610: 3633 3834 2c2d 302e 3538 3139 3230 3420  6384,-0.5819204 
-00002620: 2d30 2e30 3231 3837 322c 2d31 2e32 3131  -0.021872,-1.211
-00002630: 3635 3535 202d 302e 3032 3138 3732 2c2d  6555 -0.021872,-
-00002640: 312e 3830 3036 3338 3620 7a22 0d0a 2020  1.8006386 z"..  
-00002650: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00002660: 6c6c 3a23 6666 6666 6666 3b66 696c 6c2d  ll:#ffffff;fill-
-00002670: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
-00002680: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-00002690: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
-000026a0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-000026b0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-000026c0: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
-000026d0: 7479 3a31 2220 2f3e 0d0a 2020 2020 2020  ty:1" />..      
-000026e0: 3c70 6174 680d 0a20 2020 2020 2020 2020  <path..         
-000026f0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-00002700: 7828 2d30 2e37 3238 3432 3632 392c 2d30  x(-0.72842629,-0
-00002710: 2e34 3833 3430 3836 312c 2d30 2e34 3839  .48340861,-0.489
-00002720: 3132 3238 342c 302e 3731 3939 3136 3337  12284,0.71991637
-00002730: 2c32 302e 3739 3333 3234 2c35 2e35 3332  ,20.793324,5.532
-00002740: 3637 3932 2922 0d0a 2020 2020 2020 2020  6792)"..        
-00002750: 2069 6e6b 7363 6170 653a 6f72 6967 696e   inkscape:origin
-00002760: 616c 2d64 3d22 4d20 372e 3335 3833 3239  al-d="M 7.358329
-00002770: 392c 382e 3139 3937 3238 3320 4320 362e  9,8.1997283 C 6.
-00002780: 3639 3534 3137 332c 392e 3137 3230 3030  6954173,9.172000
-00002790: 3120 352e 3034 3332 3731 342c 392e 3035  1 5.0432714,9.05
-000027a0: 3833 3434 3920 352e 3531 3830 3239 362c  83449 5.5180296,
-000027b0: 392e 3939 3539 3438 3720 362e 3035 3932  9.9959487 6.0592
-000027c0: 3331 2c31 302e 3933 3333 3337 2034 2e36  31,10.933337 4.6
-000027d0: 3735 3830 3733 2c31 312e 3534 3138 3233  758073,11.541823
-000027e0: 2033 2e39 3737 3437 3537 2c31 312e 3133   3.9774757,11.13
-000027f0: 3836 3431 2033 2e32 3938 3536 3431 2c31  8641 3.2985641,1
-00002800: 302e 3734 3636 3731 2033 2e30 3838 3830  0.746671 3.08880
-00002810: 3535 2c31 322e 3435 3537 3733 2031 2e37  55,12.455773 1.7
-00002820: 3839 3836 342c 3133 2e31 3933 3637 220d  89864,13.19367".
-00002830: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00002840: 7065 3a70 6174 682d 6566 6665 6374 3d22  pe:path-effect="
-00002850: 2370 6174 682d 6566 6665 6374 3533 3831  #path-effect5381
-00002860: 2d36 220d 0a20 2020 2020 2020 2020 736f  -6"..         so
-00002870: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00002880: 3d22 6363 6363 220d 0a20 2020 2020 2020  ="cccc"..       
-00002890: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-000028a0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-000028b0: 3022 0d0a 2020 2020 2020 2020 2069 643d  0"..         id=
-000028c0: 2270 6174 6834 3933 352d 3022 0d0a 2020  "path4935-0"..  
-000028d0: 2020 2020 2020 2064 3d22 4d20 362e 3938         d="M 6.98
-000028e0: 3635 3237 352c 372e 3934 3632 3236 3920  65275,7.9462269 
-000028f0: 4320 362e 3735 3736 3839 372c 382e 3238  C 6.7576897,8.28
-00002900: 3138 3535 3520 362e 3238 3530 3433 392c  18555 6.2850439,
-00002910: 382e 3437 3935 3737 3720 352e 3831 3632  8.4795777 5.8162
-00002920: 3430 322c 382e 3730 3534 3334 3520 352e  402,8.7054345 5.
-00002930: 3538 3138 3338 342c 382e 3831 3833 3632  5818384,8.818362
-00002940: 3920 352e 3333 3637 3639 2c38 2e39 3330  9 5.336769,8.930
-00002950: 3534 3738 2035 2e31 3437 3233 3733 2c39  5478 5.1472373,9
-00002960: 2e31 3933 3032 3433 2034 2e39 3537 3730  .1930243 4.95770
-00002970: 3535 2c39 2e34 3535 3530 3039 2034 2e39  55,9.4555009 4.9
-00002980: 3532 3031 3037 2c39 2e38 3734 3235 3735  520107,9.8742575
-00002990: 2035 2e31 3136 3536 3237 2c31 302e 3139   5.1165627,10.19
-000029a0: 3932 3333 2061 2031 2e30 3234 3630 3038  9233 a 1.0246008
-000029b0: 2c31 2e30 3234 3630 3038 2030 2030 2030  ,1.0246008 0 0 0
-000029c0: 2030 2e30 3036 3737 2c30 2e30 3133 3134   0.00677,0.01314
-000029d0: 2031 2e38 3437 3037 3232 2c31 2e38 3437   1.8470722,1.847
-000029e0: 3037 3232 2030 2030 2031 2030 2e30 3034  0722 0 0 1 0.004
-000029f0: 3938 2c30 2e30 3038 3620 6320 302e 3136  98,0.0086 c 0.16
-00002a00: 3635 3034 332c 302e 3238 3833 3934 2030  65043,0.288394 0
-00002a10: 2e30 3833 3630 342c 302e 3332 3439 3220  .083604,0.32492 
-00002a20: 2d30 2e31 3436 3935 3232 2c30 2e34 3633  -0.1469522,0.463
-00002a30: 3030 3120 2d30 2e32 3330 3535 3632 2c30  001 -0.2305562,0
-00002a40: 2e31 3338 3038 3120 2d30 2e36 3236 3035  .138081 -0.62605
-00002a50: 3131 2c30 2e31 3533 3232 3120 2d30 2e37  11,0.153221 -0.7
-00002a60: 3738 3839 3032 2c30 2e30 3634 3938 2030  788902,0.06498 0
-00002a70: 2c30 202d 332e 3631 652d 352c 2d32 2e31  ,0 -3.61e-5,-2.1
-00002a80: 652d 3520 2d33 2e36 3165 2d35 2c2d 322e  e-5 -3.61e-5,-2.
-00002a90: 3165 2d35 202d 302e 3336 3037 3230 392c  1e-5 -0.3607209,
-00002aa0: 2d30 2e31 3639 3530 3720 2d30 2e37 3133  -0.169507 -0.713
-00002ab0: 3135 352c 2d30 2e31 3031 3633 3120 2d30  155,-0.101631 -0
-00002ac0: 2e39 3632 3134 3831 2c30 2e31 3033 3133  .9621481,0.10313
-00002ad0: 3120 2d30 2e32 3538 3231 3933 2c30 2e32  1 -0.2582193,0.2
-00002ae0: 3431 3431 3620 2d30 2e34 3030 3738 3932  41416 -0.4007892
-00002af0: 2c30 2e35 3031 3534 3720 2d30 2e34 3835  ,0.501547 -0.485
-00002b00: 3838 3031 2c30 2e36 3630 3032 3520 2d30  8801,0.660025 -0
-00002b10: 2e35 3632 3933 3639 2c30 2e39 3332 3034  .5629369,0.93204
-00002b20: 3920 2d30 2e38 3130 3433 3239 2c31 2e32  9 -0.8104329,1.2
-00002b30: 3536 3435 3520 2d30 2e39 3234 3132 3335  56455 -0.9241235
-00002b40: 2c31 2e34 3435 3538 3620 2d30 2e31 3135  ,1.445586 -0.115
-00002b50: 3332 3235 2c30 2e31 3931 3834 3620 2d30  3225,0.191846 -0
-00002b60: 2e30 3333 3933 312c 302e 3233 3233 3136  .033931,0.232316
-00002b70: 202d 302e 3033 3339 3331 2c30 2e32 3332   -0.033931,0.232
-00002b80: 3331 3620 302c 3020 2d30 2e30 3039 3838  316 0,0 -0.00988
-00002b90: 2c30 2e31 3136 3937 3320 302e 3233 3335  ,0.116973 0.2335
-00002ba0: 3434 362c 302e 3036 3635 3820 302e 3234  446,0.06658 0.24
-00002bb0: 3139 3437 392c 2d30 2e30 3530 3039 2030  19479,-0.05009 0
-00002bc0: 2e37 3837 3936 3639 2c2d 302e 3239 3738  .7879669,-0.2978
-00002bd0: 3532 2031 2e34 3438 3033 312c 2d31 2e32  52 1.448031,-1.2
-00002be0: 3833 3637 3620 302e 3132 3330 3131 362c  83676 0.1230116,
-00002bf0: 2d30 2e31 3637 3934 3120 302e 3234 3134  -0.167941 0.2414
-00002c00: 3237 372c 2d30 2e33 3731 3733 3820 302e  277,-0.371738 0.
-00002c10: 3334 3535 3639 372c 2d30 2e34 3433 3637  3455697,-0.44367
-00002c20: 3220 2d30 2e30 3139 3032 332c 302e 3030  2 -0.019023,0.00
-00002c30: 3636 202d 302e 3030 3731 382c 2d30 2e30  66 -0.00718,-0.0
-00002c40: 3032 3620 2d30 2e30 3731 3033 312c 2d38  026 -0.071031,-8
-00002c50: 2e35 3265 2d34 2030 2c30 2034 2e36 652d  .52e-4 0,0 4.6e-
-00002c60: 362c 3265 2d36 2034 2e37 652d 362c 3265  6,2e-6 4.7e-6,2e
-00002c70: 2d36 2030 2e35 3435 3439 3234 2c30 2e33  -6 0.5454924,0.3
-00002c80: 3134 3934 3120 312e 3139 3038 3735 322c  14941 1.1908752,
-00002c90: 302e 3232 3734 3239 2031 2e36 3931 3331  0.227429 1.69131
-00002ca0: 3334 2c2d 302e 3037 3232 3920 4320 352e  34,-0.07229 C 5.
-00002cb0: 3934 3133 3235 322c 3131 2e31 3538 3039  9413252,11.15809
-00002cc0: 3220 362e 3237 3835 312c 3130 2e34 3238  2 6.27851,10.428
-00002cd0: 3436 3920 352e 3931 3431 3837 392c 392e  469 5.9141879,9.
-00002ce0: 3738 3232 3438 3120 352e 3834 3738 3034  7822481 5.847804
-00002cf0: 362c 392e 3635 3238 3637 3620 352e 3836  6,9.6528676 5.86
-00002d00: 3936 3435 322c 392e 3732 3939 3431 3520  96452,9.7299415 
-00002d10: 352e 3837 3638 3934 332c 392e 3731 3939  5.8768943,9.7199
-00002d20: 3032 3520 352e 3838 3433 3330 312c 392e  025 5.8843301,9.
-00002d30: 3730 3936 3034 3920 362e 3030 3437 3132  7096049 6.004712
-00002d40: 312c 392e 3631 3336 3335 3920 362e 3230  1,9.6136359 6.20
-00002d50: 3638 3635 392c 392e 3531 3632 3433 3720  68659,9.5162437 
-00002d60: 362e 3631 3131 3733 372c 392e 3332 3134  6.6111737,9.3214
-00002d70: 3539 3220 372e 3239 3630 3537 2c39 2e30  592 7.296057,9.0
-00002d80: 3839 3837 3332 2037 2e37 3330 3133 3139  898732 7.7301319
-00002d90: 2c38 2e34 3533 3233 3033 205a 220d 0a20  ,8.4532303 Z".. 
-00002da0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00002db0: 696c 6c3a 2366 6666 6666 663b 6669 6c6c  ill:#ffffff;fill
-00002dc0: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 7374  -rule:nonzero;st
-00002dd0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-00002de0: 2d77 6964 7468 3a31 7078 3b73 7472 6f6b  -width:1px;strok
-00002df0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00002e00: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00002e10: 6974 6572 3b73 7472 6f6b 652d 6f70 6163  iter;stroke-opac
-00002e20: 6974 793a 3122 202f 3e0d 0a20 2020 203c  ity:1" />..    <
-00002e30: 2f67 3e0d 0a20 203c 2f67 3e0d 0a3c 2f73  /g>..  </g>..</s
-00002e40: 7667 3e0d 0a                             vg>..
+00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
+00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
+00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
+00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
+00000070: 0a0a 3c73 7667 0a20 2020 786d 6c6e 733a  ..<svg.   xmlns:
+00000080: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
+00000090: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
+000000a0: 312e 312f 220a 2020 2078 6d6c 6e73 3a63  1.1/".   xmlns:c
+000000b0: 633d 2268 7474 703a 2f2f 6372 6561 7469  c="http://creati
+000000c0: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
+000000d0: 2322 0a20 2020 786d 6c6e 733a 7264 663d  #".   xmlns:rdf=
+000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+000000f0: 7267 2f31 3939 392f 3032 2f32 322d 7264  rg/1999/02/22-rd
+00000100: 662d 7379 6e74 6178 2d6e 7323 220a 2020  f-syntax-ns#".  
+00000110: 2078 6d6c 6e73 3a73 7667 3d22 6874 7470   xmlns:svg="http
+00000120: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000130: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
+00000140: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+00000150: 6f72 672f 3230 3030 2f73 7667 220a 2020  org/2000/svg".  
+00000160: 2078 6d6c 6e73 3a73 6f64 6970 6f64 693d   xmlns:sodipodi=
+00000170: 2268 7474 703a 2f2f 736f 6469 706f 6469  "http://sodipodi
+00000180: 2e73 6f75 7263 6566 6f72 6765 2e6e 6574  .sourceforge.net
+00000190: 2f44 5444 2f73 6f64 6970 6f64 692d 302e  /DTD/sodipodi-0.
+000001a0: 6474 6422 0a20 2020 786d 6c6e 733a 696e  dtd".   xmlns:in
+000001b0: 6b73 6361 7065 3d22 6874 7470 3a2f 2f77  kscape="http://w
+000001c0: 7777 2e69 6e6b 7363 6170 652e 6f72 672f  ww.inkscape.org/
+000001d0: 6e61 6d65 7370 6163 6573 2f69 6e6b 7363  namespaces/inksc
+000001e0: 6170 6522 0a20 2020 7769 6474 683d 2231  ape".   width="1
+000001f0: 3670 7822 0a20 2020 6865 6967 6874 3d22  6px".   height="
+00000200: 3136 7078 220a 2020 2076 6965 7742 6f78  16px".   viewBox
+00000210: 3d22 3020 3020 3136 2031 3622 0a20 2020  ="0 0 16 16".   
+00000220: 7665 7273 696f 6e3d 2231 2e31 220a 2020  version="1.1".  
+00000230: 2069 643d 2253 5647 526f 6f74 220a 2020   id="SVGRoot".  
+00000240: 2069 6e6b 7363 6170 653a 7665 7273 696f   inkscape:versio
+00000250: 6e3d 2230 2e39 322e 3520 2832 3036 3065  n="0.92.5 (2060e
+00000260: 6331 6639 662c 2032 3032 302d 3034 2d30  c1f9f, 2020-04-0
+00000270: 3829 220a 2020 2073 6f64 6970 6f64 693a  8)".   sodipodi:
+00000280: 646f 636e 616d 653d 2262 6f78 6a65 6c6c  docname="boxjell
+00000290: 792e 7376 6722 0a20 2020 696e 6b73 6361  y.svg".   inksca
+000002a0: 7065 3a6c 6162 656c 3d22 4261 636b 6772  pe:label="Backgr
+000002b0: 6f75 6e64 223e 0a20 203c 6465 6673 0a20  ound">.  <defs. 
+000002c0: 2020 2020 6964 3d22 6465 6673 3130 223e      id="defs10">
+000002d0: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
+000002e0: 6174 682d 6566 6665 6374 0a20 2020 2020  ath-effect.     
+000002f0: 2020 6566 6665 6374 3d22 7461 7065 725f    effect="taper_
+00000300: 7374 726f 6b65 220a 2020 2020 2020 2069  stroke".       i
+00000310: 643d 2270 6174 682d 6566 6665 6374 3533  d="path-effect53
+00000320: 3831 220a 2020 2020 2020 2069 735f 7669  81".       is_vi
+00000330: 7369 626c 653d 2274 7275 6522 0a20 2020  sible="true".   
+00000340: 2020 2020 7374 726f 6b65 5f77 6964 7468      stroke_width
+00000350: 3d22 302e 3922 0a20 2020 2020 2020 6174  ="0.9".       at
+00000360: 7461 6368 5f73 7461 7274 3d22 3165 2d30  tach_start="1e-0
+00000370: 3722 0a20 2020 2020 2020 656e 645f 6f66  7".       end_of
+00000380: 6673 6574 3d22 302e 3939 3939 3922 0a20  fset="0.99999". 
+00000390: 2020 2020 2020 736d 6f6f 7468 696e 673d        smoothing=
+000003a0: 2231 2e31 220a 2020 2020 2020 206a 6f69  "1.1".       joi
+000003b0: 6e74 7970 653d 2265 7874 7261 706f 6c61  ntype="extrapola
+000003c0: 7465 6422 0a20 2020 2020 2020 6d69 7465  ted".       mite
+000003d0: 725f 6c69 6d69 743d 2231 3030 2220 2f3e  r_limit="100" />
+000003e0: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
+000003f0: 6174 682d 6566 6665 6374 0a20 2020 2020  ath-effect.     
+00000400: 2020 6566 6665 6374 3d22 7461 7065 725f    effect="taper_
+00000410: 7374 726f 6b65 220a 2020 2020 2020 2069  stroke".       i
+00000420: 643d 2270 6174 682d 6566 6665 6374 3533  d="path-effect53
+00000430: 3831 2d33 220a 2020 2020 2020 2069 735f  81-3".       is_
+00000440: 7669 7369 626c 653d 2274 7275 6522 0a20  visible="true". 
+00000450: 2020 2020 2020 7374 726f 6b65 5f77 6964        stroke_wid
+00000460: 7468 3d22 302e 3922 0a20 2020 2020 2020  th="0.9".       
+00000470: 6174 7461 6368 5f73 7461 7274 3d22 3165  attach_start="1e
+00000480: 2d30 3722 0a20 2020 2020 2020 656e 645f  -07".       end_
+00000490: 6f66 6673 6574 3d22 312e 3432 3230 3039  offset="1.422009
+000004a0: 3422 0a20 2020 2020 2020 736d 6f6f 7468  4".       smooth
+000004b0: 696e 673d 2231 2e31 220a 2020 2020 2020  ing="1.1".      
+000004c0: 206a 6f69 6e74 7970 653d 2265 7874 7261   jointype="extra
+000004d0: 706f 6c61 7465 6422 0a20 2020 2020 2020  polated".       
+000004e0: 6d69 7465 725f 6c69 6d69 743d 2231 3030  miter_limit="100
+000004f0: 2220 2f3e 0a20 2020 203c 696e 6b73 6361  " />.    <inksca
+00000500: 7065 3a70 6174 682d 6566 6665 6374 0a20  pe:path-effect. 
+00000510: 2020 2020 2020 6566 6665 6374 3d22 7461        effect="ta
+00000520: 7065 725f 7374 726f 6b65 220a 2020 2020  per_stroke".    
+00000530: 2020 2069 643d 2270 6174 682d 6566 6665     id="path-effe
+00000540: 6374 3533 3831 2d33 2d37 220a 2020 2020  ct5381-3-7".    
+00000550: 2020 2069 735f 7669 7369 626c 653d 2274     is_visible="t
+00000560: 7275 6522 0a20 2020 2020 2020 7374 726f  rue".       stro
+00000570: 6b65 5f77 6964 7468 3d22 3122 0a20 2020  ke_width="1".   
+00000580: 2020 2020 6174 7461 6368 5f73 7461 7274      attach_start
+00000590: 3d22 3165 2d30 3722 0a20 2020 2020 2020  ="1e-07".       
+000005a0: 656e 645f 6f66 6673 6574 3d22 312e 3432  end_offset="1.42
+000005b0: 3230 3039 3422 0a20 2020 2020 2020 736d  20094".       sm
+000005c0: 6f6f 7468 696e 673d 2231 2e31 220a 2020  oothing="1.1".  
+000005d0: 2020 2020 206a 6f69 6e74 7970 653d 2265       jointype="e
+000005e0: 7874 7261 706f 6c61 7465 6422 0a20 2020  xtrapolated".   
+000005f0: 2020 2020 6d69 7465 725f 6c69 6d69 743d      miter_limit=
+00000600: 2231 3030 2220 2f3e 0a20 2020 203c 696e  "100" />.    <in
+00000610: 6b73 6361 7065 3a70 6174 682d 6566 6665  kscape:path-effe
+00000620: 6374 0a20 2020 2020 2020 6566 6665 6374  ct.       effect
+00000630: 3d22 7461 7065 725f 7374 726f 6b65 220a  ="taper_stroke".
+00000640: 2020 2020 2020 2069 643d 2270 6174 682d         id="path-
+00000650: 6566 6665 6374 3533 3831 2d32 220a 2020  effect5381-2".  
+00000660: 2020 2020 2069 735f 7669 7369 626c 653d       is_visible=
+00000670: 2274 7275 6522 0a20 2020 2020 2020 7374  "true".       st
+00000680: 726f 6b65 5f77 6964 7468 3d22 3122 0a20  roke_width="1". 
+00000690: 2020 2020 2020 6174 7461 6368 5f73 7461        attach_sta
+000006a0: 7274 3d22 3165 2d30 3722 0a20 2020 2020  rt="1e-07".     
+000006b0: 2020 656e 645f 6f66 6673 6574 3d22 302e    end_offset="0.
+000006c0: 3939 3939 3922 0a20 2020 2020 2020 736d  99999".       sm
+000006d0: 6f6f 7468 696e 673d 2231 2e31 220a 2020  oothing="1.1".  
+000006e0: 2020 2020 206a 6f69 6e74 7970 653d 2265       jointype="e
+000006f0: 7874 7261 706f 6c61 7465 6422 0a20 2020  xtrapolated".   
+00000700: 2020 2020 6d69 7465 725f 6c69 6d69 743d      miter_limit=
+00000710: 2231 3030 2220 2f3e 0a20 2020 203c 696e  "100" />.    <in
+00000720: 6b73 6361 7065 3a70 6174 682d 6566 6665  kscape:path-effe
+00000730: 6374 0a20 2020 2020 2020 6566 6665 6374  ct.       effect
+00000740: 3d22 7461 7065 725f 7374 726f 6b65 220a  ="taper_stroke".
+00000750: 2020 2020 2020 2069 643d 2270 6174 682d         id="path-
+00000760: 6566 6665 6374 3533 3831 2d33 2d31 220a  effect5381-3-1".
+00000770: 2020 2020 2020 2069 735f 7669 7369 626c         is_visibl
+00000780: 653d 2274 7275 6522 0a20 2020 2020 2020  e="true".       
+00000790: 7374 726f 6b65 5f77 6964 7468 3d22 302e  stroke_width="0.
+000007a0: 3922 0a20 2020 2020 2020 6174 7461 6368  9".       attach
+000007b0: 5f73 7461 7274 3d22 3165 2d30 3722 0a20  _start="1e-07". 
+000007c0: 2020 2020 2020 656e 645f 6f66 6673 6574        end_offset
+000007d0: 3d22 312e 3432 3230 3039 3422 0a20 2020  ="1.4220094".   
+000007e0: 2020 2020 736d 6f6f 7468 696e 673d 2231      smoothing="1
+000007f0: 2e31 220a 2020 2020 2020 206a 6f69 6e74  .1".       joint
+00000800: 7970 653d 2265 7874 7261 706f 6c61 7465  ype="extrapolate
+00000810: 6422 0a20 2020 2020 2020 6d69 7465 725f  d".       miter_
+00000820: 6c69 6d69 743d 2231 3030 2220 2f3e 0a20  limit="100" />. 
+00000830: 2020 203c 696e 6b73 6361 7065 3a70 6174     <inkscape:pat
+00000840: 682d 6566 6665 6374 0a20 2020 2020 2020  h-effect.       
+00000850: 6566 6665 6374 3d22 7461 7065 725f 7374  effect="taper_st
+00000860: 726f 6b65 220a 2020 2020 2020 2069 643d  roke".       id=
+00000870: 2270 6174 682d 6566 6665 6374 3533 3831  "path-effect5381
+00000880: 2d37 220a 2020 2020 2020 2069 735f 7669  -7".       is_vi
+00000890: 7369 626c 653d 2274 7275 6522 0a20 2020  sible="true".   
+000008a0: 2020 2020 7374 726f 6b65 5f77 6964 7468      stroke_width
+000008b0: 3d22 302e 3922 0a20 2020 2020 2020 6174  ="0.9".       at
+000008c0: 7461 6368 5f73 7461 7274 3d22 3165 2d30  tach_start="1e-0
+000008d0: 3722 0a20 2020 2020 2020 656e 645f 6f66  7".       end_of
+000008e0: 6673 6574 3d22 302e 3939 3939 3922 0a20  fset="0.99999". 
+000008f0: 2020 2020 2020 736d 6f6f 7468 696e 673d        smoothing=
+00000900: 2231 2e31 220a 2020 2020 2020 206a 6f69  "1.1".       joi
+00000910: 6e74 7970 653d 2265 7874 7261 706f 6c61  ntype="extrapola
+00000920: 7465 6422 0a20 2020 2020 2020 6d69 7465  ted".       mite
+00000930: 725f 6c69 6d69 743d 2231 3030 2220 2f3e  r_limit="100" />
+00000940: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
+00000950: 6174 682d 6566 6665 6374 0a20 2020 2020  ath-effect.     
+00000960: 2020 6566 6665 6374 3d22 7461 7065 725f    effect="taper_
+00000970: 7374 726f 6b65 220a 2020 2020 2020 2069  stroke".       i
+00000980: 643d 2270 6174 682d 6566 6665 6374 3533  d="path-effect53
+00000990: 3831 2d33 2d39 220a 2020 2020 2020 2069  81-3-9".       i
+000009a0: 735f 7669 7369 626c 653d 2274 7275 6522  s_visible="true"
+000009b0: 0a20 2020 2020 2020 7374 726f 6b65 5f77  .       stroke_w
+000009c0: 6964 7468 3d22 302e 3922 0a20 2020 2020  idth="0.9".     
+000009d0: 2020 6174 7461 6368 5f73 7461 7274 3d22    attach_start="
+000009e0: 3165 2d30 3722 0a20 2020 2020 2020 656e  1e-07".       en
+000009f0: 645f 6f66 6673 6574 3d22 312e 3432 3230  d_offset="1.4220
+00000a00: 3039 3422 0a20 2020 2020 2020 736d 6f6f  094".       smoo
+00000a10: 7468 696e 673d 2231 2e31 220a 2020 2020  thing="1.1".    
+00000a20: 2020 206a 6f69 6e74 7970 653d 2265 7874     jointype="ext
+00000a30: 7261 706f 6c61 7465 6422 0a20 2020 2020  rapolated".     
+00000a40: 2020 6d69 7465 725f 6c69 6d69 743d 2231    miter_limit="1
+00000a50: 3030 2220 2f3e 0a20 2020 203c 696e 6b73  00" />.    <inks
+00000a60: 6361 7065 3a70 6174 682d 6566 6665 6374  cape:path-effect
+00000a70: 0a20 2020 2020 2020 6566 6665 6374 3d22  .       effect="
+00000a80: 7461 7065 725f 7374 726f 6b65 220a 2020  taper_stroke".  
+00000a90: 2020 2020 2069 643d 2270 6174 682d 6566       id="path-ef
+00000aa0: 6665 6374 3533 3831 2d36 220a 2020 2020  fect5381-6".    
+00000ab0: 2020 2069 735f 7669 7369 626c 653d 2274     is_visible="t
+00000ac0: 7275 6522 0a20 2020 2020 2020 7374 726f  rue".       stro
+00000ad0: 6b65 5f77 6964 7468 3d22 302e 3922 0a20  ke_width="0.9". 
+00000ae0: 2020 2020 2020 6174 7461 6368 5f73 7461        attach_sta
+00000af0: 7274 3d22 3165 2d30 3722 0a20 2020 2020  rt="1e-07".     
+00000b00: 2020 656e 645f 6f66 6673 6574 3d22 302e    end_offset="0.
+00000b10: 3939 3939 3922 0a20 2020 2020 2020 736d  99999".       sm
+00000b20: 6f6f 7468 696e 673d 2231 2e31 220a 2020  oothing="1.1".  
+00000b30: 2020 2020 206a 6f69 6e74 7970 653d 2265       jointype="e
+00000b40: 7874 7261 706f 6c61 7465 6422 0a20 2020  xtrapolated".   
+00000b50: 2020 2020 6d69 7465 725f 6c69 6d69 743d      miter_limit=
+00000b60: 2231 3030 2220 2f3e 0a20 203c 2f64 6566  "100" />.  </def
+00000b70: 733e 0a20 203c 736f 6469 706f 6469 3a6e  s>.  <sodipodi:n
+00000b80: 616d 6564 7669 6577 0a20 2020 2020 6964  amedview.     id
+00000b90: 3d22 6261 7365 220a 2020 2020 2070 6167  ="base".     pag
+00000ba0: 6563 6f6c 6f72 3d22 2366 6666 6666 6622  ecolor="#ffffff"
+00000bb0: 0a20 2020 2020 626f 7264 6572 636f 6c6f  .     bordercolo
+00000bc0: 723d 2223 3636 3636 3636 220a 2020 2020  r="#666666".    
+00000bd0: 2062 6f72 6465 726f 7061 6369 7479 3d22   borderopacity="
+00000be0: 312e 3022 0a20 2020 2020 696e 6b73 6361  1.0".     inksca
+00000bf0: 7065 3a70 6167 656f 7061 6369 7479 3d22  pe:pageopacity="
+00000c00: 302e 3022 0a20 2020 2020 696e 6b73 6361  0.0".     inksca
+00000c10: 7065 3a70 6167 6573 6861 646f 773d 2232  pe:pageshadow="2
+00000c20: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000c30: 7a6f 6f6d 3d22 3435 2e32 3534 3833 3422  zoom="45.254834"
+00000c40: 0a20 2020 2020 696e 6b73 6361 7065 3a63  .     inkscape:c
+00000c50: 783d 2234 2e30 3830 3935 3537 220a 2020  x="4.0809557".  
+00000c60: 2020 2069 6e6b 7363 6170 653a 6379 3d22     inkscape:cy="
+00000c70: 382e 3539 3933 3538 220a 2020 2020 2069  8.599358".     i
+00000c80: 6e6b 7363 6170 653a 646f 6375 6d65 6e74  nkscape:document
+00000c90: 2d75 6e69 7473 3d22 7078 220a 2020 2020  -units="px".    
+00000ca0: 2069 6e6b 7363 6170 653a 6375 7272 656e   inkscape:curren
+00000cb0: 742d 6c61 7965 723d 226c 6179 6572 3122  t-layer="layer1"
+00000cc0: 0a20 2020 2020 7368 6f77 6772 6964 3d22  .     showgrid="
+00000cd0: 6661 6c73 6522 0a20 2020 2020 696e 6b73  false".     inks
+00000ce0: 6361 7065 3a77 696e 646f 772d 7769 6474  cape:window-widt
+00000cf0: 683d 2233 3434 3022 0a20 2020 2020 696e  h="3440".     in
+00000d00: 6b73 6361 7065 3a77 696e 646f 772d 6865  kscape:window-he
+00000d10: 6967 6874 3d22 3133 3231 220a 2020 2020  ight="1321".    
+00000d20: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+00000d30: 2d78 3d22 3022 0a20 2020 2020 696e 6b73  -x="0".     inks
+00000d40: 6361 7065 3a77 696e 646f 772d 793d 2232  cape:window-y="2
+00000d50: 3422 0a20 2020 2020 696e 6b73 6361 7065  4".     inkscape
+00000d60: 3a77 696e 646f 772d 6d61 7869 6d69 7a65  :window-maximize
+00000d70: 643d 2231 220a 2020 2020 2069 6e6b 7363  d="1".     inksc
+00000d80: 6170 653a 6772 6964 2d62 626f 783d 2274  ape:grid-bbox="t
+00000d90: 7275 6522 0a20 2020 2020 696e 6b73 6361  rue".     inksca
+00000da0: 7065 3a73 6e61 702d 6e6f 6465 733d 2274  pe:snap-nodes="t
+00000db0: 7275 6522 202f 3e0a 2020 3c6d 6574 6164  rue" />.  <metad
+00000dc0: 6174 610a 2020 2020 2069 643d 226d 6574  ata.     id="met
+00000dd0: 6164 6174 6131 3322 3e0a 2020 2020 3c72  adata13">.    <r
+00000de0: 6466 3a52 4446 3e0a 2020 2020 2020 3c63  df:RDF>.      <c
+00000df0: 633a 576f 726b 0a20 2020 2020 2020 2020  c:Work.         
+00000e00: 7264 663a 6162 6f75 743d 2222 3e0a 2020  rdf:about="">.  
+00000e10: 2020 2020 2020 3c64 633a 666f 726d 6174        <dc:format
+00000e20: 3e69 6d61 6765 2f73 7667 2b78 6d6c 3c2f  >image/svg+xml</
+00000e30: 6463 3a66 6f72 6d61 743e 0a20 2020 2020  dc:format>.     
+00000e40: 2020 203c 6463 3a74 7970 650a 2020 2020     <dc:type.    
+00000e50: 2020 2020 2020 2072 6466 3a72 6573 6f75         rdf:resou
+00000e60: 7263 653d 2268 7474 703a 2f2f 7075 726c  rce="http://purl
+00000e70: 2e6f 7267 2f64 632f 6463 6d69 7479 7065  .org/dc/dcmitype
+00000e80: 2f53 7469 6c6c 496d 6167 6522 202f 3e0a  /StillImage" />.
+00000e90: 2020 2020 2020 2020 3c64 633a 7469 746c          <dc:titl
+00000ea0: 6520 2f3e 0a20 2020 2020 203c 2f63 633a  e />.      </cc:
+00000eb0: 576f 726b 3e0a 2020 2020 3c2f 7264 663a  Work>.    </rdf:
+00000ec0: 5244 463e 0a20 203c 2f6d 6574 6164 6174  RDF>.  </metadat
+00000ed0: 613e 0a20 203c 656c 6c69 7073 650a 2020  a>.  <ellipse.  
+00000ee0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00000ef0: 3030 3434 6161 3b66 696c 6c2d 6f70 6163  0044aa;fill-opac
+00000f00: 6974 793a 313b 7374 726f 6b65 3a23 3030  ity:1;stroke:#00
+00000f10: 3333 3830 3b73 7472 6f6b 652d 7769 6474  3380;stroke-widt
+00000f20: 683a 312e 3031 3233 3531 3735 3b73 7472  h:1.01235175;str
+00000f30: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00000f40: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00000f50: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00000f60: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00000f70: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00000f80: 2020 6964 3d22 7061 7468 3832 3822 0a20    id="path828". 
+00000f90: 2020 2020 6378 3d22 3822 0a20 2020 2020      cx="8".     
+00000fa0: 6379 3d22 3822 0a20 2020 2020 7278 3d22  cy="8".     rx="
+00000fb0: 372e 3439 3338 3234 3522 0a20 2020 2020  7.4938245".     
+00000fc0: 7279 3d22 372e 3439 3338 3234 2220 2f3e  ry="7.493824" />
+00000fd0: 0a20 203c 670a 2020 2020 2069 6e6b 7363  .  <g.     inksc
+00000fe0: 6170 653a 6c61 6265 6c3d 224a 656c 6c79  ape:label="Jelly
+00000ff0: 220a 2020 2020 2069 643d 226c 6179 6572  ".     id="layer
+00001000: 3122 0a20 2020 2020 7374 796c 653d 2264  1".     style="d
+00001010: 6973 706c 6179 3a69 6e6c 696e 6522 0a20  isplay:inline". 
+00001020: 2020 2020 696e 6b73 6361 7065 3a67 726f      inkscape:gro
+00001030: 7570 6d6f 6465 3d22 6c61 7965 7222 3e0a  upmode="layer">.
+00001040: 2020 2020 3c67 0a20 2020 2020 2020 6964      <g.       id
+00001050: 3d22 6738 3431 220a 2020 2020 2020 2074  ="g841".       t
+00001060: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00001070: 2830 2e38 3834 3237 3135 332c 302c 302c  (0.88427153,0,0,
+00001080: 302e 3838 3432 3731 3533 2c30 2e32 3038  0.88427153,0.208
+00001090: 3135 3730 312c 302e 3734 3236 3739 3735  15701,0.74267975
+000010a0: 2922 3e0a 2020 2020 2020 3c70 6174 680a  )">.      <path.
+000010b0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+000010c0: 693a 6e6f 6465 7479 7065 733d 2273 7373  i:nodetypes="sss
+000010d0: 7373 7373 7373 220a 2020 2020 2020 2020  ssssss".        
+000010e0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+000010f0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+00001100: 220a 2020 2020 2020 2020 2069 643d 2272  ".         id="r
+00001110: 6563 7432 3035 220a 2020 2020 2020 2020  ect205".        
+00001120: 2064 3d22 6d20 3131 2e32 3135 3730 362c   d="m 11.215706,
+00001130: 312e 3931 3230 3036 3120 302e 3733 3434  1.9120061 0.7344
+00001140: 3537 2c30 2e33 3137 3133 3135 2063 2030  57,0.3171315 c 0
+00001150: 2e38 3133 3737 382c 302e 3335 3133 3832  .813778,0.351382
+00001160: 3220 312e 3939 3930 3432 2c31 2e33 3838  2 1.999042,1.388
+00001170: 3333 3031 2031 2e34 3937 3139 382c 322e  3301 1.497198,2.
+00001180: 3138 3532 3837 3120 4c20 3131 2e38 3431  1852871 L 11.841
+00001190: 3136 332c 362e 3936 3531 3631 3120 4320  163,6.9651611 C 
+000011a0: 3131 2e33 3339 3331 392c 372e 3736 3231  11.339319,7.7621
+000011b0: 3138 3320 3130 2e39 3336 3832 382c 382e  183 10.936828,8.
+000011c0: 3332 3730 3238 3620 392e 3537 3136 3732  3270286 9.571672
+000011d0: 382c 372e 3733 3735 3636 3820 4c20 382e  8,7.7375668 L 8.
+000011e0: 3833 3732 3136 362c 372e 3432 3034 3335  8372166,7.420435
+000011f0: 3320 4320 372e 3431 3438 3336 352c 362e  3 C 7.4148365,6.
+00001200: 3830 3632 3634 3520 372e 3730 3632 3430  8062645 7.706240
+00001210: 352c 362e 3130 3030 3237 3920 382e 3030  5,6.1000279 8.00
+00001220: 3133 3635 342c 352e 3230 3536 3632 3420  13654,5.2056624 
+00001230: 4c20 382e 3933 3735 3137 322c 322e 3336  L 8.9375172,2.36
+00001240: 3836 3837 3320 4320 392e 3233 3236 3431  86873 C 9.232641
+00001250: 392c 312e 3437 3433 3232 3420 3130 2e34  9,1.4743224 10.4
+00001260: 3031 3932 382c 312e 3536 3036 3233 3720  01928,1.5606237 
+00001270: 3131 2e32 3135 3730 362c 312e 3931 3230  11.215706,1.9120
+00001280: 3036 3120 5a22 0a20 2020 2020 2020 2020  061 Z".         
+00001290: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
+000012a0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+000012b0: 7374 726f 6b65 2d77 6964 7468 3a31 3b73  stroke-width:1;s
+000012c0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+000012d0: 7474 3b73 7472 6f6b 652d 6d69 7465 726c  tt;stroke-miterl
+000012e0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+000012f0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00001300: 6f6b 652d 6f70 6163 6974 793a 3122 202f  oke-opacity:1" /
+00001310: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+00001320: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00001330: 3d22 7472 616e 736c 6174 6528 302e 3431  ="translate(0.41
+00001340: 3230 3731 3631 2c2d 312e 3435 3732 3431  207161,-1.457241
+00001350: 3529 220a 2020 2020 2020 2020 2069 6e6b  5)".         ink
+00001360: 7363 6170 653a 6f72 6967 696e 616c 2d64  scape:original-d
+00001370: 3d22 4d20 372e 3335 3833 3239 392c 382e  ="M 7.3583299,8.
+00001380: 3139 3937 3238 3320 4320 362e 3639 3534  1997283 C 6.6954
+00001390: 3137 332c 392e 3137 3230 3030 3120 352e  173,9.1720001 5.
+000013a0: 3034 3332 3731 342c 392e 3035 3833 3434  0432714,9.058344
+000013b0: 3920 352e 3531 3830 3239 362c 392e 3939  9 5.5180296,9.99
+000013c0: 3539 3438 3720 362e 3035 3932 3331 2c31  59487 6.059231,1
+000013d0: 302e 3933 3333 3337 2034 2e36 3735 3830  0.933337 4.67580
+000013e0: 3733 2c31 312e 3534 3138 3233 2033 2e39  73,11.541823 3.9
+000013f0: 3737 3437 3537 2c31 312e 3133 3836 3431  774757,11.138641
+00001400: 2033 2e32 3938 3536 3431 2c31 302e 3734   3.2985641,10.74
+00001410: 3636 3731 2033 2e30 3838 3830 3535 2c31  6671 3.0888055,1
+00001420: 322e 3435 3537 3733 2031 2e37 3839 3836  2.455773 1.78986
+00001430: 342c 3133 2e31 3933 3637 220a 2020 2020  4,13.19367".    
+00001440: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
+00001450: 7468 2d65 6666 6563 743d 2223 7061 7468  th-effect="#path
+00001460: 2d65 6666 6563 7435 3338 3122 0a20 2020  -effect5381".   
+00001470: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00001480: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
+00001490: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+000014a0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+000014b0: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+000014c0: 2020 2069 643d 2270 6174 6834 3933 3522     id="path4935"
+000014d0: 0a20 2020 2020 2020 2020 643d 224d 2036  .         d="M 6
+000014e0: 2e39 3836 3532 3735 2c37 2e39 3436 3232  .9865275,7.94622
+000014f0: 3639 2043 2036 2e37 3537 3638 3937 2c38  69 C 6.7576897,8
+00001500: 2e32 3831 3835 3535 2036 2e32 3835 3034  .2818555 6.28504
+00001510: 3339 2c38 2e34 3739 3537 3737 2035 2e38  39,8.4795777 5.8
+00001520: 3136 3234 3032 2c38 2e37 3035 3433 3435  162402,8.7054345
+00001530: 2035 2e35 3831 3833 3834 2c38 2e38 3138   5.5818384,8.818
+00001540: 3336 3239 2035 2e33 3336 3736 392c 382e  3629 5.336769,8.
+00001550: 3933 3035 3437 3820 352e 3134 3732 3337  9305478 5.147237
+00001560: 332c 392e 3139 3330 3234 3320 342e 3935  3,9.1930243 4.95
+00001570: 3737 3035 352c 392e 3435 3535 3030 3920  77055,9.4555009 
+00001580: 342e 3935 3230 3130 372c 392e 3837 3432  4.9520107,9.8742
+00001590: 3537 3520 352e 3131 3635 3632 372c 3130  575 5.1165627,10
+000015a0: 2e31 3939 3233 3320 6120 312e 3032 3436  .199233 a 1.0246
+000015b0: 3030 382c 312e 3032 3436 3030 3820 3020  008,1.0246008 0 
+000015c0: 3020 3020 302e 3030 3637 372c 302e 3031  0 0 0.00677,0.01
+000015d0: 3331 3420 312e 3834 3730 3732 322c 312e  314 1.8470722,1.
+000015e0: 3834 3730 3732 3220 3020 3020 3120 302e  8470722 0 0 1 0.
+000015f0: 3030 3439 382c 302e 3030 3836 2063 2030  00498,0.0086 c 0
+00001600: 2e31 3636 3530 3433 2c30 2e32 3838 3339  .1665043,0.28839
+00001610: 3420 302e 3038 3336 3034 2c30 2e33 3234  4 0.083604,0.324
+00001620: 3932 202d 302e 3134 3639 3532 322c 302e  92 -0.1469522,0.
+00001630: 3436 3330 3031 202d 302e 3233 3035 3536  463001 -0.230556
+00001640: 322c 302e 3133 3830 3831 202d 302e 3632  2,0.138081 -0.62
+00001650: 3630 3531 312c 302e 3135 3332 3231 202d  60511,0.153221 -
+00001660: 302e 3737 3838 3930 322c 302e 3036 3439  0.7788902,0.0649
+00001670: 3820 302c 3020 2d33 2e36 3165 2d35 2c2d  8 0,0 -3.61e-5,-
+00001680: 322e 3165 2d35 202d 332e 3631 652d 352c  2.1e-5 -3.61e-5,
+00001690: 2d32 2e31 652d 3520 2d30 2e33 3630 3732  -2.1e-5 -0.36072
+000016a0: 3039 2c2d 302e 3136 3935 3037 202d 302e  09,-0.169507 -0.
+000016b0: 3731 3331 3535 2c2d 302e 3130 3136 3331  713155,-0.101631
+000016c0: 202d 302e 3936 3231 3438 312c 302e 3130   -0.9621481,0.10
+000016d0: 3331 3331 202d 302e 3235 3832 3139 332c  3131 -0.2582193,
+000016e0: 302e 3234 3134 3136 202d 302e 3430 3037  0.241416 -0.4007
+000016f0: 3839 322c 302e 3530 3135 3437 202d 302e  892,0.501547 -0.
+00001700: 3438 3538 3830 312c 302e 3636 3030 3235  4858801,0.660025
+00001710: 202d 302e 3536 3239 3336 392c 302e 3933   -0.5629369,0.93
+00001720: 3230 3439 202d 302e 3831 3034 3332 392c  2049 -0.8104329,
+00001730: 312e 3235 3634 3535 202d 302e 3932 3431  1.256455 -0.9241
+00001740: 3233 352c 312e 3434 3535 3836 202d 302e  235,1.445586 -0.
+00001750: 3131 3533 3232 352c 302e 3139 3138 3436  1153225,0.191846
+00001760: 202d 302e 3033 3339 3331 2c30 2e32 3332   -0.033931,0.232
+00001770: 3331 3620 2d30 2e30 3333 3933 312c 302e  316 -0.033931,0.
+00001780: 3233 3233 3136 2030 2c30 202d 302e 3030  232316 0,0 -0.00
+00001790: 3938 382c 302e 3131 3639 3733 2030 2e32  988,0.116973 0.2
+000017a0: 3333 3534 3436 2c30 2e30 3636 3538 2030  335446,0.06658 0
+000017b0: 2e32 3431 3934 3739 2c2d 302e 3035 3030  .2419479,-0.0500
+000017c0: 3920 302e 3738 3739 3636 392c 2d30 2e32  9 0.7879669,-0.2
+000017d0: 3937 3835 3220 312e 3434 3830 3331 2c2d  97852 1.448031,-
+000017e0: 312e 3238 3336 3736 2030 2e31 3233 3031  1.283676 0.12301
+000017f0: 3136 2c2d 302e 3136 3739 3431 2030 2e32  16,-0.167941 0.2
+00001800: 3431 3432 3737 2c2d 302e 3337 3137 3338  414277,-0.371738
+00001810: 2030 2e33 3435 3536 3937 2c2d 302e 3434   0.3455697,-0.44
+00001820: 3336 3732 202d 302e 3031 3930 3233 2c30  3672 -0.019023,0
+00001830: 2e30 3036 3620 2d30 2e30 3037 3138 2c2d  .0066 -0.00718,-
+00001840: 302e 3030 3236 202d 302e 3037 3130 3331  0.0026 -0.071031
+00001850: 2c2d 382e 3532 652d 3420 302c 3020 342e  ,-8.52e-4 0,0 4.
+00001860: 3665 2d36 2c32 652d 3620 342e 3765 2d36  6e-6,2e-6 4.7e-6
+00001870: 2c32 652d 3620 302e 3534 3534 3932 342c  ,2e-6 0.5454924,
+00001880: 302e 3331 3439 3431 2031 2e31 3930 3837  0.314941 1.19087
+00001890: 3532 2c30 2e32 3237 3432 3920 312e 3639  52,0.227429 1.69
+000018a0: 3133 3133 342c 2d30 2e30 3732 3239 2043  13134,-0.07229 C
+000018b0: 2035 2e39 3431 3332 3532 2c31 312e 3135   5.9413252,11.15
+000018c0: 3830 3932 2036 2e32 3738 3531 2c31 302e  8092 6.27851,10.
+000018d0: 3432 3834 3639 2035 2e39 3134 3138 3739  428469 5.9141879
+000018e0: 2c39 2e37 3832 3234 3831 2035 2e38 3437  ,9.7822481 5.847
+000018f0: 3830 3436 2c39 2e36 3532 3836 3736 2035  8046,9.6528676 5
+00001900: 2e38 3639 3634 3532 2c39 2e37 3239 3934  .8696452,9.72994
+00001910: 3135 2035 2e38 3736 3839 3433 2c39 2e37  15 5.8768943,9.7
+00001920: 3139 3930 3235 2035 2e38 3834 3333 3031  199025 5.8843301
+00001930: 2c39 2e37 3039 3630 3439 2036 2e30 3034  ,9.7096049 6.004
+00001940: 3731 3231 2c39 2e36 3133 3633 3539 2036  7121,9.6136359 6
+00001950: 2e32 3036 3836 3539 2c39 2e35 3136 3234  .2068659,9.51624
+00001960: 3337 2036 2e36 3131 3137 3337 2c39 2e33  37 6.6111737,9.3
+00001970: 3231 3435 3932 2037 2e32 3936 3035 372c  214592 7.296057,
+00001980: 392e 3038 3938 3733 3220 372e 3733 3031  9.0898732 7.7301
+00001990: 3331 392c 382e 3435 3332 3330 3320 5a22  319,8.4532303 Z"
+000019a0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000019b0: 2266 696c 6c3a 2366 6666 6666 663b 6669  "fill:#ffffff;fi
+000019c0: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+000019d0: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
+000019e0: 6b65 2d77 6964 7468 3a31 7078 3b73 7472  ke-width:1px;str
+000019f0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00001a00: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00001a10: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+00001a20: 6163 6974 793a 3122 202f 3e0a 2020 2020  acity:1" />.    
+00001a30: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00001a40: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00001a50: 736c 6174 6528 322e 3536 3435 3137 352c  slate(2.5645175,
+00001a60: 2d30 2e34 3630 3533 3733 3429 220a 2020  -0.46053734)".  
+00001a70: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00001a80: 6f72 6967 696e 616c 2d64 3d22 6d20 382e  original-d="m 8.
+00001a90: 3137 3539 3232 312c 382e 3033 3430 3030  1759221,8.034000
+00001aa0: 3120 6320 302c 312e 3236 3139 3036 3220  1 c 0,1.2619062 
+00001ab0: 302e 3335 3330 3830 382c 322e 3533 3737  0.3530808,2.5377
+00001ac0: 3137 3920 2d30 2e38 3533 3634 3832 2c32  179 -0.8536482,2
+00001ad0: 2e35 3337 3731 3739 202d 312e 3530 3635  .5377179 -1.5065
+00001ae0: 3834 2c30 202d 312e 3135 3831 3336 382c  84,0 -1.1581368,
+00001af0: 312e 3238 3830 3631 202d 302e 3636 3634  1.288061 -0.6664
+00001b00: 3138 2c32 2e31 3339 3734 3320 302e 3537  18,2.139743 0.57
+00001b10: 3439 3331 352c 312e 3035 3537 3033 202d  49315,1.055703 -
+00001b20: 302e 3431 3233 3630 382c 312e 3138 3939  0.4123608,1.1899
+00001b30: 3120 2d31 2e37 3131 3330 3233 2c31 2e39  1 -1.7113023,1.9
+00001b40: 3237 3830 3722 0a20 2020 2020 2020 2020  27807".         
+00001b50: 696e 6b73 6361 7065 3a70 6174 682d 6566  inkscape:path-ef
+00001b60: 6665 6374 3d22 2370 6174 682d 6566 6665  fect="#path-effe
+00001b70: 6374 3533 3831 2d33 220a 2020 2020 2020  ct5381-3".      
+00001b80: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+00001b90: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
+00001ba0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00001bb0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00001bc0: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
+00001bd0: 6964 3d22 7061 7468 3439 3335 2d36 220a  id="path4935-6".
+00001be0: 2020 2020 2020 2020 2064 3d22 6d20 372e           d="m 7.
+00001bf0: 3732 3539 3232 312c 382e 3033 3430 3030  7259221,8.034000
+00001c00: 3520 6320 302c 302e 3637 3239 3232 3920  5 c 0,0.6729229 
+00001c10: 302e 3037 3832 3835 2c31 2e33 3132 3034  0.078285,1.31204
+00001c20: 3636 2030 2e30 3239 3532 372c 312e 3638  66 0.029527,1.68
+00001c30: 3335 3038 3420 2d30 2e30 3438 3735 382c  35084 -0.048758,
+00001c40: 302e 3337 3134 3632 3120 302e 3031 3136  0.3714621 0.0116
+00001c50: 3033 2c30 2e34 3034 3230 3931 202d 302e  03,0.4042091 -0.
+00001c60: 3433 3331 3734 372c 302e 3430 3432 3039  4331747,0.404209
+00001c70: 3120 2d30 2e35 3039 3531 3931 2c30 202d  1 -0.5095191,0 -
+00001c80: 302e 3933 3030 3139 372c 302e 3133 3130  0.9300197,0.1310
+00001c90: 3439 202d 312e 3230 3730 3934 322c 302e  49 -1.2070942,0.
+00001ca0: 3431 3932 3133 202d 302e 3237 3730 3734  419213 -0.277074
+00001cb0: 352c 302e 3238 3831 3634 202d 302e 3335  5,0.288164 -0.35
+00001cc0: 3032 3934 372c 302e 3637 3737 3435 202d  02947,0.677745 -
+00001cd0: 302e 3332 3534 3837 382c 312e 3032 3131  0.3254878,1.0211
+00001ce0: 3535 2030 2e30 3439 3837 2c30 2e35 3730  55 0.04987,0.570
+00001cf0: 3731 3220 302e 3238 3036 3530 342c 312e  712 0.2806504,1.
+00001d00: 3033 3834 3833 2030 2e34 3834 3831 3735  038483 0.4848175
+00001d10: 2c31 2e33 3633 3235 3620 302e 3135 3635  ,1.363256 0.1565
+00001d20: 3333 382c 302e 3235 3531 3035 2030 2e31  338,0.255105 0.1
+00001d30: 3232 3437 3439 2c30 2e35 3031 3138 3920  224749,0.501189 
+00001d40: 2d30 2e30 3037 3932 2c30 2e35 3539 3932  -0.00792,0.55992
+00001d50: 3120 2d30 2e36 3339 3838 362c 302e 3538  1 -0.639886,0.58
+00001d60: 3238 3735 202d 312e 3134 3030 3739 312c  2875 -1.1400791,
+00001d70: 302e 3739 3332 3132 202d 312e 3237 3236  0.793212 -1.2726
+00001d80: 3631 342c 302e 3935 3731 3732 202d 302e  614,0.957172 -0.
+00001d90: 3133 3230 3335 372c 302e 3136 3332 3834  1320357,0.163284
+00001da0: 202d 302e 3034 3036 3034 2c30 2e31 3931   -0.040604,0.191
+00001db0: 3836 3620 2d30 2e30 3430 3630 342c 302e  866 -0.040604,0.
+00001dc0: 3139 3138 3636 2030 2c30 202d 302e 3032  191866 0,0 -0.02
+00001dd0: 3133 3435 2c30 2e30 3834 3731 2030 2e31  1345,0.08471 0.1
+00001de0: 3830 3532 3733 2c30 2e30 3730 3538 202d  805273,0.07058 -
+00001df0: 302e 3031 3433 3537 2c30 2e30 3031 2030  0.014357,0.001 0
+00001e00: 2e38 3338 3130 3639 2c2d 302e 3038 3937  .8381069,-0.0897
+00001e10: 2031 2e36 3035 3338 3235 2c2d 302e 3630   1.6053825,-0.60
+00001e20: 3130 3633 2030 2e33 3839 3334 3631 2c2d  1063 0.3893461,-
+00001e30: 302e 3334 3030 3737 2030 2e36 3236 3435  0.340077 0.62645
+00001e40: 3831 2c2d 302e 3937 3236 3239 2030 2e32  81,-0.972629 0.2
+00001e50: 3937 3937 3332 2c2d 312e 3630 3632 3431  979732,-1.606241
+00001e60: 202d 302e 3135 3230 3737 372c 2d30 2e32   -0.1520777,-0.2
+00001e70: 3931 3935 3820 2d30 2e33 3333 3739 3032  91958 -0.3337902
+00001e80: 2c2d 302e 3636 3039 3232 202d 302e 3334  ,-0.660922 -0.34
+00001e90: 3938 3439 352c 2d31 2e30 3030 3333 3920  98495,-1.000339 
+00001ea0: 2d30 2e30 3133 3330 382c 2d30 2e31 3834  -0.013308,-0.184
+00001eb0: 3232 3920 302e 3031 3939 3532 2c2d 302e  229 0.019952,-0.
+00001ec0: 3237 3336 3231 2030 2e30 3736 3538 342c  273621 0.076584,
+00001ed0: 2d30 2e33 3332 3532 2030 2e30 3536 3633  -0.33252 0.05663
+00001ee0: 322c 2d30 2e30 3538 3920 302e 3139 3730  2,-0.0589 0.1970
+00001ef0: 3634 392c 2d30 2e31 3433 3030 3320 302e  649,-0.143003 0.
+00001f00: 3535 3833 3337 322c 2d30 2e31 3433 3030  5583372,-0.14300
+00001f10: 3320 302e 3736 3139 3531 362c 3020 312e  3 0.7619516,0 1.
+00001f20: 3234 3931 3336 382c 2d30 2e36 3035 3135  2491368,-0.60515
+00001f30: 3920 312e 3332 3535 3230 322c 2d31 2e31  9 1.3255202,-1.1
+00001f40: 3837 3037 3839 2030 2e30 3736 3338 342c  870789 0.076384,
+00001f50: 2d30 2e35 3831 3932 3034 202d 302e 3032  -0.5819204 -0.02
+00001f60: 3138 3732 2c2d 312e 3231 3136 3535 3520  1872,-1.2116555 
+00001f70: 2d30 2e30 3231 3837 322c 2d31 2e38 3030  -0.021872,-1.800
+00001f80: 3633 3836 207a 220a 2020 2020 2020 2020  6386 z".        
+00001f90: 2073 7479 6c65 3d22 6669 6c6c 3a23 6666   style="fill:#ff
+00001fa0: 6666 6666 3b66 696c 6c2d 7275 6c65 3a6e  ffff;fill-rule:n
+00001fb0: 6f6e 7a65 726f 3b73 7472 6f6b 653a 6e6f  onzero;stroke:no
+00001fc0: 6e65 3b73 7472 6f6b 652d 7769 6474 683a  ne;stroke-width:
+00001fd0: 3170 783b 7374 726f 6b65 2d6c 696e 6563  1px;stroke-linec
+00001fe0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+00001ff0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00002000: 726f 6b65 2d6f 7061 6369 7479 3a31 2220  roke-opacity:1" 
+00002010: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+00002020: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+00002030: 6d3d 226d 6174 7269 7828 302e 3734 3533  m="matrix(0.7453
+00002040: 3433 3931 2c2d 302e 3130 3037 3430 372c  4391,-0.1007407,
+00002050: 302e 3130 3037 3430 372c 302e 3734 3533  0.1007407,0.7453
+00002060: 3433 3931 2c31 2e31 3639 3630 3139 2c31  4391,1.1696019,1
+00002070: 2e35 3830 3434 3436 2922 0a20 2020 2020  .5804446)".     
+00002080: 2020 2020 696e 6b73 6361 7065 3a6f 7269      inkscape:ori
+00002090: 6769 6e61 6c2d 643d 226d 2038 2e31 3735  ginal-d="m 8.175
+000020a0: 3932 3231 2c38 2e30 3334 3030 3031 2063  9221,8.0340001 c
+000020b0: 2030 2c31 2e32 3631 3930 3632 2030 2e33   0,1.2619062 0.3
+000020c0: 3533 3038 3038 2c32 2e35 3337 3731 3739  530808,2.5377179
+000020d0: 202d 302e 3835 3336 3438 322c 322e 3533   -0.8536482,2.53
+000020e0: 3737 3137 3920 2d31 2e35 3036 3538 342c  77179 -1.506584,
+000020f0: 3020 2d31 2e31 3538 3133 3638 2c31 2e32  0 -1.1581368,1.2
+00002100: 3838 3036 3120 2d30 2e36 3636 3431 382c  88061 -0.666418,
+00002110: 322e 3133 3937 3433 2030 2e35 3734 3933  2.139743 0.57493
+00002120: 3135 2c31 2e30 3535 3730 3320 2d30 2e34  15,1.055703 -0.4
+00002130: 3132 3336 3038 2c31 2e31 3839 3931 202d  123608,1.18991 -
+00002140: 312e 3731 3133 3032 332c 312e 3932 3738  1.7113023,1.9278
+00002150: 3037 220a 2020 2020 2020 2020 2069 6e6b  07".         ink
+00002160: 7363 6170 653a 7061 7468 2d65 6666 6563  scape:path-effec
+00002170: 743d 2223 7061 7468 2d65 6666 6563 7435  t="#path-effect5
+00002180: 3338 312d 332d 3922 0a20 2020 2020 2020  381-3-9".       
+00002190: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+000021a0: 7970 6573 3d22 6363 6363 220a 2020 2020  ypes="cccc".    
+000021b0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+000021c0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+000021d0: 653d 2230 220a 2020 2020 2020 2020 2069  e="0".         i
+000021e0: 643d 2270 6174 6834 3933 352d 362d 3322  d="path4935-6-3"
+000021f0: 0a20 2020 2020 2020 2020 643d 226d 2037  .         d="m 7
+00002200: 2e37 3235 3932 3231 2c38 2e30 3334 3030  .7259221,8.03400
+00002210: 3035 2063 2030 2c30 2e36 3732 3932 3239  05 c 0,0.6729229
+00002220: 2030 2e30 3738 3238 352c 312e 3331 3230   0.078285,1.3120
+00002230: 3436 3620 302e 3032 3935 3237 2c31 2e36  466 0.029527,1.6
+00002240: 3833 3530 3834 202d 302e 3034 3837 3538  835084 -0.048758
+00002250: 2c30 2e33 3731 3436 3231 2030 2e30 3131  ,0.3714621 0.011
+00002260: 3630 332c 302e 3430 3432 3039 3120 2d30  603,0.4042091 -0
+00002270: 2e34 3333 3137 3437 2c30 2e34 3034 3230  .4331747,0.40420
+00002280: 3931 202d 302e 3530 3935 3139 312c 3020  91 -0.5095191,0 
+00002290: 2d30 2e39 3330 3031 3937 2c30 2e31 3331  -0.9300197,0.131
+000022a0: 3034 3920 2d31 2e32 3037 3039 3432 2c30  049 -1.2070942,0
+000022b0: 2e34 3139 3231 3320 2d30 2e32 3737 3037  .419213 -0.27707
+000022c0: 3435 2c30 2e32 3838 3136 3420 2d30 2e33  45,0.288164 -0.3
+000022d0: 3530 3239 3437 2c30 2e36 3737 3734 3520  502947,0.677745 
+000022e0: 2d30 2e33 3235 3438 3738 2c31 2e30 3231  -0.3254878,1.021
+000022f0: 3135 3520 302e 3034 3938 372c 302e 3537  155 0.04987,0.57
+00002300: 3037 3132 2030 2e32 3830 3635 3034 2c31  0712 0.2806504,1
+00002310: 2e30 3338 3438 3320 302e 3438 3438 3137  .038483 0.484817
+00002320: 352c 312e 3336 3332 3536 2030 2e31 3536  5,1.363256 0.156
+00002330: 3533 3338 2c30 2e32 3535 3130 3520 302e  5338,0.255105 0.
+00002340: 3132 3234 3734 392c 302e 3530 3131 3839  1224749,0.501189
+00002350: 202d 302e 3030 3739 322c 302e 3535 3939   -0.00792,0.5599
+00002360: 3231 202d 302e 3633 3938 3836 2c30 2e35  21 -0.639886,0.5
+00002370: 3832 3837 3520 2d31 2e31 3430 3037 3931  82875 -1.1400791
+00002380: 2c30 2e37 3933 3231 3220 2d31 2e32 3732  ,0.793212 -1.272
+00002390: 3636 3134 2c30 2e39 3537 3137 3220 2d30  6614,0.957172 -0
+000023a0: 2e31 3332 3033 3537 2c30 2e31 3633 3238  .1320357,0.16328
+000023b0: 3420 2d30 2e30 3430 3630 342c 302e 3139  4 -0.040604,0.19
+000023c0: 3138 3636 202d 302e 3034 3036 3034 2c30  1866 -0.040604,0
+000023d0: 2e31 3931 3836 3620 302c 3020 2d30 2e30  .191866 0,0 -0.0
+000023e0: 3231 3334 352c 302e 3038 3437 3120 302e  21345,0.08471 0.
+000023f0: 3138 3035 3237 332c 302e 3037 3035 3820  1805273,0.07058 
+00002400: 2d30 2e30 3134 3335 372c 302e 3030 3120  -0.014357,0.001 
+00002410: 302e 3833 3831 3036 392c 2d30 2e30 3839  0.8381069,-0.089
+00002420: 3720 312e 3630 3533 3832 352c 2d30 2e36  7 1.6053825,-0.6
+00002430: 3031 3036 3320 302e 3338 3933 3436 312c  01063 0.3893461,
+00002440: 2d30 2e33 3430 3037 3720 302e 3632 3634  -0.340077 0.6264
+00002450: 3538 312c 2d30 2e39 3732 3632 3920 302e  581,-0.972629 0.
+00002460: 3239 3739 3733 322c 2d31 2e36 3036 3234  2979732,-1.60624
+00002470: 3120 2d30 2e31 3532 3037 3737 2c2d 302e  1 -0.1520777,-0.
+00002480: 3239 3139 3538 202d 302e 3333 3337 3930  291958 -0.333790
+00002490: 322c 2d30 2e36 3630 3932 3220 2d30 2e33  2,-0.660922 -0.3
+000024a0: 3439 3834 3935 2c2d 312e 3030 3033 3339  498495,-1.000339
+000024b0: 202d 302e 3031 3333 3038 2c2d 302e 3138   -0.013308,-0.18
+000024c0: 3432 3239 2030 2e30 3139 3935 322c 2d30  4229 0.019952,-0
+000024d0: 2e32 3733 3632 3120 302e 3037 3635 3834  .273621 0.076584
+000024e0: 2c2d 302e 3333 3235 3220 302e 3035 3636  ,-0.33252 0.0566
+000024f0: 3332 2c2d 302e 3035 3839 2030 2e31 3937  32,-0.0589 0.197
+00002500: 3036 3439 2c2d 302e 3134 3330 3033 2030  0649,-0.143003 0
+00002510: 2e35 3538 3333 3732 2c2d 302e 3134 3330  .5583372,-0.1430
+00002520: 3033 2030 2e37 3631 3935 3136 2c30 2031  03 0.7619516,0 1
+00002530: 2e32 3439 3133 3638 2c2d 302e 3630 3531  .2491368,-0.6051
+00002540: 3539 2031 2e33 3235 3532 3032 2c2d 312e  59 1.3255202,-1.
+00002550: 3138 3730 3738 3920 302e 3037 3633 3834  1870789 0.076384
+00002560: 2c2d 302e 3538 3139 3230 3420 2d30 2e30  ,-0.5819204 -0.0
+00002570: 3231 3837 322c 2d31 2e32 3131 3635 3535  21872,-1.2116555
+00002580: 202d 302e 3032 3138 3732 2c2d 312e 3830   -0.021872,-1.80
+00002590: 3036 3338 3620 7a22 0a20 2020 2020 2020  06386 z".       
+000025a0: 2020 7374 796c 653d 2266 696c 6c3a 2366    style="fill:#f
+000025b0: 6666 6666 663b 6669 6c6c 2d72 756c 653a  fffff;fill-rule:
+000025c0: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
+000025d0: 6f6e 653b 7374 726f 6b65 2d77 6964 7468  one;stroke-width
+000025e0: 3a31 7078 3b73 7472 6f6b 652d 6c69 6e65  :1px;stroke-line
+000025f0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00002600: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00002610: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00002620: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00002630: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
+00002640: 726d 3d22 6d61 7472 6978 282d 302e 3732  rm="matrix(-0.72
+00002650: 3834 3236 3239 2c2d 302e 3438 3334 3038  842629,-0.483408
+00002660: 3631 2c2d 302e 3438 3931 3232 3834 2c30  61,-0.48912284,0
+00002670: 2e37 3139 3931 3633 372c 3230 2e37 3933  .71991637,20.793
+00002680: 3332 342c 352e 3533 3236 3739 3229 220a  324,5.5326792)".
+00002690: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+000026a0: 653a 6f72 6967 696e 616c 2d64 3d22 4d20  e:original-d="M 
+000026b0: 372e 3335 3833 3239 392c 382e 3139 3937  7.3583299,8.1997
+000026c0: 3238 3320 4320 362e 3639 3534 3137 332c  283 C 6.6954173,
+000026d0: 392e 3137 3230 3030 3120 352e 3034 3332  9.1720001 5.0432
+000026e0: 3731 342c 392e 3035 3833 3434 3920 352e  714,9.0583449 5.
+000026f0: 3531 3830 3239 362c 392e 3939 3539 3438  5180296,9.995948
+00002700: 3720 362e 3035 3932 3331 2c31 302e 3933  7 6.059231,10.93
+00002710: 3333 3337 2034 2e36 3735 3830 3733 2c31  3337 4.6758073,1
+00002720: 312e 3534 3138 3233 2033 2e39 3737 3437  1.541823 3.97747
+00002730: 3537 2c31 312e 3133 3836 3431 2033 2e32  57,11.138641 3.2
+00002740: 3938 3536 3431 2c31 302e 3734 3636 3731  985641,10.746671
+00002750: 2033 2e30 3838 3830 3535 2c31 322e 3435   3.0888055,12.45
+00002760: 3537 3733 2031 2e37 3839 3836 342c 3133  5773 1.789864,13
+00002770: 2e31 3933 3637 220a 2020 2020 2020 2020  .19367".        
+00002780: 2069 6e6b 7363 6170 653a 7061 7468 2d65   inkscape:path-e
+00002790: 6666 6563 743d 2223 7061 7468 2d65 6666  ffect="#path-eff
+000027a0: 6563 7435 3338 312d 3622 0a20 2020 2020  ect5381-6".     
+000027b0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+000027c0: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
+000027d0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000027e0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+000027f0: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+00002800: 2069 643d 2270 6174 6834 3933 352d 3022   id="path4935-0"
+00002810: 0a20 2020 2020 2020 2020 643d 224d 2036  .         d="M 6
+00002820: 2e39 3836 3532 3735 2c37 2e39 3436 3232  .9865275,7.94622
+00002830: 3639 2043 2036 2e37 3537 3638 3937 2c38  69 C 6.7576897,8
+00002840: 2e32 3831 3835 3535 2036 2e32 3835 3034  .2818555 6.28504
+00002850: 3339 2c38 2e34 3739 3537 3737 2035 2e38  39,8.4795777 5.8
+00002860: 3136 3234 3032 2c38 2e37 3035 3433 3435  162402,8.7054345
+00002870: 2035 2e35 3831 3833 3834 2c38 2e38 3138   5.5818384,8.818
+00002880: 3336 3239 2035 2e33 3336 3736 392c 382e  3629 5.336769,8.
+00002890: 3933 3035 3437 3820 352e 3134 3732 3337  9305478 5.147237
+000028a0: 332c 392e 3139 3330 3234 3320 342e 3935  3,9.1930243 4.95
+000028b0: 3737 3035 352c 392e 3435 3535 3030 3920  77055,9.4555009 
+000028c0: 342e 3935 3230 3130 372c 392e 3837 3432  4.9520107,9.8742
+000028d0: 3537 3520 352e 3131 3635 3632 372c 3130  575 5.1165627,10
+000028e0: 2e31 3939 3233 3320 6120 312e 3032 3436  .199233 a 1.0246
+000028f0: 3030 382c 312e 3032 3436 3030 3820 3020  008,1.0246008 0 
+00002900: 3020 3020 302e 3030 3637 372c 302e 3031  0 0 0.00677,0.01
+00002910: 3331 3420 312e 3834 3730 3732 322c 312e  314 1.8470722,1.
+00002920: 3834 3730 3732 3220 3020 3020 3120 302e  8470722 0 0 1 0.
+00002930: 3030 3439 382c 302e 3030 3836 2063 2030  00498,0.0086 c 0
+00002940: 2e31 3636 3530 3433 2c30 2e32 3838 3339  .1665043,0.28839
+00002950: 3420 302e 3038 3336 3034 2c30 2e33 3234  4 0.083604,0.324
+00002960: 3932 202d 302e 3134 3639 3532 322c 302e  92 -0.1469522,0.
+00002970: 3436 3330 3031 202d 302e 3233 3035 3536  463001 -0.230556
+00002980: 322c 302e 3133 3830 3831 202d 302e 3632  2,0.138081 -0.62
+00002990: 3630 3531 312c 302e 3135 3332 3231 202d  60511,0.153221 -
+000029a0: 302e 3737 3838 3930 322c 302e 3036 3439  0.7788902,0.0649
+000029b0: 3820 302c 3020 2d33 2e36 3165 2d35 2c2d  8 0,0 -3.61e-5,-
+000029c0: 322e 3165 2d35 202d 332e 3631 652d 352c  2.1e-5 -3.61e-5,
+000029d0: 2d32 2e31 652d 3520 2d30 2e33 3630 3732  -2.1e-5 -0.36072
+000029e0: 3039 2c2d 302e 3136 3935 3037 202d 302e  09,-0.169507 -0.
+000029f0: 3731 3331 3535 2c2d 302e 3130 3136 3331  713155,-0.101631
+00002a00: 202d 302e 3936 3231 3438 312c 302e 3130   -0.9621481,0.10
+00002a10: 3331 3331 202d 302e 3235 3832 3139 332c  3131 -0.2582193,
+00002a20: 302e 3234 3134 3136 202d 302e 3430 3037  0.241416 -0.4007
+00002a30: 3839 322c 302e 3530 3135 3437 202d 302e  892,0.501547 -0.
+00002a40: 3438 3538 3830 312c 302e 3636 3030 3235  4858801,0.660025
+00002a50: 202d 302e 3536 3239 3336 392c 302e 3933   -0.5629369,0.93
+00002a60: 3230 3439 202d 302e 3831 3034 3332 392c  2049 -0.8104329,
+00002a70: 312e 3235 3634 3535 202d 302e 3932 3431  1.256455 -0.9241
+00002a80: 3233 352c 312e 3434 3535 3836 202d 302e  235,1.445586 -0.
+00002a90: 3131 3533 3232 352c 302e 3139 3138 3436  1153225,0.191846
+00002aa0: 202d 302e 3033 3339 3331 2c30 2e32 3332   -0.033931,0.232
+00002ab0: 3331 3620 2d30 2e30 3333 3933 312c 302e  316 -0.033931,0.
+00002ac0: 3233 3233 3136 2030 2c30 202d 302e 3030  232316 0,0 -0.00
+00002ad0: 3938 382c 302e 3131 3639 3733 2030 2e32  988,0.116973 0.2
+00002ae0: 3333 3534 3436 2c30 2e30 3636 3538 2030  335446,0.06658 0
+00002af0: 2e32 3431 3934 3739 2c2d 302e 3035 3030  .2419479,-0.0500
+00002b00: 3920 302e 3738 3739 3636 392c 2d30 2e32  9 0.7879669,-0.2
+00002b10: 3937 3835 3220 312e 3434 3830 3331 2c2d  97852 1.448031,-
+00002b20: 312e 3238 3336 3736 2030 2e31 3233 3031  1.283676 0.12301
+00002b30: 3136 2c2d 302e 3136 3739 3431 2030 2e32  16,-0.167941 0.2
+00002b40: 3431 3432 3737 2c2d 302e 3337 3137 3338  414277,-0.371738
+00002b50: 2030 2e33 3435 3536 3937 2c2d 302e 3434   0.3455697,-0.44
+00002b60: 3336 3732 202d 302e 3031 3930 3233 2c30  3672 -0.019023,0
+00002b70: 2e30 3036 3620 2d30 2e30 3037 3138 2c2d  .0066 -0.00718,-
+00002b80: 302e 3030 3236 202d 302e 3037 3130 3331  0.0026 -0.071031
+00002b90: 2c2d 382e 3532 652d 3420 302c 3020 342e  ,-8.52e-4 0,0 4.
+00002ba0: 3665 2d36 2c32 652d 3620 342e 3765 2d36  6e-6,2e-6 4.7e-6
+00002bb0: 2c32 652d 3620 302e 3534 3534 3932 342c  ,2e-6 0.5454924,
+00002bc0: 302e 3331 3439 3431 2031 2e31 3930 3837  0.314941 1.19087
+00002bd0: 3532 2c30 2e32 3237 3432 3920 312e 3639  52,0.227429 1.69
+00002be0: 3133 3133 342c 2d30 2e30 3732 3239 2043  13134,-0.07229 C
+00002bf0: 2035 2e39 3431 3332 3532 2c31 312e 3135   5.9413252,11.15
+00002c00: 3830 3932 2036 2e32 3738 3531 2c31 302e  8092 6.27851,10.
+00002c10: 3432 3834 3639 2035 2e39 3134 3138 3739  428469 5.9141879
+00002c20: 2c39 2e37 3832 3234 3831 2035 2e38 3437  ,9.7822481 5.847
+00002c30: 3830 3436 2c39 2e36 3532 3836 3736 2035  8046,9.6528676 5
+00002c40: 2e38 3639 3634 3532 2c39 2e37 3239 3934  .8696452,9.72994
+00002c50: 3135 2035 2e38 3736 3839 3433 2c39 2e37  15 5.8768943,9.7
+00002c60: 3139 3930 3235 2035 2e38 3834 3333 3031  199025 5.8843301
+00002c70: 2c39 2e37 3039 3630 3439 2036 2e30 3034  ,9.7096049 6.004
+00002c80: 3731 3231 2c39 2e36 3133 3633 3539 2036  7121,9.6136359 6
+00002c90: 2e32 3036 3836 3539 2c39 2e35 3136 3234  .2068659,9.51624
+00002ca0: 3337 2036 2e36 3131 3137 3337 2c39 2e33  37 6.6111737,9.3
+00002cb0: 3231 3435 3932 2037 2e32 3936 3035 372c  214592 7.296057,
+00002cc0: 392e 3038 3938 3733 3220 372e 3733 3031  9.0898732 7.7301
+00002cd0: 3331 392c 382e 3435 3332 3330 3320 5a22  319,8.4532303 Z"
+00002ce0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00002cf0: 2266 696c 6c3a 2366 6666 6666 663b 6669  "fill:#ffffff;fi
+00002d00: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00002d10: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
+00002d20: 6b65 2d77 6964 7468 3a31 7078 3b73 7472  ke-width:1px;str
+00002d30: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00002d40: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00002d50: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+00002d60: 6163 6974 793a 3122 202f 3e0a 2020 2020  acity:1" />.    
+00002d70: 3c2f 673e 0a20 203c 2f67 3e0a 3c2f 7376  </g>.  </g>.</sv
+00002d80: 673e 0a                                  g>.
```

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/delete.png` & `boxjelly-0.3.3/boxjelly/assets/icons/delete.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/merge.png` & `boxjelly-0.3.3/boxjelly/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/redo.png` & `boxjelly-0.3.3/boxjelly/assets/icons/redo.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/rename.png` & `boxjelly-0.3.3/boxjelly/assets/icons/rename.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/split.png` & `boxjelly-0.3.3/boxjelly/assets/icons/split.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/icons/undo.png` & `boxjelly-0.3.3/boxjelly/assets/icons/undo.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_1024.png` & `boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_1024.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_128.png` & `boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_128.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_256.png` & `boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_256.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/assets/images/boxjelly_logo_512.png` & `boxjelly-0.3.3/boxjelly/assets/images/boxjelly_logo_512.png`

 * *Files identical despite different names*

### Comparing `boxjelly-0.3.2/boxjelly/delegates/TrackHeadersDelegate.py` & `boxjelly-0.3.3/boxjelly/delegates/TrackHeadersDelegate.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from PyQt6 import QtWidgets, QtCore, QtGui
-
-from boxjelly.models.TrackListModel import TrackListModel
-
-
-class TrackHeadersDelegate(QtWidgets.QStyledItemDelegate):
-    
-    def paint(self, painter: QtGui.QPainter, opt: QtWidgets.QStyleOptionViewItem, index: QtCore.QModelIndex):
-        self.initStyleOption(opt, index)
-        
-        rect = opt.rect
-        
-        painter.save()
-        
-        # Get the track ID and label
-        id = index.data(TrackListModel.IDRole)
-        label = index.data(TrackListModel.LabelRole)
-        
-        # Draw the highlight if the track is selected
-        if opt.state & QtWidgets.QStyle.StateFlag.State_Selected:
-            painter.fillRect(rect, opt.palette.highlight())
-            
-        # Define padded contents rect
-        contents = rect.adjusted(5, 0, -5, 0)
-        
-        # Check if mouse hover
-        hover = opt.state & QtWidgets.QStyle.StateFlag.State_MouseOver
-        
-        # Draw the track ID
-        str_id = str(id)
-        if not hover:
-            str_id = str_id[:8] + '...'  # limit to first 8 characters of UUID
-        painter.setPen(QtGui.QPen(opt.palette.color(QtGui.QPalette.ColorRole.Text)))
-        painter.drawText(contents, QtCore.Qt.AlignmentFlag.AlignLeft | QtCore.Qt.AlignmentFlag.AlignVCenter, str_id)
-        
-        # Draw the track label if not hovering
-        if not hover:
-            painter.drawText(contents, QtCore.Qt.AlignmentFlag.AlignRight | QtCore.Qt.AlignmentFlag.AlignVCenter, label)
-        
-        painter.restore()
-    
-    def sizeHint(self, option: QtWidgets.QStyleOptionViewItem, index: QtCore.QModelIndex):
+from PyQt6 import QtWidgets, QtCore, QtGui
+
+from boxjelly.models.TrackListModel import TrackListModel
+
+
+class TrackHeadersDelegate(QtWidgets.QStyledItemDelegate):
+    
+    def paint(self, painter: QtGui.QPainter, opt: QtWidgets.QStyleOptionViewItem, index: QtCore.QModelIndex):
+        self.initStyleOption(opt, index)
+        
+        rect = opt.rect
+        
+        painter.save()
+        
+        # Get the track ID and label
+        id = index.data(TrackListModel.IDRole)
+        label = index.data(TrackListModel.LabelRole)
+        
+        # Draw the highlight if the track is selected
+        if opt.state & QtWidgets.QStyle.StateFlag.State_Selected:
+            painter.fillRect(rect, opt.palette.highlight())
+            
+        # Define padded contents rect
+        contents = rect.adjusted(5, 0, -5, 0)
+        
+        # Check if mouse hover
+        hover = opt.state & QtWidgets.QStyle.StateFlag.State_MouseOver
+        
+        # Draw the track ID
+        str_id = str(id)
+        if not hover:
+            str_id = str_id[:8] + '...'  # limit to first 8 characters of UUID
+        painter.setPen(QtGui.QPen(opt.palette.color(QtGui.QPalette.ColorRole.Text)))
+        painter.drawText(contents, QtCore.Qt.AlignmentFlag.AlignLeft | QtCore.Qt.AlignmentFlag.AlignVCenter, str_id)
+        
+        # Draw the track label if not hovering
+        if not hover:
+            painter.drawText(contents, QtCore.Qt.AlignmentFlag.AlignRight | QtCore.Qt.AlignmentFlag.AlignVCenter, label)
+        
+        painter.restore()
+    
+    def sizeHint(self, option: QtWidgets.QStyleOptionViewItem, index: QtCore.QModelIndex):
         return QtCore.QSize(100, 30)
```

### Comparing `boxjelly-0.3.2/boxjelly/lib/resources.py` & `boxjelly-0.3.3/boxjelly/lib/resources.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,592 +1,592 @@
-# Resource object code (Python 3)
-# Created by: object code
-# Created by: The Resource Compiler for Qt version 6.3.1
-# WARNING! All changes made in this file will be lost!
-
-from PyQt6 import QtCore
-
-qt_resource_data = b"\
-\x00\x00\x02\xd3\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x02\x88IDATx\x9c\xed\x9a9\x8b\
-\x14A\x18\x86\x1f\xcf\x11\x9c\x83\xcd\x04\x13\x97\x11\xd4\x1f\
-\xa0\xa2\xb2\x89G\xe4\x1d\x9b.\x86\xba?a\x91\x055\
-\xf5\xc0\xc8\xcch\xe3\xdd\xf5\x001\x1aD\x14\x05\xc1u\
-#\x15Q\x0c]50p\xa1\x0d\xca\x86\xa1\xec\xea\xee\
-\xed:\xbe\xda\x99z\xe0\x0b\x06j\xe6{\xeb\xad\xa3\xbf\
-\xae\x1aH$\x12\x89Db\xa32\x0fLH\x8b\x90$\
-\x03>\x01S\xd2B\xa4\xc8\xfe\xc5\x1ap\x03\xd8&+\
-'<\x99\x16/\x80\xbd\xa2\x8a\x02\xa3\x1b\x90\x01?\x80\
-\xcb\x92\xa2BRd@\x1ec\xb1A\x96\x19\x10|\x83\
-\xec\x03\xd3\xc0}`\x00|CM\xc7*\x91\xbe\xe3\x0f\
-0\x0bl\xf5\xd1\xe9\x1e0\x03\xbc\x89\xa0\xa3U1\x00\
-&]u\xbc\x03\xcc\x01\xab\x11tl=\xb1\x0a\x5c\x1a\
-\xeeH\x93iq\x01\xb8\x03\xecn\xf0\xdd\x0dM\x0b\xb8\
-\x8b\xfc(\x8a,\x816\xf0$\x82N4\x09\xeb*\xb1\
-\x07\xbc\xaa\x99\xec-p\x1d8\x8dz*t\x9a&\xad\
-I\x95\x9e\x0f\xc0Q\x9b\x04-\xe0Y\x8dD\x8f\x80\x83\
-6\x89\x1aR\xa6\xe9\x01j\xf0\xac\xa8Z\xf3\xcb\xc0\x09\
-\xdb$\x16\x14i\xfao\xa7o\xcaEC\x82<\x16\x81\
-\xae\x8bD\x168\xdd\xe8\x86\xe9\x00_\x0a\x12\xe4q\x0f\
-\xd8\xe2\x22\x91%\xb9\x1e\xe7\xd5\xde\x1c\xe5#\x1fC\xe7\
-\xc1\xd1F\xa7\xd3\xc3\x5c\xe1-#?\xed\x87q\xb2\xd1\
-\xe9\xcc`\x1e}\xc9\x0d/\x18\xa6\x17\x9b\x87\x92\xa2B\
-\xd1\xc7<\xfa\x12\xcf\xf9\xe0Lc\xae\xf0F\x92\xcd\xda\
-\xe7#\x86v\x0b\xbe\x85H\xa1\x1b\xb0\xdf\xd0n\xe0[\
-H,|\xa5x\x09\xf4%E\x85\xe4\x17\xc5\x06\xec\x94\
-\x14\x15\x925\x8a\x0d\x88\xa5\xf2s\x8e\xbe\x07\xfc6\xb4\
-\xdb\xe1[\x88\x14\xba\x01?\x0d\xedv\xf9\x16\x22\x85n\
-\xc0GC\xbb\x03\xbe\x85H\xa1\x1b\xb0bhw\xcc\xb7\
-\x10)t\x03\x9e\x1b\xda\x9d\xf1-$\x16&1\xbf\x0b\
-\x1c\x12\xd4\x15\x94\xd7\x14\x1b\xf0XRTH\xaeb\x9e\
-\x05'\x05u\x05\xa3\x07|\xa7\xd8\x80\x15<\x9c\xc0\xc4\
-\xc85\xcc\xb3`\x89\x11\xae\x0cs\xda\xc0g\xe2?\x15\
-\xf6\xcay\xca\xef\x05\x96\x18\x83\xe5p\x9br\x13\xde\x03\
-\xa7\xc4\xd4\x05\xa0\x05<\xa5\xdc\x84\x0cus|XH\
-\xa3w\xba\xc0K\xaaM\xc8\x80w\xc0M\xe0,\xea\xff\
-z1\xdd!X\xd1F\x15BuL\xb0\x89\xa8\xd9\x0e\
-\xdcb\x8c\x0d\xc89G\xf9#r\xe4\x0d\x00uF8\
-\x8b\xb9b\x1cy\x03r\xba\xc0\x15\xea\xff\x85&:\x03\
-69\xfc\xad=\xc0q\xd4\xe5\xca>\xd4Qz\x9b\xf5\
-=\x09\x5c\xeaI$\x12\x89D\x22\x91(\xe5/pw\
-Ld\x1eW\x19\x04\x00\x00\x00\x00IEND\xaeB\
-`\x82\
-\x00\x00\x02/\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x01\xe4IDATx\x9c\xed\x9a\xbfJ\
-\x03A\x10\x87\xbf\xf8\xa7U\xf4\x05D\xb0\xb6\x11\x14\x04\
-{}\x00;m}\x05\x0b-\x15|\x05[I\xe5c\
-(\x88y\x06\x0bE\xad\x13b)\x81X$\xab\xe1\xb8\
-\xdc\xee\xe4f3\x86\xcc\x07\x0bGng\xf6\xc7\x8f\xdd\
-\xd9\xbd%\xe08\x8e\xe3\xcc/\x8d\xcc\xf9\xfb\xc2q\xa5\
-\xfdk\xb3\x90+\xf1\xac\xe0\x06X\x0b\xb0\xc6\x0d\xb0\x16\
-`\x8d\x1b`-\xc0\x1a7\xc0Z\x805n\x80\xb5\x00\
-k\xdc\x00k\x01\xd6\xb8\x01\xd6\x02\xac\x91\x18p\x0f\xac\
-\xe5\x12\xa2\xc8\x0ap\x97#q\x1fx\x03\x0e\x841e\
-M\xab\x7f\x91=\xe0E\x18\x93L\x10\xd3\x03n\x80e\
-ALn\x03\x16\x81s\xe0[\x10#\xa6(\xaa\x05l\
-\x09cr\x18\xb0\x01<\x08c&\xa2LX\x178\x13\
-\xc6h\x1ap\x0c\xb4\x851\x133N\x5c\x9f\xf1\x052\
-\x97\x01\xa1\xd0UiJ\x22\xdc\xb6\xa6T\xf7v\xe4\xfd\
-+p\x02<\x8d\xfc\x96\xe3Vx\x1fh\x02\x9b\x11=\
-\xeb\x91\xf7\x00\x9d\xd1\x815Z\xb1@j\xce\x80\xb2B\
-W\xb7E\x07\x9e\xb4\x85\x02\xa9e\xc0\xb8BW\xdb\x80\
-0\xb5\x92\xd7\x8c\x80/\x06k\xb5\x0c\xe9\x12\xa8\xcaU\
-\x87\x86\x1f\x853\xe5m\x01;\x8a\xf9\xb6\x81G\xc5|\
-\xbf\x84\xa9\x18\xab\xf0\x90\xb6S\xf4\x80k\xe0j\xf8\xac\
-\xb9\x0b,\x01\x97\xc0\xc5\xf09F'\xde%i\xa7\xf8\
-%VP\xca\xbe\x134w\x81\xc0.\x7f\xe7\xfd\xa4\x0a\
-\xafE\xd5`\x16\x07\xa1\xdb\x88&u\xca\x06\xe9\x02\xa7\
-\xc2\x18\x0d\x03\x02\xa6G\xe1g\xe6\xf4ch\xae?\x87\
-\xff\xfb\x85\xc8h\x81T\xa7\x09\xac\x0ac\xa6m\x00C\
-\x8d\xcd\xd4\xce\xfe\x1f\xa1\x5c\x89g\x057\xc0Z\x805\
-n\x80\xb5\x00k\xdc\x00k\x01\xd6\xb8\x01\xd6\x02\xacq\
-\x03\xac\x05X\xe3\x06X\x0b\xb0\xc6\x0d0\x18\xf3\xa3\xe2\
-\xdd\xe7\xd4TL\x89\xe2\xc5\xc6;pX\xd1\xff\x88\x81\
-A\xd9\xef\xf7\x1c\xc7q\x1c\xe0\x07\xaf\xfd\x93\xbd\x10\x9a\
-g\x8e\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x03\x22\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x02\xd7IDATx\x9c\xed\x9a\xcbj\
-\x14A\x14\x86\xbf\x98\xd1\x85\x0b1+\xddd\x130\xa2\
-\x09\xe8:+\x05}\x03\x09\x127\xbe\x85\xee\xcc\xd2\xd7\
-\x10\x03F\x13\x88/\xa0\x0b\xf5\x09\x8c\x11\xdd\xc8\x80\xa8\
-\xe0e\xc4\x04Q\x83\xa6]t\x17\x8cmO\xd7\xa9S\
-\x97\x99L\xea\x83\x82f\xbaN\xd7\xff\x9f\xaa\xae\xae\xae\
-\x1e\xc8d2\x99L&6\xd3\xc0:\xb0\x0d\x14\x96\xb2\
-\x0dl\x00\xa7\x87\xa24\x02\xd3\xc0\x17\xec\xc6\xeb\xa5W\
-\xc5\xee{\xd6q7o\xca\x83!\xe8\x0d\x8ed\xd8\x0f\
-*\xdfb\x8b\x9b\x88\xdd\x00\xa5\x11\x976]\xeb{q\
-(\xe6\xc5\xf7\x03\x9d@\xd7\x99\x02f\x809\xe0lu\
-<\x03\x9ci\xa8[\xefa\x1b\xbb\xc0[\xe0MU^\
-\x02[\xd5q\x17\xd8\xd3I.q\x19^\xc6\xa4)\xc6\
-\xec)\xe0\x98\x8f\x08\x0f~\x01\xef\xf87)&I\xef\
-%\x17pI\x80k\xcf\x0d\x1b\x91\xb7\x03?\x07\x1c\xf8\
-\x04d\x0e:\x9aE\xc6w\xe0(\xf0\x13\xf8Q\xfdf\
-\x8e\x9b~Ky\xde\xd4\x89J\x17\xfd\xd26v\xe9\xba\
-\x9a\xd1L\x82\x9f\x141\xa9p\xd6\xa6I\xc0gEL\
-*\x92$`\x94G\x80s\xe7\x8c[\x02\xf2-\xe0\x1a\
-\x90b\x04l)\xda\xd0\xc6\x8e\xdc-\xb0\x0c\x9c\x03V\
-\x14\xed\xac\x01\xe7\x81\x9b\x0e1In\xcf\x05d\xcf\xe4\
-[}1\x93\xc0]a\x9c\xd9\x0b\xec\xdf\xab\xb8!\x8c\
-[\x08\xec\xb5\x91Y\x81\x90M\xfe\xdfl\xe9\x00\xab\x82\
-\xd8\xd5\x01\xb1\x9b\x82\xd8\xd9`.[\x98\x12\x08)(\
-\x87p\xdd\x88m$\xd4{\xde\xc4\xac\x08\xdb<\x1e\xcc\
-e\x0b\x13\x94\xdbT\xa1\x93\xe0k~\x974\x9b\xbc\x00\
-|\x10\x8a\x92&\xc1\xd7|QiJ\xc6s\x07a\xb6\
-$\x840_T\x9a\x92\xf1\xc8Q\x5c\xdb\xe4\xa6\x9d,\
-\xeb\xe5q@\x7fV\xee+\x04\x0e\x1a\x09\xfdhz\xbe\
-?\xc1\xceh\xf7\x04\xb5\x0b\x8e+\xc0=\x9a\x930\x09\
-\xdc\x01\xae\xa5\xd4\x94:\x01P\xf6\x96\xe6\x9c\x0d\xd5;\
-\x8a6\x01\xda\x17\xa25`\x09\xf8\xddp\xee\x0fp\x1d\
-\xdd\xb2\x19\x12\xbf\xa5.2z\x93\xe0b@\x7fV.\
-:\x8ak{\xd4iV\x8cM\xe5B@\x7fV\xe6\x1d\
-\x84I\x9e\xf3!\x920\x1f\xd0\x9f\x95\x93BQ.\x8b\
-\x1c\xdf$\x9c\x08\xe8\xcfJ\x87\xf2\xb3t(\xf3\xbeI\
-\xd8k\x88\x8bN\xafEP\xea\xd7\xe1^PgB^\
-\xb7\x08*\x80\xdb}u]Wx\xf5\x91\xb0l\xa9\xff\
-*\x82?+\xcf,\xa2L\x12\xb4\xcb[\x93\x04\x9b\xf9\
-\x02x\x1a\xd9k#\x1b\x02a\x05\xf0BX\xcf'\xf6\
-\xa1\xd6\x84\xcf\xff\x03\xa4\xab\xc19\x8f6\xa4\xb1\x1f\xb5\
-\x0d\xf8$`\x94>\x90\xa8\xb5\x8cK\x02\xd4\x1fkR\
-\xdc\x02)\x18\xca\x08p\xfe\x16\x1f\x91\xa1h9\x02|\
-E?\xc3\x87*=\xe0pd\xaf\x03Y\x12\x08\x8c]\
-\xaeFwi\xe12\xe5Bd\x87t\xa6w\x80'\xc0\
-\xa5\x04\xfe2\x99L&\x93\xc9\x8c)\x7f\x01\xd3\xf3\xeb\
-\x98\xbb\xef\xcd8\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-\x00\x00\x01\x9b\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x01PIDATx\x9c\xed\x9aA.\
-EA\x10E\xcf\x17\x06&\xa6\xc4\x0e\xd8\x01\xdb\xc0\x16\
-,\x80\x0d\xd8\x86m\x08\xcb`\x03\x18\x99\x9a\x0a\x03\x09\
-\x03\xf9I\xc5Dy\xf4\xef\xd7u\xefI\xde\xb4\xab\xfa\
-$/\xf7\xbd\xee\x02c\x8c1\xc6\x18\x93\xe2#\xf1\xac\
-\x9a]\xe0\x0a\xb8\x006[\x17\x9b\x9b\x80#\xe09\xd4\
-~\x02NZ\x16\x9c\x8b\x80-\xe0\xb2G\x0fs\x10p\
-\x00\xdc\xf7\xea\xa1\xa7\x80u\xbe\xde\xf3\xf7\x8e=t\x13\
-\xb0\x07\xdc&\xeb\x97\x12\xb0\x00N\x81\x97d\xedR\x02\
-\xb6\x81\xebd\xcdr\x02\xbe\xc7\x9b\x8c\x80\x9f\xe2\xad\xb4\
-\x80\x03\xe0!Y\xa3\x94\x80\x0d\xf2\xf1VN\xc0>p\
-\x97\x5c\xb7\x94\x80\xa9\xf1VB\xc0\x0ep\x93\x5c\xab\x9c\
-\x80c\xfe\x16o\xc3\x0a\xf8\xafx\x1bR\xc0!\xf08\
-a\x13\xc3\x0bh\x11o\xc3\x08h\x15oC\x088\x03\
-^;lz\x92\x80\xc5\x04\x01#\x90\xde\xd7Z\xcb.\
-F\xc0\x02z7\xd0\x9b\x16\x02\xce\x81\xb7\x06\xeb\xce\x02\
-\xc7\xe0/\x8aK\x7f\x08Ed?\x85#\xd2?C\x11\
-\xd9\xdf\xe1\x88\xf4\x81\xc8\x12\xe9#\xb1\x88\xec\xa1hD\
-\xfaX<\x22{1\x12\x91\xbe\x1a\x8b\xc8^\x8eF\xa4\
-\xaf\xc7\x97H\x0fHDdGd\x22\xd2CR\x11\xd9\
-1\xb9\x88\xf4\xa0dDvT6\xb2\xd2aic\x8c\
-1\xc6\x982|\x02\xbb\xfd@xy\x91\xc8\x87\x00\x00\
-\x00\x00IEND\xaeB`\x82\
-\x00\x00\x0b\x98\
-\x00\
-\x00.Ex\x9c\xedY\xd9\xae\xdb\xd6\x15}\x0f\x90\x7f\
-`\xe5\x17\x1b\x15\xa93\x0f\xca\x95\x03$F\x8a\x14\xcd\
-K\x92\xb6@_\x0c^\x91\xd2e,\x91\x02I\xdd\xc1\
-_\xdf\xb5\x0f\x07\xf1Nn\x9b\xc4\x06\xdcHN j\
-\x9fy\xef\xb5\xd7\xda\x87\xf7\xe2\xeb\xdb\xfd.\xba\xce\xeb\
-\xa6\xa8\xca\xd5\x8c'l\x16\xe5\xe5\xba\xca\x8ar\xbb\x9a\
-\xfd\xfd\xe7\xefb7\x8b\x9a6-\xb3tW\x95\xf9j\
-VV\xb3\xaf_\x7f\xf9\xc5\xc5\x9f\xe28\xfa\xb6\xce\xd3\
-6\xcf\xa2\x9b\xa2\xbd\x8a\xbe/\xdf5\xeb\xf4\x90G/\
-\xaf\xda\xf6\xb0\x5c,nnn\x92\xa27&U\xbd]\
-\xbc\x8a\xe2\x18C1\xb8\xb9\xde~\xf9E\x14EX\xbb\
-l\x96\xd9z5\xeb\xc7\x1c\x8e\xf5.\xf4\xcd\xd6\x8b|\
-\x97\xef\xf3\xb2m\x16<\xe1\x8b\xd9\xa4\xff\xfa\xd4\x7fM\
-;(\xae\xf3u\xb5\xdfWe\x13\x86\x96\xcd\x8bi\xef\
-:\xdb\x8c\xddiK72\xf4\xe2\xde\xfb\x05\x13\x0b!\
-b\xf4\x88\x9b\xbb\xb2Mo\xe3\x07c\xb1\xcf\xa7\xc6\x0a\
-\xc6\xd8\x02m\x93\xae\xffe\xb7e\x03\xcf\x1e\xf0\xff\xd8\
-\x7f0$Mu\xac\xd7\xf9\x06\x03\xf3\xa4\xcc\xdb\xc5\x9b\
-\x9f\xdf\x8c\x8d1K\xb26\x9b\xce38\xf6\xde\xba\xf7\
-\xbc]\xa6\xfb\xbc9\xa4\xeb\xbcY\x0c\xf6n\x82\x9b\x22\
-k\xaf\x10js\xb8\xed\x0cWy\xb1\xbdj\xa7\x96\xeb\
-\x22\xbf\xf9\xa6\xba]\xcdX\xc4\x22n\xf0_o?\xe1\
-\x84w\x96\x22[\xcd~\xfa\xc7_~\xac\xaa\xb67\xf4\
-k-\xc7\xbe,\xf1\x22\xd1\xd1K\xc1\x0c\xcb\xd7|\xe3\
-7\xf3H0\xc1b\xa6b\xe6^u\xc3\x86\x93.\xb3\
-jM;_\xcd.\xab\xdb_\xf2\xdd\xee.\x19=8\
-N\xbdK/\xf3\xddj\xf6M\xba~\xb7\xad\xabc\x99\
-\xcd^S\x87\x8b,\xdf4\xa1g\xb7/\xfa\xc9Y\xd7\
-\x86\xd6q\xf8!m\xaf\xe2|\xb3\xc9\xd7m\xdf;\x8a\
-\xba\x9f\xabY\x8b\x0e\xf5\xdb\xa6\xad\xabw\xbd\xbb\x86\xd9\
-&\xa3\xb4t|\xd2\xd8\xbc\xbd.\x9a\xe2r\x87M\xb7\
-\xf5q2\xac\x9b\xe6m\xefp\xf8\xe1\xd4\x94\xb6m\xba\
-\xbe\xc2BiM\x9e\xcfcfO\x8dy\x99\xbd\xad6\
-\x9b&o\xc3(\xfaL&\xdd\xc3\xd7W!=\xc7(\
-\xd0\xe7\x97\xaa(\xdb;BD~\xdb\xd6\xe9\xa1\xdaQ\
-n\x9e\xda\xf7E\x8b\x93\xed\x0a|c$C\x9e/>\
-\x8egb\xf9\xa9|\xc3\x13%\x90d^}V\xde\x89\
-\xed\xff\xee\x1f\xfeG\xf1\x8e\xf84\xbe\xf9\x1c\xb3*\xfe\
-d\x9c\xf3Y\x22\xe7Wd\xd5\x1f\x87\x91c\x7f\xc6\xce\
-\x07\xfcc\xfeo\xb0s\xb1\xa0\xaa\xa7{\x1ck**\
-\xa82\xaa\xe9&\xc5\xd1e\xda\x8cg;\xa4[T\xd0\
-\xbb\xaa^\xcd^l\xc2gh\xb9\xac\xea,\xaf\x876\
-\x13>\xf7\xdb*\x94\x98E{\xd7]\x1d\x86\xf9O\xd1\
-\xd9\xe6c\x07\xf6L\x87\xe6*\xcd\xaa\x9b\xd5L<j\
-}_U\xfb\xd5L\xe9Dh\xe5\xa4z\xd4\xbeF\x85\
-\xaa\x12\xe6\x98\xd7\xda>n\xc5\x9a.\xd1\xdeK\xed\x1e\
-5\xa2\xcc<\xd2\xed\x22>\x96E\x8b\xea}\xa8|\xa7\
-\xe3\x8fuM=v\xe9]\x8e\xd3\x87\xaf1B\xcdU\
-u\xb3\xad\xc9\x91\x9btw\xf2\xe48\xf8\xa6(q\xa8\
-\xb8\x07\x8bT\xea\xf1\xd9\xfb.c\xf5-\x05\x7f\xae\x0f\
-U\xe2\xcf\xb5\xe1\x94\xe2\xb1k\xfa\xc6}z\x0b\x88\xbc\
-\xcf\xb3\x89L\x8e}h\xff\xf1\xe5%\xd5\xf9S\xa4\x8f\
-\xedM\x99\x1e\xe2\xb2\xca\xf2\xa6\xef0`l\x9f\xb7i\
-\x96\xb6\xe9\x04N\x83\x89\xcb\xb1\xde\xc6\xb5j\xf9\xe3\x9b\
-\xef^\x0f\x98\xbdX\xaf\x97\xff\xac\xeaw#\x86\xa3\x88\
-\xba\xa4\x97\xd5\x11\xc7\x9f\xbd>\xd9/\xb2\xf5\x12\x17\xa1\
-}\xda\xbe.\xf6@\x08]\xa2\xfe\x8c{\x0f\xc0=6\
-\xdc\xefM\xa92\x99\xb7\x9b\xb9\xce\xbb;\xd5\x93\xb7\xcb\
-l\x8d\xd4\xc1\xa8\xc5Om\xb1\xdb}O\xcb\x9c\xf8e\
-\x9c\xb6hw\xf9\xc4z\xb1\xe8\xcf0\x9cq1=\xe4\
-\xc5b\xf0B\xf7\x13\xb7\x97\xe2\xd0\x0c\xfbj\xda;\xe2\
-\x94\x0dV[\xbe`L\xa94\xfd\x8a~\xc4}\x82,\
-\xf9W\x1d\xc3P\xab\x94\x8e\xf5?;\x0c-\x91^\x5c\
-H\xcd\xad\x1e\xec\xbb\xa2\xcc\x11\xa7\xe5\xe5\xb1m\x07[\
-\xa0\x85\xc0\x0aK5\xd8\xb2\x14\x19V\xd7\xe9\xdd\xb2\xc4\
-\x0d~\xb0\x8e\xab\xce&Q$^tb\xcc\x16\xca\xaf\
-\xd3\x8f\xbb\xc9\x8f\x1a-6Q^:\xa1\xf4h\xbc;\
-\x19G\xacl\x1f\xa2\xaa\xbf\xbc\xfd\x95\xeev\xd3\xb5\x1f\
-\xe4W\xe7\xad\xach\x0eh\xc0u\x97N\xfb\x04\x82\xab\
-\xe3a\x0f\x84\xf6\xc3G\xecm\xc78\xd2\xd4[\xa7&\
-\xd4\x0a:-\x1bB\x11P\x9b\xb6uq\xfb\x92%\xce\
-)a\xb9\x96sF\xff&?\x13\xc1\x1c\xd7\x96q<\
-Z%\x8c\xf5V\xbf:a\xf5\x82<6\x01\xde\x89r\
-\xb1)\x82\x17R\xa7\x19>\xb3I\xc7\x13\xcbT%\xc2\
-\xd8Vu\x0c\xbe\xb9N\xdbc\x9dO\x92}8A\x8d\
-.\x82\xe9\xa9\x99\x92.\xe2<\x11\xb4=3\xe7\x89\xe7\
-\xd0]\xc3#l\x14|\xa3-v,\xb9\xe5\x92\xebh\
-\x0d\xa3\xe3\xd2ZGF\xcd\x11!\x11q\xd2\x22\xa6\x04\
-\x86J\xe7\xa4d\x1c&\xe5-\xf7n.\x12\xee\xb4p\
-\x96G\x7f\xa35\xe0?n\xe4\xdc$\xdehn8\x8f\
-\xbe%\xab\x94^r?\xb7\x895\x82s'#\x0ey\
-\x93\x06\x00\x9a\xbbD\x0a\xcb\x843\x91O\xb4\xe5\xc6\xc2\
-\x86~\xd2jc\x1c\xe6t\x89\x93Vpc`U\x82\
-)\xa9%\xe6\xc43\x07\xd1\x1b\x8d\x95\x1c3\xc2(\x0d\
-\x1bN'\x14#\x1bt\x8e\x09\xeb1\x9a1\x8enj\
-\x0ei`\x98R\xa80\xa7\xc7\xfc\xdc\x0a\xec\x1e\xbb0\
-\xce\xd2\x9c>\x11\x12\x13a\x9f8\x9cUR\xa0/\xf6\
-\xa9\x18\xf7\xd8\x13O\xb4\xc1\xf4\xd2>\xe9\xc9\x7fM\xfd\
-=\xcd\xdfI\x22-{\xc5|\x90\xad\xbfw\x92NI\
-\xe8\x01\xe6&x\x0e\x8fT)\x00\xd2\x0a\x87\x80\xe7\xf9\
-<\xc6\xc1\xb5\x15\x8a\xebWO\x22\xb0\xaa\x8bmQ\xa6\
-\xbb\x18\x88\xfa\x01\xfe\x86\x5cJ\xe1=b\xc8\xbdG\xe0\
-\xc8\x8b&1^+n\xe5\xdc'\xf00\xe2\xc0#\x9d\
- nH\x13\x05\x1b\xc3\x18\xa5<l\x9a;&\xbc\x81\
-\xcd{\xed\x95\xb3\x18\xcb\xb4\x17\x92\xcf\x03<\xf0\xb1\x91\
-J\x8c\xd5\x8ea:\xb8\x1d\xf3:!#\x99xk\x95\
-\x05na\x03B\x113\xd8\x84w\x1aO4\xd6*c\
-,\xd9\x98s\x8ei=\xe7\x02\x07\xd3\x16a\xe6\x89u\
-\x1e#\xe6\x5cb\xd3\xd2\xd8'\x0f:\xa9\xfaP\xcc<\
-\xfb>\xe7\xe9,^\xe3\xf3\x1b\x12\x98V\x033>\xcc\
-\xe0\x1f\xe0\x1dl\x5c\x0b\xab\x91\x09^\x19!\x8c\x0f\xfe\
-\x86#\x8c\xf3\x16Q\x10\x0e\xb9\xa85l\xc2i\xb8\x9c\
-\x22\xa3\xac\xc7\xc1-\xfc\xed8e\x87\x80\xcd2\xad$\
-2\x061\xc0\x08\xe9\x14l\xf4`\x04\xc5E\xc2+\x86\
-\x86z\x89~\xd6\xc1\xc4\x95\x05\xf2CHa\x14J\x22\
-.4-\xf9\xd6\x93k5\xea\xf8`\x13\x8c3\x0b\x9b\
-\x03\x05jKK\x80\x0f\xb4\x11\x96\xe2\x02\x94\x08)\xa3\
-\x14Q\xc0$\x861J\xab\xfe)b\xdd?$\xac\xb1\
-\xc4H\xc8[\x8e\x04\x04\xa3Xf\x05qO\xff\x14\xfa\
-\xf1\xd0Sy\xa2)\x8c6\x81\xb8\xc0\x12tl\xe2b\
-\xd0\x94W\xd4\x07\xa7b\x8a\xb8L(/\xa2\x18\x9d\x14\
-\x00\x8a\xf9\x80{#\x09\x9d\xb0\x09\x9c\x14\x9b\x84\x0dp\
-\x02\x8d\x93\x0d\xa4\xc24'6\x07\xbd\x0b\x11l\xa0E\
-\xe7\x19\xf5c\x06kGP\x80(\x96\x89A\x1d\xaf\xe7\
-1\xa8\x10\xdfO\x18\xb0\xba\xc1\xce\x99\x9f\xd3\xfaX\x9e\
-\xd90\x1b1\xae\x0e6\x06\xd2\x0c+x\x10\xa4ra\
-U&yg\x13\xda\x09\xf8\x9d\x8e\x05\xd6\xe3\x86l\x8a\
-1\x00\x99v\xa2\x19G\x94\x82\xcdi\xc0\x9d\xc6\x1ax\
-T\x84\x85q*\xa0\xdc\xcf)\xa1\xc0\x9e\x9el\x8eS\
-:\x12\xcd\x09d\x8c\x0e\xfd<\xa6F\xd1@\xd4\x07\x8b\
-\x0bk\xf0ppM{\xf1\xdc\xa9`c\x81\xcai+\
-\x12\x89\xfa\xa4)8\x85\xa2\xe2\x1dE\x07\xf1\xf7H<\
-j\x96Z)\x13\x9cg\xb4\x8b\xc2q<\xf0I\x1e`\
-\x01A\xf0\x89\xb3\xde\x98`\x12\xdeBYHi\x94\x83\
-/\x88\x9d@1\xc0&E\x1a\x11\xc3\xc4\x9d?\xadW\
-\xbc\x9b\x0dZl\xc9&-\x08\x88V\x00\xca5\x96'\
-\x9bR\x18\x1b\x10\x00BgB\x06\xe0\x98\xee\x04\xa0?\
-\x17v\xc1Dg\xb0<\xac\x88K\x81\xc8c\x15\x8e\x04\
-&\xcac3\xc7o\x83g;>\xc3\xc7J\x03[\x01\
-d\x5c\xd1^\xc0J\x9e9\xab)<B \x13<L\
-\xc6#\x9cR\x85e\x80b\xca]\x8d<F1\x8f~\
-Dd\xa09 \x14\xb9\x8bc\x07\x1aS\x02N\xa7\x8c\
-\xf4\x88:\xfc\x82\xb4\xb2\x90c\xc0\x83\xb2\x19\x99\xc9\x14\
-\xb1'8\xc1\x91W`3\x1e\xf1\x14\xd4\x0f\xb4\x0c\x1a\
-'\x1b\x91\x83\xa2\xd4\x85\x5c{B\x85\xa6\xa2\x85D\x9c\
-l\xcc\x1bB\x85\xa1d\xb2\x5c\x90\xcd@0\xa5&\x9b\
-`\x10GM\xebj\xe2\x0eI\x0c\x0dM\x87o)\xc5\
-q\x0bQ\xa0k\xe8\x00X\x9ci21p\xab\x95d\
-\xb2\x92\xf27\x10\x10@$\x99|^\x22\x07Y\x0c%\
-n}\xdc\xe5$l\xefq_\x1cts\xaas\xbdh\
-\x1en?$\x9bd\xa3k\xf12\xe8\xe7o\x97H\x91\
-P\x9e\xa0\xa0\x0e8\xc2Y\xc1\x85\xea?K\xe4\x1e\x85\
-\x06\x06y\x90\x07\xfc\xc0\xa4\x0ab\x08\xa2\xa2\xcc3\x80\
-\x88\x11\x04Q-q/\xa5B\x0a\xd3\x02\xb7]\x8aj\
-i\x94\x13S#\xe4\x8f!m\x14eW@\x0b\xc2D\
-\xfc\x09\xaa\xa3\x0a\x84\x18\xcb@\xffBE&=\xea\x17\
-B\xa6\x85\x92p\xcaj\xf0\x9bE\x10\xe2\xa0\xf6`#\
-\x1a\xc9\x9d\xf7\x9c&\xb3\x9cK\xca\x08\xd43\x00\x1f\xfb\
-\x15\x9a8}\x93\xffQUq\xfa\x02\xa6\xafl\x016\
-q\xdf\xc9\xa1\x8c%\x1aD\x1aP\xa6Q\xc6\xa1\xd6$\
-?H\xd4:\xa8\x0e\xc8$ \x03\x90\xa5\xc48\xa9\x99\
-S!\xefQ\x85\xe8P\xf9\xa2X\x01\x13S7\xd0\x0c\
-#\xb2P(\x80\x99\x0f\x8eF\xf6p\x14 \xf7\x8d\x9a\
-y\x0d\x9e\xec\xc8\xcf\x93\xb2x\x1b\x04\x85\x07\xdaE\xa0\
-\x18\xb2M\x05\xe1AE\xc9C0\xc0W\xcc*\xdd)\
-\x167a\x13\xd8\x8d\xf0av\x08!\x1a\x83\x8d\xdek\
-\xd8N.A\xcb\x9a6\x06\x01\xa2N\x88+\x12\x97\xf8\
-\x0f8\x80\xfcQ\x1fH\xba\xa3\xf8+|\x13lqn\
-\x83)\x02sj\xa3qg\xa4\x15\xb5\xe6L\x072\x15\
-\xa8w}\xa7%\x00EO\x89\x9d\xbahhv\x87.\
-\x09>'\xf6\x86\x1a\xc1K\x01\x84\xa4B>\x5cx\xa0\
-.\xd8\x04\x9d\xd2\x0ac8\x91!\x0a\x04\xde\x11.8\
-\x8e\xc9p\xcd\x80\xcc\x89\xc1\xd5\xac\x13f\xd2\x96\x9e\x86\
-\x1f\x98\x06!\x81\xaf\x82\x8b\x10$K!A\xdd\x88\xc8\
-\x05\x02G\x05\xe2:JW\xdd\x02\x94aH\x1f@\x92\
-u*\x02J\xb2\xc4\xbeHZ'B\x02\x1b\x94(\x86\
-\xbc#\x9d\x97\x8a\xca^\xd2\x09\x9c\xc4FA\xf5\x15R\
-\x8bl\xa8hM\x00\x0f\x84\x08\x0a&H\x80\xe8\x0a\xa0\
-\x82;8J\x1d\xdb\xa9\x8d\xf0\xdcw\xdb\xa0\x92\x95\xea\
-\x83\x90\x8c`\xf3pz\x89@)\xafi8\xa3\xfbz\
-\xe7_\x0e\x06\x0e\x9a\x03e\xed1\x0a~\xd6a,\x0e\
-\xd7\x83\xcf\x86\x8c\x0f3C&\xc8\x82;\x8c\x14\x9db\
-:\x1a\x05\x94Q-\x12fR@]H{\xd4\xd8\xb8\
-4\xdd\xb3Y\x10\x0eX\x1c.E\x8c\x94\x0f\xe4\x11\x9c\
-\xa1\xb9&y\xc2\xfc8Q8$\xb4\x86\x8a\x8bn}\
-\xd9\xad\x0f\x9fxdN\x1f\x0fgCGA\xb5]W\
-?\x9c\x8c\x0e\xaa\x8a\x9a<z\xff\xb9\xf1\xfdx\xc5G\
-\xceI\x14\xcf\xbc\xab\xcc\x90\x9f,@w|\x1a\xdb9\
-\x15s\x80\x13\x95RPo\x85\xea\xe6\xac\x0a\xcf\xfe5\
-\xe1#\xeb\xc2}\x09:+\xc3Y\x19\xce\xcapV\x86\
-\xdfS\x19\xe8\xca\x0e\x8cR\xec\xc3E\xc0\x01\x1b\xaeC\
-\x89r\x1e\xb9B4\x1c\xaeY\x00\xb3\x9d\x8b\x00~)\
-\xe8\xdd#\xee@\xb8\xa6\x8a\xf3k\xb5\x0f\x88\x85\xf9T\
-R\xc1\xce\xaf\xd6\xce\xaf\xd6\xce\xaf\xd6\xce\xaf\xd6\xce\xaf\
-\xd6>\x9e\xa0^,\xb6\xfd\x9f\xba\xe9\xfb\x82\xfe0\x8f\
-\xef\x7f\x036@F\xa0\
-\x00\x00\x02\xbb\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x02pIDATx\x9c\xed\xd9\xbfk\
-\x14A\x18\xc6\xf1O\xbc\xa0\xa0\xc6Ki\x17\x7f \xe8\
-?`\x88\xb5\xc6BIge\xa5\xd6jii\xb0\xb1\
-\x14\x14\xb1\xb1\x12\xff\x04Q4\xa8 \xd1\xc2\x80\x8d\x88\
-\x09\x82\xc6\x1f`\x17\x8d\x88\x85Jb\xb1\x1c.\xb8s\
-w\xe6vw\xee\xf6\xf6\x0bo1\xc3\x1e\xf3\xbc\xcf\xce\
-\xbc37KMMMMM\xcdF\xd9\x81[\xb1E\
-\xc4b\x12o\xb0\x1e[H\xd94p\x01?%\xc9\x0f\
-\x95\x01\x13x\xe2o\xe2Ce\xc0\x09\xac\xf87\xf9\xca\
-\x1b\xd0*tY\x89W\xde\x80t\xa1\x1b*\x03F1\
-\x8b_:'_t\xac\xe23\xe6q\x13g\xb0\xa7\xb8\
-\xd4\xd9\x8d\xa7\x91\x93\xee&^\xe0<\x9ay&\x7f\x12\
-_\xfb \xb9\xff\x89/\xb8\x84\xed\xc3j@+>`\
-&\x0f\x13\x06e\x09\x84\xe2\x1a\xb6\xf4jB\xd6io\
-\x90\xe2\xb1\x9cj\xc3!\xbc\xedb\xc0\x22\x19\xc3^\x1c\
-\xc3e\xbc\xecB\xcf:\x16$g\x98\x9ei\xe2v\x87\
-\xc1\xca\xe6 \xeew\xd0\xb4\x8e\x87\xd8\x9c\xd7\xa0\xed\x0a\
-d,\x0e\xe3u@S+\xae\xe69`\xa8@\xc6\xa4\
-\x89\xbb\xda\x9b\x90\xcb\xee\xd0\x22\xeb\x94\x18\x9b\x06n\x08\
-\x1b\xf0\x1e\xdb\xf2\x1e4] \xfb\x81\x86\xf63a\xb6\
-\x88A[\x05\xb2_hbQ\xb6\x01+r\xda\x15\xfa\
-\x9d#\xc2\xb3\xe0\x5cD]\xa5\xf2@\xf8l0\x14L\
-\x0a\xcf\x82]\x11u\x95\xca+\xd9\x06\x9cN?\xb4\xa9\
-|]\xa5q'\xd0?\x95nT\xd9\x80\xf9@\xff\xfe\
-RUDd\x9f\xec%\xf0)\xa6\xa82\x19\x93m\xc0\
-\xb7\x98\xa2\xca\xa4!\xdb\x80\xdf\xe9\x87\xaa\x5c\x03\xb6\x06\
-\xfa\x7f\xa4\x1bU6`g\xa0\x7f5\xdd\xa8\xb2\x01\x07\
-\x02\xfd\xef\xd2\x8d*\x1bp4\xd0\xbfX\xaa\x8aH\x8c\
-\xe0\xa3\xec\x22x*\xa2\xae\xd2\x98\x12\xfe/0\x11Q\
-Wi\xcc\xc9N\xfeyLQe1-\xfc\xf6\xcfF\
-\xd4U\x0a\xe3X2\xa47B\x0d\xdc\x13~\xfb\x17\xe3\
-I+\x9eN\xb7\xc2\xcb\xc2'\xc3\x81g\x5c\xfb7\xbf\
-\x86\xe3\xd1\xd4\x15\xcc\xb4\xf0\x9ao\xc5\x95h\xea\x0ab\
-D\xb2\xcf\x87\xb6\xbat\xcc\xc9\xf1\xdb`,\x9a\x92\xcb\
-\x8d\x19\x5c\x17>\xe1e\xdd\x00\x8fE\xd0\xdb\x15\xdd$\
-\xd0K<\xd4\xe7[^Q\x89\xafI\xd6|\xdfO\xfb\
-\x22\x92_6@\xd5>\xcf\xc4W$\x87\x9c\x81\xda\xe7\
-\xf3H|Ar\xb6\xefi\xad\x8f\xf6\xf2\xe3\x92X\xc5\
-w\xc9\xa7\xf8%<\xc3#\xc97\xff\x9a\x9a\x9a\x9a\x9a\
-\x9a\x9a\x9a\x0d\xf3\x078\xcd\x84p\xe6]\x83;\x00\x00\
-\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\x10\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x01\xc5IDATx\x9c\xed\x9aMJ\
-\xc3@\x18\x86\x1f\xff\xb6\x15\xbd\x80\x08\x9eAAp\xaf\
-\x07p\xa7[\xaf\xe0B\x97\x0a^\xc1\xadt\xe51\x5c\
-\x88\x9e\xc1\x85\xa2\xae+\xae\x04)\xc4E\x1b\x88\xb5\x93\
-\xccL\x93yM\xf3=0\x10\x92\x99\xcc\xcb\xd3\xf6\xcb\
-d(\x18\x86a\x18\xdde\xa1\xe1\xfbg\x81\xf3\x86\xf6\
-\x9f\x99\xc5\xa6n\xdc\x16L\x80:\x80\x1a\x13\xa0\x0e\xa0\
-\xc6\x04\xa8\x03\xa81\x01\xea\x00jL\x80:\x80\x1a\x13\
-\xa0\x0e\xa0\xc6\x04\xa8\x03\xa8\x89\x15\xd0\x03n\xea\x0c2\
-#\xb7\xc0Z\xaa\xc9v\x80'\xdc\x9b\x17E2G\xab\
-\xab\x7fq\xdc\x0b\xb0\xe7\xd17\x9a%\xe0\x14\xf8&,\
-X*\x01\x190\x04\xae\x80\x15\x8f1Al\x00w3\
-\x04K% o\x8f\xc0\x96\xc78/\x0e\x81AM\xc1\
-R\x09\xc8\x80O\xe0\xc4c\xac\x93\xbc\xd0\xb9B\xfdw\
-\x01y\x8b*\x90\xc5B\xd7v\x01\xa5\x05rr\xbby\
-\x198\x07\xce\xc6\xc7U|T\x5cw\x99\x0f\xdd\x16\x8f\
-\x9d\xa7\xc8\x10\xb8\x04.\xc6\xc7\x7fp\x15\xba&\x9a\x8b\
-\x14sO-\x90e\x85n\xde\x04d\x14\x0ad\x97\x97\
-\xc2_\x93'\xba\xf2\x13x\xa0d\x8d0m\xb57/\
-\x02\xa6\xae\x12]\xd5x\x17\xe8\x03\x9b%a\x01\xd6+\
-\xae\x0f\x1c\xe7C\x9f\x02\xb1\xf3\xe4<\x03G\xc0}E\
-\xbf_\xf4\x80k\xe2>\xc9\x9c\xba\xbe\x01\xb1\xf3d\xd4\
-\xf0\xa6\xd8\xe6\xa5\xf0\xb1\xc7X/\xda\xf62TZ\xe8\
-b\xe9\xf4\xebp\x91m:\xba!Rd\x95\xd1S\xa2\
-\x8aT\x02\xfa\xe3L\xc1\xd8\x7f\x84\x9a\xbaq[0\x01\
-\xea\x00jL\x80:\x80\x1a\x13\xa0\x0e\xa0\xc6\x04\xa8\x03\
-\xa81\x01\xea\x00jL\x80:\x80\x1a\x13 \x98\xf3\xad\
-\xe4\xda{\xb2\x14\x89\x98\xdc\xd8x\x05\xf6K\xfa\x1f0\
-\x12\x14\xba!b\x18\x86a\xc4\xf0\x03\x16\xf2\xf2\xcaR\
-\xed\xcdq\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x01\xb0\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x01eIDATx\x9c\xed\x9a\xb1M\
-\x03A\x10E\x1f$\x88\x10BD\x0f\xd0\x01P\x00\x15\
-\xe0*  \xa5\x05\xdapH\x0a]@\x8a\x04\x15@\
-\x86#\x86\xe0\xb4\x92\x03#\xad\xcf;7\xda\xfb\xf3\xa4\
-\xc9,\xcd\xf7K\xe6vw I\x92$I\x92$\xa9\
-\xe6\x10x\x00\x9e\x80\x93\x80\xfeVQn\x5c\x03\xefk\
-\x8d\xbe\x80\x1b\xcf\x86\x1b\x08\x15\xf0_\xc3%p\xe4\xd9\
-\xb8\x22C\xa8\x00\x03>\x80\x0b\xcf\xe6\x15\x19B\x05\x18\
-\xf0\x0b<\x02\x07\x81\x19B\x05\x94z\x05\xce\x023\xb8\
-Q+\xc0\x80\x1f\xe0\x1e\xd8\x0f\xc8\xe0\xc66\x02J=\
-\x03\xa7\x13gpc\x8c\x00\x03\xbei7.\xbb\x14P\
-\xaa\xc5\xb8\xecZ\x80\x01\x9f\xc0\xa5s\x067Z\x080\
-v\x1b\x97\xb3\x10P\xea\x0d8w\xc8\xe0Fk\x01\xc6\
-\xf6\xe3rv\x02J\xbdP7.g+\xc0\x18\xc6\xe5\
-\xa2A\x067\xbc\x05\x94Z\x02\xc7;dpc*\x01\
-\xc60.\xafFfpcJ\x01\xc6\xe6q)%\xa0\
-\xd4\xfa\xb8\x94\x14`\x0c\xe3\xf2\xb6\xf2\xb7\xd5\xec\x8d\x10\
-\xd0\x03\xd5\xff\xab\xf5Y\xbd;R@t\x80hz\x12\
-\xb0\x02\xee\xa2C\xe4\x18\x9c\xb8\xa4?\x84\xa4?\x85e\
-\x0fC\xd2\xc7a\xd9\x0b\x11\xe9+1\xd9KQ\xe9k\
-q\xe9\x87\x11\xd9\xa71\xe9\xc7Q\xd9\xe7q\xe9\x05\x09\
-\xd9\x15\x19\xe9%)\xe959\x99EI\xf9UY\x10\
-_\x96N\x92$I\x92$\x99\x0d\x7f\x8e\xb3B\xa6\x95\
-\xe9\xbb^\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\x82\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x027IDATx\x9c\xed\x9b\xb1N\
-\x1bA\x10\x86?\x03\x9d-\x8a\x00e*hp\x02\xb4\
-\x90\x22\xd0\xc0\x9b \x04\x02\x92\xc7Hx\x06x\x05d\
-\xf9)\xa0\x8b\xa1\x8a\x08\x12\x88\x12#@\x02c\x1aL\
-q\x17\xc5\xb9[/\xb69\xcf\xee\x9e\xe7\x93N\xb2v\
-wnf~\xcf\xee\x9d\xee\xf6@Q\x14EqN\x03\
-\xb8\x02\xaa\xc060\xd9\x83\xedTlS\x8d\xcf\xd1\xc8\
-<:\x01Z\x89\xe3\x11\xf8\x09\x14-6%`\x8f(\
-\xe1\xa4}p$\x13\xf8{\x9c\x01\xf3\x86\xf1\x0b\xc0\x1f\
-\x8b]ptJ\xa4\x05\xdc\x01Kmc\xbf\x00\xf7o\
-\xd8\x04G\x11(\x03\xbb@\x8dtBu`\x1a\x98\x01\
-n\x0c\xfd\xbf\x80\x1d`\x16\xfb\xb4\x09\x82\x11`\x03h\
-\xf2\x7f\x92G\xc0q\xa2\xed\x09X\x8fmr\xc72i\
-\x11\x92\xc9\x7fu\x16\x9d\x10\x9bt\x16`\xdda\x5cb\
-\x8c\x00'\x98\xe7|&e\xef\xfb\xdcy\x01\x0e\x0c\xed\
-\xfbq\xdfPP&]\x01\xb3N#\x12\xa6DZ\x80\
-RV'/\xb4\xfd\xf6\xe5\x06\xa2Nt\x7f\xdf\xce \
-b+\x80\x9fk@S\xd2\x99\x0a \xe9\xacK\x9e%\
-\x9d\x8dY\xfa\x0a\x96>\xd7\xf4\x13\x9bq\x1d\xf1\xb1\x02\
-DQ\x01\x5c\x07\xe0\x9a^\x04\xb0=\x80\xc8\xf28|\
-gN=\xe1c\x05\x0c\xfdeP\x05\x90t\xe6\xa3\x00\
-\xa27B>\x0a\xa0\x15 \xe9\xccG\x01\x86\xbe\x02T\
-\x00Ig>\x0a\xa0k\x80\xa43\x15@\xd2Y\x97\x88\
-\x0a`{\x22\x94\xc4\xe7'D}\xe3c\x05\x88\xa2\x02\
-\xb8\x0e\xc05\xb65\xc0\xd5\x9b\xa2\x19\xe0\xfc\x8d1\x99\
-\xc5\xe6c\x05\xe8eP\xd2\xd9\xd0\x0b\x10\x02\xe3\x0c\xf0\
-\xf5\xb8\x8f\x15\x90\xe4c\x97m}\x11\x82\x00k\x86\xb6\
-U\xf1(\x1c1\x0a\x9c\x92\x9e\x025\xc2\xf8\xf3\xde\xcd\
-\x16\x9d\xdf m8\x8cK\x84\x15\xec\x1b%\x9bD\x9b\
-)s\xc7(\xd1?o\xda*{DZ\x84Mr0\
-\x1dJ\xc0'\xe0;\xe69\x7f\xcd\xbf\xcd\xd2uC\xff\
-\x09\xf0->G\x90\x9b\xa5mo\x8bo\x81\xc5\xb6\xb1\
-KD[\xe8s\xb5]\xbeS\x22\xbf\x81\xcf\x86\xf1s\
-D\x1fS\xe4V\x80\x07\xe0\x07\xf6r.\xc6c\x1e\x0d\
-\xf6\xc1\xd1\x00.\x80\x0a\xd1\xa2\xf6\xa1\x07\xdb\x09\xa2E\
-\xb3\x02\x5c\x12\xe8GS\x8a\xa2(Nx\x05\x0dw\xfb\
-\xc6$R\xf4\x9c\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-"
-
-qt_resource_name = b"\
-\x00\x05\
-\x00o\xa6S\
-\x00i\
-\x00c\x00o\x00n\x00s\
-\x00\x04\
-\x00\x07\x8b\xaf\
-\x00r\
-\x00e\x00d\x00o\
-\x00\x05\
-\x00s\xc8\xd5\
-\x00m\
-\x00e\x00r\x00g\x00e\
-\x00\x06\
-\x06\xac,\xa5\
-\x00d\
-\x00e\x00l\x00e\x00t\x00e\
-\x00\x0e\
-\x0a\x87\xe3G\
-\x00s\
-\x00e\x00e\x00k\x00_\x00b\x00e\x00g\x00i\x00n\x00n\x00i\x00n\x00g\
-\x00\x04\
-\x00\x075\xdf\
-\x00l\
-\x00o\x00g\x00o\
-\x00\x04\
-\x00\x07\xc4\xaf\
-\x00u\
-\x00n\x00d\x00o\
-\x00\x05\
-\x00zs\x04\
-\x00s\
-\x00p\x00l\x00i\x00t\
-\x00\x08\
-\x0b\xc1Wd\
-\x00s\
-\x00e\x00e\x00k\x00_\x00e\x00n\x00d\
-\x00\x06\
-\x07\x8cH5\
-\x00r\
-\x00e\x00n\x00a\x00m\x00e\
-"
-
-qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x09\x00\x00\x00\x02\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00b\x00\x01\x00\x00\x00\x01\x00\x00\x09\xcf\
-\x00\x00\x01\x81_5\x1f{\
-\x00\x00\x00\x10\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x81\x96\x8cK\xb5\
-\x00\x00\x00p\x00\x00\x00\x00\x00\x01\x00\x00\x15k\
-\x00\x00\x01\x81\x96\x8cK\xb9\
-\x00\x00\x00\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x02\xd7\
-\x00\x00\x01\x81\x96\x8cK\xb4\
-\x00\x00\x00~\x00\x00\x00\x00\x00\x01\x00\x00\x18*\
-\x00\x00\x01\x81\x96\x8cK\xb8\
-\x00\x00\x00.\x00\x00\x00\x00\x00\x01\x00\x00\x05\x0a\
-\x00\x00\x01\x81\x96\x8cK\xb3\
-\x00\x00\x00\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x1b\xf2\
-\x00\x00\x01\x81\x96\x8cK\xb6\
-\x00\x00\x00@\x00\x00\x00\x00\x00\x01\x00\x00\x080\
-\x00\x00\x01\x81\x96\x8cK\xb7\
-\x00\x00\x00\x8e\x00\x00\x00\x00\x00\x01\x00\x00\x1a>\
-\x00\x00\x01\x81\x96\x8cK\xb7\
-"
-
-def qInitResources():
-    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-def qCleanupResources():
-    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-qInitResources()
+# Resource object code (Python 3)
+# Created by: object code
+# Created by: The Resource Compiler for Qt version 6.3.1
+# WARNING! All changes made in this file will be lost!
+
+from PyQt6 import QtCore
+
+qt_resource_data = b"\
+\x00\x00\x02\xd3\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x02\x88IDATx\x9c\xed\x9a9\x8b\
+\x14A\x18\x86\x1f\xcf\x11\x9c\x83\xcd\x04\x13\x97\x11\xd4\x1f\
+\xa0\xa2\xb2\x89G\xe4\x1d\x9b.\x86\xba?a\x91\x055\
+\xf5\xc0\xc8\xcch\xe3\xdd\xf5\x001\x1aD\x14\x05\xc1u\
+#\x15Q\x0c]50p\xa1\x0d\xca\x86\xa1\xec\xea\xee\
+\xed:\xbe\xda\x99z\xe0\x0b\x06j\xe6{\xeb\xad\xa3\xbf\
+\xae\x1aH$\x12\x89Db\xa32\x0fLH\x8b\x90$\
+\x03>\x01S\xd2B\xa4\xc8\xfe\xc5\x1ap\x03\xd8&+\
+'<\x99\x16/\x80\xbd\xa2\x8a\x02\xa3\x1b\x90\x01?\x80\
+\xcb\x92\xa2BRd@\x1ec\xb1A\x96\x19\x10|\x83\
+\xec\x03\xd3\xc0}`\x00|CM\xc7*\x91\xbe\xe3\x0f\
+0\x0bl\xf5\xd1\xe9\x1e0\x03\xbc\x89\xa0\xa3U1\x00\
+&]u\xbc\x03\xcc\x01\xab\x11tl=\xb1\x0a\x5c\x1a\
+\xeeH\x93iq\x01\xb8\x03\xecn\xf0\xdd\x0dM\x0b\xb8\
+\x8b\xfc(\x8a,\x816\xf0$\x82N4\x09\xeb*\xb1\
+\x07\xbc\xaa\x99\xec-p\x1d8\x8dz*t\x9a&\xad\
+I\x95\x9e\x0f\xc0Q\x9b\x04-\xe0Y\x8dD\x8f\x80\x83\
+6\x89\x1aR\xa6\xe9\x01j\xf0\xac\xa8Z\xf3\xcb\xc0\x09\
+\xdb$\x16\x14i\xfao\xa7o\xcaEC\x82<\x16\x81\
+\xae\x8bD\x168\xdd\xe8\x86\xe9\x00_\x0a\x12\xe4q\x0f\
+\xd8\xe2\x22\x91%\xb9\x1e\xe7\xd5\xde\x1c\xe5#\x1fC\xe7\
+\xc1\xd1F\xa7\xd3\xc3\x5c\xe1-#?\xed\x87q\xb2\xd1\
+\xe9\xcc`\x1e}\xc9\x0d/\x18\xa6\x17\x9b\x87\x92\xa2B\
+\xd1\xc7<\xfa\x12\xcf\xf9\xe0Lc\xae\xf0F\x92\xcd\xda\
+\xe7#\x86v\x0b\xbe\x85H\xa1\x1b\xb0\xdf\xd0n\xe0[\
+H,|\xa5x\x09\xf4%E\x85\xe4\x17\xc5\x06\xec\x94\
+\x14\x15\x925\x8a\x0d\x88\xa5\xf2s\x8e\xbe\x07\xfc6\xb4\
+\xdb\xe1[\x88\x14\xba\x01?\x0d\xedv\xf9\x16\x22\x85n\
+\xc0GC\xbb\x03\xbe\x85H\xa1\x1b\xb0bhw\xcc\xb7\
+\x10)t\x03\x9e\x1b\xda\x9d\xf1-$\x16&1\xbf\x0b\
+\x1c\x12\xd4\x15\x94\xd7\x14\x1b\xf0XRTH\xaeb\x9e\
+\x05'\x05u\x05\xa3\x07|\xa7\xd8\x80\x15<\x9c\xc0\xc4\
+\xc85\xcc\xb3`\x89\x11\xae\x0cs\xda\xc0g\xe2?\x15\
+\xf6\xcay\xca\xef\x05\x96\x18\x83\xe5p\x9br\x13\xde\x03\
+\xa7\xc4\xd4\x05\xa0\x05<\xa5\xdc\x84\x0cus|XH\
+\xa3w\xba\xc0K\xaaM\xc8\x80w\xc0M\xe0,\xea\xff\
+z1\xdd!X\xd1F\x15BuL\xb0\x89\xa8\xd9\x0e\
+\xdcb\x8c\x0d\xc89G\xf9#r\xe4\x0d\x00uF8\
+\x8b\xb9b\x1cy\x03r\xba\xc0\x15\xea\xff\x85&:\x03\
+69\xfc\xad=\xc0q\xd4\xe5\xca>\xd4Qz\x9b\xf5\
+=\x09\x5c\xeaI$\x12\x89D\x22\x91(\xe5/pw\
+Ld\x1eW\x19\x04\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x02/\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x01\xe4IDATx\x9c\xed\x9a\xbfJ\
+\x03A\x10\x87\xbf\xf8\xa7U\xf4\x05D\xb0\xb6\x11\x14\x04\
+{}\x00;m}\x05\x0b-\x15|\x05[I\xe5c\
+(\x88y\x06\x0bE\xad\x13b)\x81X$\xab\xe1\xb8\
+\xdc\xee\xe4f3\x86\xcc\x07\x0bGng\xf6\xc7\x8f\xdd\
+\xd9\xbd%\xe08\x8e\xe3\xcc/\x8d\xcc\xf9\xfb\xc2q\xa5\
+\xfdk\xb3\x90+\xf1\xac\xe0\x06X\x0b\xb0\xc6\x0d\xb0\x16\
+`\x8d\x1b`-\xc0\x1a7\xc0Z\x805n\x80\xb5\x00\
+k\xdc\x00k\x01\xd6\xb8\x01\xd6\x02\xac\x91\x18p\x0f\xac\
+\xe5\x12\xa2\xc8\x0ap\x97#q\x1fx\x03\x0e\x841e\
+M\xab\x7f\x91=\xe0E\x18\x93L\x10\xd3\x03n\x80e\
+ALn\x03\x16\x81s\xe0[\x10#\xa6(\xaa\x05l\
+\x09cr\x18\xb0\x01<\x08c&\xa2LX\x178\x13\
+\xc6h\x1ap\x0c\xb4\x851\x133N\x5c\x9f\xf1\x052\
+\x97\x01\xa1\xd0UiJ\x22\xdc\xb6\xa6T\xf7v\xe4\xfd\
++p\x02<\x8d\xfc\x96\xe3Vx\x1fh\x02\x9b\x11=\
+\xeb\x91\xf7\x00\x9d\xd1\x815Z\xb1@j\xce\x80\xb2B\
+W\xb7E\x07\x9e\xb4\x85\x02\xa9e\xc0\xb8BW\xdb\x80\
+0\xb5\x92\xd7\x8c\x80/\x06k\xb5\x0c\xe9\x12\xa8\xcaU\
+\x87\x86\x1f\x853\xe5m\x01;\x8a\xf9\xb6\x81G\xc5|\
+\xbf\x84\xa9\x18\xab\xf0\x90\xb6S\xf4\x80k\xe0j\xf8\xac\
+\xb9\x0b,\x01\x97\xc0\xc5\xf09F'\xde%i\xa7\xf8\
+%VP\xca\xbe\x134w\x81\xc0.\x7f\xe7\xfd\xa4\x0a\
+\xafE\xd5`\x16\x07\xa1\xdb\x88&u\xca\x06\xe9\x02\xa7\
+\xc2\x18\x0d\x03\x02\xa6G\xe1g\xe6\xf4ch\xae?\x87\
+\xff\xfb\x85\xc8h\x81T\xa7\x09\xac\x0ac\xa6m\x00C\
+\x8d\xcd\xd4\xce\xfe\x1f\xa1\x5c\x89g\x057\xc0Z\x805\
+n\x80\xb5\x00k\xdc\x00k\x01\xd6\xb8\x01\xd6\x02\xacq\
+\x03\xac\x05X\xe3\x06X\x0b\xb0\xc6\x0d0\x18\xf3\xa3\xe2\
+\xdd\xe7\xd4TL\x89\xe2\xc5\xc6;pX\xd1\xff\x88\x81\
+A\xd9\xef\xf7\x1c\xc7q\x1c\xe0\x07\xaf\xfd\x93\xbd\x10\x9a\
+g\x8e\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x03\x22\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x02\xd7IDATx\x9c\xed\x9a\xcbj\
+\x14A\x14\x86\xbf\x98\xd1\x85\x0b1+\xddd\x130\xa2\
+\x09\xe8:+\x05}\x03\x09\x127\xbe\x85\xee\xcc\xd2\xd7\
+\x10\x03F\x13\x88/\xa0\x0b\xf5\x09\x8c\x11\xdd\xc8\x80\xa8\
+\xe0e\xc4\x04Q\x83\xa6]t\x17\x8cmO\xd7\xa9S\
+\x97\x99L\xea\x83\x82f\xbaN\xd7\xff\x9f\xaa\xae\xae\xae\
+\x1e\xc8d2\x99L&6\xd3\xc0:\xb0\x0d\x14\x96\xb2\
+\x0dl\x00\xa7\x87\xa24\x02\xd3\xc0\x17\xec\xc6\xeb\xa5W\
+\xc5\xee{\xd6q7o\xca\x83!\xe8\x0d\x8ed\xd8\x0f\
+*\xdfb\x8b\x9b\x88\xdd\x00\xa5\x11\x976]\xeb{q\
+(\xe6\xc5\xf7\x03\x9d@\xd7\x99\x02f\x809\xe0lu\
+<\x03\x9ci\xa8[\xefa\x1b\xbb\xc0[\xe0MU^\
+\x02[\xd5q\x17\xd8\xd3I.q\x19^\xc6\xa4)\xc6\
+\xec)\xe0\x98\x8f\x08\x0f~\x01\xef\xf87)&I\xef\
+%\x17pI\x80k\xcf\x0d\x1b\x91\xb7\x03?\x07\x1c\xf8\
+\x04d\x0e:\x9aE\xc6w\xe0(\xf0\x13\xf8Q\xfdf\
+\x8e\x9b~Ky\xde\xd4\x89J\x17\xfd\xd26v\xe9\xba\
+\x9a\xd1L\x82\x9f\x141\xa9p\xd6\xa6I\xc0gEL\
+*\x92$`\x94G\x80s\xe7\x8c[\x02\xf2-\xe0\x1a\
+\x90b\x04l)\xda\xd0\xc6\x8e\xdc-\xb0\x0c\x9c\x03V\
+\x14\xed\xac\x01\xe7\x81\x9b\x0e1In\xcf\x05d\xcf\xe4\
+[}1\x93\xc0]a\x9c\xd9\x0b\xec\xdf\xab\xb8!\x8c\
+[\x08\xec\xb5\x91Y\x81\x90M\xfe\xdfl\xe9\x00\xab\x82\
+\xd8\xd5\x01\xb1\x9b\x82\xd8\xd9`.[\x98\x12\x08)(\
+\x87p\xdd\x88m$\xd4{\xde\xc4\xac\x08\xdb<\x1e\xcc\
+e\x0b\x13\x94\xdbT\xa1\x93\xe0k~\x974\x9b\xbc\x00\
+|\x10\x8a\x92&\xc1\xd7|QiJ\xc6s\x07a\xb6\
+$\x840_T\x9a\x92\xf1\xc8Q\x5c\xdb\xe4\xa6\x9d,\
+\xeb\xe5q@\x7fV\xee+\x04\x0e\x1a\x09\xfdhz\xbe\
+?\xc1\xceh\xf7\x04\xb5\x0b\x8e+\xc0=\x9a\x930\x09\
+\xdc\x01\xae\xa5\xd4\x94:\x01P\xf6\x96\xe6\x9c\x0d\xd5;\
+\x8a6\x01\xda\x17\xa25`\x09\xf8\xddp\xee\x0fp\x1d\
+\xdd\xb2\x19\x12\xbf\xa5.2z\x93\xe0b@\x7fV.\
+:\x8ak{\xd4iV\x8cM\xe5B@\x7fV\xe6\x1d\
+\x84I\x9e\xf3!\x920\x1f\xd0\x9f\x95\x93BQ.\x8b\
+\x1c\xdf$\x9c\x08\xe8\xcfJ\x87\xf2\xb3t(\xf3\xbeI\
+\xd8k\x88\x8bN\xafEP\xea\xd7\xe1^PgB^\
+\xb7\x08*\x80\xdb}u]Wx\xf5\x91\xb0l\xa9\xff\
+*\x82?+\xcf,\xa2L\x12\xb4\xcb[\x93\x04\x9b\xf9\
+\x02x\x1a\xd9k#\x1b\x02a\x05\xf0BX\xcf'\xf6\
+\xa1\xd6\x84\xcf\xff\x03\xa4\xab\xc19\x8f6\xa4\xb1\x1f\xb5\
+\x0d\xf8$`\x94>\x90\xa8\xb5\x8cK\x02\xd4\x1fkR\
+\xdc\x02)\x18\xca\x08p\xfe\x16\x1f\x91\xa1h9\x02|\
+E?\xc3\x87*=\xe0pd\xaf\x03Y\x12\x08\x8c]\
+\xaeFwi\xe12\xe5Bd\x87t\xa6w\x80'\xc0\
+\xa5\x04\xfe2\x99L&\x93\xc9\x8c)\x7f\x01\xd3\xf3\xeb\
+\x98\xbb\xef\xcd8\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x01\x9b\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x01PIDATx\x9c\xed\x9aA.\
+EA\x10E\xcf\x17\x06&\xa6\xc4\x0e\xd8\x01\xdb\xc0\x16\
+,\x80\x0d\xd8\x86m\x08\xcb`\x03\x18\x99\x9a\x0a\x03\x09\
+\x03\xf9I\xc5Dy\xf4\xef\xd7u\xefI\xde\xb4\xab\xfa\
+$/\xf7\xbd\xee\x02c\x8c1\xc6\x18\x93\xe2#\xf1\xac\
+\x9a]\xe0\x0a\xb8\x006[\x17\x9b\x9b\x80#\xe09\xd4\
+~\x02NZ\x16\x9c\x8b\x80-\xe0\xb2G\x0fs\x10p\
+\x00\xdc\xf7\xea\xa1\xa7\x80u\xbe\xde\xf3\xf7\x8e=t\x13\
+\xb0\x07\xdc&\xeb\x97\x12\xb0\x00N\x81\x97d\xedR\x02\
+\xb6\x81\xebd\xcdr\x02\xbe\xc7\x9b\x8c\x80\x9f\xe2\xad\xb4\
+\x80\x03\xe0!Y\xa3\x94\x80\x0d\xf2\xf1VN\xc0>p\
+\x97\x5c\xb7\x94\x80\xa9\xf1VB\xc0\x0ep\x93\x5c\xab\x9c\
+\x80c\xfe\x16o\xc3\x0a\xf8\xafx\x1bR\xc0!\xf08\
+a\x13\xc3\x0bh\x11o\xc3\x08h\x15oC\x088\x03\
+^;lz\x92\x80\xc5\x04\x01#\x90\xde\xd7Z\xcb.\
+F\xc0\x02z7\xd0\x9b\x16\x02\xce\x81\xb7\x06\xeb\xce\x02\
+\xc7\xe0/\x8aK\x7f\x08Ed?\x85#\xd2?C\x11\
+\xd9\xdf\xe1\x88\xf4\x81\xc8\x12\xe9#\xb1\x88\xec\xa1hD\
+\xfaX<\x22{1\x12\x91\xbe\x1a\x8b\xc8^\x8eF\xa4\
+\xaf\xc7\x97H\x0fHDdGd\x22\xd2CR\x11\xd9\
+1\xb9\x88\xf4\xa0dDvT6\xb2\xd2aic\x8c\
+1\xc6\x982|\x02\xbb\xfd@xy\x91\xc8\x87\x00\x00\
+\x00\x00IEND\xaeB`\x82\
+\x00\x00\x0b\x98\
+\x00\
+\x00.Ex\x9c\xedY\xd9\xae\xdb\xd6\x15}\x0f\x90\x7f\
+`\xe5\x17\x1b\x15\xa93\x0f\xca\x95\x03$F\x8a\x14\xcd\
+K\x92\xb6@_\x0c^\x91\xd2e,\x91\x02I\xdd\xc1\
+_\xdf\xb5\x0f\x07\xf1Nn\x9b\xc4\x06\xdcHN j\
+\x9fy\xef\xb5\xd7\xda\x87\xf7\xe2\xeb\xdb\xfd.\xba\xce\xeb\
+\xa6\xa8\xca\xd5\x8c'l\x16\xe5\xe5\xba\xca\x8ar\xbb\x9a\
+\xfd\xfd\xe7\xefb7\x8b\x9a6-\xb3tW\x95\xf9j\
+VV\xb3\xaf_\x7f\xf9\xc5\xc5\x9f\xe28\xfa\xb6\xce\xd3\
+6\xcf\xa2\x9b\xa2\xbd\x8a\xbe/\xdf5\xeb\xf4\x90G/\
+\xaf\xda\xf6\xb0\x5c,nnn\x92\xa27&U\xbd]\
+\xbc\x8a\xe2\x18C1\xb8\xb9\xde~\xf9E\x14EX\xbb\
+l\x96\xd9z5\xeb\xc7\x1c\x8e\xf5.\xf4\xcd\xd6\x8b|\
+\x97\xef\xf3\xb2m\x16<\xe1\x8b\xd9\xa4\xff\xfa\xd4\x7fM\
+;(\xae\xf3u\xb5\xdfWe\x13\x86\x96\xcd\x8bi\xef\
+:\xdb\x8c\xddiK72\xf4\xe2\xde\xfb\x05\x13\x0b!\
+b\xf4\x88\x9b\xbb\xb2Mo\xe3\x07c\xb1\xcf\xa7\xc6\x0a\
+\xc6\xd8\x02m\x93\xae\xffe\xb7e\x03\xcf\x1e\xf0\xff\xd8\
+\x7f0$Mu\xac\xd7\xf9\x06\x03\xf3\xa4\xcc\xdb\xc5\x9b\
+\x9f\xdf\x8c\x8d1K\xb26\x9b\xce38\xf6\xde\xba\xf7\
+\xbc]\xa6\xfb\xbc9\xa4\xeb\xbcY\x0c\xf6n\x82\x9b\x22\
+k\xaf\x10js\xb8\xed\x0cWy\xb1\xbdj\xa7\x96\xeb\
+\x22\xbf\xf9\xa6\xba]\xcdX\xc4\x22n\xf0_o?\xe1\
+\x84w\x96\x22[\xcd~\xfa\xc7_~\xac\xaa\xb67\xf4\
+k-\xc7\xbe,\xf1\x22\xd1\xd1K\xc1\x0c\xcb\xd7|\xe3\
+7\xf3H0\xc1b\xa6b\xe6^u\xc3\x86\x93.\xb3\
+jM;_\xcd.\xab\xdb_\xf2\xdd\xee.\x19=8\
+N\xbdK/\xf3\xddj\xf6M\xba~\xb7\xad\xabc\x99\
+\xcd^S\x87\x8b,\xdf4\xa1g\xb7/\xfa\xc9Y\xd7\
+\x86\xd6q\xf8!m\xaf\xe2|\xb3\xc9\xd7m\xdf;\x8a\
+\xba\x9f\xabY\x8b\x0e\xf5\xdb\xa6\xad\xabw\xbd\xbb\x86\xd9\
+&\xa3\xb4t|\xd2\xd8\xbc\xbd.\x9a\xe2r\x87M\xb7\
+\xf5q2\xac\x9b\xe6m\xefp\xf8\xe1\xd4\x94\xb6m\xba\
+\xbe\xc2BiM\x9e\xcfcfO\x8dy\x99\xbd\xad6\
+\x9b&o\xc3(\xfaL&\xdd\xc3\xd7W!=\xc7(\
+\xd0\xe7\x97\xaa(\xdb;BD~\xdb\xd6\xe9\xa1\xdaQ\
+n\x9e\xda\xf7E\x8b\x93\xed\x0a|c$C\x9e/>\
+\x8egb\xf9\xa9|\xc3\x13%\x90d^}V\xde\x89\
+\xed\xff\xee\x1f\xfeG\xf1\x8e\xf84\xbe\xf9\x1c\xb3*\xfe\
+d\x9c\xf3Y\x22\xe7Wd\xd5\x1f\x87\x91c\x7f\xc6\xce\
+\x07\xfcc\xfeo\xb0s\xb1\xa0\xaa\xa7{\x1ck**\
+\xa82\xaa\xe9&\xc5\xd1e\xda\x8cg;\xa4[T\xd0\
+\xbb\xaa^\xcd^l\xc2gh\xb9\xac\xea,\xaf\x876\
+\x13>\xf7\xdb*\x94\x98E{\xd7]\x1d\x86\xf9O\xd1\
+\xd9\xe6c\x07\xf6L\x87\xe6*\xcd\xaa\x9b\xd5L<j\
+}_U\xfb\xd5L\xe9Dh\xe5\xa4z\xd4\xbeF\x85\
+\xaa\x12\xe6\x98\xd7\xda>n\xc5\x9a.\xd1\xdeK\xed\x1e\
+5\xa2\xcc<\xd2\xed\x22>\x96E\x8b\xea}\xa8|\xa7\
+\xe3\x8fuM=v\xe9]\x8e\xd3\x87\xaf1B\xcdU\
+u\xb3\xad\xc9\x91\x9btw\xf2\xe48\xf8\xa6(q\xa8\
+\xb8\x07\x8bT\xea\xf1\xd9\xfb.c\xf5-\x05\x7f\xae\x0f\
+U\xe2\xcf\xb5\xe1\x94\xe2\xb1k\xfa\xc6}z\x0b\x88\xbc\
+\xcf\xb3\x89L\x8e}h\xff\xf1\xe5%\xd5\xf9S\xa4\x8f\
+\xedM\x99\x1e\xe2\xb2\xca\xf2\xa6\xef0`l\x9f\xb7i\
+\x96\xb6\xe9\x04N\x83\x89\xcb\xb1\xde\xc6\xb5j\xf9\xe3\x9b\
+\xef^\x0f\x98\xbdX\xaf\x97\xff\xac\xeaw#\x86\xa3\x88\
+\xba\xa4\x97\xd5\x11\xc7\x9f\xbd>\xd9/\xb2\xf5\x12\x17\xa1\
+}\xda\xbe.\xf6@\x08]\xa2\xfe\x8c{\x0f\xc0=6\
+\xdc\xefM\xa92\x99\xb7\x9b\xb9\xce\xbb;\xd5\x93\xb7\xcb\
+l\x8d\xd4\xc1\xa8\xc5Om\xb1\xdb}O\xcb\x9c\xf8e\
+\x9c\xb6hw\xf9\xc4z\xb1\xe8\xcf0\x9cq1=\xe4\
+\xc5b\xf0B\xf7\x13\xb7\x97\xe2\xd0\x0c\xfbj\xda;\xe2\
+\x94\x0dV[\xbe`L\xa94\xfd\x8a~\xc4}\x82,\
+\xf9W\x1d\xc3P\xab\x94\x8e\xf5?;\x0c-\x91^\x5c\
+H\xcd\xad\x1e\xec\xbb\xa2\xcc\x11\xa7\xe5\xe5\xb1m\x07[\
+\xa0\x85\xc0\x0aK5\xd8\xb2\x14\x19V\xd7\xe9\xdd\xb2\xc4\
+\x0d~\xb0\x8e\xab\xce&Q$^tb\xcc\x16\xca\xaf\
+\xd3\x8f\xbb\xc9\x8f\x1a-6Q^:\xa1\xf4h\xbc;\
+\x19G\xacl\x1f\xa2\xaa\xbf\xbc\xfd\x95\xeev\xd3\xb5\x1f\
+\xe4W\xe7\xad\xach\x0eh\xc0u\x97N\xfb\x04\x82\xab\
+\xe3a\x0f\x84\xf6\xc3G\xecm\xc78\xd2\xd4[\xa7&\
+\xd4\x0a:-\x1bB\x11P\x9b\xb6uq\xfb\x92%\xce\
+)a\xb9\x96sF\xff&?\x13\xc1\x1c\xd7\x96q<\
+Z%\x8c\xf5V\xbf:a\xf5\x82<6\x01\xde\x89r\
+\xb1)\x82\x17R\xa7\x19>\xb3I\xc7\x13\xcbT%\xc2\
+\xd8Vu\x0c\xbe\xb9N\xdbc\x9dO\x92}8A\x8d\
+.\x82\xe9\xa9\x99\x92.\xe2<\x11\xb4=3\xe7\x89\xe7\
+\xd0]\xc3#l\x14|\xa3-v,\xb9\xe5\x92\xebh\
+\x0d\xa3\xe3\xd2ZGF\xcd\x11!\x11q\xd2\x22\xa6\x04\
+\x86J\xe7\xa4d\x1c&\xe5-\xf7n.\x12\xee\xb4p\
+\x96G\x7f\xa35\xe0?n\xe4\xdc$\xdehn8\x8f\
+\xbe%\xab\x94^r?\xb7\x895\x82s'#\x0ey\
+\x93\x06\x00\x9a\xbbD\x0a\xcb\x843\x91O\xb4\xe5\xc6\xc2\
+\x86~\xd2jc\x1c\xe6t\x89\x93Vpc`U\x82\
+)\xa9%\xe6\xc43\x07\xd1\x1b\x8d\x95\x1c3\xc2(\x0d\
+\x1bN'\x14#\x1bt\x8e\x09\xeb1\x9a1\x8enj\
+\x0ei`\x98R\xa80\xa7\xc7\xfc\xdc\x0a\xec\x1e\xbb0\
+\xce\xd2\x9c>\x11\x12\x13a\x9f8\x9cUR\xa0/\xf6\
+\xa9\x18\xf7\xd8\x13O\xb4\xc1\xf4\xd2>\xe9\xc9\x7fM\xfd\
+=\xcd\xdfI\x22-{\xc5|\x90\xad\xbfw\x92NI\
+\xe8\x01\xe6&x\x0e\x8fT)\x00\xd2\x0a\x87\x80\xe7\xf9\
+<\xc6\xc1\xb5\x15\x8a\xebWO\x22\xb0\xaa\x8bmQ\xa6\
+\xbb\x18\x88\xfa\x01\xfe\x86\x5cJ\xe1=b\xc8\xbdG\xe0\
+\xc8\x8b&1^+n\xe5\xdc'\xf00\xe2\xc0#\x9d\
+ nH\x13\x05\x1b\xc3\x18\xa5<l\x9a;&\xbc\x81\
+\xcd{\xed\x95\xb3\x18\xcb\xb4\x17\x92\xcf\x03<\xf0\xb1\x91\
+J\x8c\xd5\x8ea:\xb8\x1d\xf3:!#\x99xk\x95\
+\x05na\x03B\x113\xd8\x84w\x1aO4\xd6*c\
+,\xd9\x98s\x8ei=\xe7\x02\x07\xd3\x16a\xe6\x89u\
+\x1e#\xe6\x5cb\xd3\xd2\xd8'\x0f:\xa9\xfaP\xcc<\
+\xfb>\xe7\xe9,^\xe3\xf3\x1b\x12\x98V\x033>\xcc\
+\xe0\x1f\xe0\x1dl\x5c\x0b\xab\x91\x09^\x19!\x8c\x0f\xfe\
+\x86#\x8c\xf3\x16Q\x10\x0e\xb9\xa85l\xc2i\xb8\x9c\
+\x22\xa3\xac\xc7\xc1-\xfc\xed8e\x87\x80\xcd2\xad$\
+2\x061\xc0\x08\xe9\x14l\xf4`\x04\xc5E\xc2+\x86\
+\x86z\x89~\xd6\xc1\xc4\x95\x05\xf2CHa\x14J\x22\
+.4-\xf9\xd6\x93k5\xea\xf8`\x13\x8c3\x0b\x9b\
+\x03\x05jKK\x80\x0f\xb4\x11\x96\xe2\x02\x94\x08)\xa3\
+\x14Q\xc0$\x861J\xab\xfe)b\xdd?$\xac\xb1\
+\xc4H\xc8[\x8e\x04\x04\xa3Xf\x05qO\xff\x14\xfa\
+\xf1\xd0Sy\xa2)\x8c6\x81\xb8\xc0\x12tl\xe2b\
+\xd0\x94W\xd4\x07\xa7b\x8a\xb8L(/\xa2\x18\x9d\x14\
+\x00\x8a\xf9\x80{#\x09\x9d\xb0\x09\x9c\x14\x9b\x84\x0dp\
+\x02\x8d\x93\x0d\xa4\xc24'6\x07\xbd\x0b\x11l\xa0E\
+\xe7\x19\xf5c\x06kGP\x80(\x96\x89A\x1d\xaf\xe7\
+1\xa8\x10\xdfO\x18\xb0\xba\xc1\xce\x99\x9f\xd3\xfaX\x9e\
+\xd90\x1b1\xae\x0e6\x06\xd2\x0c+x\x10\xa4ra\
+U&yg\x13\xda\x09\xf8\x9d\x8e\x05\xd6\xe3\x86l\x8a\
+1\x00\x99v\xa2\x19G\x94\x82\xcdi\xc0\x9d\xc6\x1ax\
+T\x84\x85q*\xa0\xdc\xcf)\xa1\xc0\x9e\x9el\x8eS\
+:\x12\xcd\x09d\x8c\x0e\xfd<\xa6F\xd1@\xd4\x07\x8b\
+\x0bk\xf0ppM{\xf1\xdc\xa9`c\x81\xcai+\
+\x12\x89\xfa\xa4)8\x85\xa2\xe2\x1dE\x07\xf1\xf7H<\
+j\x96Z)\x13\x9cg\xb4\x8b\xc2q<\xf0I\x1e`\
+\x01A\xf0\x89\xb3\xde\x98`\x12\xdeBYHi\x94\x83\
+/\x88\x9d@1\xc0&E\x1a\x11\xc3\xc4\x9d?\xadW\
+\xbc\x9b\x0dZl\xc9&-\x08\x88V\x00\xca5\x96'\
+\x9bR\x18\x1b\x10\x00BgB\x06\xe0\x98\xee\x04\xa0?\
+\x17v\xc1Dg\xb0<\xac\x88K\x81\xc8c\x15\x8e\x04\
+&\xcac3\xc7o\x83g;>\xc3\xc7J\x03[\x01\
+d\x5c\xd1^\xc0J\x9e9\xab)<B \x13<L\
+\xc6#\x9cR\x85e\x80b\xca]\x8d<F1\x8f~\
+Dd\xa09 \x14\xb9\x8bc\x07\x1aS\x02N\xa7\x8c\
+\xf4\x88:\xfc\x82\xb4\xb2\x90c\xc0\x83\xb2\x19\x99\xc9\x14\
+\xb1'8\xc1\x91W`3\x1e\xf1\x14\xd4\x0f\xb4\x0c\x1a\
+'\x1b\x91\x83\xa2\xd4\x85\x5c{B\x85\xa6\xa2\x85D\x9c\
+l\xcc\x1bB\x85\xa1d\xb2\x5c\x90\xcd@0\xa5&\x9b\
+`\x10GM\xebj\xe2\x0eI\x0c\x0dM\x87o)\xc5\
+q\x0bQ\xa0k\xe8\x00X\x9ci21p\xab\x95d\
+\xb2\x92\xf27\x10\x10@$\x99|^\x22\x07Y\x0c%\
+n}\xdc\xe5$l\xefq_\x1cts\xaas\xbdh\
+\x1en?$\x9bd\xa3k\xf12\xe8\xe7o\x97H\x91\
+P\x9e\xa0\xa0\x0e8\xc2Y\xc1\x85\xea?K\xe4\x1e\x85\
+\x06\x06y\x90\x07\xfc\xc0\xa4\x0ab\x08\xa2\xa2\xcc3\x80\
+\x88\x11\x04Q-q/\xa5B\x0a\xd3\x02\xb7]\x8aj\
+i\x94\x13S#\xe4\x8f!m\x14eW@\x0b\xc2D\
+\xfc\x09\xaa\xa3\x0a\x84\x18\xcb@\xffBE&=\xea\x17\
+B\xa6\x85\x92p\xcaj\xf0\x9bE\x10\xe2\xa0\xf6`#\
+\x1a\xc9\x9d\xf7\x9c&\xb3\x9cK\xca\x08\xd43\x00\x1f\xfb\
+\x15\x9a8}\x93\xffQUq\xfa\x02\xa6\xafl\x016\
+q\xdf\xc9\xa1\x8c%\x1aD\x1aP\xa6Q\xc6\xa1\xd6$\
+?H\xd4:\xa8\x0e\xc8$ \x03\x90\xa5\xc48\xa9\x99\
+S!\xefQ\x85\xe8P\xf9\xa2X\x01\x13S7\xd0\x0c\
+#\xb2P(\x80\x99\x0f\x8eF\xf6p\x14 \xf7\x8d\x9a\
+y\x0d\x9e\xec\xc8\xcf\x93\xb2x\x1b\x04\x85\x07\xdaE\xa0\
+\x18\xb2M\x05\xe1AE\xc9C0\xc0W\xcc*\xdd)\
+\x167a\x13\xd8\x8d\xf0av\x08!\x1a\x83\x8d\xdek\
+\xd8N.A\xcb\x9a6\x06\x01\xa2N\x88+\x12\x97\xf8\
+\x0f8\x80\xfcQ\x1fH\xba\xa3\xf8+|\x13lqn\
+\x83)\x02sj\xa3qg\xa4\x15\xb5\xe6L\x072\x15\
+\xa8w}\xa7%\x00EO\x89\x9d\xbahhv\x87.\
+\x09>'\xf6\x86\x1a\xc1K\x01\x84\xa4B>\x5cx\xa0\
+.\xd8\x04\x9d\xd2\x0ac8\x91!\x0a\x04\xde\x11.8\
+\x8e\xc9p\xcd\x80\xcc\x89\xc1\xd5\xac\x13f\xd2\x96\x9e\x86\
+\x1f\x98\x06!\x81\xaf\x82\x8b\x10$K!A\xdd\x88\xc8\
+\x05\x02G\x05\xe2:JW\xdd\x02\x94aH\x1f@\x92\
+u*\x02J\xb2\xc4\xbeHZ'B\x02\x1b\x94(\x86\
+\xbc#\x9d\x97\x8a\xca^\xd2\x09\x9c\xc4FA\xf5\x15R\
+\x8bl\xa8hM\x00\x0f\x84\x08\x0a&H\x80\xe8\x0a\xa0\
+\x82;8J\x1d\xdb\xa9\x8d\xf0\xdcw\xdb\xa0\x92\x95\xea\
+\x83\x90\x8c`\xf3pz\x89@)\xafi8\xa3\xfbz\
+\xe7_\x0e\x06\x0e\x9a\x03e\xed1\x0a~\xd6a,\x0e\
+\xd7\x83\xcf\x86\x8c\x0f3C&\xc8\x82;\x8c\x14\x9db\
+:\x1a\x05\x94Q-\x12fR@]H{\xd4\xd8\xb8\
+4\xdd\xb3Y\x10\x0eX\x1c.E\x8c\x94\x0f\xe4\x11\x9c\
+\xa1\xb9&y\xc2\xfc8Q8$\xb4\x86\x8a\x8bn}\
+\xd9\xad\x0f\x9fxdN\x1f\x0fgCGA\xb5]W\
+?\x9c\x8c\x0e\xaa\x8a\x9a<z\xff\xb9\xf1\xfdx\xc5G\
+\xceI\x14\xcf\xbc\xab\xcc\x90\x9f,@w|\x1a\xdb9\
+\x15s\x80\x13\x95RPo\x85\xea\xe6\xac\x0a\xcf\xfe5\
+\xe1#\xeb\xc2}\x09:+\xc3Y\x19\xce\xcapV\x86\
+\xdfS\x19\xe8\xca\x0e\x8cR\xec\xc3E\xc0\x01\x1b\xaeC\
+\x89r\x1e\xb9B4\x1c\xaeY\x00\xb3\x9d\x8b\x00~)\
+\xe8\xdd#\xee@\xb8\xa6\x8a\xf3k\xb5\x0f\x88\x85\xf9T\
+R\xc1\xce\xaf\xd6\xce\xaf\xd6\xce\xaf\xd6\xce\xaf\xd6\xce\xaf\
+\xd6>\x9e\xa0^,\xb6\xfd\x9f\xba\xe9\xfb\x82\xfe0\x8f\
+\xef\x7f\x036@F\xa0\
+\x00\x00\x02\xbb\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x02pIDATx\x9c\xed\xd9\xbfk\
+\x14A\x18\xc6\xf1O\xbc\xa0\xa0\xc6Ki\x17\x7f \xe8\
+?`\x88\xb5\xc6BIge\xa5\xd6jii\xb0\xb1\
+\x14\x14\xb1\xb1\x12\xff\x04Q4\xa8 \xd1\xc2\x80\x8d\x88\
+\x09\x82\xc6\x1f`\x17\x8d\x88\x85Jb\xb1\x1c.\xb8s\
+w\xe6vw\xee\xf6\xf6\x0bo1\xc3\x1e\xf3\xbc\xcf\xce\
+\xbc37KMMMMM\xcdF\xd9\x81[\xb1E\
+\xc4b\x12o\xb0\x1e[H\xd94p\x01?%\xc9\x0f\
+\x95\x01\x13x\xe2o\xe2Ce\xc0\x09\xac\xf87\xf9\xca\
+\x1b\xd0*tY\x89W\xde\x80t\xa1\x1b*\x03F1\
+\x8b_:'_t\xac\xe23\xe6q\x13g\xb0\xa7\xb8\
+\xd4\xd9\x8d\xa7\x91\x93\xee&^\xe0<\x9ay&\x7f\x12\
+_\xfb \xb9\xff\x89/\xb8\x84\xed\xc3j@+>`\
+&\x0f\x13\x06e\x09\x84\xe2\x1a\xb6\xf4jB\xd6io\
+\x90\xe2\xb1\x9cj\xc3!\xbc\xedb\xc0\x22\x19\xc3^\x1c\
+\xc3e\xbc\xecB\xcf:\x16$g\x98\x9ei\xe2v\x87\
+\xc1\xca\xe6 \xeew\xd0\xb4\x8e\x87\xd8\x9c\xd7\xa0\xed\x0a\
+d,\x0e\xe3u@S+\xae\xe69`\xa8@\xc6\xa4\
+\x89\xbb\xda\x9b\x90\xcb\xee\xd0\x22\xeb\x94\x18\x9b\x06n\x08\
+\x1b\xf0\x1e\xdb\xf2\x1e4] \xfb\x81\x86\xf63a\xb6\
+\x88A[\x05\xb2_hbQ\xb6\x01+r\xda\x15\xfa\
+\x9d#\xc2\xb3\xe0\x5cD]\xa5\xf2@\xf8l0\x14L\
+\x0a\xcf\x82]\x11u\x95\xca+\xd9\x06\x9cN?\xb4\xa9\
+|]\xa5q'\xd0?\x95nT\xd9\x80\xf9@\xff\xfe\
+RUDd\x9f\xec%\xf0)\xa6\xa82\x19\x93m\xc0\
+\xb7\x98\xa2\xca\xa4!\xdb\x80\xdf\xe9\x87\xaa\x5c\x03\xb6\x06\
+\xfa\x7f\xa4\x1bU6`g\xa0\x7f5\xdd\xa8\xb2\x01\x07\
+\x02\xfd\xef\xd2\x8d*\x1bp4\xd0\xbfX\xaa\x8aH\x8c\
+\xe0\xa3\xec\x22x*\xa2\xae\xd2\x98\x12\xfe/0\x11Q\
+Wi\xcc\xc9N\xfeyLQe1-\xfc\xf6\xcfF\
+\xd4U\x0a\xe3X2\xa47B\x0d\xdc\x13~\xfb\x17\xe3\
+I+\x9eN\xb7\xc2\xcb\xc2'\xc3\x81g\x5c\xfb7\xbf\
+\x86\xe3\xd1\xd4\x15\xcc\xb4\xf0\x9ao\xc5\x95h\xea\x0ab\
+D\xb2\xcf\x87\xb6\xbat\xcc\xc9\xf1\xdb`,\x9a\x92\xcb\
+\x8d\x19\x5c\x17>\xe1e\xdd\x00\x8fE\xd0\xdb\x15\xdd$\
+\xd0K<\xd4\xe7[^Q\x89\xafI\xd6|\xdfO\xfb\
+\x22\x92_6@\xd5>\xcf\xc4W$\x87\x9c\x81\xda\xe7\
+\xf3H|Ar\xb6\xefi\xad\x8f\xf6\xf2\xe3\x92X\xc5\
+w\xc9\xa7\xf8%<\xc3#\xc97\xff\x9a\x9a\x9a\x9a\x9a\
+\x9a\x9a\x9a\x0d\xf3\x078\xcd\x84p\xe6]\x83;\x00\x00\
+\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x10\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x01\xc5IDATx\x9c\xed\x9aMJ\
+\xc3@\x18\x86\x1f\xff\xb6\x15\xbd\x80\x08\x9eAAp\xaf\
+\x07p\xa7[\xaf\xe0B\x97\x0a^\xc1\xadt\xe51\x5c\
+\x88\x9e\xc1\x85\xa2\xae+\xae\x04)\xc4E\x1b\x88\xb5\x93\
+\xccL\x93yM\xf3=0\x10\x92\x99\xcc\xcb\xd3\xf6\xcb\
+d(\x18\x86a\x18\xdde\xa1\xe1\xfbg\x81\xf3\x86\xf6\
+\x9f\x99\xc5\xa6n\xdc\x16L\x80:\x80\x1a\x13\xa0\x0e\xa0\
+\xc6\x04\xa8\x03\xa81\x01\xea\x00jL\x80:\x80\x1a\x13\
+\xa0\x0e\xa0\xc6\x04\xa8\x03\xa8\x89\x15\xd0\x03n\xea\x0c2\
+#\xb7\xc0Z\xaa\xc9v\x80'\xdc\x9b\x17E2G\xab\
+\xab\x7fq\xdc\x0b\xb0\xe7\xd17\x9a%\xe0\x14\xf8&,\
+X*\x01\x190\x04\xae\x80\x15\x8f1Al\x00w3\
+\x04K% o\x8f\xc0\x96\xc78/\x0e\x81AM\xc1\
+R\x09\xc8\x80O\xe0\xc4c\xac\x93\xbc\xd0\xb9B\xfdw\
+\x01y\x8b*\x90\xc5B\xd7v\x01\xa5\x05rr\xbby\
+\x198\x07\xce\xc6\xc7U|T\x5cw\x99\x0f\xdd\x16\x8f\
+\x9d\xa7\xc8\x10\xb8\x04.\xc6\xc7\x7fp\x15\xba&\x9a\x8b\
+\x14sO-\x90e\x85n\xde\x04d\x14\x0ad\x97\x97\
+\xc2_\x93'\xba\xf2\x13x\xa0d\x8d0m\xb57/\
+\x02\xa6\xae\x12]\xd5x\x17\xe8\x03\x9b%a\x01\xd6+\
+\xae\x0f\x1c\xe7C\x9f\x02\xb1\xf3\xe4<\x03G\xc0}E\
+\xbf_\xf4\x80k\xe2>\xc9\x9c\xba\xbe\x01\xb1\xf3d\xd4\
+\xf0\xa6\xd8\xe6\xa5\xf0\xb1\xc7X/\xda\xf62TZ\xe8\
+b\xe9\xf4\xebp\x91m:\xba!Rd\x95\xd1S\xa2\
+\x8aT\x02\xfa\xe3L\xc1\xd8\x7f\x84\x9a\xbaq[0\x01\
+\xea\x00jL\x80:\x80\x1a\x13\xa0\x0e\xa0\xc6\x04\xa8\x03\
+\xa81\x01\xea\x00jL\x80:\x80\x1a\x13 \x98\xf3\xad\
+\xe4\xda{\xb2\x14\x89\x98\xdc\xd8x\x05\xf6K\xfa\x1f0\
+\x12\x14\xba!b\x18\x86a\xc4\xf0\x03\x16\xf2\xf2\xcaR\
+\xed\xcdq\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x01\xb0\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x01eIDATx\x9c\xed\x9a\xb1M\
+\x03A\x10E\x1f$\x88\x10BD\x0f\xd0\x01P\x00\x15\
+\xe0*  \xa5\x05\xdapH\x0a]@\x8a\x04\x15@\
+\x86#\x86\xe0\xb4\x92\x03#\xad\xcf;7\xda\xfb\xf3\xa4\
+\xc9,\xcd\xf7K\xe6vw I\x92$I\x92$\xa9\
+\xe6\x10x\x00\x9e\x80\x93\x80\xfeVQn\x5c\x03\xefk\
+\x8d\xbe\x80\x1b\xcf\x86\x1b\x08\x15\xf0_\xc3%p\xe4\xd9\
+\xb8\x22C\xa8\x00\x03>\x80\x0b\xcf\xe6\x15\x19B\x05\x18\
+\xf0\x0b<\x02\x07\x81\x19B\x05\x94z\x05\xce\x023\xb8\
+Q+\xc0\x80\x1f\xe0\x1e\xd8\x0f\xc8\xe0\xc66\x02J=\
+\x03\xa7\x13gpc\x8c\x00\x03\xbei7.\xbb\x14P\
+\xaa\xc5\xb8\xecZ\x80\x01\x9f\xc0\xa5s\x067Z\x080\
+v\x1b\x97\xb3\x10P\xea\x0d8w\xc8\xe0Fk\x01\xc6\
+\xf6\xe3rv\x02J\xbdP7.g+\xc0\x18\xc6\xe5\
+\xa2A\x067\xbc\x05\x94Z\x02\xc7;dpc*\x01\
+\xc60.\xafFfpcJ\x01\xc6\xe6q)%\xa0\
+\xd4\xfa\xb8\x94\x14`\x0c\xe3\xf2\xb6\xf2\xb7\xd5\xec\x8d\x10\
+\xd0\x03\xd5\xff\xab\xf5Y\xbd;R@t\x80hz\x12\
+\xb0\x02\xee\xa2C\xe4\x18\x9c\xb8\xa4?\x84\xa4?\x85e\
+\x0fC\xd2\xc7a\xd9\x0b\x11\xe9+1\xd9KQ\xe9k\
+q\xe9\x87\x11\xd9\xa71\xe9\xc7Q\xd9\xe7q\xe9\x05\x09\
+\xd9\x15\x19\xe9%)\xe959\x99EI\xf9UY\x10\
+_\x96N\x92$I\x92$\x99\x0d\x7f\x8e\xb3B\xa6\x95\
+\xe9\xbb^\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x82\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x027IDATx\x9c\xed\x9b\xb1N\
+\x1bA\x10\x86?\x03\x9d-\x8a\x00e*hp\x02\xb4\
+\x90\x22\xd0\xc0\x9b \x04\x02\x92\xc7Hx\x06x\x05d\
+\xf9)\xa0\x8b\xa1\x8a\x08\x12\x88\x12#@\x02c\x1aL\
+q\x17\xc5\xb9[/\xb69\xcf\xee\x9e\xe7\x93N\xb2v\
+wnf~\xcf\xee\x9d\xee\xf6@Q\x14EqN\x03\
+\xb8\x02\xaa\xc060\xd9\x83\xedTlS\x8d\xcf\xd1\xc8\
+<:\x01Z\x89\xe3\x11\xf8\x09\x14-6%`\x8f(\
+\xe1\xa4}p$\x13\xf8{\x9c\x01\xf3\x86\xf1\x0b\xc0\x1f\
+\x8b]ptJ\xa4\x05\xdc\x01Kmc\xbf\x00\xf7o\
+\xd8\x04G\x11(\x03\xbb@\x8dtBu`\x1a\x98\x01\
+n\x0c\xfd\xbf\x80\x1d`\x16\xfb\xb4\x09\x82\x11`\x03h\
+\xf2\x7f\x92G\xc0q\xa2\xed\x09X\x8fmr\xc72i\
+\x11\x92\xc9\x7fu\x16\x9d\x10\x9bt\x16`\xdda\x5cb\
+\x8c\x00'\x98\xe7|&e\xef\xfb\xdcy\x01\x0e\x0c\xed\
+\xfbq\xdfPP&]\x01\xb3N#\x12\xa6DZ\x80\
+RV'/\xb4\xfd\xf6\xe5\x06\xa2Nt\x7f\xdf\xce \
+b+\x80\x9fk@S\xd2\x99\x0a \xe9\xacK\x9e%\
+\x9d\x8dY\xfa\x0a\x96>\xd7\xf4\x13\x9bq\x1d\xf1\xb1\x02\
+DQ\x01\x5c\x07\xe0\x9a^\x04\xb0=\x80\xc8\xf28|\
+gN=\xe1c\x05\x0c\xfdeP\x05\x90t\xe6\xa3\x00\
+\xa27B>\x0a\xa0\x15 \xe9\xccG\x01\x86\xbe\x02T\
+\x00Ig>\x0a\xa0k\x80\xa43\x15@\xd2Y\x97\x88\
+\x0a`{\x22\x94\xc4\xe7'D}\xe3c\x05\x88\xa2\x02\
+\xb8\x0e\xc05\xb65\xc0\xd5\x9b\xa2\x19\xe0\xfc\x8d1\x99\
+\xc5\xe6c\x05\xe8eP\xd2\xd9\xd0\x0b\x10\x02\xe3\x0c\xf0\
+\xf5\xb8\x8f\x15\x90\xe4c\x97m}\x11\x82\x00k\x86\xb6\
+U\xf1(\x1c1\x0a\x9c\x92\x9e\x025\xc2\xf8\xf3\xde\xcd\
+\x16\x9d\xdf m8\x8cK\x84\x15\xec\x1b%\x9bD\x9b\
+)s\xc7(\xd1?o\xda*{DZ\x84Mr0\
+\x1dJ\xc0'\xe0;\xe69\x7f\xcd\xbf\xcd\xd2uC\xff\
+\x09\xf0->G\x90\x9b\xa5mo\x8bo\x81\xc5\xb6\xb1\
+KD[\xe8s\xb5]\xbeS\x22\xbf\x81\xcf\x86\xf1s\
+D\x1fS\xe4V\x80\x07\xe0\x07\xf6r.\xc6c\x1e\x0d\
+\xf6\xc1\xd1\x00.\x80\x0a\xd1\xa2\xf6\xa1\x07\xdb\x09\xa2E\
+\xb3\x02\x5c\x12\xe8GS\x8a\xa2(Nx\x05\x0dw\xfb\
+\xc6$R\xf4\x9c\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+"
+
+qt_resource_name = b"\
+\x00\x05\
+\x00o\xa6S\
+\x00i\
+\x00c\x00o\x00n\x00s\
+\x00\x04\
+\x00\x07\x8b\xaf\
+\x00r\
+\x00e\x00d\x00o\
+\x00\x05\
+\x00s\xc8\xd5\
+\x00m\
+\x00e\x00r\x00g\x00e\
+\x00\x06\
+\x06\xac,\xa5\
+\x00d\
+\x00e\x00l\x00e\x00t\x00e\
+\x00\x0e\
+\x0a\x87\xe3G\
+\x00s\
+\x00e\x00e\x00k\x00_\x00b\x00e\x00g\x00i\x00n\x00n\x00i\x00n\x00g\
+\x00\x04\
+\x00\x075\xdf\
+\x00l\
+\x00o\x00g\x00o\
+\x00\x04\
+\x00\x07\xc4\xaf\
+\x00u\
+\x00n\x00d\x00o\
+\x00\x05\
+\x00zs\x04\
+\x00s\
+\x00p\x00l\x00i\x00t\
+\x00\x08\
+\x0b\xc1Wd\
+\x00s\
+\x00e\x00e\x00k\x00_\x00e\x00n\x00d\
+\x00\x06\
+\x07\x8cH5\
+\x00r\
+\x00e\x00n\x00a\x00m\x00e\
+"
+
+qt_resource_struct = b"\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x09\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00b\x00\x01\x00\x00\x00\x01\x00\x00\x09\xcf\
+\x00\x00\x01\x81_5\x1f{\
+\x00\x00\x00\x10\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x81\x96\x8cK\xb5\
+\x00\x00\x00p\x00\x00\x00\x00\x00\x01\x00\x00\x15k\
+\x00\x00\x01\x81\x96\x8cK\xb9\
+\x00\x00\x00\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x02\xd7\
+\x00\x00\x01\x81\x96\x8cK\xb4\
+\x00\x00\x00~\x00\x00\x00\x00\x00\x01\x00\x00\x18*\
+\x00\x00\x01\x81\x96\x8cK\xb8\
+\x00\x00\x00.\x00\x00\x00\x00\x00\x01\x00\x00\x05\x0a\
+\x00\x00\x01\x81\x96\x8cK\xb3\
+\x00\x00\x00\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x1b\xf2\
+\x00\x00\x01\x81\x96\x8cK\xb6\
+\x00\x00\x00@\x00\x00\x00\x00\x00\x01\x00\x00\x080\
+\x00\x00\x01\x81\x96\x8cK\xb7\
+\x00\x00\x00\x8e\x00\x00\x00\x00\x00\x01\x00\x00\x1a>\
+\x00\x00\x01\x81\x96\x8cK\xb7\
+"
+
+def qInitResources():
+    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+def qCleanupResources():
+    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+qInitResources()
```

### Comparing `boxjelly-0.3.2/boxjelly/models/TrackListModel.py` & `boxjelly-0.3.3/boxjelly/models/TrackListModel.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,408 +1,408 @@
-import logging
-from typing import Iterable, List, Set
-from uuid import UUID, uuid4
-from intervaltree.interval import Interval
-from intervaltree.intervaltree import IntervalTree
-
-from PyQt6 import QtCore
-from sharktopoda_client.localization.LocalizationController import LocalizationController
-from sharktopoda_client.localization.Localization import Localization
-from sharktopoda_client.localization.IO import IO as LocalizationIO
-from boxjelly.lib.settings import SettingsManager
-
-from boxjelly.lib.track import Track
-
-
-class TrackListModel(QtCore.QAbstractListModel):
-    """
-    Track list model. Wraps a list of tracks and synchronizes with a Sharktopoda client LocalizationController.
-    """
-    
-    IDRole = QtCore.Qt.ItemDataRole.UserRole + 1  # Integer ID (e.g. 42)
-    LabelRole = QtCore.Qt.ItemDataRole.UserRole + 2  # String label (e.g. "fish")
-    StartFrameRole = QtCore.Qt.ItemDataRole.UserRole + 3  # Integer start frame (e.g. 12345)
-    EndFrameRole = QtCore.Qt.ItemDataRole.UserRole + 4  # Integer end frame (e.g. 67890). This is derived, so cannot be set directly.
-    EventsRole = QtCore.Qt.ItemDataRole.UserRole + 5  # List of track's boxes (None indicates no box at that frame)
-    EventLabelsRole = QtCore.Qt.ItemDataRole.UserRole + 6  # List of strings for all event labels (e.g. ["fish", "fish"])
-    
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        
-        self._tracks: List[Track] = []  # Root list of tracks
-        
-        # IntervalTree for quick lookup of tracks by frame
-        self._track_id_interval_dict = {}
-        self._track_tree = IntervalTree()
-        
-        # Sharktopoda client LocalizationController for adding/removing localizations
-        self._track_id_localization_list_dict = {}
-        self._localization_controller = LocalizationController()
-        self._localization_controller.log.setLevel(logging.INFO)
-        
-        # Get the app settings manager, connect signals from setting proxies
-        self._settings = SettingsManager.get_instance()
-        self._settings.incoming_port.valueChanged.connect(self._refresh_localization_io)
-        self._settings.incoming_topic.valueChanged.connect(self._refresh_localization_io)
-        self._settings.outgoing_port.valueChanged.connect(self._refresh_localization_io)
-        self._settings.outgoing_topic.valueChanged.connect(self._refresh_localization_io)
-        
-        # Create the localization IO
-        self._localization_io = None
-        self._selection_controller = None
-        self._refresh_localization_io()
-        
-        # Video info (TODO: find this a new home)
-        self._video_reference_uuid = None
-        self._frame_rate = None
-        self._settings.frame_rate.valueChanged.connect(self.set_frame_rate)
-        
-        # Set of track IDs that have been loaded into the LocalizationController
-        self._loaded_ids = set()  # Set of track IDs that are currently loaded in Cthulhu
-    
-    @QtCore.pyqtSlot()
-    def _refresh_localization_io(self):
-        """
-        Refresh the LocalizationIO.
-        """
-        # Close the current IO
-        old_io = self._localization_io
-        if old_io is not None:
-            old_io.ok = False
-            old_io.context.destroy()
-        
-        # Create a new IO from the current settings
-        new_io = LocalizationIO(
-            self._settings.incoming_port.value,
-            self._settings.outgoing_port.value,
-            self._settings.incoming_topic.value,
-            self._settings.outgoing_topic.value,
-            self._localization_controller
-        )
-        
-        # Replace the old IO with the new one
-        self._localization_io = new_io
-        self._localization_io.log.setLevel(logging.INFO)
-        self._selection_controller = self._localization_io.selectionController
-    
-    @property
-    def video_loaded(self) -> bool:
-        """
-        Property to tell whether or not the video is loaded.
-        """
-        return self._video_reference_uuid is not None and self._frame_rate is not None
-    
-    def set_video_reference_uuid(self, uuid: str):
-        """
-        Set the video reference UUID.
-        """
-        self._video_reference_uuid = uuid
-    
-    def set_frame_rate(self, frame_rate: float):
-        """
-        Set the video frame rate.
-        """
-        # Check if we need to reload tracks
-        if self._frame_rate is not None and self._frame_rate != frame_rate:
-            self._localization_controller.clear()
-            self._loaded_ids.clear()
-        
-        self._frame_rate = frame_rate
-    
-    def frame_to_ms(self, frame: int):
-        """
-        Convert a frame number to elapsed milliseconds.
-        """
-        if not self.video_loaded:
-            return ValueError('Video not loaded')
-        
-        return round((1e3 / self._frame_rate) * frame)
-
-    def ms_to_frame(self, ms: int):
-        """
-        Convert elapsed milliseconds to a frame number.
-        """
-        if not self.video_loaded:
-            return ValueError('Video not loaded')
-        
-        return round(self._frame_rate * (ms / 1e3))
-    
-    def sort(self, *_):
-        """
-        Sort the list of tracks by start frame.
-        """
-        self._tracks.sort(key=lambda track: (track.start_frame, track.id))
-        self.layoutChanged.emit()
-
-    def rowCount(self, parent) -> int:
-        """
-        Get the number of tracks in the list.
-        """
-        return len(self._tracks)
-
-    def _register(self, track: Track):
-        """
-        Register a track internally. Do not call this directly - use add_track or set_tracks instead.
-        """
-        # Add the track to the list
-        self._tracks.append(track)
-        
-        # Create an interval that represents the track duration
-        interval = Interval(track.start_frame, track.start_frame + len(track), track)
-        self._track_tree.add(interval)  # Add the interval to the IntervalTree
-        self._track_id_interval_dict[track.id] = interval  # Keep a reference to the interval
-        
-        # Generate a list of Localizations for the track, but don't add them to the LocalizationController yet
-        localizations = list(self._generate_localizations(track))
-        self._track_id_localization_list_dict[track.id] = localizations
-        
-    def _unregister(self, idx: int):
-        """
-        Unregister a track internally. Do not call this directly - use remove_track instead.
-        """
-        track_id = self.get_track(idx).id
-        
-        # Immediately remove the track from the LocalizationController, if loaded
-        if track_id in self._loaded_ids:
-            self._localization_controller.removeLocalizations(self._track_id_localization_list_dict[track_id])
-            self._loaded_ids.remove(track_id)
-        del self._track_id_localization_list_dict[track_id]
-        
-        # Remove the track's interval from the IntervalTree
-        interval = self._track_id_interval_dict[track_id]
-        self._track_tree.remove(interval)
-        del self._track_id_interval_dict[track_id]
-        
-        # Remove the track from the list
-        del self._tracks[idx]
-
-    def add_track(self, track: Track):
-        """
-        Add a track to the list.
-        
-        Note: this will emit the layoutChanged signal on each call, which is inefficient when rendering to multiple displays. 
-        If you want to add multiple tracks at once, use set_tracks instead.
-        """
-        self.beginInsertRows(QtCore.QModelIndex(), len(self._tracks), len(self._tracks))
-        self._register(track)
-        self.endInsertRows()
-        self.sort()
-    
-    def clear(self):
-        """
-        Clear the list of tracks.
-        """
-        self.beginResetModel()
-        self._tracks = []
-        self._track_tree.clear()
-        self._track_id_interval_dict = {}
-        self._track_id_localization_list_dict = {}
-        self._loaded_ids = set()
-        self._localization_controller.clear()
-        self.endResetModel()
-    
-    def set_tracks(self, tracks: List[Track]):
-        """
-        Set the list of tracks.
-        """
-        self.clear()
-        self.beginInsertRows(QtCore.QModelIndex(), 0, len(tracks) - 1)
-        for track in tracks:
-            self._register(track)
-        self.endInsertRows()
-        self.sort()
-    
-    def _load_localizations(self, track: Track):
-        """
-        Load the track's localizations into the LocalizationController.
-        """
-        if track.id in self._loaded_ids:  # Short-circuit if the track is already loaded
-            return
-        
-        localizations = self._track_id_localization_list_dict[track.id]
-        self._localization_controller.addLocalizations(localizations)
-        self._loaded_ids.add(track.id)
-    
-    def load_at_frame(self, frame_number: int):
-        """
-        Load localizations for tracks overlapping the given frame number.
-        """
-        overlapping_intervals = self._track_tree[frame_number-100:frame_number+100]
-        for interval in overlapping_intervals:
-            self._load_localizations(interval.data)
-    
-    def get_track(self, idx: int) -> Track:
-        """
-        Get the track at the given index.
-        """
-        return self._tracks[idx]
-            
-    def index_by_id(self, id: UUID) -> int:
-        """
-        Find the row index of the track with the given ID.
-        
-        Raises a ValueError if a track with the given ID is not found.
-        """
-        return self._tracks.index(self._track_id_interval_dict[id].data)
-    
-    def get_interval(self, key):
-        """
-        Index the IntervalTree with the given key.
-        
-        TODO: Don't interfaace with the IntervalTree directly.
-        """
-        return self._track_tree[key]
-    
-    def set_track(self, idx: int, track: Track):
-        """
-        Update the track at the given row index.
-        """
-        self._tracks[idx] = track
-        self.dataChanged.emit(self.index(idx), self.index(idx))
-        self.sort()
-        
-    def delete_track(self, idx: int):
-        """
-        Delete the track at the given row index.
-        """
-        self.beginRemoveRows(QtCore.QModelIndex(), idx, idx)
-        self._unregister(idx)
-        self.endRemoveRows()
-        
-    def get_all_tracks(self):
-        """
-        Get the list of all tracks.
-        """
-        return self._tracks
-
-    def get_new_id(self) -> UUID:
-        """
-        Get the next available track ID.
-        """
-        new_id = uuid4()
-        while new_id in self._track_id_interval_dict:
-            new_id = uuid4()
-        
-        return new_id
-
-    def data(self, index, role):
-        if not index.isValid():
-            return None
-        
-        track = self.get_track(index.row())
-        
-        if role == QtCore.Qt.ItemDataRole.DisplayRole:
-            return track.label_mode
-        elif role == self.IDRole:
-            return track.id
-        elif role == self.LabelRole:
-            return track.label_mode
-        elif role == self.StartFrameRole:
-            return track.start_frame
-        elif role == self.EndFrameRole:
-            return track.start_frame + len(track) - 1
-        elif role == self.EventsRole:
-            return track.events
-        elif role == self.EventLabelsRole:
-            return [event.label if event else None for event in track.events]
-        return None
-    
-    def setData(self, index, value, role):
-        if not index.isValid():
-            return False
-        
-        track = self.get_track(index.row())
-        
-        if role == self.EventLabelsRole:
-            # Update the labels
-            for event, label in zip(track.events, value):
-                if event:
-                    event.label = label
-            
-            # Replace localizations
-            localizations = self._track_id_localization_list_dict[track.id]  # Get old localizations
-            new_localizations = list(self._generate_localizations(track))  # Make the new localizations
-            self._localization_controller.removeLocalizations(localizations)  # Remove the old localizations
-            self._localization_controller.addLocalizations(new_localizations)  # Add the new localizations
-            self._track_id_localization_list_dict[track.id] = new_localizations  # Update the localization list dict
-            
-            self.dataChanged.emit(index, index)
-        elif role == self.EventsRole:    
-            # Update the boxes
-            track.events = value
-            
-            # Replace interval
-            interval = self._track_id_interval_dict[track.id]  # Get old interval
-            new_interval = Interval(interval.begin, interval.begin + len(value), track)  # Make the new interval
-            self._track_tree.remove(interval)  # Remove the old interval
-            self._track_tree.add(new_interval)  # Add the new interval
-            self._track_id_interval_dict[track.id] = new_interval  # Update the interval dict
-            
-            # Replace localizations
-            localizations = self._track_id_localization_list_dict[track.id]  # Get old localizations
-            new_localizations = list(self._generate_localizations(track))  # Make the new localizations
-            self._localization_controller.removeLocalizations(localizations)  # Remove the old localizations
-            self._localization_controller.addLocalizations(new_localizations)  # Add the new localizations
-            self._track_id_localization_list_dict[track.id] = new_localizations  # Update the localization list dict
-            
-            self.dataChanged.emit(index, index)
-        else:
-            return False
-        
-        return True
-
-    def _generate_localizations(self, track: Track) -> Iterable[Localization]:
-        """
-        Generate localizations for the given track.
-        """
-        for frame_offset, event in enumerate(track.events):
-            if not event:  # skip if there is no event
-                continue
-            
-            yield Localization(
-                concept=f'{str(track.id)[:8]} - {event.label}',  # truncate the ID to 8 characters
-                elapsedTime=self.frame_to_ms(track.start_frame + frame_offset),
-                duration=0,
-                videoReferenceUuid=UUID(self._video_reference_uuid),
-                annotationUuid=track.id,
-                localizationUuid=event.id,
-                x=event.box.x,
-                y=event.box.y,
-                width=event.box.w,
-                height=event.box.h
-            )
-    
-    def select_track(self, idx: int):
-        """
-        Select the track at the given index.
-        """
-        if not self._settings.selection_enabled.value:
-            return
-        
-        selected_track = self.get_track(idx)
-        if selected_track.id not in self._loaded_ids:  # track needs load
-            self._load_localizations(selected_track)
-        
-        track_localizations = self._track_id_localization_list_dict[selected_track.id]
-        
-        # Sharktopoda client clears the selection. We avoid this by unioning the new selection with the old selection.
-        previous_localizations = self._selection_controller.getSelectedLocalizations()
-        previous_localization_uuids = set(localization.localizationUuid for localization in previous_localizations)
-        
-        union = previous_localizations + [loc for loc in track_localizations if loc.localizationUuid not in previous_localization_uuids]
-        
-        self._selection_controller.select(union, True)
-    
-    def deselect_track(self, idx: int):
-        """
-        Deselect the track at the given index.
-        """
-        if not self._settings.selection_enabled.value:
-            return
-        
-        deselected_track = self.get_track(idx)
-        if deselected_track.id not in self._loaded_ids:  # track needs load
-            self._load_localizations(deselected_track)
-        
-        track_localizations = self._track_id_localization_list_dict[deselected_track.id]
-        
-        self._selection_controller.deselect(track_localizations, True)
+import logging
+from typing import Iterable, List, Set
+from uuid import UUID, uuid4
+from intervaltree.interval import Interval
+from intervaltree.intervaltree import IntervalTree
+
+from PyQt6 import QtCore
+from sharktopoda_client.localization.LocalizationController import LocalizationController
+from sharktopoda_client.localization.Localization import Localization
+from sharktopoda_client.localization.IO import IO as LocalizationIO
+from boxjelly.lib.settings import SettingsManager
+
+from boxjelly.lib.track import Track
+
+
+class TrackListModel(QtCore.QAbstractListModel):
+    """
+    Track list model. Wraps a list of tracks and synchronizes with a Sharktopoda client LocalizationController.
+    """
+    
+    IDRole = QtCore.Qt.ItemDataRole.UserRole + 1  # Integer ID (e.g. 42)
+    LabelRole = QtCore.Qt.ItemDataRole.UserRole + 2  # String label (e.g. "fish")
+    StartFrameRole = QtCore.Qt.ItemDataRole.UserRole + 3  # Integer start frame (e.g. 12345)
+    EndFrameRole = QtCore.Qt.ItemDataRole.UserRole + 4  # Integer end frame (e.g. 67890). This is derived, so cannot be set directly.
+    EventsRole = QtCore.Qt.ItemDataRole.UserRole + 5  # List of track's boxes (None indicates no box at that frame)
+    EventLabelsRole = QtCore.Qt.ItemDataRole.UserRole + 6  # List of strings for all event labels (e.g. ["fish", "fish"])
+    
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        
+        self._tracks: List[Track] = []  # Root list of tracks
+        
+        # IntervalTree for quick lookup of tracks by frame
+        self._track_id_interval_dict = {}
+        self._track_tree = IntervalTree()
+        
+        # Sharktopoda client LocalizationController for adding/removing localizations
+        self._track_id_localization_list_dict = {}
+        self._localization_controller = LocalizationController()
+        self._localization_controller.log.setLevel(logging.INFO)
+        
+        # Get the app settings manager, connect signals from setting proxies
+        self._settings = SettingsManager.get_instance()
+        self._settings.incoming_port.valueChanged.connect(self._refresh_localization_io)
+        self._settings.incoming_topic.valueChanged.connect(self._refresh_localization_io)
+        self._settings.outgoing_port.valueChanged.connect(self._refresh_localization_io)
+        self._settings.outgoing_topic.valueChanged.connect(self._refresh_localization_io)
+        
+        # Create the localization IO
+        self._localization_io = None
+        self._selection_controller = None
+        self._refresh_localization_io()
+        
+        # Video info (TODO: find this a new home)
+        self._video_reference_uuid = None
+        self._frame_rate = None
+        self._settings.frame_rate.valueChanged.connect(self.set_frame_rate)
+        
+        # Set of track IDs that have been loaded into the LocalizationController
+        self._loaded_ids = set()  # Set of track IDs that are currently loaded in Cthulhu
+    
+    @QtCore.pyqtSlot()
+    def _refresh_localization_io(self):
+        """
+        Refresh the LocalizationIO.
+        """
+        # Close the current IO
+        old_io = self._localization_io
+        if old_io is not None:
+            old_io.ok = False
+            old_io.context.destroy()
+        
+        # Create a new IO from the current settings
+        new_io = LocalizationIO(
+            self._settings.incoming_port.value,
+            self._settings.outgoing_port.value,
+            self._settings.incoming_topic.value,
+            self._settings.outgoing_topic.value,
+            self._localization_controller
+        )
+        
+        # Replace the old IO with the new one
+        self._localization_io = new_io
+        self._localization_io.log.setLevel(logging.INFO)
+        self._selection_controller = self._localization_io.selectionController
+    
+    @property
+    def video_loaded(self) -> bool:
+        """
+        Property to tell whether or not the video is loaded.
+        """
+        return self._video_reference_uuid is not None and self._frame_rate is not None
+    
+    def set_video_reference_uuid(self, uuid: str):
+        """
+        Set the video reference UUID.
+        """
+        self._video_reference_uuid = uuid
+    
+    def set_frame_rate(self, frame_rate: float):
+        """
+        Set the video frame rate.
+        """
+        # Check if we need to reload tracks
+        if self._frame_rate is not None and self._frame_rate != frame_rate:
+            self._localization_controller.clear()
+            self._loaded_ids.clear()
+        
+        self._frame_rate = frame_rate
+    
+    def frame_to_ms(self, frame: int):
+        """
+        Convert a frame number to elapsed milliseconds.
+        """
+        if not self.video_loaded:
+            return ValueError('Video not loaded')
+        
+        return round((1e3 / self._frame_rate) * frame)
+
+    def ms_to_frame(self, ms: int):
+        """
+        Convert elapsed milliseconds to a frame number.
+        """
+        if not self.video_loaded:
+            return ValueError('Video not loaded')
+        
+        return round(self._frame_rate * (ms / 1e3))
+    
+    def sort(self, *_):
+        """
+        Sort the list of tracks by start frame.
+        """
+        self._tracks.sort(key=lambda track: (track.start_frame, track.id))
+        self.layoutChanged.emit()
+
+    def rowCount(self, parent) -> int:
+        """
+        Get the number of tracks in the list.
+        """
+        return len(self._tracks)
+
+    def _register(self, track: Track):
+        """
+        Register a track internally. Do not call this directly - use add_track or set_tracks instead.
+        """
+        # Add the track to the list
+        self._tracks.append(track)
+        
+        # Create an interval that represents the track duration
+        interval = Interval(track.start_frame, track.start_frame + len(track), track)
+        self._track_tree.add(interval)  # Add the interval to the IntervalTree
+        self._track_id_interval_dict[track.id] = interval  # Keep a reference to the interval
+        
+        # Generate a list of Localizations for the track, but don't add them to the LocalizationController yet
+        localizations = list(self._generate_localizations(track))
+        self._track_id_localization_list_dict[track.id] = localizations
+        
+    def _unregister(self, idx: int):
+        """
+        Unregister a track internally. Do not call this directly - use remove_track instead.
+        """
+        track_id = self.get_track(idx).id
+        
+        # Immediately remove the track from the LocalizationController, if loaded
+        if track_id in self._loaded_ids:
+            self._localization_controller.removeLocalizations(self._track_id_localization_list_dict[track_id])
+            self._loaded_ids.remove(track_id)
+        del self._track_id_localization_list_dict[track_id]
+        
+        # Remove the track's interval from the IntervalTree
+        interval = self._track_id_interval_dict[track_id]
+        self._track_tree.remove(interval)
+        del self._track_id_interval_dict[track_id]
+        
+        # Remove the track from the list
+        del self._tracks[idx]
+
+    def add_track(self, track: Track):
+        """
+        Add a track to the list.
+        
+        Note: this will emit the layoutChanged signal on each call, which is inefficient when rendering to multiple displays. 
+        If you want to add multiple tracks at once, use set_tracks instead.
+        """
+        self.beginInsertRows(QtCore.QModelIndex(), len(self._tracks), len(self._tracks))
+        self._register(track)
+        self.endInsertRows()
+        self.sort()
+    
+    def clear(self):
+        """
+        Clear the list of tracks.
+        """
+        self.beginResetModel()
+        self._tracks = []
+        self._track_tree.clear()
+        self._track_id_interval_dict = {}
+        self._track_id_localization_list_dict = {}
+        self._loaded_ids = set()
+        self._localization_controller.clear()
+        self.endResetModel()
+    
+    def set_tracks(self, tracks: List[Track]):
+        """
+        Set the list of tracks.
+        """
+        self.clear()
+        self.beginInsertRows(QtCore.QModelIndex(), 0, len(tracks) - 1)
+        for track in tracks:
+            self._register(track)
+        self.endInsertRows()
+        self.sort()
+    
+    def _load_localizations(self, track: Track):
+        """
+        Load the track's localizations into the LocalizationController.
+        """
+        if track.id in self._loaded_ids:  # Short-circuit if the track is already loaded
+            return
+        
+        localizations = self._track_id_localization_list_dict[track.id]
+        self._localization_controller.addLocalizations(localizations)
+        self._loaded_ids.add(track.id)
+    
+    def load_at_frame(self, frame_number: int):
+        """
+        Load localizations for tracks overlapping the given frame number.
+        """
+        overlapping_intervals = self._track_tree[frame_number-100:frame_number+100]
+        for interval in overlapping_intervals:
+            self._load_localizations(interval.data)
+    
+    def get_track(self, idx: int) -> Track:
+        """
+        Get the track at the given index.
+        """
+        return self._tracks[idx]
+            
+    def index_by_id(self, id: UUID) -> int:
+        """
+        Find the row index of the track with the given ID.
+        
+        Raises a ValueError if a track with the given ID is not found.
+        """
+        return self._tracks.index(self._track_id_interval_dict[id].data)
+    
+    def get_interval(self, key):
+        """
+        Index the IntervalTree with the given key.
+        
+        TODO: Don't interfaace with the IntervalTree directly.
+        """
+        return self._track_tree[key]
+    
+    def set_track(self, idx: int, track: Track):
+        """
+        Update the track at the given row index.
+        """
+        self._tracks[idx] = track
+        self.dataChanged.emit(self.index(idx), self.index(idx))
+        self.sort()
+        
+    def delete_track(self, idx: int):
+        """
+        Delete the track at the given row index.
+        """
+        self.beginRemoveRows(QtCore.QModelIndex(), idx, idx)
+        self._unregister(idx)
+        self.endRemoveRows()
+        
+    def get_all_tracks(self):
+        """
+        Get the list of all tracks.
+        """
+        return self._tracks
+
+    def get_new_id(self) -> UUID:
+        """
+        Get the next available track ID.
+        """
+        new_id = uuid4()
+        while new_id in self._track_id_interval_dict:
+            new_id = uuid4()
+        
+        return new_id
+
+    def data(self, index, role):
+        if not index.isValid():
+            return None
+        
+        track = self.get_track(index.row())
+        
+        if role == QtCore.Qt.ItemDataRole.DisplayRole:
+            return track.label_mode
+        elif role == self.IDRole:
+            return track.id
+        elif role == self.LabelRole:
+            return track.label_mode
+        elif role == self.StartFrameRole:
+            return track.start_frame
+        elif role == self.EndFrameRole:
+            return track.start_frame + len(track) - 1
+        elif role == self.EventsRole:
+            return track.events
+        elif role == self.EventLabelsRole:
+            return [event.label if event else None for event in track.events]
+        return None
+    
+    def setData(self, index, value, role):
+        if not index.isValid():
+            return False
+        
+        track = self.get_track(index.row())
+        
+        if role == self.EventLabelsRole:
+            # Update the labels
+            for event, label in zip(track.events, value):
+                if event:
+                    event.label = label
+            
+            # Replace localizations
+            localizations = self._track_id_localization_list_dict[track.id]  # Get old localizations
+            new_localizations = list(self._generate_localizations(track))  # Make the new localizations
+            self._localization_controller.removeLocalizations(localizations)  # Remove the old localizations
+            self._localization_controller.addLocalizations(new_localizations)  # Add the new localizations
+            self._track_id_localization_list_dict[track.id] = new_localizations  # Update the localization list dict
+            
+            self.dataChanged.emit(index, index)
+        elif role == self.EventsRole:    
+            # Update the boxes
+            track.events = value
+            
+            # Replace interval
+            interval = self._track_id_interval_dict[track.id]  # Get old interval
+            new_interval = Interval(interval.begin, interval.begin + len(value), track)  # Make the new interval
+            self._track_tree.remove(interval)  # Remove the old interval
+            self._track_tree.add(new_interval)  # Add the new interval
+            self._track_id_interval_dict[track.id] = new_interval  # Update the interval dict
+            
+            # Replace localizations
+            localizations = self._track_id_localization_list_dict[track.id]  # Get old localizations
+            new_localizations = list(self._generate_localizations(track))  # Make the new localizations
+            self._localization_controller.removeLocalizations(localizations)  # Remove the old localizations
+            self._localization_controller.addLocalizations(new_localizations)  # Add the new localizations
+            self._track_id_localization_list_dict[track.id] = new_localizations  # Update the localization list dict
+            
+            self.dataChanged.emit(index, index)
+        else:
+            return False
+        
+        return True
+
+    def _generate_localizations(self, track: Track) -> Iterable[Localization]:
+        """
+        Generate localizations for the given track.
+        """
+        for frame_offset, event in enumerate(track.events):
+            if not event:  # skip if there is no event
+                continue
+            
+            yield Localization(
+                concept=f'{str(track.id)[:8]} - {event.label}',  # truncate the ID to 8 characters
+                elapsedTime=self.frame_to_ms(track.start_frame + frame_offset),
+                duration=0,
+                videoReferenceUuid=UUID(self._video_reference_uuid),
+                annotationUuid=track.id,
+                localizationUuid=event.id,
+                x=event.box.x,
+                y=event.box.y,
+                width=event.box.w,
+                height=event.box.h
+            )
+    
+    def select_track(self, idx: int):
+        """
+        Select the track at the given index.
+        """
+        if not self._settings.selection_enabled.value:
+            return
+        
+        selected_track = self.get_track(idx)
+        if selected_track.id not in self._loaded_ids:  # track needs load
+            self._load_localizations(selected_track)
+        
+        track_localizations = self._track_id_localization_list_dict[selected_track.id]
+        
+        # Sharktopoda client clears the selection. We avoid this by unioning the new selection with the old selection.
+        previous_localizations = self._selection_controller.getSelectedLocalizations()
+        previous_localization_uuids = set(localization.localizationUuid for localization in previous_localizations)
+        
+        union = previous_localizations + [loc for loc in track_localizations if loc.localizationUuid not in previous_localization_uuids]
+        
+        self._selection_controller.select(union, True)
+    
+    def deselect_track(self, idx: int):
+        """
+        Deselect the track at the given index.
+        """
+        if not self._settings.selection_enabled.value:
+            return
+        
+        deselected_track = self.get_track(idx)
+        if deselected_track.id not in self._loaded_ids:  # track needs load
+            self._load_localizations(deselected_track)
+        
+        track_localizations = self._track_id_localization_list_dict[deselected_track.id]
+        
+        self._selection_controller.deselect(track_localizations, True)
```

### Comparing `boxjelly-0.3.2/boxjelly/scripts/run.py` & `boxjelly-0.3.3/boxjelly/scripts/run.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""
-Entry point for the BoxJelly application.
-"""
-
-from pathlib import Path
-import sys
-
-from PyQt6 import QtWidgets, QtGui, QtCore
-
-import boxjelly.lib.resources
-from boxjelly.lib.constants import APP_NAME, APP_ORGANIZATION, CONTROL_PORT_DEFAULT, FRAME_RATE_DEFAULT, INCOMING_PORT_DEFAULT, INCOMING_TOPIC_DEFAULT, OUTGOING_PORT_DEFAULT, OUTGOING_TOPIC_DEFAULT
-from boxjelly.lib.settings import SettingsManager
-from boxjelly.ui.MainWindow import MainWindow
-
-
-def start(argv):
-    """Start the application"""
-    # Create the application
-    app = QtWidgets.QApplication(argv)
-    
-    QtCore.QSettings.setDefaultFormat(QtCore.QSettings.Format.IniFormat)
-    init_settings()
-    
-    app.setApplicationName(APP_NAME)
-    app.setOrganizationName(APP_ORGANIZATION)
-    
-    # Create the splash screen
-    splash_logo = QtGui.QIcon(':/icons/logo').pixmap(256, 256)
-    splash = QtWidgets.QSplashScreen(splash_logo)
-    splash.show()
-    
-    # Create the main window
-    window = MainWindow()
-    window.show()
-    splash.finish(window)
-    
-    # Start the application
-    app.exec()
-
-
-def init_settings():
-    """Initialize settings"""
-    settings = SettingsManager.get_instance()
-    
-    settings.control_port = ('network/control_port', int, CONTROL_PORT_DEFAULT)
-    settings.incoming_port = ('network/incoming_port', int, INCOMING_PORT_DEFAULT)
-    settings.incoming_topic = ('network/incoming_topic', str, INCOMING_TOPIC_DEFAULT)
-    settings.outgoing_port = ('network/outgoing_port', int, OUTGOING_PORT_DEFAULT)
-    settings.outgoing_topic = ('network/outgoing_topic', str, OUTGOING_TOPIC_DEFAULT)
-    settings.selection_enabled = ('network/selection_enabled', bool, False)
-    
-    settings.frame_rate = ('video/frame_rate', float, FRAME_RATE_DEFAULT)
-    
-
-
-def main():
-    """Parse command line arguments and start"""
-    start(sys.argv)
-
-
-if __name__ == "__main__":
-    main()
+"""
+Entry point for the BoxJelly application.
+"""
+
+from pathlib import Path
+import sys
+
+from PyQt6 import QtWidgets, QtGui, QtCore
+
+import boxjelly.lib.resources
+from boxjelly.lib.constants import APP_NAME, APP_ORGANIZATION, CONTROL_PORT_DEFAULT, FRAME_RATE_DEFAULT, INCOMING_PORT_DEFAULT, INCOMING_TOPIC_DEFAULT, OUTGOING_PORT_DEFAULT, OUTGOING_TOPIC_DEFAULT
+from boxjelly.lib.settings import SettingsManager
+from boxjelly.ui.MainWindow import MainWindow
+
+
+def start(argv):
+    """Start the application"""
+    # Create the application
+    app = QtWidgets.QApplication(argv)
+    
+    QtCore.QSettings.setDefaultFormat(QtCore.QSettings.Format.IniFormat)
+    init_settings()
+    
+    app.setApplicationName(APP_NAME)
+    app.setOrganizationName(APP_ORGANIZATION)
+    
+    # Create the splash screen
+    splash_logo = QtGui.QIcon(':/icons/logo').pixmap(256, 256)
+    splash = QtWidgets.QSplashScreen(splash_logo)
+    splash.show()
+    
+    # Create the main window
+    window = MainWindow()
+    window.show()
+    splash.finish(window)
+    
+    # Start the application
+    app.exec()
+
+
+def init_settings():
+    """Initialize settings"""
+    settings = SettingsManager.get_instance()
+    
+    settings.control_port = ('network/control_port', int, CONTROL_PORT_DEFAULT)
+    settings.incoming_port = ('network/incoming_port', int, INCOMING_PORT_DEFAULT)
+    settings.incoming_topic = ('network/incoming_topic', str, INCOMING_TOPIC_DEFAULT)
+    settings.outgoing_port = ('network/outgoing_port', int, OUTGOING_PORT_DEFAULT)
+    settings.outgoing_topic = ('network/outgoing_topic', str, OUTGOING_TOPIC_DEFAULT)
+    settings.selection_enabled = ('network/selection_enabled', bool, False)
+    
+    settings.frame_rate = ('video/frame_rate', float, FRAME_RATE_DEFAULT)
+    
+
+
+def main():
+    """Parse command line arguments and start"""
+    start(sys.argv)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/graphicsitems/TimelineTrack.py` & `boxjelly-0.3.3/boxjelly/ui/graphicsitems/TimelineTrack.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from PyQt6 import QtWidgets, QtCore, QtGui
-
-from boxjelly.lib.track import Track
-from boxjelly.lib.util import concept_color
-
-
-class TimelineTrack(QtWidgets.QGraphicsObject):
-    """
-    Graphical representation of a track within the timeline view.
-    """
-    
-    DEFAULT_HEIGHT = 30
-    
-    clicked = QtCore.pyqtSignal(object)
-    
-    def __init__(self, track: Track, scale_x: float = 1.0, scale_y: float = 1.0, parent=None):
-        super().__init__(parent)
-        
-        self._track = track  # original track
-        
-        self._scale_x = scale_x  # horizontal scale, in scene units per frame
-        self._scale_y = scale_y  # vertical scale, in scene units per height unit
-        
-        self._track_rect = QtWidgets.QGraphicsRectItem(self)
-        self._track_id_text = QtWidgets.QGraphicsSimpleTextItem(str(track.id)[:8], self)  # truncate to 8 characters
-        
-        self.update()
-        
-    def update(self):
-        self._track_rect.setBrush(concept_color(self._track.label_mode))
-        self._rescale()
-        super().update()
-    
-    def set_scale(self, scale_x: float, scale_y: float):
-        """
-        Set the scale of the track.
-        """
-        self._scale_x = scale_x
-        self._scale_y = scale_y
-        
-        self._rescale()
-    
-    def __len__(self):
-        return len(self._track)
-    
-    @property
-    def width_scene(self):
-        return len(self) * self._scale_x
-    
-    @property
-    def height_scene(self):
-        return self.DEFAULT_HEIGHT * self._scale_y 
-    
-    def _rescale(self):
-        """
-        Rescale the child items.
-        """
-        self._track_rect.setRect(0, 0, self.width_scene, self.height_scene)
-        
-        rect_bounds = self._track_rect.boundingRect()
-        text_bounds = self._track_id_text.boundingRect()
-        self._track_id_text.setPos(
-            int(rect_bounds.width() / 2 - text_bounds.width() / 2), 
-            int(rect_bounds.height() / 2 - text_bounds.height() / 2)
-        )
-        self._track_id_text.setVisible(text_bounds.width() < rect_bounds.width())
-            
-    @property
-    def track(self):
-        return self._track
-    
-    def boundingRect(self) -> QtCore.QRectF:
-        return self._track_rect.boundingRect()
-    
-    def mousePressEvent(self, event: QtWidgets.QGraphicsSceneMouseEvent) -> None:
-        if event.button() == QtCore.Qt.MouseButton.LeftButton:
-            self.clicked.emit(self)
-        return super().mousePressEvent(event)
-    
-    def paint(self, painter: QtGui.QPainter, option: QtWidgets.QStyleOptionGraphicsItem, widget: QtWidgets.QWidget) -> None:
-        pass  # don't paint anything. we're just a container for child items.
-
+from PyQt6 import QtWidgets, QtCore, QtGui
+
+from boxjelly.lib.track import Track
+from boxjelly.lib.util import concept_color
+
+
+class TimelineTrack(QtWidgets.QGraphicsObject):
+    """
+    Graphical representation of a track within the timeline view.
+    """
+    
+    DEFAULT_HEIGHT = 30
+    
+    clicked = QtCore.pyqtSignal(object)
+    
+    def __init__(self, track: Track, scale_x: float = 1.0, scale_y: float = 1.0, parent=None):
+        super().__init__(parent)
+        
+        self._track = track  # original track
+        
+        self._scale_x = scale_x  # horizontal scale, in scene units per frame
+        self._scale_y = scale_y  # vertical scale, in scene units per height unit
+        
+        self._track_rect = QtWidgets.QGraphicsRectItem(self)
+        self._track_id_text = QtWidgets.QGraphicsSimpleTextItem(str(track.id)[:8], self)  # truncate to 8 characters
+        
+        self.update()
+        
+    def update(self):
+        self._track_rect.setBrush(concept_color(self._track.label_mode))
+        self._rescale()
+        super().update()
+    
+    def set_scale(self, scale_x: float, scale_y: float):
+        """
+        Set the scale of the track.
+        """
+        self._scale_x = scale_x
+        self._scale_y = scale_y
+        
+        self._rescale()
+    
+    def __len__(self):
+        return len(self._track)
+    
+    @property
+    def width_scene(self):
+        return len(self) * self._scale_x
+    
+    @property
+    def height_scene(self):
+        return self.DEFAULT_HEIGHT * self._scale_y 
+    
+    def _rescale(self):
+        """
+        Rescale the child items.
+        """
+        self._track_rect.setRect(0, 0, self.width_scene, self.height_scene)
+        
+        rect_bounds = self._track_rect.boundingRect()
+        text_bounds = self._track_id_text.boundingRect()
+        self._track_id_text.setPos(
+            int(rect_bounds.width() / 2 - text_bounds.width() / 2), 
+            int(rect_bounds.height() / 2 - text_bounds.height() / 2)
+        )
+        self._track_id_text.setVisible(text_bounds.width() < rect_bounds.width())
+            
+    @property
+    def track(self):
+        return self._track
+    
+    def boundingRect(self) -> QtCore.QRectF:
+        return self._track_rect.boundingRect()
+    
+    def mousePressEvent(self, event: QtWidgets.QGraphicsSceneMouseEvent) -> None:
+        if event.button() == QtCore.Qt.MouseButton.LeftButton:
+            self.clicked.emit(self)
+        return super().mousePressEvent(event)
+    
+    def paint(self, painter: QtGui.QPainter, option: QtWidgets.QStyleOptionGraphicsItem, widget: QtWidgets.QWidget) -> None:
+        pass  # don't paint anything. we're just a container for child items.
+
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/MainWindow.py` & `boxjelly-0.3.3/boxjelly/ui/MainWindow.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,321 +1,321 @@
-from PyQt6 import QtCore, QtMultimedia, QtWidgets, QtGui
-
-from boxjelly.commands.TrackListCommand import BatchRenameTracksCommand, DeleteTrackByIDCommand, BatchDeleteTracksByIDCommand, BatchRenameTracksCommand, SplitTrackCommand, MergeTracksCommand
-from boxjelly.lib.constants import APP_NAME
-from boxjelly.models.TrackListModel import TrackListModel
-from boxjelly.ui.OpenDialog import OpenDialog
-from boxjelly.ui.settings.SettingsDialog import SettingsDialog
-from boxjelly.ui.track.TrackPanel import TrackPanel
-from boxjelly.ui.video.CthulhuVideoController import CthulhuVideoController
-
-class MainWindow(QtWidgets.QMainWindow):
-    """Application main window"""
-    
-    mediaLoaded = QtCore.pyqtSignal(QtCore.QUrl)
-    tracksLoaded = QtCore.pyqtSignal(list)
-    
-    readRequested = QtCore.pyqtSignal()
-    writeRequested = QtCore.pyqtSignal(list)
-    
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        
-        # Set window title
-        self.setWindowTitle(APP_NAME)
-        
-        # Set window icon
-        self.setWindowIcon(QtGui.QIcon(':/icons/logo'))
-        
-        # Create media
-        self._media = None
-        
-        # Create track list model
-        self._track_model = TrackListModel(self)
-        
-        # Create selection model
-        self._selection_model = QtCore.QItemSelectionModel(self._track_model)
-        
-        # Create undo stack
-        self._undo_stack = QtGui.QUndoStack(self)
-        
-        # Create the menu bar
-        self._create_menu_bar()
-        
-        # Create the track panel and set it as the main widget
-        self._track_panel = TrackPanel(self, self._track_model, self._selection_model)
-        self.setCentralWidget(self._track_panel)
-        
-        # Create the Cthulhu video controller
-        self._video_controller = CthulhuVideoController(self, self._track_model, self._selection_model)
-        
-        # Create the settings dialog
-        self._settings_dialog = SettingsDialog(self)
-        
-        # Media content and track IO
-        self._media_content = None
-        self._track_io = None
-        
-        # Create the background worker thread
-        self._worker_thread = QtCore.QThread()
-        self._worker_thread.start()
-        
-        # Connect signals
-        self.mediaLoaded.connect(self._video_controller.set_media)
-        self._video_controller.mediaSetStatus.connect(self._on_media_set_status)
-        self._track_panel.frameSelected.connect(self._video_controller.set_frame)
-        self._video_controller.frameUpdated.connect(self._track_panel.show_frame)
-        self._selection_model.selectionChanged.connect(self._on_selection_changed)
-    
-    @QtCore.pyqtSlot(bool)
-    def _on_media_set_status(self, status):
-        """Handle the media set status."""
-        if not status:  # Failure to set media
-            QtWidgets.QMessageBox.critical(self, 'Error', 'Failed to open media in Cthulhu.\nIs Cthulhu running?')
-    
-    @QtCore.pyqtSlot(QtCore.QItemSelection, QtCore.QItemSelection)
-    def _on_selection_changed(self, selected: QtCore.QItemSelection, deselected: QtCore.QItemSelection):
-        # Select
-        for model_index in selected.indexes():
-            self._track_model.select_track(model_index.row())
-        
-        # Deselect
-        for model_index in deselected.indexes():
-            self._track_model.deselect_track(model_index.row())
-
-    def _create_menu_bar(self):
-        menu_bar = self.menuBar()
-        
-        # File menu
-        file_menu = menu_bar.addMenu('&File')
-        file_menu.addAction('&Open', QtGui.QKeySequence('Ctrl+O'), self.open)
-        file_menu.addAction('&Save', QtGui.QKeySequence('Ctrl+S'), self.save)
-        file_menu.addAction('Save &As', QtGui.QKeySequence('Ctrl+Shift+S'), self.save_as)
-        file_menu.addSeparator()
-        file_menu.addAction('Se&ttings', QtGui.QKeySequence('Ctrl+,'), self.open_settings)
-        file_menu.addSeparator()
-        file_menu.addAction('&Quit', QtGui.QKeySequence('Ctrl+Q'), self.close)
-        
-        # Edit menu
-        edit_menu = menu_bar.addMenu('&Edit')
-        rename_action = edit_menu.addAction(QtGui.QIcon(':/icons/rename'), 'Re&name', QtGui.QKeySequence('Ctrl+R'), self.rename_selected_tracks)
-        split_action = edit_menu.addAction(QtGui.QIcon(':/icons/split'), '&Split', QtGui.QKeySequence('Ctrl+N'), self.split_selected_track)
-        merge_action = edit_menu.addAction(QtGui.QIcon(':/icons/merge'), '&Merge', QtGui.QKeySequence('Ctrl+M'), self.merge_selected_tracks)
-        delete_action = edit_menu.addAction(QtGui.QIcon(':/icons/delete'), '&Delete', QtGui.QKeySequence('Del'), self.delete_selected_tracks)
-        edit_menu.addSeparator()
-        undo_action = edit_menu.addAction(QtGui.QIcon(':/icons/undo'), '&Undo', QtGui.QKeySequence('Ctrl+Z'), self._undo_stack.undo)
-        redo_action = edit_menu.addAction(QtGui.QIcon(':/icons/redo'), '&Redo', QtGui.QKeySequence('Ctrl+Shift+Z'), self._undo_stack.redo)
-        
-        # Go menu
-        go_menu = menu_bar.addMenu('&Go')
-        seek_beginning_action = go_menu.addAction(QtGui.QIcon(':/icons/seek_beginning'), 'Seek &beginning', QtGui.QKeySequence('Ctrl+['), self.seek_beginning_selected_tracks)
-        seek_end_action = go_menu.addAction(QtGui.QIcon(':/icons/seek_end'), 'Seek &end', QtGui.QKeySequence('Ctrl+]'), self.seek_end_selected_tracks)
-        
-        # Add actions to toolbar
-        toolbar = QtWidgets.QToolBar('Edit', self)
-        self.addToolBar(QtCore.Qt.ToolBarArea.LeftToolBarArea, toolbar)
-        toolbar.addActions([rename_action, split_action, merge_action, delete_action])
-        toolbar.addSeparator()
-        toolbar.addActions([seek_beginning_action, seek_end_action])
-        toolbar.addSeparator()
-        toolbar.addActions([undo_action, redo_action])
-    
-    def open_settings(self):
-        """Open the settings dialog."""
-        self._settings_dialog.show()
-    
-    def open(self):
-        """Show the open dialog and load."""
-        # Create and run the dialog
-        open_dialog = OpenDialog(self)
-        open_dialog.exec()
-        
-        # If not accepted, return
-        if open_dialog.result() != QtWidgets.QDialog.DialogCode.Accepted:
-            return
-        
-        # Otherwise, get the media content and track IO
-        self._media_content = open_dialog.media_content
-        self._track_io = open_dialog.track_io
-        
-        # Load the media
-        self.load_media(self._media_content)
-        
-        # Run the track IO read in the worker thread thread
-        self._track_io.moveToThread(self._worker_thread)
-        self._track_io.fileRead.connect(self._track_model.set_tracks)
-        self._track_io.fileWritten.connect(self._on_save_finished)
-        self._track_io.fileReadFailure.connect(self._on_read_failure)
-        self._track_io.fileWriteFailure.connect(self._on_write_failure)
-        self.readRequested.connect(self._track_io.read)
-        self.writeRequested.connect(self._track_io.write)
-        self.do_read()
-    
-    def do_read(self):
-        """Read the tracks from the track IO."""
-        self.readRequested.emit()
-        
-        # Show a progress dialog while reading
-        progress = QtWidgets.QProgressDialog('Reading tracks...', None, 0, 0, self)
-        progress.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
-        progress.setMinimumDuration(0)
-        progress.show()
-        
-        # Wait for the read to finish or fail, then close
-        self._track_io.fileRead.connect(progress.close)
-        self._track_io.fileReadFailure.connect(progress.close)
-    
-    @QtCore.pyqtSlot(str)
-    def _on_read_failure(self, error_message: str):
-        """Show a message box when reading fails."""
-        QtWidgets.QMessageBox.critical(self, 'Error', 'Failed to read tracks: \n\n{}'.format(error_message))
-    
-    def do_write(self):
-        """Write the tracks to the track IO."""
-        self.writeRequested.emit(self._track_model.get_all_tracks())
-    
-    @QtCore.pyqtSlot(str)
-    def _on_write_failure(self, error_message: str):
-        """Show a message box when writing fails."""
-        QtWidgets.QMessageBox.critical(self, 'Error', 'Failed to write tracks: \n\n{}'.format(error_message))
-    
-    @QtCore.pyqtSlot()
-    def _on_save_finished(self):
-        QtWidgets.QMessageBox.information(self, 'Saved', 'Saved successfully.')
-    
-    def save(self):
-        # If no track IO, show an error
-        if not self._track_io:
-            QtWidgets.QMessageBox.warning(self, 'Error', 'No file open.')
-            return
-        
-        # Get confirmation
-        confirm = QtWidgets.QMessageBox.question(self, 'Confirm', 'Are you sure you want to save?')
-        
-        # If confirmed, send the signal to save
-        if confirm == QtWidgets.QMessageBox.StandardButton.Yes:
-            self.do_write()
-    
-    def save_as(self):
-        # If no track IO, show an error
-        if not self._track_io:
-            QtWidgets.QMessageBox.warning(self, 'Error', 'No file open.')
-            return
-        
-        # Get the new file path, requiring the same suffix as the current
-        current_dir = self._track_io.path.parent
-        current_suffix = self._track_io.path.suffix
-        new_path_str, ok = QtWidgets.QFileDialog.getSaveFileName(self, 'Save As', str(current_dir), f'{current_suffix[1:].upper()} (*{current_suffix})')
-        
-        if not ok:
-            return
-        
-        # Update the track IO target path
-        self._track_io.path = new_path_str
-        
-        # Send the signal to save
-        self.do_write()
-        
-    
-    @QtCore.pyqtSlot(QtCore.QUrl)
-    def load_media(self, media):
-        """Load the media and emit the mediaLoaded signal."""
-        self._media = media
-        self.mediaLoaded.emit(media)
-    
-    @QtCore.pyqtSlot(list)
-    def load_tracks(self, tracks):
-        """Load the tracks and emit the tracksLoaded signal."""
-        self._track_model.set_tracks(tracks)
-        self.tracksLoaded.emit(tracks)
-    
-    @QtCore.pyqtSlot(int)
-    def delete_track(self, track_id):
-        """Delete a track from the model by its ID."""
-        command = DeleteTrackByIDCommand(self._track_model, track_id)
-        self._undo_stack.push(command)
-    
-    def delete_selected_tracks(self):
-        """Delete the selected tracks."""
-        selected_indices = self._selection_model.selectedIndexes()
-        selected_ids = [index.data(TrackListModel.IDRole) for index in selected_indices]
-        
-        command = BatchDeleteTracksByIDCommand(self._track_model, selected_ids)
-        self._undo_stack.push(command)
-    
-    def rename_selected_tracks(self):
-        """Change the label of a track by its ID."""
-        new_label, ok = QtWidgets.QInputDialog.getText(self, 'Rename track', 'Label:')
-        if not ok:
-            return
-        
-        selected_indices = self._selection_model.selectedIndexes()
-        selected_ids = [index.data(TrackListModel.IDRole) for index in selected_indices]
-        
-        command = BatchRenameTracksCommand(self._track_model, selected_ids, new_label)
-        self._undo_stack.push(command)
-        
-    def split_selected_track(self):
-        """Split a track at the current frame."""
-        selected_indices = self._selection_model.selectedIndexes()
-        if len(selected_indices) != 1:
-            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select a single track to split.')
-            return
-        
-        selected_id = selected_indices[0].data(TrackListModel.IDRole)
-        selected_start_frame = selected_indices[0].data(TrackListModel.StartFrameRole)
-        
-        split_idx = self._video_controller.get_frame_number() - selected_start_frame
-        
-        if not 1 <= split_idx <= len(selected_indices[0].data(TrackListModel.EventsRole)):
-            QtWidgets.QMessageBox.warning(self, 'Error', 'Invalid split position for selected track.')
-            return
-        
-        command = SplitTrackCommand(self._track_model, selected_id, split_idx)
-        self._undo_stack.push(command)
-        
-        # Add the new track to the selection
-        new_row_idx = self._track_model.index_by_id(command.new_track_id)
-        self._selection_model.select(self._track_model.index(new_row_idx), QtCore.QItemSelectionModel.SelectionFlag.Select)
-    
-    def merge_selected_tracks(self):
-        """Merge the selected tracks."""
-        selected_indices = self._selection_model.selectedIndexes()
-        if len(selected_indices) < 2:
-            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select at least two tracks to merge.')
-            return
-        
-        selected_ids = [index.data(TrackListModel.IDRole) for index in selected_indices]
-        
-        command = MergeTracksCommand(self._track_model, selected_ids)
-        self._undo_stack.push(command)
-        
-        # Add the new track to the selection
-        new_row_idx = self._track_model.index_by_id(command.new_track_id)
-        self._selection_model.select(self._track_model.index(new_row_idx), QtCore.QItemSelectionModel.SelectionFlag.Select)
-    
-    def seek_beginning_selected_tracks(self):
-        """Seek to the first frame of the selected tracks."""
-        selected_indices = self._selection_model.selectedIndexes()
-        if len(selected_indices) < 1:
-            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select at least one track to seek to.')
-            return
-        
-        selected_start_frames = [index.data(TrackListModel.StartFrameRole) for index in selected_indices]
-        
-        self._video_controller.set_frame(min(selected_start_frames))
-    
-    def seek_end_selected_tracks(self):
-        """Seek to the last frame of the selected tracks."""
-        selected_indices = self._selection_model.selectedIndexes()
-        if len(selected_indices) < 1:
-            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select at least one track to seek to.')
-            return
-        
-        selected_end_frames = [index.data(TrackListModel.EndFrameRole) for index in selected_indices]
-        
-        self._video_controller.set_frame(max(selected_end_frames))
-    
-    def closeEvent(self, a0: QtGui.QCloseEvent) -> None:
-        self._video_controller.try_close()
-        self._worker_thread.quit()
-        return super().closeEvent(a0)
+from PyQt6 import QtCore, QtMultimedia, QtWidgets, QtGui
+
+from boxjelly.commands.TrackListCommand import BatchRenameTracksCommand, DeleteTrackByIDCommand, BatchDeleteTracksByIDCommand, BatchRenameTracksCommand, SplitTrackCommand, MergeTracksCommand
+from boxjelly.lib.constants import APP_NAME
+from boxjelly.models.TrackListModel import TrackListModel
+from boxjelly.ui.OpenDialog import OpenDialog
+from boxjelly.ui.settings.SettingsDialog import SettingsDialog
+from boxjelly.ui.track.TrackPanel import TrackPanel
+from boxjelly.ui.video.CthulhuVideoController import CthulhuVideoController
+
+class MainWindow(QtWidgets.QMainWindow):
+    """Application main window"""
+    
+    mediaLoaded = QtCore.pyqtSignal(QtCore.QUrl)
+    tracksLoaded = QtCore.pyqtSignal(list)
+    
+    readRequested = QtCore.pyqtSignal()
+    writeRequested = QtCore.pyqtSignal(list)
+    
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        
+        # Set window title
+        self.setWindowTitle(APP_NAME)
+        
+        # Set window icon
+        self.setWindowIcon(QtGui.QIcon(':/icons/logo'))
+        
+        # Create media
+        self._media = None
+        
+        # Create track list model
+        self._track_model = TrackListModel(self)
+        
+        # Create selection model
+        self._selection_model = QtCore.QItemSelectionModel(self._track_model)
+        
+        # Create undo stack
+        self._undo_stack = QtGui.QUndoStack(self)
+        
+        # Create the menu bar
+        self._create_menu_bar()
+        
+        # Create the track panel and set it as the main widget
+        self._track_panel = TrackPanel(self, self._track_model, self._selection_model)
+        self.setCentralWidget(self._track_panel)
+        
+        # Create the Cthulhu video controller
+        self._video_controller = CthulhuVideoController(self, self._track_model, self._selection_model)
+        
+        # Create the settings dialog
+        self._settings_dialog = SettingsDialog(self)
+        
+        # Media content and track IO
+        self._media_content = None
+        self._track_io = None
+        
+        # Create the background worker thread
+        self._worker_thread = QtCore.QThread()
+        self._worker_thread.start()
+        
+        # Connect signals
+        self.mediaLoaded.connect(self._video_controller.set_media)
+        self._video_controller.mediaSetStatus.connect(self._on_media_set_status)
+        self._track_panel.frameSelected.connect(self._video_controller.set_frame)
+        self._video_controller.frameUpdated.connect(self._track_panel.show_frame)
+        self._selection_model.selectionChanged.connect(self._on_selection_changed)
+    
+    @QtCore.pyqtSlot(bool)
+    def _on_media_set_status(self, status):
+        """Handle the media set status."""
+        if not status:  # Failure to set media
+            QtWidgets.QMessageBox.critical(self, 'Error', 'Failed to open media in Cthulhu.\nIs Cthulhu running?')
+    
+    @QtCore.pyqtSlot(QtCore.QItemSelection, QtCore.QItemSelection)
+    def _on_selection_changed(self, selected: QtCore.QItemSelection, deselected: QtCore.QItemSelection):
+        # Select
+        for model_index in selected.indexes():
+            self._track_model.select_track(model_index.row())
+        
+        # Deselect
+        for model_index in deselected.indexes():
+            self._track_model.deselect_track(model_index.row())
+
+    def _create_menu_bar(self):
+        menu_bar = self.menuBar()
+        
+        # File menu
+        file_menu = menu_bar.addMenu('&File')
+        file_menu.addAction('&Open', QtGui.QKeySequence('Ctrl+O'), self.open)
+        file_menu.addAction('&Save', QtGui.QKeySequence('Ctrl+S'), self.save)
+        file_menu.addAction('Save &As', QtGui.QKeySequence('Ctrl+Shift+S'), self.save_as)
+        file_menu.addSeparator()
+        file_menu.addAction('Se&ttings', QtGui.QKeySequence('Ctrl+,'), self.open_settings)
+        file_menu.addSeparator()
+        file_menu.addAction('&Quit', QtGui.QKeySequence('Ctrl+Q'), self.close)
+        
+        # Edit menu
+        edit_menu = menu_bar.addMenu('&Edit')
+        rename_action = edit_menu.addAction(QtGui.QIcon(':/icons/rename'), 'Re&name', QtGui.QKeySequence('Ctrl+R'), self.rename_selected_tracks)
+        split_action = edit_menu.addAction(QtGui.QIcon(':/icons/split'), '&Split', QtGui.QKeySequence('Ctrl+N'), self.split_selected_track)
+        merge_action = edit_menu.addAction(QtGui.QIcon(':/icons/merge'), '&Merge', QtGui.QKeySequence('Ctrl+M'), self.merge_selected_tracks)
+        delete_action = edit_menu.addAction(QtGui.QIcon(':/icons/delete'), '&Delete', QtGui.QKeySequence('Del'), self.delete_selected_tracks)
+        edit_menu.addSeparator()
+        undo_action = edit_menu.addAction(QtGui.QIcon(':/icons/undo'), '&Undo', QtGui.QKeySequence('Ctrl+Z'), self._undo_stack.undo)
+        redo_action = edit_menu.addAction(QtGui.QIcon(':/icons/redo'), '&Redo', QtGui.QKeySequence('Ctrl+Shift+Z'), self._undo_stack.redo)
+        
+        # Go menu
+        go_menu = menu_bar.addMenu('&Go')
+        seek_beginning_action = go_menu.addAction(QtGui.QIcon(':/icons/seek_beginning'), 'Seek &beginning', QtGui.QKeySequence('Ctrl+['), self.seek_beginning_selected_tracks)
+        seek_end_action = go_menu.addAction(QtGui.QIcon(':/icons/seek_end'), 'Seek &end', QtGui.QKeySequence('Ctrl+]'), self.seek_end_selected_tracks)
+        
+        # Add actions to toolbar
+        toolbar = QtWidgets.QToolBar('Edit', self)
+        self.addToolBar(QtCore.Qt.ToolBarArea.LeftToolBarArea, toolbar)
+        toolbar.addActions([rename_action, split_action, merge_action, delete_action])
+        toolbar.addSeparator()
+        toolbar.addActions([seek_beginning_action, seek_end_action])
+        toolbar.addSeparator()
+        toolbar.addActions([undo_action, redo_action])
+    
+    def open_settings(self):
+        """Open the settings dialog."""
+        self._settings_dialog.show()
+    
+    def open(self):
+        """Show the open dialog and load."""
+        # Create and run the dialog
+        open_dialog = OpenDialog(self)
+        open_dialog.exec()
+        
+        # If not accepted, return
+        if open_dialog.result() != QtWidgets.QDialog.DialogCode.Accepted:
+            return
+        
+        # Otherwise, get the media content and track IO
+        self._media_content = open_dialog.media_content
+        self._track_io = open_dialog.track_io
+        
+        # Load the media
+        self.load_media(self._media_content)
+        
+        # Run the track IO read in the worker thread thread
+        self._track_io.moveToThread(self._worker_thread)
+        self._track_io.fileRead.connect(self._track_model.set_tracks)
+        self._track_io.fileWritten.connect(self._on_save_finished)
+        self._track_io.fileReadFailure.connect(self._on_read_failure)
+        self._track_io.fileWriteFailure.connect(self._on_write_failure)
+        self.readRequested.connect(self._track_io.read)
+        self.writeRequested.connect(self._track_io.write)
+        self.do_read()
+    
+    def do_read(self):
+        """Read the tracks from the track IO."""
+        self.readRequested.emit()
+        
+        # Show a progress dialog while reading
+        progress = QtWidgets.QProgressDialog('Reading tracks...', None, 0, 0, self)
+        progress.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
+        progress.setMinimumDuration(0)
+        progress.show()
+        
+        # Wait for the read to finish or fail, then close
+        self._track_io.fileRead.connect(progress.close)
+        self._track_io.fileReadFailure.connect(progress.close)
+    
+    @QtCore.pyqtSlot(str)
+    def _on_read_failure(self, error_message: str):
+        """Show a message box when reading fails."""
+        QtWidgets.QMessageBox.critical(self, 'Error', 'Failed to read tracks: \n\n{}'.format(error_message))
+    
+    def do_write(self):
+        """Write the tracks to the track IO."""
+        self.writeRequested.emit(self._track_model.get_all_tracks())
+    
+    @QtCore.pyqtSlot(str)
+    def _on_write_failure(self, error_message: str):
+        """Show a message box when writing fails."""
+        QtWidgets.QMessageBox.critical(self, 'Error', 'Failed to write tracks: \n\n{}'.format(error_message))
+    
+    @QtCore.pyqtSlot()
+    def _on_save_finished(self):
+        QtWidgets.QMessageBox.information(self, 'Saved', 'Saved successfully.')
+    
+    def save(self):
+        # If no track IO, show an error
+        if not self._track_io:
+            QtWidgets.QMessageBox.warning(self, 'Error', 'No file open.')
+            return
+        
+        # Get confirmation
+        confirm = QtWidgets.QMessageBox.question(self, 'Confirm', 'Are you sure you want to save?')
+        
+        # If confirmed, send the signal to save
+        if confirm == QtWidgets.QMessageBox.StandardButton.Yes:
+            self.do_write()
+    
+    def save_as(self):
+        # If no track IO, show an error
+        if not self._track_io:
+            QtWidgets.QMessageBox.warning(self, 'Error', 'No file open.')
+            return
+        
+        # Get the new file path, requiring the same suffix as the current
+        current_dir = self._track_io.path.parent
+        current_suffix = self._track_io.path.suffix
+        new_path_str, ok = QtWidgets.QFileDialog.getSaveFileName(self, 'Save As', str(current_dir), f'{current_suffix[1:].upper()} (*{current_suffix})')
+        
+        if not ok:
+            return
+        
+        # Update the track IO target path
+        self._track_io.path = new_path_str
+        
+        # Send the signal to save
+        self.do_write()
+        
+    
+    @QtCore.pyqtSlot(QtCore.QUrl)
+    def load_media(self, media):
+        """Load the media and emit the mediaLoaded signal."""
+        self._media = media
+        self.mediaLoaded.emit(media)
+    
+    @QtCore.pyqtSlot(list)
+    def load_tracks(self, tracks):
+        """Load the tracks and emit the tracksLoaded signal."""
+        self._track_model.set_tracks(tracks)
+        self.tracksLoaded.emit(tracks)
+    
+    @QtCore.pyqtSlot(int)
+    def delete_track(self, track_id):
+        """Delete a track from the model by its ID."""
+        command = DeleteTrackByIDCommand(self._track_model, track_id)
+        self._undo_stack.push(command)
+    
+    def delete_selected_tracks(self):
+        """Delete the selected tracks."""
+        selected_indices = self._selection_model.selectedIndexes()
+        selected_ids = [index.data(TrackListModel.IDRole) for index in selected_indices]
+        
+        command = BatchDeleteTracksByIDCommand(self._track_model, selected_ids)
+        self._undo_stack.push(command)
+    
+    def rename_selected_tracks(self):
+        """Change the label of a track by its ID."""
+        new_label, ok = QtWidgets.QInputDialog.getText(self, 'Rename track', 'Label:')
+        if not ok:
+            return
+        
+        selected_indices = self._selection_model.selectedIndexes()
+        selected_ids = [index.data(TrackListModel.IDRole) for index in selected_indices]
+        
+        command = BatchRenameTracksCommand(self._track_model, selected_ids, new_label)
+        self._undo_stack.push(command)
+        
+    def split_selected_track(self):
+        """Split a track at the current frame."""
+        selected_indices = self._selection_model.selectedIndexes()
+        if len(selected_indices) != 1:
+            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select a single track to split.')
+            return
+        
+        selected_id = selected_indices[0].data(TrackListModel.IDRole)
+        selected_start_frame = selected_indices[0].data(TrackListModel.StartFrameRole)
+        
+        split_idx = self._video_controller.get_frame_number() - selected_start_frame
+        
+        if not 1 <= split_idx <= len(selected_indices[0].data(TrackListModel.EventsRole)):
+            QtWidgets.QMessageBox.warning(self, 'Error', 'Invalid split position for selected track.')
+            return
+        
+        command = SplitTrackCommand(self._track_model, selected_id, split_idx)
+        self._undo_stack.push(command)
+        
+        # Add the new track to the selection
+        new_row_idx = self._track_model.index_by_id(command.new_track_id)
+        self._selection_model.select(self._track_model.index(new_row_idx), QtCore.QItemSelectionModel.SelectionFlag.Select)
+    
+    def merge_selected_tracks(self):
+        """Merge the selected tracks."""
+        selected_indices = self._selection_model.selectedIndexes()
+        if len(selected_indices) < 2:
+            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select at least two tracks to merge.')
+            return
+        
+        selected_ids = [index.data(TrackListModel.IDRole) for index in selected_indices]
+        
+        command = MergeTracksCommand(self._track_model, selected_ids)
+        self._undo_stack.push(command)
+        
+        # Add the new track to the selection
+        new_row_idx = self._track_model.index_by_id(command.new_track_id)
+        self._selection_model.select(self._track_model.index(new_row_idx), QtCore.QItemSelectionModel.SelectionFlag.Select)
+    
+    def seek_beginning_selected_tracks(self):
+        """Seek to the first frame of the selected tracks."""
+        selected_indices = self._selection_model.selectedIndexes()
+        if len(selected_indices) < 1:
+            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select at least one track to seek to.')
+            return
+        
+        selected_start_frames = [index.data(TrackListModel.StartFrameRole) for index in selected_indices]
+        
+        self._video_controller.set_frame(min(selected_start_frames))
+    
+    def seek_end_selected_tracks(self):
+        """Seek to the last frame of the selected tracks."""
+        selected_indices = self._selection_model.selectedIndexes()
+        if len(selected_indices) < 1:
+            QtWidgets.QMessageBox.warning(self, 'Error', 'Please select at least one track to seek to.')
+            return
+        
+        selected_end_frames = [index.data(TrackListModel.EndFrameRole) for index in selected_indices]
+        
+        self._video_controller.set_frame(max(selected_end_frames))
+    
+    def closeEvent(self, a0: QtGui.QCloseEvent) -> None:
+        self._video_controller.try_close()
+        self._worker_thread.quit()
+        return super().closeEvent(a0)
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/MediaSelectionBox.py` & `boxjelly-0.3.3/boxjelly/ui/MediaSelectionBox.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from PyQt6 import QtWidgets, QtCore
-
-from boxjelly.ui.WidgetComboBox import WidgetComboBox
-from boxjelly.ui.SourceWidgets import LocalVideoMediaSourceWidget, URLMediaSourceWidget
-
-
-class MediaSelectionBox(QtWidgets.QGroupBox):
-    """Media selection group box"""
-    
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        
-        self.setTitle('Media')
-        
-        self.widget_combo_box = WidgetComboBox(self)
-        self.widget_combo_box.add_widget(LocalVideoMediaSourceWidget(self), 'Video file')
-        self.widget_combo_box.add_widget(URLMediaSourceWidget(self), 'Video URL')
-        self.widget_combo_box.refresh()
-        
-        self.arrange()
-    
-    def arrange(self):
-        """Arrange the widget"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        # Add widget combo box
-        self.layout().addWidget(self.widget_combo_box)
-        
-        # Add stretch
-        self.layout().addStretch()
-    
-    @property
-    def media_content(self) -> QtCore.QUrl:
-        return self.widget_combo_box.widget.media_content
+from PyQt6 import QtWidgets, QtCore
+
+from boxjelly.ui.WidgetComboBox import WidgetComboBox
+from boxjelly.ui.SourceWidgets import LocalVideoMediaSourceWidget, URLMediaSourceWidget
+
+
+class MediaSelectionBox(QtWidgets.QGroupBox):
+    """Media selection group box"""
+    
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        
+        self.setTitle('Media')
+        
+        self.widget_combo_box = WidgetComboBox(self)
+        self.widget_combo_box.add_widget(LocalVideoMediaSourceWidget(self), 'Video file')
+        self.widget_combo_box.add_widget(URLMediaSourceWidget(self), 'Video URL')
+        self.widget_combo_box.refresh()
+        
+        self.arrange()
+    
+    def arrange(self):
+        """Arrange the widget"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        # Add widget combo box
+        self.layout().addWidget(self.widget_combo_box)
+        
+        # Add stretch
+        self.layout().addStretch()
+    
+    @property
+    def media_content(self) -> QtCore.QUrl:
+        return self.widget_combo_box.widget.media_content
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/OpenDialog.py` & `boxjelly-0.3.3/boxjelly/ui/OpenDialog.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from PyQt6 import QtWidgets, QtGui
-
-from boxjelly.ui.MediaSelectionBox import MediaSelectionBox
-from boxjelly.ui.TrackSelectionBox import TrackSelectionBox
-
-
-class OpenDialog(QtWidgets.QDialog):
-    """Dialog to get a video and track source."""
-    
-    def __init__(self, parent):
-        super().__init__(parent)
-        
-        # Style
-        self.setWindowTitle('Open')
-        self.setModal(True)
-        self.resize(500, 0)
-        
-        # Create the selection boxes
-        self._media_selection_box = MediaSelectionBox()
-        self._track_selection_box = TrackSelectionBox()
-        
-        # Create the dialog buttons
-        self._button_box = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.StandardButton.Ok | QtWidgets.QDialogButtonBox.StandardButton.Cancel)
-        self._button_box.accepted.connect(self.accept)
-        self._button_box.rejected.connect(self.reject)
-        
-        # Arrange the widgets
-        self._arrange()
-        
-    def _arrange(self):
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        self.layout().addWidget(self._media_selection_box)
-        self.layout().addWidget(self._track_selection_box)
-        self.layout().addWidget(self._button_box)
-    
-    @property
-    def media_content(self):
-        return self._media_selection_box.media_content
-    
-    @property
-    def track_io(self):
-        return self._track_selection_box.io
+from PyQt6 import QtWidgets, QtGui
+
+from boxjelly.ui.MediaSelectionBox import MediaSelectionBox
+from boxjelly.ui.TrackSelectionBox import TrackSelectionBox
+
+
+class OpenDialog(QtWidgets.QDialog):
+    """Dialog to get a video and track source."""
+    
+    def __init__(self, parent):
+        super().__init__(parent)
+        
+        # Style
+        self.setWindowTitle('Open')
+        self.setModal(True)
+        self.resize(500, 0)
+        
+        # Create the selection boxes
+        self._media_selection_box = MediaSelectionBox()
+        self._track_selection_box = TrackSelectionBox()
+        
+        # Create the dialog buttons
+        self._button_box = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.StandardButton.Ok | QtWidgets.QDialogButtonBox.StandardButton.Cancel)
+        self._button_box.accepted.connect(self.accept)
+        self._button_box.rejected.connect(self.reject)
+        
+        # Arrange the widgets
+        self._arrange()
+        
+    def _arrange(self):
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        self.layout().addWidget(self._media_selection_box)
+        self.layout().addWidget(self._track_selection_box)
+        self.layout().addWidget(self._button_box)
+    
+    @property
+    def media_content(self):
+        return self._media_selection_box.media_content
+    
+    @property
+    def track_io(self):
+        return self._track_selection_box.io
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/settings/SettingsDialog.py` & `boxjelly-0.3.3/boxjelly/ui/settings/SettingsDialog.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-
-from PyQt6 import QtWidgets, QtCore, QtGui
-
-from boxjelly.ui.settings.tabs.AbstractSettingsTab import AbstractSettingsTab
-from boxjelly.ui.settings.tabs.NetworkSettingsTab import NetworkSettingsTab
-from boxjelly.ui.settings.tabs.VideoSettingsTab import VideoSettingsTab
-
-
-class SettingsDialog(QtWidgets.QDialog):
-    """
-    Settings dialog.
-
-    Contains settings for the application.
-    """
-    
-    applySettings = QtCore.pyqtSignal()
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        
-        self.setWindowTitle('Settings')
-        
-        # Create tab widget to hold settings pages
-        self._tab_widget = QtWidgets.QTabWidget()
-        
-        # Create button box (OK, Apply, Cancel)
-        self._button_box = QtWidgets.QDialogButtonBox(
-            QtWidgets.QDialogButtonBox.StandardButton.Ok | 
-            QtWidgets.QDialogButtonBox.StandardButton.Apply | 
-            QtWidgets.QDialogButtonBox.StandardButton.Cancel
-        )
-        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).pressed.connect(self.accept)
-        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Apply).pressed.connect(self._on_apply_pressed)
-        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Cancel).pressed.connect(self.reject)
-        
-        # self.accepted.connect(self.close)
-        self.accepted.connect(self._apply)
-        self._needs_apply = False
-        self._update_apply_enabled()
-        
-        # Add tabs
-        self._add_tabs()
-        
-        # Arrange the dialog layout
-        self._arrange()
-        
-    def _arrange(self):
-        layout = QtWidgets.QVBoxLayout()
-        
-        layout.addWidget(self._tab_widget)
-        layout.addWidget(self._button_box)
-        
-        self.setLayout(layout)
-    
-    def _update_apply_enabled(self):
-        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Apply).setEnabled(self._needs_apply)
-    
-    def _on_settings_changed(self):
-        self._needs_apply = True
-        self._update_apply_enabled()
-    
-    def _on_apply_pressed(self):
-        self._apply()
-        
-        self._needs_apply = False
-        self._update_apply_enabled()
-    
-    def _apply(self):
-        if self._needs_apply:
-            self.applySettings.emit()
-    
-    def _register_tab(self, tab: AbstractSettingsTab):
-        # Add tab to tab widget
-        if tab.icon is not None:
-            self._tab_widget.addTab(tab, tab.icon, tab.name)
-        else:
-            self._tab_widget.addTab(tab, tab.name)
-            
-        # Connect signals/slots
-        tab.settingsChanged.connect(self._on_settings_changed)
-        self.applySettings.connect(tab.apply_settings)
-    
-    def _add_tabs(self):
-        network_tab = NetworkSettingsTab()
-        self._register_tab(network_tab)
-        
-        video_tab = VideoSettingsTab()
-        self._register_tab(video_tab)
+
+from PyQt6 import QtWidgets, QtCore, QtGui
+
+from boxjelly.ui.settings.tabs.AbstractSettingsTab import AbstractSettingsTab
+from boxjelly.ui.settings.tabs.NetworkSettingsTab import NetworkSettingsTab
+from boxjelly.ui.settings.tabs.VideoSettingsTab import VideoSettingsTab
+
+
+class SettingsDialog(QtWidgets.QDialog):
+    """
+    Settings dialog.
+
+    Contains settings for the application.
+    """
+    
+    applySettings = QtCore.pyqtSignal()
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        
+        self.setWindowTitle('Settings')
+        
+        # Create tab widget to hold settings pages
+        self._tab_widget = QtWidgets.QTabWidget()
+        
+        # Create button box (OK, Apply, Cancel)
+        self._button_box = QtWidgets.QDialogButtonBox(
+            QtWidgets.QDialogButtonBox.StandardButton.Ok | 
+            QtWidgets.QDialogButtonBox.StandardButton.Apply | 
+            QtWidgets.QDialogButtonBox.StandardButton.Cancel
+        )
+        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).pressed.connect(self.accept)
+        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Apply).pressed.connect(self._on_apply_pressed)
+        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Cancel).pressed.connect(self.reject)
+        
+        # self.accepted.connect(self.close)
+        self.accepted.connect(self._apply)
+        self._needs_apply = False
+        self._update_apply_enabled()
+        
+        # Add tabs
+        self._add_tabs()
+        
+        # Arrange the dialog layout
+        self._arrange()
+        
+    def _arrange(self):
+        layout = QtWidgets.QVBoxLayout()
+        
+        layout.addWidget(self._tab_widget)
+        layout.addWidget(self._button_box)
+        
+        self.setLayout(layout)
+    
+    def _update_apply_enabled(self):
+        self._button_box.button(QtWidgets.QDialogButtonBox.StandardButton.Apply).setEnabled(self._needs_apply)
+    
+    def _on_settings_changed(self):
+        self._needs_apply = True
+        self._update_apply_enabled()
+    
+    def _on_apply_pressed(self):
+        self._apply()
+        
+        self._needs_apply = False
+        self._update_apply_enabled()
+    
+    def _apply(self):
+        if self._needs_apply:
+            self.applySettings.emit()
+    
+    def _register_tab(self, tab: AbstractSettingsTab):
+        # Add tab to tab widget
+        if tab.icon is not None:
+            self._tab_widget.addTab(tab, tab.icon, tab.name)
+        else:
+            self._tab_widget.addTab(tab, tab.name)
+            
+        # Connect signals/slots
+        tab.settingsChanged.connect(self._on_settings_changed)
+        self.applySettings.connect(tab.apply_settings)
+    
+    def _add_tabs(self):
+        network_tab = NetworkSettingsTab()
+        self._register_tab(network_tab)
+        
+        video_tab = VideoSettingsTab()
+        self._register_tab(video_tab)
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/settings/tabs/NetworkSettingsTab.py` & `boxjelly-0.3.3/boxjelly/ui/settings/tabs/NetworkSettingsTab.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from PyQt6 import QtWidgets
-
-from boxjelly.ui.settings.tabs.AbstractSettingsTab import AbstractSettingsTab
-
-
-class NetworkSettingsTab(AbstractSettingsTab):
-    """
-    Network settings tab.
-    """
-    
-    def __init__(self, parent=None):
-        super().__init__('Network', parent=parent)
-        
-        self._remote_control_section = QtWidgets.QGroupBox('Remote Control')
-        
-        self._control_port_edit = QtWidgets.QSpinBox()
-        self._control_port_edit.setRange(0, 65535)
-        self._control_port_edit.setValue(self._settings.control_port.value)
-        
-        self._localization_section = QtWidgets.QGroupBox('Localization')
-        
-        self._incoming_port_edit = QtWidgets.QSpinBox()
-        self._incoming_port_edit.setRange(0, 65535)
-        self._incoming_port_edit.setValue(self._settings.incoming_port.value)
-        
-        self._incoming_port_topic_edit = QtWidgets.QLineEdit()
-        self._incoming_port_topic_edit.setText(self._settings.incoming_topic.value)
-        
-        self._outgoing_port_edit = QtWidgets.QSpinBox()
-        self._outgoing_port_edit.setRange(0, 65535)
-        self._outgoing_port_edit.setValue(self._settings.outgoing_port.value)
-        
-        self._outgoing_port_topic_edit = QtWidgets.QLineEdit()
-        self._outgoing_port_topic_edit.setText(self._settings.outgoing_topic.value)
-        
-        self._cthulhu_section = QtWidgets.QGroupBox('Cthulhu')
-        self._selection_enabled_checkbox = QtWidgets.QCheckBox()
-        self._selection_enabled_checkbox.setChecked(self._settings.selection_enabled.value)
-        
-        self._control_port_edit.valueChanged.connect(self._settings_changed)
-        self._incoming_port_edit.valueChanged.connect(self._settings_changed)
-        self._incoming_port_topic_edit.textChanged.connect(self._settings_changed)
-        self._outgoing_port_edit.valueChanged.connect(self._settings_changed)
-        self._outgoing_port_topic_edit.textChanged.connect(self._settings_changed)
-        self._selection_enabled_checkbox.stateChanged.connect(self._settings_changed)
-        
-        self._arrange()
-    
-    def _arrange(self):
-        layout = QtWidgets.QVBoxLayout()
-        
-        remote_control_layout = QtWidgets.QFormLayout()
-        remote_control_layout.addRow('Control Port', self._control_port_edit)
-        self._remote_control_section.setLayout(remote_control_layout)
-        
-        localization_layout = QtWidgets.QFormLayout()
-        localization_layout.addRow('Incoming Port', self._incoming_port_edit)
-        localization_layout.addRow('Incoming Topic', self._incoming_port_topic_edit)
-        localization_layout.addRow('Outgoing Port', self._outgoing_port_edit)
-        localization_layout.addRow('Outgoing Topic', self._outgoing_port_topic_edit)
-        self._localization_section.setLayout(localization_layout)
-        
-        cthulhu_layout = QtWidgets.QFormLayout()
-        cthulhu_layout.addRow('Enable Selection Highlight', self._selection_enabled_checkbox)
-        self._cthulhu_section.setLayout(cthulhu_layout)
-        
-        layout.addWidget(self._remote_control_section)
-        layout.addWidget(self._localization_section)
-        layout.addWidget(self._cthulhu_section)
-        
-        self.setLayout(layout)
-    
-    def apply_settings(self):
-        # Remote control
-        self._settings.control_port.value = self._control_port_edit.value()
-        
-        # Localization control
-        if self._settings.incoming_port.value != self._incoming_port_edit.value():
-            self._settings.incoming_port.value = self._incoming_port_edit.value()
-        
-        if self._settings.incoming_topic.value != self._incoming_port_topic_edit.text():
-            self._settings.incoming_topic.value = self._incoming_port_topic_edit.text()
-        
-        if self._settings.outgoing_port.value != self._outgoing_port_edit.value():
-            self._settings.outgoing_port.value = self._outgoing_port_edit.value()
-        
-        if self._settings.outgoing_topic.value != self._outgoing_port_topic_edit.text():
-            self._settings.outgoing_topic.value = self._outgoing_port_topic_edit.text()
-        
-        # Selection enable/disable
-        self._settings.selection_enabled.value = self._selection_enabled_checkbox.isChecked()
+from PyQt6 import QtWidgets
+
+from boxjelly.ui.settings.tabs.AbstractSettingsTab import AbstractSettingsTab
+
+
+class NetworkSettingsTab(AbstractSettingsTab):
+    """
+    Network settings tab.
+    """
+    
+    def __init__(self, parent=None):
+        super().__init__('Network', parent=parent)
+        
+        self._remote_control_section = QtWidgets.QGroupBox('Remote Control')
+        
+        self._control_port_edit = QtWidgets.QSpinBox()
+        self._control_port_edit.setRange(0, 65535)
+        self._control_port_edit.setValue(self._settings.control_port.value)
+        
+        self._localization_section = QtWidgets.QGroupBox('Localization')
+        
+        self._incoming_port_edit = QtWidgets.QSpinBox()
+        self._incoming_port_edit.setRange(0, 65535)
+        self._incoming_port_edit.setValue(self._settings.incoming_port.value)
+        
+        self._incoming_port_topic_edit = QtWidgets.QLineEdit()
+        self._incoming_port_topic_edit.setText(self._settings.incoming_topic.value)
+        
+        self._outgoing_port_edit = QtWidgets.QSpinBox()
+        self._outgoing_port_edit.setRange(0, 65535)
+        self._outgoing_port_edit.setValue(self._settings.outgoing_port.value)
+        
+        self._outgoing_port_topic_edit = QtWidgets.QLineEdit()
+        self._outgoing_port_topic_edit.setText(self._settings.outgoing_topic.value)
+        
+        self._cthulhu_section = QtWidgets.QGroupBox('Cthulhu')
+        self._selection_enabled_checkbox = QtWidgets.QCheckBox()
+        self._selection_enabled_checkbox.setChecked(self._settings.selection_enabled.value)
+        
+        self._control_port_edit.valueChanged.connect(self._settings_changed)
+        self._incoming_port_edit.valueChanged.connect(self._settings_changed)
+        self._incoming_port_topic_edit.textChanged.connect(self._settings_changed)
+        self._outgoing_port_edit.valueChanged.connect(self._settings_changed)
+        self._outgoing_port_topic_edit.textChanged.connect(self._settings_changed)
+        self._selection_enabled_checkbox.stateChanged.connect(self._settings_changed)
+        
+        self._arrange()
+    
+    def _arrange(self):
+        layout = QtWidgets.QVBoxLayout()
+        
+        remote_control_layout = QtWidgets.QFormLayout()
+        remote_control_layout.addRow('Control Port', self._control_port_edit)
+        self._remote_control_section.setLayout(remote_control_layout)
+        
+        localization_layout = QtWidgets.QFormLayout()
+        localization_layout.addRow('Incoming Port', self._incoming_port_edit)
+        localization_layout.addRow('Incoming Topic', self._incoming_port_topic_edit)
+        localization_layout.addRow('Outgoing Port', self._outgoing_port_edit)
+        localization_layout.addRow('Outgoing Topic', self._outgoing_port_topic_edit)
+        self._localization_section.setLayout(localization_layout)
+        
+        cthulhu_layout = QtWidgets.QFormLayout()
+        cthulhu_layout.addRow('Enable Selection Highlight', self._selection_enabled_checkbox)
+        self._cthulhu_section.setLayout(cthulhu_layout)
+        
+        layout.addWidget(self._remote_control_section)
+        layout.addWidget(self._localization_section)
+        layout.addWidget(self._cthulhu_section)
+        
+        self.setLayout(layout)
+    
+    def apply_settings(self):
+        # Remote control
+        self._settings.control_port.value = self._control_port_edit.value()
+        
+        # Localization control
+        if self._settings.incoming_port.value != self._incoming_port_edit.value():
+            self._settings.incoming_port.value = self._incoming_port_edit.value()
+        
+        if self._settings.incoming_topic.value != self._incoming_port_topic_edit.text():
+            self._settings.incoming_topic.value = self._incoming_port_topic_edit.text()
+        
+        if self._settings.outgoing_port.value != self._outgoing_port_edit.value():
+            self._settings.outgoing_port.value = self._outgoing_port_edit.value()
+        
+        if self._settings.outgoing_topic.value != self._outgoing_port_topic_edit.text():
+            self._settings.outgoing_topic.value = self._outgoing_port_topic_edit.text()
+        
+        # Selection enable/disable
+        self._settings.selection_enabled.value = self._selection_enabled_checkbox.isChecked()
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/settings/tabs/VideoSettingsTab.py` & `boxjelly-0.3.3/boxjelly/ui/settings/tabs/VideoSettingsTab.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from PyQt6 import QtWidgets
-
-from boxjelly.ui.settings.tabs.AbstractSettingsTab import AbstractSettingsTab
-
-
-class VideoSettingsTab(AbstractSettingsTab):
-    """
-    Video settings tab.
-    """
-    
-    def __init__(self, parent=None):
-        super().__init__('Video', parent=parent)
-        
-        self._frame_rate_edit = QtWidgets.QDoubleSpinBox()
-        self._frame_rate_edit.setRange(0.01, 1000.0)
-        self._frame_rate_edit.setDecimals(2)
-        self._frame_rate_edit.setSuffix(' fps')
-        self._frame_rate_edit.setSingleStep(0.01)
-        self._frame_rate_edit.setStepType(QtWidgets.QAbstractSpinBox.StepType.DefaultStepType)
-        self._frame_rate_edit.setValue(self._settings.frame_rate.value)
-        
-        self._frame_rate_edit.valueChanged.connect(self._settings_changed)
-        
-        self._arrange()
-    
-    def _arrange(self):
-        layout = QtWidgets.QFormLayout()
-        
-        layout.addRow('Frame Rate', self._frame_rate_edit)
-        
-        self.setLayout(layout)
-    
-    def apply_settings(self):
-        self._settings.frame_rate.value = self._frame_rate_edit.value()
+from PyQt6 import QtWidgets
+
+from boxjelly.ui.settings.tabs.AbstractSettingsTab import AbstractSettingsTab
+
+
+class VideoSettingsTab(AbstractSettingsTab):
+    """
+    Video settings tab.
+    """
+    
+    def __init__(self, parent=None):
+        super().__init__('Video', parent=parent)
+        
+        self._frame_rate_edit = QtWidgets.QDoubleSpinBox()
+        self._frame_rate_edit.setRange(0.01, 1000.0)
+        self._frame_rate_edit.setDecimals(2)
+        self._frame_rate_edit.setSuffix(' fps')
+        self._frame_rate_edit.setSingleStep(0.01)
+        self._frame_rate_edit.setStepType(QtWidgets.QAbstractSpinBox.StepType.DefaultStepType)
+        self._frame_rate_edit.setValue(self._settings.frame_rate.value)
+        
+        self._frame_rate_edit.valueChanged.connect(self._settings_changed)
+        
+        self._arrange()
+    
+    def _arrange(self):
+        layout = QtWidgets.QFormLayout()
+        
+        layout.addRow('Frame Rate', self._frame_rate_edit)
+        
+        self.setLayout(layout)
+    
+    def apply_settings(self):
+        self._settings.frame_rate.value = self._frame_rate_edit.value()
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/SourceWidgets.py` & `boxjelly-0.3.3/boxjelly/ui/SourceWidgets.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-from PyQt6 import QtWidgets, QtMultimedia, QtCore
-
-from boxjelly.lib.fileio import AbstractTrackFileIO, DeepseaTrackFileIO, JSONTrackFileIO, YOLOv5DeepSortTrackFileIO
-from boxjelly.ui.FileSelector import FileSelector
-
-
-class AbstractMediaSourceWidget(QtWidgets.QWidget):
-    """Abstract media source widget"""
-    
-    @property
-    def media_content(self) -> QtCore.QUrl:
-        raise NotImplementedError()
-
-
-class AbstractTrackSourceWidget(QtWidgets.QWidget):
-    """Abstract track source widget"""
-    
-    @property
-    def io(self) -> AbstractTrackFileIO:
-        raise NotImplementedError()
-
-
-class LocalVideoMediaSourceWidget(AbstractMediaSourceWidget):
-    """Video file media source widget. Loads local video files."""
-    def __init__(self, parent):
-        super().__init__(parent)
-    
-        self._filename = None
-        
-        self._selector = FileSelector(self, filter='Video files (*.mp4 *.mov *.wmv *.avi)')
-        self._selector.fileSelected.connect(self._update_filename)
-
-        self.arrange()
-    
-    def arrange(self):
-        """Arrange the widget"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        # Set zero margins
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        
-        # Arrange the file selector
-        self.layout().addWidget(self._selector)
-    
-    def _update_filename(self, filename):
-        self._filename = filename
-    
-    @property
-    def media_content(self) -> QtCore.QUrl:
-        return QtCore.QUrl.fromLocalFile(self._filename)
-
-
-class URLMediaSourceWidget(AbstractMediaSourceWidget):
-    """URL media source widget. Loads video files from URL."""
-    def __init__(self, parent):
-        super().__init__(parent)
-    
-        self._url = None
-        
-        self._line_edit = QtWidgets.QLineEdit()
-        self._line_edit.setPlaceholderText('URL')
-        self._line_edit.textChanged.connect(self._update_url)
-        
-        self.arrange()
-    
-    def arrange(self):
-        """Arrange the widget"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        # Set zero margins
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        
-        # Arrange the text input
-        self.layout().addWidget(self._line_edit)
-    
-    def _update_url(self, url):
-        self._url = url
-    
-    @property
-    def media_content(self) -> QtCore.QUrl:
-        return QtCore.QUrl(self._url)
-
-
-class YOLOv5DeepSortTrackSourceWidget(AbstractTrackSourceWidget):
-    """YOLOv5-DeepSort file track source widget. Loads tracks from a modified MOT text file."""
-    def __init__(self, parent):
-        super().__init__(parent)
-    
-        self._filename = None
-        
-        self._selector = FileSelector(self, filter='Text files (*.txt)')
-        self._selector.fileSelected.connect(self._update_filename)
-        
-        self.arrange()
-    
-    def arrange(self):
-        """Arrange the widget"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        # Set zero margins
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        
-        # Arrange the file selector
-        self.layout().addWidget(self._selector)
-    
-    def _update_filename(self, filename):
-        self._filename = filename
-    
-    @property
-    def io(self) -> YOLOv5DeepSortTrackFileIO:
-        return YOLOv5DeepSortTrackFileIO(self._filename)
-
-
-class DeepseaTrackSourceWidget(AbstractTrackSourceWidget):
-    """deepsea-track artifact track source widget. Loads tracks from a tar.gz artifact of track JSONs as output by deepsea-track."""
-    def __init__(self, parent):
-        super().__init__(parent)
-        
-        self._filename = None
-        
-        self._selector = FileSelector(self, filter='Tar.gz files (*.tar.gz)')
-        self._selector.fileSelected.connect(self._update_filename)
-        
-        self.arrange()
-        
-    def arrange(self):
-        """Arrange the widget"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        # Set zero margins
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        
-        # Arrange the file selector
-        self.layout().addWidget(self._selector)
-    
-    def _update_filename(self, filename):
-        self._filename = filename
-    
-    @property
-    def io(self) -> DeepseaTrackFileIO:
-        return DeepseaTrackFileIO(self._filename)
-
-
-class JSONTrackSourceWidget(AbstractTrackSourceWidget):
-    """JSON track source widget"""
-    def __init__(self, parent):
-        super().__init__(parent)
-        
-        self._filename = None
-        
-        self._selector = FileSelector(self, filter='JSON files (*.json)')
-        self._selector.fileSelected.connect(self._update_filename)
-        
-        self.arrange()
-        
-    def arrange(self):
-        """Arrange the widget"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        # Set zero margins
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        
-        # Arrange the file selector
-        self.layout().addWidget(self._selector)
-    
-    def _update_filename(self, filename):
-        self._filename = filename
-    
-    @property
-    def io(self) -> JSONTrackFileIO:
-        return JSONTrackFileIO(self._filename)
+from PyQt6 import QtWidgets, QtMultimedia, QtCore
+
+from boxjelly.lib.fileio import AbstractTrackFileIO, DeepseaTrackFileIO, JSONTrackFileIO, YOLOv5DeepSortTrackFileIO
+from boxjelly.ui.FileSelector import FileSelector
+
+
+class AbstractMediaSourceWidget(QtWidgets.QWidget):
+    """Abstract media source widget"""
+    
+    @property
+    def media_content(self) -> QtCore.QUrl:
+        raise NotImplementedError()
+
+
+class AbstractTrackSourceWidget(QtWidgets.QWidget):
+    """Abstract track source widget"""
+    
+    @property
+    def io(self) -> AbstractTrackFileIO:
+        raise NotImplementedError()
+
+
+class LocalVideoMediaSourceWidget(AbstractMediaSourceWidget):
+    """Video file media source widget. Loads local video files."""
+    def __init__(self, parent):
+        super().__init__(parent)
+    
+        self._filename = None
+        
+        self._selector = FileSelector(self, filter='Video files (*.mp4 *.mov *.wmv *.avi)')
+        self._selector.fileSelected.connect(self._update_filename)
+
+        self.arrange()
+    
+    def arrange(self):
+        """Arrange the widget"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        # Set zero margins
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        
+        # Arrange the file selector
+        self.layout().addWidget(self._selector)
+    
+    def _update_filename(self, filename):
+        self._filename = filename
+    
+    @property
+    def media_content(self) -> QtCore.QUrl:
+        return QtCore.QUrl.fromLocalFile(self._filename)
+
+
+class URLMediaSourceWidget(AbstractMediaSourceWidget):
+    """URL media source widget. Loads video files from URL."""
+    def __init__(self, parent):
+        super().__init__(parent)
+    
+        self._url = None
+        
+        self._line_edit = QtWidgets.QLineEdit()
+        self._line_edit.setPlaceholderText('URL')
+        self._line_edit.textChanged.connect(self._update_url)
+        
+        self.arrange()
+    
+    def arrange(self):
+        """Arrange the widget"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        # Set zero margins
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        
+        # Arrange the text input
+        self.layout().addWidget(self._line_edit)
+    
+    def _update_url(self, url):
+        self._url = url
+    
+    @property
+    def media_content(self) -> QtCore.QUrl:
+        return QtCore.QUrl(self._url)
+
+
+class YOLOv5DeepSortTrackSourceWidget(AbstractTrackSourceWidget):
+    """YOLOv5-DeepSort file track source widget. Loads tracks from a modified MOT text file."""
+    def __init__(self, parent):
+        super().__init__(parent)
+    
+        self._filename = None
+        
+        self._selector = FileSelector(self, filter='Text files (*.txt)')
+        self._selector.fileSelected.connect(self._update_filename)
+        
+        self.arrange()
+    
+    def arrange(self):
+        """Arrange the widget"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        # Set zero margins
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        
+        # Arrange the file selector
+        self.layout().addWidget(self._selector)
+    
+    def _update_filename(self, filename):
+        self._filename = filename
+    
+    @property
+    def io(self) -> YOLOv5DeepSortTrackFileIO:
+        return YOLOv5DeepSortTrackFileIO(self._filename)
+
+
+class DeepseaTrackSourceWidget(AbstractTrackSourceWidget):
+    """deepsea-track artifact track source widget. Loads tracks from a tar.gz artifact of track JSONs as output by deepsea-track."""
+    def __init__(self, parent):
+        super().__init__(parent)
+        
+        self._filename = None
+        
+        self._selector = FileSelector(self, filter='Tar.gz files (*.tar.gz)')
+        self._selector.fileSelected.connect(self._update_filename)
+        
+        self.arrange()
+        
+    def arrange(self):
+        """Arrange the widget"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        # Set zero margins
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        
+        # Arrange the file selector
+        self.layout().addWidget(self._selector)
+    
+    def _update_filename(self, filename):
+        self._filename = filename
+    
+    @property
+    def io(self) -> DeepseaTrackFileIO:
+        return DeepseaTrackFileIO(self._filename)
+
+
+class JSONTrackSourceWidget(AbstractTrackSourceWidget):
+    """JSON track source widget"""
+    def __init__(self, parent):
+        super().__init__(parent)
+        
+        self._filename = None
+        
+        self._selector = FileSelector(self, filter='JSON files (*.json)')
+        self._selector.fileSelected.connect(self._update_filename)
+        
+        self.arrange()
+        
+    def arrange(self):
+        """Arrange the widget"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        # Set zero margins
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        
+        # Arrange the file selector
+        self.layout().addWidget(self._selector)
+    
+    def _update_filename(self, filename):
+        self._filename = filename
+    
+    @property
+    def io(self) -> JSONTrackFileIO:
+        return JSONTrackFileIO(self._filename)
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/track/Timeline.py` & `boxjelly-0.3.3/boxjelly/ui/track/Timeline.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import math
-
-from PyQt6 import QtWidgets, QtCore, QtGui
-
-from boxjelly.lib.settings import SettingsManager
-
-
-class Timeline(QtWidgets.QWidget):
-    
-    frameChanged = QtCore.pyqtSignal(int)
-    frameStepChanged = QtCore.pyqtSignal(int)
-    frameScaleChanged = QtCore.pyqtSignal(float)
-    frameSelected = QtCore.pyqtSignal(int)
-    
-    def __init__(self, parent, frame_step: int, frame_scale: float = 1.0):
-        super().__init__(parent)
-        
-        self._background_brush = self.palette().window()
-        self._foreground_brush = self.palette().windowText()
-        
-        self._frame = 0
-        self._frame_step = frame_step
-        self._frame_scale = frame_scale
-        
-        self._settings = SettingsManager.get_instance()
-        
-        self.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Fixed)
-
-    def set_frame(self, frame: int):
-        """
-        Set the current frame to be displayed.
-        """
-        if frame != self._frame:
-            self.frameChanged.emit(frame)
-        self._frame = frame
-        self.update()
-    
-    def set_frame_step(self, frame_step: int):
-        """
-        Set the frame step.
-        """
-        if frame_step != self._frame_step:
-            self.frameStepChanged.emit(frame_step)
-        self._frame_step = frame_step
-        self.update()
-    
-    def set_frame_scale(self, frame_scale: float):
-        """
-        Set the frame scale.
-        """
-        if frame_scale != self._frame_scale:
-            self.frameScaleChanged.emit(frame_scale)
-        self._frame_scale = frame_scale
-        self.update()
-    
-    def map_frame_to_x(self, frame: int) -> int:
-        """
-        Map a frame to an x coordinate.
-        """
-        return int((frame - self._frame) * self._frame_scale)
-    
-    def map_x_to_frame(self, x: int) -> int:
-        """
-        Map an x coordinate to a frame.
-        """
-        return int(x / self._frame_scale + self._frame)
-    
-    def map_frame_to_elapsed_time_ms(self, frame: int) -> int:
-        """
-        Map a frame to an elapsed time in milliseconds.
-        """
-        frame_rate = self._settings.frame_rate.value
-        return round(frame * 1000 / frame_rate)
-
-    @property
-    def frame(self):
-        return self._frame
-    
-    @property
-    def frame_step(self):
-        return self._frame_step
-    
-    @property
-    def frame_scale(self):
-        return self._frame_scale
-    
-    @property
-    def max_frame(self) -> int:
-        return int(self._frame + self.width() / self._frame_scale)
-
-    def paintEvent(self, event: QtGui.QPaintEvent):
-        # Get the painter
-        painter = QtGui.QPainter(self)
-        
-        # Get the device size
-        width = painter.device().width()
-        height = painter.device().height()
-        
-        # Set pen to foreground
-        painter.setPen(self._foreground_brush.color())
-        
-        # Draw horizontal line at bottom
-        painter.drawLine(0, height - 1, width, height - 1)
-        
-        # Compute the multiples of the frame step in the range [frame, max_frame]
-        tick_frames = range(math.floor(self._frame / self._frame_step) * self._frame_step, self.max_frame + 1, self._frame_step)
-        
-        # Compute inter-tick distance and label modulus
-        inter_tick_distance = self._frame_scale * self._frame_step
-        label_modulus = max(1, 2**math.floor(math.log2(100 / inter_tick_distance)))
-        
-        # Draw vertical lines and labels at the tick frames
-        for tick_frame in tick_frames:
-            x = self.map_frame_to_x(tick_frame)
-            painter.drawLine(x, height - 1, x, height - height // 4)
-            if tick_frame // self._frame_step % label_modulus == 0:
-                tick_elaped_time_ms = self.map_frame_to_elapsed_time_ms(tick_frame)
-                timedelta_str = QtCore.QTime(0, 0, 0).addMSecs(tick_elaped_time_ms).toString('mm:ss')
-                painter.drawText(x + 5, height - 5, timedelta_str)
-    
-    def sizeHint(self):
-        return QtCore.QSize(100, 20)
-    
-    def mousePressEvent(self, event: QtGui.QMouseEvent):
-        if event.button() == QtCore.Qt.MouseButton.LeftButton:
-            self.frameSelected.emit(self.map_x_to_frame(event.pos().x()))
+import math
+
+from PyQt6 import QtWidgets, QtCore, QtGui
+
+from boxjelly.lib.settings import SettingsManager
+
+
+class Timeline(QtWidgets.QWidget):
+    
+    frameChanged = QtCore.pyqtSignal(int)
+    frameStepChanged = QtCore.pyqtSignal(int)
+    frameScaleChanged = QtCore.pyqtSignal(float)
+    frameSelected = QtCore.pyqtSignal(int)
+    
+    def __init__(self, parent, frame_step: int, frame_scale: float = 1.0):
+        super().__init__(parent)
+        
+        self._background_brush = self.palette().window()
+        self._foreground_brush = self.palette().windowText()
+        
+        self._frame = 0
+        self._frame_step = frame_step
+        self._frame_scale = frame_scale
+        
+        self._settings = SettingsManager.get_instance()
+        
+        self.setSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Fixed)
+
+    def set_frame(self, frame: int):
+        """
+        Set the current frame to be displayed.
+        """
+        if frame != self._frame:
+            self.frameChanged.emit(frame)
+        self._frame = frame
+        self.update()
+    
+    def set_frame_step(self, frame_step: int):
+        """
+        Set the frame step.
+        """
+        if frame_step != self._frame_step:
+            self.frameStepChanged.emit(frame_step)
+        self._frame_step = frame_step
+        self.update()
+    
+    def set_frame_scale(self, frame_scale: float):
+        """
+        Set the frame scale.
+        """
+        if frame_scale != self._frame_scale:
+            self.frameScaleChanged.emit(frame_scale)
+        self._frame_scale = frame_scale
+        self.update()
+    
+    def map_frame_to_x(self, frame: int) -> int:
+        """
+        Map a frame to an x coordinate.
+        """
+        return int((frame - self._frame) * self._frame_scale)
+    
+    def map_x_to_frame(self, x: int) -> int:
+        """
+        Map an x coordinate to a frame.
+        """
+        return int(x / self._frame_scale + self._frame)
+    
+    def map_frame_to_elapsed_time_ms(self, frame: int) -> int:
+        """
+        Map a frame to an elapsed time in milliseconds.
+        """
+        frame_rate = self._settings.frame_rate.value
+        return round(frame * 1000 / frame_rate)
+
+    @property
+    def frame(self):
+        return self._frame
+    
+    @property
+    def frame_step(self):
+        return self._frame_step
+    
+    @property
+    def frame_scale(self):
+        return self._frame_scale
+    
+    @property
+    def max_frame(self) -> int:
+        return int(self._frame + self.width() / self._frame_scale)
+
+    def paintEvent(self, event: QtGui.QPaintEvent):
+        # Get the painter
+        painter = QtGui.QPainter(self)
+        
+        # Get the device size
+        width = painter.device().width()
+        height = painter.device().height()
+        
+        # Set pen to foreground
+        painter.setPen(self._foreground_brush.color())
+        
+        # Draw horizontal line at bottom
+        painter.drawLine(0, height - 1, width, height - 1)
+        
+        # Compute the multiples of the frame step in the range [frame, max_frame]
+        tick_frames = range(math.floor(self._frame / self._frame_step) * self._frame_step, self.max_frame + 1, self._frame_step)
+        
+        # Compute inter-tick distance and label modulus
+        inter_tick_distance = self._frame_scale * self._frame_step
+        label_modulus = max(1, 2**math.floor(math.log2(100 / inter_tick_distance)))
+        
+        # Draw vertical lines and labels at the tick frames
+        for tick_frame in tick_frames:
+            x = self.map_frame_to_x(tick_frame)
+            painter.drawLine(x, height - 1, x, height - height // 4)
+            if tick_frame // self._frame_step % label_modulus == 0:
+                tick_elaped_time_ms = self.map_frame_to_elapsed_time_ms(tick_frame)
+                timedelta_str = QtCore.QTime(0, 0, 0).addMSecs(tick_elaped_time_ms).toString('mm:ss')
+                painter.drawText(x + 5, height - 5, timedelta_str)
+    
+    def sizeHint(self):
+        return QtCore.QSize(100, 20)
+    
+    def mousePressEvent(self, event: QtGui.QMouseEvent):
+        if event.button() == QtCore.Qt.MouseButton.LeftButton:
+            self.frameSelected.emit(self.map_x_to_frame(event.pos().x()))
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/track/TrackGraphicsView.py` & `boxjelly-0.3.3/boxjelly/ui/track/TrackGraphicsView.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-from PyQt6 import QtWidgets, QtGui, QtCore
-
-from boxjelly.models.TrackListModel import TrackListModel
-from boxjelly.ui.graphicsitems.TimelineTrack import TimelineTrack
-
-class TrackGraphicsView(QtWidgets.QGraphicsView):
-    
-    TRACK_HEIGHT = 30
-    
-    frameSelected = QtCore.pyqtSignal(int)
-    scaleChanged = QtCore.pyqtSignal(float, float)
-    
-    verticalScrollBarChanged = QtCore.pyqtSignal(int)
-    horizontalScrollBarChanged = QtCore.pyqtSignal(int)
-    frameScrolled = QtCore.pyqtSignal(int)
-    
-    def __init__(self, parent, track_model: TrackListModel, selection_model: QtCore.QItemSelectionModel):
-        super().__init__(parent)
-        
-        self._track_model = track_model
-        self._track_model.dataChanged.connect(self._on_track_model_data_changed)
-        self._track_model.modelReset.connect(self._on_track_model_reset)
-        self._track_model.rowsInserted.connect(self._on_track_model_rows_inserted)
-        self._track_model.rowsAboutToBeRemoved.connect(self._on_track_model_rows_about_to_be_removed)
-        self._track_model.rowsRemoved.connect(self._on_track_model_rows_removed)
-        self._track_model.layoutChanged.connect(self._on_track_model_layout_changed)
-        
-        self._selection_model = selection_model
-        
-        self._scene = QtWidgets.QGraphicsScene()
-        self.setScene(self._scene)
-        self.setViewportMargins(0, 0, 0, 0)
-        self.setFrameStyle(QtWidgets.QFrame.Shape.NoFrame)
-        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeft | QtCore.Qt.AlignmentFlag.AlignTop)
-        
-        self._background_rect = None  # backround rectangle
-        self._timeline_track_dict = {}  # track ID -> TimelineTrack graphics item
-        
-        self._current_frame = 0  # current frame that the playhead is on
-        self._frame_scale = 1.0  # horizontal scale of the timeline, in scene units per frame
-        
-        self.scaleChanged.connect(self._rescale)
-        
-        self.set_frame_scale(self._frame_scale)
-        
-        self.verticalScrollBar().valueChanged.connect(self.verticalScrollBarChanged.emit)
-        self.horizontalScrollBar().valueChanged.connect(self.horizontalScrollBarChanged.emit)
-        self.horizontalScrollBar().valueChanged.connect(lambda value: self.frameScrolled.emit(self._map_scene_to_frame(value)))
-    
-    def compute_frame_count(self):
-        if self._track_model.rowCount(None) == 0:
-            return 0
-    
-        end_frames = [self._track_model.data(self._track_model.index(row_idx, 0), TrackListModel.EndFrameRole) for row_idx in range(self._track_model.rowCount(None))]
-        return max(end_frames) + 1
-    
-    def is_loaded(self):
-        return self.compute_frame_count() > 0
-    
-    @QtCore.pyqtSlot(QtCore.QModelIndex, QtCore.QModelIndex)
-    def _on_track_model_data_changed(self, top_left: QtCore.QModelIndex, bottom_right: QtCore.QModelIndex):
-        """Handle track data changes."""
-        if not self.is_loaded():
-            return
-        
-        for row_idx in range(top_left.row(), bottom_right.row() + 1):
-            index = self._track_model.index(row_idx, 0)
-            track_id = self._track_model.data(index, TrackListModel.IDRole)
-            
-            timeline_track = self._timeline_track_dict[track_id]
-            timeline_track.update()
-    
-    @QtCore.pyqtSlot()
-    def _on_track_model_reset(self):
-        """When the track model is reset, reset the scene."""
-        self._reset_scene()
-    
-    @QtCore.pyqtSlot(QtCore.QModelIndex, int, int)
-    def _on_track_model_rows_inserted(self, parent, start, end):
-        """When tracks are added, add new timeline tracks."""
-        for row_idx in range(start, end + 1):
-            track = self._track_model.get_track(row_idx)
-            
-            timeline_track = TimelineTrack(track)
-            
-            timeline_track.setZValue(0)
-            timeline_track.set_scale(self._frame_scale, 1.0)
-            self.scaleChanged.connect(timeline_track.set_scale)
-            timeline_track.clicked.connect(self._on_timeline_track_clicked)
-            
-            self._scene.addItem(timeline_track)
-            self._timeline_track_dict[track.id] = timeline_track
-        
-        # Trigger a rescale
-        self._rescale(self._frame_scale, ...)
-    
-    @QtCore.pyqtSlot(object)
-    def _on_timeline_track_clicked(self, timeline_track: TimelineTrack):
-        """When timeline track is clicked, select it."""
-        model_index = self._track_model.index(self._track_model.index_by_id(timeline_track.track.id), 0)
-        self._selection_model.select(model_index, QtCore.QItemSelectionModel.SelectionFlag.ClearAndSelect)
-    
-    @QtCore.pyqtSlot('QList<QPersistentModelIndex>', QtCore.QAbstractItemModel.LayoutChangeHint)
-    def _on_track_model_layout_changed(self, removed_indexes, change_hint):
-        """When the track model layout changes, reposition the tracks."""
-        self._reposition_tracks()
-    
-    @QtCore.pyqtSlot(QtCore.QModelIndex, int, int)
-    def _on_track_model_rows_about_to_be_removed(self, parent, start, end):
-        """When tracks are removed, remove the corresponding timeline tracks."""
-        for row_idx in range(start, end + 1):
-            track = self._track_model.get_track(row_idx)
-            
-            timeline_track = self._timeline_track_dict[track.id]
-            
-            self._scene.removeItem(timeline_track)
-            del self._timeline_track_dict[track.id]
-    
-    @QtCore.pyqtSlot(QtCore.QModelIndex, int, int)
-    def _on_track_model_rows_removed(self, parent, start, end):
-        self._reposition_tracks()
-    
-    def _center_on_frame(self, frame: int):
-        self.horizontalScrollBar().setValue(self._map_frame_to_scene(frame) - self.width() / 2)
-    
-    def set_frame_scale(self, scale: float):
-        self._frame_scale = scale
-        self._center_on_frame(self._current_frame)
-        self.scaleChanged.emit(scale, 1.0)
-    
-    def _map_scene_to_frame(self, scene_x: float) -> int:
-        return int(scene_x / self._frame_scale)
-    
-    def _map_frame_to_scene(self, frame: int) -> float:
-        return frame * self._frame_scale
-    
-    @property
-    def scene_width(self) -> float:
-        if not self.is_loaded():
-            return 0.
-        
-        return self._map_frame_to_scene(self.compute_frame_count())
-
-    @property
-    def scene_height(self):
-        if not self.is_loaded():
-            return 0.
-        
-        return self.TRACK_HEIGHT * len(self._track_model)
-    
-    @QtCore.pyqtSlot(float, float)
-    def _rescale(self, new_frame_scale: float, _):
-        """
-        Rescale scene.
-        """
-        if not self.is_loaded():
-            return
-        
-        self._frame_scale = new_frame_scale
-        
-        self._reposition_tracks()
-        
-        self._scene.setSceneRect(0, 0, self.scene_width, self.TRACK_HEIGHT * self._track_model.rowCount(None))  # update scene size
-        
-        self._background_rect.setRect(0, 0, self._scene.width(), self._scene.height())  # rescale background rect
-    
-    def _clear_scene(self):
-        self._scene.clear()
-        
-        self._background_rect = None
-        self._timeline_track_dict = {}
-    
-    def _reset_scene(self):
-        self._clear_scene()
-        self._add_background()
-        self._reposition_tracks()
-        self.set_frame_scale(self._frame_scale)
-    
-    def _add_background(self):
-        """Add a background rectangle to the scene."""
-        self._background_rect = QtWidgets.QGraphicsRectItem(0, 0, self._scene.width(), self._scene.height())
-        self._background_rect.setBrush(QtGui.QColor(0, 0, 0, 0))
-        self._background_rect.setPen(QtGui.QPen(QtCore.Qt.PenStyle.NoPen))
-        self._background_rect.setZValue(-1)
-        
-        self._scene.addItem(self._background_rect)
-    
-    def _reposition_tracks(self):
-        """Reposition tracks."""
-        for row_idx in range(self._track_model.rowCount(None)):
-            index = self._track_model.index(row_idx, 0)
-            track_id = self._track_model.data(index, TrackListModel.IDRole)
-            
-            timeline_track = self._timeline_track_dict[track_id]
-            timeline_track.setPos(timeline_track.track.start_frame * self._frame_scale, row_idx * self.TRACK_HEIGHT)
-    
-    def show_frame(self, frame: int):
-        """Update the view to a specific frame, trying to center it in the viewport."""
-        if not self.is_loaded():
-            return
-        
-        self._current_frame = frame
-        
-        new_scrollbar_position = self._map_frame_to_scene(frame) - self.viewport().width() / 2
-        if new_scrollbar_position < 0:
-            new_scrollbar_position = 0
-        elif new_scrollbar_position > self.scene_width - self.viewport().width():
-            new_scrollbar_position = self.scene_width - self.viewport().width()
-        self.horizontalScrollBar().setValue(new_scrollbar_position)
-        
-        self.viewport().repaint()  # Trigger a repaint of the viewport.
-    
-    def paintEvent(self, event: QtGui.QPaintEvent):
-        super().paintEvent(event)
-        
-        if not self.is_loaded():
-            return
-        
-        # Draw a red line to mark the current frame.
-        painter = QtGui.QPainter(self.viewport())
-        scene_x = self._map_frame_to_scene(self._current_frame)
-        view_x = self.mapFromScene(scene_x, 0).x()
-        painter.setPen(QtGui.QPen(QtGui.QColor(255, 0, 0), 1))
-        painter.drawLine(view_x, 0, view_x, self._scene.height())
-    
-    def mousePressEvent(self, event: QtGui.QMouseEvent):
-        """Handle mouse press events."""
-        super().mousePressEvent(event)
-        
-        scene_pos = self.mapToScene(event.pos())
-        
-        if event.button() == QtCore.Qt.MouseButton.LeftButton:  # Left click
-            self.frameSelected.emit(self._map_scene_to_frame(scene_pos.x()))  # Emit the frame selected signal.
-    
-    def wheelEvent(self, event: QtGui.QWheelEvent):
-        """Handle mouse wheel events."""
-        
-        # If Ctrl+scroll, change the frame scale.
-        if event.modifiers() == QtCore.Qt.KeyboardModifier.ControlModifier:
-            if event.angleDelta().y() > 0:
-                self.set_frame_scale(round(self._frame_scale * 1.1, 2))
-            else:
-                self.set_frame_scale(round(self._frame_scale / 1.1, 2))
-            return
-        
-        # Otherwise, scroll the view.
-        super().wheelEvent(event)
+from PyQt6 import QtWidgets, QtGui, QtCore
+
+from boxjelly.models.TrackListModel import TrackListModel
+from boxjelly.ui.graphicsitems.TimelineTrack import TimelineTrack
+
+class TrackGraphicsView(QtWidgets.QGraphicsView):
+    
+    TRACK_HEIGHT = 30
+    
+    frameSelected = QtCore.pyqtSignal(int)
+    scaleChanged = QtCore.pyqtSignal(float, float)
+    
+    verticalScrollBarChanged = QtCore.pyqtSignal(int)
+    horizontalScrollBarChanged = QtCore.pyqtSignal(int)
+    frameScrolled = QtCore.pyqtSignal(int)
+    
+    def __init__(self, parent, track_model: TrackListModel, selection_model: QtCore.QItemSelectionModel):
+        super().__init__(parent)
+        
+        self._track_model = track_model
+        self._track_model.dataChanged.connect(self._on_track_model_data_changed)
+        self._track_model.modelReset.connect(self._on_track_model_reset)
+        self._track_model.rowsInserted.connect(self._on_track_model_rows_inserted)
+        self._track_model.rowsAboutToBeRemoved.connect(self._on_track_model_rows_about_to_be_removed)
+        self._track_model.rowsRemoved.connect(self._on_track_model_rows_removed)
+        self._track_model.layoutChanged.connect(self._on_track_model_layout_changed)
+        
+        self._selection_model = selection_model
+        
+        self._scene = QtWidgets.QGraphicsScene()
+        self.setScene(self._scene)
+        self.setViewportMargins(0, 0, 0, 0)
+        self.setFrameStyle(QtWidgets.QFrame.Shape.NoFrame)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeft | QtCore.Qt.AlignmentFlag.AlignTop)
+        
+        self._background_rect = None  # backround rectangle
+        self._timeline_track_dict = {}  # track ID -> TimelineTrack graphics item
+        
+        self._current_frame = 0  # current frame that the playhead is on
+        self._frame_scale = 1.0  # horizontal scale of the timeline, in scene units per frame
+        
+        self.scaleChanged.connect(self._rescale)
+        
+        self.set_frame_scale(self._frame_scale)
+        
+        self.verticalScrollBar().valueChanged.connect(self.verticalScrollBarChanged.emit)
+        self.horizontalScrollBar().valueChanged.connect(self.horizontalScrollBarChanged.emit)
+        self.horizontalScrollBar().valueChanged.connect(lambda value: self.frameScrolled.emit(self._map_scene_to_frame(value)))
+    
+    def compute_frame_count(self):
+        if self._track_model.rowCount(None) == 0:
+            return 0
+    
+        end_frames = [self._track_model.data(self._track_model.index(row_idx, 0), TrackListModel.EndFrameRole) for row_idx in range(self._track_model.rowCount(None))]
+        return max(end_frames) + 1
+    
+    def is_loaded(self):
+        return self.compute_frame_count() > 0
+    
+    @QtCore.pyqtSlot(QtCore.QModelIndex, QtCore.QModelIndex)
+    def _on_track_model_data_changed(self, top_left: QtCore.QModelIndex, bottom_right: QtCore.QModelIndex):
+        """Handle track data changes."""
+        if not self.is_loaded():
+            return
+        
+        for row_idx in range(top_left.row(), bottom_right.row() + 1):
+            index = self._track_model.index(row_idx, 0)
+            track_id = self._track_model.data(index, TrackListModel.IDRole)
+            
+            timeline_track = self._timeline_track_dict[track_id]
+            timeline_track.update()
+    
+    @QtCore.pyqtSlot()
+    def _on_track_model_reset(self):
+        """When the track model is reset, reset the scene."""
+        self._reset_scene()
+    
+    @QtCore.pyqtSlot(QtCore.QModelIndex, int, int)
+    def _on_track_model_rows_inserted(self, parent, start, end):
+        """When tracks are added, add new timeline tracks."""
+        for row_idx in range(start, end + 1):
+            track = self._track_model.get_track(row_idx)
+            
+            timeline_track = TimelineTrack(track)
+            
+            timeline_track.setZValue(0)
+            timeline_track.set_scale(self._frame_scale, 1.0)
+            self.scaleChanged.connect(timeline_track.set_scale)
+            timeline_track.clicked.connect(self._on_timeline_track_clicked)
+            
+            self._scene.addItem(timeline_track)
+            self._timeline_track_dict[track.id] = timeline_track
+        
+        # Trigger a rescale
+        self._rescale(self._frame_scale, ...)
+    
+    @QtCore.pyqtSlot(object)
+    def _on_timeline_track_clicked(self, timeline_track: TimelineTrack):
+        """When timeline track is clicked, select it."""
+        model_index = self._track_model.index(self._track_model.index_by_id(timeline_track.track.id), 0)
+        self._selection_model.select(model_index, QtCore.QItemSelectionModel.SelectionFlag.ClearAndSelect)
+    
+    @QtCore.pyqtSlot('QList<QPersistentModelIndex>', QtCore.QAbstractItemModel.LayoutChangeHint)
+    def _on_track_model_layout_changed(self, removed_indexes, change_hint):
+        """When the track model layout changes, reposition the tracks."""
+        self._reposition_tracks()
+    
+    @QtCore.pyqtSlot(QtCore.QModelIndex, int, int)
+    def _on_track_model_rows_about_to_be_removed(self, parent, start, end):
+        """When tracks are removed, remove the corresponding timeline tracks."""
+        for row_idx in range(start, end + 1):
+            track = self._track_model.get_track(row_idx)
+            
+            timeline_track = self._timeline_track_dict[track.id]
+            
+            self._scene.removeItem(timeline_track)
+            del self._timeline_track_dict[track.id]
+    
+    @QtCore.pyqtSlot(QtCore.QModelIndex, int, int)
+    def _on_track_model_rows_removed(self, parent, start, end):
+        self._reposition_tracks()
+    
+    def _center_on_frame(self, frame: int):
+        self.horizontalScrollBar().setValue(round(self._map_frame_to_scene(frame) - self.width() / 2))
+    
+    def set_frame_scale(self, scale: float):
+        self._frame_scale = scale
+        self._center_on_frame(self._current_frame)
+        self.scaleChanged.emit(scale, 1.0)
+    
+    def _map_scene_to_frame(self, scene_x: float) -> int:
+        return int(scene_x / self._frame_scale)
+    
+    def _map_frame_to_scene(self, frame: int) -> float:
+        return frame * self._frame_scale
+    
+    @property
+    def scene_width(self) -> float:
+        if not self.is_loaded():
+            return 0.
+        
+        return self._map_frame_to_scene(self.compute_frame_count())
+
+    @property
+    def scene_height(self):
+        if not self.is_loaded():
+            return 0.
+        
+        return self.TRACK_HEIGHT * len(self._track_model)
+    
+    @QtCore.pyqtSlot(float, float)
+    def _rescale(self, new_frame_scale: float, _):
+        """
+        Rescale scene.
+        """
+        if not self.is_loaded():
+            return
+        
+        self._frame_scale = new_frame_scale
+        
+        self._reposition_tracks()
+        
+        self._scene.setSceneRect(0, 0, self.scene_width, self.TRACK_HEIGHT * self._track_model.rowCount(None))  # update scene size
+        
+        self._background_rect.setRect(0, 0, self._scene.width(), self._scene.height())  # rescale background rect
+    
+    def _clear_scene(self):
+        self._scene.clear()
+        
+        self._background_rect = None
+        self._timeline_track_dict = {}
+    
+    def _reset_scene(self):
+        self._clear_scene()
+        self._add_background()
+        self._reposition_tracks()
+        self.set_frame_scale(self._frame_scale)
+    
+    def _add_background(self):
+        """Add a background rectangle to the scene."""
+        self._background_rect = QtWidgets.QGraphicsRectItem(0, 0, self._scene.width(), self._scene.height())
+        self._background_rect.setBrush(QtGui.QColor(0, 0, 0, 0))
+        self._background_rect.setPen(QtGui.QPen(QtCore.Qt.PenStyle.NoPen))
+        self._background_rect.setZValue(-1)
+        
+        self._scene.addItem(self._background_rect)
+    
+    def _reposition_tracks(self):
+        """Reposition tracks."""
+        for row_idx in range(self._track_model.rowCount(None)):
+            index = self._track_model.index(row_idx, 0)
+            track_id = self._track_model.data(index, TrackListModel.IDRole)
+            
+            timeline_track = self._timeline_track_dict[track_id]
+            timeline_track.setPos(timeline_track.track.start_frame * self._frame_scale, row_idx * self.TRACK_HEIGHT)
+    
+    def show_frame(self, frame: int):
+        """Update the view to a specific frame, trying to center it in the viewport."""
+        if not self.is_loaded():
+            return
+        
+        self._current_frame = frame
+        
+        new_scrollbar_position = self._map_frame_to_scene(frame) - self.viewport().width() / 2
+        if new_scrollbar_position < 0:
+            new_scrollbar_position = 0
+        elif new_scrollbar_position > self.scene_width - self.viewport().width():
+            new_scrollbar_position = self.scene_width - self.viewport().width()
+        self.horizontalScrollBar().setValue(round(new_scrollbar_position))
+        
+        self.viewport().repaint()  # Trigger a repaint of the viewport.
+    
+    def paintEvent(self, event: QtGui.QPaintEvent):
+        super().paintEvent(event)
+        
+        if not self.is_loaded():
+            return
+        
+        # Draw a red line to mark the current frame.
+        painter = QtGui.QPainter(self.viewport())
+        scene_x = self._map_frame_to_scene(self._current_frame)
+        view_x = self.mapFromScene(scene_x, 0).x()
+        painter.setPen(QtGui.QPen(QtGui.QColor(255, 0, 0), 1))
+        painter.drawLine(view_x, 0, view_x, round(self._scene.height()))
+    
+    def mousePressEvent(self, event: QtGui.QMouseEvent):
+        """Handle mouse press events."""
+        super().mousePressEvent(event)
+        
+        scene_pos = self.mapToScene(event.pos())
+        
+        if event.button() == QtCore.Qt.MouseButton.LeftButton:  # Left click
+            self.frameSelected.emit(self._map_scene_to_frame(scene_pos.x()))  # Emit the frame selected signal.
+    
+    def wheelEvent(self, event: QtGui.QWheelEvent):
+        """Handle mouse wheel events."""
+        
+        # If Ctrl+scroll, change the frame scale.
+        if event.modifiers() == QtCore.Qt.KeyboardModifier.ControlModifier:
+            if event.angleDelta().y() > 0:
+                self.set_frame_scale(round(self._frame_scale * 1.1, 2))
+            else:
+                self.set_frame_scale(round(self._frame_scale / 1.1, 2))
+            return
+        
+        # Otherwise, scroll the view.
+        super().wheelEvent(event)
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/track/TrackHeadersView.py` & `boxjelly-0.3.3/boxjelly/ui/track/TrackHeadersView.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from PyQt6 import QtWidgets, QtCore, QtGui
-
-from boxjelly.delegates.TrackHeadersDelegate import TrackHeadersDelegate
-
-
-class TrackHeadersView(QtWidgets.QListView):
-    def __init__(self, parent):
-        super().__init__(parent)
-        
-        self.setSelectionMode(QtWidgets.QAbstractItemView.SelectionMode.ExtendedSelection)
-        self.setItemDelegate(TrackHeadersDelegate(self))
-        self.viewport().setMouseTracking(True)
-        
-        self.setFrameStyle(QtWidgets.QFrame.Shape.NoFrame)
-        
-        self.setVerticalScrollMode(QtWidgets.QAbstractItemView.ScrollMode.ScrollPerPixel)
-        self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
-    
-    def set_vertical_scroll(self, value: int):
-        self.verticalScrollBar().setValue(value)
-    
-    def wheelEvent(self, e: QtGui.QWheelEvent):
+from PyQt6 import QtWidgets, QtCore, QtGui
+
+from boxjelly.delegates.TrackHeadersDelegate import TrackHeadersDelegate
+
+
+class TrackHeadersView(QtWidgets.QListView):
+    def __init__(self, parent):
+        super().__init__(parent)
+        
+        self.setSelectionMode(QtWidgets.QAbstractItemView.SelectionMode.ExtendedSelection)
+        self.setItemDelegate(TrackHeadersDelegate(self))
+        self.viewport().setMouseTracking(True)
+        
+        self.setFrameStyle(QtWidgets.QFrame.Shape.NoFrame)
+        
+        self.setVerticalScrollMode(QtWidgets.QAbstractItemView.ScrollMode.ScrollPerPixel)
+        self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+    
+    def set_vertical_scroll(self, value: int):
+        self.verticalScrollBar().setValue(value)
+    
+    def wheelEvent(self, e: QtGui.QWheelEvent):
         pass
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/track/TrackPanel.py` & `boxjelly-0.3.3/boxjelly/ui/track/TrackPanel.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from PyQt6 import QtWidgets, QtCore
-
-from boxjelly.ui.track.Timeline import Timeline
-from boxjelly.ui.track.TrackHeadersView import TrackHeadersView
-from boxjelly.ui.track.TrackGraphicsView import TrackGraphicsView
-from boxjelly.models.TrackListModel import TrackListModel
-
-
-class TrackPanel(QtWidgets.QWidget):
-    """Track panel widget"""
-    
-    frameSelected = QtCore.pyqtSignal(int)
-    
-    def __init__(self, parent, track_model: TrackListModel, selection_model: QtCore.QItemSelectionModel):
-        super().__init__(parent)
-        
-        self._track_model = track_model
-        self._selection_model = selection_model
-        
-        # Set minimum size
-        self.setMinimumSize(800, 0)
-        
-        # Set default size
-        self.setGeometry(0, 0, 800, 100)
-        
-        # Create timeline
-        self.timeline = Timeline(self, 300)
-        
-        # Create track view
-        self.track_view = TrackGraphicsView(self, self._track_model, self._selection_model)
-        
-        # Create track headers view
-        self.track_headers_view = TrackHeadersView(self)
-        self.track_headers_view.setModel(self._track_model)
-        self.track_headers_view.setSelectionModel(self._selection_model)
-        
-        # Connect signals and slots
-        self.track_view.frameScrolled.connect(self.timeline.set_frame)
-        self.track_view.verticalScrollBarChanged.connect(self.track_headers_view.set_vertical_scroll)
-        self.track_view.scaleChanged.connect(lambda x_scale, y_scale: self.timeline.set_frame_scale(x_scale))
-        self.timeline.frameSelected.connect(self.frameSelected.emit)
-        
-        self.arrange()
-    
-    def arrange(self):
-        """Arrange the track panel"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QGridLayout())
-        
-        # Arrange timeline
-        self.layout().addWidget(self.timeline, 0, 1, 1, 1)
-        
-        # Arrange track headers list view
-        self.layout().addWidget(self.track_headers_view, 1, 0, 1, 1)
-        
-        # Arrange track view
-        self.layout().addWidget(self.track_view, 1, 1, 1, 1)
-        
-        self.layout().setRowStretch(0, 0)
-        self.layout().setRowStretch(1, 1)
-        self.layout().setColumnStretch(0, 0)
-        self.layout().setColumnStretch(1, 1)
-    
-    def show_frame(self, frame: int):
-        """Show data corresponding to a particular frame number"""
-        self.track_view.show_frame(frame)
+from PyQt6 import QtWidgets, QtCore
+
+from boxjelly.ui.track.Timeline import Timeline
+from boxjelly.ui.track.TrackHeadersView import TrackHeadersView
+from boxjelly.ui.track.TrackGraphicsView import TrackGraphicsView
+from boxjelly.models.TrackListModel import TrackListModel
+
+
+class TrackPanel(QtWidgets.QWidget):
+    """Track panel widget"""
+    
+    frameSelected = QtCore.pyqtSignal(int)
+    
+    def __init__(self, parent, track_model: TrackListModel, selection_model: QtCore.QItemSelectionModel):
+        super().__init__(parent)
+        
+        self._track_model = track_model
+        self._selection_model = selection_model
+        
+        # Set minimum size
+        self.setMinimumSize(800, 0)
+        
+        # Set default size
+        self.setGeometry(0, 0, 800, 100)
+        
+        # Create timeline
+        self.timeline = Timeline(self, 300)
+        
+        # Create track view
+        self.track_view = TrackGraphicsView(self, self._track_model, self._selection_model)
+        
+        # Create track headers view
+        self.track_headers_view = TrackHeadersView(self)
+        self.track_headers_view.setModel(self._track_model)
+        self.track_headers_view.setSelectionModel(self._selection_model)
+        
+        # Connect signals and slots
+        self.track_view.frameScrolled.connect(self.timeline.set_frame)
+        self.track_view.verticalScrollBarChanged.connect(self.track_headers_view.set_vertical_scroll)
+        self.track_view.scaleChanged.connect(lambda x_scale, y_scale: self.timeline.set_frame_scale(x_scale))
+        self.timeline.frameSelected.connect(self.frameSelected.emit)
+        
+        self.arrange()
+    
+    def arrange(self):
+        """Arrange the track panel"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QGridLayout())
+        
+        # Arrange timeline
+        self.layout().addWidget(self.timeline, 0, 1, 1, 1)
+        
+        # Arrange track headers list view
+        self.layout().addWidget(self.track_headers_view, 1, 0, 1, 1)
+        
+        # Arrange track view
+        self.layout().addWidget(self.track_view, 1, 1, 1, 1)
+        
+        self.layout().setRowStretch(0, 0)
+        self.layout().setRowStretch(1, 1)
+        self.layout().setColumnStretch(0, 0)
+        self.layout().setColumnStretch(1, 1)
+    
+    def show_frame(self, frame: int):
+        """Show data corresponding to a particular frame number"""
+        self.track_view.show_frame(frame)
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/TrackSelectionBox.py` & `boxjelly-0.3.3/boxjelly/ui/TrackSelectionBox.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from PyQt6 import QtWidgets
-
-from boxjelly.ui.WidgetComboBox import WidgetComboBox
-from boxjelly.ui.SourceWidgets import DeepseaTrackSourceWidget, YOLOv5DeepSortTrackSourceWidget, JSONTrackSourceWidget
-from boxjelly.lib.fileio import AbstractTrackFileIO
-
-
-class TrackSelectionBox(QtWidgets.QGroupBox):
-    """Track selection group box"""
-    
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        
-        self.setTitle('Tracks')
-        
-        self.widget_combo_box = WidgetComboBox(self)
-        self.widget_combo_box.add_widget(YOLOv5DeepSortTrackSourceWidget(self), 'YOLOv5-DeepSort')
-        self.widget_combo_box.add_widget(DeepseaTrackSourceWidget(self), 'deepsea-track')
-        self.widget_combo_box.add_widget(JSONTrackSourceWidget(self), 'JSON')
-        self.widget_combo_box.refresh()
-        
-        self.arrange()
-    
-    def arrange(self):
-        """Arrange the widget"""
-        # Set vertical layout
-        self.setLayout(QtWidgets.QVBoxLayout())
-        
-        # Add widget combo box
-        self.layout().addWidget(self.widget_combo_box)
-        
-        # Add stretch
-        self.layout().addStretch()
-    
-    @property
-    def io(self) -> AbstractTrackFileIO:
+from PyQt6 import QtWidgets
+
+from boxjelly.ui.WidgetComboBox import WidgetComboBox
+from boxjelly.ui.SourceWidgets import DeepseaTrackSourceWidget, YOLOv5DeepSortTrackSourceWidget, JSONTrackSourceWidget
+from boxjelly.lib.fileio import AbstractTrackFileIO
+
+
+class TrackSelectionBox(QtWidgets.QGroupBox):
+    """Track selection group box"""
+    
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        
+        self.setTitle('Tracks')
+        
+        self.widget_combo_box = WidgetComboBox(self)
+        self.widget_combo_box.add_widget(YOLOv5DeepSortTrackSourceWidget(self), 'YOLOv5-DeepSort')
+        self.widget_combo_box.add_widget(DeepseaTrackSourceWidget(self), 'deepsea-track')
+        self.widget_combo_box.add_widget(JSONTrackSourceWidget(self), 'JSON')
+        self.widget_combo_box.refresh()
+        
+        self.arrange()
+    
+    def arrange(self):
+        """Arrange the widget"""
+        # Set vertical layout
+        self.setLayout(QtWidgets.QVBoxLayout())
+        
+        # Add widget combo box
+        self.layout().addWidget(self.widget_combo_box)
+        
+        # Add stretch
+        self.layout().addStretch()
+    
+    @property
+    def io(self) -> AbstractTrackFileIO:
         return self.widget_combo_box.widget.io
```

### Comparing `boxjelly-0.3.2/boxjelly/ui/video/CthulhuVideoController.py` & `boxjelly-0.3.3/boxjelly/ui/video/CthulhuVideoController.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-from socket import socket, AF_INET, SOCK_DGRAM, timeout
-from typing import Optional
-from uuid import uuid4
-
-from sharktopoda_client.model.GenericCommand import GenericCommand
-from sharktopoda_client.model.GenericResponse import GenericResponse
-from PyQt6 import QtMultimedia, QtCore
-from boxjelly.lib.constants import CONTROL_HOST
-from boxjelly.lib.settings import SettingsManager
-
-from boxjelly.models.TrackListModel import TrackListModel
-
-
-class CthulhuVideoController(QtCore.QObject):
-    """
-    Cthulhu video controller. Redirects calls to Cthulhu UDP commands/responses.
-    """
-    
-    SOCKET_TIMEOUT = 500  # UDP response timeout, in milliseconds
-    FRAME_UPDATE_INTERVAL = 100  # frame update interval, in milliseconds
-    
-    mediaSetStatus = QtCore.pyqtSignal(bool)
-    positionChanged = QtCore.pyqtSignal(int)
-    frameUpdated = QtCore.pyqtSignal(int)
-    
-    def __init__(self, parent, track_model: TrackListModel, selection_model: QtCore.QItemSelectionModel):
-        super().__init__(parent)
-        
-        self._track_model = track_model
-        self._selection_model = selection_model
-        
-        self._udp_socket = socket(AF_INET, SOCK_DGRAM)
-        self._udp_socket.settimeout(CthulhuVideoController.SOCKET_TIMEOUT / 1e3)
-        
-        self._url = None
-        self._uuid = None
-        
-        self._dummy_player = QtMultimedia.QMediaPlayer(self)
-        
-        self._last_frame_number = None
-        
-        self._settings = SettingsManager.get_instance()
-        
-        # Start polling to update the current frame every FRAME_UPDATE_INTERVAL milliseconds
-        self.frame_update_timer = QtCore.QTimer(self)
-        self.frame_update_timer.timeout.connect(self._do_frame_update)
-        self.frame_update_timer.start(CthulhuVideoController.FRAME_UPDATE_INTERVAL)
-    
-    def send(self, command: GenericCommand) -> None:
-        try:
-            self._udp_socket.sendto(command.to_json().encode('utf-8'), (CONTROL_HOST, self._settings.control_port.value))
-        except OSError as e:
-            print(f'Error ({e}) while sending command to Cthulhu:\n{command.to_json(indent=2)}')  # TODO: Log
-    
-    def send_and_wait(self, command: GenericCommand) -> Optional[GenericResponse]:
-        # Send the command
-        self.send(command)
-        
-        # Wait for a response
-        try:
-            response_raw = self._udp_socket.recv(4096)
-            return GenericResponse.from_json(response_raw.decode('utf-8'))
-        except timeout:
-            # print(f'Timeout while waiting for response to command:\n{command.to_json(indent=2)}')  # TODO: Log
-            return None
-        except ConnectionResetError:
-            return None
-    
-    def set_media(self, media: QtCore.QUrl):
-        self._url = media.url()
-        self._uuid = str(uuid4())
-        
-        # Update track model video data
-        self._track_model.set_video_reference_uuid(self._uuid)
-        self._track_model.set_frame_rate(self._settings.frame_rate.value)
-        
-        success = self.open(self._url, self._uuid)
-        if success:
-            self.pause()
-        
-        self.mediaSetStatus.emit(success)
-    
-    def open(self, url: str, uuid: str):
-        """
-        Open a video file by URL and assign it a given UUID.
-        """
-        open_video_command = GenericCommand(command='open', url=url, uuid=uuid)
-        res = self.send_and_wait(open_video_command)
-        
-        return res is not None
-    
-    def play(self):
-        """
-        Play (resume) the current video.
-        """
-        play_command = GenericCommand(command='play', uuid=self._uuid)
-        self.send_and_wait(play_command)
-    
-    def pause(self):
-        """
-        Pause the current video.
-        """
-        pause_command = GenericCommand(command='pause', uuid=self._uuid)
-        self.send_and_wait(pause_command)
-    
-    def stop(self):
-        """
-        Stop the current video (pause and seek to beginning).
-        """
-        self.pause()
-        
-        seek_beginning_command = GenericCommand(command='seek elapsed time', uuid=self._uuid, elapsedTime=0)
-        self.send(seek_beginning_command)
-    
-    def set_frame(self, frame: int):
-        """
-        Seek the current video to a given frame.
-        """
-        seek_command = GenericCommand(command='seek elapsed time', uuid=self._uuid, elapsedTime=self._track_model.frame_to_ms(frame))
-        self.send(seek_command)
-    
-    def get_elapsed_time(self):
-        """
-        Get the current elapsed time in milliseconds of the current video.
-        """
-        elapsed_time_command = GenericCommand(command='request elapsed time', uuid=self._uuid)
-        res = self.send_and_wait(elapsed_time_command)
-        
-        if not res:
-            return
-        
-        return res.elapsedTime
-    
-    def get_frame_number(self) -> Optional[int]:
-        """
-        Get the current frame number of the current video.
-        """
-        if not (self._url and self._uuid):
-            return
-        
-        elapsed_time = self.get_elapsed_time()
-        if not elapsed_time:
-            return
-        
-        return self._track_model.ms_to_frame(elapsed_time)
-    
-    def try_close(self):
-        """
-        Try to close the current video.
-        """
-        if not (self._url and self._uuid):
-            return
-
-        close_command = GenericCommand(command='close', uuid=self._uuid)
-        self.send_and_wait(close_command)
-    
-    @QtCore.pyqtSlot()
-    def _do_frame_update(self):
-        """
-        Slot for frame update timer. Updates the current frame.
-        """
-        frame_number = self.get_frame_number()
-        if frame_number is not None and (self._last_frame_number is None or frame_number != self._last_frame_number):
-            self.frameUpdated.emit(frame_number)
-            self._track_model.load_at_frame(frame_number)
-            self._last_frame_number = frame_number
+from socket import socket, AF_INET, SOCK_DGRAM, timeout
+from typing import Optional
+from uuid import uuid4
+
+from sharktopoda_client.model.GenericCommand import GenericCommand
+from sharktopoda_client.model.GenericResponse import GenericResponse
+from PyQt6 import QtMultimedia, QtCore
+from boxjelly.lib.constants import CONTROL_HOST
+from boxjelly.lib.settings import SettingsManager
+
+from boxjelly.models.TrackListModel import TrackListModel
+
+
+class CthulhuVideoController(QtCore.QObject):
+    """
+    Cthulhu video controller. Redirects calls to Cthulhu UDP commands/responses.
+    """
+    
+    SOCKET_TIMEOUT = 500  # UDP response timeout, in milliseconds
+    FRAME_UPDATE_INTERVAL = 100  # frame update interval, in milliseconds
+    
+    mediaSetStatus = QtCore.pyqtSignal(bool)
+    positionChanged = QtCore.pyqtSignal(int)
+    frameUpdated = QtCore.pyqtSignal(int)
+    
+    def __init__(self, parent, track_model: TrackListModel, selection_model: QtCore.QItemSelectionModel):
+        super().__init__(parent)
+        
+        self._track_model = track_model
+        self._selection_model = selection_model
+        
+        self._udp_socket = socket(AF_INET, SOCK_DGRAM)
+        self._udp_socket.settimeout(CthulhuVideoController.SOCKET_TIMEOUT / 1e3)
+        
+        self._url = None
+        self._uuid = None
+        
+        self._dummy_player = QtMultimedia.QMediaPlayer(self)
+        
+        self._last_frame_number = None
+        
+        self._settings = SettingsManager.get_instance()
+        
+        # Start polling to update the current frame every FRAME_UPDATE_INTERVAL milliseconds
+        self.frame_update_timer = QtCore.QTimer(self)
+        self.frame_update_timer.timeout.connect(self._do_frame_update)
+        self.frame_update_timer.start(CthulhuVideoController.FRAME_UPDATE_INTERVAL)
+    
+    def send(self, command: GenericCommand) -> None:
+        try:
+            self._udp_socket.sendto(command.to_json().encode('utf-8'), (CONTROL_HOST, self._settings.control_port.value))
+        except OSError as e:
+            print(f'Error ({e}) while sending command to Cthulhu:\n{command.to_json(indent=2)}')  # TODO: Log
+    
+    def send_and_wait(self, command: GenericCommand) -> Optional[GenericResponse]:
+        # Send the command
+        self.send(command)
+        
+        # Wait for a response
+        try:
+            response_raw = self._udp_socket.recv(4096)
+            return GenericResponse.from_json(response_raw.decode('utf-8'))
+        except timeout:
+            # print(f'Timeout while waiting for response to command:\n{command.to_json(indent=2)}')  # TODO: Log
+            return None
+        except ConnectionResetError:
+            return None
+    
+    def set_media(self, media: QtCore.QUrl):
+        self._url = media.url()
+        self._uuid = str(uuid4())
+        
+        # Update track model video data
+        self._track_model.set_video_reference_uuid(self._uuid)
+        self._track_model.set_frame_rate(self._settings.frame_rate.value)
+        
+        success = self.open(self._url, self._uuid)
+        if success:
+            self.pause()
+        
+        self.mediaSetStatus.emit(success)
+    
+    def open(self, url: str, uuid: str):
+        """
+        Open a video file by URL and assign it a given UUID.
+        """
+        open_video_command = GenericCommand(command='open', url=url, uuid=uuid)
+        res = self.send_and_wait(open_video_command)
+        
+        return res is not None
+    
+    def play(self):
+        """
+        Play (resume) the current video.
+        """
+        play_command = GenericCommand(command='play', uuid=self._uuid)
+        self.send_and_wait(play_command)
+    
+    def pause(self):
+        """
+        Pause the current video.
+        """
+        pause_command = GenericCommand(command='pause', uuid=self._uuid)
+        self.send_and_wait(pause_command)
+    
+    def stop(self):
+        """
+        Stop the current video (pause and seek to beginning).
+        """
+        self.pause()
+        
+        seek_beginning_command = GenericCommand(command='seek elapsed time', uuid=self._uuid, elapsedTime=0)
+        self.send(seek_beginning_command)
+    
+    def set_frame(self, frame: int):
+        """
+        Seek the current video to a given frame.
+        """
+        seek_command = GenericCommand(command='seek elapsed time', uuid=self._uuid, elapsedTime=self._track_model.frame_to_ms(frame))
+        self.send(seek_command)
+    
+    def get_elapsed_time(self):
+        """
+        Get the current elapsed time in milliseconds of the current video.
+        """
+        elapsed_time_command = GenericCommand(command='request elapsed time', uuid=self._uuid)
+        res = self.send_and_wait(elapsed_time_command)
+        
+        if not res:
+            return
+        
+        return res.elapsedTime
+    
+    def get_frame_number(self) -> Optional[int]:
+        """
+        Get the current frame number of the current video.
+        """
+        if not (self._url and self._uuid):
+            return
+        
+        elapsed_time = self.get_elapsed_time()
+        if not elapsed_time:
+            return
+        
+        return self._track_model.ms_to_frame(elapsed_time)
+    
+    def try_close(self):
+        """
+        Try to close the current video.
+        """
+        if not (self._url and self._uuid):
+            return
+
+        close_command = GenericCommand(command='close', uuid=self._uuid)
+        self.send_and_wait(close_command)
+    
+    @QtCore.pyqtSlot()
+    def _do_frame_update(self):
+        """
+        Slot for frame update timer. Updates the current frame.
+        """
+        frame_number = self.get_frame_number()
+        if frame_number is not None and (self._last_frame_number is None or frame_number != self._last_frame_number):
+            self.frameUpdated.emit(frame_number)
+            self._track_model.load_at_frame(frame_number)
+            self._last_frame_number = frame_number
```

### Comparing `boxjelly-0.3.2/LICENSE` & `boxjelly-0.3.3/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 Monterey Bay Aquarium Research Institute
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2022 Monterey Bay Aquarium Research Institute
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `boxjelly-0.3.2/pyproject.toml` & `boxjelly-0.3.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[tool.poetry]
-name = "boxjelly"
-version = "0.3.2"
-description = "BoxJelly is a tool for viewing and editing object tracks in video."
-authors = ["Kevin Barnard <kbarnard@mbari.org>"]
-readme = "README.md"
-license = "MIT"
-
-[tool.poetry.scripts]
-boxjelly = "boxjelly.scripts.run:main"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-intervaltree = "^3.1.0"
-sharktopoda-client = "^0.1.4"
-dataclasses-json = "^0.5.7"
-PyQt6 = "^6.3.1"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "boxjelly"
+version = "0.3.3"
+description = "BoxJelly is a tool for viewing and editing object tracks in video."
+authors = ["Kevin Barnard <kbarnard@mbari.org>"]
+readme = "README.md"
+license = "MIT"
+
+[tool.poetry.scripts]
+boxjelly = "boxjelly.scripts.run:main"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+intervaltree = "^3.1.0"
+sharktopoda-client = "^0.1.4"
+dataclasses-json = "^0.5.7"
+PyQt6 = "^6.3.1"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `boxjelly-0.3.2/README.md` & `boxjelly-0.3.3/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-![BoxJelly logo](boxjelly/assets/images/boxjelly_logo_128.png)
-
-# BoxJelly
-
-**BoxJelly** is a tool for viewing and editing object tracks in video.
-
-[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![Python](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/downloads/)
-
-Author: Kevin Barnard, [kbarnard@mbari.org](mailto:kbarnard@mbari.org)
-
----
-
-## Install
-
-### From PyPI
-
-BoxJelly is available on PyPI as `boxjelly`. To install, run:
-
-```bash
-pip install boxjelly
-```
-
-### From source
-
-This project is build with Poetry. To install from source, run (in the project root):
-
-```bash
-poetry install
-```
-
-## Run
-
-Once BoxJelly is installed, you can run it from the command line:
-
-```bash
-boxjelly
-```
-
-**You must have Cthulhu installed and running before you can use BoxJelly.**
-
-## Documentation
-
-Official documentation is available at [docs.mbari.org/boxjelly](https://docs.mbari.org/boxjelly/).
-Alternatively, you can build the documentation from source with `mkdocs build`.
-
-## Credits
-
-Icons from [icons8.com](https://icons8.com/).
-
----
-
-Copyright &copy; 2021&ndash;2022 [Monterey Bay Aquarium Research Institute](https://www.mbari.org)
+![BoxJelly logo](boxjelly/assets/images/boxjelly_logo_128.png)
+
+# BoxJelly
+
+**BoxJelly** is a tool for viewing and editing object tracks in video.
+
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![Python](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/downloads/)
+
+Author: Kevin Barnard, [kbarnard@mbari.org](mailto:kbarnard@mbari.org)
+
+---
+
+## Install
+
+### From PyPI
+
+BoxJelly is available on PyPI as `boxjelly`. To install, run:
+
+```bash
+pip install boxjelly
+```
+
+### From source
+
+This project is build with Poetry. To install from source, run (in the project root):
+
+```bash
+poetry install
+```
+
+## Run
+
+Once BoxJelly is installed, you can run it from the command line:
+
+```bash
+boxjelly
+```
+
+**You must have Cthulhu installed and running before you can use BoxJelly.**
+
+## Documentation
+
+Official documentation is available at [docs.mbari.org/boxjelly](https://docs.mbari.org/boxjelly/).
+Alternatively, you can build the documentation from source with `mkdocs build`.
+
+## Credits
+
+Icons from [icons8.com](https://icons8.com/).
+
+---
+
+Copyright &copy; 2021&ndash;2022 [Monterey Bay Aquarium Research Institute](https://www.mbari.org)
```

### Comparing `boxjelly-0.3.2/PKG-INFO` & `boxjelly-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: boxjelly
-Version: 0.3.2
+Version: 0.3.3
 Summary: BoxJelly is a tool for viewing and editing object tracks in video.
 License: MIT
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyQt6 (>=6.3.1,<7.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: intervaltree (>=3.1.0,<4.0.0)
 Requires-Dist: sharktopoda-client (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 ![BoxJelly logo](boxjelly/assets/images/boxjelly_logo_128.png)
```

