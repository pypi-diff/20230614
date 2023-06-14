# Comparing `tmp/GlyCONFORMER-1.0.0.tar.gz` & `tmp/GlyCONFORMER-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlyCONFORMER-1.0.0.tar", last modified: Wed Jun 14 09:46:48 2023, max compression
+gzip compressed data, was "GlyCONFORMER-1.0.1.tar", last modified: Wed Jun 14 11:07:57 2023, max compression
```

## Comparing `GlyCONFORMER-1.0.0.tar` & `GlyCONFORMER-1.0.1.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.919331 GlyCONFORMER-1.0.0/
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.385323 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/
--rw-r--r--   0 grothaus (20118) hmi      (20000)     3764 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/PKG-INFO
--rw-r--r--   0 grothaus (20118) hmi      (20000)     6534 2023-06-14 09:46:48.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/SOURCES.txt
--rw-r--r--   0 grothaus (20118) hmi      (20000)        1 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/dependency_links.txt
--rw-r--r--   0 grothaus (20118) hmi      (20000)       37 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/requires.txt
--rw-r--r--   0 grothaus (20118) hmi      (20000)       29 2023-06-14 09:46:47.000000 GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/top_level.txt
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.388323 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.456324 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/
--rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)      121 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_omega3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1334 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi3_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi7_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1421 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi3_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi7_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      572 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/info.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      598 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/maxima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      811 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/minima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)        9 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/omega_angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       26 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/separator.dat
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.545325 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/
--rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)      175 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega10_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega3_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega6_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi10_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1305 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi3_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi6_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi9_10.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi10_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi3_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi6_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi9_10.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      716 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/info.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      872 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/maxima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1143 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/minima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       29 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/omega_angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       26 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/separator.dat
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.681327 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/
--rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)      299 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega11_15.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega1_18.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega3_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi11_12.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi11_15.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi12_13.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi13_14.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi15_16.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi16_17.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi1_18.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1247 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi3_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1421 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1305 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi4_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi6_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1392 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi9_10.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi11_12.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi11_15.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi12_13.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi13_14.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi15_16.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi16_17.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi1_18.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi3_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi4_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi6_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi9_10.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1031 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/info.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1410 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/maxima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1891 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/minima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       31 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/omega_angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)    10857 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/plumed_allangle.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       90 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/separator.dat
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.752328 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/
--rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)      125 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega1_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega3_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega5_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi1_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi3_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi5_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi1_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi3_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi5_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      553 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/info.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      596 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/maxima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      799 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/minima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       27 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/omega_angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     6821 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/plumed_allangle.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       66 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/separator.dat
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.819329 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/
--rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)      102 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_omega3_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_omega5_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi3_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi5_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi3_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi5_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      488 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/info.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      489 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/maxima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      668 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/minima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       18 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/omega_angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       54 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/separator.dat
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.906331 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/
--rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)      165 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_omega3_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_omega7_10.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi10_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1363 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi3_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      957 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      957 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi7_10.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi7_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi10_11.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi1_2.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi2_3.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi3_4.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi3_7.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi4_5.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi5_6.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi7_10.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi7_8.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi8_9.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      638 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/info.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      680 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/maxima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)      959 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/minima.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       19 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/omega_angles.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)       54 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/separator.dat
--rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)    35149 2023-06-13 07:44:59.000000 GlyCONFORMER-1.0.0/LICENSE
--rw-r--r--   0 grothaus (20118) hmi      (20000)     3764 2023-06-14 09:46:48.917331 GlyCONFORMER-1.0.0/PKG-INFO
--rw-r--r--   0 grothaus (20118) hmi      (20000)     3167 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.0/README.md
-drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 09:46:48.913331 GlyCONFORMER-1.0.0/glyconformer/
--rw-r--r--   0 grothaus (20118) hmi      (20000)       76 2023-06-13 11:37:27.000000 GlyCONFORMER-1.0.0/glyconformer/__init__.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)    35691 2023-06-13 14:53:28.000000 GlyCONFORMER-1.0.0/glyconformer/lib.py
--rw-r--r--   0 grothaus (20118) hmi      (20000)       38 2023-06-14 09:46:48.920331 GlyCONFORMER-1.0.0/setup.cfg
--rw-r--r--   0 grothaus (20118) hmi      (20000)     1034 2023-06-14 09:45:14.000000 GlyCONFORMER-1.0.0/setup.py
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.689407 GlyCONFORMER-1.0.1/
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.106397 GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     3866 2023-06-14 11:07:55.000000 GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/PKG-INFO
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     6534 2023-06-14 11:07:56.000000 GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/SOURCES.txt
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        1 2023-06-14 11:07:55.000000 GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/dependency_links.txt
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       44 2023-06-14 11:07:55.000000 GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/requires.txt
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       29 2023-06-14 11:07:55.000000 GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/top_level.txt
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.109397 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.181398 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      121 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_omega3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1334 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1421 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      572 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      598 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      811 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        9 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       26 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.273400 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      175 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_omega10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_omega3_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_omega6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1305 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi3_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi3_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      716 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      872 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1143 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       29 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       26 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.417402 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      299 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_omega11_15.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_omega1_18.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_omega3_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi11_12.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi11_15.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi12_13.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi13_14.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi15_16.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi16_17.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi1_18.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1247 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi3_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1421 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1305 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi4_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1392 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi11_12.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi11_15.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi12_13.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi13_14.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi15_16.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi16_17.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi1_18.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi3_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi4_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi6_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi9_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1031 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1410 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1891 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       31 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)    10857 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/plumed_allangle.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       90 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.523404 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:22.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      125 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_omega1_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_omega3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_omega5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1450 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi1_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi1_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      553 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      596 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      799 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       27 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     6821 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/plumed_allangle.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       66 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.590405 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      102 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_omega3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_omega5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      928 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi3_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi5_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      488 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      489 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      668 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       18 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       54 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/separator.dat
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.679407 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      165 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_omega3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_omega7_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1363 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      957 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      957 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi7_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi10_11.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi1_2.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi2_3.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi3_4.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi3_7.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi4_5.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi5_6.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi7_10.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi7_8.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1479 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi8_9.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      638 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/info.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      680 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/maxima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)      959 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/minima.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       19 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/omega_angles.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       54 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/separator.dat
+-rw-r--r--   0 grothaus (20118) hmi      (20000)        0 2023-06-13 11:37:23.000000 GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)    35149 2023-06-13 07:44:59.000000 GlyCONFORMER-1.0.1/LICENSE
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     3866 2023-06-14 11:07:57.688407 GlyCONFORMER-1.0.1/PKG-INFO
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     3269 2023-06-14 11:06:35.000000 GlyCONFORMER-1.0.1/README.md
+drwxr-xr-x   0 grothaus (20118) hmi      (20000)        0 2023-06-14 11:07:57.684407 GlyCONFORMER-1.0.1/glyconformer/
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       76 2023-06-13 11:37:27.000000 GlyCONFORMER-1.0.1/glyconformer/__init__.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)    35691 2023-06-13 14:53:28.000000 GlyCONFORMER-1.0.1/glyconformer/lib.py
+-rw-r--r--   0 grothaus (20118) hmi      (20000)       38 2023-06-14 11:07:57.690407 GlyCONFORMER-1.0.1/setup.cfg
+-rw-r--r--   0 grothaus (20118) hmi      (20000)     1041 2023-06-14 11:07:37.000000 GlyCONFORMER-1.0.1/setup.py
```

### Comparing `GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/PKG-INFO` & `GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlyCONFORMER
-Version: 1.0.0
+Version: 1.0.1
 Summary: GlyCONFORMERS is a Python package that assigns conformer strings to N-glycan conformers, based on their torsion angle values.
 Home-page: https://github.com/IsabellGrothaus/GlyCONFORMER
 Author: Isabell Grothaus
 Author-email: grothaus@uni-bremen.de
 License: GPL-3.0 license
 Keywords: glycan,conformer,classification,sugar,carbohydrates
 Classifier: Development Status :: 3 - Alpha
@@ -22,17 +22,20 @@
 ![](https://github.com/IsabellGrothaus/GlyCONFORMER/blob/v1.0.0-alpha/TUTORIAL/Conformer_string.png?raw=true)
 
 Check the paper or tutorial for a detailed explanation of the GlyCONFORMER string generation. The workflow is not exclusivly designed for N-glycans, but can also be applyied to any other glycan type there is. 
 
 ## Installation
 
 To use GlyCONFORMER, first install it using pip:
-
-$ pip install GlyCONFORMER
-    
+```
+pip install GlyCONFORMER
+```
+Stable performance was only tested and verified with python version 3.8.
+Pandas<=1.3.5 is required!
+ 
 ## Tutorial
 
 The tutorial juypter notebook should be run from within the GlyCONFORMER package folder or you have to change the path directing to the TUTORIAL folder.
 
 The tutorial includes different N-glycan types and different complexity levels of how to obtain a GlyCONFORMER label string for custom glycan types and their recorded torsion angle values. The minimum example is given by the high-mannose type N-glycan M5, where only the file **M5_angles.dat** with torsion angle values is used as input:
 
 ![](https://github.com/IsabellGrothaus/GlyCONFORMER/blob/v1.0.0-alpha/TUTORIAL/Input.png?raw=true)
```

### Comparing `GlyCONFORMER-1.0.0/GlyCONFORMER.egg-info/SOURCES.txt` & `GlyCONFORMER-1.0.1/GlyCONFORMER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_omega3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_omega3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi3_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi3_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi7_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi7_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_phi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_phi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi3_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi3_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi7_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi7_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/fes_psi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/fes_psi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/info.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/info.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/maxima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/maxima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2/minima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2/minima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega10_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_omega10_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega3_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_omega3_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_omega6_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_omega6_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi10_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi10_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi3_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi3_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi6_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi6_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_phi9_10.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_phi9_10.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi10_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi10_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi3_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi3_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi6_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi6_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/fes_psi9_10.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/fes_psi9_10.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/info.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/info.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/maxima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/maxima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A2G2S2/minima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A2G2S2/minima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega11_15.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_omega11_15.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega1_18.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_omega1_18.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_omega3_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_omega3_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi11_12.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi11_12.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi11_15.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi11_15.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi12_13.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi12_13.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi13_14.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi13_14.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi15_16.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi15_16.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi16_17.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi16_17.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi1_18.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi1_18.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi3_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi3_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi4_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi4_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi6_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi6_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_phi9_10.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_phi9_10.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi11_12.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi11_12.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi11_15.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi11_15.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi12_13.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi12_13.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi13_14.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi13_14.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi15_16.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi15_16.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi16_17.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi16_17.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi1_18.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi1_18.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi3_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi3_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi4_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi4_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi6_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi6_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/fes_psi9_10.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/fes_psi9_10.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/info.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/info.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/maxima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/maxima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/minima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/minima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/A4G4S4/plumed_allangle.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/A4G4S4/plumed_allangle.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega1_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_omega1_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega3_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_omega3_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_omega5_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_omega5_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi1_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi1_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi3_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi3_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_phi5_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_phi5_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi1_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi1_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi3_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi3_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/fes_psi5_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/fes_psi5_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/info.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/info.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/maxima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/maxima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/minima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/minima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/FM5/plumed_allangle.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/FM5/plumed_allangle.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_omega3_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_omega3_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_omega5_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_omega5_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi3_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi3_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_phi5_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_phi5_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi3_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi3_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/fes_psi5_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/fes_psi5_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M5/minima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M5/minima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_omega3_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_omega3_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_omega7_10.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_omega7_10.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi10_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi10_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi3_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi3_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi7_10.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi7_10.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi7_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi7_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_phi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_phi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi10_11.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi10_11.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi1_2.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi1_2.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi2_3.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi2_3.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi3_4.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi3_4.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi3_7.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi3_7.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi4_5.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi4_5.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi5_6.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi5_6.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi7_10.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi7_10.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi7_8.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi7_8.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/fes_psi8_9.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/fes_psi8_9.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/info.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/info.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/maxima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/maxima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LIBRARY_GLYCANS/M9/minima.dat` & `GlyCONFORMER-1.0.1/LIBRARY_GLYCANS/M9/minima.dat`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/LICENSE` & `GlyCONFORMER-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/PKG-INFO` & `GlyCONFORMER-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlyCONFORMER
-Version: 1.0.0
+Version: 1.0.1
 Summary: GlyCONFORMERS is a Python package that assigns conformer strings to N-glycan conformers, based on their torsion angle values.
 Home-page: https://github.com/IsabellGrothaus/GlyCONFORMER
 Author: Isabell Grothaus
 Author-email: grothaus@uni-bremen.de
 License: GPL-3.0 license
 Keywords: glycan,conformer,classification,sugar,carbohydrates
 Classifier: Development Status :: 3 - Alpha
@@ -22,17 +22,20 @@
 ![](https://github.com/IsabellGrothaus/GlyCONFORMER/blob/v1.0.0-alpha/TUTORIAL/Conformer_string.png?raw=true)
 
 Check the paper or tutorial for a detailed explanation of the GlyCONFORMER string generation. The workflow is not exclusivly designed for N-glycans, but can also be applyied to any other glycan type there is. 
 
 ## Installation
 
 To use GlyCONFORMER, first install it using pip:
-
-$ pip install GlyCONFORMER
-    
+```
+pip install GlyCONFORMER
+```
+Stable performance was only tested and verified with python version 3.8.
+Pandas<=1.3.5 is required!
+ 
 ## Tutorial
 
 The tutorial juypter notebook should be run from within the GlyCONFORMER package folder or you have to change the path directing to the TUTORIAL folder.
 
 The tutorial includes different N-glycan types and different complexity levels of how to obtain a GlyCONFORMER label string for custom glycan types and their recorded torsion angle values. The minimum example is given by the high-mannose type N-glycan M5, where only the file **M5_angles.dat** with torsion angle values is used as input:
 
 ![](https://github.com/IsabellGrothaus/GlyCONFORMER/blob/v1.0.0-alpha/TUTORIAL/Input.png?raw=true)
```

### Comparing `GlyCONFORMER-1.0.0/README.md` & `GlyCONFORMER-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 ![](https://github.com/IsabellGrothaus/GlyCONFORMER/blob/v1.0.0-alpha/TUTORIAL/Conformer_string.png?raw=true)
 
 Check the paper or tutorial for a detailed explanation of the GlyCONFORMER string generation. The workflow is not exclusivly designed for N-glycans, but can also be applyied to any other glycan type there is. 
 
 ## Installation
 
 To use GlyCONFORMER, first install it using pip:
-
-$ pip install GlyCONFORMER
-    
+```
+pip install GlyCONFORMER
+```
+Stable performance was only tested and verified with python version 3.8.
+Pandas<=1.3.5 is required!
+ 
 ## Tutorial
 
 The tutorial juypter notebook should be run from within the GlyCONFORMER package folder or you have to change the path directing to the TUTORIAL folder.
 
 The tutorial includes different N-glycan types and different complexity levels of how to obtain a GlyCONFORMER label string for custom glycan types and their recorded torsion angle values. The minimum example is given by the high-mannose type N-glycan M5, where only the file **M5_angles.dat** with torsion angle values is used as input:
 
 ![](https://github.com/IsabellGrothaus/GlyCONFORMER/blob/v1.0.0-alpha/TUTORIAL/Input.png?raw=true)
```

### Comparing `GlyCONFORMER-1.0.0/glyconformer/lib.py` & `GlyCONFORMER-1.0.1/glyconformer/lib.py`

 * *Files identical despite different names*

### Comparing `GlyCONFORMER-1.0.0/setup.py` & `GlyCONFORMER-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Education',
     'Programming Language :: Python :: 3'
     ]
 
 setup(name='GlyCONFORMER',
-      version='1.0.0',
+      version='1.0.1',
       description="GlyCONFORMERS is a Python package that assigns conformer strings to N-glycan conformers, based on their torsion angle values.",
       url="https://github.com/IsabellGrothaus/GlyCONFORMER",
       long_description = (here / "README.md").read_text(),
       long_description_content_type='text/markdown',
       author='Isabell Grothaus',
       author_email='grothaus@uni-bremen.de',
       classifiers=classifiers,
       keywords="glycan, conformer, classification, sugar, carbohydrates",
       license='GPL-3.0 license',
       packages=find_packages(),
       package_data={'':['**/*.dat']},
       install_requires=[
-                       "numpy","matplotlib","pandas","plumed","scipy"
+                       "numpy","matplotlib","pandas<=1.3.5","plumed","scipy"
                        ],
       )
```

