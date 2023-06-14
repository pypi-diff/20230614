# Comparing `tmp/mrtutils-0.3.8.tar.gz` & `tmp/mrtutils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrtutils-0.3.8.tar", last modified: Tue Mar 21 16:41:21 2023, max compression
+gzip compressed data, was "mrtutils-0.3.9.tar", last modified: Thu Mar 30 03:13:45 2023, max compression
```

## Comparing `mrtutils-0.3.8.tar` & `mrtutils-0.3.9.tar`

### file list

```diff
@@ -1,86 +1,92 @@
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:21.550651 mrtutils-0.3.8/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3676 2023-03-21 16:41:21.547837 mrtutils-0.3.8/PKG-INFO
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2818 2022-10-11 13:12:35.000000 mrtutils-0.3.8/README.rst
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:19.809247 mrtutils-0.3.8/mrtutils/
--rwxrwxrwx   0 jason     (1000) jason     (1000)      313 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/__init__.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)    26284 2022-10-11 16:28:31.000000 mrtutils-0.3.8/mrtutils/device.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)    17526 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/gatt_profile.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)   105249 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/menuconfig.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)    18433 2023-03-21 16:34:55.000000 mrtutils-0.3.8/mrtutils/modsync.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)     7851 2023-03-03 03:34:37.000000 mrtutils-0.3.8/mrtutils/mrt-ble
--rwxrwxrwx   0 jason     (1000) jason     (1000)     5232 2023-03-08 15:30:05.000000 mrtutils-0.3.8/mrtutils/mrt-config
--rwxrwxrwx   0 jason     (1000) jason     (1000)     4171 2022-10-11 16:41:23.000000 mrtutils-0.3.8/mrtutils/mrt-config-gui
--rwxrwxrwx   0 jason     (1000) jason     (1000)     4947 2022-10-11 16:28:31.000000 mrtutils-0.3.8/mrtutils/mrt-device
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2631 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/mrt-doc
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3577 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/mrt-gen
--rwxrwxrwx   0 jason     (1000) jason     (1000)     9432 2023-03-21 16:40:40.000000 mrtutils-0.3.8/mrtutils/mrt-version
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3059 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/mrtDocHelper.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)     4814 2023-03-03 03:34:37.000000 mrtutils-0.3.8/mrtutils/mrtTemplateHelper.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1969 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/mrtYamlHelper.py
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:19.462884 mrtutils-0.3.8/mrtutils/templates/
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:20.244233 mrtutils-0.3.8/mrtutils/templates/ble/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2508 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/app_service_source.c
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:20.491182 mrtutils-0.3.8/mrtutils/templates/ble/esp32/
--rwxrwxrwx   0 jason     (1000) jason     (1000)      381 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/esp32/CMakeLists.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)      391 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/esp32/component.mk
--rwxrwxrwx   0 jason     (1000) jason     (1000)    13953 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/esp32/gatt_server.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3533 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/esp32/gatt_server.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)      302 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/esp32/kconfig
--rwxrwxrwx   0 jason     (1000) jason     (1000)     5621 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/gatt_descriptor_template.yml
--rwxrwxrwx   0 jason     (1000) jason     (1000)     4732 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/gatt_icd.html
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3747 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/gatt_icd.rst
--rwxrwxrwx   0 jason     (1000) jason     (1000)      390 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/nrf_definitions.json
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1179 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/profile_header.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1311 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/profile_source.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3558 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/service_header.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3751 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/service_source.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)    30537 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/ble/smart_icd.html
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:20.753242 mrtutils-0.3.8/mrtutils/templates/device/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2131 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/device/device_descriptor_template.yml
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2996 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/device/device_doc.md
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2341 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/device/device_doc.rst
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2566 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/device/device_header_template.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)    11523 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/device/device_regmap.html
--rwxrwxrwx   0 jason     (1000) jason     (1000)     6283 2022-10-11 16:28:31.000000 mrtutils-0.3.8/mrtutils/templates/device/device_regs_header.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2593 2022-10-11 16:28:31.000000 mrtutils-0.3.8/mrtutils/templates/device/device_slave_header.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3511 2022-10-11 16:28:31.000000 mrtutils-0.3.8/mrtutils/templates/device/device_slave_source.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2151 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/device/device_source_template.c
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:20.956864 mrtutils-0.3.8/mrtutils/templates/doc/
--rwxrwxrwx   0 jason     (1000) jason     (1000)      635 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/Makefile
--rwxrwxrwx   0 jason     (1000) jason     (1000)       34 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/README.rst
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:19.445371 mrtutils-0.3.8/mrtutils/templates/doc/assets/
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:21.111553 mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/
--rwxrwxrwx   0 jason     (1000) jason     (1000)      163 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/button.puml
--rwxrwxrwx   0 jason     (1000) jason     (1000)      699 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/led.puml
--rwxrwxrwx   0 jason     (1000) jason     (1000)    50339 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/mockup.dio.png
--rwxrwxrwx   0 jason     (1000) jason     (1000)    37764 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/system.dio.png
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:21.235043 mrtutils-0.3.8/mrtutils/templates/doc/assets/images/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1150 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/assets/images/favicon.ico
--rwxrwxrwx   0 jason     (1000) jason     (1000)     6636 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/assets/images/logo.png
--rwxrwxrwx   0 jason     (1000) jason     (1000)      488 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/assets/images/remote_button.png
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2398 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/conf.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)      192 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/index.rst
--rwxrwxrwx   0 jason     (1000) jason     (1000)      352 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/layout.html
--rwxrwxrwx   0 jason     (1000) jason     (1000)        0 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/moddoc_index.rst
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:21.268255 mrtutils-0.3.8/mrtutils/templates/doc/pages/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     4010 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/doc/pages/examples.rst
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:21.420764 mrtutils-0.3.8/mrtutils/templates/gen/
--rwxrwxrwx   0 jason     (1000) jason     (1000)      367 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/gen/UT.cpp
--rwxrwxrwx   0 jason     (1000) jason     (1000)      381 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/gen/c.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)      606 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/gen/c.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)      384 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/gen/cpp.cpp
--rwxrwxrwx   0 jason     (1000) jason     (1000)       59 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/templates/gen/mrt.yml
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:21.528360 mrtutils-0.3.8/mrtutils/templates/version/
--rwxrwxrwx   0 jason     (1000) jason     (1000)      351 2023-03-21 02:28:50.000000 mrtutils-0.3.8/mrtutils/templates/version/version.env
--rwxrwxrwx   0 jason     (1000) jason     (1000)      871 2023-03-14 17:18:40.000000 mrtutils-0.3.8/mrtutils/templates/version/version.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)      312 2023-03-14 17:18:25.000000 mrtutils-0.3.8/mrtutils/templates/version/version.json
--rwxrwxrwx   0 jason     (1000) jason     (1000)      456 2023-03-14 17:23:43.000000 mrtutils-0.3.8/mrtutils/templates/version/version.yml
--rwxrwxrwx   0 jason     (1000) jason     (1000)      718 2022-10-11 13:12:35.000000 mrtutils-0.3.8/mrtutils/updates.py
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-21 16:41:19.908515 mrtutils-0.3.8/mrtutils.egg-info/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3676 2023-03-21 16:41:18.000000 mrtutils-0.3.8/mrtutils.egg-info/PKG-INFO
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2476 2023-03-21 16:41:19.000000 mrtutils-0.3.8/mrtutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)        1 2023-03-21 16:41:18.000000 mrtutils-0.3.8/mrtutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)       67 2023-03-21 16:41:18.000000 mrtutils-0.3.8/mrtutils.egg-info/requires.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)        9 2023-03-21 16:41:18.000000 mrtutils-0.3.8/mrtutils.egg-info/top_level.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)       38 2023-03-21 16:41:21.551659 mrtutils-0.3.8/setup.cfg
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1125 2023-03-21 16:41:18.000000 mrtutils-0.3.8/setup.py
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:45.435140 mrtutils-0.3.9/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3676 2023-03-30 03:13:45.433143 mrtutils-0.3.9/PKG-INFO
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2818 2022-10-11 13:12:35.000000 mrtutils-0.3.9/README.rst
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:43.626359 mrtutils-0.3.9/mrtutils/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      313 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/__init__.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    26284 2022-10-11 16:28:31.000000 mrtutils-0.3.9/mrtutils/device.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    17526 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/gatt_profile.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)   105249 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/menuconfig.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    18433 2023-03-21 16:34:55.000000 mrtutils-0.3.9/mrtutils/modsync.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     7851 2023-03-03 03:34:37.000000 mrtutils-0.3.9/mrtutils/mrt-ble
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     5232 2023-03-08 15:30:05.000000 mrtutils-0.3.9/mrtutils/mrt-config
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4171 2022-10-11 16:41:23.000000 mrtutils-0.3.9/mrtutils/mrt-config-gui
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4947 2022-10-11 16:28:31.000000 mrtutils-0.3.9/mrtutils/mrt-device
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2631 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/mrt-doc
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4855 2023-03-30 03:07:31.000000 mrtutils-0.3.9/mrtutils/mrt-gen
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     9432 2023-03-21 16:40:40.000000 mrtutils-0.3.9/mrtutils/mrt-version
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3059 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/mrtDocHelper.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4814 2023-03-03 03:34:37.000000 mrtutils-0.3.9/mrtutils/mrtTemplateHelper.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     1969 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/mrtYamlHelper.py
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:43.284265 mrtutils-0.3.9/mrtutils/templates/
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:44.031035 mrtutils-0.3.9/mrtutils/templates/ble/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2508 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/app_service_source.c
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:44.259703 mrtutils-0.3.9/mrtutils/templates/ble/esp32/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      381 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/esp32/CMakeLists.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      391 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/esp32/component.mk
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    13953 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/esp32/gatt_server.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3533 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/esp32/gatt_server.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      302 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/esp32/kconfig
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     5621 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/gatt_descriptor_template.yml
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4732 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/gatt_icd.html
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3747 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/gatt_icd.rst
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      390 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/nrf_definitions.json
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     1179 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/profile_header.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     1311 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/profile_source.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3558 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/service_header.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3751 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/service_source.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    30537 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/ble/smart_icd.html
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:44.548012 mrtutils-0.3.9/mrtutils/templates/device/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2131 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/device/device_descriptor_template.yml
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2996 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/device/device_doc.md
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2341 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/device/device_doc.rst
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2566 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/device/device_header_template.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    11523 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/device/device_regmap.html
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     6283 2022-10-11 16:28:31.000000 mrtutils-0.3.9/mrtutils/templates/device/device_regs_header.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2593 2022-10-11 16:28:31.000000 mrtutils-0.3.9/mrtutils/templates/device/device_slave_header.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3511 2022-10-11 16:28:31.000000 mrtutils-0.3.9/mrtutils/templates/device/device_slave_source.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2151 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/device/device_source_template.c
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:44.722186 mrtutils-0.3.9/mrtutils/templates/doc/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      635 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/Makefile
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       34 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/README.rst
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:43.252392 mrtutils-0.3.9/mrtutils/templates/doc/assets/
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:44.887449 mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      163 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/button.puml
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      699 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/led.puml
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    50339 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/mockup.dio.png
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    37764 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/system.dio.png
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:45.008576 mrtutils-0.3.9/mrtutils/templates/doc/assets/images/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     1150 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/assets/images/favicon.ico
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     6636 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/assets/images/logo.png
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      488 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/assets/images/remote_button.png
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2398 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/conf.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      192 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/index.rst
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      352 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/layout.html
+-rwxrwxrwx   0 jason     (1000) jason     (1000)        0 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/moddoc_index.rst
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:45.038124 mrtutils-0.3.9/mrtutils/templates/doc/pages/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4010 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/doc/pages/examples.rst
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:45.165455 mrtutils-0.3.9/mrtutils/templates/gen/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      367 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/gen/UT.cpp
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      381 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/gen/c.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      606 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/gen/c.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      384 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/gen/cpp.cpp
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       59 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/templates/gen/mrt.yml
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:45.311735 mrtutils-0.3.9/mrtutils/templates/gen/vue/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      320 2023-03-30 02:55:02.000000 mrtutils-0.3.9/mrtutils/templates/gen/vue/vue-single.vue
+-rwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 02:51:23.000000 mrtutils-0.3.9/mrtutils/templates/gen/vue/vue.css
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       35 2023-03-30 02:50:25.000000 mrtutils-0.3.9/mrtutils/templates/gen/vue/vue.html
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      199 2023-03-30 02:58:44.000000 mrtutils-0.3.9/mrtutils/templates/gen/vue/vue.ts
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      131 2023-03-30 02:51:17.000000 mrtutils-0.3.9/mrtutils/templates/gen/vue/vue.vue
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:45.408033 mrtutils-0.3.9/mrtutils/templates/version/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      351 2023-03-21 02:28:50.000000 mrtutils-0.3.9/mrtutils/templates/version/version.env
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      871 2023-03-14 17:18:40.000000 mrtutils-0.3.9/mrtutils/templates/version/version.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      312 2023-03-14 17:18:25.000000 mrtutils-0.3.9/mrtutils/templates/version/version.json
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      456 2023-03-14 17:23:43.000000 mrtutils-0.3.9/mrtutils/templates/version/version.yml
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      718 2022-10-11 13:12:35.000000 mrtutils-0.3.9/mrtutils/updates.py
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2023-03-30 03:13:43.729411 mrtutils-0.3.9/mrtutils.egg-info/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3676 2023-03-30 03:13:42.000000 mrtutils-0.3.9/mrtutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     2658 2023-03-30 03:13:43.000000 mrtutils-0.3.9/mrtutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)        1 2023-03-30 03:13:42.000000 mrtutils-0.3.9/mrtutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       67 2023-03-30 03:13:42.000000 mrtutils-0.3.9/mrtutils.egg-info/requires.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)        9 2023-03-30 03:13:42.000000 mrtutils-0.3.9/mrtutils.egg-info/top_level.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       38 2023-03-30 03:13:45.436141 mrtutils-0.3.9/setup.cfg
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     1125 2023-03-30 03:13:42.000000 mrtutils-0.3.9/setup.py
```

### Comparing `mrtutils-0.3.8/PKG-INFO` & `mrtutils-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrtutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Utilities for MrT
 Home-page: https://mrt.readthedocs.io/en/latest/index.html
 Author: Jason Berger
 Author-email: JBerger@up-rev.com
 License: UNKNOWN
 Description: 
         MrT Framework
```

### Comparing `mrtutils-0.3.8/README.rst` & `mrtutils-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/device.py` & `mrtutils-0.3.9/mrtutils/device.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/gatt_profile.py` & `mrtutils-0.3.9/mrtutils/gatt_profile.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/menuconfig.py` & `mrtutils-0.3.9/mrtutils/menuconfig.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/modsync.py` & `mrtutils-0.3.9/mrtutils/modsync.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrt-ble` & `mrtutils-0.3.9/mrtutils/mrt-ble`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrt-config` & `mrtutils-0.3.9/mrtutils/mrt-config`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrt-config-gui` & `mrtutils-0.3.9/mrtutils/mrt-config-gui`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrt-device` & `mrtutils-0.3.9/mrtutils/mrt-device`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrt-doc` & `mrtutils-0.3.9/mrtutils/mrt-doc`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrt-version` & `mrtutils-0.3.9/mrtutils/mrt-version`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrtDocHelper.py` & `mrtutils-0.3.9/mrtutils/mrtDocHelper.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrtTemplateHelper.py` & `mrtutils-0.3.9/mrtutils/mrtTemplateHelper.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/mrtYamlHelper.py` & `mrtutils-0.3.9/mrtutils/mrtYamlHelper.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/app_service_source.c` & `mrtutils-0.3.9/mrtutils/templates/ble/app_service_source.c`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/esp32/gatt_server.c` & `mrtutils-0.3.9/mrtutils/templates/ble/esp32/gatt_server.c`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/esp32/gatt_server.h` & `mrtutils-0.3.9/mrtutils/templates/ble/esp32/gatt_server.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/gatt_descriptor_template.yml` & `mrtutils-0.3.9/mrtutils/templates/ble/gatt_descriptor_template.yml`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/gatt_icd.html` & `mrtutils-0.3.9/mrtutils/templates/ble/gatt_icd.html`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/gatt_icd.rst` & `mrtutils-0.3.9/mrtutils/templates/ble/gatt_icd.rst`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/profile_header.h` & `mrtutils-0.3.9/mrtutils/templates/ble/profile_header.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/profile_source.c` & `mrtutils-0.3.9/mrtutils/templates/ble/profile_source.c`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/service_header.h` & `mrtutils-0.3.9/mrtutils/templates/ble/service_header.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/service_source.c` & `mrtutils-0.3.9/mrtutils/templates/ble/service_source.c`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/ble/smart_icd.html` & `mrtutils-0.3.9/mrtutils/templates/ble/smart_icd.html`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_descriptor_template.yml` & `mrtutils-0.3.9/mrtutils/templates/device/device_descriptor_template.yml`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_doc.md` & `mrtutils-0.3.9/mrtutils/templates/device/device_doc.md`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_doc.rst` & `mrtutils-0.3.9/mrtutils/templates/device/device_doc.rst`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_header_template.h` & `mrtutils-0.3.9/mrtutils/templates/device/device_header_template.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_regmap.html` & `mrtutils-0.3.9/mrtutils/templates/device/device_regmap.html`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_regs_header.h` & `mrtutils-0.3.9/mrtutils/templates/device/device_regs_header.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_slave_header.h` & `mrtutils-0.3.9/mrtutils/templates/device/device_slave_header.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_slave_source.c` & `mrtutils-0.3.9/mrtutils/templates/device/device_slave_source.c`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/device/device_source_template.c` & `mrtutils-0.3.9/mrtutils/templates/device/device_source_template.c`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/Makefile` & `mrtutils-0.3.9/mrtutils/templates/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/led.puml` & `mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/led.puml`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/mockup.dio.png` & `mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/mockup.dio.png`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/assets/diagrams/system.dio.png` & `mrtutils-0.3.9/mrtutils/templates/doc/assets/diagrams/system.dio.png`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/assets/images/favicon.ico` & `mrtutils-0.3.9/mrtutils/templates/doc/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/assets/images/logo.png` & `mrtutils-0.3.9/mrtutils/templates/doc/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/conf.py` & `mrtutils-0.3.9/mrtutils/templates/doc/conf.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/doc/pages/examples.rst` & `mrtutils-0.3.9/mrtutils/templates/doc/pages/examples.rst`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/gen/c.h` & `mrtutils-0.3.9/mrtutils/templates/gen/c.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/templates/version/version.h` & `mrtutils-0.3.9/mrtutils/templates/version/version.h`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils/updates.py` & `mrtutils-0.3.9/mrtutils/updates.py`

 * *Files identical despite different names*

### Comparing `mrtutils-0.3.8/mrtutils.egg-info/PKG-INFO` & `mrtutils-0.3.9/mrtutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrtutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Utilities for MrT
 Home-page: https://mrt.readthedocs.io/en/latest/index.html
 Author: Jason Berger
 Author-email: JBerger@up-rev.com
 License: UNKNOWN
 Description: 
         MrT Framework
```

### Comparing `mrtutils-0.3.8/mrtutils.egg-info/SOURCES.txt` & `mrtutils-0.3.9/mrtutils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -60,11 +60,16 @@
 mrtutils/templates/doc/assets/images/remote_button.png
 mrtutils/templates/doc/pages/examples.rst
 mrtutils/templates/gen/UT.cpp
 mrtutils/templates/gen/c.c
 mrtutils/templates/gen/c.h
 mrtutils/templates/gen/cpp.cpp
 mrtutils/templates/gen/mrt.yml
+mrtutils/templates/gen/vue/vue-single.vue
+mrtutils/templates/gen/vue/vue.css
+mrtutils/templates/gen/vue/vue.html
+mrtutils/templates/gen/vue/vue.ts
+mrtutils/templates/gen/vue/vue.vue
 mrtutils/templates/version/version.env
 mrtutils/templates/version/version.h
 mrtutils/templates/version/version.json
 mrtutils/templates/version/version.yml
```

### Comparing `mrtutils-0.3.8/setup.py` & `mrtutils-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
      name='mrtutils',
-     version="0.3.8",
+     version="0.3.9",
      author="Jason Berger",
      author_email="JBerger@up-rev.com",
      description="Utilities for MrT",
      long_description=long_description,
      scripts=['mrtutils/mrt-config','mrtutils/mrt-device', 'mrtutils/mrt-ble', 'mrtutils/mrt-config-gui','mrtutils/mrt-doc', 'mrtutils/mrt-version','mrtutils/mrt-gen'],
      long_description_content_type="text/x-rst",
      url="https://mrt.readthedocs.io/en/latest/index.html",
```

