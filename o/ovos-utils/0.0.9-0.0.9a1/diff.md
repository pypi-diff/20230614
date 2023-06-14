# Comparing `tmp/ovos_utils-0.0.9.tar.gz` & `tmp/ovos_utils-0.0.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ovos_utils-0.0.9.tar", last modified: Sun May 16 21:24:46 2021, max compression
+gzip compressed data, was "dist/ovos_utils-0.0.9a1.tar", last modified: Sun Apr  4 11:00:19 2021, max compression
```

## Comparing `ovos_utils-0.0.9.tar` & `ovos_utils-0.0.9a1.tar`

### file list

```diff
@@ -1,66 +1,136 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/
--rw-rw-r--   0 user      (1000) user      (1000)       35 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)      316 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.541195 ovos_utils-0.0.9/ovos_utils/
--rw-rw-r--   0 user      (1000) user      (1000)     6672 2021-05-09 22:57:29.000000 ovos_utils-0.0.9/ovos_utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     7215 2020-12-20 16:25:19.000000 ovos_utils-0.0.9/ovos_utils/colors.py
--rw-rw-r--   0 user      (1000) user      (1000)     6218 2021-05-16 21:23:32.000000 ovos_utils-0.0.9/ovos_utils/configuration.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.541195 ovos_utils-0.0.9/ovos_utils/enclosure/
--rw-rw-r--   0 user      (1000) user      (1000)     1913 2021-05-16 21:23:32.000000 ovos_utils-0.0.9/ovos_utils/enclosure/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10838 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/api.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.541195 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/
--rw-rw-r--   0 user      (1000) user      (1000)      134 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.541195 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/eyes/
--rw-rw-r--   0 user      (1000) user      (1000)    14115 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/eyes/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.541195 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/
--rw-rw-r--   0 user      (1000) user      (1000)    13244 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    19821 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/animations.py
--rw-rw-r--   0 user      (1000) user      (1000)    15039 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/cellular_automaton.py
--rw-rw-r--   0 user      (1000) user      (1000)     5542 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/icons.py
--rw-rw-r--   0 user      (1000) user      (1000)    14722 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/enclosure/template.py
--rw-rw-r--   0 user      (1000) user      (1000)    15148 2021-05-16 21:23:32.000000 ovos_utils-0.0.9/ovos_utils/fingerprinting.py
--rw-rw-r--   0 user      (1000) user      (1000)    30682 2021-04-02 15:27:29.000000 ovos_utils-0.0.9/ovos_utils/gui.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/ovos_utils/intents/
--rw-rw-r--   0 user      (1000) user      (1000)    17290 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/intents/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5378 2020-12-20 16:25:19.000000 ovos_utils-0.0.9/ovos_utils/intents/layers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2021-05-16 21:23:48.000000 ovos_utils-0.0.9/ovos_utils/json_helper.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/ovos_utils/lang/
--rw-rw-r--   0 user      (1000) user      (1000)     1606 2021-03-07 16:27:35.000000 ovos_utils-0.0.9/ovos_utils/lang/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1527 2021-03-07 16:27:35.000000 ovos_utils-0.0.9/ovos_utils/lang/detect.py
--rw-rw-r--   0 user      (1000) user      (1000)     1240 2021-01-20 19:17:32.000000 ovos_utils-0.0.9/ovos_utils/lang/phonemes.py
--rw-rw-r--   0 user      (1000) user      (1000)      634 2021-03-07 16:27:35.000000 ovos_utils-0.0.9/ovos_utils/lang/translate.py
--rw-rw-r--   0 user      (1000) user      (1000)     1209 2021-01-20 19:17:32.000000 ovos_utils-0.0.9/ovos_utils/lang/visimes.py
--rw-rw-r--   0 user      (1000) user      (1000)     3957 2021-01-20 19:17:32.000000 ovos_utils-0.0.9/ovos_utils/log.py
--rw-rw-r--   0 user      (1000) user      (1000)    16401 2021-05-16 21:23:32.000000 ovos_utils-0.0.9/ovos_utils/messagebus.py
--rw-rw-r--   0 user      (1000) user      (1000)      966 2021-05-09 23:12:54.000000 ovos_utils-0.0.9/ovos_utils/network_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    10051 2021-03-25 17:47:40.000000 ovos_utils-0.0.9/ovos_utils/parse.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.541195 ovos_utils-0.0.9/ovos_utils/res/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/ovos_utils/res/platform_fingerprints/
--rw-rw-r--   0 user      (1000) user      (1000)      800 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/res/platform_fingerprints/spoofed_ovos.json
--rw-rw-r--   0 user      (1000) user      (1000)     3736 2021-03-07 16:27:35.000000 ovos_utils-0.0.9/ovos_utils/security.py
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2021-03-06 13:19:50.000000 ovos_utils-0.0.9/ovos_utils/signal.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/ovos_utils/skills/
--rw-rw-r--   0 user      (1000) user      (1000)     2633 2021-05-09 22:57:24.000000 ovos_utils-0.0.9/ovos_utils/skills/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6530 2021-04-02 15:27:29.000000 ovos_utils-0.0.9/ovos_utils/skills/audioservice.py
--rw-rw-r--   0 user      (1000) user      (1000)     2845 2021-03-07 16:27:35.000000 ovos_utils-0.0.9/ovos_utils/skills/settings.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/ovos_utils/sound/
--rw-rw-r--   0 user      (1000) user      (1000)     2995 2020-12-20 16:34:54.000000 ovos_utils-0.0.9/ovos_utils/sound/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3256 2020-12-20 16:25:19.000000 ovos_utils-0.0.9/ovos_utils/sound/alsa.py
--rw-rw-r--   0 user      (1000) user      (1000)     4926 2020-12-20 16:25:19.000000 ovos_utils-0.0.9/ovos_utils/sound/pulse.py
--rw-rw-r--   0 user      (1000) user      (1000)     9528 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/ovos_utils/ssml.py
--rw-rw-r--   0 user      (1000) user      (1000)     6611 2021-05-16 21:23:32.000000 ovos_utils-0.0.9/ovos_utils/system.py
--rw-rw-r--   0 user      (1000) user      (1000)     1683 2020-12-20 16:25:19.000000 ovos_utils-0.0.9/ovos_utils/xml_helper.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.541195 ovos_utils-0.0.9/ovos_utils.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      316 2021-05-16 21:24:46.000000 ovos_utils-0.0.9/ovos_utils.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1444 2021-05-16 21:24:46.000000 ovos_utils-0.0.9/ovos_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2021-05-16 21:24:46.000000 ovos_utils-0.0.9/ovos_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      132 2021-05-16 21:24:46.000000 ovos_utils-0.0.9/ovos_utils.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       11 2021-05-16 21:24:46.000000 ovos_utils-0.0.9/ovos_utils.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      983 2021-05-16 21:23:48.000000 ovos_utils-0.0.9/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-05-16 21:24:46.545195 ovos_utils-0.0.9/test/
--rw-rw-r--   0 user      (1000) user      (1000)     3072 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/test/test_color.py
--rw-rw-r--   0 user      (1000) user      (1000)     5451 2021-05-16 21:23:46.000000 ovos_utils-0.0.9/test/test_json_helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6262 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/test/test_parse.py
--rw-rw-r--   0 user      (1000) user      (1000)     6613 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/test/test_ssml.py
--rw-rw-r--   0 user      (1000) user      (1000)     1422 2021-01-20 19:10:59.000000 ovos_utils-0.0.9/test/test_utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.210512 ovos_utils-0.0.9a1/
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)      318 2021-04-04 11:00:19.210512 ovos_utils-0.0.9a1/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.174511 ovos_utils-0.0.9a1/ovos_utils/
+-rw-rw-r--   0 user      (1000) user      (1000)     7096 2021-04-04 10:59:30.000000 ovos_utils-0.0.9a1/ovos_utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7215 2020-12-20 16:25:19.000000 ovos_utils-0.0.9a1/ovos_utils/colors.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5318 2021-03-02 11:47:43.000000 ovos_utils-0.0.9a1/ovos_utils/configuration.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.178511 ovos_utils-0.0.9a1/ovos_utils/enclosure/
+-rw-rw-r--   0 user      (1000) user      (1000)     2056 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10838 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/api.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.182511 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/
+-rw-rw-r--   0 user      (1000) user      (1000)      134 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.186511 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/eyes/
+-rw-rw-r--   0 user      (1000) user      (1000)    14115 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/eyes/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.190512 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/
+-rw-rw-r--   0 user      (1000) user      (1000)    13244 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19821 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/animations.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15039 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/cellular_automaton.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5542 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/icons.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14722 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/enclosure/template.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30682 2021-04-02 15:27:29.000000 ovos_utils-0.0.9a1/ovos_utils/gui.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.190512 ovos_utils-0.0.9a1/ovos_utils/intents/
+-rw-rw-r--   0 user      (1000) user      (1000)    17290 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/intents/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5378 2020-12-20 16:25:19.000000 ovos_utils-0.0.9a1/ovos_utils/intents/layers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4407 2021-03-25 17:48:15.000000 ovos_utils-0.0.9a1/ovos_utils/json_helper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.194512 ovos_utils-0.0.9a1/ovos_utils/lang/
+-rw-rw-r--   0 user      (1000) user      (1000)     1606 2021-03-07 16:27:35.000000 ovos_utils-0.0.9a1/ovos_utils/lang/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1527 2021-03-07 16:27:35.000000 ovos_utils-0.0.9a1/ovos_utils/lang/detect.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1240 2021-01-20 19:17:32.000000 ovos_utils-0.0.9a1/ovos_utils/lang/phonemes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      634 2021-03-07 16:27:35.000000 ovos_utils-0.0.9a1/ovos_utils/lang/translate.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1209 2021-01-20 19:17:32.000000 ovos_utils-0.0.9a1/ovos_utils/lang/visimes.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3957 2021-01-20 19:17:32.000000 ovos_utils-0.0.9a1/ovos_utils/log.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16865 2021-03-02 11:47:43.000000 ovos_utils-0.0.9a1/ovos_utils/messagebus.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10051 2021-03-25 17:47:40.000000 ovos_utils-0.0.9a1/ovos_utils/parse.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.162511 ovos_utils-0.0.9a1/ovos_utils/res/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.194512 ovos_utils-0.0.9a1/ovos_utils/res/platform_fingerprints/
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/res/platform_fingerprints/spoofed_ovos.json
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.198511 ovos_utils-0.0.9a1/ovos_utils/res/ui/
+-rw-rw-r--   0 user      (1000) user      (1000)    13139 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/AudioPlayer.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     1992 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/CategoryBoxHistoryView.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     1927 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/CategoryBoxHomeView.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     4478 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/CategoryBoxSearchView.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     6023 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/Disambiguation.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     6730 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/Homescreen.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     6006 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/Playlist.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     2742 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_AnimatedImageFrame.qml
+-rw-rw-r--   0 user      (1000) user      (1000)      478 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_HtmlFrame.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     2734 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_ImageFrame.qml
+-rw-rw-r--   0 user      (1000) user      (1000)    11237 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_SkillSettings.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     1020 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_TextFrame.qml
+-rw-rw-r--   0 user      (1000) user      (1000)      405 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_UrlFrame.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     6421 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_VideoPlayer.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     1185 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SYSTEM_status.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     8657 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/SeekControl.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     1831 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/TopBarTabButton.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     5696 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/VideoPlayer.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     2727 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/WebViewHtmlFrame.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     2539 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/WebViewUrlFrame.qml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.198511 ovos_utils-0.0.9a1/ovos_utils/res/ui/delegates/
+-rw-rw-r--   0 user      (1000) user      (1000)     4693 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/delegates/GridVideoCard.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     6212 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/delegates/ListVideoCard.qml
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/delegates/qmldir
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.198511 ovos_utils-0.0.9a1/ovos_utils/res/ui/icons/
+-rw-rw-r--   0 user      (1000) user      (1000)     1861 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/icons/check-circle.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     1998 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/icons/info-circle.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     1880 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/icons/times-circle.svg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.202512 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/
+-rw-rw-r--   0 user      (1000) user      (1000)     1772 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/back.png
+-rw-rw-r--   0 user      (1000) user      (1000)     2644 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/back.svg
+-rw-rw-r--   0 user      (1000) user      (1000)    31940 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/gridpage.jpg
+-rw-rw-r--   0 user      (1000) user      (1000)     2186 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/history.png
+-rw-rw-r--   0 user      (1000) user      (1000)     1446 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/home.png
+-rw-rw-r--   0 user      (1000) user      (1000)     2708 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/information.png
+-rw-rw-r--   0 user      (1000) user      (1000)      951 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-album-track.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     4479 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-fullscreen.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     3881 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-mute.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     3046 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-next.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     3013 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-pause.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     2666 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-play.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      290 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-playback-pause.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      275 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-playback-start.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      277 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-playback-stop.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      665 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-playlist-play.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      561 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-playlist-repeat.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      644 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-playlist-shuffle.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     3050 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-previous.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     1334 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-repeat-playlist.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     1168 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-repeat-track.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     5492 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-repeat.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      288 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-seek-backward.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      287 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-seek-forward.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      383 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-skip-backward.svg
+-rw-rw-r--   0 user      (1000) user      (1000)      386 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-skip-forward.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     2822 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-stop.svg
+-rw-rw-r--   0 user      (1000) user      (1000)     4002 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/media-unmute.svg
+-rwxrwxr-x   0 user      (1000) user      (1000)     7281 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/moviesandfilms.png
+-rw-rw-r--   0 user      (1000) user      (1000)     2385 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/search.png
+-rw-rw-r--   0 user      (1000) user      (1000)    97623 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/images/spinner.gif
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.202512 ovos_utils-0.0.9a1/ovos_utils/res/ui/settings_ui/
+-rw-rw-r--   0 user      (1000) user      (1000)      374 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/settings_ui/settingButton.qml
+-rw-rw-r--   0 user      (1000) user      (1000)      360 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/settings_ui/settingCheckBox.qml
+-rw-rw-r--   0 user      (1000) user      (1000)      174 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/settings_ui/settingLabelBox.qml
+-rw-rw-r--   0 user      (1000) user      (1000)      441 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/settings_ui/settingNumberBox.qml
+-rw-rw-r--   0 user      (1000) user      (1000)      439 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/settings_ui/settingPasswordBox.qml
+-rw-rw-r--   0 user      (1000) user      (1000)      392 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/settings_ui/settingTextBox.qml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.202512 ovos_utils-0.0.9a1/ovos_utils/res/ui/views/
+-rw-rw-r--   0 user      (1000) user      (1000)     3171 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/views/GridTileView.qml
+-rw-rw-r--   0 user      (1000) user      (1000)     4927 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/views/TileView.qml
+-rw-rw-r--   0 user      (1000) user      (1000)       60 2021-04-03 23:51:25.000000 ovos_utils-0.0.9a1/ovos_utils/res/ui/views/qmldir
+-rw-rw-r--   0 user      (1000) user      (1000)     3736 2021-03-07 16:27:35.000000 ovos_utils-0.0.9a1/ovos_utils/security.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2021-03-06 13:19:50.000000 ovos_utils-0.0.9a1/ovos_utils/signal.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.202512 ovos_utils-0.0.9a1/ovos_utils/skills/
+-rw-rw-r--   0 user      (1000) user      (1000)     2035 2021-03-06 16:18:51.000000 ovos_utils-0.0.9a1/ovos_utils/skills/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6530 2021-04-02 15:27:29.000000 ovos_utils-0.0.9a1/ovos_utils/skills/audioservice.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2845 2021-03-07 16:27:35.000000 ovos_utils-0.0.9a1/ovos_utils/skills/settings.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.206512 ovos_utils-0.0.9a1/ovos_utils/sound/
+-rw-rw-r--   0 user      (1000) user      (1000)     2995 2020-12-20 16:34:54.000000 ovos_utils-0.0.9a1/ovos_utils/sound/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3256 2020-12-20 16:25:19.000000 ovos_utils-0.0.9a1/ovos_utils/sound/alsa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4926 2020-12-20 16:25:19.000000 ovos_utils-0.0.9a1/ovos_utils/sound/pulse.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9528 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/ssml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6982 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/ovos_utils/system.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1683 2020-12-20 16:25:19.000000 ovos_utils-0.0.9a1/ovos_utils/xml_helper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.174511 ovos_utils-0.0.9a1/ovos_utils.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      318 2021-04-04 11:00:19.000000 ovos_utils-0.0.9a1/ovos_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     4170 2021-04-04 11:00:19.000000 ovos_utils-0.0.9a1/ovos_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2021-04-04 11:00:19.000000 ovos_utils-0.0.9a1/ovos_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      126 2021-04-04 11:00:19.000000 ovos_utils-0.0.9a1/ovos_utils.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       11 2021-04-04 11:00:19.000000 ovos_utils-0.0.9a1/ovos_utils.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2021-04-04 11:00:19.210512 ovos_utils-0.0.9a1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      968 2021-04-03 23:46:07.000000 ovos_utils-0.0.9a1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-04 11:00:19.210512 ovos_utils-0.0.9a1/test/
+-rw-rw-r--   0 user      (1000) user      (1000)     3072 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/test/test_color.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3501 2021-03-25 17:48:27.000000 ovos_utils-0.0.9a1/test/test_json_helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6262 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/test/test_parse.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6613 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/test/test_ssml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1422 2021-01-20 19:10:59.000000 ovos_utils-0.0.9a1/test/test_utils.py
```

### Comparing `ovos_utils-0.0.9/ovos_utils/__init__.py` & `ovos_utils-0.0.9a1/ovos_utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from threading import Thread
 from time import sleep
+import requests
 import os
 from os.path import isdir, join, dirname
 import re
+import socket
 import datetime
 import kthread
-from ovos_utils.network_utils import *
 from inflection import camelize, titleize, transliterate, parameterize, \
     ordinalize
 
 
 def ensure_mycroft_import():
     try:
         import mycroft
@@ -31,14 +32,32 @@
         MYCROFT_ROOT_PATH = get_mycroft_root()
         if MYCROFT_ROOT_PATH is not None:
             sys.path.append(MYCROFT_ROOT_PATH)
         else:
             raise
 
 
+def get_ip():
+    # taken from https://stackoverflow.com/a/28950776/13703283
+    s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+    try:
+        # doesn't even have to be reachable
+        s.connect(('10.255.255.255', 1))
+        IP = s.getsockname()[0]
+    except Exception:
+        IP = '127.0.0.1'
+    finally:
+        s.close()
+    return IP
+
+
+def get_external_ip():
+    return requests.get('https://api.ipify.org').text
+
+
 def resolve_ovos_resource_file(res_name):
     """Convert a resource into an absolute filename.
     used internally for ovos resources
     """
     # First look for fully qualified file (e.g. a user setting)
     if os.path.isfile(res_name):
         return res_name
```

### Comparing `ovos_utils-0.0.9/ovos_utils/colors.py` & `ovos_utils-0.0.9a1/ovos_utils/colors.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/configuration.py` & `ovos_utils-0.0.9a1/ovos_utils/configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-from os.path import isfile, exists, expanduser, join, dirname, isdir
-from os import makedirs
-import json
 from ovos_utils.log import LOG
+from ovos_utils.enclosure import detect_enclosure
+from ovos_utils.enclosure import MycroftEnclosures
 from ovos_utils.json_helper import merge_dict, load_commented_json
 from ovos_utils.system import search_mycroft_core_location
-from xdg import BaseDirectory as XDG
-from ovos_utils.fingerprinting import core_supports_xdg, \
-    detect_platform, MycroftPlatform, get_config_fingerprint
-
+from os.path import isfile, exists, expanduser, join, dirname, isdir
+from os import makedirs
+import json
 
-MYCROFT_DEFAULT_CONFIG = join("{ROOT_PATH}", "mycroft",
-                              "configuration", "mycroft.conf")
 MYCROFT_SYSTEM_CONFIG = "/etc/mycroft/mycroft.conf"
-MYCROFT_OLD_USER_CONFIG = join(expanduser("~"), ".mycroft", "mycroft.conf")
-MYCROFT_XDG_USER_CONFIG = join(XDG.save_config_path('mycroft'), 'mycroft.conf')
-MYCROFT_USER_CONFIG = MYCROFT_XDG_USER_CONFIG
-
-
-def set_config_name(name, core_folder=None):
-    global MYCROFT_USER_CONFIG, MYCROFT_SYSTEM_CONFIG, \
-        MYCROFT_XDG_USER_CONFIG, MYCROFT_OLD_USER_CONFIG, \
-        MYCROFT_DEFAULT_CONFIG
-
-    core_folder = core_folder or name
-    MYCROFT_DEFAULT_CONFIG = join("{ROOT_PATH}", core_folder,
-                                  "configuration", f"{name}.conf")
-    MYCROFT_SYSTEM_CONFIG = f"/etc/{name}/{name}.conf"
-    MYCROFT_OLD_USER_CONFIG = join(expanduser("~"), f".{name}", f"{name}.conf")
-    MYCROFT_XDG_USER_CONFIG = join(XDG.save_config_path(name), f'{name}.conf')
-    MYCROFT_USER_CONFIG = MYCROFT_XDG_USER_CONFIG
-    LOG.info("config paths changed:\n"
-             f"DEFAULT: {MYCROFT_DEFAULT_CONFIG}\n"
-             f"SYSTEM: {MYCROFT_SYSTEM_CONFIG}\n"
-             f"USER: {MYCROFT_USER_CONFIG}\n"
-             f"OLD_USER: {MYCROFT_OLD_USER_CONFIG}")
+MYCROFT_USER_CONFIG = join(expanduser("~"), ".mycroft", "mycroft.conf")
+
+
+def get_config_fingerprint(config=None):
+    conf = config or read_mycroft_config()
+    listener_conf = conf.get("listener", {})
+    skills_conf = conf.get("skills", {})
+    return {
+        "enclosure": conf.get("enclosure", {}).get("platform"),
+        "data_dir": conf.get("data_dir"),
+        "msm_skills_dir": skills_conf.get("msm", {}).get("directory"),
+        "ipc_path": conf.get("ipc_path"),
+        "input_device_name": listener_conf.get("device_name"),
+        "input_device_index": listener_conf.get("device_index"),
+        "default_audio_backend": conf.get("Audio", {}).get("default-backend"),
+        "priority_skills": skills_conf.get("priority_skills"),
+        "backend_url": conf.get("server", {}).get("url")
+    }
 
 
 def read_mycroft_config():
     conf = LocalConf(None)
     conf.merge(MycroftDefaultConfig())
     conf.merge(MycroftSystemConfig())
     conf.merge(MycroftUserConfig())
@@ -50,15 +42,15 @@
     else:
         conf = LocalConf(path)
     conf.merge(config)
     conf.store()
     return conf
 
 
-# TODO consider using json_database.JsonStorage
+# TODO use json_database.JsonStorage
 class LocalConf(dict):
     """
         Config dict from file.
     """
     allow_overwrite = True
 
     def __init__(self, path):
@@ -109,15 +101,14 @@
     def merge(self, conf):
         merge_dict(self, conf)
         return self
 
 
 class ReadOnlyConfig(LocalConf):
     """ read only  """
-
     def __init__(self, path, allow_overwrite=False):
         super().__init__(path)
         self.allow_overwrite = allow_overwrite
 
     def reload(self):
         old = self.allow_overwrite
         self.allow_overwrite = True
@@ -143,37 +134,29 @@
         if not self.allow_overwrite:
             raise PermissionError
         super().store(path)
 
 
 class MycroftUserConfig(LocalConf):
     def __init__(self):
-        if core_supports_xdg():
-            path = MYCROFT_XDG_USER_CONFIG
-        else:
-            path = MYCROFT_USER_CONFIG
-            # mark1 runs as a different user
-            if detect_platform() == MycroftPlatform.MARK1:
-                path = "/home/mycroft/.mycroft/mycroft.conf"
-
-        if not isfile(path) and isfile(MYCROFT_OLD_USER_CONFIG):
-            # xdg might be disabled in HolmesV compatibility mode
-            # or migration might be in progress
-            # (user action required when updated from a no xdg install)
-            path = MYCROFT_OLD_USER_CONFIG
-
+        path = MYCROFT_USER_CONFIG
+        enclosure = detect_enclosure()
+        if enclosure == MycroftEnclosures.MARK1 or \
+                enclosure == MycroftEnclosures.OLD_MARK1:
+            path = "/home/mycroft/.mycroft/mycroft.conf"
         super().__init__(path)
 
 
 class MycroftDefaultConfig(ReadOnlyConfig):
     def __init__(self):
         mycroft_root = search_mycroft_core_location()
         if not mycroft_root:
             raise FileNotFoundError("Couldn't find mycroft core root folder.")
-        path = MYCROFT_DEFAULT_CONFIG.replace("{ROOT_PATH}", mycroft_root)
+        path = join(mycroft_root, "mycroft",
+                    "configuration", "mycroft.conf")
         super().__init__(path)
         if not self.path or not isfile(self.path):
             LOG.error("mycroft root path not found, could not load default "
                       ".conf")
 
     def set_root_config_path(self, root_config):
         # in case we got it wrong / non standard
@@ -182,11 +165,8 @@
 
 
 class MycroftSystemConfig(ReadOnlyConfig):
     def __init__(self, allow_overwrite=False):
         super().__init__(MYCROFT_SYSTEM_CONFIG, allow_overwrite)
 
 
-class MycroftXDGConfig(LocalConf):
-    def __init__(self):
-        path = MYCROFT_XDG_USER_CONFIG
-        super().__init__(path)
+
```

### Comparing `ovos_utils-0.0.9/ovos_utils/enclosure/api.py` & `ovos_utils-0.0.9a1/ovos_utils/enclosure/api.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/enclosure/mark1/eyes/__init__.py` & `ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/eyes/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/__init__.py` & `ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/animations.py` & `ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/animations.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/cellular_automaton.py` & `ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/cellular_automaton.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/enclosure/mark1/faceplate/icons.py` & `ovos_utils-0.0.9a1/ovos_utils/enclosure/mark1/faceplate/icons.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/enclosure/template.py` & `ovos_utils-0.0.9a1/ovos_utils/enclosure/template.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/gui.py` & `ovos_utils-0.0.9a1/ovos_utils/gui.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/intents/__init__.py` & `ovos_utils-0.0.9a1/ovos_utils/intents/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/intents/layers.py` & `ovos_utils-0.0.9a1/ovos_utils/intents/layers.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/json_helper.py` & `ovos_utils-0.0.9a1/ovos_utils/json_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,13 @@
 import json
-from copy import copy
 from json_database.utils import is_jsonifiable, get_key_recursively, \
     get_key_recursively_fuzzy, get_value_recursively_fuzzy, \
     get_value_recursively, jsonify_recursively
 
 
-def nested_get(base, key_list):
-    """Access a nested object in base by item sequence."""
-    if not len(key_list):
-        return None
-    val = copy(base)
-    for key in key_list:
-        if key not in val:
-            return None
-        val = val[key]
-    return val
-
-
-def nested_set(base, key_list, value):
-    """Set a value in a nested object in base by item sequence."""
-    for key in key_list[:-1]:
-        base = base.setdefault(key, {})
-    base[key_list[-1]] = value
-    return base
-
-
-def nested_delete(base, key_list):
-    """Delete a value in a nested object in base by item sequence."""
-    if not len(key_list):
-        return base
-    d = base
-    for key in key_list[:-1]:
-        if key not in base:
-            return base
-        d = d[key]
-    d.pop(key_list[-1])
-    return base
-
-
-def flatten_dict(base, separator=":"):
-    new_dict = {}
-    for key, value in base.items():
-        if isinstance(value, dict):
-            new_dict.update(
-                {separator.join([key, k]): v
-                 for k, v in flatten_dict(value).items()}
-            )
-        else:
-            new_dict[key] = value
-    return new_dict
-
-
-def flattened_get(base, key, separator=":"):
-    return flatten_dict(base, separator=separator).get(key)
-
-
-def flattened_set(base, key, value, separator=":"):
-    keys = key.split(separator)
-    return nested_set(base, keys, value)
-
-
-def flattened_delete(base, key, separator=":"):
-    keys = key.split(separator)
-    return nested_delete(base, keys)
-
-
-def invert_dict(base):
-    return {v: k for k, v in base.items()}
-
-
 def merge_dict(base, delta, merge_lists=False, skip_empty=False,
                no_dupes=True, new_only=False):
     """
         Recursively merges two dictionaries
         including dictionaries within dictionaries.
 
         Args:
@@ -170,7 +105,27 @@
             continue
         elif isinstance(base[k], dict) and isinstance(delta[k], dict):
             if not is_compatible_dict(delta[k], base[k]):
                 return False
         elif type(base[k]) != type(delta[k]):
             return False
     return True
+
+
+def delete_key_from_dict(key, dictionary):
+    """Recursivily find nested key in a dict and delete it.
+    Arguments:
+        key (str): a period separated list of nested keys to remove
+                   eg "nested.dict.keys"
+        dictionary (dict): the dictionary to remove keys from
+    Returns:
+        Dict: original dictionary with specified keys deleted.
+    """
+    modified_dict = dict(dictionary)
+    key_list = key.split('.')
+    if len(key_list) == 1 and modified_dict.get(key) is not None:
+        del modified_dict[key]
+    elif len(key_list) > 1:
+        remaining_keys = '.'.join(key_list[1:])
+        if modified_dict.get(key_list[0]) is not None:
+            modified_dict[key_list[0]] = delete_key_from_dict(remaining_keys, modified_dict[key_list[0]])
+    return modified_dict
```

### Comparing `ovos_utils-0.0.9/ovos_utils/lang/__init__.py` & `ovos_utils-0.0.9a1/ovos_utils/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/lang/detect.py` & `ovos_utils-0.0.9a1/ovos_utils/lang/detect.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/lang/phonemes.py` & `ovos_utils-0.0.9a1/ovos_utils/lang/phonemes.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/lang/translate.py` & `ovos_utils-0.0.9a1/ovos_utils/lang/translate.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/lang/visimes.py` & `ovos_utils-0.0.9a1/ovos_utils/lang/visimes.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/log.py` & `ovos_utils-0.0.9a1/ovos_utils/log.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/messagebus.py` & `ovos_utils-0.0.9a1/ovos_utils/messagebus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,116 +1,113 @@
 from mycroft_bus_client import MessageBusClient, Message
 from ovos_utils.log import LOG
 from ovos_utils.configuration import read_mycroft_config
 from ovos_utils import create_loop
 from ovos_utils.json_helper import merge_dict
 import time
 import json
-from pyee import BaseEventEmitter
-from threading import Event
 
 
 class FakeBus:
     def __init__(self, *args, **kwargs):
-        self.started_running = False
-        self.ee = kwargs.get("emitter") or BaseEventEmitter()
-        self.ee.on("error", self.on_error)
-        self.on_open()
+        self.events = {}
+        self.once_events = {}
+        self.received_msgs = []
 
     def on(self, msg_type, handler):
-        self.ee.on(msg_type, handler)
+        if msg_type not in self.events:
+            self.events[msg_type] = []
+        self.events[msg_type].append(handler)
 
     def once(self, msg_type, handler):
-        self.ee.once(msg_type, handler)
+        if msg_type not in self.once_events:
+            self.once_events[msg_type] = []
+        self.once_events[msg_type].append(handler)
 
     def emit(self, message):
-        self.ee.emit("message", message.serialize())
-        self.ee.emit(message.msg_type, message)
+        self.received_msgs.append(message)
+        if message.msg_type in self.events:
+            for handler in self.events[message.msg_type]:
+                handler(message)
+        if message.msg_type in self.once_events:
+            for handler in self.once_events[message.msg_type]:
+                handler(message)
+            self.once_events.pop(message.msg_type)
 
     def wait_for_message(self, message_type, timeout=3.0):
         """Wait for a message of a specific type.
 
         Arguments:
             message_type (str): the message type of the expected message
             timeout: seconds to wait before timeout, defaults to 3
 
         Returns:
             The received message or None if the response timed out
         """
-        received_event = Event()
-        received_event.clear()
-
-        msg = None
-
-        def rcv(m):
-            nonlocal msg
-            msg = m
-            received_event.set()
-
-        self.ee.once(message_type, rcv)
-        received_event.wait(timeout)
-        return msg
+        start = time.monotonic()
+        while time.monotonic() - start <= timeout:
+            time.sleep(0.1)
+            for m in self.received_msgs:
+                if m.msg_type == message_type:
+                    return m
+        return None
 
     def wait_for_response(self, message, reply_type=None, timeout=3.0):
         """Send a message and wait for a response.
 
         Arguments:
             message (Message): message to send
             reply_type (str): the message type of the expected reply.
                               Defaults to "<message.msg_type>.response".
             timeout: seconds to wait before timeout, defaults to 3
 
         Returns:
             The received message or None if the response timed out
         """
+        start = time.monotonic()
         reply_type = reply_type or message.msg_type + ".response"
-        received_event = Event()
-        received_event.clear()
-
-        msg = None
-
-        def rcv(m):
-            nonlocal msg
-            msg = m
-            received_event.set()
-
-        self.ee.once(reply_type, rcv)
         self.emit(message)
-        received_event.wait(timeout)
-        return msg
+        while time.monotonic() - start <= timeout:
+            time.sleep(0.1)
+            for m in self.received_msgs:
+                if m.msg_type == reply_type:
+                    return m
+        return None
 
     def remove(self, msg_type, handler):
-        try:
-            self.ee.remove_listener(msg_type, handler)
-        except:
-            pass
+        if msg_type in self.events:
+            if handler in self.events[msg_type]:
+                self.events[msg_type].remove(handler)
+        if msg_type in self.once_events:
+            if handler in self.once_events[msg_type]:
+                self.once_events[msg_type].remove(handler)
 
     def remove_all_listeners(self, event_name):
-        self.ee.remove_all_listeners(event_name)
+        if event_name in self.events:
+            self.events.pop(event_name)
+        if event_name in self.once_events:
+            self.once_events.pop(event_name)
 
     def create_client(self):
         return self
 
     def on_error(self, error):
-        LOG.error(error)
+        pass
 
     def on_open(self):
         pass
 
     def on_close(self):
         pass
 
     def run_forever(self):
-        self.started_running = True
-
-    def run_in_thread(self):
-        self.run_forever()
+        pass
 
     def close(self):
-        self.on_close()
+        pass
 
 
 def get_websocket(host, port, route='/', ssl=False, threaded=True):
     """
     Returns a connection to a websocket
     """
     client = MessageBusClient(host, port, route, ssl)
```

### Comparing `ovos_utils-0.0.9/ovos_utils/parse.py` & `ovos_utils-0.0.9a1/ovos_utils/parse.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/res/platform_fingerprints/spoofed_ovos.json` & `ovos_utils-0.0.9a1/ovos_utils/res/platform_fingerprints/spoofed_ovos.json`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/security.py` & `ovos_utils-0.0.9a1/ovos_utils/security.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/signal.py` & `ovos_utils-0.0.9a1/ovos_utils/signal.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/skills/audioservice.py` & `ovos_utils-0.0.9a1/ovos_utils/skills/audioservice.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/skills/settings.py` & `ovos_utils-0.0.9a1/ovos_utils/skills/settings.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/sound/__init__.py` & `ovos_utils-0.0.9a1/ovos_utils/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/sound/alsa.py` & `ovos_utils-0.0.9a1/ovos_utils/sound/alsa.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/sound/pulse.py` & `ovos_utils-0.0.9a1/ovos_utils/sound/pulse.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/ssml.py` & `ovos_utils-0.0.9a1/ovos_utils/ssml.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/ovos_utils/system.py` & `ovos_utils-0.0.9a1/ovos_utils/system.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,31 @@
+#!/usr/bin/env python3
+import sys
 import os
 import subprocess
 import re
 import shutil
 import sys
 import sysconfig
 from enum import Enum
-
-from os.path import expanduser, exists, join, isfile
-from ovos_utils.log import LOG
+import platform
+import socket
+from os.path import expanduser, exists, join
 
 
 class MycroftRootLocations(str, Enum):
     PICROFT = "/home/pi/mycroft-core"
     BIGSCREEN = "/home/mycroft/mycroft-core"
     OVOS = "/usr/lib/python3.9/site-packages"
     OLD_MARK1 = "/opt/venvs/mycroft-core/lib/python3.4/site-packages"
     MARK1 = "/opt/venvs/mycroft-core/lib/python3.7/site-packages"
     MARK2 = "/opt/mycroft"
     HOME = expanduser("~/mycroft-core")  # git clones
 
 
-_USER_DEFINED_ROOT = None
-
-
-# system utils
-def ntp_sync():
-    # Force the system clock to synchronize with internet time servers
-    subprocess.call('service ntp stop', shell=True)
-    subprocess.call('ntpd -gq', shell=True)
-    subprocess.call('service ntp start', shell=True)
-
-
-def system_shutdown():
-    # Turn the system completely off (with no option to inhibit it)
-    subprocess.call('sudo systemctl poweroff -i', shell=True)
-
-
-def system_reboot():
-    # Shut down and restart the system
-    subprocess.call('sudo systemctl reboot -i', shell=True)
-
-
-def ssh_enable():
-    # Permanently allow SSH access
-    subprocess.call('sudo systemctl enable ssh.service', shell=True)
-    subprocess.call('sudo systemctl start ssh.service', shell=True)
-
-
-def ssh_disable():
-    # Permanently block SSH access from the outside
-    subprocess.call('sudo systemctl stop ssh.service', shell=True)
-    subprocess.call('sudo systemctl disable ssh.service', shell=True)
-
-
-# platform fingerprinting
-def set_root_path(path):
-    global _USER_DEFINED_ROOT
-    _USER_DEFINED_ROOT = path
-    LOG.info(f"mycroft root set to {path}")
-
-
 def find_root_from_sys_path():
     """Find mycroft root folder from sys.path, eg. venv site-packages."""
     for p in [path for path in sys.path if path != '']:
         if exists(join(p, 'mycroft', 'configuration', 'mycroft.conf')):
             return p
     else:
         return None
@@ -77,17 +39,14 @@
     else:
         return None
 
 
 def search_mycroft_core_location():
     """Check python path (.venv), system packages and finally known mycroft
     locations."""
-    # downstream wants to override the root location
-    if _USER_DEFINED_ROOT:
-        return _USER_DEFINED_ROOT
     # if we are in a .venv that should take precedence over everything else
     if find_root_from_sitepackages():
         return find_root_from_sitepackages()
     # if there is a system wide install that should take precedence over
     # hardcoded locations
     elif find_root_from_sys_path():
         return find_root_from_sys_path()
@@ -184,9 +143,52 @@
             except:
                 have_display = False
         except ImportError:
             pass
     return have_display
 
 
+def get_platform_fingerprint():
+    return {
+        "hostname": socket.gethostname(),
+        "platform": platform.platform(),
+        "python_version": platform.python_version(),
+        "system": platform.system(),
+        "version": platform.version(),
+        "arch": platform.machine(),
+        "release": platform.release(),
+        "desktop_env": get_desktop_environment(),
+        "mycroft_core_location": search_mycroft_core_location(),
+        "can_display": has_screen(),
+        "is_gui_installed": is_installed("mycroft-gui-app"),
+        "is_vlc_installed": is_installed("vlc"),
+        "pulseaudio_running": is_process_running("pulseaudio")
+    }
+
+
+def ntp_sync():
+    # Force the system clock to synchronize with internet time servers
+    subprocess.call('service ntp stop', shell=True)
+    subprocess.call('ntpd -gq', shell=True)
+    subprocess.call('service ntp start', shell=True)
+
+
+def system_shutdown():
+    # Turn the system completely off (with no option to inhibit it)
+    subprocess.call('sudo systemctl poweroff -i', shell=True)
 
 
+def system_reboot():
+    # Shut down and restart the system
+    subprocess.call('sudo systemctl reboot -i', shell=True)
+
+
+def ssh_enable():
+    # Permanently allow SSH access
+    subprocess.call('sudo systemctl enable ssh.service', shell=True)
+    subprocess.call('sudo systemctl start ssh.service', shell=True)
+
+
+def ssh_disable():
+    # Permanently block SSH access from the outside
+    subprocess.call('sudo systemctl stop ssh.service', shell=True)
+    subprocess.call('sudo systemctl disable ssh.service', shell=True)
```

### Comparing `ovos_utils-0.0.9/ovos_utils/xml_helper.py` & `ovos_utils-0.0.9a1/ovos_utils/xml_helper.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/setup.py` & `ovos_utils-0.0.9a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup
 
 setup(
     name='ovos_utils',
-    version='0.0.9',
+    version='0.0.9a1',
     packages=['ovos_utils',
               'ovos_utils.intents',
               'ovos_utils.sound',
               "ovos_utils.enclosure",
               'ovos_utils.enclosure.mark1',
               'ovos_utils.enclosure.mark1.eyes',
               'ovos_utils.enclosure.mark1.faceplate',
               'ovos_utils.skills',
               'ovos_utils.lang'],
     url='https://github.com/OpenVoiceOS/ovos_utils',
     install_requires=[
         "mycroft-messagebus-client",
         "pexpect",
-        "pyxdg",
         "PyYAML",
         "kthread",
         "json_database",
         "requests",
         "inflection"],
     extras_require={
         "extras": ["phoneme_guesser", "colour", "rapidfuzz"]
```

### Comparing `ovos_utils-0.0.9/test/test_color.py` & `ovos_utils-0.0.9a1/test/test_color.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/test/test_parse.py` & `ovos_utils-0.0.9a1/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/test/test_ssml.py` & `ovos_utils-0.0.9a1/test/test_ssml.py`

 * *Files identical despite different names*

### Comparing `ovos_utils-0.0.9/test/test_utils.py` & `ovos_utils-0.0.9a1/test/test_utils.py`

 * *Files identical despite different names*

