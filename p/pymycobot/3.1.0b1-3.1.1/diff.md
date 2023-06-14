# Comparing `tmp/pymycobot-3.1.0b1.tar.gz` & `tmp/pymycobot-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.1.0b1.tar", last modified: Tue May 23 05:46:01 2023, max compression
+gzip compressed data, was "pymycobot-3.1.1.tar", last modified: Wed Jun 14 03:12:55 2023, max compression
```

## Comparing `pymycobot-3.1.0b1.tar` & `pymycobot-3.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 05:46:01.789836 pymycobot-3.1.0b1/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0    55520 2023-05-23 05:46:01.788772 pymycobot-3.1.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.0b1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 05:46:01.754319 pymycobot-3.1.0b1/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.0b1/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1562 2023-05-23 05:45:44.000000 pymycobot-3.1.0b1/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2022-07-18 09:51:08.000000 pymycobot-3.1.0b1/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    12065 2023-03-06 07:56:35.000000 pymycobot-3.1.0b1/pymycobot/common.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/error.py
--rw-rw-rw-   0        0        0    32911 2023-03-13 09:04:37.000000 pymycobot-3.1.0b1/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.0b1/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8869 2023-01-10 08:08:44.000000 pymycobot-3.1.0b1/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13315 2023-04-14 05:34:53.000000 pymycobot-3.1.0b1/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.0b1/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.0b1/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.0b1/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7414 2023-05-23 05:42:22.000000 pymycobot-3.1.0b1/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7441 2022-06-28 10:56:36.000000 pymycobot-3.1.0b1/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8483 2023-05-23 05:43:01.000000 pymycobot-3.1.0b1/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7445 2022-10-20 05:52:29.000000 pymycobot-3.1.0b1/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19564 2023-04-27 09:34:23.000000 pymycobot-3.1.0b1/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 05:46:01.785533 pymycobot-3.1.0b1/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    55520 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-23 05:46:01.000000 pymycobot-3.1.0b1/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.0b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 05:46:01.789836 pymycobot-3.1.0b1/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:55.873676 pymycobot-3.1.1/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.1/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    55974 2023-06-14 03:12:55.872652 pymycobot-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:55.841543 pymycobot-3.1.1/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.1/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1554 2023-06-14 03:09:18.000000 pymycobot-3.1.1/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.1/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    12276 2023-06-14 02:54:52.000000 pymycobot-3.1.1/pymycobot/common.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/error.py
+-rw-rw-rw-   0        0        0    33724 2023-06-14 02:59:25.000000 pymycobot-3.1.1/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.1/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     9015 2023-06-12 07:33:26.000000 pymycobot-3.1.1/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13315 2023-04-14 05:34:53.000000 pymycobot-3.1.1/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.1/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.1/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.1/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7503 2023-06-09 06:51:47.000000 pymycobot-3.1.1/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.1/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8483 2023-05-23 05:43:01.000000 pymycobot-3.1.1/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.1/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19631 2023-05-24 08:27:45.000000 pymycobot-3.1.1/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:55.871026 pymycobot-3.1.1/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    55974 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:12:55.873676 pymycobot-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.1/setup.py
```

### Comparing `pymycobot-3.1.0b1/LICENSE` & `pymycobot-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/PKG-INFO` & `pymycobot-3.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.0b1
+Version: 3.1.1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -93,223 +91,225 @@
 <summary>Catalogue:</summary>
 
 <!-- vim-markdown-toc GFM -->
 
 - [pymycobot](#pymycobot)
 - [MyCobot / Mypalletizer / MechArm](#mycobot--mypalletizer--mecharm)
   - [Overall status](#overall-status)
-    - [power_on](#power_on)
-    - [power_off](#power_off)
-    - [is_power_on](#is_power_on)
-    - [read_next_error](#read_next_error)
-    - [release_all_servos](#release_all_servos)
-    - [is_controller_connected](#is_controller_connected)
+    - [power\_on](#power_on)
+    - [power\_off](#power_off)
+    - [is\_power\_on](#is_power_on)
+    - [read\_next\_error](#read_next_error)
+    - [release\_all\_servos](#release_all_servos)
+    - [is\_controller\_connected](#is_controller_connected)
+    - [get\_error\_information](#get_error_information)
+    - [clear\_error\_information](#clear_error_information)
   - [MDI mode and operation](#mdi-mode-and-operation)
-    - [get_angles](#get_angles)
-    - [set_fresh_mode(mode)](#set_fresh_modemode)
-    - [send_angle](#send_angle)
-    - [send_angles()](#send_angles)
-    - [get_radians](#get_radians)
-    - [send_radians](#send_radians)
-    - [get_coords](#get_coords)
-    - [send_coord](#send_coord)
-    - [send_coords](#send_coords)
-    - [sync_send_angles](#sync_send_angles)
-    - [sync_send_coords](#sync_send_coords)
-    - [is_in_position](#is_in_position)
+    - [get\_angles](#get_angles)
+    - [set\_fresh\_mode(mode)](#set_fresh_modemode)
+    - [send\_angle](#send_angle)
+    - [send\_angles()](#send_angles)
+    - [get\_radians](#get_radians)
+    - [send\_radians](#send_radians)
+    - [get\_coords](#get_coords)
+    - [send\_coord](#send_coord)
+    - [send\_coords](#send_coords)
+    - [sync\_send\_angles](#sync_send_angles)
+    - [sync\_send\_coords](#sync_send_coords)
+    - [is\_in\_position](#is_in_position)
   - [JOG mode and operation](#jog-mode-and-operation)
-    - [jog_angle](#jog_angle)
-    - [jog_coord](#jog_coord)
-    - [jog_increment](#jog_increment)
-    - [jog_stop](#jog_stop)
+    - [jog\_angle](#jog_angle)
+    - [jog\_coord](#jog_coord)
+    - [jog\_increment](#jog_increment)
+    - [jog\_stop](#jog_stop)
     - [pause](#pause)
     - [resume](#resume)
     - [stop](#stop)
-    - [is_paused](#is_paused)
-    - [set_encoder](#set_encoder)
-    - [get_encoder](#get_encoder)
-    - [set_encoders](#set_encoders)
-    - [get_encoders](#get_encoders)
+    - [is\_paused](#is_paused)
+    - [set\_encoder](#set_encoder)
+    - [get\_encoder](#get_encoder)
+    - [set\_encoders](#set_encoders)
+    - [get\_encoders](#get_encoders)
   - [Running status and Settings](#running-status-and-settings)
-    - [get_speed](#get_speed)
-    - [set_speed](#set_speed)
-    - [set_joint_min](#set_joint_min)
-    - [set_joint_max](#set_joint_max)
-    - [get_joint_min_angle](#get_joint_min_angle)
-    - [get_joint_max_angle](#get_joint_max_angle)
+    - [get\_speed](#get_speed)
+    - [set\_speed](#set_speed)
+    - [set\_joint\_min](#set_joint_min)
+    - [set\_joint\_max](#set_joint_max)
+    - [get\_joint\_min\_angle](#get_joint_min_angle)
+    - [get\_joint\_max\_angle](#get_joint_max_angle)
   - [Servo control](#servo-control)
-    - [is_servo_enable](#is_servo_enable)
-    - [is_all_servo_enable](#is_all_servo_enable)
-    - [set_servo_data](#set_servo_data)
-    - [get_servo_data](#get_servo_data)
-    - [set_servo_calibration](#set_servo_calibration)
-    - [release_servo](#release_servo)
-    - [focus_servo](#focus_servo)
+    - [is\_servo\_enable](#is_servo_enable)
+    - [is\_all\_servo\_enable](#is_all_servo_enable)
+    - [set\_servo\_data](#set_servo_data)
+    - [get\_servo\_data](#get_servo_data)
+    - [set\_servo\_calibration](#set_servo_calibration)
+    - [release\_servo](#release_servo)
+    - [focus\_servo](#focus_servo)
   - [Atom IO](#atom-io)
-    - [set_color](#set_color)
-    - [set_pin_mode](#set_pin_mode)
-    - [set_digital_output()](#set_digital_output)
-    - [get_digital_input()](#get_digital_input)
-    - [set_pwm_output()](#set_pwm_output)
-    - [get_gripper_value](#get_gripper_value)
-    - [set_gripper_state](#set_gripper_state)
-    - [set_gripper_value](#set_gripper_value)
-    - [set_gripper_ini](#set_gripper_ini)
-    - [is_gripper_moving](#is_gripper_moving)
-    - [get_basic_input](#get_basic_input)
-    - [set_basic_output](#set_basic_output)
-    - [set_ssid_pwd](#set_ssid_pwd)
-    - [get_ssid_pwd](#get_ssid_pwd)
-    - [set_server_port](#set_server_port)
-    - [get_tof_distance](#get_tof_distance)
-    - [get_tool_reference](#get_tool_reference)
-    - [set_tool_reference](#set_tool_reference)
-    - [set_world_reference](#set_world_reference)
-    - [get_world_reference](#get_world_reference)
-    - [set_reference_frame](#set_reference_frame)
-    - [get_reference_frame](#get_reference_frame)
-    - [set_movement_type](#set_movement_type)
-    - [get_movement_type](#get_movement_type)
-    - [set_end_type](#set_end_type)
-    - [get_end_type](#get_end_type)
-    - [get_plan_speed](#get_plan_speed)
-    - [get_plan_acceleration](#get_plan_acceleration)
-    - [set_plan_speed](#set_plan_speed)
-    - [set_plan_acceleration](#set_plan_acceleration)
-    - [get_servo_speeds](#get_servo_speeds)
-    - [get_servo_currents](#get_servo_currents)
-    - [get_servo_voltages](#get_servo_voltages)
-    - [get_servo_status](#get_servo_status)
-    - [get_servo_temps](#get_servo_temps)
-    - [init_eletric_gripper](#init_eletric_gripper)
-    - [set_eletric_gripper](#set_eletric_gripper)
-    - [set_encoders_drag](#set_encoders_drag)
-    - [set_refresh_mode](#set_refresh_mode)
+    - [set\_color](#set_color)
+    - [set\_pin\_mode](#set_pin_mode)
+    - [set\_digital\_output()](#set_digital_output)
+    - [get\_digital\_input()](#get_digital_input)
+    - [set\_pwm\_output()](#set_pwm_output)
+    - [get\_gripper\_value](#get_gripper_value)
+    - [set\_gripper\_state](#set_gripper_state)
+    - [set\_gripper\_value](#set_gripper_value)
+    - [set\_gripper\_ini](#set_gripper_ini)
+    - [is\_gripper\_moving](#is_gripper_moving)
+    - [get\_basic\_input](#get_basic_input)
+    - [set\_basic\_output](#set_basic_output)
+    - [set\_ssid\_pwd](#set_ssid_pwd)
+    - [get\_ssid\_pwd](#get_ssid_pwd)
+    - [set\_server\_port](#set_server_port)
+    - [get\_tof\_distance](#get_tof_distance)
+    - [get\_tool\_reference](#get_tool_reference)
+    - [set\_tool\_reference](#set_tool_reference)
+    - [set\_world\_reference](#set_world_reference)
+    - [get\_world\_reference](#get_world_reference)
+    - [set\_reference\_frame](#set_reference_frame)
+    - [get\_reference\_frame](#get_reference_frame)
+    - [set\_movement\_type](#set_movement_type)
+    - [get\_movement\_type](#get_movement_type)
+    - [set\_end\_type](#set_end_type)
+    - [get\_end\_type](#get_end_type)
+    - [get\_plan\_speed](#get_plan_speed)
+    - [get\_plan\_acceleration](#get_plan_acceleration)
+    - [set\_plan\_speed](#set_plan_speed)
+    - [set\_plan\_acceleration](#set_plan_acceleration)
+    - [set\_gservo\_round](#set_gservo_round)
+    - [get\_servo\_speeds](#get_servo_speeds)
+    - [get\_servo\_currents](#get_servo_currents)
+    - [get\_servo\_voltages](#get_servo_voltages)
+    - [get\_servo\_status](#get_servo_status)
+    - [get\_servo\_temps](#get_servo_temps)
+    - [init\_eletric\_gripper](#init_eletric_gripper)
+    - [set\_eletric\_gripper](#set_eletric_gripper)
+    - [set\_encoders\_drag](#set_encoders_drag)
+    - [set\_refresh\_mode](#set_refresh_mode)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
-    - [gpio_init](#gpio_init)
-    - [gpio_output](#gpio_output)
+    - [gpio\_init](#gpio_init)
+    - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
-  - [get_port_list](#get_port_list)
-  - [detect_port_of_basic](#detect_port_of_basic)
+  - [get\_port\_list](#get_port_list)
+  - [detect\_port\_of\_basic](#detect_port_of_basic)
 - [MyCobotSocket](#mycobotsocket)
     - [Client](#client)
     - [Server](#server)
   - [socket control](#socket-control)
-    - [connect](#connect)
-    - [set_gpio_mode](#set_gpio_mode)
-    - [set_gpio_out](#set_gpio_out)
-    - [set_gpio_output](#set_gpio_output)
-    - [get_gpio_in](#get_gpio_in)
+    - [set\_gpio\_mode](#set_gpio_mode)
+    - [set\_gpio\_out](#set_gpio_out)
+    - [set\_gpio\_output](#set_gpio_output)
+    - [get\_gpio\_in](#get_gpio_in)
 - [MyBuddy](#mybuddy)
-    - [base_to_single_coords(base_coords, arm)](#base_to_single_coordsbase_coords-arm)
-    - [collision(left_angles, right_angles)](#collisionleft_angles-right_angles)
-    - [collision_switch(state)](#collision_switchstate)
-    - [focus_servo(id, servo_id)](#focus_servoid-servo_id)
-    - [get_acceleration(id)](#get_accelerationid)
-    - [get_angle(id, joint_id)](#get_angleid-joint_id)
-    - [get_angles(id)](#get_anglesid)
-    - [get_base_coord(id)](#get_base_coordid)
-    - [get_base_coords(\*args: int)](#get_base_coordsargs-int)
-    - [get_coord(id, joint_id)](#get_coordid-joint_id)
-    - [get_coords(id)](#get_coordsid)
-    - [get_digital_input(id, pin_no)](#get_digital_inputid-pin_no)
-    - [get_encoder(id, joint_id)](#get_encoderid-joint_id)
-    - [get_encoders(id)](#get_encodersid)
-    - [get_end_type(id)](#get_end_typeid)
-    - [get_gripper_value(id)](#get_gripper_valueid)
-    - [get_joint_current(id, joint_id)](#get_joint_currentid-joint_id)
-    - [get_joint_max_angle(id, joint_id)](#get_joint_max_angleid-joint_id)
-    - [get_joint_min_angle(id, joint_id)](#get_joint_min_angleid-joint_id)
-    - [get_movement_type(id)](#get_movement_typeid)
-    - [get_plan_acceleration(id=0)](#get_plan_accelerationid0)
-    - [get_plan_speed(id=0)](#get_plan_speedid0)
-    - [get_reference_frame(id)](#get_reference_frameid)
-    - [get_robot_id(id)](#get_robot_idid)
-    - [get_robot_version(id)](#get_robot_versionid)
-    - [get_servo_currents(id)](#get_servo_currentsid)
-    - [get_servo_data(id, servo_no, data_id)](#get_servo_dataid-servo_no-data_id)
-    - [get_servo_status(id)](#get_servo_statusid)
-    - [get_servo_spees(id)](#get_servo_speesid)
-    - [get_servo_temps(id)](#get_servo_tempsid)
-    - [get_servo_voltages(id)](#get_servo_voltagesid)
-    - [get_speed(id)](#get_speedid)
-    - [get_system_version(id)](#get_system_versionid)
-    - [get_tool_reference(id)](#get_tool_referenceid)
-    - [get_world_reference(id)](#get_world_referenceid)
-    - [is_all_servo_enable(id)](#is_all_servo_enableid)
-    - [is_collision_on()](#is_collision_on)
-    - [is_controller_connected(id=0)](#is_controller_connectedid0)
-    - [is_free_mode(id)](#is_free_modeid)
-    - [is_gripper_moving(id)](#is_gripper_movingid)
-    - [is_in_position(id, data, mode)](#is_in_positionid-data-mode)
-    - [is_moving(id)](#is_movingid)
-    - [is_paused(id)](#is_pausedid)
-    - [is_power_on(id=0)](#is_power_onid0)
-    - [is_servo_enable(id, servo_id)](#is_servo_enableid-servo_id)
-    - [jog_absolute(id, joint_id, angle, speed)](#jog_absoluteid-joint_id-angle-speed)
-    - [jog_angle(id, joint_id, direction, speed)](#jog_angleid-joint_id-direction-speed)
-    - [jog_coord(id, coord_id, direction, speed)](#jog_coordid-coord_id-direction-speed)
-    - [jog_inc_coord(axis, increment, speed)](#jog_inc_coordaxis-increment-speed)
-    - [jog_increment(id, joint_id, increment, speed)](#jog_incrementid-joint_id-increment-speed)
-    - [jog_stop(id)](#jog_stopid)
-    - [joint_brake(id, joint_id)](#joint_brakeid-joint_id)
+    - [base\_to\_single\_coords(base\_coords, arm)](#base_to_single_coordsbase_coords-arm)
+    - [collision(left\_angles, right\_angles)](#collisionleft_angles-right_angles)
+    - [collision\_switch(state)](#collision_switchstate)
+    - [focus\_servo(id, servo\_id)](#focus_servoid-servo_id)
+    - [get\_acceleration(id)](#get_accelerationid)
+    - [get\_angle(id, joint\_id)](#get_angleid-joint_id)
+    - [get\_angles(id)](#get_anglesid)
+    - [get\_base\_coord(id)](#get_base_coordid)
+    - [get\_base\_coords(\*args: int)](#get_base_coordsargs-int)
+    - [get\_coord(id, joint\_id)](#get_coordid-joint_id)
+    - [get\_coords(id)](#get_coordsid)
+    - [get\_digital\_input(id, pin\_no)](#get_digital_inputid-pin_no)
+    - [get\_encoder(id, joint\_id)](#get_encoderid-joint_id)
+    - [get\_encoders(id)](#get_encodersid)
+    - [get\_end\_type(id)](#get_end_typeid)
+    - [get\_gripper\_value(id)](#get_gripper_valueid)
+    - [get\_joint\_current(id, joint\_id)](#get_joint_currentid-joint_id)
+    - [get\_joint\_max\_angle(id, joint\_id)](#get_joint_max_angleid-joint_id)
+    - [get\_joint\_min\_angle(id, joint\_id)](#get_joint_min_angleid-joint_id)
+    - [get\_movement\_type(id)](#get_movement_typeid)
+    - [get\_plan\_acceleration(id=0)](#get_plan_accelerationid0)
+    - [get\_plan\_speed(id=0)](#get_plan_speedid0)
+    - [get\_reference\_frame(id)](#get_reference_frameid)
+    - [get\_robot\_id(id)](#get_robot_idid)
+    - [get\_robot\_version(id)](#get_robot_versionid)
+    - [get\_servo\_currents(id)](#get_servo_currentsid)
+    - [get\_servo\_data(id, servo\_no, data\_id)](#get_servo_dataid-servo_no-data_id)
+    - [get\_servo\_status(id)](#get_servo_statusid)
+    - [get\_servo\_spees(id)](#get_servo_speesid)
+    - [get\_servo\_temps(id)](#get_servo_tempsid)
+    - [get\_servo\_voltages(id)](#get_servo_voltagesid)
+    - [get\_speed(id)](#get_speedid)
+    - [get\_system\_version(id)](#get_system_versionid)
+    - [get\_tool\_reference(id)](#get_tool_referenceid)
+    - [get\_world\_reference(id)](#get_world_referenceid)
+    - [is\_all\_servo\_enable(id)](#is_all_servo_enableid)
+    - [is\_collision\_on()](#is_collision_on)
+    - [is\_controller\_connected(id=0)](#is_controller_connectedid0)
+    - [is\_free\_mode(id)](#is_free_modeid)
+    - [is\_gripper\_moving(id)](#is_gripper_movingid)
+    - [is\_in\_position(id, data, mode)](#is_in_positionid-data-mode)
+    - [is\_moving(id)](#is_movingid)
+    - [is\_paused(id)](#is_pausedid)
+    - [is\_power\_on(id=0)](#is_power_onid0)
+    - [is\_servo\_enable(id, servo\_id)](#is_servo_enableid-servo_id)
+    - [jog\_absolute(id, joint\_id, angle, speed)](#jog_absoluteid-joint_id-angle-speed)
+    - [jog\_angle(id, joint\_id, direction, speed)](#jog_angleid-joint_id-direction-speed)
+    - [jog\_coord(id, coord\_id, direction, speed)](#jog_coordid-coord_id-direction-speed)
+    - [jog\_inc\_coord(axis, increment, speed)](#jog_inc_coordaxis-increment-speed)
+    - [jog\_increment(id, joint\_id, increment, speed)](#jog_incrementid-joint_id-increment-speed)
+    - [jog\_stop(id)](#jog_stopid)
+    - [joint\_brake(id, joint\_id)](#joint_brakeid-joint_id)
     - [pause(id)](#pauseid)
-    - [power_off(id=0)](#power_offid0)
-    - [power_on(id=0)](#power_onid0)
-    - [read_next_error(id=0)](#read_next_errorid0)
-    - [release_all_servos(id=0)](#release_all_servosid0)
-    - [release_servo(id, servo_id)](#release_servoid-servo_id)
+    - [power\_off(id=0)](#power_offid0)
+    - [power\_on(id=0)](#power_onid0)
+    - [read\_next\_error(id=0)](#read_next_errorid0)
+    - [release\_all\_servos(id=0)](#release_all_servosid0)
+    - [release\_servo(id, servo\_id)](#release_servoid-servo_id)
     - [resume(id)](#resumeid)
-    - [send_angle(id, joint, angle, speed)](#send_angleid-joint-angle-speed)
-    - [send_angles(id, degrees, speed)](#send_anglesid-degrees-speed)
-    - [send_coord(id, coord, data, speed)](#send_coordid-coord-data-speed)
-    - [send_coords(id, coords, speed, mode)](#send_coordsid-coords-speed-mode)
-    - [set_acceleration(id, acc)](#set_accelerationid-acc)
-    - [set_color(id, r=0, g=0, b=0)](#set_colorid-r0-g0-b0)
-    - [set_digital_output(id, pin_no, pin_signal)](#set_digital_outputid-pin_no-pin_signal)
-    - [set_encoder(id, joint_id, encoder, speed)](#set_encoderid-joint_id-encoder-speed)
-    - [set_encoders(id, encoders, speed)](#set_encodersid-encoders-speed)
-    - [set_end_type(id, end)](#set_end_typeid-end)
-    - [set_encoders_drag(id, encoders, speeds)](#set_encoders_dragid-encoders-speeds)
-    - [set_free_mode(id, value)](#set_free_modeid-value)
-    - [set_fresh_mode(id, mode)](#set_fresh_modeid-mode)
-    - [set_gripper_calibration(id)](#set_gripper_calibrationid)
-    - [set_gripper_state(id, flag)](#set_gripper_stateid-flag)
-    - [set_gripper_value(id, value, speed)](#set_gripper_valueid-value-speed)
-    - [set_joint_current(id, joint_id, current)](#set_joint_currentid-joint_id-current)
-    - [set_joint_max(id, joint_id, angle)](#set_joint_maxid-joint_id-angle)
-    - [set_joint_min(id, joint_id, angle)](#set_joint_minid-joint_id-angle)
-    - [set_movement_type(id, move_type)](#set_movement_typeid-move_type)
-    - [set_pin_mode(id, pin_no, pin_mode)](#set_pin_modeid-pin_no-pin_mode)
-    - [set_plan_acceleration(id, acceleration)](#set_plan_accelerationid-acceleration)
-    - [set_plan_speed(id, speed)](#set_plan_speedid-speed)
-    - [set_pwm_output(id, channel, frequency, pin_val)](#set_pwm_outputid-channel-frequency-pin_val)
-    - [set_reference_frame(id, rftype)](#set_reference_frameid-rftype)
-    - [set_robot_id(id, new_id)](#set_robot_idid-new_id)
-    - [set_servo_calibration(id, servo_no)](#set_servo_calibrationid-servo_no)
-    - [set_servo_data(id, servo_no, data_id, value)](#set_servo_dataid-servo_no-data_id-value)
-    - [set_speed(id, speed)](#set_speedid-speed)
-    - [set_tool_reference(id, coords)](#set_tool_referenceid-coords)
-    - [set_world_reference(id, coords)](#set_world_referenceid-coords)
+    - [send\_angle(id, joint, angle, speed)](#send_angleid-joint-angle-speed)
+    - [send\_angles(id, degrees, speed)](#send_anglesid-degrees-speed)
+    - [send\_coord(id, coord, data, speed)](#send_coordid-coord-data-speed)
+    - [send\_coords(id, coords, speed, mode)](#send_coordsid-coords-speed-mode)
+    - [set\_acceleration(id, acc)](#set_accelerationid-acc)
+    - [set\_color(id, r=0, g=0, b=0)](#set_colorid-r0-g0-b0)
+    - [set\_digital\_output(id, pin\_no, pin\_signal)](#set_digital_outputid-pin_no-pin_signal)
+    - [set\_encoder(id, joint\_id, encoder, speed)](#set_encoderid-joint_id-encoder-speed)
+    - [set\_encoders(id, encoders, speed)](#set_encodersid-encoders-speed)
+    - [set\_end\_type(id, end)](#set_end_typeid-end)
+    - [set\_encoders\_drag(id, encoders, speeds)](#set_encoders_dragid-encoders-speeds)
+    - [set\_free\_mode(id, value)](#set_free_modeid-value)
+    - [set\_fresh\_mode(id, mode)](#set_fresh_modeid-mode)
+    - [set\_gripper\_calibration(id)](#set_gripper_calibrationid)
+    - [set\_gripper\_state(id, flag)](#set_gripper_stateid-flag)
+    - [set\_gripper\_value(id, value, speed)](#set_gripper_valueid-value-speed)
+    - [set\_joint\_current(id, joint\_id, current)](#set_joint_currentid-joint_id-current)
+    - [set\_joint\_max(id, joint\_id, angle)](#set_joint_maxid-joint_id-angle)
+    - [set\_joint\_min(id, joint\_id, angle)](#set_joint_minid-joint_id-angle)
+    - [set\_movement\_type(id, move\_type)](#set_movement_typeid-move_type)
+    - [set\_pin\_mode(id, pin\_no, pin\_mode)](#set_pin_modeid-pin_no-pin_mode)
+    - [set\_plan\_acceleration(id, acceleration)](#set_plan_accelerationid-acceleration)
+    - [set\_plan\_speed(id, speed)](#set_plan_speedid-speed)
+    - [set\_pwm\_output()](#set_pwm_output-1)
+    - [set\_reference\_frame(id, rftype)](#set_reference_frameid-rftype)
+    - [set\_robot\_id(id, new\_id)](#set_robot_idid-new_id)
+    - [set\_servo\_calibration(id, servo\_no)](#set_servo_calibrationid-servo_no)
+    - [set\_servo\_data(id, servo\_no, data\_id, value)](#set_servo_dataid-servo_no-data_id-value)
+    - [set\_speed(id, speed)](#set_speedid-speed)
+    - [set\_tool\_reference(id, coords)](#set_tool_referenceid-coords)
+    - [set\_world\_reference(id, coords)](#set_world_referenceid-coords)
     - [stop(id)](#stopid)
-    - [write_base_coord(id, axis, coord, speed)](#write_base_coordid-axis-coord-speed)
-    - [write_base_coords(id, coords, speed)](#write_base_coordsid-coords-speed)
-    - [get_radians(id)](#get_radiansid)
-    - [send_radians(id, radians, speed)](#send_radiansid-radians-speed)
-    - [set_gpio_input(pin)](#set_gpio_inputpin)
-    - [set_gpio_mode(pin_no, mode)](#set_gpio_modepin_no-mode)
-    - [set_gpio_output(pin, v)](#set_gpio_outputpin-v)
-    - [set_gpio_pwm(pin, baud, dc)](#set_gpio_pwmpin-baud-dc)
+    - [write\_base\_coord(id, axis, coord, speed)](#write_base_coordid-axis-coord-speed)
+    - [write\_base\_coords(id, coords, speed)](#write_base_coordsid-coords-speed)
+    - [get\_radians(id)](#get_radiansid)
+    - [send\_radians(id, radians, speed)](#send_radiansid-radians-speed)
+    - [set\_gpio\_input(pin)](#set_gpio_inputpin)
+    - [set\_gpio\_mode(pin\_no, mode)](#set_gpio_modepin_no-mode)
+    - [set\_gpio\_output(pin, v)](#set_gpio_outputpin-v)
+    - [set\_gpio\_pwm(pin, baud, dc)](#set_gpio_pwmpin-baud-dc)
 - [MyBuddyEmoticon](#mybuddyemoticon)
-  - [MyBuddyEmoticon(file_path: list = [], window_size: tuple = [], loop=False)](#mybuddyemoticonfile_path-list---window_size-tuple---loopfalse)
-    - [add_file_path(path_time: list)](#add_file_pathpath_time-list)
-    - [del_file_path(index: int)](#del_file_pathindex-int)
-    - [file_path](#file_path)
+  - [MyBuddyEmoticon(file\_path: list = \[\], window\_size: tuple = \[\], loop=False)](#mybuddyemoticonfile_path-list---window_size-tuple---loopfalse)
+    - [add\_file\_path(path\_time: list)](#add_file_pathpath_time-list)
+    - [del\_file\_path(index: int)](#del_file_pathindex-int)
+    - [file\_path](#file_path)
     - [join()](#join)
     - [pause()](#pause-1)
     - [run()](#run)
     - [start()](#start)
   
 <!-- vim-markdown-toc -->
 </details>
@@ -389,14 +389,33 @@
 
 - **Returns**
 
   - `1`: connected
   - `0`: not connected
   - `-1`: error
 
+### get_error_information
+
+- **Prototype**: `get_error_information()`
+
+- **Description**: Obtaining robot error information.
+
+- **Returns**
+
+  - `0`: No error message.
+  - `1 ~ 6`: The corresponding joint exceeds the limit position.
+  - `32`: Kinematics inverse solution has no solution.
+  - `33 ~ 34`: Linear motion has no adjacent solution.
+
+### clear_error_information
+
+- **Prototype**: `clear_error_information()`
+
+- **Description**: Clear robot error message.
+
 ## MDI mode and operation
 
 ### get_angles
 
 - **Prototype**: `get_angles()`
 
 - **Description**: Get the degree of all joints.
@@ -1111,14 +1130,21 @@
 - **Description**: Set planning acceleration.
 
 - **Parameters**
 
   - `acceleration` (`int`) 0 - 100.
   - `is_linear` (`int`): 0 / 1 (0 ->joint, 1 -> line)
 
+
+### set_gservo_round
+
+- **Prototype**: `set_gservo_round()`
+
+- **Description**: Drive the 9g steering gear clockwise for one revolution.
+
 ### get_servo_speeds
 
 - **Prototype**: `get_servo_speeds()`
 
 - **Description**: Get joint velocity.
 
 - **Return**: `list` Speed of each joint.
@@ -1280,44 +1306,31 @@
 
 ```python
 # demo
 from pymycobot import MyCobotSocket
 # Port 9000 is used by default
 mc = MyCobotSocket("192.168.10.10","9000")
 
-mc.connect("/dev/ttyAMA0","1000000")
-
 res = mc.get_angles()
 print(res)
 
 mc.send_angles([0,0,0,0,0,0],20)
 ...
 
 ```
 
 ### Server
 
-Server file is in the demo folder
+Server file is in the `demo folder`,For details, please check the [Server.py](../demo/Server.py) file in the demo folder
 
 ## socket control
 
 > Note:
 > Most of the methods are the same as the class mycobot, only the new methods are listed here.
 
-### connect
-
-- **Prototype**: `connect(serialport, baudrate, timeout)`
-
-- **Description**: Connect the robot arm through the serial port and baud rate
-
-- **Parameters**
-
-  - `serialport`: (`str`) default `/dev/ttyAMA0`.
-  - `baudrate`: default `1000000`.
-  - `timeout`: default `0.1`.
 
 ### set_gpio_mode
 
 - **Prototype**: `set_gpio_mode(mode)`
 
 - **Description**: Set pin coding method.
 
@@ -1359,16 +1372,14 @@
 
 ```python
 # Set up the demo of the suction pump
 import time
 from pymycobot import MyCobotSocket
 # connect server
 m = MyCobotSocket("192.168.10.10", '9000')
-# default serialport:/dev/ttyAMA0 Baudrate:1000000
-m.connect()
 
 m.set_gpio_mode("BCM")
 m.set_gpio_out(20, "out")
 m.set_gpio_out(21, "out")
 # open
 m.set_gpio_output(20, 0)
 m.set_gpio_output(21, 0)
@@ -2311,27 +2322,17 @@
 
 * **Parameters**
 
   * **id** – 0/1/2/3 (ALL/L/R/W)
 
   * **speed** (_int_) – (0 ~ 100).
 
-### set_pwm_output(id, channel, frequency, pin_val)
-
-PWM control
-
-* **Parameters**
-
-  * **id** – 1/2 (L/R)
-
-  * **channel** (_int_) – IO number (1 - 5).
-
-  * **frequency** (_int_) – clock frequency (0/1: 0 - 1Mhz 1 - 10Mhz)
+### set_pwm_output()
 
-  * **pin_val** (_int_) – Duty cycle 0 ~ 100: 0 ~ 100%
+Set PWM output
 
 ### set_reference_frame(id, rftype)
 
 Set the base coordinate system
 
 * **Parameters**
 
@@ -2589,9 +2590,7 @@
 
 
 ### start()
 Start playing
 
 ---
 More demo can go to [here](../demo).
-
-
```

### Comparing `pymycobot-3.1.0b1/README.md` & `pymycobot-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/Interface.py` & `pymycobot-3.1.1/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/__init__.py` & `pymycobot-3.1.1/pymycobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from pymycobot.genre import Angle, Coord
 from pymycobot import utils
 from pymycobot.mybuddysocket import MyBuddySocket
 from pymycobot.ultraArm import ultraArm
 from pymycobot.mybuddybluetooth import MyBuddyBlueTooth
 from pymycobot.mypalletizersocket import MyPalletizerSocket
 from pymycobot.myarm import MyArm
-    
 
 __all__ = [
     "MyCobot",
     "MyCobotCommandGenerator",
     "Angle",
     "Coord",
     "utils",
@@ -39,15 +38,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.1.0b1"
+__version__ = "3.1.1"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.1.0b1/pymycobot/bluet.py` & `pymycobot-3.1.1/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/common.py` & `pymycobot-3.1.1/pymycobot/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     FOOTER = 0xFA
 
     # System status
     ROBOT_VERSION = 0x01
     SOFTWARE_VERSION = 0x02
     GET_ROBOT_ID = 0x03
     SET_ROBOT_ID = 0x04
+    
+    GET_ERROR_INFO = 0x07
+    CLEAR_ERROR_INFO = 0x08
 
     # Overall status
     POWER_ON = 0x10
     POWER_OFF = 0x11
     IS_POWER_ON = 0x12
     RELEASE_ALL_SERVOS = 0x13
     IS_CONTROLLER_CONNECTED = 0x14
@@ -137,14 +140,15 @@
     SET_CURRENT_STATE = 0x92
 
     # planning speed
     GET_PLAN_SPEED = 0xD0
     GET_PLAN_ACCELERATION = 0xD1
     SET_PLAN_SPEED = 0xD2
     SET_PLAN_ACCELERATION = 0xD3
+    SET_GSERVO_ROUND = 0xD4
 
     # Motor status read
     GET_SERVO_SPEED = 0xE1
     GET_SERVO_CURRENTS = 0xE2
     GET_SERVO_VOLTAGES = 0xE3
     GET_SERVO_STATUS = 0xE4
     GET_SERVO_TEMPS = 0xE5
@@ -302,16 +306,18 @@
                 ProtocolCode.GET_PLAN_SPEED,
                 ProtocolCode.GET_PLAN_ACCELERATION,
             ]:
                 return [
                     self._decode_int8(valid_data[0:1]),
                     self._decode_int8(valid_data[1:]),
                 ]
-            if genre in [ProtocolCode.IS_SERVO_ENABLE]:
+            elif genre in [ProtocolCode.IS_SERVO_ENABLE]:
                 return [self._decode_int8(valid_data[1:2])]
+            elif genre in [ProtocolCode.GET_ERROR_INFO]:
+                return [self._decode_int8(valid_data[1:])]
             res.append(self._decode_int16(valid_data))
         elif data_len == 3:
             res.append(self._decode_int16(valid_data[1:]))
         elif data_len == 4:
             for i in range(1,4):
                 res.append(valid_data[i])
         elif data_len == 7:
```

### Comparing `pymycobot-3.1.0b1/pymycobot/error.py` & `pymycobot-3.1.1/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/generate.py` & `pymycobot-3.1.1/pymycobot/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -675,15 +675,15 @@
         """
         return self._mesg(ProtocolCode.GET_GRIPPER_VALUE, has_reply=True)
 
     def set_gripper_state(self, flag, speed):
         """Set gripper switch state
 
         Args:
-            flag  (int): 0 - open, 1 - close
+            flag  (int): 0 - open, 1 - close, 10 - release
             speed (int): 0 ~ 100
         """
         return self._mesg(ProtocolCode.SET_GRIPPER_STATE, flag, speed)
 
     def set_gripper_value(self, value, speed):
         """Set gripper value
 
@@ -1004,8 +1004,27 @@
     def get_servo_last_pdi(self, id):
         """Obtain the pdi of a single steering gear before modification
         
         Args:
             id: 1 - 6
         """
         return self._mesg(ProtocolCode.GET_SERVO_LASTPDI, id, has_reply = True)
+    
+    def get_error_information(self):
+        """Obtaining robot error information
         
+        Return:
+            0: No error message.
+            1 ~ 6: The corresponding joint exceeds the limit position.
+            16 ~ 19: Collision protection.
+            32: Kinematics inverse solution has no solution.
+            33 ~ 34: Linear motion has no adjacent solution.
+        """
+        return self._mesg(ProtocolCode.GET_ERROR_INFO, has_reply = True)
+    
+    def clear_error_information(self):
+        """Clear robot error message"""
+        return self._mesg(ProtocolCode.CLEAR_ERROR_INFO, has_reply = True)
+    
+    def set_gservo_round(self):
+        """Drive the 9g steering gear clockwise for one revolution"""
+        return self._mesg(ProtocolCode.SET_GSERVO_ROUND)
```

### Comparing `pymycobot-3.1.0b1/pymycobot/log.py` & `pymycobot-3.1.1/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/myarm.py` & `pymycobot-3.1.1/pymycobot/myarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,16 +104,14 @@
                 ProtocolCode.GET_SPEED,
                 ProtocolCode.GET_ENCODER,
                 ProtocolCode.GET_BASIC_INPUT,
                 ProtocolCode.GET_TOF_DISTANCE,
                 ProtocolCode.GET_END_TYPE,
                 ProtocolCode.GET_MOVEMENT_TYPE,
                 ProtocolCode.GET_REFERENCE_FRAME,
-                ProtocolCode.GET_JOINT_MIN_ANGLE,
-                ProtocolCode.GET_JOINT_MAX_ANGLE,
                 ProtocolCode.GET_FRESH_MODE,
                 ProtocolCode.GET_GRIPPER_MODE,
                 ProtocolCode.SET_SSID_PWD
             ]:
                 return self._process_single(res)
             elif genre in [ProtocolCode.GET_ANGLES]:
                 return [self._int2angle(angle) for angle in res]
@@ -125,14 +123,16 @@
                     for idx in range(3, 6):
                         r.append(self._int2angle(res[idx]))
                     return r
                 else:
                     return res
             elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
                 return [self._int2coord(angle) for angle in res]
+            elif genre in [ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
+                return self._int2coord(res[0])
             else:
                 return res
         return None
 
     def get_radians(self):
         """Get the radians of all joints
 
@@ -145,15 +145,14 @@
     def send_radians(self, radians, speed):
         """Send the radians of all joints to robot arm
 
         Args:
             radians: a list of radian values( List[float]), length 6
             speed: (int )0 ~ 100
         """
-        calibration_parameters(len6=radians, speed=speed)
         degrees = [self._angle2int(radian * (180 / math.pi))
                    for radian in radians]
         return self._mesg(ProtocolCode.SEND_ANGLES, degrees, speed)
 
     def sync_send_angles(self, degrees, speed, timeout=7):
         """Send the angle in synchronous state and return when the target point is reached
             
@@ -220,21 +219,24 @@
         """
         return self._mesg(ProtocolCode.SET_SOLUTION_ANGLES, [self._angle2int(angle)], speed)
     
     def get_solution_angles(self):
         """Get zero space deflection angle value"""
         return self._mesg(ProtocolCode.GET_SOLUTION_ANGLES, has_reply=True)
     
-    def release_all_servos(self, data):
+    def release_all_servos(self, data=None):
         """Relax all joints
         
         Args:
             data: 1 - Undamping (The default is damping)
         """
-        return self._mesg(ProtocolCode.RELEASE_ALL_SERVOS, data)
+        if data is None:
+            return super().release_all_servos()
+        else:
+            return self._mesg(ProtocolCode.RELEASE_ALL_SERVOS, data)
             
     def get_transpoendr_mode(self):
         """Obtain the configuration information of serial transmission mode
         
         Return:
             mode: 0 - 1 - 2
         """
@@ -246,8 +248,11 @@
         Args:
             mode: 
                 0 - Turn off transparent transmission.\n
                 1 - Turn on transparent transmission. verify all data.\n
                 2 - Turn on transparent transmission, only verify the configuration information of communication forwarding mode (default is 0)
         """
         return self._mesg(ProtocolCode.GET_SSID_PWD, mode)
+    
+    def close(self):
+        self._serial_port.close()
```

### Comparing `pymycobot-3.1.0b1/pymycobot/mybuddy.py` & `pymycobot-3.1.1/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.1/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.1/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/mybuddysocket.py` & `pymycobot-3.1.1/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/mycobot.py` & `pymycobot-3.1.1/pymycobot/mycobot.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,17 @@
                 ProtocolCode.GET_SPEED,
                 ProtocolCode.GET_ENCODER,
                 ProtocolCode.GET_BASIC_INPUT,
                 ProtocolCode.GET_TOF_DISTANCE,
                 ProtocolCode.GET_END_TYPE,
                 ProtocolCode.GET_MOVEMENT_TYPE,
                 ProtocolCode.GET_REFERENCE_FRAME,
-                ProtocolCode.GET_JOINT_MIN_ANGLE,
-                ProtocolCode.GET_JOINT_MAX_ANGLE,
                 ProtocolCode.GET_FRESH_MODE,
-                ProtocolCode.GET_GRIPPER_MODE
+                ProtocolCode.GET_GRIPPER_MODE,
+                ProtocolCode.GET_ERROR_INFO
             ]:
                 return self._process_single(res)
             elif genre in [ProtocolCode.GET_ANGLES]:
                 return [self._int2angle(angle) for angle in res]
             elif genre in [ProtocolCode.GET_COORDS, ProtocolCode.GET_TOOL_REFERENCE, ProtocolCode.GET_WORLD_REFERENCE]:
                 if res:
                     r = []
@@ -124,14 +123,16 @@
                     for idx in range(3, 6):
                         r.append(self._int2angle(res[idx]))
                     return r
                 else:
                     return res
             elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
                 return [self._int2coord(angle) for angle in res]
+            elif genre in [ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
+                return self._int2coord(res[0])
             else:
                 return res
         return None
 
     def get_radians(self):
         """Get the radians of all joints
```

### Comparing `pymycobot-3.1.0b1/pymycobot/mycobotsocket.py` & `pymycobot-3.1.1/pymycobot/mypalletizersocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pymycobot.log import setup_logging
 from pymycobot.generate import MyCobotCommandGenerator
 from pymycobot.common import ProtocolCode, write, read
 from pymycobot.error import calibration_parameters
 
 
-class MyCobotSocket(MyCobotCommandGenerator):
+class MyPalletizerSocket(MyCobotCommandGenerator):
     """MyCobot Python API Serial communication class.
     Note: Please use this class under the same network
 
     Supported methods:
 
         # Overall status
             Look at parent class: `MyCobotCommandGenerator`.
@@ -51,15 +51,15 @@
 
     def __init__(self, ip, netport=9000):
         """
         Args:
             ip: Server ip
             netport: Server port
         """
-        super(MyCobotSocket, self).__init__()
+        super(MyPalletizerSocket, self).__init__()
         self.calibration_parameters = calibration_parameters
         self.SERVER_IP = ip
         self.SERVER_PORT = netport
         self.rasp = False
         self.sock = self.connect_socket()
 
     def connect(self, serialport="/dev/ttyAMA0", baudrate="1000000", timeout='0.1'):
@@ -90,15 +90,15 @@
                    It is converted to octal by default.
                    If the data needs to be encapsulated into hexadecimal,
                    the array is used to include them. (Data cannot be nested)
             **kwargs: support `has_reply`
                 has_reply: Whether there is a return value to accept.
         """
         real_command, has_reply = super(
-            MyCobotSocket, self)._mesg(genre, *args, **kwargs)
+            MyPalletizerSocket, self)._mesg(genre, *args, **kwargs)
         # [254,...,255]
         data = self._write(self._flatten(real_command), "socket")
         if data:
             res = self._process_received(data, genre)
             if genre in [
                 ProtocolCode.ROBOT_VERSION,
                 ProtocolCode.IS_POWER_ON,
@@ -121,16 +121,16 @@
             elif genre in [ProtocolCode.GET_ANGLES]:
                 return [self._int2angle(angle) for angle in res]
             elif genre in [ProtocolCode.GET_COORDS]:
                 if res:
                     r = []
                     for idx in range(3):
                         r.append(self._int2coord(res[idx]))
-                    for idx in range(3, 6):
-                        r.append(self._int2angle(res[idx]))
+                    if len(res)>3:
+                        r.append(self._int2angle(res[3]))
                     return r
                 else:
                     return res
             elif genre in [
                 ProtocolCode.GET_JOINT_MIN_ANGLE,
                 ProtocolCode.GET_JOINT_MAX_ANGLE,
             ]:
@@ -216,7 +216,10 @@
         """
         return self._mesg(ProtocolCode.GET_GPIO_IN, pin_no)
 
     # Other
     def wait(self, t):
         time.sleep(t)
         return self
+    
+    def close(self):
+        self.sock.close()
```

### Comparing `pymycobot-3.1.0b1/pymycobot/mypalletizer.py` & `pymycobot-3.1.1/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot/ultraArm.py` & `pymycobot-3.1.1/pymycobot/ultraArm.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,7 +574,10 @@
                             begin = i
                             break
                     except Exception:
                         print("Retry receive...")
             command = ""
 
         self.set_speed_mode(2)  # Acceleration / deceleration mode
+        
+    def close(self):
+        self._serial_port.close()
```

### Comparing `pymycobot-3.1.0b1/pymycobot/utils.py` & `pymycobot-3.1.1/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.1/pymycobot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.0b1
+Version: 3.1.1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -93,223 +91,225 @@
 <summary>Catalogue:</summary>
 
 <!-- vim-markdown-toc GFM -->
 
 - [pymycobot](#pymycobot)
 - [MyCobot / Mypalletizer / MechArm](#mycobot--mypalletizer--mecharm)
   - [Overall status](#overall-status)
-    - [power_on](#power_on)
-    - [power_off](#power_off)
-    - [is_power_on](#is_power_on)
-    - [read_next_error](#read_next_error)
-    - [release_all_servos](#release_all_servos)
-    - [is_controller_connected](#is_controller_connected)
+    - [power\_on](#power_on)
+    - [power\_off](#power_off)
+    - [is\_power\_on](#is_power_on)
+    - [read\_next\_error](#read_next_error)
+    - [release\_all\_servos](#release_all_servos)
+    - [is\_controller\_connected](#is_controller_connected)
+    - [get\_error\_information](#get_error_information)
+    - [clear\_error\_information](#clear_error_information)
   - [MDI mode and operation](#mdi-mode-and-operation)
-    - [get_angles](#get_angles)
-    - [set_fresh_mode(mode)](#set_fresh_modemode)
-    - [send_angle](#send_angle)
-    - [send_angles()](#send_angles)
-    - [get_radians](#get_radians)
-    - [send_radians](#send_radians)
-    - [get_coords](#get_coords)
-    - [send_coord](#send_coord)
-    - [send_coords](#send_coords)
-    - [sync_send_angles](#sync_send_angles)
-    - [sync_send_coords](#sync_send_coords)
-    - [is_in_position](#is_in_position)
+    - [get\_angles](#get_angles)
+    - [set\_fresh\_mode(mode)](#set_fresh_modemode)
+    - [send\_angle](#send_angle)
+    - [send\_angles()](#send_angles)
+    - [get\_radians](#get_radians)
+    - [send\_radians](#send_radians)
+    - [get\_coords](#get_coords)
+    - [send\_coord](#send_coord)
+    - [send\_coords](#send_coords)
+    - [sync\_send\_angles](#sync_send_angles)
+    - [sync\_send\_coords](#sync_send_coords)
+    - [is\_in\_position](#is_in_position)
   - [JOG mode and operation](#jog-mode-and-operation)
-    - [jog_angle](#jog_angle)
-    - [jog_coord](#jog_coord)
-    - [jog_increment](#jog_increment)
-    - [jog_stop](#jog_stop)
+    - [jog\_angle](#jog_angle)
+    - [jog\_coord](#jog_coord)
+    - [jog\_increment](#jog_increment)
+    - [jog\_stop](#jog_stop)
     - [pause](#pause)
     - [resume](#resume)
     - [stop](#stop)
-    - [is_paused](#is_paused)
-    - [set_encoder](#set_encoder)
-    - [get_encoder](#get_encoder)
-    - [set_encoders](#set_encoders)
-    - [get_encoders](#get_encoders)
+    - [is\_paused](#is_paused)
+    - [set\_encoder](#set_encoder)
+    - [get\_encoder](#get_encoder)
+    - [set\_encoders](#set_encoders)
+    - [get\_encoders](#get_encoders)
   - [Running status and Settings](#running-status-and-settings)
-    - [get_speed](#get_speed)
-    - [set_speed](#set_speed)
-    - [set_joint_min](#set_joint_min)
-    - [set_joint_max](#set_joint_max)
-    - [get_joint_min_angle](#get_joint_min_angle)
-    - [get_joint_max_angle](#get_joint_max_angle)
+    - [get\_speed](#get_speed)
+    - [set\_speed](#set_speed)
+    - [set\_joint\_min](#set_joint_min)
+    - [set\_joint\_max](#set_joint_max)
+    - [get\_joint\_min\_angle](#get_joint_min_angle)
+    - [get\_joint\_max\_angle](#get_joint_max_angle)
   - [Servo control](#servo-control)
-    - [is_servo_enable](#is_servo_enable)
-    - [is_all_servo_enable](#is_all_servo_enable)
-    - [set_servo_data](#set_servo_data)
-    - [get_servo_data](#get_servo_data)
-    - [set_servo_calibration](#set_servo_calibration)
-    - [release_servo](#release_servo)
-    - [focus_servo](#focus_servo)
+    - [is\_servo\_enable](#is_servo_enable)
+    - [is\_all\_servo\_enable](#is_all_servo_enable)
+    - [set\_servo\_data](#set_servo_data)
+    - [get\_servo\_data](#get_servo_data)
+    - [set\_servo\_calibration](#set_servo_calibration)
+    - [release\_servo](#release_servo)
+    - [focus\_servo](#focus_servo)
   - [Atom IO](#atom-io)
-    - [set_color](#set_color)
-    - [set_pin_mode](#set_pin_mode)
-    - [set_digital_output()](#set_digital_output)
-    - [get_digital_input()](#get_digital_input)
-    - [set_pwm_output()](#set_pwm_output)
-    - [get_gripper_value](#get_gripper_value)
-    - [set_gripper_state](#set_gripper_state)
-    - [set_gripper_value](#set_gripper_value)
-    - [set_gripper_ini](#set_gripper_ini)
-    - [is_gripper_moving](#is_gripper_moving)
-    - [get_basic_input](#get_basic_input)
-    - [set_basic_output](#set_basic_output)
-    - [set_ssid_pwd](#set_ssid_pwd)
-    - [get_ssid_pwd](#get_ssid_pwd)
-    - [set_server_port](#set_server_port)
-    - [get_tof_distance](#get_tof_distance)
-    - [get_tool_reference](#get_tool_reference)
-    - [set_tool_reference](#set_tool_reference)
-    - [set_world_reference](#set_world_reference)
-    - [get_world_reference](#get_world_reference)
-    - [set_reference_frame](#set_reference_frame)
-    - [get_reference_frame](#get_reference_frame)
-    - [set_movement_type](#set_movement_type)
-    - [get_movement_type](#get_movement_type)
-    - [set_end_type](#set_end_type)
-    - [get_end_type](#get_end_type)
-    - [get_plan_speed](#get_plan_speed)
-    - [get_plan_acceleration](#get_plan_acceleration)
-    - [set_plan_speed](#set_plan_speed)
-    - [set_plan_acceleration](#set_plan_acceleration)
-    - [get_servo_speeds](#get_servo_speeds)
-    - [get_servo_currents](#get_servo_currents)
-    - [get_servo_voltages](#get_servo_voltages)
-    - [get_servo_status](#get_servo_status)
-    - [get_servo_temps](#get_servo_temps)
-    - [init_eletric_gripper](#init_eletric_gripper)
-    - [set_eletric_gripper](#set_eletric_gripper)
-    - [set_encoders_drag](#set_encoders_drag)
-    - [set_refresh_mode](#set_refresh_mode)
+    - [set\_color](#set_color)
+    - [set\_pin\_mode](#set_pin_mode)
+    - [set\_digital\_output()](#set_digital_output)
+    - [get\_digital\_input()](#get_digital_input)
+    - [set\_pwm\_output()](#set_pwm_output)
+    - [get\_gripper\_value](#get_gripper_value)
+    - [set\_gripper\_state](#set_gripper_state)
+    - [set\_gripper\_value](#set_gripper_value)
+    - [set\_gripper\_ini](#set_gripper_ini)
+    - [is\_gripper\_moving](#is_gripper_moving)
+    - [get\_basic\_input](#get_basic_input)
+    - [set\_basic\_output](#set_basic_output)
+    - [set\_ssid\_pwd](#set_ssid_pwd)
+    - [get\_ssid\_pwd](#get_ssid_pwd)
+    - [set\_server\_port](#set_server_port)
+    - [get\_tof\_distance](#get_tof_distance)
+    - [get\_tool\_reference](#get_tool_reference)
+    - [set\_tool\_reference](#set_tool_reference)
+    - [set\_world\_reference](#set_world_reference)
+    - [get\_world\_reference](#get_world_reference)
+    - [set\_reference\_frame](#set_reference_frame)
+    - [get\_reference\_frame](#get_reference_frame)
+    - [set\_movement\_type](#set_movement_type)
+    - [get\_movement\_type](#get_movement_type)
+    - [set\_end\_type](#set_end_type)
+    - [get\_end\_type](#get_end_type)
+    - [get\_plan\_speed](#get_plan_speed)
+    - [get\_plan\_acceleration](#get_plan_acceleration)
+    - [set\_plan\_speed](#set_plan_speed)
+    - [set\_plan\_acceleration](#set_plan_acceleration)
+    - [set\_gservo\_round](#set_gservo_round)
+    - [get\_servo\_speeds](#get_servo_speeds)
+    - [get\_servo\_currents](#get_servo_currents)
+    - [get\_servo\_voltages](#get_servo_voltages)
+    - [get\_servo\_status](#get_servo_status)
+    - [get\_servo\_temps](#get_servo_temps)
+    - [init\_eletric\_gripper](#init_eletric_gripper)
+    - [set\_eletric\_gripper](#set_eletric_gripper)
+    - [set\_encoders\_drag](#set_encoders_drag)
+    - [set\_refresh\_mode](#set_refresh_mode)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
-    - [gpio_init](#gpio_init)
-    - [gpio_output](#gpio_output)
+    - [gpio\_init](#gpio_init)
+    - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
-  - [get_port_list](#get_port_list)
-  - [detect_port_of_basic](#detect_port_of_basic)
+  - [get\_port\_list](#get_port_list)
+  - [detect\_port\_of\_basic](#detect_port_of_basic)
 - [MyCobotSocket](#mycobotsocket)
     - [Client](#client)
     - [Server](#server)
   - [socket control](#socket-control)
-    - [connect](#connect)
-    - [set_gpio_mode](#set_gpio_mode)
-    - [set_gpio_out](#set_gpio_out)
-    - [set_gpio_output](#set_gpio_output)
-    - [get_gpio_in](#get_gpio_in)
+    - [set\_gpio\_mode](#set_gpio_mode)
+    - [set\_gpio\_out](#set_gpio_out)
+    - [set\_gpio\_output](#set_gpio_output)
+    - [get\_gpio\_in](#get_gpio_in)
 - [MyBuddy](#mybuddy)
-    - [base_to_single_coords(base_coords, arm)](#base_to_single_coordsbase_coords-arm)
-    - [collision(left_angles, right_angles)](#collisionleft_angles-right_angles)
-    - [collision_switch(state)](#collision_switchstate)
-    - [focus_servo(id, servo_id)](#focus_servoid-servo_id)
-    - [get_acceleration(id)](#get_accelerationid)
-    - [get_angle(id, joint_id)](#get_angleid-joint_id)
-    - [get_angles(id)](#get_anglesid)
-    - [get_base_coord(id)](#get_base_coordid)
-    - [get_base_coords(\*args: int)](#get_base_coordsargs-int)
-    - [get_coord(id, joint_id)](#get_coordid-joint_id)
-    - [get_coords(id)](#get_coordsid)
-    - [get_digital_input(id, pin_no)](#get_digital_inputid-pin_no)
-    - [get_encoder(id, joint_id)](#get_encoderid-joint_id)
-    - [get_encoders(id)](#get_encodersid)
-    - [get_end_type(id)](#get_end_typeid)
-    - [get_gripper_value(id)](#get_gripper_valueid)
-    - [get_joint_current(id, joint_id)](#get_joint_currentid-joint_id)
-    - [get_joint_max_angle(id, joint_id)](#get_joint_max_angleid-joint_id)
-    - [get_joint_min_angle(id, joint_id)](#get_joint_min_angleid-joint_id)
-    - [get_movement_type(id)](#get_movement_typeid)
-    - [get_plan_acceleration(id=0)](#get_plan_accelerationid0)
-    - [get_plan_speed(id=0)](#get_plan_speedid0)
-    - [get_reference_frame(id)](#get_reference_frameid)
-    - [get_robot_id(id)](#get_robot_idid)
-    - [get_robot_version(id)](#get_robot_versionid)
-    - [get_servo_currents(id)](#get_servo_currentsid)
-    - [get_servo_data(id, servo_no, data_id)](#get_servo_dataid-servo_no-data_id)
-    - [get_servo_status(id)](#get_servo_statusid)
-    - [get_servo_spees(id)](#get_servo_speesid)
-    - [get_servo_temps(id)](#get_servo_tempsid)
-    - [get_servo_voltages(id)](#get_servo_voltagesid)
-    - [get_speed(id)](#get_speedid)
-    - [get_system_version(id)](#get_system_versionid)
-    - [get_tool_reference(id)](#get_tool_referenceid)
-    - [get_world_reference(id)](#get_world_referenceid)
-    - [is_all_servo_enable(id)](#is_all_servo_enableid)
-    - [is_collision_on()](#is_collision_on)
-    - [is_controller_connected(id=0)](#is_controller_connectedid0)
-    - [is_free_mode(id)](#is_free_modeid)
-    - [is_gripper_moving(id)](#is_gripper_movingid)
-    - [is_in_position(id, data, mode)](#is_in_positionid-data-mode)
-    - [is_moving(id)](#is_movingid)
-    - [is_paused(id)](#is_pausedid)
-    - [is_power_on(id=0)](#is_power_onid0)
-    - [is_servo_enable(id, servo_id)](#is_servo_enableid-servo_id)
-    - [jog_absolute(id, joint_id, angle, speed)](#jog_absoluteid-joint_id-angle-speed)
-    - [jog_angle(id, joint_id, direction, speed)](#jog_angleid-joint_id-direction-speed)
-    - [jog_coord(id, coord_id, direction, speed)](#jog_coordid-coord_id-direction-speed)
-    - [jog_inc_coord(axis, increment, speed)](#jog_inc_coordaxis-increment-speed)
-    - [jog_increment(id, joint_id, increment, speed)](#jog_incrementid-joint_id-increment-speed)
-    - [jog_stop(id)](#jog_stopid)
-    - [joint_brake(id, joint_id)](#joint_brakeid-joint_id)
+    - [base\_to\_single\_coords(base\_coords, arm)](#base_to_single_coordsbase_coords-arm)
+    - [collision(left\_angles, right\_angles)](#collisionleft_angles-right_angles)
+    - [collision\_switch(state)](#collision_switchstate)
+    - [focus\_servo(id, servo\_id)](#focus_servoid-servo_id)
+    - [get\_acceleration(id)](#get_accelerationid)
+    - [get\_angle(id, joint\_id)](#get_angleid-joint_id)
+    - [get\_angles(id)](#get_anglesid)
+    - [get\_base\_coord(id)](#get_base_coordid)
+    - [get\_base\_coords(\*args: int)](#get_base_coordsargs-int)
+    - [get\_coord(id, joint\_id)](#get_coordid-joint_id)
+    - [get\_coords(id)](#get_coordsid)
+    - [get\_digital\_input(id, pin\_no)](#get_digital_inputid-pin_no)
+    - [get\_encoder(id, joint\_id)](#get_encoderid-joint_id)
+    - [get\_encoders(id)](#get_encodersid)
+    - [get\_end\_type(id)](#get_end_typeid)
+    - [get\_gripper\_value(id)](#get_gripper_valueid)
+    - [get\_joint\_current(id, joint\_id)](#get_joint_currentid-joint_id)
+    - [get\_joint\_max\_angle(id, joint\_id)](#get_joint_max_angleid-joint_id)
+    - [get\_joint\_min\_angle(id, joint\_id)](#get_joint_min_angleid-joint_id)
+    - [get\_movement\_type(id)](#get_movement_typeid)
+    - [get\_plan\_acceleration(id=0)](#get_plan_accelerationid0)
+    - [get\_plan\_speed(id=0)](#get_plan_speedid0)
+    - [get\_reference\_frame(id)](#get_reference_frameid)
+    - [get\_robot\_id(id)](#get_robot_idid)
+    - [get\_robot\_version(id)](#get_robot_versionid)
+    - [get\_servo\_currents(id)](#get_servo_currentsid)
+    - [get\_servo\_data(id, servo\_no, data\_id)](#get_servo_dataid-servo_no-data_id)
+    - [get\_servo\_status(id)](#get_servo_statusid)
+    - [get\_servo\_spees(id)](#get_servo_speesid)
+    - [get\_servo\_temps(id)](#get_servo_tempsid)
+    - [get\_servo\_voltages(id)](#get_servo_voltagesid)
+    - [get\_speed(id)](#get_speedid)
+    - [get\_system\_version(id)](#get_system_versionid)
+    - [get\_tool\_reference(id)](#get_tool_referenceid)
+    - [get\_world\_reference(id)](#get_world_referenceid)
+    - [is\_all\_servo\_enable(id)](#is_all_servo_enableid)
+    - [is\_collision\_on()](#is_collision_on)
+    - [is\_controller\_connected(id=0)](#is_controller_connectedid0)
+    - [is\_free\_mode(id)](#is_free_modeid)
+    - [is\_gripper\_moving(id)](#is_gripper_movingid)
+    - [is\_in\_position(id, data, mode)](#is_in_positionid-data-mode)
+    - [is\_moving(id)](#is_movingid)
+    - [is\_paused(id)](#is_pausedid)
+    - [is\_power\_on(id=0)](#is_power_onid0)
+    - [is\_servo\_enable(id, servo\_id)](#is_servo_enableid-servo_id)
+    - [jog\_absolute(id, joint\_id, angle, speed)](#jog_absoluteid-joint_id-angle-speed)
+    - [jog\_angle(id, joint\_id, direction, speed)](#jog_angleid-joint_id-direction-speed)
+    - [jog\_coord(id, coord\_id, direction, speed)](#jog_coordid-coord_id-direction-speed)
+    - [jog\_inc\_coord(axis, increment, speed)](#jog_inc_coordaxis-increment-speed)
+    - [jog\_increment(id, joint\_id, increment, speed)](#jog_incrementid-joint_id-increment-speed)
+    - [jog\_stop(id)](#jog_stopid)
+    - [joint\_brake(id, joint\_id)](#joint_brakeid-joint_id)
     - [pause(id)](#pauseid)
-    - [power_off(id=0)](#power_offid0)
-    - [power_on(id=0)](#power_onid0)
-    - [read_next_error(id=0)](#read_next_errorid0)
-    - [release_all_servos(id=0)](#release_all_servosid0)
-    - [release_servo(id, servo_id)](#release_servoid-servo_id)
+    - [power\_off(id=0)](#power_offid0)
+    - [power\_on(id=0)](#power_onid0)
+    - [read\_next\_error(id=0)](#read_next_errorid0)
+    - [release\_all\_servos(id=0)](#release_all_servosid0)
+    - [release\_servo(id, servo\_id)](#release_servoid-servo_id)
     - [resume(id)](#resumeid)
-    - [send_angle(id, joint, angle, speed)](#send_angleid-joint-angle-speed)
-    - [send_angles(id, degrees, speed)](#send_anglesid-degrees-speed)
-    - [send_coord(id, coord, data, speed)](#send_coordid-coord-data-speed)
-    - [send_coords(id, coords, speed, mode)](#send_coordsid-coords-speed-mode)
-    - [set_acceleration(id, acc)](#set_accelerationid-acc)
-    - [set_color(id, r=0, g=0, b=0)](#set_colorid-r0-g0-b0)
-    - [set_digital_output(id, pin_no, pin_signal)](#set_digital_outputid-pin_no-pin_signal)
-    - [set_encoder(id, joint_id, encoder, speed)](#set_encoderid-joint_id-encoder-speed)
-    - [set_encoders(id, encoders, speed)](#set_encodersid-encoders-speed)
-    - [set_end_type(id, end)](#set_end_typeid-end)
-    - [set_encoders_drag(id, encoders, speeds)](#set_encoders_dragid-encoders-speeds)
-    - [set_free_mode(id, value)](#set_free_modeid-value)
-    - [set_fresh_mode(id, mode)](#set_fresh_modeid-mode)
-    - [set_gripper_calibration(id)](#set_gripper_calibrationid)
-    - [set_gripper_state(id, flag)](#set_gripper_stateid-flag)
-    - [set_gripper_value(id, value, speed)](#set_gripper_valueid-value-speed)
-    - [set_joint_current(id, joint_id, current)](#set_joint_currentid-joint_id-current)
-    - [set_joint_max(id, joint_id, angle)](#set_joint_maxid-joint_id-angle)
-    - [set_joint_min(id, joint_id, angle)](#set_joint_minid-joint_id-angle)
-    - [set_movement_type(id, move_type)](#set_movement_typeid-move_type)
-    - [set_pin_mode(id, pin_no, pin_mode)](#set_pin_modeid-pin_no-pin_mode)
-    - [set_plan_acceleration(id, acceleration)](#set_plan_accelerationid-acceleration)
-    - [set_plan_speed(id, speed)](#set_plan_speedid-speed)
-    - [set_pwm_output(id, channel, frequency, pin_val)](#set_pwm_outputid-channel-frequency-pin_val)
-    - [set_reference_frame(id, rftype)](#set_reference_frameid-rftype)
-    - [set_robot_id(id, new_id)](#set_robot_idid-new_id)
-    - [set_servo_calibration(id, servo_no)](#set_servo_calibrationid-servo_no)
-    - [set_servo_data(id, servo_no, data_id, value)](#set_servo_dataid-servo_no-data_id-value)
-    - [set_speed(id, speed)](#set_speedid-speed)
-    - [set_tool_reference(id, coords)](#set_tool_referenceid-coords)
-    - [set_world_reference(id, coords)](#set_world_referenceid-coords)
+    - [send\_angle(id, joint, angle, speed)](#send_angleid-joint-angle-speed)
+    - [send\_angles(id, degrees, speed)](#send_anglesid-degrees-speed)
+    - [send\_coord(id, coord, data, speed)](#send_coordid-coord-data-speed)
+    - [send\_coords(id, coords, speed, mode)](#send_coordsid-coords-speed-mode)
+    - [set\_acceleration(id, acc)](#set_accelerationid-acc)
+    - [set\_color(id, r=0, g=0, b=0)](#set_colorid-r0-g0-b0)
+    - [set\_digital\_output(id, pin\_no, pin\_signal)](#set_digital_outputid-pin_no-pin_signal)
+    - [set\_encoder(id, joint\_id, encoder, speed)](#set_encoderid-joint_id-encoder-speed)
+    - [set\_encoders(id, encoders, speed)](#set_encodersid-encoders-speed)
+    - [set\_end\_type(id, end)](#set_end_typeid-end)
+    - [set\_encoders\_drag(id, encoders, speeds)](#set_encoders_dragid-encoders-speeds)
+    - [set\_free\_mode(id, value)](#set_free_modeid-value)
+    - [set\_fresh\_mode(id, mode)](#set_fresh_modeid-mode)
+    - [set\_gripper\_calibration(id)](#set_gripper_calibrationid)
+    - [set\_gripper\_state(id, flag)](#set_gripper_stateid-flag)
+    - [set\_gripper\_value(id, value, speed)](#set_gripper_valueid-value-speed)
+    - [set\_joint\_current(id, joint\_id, current)](#set_joint_currentid-joint_id-current)
+    - [set\_joint\_max(id, joint\_id, angle)](#set_joint_maxid-joint_id-angle)
+    - [set\_joint\_min(id, joint\_id, angle)](#set_joint_minid-joint_id-angle)
+    - [set\_movement\_type(id, move\_type)](#set_movement_typeid-move_type)
+    - [set\_pin\_mode(id, pin\_no, pin\_mode)](#set_pin_modeid-pin_no-pin_mode)
+    - [set\_plan\_acceleration(id, acceleration)](#set_plan_accelerationid-acceleration)
+    - [set\_plan\_speed(id, speed)](#set_plan_speedid-speed)
+    - [set\_pwm\_output()](#set_pwm_output-1)
+    - [set\_reference\_frame(id, rftype)](#set_reference_frameid-rftype)
+    - [set\_robot\_id(id, new\_id)](#set_robot_idid-new_id)
+    - [set\_servo\_calibration(id, servo\_no)](#set_servo_calibrationid-servo_no)
+    - [set\_servo\_data(id, servo\_no, data\_id, value)](#set_servo_dataid-servo_no-data_id-value)
+    - [set\_speed(id, speed)](#set_speedid-speed)
+    - [set\_tool\_reference(id, coords)](#set_tool_referenceid-coords)
+    - [set\_world\_reference(id, coords)](#set_world_referenceid-coords)
     - [stop(id)](#stopid)
-    - [write_base_coord(id, axis, coord, speed)](#write_base_coordid-axis-coord-speed)
-    - [write_base_coords(id, coords, speed)](#write_base_coordsid-coords-speed)
-    - [get_radians(id)](#get_radiansid)
-    - [send_radians(id, radians, speed)](#send_radiansid-radians-speed)
-    - [set_gpio_input(pin)](#set_gpio_inputpin)
-    - [set_gpio_mode(pin_no, mode)](#set_gpio_modepin_no-mode)
-    - [set_gpio_output(pin, v)](#set_gpio_outputpin-v)
-    - [set_gpio_pwm(pin, baud, dc)](#set_gpio_pwmpin-baud-dc)
+    - [write\_base\_coord(id, axis, coord, speed)](#write_base_coordid-axis-coord-speed)
+    - [write\_base\_coords(id, coords, speed)](#write_base_coordsid-coords-speed)
+    - [get\_radians(id)](#get_radiansid)
+    - [send\_radians(id, radians, speed)](#send_radiansid-radians-speed)
+    - [set\_gpio\_input(pin)](#set_gpio_inputpin)
+    - [set\_gpio\_mode(pin\_no, mode)](#set_gpio_modepin_no-mode)
+    - [set\_gpio\_output(pin, v)](#set_gpio_outputpin-v)
+    - [set\_gpio\_pwm(pin, baud, dc)](#set_gpio_pwmpin-baud-dc)
 - [MyBuddyEmoticon](#mybuddyemoticon)
-  - [MyBuddyEmoticon(file_path: list = [], window_size: tuple = [], loop=False)](#mybuddyemoticonfile_path-list---window_size-tuple---loopfalse)
-    - [add_file_path(path_time: list)](#add_file_pathpath_time-list)
-    - [del_file_path(index: int)](#del_file_pathindex-int)
-    - [file_path](#file_path)
+  - [MyBuddyEmoticon(file\_path: list = \[\], window\_size: tuple = \[\], loop=False)](#mybuddyemoticonfile_path-list---window_size-tuple---loopfalse)
+    - [add\_file\_path(path\_time: list)](#add_file_pathpath_time-list)
+    - [del\_file\_path(index: int)](#del_file_pathindex-int)
+    - [file\_path](#file_path)
     - [join()](#join)
     - [pause()](#pause-1)
     - [run()](#run)
     - [start()](#start)
   
 <!-- vim-markdown-toc -->
 </details>
@@ -389,14 +389,33 @@
 
 - **Returns**
 
   - `1`: connected
   - `0`: not connected
   - `-1`: error
 
+### get_error_information
+
+- **Prototype**: `get_error_information()`
+
+- **Description**: Obtaining robot error information.
+
+- **Returns**
+
+  - `0`: No error message.
+  - `1 ~ 6`: The corresponding joint exceeds the limit position.
+  - `32`: Kinematics inverse solution has no solution.
+  - `33 ~ 34`: Linear motion has no adjacent solution.
+
+### clear_error_information
+
+- **Prototype**: `clear_error_information()`
+
+- **Description**: Clear robot error message.
+
 ## MDI mode and operation
 
 ### get_angles
 
 - **Prototype**: `get_angles()`
 
 - **Description**: Get the degree of all joints.
@@ -1111,14 +1130,21 @@
 - **Description**: Set planning acceleration.
 
 - **Parameters**
 
   - `acceleration` (`int`) 0 - 100.
   - `is_linear` (`int`): 0 / 1 (0 ->joint, 1 -> line)
 
+
+### set_gservo_round
+
+- **Prototype**: `set_gservo_round()`
+
+- **Description**: Drive the 9g steering gear clockwise for one revolution.
+
 ### get_servo_speeds
 
 - **Prototype**: `get_servo_speeds()`
 
 - **Description**: Get joint velocity.
 
 - **Return**: `list` Speed of each joint.
@@ -1280,44 +1306,31 @@
 
 ```python
 # demo
 from pymycobot import MyCobotSocket
 # Port 9000 is used by default
 mc = MyCobotSocket("192.168.10.10","9000")
 
-mc.connect("/dev/ttyAMA0","1000000")
-
 res = mc.get_angles()
 print(res)
 
 mc.send_angles([0,0,0,0,0,0],20)
 ...
 
 ```
 
 ### Server
 
-Server file is in the demo folder
+Server file is in the `demo folder`,For details, please check the [Server.py](../demo/Server.py) file in the demo folder
 
 ## socket control
 
 > Note:
 > Most of the methods are the same as the class mycobot, only the new methods are listed here.
 
-### connect
-
-- **Prototype**: `connect(serialport, baudrate, timeout)`
-
-- **Description**: Connect the robot arm through the serial port and baud rate
-
-- **Parameters**
-
-  - `serialport`: (`str`) default `/dev/ttyAMA0`.
-  - `baudrate`: default `1000000`.
-  - `timeout`: default `0.1`.
 
 ### set_gpio_mode
 
 - **Prototype**: `set_gpio_mode(mode)`
 
 - **Description**: Set pin coding method.
 
@@ -1359,16 +1372,14 @@
 
 ```python
 # Set up the demo of the suction pump
 import time
 from pymycobot import MyCobotSocket
 # connect server
 m = MyCobotSocket("192.168.10.10", '9000')
-# default serialport:/dev/ttyAMA0 Baudrate:1000000
-m.connect()
 
 m.set_gpio_mode("BCM")
 m.set_gpio_out(20, "out")
 m.set_gpio_out(21, "out")
 # open
 m.set_gpio_output(20, 0)
 m.set_gpio_output(21, 0)
@@ -2311,27 +2322,17 @@
 
 * **Parameters**
 
   * **id** – 0/1/2/3 (ALL/L/R/W)
 
   * **speed** (_int_) – (0 ~ 100).
 
-### set_pwm_output(id, channel, frequency, pin_val)
-
-PWM control
-
-* **Parameters**
-
-  * **id** – 1/2 (L/R)
-
-  * **channel** (_int_) – IO number (1 - 5).
-
-  * **frequency** (_int_) – clock frequency (0/1: 0 - 1Mhz 1 - 10Mhz)
+### set_pwm_output()
 
-  * **pin_val** (_int_) – Duty cycle 0 ~ 100: 0 ~ 100%
+Set PWM output
 
 ### set_reference_frame(id, rftype)
 
 Set the base coordinate system
 
 * **Parameters**
 
@@ -2589,9 +2590,7 @@
 
 
 ### start()
 Start playing
 
 ---
 More demo can go to [here](../demo).
-
-
```

### Comparing `pymycobot-3.1.0b1/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.1/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.0b1/setup.py` & `pymycobot-3.1.1/setup.py`

 * *Files identical despite different names*

