# Comparing `tmp/rustplus-5.6.4.tar.gz` & `tmp/rustplus-5.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustplus-5.6.4.tar", last modified: Mon Jun  5 17:46:08 2023, max compression
+gzip compressed data, was "rustplus-5.6.5.tar", last modified: Wed Jun 14 14:01:27 2023, max compression
```

## Comparing `rustplus-5.6.4.tar` & `rustplus-5.6.5.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.999484 rustplus-5.6.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-05 17:45:57.000000 rustplus-5.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-05 17:45:57.000000 rustplus-5.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-05 17:46:07.999484 rustplus-5.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-06-05 17:45:57.000000 rustplus-5.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.991484 rustplus-5.6.4/rustplus/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.991484 rustplus-5.6.4/rustplus/api/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19956 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/base_rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.995484 rustplus-5.6.4/rustplus/api/icons/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/airfield.png
--rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/arctic_base.png
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/bandit.png
--rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/barn.png
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/cargo.png
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/chinook.png
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/chinook_blades.png
--rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/crate.png
--rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/desert_base.png
--rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/dome.png
--rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/excavator.png
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/explosion.png
--rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/fishing.png
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/harbour.png
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/junkyard.png
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/large_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/launchsite.png
--rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/lighthouse.png
--rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/military_tunnels.png
--rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/mining_outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/oxums.png
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/patrol.png
--rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/power_plant.png
--rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/quarry.png
--rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/satellite.png
--rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/sewer.png
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/small_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/stable.png
--rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/supermarket.png
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/swamp.png
--rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/train.png
--rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/train_yard.png
--rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/underwater_lab.png
--rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/vending_machine.png
--rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/icons/water_treatment.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.995484 rustplus-5.6.4/rustplus/api/remote/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.995484 rustplus-5.6.4/rustplus/api/remote/camera/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/camera/camera_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/camera/camera_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/camera/camera_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/camera/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.995484 rustplus-5.6.4/rustplus/api/remote/events/
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/events/event_loop_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/events/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/events/handler_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/events/map_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/events/registered_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/expo_bundle_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/fcm_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/rust_remote_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.995484 rustplus-5.6.4/rustplus/api/remote/rustplus_proto/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/rustplus_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/rustplus_proto/rustplus.py
--rw-r--r--   0 runner    (1001) docker     (122)    11369 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/rustws.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/remote/server_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.999484 rustplus-5.6.4/rustplus/api/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_contents.py
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_entity_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_team_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/rust_time.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/api/structures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.999484 rustplus-5.6.4/rustplus/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/commands/command_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/commands/command_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/commands/command_options.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.999484 rustplus-5.6.4/rustplus/conversation/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/conversation/conversation_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/conversation/conversation_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.999484 rustplus-5.6.4/rustplus/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.999484 rustplus-5.6.4/rustplus/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.999484 rustplus-5.6.4/rustplus/utils/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/fonts/PermanentMarker.ttf
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26480 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/grab_items.py
--rw-r--r--   0 runner    (1001) docker     (122)     5388 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/server_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-05 17:45:57.000000 rustplus-5.6.4/rustplus/utils/yielding_event.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:46:07.991484 rustplus-5.6.4/rustplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-05 17:46:07.000000 rustplus-5.6.4/rustplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-06-05 17:46:07.000000 rustplus-5.6.4/rustplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 17:46:07.000000 rustplus-5.6.4/rustplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-05 17:46:07.000000 rustplus-5.6.4/rustplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-05 17:46:07.000000 rustplus-5.6.4/rustplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-05 17:46:07.999484 rustplus-5.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-05 17:45:57.000000 rustplus-5.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-14 14:01:10.000000 rustplus-5.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-14 14:01:10.000000 rustplus-5.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-14 14:01:27.449625 rustplus-5.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-06-14 14:01:10.000000 rustplus-5.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.421625 rustplus-5.6.5/rustplus/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.421625 rustplus-5.6.5/rustplus/api/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20349 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/base_rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.433625 rustplus-5.6.5/rustplus/api/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/airfield.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/arctic_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/bandit.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/barn.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/cargo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/chinook.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/chinook_blades.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/crate.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/desert_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/dome.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/excavator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/explosion.png
+-rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/fishing.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/harbour.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/junkyard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/large_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/launchsite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/lighthouse.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/military_tunnels.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/mining_outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/oxums.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/patrol.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/power_plant.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/quarry.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/satellite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/sewer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/small_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/stable.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/supermarket.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/swamp.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/train.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/train_yard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/underwater_lab.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/vending_machine.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/water_treatment.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.437625 rustplus-5.6.5/rustplus/api/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.437625 rustplus-5.6.5/rustplus/api/remote/camera/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/camera_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/camera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/camera_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.441625 rustplus-5.6.5/rustplus/api/remote/events/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/event_loop_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/handler_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/map_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/registered_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/expo_bundle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/fcm_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rust_remote_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.441625 rustplus-5.6.5/rustplus/api/remote/rustplus_proto/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rustplus_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rustplus_proto/rustplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12369 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rustws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/server_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.441625 rustplus-5.6.5/rustplus/api/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_contents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_entity_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_team_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command_options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/conversation/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/conversation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/conversation_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/utils/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/fonts/PermanentMarker.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26480 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/grab_items.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5388 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/yielding_event.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.421625 rustplus-5.6.5/rustplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-14 14:01:27.449625 rustplus-5.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-14 14:01:10.000000 rustplus-5.6.5/setup.py
```

### Comparing `rustplus-5.6.4/LICENSE` & `rustplus-5.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/PKG-INFO` & `rustplus-5.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.6.4
+Version: 5.6.5
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.6.4/README.md` & `rustplus-5.6.5/README.md`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/__init__.py` & `rustplus-5.6.5/rustplus/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .commands import CommandOptions, Command
 from .exceptions import *
 from .conversation import ConversationFactory, Conversation, ConversationPrompt
 from .utils import *
 
 __name__ = "rustplus"
 __author__ = "olijeffers0n"
-__version__ = "5.6.4"
+__version__ = "5.6.5"
 __support__ = "Discord: https://discord.gg/nQqJe8qvP8"
```

### Comparing `rustplus-5.6.4/rustplus/api/base_rust_api.py` & `rustplus-5.6.5/rustplus/api/base_rust_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,19 +104,25 @@
         app_request.player_token = self.server_id.player_token
 
         self.seq += 1
 
         return app_request
 
     async def connect(
-        self, retries: int = float("inf"), delay: int = 20, on_failure=None
+        self, retries: int = float("inf"), delay: int = 20, on_failure=None, on_success=None
     ) -> None:
         """
         Attempts to open a connection to the rust game server specified in the constructor
 
+        :param retries: The number of times to attempt reconnecting. Defaults to infinite.
+        :param delay: The delay (in seconds) between reconnection attempts.
+        :param on_failure: Optional function to be called when connecting fails.
+        :param on_success: Optional function to be called when connecting succeeds.
+
+
         :return: None
         """
         EventLoopManager.set_loop(
             self.event_loop
             if self.event_loop is not None
             else asyncio.get_event_loop(),
             self.server_id,
@@ -134,14 +140,15 @@
 
         try:
             if self.remote.ws is None:
                 await self.remote.connect(
                     retries=retries,
                     delay=delay,
                     on_failure=on_failure,
+                    on_success=on_success
                 )
                 await self.heartbeat.start_beat()
         except ConnectionRefusedError:
             raise ServerNotResponsiveError("Cannot Connect")
 
     async def close_connection(self) -> None:
         """
```

### Comparing `rustplus-5.6.4/rustplus/api/icons/airfield.png` & `rustplus-5.6.5/rustplus/api/icons/airfield.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/arctic_base.png` & `rustplus-5.6.5/rustplus/api/icons/arctic_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/bandit.png` & `rustplus-5.6.5/rustplus/api/icons/bandit.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/barn.png` & `rustplus-5.6.5/rustplus/api/icons/barn.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/cargo.png` & `rustplus-5.6.5/rustplus/api/icons/cargo.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/chinook.png` & `rustplus-5.6.5/rustplus/api/icons/chinook.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/chinook_blades.png` & `rustplus-5.6.5/rustplus/api/icons/chinook_blades.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/crate.png` & `rustplus-5.6.5/rustplus/api/icons/crate.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/desert_base.png` & `rustplus-5.6.5/rustplus/api/icons/desert_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/dome.png` & `rustplus-5.6.5/rustplus/api/icons/dome.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/excavator.png` & `rustplus-5.6.5/rustplus/api/icons/excavator.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/explosion.png` & `rustplus-5.6.5/rustplus/api/icons/explosion.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/fishing.png` & `rustplus-5.6.5/rustplus/api/icons/fishing.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/harbour.png` & `rustplus-5.6.5/rustplus/api/icons/harbour.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/icon.png` & `rustplus-5.6.5/rustplus/api/icons/icon.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/junkyard.png` & `rustplus-5.6.5/rustplus/api/icons/junkyard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/large_oil_rig.png` & `rustplus-5.6.5/rustplus/api/icons/large_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/launchsite.png` & `rustplus-5.6.5/rustplus/api/icons/launchsite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/lighthouse.png` & `rustplus-5.6.5/rustplus/api/icons/lighthouse.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/military_tunnels.png` & `rustplus-5.6.5/rustplus/api/icons/military_tunnels.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/mining_outpost.png` & `rustplus-5.6.5/rustplus/api/icons/mining_outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/outpost.png` & `rustplus-5.6.5/rustplus/api/icons/outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/oxums.png` & `rustplus-5.6.5/rustplus/api/icons/oxums.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/patrol.png` & `rustplus-5.6.5/rustplus/api/icons/patrol.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/power_plant.png` & `rustplus-5.6.5/rustplus/api/icons/power_plant.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/quarry.png` & `rustplus-5.6.5/rustplus/api/icons/quarry.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/satellite.png` & `rustplus-5.6.5/rustplus/api/icons/satellite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/sewer.png` & `rustplus-5.6.5/rustplus/api/icons/sewer.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/small_oil_rig.png` & `rustplus-5.6.5/rustplus/api/icons/small_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/stable.png` & `rustplus-5.6.5/rustplus/api/icons/stable.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/supermarket.png` & `rustplus-5.6.5/rustplus/api/icons/supermarket.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/swamp.png` & `rustplus-5.6.5/rustplus/api/icons/swamp.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/train.png` & `rustplus-5.6.5/rustplus/api/icons/train.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/train_yard.png` & `rustplus-5.6.5/rustplus/api/icons/train_yard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/underwater_lab.png` & `rustplus-5.6.5/rustplus/api/icons/underwater_lab.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/vending_machine.png` & `rustplus-5.6.5/rustplus/api/icons/vending_machine.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/icons/water_treatment.png` & `rustplus-5.6.5/rustplus/api/icons/water_treatment.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/camera/camera_constants.py` & `rustplus-5.6.5/rustplus/api/remote/camera/camera_constants.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/camera/camera_manager.py` & `rustplus-5.6.5/rustplus/api/remote/camera/camera_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/camera/camera_parser.py` & `rustplus-5.6.5/rustplus/api/remote/camera/camera_parser.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/camera/structures.py` & `rustplus-5.6.5/rustplus/api/remote/camera/structures.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/events/event_handler.py` & `rustplus-5.6.5/rustplus/api/remote/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/events/event_loop_manager.py` & `rustplus-5.6.5/rustplus/api/remote/events/event_loop_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/events/events.py` & `rustplus-5.6.5/rustplus/api/remote/events/events.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/events/handler_list.py` & `rustplus-5.6.5/rustplus/api/remote/events/handler_list.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/events/map_event_listener.py` & `rustplus-5.6.5/rustplus/api/remote/events/map_event_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/events/registered_listener.py` & `rustplus-5.6.5/rustplus/api/remote/events/registered_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/expo_bundle_handler.py` & `rustplus-5.6.5/rustplus/api/remote/expo_bundle_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/fcm_listener.py` & `rustplus-5.6.5/rustplus/api/remote/fcm_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/heartbeat.py` & `rustplus-5.6.5/rustplus/api/remote/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/ratelimiter.py` & `rustplus-5.6.5/rustplus/api/remote/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/rust_remote_interface.py` & `rustplus-5.6.5/rustplus/api/remote/rust_remote_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,22 +62,23 @@
 
         self.magic_value = MagicValueGrabber.get_magic_value()
         self.conversation_factory = ConversationFactory(api)
         self.use_test_server = use_test_server
         self.pending_entity_subscriptions = []
         self.camera_manager: Union[CameraManager, None] = None
 
-    async def connect(self, retries, delay, on_failure=None) -> None:
+    async def connect(self, retries, delay, on_failure=None, on_success=None) -> None:
         self.ws = RustWebsocket(
             server_id=self.server_id,
             remote=self,
             use_proxy=self.use_proxy,
             magic_value=self.magic_value,
             use_test_server=self.use_test_server,
             on_failure=on_failure,
+            on_success=on_success,
             delay=delay,
         )
         await self.ws.connect(retries=retries)
 
         for entity_id, coroutine in self.pending_entity_subscriptions:
             self.handle_subscribing_entity(entity_id, coroutine)
```

### Comparing `rustplus-5.6.4/rustplus/api/remote/rustplus_proto/rustplus.py` & `rustplus-5.6.5/rustplus/api/remote/rustplus_proto/rustplus.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/remote/rustws.py` & `rustplus-5.6.5/rustplus/api/remote/rustws.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import base64
 import logging
 import time
 from datetime import datetime
-from typing import Optional, Union
+from typing import Optional, Union, Coroutine
 import betterproto
-from asyncio import Task
+from asyncio import Task, AbstractEventLoop
 from websockets.client import connect
 from websockets.legacy.client import WebSocketClientProtocol
 
 from .camera.structures import RayPacket
 from .rustplus_proto import AppMessage, AppRequest
 from .events import EventHandler
 from ..structures import RustChatMessage
@@ -28,28 +28,30 @@
         self,
         server_id: ServerID,
         remote,
         use_proxy,
         magic_value,
         use_test_server,
         on_failure,
+        on_success,
         delay,
     ):
         self.connection: Union[WebSocketClientProtocol, None] = None
         self.task: Union[Task, None] = None
         self.server_id = server_id
         self.connection_status = CLOSED
         self.use_proxy = use_proxy
         self.remote = remote
         self.logger = logging.getLogger("rustplus.py")
         self.connected_time = time.time()
         self.magic_value = magic_value
         self.use_test_server = use_test_server
         self.outgoing_conversation_messages = []
         self.on_failure = on_failure
+        self.on_success = on_success
         self.delay = delay
 
     async def connect(
         self, retries=float("inf"), ignore_open_value: bool = False
     ) -> None:
         if (
             not self.connection_status == CONNECTED or ignore_open_value
@@ -75,32 +77,42 @@
                             if self.use_proxy
                             else f"ws://{self.server_id.ip}:{self.server_id.port}"
                         )
                     )
                     address += f"?v={str(self.magic_value)}"
                     self.connection = await connect(address, close_timeout=0, ping_interval=None)
                     self.connected_time = time.time()
+
+                    if self.on_success is not None:
+                        try:
+                            if asyncio.iscoroutinefunction(self.on_success):
+                                await self.on_success()
+                            else:
+                                self.on_success()
+                        except Exception as e:
+                            self.logger.warning(e)
                     break
+
                 except Exception as exception:
                     print_error = True
 
                     if not isinstance(exception, KeyboardInterrupt):
                         # Run the failure callback
-                        try:
-                            if self.on_failure is not None:
+                        if self.on_failure is not None:
+                            try:
                                 if asyncio.iscoroutinefunction(self.on_failure):
                                     val = await self.on_failure()
                                 else:
                                     val = self.on_failure()
 
                                 if val is not None:
                                     print_error = val
 
-                        except Exception as e:
-                            self.logger.warning(e)
+                            except Exception as e:
+                                self.logger.warning(e)
 
                     if print_error:
                         self.logger.warning(
                             f"{datetime.now().strftime('%d/%m/%Y %H:%M:%S')} "
                             f"[RustPlus.py] Cannot Connect to server. Retrying in {str(self.delay)} second/s"
                         )
                     attempts += 1
@@ -144,15 +156,15 @@
             return await self.send_message(message)
 
     async def run(self) -> None:
         while self.connection_status == CONNECTED:
             try:
                 data = await self.connection.recv()
 
-                await EventHandler.run_proto_event(data, self.server_id)
+                await self.run_coroutine_non_blocking(EventHandler.run_proto_event(data, self.server_id))
 
                 app_message = AppMessage()
                 app_message.parse(
                     base64.b64decode(data) if self.use_test_server else data
                 )
 
             except Exception as e:
@@ -180,34 +192,34 @@
             str(app_message.broadcast.team_message.message.message)
         )
 
         if prefix is not None:
             # This means it is a command
 
             message = RustChatMessage(app_message.broadcast.team_message.message)
-            await self.remote.command_handler.run_command(message, prefix)
+            await self.run_coroutine_non_blocking(self.remote.command_handler.run_command(message, prefix))
 
         if self.is_entity_broadcast(app_message):
             # This means that an entity has changed state
 
-            await EventHandler.run_entity_event(
+            await self.run_coroutine_non_blocking(EventHandler.run_entity_event(
                 app_message.broadcast.entity_changed.entity_id,
                 app_message,
                 self.server_id,
-            )
+            ))
 
         elif self.is_camera_broadcast(app_message):
             if self.remote.camera_manager is not None:
-                await self.remote.camera_manager.add_packet(
+                await self.run_coroutine_non_blocking(self.remote.camera_manager.add_packet(
                     RayPacket(app_message.broadcast.camera_rays)
-                )
+                ))
 
         elif self.is_team_broadcast(app_message):
             # This means that the team of the current player has changed
-            await EventHandler.run_team_event(app_message, self.server_id)
+            await self.run_coroutine_non_blocking(EventHandler.run_team_event(app_message, self.server_id))
 
         elif self.is_message(app_message):
             # This means that a message has been sent to the team chat
 
             steam_id = int(app_message.broadcast.team_message.message.steam_id)
             message = str(app_message.broadcast.team_message.message.message)
 
@@ -215,34 +227,34 @@
             if self.remote.conversation_factory.has_conversation(steam_id):
                 if message not in self.outgoing_conversation_messages:
                     conversation: Conversation = (
                         self.remote.conversation_factory.get_conversation(steam_id)
                     )
 
                     conversation.get_answers().append(message)
-                    await conversation.get_current_prompt().on_response(message)
+                    await self.run_coroutine_non_blocking(conversation.get_current_prompt().on_response(message))
 
                     if conversation.has_next():
                         conversation.increment_prompt()
                         prompt = conversation.get_current_prompt()
                         prompt_string = await prompt.prompt()
-                        await conversation.send_prompt(prompt_string)
+                        await self.run_coroutine_non_blocking(conversation.send_prompt(prompt_string))
 
                     else:
                         prompt = conversation.get_current_prompt()
                         prompt_string = await prompt.on_finish()
                         if prompt_string != "":
-                            await conversation.send_prompt(prompt_string)
+                            await self.run_coroutine_non_blocking(conversation.send_prompt(prompt_string))
                         self.remote.conversation_factory.abort_conversation(steam_id)
                 else:
                     self.outgoing_conversation_messages.remove(message)
 
                 # Conversation API end
 
-            await EventHandler.run_chat_event(app_message, self.server_id)
+            await self.run_coroutine_non_blocking(EventHandler.run_chat_event(app_message, self.server_id))
 
         else:
             # This means that it wasn't sent by the server and is a message from the server in response to an action
             event: YieldingEvent = self.remote.pending_response_events[
                 app_message.response.seq
             ]
             event.set_with_value(app_message)
@@ -303,7 +315,12 @@
 
     @staticmethod
     def error_present(message) -> bool:
         """
         Checks message for error
         """
         return message != ""
+
+    @staticmethod
+    async def run_coroutine_non_blocking(coroutine: Coroutine) -> None:
+        loop: AbstractEventLoop = asyncio.get_event_loop_policy().get_event_loop()
+        loop.create_task(coroutine)
```

### Comparing `rustplus-5.6.4/rustplus/api/remote/server_checker.py` & `rustplus-5.6.5/rustplus/api/remote/server_checker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/rust_api.py` & `rustplus-5.6.5/rustplus/api/rust_api.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_chat_message.py` & `rustplus-5.6.5/rustplus/api/structures/rust_chat_message.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_contents.py` & `rustplus-5.6.5/rustplus/api/structures/rust_contents.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_entity_info.py` & `rustplus-5.6.5/rustplus/api/structures/rust_entity_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_info.py` & `rustplus-5.6.5/rustplus/api/structures/rust_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_item.py` & `rustplus-5.6.5/rustplus/api/structures/rust_item.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_map.py` & `rustplus-5.6.5/rustplus/api/structures/rust_map.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_marker.py` & `rustplus-5.6.5/rustplus/api/structures/rust_marker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_team_info.py` & `rustplus-5.6.5/rustplus/api/structures/rust_team_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/api/structures/rust_time.py` & `rustplus-5.6.5/rustplus/api/structures/rust_time.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/commands/command.py` & `rustplus-5.6.5/rustplus/commands/command.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/commands/command_data.py` & `rustplus-5.6.5/rustplus/commands/command_data.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/commands/command_handler.py` & `rustplus-5.6.5/rustplus/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/conversation/conversation.py` & `rustplus-5.6.5/rustplus/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/conversation/conversation_factory.py` & `rustplus-5.6.5/rustplus/conversation/conversation_factory.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/exceptions/exceptions.py` & `rustplus-5.6.5/rustplus/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/utils/deprecated.py` & `rustplus-5.6.5/rustplus/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/utils/fonts/PermanentMarker.ttf` & `rustplus-5.6.5/rustplus/utils/fonts/PermanentMarker.ttf`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/utils/grab_items.py` & `rustplus-5.6.5/rustplus/utils/grab_items.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/utils/rust_utils.py` & `rustplus-5.6.5/rustplus/utils/rust_utils.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/utils/server_id.py` & `rustplus-5.6.5/rustplus/utils/server_id.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus/utils/yielding_event.py` & `rustplus-5.6.5/rustplus/utils/yielding_event.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/rustplus.egg-info/PKG-INFO` & `rustplus-5.6.5/rustplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.6.4
+Version: 5.6.5
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.6.4/rustplus.egg-info/SOURCES.txt` & `rustplus-5.6.5/rustplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.4/setup.py` & `rustplus-5.6.5/setup.py`

 * *Files identical despite different names*

