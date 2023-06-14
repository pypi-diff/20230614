# Comparing `tmp/GlyCONFORMER-0.0.1.tar.gz` & `tmp/GlyCONFORMER-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlyCONFORMER-0.0.1.tar", last modified: Fri Jul 29 11:49:43 2022, max compression
+gzip compressed data, was "GlyCONFORMER-1.0.0.tar", last modified: Wed Jun 14 09:46:48 2023, max compression
```

## Comparing `GlyCONFORMER-0.0.1.tar` & `GlyCONFORMER-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,197 @@
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2022-07-29 11:49:14.855260 GlyCONFORMER-0.0.1/
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2022-07-29 11:49:14.806259 GlyCONFORMER-0.0.1/GlyCONFORMER.egg-info/
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1311 2022-07-29 11:49:14.000000 GlyCONFORMER-0.0.1/GlyCONFORMER.egg-info/PKG-INFO
--rw-r--r--   0 grothaus (20118) hmi      (20000)      307 2022-07-29 11:49:14.000000 GlyCONFORMER-0.0.1/GlyCONFORMER.egg-info/SOURCES.txt
--rw-r--r--   0 grothaus (20118) hmi      (20000)        1 2022-07-29 11:49:14.000000 GlyCONFORMER-0.0.1/GlyCONFORMER.egg-info/dependency_links.txt
--rw-r--r--   0 grothaus (20118) hmi      (20000)       37 2022-07-29 11:49:14.000000 GlyCONFORMER-0.0.1/GlyCONFORMER.egg-info/requires.txt
--rw-r--r--   0 grothaus (20118) hmi      (20000)       13 2022-07-29 11:49:14.000000 GlyCONFORMER-0.0.1/GlyCONFORMER.egg-info/top_level.txt
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1311 2022-07-29 11:49:14.853260 GlyCONFORMER-0.0.1/PKG-INFO
--rw-r--r--   0 grothaus (20118) hmi      (20000)      537 2022-07-29 10:23:52.000000 GlyCONFORMER-0.0.1/README.rst
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2022-07-29 11:49:14.851260 GlyCONFORMER-0.0.1/glyconformer/
--rw-r--r--   0 grothaus (20118) hmi      (20000)      142 2022-07-29 11:37:37.000000 GlyCONFORMER-0.0.1/glyconformer/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)    24739 2022-07-29 10:29:46.000000 GlyCONFORMER-0.0.1/glyconformer/glycan_conformer.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)    11968 2022-07-29 11:38:05.000000 GlyCONFORMER-0.0.1/glyconformer/plot.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)     4006 2022-07-29 10:33:03.000000 GlyCONFORMER-0.0.1/glyconformer/process_files.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)       38 2022-07-29 11:49:14.855260 GlyCONFORMER-0.0.1/setup.cfg
--rw-r--r--   0 grothaus (20118) hmi      (20000)      960 2022-07-29 11:26:42.000000 GlyCONFORMER-0.0.1/setup.py
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.919331 GlyCONFORMER-1.0.0/
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.385323 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     3764 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/PKG-INFO
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     6534 2023-06-14 09:46:48.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/SOURCES.txt
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        1 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/dependency_links.txt
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       37 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/requires.txt
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       29 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/top_level.txt
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.388323 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.456324 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      121 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_omega3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1334 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1421 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      572 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      598 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      811 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        9 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       26 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.545325 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      175 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega3_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1305 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi3_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi3_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      716 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      872 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1143 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       29 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       26 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.681327 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      299 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega11_15.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega1_18.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega3_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi11_12.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi11_15.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi12_13.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi13_14.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi15_16.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi16_17.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi1_18.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1247 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi3_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1421 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1305 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi4_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1392 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi11_12.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi11_15.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi12_13.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi13_14.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi15_16.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi16_17.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi1_18.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi3_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi4_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1031 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1410 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1891 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       31 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)    10857 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/plumed_allangle.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       90 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.752328 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      125 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega1_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi1_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi1_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      553 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      596 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      799 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       27 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     6821 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/plumed_allangle.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       66 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.819329 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      102 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_omega3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_omega5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      488 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      489 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      668 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       18 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       54 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.906331 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      165 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_omega3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_omega7_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1363 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      957 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      957 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi7_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi7_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      638 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      680 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      959 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       19 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       54 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/separator.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)    35149 2023-06-13 07:44:59.000000 GlyCONFORMER-1.0.0/LICENSE
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     3764 2023-06-14 09:46:48.917331 GlyCONFORMER-1.0.0/PKG-INFO
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     3167 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/README.md
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.913331 GlyCONFORMER-1.0.0/glyconformer/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       76 2023-06-13 11:37:27.000000 GlyCONFORMER-1.0.0/glyconformer/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)    35691 2023-06-13 14:53:28.000000 GlyCONFORMER-1.0.0/glyconformer/lib.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       38 2023-06-14 09:46:48.920331 GlyCONFORMER-1.0.0/setup.cfg
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1034 2023-06-14 09:45:14.000000 GlyCONFORMER-1.0.0/setup.py
```

### Comparing `GlyCONFORMER-0.0.1/setup.py` & `GlyCONFORMER-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Education',
     'Programming Language :: Python :: 3'
     ]
 
 setup(name='GlyCONFORMER',
-      version='0.0.1',
+      version='1.0.0',
       description="GlyCONFORMERS is a Python package that assigns conformer strings to N-glycan conformers, based on their torsion angle values.",
       url="https://github.com/IsabellGrothaus/GlyCONFORMER",
-      long_description = (here / "README.rst").read_text(encoding="utf-8"),
+      long_description = (here / "README.md").read_text(),
+      long_description_content_type='text/markdown',
       author='Isabell Grothaus',
       author_email='grothaus@uni-bremen.de',
       classifiers=classifiers,
       keywords="glycan, conformer, classification, sugar, carbohydrates",
       license='GPL-3.0 license',
       packages=find_packages(),
+      package_data={'':['**/*.dat']},
       install_requires=[
                        "numpy","matplotlib","pandas","plumed","scipy"
                        ],
       )
```

