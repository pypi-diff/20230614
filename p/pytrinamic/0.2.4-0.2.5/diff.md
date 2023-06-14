# Comparing `tmp/pytrinamic-0.2.4.tar.gz` & `tmp/pytrinamic-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrinamic-0.2.4.tar", last modified: Fri Jan 27 17:19:19 2023, max compression
+gzip compressed data, was "pytrinamic-0.2.5.tar", last modified: Wed Mar 29 14:11:02 2023, max compression
```

## Comparing `pytrinamic-0.2.4.tar` & `pytrinamic-0.2.5.tar`

### file list

```diff
@@ -1,167 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.812200 pytrinamic-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-01-27 17:19:19.812200 pytrinamic-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.792200 pytrinamic-0.2.4/pytrinamic/
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/RAMDebug.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.796200 pytrinamic-0.2.4/pytrinamic/connections/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.796200 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/can_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/dummy_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/serial_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/uart_ic_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/connections/usb_tmcl_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.800200 pytrinamic-0.2.4/pytrinamic/evalboards/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/MAX22216_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2100_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2130_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2160_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2208_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2209_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2224_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2225_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2240_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2300_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2590_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC2660_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC4361_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC4671_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5031_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5041_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5062_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5072_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5130_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5160_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5160_shield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC5240_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC6100_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC6200_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC6300_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/TMC7300_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/evalboards/tmcl_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.804200 pytrinamic-0.2.4/pytrinamic/features/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/abn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/abn_encoder_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/absolute_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/absolute_encoder_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/coolstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/coolstep_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/current_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/current_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/digital_hall.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/digital_hall_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/drive_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/drive_setting_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/linear_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/linear_ramp_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/linear_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/motor_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/motor_control_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/motor_control_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/pid_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/ramp_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/ramp_settings_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/s_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/s_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/six_point_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/six_point_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/solenoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/solenoid_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/solenoid_control_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/solenoid_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/stallguard2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/stallguard2_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/features/stallguard2_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.808200 pytrinamic-0.2.4/pytrinamic/ic/
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/MAX22216.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2100.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2130.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2160.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2208.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2209.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2224.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2225.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2240.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2300.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2590.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC2660.py
--rw-r--r--   0 runner    (1001) docker     (123)    38190 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC4361.py
--rw-r--r--   0 runner    (1001) docker     (123)    49011 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC4671.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC5031.py
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC5041.py
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC5062.py
--rw-r--r--   0 runner    (1001) docker     (123)    25681 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC5072.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC5130.py
--rw-r--r--   0 runner    (1001) docker     (123)    33995 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC5160.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC5240.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC6100.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC6200.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC6300.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/TMC7300.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/ic/tmc_ic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.812200 pytrinamic-0.2.4/pytrinamic/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/Landungsbruecke.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCC160.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1140.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1141.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1160.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1161.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1231.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1240.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1260.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1270.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1276.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1370.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1617.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1630.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1633.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1636.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1637.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1638.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1640.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM1670.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM3110.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM3312.py
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM3351.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM6110.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM6212.py
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM6214.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/TMCM_Python.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/canopen_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/tmc_eval_shield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/modules/tmcl_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.812200 pytrinamic-0.2.4/pytrinamic/referencedesigns/
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/referencedesigns/TMC4671_LEV_REF.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/referencedesigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/tmcl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.812200 pytrinamic-0.2.4/pytrinamic/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/tools/velocity_ramp_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/pytrinamic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:19:19.796200 pytrinamic-0.2.4/pytrinamic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-01-27 17:19:19.000000 pytrinamic-0.2.4/pytrinamic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-01-27 17:19:19.000000 pytrinamic-0.2.4/pytrinamic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 17:19:19.000000 pytrinamic-0.2.4/pytrinamic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 17:19:19.000000 pytrinamic-0.2.4/pytrinamic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-27 17:19:19.000000 pytrinamic-0.2.4/pytrinamic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-27 17:19:19.000000 pytrinamic-0.2.4/pytrinamic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-27 17:19:19.812200 pytrinamic-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-01-27 17:19:10.000000 pytrinamic-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.858040 pytrinamic-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-29 14:11:02.858040 pytrinamic-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.814041 pytrinamic-0.2.5/pytrinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/RAMDebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.818041 pytrinamic-0.2.5/pytrinamic/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.818041 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/can_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/dummy_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/serial_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/uart_ic_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/connections/usb_tmcl_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.826041 pytrinamic-0.2.5/pytrinamic/evalboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/MAX22216_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2100_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2130_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2160_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2208_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2209_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2224_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2225_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2240_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2590_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC2660_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC4361_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC4671_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5031_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5041_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5062_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5072_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5130_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5160_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5160_shield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC5240_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC6100_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC6200_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC6300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/TMC7300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/evalboards/tmcl_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.838040 pytrinamic-0.2.5/pytrinamic/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/abn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/abn_encoder_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/absolute_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/absolute_encoder_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/coolstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/coolstep_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/current_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/current_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/digital_hall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/digital_hall_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/drive_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/drive_setting_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/linear_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/linear_ramp_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/linear_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/motor_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/motor_control_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/motor_control_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/pid_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/ramp_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/ramp_settings_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/s_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/s_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/six_point_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/six_point_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/solenoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/solenoid_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/solenoid_control_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/solenoid_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/stallguard2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/stallguard2_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/features/stallguard2_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.850040 pytrinamic-0.2.5/pytrinamic/ic/
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/MAX22216.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2130.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2208.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2209.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2225.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2240.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2300.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2590.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC2660.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38190 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC4361.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49011 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC4671.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC5031.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC5041.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC5062.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25681 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC5072.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC5130.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33995 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC5160.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC5240.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC6100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC6200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC6300.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/TMC7300.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/ic/tmc_ic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.858040 pytrinamic-0.2.5/pytrinamic/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/Landungsbruecke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCC160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1140.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1141.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1161.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1231.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1240.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1260.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1270.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1276.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1370.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1617.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1630.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1633.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1636.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1637.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1638.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM1670.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM3110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM3312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM3351.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM6110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM6212.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM6214.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/TMCM_Python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/canopen_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/tmc_eval_shield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/modules/tmcl_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.858040 pytrinamic-0.2.5/pytrinamic/referencedesigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/referencedesigns/TMC4671_LEV_REF.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/referencedesigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/tmcl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.858040 pytrinamic-0.2.5/pytrinamic/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/tools/velocity_ramp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/pytrinamic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.814041 pytrinamic-0.2.5/pytrinamic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-29 14:11:02.000000 pytrinamic-0.2.5/pytrinamic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-03-29 14:11:02.000000 pytrinamic-0.2.5/pytrinamic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:11:02.000000 pytrinamic-0.2.5/pytrinamic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:11:02.000000 pytrinamic-0.2.5/pytrinamic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-29 14:11:02.000000 pytrinamic-0.2.5/pytrinamic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 14:11:02.000000 pytrinamic-0.2.5/pytrinamic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-29 14:11:02.858040 pytrinamic-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:11:02.858040 pytrinamic-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/tests/test_can_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-03-29 14:10:49.000000 pytrinamic-0.2.5/tests/test_interface_timeouts.py
```

### Comparing `pytrinamic-0.2.4/LICENSE` & `pytrinamic-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/MANIFEST.in` & `pytrinamic-0.2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/PKG-INFO` & `pytrinamic-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrinamic
-Version: 0.2.4
+Version: 0.2.5
 Summary: TRINAMIC's Python Technology Access Package.
 Home-page: https://github.com/trinamic/PyTrinamic
 Author: Trinamic Software Team
 Author-email: tmc_info@trinamic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrinamic-0.2.4/README.md` & `pytrinamic-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/RAMDebug.py` & `pytrinamic-0.2.5/pytrinamic/RAMDebug.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/__init__.py` & `pytrinamic-0.2.5/pytrinamic/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/can_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/can_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/connection_manager.py` & `pytrinamic-0.2.5/pytrinamic/connections/connection_manager.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/dummy_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/dummy_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/serial_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/serial_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/uart_ic_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/uart_ic_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/connections/usb_tmcl_interface.py` & `pytrinamic-0.2.5/pytrinamic/connections/usb_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/MAX22216_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/MAX22216_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2100_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2100_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2130_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2130_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2160_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2160_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2208_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2208_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2209_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2209_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2224_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2224_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2225_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2225_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2240_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2240_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2300_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2590_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2590_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC2660_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC2660_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC4361_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC4361_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC4671_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC4671_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5031_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5031_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5041_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5041_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5062_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5062_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5072_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5072_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5130_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5130_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5160_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5160_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5160_shield.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5160_shield.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC5240_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC5240_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC6100_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC6100_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC6200_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC6200_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC6300_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC6300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/TMC7300_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/TMC7300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/__init__.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/evalboards/tmcl_eval.py` & `pytrinamic-0.2.5/pytrinamic/evalboards/tmcl_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/abn_encoder.py` & `pytrinamic-0.2.5/pytrinamic/features/abn_encoder.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/abn_encoder_module.py` & `pytrinamic-0.2.5/pytrinamic/features/abn_encoder_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/absolute_encoder.py` & `pytrinamic-0.2.5/pytrinamic/features/absolute_encoder.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/absolute_encoder_module.py` & `pytrinamic-0.2.5/pytrinamic/features/absolute_encoder_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/coolstep.py` & `pytrinamic-0.2.5/pytrinamic/features/coolstep.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/coolstep_module.py` & `pytrinamic-0.2.5/pytrinamic/features/coolstep_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/current.py` & `pytrinamic-0.2.5/pytrinamic/features/current.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/current_ic.py` & `pytrinamic-0.2.5/pytrinamic/features/current_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/current_module.py` & `pytrinamic-0.2.5/pytrinamic/features/current_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/digital_hall.py` & `pytrinamic-0.2.5/pytrinamic/features/digital_hall.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/digital_hall_module.py` & `pytrinamic-0.2.5/pytrinamic/features/digital_hall_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/drive_setting.py` & `pytrinamic-0.2.5/pytrinamic/features/drive_setting.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/drive_setting_module.py` & `pytrinamic-0.2.5/pytrinamic/features/drive_setting_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/linear_ramp.py` & `pytrinamic-0.2.5/pytrinamic/features/linear_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/linear_ramp_ic.py` & `pytrinamic-0.2.5/pytrinamic/features/linear_ramp_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/linear_ramp_module.py` & `pytrinamic-0.2.5/pytrinamic/features/linear_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/motor_control.py` & `pytrinamic-0.2.5/pytrinamic/features/motor_control.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/motor_control_ic.py` & `pytrinamic-0.2.5/pytrinamic/features/motor_control_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/motor_control_module.py` & `pytrinamic-0.2.5/pytrinamic/features/motor_control_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/pid.py` & `pytrinamic-0.2.5/pytrinamic/features/pid.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/pid_module.py` & `pytrinamic-0.2.5/pytrinamic/features/pid_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/ramp_settings.py` & `pytrinamic-0.2.5/pytrinamic/features/ramp_settings.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/ramp_settings_module.py` & `pytrinamic-0.2.5/pytrinamic/features/ramp_settings_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/s_ramp.py` & `pytrinamic-0.2.5/pytrinamic/features/s_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/s_ramp_module.py` & `pytrinamic-0.2.5/pytrinamic/features/s_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/six_point_ramp.py` & `pytrinamic-0.2.5/pytrinamic/features/six_point_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/six_point_ramp_module.py` & `pytrinamic-0.2.5/pytrinamic/features/six_point_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/solenoid.py` & `pytrinamic-0.2.5/pytrinamic/features/solenoid.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/solenoid_control_ic.py` & `pytrinamic-0.2.5/pytrinamic/features/solenoid_control_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/solenoid_ic.py` & `pytrinamic-0.2.5/pytrinamic/features/solenoid_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/stallguard2.py` & `pytrinamic-0.2.5/pytrinamic/features/stallguard2.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/stallguard2_ic.py` & `pytrinamic-0.2.5/pytrinamic/features/stallguard2_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/features/stallguard2_module.py` & `pytrinamic-0.2.5/pytrinamic/features/stallguard2_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/helpers.py` & `pytrinamic-0.2.5/pytrinamic/helpers.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/MAX22216.py` & `pytrinamic-0.2.5/pytrinamic/ic/MAX22216.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2100.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2100.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2130.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2130.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2160.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2208.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2208.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2209.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2209.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2224.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2224.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2225.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2225.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2240.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2300.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2300.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2590.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2590.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC2660.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC2660.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC4361.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC4361.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC4671.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC4671.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC5031.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC5031.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC5041.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC5041.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC5062.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC5062.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC5072.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC5072.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC5130.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC5130.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC5160.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC5160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC5240.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC5240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC6100.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC6100.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC6200.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC6200.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/TMC7300.py` & `pytrinamic-0.2.5/pytrinamic/ic/TMC7300.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/ic/__init__.py` & `pytrinamic-0.2.5/pytrinamic/ic/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/Landungsbruecke.py` & `pytrinamic-0.2.5/pytrinamic/modules/Landungsbruecke.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCC160.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCC160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1140.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1140.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1141.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1141.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1160.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1161.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1161.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1231.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1231.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1240.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1260.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1260.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1270.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1270.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1276.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1276.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1370.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1370.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1617.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1617.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1630.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1630.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1633.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1633.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1636.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1636.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1637.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1637.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1638.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1638.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1640.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1640.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM1670.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM1670.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM3110.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM3110.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM3312.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM3312.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM3351.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM3351.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM6110.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM6110.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM6212.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM6212.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM6214.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM6214.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/TMCM_Python.py` & `pytrinamic-0.2.5/pytrinamic/modules/TMCM_Python.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/__init__.py` & `pytrinamic-0.2.5/pytrinamic/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/canopen_node.py` & `pytrinamic-0.2.5/pytrinamic/modules/canopen_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,57 +22,57 @@
 
     class StateMachineFault(Exception):
         pass
 
     def __init__(self, *args, **kwargs):
         super(TmcmNode, self).__init__(*args, **kwargs)
 
-    def go_to_operation_enabled(self):
+    def go_to_operation_enabled(self, motor=1):
         # clear an eventually present fault
-        state = self.get_state()
+        state = self.get_state(motor)
         if state == 'Fault':
-            self.sdo[0x6040].raw = self.Cmd.FAULT_RESET
+            self.sdo['Controlword {number}'.format(number=motor)].raw = self.Cmd.FAULT_RESET
             while 1:
-                state = self.get_state()
+                state = self.get_state(motor)
                 if state == 'Switch on disable':
                     break
                 time.sleep(1)
         sequence_from_state = {
             'Switch on disable': [(self.Cmd.SHUTDOWN, 'Ready to switch on'),
                                   (self.Cmd.SWITCH_ON, 'Switched on'),
                                   (self.Cmd.ENABLE_OPERATION, 'Operation enabled')],
             'Ready to switch on': [(self.Cmd.SWITCH_ON, 'Switched on'),
                                    (self.Cmd.ENABLE_OPERATION, 'Operation enabled')],
             'Switched on': [(self.Cmd.ENABLE_OPERATION, 'Operation enabled')],
             'Operation enabled': [],
         }
         # go up the state machine states
         for cmd, expected_status in sequence_from_state[state]:
-            self.sdo[0x6040].raw = cmd
+            self.sdo['Controlword {number}'.format(number=motor)].raw = cmd
             time.sleep(0.1)
             while 1:
-                state = self.get_state()
+                state = self.get_state(motor)
                 if state == 'Fault':
                     raise self.StateMachineFault(f'Fault when transitioning to {expected_status}')
                 if state == expected_status:
                     break
 
-    def shutdown(self):
-        if self.get_state() != 'Switch on disable':
-            self.sdo[0x6040].raw = 0
+    def shutdown(self, motor=1):
+        if self.get_state(motor) != 'Switch on disable':
+            self.sdo['Controlword {number}'.format(number=motor)].raw = 0
             time.sleep(0.1)
 
-    def get_state(self):
+    def get_state(self, motor=1):
         states = [
             ('Not ready to switch on', 0b0000_0000_0100_1111, 0b0000_0000_0000_0000),
             ('Switch on disable', 0b0000_0000_0100_1111, 0b0000_0000_0100_0000),
             ('Ready to switch on', 0b0000_0000_0110_1111, 0b0000_0000_0010_0001),
             ('Switched on', 0b0000_0000_0110_1111, 0b0000_0000_0010_0011),
             ('Operation enabled', 0b0000_0000_0110_1111, 0b0000_0000_0010_0111),
             ('Quick Stop active', 0b0000_0000_0110_1111, 0b0000_0000_0000_0111),
             ('Fault reaction active', 0b0000_0000_0100_1111, 0b0000_0000_0000_1111),
             ('Fault', 0b0000_0000_0100_1111, 0b0000_0000_0000_1000),
         ]
-        statusword = self.sdo[0x6041].raw
+        statusword = self.sdo['Statusword {number}'.format(number=motor)].raw
         for name, mask, bits in states:
             if (statusword & mask) == bits:
                 return name
```

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/tmc_eval_shield.py` & `pytrinamic-0.2.5/pytrinamic/modules/tmc_eval_shield.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/modules/tmcl_module.py` & `pytrinamic-0.2.5/pytrinamic/modules/tmcl_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/referencedesigns/TMC4671_LEV_REF.py` & `pytrinamic-0.2.5/pytrinamic/referencedesigns/TMC4671_LEV_REF.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/tmcl.py` & `pytrinamic-0.2.5/pytrinamic/tmcl.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic/tools/velocity_ramp_runner.py` & `pytrinamic-0.2.5/pytrinamic/tools/velocity_ramp_runner.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.4/pytrinamic.egg-info/PKG-INFO` & `pytrinamic-0.2.5/pytrinamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrinamic
-Version: 0.2.4
+Version: 0.2.5
 Summary: TRINAMIC's Python Technology Access Package.
 Home-page: https://github.com/trinamic/PyTrinamic
 Author: Trinamic Software Team
 Author-email: tmc_info@trinamic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrinamic-0.2.4/pytrinamic.egg-info/SOURCES.txt` & `pytrinamic-0.2.5/pytrinamic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -148,8 +148,10 @@
 pytrinamic/modules/__init__.py
 pytrinamic/modules/canopen_node.py
 pytrinamic/modules/tmc_eval_shield.py
 pytrinamic/modules/tmcl_module.py
 pytrinamic/referencedesigns/TMC4671_LEV_REF.py
 pytrinamic/referencedesigns/__init__.py
 pytrinamic/tools/__init__.py
-pytrinamic/tools/velocity_ramp_runner.py
+pytrinamic/tools/velocity_ramp_runner.py
+tests/test_can_adapters.py
+tests/test_interface_timeouts.py
```

### Comparing `pytrinamic-0.2.4/setup.py` & `pytrinamic-0.2.5/setup.py`

 * *Files identical despite different names*

