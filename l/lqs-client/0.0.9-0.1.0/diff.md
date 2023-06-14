# Comparing `tmp/lqs-client-0.0.9.tar.gz` & `tmp/lqs-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqs-client-0.0.9.tar", last modified: Wed Nov  2 14:53:18 2022, max compression
+gzip compressed data, was "lqs-client-0.1.0.tar", last modified: Mon Jun  5 19:28:06 2023, max compression
```

## Comparing `lqs-client-0.0.9.tar` & `lqs-client-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,180 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.956888 lqs-client-0.0.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3215 2022-11-02 14:53:18.956888 lqs-client-0.0.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2716 2022-11-01 17:35:01.000000 lqs-client-0.0.9/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.948888 lqs-client-0.0.9/lqs_client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1846 2022-11-01 17:35:32.000000 lqs-client-0.0.9/lqs_client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2022-11-01 15:39:56.000000 lqs-client-0.0.9/lqs_client/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.956888 lqs-client-0.0.9/lqs_client/interface/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2022-10-04 18:08:06.000000 lqs-client-0.0.9/lqs_client/interface/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3191 2022-11-02 14:52:48.000000 lqs-client-0.0.9/lqs_client/interface/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5855 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/creator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/deleter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/getter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16405 2022-11-01 17:32:17.000000 lqs-client-0.0.9/lqs_client/interface/lister.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16849 2022-10-04 19:16:48.000000 lqs-client-0.0.9/lqs_client/interface/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2221 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/updater.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.952888 lqs-client-0.0.9/lqs_client.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3215 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-09-29 18:21:02.000000 lqs-client-0.0.9/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-11-02 14:53:18.956888 lqs-client-0.0.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2022-11-02 14:52:26.000000 lqs-client-0.0.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:06.001140 lqs-client-0.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2022-12-19 19:59:13.000000 lqs-client-0.1.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4445 2023-06-05 19:28:06.001140 lqs-client-0.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3946 2023-03-31 19:13:53.000000 lqs-client-0.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.921141 lqs-client-0.1.0/lqs_client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5721 2023-04-25 20:40:06.000000 lqs-client-0.1.0/lqs_client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2022-11-01 15:39:56.000000 lqs-client-0.1.0/lqs_client/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.921141 lqs-client-0.1.0/lqs_client/definitions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-19 19:48:58.000000 lqs-client-0.1.0/lqs_client/definitions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/actionlib_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.925141 lqs-client-0.1.0/lqs_client/definitions/actionlib_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2022-12-20 19:36:05.000000 lqs-client-0.1.0/lqs_client/definitions/actionlib_msgs/msg/GoalID.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1626 2022-12-20 19:36:05.000000 lqs-client-0.1.0/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2022-12-20 19:36:05.000000 lqs-client-0.1.0/lqs_client/definitions/actionlib_msgs/msg/GoalStatusArray.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/diagnostic_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.925141 lqs-client-0.1.0/lqs_client/definitions/diagnostic_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2022-12-20 19:36:25.000000 lqs-client-0.1.0/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      426 2022-12-20 19:36:25.000000 lqs-client-0.1.0/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticStatus.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2022-12-20 19:36:25.000000 lqs-client-0.1.0/lqs_client/definitions/diagnostic_msgs/msg/KeyValue.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.949140 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Accel.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/AccelStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/AccelWithCovariance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/AccelWithCovarianceStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Inertia.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/InertiaStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Point.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Point32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/PointStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Polygon.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      104 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/PolygonStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Pose.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/PoseArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/PoseStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/PoseWithCovariance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      122 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/PoseWithCovarianceStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Quaternion.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/QuaternionStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Transform.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/TransformStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Twist.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/TwistStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/TwistWithCovariance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/TwistWithCovarianceStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      382 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Vector3.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      103 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Vector3Stamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/Wrench.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.0/lqs_client/definitions/geometry_msgs/msg/WrenchStamped.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/nav_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.949140 lqs-client-0.1.0/lqs_client/definitions/nav_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2022-12-20 19:36:31.000000 lqs-client-0.1.0/lqs_client/definitions/nav_msgs/msg/GridCells.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2022-12-20 19:36:31.000000 lqs-client-0.1.0/lqs_client/definitions/nav_msgs/msg/MapMetaData.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2022-12-20 19:36:31.000000 lqs-client-0.1.0/lqs_client/definitions/nav_msgs/msg/OccupancyGrid.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2022-12-20 19:36:31.000000 lqs-client-0.1.0/lqs_client/definitions/nav_msgs/msg/Odometry.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2022-12-20 19:36:31.000000 lqs-client-0.1.0/lqs_client/definitions/nav_msgs/msg/Path.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/rosgraph_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.953141 lqs-client-0.1.0/lqs_client/definitions/rosgraph_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      184 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/rosgraph_msgs/msg/Clock.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/rosgraph_msgs/msg/Log.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      722 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.969140 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6284 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1008 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      640 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      986 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1362 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/Image.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1206 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/Imu.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/JointState.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/Joy.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/JoyFeedback.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/JoyFeedbackArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/LaserEcho.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1519 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1596 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      425 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/PointField.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/Range.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      618 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      331 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/Temperature.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-20 19:36:33.000000 lqs-client-0.1.0/lqs_client/definitions/sensor_msgs/msg/TimeReference.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/shape_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.969140 lqs-client-0.1.0/lqs_client/definitions/shape_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      196 2022-12-20 19:36:36.000000 lqs-client-0.1.0/lqs_client/definitions/shape_msgs/msg/Mesh.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2022-12-20 19:36:36.000000 lqs-client-0.1.0/lqs_client/definitions/shape_msgs/msg/MeshTriangle.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2022-12-20 19:36:36.000000 lqs-client-0.1.0/lqs_client/definitions/shape_msgs/msg/Plane.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2022-12-20 19:36:36.000000 lqs-client-0.1.0/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/std_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.985140 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Bool.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Byte.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/ByteMultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Char.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/ColorRGBA.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Duration.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Empty.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Float32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Float32MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Float64.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Float64MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      551 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Header.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int16.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int16MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int32MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int64.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int64MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int8.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Int8MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      141 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/MultiArrayDimension.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      911 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/String.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/Time.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt16.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt16MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt32MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt64.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt64MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt8.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.0/lqs_client/definitions/std_msgs/msg/UInt8MultiArray.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.917141 lqs-client-0.1.0/lqs_client/definitions/stereo_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.989140 lqs-client-0.1.0/lqs_client/definitions/stereo_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1137 2022-12-20 19:36:39.000000 lqs-client-0.1.0/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.921141 lqs-client-0.1.0/lqs_client/definitions/trajectory_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.989140 lqs-client-0.1.0/lqs_client/definitions/trajectory_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2022-12-20 19:36:42.000000 lqs-client-0.1.0/lqs_client/definitions/trajectory_msgs/msg/JointTrajectory.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:42.000000 lqs-client-0.1.0/lqs_client/definitions/trajectory_msgs/msg/JointTrajectoryPoint.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      476 2022-12-20 19:36:42.000000 lqs-client-0.1.0/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectory.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:42.000000 lqs-client-0.1.0/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectoryPoint.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.921141 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.997140 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      827 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      808 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2586 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerInit.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerPose.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      950 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1935 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/Marker.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/MarkerArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1586 2022-12-20 19:36:44.000000 lqs-client-0.1.0/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.997140 lqs-client-0.1.0/lqs_client/gen/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-04-26 13:56:12.000000 lqs-client-0.1.0/lqs_client/gen/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:06.001140 lqs-client-0.1.0/lqs_client/interface/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      239 2023-04-11 20:07:37.000000 lqs-client-0.1.0/lqs_client/interface/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8696 2023-06-05 19:22:37.000000 lqs-client-0.1.0/lqs_client/interface/ark_deserialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2023-03-31 19:14:09.000000 lqs-client-0.1.0/lqs_client/interface/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6030 2022-11-30 15:48:08.000000 lqs-client-0.1.0/lqs_client/interface/creator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2022-11-01 15:43:34.000000 lqs-client-0.1.0/lqs_client/interface/deleter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9312 2023-05-19 14:25:06.000000 lqs-client-0.1.0/lqs_client/interface/fs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2022-11-01 15:43:34.000000 lqs-client-0.1.0/lqs_client/interface/getter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11610 2023-05-19 14:25:06.000000 lqs-client-0.1.0/lqs_client/interface/input_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18199 2023-06-05 19:22:37.000000 lqs-client-0.1.0/lqs_client/interface/lister.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16489 2023-06-05 19:22:37.000000 lqs-client-0.1.0/lqs_client/interface/message_converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6849 2023-05-09 21:11:30.000000 lqs-client-0.1.0/lqs_client/interface/node.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18309 2023-06-05 19:22:37.000000 lqs-client-0.1.0/lqs_client/interface/ros_deserialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27304 2023-05-19 14:25:06.000000 lqs-client-0.1.0/lqs_client/interface/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15734 2023-04-24 20:09:51.000000 lqs-client-0.1.0/lqs_client/interface/terminal.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2221 2022-11-01 15:43:34.000000 lqs-client-0.1.0/lqs_client/interface/updater.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15935 2023-06-05 19:22:37.000000 lqs-client-0.1.0/lqs_client/interface/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 19:28:05.921141 lqs-client-0.1.0/lqs_client.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4445 2023-06-05 19:28:05.000000 lqs-client-0.1.0/lqs_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7647 2023-06-05 19:28:05.000000 lqs-client-0.1.0/lqs_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-05 19:28:05.000000 lqs-client-0.1.0/lqs_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-06-05 19:28:05.000000 lqs-client-0.1.0/lqs_client.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-05 19:28:05.000000 lqs-client-0.1.0/lqs_client.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-09-29 18:21:02.000000 lqs-client-0.1.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-05 19:28:06.001140 lqs-client-0.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1261 2023-06-05 19:27:05.000000 lqs-client-0.1.0/setup.py
```

### Comparing `lqs-client-0.0.9/PKG-INFO` & `lqs-client-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.0.9
+Version: 0.1.0
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -80,14 +80,44 @@
 
 `LQS_PRETTY`
 
 &ensp;&ensp;A boolean parameter indicating whether or not to "prettify" the output results.  Useful when using the client in the command line.  Default is `false`.
 
 &ensp;&ensp;This parameter can be supplied/overrident with the `pretty` parameter.
 
+`LQS_VERBOSE`
+
+&ensp;&ensp;A boolean parameter indicating whether to log debug information.  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `verbose` parameter.
+
+`LQS_DRY_RUN`
+
+&ensp;&ensp;A boolean parameter indicating whether to execute actual API requests.  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `dry_run` parameter.
+
+`LQS_RETRY_COUNT`
+
+&ensp;&ensp;An integer parameter greater than or equal to 0 indicating the number of times we should retry failed API requests.  Default is `4`
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_count` parameter.
+
+`LQS_RETRY_DELAY`
+
+&ensp;&ensp;An integer parameter greater than or equal to 0 indicating the initial value, in seconds, we use for exponential backoff when waiting to retry a failed request.  Default is `4`
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_delay` parameter.
+
+`LQS_RETRY_AGRESSIVE`
+
+&ensp;&ensp;A boolean parameter indicating whether we should retry on "expected" errors from LogQS (such as "BadRequest", "Conflict", etc.).  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_aggressive` parameter.
+
 ## Development
 
 The LogQS Client module source is located in `lqs-client` and it's Python requirements are listed in the `requirements.txt` file.  You can install it locally with `pip install .`.
 
 The project uses Python 3.9, which may require some dependencies to be required.  In one go,
 
     sudo apt install python3.9 python3.9-dev python3.9-distutils python3.9-venv
```

### Comparing `lqs-client-0.0.9/README.md` & `lqs-client-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -66,14 +66,44 @@
 
 `LQS_PRETTY`
 
 &ensp;&ensp;A boolean parameter indicating whether or not to "prettify" the output results.  Useful when using the client in the command line.  Default is `false`.
 
 &ensp;&ensp;This parameter can be supplied/overrident with the `pretty` parameter.
 
+`LQS_VERBOSE`
+
+&ensp;&ensp;A boolean parameter indicating whether to log debug information.  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `verbose` parameter.
+
+`LQS_DRY_RUN`
+
+&ensp;&ensp;A boolean parameter indicating whether to execute actual API requests.  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `dry_run` parameter.
+
+`LQS_RETRY_COUNT`
+
+&ensp;&ensp;An integer parameter greater than or equal to 0 indicating the number of times we should retry failed API requests.  Default is `4`
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_count` parameter.
+
+`LQS_RETRY_DELAY`
+
+&ensp;&ensp;An integer parameter greater than or equal to 0 indicating the initial value, in seconds, we use for exponential backoff when waiting to retry a failed request.  Default is `4`
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_delay` parameter.
+
+`LQS_RETRY_AGRESSIVE`
+
+&ensp;&ensp;A boolean parameter indicating whether we should retry on "expected" errors from LogQS (such as "BadRequest", "Conflict", etc.).  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_aggressive` parameter.
+
 ## Development
 
 The LogQS Client module source is located in `lqs-client` and it's Python requirements are listed in the `requirements.txt` file.  You can install it locally with `pip install .`.
 
 The project uses Python 3.9, which may require some dependencies to be required.  In one go,
 
     sudo apt install python3.9 python3.9-dev python3.9-distutils python3.9-venv
```

### Comparing `lqs-client-0.0.9/lqs_client/interface/creator.py` & `lqs-client-0.1.0/lqs_client/interface/creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,45 +101,47 @@
         return result
 
     @output_decorator
     def message_type(
         self,
         group_id: UUID,
         name: str,
-        md5: str,
         definition: str,
+        md5: Optional[str] = None,
         note: Optional[str] = None,
     ):
         args = locals()
         data = self._get_payload_data(args, [])
         result = self._create_resource(f"messageTypes", data)
         return result
 
     @output_decorator
     def record(
         self,
         timestamp: float,
         topic_id: UUID,
-        offset: int,
-        length: int,
-        data_offset: int,
-        data_length: int,
+        offset: Optional[int] = None,
+        length: Optional[int] = None,
+        data_offset: Optional[int] = None,
+        data_length: Optional[int] = None,
         errored: Optional[bool] = False,
         archived: Optional[bool] = False,
         error: Optional[dict] = None,
         note: Optional[str] = None,
         chunk_compression: Optional[str] = None,
         chunk_offset: Optional[int] = None,
         chunk_length: Optional[int] = None,
         s3_bucket: Optional[str] = None,
         s3_key: Optional[str] = None,
         format: Optional[LogFormat] = None,
         message_data: Optional[dict] = None,
         message_type_id: Optional[UUID] = None,
         ingestion_id: Optional[UUID] = None,
+        payload_bytes: Optional[str] = None,
+        payload_dict: Optional[dict] = None,
     ):
         args = locals()
         data = self._get_payload_data(args, ["topic_id"])
         result = self._create_resource(f"topics/{topic_id}/records", data)
         return result
 
     @output_decorator
```

### Comparing `lqs-client-0.0.9/lqs_client/interface/deleter.py` & `lqs-client-0.1.0/lqs_client/interface/deleter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.9/lqs_client/interface/getter.py` & `lqs-client-0.1.0/lqs_client/interface/getter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.9/lqs_client/interface/lister.py` & `lqs-client-0.1.0/lqs_client/interface/lister.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,28 +48,30 @@
         group_id: Optional[UUID] = None,
         status: Optional[ProcessStatus] = None,
         processing: Optional[bool] = None,
         queued: Optional[bool] = None,
         cancelled: Optional[bool] = None,
         errored: Optional[bool] = None,
         archived: Optional[bool] = None,
+        completed: Optional[bool] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         format: Optional[LogFormat] = None,
         s3_bucket: Optional[str] = None,
         s3_key: Optional[str] = None,
         s3_key_prefix: Optional[str] = None,
         size_null: Optional[bool] = None,
         size_gte: Optional[int] = None,
         size_lte: Optional[int] = None,
         progress_null: Optional[bool] = None,
         progress_gte: Optional[float] = None,
         progress_lte: Optional[float] = None,
         error_like: Optional[str] = None,
         note_like: Optional[str] = None,
+        context_filter: Optional[dict] = None,
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
         updated_by_null: Optional[bool] = None,
         deleted_by_null: Optional[bool] = None,
         updated_at_null: Optional[bool] = None,
         deleted_at_null: Optional[bool] = None,
@@ -192,14 +194,15 @@
         group_id: Optional[UUID] = None,
         status: Optional[ProcessStatus] = None,
         processing: Optional[bool] = None,
         queued: Optional[bool] = None,
         cancelled: Optional[bool] = None,
         errored: Optional[bool] = None,
         archived: Optional[bool] = None,
+        completed: Optional[bool] = None,
         format: Optional[LogFormat] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         s3_bucket: Optional[str] = None,
         s3_key: Optional[str] = None,
         s3_key_prefix: Optional[str] = None,
         size_null: Optional[bool] = None,
@@ -207,14 +210,15 @@
         size_lte: Optional[int] = None,
         progress_null: Optional[bool] = None,
         progress_gte: Optional[float] = None,
         progress_lte: Optional[float] = None,
         meta_like: Optional[str] = None,
         error_like: Optional[str] = None,
         note_like: Optional[str] = None,
+        context_filter: Optional[dict] = None,
         start_offset_null: Optional[bool] = None,
         start_offset_gte: Optional[int] = None,
         start_offset_lte: Optional[int] = None,
         end_offset_null: Optional[bool] = None,
         end_offset_gte: Optional[int] = None,
         end_offset_lte: Optional[int] = None,
         created_by: Optional[UUID] = None,
@@ -240,23 +244,25 @@
     def log(
         self,
         offset: Optional[int] = 0,
         limit: Optional[int] = 10,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         group_id: Optional[UUID] = None,
+        locked: Optional[bool] = None,
         start_time_null: Optional[bool] = None,
         start_time_gte: Optional[float] = None,
         start_time_lte: Optional[float] = None,
         end_time_null: Optional[bool] = None,
         end_time_gte: Optional[float] = None,
         end_time_lte: Optional[float] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         note_like: Optional[str] = None,
+        context_filter: Optional[dict] = None,
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
         updated_by_null: Optional[bool] = None,
         deleted_by_null: Optional[bool] = None,
         updated_at_null: Optional[bool] = None,
         deleted_at_null: Optional[bool] = None,
@@ -281,14 +287,15 @@
         sort: Optional[str] = "ASC",
         group_id: Optional[UUID] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         md5: Optional[str] = None,
         definition_like: Optional[str] = None,
         note_like: Optional[str] = None,
+        context_filter: Optional[dict] = None,
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
         updated_by_null: Optional[bool] = None,
         deleted_by_null: Optional[bool] = None,
         updated_at_null: Optional[bool] = None,
         deleted_at_null: Optional[bool] = None,
@@ -310,28 +317,33 @@
         topic_id: UUID,
         offset: Optional[int] = 0,
         limit: Optional[int] = 10,
         order: Optional[str] = "timestamp",
         sort: Optional[str] = "ASC",
         log_id: Optional[UUID] = None,
         ingestion_id: Optional[UUID] = None,
-        data_filter: Optional[object] = None,
+        errored: Optional[bool] = None,
+        archived: Optional[bool] = None,
+        data_filter: Optional[dict] = None,
+        context_filter: Optional[dict] = None,
         frequency: Optional[float] = None,
         timestamp_gt: Optional[float] = None,
         timestamp_lt: Optional[float] = None,
         timestamp_gte: Optional[float] = None,
         timestamp_lte: Optional[float] = None,
         length_gte: Optional[int] = None,
         length_lte: Optional[int] = None,
         data_length_gte: Optional[int] = None,
         data_length_lte: Optional[int] = None,
         offset_gte: Optional[int] = None,
         offset_lte: Optional[int] = None,
         data_offset_gte: Optional[int] = None,
         data_offset_lte: Optional[int] = None,
+        nanosecond_gte: Optional[int] = None,
+        nanosecond_lte: Optional[int] = None,
         error_like: Optional[str] = None,
         note_like: Optional[str] = None,
         include_image: Optional[bool] = False,
         include_bytes: Optional[bool] = False,
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -359,17 +371,26 @@
         offset: Optional[int] = 0,
         limit: Optional[int] = 10,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         log_id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         message_type_id: Optional[UUID] = None,
+        associated_topic_id: Optional[UUID] = None,
         ingestion_id: Optional[UUID] = None,
+        locked: Optional[bool] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
+        context_filter: Optional[dict] = None,
+        type_name: Optional[str] = None,
+        type_name_like: Optional[str] = None,
+        type_encoding: Optional[str] = None,
+        type_encoding_like: Optional[str] = None,
+        type_data: Optional[str] = None,
+        type_data_like: Optional[str] = None,
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
         updated_by_null: Optional[bool] = None,
         deleted_by_null: Optional[bool] = None,
         updated_at_null: Optional[bool] = None,
         deleted_at_null: Optional[bool] = None,
@@ -409,7 +430,41 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         args = locals()
         resource_path = f"users" + self._get_url_param_string(args, [])
         result = self._get_resource(resource_path)
         return result
+
+    # Plural methods
+    def api_keys(self, **kwargs):
+        return self.api_key(**kwargs)
+
+    def extractions(self, **kwargs):
+        return self.extraction(**kwargs)
+
+    def extraction_topics(self, **kwargs):
+        return self.extraction_topic(**kwargs)
+
+    def groups(self, **kwargs):
+        return self.group(**kwargs)
+
+    def group_associations(self, **kwargs):
+        return self.group_association(**kwargs)
+
+    def ingestions(self, **kwargs):
+        return self.ingestion(**kwargs)
+
+    def logs(self, **kwargs):
+        return self.log(**kwargs)
+
+    def message_types(self, **kwargs):
+        return self.message_type(**kwargs)
+
+    def records(self, **kwargs):
+        return self.record(**kwargs)
+
+    def topics(self, **kwargs):
+        return self.topic(**kwargs)
+
+    def users(self, **kwargs):
+        return self.user(**kwargs)
```

### Comparing `lqs-client-0.0.9/lqs_client/interface/updater.py` & `lqs-client-0.1.0/lqs_client/interface/updater.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.9/lqs_client.egg-info/PKG-INFO` & `lqs-client-0.1.0/lqs_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.0.9
+Version: 0.1.0
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -80,14 +80,44 @@
 
 `LQS_PRETTY`
 
 &ensp;&ensp;A boolean parameter indicating whether or not to "prettify" the output results.  Useful when using the client in the command line.  Default is `false`.
 
 &ensp;&ensp;This parameter can be supplied/overrident with the `pretty` parameter.
 
+`LQS_VERBOSE`
+
+&ensp;&ensp;A boolean parameter indicating whether to log debug information.  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `verbose` parameter.
+
+`LQS_DRY_RUN`
+
+&ensp;&ensp;A boolean parameter indicating whether to execute actual API requests.  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `dry_run` parameter.
+
+`LQS_RETRY_COUNT`
+
+&ensp;&ensp;An integer parameter greater than or equal to 0 indicating the number of times we should retry failed API requests.  Default is `4`
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_count` parameter.
+
+`LQS_RETRY_DELAY`
+
+&ensp;&ensp;An integer parameter greater than or equal to 0 indicating the initial value, in seconds, we use for exponential backoff when waiting to retry a failed request.  Default is `4`
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_delay` parameter.
+
+`LQS_RETRY_AGRESSIVE`
+
+&ensp;&ensp;A boolean parameter indicating whether we should retry on "expected" errors from LogQS (such as "BadRequest", "Conflict", etc.).  Default is `false`.
+
+&ensp;&ensp;This parameter can be supplied/overriden with the `retry_aggressive` parameter.
+
 ## Development
 
 The LogQS Client module source is located in `lqs-client` and it's Python requirements are listed in the `requirements.txt` file.  You can install it locally with `pip install .`.
 
 The project uses Python 3.9, which may require some dependencies to be required.  In one go,
 
     sudo apt install python3.9 python3.9-dev python3.9-distutils python3.9-venv
```

### Comparing `lqs-client-0.0.9/setup.py` & `lqs-client-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lqs-client",
-    version="0.0.9",
+    version="0.1.0",
     author="Nathan Margaglio",
     author_email="nmargaglio@carnegierobotics.com",
     description="LogQS Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/carnegierobotics/LogQS-Client",
     project_urls={
         "Bug Tracker": "https://github.com/carnegierobotics/LogQS-Client/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=["lqs_client", "lqs_client.interface"],
+    include_package_data=True,
+    packages=[
+        "lqs_client",
+        "lqs_client.interface",
+        "lqs_client.gen",
+        "lqs_client.definitions",
+    ],
     python_requires=">=3.6",
     install_requires=[
         "fire==0.4.*",
         "python-dotenv==0.*",
         "requests==2.*",
         "xmltodict==0.13.*",
+        "py3rosmsgs==1.18.*",
+        "rospkg==1.4.*",
+        "tqdm==4.*",
+        "boto3==1.26.*",
+        "Pillow==9.0.*",
+        "numpy==1.22.*",
+        "av==9.2.*",
+        "lz4==4.0.*",
+        "zstd==1.5.*",
     ],
 )
```

