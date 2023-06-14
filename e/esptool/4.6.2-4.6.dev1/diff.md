# Comparing `tmp/esptool-4.6.2.tar.gz` & `tmp/esptool-4.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esptool-4.6.2.tar", last modified: Wed Jun 14 08:15:44 2023, max compression
+gzip compressed data, was "dist/esptool-4.6.dev1.tar", last modified: Mon Mar 27 16:51:19 2023, max compression
```

## Comparing `esptool-4.6.2.tar` & `esptool-4.6.dev1.tar`

### file list

```diff
@@ -1,131 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 08:15:33.000000 esptool-4.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-14 08:15:33.000000 esptool-4.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-14 08:15:44.000000 esptool-4.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-14 08:15:33.000000 esptool-4.6.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     9762 2023-06-14 08:15:33.000000 esptool-4.6.2/esp_rfc2217_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9718 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30777 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    27177 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/base_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/emulate_efuse_controller_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32c2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32c3/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c3/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c3/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c3/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32c6/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c6/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c6/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c6/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32c6/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32h2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18561 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32h2beta1/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2beta1/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2beta1/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32h2beta1/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32s2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32s3/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse/esp32s3beta2/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3beta2/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3beta2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/esp32s3beta2/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/mem_definition_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espefuse/efuse_defs/
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse_defs/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse_defs/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33961 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse_defs/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33534 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse_defs/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29352 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse_defs/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35820 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse_defs/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    40280 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse/efuse_defs/esp32s3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-06-14 08:15:33.000000 esptool-4.6.2/espefuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espsecure/
--rwxr-xr-x   0 runner    (1001) docker     (123)    63263 2023-06-14 08:15:33.000000 esptool-4.6.2/espsecure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-14 08:15:33.000000 esptool-4.6.2/espsecure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/espsecure/esp_hsm_sign/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-14 08:15:33.000000 esptool-4.6.2/espsecure/esp_hsm_sign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-14 08:15:33.000000 esptool-4.6.2/espsecure/esp_hsm_sign/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1185 2023-06-14 08:15:33.000000 esptool-4.6.2/espsecure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool/
--rw-r--r--   0 runner    (1001) docker     (123)    36822 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46660 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/bin_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    47212 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    60941 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool/targets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32c2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32c3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32c6.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32c6beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32h2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32h2beta1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32h2beta2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32s2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp32s3beta2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/esp8266.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool/targets/stub_flasher/
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32.json
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c6.json
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c6beta.json
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32h2.json
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32s2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32s3.json
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_8266.json
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 08:15:44.000000 esptool-4.6.2/esptool.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-06-14 08:15:33.000000 esptool-4.6.2/esptool.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-14 08:15:44.000000 esptool-4.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-14 08:15:33.000000 esptool-4.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/
+-rw-rw-rw-   0 root         (0) root         (0)    18092 2023-03-27 11:04:17.000000 esptool-4.6.dev1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-03-27 11:04:17.000000 esptool-4.6.dev1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-03-27 16:51:19.000000 esptool-4.6.dev1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-03-27 11:04:17.000000 esptool-4.6.dev1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     9762 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esp_rfc2217_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/
+-rwxrwxrwx   0 root         (0) root         (0)     9431 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30121 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/base_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    25744 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/base_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     8747 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/emulate_efuse_controller_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5250 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18032 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    10833 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12519 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    15486 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11557 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12287 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c2/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18304 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    20780 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14960 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c3/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18299 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    22114 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14955 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32c6/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3015 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18498 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    21925 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    15383 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3050 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    18149 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    20202 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14979 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    20851 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    23423 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    18946 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s2/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    19340 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    22508 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    18946 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    19354 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    21654 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/mem_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    18953 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/mem_definition_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse/efuse/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espefuse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espsecure/
+-rwxrwxrwx   0 root         (0) root         (0)    62428 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/espsecure/esp_hsm_sign/
+-rw-rw-rw-   0 root         (0) root         (0)     5505 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/esp_hsm_sign/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure/esp_hsm_sign/exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)     1094 2023-03-27 11:04:17.000000 esptool-4.6.dev1/espsecure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool/
+-rw-rw-rw-   0 root         (0) root         (0)    35233 2023-03-27 16:51:18.000000 esptool-4.6.dev1/esptool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46489 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/bin_image.py
+-rw-rw-rw-   0 root         (0) root         (0)    45474 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/cmds.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    60747 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5743 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/reset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool/targets/
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13506 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32.py
+-rw-rw-rw-   0 root         (0) root         (0)     5735 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c6.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32c6beta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1884 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32h2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32h2beta1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32h2beta2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10606 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32s2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11158 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp32s3beta2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5970 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/esp8266.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/
+-rw-rw-rw-   0 root         (0) root         (0)     4883 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32.json
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c2.json
+-rw-rw-rw-   0 root         (0) root         (0)     5291 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c3.json
+-rw-rw-rw-   0 root         (0) root         (0)     5231 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6.json
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6beta.json
+-rw-rw-rw-   0 root         (0) root         (0)     5231 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2.json
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json
+-rw-rw-rw-   0 root         (0) root         (0)     6119 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s2.json
+-rw-rw-rw-   0 root         (0) root         (0)     7155 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s3.json
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json
+-rw-rw-rw-   0 root         (0) root         (0)    12119 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_8266.json
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-03-27 16:51:19.000000 esptool-4.6.dev1/esptool.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1084 2023-03-27 11:04:17.000000 esptool-4.6.dev1/esptool.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-03-27 16:51:19.000000 esptool-4.6.dev1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4254 2023-03-27 11:04:17.000000 esptool-4.6.dev1/setup.py
```

### Comparing `esptool-4.6.2/LICENSE` & `esptool-4.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/PKG-INFO` & `esptool-4.6.dev1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 Metadata-Version: 2.1
 Name: esptool
-Version: 4.6.2
+Version: 4.6.dev1
 Summary: A serial utility to communicate & flash code to Espressif chips.
 Home-page: https://github.com/espressif/esptool/
 Author: Fredrik Ahlberg (themadinventor) & Angus Gratton (projectgus) & Espressif Systems
 Author-email: 
 License: GPLv2+
 Project-URL: Documentation, https://docs.espressif.com/projects/esptool/
 Project-URL: Source, https://github.com/espressif/esptool/
 Project-URL: Tracker, https://github.com/espressif/esptool/issues/
-Description: 
-        ==========
-        esptool.py
-        ==========
-        A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
-        
-        The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
-        
-        Documentation
-        -------------
-        Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
-        
-        Contributing
-        ------------
-        Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -38,7 +22,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: hsm
+License-File: LICENSE
+
+
+==========
+esptool.py
+==========
+A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
+
+The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
+
+Documentation
+-------------
+Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
+
+Contributing
+------------
+Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
+
+
```

### Comparing `esptool-4.6.2/README.md` & `esptool-4.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/esp_rfc2217_server.py` & `esptool-4.6.dev1/esp_rfc2217_server.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse/__init__.py` & `esptool-4.6.dev1/espefuse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,29 +128,23 @@
             cmd = []
         cmd.append(item)
     if cmd:
         groups.append(cmd)
     return groups, used_cmds
 
 
-def main(custom_commandline=None, esp=None):
+def main(custom_commandline=None):
     """
     Main function for espefuse
 
     custom_commandline - Optional override for default arguments parsing
     (that uses sys.argv), can be a list of custom arguments as strings.
     Arguments and their values need to be added as individual items to the list
     e.g. "--port /dev/ttyUSB1" thus becomes ['--port', '/dev/ttyUSB1'].
-
-    esp - Optional override of the connected device previously
-    returned by esptool.get_default_connected_device()
     """
-
-    external_esp = esp is not None
-
     init_parser = argparse.ArgumentParser(
         description="espefuse.py v%s - [ESP32xx] efuse get/set tool"
         % esptool.__version__,
         prog="espefuse",
         add_help=False,
     )
 
@@ -213,32 +207,30 @@
     debug_mode = common_args.debug or ("dump" in remaining_args)
     just_print_help = [
         True for arg in remaining_args if arg in ["--help", "-h"]
     ] or remaining_args == []
 
     print("espefuse.py v{}".format(esptool.__version__))
 
-    if not external_esp:
-        try:
-            esp = get_esp(
-                common_args.port,
-                common_args.baud,
-                common_args.before,
-                common_args.chip,
-                just_print_help,
-                common_args.virt,
-                common_args.debug,
-                common_args.path_efuse_file,
-            )
-        except esptool.FatalError as e:
-            raise esptool.FatalError(
-                f"{e}\nPlease make sure that you have specified "
-                "the right port with the --port argument"
-            )
-            # TODO: Require the --port argument in the next major release, ESPTOOL-490
+    try:
+        esp = get_esp(
+            common_args.port,
+            common_args.baud,
+            common_args.before,
+            common_args.chip,
+            just_print_help,
+            common_args.virt,
+            common_args.debug,
+            common_args.path_efuse_file,
+        )
+    except esptool.FatalError as e:
+        raise esptool.FatalError(
+            f"{e}\nPlease make sure that you have specified "
+            "the right port with the --port argument"
+        )  # TODO: Require the --port argument in the next major release, ESPTOOL-490
 
     efuses, efuse_operations = get_efuses(
         esp, just_print_help, debug_mode, common_args.do_not_confirm
     )
 
     parser = argparse.ArgumentParser(parents=[init_parser])
     subparsers = parser.add_subparsers(
@@ -280,15 +272,15 @@
             operation_func(esp, efuses, args)
 
         if there_are_multiple_burn_commands_in_args:
             efuses.batch_mode_cnt -= 1
             if not efuses.burn_all(check_batch_mode=True):
                 raise esptool.FatalError("BURN was not done")
     finally:
-        if not external_esp and not common_args.virt and esp._port:
+        if not common_args.virt and esp._port:
             esp._port.close()
 
 
 def _main():
     try:
         main()
     except esptool.FatalError as e:
```

### Comparing `esptool-4.6.2/espefuse/efuse/base_fields.py` & `esptool-4.6.dev1/espefuse/efuse/base_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file describes the common eFuses structures for chips
 #
 # SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
+import re
 import sys
 
 from bitstring import BitArray, BitStream, CreationError
 
 import esptool
 
 from . import util
@@ -546,18 +547,14 @@
             if not self.force_write_always:
                 error_msg += "(use '--force-write-always' option to ignore it)"
         if self.force_write_always:
             print(error_msg, "Skipped because '--force-write-always' option.")
         else:
             raise esptool.FatalError(error_msg)
 
-    def get_block_errors(self, block_num):
-        """Returns (error count, failure boolean flag)"""
-        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
-
 
 class EfuseFieldBase(EfuseProtectBase):
     def __init__(self, parent, param):
         self.category = param.category
         self.parent = parent
         self.block = param.block
         self.word = param.word
@@ -565,25 +562,27 @@
         self.write_disable_bit = param.write_disable_bit
         self.read_disable_bit = param.read_disable_bit
         self.name = param.name
         self.efuse_class = param.class_type
         self.efuse_type = param.type
         self.description = param.description
         self.dict_value = param.dictionary
-        self.bit_len = param.bit_len
-        self.alt_names = param.alt_names
         self.fail = False
         self.num_errors = 0
-        self.bitarray = BitStream(self.bit_len)
+        if self.efuse_type.startswith("bool"):
+            field_len = 1
+        else:
+            field_len = int(re.search(r"\d+", self.efuse_type).group())
+            if self.efuse_type.startswith("bytes"):
+                field_len *= 8
+        self.bitarray = BitStream(field_len)
+        self.bit_len = field_len
         self.bitarray.set(0)
         self.update(self.parent.blocks[self.block].bitarray)
 
-    def is_field_calculated(self):
-        return self.word is None or self.pos is None
-
     def check_format(self, new_value_str):
         if new_value_str is None:
             return new_value_str
         else:
             if self.efuse_type.startswith("bytes"):
                 if new_value_str.startswith("0x"):
                     # cmd line: 0x0102030405060708 .... 112233ff      (hex)
@@ -668,18 +667,16 @@
 
     def save(self, new_value):
         bitarray_field = self.convert_to_bitstring(new_value)
         self.check_new_value(bitarray_field)
         self.save_to_block(bitarray_field)
 
     def update(self, bit_array_block):
-        if self.is_field_calculated():
-            self.bitarray.overwrite(
-                self.convert_to_bitstring(self.check_format(self.get())), pos=0
-            )
+        if self.word is None or self.pos is None:
+            self.bitarray.overwrite(self.convert_to_bitstring(self.get()), pos=0)
             return
         field_len = self.bitarray.len
         bit_array_block.pos = bit_array_block.length - (
             self.word * 32 + self.pos + field_len
         )
         self.bitarray.overwrite(bit_array_block.read(field_len), pos=0)
         err_bitarray = self.parent.blocks[self.block].err_bitarray
@@ -733,22 +730,7 @@
             )
             return block.wr_bitarray.read(self.bitarray.len)
 
     def burn(self, new_value):
         # Burn a efuse. Added for compatibility reason.
         self.save(new_value)
         self.parent.burn_all()
-
-    def get_info(self):
-        output = f"{self.name} (BLOCK{self.block})"
-        if self.block == 0:
-            if self.fail:
-                output += "[error]"
-        else:
-            errs, fail = self.parent.get_block_errors(self.block)
-            if errs != 0 or fail:
-                output += "[error]"
-        if self.efuse_class == "keyblock":
-            name = self.parent.blocks[self.block].key_purpose_name
-            if name is not None:
-                output += f"\n  Purpose: {self.parent[name].get()}\n "
-        return output
```

### Comparing `esptool-4.6.2/espefuse/efuse/base_operations.py` & `esptool-4.6.dev1/espefuse/efuse/base_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,53 +67,38 @@
         "name_value_pairs",
         help="Name of efuse register and New value pairs to burn",
         action=ActionEfuseValuePair,
         nargs="+",
         metavar="[EFUSE_NAME VALUE] [{} VALUE".format(
             " VALUE] [".join([e.name for e in efuses.efuses])
         ),
-        efuse_choices=[e.name for e in efuses.efuses]
-        + [name for e in efuses.efuses for name in e.alt_names if name != ""],
+        efuse_choices=[e.name for e in efuses.efuses],
         efuses=efuses,
     )
 
     read_protect_efuse = subparsers.add_parser(
         "read_protect_efuse",
         help="Disable readback for the efuse with the specified name",
     )
     read_protect_efuse.add_argument(
         "efuse_name",
         help="Name of efuse register to burn",
         nargs="+",
-        choices=[e.name for e in efuses.efuses if e.read_disable_bit is not None]
-        + [
-            name
-            for e in efuses.efuses
-            if e.read_disable_bit is not None
-            for name in e.alt_names
-            if name != ""
-        ],
+        choices=[e.name for e in efuses.efuses if e.read_disable_bit is not None],
     )
 
     write_protect_efuse = subparsers.add_parser(
         "write_protect_efuse",
         help="Disable writing to the efuse with the specified name",
     )
     write_protect_efuse.add_argument(
         "efuse_name",
         help="Name of efuse register to burn",
         nargs="+",
-        choices=[e.name for e in efuses.efuses if e.write_disable_bit is not None]
-        + [
-            name
-            for e in efuses.efuses
-            if e.write_disable_bit is not None
-            for name in e.alt_names
-            if name != ""
-        ],
+        choices=[e.name for e in efuses.efuses if e.write_disable_bit is not None],
     )
 
     burn_block_data = subparsers.add_parser(
         "burn_block_data",
         help="Burn non-key data to EFUSE blocks. "
         "(Don't use this command to burn key data for Flash Encryption or "
         "ESP32 Secure Boot V1, as the byte order of keys is swapped (use burn_key)).",
@@ -679,53 +664,30 @@
     block.save(data_block.bytes[::-1])
 
     if not efuses.burn_all(check_batch_mode=True):
         return
     print("Successful")
 
 
-def get_error_summary(efuses):
-    error_in_blocks = efuses.get_coding_scheme_warnings()
-    if not error_in_blocks:
-        return False
-    writable = True
-    for blk in efuses.blocks:
-        if blk.fail or blk.num_errors:
-            if blk.id == 0:
-                for field in efuses:
-                    if field.block == blk.id and (field.fail or field.num_errors):
-                        wr = "writable" if field.is_writeable() else "not writable"
-                        writable &= wr == "writable"
-                        name = field.name
-                        val = field.get()
-                        print(f"BLOCK{field.block:<2}: {name:<40} = {val:<8} ({wr})")
-            else:
-                wr = "writable" if blk.is_writeable() else "not writable"
-                writable &= wr == "writable"
-                name = f"{blk.name} [ERRORS:{blk.num_errors} FAIL:{int(blk.fail)}]"
-                val = str(blk.get_bitstring())
-                print(f"BLOCK{blk.id:<2}: {name:<40} = {val:<8} ({wr})")
-    if not writable and error_in_blocks:
-        print("Not all errors can be fixed because some fields are write-protected!")
-    return True
-
-
 def check_error(esp, efuses, args):
-    error_in_blocks = get_error_summary(efuses)
-    if args.recovery and error_in_blocks:
-        confirmed = False
-        for block in reversed(efuses.blocks):
-            if block.fail or block.num_errors > 0:
-                if not block.get_bitstring().all(False):
-                    block.save(block.get_bitstring().bytes[::-1])
-                    if not confirmed:
-                        confirmed = True
-                        efuses.confirm(
-                            "Recovery of block coding errors", args.do_not_confirm
-                        )
-                    block.burn()
-        if confirmed:
-            efuses.update_efuses()
-        error_in_blocks = get_error_summary(efuses)
-    if error_in_blocks:
-        raise esptool.FatalError("Error(s) were detected in eFuses")
+    error_in_blocks = efuses.get_coding_scheme_warnings()
+    if args.recovery:
+        if error_in_blocks:
+            confirmed = False
+            for block in reversed(efuses.blocks):
+                if block.fail or block.num_errors > 0:
+                    if not block.get_bitstring().all(False):
+                        block.save(block.get_bitstring().bytes[::-1])
+                        if not confirmed:
+                            confirmed = True
+                            efuses.confirm(
+                                "Recovery of block coding errors", args.do_not_confirm
+                            )
+                        block.burn()
+            # Reset the recovery flag to run check_error() without it,
+            # just to check the new state of eFuse blocks.
+            args.recovery = False
+            check_error(esp, efuses, args)
+    else:
+        if error_in_blocks:
+            raise esptool.FatalError("Error(s) were detected in eFuses")
     print("No errors detected")
```

### Comparing `esptool-4.6.2/espefuse/efuse/emulate_efuse_controller_base.py` & `esptool-4.6.dev1/espefuse/efuse/emulate_efuse_controller_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,15 +105,16 @@
         for b in self.Blocks.BLOCKS:
             blk = self.Blocks.get(b)
             for offset in range(0, blk.len * 4, 4):
                 wr_addr = blk.wr_addr + offset
                 self.write_reg(wr_addr, 0)
 
     def read_field(self, name, bitstring=True):
-        for field in self.Fields.EFUSES:
+        for e in self.Fields.EFUSES:
+            field = self.Fields.get(e)
             if field.name == name:
                 self.read_block(field.block)
                 block = self.read_block(field.block)
                 if field.type.startswith("bool"):
                     field_len = 1
                 else:
                     field_len = int(re.search(r"\d+", field.type).group())
@@ -161,15 +162,16 @@
         mask_wr_data.set(0)
         blk = self.Blocks.get(self.Blocks.BLOCKS[num_blk])
         if blk.write_disable_bit is not None and write_disable_bit & (
             1 << blk.write_disable_bit
         ):
             mask_wr_data.set(1)
         else:
-            for field in self.Fields.EFUSES:
+            for e in self.Fields.EFUSES:
+                field = self.Fields.get(e)
                 if blk.id == field.block and field.block == num_blk:
                     if field.write_disable_bit is not None and write_disable_bit & (
                         1 << field.write_disable_bit
                     ):
                         data = self.read_field(field.name)
                         data.set(1)
                         mask_wr_data.pos = mask_wr_data.length - (
@@ -187,15 +189,16 @@
             blk = self.Blocks.get(b)
             block = self.read_block(blk.id)
             if blk.read_disable_bit is not None and read_disable_bit & (
                 1 << blk.read_disable_bit
             ):
                 block.set(0)
             else:
-                for field in self.Fields.EFUSES:
+                for e in self.Fields.EFUSES:
+                    field = self.Fields.get(e)
                     if (
                         blk.id == field.block
                         and field.read_disable_bit is not None
                         and read_disable_bit & (1 << field.read_disable_bit)
                     ):
                         raw_data = self.read_field(field.name)
                         raw_data.set(0)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32/emulate_efuse_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operations. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
 
     """ esptool method start >> """
 
     def get_major_chip_version(self):
         return 3
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32/fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,102 +61,132 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS_256
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.KEYBLOCKS_256
             ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CUSTOM_MAC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CUSTOM_MAC
             ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.ADC_CALIBRATION
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.ADC_CALIBRATION
             ]
         else:
             if self.coding_scheme == self.REGS.CODING_SCHEME_NONE:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.KEYBLOCKS_256
                 ]
             elif self.coding_scheme == self.REGS.CODING_SCHEME_34:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.KEYBLOCKS_192
                 ]
             else:
                 raise esptool.FatalError(
                     "The coding scheme (%d) - is not supported" % self.coding_scheme
                 )
             if self["MAC_VERSION"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse) for efuse in self.Fields.CUSTOM_MAC
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
+                    for efuse in self.Fields.CUSTOM_MAC
                 ]
             if self["BLK3_PART_RESERVE"].get():
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.ADC_CALIBRATION
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.CUSTOM_MAC:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse) for efuse in self.Fields.CUSTOM_MAC
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
+                    for efuse in self.Fields.CUSTOM_MAC
                 ]
                 new_fields = True
         for efuse in self.Fields.ADC_CALIBRATION:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.ADC_CALIBRATION
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = (
             self.read_efuse(self.REGS.EFUSE_CODING_SCHEME_WORD)
             & self.REGS.EFUSE_CODING_SCHEME_MASK
@@ -229,35 +259,39 @@
                 )
         if (self.debug or err) and not silent:
             self.print_status_regs()
         return err != 0
 
     def summary(self):
         if self["XPD_SDIO_FORCE"].get() == 0:
-            output = "Flash voltage (VDD_SDIO) determined by GPIO12 on reset (High for 1.8V, Low/NC for 3.3V)"
+            output = "Flash voltage (VDD_SDIO) determined by GPIO12 on reset "
+            "(High for 1.8V, Low/NC for 3.3V)."
         elif self["XPD_SDIO_REG"].get() == 0:
             output = "Flash voltage (VDD_SDIO) internal regulator disabled by efuse."
         elif self["XPD_SDIO_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SDIO) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SDIO) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "spipin": EfuseSpiPinField,
             "vref": EfuseVRefField,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
             "pkg": EfusePkg,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        return "%s (BLOCK%d):" % (self.name, self.block)
 
 
 class EfuseMacField(EfuseField):
     """
     Supports: MAC and CUSTOM_MAC fields.
     (if MAC_VERSION == 1 then the CUSTOM_MAC is used)
     """
@@ -364,17 +398,15 @@
             # as it's written in the factory.
             raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         rev_bit0 = self.parent["CHIP_VER_REV1"].get(from_read)
-        assert self.parent["CHIP_VER_REV1"].bit_len == 1
         rev_bit1 = self.parent["CHIP_VER_REV2"].get(from_read)
-        assert self.parent["CHIP_VER_REV2"].bit_len == 1
         apb_ctl_date = self.parent.read_reg(self.parent.REGS.APB_CTL_DATE_ADDR)
         rev_bit2 = (
             apb_ctl_date >> self.parent.REGS.APB_CTL_DATE_S
         ) & self.parent.REGS.APB_CTL_DATE_V
         combine_value = (rev_bit2 << 2) | (rev_bit1 << 1) | rev_bit0
 
         revision = {
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c2/emulate_efuse_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-C2"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 1
@@ -120,15 +120,16 @@
                             0, [i for i in range(blk.len * 32 // 2, blk.len * 32)]
                         )
                     if read_disable_bit & (1 << blk.read_disable_bit[1]):
                         block.set(0, [i for i in range(0, blk.len * 32 // 2)])
                 else:
                     block.set(0)
             else:
-                for field in self.Fields.EFUSES:
+                for e in self.Fields.EFUSES:
+                    field = self.Fields.get(e)
                     if (
                         blk.id == field.block
                         and field.read_disable_bit is not None
                         and read_disable_bit & get_read_disable_mask(field)
                     ):
                         raw_data = self.read_field(field.name)
                         raw_data.set(0)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c2/fields.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-C2":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-C2 chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,48 +81,61 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MINOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -129,14 +143,18 @@
         self.blocks[0].print_block(self.blocks[0].err_bitarray, "err__regs", debug=True)
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -216,21 +234,14 @@
         # Configure clock
         xtal_freq = self.get_crystal_freq()
         if xtal_freq not in [26, 40]:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=26M and 40M (xtal was %d)" % xtal_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
         tpgm_inactive_val = 200 if xtal_freq == 40 else 130
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF0_REG,
@@ -245,17 +256,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR_REG + offs * 4)
                     for offs in range(1)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -278,21 +292,36 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseTempSensor(EfuseField):
     def get(self, from_read=True):
         value = self.get_bitstring(from_read)
         sig = -1 if value[0] else 1
         return sig * value[1:].uint * 0.1
@@ -360,18 +389,27 @@
             super(EfuseMacField, self).save(new_value)
         else:
             raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
-        # fmt: off
-        ("USER",                                        0, None),      # User purposes (software-only use)
-        ("XTS_AES_128_KEY",                             1, None),      # (whole 256bits) flash/PSRAM encryption
-        ("XTS_AES_128_KEY_DERIVED_FROM_128_EFUSE_BITS", 2, None),      # (lo 128bits) flash/PSRAM encryption
-        ("SECURE_BOOT_DIGEST",                          3, "DIGEST"),
-        # (hi 128bits) Secure Boot key digest
-        # fmt: on
+        ("USER", 0, None),  # User purposes (software-only use)
+        (
+            "XTS_AES_128_KEY",
+            1,
+            None,
+        ),  # (whole 256bits) XTS_AES_128_KEY (flash/PSRAM encryption)
+        (
+            "XTS_AES_128_KEY_DERIVED_FROM_128_EFUSE_BITS",
+            2,
+            None,
+        ),  # (lo 128bits) XTS_AES_128_KEY (flash/PSRAM encryption)
+        (
+            "SECURE_BOOT_DIGEST",
+            3,
+            "DIGEST",
+        ),  # (hi 128bits)SECURE_BOOT_DIGEST (Secure Boot key digest)
     ]
 
     KEY_PURPOSES_NAME = [name[0] for name in KEY_PURPOSES]
     DIGEST_KEY_PURPOSES = [name[0] for name in KEY_PURPOSES if name[2] == "DIGEST"]
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c3/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# This file describes eFuses controller for ESP32-C3 chip
+# This file describes eFuses controller for ESP32-H2 chip
 #
-# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import reedsolo
 
 from .mem_definition import EfuseDefineBlocks, EfuseDefineFields, EfuseDefineRegisters
 from ..emulate_efuse_controller_base import EmulateEfuseControllerBase, FatalError
 
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
-    CHIP_NAME = "ESP32-C3"
+    CHIP_NAME = "ESP32-H2"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
 
     def get_minor_chip_version(self):
-        return 4
+        return 0
 
     def get_crystal_freq(self):
-        return 40  # MHz (common for all chips)
+        return 32  # MHz
 
     def get_security_info(self):
         return {
             "flags": 0,
             "flash_crypt_cnt": 0,
             "key_purposes": 0,
             "chip_id": 0,
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c3/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c6/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses for ESP32-C3 chip
+# This file describes eFuses for ESP32-C6 chip
 #
-# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-C3":
+        if esp.CHIP_NAME != "ESP32-C6":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-C3 chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-C6 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -224,37 +245,33 @@
         # Configure clock
         apb_freq = self.get_crystal_freq()
         if apb_freq != 40:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg_f, fail_bit = self.REGS.BLOCK_FAIL_BIT[block.id]
                 if fail_bit is None:
                     block.fail = False
                 else:
@@ -281,30 +298,43 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -425,18 +455,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c3/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c3/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c6/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c6/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-C6"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c6/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses for ESP32-C6 chip
+# This file describes eFuses for ESP32-H2 chip
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2021-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-C6":
+        if esp.CHIP_NAME != "ESP32-H2(beta1)":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-C6 chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-H2(beta1) chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,61 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
-            if self["BLK_VERSION_MINOR"].get() == 1:
+            if self["BLOCK2_VERSION"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
-            self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
-            ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +148,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -219,26 +234,19 @@
                     exit(0)  # finish without errors
             raise
 
     def set_efuse_timing(self):
         """Set timing registers for burning efuses"""
         # Configure clock
         apb_freq = self.get_crystal_freq()
-        if apb_freq != 40:
+        if apb_freq != 32:
             raise esptool.FatalError(
-                "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
+                "The eFuse supports only xtal=32M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         old_addr_reg = 0
@@ -246,17 +254,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -279,34 +290,36 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
-            "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
 
-
-class EfuseWafer(EfuseField):
-    def get(self, from_read=True):
-        hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
-        lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
-        return (hi_bits << 3) + lo_bits
-
-    def save(self, new_value):
-        raise esptool.FatalError("Burning %s is not supported" % self.name)
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseTempSensor(EfuseField):
     def get(self, from_read=True):
         value = self.get_bitstring(from_read)
         sig = -1 if value[0] else 1
         return sig * value[1:].uint * 0.1
@@ -322,55 +335,48 @@
 
 class EfuseMacField(EfuseField):
     def check_format(self, new_value_str):
         if new_value_str is None:
             raise esptool.FatalError(
                 "Required MAC Address in AA:CD:EF:01:02:03 format!"
             )
-        num_bytes = 8 if self.name == "MAC_EUI64" else 6
-        if new_value_str.count(":") != num_bytes - 1:
+        if new_value_str.count(":") != 5:
             raise esptool.FatalError(
-                f"MAC Address needs to be a {num_bytes}-byte hexadecimal format "
+                "MAC Address needs to be a 6-byte hexadecimal format "
                 "separated by colons (:)!"
             )
-        hexad = new_value_str.replace(":", "").split(" ", 1)[0]
-        hexad = hexad.split(" ", 1)[0] if self.is_field_calculated() else hexad
-        if len(hexad) != num_bytes * 2:
+        hexad = new_value_str.replace(":", "")
+        if len(hexad) != 12:
             raise esptool.FatalError(
-                f"MAC Address needs to be a {num_bytes}-byte hexadecimal number "
-                f"({num_bytes * 2} hexadecimal characters)!"
+                "MAC Address needs to be a 6-byte hexadecimal number "
+                "(12 hexadecimal characters)!"
             )
         # order of bytearray = b'\xaa\xcd\xef\x01\x02\x03',
         bindata = binascii.unhexlify(hexad)
-
-        if not self.is_field_calculated():
-            # unicast address check according to
-            # https://tools.ietf.org/html/rfc7042#section-2.1
-            if esptool.util.byte(bindata, 0) & 0x01:
-                raise esptool.FatalError("Custom MAC must be a unicast MAC!")
+        # unicast address check according to
+        # https://tools.ietf.org/html/rfc7042#section-2.1
+        if esptool.util.byte(bindata, 0) & 0x01:
+            raise esptool.FatalError("Custom MAC must be a unicast MAC!")
         return bindata
 
     def check(self):
         errs, fail = self.parent.get_block_errors(self.block)
         if errs != 0 or fail:
             output = "Block%d has ERRORS:%d FAIL:%d" % (self.block, errs, fail)
         else:
             output = "OK"
         return "(" + output + ")"
 
     def get(self, from_read=True):
         if self.name == "CUSTOM_MAC":
-            mac = self.get_raw(from_read)[::-1]
+            mac = self.get_raw(from_read)[::-1] + self.parent["MAC_EXT"].get_raw(
+                from_read
+            )
         elif self.name == "MAC":
-            mac = self.get_raw(from_read)
-        elif self.name == "MAC_EUI64":
-            mac = self.parent["MAC"].get_bitstring(from_read).copy()
-            mac_ext = self.parent["MAC_EXT"].get_bitstring(from_read)
-            mac.insert(mac_ext, 24)
-            mac = mac.bytes
+            mac = self.get_raw(from_read) + self.parent["MAC_EXT"].get_raw(from_read)
         else:
             mac = self.get_raw(from_read)
         return "%s %s" % (util.hexify(mac, ":"), self.check())
 
     def save(self, new_value):
         def print_field(e, new_value):
             print(
@@ -382,32 +388,35 @@
         if self.name == "CUSTOM_MAC":
             bitarray_mac = self.convert_to_bitstring(new_value)
             print_field(self, bitarray_mac)
             super(EfuseMacField, self).save(new_value)
         else:
             # Writing the BLOCK1 (MAC_SPI_8M_0) default MAC is not possible,
             # as it's written in the factory.
-            raise esptool.FatalError(f"Burning {self.name} is not supported")
+            raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 # fmt: off
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
         ("USER",                         0,  None,       None,      "no_need_rd_protect"),   # User purposes (software-only use)
         ("RESERVED",                     1,  None,       None,      "no_need_rd_protect"),   # Reserved
+        ("XTS_AES_256_KEY_1",            2,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_256_KEY_1 (flash/PSRAM encryption)
+        ("XTS_AES_256_KEY_2",            3,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_256_KEY_2 (flash/PSRAM encryption)
         ("XTS_AES_128_KEY",              4,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_128_KEY (flash/PSRAM encryption)
         ("HMAC_DOWN_ALL",                5,  None,       None,      "need_rd_protect"),      # HMAC Downstream mode
         ("HMAC_DOWN_JTAG",               6,  None,       None,      "need_rd_protect"),      # JTAG soft enable key (uses HMAC Downstream mode)
         ("HMAC_DOWN_DIGITAL_SIGNATURE",  7,  None,       None,      "need_rd_protect"),      # Digital Signature peripheral key (uses HMAC Downstream mode)
         ("HMAC_UP",                      8,  None,       None,      "need_rd_protect"),      # HMAC Upstream mode
         ("SECURE_BOOT_DIGEST0",          9,  "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST0 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST1",          10, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST1 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST2",          11, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST2 (Secure Boot key digest)
     ]
 # fmt: on
+
     KEY_PURPOSES_NAME = [name[0] for name in KEY_PURPOSES]
     DIGEST_KEY_PURPOSES = [name[0] for name in KEY_PURPOSES if name[2] == "DIGEST"]
 
     def check_format(self, new_value_str):
         # str convert to int: "XTS_AES_128_KEY" - > str(4)
         # if int: 4 -> str(4)
         raw_val = new_value_str
@@ -434,18 +443,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32c6/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c6/operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -190,37 +190,46 @@
 def set_flash_voltage(esp, efuses, args):
     raise esptool.FatalError("set_flash_voltage is not supported!")
 
 
 def adc_info(esp, efuses, args):
     print("")
     # fmt: off
-    if efuses["BLK_VERSION_MINOR"].get() == 1:
-        print("Temperature Sensor Calibration = {}C".format(efuses["TEMP_CALIB"].get()))
+    if efuses["BLK_VERSION_MAJOR"].get() == 1:
+        print("Temperature Sensor Calibration = {}C".format(efuses["TEMP_SENSOR_CAL"].get()))
 
         print("")
-        print("ADC1 Calibration data stored in efuse BLOCK2:")
-        print(f"OCODE: {efuses['OCODE'].get()}")
-        print(f"INIT_CODE_ATTEN0: {efuses['ADC1_INIT_CODE_ATTEN0'].get()}")
-        print(f"INIT_CODE_ATTEN1: {efuses['ADC1_INIT_CODE_ATTEN1'].get()}")
-        print(f"INIT_CODE_ATTEN2: {efuses['ADC1_INIT_CODE_ATTEN2'].get()}")
-        print(f"INIT_CODE_ATTEN3: {efuses['ADC1_INIT_CODE_ATTEN3'].get()}")
-        print(f"CAL_VOL_ATTEN0: {efuses['ADC1_CAL_VOL_ATTEN0'].get()}")
-        print(f"CAL_VOL_ATTEN1: {efuses['ADC1_CAL_VOL_ATTEN1'].get()}")
-        print(f"CAL_VOL_ATTEN2: {efuses['ADC1_CAL_VOL_ATTEN2'].get()}")
-        print(f"CAL_VOL_ATTEN3: {efuses['ADC1_CAL_VOL_ATTEN3'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH0: {efuses['ADC1_INIT_CODE_ATTEN0_CH0'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH1: {efuses['ADC1_INIT_CODE_ATTEN0_CH1'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH2: {efuses['ADC1_INIT_CODE_ATTEN0_CH2'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH3: {efuses['ADC1_INIT_CODE_ATTEN0_CH3'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH4: {efuses['ADC1_INIT_CODE_ATTEN0_CH4'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH5: {efuses['ADC1_INIT_CODE_ATTEN0_CH5'].get()}")
-        print(f"INIT_CODE_ATTEN0_CH6: {efuses['ADC1_INIT_CODE_ATTEN0_CH6'].get()}")
+        print("ADC1 readings stored in efuse BLOCK2:")
+        print("    MODE0 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE0_D1"].get()))
+        print("    MODE0 D2 reading  (600mV):  {}".format(efuses["ADC1_MODE0_D2"].get()))
+
+        print("    MODE1 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE1_D1"].get()))
+        print("    MODE1 D2 reading  (800mV):  {}".format(efuses["ADC1_MODE1_D2"].get()))
+
+        print("    MODE2 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE2_D1"].get()))
+        print("    MODE2 D2 reading  (1000mV): {}".format(efuses["ADC1_MODE2_D2"].get()))
+
+        print("    MODE3 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE3_D1"].get()))
+        print("    MODE3 D2 reading  (2000mV): {}".format(efuses["ADC1_MODE3_D2"].get()))
+
+        print("")
+        print("ADC2 readings stored in efuse BLOCK2:")
+        print("    MODE0 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE0_D1"].get()))
+        print("    MODE0 D2 reading  (600mV):  {}".format(efuses["ADC2_MODE0_D2"].get()))
+
+        print("    MODE1 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE1_D1"].get()))
+        print("    MODE1 D2 reading  (800mV):  {}".format(efuses["ADC2_MODE1_D2"].get()))
+
+        print("    MODE2 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE2_D1"].get()))
+        print("    MODE2 D2 reading  (1000mV): {}".format(efuses["ADC2_MODE2_D2"].get()))
+
+        print("    MODE3 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE3_D1"].get()))
+        print("    MODE3 D2 reading  (2000mV): {}".format(efuses["ADC2_MODE3_D2"].get()))
     else:
-        print("BLK_VERSION_MINOR = {}".format(efuses["BLK_VERSION_MINOR"].get_meaning()))
+        print("BLK_VERSION_MAJOR = {}".format(efuses["BLK_VERSION_MAJOR"].get_meaning()))
     # fmt: on
 
 
 def burn_key(esp, efuses, args, digest=None):
     if digest is None:
         datafile_list = args.keyfile[
             0 : len([name for name in args.keyfile if name is not None]) :
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32h2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c3/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# This file describes eFuses controller for ESP32-H2 chip
+# This file describes eFuses controller for ESP32-C3 chip
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import reedsolo
 
 from .mem_definition import EfuseDefineBlocks, EfuseDefineFields, EfuseDefineRegisters
 from ..emulate_efuse_controller_base import EmulateEfuseControllerBase, FatalError
 
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
-    CHIP_NAME = "ESP32-H2"
+    CHIP_NAME = "ESP32-C3"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
 
     def get_minor_chip_version(self):
-        return 0
+        return 4
 
     def get_crystal_freq(self):
-        return 32  # MHz
+        return 40  # MHz (common for all chips)
 
     def get_security_info(self):
         return {
             "flags": 0,
             "flash_crypt_cnt": 0,
             "key_purposes": 0,
             "chip_id": 0,
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32h2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32c3/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses for ESP32-H2 chip
+# This file describes eFuses for ESP32-C3 chip
 #
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-H2":
+        if esp.CHIP_NAME != "ESP32-C3":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-H2 chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-C3 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -219,58 +240,55 @@
                     exit(0)  # finish without errors
             raise
 
     def set_efuse_timing(self):
         """Set timing registers for burning efuses"""
         # Configure clock
         apb_freq = self.get_crystal_freq()
-        # Based on `CONFIG_SOC_XTAL_SUPPORT_32M=y` for this target from ESP-IDF configuration
-        if apb_freq != 32:
+        if apb_freq != 40:
             raise esptool.FatalError(
-                "The eFuse supports only xtal=32M (xtal was %d)" % apb_freq
+                "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
-        old_addr_reg = 0
-        reg_value = 0
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
-                addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
-                    block.id
-                ]
-                if err_num_mask is None or err_num_offs is None or fail_bit is None:
-                    continue
-                if addr_reg != old_addr_reg:
-                    old_addr_reg = addr_reg
-                    reg_value = self.read_reg(addr_reg)
-                block.fail = reg_value & (1 << fail_bit) != 0
-                block.num_errors = (reg_value >> err_num_offs) & err_num_mask
+                addr_reg_f, fail_bit = self.REGS.BLOCK_FAIL_BIT[block.id]
+                if fail_bit is None:
+                    block.fail = False
+                else:
+                    block.fail = self.read_reg(addr_reg_f) & (1 << fail_bit) != 0
+
+                addr_reg_n, num_mask, num_offs = self.REGS.BLOCK_NUM_ERRORS[block.id]
+                if num_mask is None or num_offs is None:
+                    block.num_errors = 0
+                else:
+                    block.num_errors = (
+                        self.read_reg(addr_reg_n) >> num_offs
+                    ) & num_mask
+
             ret_fail |= block.fail
             if not silent and (block.fail or block.num_errors):
                 print(
                     "Error(s) in BLOCK%d [ERRORS:%d FAIL:%d]"
                     % (block.id, block.num_errors, block.fail)
                 )
         if (self.debug or ret_fail) and not silent:
@@ -280,30 +298,43 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -323,55 +354,44 @@
 
 class EfuseMacField(EfuseField):
     def check_format(self, new_value_str):
         if new_value_str is None:
             raise esptool.FatalError(
                 "Required MAC Address in AA:CD:EF:01:02:03 format!"
             )
-        num_bytes = 8 if self.name == "MAC_EUI64" else 6
-        if new_value_str.count(":") != num_bytes - 1:
+        if new_value_str.count(":") != 5:
             raise esptool.FatalError(
-                f"MAC Address needs to be a {num_bytes}-byte hexadecimal format "
+                "MAC Address needs to be a 6-byte hexadecimal format "
                 "separated by colons (:)!"
             )
         hexad = new_value_str.replace(":", "")
-        hexad = hexad.split(" ", 1)[0] if self.is_field_calculated() else hexad
-        if len(hexad) != num_bytes * 2:
+        if len(hexad) != 12:
             raise esptool.FatalError(
-                f"MAC Address needs to be a {num_bytes}-byte hexadecimal number "
-                f"({num_bytes * 2} hexadecimal characters)!"
+                "MAC Address needs to be a 6-byte hexadecimal number "
+                "(12 hexadecimal characters)!"
             )
         # order of bytearray = b'\xaa\xcd\xef\x01\x02\x03',
         bindata = binascii.unhexlify(hexad)
-
-        if not self.is_field_calculated():
-            # unicast address check according to
-            # https://tools.ietf.org/html/rfc7042#section-2.1
-            if esptool.util.byte(bindata, 0) & 0x01:
-                raise esptool.FatalError("Custom MAC must be a unicast MAC!")
+        # unicast address check according to
+        # https://tools.ietf.org/html/rfc7042#section-2.1
+        if esptool.util.byte(bindata, 0) & 0x01:
+            raise esptool.FatalError("Custom MAC must be a unicast MAC!")
         return bindata
 
     def check(self):
         errs, fail = self.parent.get_block_errors(self.block)
         if errs != 0 or fail:
             output = "Block%d has ERRORS:%d FAIL:%d" % (self.block, errs, fail)
         else:
             output = "OK"
         return "(" + output + ")"
 
     def get(self, from_read=True):
         if self.name == "CUSTOM_MAC":
             mac = self.get_raw(from_read)[::-1]
-        elif self.name == "MAC":
-            mac = self.get_raw(from_read)
-        elif self.name == "MAC_EUI64":
-            mac = self.parent["MAC"].get_bitstring(from_read).copy()
-            mac_ext = self.parent["MAC_EXT"].get_bitstring(from_read)
-            mac.insert(mac_ext, 24)
-            mac = mac.bytes
         else:
             mac = self.get_raw(from_read)
         return "%s %s" % (util.hexify(mac, ":"), self.check())
 
     def save(self, new_value):
         def print_field(e, new_value):
             print(
@@ -383,23 +403,22 @@
         if self.name == "CUSTOM_MAC":
             bitarray_mac = self.convert_to_bitstring(new_value)
             print_field(self, bitarray_mac)
             super(EfuseMacField, self).save(new_value)
         else:
             # Writing the BLOCK1 (MAC_SPI_8M_0) default MAC is not possible,
             # as it's written in the factory.
-            raise esptool.FatalError(f"Burning {self.name} is not supported")
+            raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 # fmt: off
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
         ("USER",                         0,  None,       None,      "no_need_rd_protect"),   # User purposes (software-only use)
-        ("ECDSA_KEY",                    1,  None,       "Reverse", "need_rd_protect"),      # ECDSA key
-        ("RESERVED",                     2,  None,       None,      "no_need_rd_protect"),   # Reserved
+        ("RESERVED",                     1,  None,       None,      "no_need_rd_protect"),   # Reserved
         ("XTS_AES_128_KEY",              4,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_128_KEY (flash/PSRAM encryption)
         ("HMAC_DOWN_ALL",                5,  None,       None,      "need_rd_protect"),      # HMAC Downstream mode
         ("HMAC_DOWN_JTAG",               6,  None,       None,      "need_rd_protect"),      # JTAG soft enable key (uses HMAC Downstream mode)
         ("HMAC_DOWN_DIGITAL_SIGNATURE",  7,  None,       None,      "need_rd_protect"),      # Digital Signature peripheral key (uses HMAC Downstream mode)
         ("HMAC_UP",                      8,  None,       None,      "need_rd_protect"),      # HMAC Upstream mode
         ("SECURE_BOOT_DIGEST0",          9,  "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST0 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST1",          10, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST1 (Secure Boot key digest)
@@ -436,18 +455,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value in ["XTS_AES_128_KEY", "ECDSA_KEY"]:
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32h2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,16 +151,17 @@
             metavar="KEYPURPOSE",
             choices=fields.EfuseKeyPurposeField.DIGEST_KEY_PURPOSES,
         )
 
     p = subparsers.add_parser(
         "set_flash_voltage",
         help="Permanently set the internal flash voltage regulator "
-        "to either 1.8V, 3.3V or OFF. This means GPIO45 can be high or low "
-        "at reset without changing the flash voltage.",
+        "to either 1.8V, 3.3V or OFF. "
+        "This means GPIO45 can be high or low at reset without "
+        "changing the flash voltage.",
     )
     p.add_argument("voltage", help="Voltage selection", choices=["1.8V", "3.3V", "OFF"])
 
     p = subparsers.add_parser(
         "burn_custom_mac", help="Burn a 48-bit Custom MAC Address to EFUSE BLOCK3."
     )
     p.add_argument(
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-H2(beta1)"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32h2beta1/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file describes eFuses for ESP32-H2 chip
 #
-# SPDX-FileCopyrightText: 2021-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import binascii
 import struct
 import time
 
@@ -50,29 +50,30 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
-        if esp.CHIP_NAME != "ESP32-H2(beta1)":
+        if esp.CHIP_NAME != "ESP32-H2":
             raise esptool.FatalError(
-                "Expected the 'esp' param for ESP32-H2(beta1) chip but got for '%s'."
+                "Expected the 'esp' param for ESP32-H2 chip but got for '%s'."
                 % (esp.CHIP_NAME)
             )
         if not skip_connect:
             flags = self._esp.get_security_info()["flags"]
             GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE = 1 << 2
             if flags & GET_SECURITY_INFO_FLAG_SECURE_DOWNLOAD_ENABLE:
                 raise esptool.FatalError(
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -219,57 +240,56 @@
                     exit(0)  # finish without errors
             raise
 
     def set_efuse_timing(self):
         """Set timing registers for burning efuses"""
         # Configure clock
         apb_freq = self.get_crystal_freq()
+        # Based on `CONFIG_SOC_XTAL_SUPPORT_32M=y` for this target from ESP-IDF configuration
         if apb_freq != 32:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=32M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
-        old_addr_reg = 0
-        reg_value = 0
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
-                addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
-                    block.id
-                ]
-                if err_num_mask is None or err_num_offs is None or fail_bit is None:
-                    continue
-                if addr_reg != old_addr_reg:
-                    old_addr_reg = addr_reg
-                    reg_value = self.read_reg(addr_reg)
-                block.fail = reg_value & (1 << fail_bit) != 0
-                block.num_errors = (reg_value >> err_num_offs) & err_num_mask
+                addr_reg_f, fail_bit = self.REGS.BLOCK_FAIL_BIT[block.id]
+                if fail_bit is None:
+                    block.fail = False
+                else:
+                    block.fail = self.read_reg(addr_reg_f) & (1 << fail_bit) != 0
+
+                addr_reg_n, num_mask, num_offs = self.REGS.BLOCK_NUM_ERRORS[block.id]
+                if num_mask is None or num_offs is None:
+                    block.num_errors = 0
+                else:
+                    block.num_errors = (
+                        self.read_reg(addr_reg_n) >> num_offs
+                    ) & num_mask
+
             ret_fail |= block.fail
             if not silent and (block.fail or block.num_errors):
                 print(
                     "Error(s) in BLOCK%d [ERRORS:%d FAIL:%d]"
                     % (block.id, block.num_errors, block.fail)
                 )
         if (self.debug or ret_fail) and not silent:
@@ -279,30 +299,43 @@
     def summary(self):
         # TODO add support set_flash_voltage - "Flash voltage (VDD_SPI)"
         return ""
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -322,55 +355,44 @@
 
 class EfuseMacField(EfuseField):
     def check_format(self, new_value_str):
         if new_value_str is None:
             raise esptool.FatalError(
                 "Required MAC Address in AA:CD:EF:01:02:03 format!"
             )
-        num_bytes = 8 if self.name == "MAC_EUI64" else 6
-        if new_value_str.count(":") != num_bytes - 1:
+        if new_value_str.count(":") != 5:
             raise esptool.FatalError(
-                f"MAC Address needs to be a {num_bytes}-byte hexadecimal format "
+                "MAC Address needs to be a 6-byte hexadecimal format "
                 "separated by colons (:)!"
             )
-        hexad = new_value_str.replace(":", "").split(" ", 1)[0]
-        hexad = hexad.split(" ", 1)[0] if self.is_field_calculated() else hexad
-        if len(hexad) != num_bytes * 2:
+        hexad = new_value_str.replace(":", "")
+        if len(hexad) != 12:
             raise esptool.FatalError(
-                f"MAC Address needs to be a {num_bytes}-byte hexadecimal number "
-                f"({num_bytes * 2} hexadecimal characters)!"
+                "MAC Address needs to be a 6-byte hexadecimal number "
+                "(12 hexadecimal characters)!"
             )
         # order of bytearray = b'\xaa\xcd\xef\x01\x02\x03',
         bindata = binascii.unhexlify(hexad)
-
-        if not self.is_field_calculated():
-            # unicast address check according to
-            # https://tools.ietf.org/html/rfc7042#section-2.1
-            if esptool.util.byte(bindata, 0) & 0x01:
-                raise esptool.FatalError("Custom MAC must be a unicast MAC!")
+        # unicast address check according to
+        # https://tools.ietf.org/html/rfc7042#section-2.1
+        if esptool.util.byte(bindata, 0) & 0x01:
+            raise esptool.FatalError("Custom MAC must be a unicast MAC!")
         return bindata
 
     def check(self):
         errs, fail = self.parent.get_block_errors(self.block)
         if errs != 0 or fail:
             output = "Block%d has ERRORS:%d FAIL:%d" % (self.block, errs, fail)
         else:
             output = "OK"
         return "(" + output + ")"
 
     def get(self, from_read=True):
         if self.name == "CUSTOM_MAC":
             mac = self.get_raw(from_read)[::-1]
-        elif self.name == "MAC":
-            mac = self.get_raw(from_read)
-        elif self.name == "MAC_EUI64":
-            mac = self.parent["MAC"].get_bitstring(from_read).copy()
-            mac_ext = self.parent["MAC_EXT"].get_bitstring(from_read)
-            mac.insert(mac_ext, 24)
-            mac = mac.bytes
         else:
             mac = self.get_raw(from_read)
         return "%s %s" % (util.hexify(mac, ":"), self.check())
 
     def save(self, new_value):
         def print_field(e, new_value):
             print(
@@ -382,34 +404,33 @@
         if self.name == "CUSTOM_MAC":
             bitarray_mac = self.convert_to_bitstring(new_value)
             print_field(self, bitarray_mac)
             super(EfuseMacField, self).save(new_value)
         else:
             # Writing the BLOCK1 (MAC_SPI_8M_0) default MAC is not possible,
             # as it's written in the factory.
-            raise esptool.FatalError(f"Burning {self.name} is not supported")
             raise esptool.FatalError("Writing Factory MAC address is not supported")
 
 
 # fmt: off
 class EfuseKeyPurposeField(EfuseField):
     KEY_PURPOSES = [
         ("USER",                         0,  None,       None,      "no_need_rd_protect"),   # User purposes (software-only use)
-        ("RESERVED",                     1,  None,       None,      "no_need_rd_protect"),   # Reserved
+        ("ECDSA_KEY",                    1,  None,       "Reverse", "need_rd_protect"),      # ECDSA key
+        ("RESERVED",                     2,  None,       None,      "no_need_rd_protect"),   # Reserved
         ("XTS_AES_128_KEY",              4,  None,       "Reverse", "need_rd_protect"),      # XTS_AES_128_KEY (flash/PSRAM encryption)
         ("HMAC_DOWN_ALL",                5,  None,       None,      "need_rd_protect"),      # HMAC Downstream mode
         ("HMAC_DOWN_JTAG",               6,  None,       None,      "need_rd_protect"),      # JTAG soft enable key (uses HMAC Downstream mode)
         ("HMAC_DOWN_DIGITAL_SIGNATURE",  7,  None,       None,      "need_rd_protect"),      # Digital Signature peripheral key (uses HMAC Downstream mode)
         ("HMAC_UP",                      8,  None,       None,      "need_rd_protect"),      # HMAC Upstream mode
         ("SECURE_BOOT_DIGEST0",          9,  "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST0 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST1",          10, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST1 (Secure Boot key digest)
         ("SECURE_BOOT_DIGEST2",          11, "DIGEST",   None,      "no_need_rd_protect"),   # SECURE_BOOT_DIGEST2 (Secure Boot key digest)
     ]
 # fmt: on
-
     KEY_PURPOSES_NAME = [name[0] for name in KEY_PURPOSES]
     DIGEST_KEY_PURPOSES = [name[0] for name in KEY_PURPOSES if name[2] == "DIGEST"]
 
     def check_format(self, new_value_str):
         # str convert to int: "XTS_AES_128_KEY" - > str(4)
         # if int: 4 -> str(4)
         raw_val = new_value_str
@@ -436,18 +457,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32h2beta1/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32h2beta1/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,16 @@
 
     p = subparsers.add_parser(
         "burn_custom_mac", help="Burn a 48-bit Custom MAC Address to EFUSE BLOCK3."
     )
     p.add_argument(
         "mac",
         help="Custom MAC Address to burn given in hexadecimal format with bytes "
-        "separated by colons (e.g. AA:CD:EF:01:02:03).",
+        "separated by colons (e.g. AA:CD:EF:01:02:03). "
+        "Final CUSTOM_MAC = CUSTOM_MAC[48] + MAC_EXT[16]",
         type=fields.base_fields.CheckArgValue(efuses, "CUSTOM_MAC"),
     )
     add_force_write_always(p)
 
     p = subparsers.add_parser("get_custom_mac", help="Prints the Custom MAC Address.")
 
 
@@ -189,15 +190,15 @@
 def set_flash_voltage(esp, efuses, args):
     raise esptool.FatalError("set_flash_voltage is not supported!")
 
 
 def adc_info(esp, efuses, args):
     print("")
     # fmt: off
-    if efuses["BLK_VERSION_MAJOR"].get() == 1:
+    if efuses["BLOCK2_VERSION"].get() == 1:
         print("Temperature Sensor Calibration = {}C".format(efuses["TEMP_SENSOR_CAL"].get()))
 
         print("")
         print("ADC1 readings stored in efuse BLOCK2:")
         print("    MODE0 D1 reading  (250mV):  {}".format(efuses["ADC1_MODE0_D1"].get()))
         print("    MODE0 D2 reading  (600mV):  {}".format(efuses["ADC1_MODE0_D2"].get()))
 
@@ -220,15 +221,15 @@
 
         print("    MODE2 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE2_D1"].get()))
         print("    MODE2 D2 reading  (1000mV): {}".format(efuses["ADC2_MODE2_D2"].get()))
 
         print("    MODE3 D1 reading  (250mV):  {}".format(efuses["ADC2_MODE3_D1"].get()))
         print("    MODE3 D2 reading  (2000mV): {}".format(efuses["ADC2_MODE3_D2"].get()))
     else:
-        print("BLK_VERSION_MAJOR = {}".format(efuses["BLK_VERSION_MAJOR"].get_meaning()))
+        print("BLOCK2_VERSION = {}".format(efuses["BLOCK2_VERSION"].get_meaning()))
     # fmt: on
 
 
 def burn_key(esp, efuses, args, digest=None):
     if digest is None:
         datafile_list = args.keyfile[
             0 : len([name for name in args.keyfile if name is not None]) :
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s2/emulate_efuse_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-S2"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 1
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s2/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-S2":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-S2 chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MINOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -285,17 +306,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -314,45 +338,57 @@
         if (self.debug or ret_fail) and not silent:
             self.print_status_regs()
         return ret_fail
 
     def summary(self):
         if self["VDD_SPI_FORCE"].get() == 0:
             output = "Flash voltage (VDD_SPI) determined by GPIO45 on reset "
-            output += "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
+            "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
             output += "GPIO45=Low or NC: VDD_SPI pin is powered directly from "
-            output += "VDD3P3_RTC_IO via resistor Rspi. "
-            output += "Typically this voltage is 3.3 V)."
+            "VDD3P3_RTC_IO via resistor Rspi. Typically this voltage is 3.3 V)."
         elif self["VDD_SPI_XPD"].get() == 0:
             output = "Flash voltage (VDD_SPI) internal regulator disabled by efuse."
         elif self["VDD_SPI_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SPI) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SPI) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s3/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-S3"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s3/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-S3":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-S3 chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -224,21 +245,14 @@
         # Configure clock
         apb_freq = self.get_crystal_freq()
         if apb_freq != 40:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         old_addr_reg = 0
@@ -246,17 +260,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -275,45 +292,57 @@
         if (self.debug or ret_fail) and not silent:
             self.print_status_regs()
         return ret_fail
 
     def summary(self):
         if self["VDD_SPI_FORCE"].get() == 0:
             output = "Flash voltage (VDD_SPI) determined by GPIO45 on reset "
-            output += "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
+            "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
             output += "GPIO45=Low or NC: VDD_SPI pin is powered directly from "
-            output += "VDD3P3_RTC_IO via resistor Rspi. "
-            output += "Typically this voltage is 3.3 V)."
+            "VDD3P3_RTC_IO via resistor Rspi. Typically this voltage is 3.3 V)."
         elif self["VDD_SPI_XPD"].get() == 0:
             output = "Flash voltage (VDD_SPI) internal regulator disabled by efuse."
         elif self["VDD_SPI_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SPI) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SPI) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -438,18 +467,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s3/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 class EmulateEfuseController(EmulateEfuseControllerBase):
     """The class for virtual efuse operation. Using for HOST_TEST."""
 
     CHIP_NAME = "ESP32-S3(beta2)"
     mem = None
     debug = False
+    Blocks = EfuseDefineBlocks
+    Fields = EfuseDefineFields
+    REGS = EfuseDefineRegisters
 
     def __init__(self, efuse_file=None, debug=False):
-        self.Blocks = EfuseDefineBlocks
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
         super(EmulateEfuseController, self).__init__(efuse_file, debug)
         self.write_reg(self.REGS.EFUSE_STATUS_REG, 1)
 
     """ esptool method start >>"""
 
     def get_major_chip_version(self):
         return 0
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s3beta2/fields.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 
 
 class EspEfuses(base_fields.EspEfusesBase):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
+    Blocks = EfuseDefineBlocks()
+    Fields = EfuseDefineFields()
+    REGS = EfuseDefineRegisters
+    BURN_BLOCK_DATA_NAMES = Blocks.get_burn_block_data_names()
+    BLOCKS_FOR_KEYS = Blocks.get_blocks_for_keys()
+
     debug = False
     do_not_confirm = False
 
     def __init__(self, esp, skip_connect=False, debug=False, do_not_confirm=False):
-        self.Blocks = EfuseDefineBlocks()
-        self.Fields = EfuseDefineFields()
-        self.REGS = EfuseDefineRegisters
-        self.BURN_BLOCK_DATA_NAMES = self.Blocks.get_burn_block_data_names()
-        self.BLOCKS_FOR_KEYS = self.Blocks.get_blocks_for_keys()
         self._esp = esp
         self.debug = debug
         self.do_not_confirm = do_not_confirm
         if esp.CHIP_NAME != "ESP32-S3(beta2)":
             raise esptool.FatalError(
                 "Expected the 'esp' param for ESP32-S3(beta2) chip but got for '%s'."
                 % (esp.CHIP_NAME)
@@ -80,51 +81,67 @@
                 )
         self.blocks = [
             EfuseBlock(self, self.Blocks.get(block), skip_read=skip_connect)
             for block in self.Blocks.BLOCKS
         ]
         if not skip_connect:
             self.get_coding_scheme_warnings()
-        self.efuses = [EfuseField.convert(self, efuse) for efuse in self.Fields.EFUSES]
+        self.efuses = [
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.EFUSES
+        ]
         self.efuses += [
-            EfuseField.convert(self, efuse) for efuse in self.Fields.KEYBLOCKS
+            EfuseField.from_tuple(
+                self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+            )
+            for efuse in self.Fields.KEYBLOCKS
         ]
         if skip_connect:
             self.efuses += [
-                EfuseField.convert(self, efuse)
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
                 for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
             ]
         else:
             if self["BLK_VERSION_MAJOR"].get() == 1:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
             self.efuses += [
-                EfuseField.convert(self, efuse) for efuse in self.Fields.CALC
+                EfuseField.from_tuple(
+                    self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                )
+                for efuse in self.Fields.CALC
             ]
 
     def __getitem__(self, efuse_name):
         """Return the efuse field with the given name"""
         for e in self.efuses:
-            if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+            if efuse_name == e.name:
                 return e
         new_fields = False
         for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES:
-            if efuse.name == efuse_name or any(
-                x == efuse_name for x in efuse.alt_names
-            ):
+            e = self.Fields.get(efuse)
+            if e.name == efuse_name:
                 self.efuses += [
-                    EfuseField.convert(self, efuse)
+                    EfuseField.from_tuple(
+                        self, self.Fields.get(efuse), self.Fields.get(efuse).class_type
+                    )
                     for efuse in self.Fields.BLOCK2_CALIBRATION_EFUSES
                 ]
                 new_fields = True
         if new_fields:
             for e in self.efuses:
-                if efuse_name == e.name or any(x == efuse_name for x in e.alt_names):
+                if efuse_name == e.name:
                     return e
         raise KeyError
 
     def read_coding_scheme(self):
         self.coding_scheme = self.REGS.CODING_SCHEME_RS
 
     def print_status_regs(self):
@@ -137,14 +154,18 @@
         )
         print(
             "{:27} 0x{:08x}".format(
                 "EFUSE_RD_RS_ERR1_REG", self.read_reg(self.REGS.EFUSE_RD_RS_ERR1_REG)
             )
         )
 
+    def get_block_errors(self, block_num):
+        """Returns (error count, failure boolean flag)"""
+        return self.blocks[block_num].num_errors, self.blocks[block_num].fail
+
     def efuse_controller_setup(self):
         self.set_efuse_timing()
         self.clear_pgm_registers()
         self.wait_efuse_idle()
 
     def write_efuses(self, block):
         self.efuse_program(block)
@@ -224,21 +245,14 @@
         # Configure clock
         apb_freq = self.get_crystal_freq()
         if apb_freq != 40:
             raise esptool.FatalError(
                 "The eFuse supports only xtal=40M (xtal was %d)" % apb_freq
             )
 
-        self.update_reg(self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_NUM_M, 0xFF)
-        self.update_reg(
-            self.REGS.EFUSE_DAC_CONF_REG, self.REGS.EFUSE_DAC_CLK_DIV_M, 0x28
-        )
-        self.update_reg(
-            self.REGS.EFUSE_WR_TIM_CONF1_REG, self.REGS.EFUSE_PWR_ON_NUM_M, 0x3000
-        )
         self.update_reg(
             self.REGS.EFUSE_WR_TIM_CONF2_REG, self.REGS.EFUSE_PWR_OFF_NUM_M, 0x190
         )
 
     def get_coding_scheme_warnings(self, silent=False):
         """Check if the coding scheme has detected any errors."""
         old_addr_reg = 0
@@ -246,17 +260,20 @@
         ret_fail = False
         for block in self.blocks:
             if block.id == 0:
                 words = [
                     self.read_reg(self.REGS.EFUSE_RD_REPEAT_ERR0_REG + offs * 4)
                     for offs in range(5)
                 ]
-                block.err_bitarray.pos = 0
+                data = BitArray()
                 for word in reversed(words):
-                    block.err_bitarray.overwrite(BitArray("uint:32=%d" % word))
+                    data.append("uint:32=%d" % word)
+                # pos=32 because EFUSE_WR_DIS goes first it is 32bit long
+                # and not under error control
+                block.err_bitarray.overwrite(data, pos=32)
                 block.num_errors = block.err_bitarray.count(True)
                 block.fail = block.num_errors != 0
             else:
                 addr_reg, err_num_mask, err_num_offs, fail_bit = self.REGS.BLOCK_ERRORS[
                     block.id
                 ]
                 if err_num_mask is None or err_num_offs is None or fail_bit is None:
@@ -275,45 +292,57 @@
         if (self.debug or ret_fail) and not silent:
             self.print_status_regs()
         return ret_fail
 
     def summary(self):
         if self["VDD_SPI_FORCE"].get() == 0:
             output = "Flash voltage (VDD_SPI) determined by GPIO45 on reset "
-            output += "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
+            "(GPIO45=High: VDD_SPI pin is powered from internal 1.8V LDO\n"
             output += "GPIO45=Low or NC: VDD_SPI pin is powered directly from "
-            output += "VDD3P3_RTC_IO via resistor Rspi. "
-            output += "Typically this voltage is 3.3 V)."
+            "VDD3P3_RTC_IO via resistor Rspi. Typically this voltage is 3.3 V)."
         elif self["VDD_SPI_XPD"].get() == 0:
             output = "Flash voltage (VDD_SPI) internal regulator disabled by efuse."
         elif self["VDD_SPI_TIEH"].get() == 0:
             output = "Flash voltage (VDD_SPI) set to 1.8V by efuse."
         else:
             output = "Flash voltage (VDD_SPI) set to 3.3V by efuse."
         return output
 
 
 class EfuseField(base_fields.EfuseFieldBase):
     @staticmethod
-    def convert(parent, efuse):
+    def from_tuple(parent, efuse_tuple, type_class):
         return {
             "mac": EfuseMacField,
             "keypurpose": EfuseKeyPurposeField,
             "t_sensor": EfuseTempSensor,
             "adc_tp": EfuseAdcPointCalibration,
             "wafer": EfuseWafer,
-        }.get(efuse.class_type, EfuseField)(parent, efuse)
+        }.get(type_class, EfuseField)(parent, efuse_tuple)
+
+    def get_info(self):
+        output = "%s (BLOCK%d)" % (self.name, self.block)
+        errs, fail = self.parent.get_block_errors(self.block)
+        if errs != 0 or fail:
+            output += (
+                "[FAIL:%d]" % (fail)
+                if self.block == 0
+                else "[ERRS:%d FAIL:%d]" % (errs, fail)
+            )
+        if self.efuse_class == "keyblock":
+            name = self.parent.blocks[self.block].key_purpose_name
+            if name is not None:
+                output += "\n  Purpose: %s\n " % (self.parent[name].get())
+        return output
 
 
 class EfuseWafer(EfuseField):
     def get(self, from_read=True):
         hi_bits = self.parent["WAFER_VERSION_MINOR_HI"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_HI"].bit_len == 1
         lo_bits = self.parent["WAFER_VERSION_MINOR_LO"].get(from_read)
-        assert self.parent["WAFER_VERSION_MINOR_LO"].bit_len == 3
         return (hi_bits << 3) + lo_bits
 
     def save(self, new_value):
         raise esptool.FatalError("Burning %s is not supported" % self.name)
 
 
 class EfuseTempSensor(EfuseField):
@@ -438,18 +467,10 @@
 
     def get(self, from_read=True):
         for p in self.KEY_PURPOSES:
             if p[1] == self.get_raw(from_read):
                 return p[0]
         return "FORBIDDEN_STATE"
 
-    def get_name(self, raw_val):
-        for key in self.KEY_PURPOSES:
-            if key[1] == raw_val:
-                return key[0]
-
     def save(self, new_value):
         raw_val = int(self.check_format(str(new_value)))
-        str_new_value = self.get_name(raw_val)
-        if self.name == "KEY_PURPOSE_5" and str_new_value.startswith("XTS_AES"):
-            raise esptool.FatalError(f"{self.name} can not have {str_new_value} key due to a hardware bug (please see TRM for more details)")
         return super(EfuseKeyPurposeField, self).save(raw_val)
```

### Comparing `esptool-4.6.2/espefuse/efuse/esp32s3beta2/operations.py` & `esptool-4.6.dev1/espefuse/efuse/esp32s3beta2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse/efuse/util.py` & `esptool-4.6.dev1/espefuse/efuse/util.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espefuse.py` & `esptool-4.6.dev1/espefuse.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 import os
 import sys
 
 if os.name != "nt":
     # Linux/macOS: remove current script directory to avoid importing this file
     # as a module; we want to import the installed espefuse module instead
     with contextlib.suppress(ValueError):
-        executable_dir = os.path.dirname(sys.executable)
-        sys.path = [
-            path
-            for path in sys.path
-            if not path.endswith(("/bin", "/sbin")) and path != executable_dir
-        ]
+        if sys.path[0].endswith("/bin"):
+            sys.path.pop(0)
+        sys.path.remove(os.path.dirname(sys.executable))
 
     # Linux/macOS: delete imported module entry to force Python to load
     # the module from scratch; this enables importing espefuse module in
     # other Python scripts
     with contextlib.suppress(KeyError):
         del sys.modules["espefuse"]
```

### Comparing `esptool-4.6.2/espsecure/__init__.py` & `esptool-4.6.dev1/espsecure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,21 +198,15 @@
             raise esptool.FatalError(
                 "ERROR: Unsupported signing scheme (%s)" % args.scheme
             )
 
 
 def load_ecdsa_signing_key(keyfile):
     """Load ECDSA signing key"""
-    try:
-        sk = ecdsa.SigningKey.from_pem(keyfile.read())
-    except ValueError:
-        raise esptool.FatalError(
-            "Incorrect ECDSA private key specified. "
-            "Please check algorithm and/or format."
-        )
+    sk = ecdsa.SigningKey.from_pem(keyfile.read())
     if sk.curve not in [ecdsa.NIST192p, ecdsa.NIST256p]:
         raise esptool.FatalError("Supports NIST192p and NIST256p keys only")
     return sk
 
 
 def _load_ecdsa_signing_key(keyfile):
     """Load ECDSA signing key for Secure Boot V1 only"""
@@ -223,21 +217,15 @@
             "NIST256p (openssl calls this curve 'prime256v1')"
         )
     return sk
 
 
 def _load_ecdsa_verifying_key(keyfile):
     """Load ECDSA verifying key for Secure Boot V1 only"""
-    try:
-        vk = ecdsa.VerifyingKey.from_pem(keyfile.read())
-    except ValueError:
-        raise esptool.FatalError(
-            "Incorrect ECDSA public key specified. "
-            "Please check algorithm and/or format."
-        )
+    vk = ecdsa.VerifyingKey.from_pem(keyfile.read())
     if vk.curve != ecdsa.NIST256p:
         raise esptool.FatalError(
             "Signing key uses incorrect curve. ESP32 Secure Boot only supports "
             "NIST256p (openssl calls this curve 'prime256v1')"
         )
     return vk
 
@@ -1653,16 +1641,15 @@
         help="Secure boot v2 signed data file.",
         type=argparse.FileType("rb"),
     )
 
     p = subparsers.add_parser(
         "digest_private_key",
         help="Generate an SHA-256 digest of the private signing key. "
-        "This can be used as a reproducible secure bootloader (only secure boot v1) "
-        "or flash encryption key.",
+        "This can be used as a reproducible secure bootloader or flash encryption key.",
     )
     p.add_argument(
         "--keyfile",
         "-k",
         help="Private key file (PEM format) to generate a digest from.",
         type=argparse.FileType("rb"),
         required=True,
@@ -1808,21 +1795,11 @@
 
 def _main():
     try:
         main()
     except esptool.FatalError as e:
         print("\nA fatal error occurred: %s" % e)
         sys.exit(2)
-    except ValueError as e:
-        try:
-            if [arg for arg in e.args if "Could not deserialize key data." in arg]:
-                print(
-                    "Note: This error originates from the cryptography module. "
-                    "It is likely not a problem with espsecure, "
-                    "please make sure you are using a compatible OpenSSL backend."
-                )
-        finally:
-            raise
 
 
 if __name__ == "__main__":
     _main()
```

### Comparing `esptool-4.6.2/espsecure/esp_hsm_sign/__init__.py` & `esptool-4.6.dev1/espsecure/esp_hsm_sign/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espsecure/esp_hsm_sign/exceptions.py` & `esptool-4.6.dev1/espsecure/esp_hsm_sign/exceptions.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/espsecure.py` & `esptool-4.6.dev1/espsecure.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 import os
 import sys
 
 if os.name != "nt":
     # Linux/macOS: remove current script directory to avoid importing this file
     # as a module; we want to import the installed espsecure module instead
     with contextlib.suppress(ValueError):
-        executable_dir = os.path.dirname(sys.executable)
-        sys.path = [
-            path
-            for path in sys.path
-            if not path.endswith(("/bin", "/sbin")) and path != executable_dir
-        ]
+        if sys.path[0].endswith("/bin"):
+            sys.path.pop(0)
+        sys.path.remove(os.path.dirname(sys.executable))
 
     # Linux/macOS: delete imported module entry to force Python to load
     # the module from scratch; this enables importing espsecure module in
     # other Python scripts
     with contextlib.suppress(KeyError):
         del sys.modules["espsecure"]
```

### Comparing `esptool-4.6.2/esptool/__init__.py` & `esptool-4.6.dev1/esptool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,24 @@
     "verify_flash",
     "version",
     "write_flash",
     "write_flash_status",
     "write_mem",
 ]
 
-__version__ = "4.6.2"
-
+__version__ = "4.6.dev1"
 import argparse
 import inspect
 import os
 import shlex
 import sys
 import time
 import traceback
 
 from esptool.cmds import (
-    DETECTED_FLASH_SIZES,
     chip_id,
     detect_chip,
     detect_flash_size,
     dump_mem,
     elf2image,
     erase_flash,
     erase_region,
@@ -351,15 +349,15 @@
         "(default if --no-stub is specified)",
         action="store_true",
     )
 
     subparsers.add_parser("run", help="Run application code in flash")
 
     parser_image_info = subparsers.add_parser(
-        "image_info", help="Dump headers from a binary file (bootloader or application)"
+        "image_info", help="Dump headers from an application image"
     )
     parser_image_info.add_argument("filename", help="Image file to parse")
     parser_image_info.add_argument(
         "--version",
         "-v",
         help="Output format version (1 - legacy, 2 - extended)",
         choices=["1", "2"],
@@ -523,17 +521,15 @@
 
     parser_read_flash = subparsers.add_parser(
         "read_flash", help="Read SPI flash content"
     )
     add_spi_connection_arg(parser_read_flash)
     parser_read_flash.add_argument("address", help="Start address", type=arg_auto_int)
     parser_read_flash.add_argument(
-        "size",
-        help="Size of region to dump. Use `ALL` to read to the end of flash.",
-        type=arg_auto_size,
+        "size", help="Size of region to dump", type=arg_auto_int
     )
     parser_read_flash.add_argument("filename", help="Name of binary dump")
     parser_read_flash.add_argument(
         "--no-progress", "-p", help="Suppress progress output", action="store_true"
     )
 
     parser_verify_flash = subparsers.add_parser(
@@ -569,17 +565,16 @@
     )
     add_spi_connection_arg(parser_erase_region)
     parser_erase_region.add_argument(
         "address", help="Start address (must be multiple of 4096)", type=arg_auto_int
     )
     parser_erase_region.add_argument(
         "size",
-        help="Size of region to erase (must be multiple of 4096). "
-        "Use `ALL` to erase to the end of flash.",
-        type=arg_auto_size,
+        help="Size of region to erase (must be multiple of 4096)",
+        type=arg_auto_int,
     )
 
     parser_merge_bin = subparsers.add_parser(
         "merge_bin",
         help="Merge multiple raw binary files into a single file for later flashing",
     )
 
@@ -709,24 +704,15 @@
             elif not esp.IS_STUB and esp.stub_is_disabled:
                 print(
                     "WARNING: Stub loader has been disabled for compatibility, "
                     "setting --no-stub"
                 )
                 args.no_stub = True
             else:
-                try:
-                    esp = esp.run_stub()
-                except Exception:
-                    # The CH9102 bridge (PID: 0x55D4) can have issues on MacOS
-                    if sys.platform == "darwin" and esp._get_pid() == 0x55D4:
-                        print(
-                            "\nNote: If issues persist, "
-                            "try installing the WCH USB-to-Serial MacOS driver."
-                        )
-                    raise
+                esp = esp.run_stub()
 
         if args.override_vddsdio:
             esp.override_vddsdio(args.override_vddsdio)
 
         if args.baud > initial_baud:
             try:
                 esp.change_baud(args.baud)
@@ -820,47 +806,24 @@
             try:
                 flash_xmc_startup()
             except FatalError as e:
                 esp.trace(f"Unable to perform XMC flash chip startup sequence ({e}).")
 
         if hasattr(args, "flash_size"):
             print("Configuring flash size...")
-            if args.flash_size == "detect":
-                flash_size = detect_flash_size(esp, args)
-            elif args.flash_size == "keep":
-                flash_size = detect_flash_size(esp, args=None)
-            else:
-                flash_size = args.flash_size
-
-            if flash_size is not None:  # Secure download mode
-                esp.flash_set_parameters(flash_size_bytes(flash_size))
+            detect_flash_size(esp, args)
+            if args.flash_size != "keep":  # TODO: should set this even with 'keep'
+                esp.flash_set_parameters(flash_size_bytes(args.flash_size))
                 # Check if stub supports chosen flash size
-                if esp.IS_STUB and flash_size in ("32MB", "64MB", "128MB"):
+                if esp.IS_STUB and args.flash_size in ("32MB", "64MB", "128MB"):
                     print(
                         "WARNING: Flasher stub doesn't fully support flash size larger "
                         "than 16MB, in case of failure use --no-stub."
                     )
 
-        if getattr(args, "size", "") == "all":
-            if esp.secure_download_mode:
-                raise FatalError(
-                    "Detecting flash size is not supported in secure download mode. "
-                    "Set an exact size value."
-                )
-            # detect flash size
-            flash_id = esp.flash_id()
-            size_id = flash_id >> 16
-            size_str = DETECTED_FLASH_SIZES.get(size_id)
-            if size_str is None:
-                raise FatalError(
-                    "Detecting flash size failed. Set an exact size value."
-                )
-            print(f"Detected flash size: {size_str}")
-            args.size = flash_size_bytes(size_str)
-
         if esp.IS_STUB and hasattr(args, "address") and hasattr(args, "size"):
             if args.address + args.size > 0x1000000:
                 print(
                     "WARNING: Flasher stub doesn't fully support flash size larger "
                     "than 16MB, in case of failure use --no-stub."
                 )
 
@@ -897,19 +860,14 @@
         operation_func(args)
 
 
 def arg_auto_int(x):
     return int(x, 0)
 
 
-def arg_auto_size(x):
-    x = x.lower()
-    return x if x == "all" else arg_auto_int(x)
-
-
 def get_port_list():
     if list_ports is None:
         raise FatalError(
             "Listing all serial ports is currently not available. "
             "Please try to specify the port when running esptool.py or update "
             "the pyserial package to the latest version"
         )
```

### Comparing `esptool-4.6.2/esptool/bin_image.py` & `esptool-4.6.dev1/esptool/bin_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,24 +636,14 @@
             # move ".flash.appdesc" segment to the top of the flash segment
             for segment in flash_segments:
                 if segment.name == ".flash.appdesc":
                     flash_segments.remove(segment)
                     flash_segments.insert(0, segment)
                     break
 
-            # For the bootloader image
-            # move ".dram0.bootdesc" segment to the top of the ram segment
-            # So bootdesc will be at the very top of the binary at 0x20 offset
-            # (in the first segment).
-            for segment in ram_segments:
-                if segment.name == ".dram0.bootdesc":
-                    ram_segments.remove(segment)
-                    ram_segments.insert(0, segment)
-                    break
-
             # check for multiple ELF sections that are mapped in the same
             # flash mapping region. This is usually a sign of a broken linker script,
             # but if you have a legitimate use case then let us know
             if len(flash_segments) > 0:
                 last_addr = flash_segments[0].addr
                 for segment in flash_segments[1:]:
                     if segment.addr // self.IROM_ALIGN == last_addr // self.IROM_ALIGN:
@@ -809,14 +799,21 @@
                 % (self.ROM_LOADER.IMAGE_CHIP_ID, self.chip_id)
             )
 
         self.min_rev = fields[5]
         self.min_rev_full = fields[6]
         self.max_rev_full = fields[7]
 
+        # reserved fields in the middle should all be zero
+        if any(f for f in fields[8:-1] if f != 0):
+            print(
+                "Warning: some reserved header fields have non-zero values. "
+                "This image may be from a newer esptool.py?"
+            )
+
         append_digest = fields[-1]  # last byte is append_digest
         if append_digest in [0, 1]:
             self.append_digest = append_digest == 1
         else:
             raise RuntimeError(
                 "Invalid value for append_digest field (0x%02x). Should be 0 or 1.",
                 append_digest,
```

### Comparing `esptool-4.6.2/esptool/cmds.py` & `esptool-4.6.dev1/esptool/cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     NotImplementedInROMError,
     NotSupportedError,
     UnsupportedCommandError,
 )
 from .util import (
     div_roundup,
     flash_size_bytes,
-    get_file_size,
     hexify,
     pad_to,
     print_overwrite,
 )
 
 DETECTED_FLASH_SIZES = {
     0x12: "256KB",
@@ -205,38 +204,32 @@
                     "%d bytes read... (%d %%)" % (f.tell(), f.tell() * 100 // args.size)
                 )
             sys.stdout.flush()
         print_overwrite("Read %d bytes" % f.tell(), last_line=True)
     print("Done!")
 
 
-def detect_flash_size(esp, args=None):
-    # TODO: Remove the dependency on args in the next major release (v5.0)
-    if esp.secure_download_mode:
-        if args is not None and args.flash_size == "detect":
+def detect_flash_size(esp, args):
+    if args.flash_size == "detect":
+        if esp.secure_download_mode:
             raise FatalError(
                 "Detecting flash size is not supported in secure download mode. "
                 "Need to manually specify flash size."
             )
-        else:
-            return None
-    flash_id = esp.flash_id()
-    size_id = flash_id >> 16
-    flash_size = DETECTED_FLASH_SIZES.get(size_id)
-    if args is not None and args.flash_size == "detect":
-        if flash_size is None:
-            flash_size = "4MB"
+        flash_id = esp.flash_id()
+        size_id = flash_id >> 16
+        args.flash_size = DETECTED_FLASH_SIZES.get(size_id)
+        if args.flash_size is None:
             print(
-                "Warning: Could not auto-detect Flash size "
-                f"(FlashID={flash_id:#x}, SizeID={size_id:#x}), defaulting to 4MB"
+                "Warning: Could not auto-detect Flash size (FlashID=0x%x, SizeID=0x%x),"
+                " defaulting to 4MB" % (flash_id, size_id)
             )
+            args.flash_size = "4MB"
         else:
-            print("Auto-detected Flash size:", flash_size)
-        args.flash_size = flash_size
-    return flash_size
+            print("Auto-detected Flash size:", args.flash_size)
 
 
 def _update_image_flash_params(esp, address, args, image):
     """
     Modify the flash mode & size bytes if this looks like an executable bootloader image
     """
     if len(image) < 8:
@@ -459,18 +452,16 @@
                     "WARNING: Detected flash encryption enabled and "
                     "download manual encrypt disabled.\n"
                     "Flashing plaintext binary may brick your device! "
                     "Use --force to override the warning."
                 )
 
     # verify file sizes fit in flash
-    flash_end = flash_size_bytes(
-        detect_flash_size(esp) if args.flash_size == "keep" else args.flash_size
-    )
-    if flash_end is not None:  # Secure download mode
+    if args.flash_size != "keep":  # TODO: check this even with 'keep'
+        flash_end = flash_size_bytes(args.flash_size)
         for address, argfile in args.addr_filename:
             argfile.seek(0, os.SEEK_END)
             if address + argfile.tell() > flash_end:
                 raise FatalError(
                     "File %s (length %d) at offset %d "
                     "will not fit in %d bytes of flash. "
                     "Use --flash_size argument, or change flashing address."
@@ -734,39 +725,28 @@
 
         # Extended header (ESP32 and later only)
         if args.chip != "esp8266":
             print()
             title = "{} extended image header".format(args.chip.upper())
             print(title)
             print("=" * len(title))
-            print(
-                f"WP pin: {image.wp_pin:#02x}",
-                *["(disabled)"] if image.wp_pin == image.WP_PIN_DISABLED else [],
-            )
+            print("WP pin: {:#02x}".format(image.wp_pin))
             print(
                 "Flash pins drive settings: "
                 "clk_drv: {:#02x}, q_drv: {:#02x}, d_drv: {:#02x}, "
                 "cs0_drv: {:#02x}, hd_drv: {:#02x}, wp_drv: {:#02x}".format(
                     image.clk_drv,
                     image.q_drv,
                     image.d_drv,
                     image.cs_drv,
                     image.hd_drv,
                     image.wp_drv,
                 )
             )
-            try:
-                chip = next(
-                    chip
-                    for chip in CHIP_DEFS.values()
-                    if getattr(chip, "IMAGE_CHIP_ID", None) == image.chip_id
-                )
-                print(f"Chip ID: {image.chip_id} ({chip.CHIP_NAME})")
-            except StopIteration:
-                print(f"Chip ID: {image.chip_id} (Unknown ID)")
+            print("Chip ID: {}".format(image.chip_id))
             print(
                 "Minimal chip revision: "
                 f"v{image.min_rev_full // 100}.{image.min_rev_full % 100}, "
                 f"(legacy min_rev = {image.min_rev})"
             )
             print(
                 "Maximal chip revision: "
@@ -785,24 +765,19 @@
             )
         )
         print(
             "{}  {}  {}  {}  {}".format("-" * 7, "-" * 7, "-" * 10, "-" * 10, "-" * 12)
         )
         format_str = "{:7}  {:#07x}  {:#010x}  {:#010x}  {}"
         app_desc = None
-        bootloader_desc = None
         for idx, seg in enumerate(image.segments, start=1):
             segs = seg.get_memory_type(image)
             seg_name = ", ".join(segs)
             if "DROM" in segs:  # The DROM segment starts with the esp_app_desc_t struct
                 app_desc = seg.data[:256]
-            elif "DRAM" in segs:
-                # The DRAM segment starts with the esp_bootloader_desc_t struct
-                if len(seg.data) >= 80:
-                    bootloader_desc = seg.data[:80]
             print(
                 format_str.format(idx, len(seg.data), seg.addr, seg.file_offs, seg_name)
             )
         print()
 
         # Footer
         title = f"{args.chip.upper()} image footer"
@@ -852,35 +827,14 @@
                 print(f'Project name: {project_name.decode("utf-8")}')
                 print(f'App version: {version.decode("utf-8")}')
                 print(f'Compile time: {date.decode("utf-8")} {time.decode("utf-8")}')
                 print(f"ELF file SHA256: {hexify(app_elf_sha256, uppercase=False)}")
                 print(f'ESP-IDF: {idf_ver.decode("utf-8")}')
                 print(f"Secure version: {secure_version}")
 
-        elif bootloader_desc:
-            BOOTLOADER_DESC_STRUCT_FMT = "<B" + "3s" + "I32s24s" + "16s"
-            (
-                magic_byte,
-                reserved,
-                version,
-                idf_ver,
-                date_time,
-                reserved2,
-            ) = struct.unpack(BOOTLOADER_DESC_STRUCT_FMT, bootloader_desc)
-
-            if magic_byte == 80:
-                print()
-                title = "Bootloader information"
-                print(title)
-                print("=" * len(title))
-                print(f"Bootloader version: {version}")
-                print(f'ESP-IDF: {idf_ver.decode("utf-8")}')
-                print(f'Compile time: {date_time.decode("utf-8")}')
-
-    print(f"File size: {get_file_size(args.filename)} (bytes)")
     with open(args.filename, "rb") as f:
         # magic number
         try:
             common_header = f.read(8)
             magic = common_header[0]
         except IndexError:
             raise FatalError("File is empty")
@@ -892,14 +846,17 @@
                 "This is not a valid image "
                 "(invalid magic number: {:#x})".format(magic)
             )
 
         if args.chip == "auto":
             try:
                 extended_header = f.read(16)
+                # reserved fields, should all be zero
+                if int.from_bytes(extended_header[7:-1], "little") != 0:
+                    raise FatalError("Reserved fields not all zero")
 
                 # append_digest, either 0 or 1
                 if extended_header[-1] not in [0, 1]:
                     raise FatalError("Append digest field not 0 or 1")
 
                 chip_id = int.from_bytes(extended_header[4:5], "little")
                 for rom in [n for n in ROM_LIST if n.CHIP_NAME != "ESP8266"]:
@@ -1025,24 +982,20 @@
         args.output = image.default_output_name(args.input)
     image.save(args.output)
 
     print("Successfully created {} image.".format(args.chip))
 
 
 def read_mac(esp, args):
+    mac = esp.read_mac()
+
     def print_mac(label, mac):
         print("%s: %s" % (label, ":".join(map(lambda x: "%02x" % x, mac))))
 
-    eui64 = esp.read_mac("EUI64")
-    if eui64:
-        print_mac("MAC", eui64)
-        print_mac("BASE MAC", esp.read_mac("BASE_MAC"))
-        print_mac("MAC_EXT", esp.read_mac("MAC_EXT"))
-    else:
-        print_mac("MAC", esp.read_mac("BASE_MAC"))
+    print_mac("MAC", mac)
 
 
 def chip_id(esp, args):
     try:
         chipid = esp.chip_id()
         print("Chip ID: 0x%08x" % chipid)
     except NotSupportedError:
```

### Comparing `esptool-4.6.2/esptool/config.py` & `esptool-4.6.dev1/esptool/config.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/esptool/loader.py` & `esptool-4.6.dev1/esptool/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,21 +93,21 @@
 # Timeout for serial port write
 DEFAULT_SERIAL_WRITE_TIMEOUT = cfg.getfloat("serial_write_timeout", 10)
 # Default number of times to try connection
 DEFAULT_CONNECT_ATTEMPTS = cfg.getint("connect_attempts", 7)
 # Number of times to try writing a data block
 WRITE_BLOCK_ATTEMPTS = cfg.getint("write_block_attempts", 3)
 
-STUBS_DIR = os.path.join(os.path.dirname(__file__), "targets", "stub_flasher")
+STUBS_DIR = os.path.join(os.path.dirname(__file__), "./targets/stub_flasher/")
 
 
 def get_stub_json_path(chip_name):
     chip_name = strip_chip_name(chip_name)
     chip_name = chip_name.replace("esp", "")
-    return os.path.join(STUBS_DIR, f"stub_flasher_{chip_name}.json")
+    return STUBS_DIR + "stub_flasher_" + chip_name + ".json"
 
 
 def timeout_per_mb(seconds_per_mb, size_bytes):
     """Scales timeouts which are size-specific"""
     result = seconds_per_mb * (size_bytes / 1e6)
     if result < DEFAULT_TIMEOUT:
         return DEFAULT_TIMEOUT
@@ -291,15 +291,14 @@
         self.stub_is_disabled = False
 
         # Device-and-runtime-specific cache
         self.cache = {
             "flash_id": None,
             "chip_id": None,
             "uart_no": None,
-            "usb_pid": None,
         }
 
         if isinstance(port, str):
             try:
                 self._port = serial.serial_for_url(port)
             except serial.serialutil.SerialException:
                 raise FatalError(f"Could not open {port}, the port doesn't exist")
@@ -472,17 +471,14 @@
         self.sync_stub_detected = val == 0
 
         for _ in range(7):
             val, _ = self.command()
             self.sync_stub_detected &= val == 0
 
     def _get_pid(self):
-        if self.cache["usb_pid"] is not None:
-            return self.cache["usb_pid"]
-
         if list_ports is None:
             print(
                 "\nListing all serial ports is currently not available. "
                 "Can't get device PID."
             )
             return
         active_port = self._port.port
@@ -494,27 +490,24 @@
                 "COM and /dev/ serial ports."
             )
             return
         # Return the real path if the active port is a symlink
         if active_port.startswith("/dev/") and os.path.islink(active_port):
             active_port = os.path.realpath(active_port)
 
-        active_ports = [active_port]
-
         # The "cu" (call-up) device has to be used for outgoing communication on MacOS
         if sys.platform == "darwin" and "tty" in active_port:
-            active_ports.append(active_port.replace("tty", "cu"))
+            active_port = [active_port, active_port.replace("tty", "cu")]
         ports = list_ports.comports()
         for p in ports:
-            if p.device in active_ports:
-                self.cache["usb_pid"] = p.pid
+            if p.device in active_port:
                 return p.pid
         print(
-            f"\nFailed to get PID of a device on {active_port}, "
-            "using standard reset sequence."
+            "\nFailed to get PID of a device on {}, "
+            "using standard reset sequence.".format(active_port)
         )
 
     def _connect_attempt(self, reset_strategy, mode="default_reset"):
         """A single connection attempt"""
         last_error = None
         boot_log_detected = False
         download_mode = False
```

### Comparing `esptool-4.6.2/esptool/reset.py` & `esptool-4.6.dev1/esptool/reset.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/esptool/targets/__init__.py` & `esptool-4.6.dev1/esptool/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/esptool/targets/esp32.py` & `esptool-4.6.dev1/esptool/targets/esp32.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,18 +279,16 @@
     def read_efuse(self, n):
         """Read the nth word of the ESP3x EFUSE region."""
         return self.read_reg(self.EFUSE_RD_REG_BASE + (4 * n))
 
     def chip_id(self):
         raise NotSupportedError(self, "chip_id")
 
-    def read_mac(self, mac_type="BASE_MAC"):
+    def read_mac(self):
         """Read MAC from EFUSE region"""
-        if mac_type != "BASE_MAC":
-            return None
         words = [self.read_efuse(2), self.read_efuse(1)]
         bitstring = struct.pack(">II", *words)
         bitstring = bitstring[2:8]  # trim the 2 byte CRC
         return tuple(bitstring)
 
     def get_erase_size(self, offset, size):
         return size
```

### Comparing `esptool-4.6.2/esptool/targets/esp32c2.py` & `esptool-4.6.dev1/esptool/targets/esp32c2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/esptool/targets/esp32c3.py` & `esptool-4.6.dev1/esptool/targets/esp32c3.py`

 * *Files 15% similar despite different names*

```diff
@@ -71,23 +71,18 @@
     SUPPORTS_ENCRYPTED_FLASH = True
 
     FLASH_ENCRYPTED_WRITE_ALIGN = 16
 
     UARTDEV_BUF_NO = 0x3FCDF07C  # Variable in ROM .bss which indicates the port in use
     UARTDEV_BUF_NO_USB_JTAG_SERIAL = 3  # The above var when USB-JTAG/Serial is used
 
+    RTC_CNTL_WDT_WKEY = 0x50D83AA1
     RTCCNTL_BASE_REG = 0x60008000
-    RTC_CNTL_SWD_CONF_REG = RTCCNTL_BASE_REG + 0x00AC
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 31
-    RTC_CNTL_SWD_WPROTECT_REG = RTCCNTL_BASE_REG + 0x00B0
-    RTC_CNTL_SWD_WKEY = 0x8F1D312A
-
     RTC_CNTL_WDTCONFIG0_REG = RTCCNTL_BASE_REG + 0x0090
     RTC_CNTL_WDTWPROTECT_REG = RTCCNTL_BASE_REG + 0x00A8
-    RTC_CNTL_WDT_WKEY = 0x50D83AA1
 
     MEMORY_MAP = [
         [0x00000000, 0x00010000, "PADDING"],
         [0x3C000000, 0x3C800000, "DROM"],
         [0x3FC80000, 0x3FCE0000, "DRAM"],
         [0x3FC88000, 0x3FD00000, "BYTE_ACCESSIBLE"],
         [0x3FF00000, 0x3FF20000, "DROM_MASK"],
@@ -130,18 +125,15 @@
         return 40
 
     def override_vddsdio(self, new_voltage):
         raise NotImplementedInROMError(
             "VDD_SDIO overrides are not supported for ESP32-C3"
         )
 
-    def read_mac(self, mac_type="BASE_MAC"):
-        """Read MAC from EFUSE region"""
-        if mac_type != "BASE_MAC":
-            return None
+    def read_mac(self):
         mac0 = self.read_reg(self.MAC_EFUSE_REG)
         mac1 = self.read_reg(self.MAC_EFUSE_REG + 4)  # only bottom 16 bits are MAC
         bitstring = struct.pack(">II", mac1, mac0)[2:]
         return tuple(bitstring)
 
     def get_flash_crypt_config(self):
         return None  # doesn't exist on ESP32-C3
@@ -179,35 +171,25 @@
         """
         Check the UARTDEV_BUF_NO register to see if USB-JTAG/Serial is being used
         """
         if self.secure_download_mode:
             return False  # Can't detect USB-JTAG/Serial in secure download mode
         return self.get_uart_no() == self.UARTDEV_BUF_NO_USB_JTAG_SERIAL
 
-    def disable_watchdogs(self):
-        # When USB-JTAG/Serial is used, the RTC WDT and SWD watchdog are not reset
-        # and can then reset the board during flashing. Disable or autofeed them.
+    def disable_rtc_watchdog(self):
+        # When USB-JTAG/Serial is used, the RTC watchdog is not reset
+        # and can then reset the board during flashing. Disable it.
         if self.uses_usb_jtag_serial():
-            # Disable RTC WDT
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, self.RTC_CNTL_WDT_WKEY)
             self.write_reg(self.RTC_CNTL_WDTCONFIG0_REG, 0)
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, 0)
 
-            # Automatically feed SWD
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, self.RTC_CNTL_SWD_WKEY)
-            self.write_reg(
-                self.RTC_CNTL_SWD_CONF_REG,
-                self.read_reg(self.RTC_CNTL_SWD_CONF_REG)
-                | self.RTC_CNTL_SWD_AUTO_FEED_EN,
-            )
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, 0)
-
     def _post_connect(self):
         if not self.sync_stub_detected:  # Don't run if stub is reused
-            self.disable_watchdogs()
+            self.disable_rtc_watchdog()
 
 
 class ESP32C3StubLoader(ESP32C3ROM):
     """Access class for ESP32C3 stub loader, runs on top of ROM.
 
     (Basically the same as ESP32StubLoader, but different base class.
     Can possibly be made into a mixin.)
```

### Comparing `esptool-4.6.2/esptool/targets/esp32c6.py` & `esptool-4.6.dev1/esptool/targets/esp32c6.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,19 +72,14 @@
     UARTDEV_BUF_NO = 0x4087F580  # Variable in ROM .bss which indicates the port in use
     UARTDEV_BUF_NO_USB_JTAG_SERIAL = 3  # The above var when USB-JTAG/Serial is used
 
     DR_REG_LP_WDT_BASE = 0x600B1C00
     RTC_CNTL_WDTCONFIG0_REG = DR_REG_LP_WDT_BASE + 0x0  # LP_WDT_RWDT_CONFIG0_REG
     RTC_CNTL_WDTWPROTECT_REG = DR_REG_LP_WDT_BASE + 0x0018  # LP_WDT_RWDT_WPROTECT_REG
 
-    RTC_CNTL_SWD_CONF_REG = DR_REG_LP_WDT_BASE + 0x001C  # LP_WDT_SWD_CONFIG_REG
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 18
-    RTC_CNTL_SWD_WPROTECT_REG = DR_REG_LP_WDT_BASE + 0x0020  # LP_WDT_SWD_WPROTECT_REG
-    RTC_CNTL_SWD_WKEY = 0x50D83AA1  # LP_WDT_SWD_WKEY, same as WDT key in this case
-
     FLASH_FREQUENCY = {
         "80m": 0x0,  # workaround for wrong mspi HS div value in ROM
         "40m": 0x0,
         "20m": 0x2,
     }
 
     MEMORY_MAP = [
@@ -99,28 +94,27 @@
         [0x50000000, 0x50004000, "RTC_IRAM"],
         [0x50000000, 0x50004000, "RTC_DRAM"],
         [0x600FE000, 0x60100000, "MEM_INTERNAL2"],
     ]
 
     def get_pkg_version(self):
         num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 24) & 0x07
+        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 29) & 0x07
 
     def get_minor_chip_version(self):
         num_word = 3
         return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 18) & 0x0F
 
     def get_major_chip_version(self):
         num_word = 3
         return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 22) & 0x03
 
     def get_chip_description(self):
         chip_name = {
-            0: "ESP32-C6 (QFN40)",
-            1: "ESP32-C6FH4 (QFN32)",
+            0: "ESP32-C6",
         }.get(self.get_pkg_version(), "unknown ESP32-C6")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return f"{chip_name} (revision v{major_rev}.{minor_rev})"
 
     def get_chip_features(self):
         return ["WiFi 6", "BT 5", "IEEE802.15.4"]
@@ -130,30 +124,19 @@
         return 40
 
     def override_vddsdio(self, new_voltage):
         raise NotImplementedInROMError(
             "VDD_SDIO overrides are not supported for ESP32-C6"
         )
 
-    def read_mac(self, mac_type="BASE_MAC"):
-        """Read MAC from EFUSE region"""
+    def read_mac(self):
         mac0 = self.read_reg(self.MAC_EFUSE_REG)
         mac1 = self.read_reg(self.MAC_EFUSE_REG + 4)  # only bottom 16 bits are MAC
-        base_mac = struct.pack(">II", mac1, mac0)[2:]
-        ext_mac = struct.pack(">H", (mac1 >> 16) & 0xFFFF)
-        eui64 = base_mac[0:3] + ext_mac + base_mac[3:6]
-        # BASE MAC: 60:55:f9:f7:2c:a2
-        # EUI64 MAC: 60:55:f9:ff:fe:f7:2c:a2
-        # EXT_MAC: ff:fe
-        macs = {
-            "BASE_MAC": tuple(base_mac),
-            "EUI64": tuple(eui64),
-            "MAC_EXT": tuple(ext_mac),
-        }
-        return macs.get(mac_type, None)
+        bitstring = struct.pack(">II", mac1, mac0)[2:]
+        return tuple(bitstring)
 
     def get_flash_crypt_config(self):
         return None  # doesn't exist on ESP32-C6
 
     def get_secure_boot_enabled(self):
         return (
             self.read_reg(self.EFUSE_SECURE_BOOT_EN_REG)
```

### Comparing `esptool-4.6.2/esptool/targets/esp32c6beta.py` & `esptool-4.6.dev1/esptool/targets/esp32c6beta.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
     CHIP_DETECT_MAGIC_VALUE = [0x0DA1806F]
 
     UART_DATE_REG_ADDR = 0x00000500
 
     def get_chip_description(self):
         chip_name = {
-            0: "ESP32-C6 (QFN40)",
-            1: "ESP32-C6FH4 (QFN32)",
+            0: "ESP32-C6",
         }.get(self.get_pkg_version(), "unknown ESP32-C6")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return f"{chip_name} (revision v{major_rev}.{minor_rev})"
 
     def _post_connect(self):
         pass
```

### Comparing `esptool-4.6.2/esptool/targets/esp32h2.py` & `esptool-4.6.dev1/esptool/targets/esp32h2.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,52 +9,38 @@
 class ESP32H2ROM(ESP32C6ROM):
     CHIP_NAME = "ESP32-H2"
     IMAGE_CHIP_ID = 16
 
     # Magic value for ESP32H2
     CHIP_DETECT_MAGIC_VALUE = [0xD7B73E80]
 
-    DR_REG_LP_WDT_BASE = 0x600B1C00
-    RTC_CNTL_WDTCONFIG0_REG = DR_REG_LP_WDT_BASE + 0x0  # LP_WDT_RWDT_CONFIG0_REG
-    RTC_CNTL_WDTWPROTECT_REG = DR_REG_LP_WDT_BASE + 0x001C  # LP_WDT_RWDT_WPROTECT_REG
-
-    RTC_CNTL_SWD_CONF_REG = DR_REG_LP_WDT_BASE + 0x0020  # LP_WDT_SWD_CONFIG_REG
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 18
-    RTC_CNTL_SWD_WPROTECT_REG = DR_REG_LP_WDT_BASE + 0x0024  # LP_WDT_SWD_WPROTECT_REG
-    RTC_CNTL_SWD_WKEY = 0x50D83AA1  # LP_WDT_SWD_WKEY, same as WDT key in this case
-
     FLASH_FREQUENCY = {
         "48m": 0xF,
         "24m": 0x0,
         "16m": 0x1,
         "12m": 0x2,
     }
 
     def get_pkg_version(self):
-        num_word = 4
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 0) & 0x07
-
-    def get_minor_chip_version(self):
-        num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 18) & 0x07
-
-    def get_major_chip_version(self):
         num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 21) & 0x03
+        block1_addr = self.EFUSE_BASE + 0x044
+        word3 = self.read_reg(block1_addr + (4 * num_word))
+        pkg_version = (word3 >> 21) & 0x0F
+        return pkg_version
 
     def get_chip_description(self):
         chip_name = {
             0: "ESP32-H2",
         }.get(self.get_pkg_version(), "unknown ESP32-H2")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return f"{chip_name} (revision v{major_rev}.{minor_rev})"
 
     def get_chip_features(self):
-        return ["BLE", "IEEE802.15.4"]
+        return ["BLE"]
 
     def get_crystal_freq(self):
         # ESP32H2 XTAL is fixed to 32MHz
         return 32
 
 
 class ESP32H2StubLoader(ESP32H2ROM):
```

### Comparing `esptool-4.6.2/esptool/targets/esp32h2beta1.py` & `esptool-4.6.dev1/esptool/targets/esp32h2beta1.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,24 +72,27 @@
         "48m": 0xF,
         "24m": 0x0,
         "16m": 0x1,
         "12m": 0x2,
     }
 
     def get_pkg_version(self):
-        num_word = 4
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 0) & 0x07
+        num_word = 3
+        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 21) & 0x0F
 
     def get_minor_chip_version(self):
-        num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 18) & 0x07
+        hi_num_word = 5
+        hi = (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * hi_num_word)) >> 23) & 0x01
+        low_num_word = 3
+        low = (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * low_num_word)) >> 18) & 0x07
+        return (hi << 3) + low
 
     def get_major_chip_version(self):
-        num_word = 3
-        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 21) & 0x03
+        num_word = 5
+        return (self.read_reg(self.EFUSE_BLOCK1_ADDR + (4 * num_word)) >> 24) & 0x03
 
     def get_chip_description(self):
         chip_name = {
             0: "ESP32-H2",
         }.get(self.get_pkg_version(), "unknown ESP32-H2")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
@@ -102,18 +105,15 @@
         return 32
 
     def override_vddsdio(self, new_voltage):
         raise NotImplementedInROMError(
             "VDD_SDIO overrides are not supported for ESP32-H2"
         )
 
-    def read_mac(self, mac_type="BASE_MAC"):
-        """Read MAC from EFUSE region"""
-        if mac_type != "BASE_MAC":
-            return None
+    def read_mac(self):
         mac0 = self.read_reg(self.MAC_EFUSE_REG)
         mac1 = self.read_reg(self.MAC_EFUSE_REG + 4)  # only bottom 16 bits are MAC
         bitstring = struct.pack(">II", mac1, mac0)[2:]
         return tuple(bitstring)
 
     def get_flash_crypt_config(self):
         return None  # doesn't exist on ESP32-H2
```

### Comparing `esptool-4.6.2/esptool/targets/esp32h2beta2.py` & `esptool-4.6.dev1/esptool/targets/esp32h2beta2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/esptool/targets/esp32s2.py` & `esptool-4.6.dev1/esptool/targets/esp32s2.py`

 * *Files 5% similar despite different names*

```diff
@@ -178,18 +178,15 @@
         return 40
 
     def override_vddsdio(self, new_voltage):
         raise NotImplementedInROMError(
             "VDD_SDIO overrides are not supported for ESP32-S2"
         )
 
-    def read_mac(self, mac_type="BASE_MAC"):
-        """Read MAC from EFUSE region"""
-        if mac_type != "BASE_MAC":
-            return None
+    def read_mac(self):
         mac0 = self.read_reg(self.MAC_EFUSE_REG)
         mac1 = self.read_reg(self.MAC_EFUSE_REG + 4)  # only bottom 16 bits are MAC
         bitstring = struct.pack(">II", mac1, mac0)[2:]
         return tuple(bitstring)
 
     def flash_type(self):
         return (
```

### Comparing `esptool-4.6.2/esptool/targets/esp32s3.py` & `esptool-4.6.dev1/esptool/targets/esp32s3.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,23 +79,18 @@
     PURPOSE_VAL_XTS_AES256_KEY_2 = 3
     PURPOSE_VAL_XTS_AES128_KEY = 4
 
     UARTDEV_BUF_NO = 0x3FCEF14C  # Variable in ROM .bss which indicates the port in use
     UARTDEV_BUF_NO_USB_OTG = 3  # The above var when USB-OTG is used
     UARTDEV_BUF_NO_USB_JTAG_SERIAL = 4  # The above var when USB-JTAG/Serial is used
 
+    RTC_CNTL_WDT_WKEY = 0x50D83AA1
     RTCCNTL_BASE_REG = 0x60008000
-    RTC_CNTL_SWD_CONF_REG = RTCCNTL_BASE_REG + 0x00B4
-    RTC_CNTL_SWD_AUTO_FEED_EN = 1 << 31
-    RTC_CNTL_SWD_WPROTECT_REG = RTCCNTL_BASE_REG + 0x00B8
-    RTC_CNTL_SWD_WKEY = 0x8F1D312A
-
-    RTC_CNTL_WDTCONFIG0_REG = RTCCNTL_BASE_REG + 0x0098
+    RTC_CNTL_WDTCONFIG0_REG = RTCCNTL_BASE_REG + 0x0090
     RTC_CNTL_WDTWPROTECT_REG = RTCCNTL_BASE_REG + 0x00B0
-    RTC_CNTL_WDT_WKEY = 0x50D83AA1
 
     USB_RAM_BLOCK = 0x800  # Max block size USB-OTG is used
 
     GPIO_STRAP_REG = 0x60004038
     GPIO_STRAP_SPI_BOOT_MASK = 0x8  # Not download mode
     RTC_CNTL_OPTION1_REG = 0x6000812C
     RTC_CNTL_FORCE_DOWNLOAD_BOOT_MASK = 0x1  # Is download mode forced over USB?
@@ -209,18 +204,15 @@
         )
 
     def override_vddsdio(self, new_voltage):
         raise NotImplementedInROMError(
             "VDD_SDIO overrides are not supported for ESP32-S3"
         )
 
-    def read_mac(self, mac_type="BASE_MAC"):
-        """Read MAC from EFUSE region"""
-        if mac_type != "BASE_MAC":
-            return None
+    def read_mac(self):
         mac0 = self.read_reg(self.MAC_EFUSE_REG)
         mac1 = self.read_reg(self.MAC_EFUSE_REG + 4)  # only bottom 16 bits are MAC
         bitstring = struct.pack(">II", mac1, mac0)[2:]
         return tuple(bitstring)
 
     def flash_type(self):
         return (
@@ -242,37 +234,27 @@
         """
         Check the UARTDEV_BUF_NO register to see if USB-JTAG/Serial is being used
         """
         if self.secure_download_mode:
             return False  # can't detect USB-JTAG/Serial in secure download mode
         return self.get_uart_no() == self.UARTDEV_BUF_NO_USB_JTAG_SERIAL
 
-    def disable_watchdogs(self):
-        # When USB-JTAG/Serial is used, the RTC WDT and SWD watchdog are not reset
-        # and can then reset the board during flashing. Disable them.
+    def disable_rtc_watchdog(self):
+        # When USB-JTAG/Serial is used, the RTC watchdog is not reset
+        # and can then reset the board during flashing. Disable it.
         if self.uses_usb_jtag_serial():
-            # Disable RTC WDT
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, self.RTC_CNTL_WDT_WKEY)
             self.write_reg(self.RTC_CNTL_WDTCONFIG0_REG, 0)
             self.write_reg(self.RTC_CNTL_WDTWPROTECT_REG, 0)
 
-            # Automatically feed SWD
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, self.RTC_CNTL_SWD_WKEY)
-            self.write_reg(
-                self.RTC_CNTL_SWD_CONF_REG,
-                self.read_reg(self.RTC_CNTL_SWD_CONF_REG)
-                | self.RTC_CNTL_SWD_AUTO_FEED_EN,
-            )
-            self.write_reg(self.RTC_CNTL_SWD_WPROTECT_REG, 0)
-
     def _post_connect(self):
         if self.uses_usb_otg():
             self.ESP_RAM_BLOCK = self.USB_RAM_BLOCK
         if not self.sync_stub_detected:  # Don't run if stub is reused
-            self.disable_watchdogs()
+            self.disable_rtc_watchdog()
 
     def _check_if_can_reset(self):
         """
         Check the strapping register to see if we can reset out of download mode.
         """
         if os.getenv("ESPTOOL_TESTING") is not None:
             print("ESPTOOL_TESTING is set, ignoring strapping mode check")
```

### Comparing `esptool-4.6.2/esptool/targets/esp32s3beta2.py` & `esptool-4.6.dev1/esptool/targets/esp32s3beta2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.6.2/esptool/targets/esp8266.py` & `esptool-4.6.dev1/esptool/targets/esp8266.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,18 +127,16 @@
         """
         Read Chip ID from efuse - the equivalent of the SDK system_get_chip_id() func
         """
         id0 = self.read_reg(self.ESP_OTP_MAC0)
         id1 = self.read_reg(self.ESP_OTP_MAC1)
         return (id0 >> 24) | ((id1 & 0xFFFFFF) << 8)
 
-    def read_mac(self, mac_type="BASE_MAC"):
+    def read_mac(self):
         """Read MAC from OTP ROM"""
-        if mac_type != "BASE_MAC":
-            return None
         mac0 = self.read_reg(self.ESP_OTP_MAC0)
         mac1 = self.read_reg(self.ESP_OTP_MAC1)
         mac3 = self.read_reg(self.ESP_OTP_MAC3)
         if mac3 != 0:
             oui = ((mac3 >> 16) & 0xFF, (mac3 >> 8) & 0xFF, mac3 & 0xFF)
         elif ((mac1 >> 16) & 0xFF) == 0:
             oui = (0x18, 0xFE, 0x34)
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'GOv8P9jnC0Bx6AtA8+wLQO3oC0CP6AtA7egLQEnpC0AG6gtAeOoLQCHqC0CB5wtAo+kLQPjpC0Bn6QtAmuoLQI7pC0Ca6gtAXegLQLPoC0Dt6AtASekLQHfoC0BM6wtAs+wLQKXmC0DX7AtApeYLQKXmC0Cl5gtApeYLQKXmC0Cl5gtApeYLQKXmC0Dz6gtApeYLQM3rC0Cz7AtA'",*

 * * "'text'": "'CAD0PxwA9D8AAPQ/AMD8PxAA9D82QQAh+v/AIAA4AkH5/8AgACgEICB0nOIGBQAAAEH1/4H2/8AgAKgEiAigoHTgCAALImYC54b0/yHx/8AgADkCHfAAAKDr/T8Ya/0/hIAAAEBAAABYq/0/pOv9PzZBALH5/yCgdBARIKXHAJYaBoH2/5KhAZCZEZqYwCAAuAmR8/+goHSaiMAgAJIYAJCQ9BvJwMD0wCAAwlgAmpvAIACiSQDAIACSGACB6v+QkPSAgPSHmUeB5f+SoQ […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "DMD8P9jnC0Br6AtAA+0LQPLoC0CL6AtA8ugLQFHpC0Ae6gtAkOoLQDnqC0CB5wtAtukLQBDqC0B06QtAtOoLQJ7pC0C06gtAWegLQLboC0Dy6AtAUekLQHHoC0Bk6wtAxewLQKTmC0Dn7AtApOYLQKTmC0Ck5gtApOYLQKTmC0Ck5gtApOYLQKTmC0AL6wtApOYLQOXrC0DF7AtA",
+    "data": "GOv8P9jnC0Bx6AtA8+wLQO3oC0CP6AtA7egLQEnpC0AG6gtAeOoLQCHqC0CB5wtAo+kLQPjpC0Bn6QtAmuoLQI7pC0Ca6gtAXegLQLPoC0Dt6AtASekLQHfoC0BM6wtAs+wLQKXmC0DX7AtApeYLQKXmC0Cl5gtApeYLQKXmC0Cl5gtApeYLQKXmC0Dz6gtApeYLQM3rC0Cz7AtA",
     "data_start": 1073605544,
     "entry": 1074521560,
-    "text": "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",
+    "text": "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",
     "text_start": 1074520064
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c2.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'GGvKP+AIOEAsCThAhAk4QCgKOECUCjhAQgo4QKgHOEDkCThAJAo4QJgJOEBYBzhAzAk4QFgHOEC6CDhA/gg4QCwJOECECThAzAg4QBIIOEBCCDhAyAg4QOYMOEAsCThArAs4QJoMOECkBjhAxAw4QKQGOECkBjhApAY4QKQGOECkBjhApAY4QKQGOECkBjhASAs4QKQGOEDICzhAmgw4QA=='",*

 * * "'text'": "'ARG3BwBgTsaDqYcASsg3Sco/JspSxAbOIsy3BABgfVoTCQkAwEwTdPQ/DeDyQGJEI6g0AUJJ0kSySSJKBWGCgIhAgycJABN19Q+Cl30U4xlE/8m/EwcADJRBqodjGOUAhUeFxiOgBQB5VYKABUdjh+YACUZjjcYAfVWCgEIFEwewDUGFY5XnAolHnMH1t5MGwA1jFtUAmMETBQAMgoCTBtANfVVjldcAmMETBbANgoC3dcs/QRGThQW6BsZhP2NFBQa3d8s/k4 […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "DEDKP+AIOEAsCThAhAk4QCgKOECUCjhAQgo4QKgHOEDkCThAJAo4QJgJOEBYBzhAzAk4QFgHOEC6CDhA/gg4QCwJOECECThAzAg4QBIIOEBCCDhAyAg4QOwMOEAsCThArAs4QKAMOECkBjhAygw4QKQGOECkBjhApAY4QKQGOECkBjhApAY4QKQGOECkBjhASAs4QKQGOEDICzhAoAw4QA==",
+    "data": "GGvKP+AIOEAsCThAhAk4QCgKOECUCjhAQgo4QKgHOEDkCThAJAo4QJgJOEBYBzhAzAk4QFgHOEC6CDhA/gg4QCwJOECECThAzAg4QBIIOEBCCDhAyAg4QOYMOEAsCThArAs4QJoMOECkBjhAxAw4QKQGOECkBjhApAY4QKQGOECkBjhApAY4QKQGOECkBjhASAs4QKQGOEDICzhAmgw4QA==",
     "data_start": 1070295976,
     "entry": 1077413304,
-    "text": "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",
+    "text": "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",
     "text_start": 1077411840
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c3.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c3.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'IGvIP1YKOECmCjhA/go4QKILOEAODDhAvAs4QCIJOEBeCzhAngs4QBILOEDSCDhARgs4QNIIOEAwCjhAdgo4QKYKOED+CjhAQgo4QIYJOEC2CThAPgo4QGAOOECmCjhAJg04QBgOOEASCDhAQA44QBIIOEASCDhAEgg4QBIIOEASCDhAEgg4QBIIOEASCDhAwgw4QBIIOEBEDThAGA44QA=='",*

 * * "'text'": "'QREixCbCBsa3NwRgEUc3RMg/2Mu3NARgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDdJyD8mylLEBs4izLcEAGB9WhMJCQDATBN09D8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kw […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "FEDIP3YKOEDGCjhAHgs4QMILOEAuDDhA3As4QEIJOEB+CzhAvgs4QDILOEDyCDhAZgs4QPIIOEBQCjhAlgo4QMYKOEAeCzhAYgo4QKYJOEDWCThAXgo4QIYOOEDGCjhARg04QD4OOEAyCDhAZg44QDIIOEAyCDhAMgg4QDIIOEAyCDhAMgg4QDIIOEAyCDhA4gw4QDIIOEBkDThAPg44QA==",
+    "data": "IGvIP1YKOECmCjhA/go4QKILOEAODDhAvAs4QCIJOEBeCzhAngs4QBILOEDSCDhARgs4QNIIOEAwCjhAdgo4QKYKOED+CjhAQgo4QIYJOEC2CThAPgo4QGAOOECmCjhAJg04QBgOOEASCDhAQA44QBIIOEASCDhAEgg4QBIIOEASCDhAEgg4QBIIOEASCDhAwgw4QBIIOEBEDThAGA44QA==",
     "data_start": 1070164912,
     "entry": 1077413532,
-    "text": "QREixCbCBsa3NwRgEUc3RMg/2Mu3NARgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDdJyD8mylLEBs4izLcEAGB9WhMJCQDATBN09D8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kwbADWMW1QCYwRMFAAyCgJMG0A19VWOV1wCYwRMFsA2CgLd1yT9BEZOFhboGxmE/Y0UFBrd3yT+ThweyA6cHCAPWRwgTdfUPkwYWAMIGwYIjktcIMpcjAKcAA9dHCJFnk4cHBGMe9wI398g/EwcHsqFnupcDpgcItzbJP7d3yT+Thweyk4YGtmMf5gAjpscII6DXCCOSBwghoPlX4wb1/LJAQQGCgCOm1wgjoOcI3bc3JwBgfEudi/X/NzcAYHxLnYv1/4KAQREGxt03tycAYCOmBwI3BwAImMOYQ33/yFeyQBNF9f8FiUEBgoBBEQbG2T993TcHAEC3JwBgmMM3JwBgHEP9/7JAQQGCgEERIsQ3xMg/kwdEAUrAA6kHAQbGJsJjCgkERTc5xb1HEwREAYFEY9YnAQREvYiTtBQAfTeFPxxENwaAABOXxwCZ4DcGAAG39v8AdY+3JgBg2MKQwphCff9BR5HgBUczCelAupcjKCQBHMSyQCJEkkQCSUEBgoABEQbOIswlNzcEzj9sABMFRP+XAMj/54Ag8KqHBUWV57JHk/cHID7GiTc3JwBgHEe3BkAAEwVE/9WPHMeyRZcAyP/ngKDtMzWgAPJAYkQFYYKAQRG3x8g/BsaTh0cBBUcjgOcAE9fFAJjHBWd9F8zDyMf5jTqVqpWxgYzLI6oHAEE3GcETBVAMskBBAYKAAREizDfEyD+TB0QBJsrER07GBs5KyKqJEwREAWPzlQCuhKnAAylEACaZE1nJABxIY1XwABxEY175ArU9fd1IQCaGzoWXAMj/54Ag4RN19Q8BxZMHQAxcyFxAppdcwFxEhY9cxPJAYkTSREJJskkFYYKAaTVtv0ERBsaXAMj/54AA1gNFhQGyQHUVEzUVAEEBgoBBEQbGxTcdyTdHyD8TBwcAXEONxxBHHcK3BgxgmEYNinGbUY+YxgVmuE4TBgbA8Y99dhMG9j9xj9mPvM6yQEEBgoBBEQbGeT8RwQ1FskBBARcDyP9nAIPMQREGxpcAyP/ngEDKQTcBxbJAQQHZv7JAQQGCgEERBsYTBwAMYxrlABMFsA3RPxMFwA2yQEEB6bcTB7AN4xvl/sE3EwXQDfW3QREixCbCBsYqhLMEtQBjF5QAskAiRJJEQQGCgANFBAAFBE0/7bc1cSbLTsf9coVp/XQizUrJUsVWwwbPk4SE+haRk4cJB6aXGAizhOcAKokmhS6ElwDI/+eAgBuThwkHGAgFarqXs4pHQTHkBWd9dZMFhfqTBwcHEwWF+RQIqpczhdcAkwcHB66Xs4XXACrGlwDI/+eAQBgyRcFFlTcBRYViFpH6QGpE2kRKSbpJKkqaSg1hgoCiiWNzigCFaU6G1oVKhZcAyP/ngEDGE3X1DwHtTobWhSaFlwDI/+eAgBNOmTMENEFRtxMFMAZVvxMFAAzZtTFx/XIFZ07XUtVW017PBt8i3SbbStla0WLNZstqyW7H/XcWkRMHBwc+lxwIupc+xiOqB/iqiS6Ksoq2ixE9kwcAAhnBtwcCAD6FlwDI/+eAIAyFZ2PlVxMFZH15EwmJ+pMHBAfKlxgIM4nnAEqFlwDI/+eAoAp9exMMO/mTDIv5EwcEB5MHBAcUCGKX5peBRDMM1wCzjNcAUk1jfE0JY/GkA0GomT+ihQgBjTW5NyKGDAFKhZcAyP/ngIAGopmilGP1RAOzh6RBY/F3AzMEmkBj84oAVoQihgwBToWXAMj/54CAtRN19Q9V3QLMAUR5XY1NowkBAGKFlwDI/+eAwKd9+QNFMQHmhWE0Y08FAOPijf6FZ5OHBweilxgIupfalyOKp/gFBPG34xWl/ZFH4wX09gVnfXWTBwcHkwWF+hMFhfkUCKqXM4XXAJMHBweul7OF1wAqxpcAyP/ngKD8cT0yRcFFZTNRPeUxtwcCABnhkwcAAj6FlwDI/+eAoPmFYhaR+lBqVNpUSlm6WSpamloKW/pLakzaTEpNuk0pYYKAt1dBSRlxk4f3hAFFht6i3KbaytjO1tLU1tLa0N7O4szmyurI7sY+zpcAyP/ngICfQTENzbcEDGCcRDdEyD8TBAQAHMS8TH13Ewf3P1zA+Y+T5wdAvMwTBUAGlwDI/+eAoJUcRPGbk+cXAJzEkTEhwbeHAGA3R9hQk4aHChMHF6qYwhOHBwkjIAcANzcdjyOgBgATB6cSk4YHC5jCk4fHCphDNwYAgFGPmMMjoAYAt0fIPzd3yT+ThwcAEwcHuyGgI6AHAJEH4+3n/kE7kUVoCHE5YTO398g/k4cHsiFnPpcjIPcItwc4QDdJyD+Th4cOIyD5ALd5yT9lPhMJCQCTiQmyYwsFELcnDGBFR7jXhUVFRZcAyP/ngCDjtwU4QAFGk4UFAEVFlwDI/+eAIOQ3NwRgHEs3BQIAk+dHABzLlwDI/+eAIOOXAMj/54Cg87dHAGCcXwnl8YvhFxO1FwCBRZcAyP/ngICWwWe3xMg//RcTBwAQhWZBZrcFAAEBRZOERAG3Ssg/DWqXAMj/54AAkROLSgEmmoOnyQj134OryQiFRyOmCQgjAvECg8cbAAlHIxPhAqMC8QIC1E1HY4HnCFFHY4/nBilHY5/nAIPHOwADxysAogfZjxFHY5bnAIOniwCcQz7UlTmhRUgQQTaDxzsAA8crAKIH2Y8RZ0EHY3T3BBMFsA05PhMFwA0hPhMF4A4JPpkxQbe3BThAAUaThYUDFUWXAMj/54BA1DcHAGBcRxMFAAKT5xcQXMcJt8lHIxPxAk23A8cbANFGY+fmAoVGY+bmAAFMEwTwD4WoeRcTd/cPyUbj6Ob+t3bJPwoHk4ZGuzaXGEMCh5MGBwOT9vYPEUbjadb8Ewf3AhN39w+NRmPr5gi3dsk/CgeThgbANpcYQwKHEwdAAmOY5xAC1B1EAUWFPAFFYTRFNnk+oUVIEH0UZTR19AFMAUQTdfQPhTwTdfwPrTRJNuMeBOqDxxsASUdjY/cuCUfjdvfq9ReT9/cPPUfjYPfqN3fJP4oHEwcHwbqXnEOChwVEnetwEIFFAUWXsMz/54CgAh3h0UVoEKk0AUQxqAVEge+X8Mf/54CAdTM0oAApoCFHY4XnAAVEAUxhtwOsiwADpMsAs2eMANIH9ffv8H+FffHBbCKc/Rx9fTMFjEBV3LN3lQGV48FsMwWMQGPmjAL9fDMFjEBV0DGBl/DH/+eAgHBV+WaU9bcxgZfwx//ngIBvVfFqlNG3QYGX8Mf/54BAblH5MwSUQcG3IUfjiefwAUwTBAAMMbdBR82/QUcFROOc5/aDpcsAA6WLAHU6sb9BRwVE45Ln9gOnCwGRZ2Pl5xyDpUsBA6WLAO/wv4A1v0FHBUTjkuf0g6cLARFnY2X3GgOnywCDpUsBA6WLADOE5wLv8C/+I6wEACMkirAxtwPHBABjDgcQA6eLAMEXEwQADGMT9wDASAFHkwbwDmNG9wKDx1sAA8dLAAFMogfZjwPHawBCB12Pg8d7AOIH2Y/jgfbmEwQQDKm9M4brAANGhgEFB7GO4beDxwQA8cPcRGOYBxLASCOABAB9tWFHY5bnAoOnywEDp4sBg6ZLAQOmCwGDpcsAA6WLAJfwx//ngEBeKowzNKAAKbUBTAVEEbURRwVE45rn5gOliwCBRZfwx//ngABfkbUT9/cA4xoH7JPcRwAThIsAAUx9XeN5nN1IRJfwx//ngIBLGERUQBBA+Y5jB6cBHEITR/f/fY/ZjhTCBQxBBNm/EUdJvUFHBUTjnOfgg6eLAAOnSwEjKPkAIybpAN2zgyXJAMEXkeWJzwFMEwRgDLW7AycJAWNm9wYT9zcA4x4H5AMoCQEBRgFHMwXoQLOG5QBjafcA4wkG1CMoqQAjJtkAmbMzhusAEE4RB5DCBUbpvyFHBUTjlufaAyQJARnAEwSADCMoCQAjJgkAMzSAAEm7AUwTBCAMEbsBTBMEgAwxswFMEwSQDBGzEwcgDWOD5wwTB0AN45DnvAPEOwCDxysAIgRdjJfwx//ngGBJA6zEAEEUY3OEASKM4w4MuMBAYpQxgJxIY1XwAJxEY1v0Cu/wD8513chAYoaThYsBl/DH/+eAYEUBxZMHQAzcyNxA4pfcwNxEs4eHQdzEl/DH/+eAQESJvgllEwUFcQOsywADpIsAl/DH/+eAADa3BwBg2Eu3BgABwRaTV0cBEgd1j72L2Y+zh4cDAUWz1YcCl/DH/+eA4DYTBYA+l/DH/+eAoDIRtoOmSwEDpgsBg6XLAAOliwDv8M/7/bSDxTsAg8crABOFiwGiBd2NwRXv8O/X2bzv8E/HPb8DxDsAg8crABOMiwEiBF2M3ERBFM3jkUeFS2P/hwiTB5AM3MhttAOnDQAi0AVIs4fsQD7WgyeKsGNz9AANSELGOsTv8M/CIkcySDfFyD/ihXwQk4ZKARAQEwXFApfwx//ngEAzN/fIP5MIRwGCVwOniLCDpQ0AHYwdjz6cslcjpOiwqou+lSOgvQCTh0oBnY0BxaFnY5f1AFqF7/CPzSOgbQEJxNxEmcPjT3D3Y98LAJMHcAy9t4VLt33JP7fMyD+TjQ27k4xMAem/45ILoNxE448HnpMHgAypt4OniwDjmAee7/BP1gllEwUFcZfwx//ngAAg7/AP0Zfwx//ngEAj+bIDpMsA4wQEnO/wz9MTBYA+l/DH/+eAoB3v8K/OApR9su/wL872UGZU1lRGWbZZJlqWWgZb9ktmTNZMRk22TQlhgoA=",
+    "text": "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",
     "text_start": 1077411840
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c6.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'HCuEQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA=='",*

 * * "'text'": "'QREixCbCBsa39wBgEUc3BIRA2Mu39ABgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDcJhEAmylLEBs4izLcEAGB9WhMJCQDATBN09A8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kw […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "EACEQEIKgECSCoBA6gqAQI4LgED6C4BAqAuAQA4JgEBKC4BAiguAQP4KgEC+CIBAMguAQL4IgEAcCoBAYgqAQJIKgEDqCoBALgqAQHIJgECiCYBAKgqAQFIOgECSCoBAEg2AQAoOgED+B4BAMg6AQP4HgED+B4BA/geAQP4HgED+B4BA/geAQP4HgED+B4BArgyAQP4HgEAwDYBACg6AQA==",
+    "data": "HCuEQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA==",
     "data_start": 1082469292,
     "entry": 1082132112,
-    "text": "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",
+    "text": "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",
     "text_start": 1082130432
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32c6beta.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'GGvIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QP4MOEBECThAxAs4QLIMOEC8BjhA3Aw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAsgw4QA=='",*

 * * "'text'": "'ARG3BwBgTsaDqYcASsg3Scg/JspSxAbOIsy3BABgfVoTCQkAwEwTdPQ/DeDyQGJEI6g0AUJJ0kSySSJKBWGCgIhAgycJABN19Q+Cl30U4xlE/8m/EwcADJRBqodjGOUAhUeFxiOgBQB5VYKABUdjh+YACUZjjcYAfVWCgEIFEwewDUGFY5XnAolHnMH1t5MGwA1jFtUAmMETBQAMgoCTBtANfVVjldcAmMETBbANgoC3dck/QRGThQW6BsZhP2NFBQa3d8k/k4 […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "DEDIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QAQNOEBECThAxAs4QLgMOEC8BjhA4gw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAuAw4QA==",
+    "data": "GGvIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QP4MOEBECThAxAs4QLIMOEC8BjhA3Aw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAsgw4QA==",
     "data_start": 1070164904,
     "entry": 1077413318,
-    "text": "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",
+    "text": "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",
     "text_start": 1077411840
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32h2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'HCuDQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA=='",*

 * * "'text'": "'QREixCbCBsa39wBgEUc3BINA2Mu39ABgEwQEANxAkYuR57JAIkSSREEBgoCIQBxAE3X1D4KX3bcBEbcHAGBOxoOphwBKyDcJg0AmylLEBs4izLcEAGB9WhMJCQDATBN09A8N4PJAYkQjqDQBQknSRLJJIkoFYYKAiECDJwkAE3X1D4KXfRTjGUT/yb8TBwAMlEGqh2MY5QCFR4XGI6AFAHlVgoAFR2OH5gAJRmONxgB9VYKAQgUTB7ANQYVjlecCiUecwfW3kw […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "EACDQEIKgECSCoBA6gqAQI4LgED6C4BAqAuAQA4JgEBKC4BAiguAQP4KgEC+CIBAMguAQL4IgEAcCoBAYgqAQJIKgEDqCoBALgqAQHIJgECiCYBAKgqAQFIOgECSCoBAEg2AQAoOgED+B4BAMg6AQP4HgED+B4BA/geAQP4HgED+B4BA/geAQP4HgED+B4BArgyAQP4HgEAwDYBACg6AQA==",
+    "data": "HCuDQCoKgEB6CoBA0gqAQHYLgEDiC4BAkAuAQPYIgEAyC4BAcguAQOYKgECmCIBAGguAQKYIgEAECoBASgqAQHoKgEDSCoBAFgqAQFoJgECKCYBAEgqAQDQOgEB6CoBA+gyAQOwNgEDmB4BAFA6AQOYHgEDmB4BA5geAQOYHgEDmB4BA5geAQOYHgEDmB4BAlgyAQOYHgEAYDYBA7A2AQA==",
     "data_start": 1082403756,
     "entry": 1082132112,
-    "text": "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",
+    "text": "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",
     "text_start": 1082130432
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'GGvIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QP4MOEBECThAxAs4QLIMOEC8BjhA3Aw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAsgw4QA=='",*

 * * "'text'": "'ARG3BwBgTsaDqYcASsg3Scg/JspSxAbOIsy3BABgfVoTCQkAwEwTdPQ/DeDyQGJEI6g0AUJJ0kSySSJKBWGCgIhAgycJABN19Q+Cl30U4xlE/8m/EwcADJRBqodjGOUAhUeFxiOgBQB5VYKABUdjh+YACUZjjcYAfVWCgEIFEwewDUGFY5XnAolHnMH1t5MGwA1jFtUAmMETBQAMgoCTBtANfVVjldcAmMETBbANgoC3dck/QRGThQW6BsZhP2NFBQa3d8k/k4 […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "DEDIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QAQNOEBECThAxAs4QLgMOEC8BjhA4gw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAuAw4QA==",
+    "data": "GGvIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QP4MOEBECThAxAs4QLIMOEC8BjhA3Aw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAsgw4QA==",
     "data_start": 1070164904,
     "entry": 1077413318,
-    "text": "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",
+    "text": "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",
     "text_start": 1077411840
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32c6beta.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'GGvIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QP4MOEBECThAxAs4QLIMOEC8BjhA3Aw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAsgw4QA=='",*

 * * "'text'": "'ARG3BwBgTsaDqYcASsg3Scg/JspSxAbOIsy3BABgfVoTCQkAwEwTdPQ/DeDyQGJEI6g0AUJJ0kSySSJKBWGCgIhAgycJABN19Q+Cl30U4xlE/8m/EwcADJRBqodjGOUAhUeFxiOgBQB5VYKABUdjh+YACUZjjcYAfVWCgEIFEwewDUGFY5XnAolHnMH1t5MGwA1jFtUAmMETBQAMgoCTBtANfVVjldcAmMETBbANgoC3dck/QRGThQW6BsZhP2NFBQa3d8k/k4 […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "DEDIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QAQNOEBECThAxAs4QLgMOEC8BjhA4gw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAuAw4QA==",
+    "data": "GGvIP/gIOEBECThAnAk4QEAKOECsCjhAWgo4QMAHOED8CThAPAo4QLAJOEBwBzhA5Ak4QHAHOEDSCDhAFgk4QEQJOECcCThA5Ag4QCoIOEBaCDhA4Ag4QP4MOEBECThAxAs4QLIMOEC8BjhA3Aw4QLwGOEC8BjhAvAY4QLwGOEC8BjhAvAY4QLwGOEC8BjhAYAs4QLwGOEDgCzhAsgw4QA==",
     "data_start": 1070164904,
     "entry": 1077413318,
-    "text": "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",
+    "text": "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",
     "text_start": 1077411840
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32s2.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s2.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'ZCv9PzaLAkDBiwJAhpACQEqMAkDjiwJASowCQKmMAkByjQJA5Y0CQI2NAkDAigJAC40CQGSNAkDMjAJACI4CQPaMAkAIjgJAr4sCQA6MAkBKjAJAqYwCQMeLAkACiwJAx44CQD2QAkDYiQJAZZACQNiJAkDYiQJA2IkCQNiJAkDYiQJA2IkCQNiJAkDYiQJAZI4CQNiJAkBZjwJAPZACQA=='",*

 * * "'text'": "'CAAAYBwAAGBIAP0/EAAAYDZBACH7/8AgADgCQfr/wCAAKAQgIJSc4kH4/0YEAAw4MIgBwCAAqAiIBKCgdOAIAAsiZgLohvT/IfH/wCAAOQId8AAA7Cv+P2Sr/T+EgAAAQEAAAKTr/T/wK/4/NkEAsfn/IKB0EBEgZQEBlhoGgfb/kqEBkJkRmpjAIAC4CZHz/6CgdJqIwCAAkhgAkJD0G8nAwPTAIADCWACam8AgAKJJAMAgAJIYAIHq/5CQ9ICA9IeZR4Hl/5 […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "WAD9PzeLAkDJiwJAjpACQFKMAkDqiwJAUowCQLGMAkB6jQJA7Y0CQJWNAkDBigJAE40CQGyNAkDUjAJAEI4CQP6MAkAQjgJAt4sCQBaMAkBSjAJAsYwCQM+LAkADiwJA044CQEaQAkDWiQJAbZACQNaJAkDWiQJA1okCQNaJAkDWiQJA1okCQNaJAkDWiQJAcI4CQNaJAkBljwJARpACQA==",
+    "data": "ZCv9PzaLAkDBiwJAhpACQEqMAkDjiwJASowCQKmMAkByjQJA5Y0CQI2NAkDAigJAC40CQGSNAkDMjAJACI4CQPaMAkAIjgJAr4sCQA6MAkBKjAJAqYwCQMeLAkACiwJAx44CQD2QAkDYiQJAZZACQNiJAkDYiQJA2IkCQNiJAkDYiQJA2IkCQNiJAkDYiQJAZI4CQNiJAkBZjwJAPZACQA==",
     "data_start": 1073622012,
     "entry": 1073907696,
-    "text": "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",
+    "text": "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",
     "text_start": 1073905664
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_32s3.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_32s3.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {"'data'": "'ZCvKP5aNN0B7jjdAPJM3QAaPN0CbjjdABo83QGWPN0AykDdApZA3QE2QN0AhjTdAyI83QCSQN0CIjzdAx5A3QLKPN0DHkDdAaY43QMaON0AGjzdAZY83QIGON0BijTdAiJE3QAKTN0A+jDdAIpM3QD6MN0A+jDdAPow3QD6MN0A+jDdAPow3QD6MN0A+jDdAIpE3QD6MN0AdkjdAApM3QAQInwAAAAAAAAAYAQQIBQAAAAAAAAAIAQQIBgAAAAAAAAAAAQQIIQAAAAAAIAAAEQQI3AAAAAAAIAAAEQQIDAAAAAAAIAAAAQQIEgAAAAAAIAAAESAoDAAQAQAA'",*

 * * "'entry'": '1077381684',*

 * * "'text'": "'FIADYACAA2BIAMo/BIADYDZBAIH7/wxJwCAAmQjGBAAAgfj/wCAAqAiB9/+goHSICOAIACH2/8AgAIgCJ+jhHfAAAAAIAABgHAAAYBAAAGA2QQAh/P/AIAA4 […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "WADKP8mNN0C/jjdAiJM3QEuPN0DfjjdAS483QKqPN0B3kDdA6ZA3QJKQN0BVjTdAC5A3QGmQN0DNjzdAC5E3QPaPN0ALkTdArY43QAyPN0BLjzdAqo83QMWON0CXjTdA0JE3QE6TN0BujDdAbpM3QG6MN0BujDdAbow3QG6MN0BujDdAbow3QG6MN0BujDdAapE3QG6MN0BlkjdATpM3QAQInwAAAAAAAAAYAQQIBQAAAAAAAAAIAQQIBgAAAAAAAAAAAQQIIQAAAAAAIAAAEQQI3AAAAAAAIAAAEQQIDAAAAAAAIAAAAQQIEgAAAAAAIAAAESAoDAAQAQAA",
+    "data": "ZCvKP5aNN0B7jjdAPJM3QAaPN0CbjjdABo83QGWPN0AykDdApZA3QE2QN0AhjTdAyI83QCSQN0CIjzdAx5A3QLKPN0DHkDdAaY43QMaON0AGjzdAZY83QIGON0BijTdAiJE3QAKTN0A+jDdAIpM3QD6MN0A+jDdAPow3QD6MN0A+jDdAPow3QD6MN0A+jDdAIpE3QD6MN0AdkjdAApM3QAQInwAAAAAAAAAYAQQIBQAAAAAAAAAIAQQIBgAAAAAAAAAAAQQIIQAAAAAAIAAAEQQI3AAAAAAAIAAAEQQIDAAAAAAAIAAAAQQIEgAAAAAAIAAAESAoDAAQAQAA",
     "data_start": 1070279668,
-    "entry": 1077381696,
-    "text": "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",
+    "entry": 1077381684,
+    "text": "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",
     "text_start": 1077379072
 }
```

### Comparing `esptool-4.6.2/esptool/targets/stub_flasher/stub_flasher_8266.json` & `esptool-4.6.dev1/esptool/targets/stub_flasher/stub_flasher_8266.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data'": "'CIH+PwUFBAACAwcAAwMLALnXEEDv1xBAHdgQQLrYEEBo5xBAHtkQQHTZEEDA2RBAaOcQQILaEED/2hBAwNsQQGjnEEBo5xBAWNwQQGjnEEA33xBAAOAQQDvgEEBo5xBAaOcQQNfgEEBo5xBAv+EQQGXiEECj4xBAY+QQQDTlEEBo5xBAaOcQQGjnEEBo5xBAYuYQQGjnEEBX5xBAkN0QQI/YEECm5RBAq9oQQPzZEEBo5xBA7OYQQDHnEEBo5xBAaOcQQGjnEEBo5xBAaOcQQGjnEEBo5xBAaOcQQCLaEEBf2hBAvuUQQAEAAAACAAAAAwAAAAQAAAAFAAAABwAAAAkAAAANAAAAEQAAABkAAAAhAAAAMQAAAEEAAABhAAAAgQAAAMEAAAABAQAAgQEAAAECAAABAwAAAQQAAAEGAAABCAAAAQwAAAEQAAABGAAAASAAAAEwAAABQAAAAWAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA […]*

```diff
@@ -1,7 +1,7 @@
 {
-    "data": "CIH+PwUFBAACAwcAAwMLANTXEEAL2BBAOdgQQNbYEECF5xBAOtkQQJDZEEDc2RBAhecQQKLaEEAf2xBA4NsQQIXnEECF5xBAeNwQQIXnEEBV3xBAHOAQQFfgEECF5xBAhecQQPPgEECF5xBA2+EQQIHiEEDA4xBAf+QQQFDlEECF5xBAhecQQIXnEECF5xBAfuYQQIXnEEB05xBAsN0QQKnYEEDC5RBAydoQQBvaEECF5xBACOcQQE/nEECF5xBAhecQQIXnEECF5xBAhecQQIXnEECF5xBAhecQQELaEEB/2hBA2uUQQAEAAAACAAAAAwAAAAQAAAAFAAAABwAAAAkAAAANAAAAEQAAABkAAAAhAAAAMQAAAEEAAABhAAAAgQAAAMEAAAABAQAAgQEAAAECAAABAwAAAQQAAAEGAAABCAAAAQwAAAEQAAABGAAAASAAAAEwAAABQAAAAWAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEAAAABAAAAAgAAAAIAAAADAAAAAwAAAAQAAAAEAAAABQAAAAUAAAAGAAAABgAAAAcAAAAHAAAACAAAAAgAAAAJAAAACQAAAAoAAAAKAAAACwAAAAsAAAAMAAAADAAAAA0AAAANAAAAAAAAAAAAAAADAAAABAAAAAUAAAAGAAAABwAAAAgAAAAJAAAACgAAAAsAAAANAAAADwAAABEAAAATAAAAFwAAABsAAAAfAAAAIwAAACsAAAAzAAAAOwAAAEMAAABTAAAAYwAAAHMAAACDAAAAowAAAMMAAADjAAAAAgEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAQAAAAEAAAABAAAAAgAAAAIAAAACAAAAAgAAAAMAAAADAAAAAwAAAAMAAAAEAAAABAAAAAQAAAAEAAAABQAAAAUAAAAFAAAABQAAAAAAAAAAAAAAAAAAABAREgAIBwkGCgULBAwDDQIOAQ8AAQEAAAEAAAAEAAAA",
+    "data": "CIH+PwUFBAACAwcAAwMLALnXEEDv1xBAHdgQQLrYEEBo5xBAHtkQQHTZEEDA2RBAaOcQQILaEED/2hBAwNsQQGjnEEBo5xBAWNwQQGjnEEA33xBAAOAQQDvgEEBo5xBAaOcQQNfgEEBo5xBAv+EQQGXiEECj4xBAY+QQQDTlEEBo5xBAaOcQQGjnEEBo5xBAYuYQQGjnEEBX5xBAkN0QQI/YEECm5RBAq9oQQPzZEEBo5xBA7OYQQDHnEEBo5xBAaOcQQGjnEEBo5xBAaOcQQGjnEEBo5xBAaOcQQCLaEEBf2hBAvuUQQAEAAAACAAAAAwAAAAQAAAAFAAAABwAAAAkAAAANAAAAEQAAABkAAAAhAAAAMQAAAEEAAABhAAAAgQAAAMEAAAABAQAAgQEAAAECAAABAwAAAQQAAAEGAAABCAAAAQwAAAEQAAABGAAAASAAAAEwAAABQAAAAWAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEAAAABAAAAAgAAAAIAAAADAAAAAwAAAAQAAAAEAAAABQAAAAUAAAAGAAAABgAAAAcAAAAHAAAACAAAAAgAAAAJAAAACQAAAAoAAAAKAAAACwAAAAsAAAAMAAAADAAAAA0AAAANAAAAAAAAAAAAAAADAAAABAAAAAUAAAAGAAAABwAAAAgAAAAJAAAACgAAAAsAAAANAAAADwAAABEAAAATAAAAFwAAABsAAAAfAAAAIwAAACsAAAAzAAAAOwAAAEMAAABTAAAAYwAAAHMAAACDAAAAowAAAMMAAADjAAAAAgEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAQAAAAEAAAABAAAAAgAAAAIAAAACAAAAAgAAAAMAAAADAAAAAwAAAAMAAAAEAAAABAAAAAQAAAAEAAAABQAAAAUAAAAFAAAABQAAAAAAAAAAAAAAAAAAABAREgAIBwkGCgULBAwDDQIOAQ8AAQEAAAEAAAAEAAAA",
     "data_start": 1073720488,
     "entry": 1074843652,
-    "text": "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",
+    "text": "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",
     "text_start": 1074843648
 }
```

### Comparing `esptool-4.6.2/esptool/util.py` & `esptool-4.6.dev1/esptool/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: 2014-2022 Fredrik Ahlberg, Angus Gratton,
 # Espressif Systems (Shanghai) CO LTD, other contributors as noted.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
-import os
 import re
 import struct
 import sys
 
 
 def byte(bitstr, index):
     return bitstr[index]
@@ -84,23 +83,14 @@
 
 
 def strip_chip_name(chip_name):
     """Strip chip name to normalized form, e.g. `ESP32-S3(beta2)` -> `esp32s3beta2`"""
     return re.sub(r"[-()]", "", chip_name.lower())
 
 
-def get_file_size(path_to_file):
-    """Returns the file size in bytes"""
-    file_size = 0
-    with open(path_to_file, "rb") as f:
-        f.seek(0, os.SEEK_END)
-        file_size = f.tell()
-    return file_size
-
-
 class FatalError(RuntimeError):
     """
     Wrapper class for runtime errors that aren't caused by internal bugs, but by
     ESP ROM responses or input content.
     """
 
     def __init__(self, message):
```

### Comparing `esptool-4.6.2/esptool.egg-info/PKG-INFO` & `esptool-4.6.dev1/esptool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 Metadata-Version: 2.1
 Name: esptool
-Version: 4.6.2
+Version: 4.6.dev1
 Summary: A serial utility to communicate & flash code to Espressif chips.
 Home-page: https://github.com/espressif/esptool/
 Author: Fredrik Ahlberg (themadinventor) & Angus Gratton (projectgus) & Espressif Systems
 Author-email: 
 License: GPLv2+
 Project-URL: Documentation, https://docs.espressif.com/projects/esptool/
 Project-URL: Source, https://github.com/espressif/esptool/
 Project-URL: Tracker, https://github.com/espressif/esptool/issues/
-Description: 
-        ==========
-        esptool.py
-        ==========
-        A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
-        
-        The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
-        
-        Documentation
-        -------------
-        Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
-        
-        Contributing
-        ------------
-        Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -38,7 +22,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: hsm
+License-File: LICENSE
+
+
+==========
+esptool.py
+==========
+A Python-based, open-source, platform-independent utility to communicate with the ROM bootloader in Espressif chips.
+
+The esptool.py project is `hosted on github <https://github.com/espressif/esptool>`_.
+
+Documentation
+-------------
+Visit online `esptool documentation <https://docs.espressif.com/projects/esptool/>`_ or run ``esptool.py -h``.
+
+Contributing
+------------
+Please see the `contributions guide <https://docs.espressif.com/projects/esptool/en/latest/contributing.html>`_.
+
+
```

### Comparing `esptool-4.6.2/esptool.egg-info/SOURCES.txt` & `esptool-4.6.dev1/esptool.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -56,21 +56,14 @@
 espefuse/efuse/esp32s3/mem_definition.py
 espefuse/efuse/esp32s3/operations.py
 espefuse/efuse/esp32s3beta2/__init__.py
 espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
 espefuse/efuse/esp32s3beta2/fields.py
 espefuse/efuse/esp32s3beta2/mem_definition.py
 espefuse/efuse/esp32s3beta2/operations.py
-espefuse/efuse_defs/esp32.yaml
-espefuse/efuse_defs/esp32c2.yaml
-espefuse/efuse_defs/esp32c3.yaml
-espefuse/efuse_defs/esp32c6.yaml
-espefuse/efuse_defs/esp32h2.yaml
-espefuse/efuse_defs/esp32s2.yaml
-espefuse/efuse_defs/esp32s3.yaml
 espsecure/__init__.py
 espsecure/__main__.py
 espsecure/esp_hsm_sign/__init__.py
 espsecure/esp_hsm_sign/exceptions.py
 esptool/__init__.py
 esptool/__main__.py
 esptool/bin_image.py
```

### Comparing `esptool-4.6.2/esptool.py` & `esptool-4.6.dev1/esptool.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 import os
 import sys
 
 if os.name != "nt":
     # Linux/macOS: remove current script directory to avoid importing this file
     # as a module; we want to import the installed esptool module instead
     with contextlib.suppress(ValueError):
-        executable_dir = os.path.dirname(sys.executable)
-        sys.path = [
-            path
-            for path in sys.path
-            if not path.endswith(("/bin", "/sbin")) and path != executable_dir
-        ]
+        if sys.path[0].endswith("/bin"):
+            sys.path.pop(0)
+        sys.path.remove(os.path.dirname(sys.executable))
 
     # Linux/macOS: delete imported module entry to force Python to load
     # the module from scratch; this enables importing esptool module in
     # other Python scripts
     with contextlib.suppress(KeyError):
         del sys.modules["esptool"]
```

### Comparing `esptool-4.6.2/setup.py` & `esptool-4.6.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,15 @@
         ],
     },
     install_requires=[
         "bitstring>=3.1.6",
         "cryptography>=2.1.4",
         "ecdsa>=0.16.0",
         "pyserial>=3.0",
-        "reedsolo>=1.5.3,<1.8",
-        "PyYAML>=5.1",
+        "reedsolo>=1.5.3,<=1.6.0",
     ],
     packages=find_packages(),
     include_package_data=True,
     package_data={"": ["esptool/targets/stub_flasher/*.json"]},
     entry_points=entry_points,
     scripts=scripts,
 )
```

