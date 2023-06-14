# Comparing `tmp/pyfem-0.0.9.tar.gz` & `tmp/pyfem-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.0.9.tar", last modified: Sun Jun  4 04:40:09 2023, max compression
+gzip compressed data, was "pyfem-0.1.0.tar", last modified: Wed Jun 14 08:38:07 2023, max compression
```

## Comparing `pyfem-0.0.9.tar` & `pyfem-0.1.0.tar`

### file list

```diff
@@ -1,76 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.251949 pyfem-0.0.9/
--rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      793 2023-06-04 04:40:09.251453 pyfem-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-19 11:01:17.000000 pyfem-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 04:40:09.251949 pyfem-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-06-04 04:29:16.000000 pyfem-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.133768 pyfem-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.149144 pyfem-0.0.9/src/pyfem/
--rw-rw-rw-   0        0        0     1025 2023-06-02 16:36:54.000000 pyfem-0.0.9/src/pyfem/Job.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      277 2023-05-22 12:37:32.000000 pyfem-0.0.9/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.164026 pyfem-0.0.9/src/pyfem/assembly/
--rw-rw-rw-   0        0        0     8811 2023-06-01 15:32:06.000000 pyfem-0.0.9/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.171072 pyfem-0.0.9/src/pyfem/bc/
--rw-rw-rw-   0        0        0      781 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2268 2023-05-30 15:48:17.000000 pyfem-0.0.9/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0      876 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.186204 pyfem-0.0.9/src/pyfem/elements/
--rw-rw-rw-   0        0        0     5142 2023-06-02 16:35:55.000000 pyfem-0.0.9/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0     2315 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/elements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    30821 2023-06-02 17:14:27.000000 pyfem-0.0.9/src/pyfem/elements/IsoElementShape.py
--rw-rw-rw-   0        0        0     6426 2023-06-02 16:09:39.000000 pyfem-0.0.9/src/pyfem/elements/SolidPlaneSmallStrain.py
--rw-rw-rw-   0        0        0     7214 2023-06-02 14:12:56.000000 pyfem-0.0.9/src/pyfem/elements/SolidVolumeSmallStrain.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-05-31 12:01:59.000000 pyfem-0.0.9/src/pyfem/elements/get_element_data.py
--rw-rw-rw-   0        0        0     1792 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/elements/get_iso_element_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.191660 pyfem-0.0.9/src/pyfem/fem/
--rw-rw-rw-   0        0        0      897 2023-06-01 12:24:10.000000 pyfem-0.0.9/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0       70 2023-06-01 14:47:42.000000 pyfem-0.0.9/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.212466 pyfem-0.0.9/src/pyfem/io/
--rw-rw-rw-   0        0        0      679 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0      577 2023-05-18 14:20:30.000000 pyfem-0.0.9/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     2411 2023-06-01 12:24:10.000000 pyfem-0.0.9/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      520 2023-05-18 14:20:30.000000 pyfem-0.0.9/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0      575 2023-05-20 17:12:32.000000 pyfem-0.0.9/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0    11352 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0      815 2023-05-18 14:20:30.000000 pyfem-0.0.9/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0      821 2023-06-01 12:26:16.000000 pyfem-0.0.9/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.9/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-06-04 04:30:48.000000 pyfem-0.0.9/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     4271 2023-06-01 12:24:10.000000 pyfem-0.0.9/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.225461 pyfem-0.0.9/src/pyfem/materials/
--rw-rw-rw-   0        0        0     1245 2023-05-31 12:01:59.000000 pyfem-0.0.9/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     6857 2023-06-01 12:36:14.000000 pyfem-0.0.9/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     1342 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/materials/PlasticIsotropicHardening.py
--rw-rw-rw-   0        0        0     5218 2023-06-04 04:38:44.000000 pyfem-0.0.9/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0     1309 2023-05-23 13:12:51.000000 pyfem-0.0.9/src/pyfem/materials/get_material_data.py
--rw-rw-rw-   0        0        0     5330 2023-06-01 15:48:19.000000 pyfem-0.0.9/src/pyfem/materials/run.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.230968 pyfem-0.0.9/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     4765 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/mesh/ElementSet.py
--rw-rw-rw-   0        0        0     4994 2023-06-01 12:32:50.000000 pyfem-0.0.9/src/pyfem/mesh/NodeSet.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.239549 pyfem-0.0.9/src/pyfem/solvers/
--rw-rw-rw-   0        0        0      738 2023-05-31 13:50:18.000000 pyfem-0.0.9/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     1450 2023-06-01 14:20:50.000000 pyfem-0.0.9/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0     7445 2023-06-02 15:54:17.000000 pyfem-0.0.9/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0      954 2023-05-23 12:42:03.000000 pyfem-0.0.9/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.249965 pyfem-0.0.9/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2350 2023-06-01 12:30:53.000000 pyfem-0.0.9/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      795 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     1518 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     1820 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1046 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.160690 pyfem-0.0.9/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      793 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1799 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.848612 pyfem-0.1.0/
+-rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      793 2023-06-14 08:38:07.848612 pyfem-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-19 03:01:04.000000 pyfem-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:38:07.849604 pyfem-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-06-14 08:37:45.000000 pyfem-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.766603 pyfem-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.776603 pyfem-0.1.0/src/pyfem/
+-rw-rw-rw-   0        0        0     1025 2023-06-13 08:12:20.000000 pyfem-0.1.0/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.0/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.787603 pyfem-0.1.0/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0      924 2023-06-09 08:03:09.000000 pyfem-0.1.0/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1357 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0      818 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.790604 pyfem-0.1.0/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    10102 2023-06-13 04:25:07.000000 pyfem-0.1.0/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.795614 pyfem-0.1.0/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     1564 2023-06-09 04:33:36.000000 pyfem-0.1.0/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2406 2023-06-09 08:02:29.000000 pyfem-0.1.0/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     3706 2023-06-09 08:02:51.000000 pyfem-0.1.0/src/pyfem/bc/NeumannBC.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1321 2023-06-09 04:19:15.000000 pyfem-0.1.0/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.805603 pyfem-0.1.0/src/pyfem/elements/
+-rw-rw-rw-   0        0        0     8145 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0     2315 2023-05-30 06:11:08.000000 pyfem-0.1.0/src/pyfem/elements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    30821 2023-06-05 12:47:22.000000 pyfem-0.1.0/src/pyfem/elements/IsoElementShape.py
+-rw-rw-rw-   0        0        0     9385 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/elements/SolidPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0    10151 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/elements/SolidVolumeSmallStrain.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-06-13 04:20:37.000000 pyfem-0.1.0/src/pyfem/elements/get_element_data.py
+-rw-rw-rw-   0        0        0     1842 2023-06-08 06:40:10.000000 pyfem-0.1.0/src/pyfem/elements/get_iso_element_type.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.808612 pyfem-0.1.0/src/pyfem/fem/
+-rw-rw-rw-   0        0        0      897 2023-06-01 03:56:06.000000 pyfem-0.1.0/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.822602 pyfem-0.1.0/src/pyfem/io/
+-rw-rw-rw-   0        0        0      592 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0      888 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0      614 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2438 2023-06-13 08:27:34.000000 pyfem-0.1.0/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      538 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0      612 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0    10307 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0      852 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0      821 2023-06-01 09:39:23.000000 pyfem-0.1.0/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1741 2023-06-14 08:37:45.000000 pyfem-0.1.0/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     4332 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.830611 pyfem-0.1.0/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     1233 2023-06-13 04:20:37.000000 pyfem-0.1.0/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     6885 2023-06-13 04:20:37.000000 pyfem-0.1.0/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     1303 2023-05-30 09:04:06.000000 pyfem-0.1.0/src/pyfem/materials/PlasticIsotropicHardening.py
+-rw-rw-rw-   0        0        0     6730 2023-06-13 08:14:44.000000 pyfem-0.1.0/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     5594 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-14 05:02:11.000000 pyfem-0.1.0/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.834603 pyfem-0.1.0/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     4977 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/mesh/ElementSet.py
+-rw-rw-rw-   0        0        0     6572 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0     5036 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/mesh/NodeSet.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.839614 pyfem-0.1.0/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0      700 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     1382 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0     7700 2023-06-14 07:58:16.000000 pyfem-0.1.0/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.847602 pyfem-0.1.0/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2350 2023-06-02 03:00:28.000000 pyfem-0.1.0/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.0/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.0/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     2352 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.0/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.783604 pyfem-0.1.0/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0      793 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2045 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.0.9/LICENSE` & `pyfem-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `pyfem-0.0.9/PKG-INFO` & `pyfem-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.9
+Version: 0.1.0
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.0.9/setup.py` & `pyfem-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.0.9",
+    version="0.1.0",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.0.9/src/pyfem/Job.py` & `pyfem-0.1.0/src/pyfem/Job.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem/assembly/Assembly.py` & `pyfem-0.1.0/src/pyfem/assembly/Assembly.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.elements.get_element_data import get_element_data
 from pyfem.elements.get_iso_element_type import get_iso_element_type
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Properties import Properties
 from pyfem.materials.get_material_data import get_material_data
+from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_dict_to_string_assembly
 from pyfem.utils.wrappers import show_running_time
 
 iso_element_shape_dict = {
     'line2': IsoElementShape('line2'),
     'line3': IsoElementShape('line3'),
     'tria3': IsoElementShape('tria3'),
@@ -36,14 +37,15 @@
 class Assembly:
     def __init__(self, props: Properties) -> None:
         self.total_dof_number: int = -1
         self.props: Properties = props
         self.timer: Timer = Timer()
         self.materials_dict: Dict = {}
         self.sections_dict: Dict = {}
+        self.amplitudes_dict: Dict = {}
         self.section_of_element_set: Dict = {}
         self.element_data_list: List[BaseElement] = []
         self.bc_data_list: List[BaseBC] = []
         self.global_stiffness: csc_matrix = csc_matrix(0)
         self.fext: ndarray = empty(0, dtype=DTYPE)
         self.fint: ndarray = empty(0, dtype=DTYPE)
         self.dof_solution: ndarray = empty(0, dtype=DTYPE)
@@ -59,142 +61,170 @@
 
     def show(self) -> None:
         print(self.to_string())
 
     @show_running_time
     def init(self) -> None:
         # 初始化 self.element_data_list
-        elements = self.props.elements
-        nodes = self.props.nodes
+        mesh_data = self.props.mesh_data
+        elements = mesh_data.elements
+        nodes = mesh_data.nodes
+        element_sets = mesh_data.element_sets
         sections = self.props.sections
         materials = self.props.materials
+        solver = self.props.solver
+        amplitudes = self.props.amplitudes
         dof = self.props.dof
         timer = self.timer
-        dimension = nodes.dimension
+        dimension = self.props.mesh_data.dimension
         self.total_dof_number = len(nodes) * len(dof.names)
 
         for material in materials:
             self.materials_dict[material.name] = material
 
         for section in sections:
             self.sections_dict[section.name] = section
 
-        for element_set in elements.element_sets:
+        for amplitude in amplitudes:
+            self.amplitudes_dict[amplitude.name] = amplitude
+
+        for element_set in element_sets:
             for section in sections:
                 if element_set in section.element_sets:
                     self.section_of_element_set[element_set] = section
 
-        for element_set_name, element_ids in elements.element_sets.items():
-            section = self.section_of_element_set[element_set_name]
-            material = self.materials_dict[section.material_name]
-            material_data = get_material_data(material=material,
-                                              dimension=dimension,
-                                              option=section.type)
-
-            for element_id in element_ids:
-                connectivity = elements[element_id]
-                node_coords = array(nodes.get_items_by_ids(list(connectivity)), dtype=DTYPE)
-                iso_element_type = get_iso_element_type(node_coords)
-                iso_element_shape = iso_element_shape_dict[iso_element_type]
-                element_data = get_element_data(element_id=element_id,
-                                                iso_element_shape=iso_element_shape,
-                                                connectivity=connectivity,
-                                                node_coords=node_coords,
-                                                section=section,
-                                                dof=dof,
-                                                material=material,
-                                                material_data=material_data,
-                                                timer=timer)
-
-                element_data.assembly_conn = array(nodes.get_indices_by_ids(list(connectivity)))
-                element_data.create_element_dof_ids()
-
-                self.element_data_list.append(element_data)
+        for element_set_name, element_ids in element_sets.items():
+            if element_set_name in self.section_of_element_set.keys():
+                section = self.section_of_element_set[element_set_name]
+                material = self.materials_dict[section.material_name]
+                material_data = get_material_data(material=material,
+                                                  dimension=dimension,
+                                                  option=section.type)
+
+                for element_id in element_ids:
+                    connectivity = elements[element_id]
+                    node_coords = nodes[connectivity]
+                    iso_element_type = get_iso_element_type(node_coords)
+                    iso_element_shape = iso_element_shape_dict[iso_element_type]
+                    element_data = get_element_data(element_id=element_id,
+                                                    iso_element_shape=iso_element_shape,
+                                                    connectivity=connectivity,
+                                                    node_coords=node_coords,
+                                                    dof=dof,
+                                                    material=material,
+                                                    section=section,
+                                                    material_data=material_data,
+                                                    timer=timer)
+
+                    element_data.assembly_conn = connectivity
+                    element_data.create_element_dof_ids()
+
+                    self.element_data_list.append(element_data)
+
+        if len(self.element_data_list) < len(self.props.mesh_data.elements):
+            raise NotImplementedError(error_style(f'some elements do not have defined section properties'))
+        elif len(self.element_data_list) > len(self.props.mesh_data.elements):
+            raise NotImplementedError(
+                error_style(f'some elements have section properties that are redundantly defined'))
 
         # 初始化 self.bc_data_list
         bcs = self.props.bcs
         for bc in bcs:
-            bc_data = get_bc_data(bc=bc, dof=dof, nodes=nodes)
+            if bc.amplitude_name is not None:
+                amplitude = self.amplitudes_dict[bc.amplitude_name]
+            else:
+                amplitude = None
+            bc_data = get_bc_data(bc=bc,
+                                  dof=dof,
+                                  mesh_data=mesh_data,
+                                  solver=solver,
+                                  amplitude=amplitude)
             self.bc_data_list.append(bc_data)
 
         bc_dof_ids = []
         for bc_data in self.bc_data_list:
             for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
                 bc_dof_ids.append(dof_id)
         self.bc_dof_ids = array(bc_dof_ids)
 
         # 初始化 rhs, fext, fint, dof_solution, ddof_solution
         self.fext = zeros(self.total_dof_number, dtype=DTYPE)
         self.fint = zeros(self.total_dof_number, dtype=DTYPE)
         self.dof_solution = zeros(self.total_dof_number, dtype=DTYPE)
         self.ddof_solution = zeros(self.total_dof_number, dtype=DTYPE)
 
+    # @show_running_time
     def assembly_global_stiffness(self) -> None:
         val = []
         row = []
         col = []
 
         for element_data in self.element_data_list:
             element_dof_ids = element_data.element_dof_ids
             element_dof_number = element_data.element_dof_number
             row += [r for r in repeat(element_dof_ids, element_dof_number)]
             for _ in range(element_dof_number):
                 col += [c for c in element_dof_ids]
             val += [v for v in element_data.element_stiffness.reshape(element_dof_number * element_dof_number)]
 
-        self.global_stiffness = coo_matrix((array(val, dtype=DTYPE), (array(row, dtype=DTYPE), array(col, dtype=DTYPE))),
-                                           shape=(self.total_dof_number, self.total_dof_number)).tocsc()
+        self.global_stiffness = coo_matrix(
+            (array(val, dtype=DTYPE), (array(row, dtype=DTYPE), array(col, dtype=DTYPE))),
+            shape=(self.total_dof_number, self.total_dof_number)).tocsc()
 
+    # @show_running_time
     def assembly_fint(self) -> None:
         self.fint = zeros(self.total_dof_number, dtype=DTYPE)
         for element_data in self.element_data_list:
             self.fint[element_data.element_dof_ids] += element_data.element_fint
 
+    # @show_running_time
     def update_element_data(self) -> None:
         dof_solution = self.dof_solution
         ddof_solution = self.ddof_solution
         for element_data in self.element_data_list:
             element_data.update_element_dof_values(dof_solution)
             element_data.update_element_ddof_values(ddof_solution)
-            element_data.update_material_state()
-            element_data.update_element_stiffness()
-            element_data.update_element_fint()
+            element_data.update_element_material_stiffness_fint()
 
+    # @show_running_time
     def update_element_stiffness(self) -> None:
         for element_data in self.element_data_list:
             element_data.update_element_stiffness()
 
+    # @show_running_time
     def update_element_data_without_stiffness(self) -> None:
         dof_solution = self.dof_solution
         ddof_solution = self.ddof_solution
         for element_data in self.element_data_list:
             element_data.update_element_dof_values(dof_solution)
             element_data.update_element_ddof_values(ddof_solution)
             element_data.update_material_state()
             element_data.update_element_fint()
 
+    # @show_running_time
     def update_element_state_variables(self) -> None:
         for element_data in self.element_data_list:
             element_data.update_element_state_variables()
 
+    # @show_running_time
     def update_element_field_variables(self) -> None:
         for element_data in self.element_data_list:
             element_data.update_element_field_variables()
 
     def assembly_field_variables(self) -> None:
-        nodes_number = len(self.props.nodes)
+        nodes_number = len(self.props.mesh_data.nodes)
 
         for output in self.props.outputs:
             if output.type == 'vtk':
                 for field_name in output.field_outputs:
                     self.field_variables[field_name] = zeros(nodes_number)
                     nodes_count = zeros(nodes_number)
                     for element_data in self.element_data_list:
                         assembly_conn = element_data.assembly_conn
                         self.field_variables[field_name][assembly_conn] += \
-                            element_data.average_field_variables[field_name]
+                            element_data.element_average_field_variables[field_name]
                         nodes_count[assembly_conn] += 1.0
                     self.field_variables[field_name] = self.field_variables[field_name] / nodes_count
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `pyfem-0.0.9/src/pyfem/bc/BaseBC.py` & `pyfem-0.1.0/src/pyfem/io/Solver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from numpy import (empty, ndarray)
+# -*- coding: utf-8 -*-
+"""
 
-from pyfem.io.BC import BC
-from pyfem.io.Dof import Dof
-from pyfem.mesh.NodeSet import NodeSet
-from pyfem.utils.visualization import object_dict_to_string_ndarray
-
-
-class BaseBC:
-    def __init__(self, bc: BC, dof: Dof, nodes: NodeSet) -> None:
-        self.bc: BC = bc
-        self.dof: Dof = dof
-        self.nodes: NodeSet = nodes
-        self.bc_node_ids: ndarray = empty(0)
-        self.bc_element_ids: ndarray = empty(0)
-        self.dof_ids: ndarray = empty(0)
-        self.dof_values: ndarray = empty(0)
+"""
+from pyfem.utils.visualization import object_dict_to_string
+
+
+class Solver:
+    def __init__(self) -> None:
+        self.type: str = None  # type: ignore
+        self.option: str = None  # type: ignore
+        self.total_time: float = 1.0
+        self.start_time: float = 0.0
+        self.max_increment: int = 100
+        self.initial_dtime: float = 1.0
+        self.max_dtime: float = 1.0
+        self.min_dtime: float = 0.001
+        self.dtype: str = 'float64'
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
+        return object_dict_to_string(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
 
 if __name__ == "__main__":
-    pass
+    solver = Solver()
+    print(solver.__dict__.keys())
+    print(solver)
+    print(solver.to_string())
```

### Comparing `pyfem-0.0.9/src/pyfem/bc/DirichletBC.py` & `pyfem-0.1.0/src/pyfem/bc/DirichletBC.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,55 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
+from typing import Optional
+
 from numpy import array
 
 from pyfem.bc.BaseBC import BaseBC
+from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
-from pyfem.mesh.NodeSet import NodeSet
+from pyfem.io.Solver import Solver
+from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_dict_to_string_ndarray
 
 
 class DirichletBC(BaseBC):
-    def __init__(self, bc: BC, dof: Dof, nodes: NodeSet) -> None:
-        super().__init__(bc, dof, nodes)
-        self.bc: BC = bc
-        self.dof: Dof = dof
-        self.nodes: NodeSet = nodes
+    def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
+        super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def create_dof_values(self) -> None:
         bc_node_sets = self.bc.node_sets
         bc_node_ids = []
         for bc_node_set in bc_node_sets:
-            bc_node_ids += list(self.nodes.node_sets[bc_node_set])
+            bc_node_ids += list(self.mesh_data.node_sets[bc_node_set])
 
         # 如果发现施加当前边界条件的点集中有重复的点则抛出异常
         if len(bc_node_ids) != len(set(bc_node_ids)):
             error_msg = f'{type(self).__name__} {self.bc.name} contains repeat nodes\n'
             error_msg += f'Please check the input file'
             raise NotImplementedError(error_style(error_msg))
         else:
             self.bc_node_ids = array(bc_node_ids)
 
         # 确定施加的边界条件对应的全局自由度编号
         bc_dof_names = self.bc.dof
         dof_names = self.dof.names
         dof_ids = []
-        for node_index in self.nodes.get_indices_by_ids(list(self.bc_node_ids)):
+        for node_index in self.bc_node_ids:
             for _, bc_dof_name in enumerate(bc_dof_names):
                 dof_ids.append(node_index * len(dof_names) + dof_names.index(bc_dof_name))
         self.dof_ids = array(dof_ids)
 
         bc_value = self.bc.value
         if isinstance(bc_value, float):
             self.dof_values = array([bc_value for _ in self.dof_ids])
@@ -53,10 +58,10 @@
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
     props.verify()
 
-    bc_data = DirichletBC(props.bcs[1], props.dof, props.nodes)
+    bc_data = DirichletBC(props.bcs[1], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
     bc_data.create_dof_values()
     bc_data.show()
```

### Comparing `pyfem-0.0.9/src/pyfem/bc/get_bc_data.py` & `pyfem-0.1.0/src/pyfem/bc/get_bc_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,42 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
+from typing import Optional
+
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.bc.DirichletBC import DirichletBC
+from pyfem.bc.NeumannBC import NeumannBC
+from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
-from pyfem.mesh.NodeSet import NodeSet
+from pyfem.io.Solver import Solver
+from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 
 bc_data_dict = {
-    'DirichletBC': DirichletBC
+    'DirichletBC': DirichletBC,
+    'NeumannBC': NeumannBC
 }
 
 
 def get_bc_data(bc: BC,
                 dof: Dof,
-                nodes: NodeSet) -> BaseBC:
-    class_name = f'{bc.type}'.strip().replace(' ', '')
+                mesh_data: MeshData,
+                solver: Solver,
+                amplitude: Optional[Amplitude]) -> BaseBC:
+    class_name = f'{bc.category}{bc.type}'.strip().replace(' ', '')
 
     if class_name in bc_data_dict:
         return bc_data_dict[class_name](bc=bc,
                                         dof=dof,
-                                        nodes=nodes)
+                                        mesh_data=mesh_data,
+                                        solver=solver,
+                                        amplitude=amplitude)
     else:
         error_msg = f'{class_name} bc is not supported.\n'
         error_msg += f'The allowed bc types are {list(bc_data_dict.keys())}.'
         raise NotImplementedError(error_style(error_msg))
 
 
 if __name__ == "__main__":
```

### Comparing `pyfem-0.0.9/src/pyfem/elements/BaseElement.py` & `pyfem-0.1.0/src/pyfem/elements/BaseElement.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,101 @@
 # -*- coding: utf-8 -*-
 """
 
 """
+from copy import deepcopy
 from typing import List, Dict
 
-from numpy import (dot, empty, array, ndarray)
-from numpy.linalg import (det, inv)
+from numpy import dot, array, ndarray
+from numpy.linalg import det, inv
 
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
-from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
-from pyfem.utils.visualization import object_dict_to_string_ndarray
-from pyfem.utils.wrappers import show_running_time
+from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class BaseElement:
+    __slots__ = ('element_id', 'iso_element_shape', 'connectivity', 'node_coords', 'assembly_conn', 'dof', 'material',
+                 'section', 'material_data', 'timer', 'dof_names', 'gp_number', 'gp_jacobis', 'gp_jacobi_invs',
+                 'gp_jacobi_dets', 'gp_weight_times_jacobi_dets', 'gp_ddsddes', 'gp_state_variables',
+                 'gp_state_variables_new', 'gp_field_variables', 'element_dof_number', 'element_dof_ids',
+                 'element_dof_values', 'element_ddof_values', 'element_fint', 'element_stiffness',
+                 'element_average_field_variables')
+
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray) -> None:
         self.element_id: int = element_id  # 用户自定义的节点编号
         self.iso_element_shape: IsoElementShape = iso_element_shape
         self.connectivity: ndarray = connectivity  # 对应用户定义的节点编号
-        self.assembly_conn: ndarray = empty(0)  # 对应系统组装时的节点序号
         self.node_coords: ndarray = node_coords
-        self.gp_jacobis: ndarray = empty(0, dtype=DTYPE)
-        self.gp_jacobi_invs: ndarray = empty(0, dtype=DTYPE)
-        self.gp_jacobi_dets: ndarray = empty(0, dtype=DTYPE)
-        self.gp_weight_times_jacobi_dets: ndarray = empty(0, dtype=DTYPE)
+        self.assembly_conn: ndarray = None  # type: ignore  # 对应系统组装时的节点序号
+
         self.dof: Dof = None  # type: ignore
-        self.dof_names: List[str] = []
-        self.element_dof_number: int = 0  # 单元自由度总数
-        self.element_dof_ids: List[int] = []  # 对应系统组装时的自由度序号
-        self.element_dof_values: ndarray = empty(0, dtype=DTYPE)  # 对应系统组装时的自由度的值
-        self.element_ddof_values: ndarray = empty(0, dtype=DTYPE)  # 对应系统组装时的自由度增量的值
-        self.element_fint: ndarray = empty(0, dtype=DTYPE)  # 对应系统组装时的内力值
         self.material: Material = None  # type: ignore
         self.section: Section = None  # type: ignore
         self.material_data: BaseMaterial = None  # type: ignore
         self.timer: Timer = None  # type: ignore
-        self.element_stiffness: ndarray = empty(0, dtype=DTYPE)
-        self.gp_ddsddes: ndarray = empty(0, dtype=DTYPE)
-        self.gp_state_variables: List[Dict[str, ndarray]] = [{} for _ in range(self.iso_element_shape.gp_number)]
-        self.gp_state_variables_new: List[Dict[str, ndarray]] = [{} for _ in range(self.iso_element_shape.gp_number)]
+
+        self.dof_names: List[str] = []
+
+        self.gp_number: int = self.iso_element_shape.gp_number
+        self.gp_jacobis: ndarray = None  # type: ignore
+        self.gp_jacobi_invs: ndarray = None  # type: ignore
+        self.gp_jacobi_dets: ndarray = None  # type: ignore
+        self.gp_weight_times_jacobi_dets: ndarray = None  # type: ignore
+        self.gp_ddsddes: List[ndarray] = []
+        self.gp_state_variables: List[Dict[str, ndarray]] = [{} for _ in range(self.gp_number)]
+        self.gp_state_variables_new: List[Dict[str, ndarray]] = [{} for _ in range(self.gp_number)]
         self.gp_field_variables: Dict[str, ndarray] = {}
-        self.average_field_variables: Dict[str, ndarray] = {}
         self.cal_jacobi()
 
+        self.element_dof_number: int = 0  # 单元自由度总数
+        self.element_dof_ids: List[int] = []  # 对应系统组装时的自由度序号
+        self.element_dof_values: ndarray = None  # type: ignore  # 对应系统组装时的自由度的值
+        self.element_ddof_values: ndarray = None  # type: ignore  # 对应系统组装时的自由度增量的值
+        self.element_fint: ndarray = None  # type: ignore  # 对应系统组装时的内力值
+        self.element_stiffness: ndarray = None  # type: ignore
+        self.element_average_field_variables: Dict[str, ndarray] = {}
+
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
+        return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def cal_jacobi(self) -> None:
         """
         通过矩阵乘法计算每个积分点上的Jacobi矩阵。
         """
 
         # 以下代码为采用for循环的计算方法，结构清晰，但计算效率较低
-        # self.jacobi = []
-        # self.jacobi_inv = []
-        # self.jacobi_det = []
+        # self.gp_jacobis = []
+        # self.gp_jacobi_invs = []
+        # self.gp_jacobi_dets = []
         # for gp_shape_gradient in self.iso_element_shape.gp_shape_gradients:
         #     jacobi = dot(self.node_coords.transpose(), gp_shape_gradient)
-        #     self.jacobi.append(jacobi)
-        #     self.jacobi_inv.append(inv(jacobi))
-        #     self.jacobi_det.append(det(jacobi))
-        # self.jacobi = array(self.jacobi)
-        # self.jacobi_inv = array(self.jacobi_inv)
-        # self.jacobi_det = array(self.jacobi_det)
+        #     self.gp_jacobis.append(jacobi)
+        #     self.gp_jacobi_invs.append(inv(jacobi))
+        #     self.gp_jacobi_dets.append(det(jacobi))
+        # self.gp_jacobis = array(self.gp_jacobis)
+        # self.gp_jacobi_invs = array(self.gp_jacobi_invs)
+        # self.gp_jacobi_dets = array(self.gp_jacobi_dets)
 
         # 以下代码为采用numpy高维矩阵乘法的计算方法，计算效率高，但要注意矩阵维度的变化
         self.gp_jacobis = dot(self.node_coords.transpose(), self.iso_element_shape.gp_shape_gradients).swapaxes(0, 1)
-        self.gp_jacobi_invs = inv(self.gp_jacobis)
         self.gp_jacobi_dets = det(self.gp_jacobis)
+        # gp_jacobi通常为2×2或3×3的方阵，可以直接根据解析式求逆矩阵，计算效率比numpy.linalg.inv()函数更高
+        # self.gp_jacobi_invs = inv(self.gp_jacobis)
+        self.gp_jacobi_invs = inverse(self.gp_jacobis, self.gp_jacobi_dets)
         self.gp_weight_times_jacobi_dets = self.iso_element_shape.gp_weights * self.gp_jacobi_dets
 
     def create_element_dof_ids(self) -> None:
         for node_index in self.assembly_conn:
             for dof_id, _ in enumerate(self.dof_names):
                 self.element_dof_ids.append(node_index * len(self.dof_names) + dof_id)
 
@@ -91,27 +104,75 @@
 
     def update_element_dof_values(self, global_dof_values: ndarray) -> None:
         self.element_dof_values = global_dof_values[self.element_dof_ids]
 
     def update_element_ddof_values(self, global_ddof_values: ndarray) -> None:
         self.element_ddof_values = global_ddof_values[self.element_dof_ids]
 
+    def update_element_state_variables(self) -> None:
+        self.gp_state_variables = deepcopy(self.gp_state_variables_new)
+
+    def update_element_material_stiffness_fint(self) -> None:
+        pass
+
     def update_material_state(self) -> None:
         pass
 
     def update_element_stiffness(self) -> None:
         pass
 
     def update_element_fint(self) -> None:
         pass
 
-    def update_element_state_variables(self) -> None:
-        pass
-
     def update_element_field_variables(self) -> None:
         pass
 
 
+def inverse(gp_jacobis: ndarray, gp_jacobi_dets: ndarray) -> ndarray:
+    """
+    对于2×2的矩阵::
+
+        | a11  a12 |
+    A = |          |
+        | a21  a22 |
+
+    A^-1 = (1 / det(A)) * | a22  -a12 |
+                          |           |
+                          |-a21   a11 |
+
+    对于3×3的矩阵::
+        | a11  a12  a13 |
+    A = |               |
+        | a21  a22  a23 |
+        |               |
+        | a31  a32  a33 |
+
+    A^-1 = (1 / det(A)) * |  A22*A33 - A23*A32   A13*A32 - A12*A33   A12*A23 - A13*A22 |
+                          |                                                            |
+                          |  A23*A31 - A21*A33   A11*A33 - A13*A31   A13*A21 - A11*A23 |
+                          |                                                            |
+                          |  A21*A32 - A22*A31   A12*A31 - A11*A32   A11*A22 - A12*A21 |
+    """
+    gp_jacobi_invs = []
+    for A, det_A in zip(gp_jacobis, gp_jacobi_dets):
+        if A.shape == (2, 2):
+            gp_jacobi_invs.append(
+                array([[A[1][1], -A[0][1]], [-A[1][0], A[0][0]]]) / det_A)
+        elif A.shape == (3, 3):
+            gp_jacobi_invs.append(array([[(A[1][1] * A[2][2] - A[1][2] * A[2][1]),
+                                          (A[0][2] * A[2][1] - A[0][1] * A[2][2]),
+                                          (A[0][1] * A[1][2] - A[0][2] * A[1][1])],
+                                         [(A[1][2] * A[2][0] - A[1][0] * A[2][2]),
+                                          (A[0][0] * A[2][2] - A[0][2] * A[2][0]),
+                                          (A[0][2] * A[1][0] - A[0][0] * A[1][2])],
+                                         [(A[1][0] * A[2][1] - A[1][1] * A[2][0]),
+                                          (A[0][1] * A[2][0] - A[0][0] * A[2][1]),
+                                          (A[0][0] * A[1][1] - A[0][1] * A[1][0])]]) / det_A)
+        else:
+            return inv(gp_jacobis)
+    return array(gp_jacobi_invs)
+
+
 if __name__ == "__main__":
     pass
     # a = array([[0,0],[0.125,0.125]])
     # inv(a)
```

### Comparing `pyfem-0.0.9/src/pyfem/elements/IsoElementDiagram.py` & `pyfem-0.1.0/src/pyfem/elements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem/elements/IsoElementShape.py` & `pyfem-0.1.0/src/pyfem/elements/IsoElementShape.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem/elements/get_element_data.py` & `pyfem-0.1.0/src/pyfem/elements/get_element_data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 
 
 # @trace_calls
 def get_element_data(element_id: int,
                      iso_element_shape: IsoElementShape,
                      connectivity: ndarray,
                      node_coords: ndarray,
-                     section: Section,
                      dof: Dof,
                      material: Material,
+                     section: Section,
                      material_data: BaseMaterial,
                      timer: Timer) -> BaseElement:
     class_name = f'{section.category}{section.type}{section.option}'.strip().replace(' ', '')
 
     if class_name in element_data_dict:
         return element_data_dict[class_name](element_id=element_id,
                                              iso_element_shape=iso_element_shape,
                                              connectivity=connectivity,
                                              node_coords=node_coords,
-                                             section=section,
                                              dof=dof,
                                              material=material,
+                                             section=section,
                                              material_data=material_data,
                                              timer=timer)
     else:
         error_msg = f'{class_name} element is not supported.\n'
         error_msg += f'The allowed element types are {list(element_data_dict.keys())}.'
         raise NotImplementedError(error_style(error_msg))
```

### Comparing `pyfem-0.0.9/src/pyfem/elements/get_iso_element_type.py` & `pyfem-0.1.0/src/pyfem/elements/get_iso_element_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from numpy import ndarray
 
 from pyfem.utils.colors import error_style
 
 
-def get_iso_element_type(node_coords: ndarray) -> str:
+def get_iso_element_type(node_coords: ndarray, dimension: int = -1) -> str:
     element_node_number = node_coords.shape[0]
-    dimension = node_coords.shape[1]
+    if dimension == -1:
+        dimension = node_coords.shape[1]
 
     if dimension == 1:
         if element_node_number == 2:
             return 'line2'
         elif element_node_number == 3:
             return 'line3'
         else:
```

### Comparing `pyfem-0.0.9/src/pyfem/fem/Timer.py` & `pyfem-0.1.0/src/pyfem/fem/Timer.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem/io/BC.py` & `pyfem-0.1.0/src/pyfem/io/BC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from typing import List
 
 from pyfem.utils.visualization import object_dict_to_string
 
 
 class BC:
     def __init__(self) -> None:
         self.name: str = None  # type: ignore
+        self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.dof: List[str] = None  # type: ignore
         self.node_sets: List[str] = None  # type: ignore
         self.element_sets: List[str] = None  # type: ignore
+        self.bc_element_sets: List[str] = None  # type: ignore
         self.value: float = None  # type: ignore
+        self.amplitude_name: str = None  # type: ignore
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string(self, level)
 
     def show(self) -> None:
         print(self.to_string())
```

### Comparing `pyfem-0.0.9/src/pyfem/io/Material.py` & `pyfem-0.1.0/src/pyfem/io/Material.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     当 self.is_read_only = True 时：
         1. Material 类的所有属性在首次被赋非None值后不能再被修改和删除，
         2. 此时许可的属性关键字存储在self.slots中。
     """
     is_read_only: bool = True
     slots: Tuple = ('name', 'category', 'type', 'data')
     allowed_keys_values: Dict = {
-        'category': [None, 'Elastic', 'Plastic'],
-        'type': [None, 'Isotropic', 'IsotropicHardening', 'KinematicHardening']
+        'category': [None, 'Elastic', 'Plastic', 'ViscoElastic'],
+        'type': [None, 'Isotropic', 'IsotropicHardening', 'KinematicHardening', 'Maxwell']
     }
 
     def __init__(self) -> None:
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.data: List[float] = None  # type: ignore
```

### Comparing `pyfem-0.0.9/src/pyfem/io/Output.py` & `pyfem-0.1.0/src/pyfem/io/Mesh.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from pyfem.utils.visualization import object_dict_to_string
 
 
-class Output:
+class Mesh:
     def __init__(self) -> None:
         self.type: str = None  # type: ignore
-        self.field_outputs: str = None  # type: ignore
-        self.on_screen: bool = None  # type: ignore
+        self.file: str = None  # type: ignore
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
 
 if __name__ == "__main__":
-    output = Output()
-    print(output.__dict__.keys())
-    print(output)
-    print(output.to_string())
+    mesh = Mesh()
+    print(mesh.__dict__.keys())
+    print(mesh)
+    print(mesh.to_string())
```

### Comparing `pyfem-0.0.9/src/pyfem/io/Properties.py` & `pyfem-0.1.0/src/pyfem/io/Properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,59 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from pathlib import Path
 from typing import Dict, List, Any, Tuple, Union
 
 try:
     import tomllib  # type: ignore
 except ModuleNotFoundError:
     import tomli as tomllib
 
 from pyfem.io.Dof import Dof
 from pyfem.io.Section import Section
 from pyfem.io.Material import Material
 from pyfem.io.Mesh import Mesh
 from pyfem.io.BC import BC
+from pyfem.io.Amplitude import Amplitude
 from pyfem.io.Solver import Solver
 from pyfem.io.Output import Output
-from pyfem.mesh.NodeSet import NodeSet
-from pyfem.mesh.ElementSet import ElementSet
+from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import CYAN, MAGENTA, BLUE, END, error_style, info_style
 
 
 class Properties:
     """
     Properties类用于解析配置文件中定义的属性。
     当 self.is_read_only = True 时：
 
     1. Properties 类的所有属性在首次被赋非None值后不能再被修改和删除，
 
     2. 此时许可的属性关键字存储在self.slots中。
     """
     is_read_only: bool = True
     slots: Tuple = (
-        'work_path', 'input_file', 'toml', 'title', 'mesh', 'dof', 'materials', 'sections', 'bcs',
-        'solver', 'outputs', 'nodes', 'elements')
+        'work_path', 'input_file', 'toml', 'title', 'mesh', 'dof', 'materials', 'sections', 'amplitudes',
+        'bcs', 'solver', 'outputs', 'mesh_data')
 
     def __init__(self) -> None:
         self.work_path: Path = None  # type: ignore
         self.input_file: Path = None  # type: ignore
         self.toml: Dict = None  # type: ignore
         self.title: str = None  # type: ignore
         self.mesh: Mesh = None  # type: ignore
         self.dof: Dof = None  # type: ignore
         self.materials: List[Material] = None  # type: ignore
         self.sections: List[Section] = None  # type: ignore
+        self.amplitudes: List[Amplitude] = None  # type: ignore
         self.bcs: List[BC] = None  # type: ignore
         self.solver: Solver = None  # type: ignore
         self.outputs: List[Output] = None  # type: ignore
-        self.nodes: NodeSet = None  # type: ignore
-        self.elements: ElementSet = None  # type: ignore
+        self.mesh_data: MeshData = None  # type: ignore
 
     def __setattr__(self, key, value):
         if self.is_read_only:
             if key not in self.slots:
                 error_msg = f'{key} is not an allowable attribute keyword of {type(self).__name__}'
                 raise AttributeError(error_style(error_msg))
             elif hasattr(self, key) and self.__getattribute__(key) is not None:
@@ -103,20 +107,22 @@
         self.mesh = Mesh()
         allowed_keys = self.mesh.__dict__.keys()
         for key, item in mesh_dict.items():
             if key in allowed_keys:
                 self.mesh.__setattr__(key, item)
             else:
                 raise AttributeError(self.key_error_message(key, self.mesh))
-        if self.mesh.type == 'gmsh':
-            self.set_nodes_from_gmsh()
-            self.set_elements_from_gmsh()
-        if self.mesh.type == 'abaqus':
-            self.set_nodes_from_abaqus()
-            self.set_elements_from_abaqus()
+
+        mesh_path = Path(self.mesh.file)
+        if mesh_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
+            abs_mesh_path = mesh_path
+        else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
+            abs_mesh_path = self.work_path.joinpath(mesh_path)
+        self.mesh_data = MeshData()
+        self.mesh_data.read_file(abs_mesh_path, self.mesh.type)
 
     def set_dofs(self, dofs_dict: Dict) -> None:
         self.dof = Dof()
         allowed_keys = self.dof.__dict__.keys()
         for key, item in dofs_dict.items():
             if key in allowed_keys:
                 self.dof.__setattr__(key, item)
@@ -152,14 +158,26 @@
             for key, item in section_dict.items():
                 if key in allowed_keys:
                     section.__setattr__(key, item)
                 else:
                     raise AttributeError(self.key_error_message(key, section))
             self.sections.append(section)
 
+    def set_amplitudes(self, amplitudes_list: List) -> None:
+        self.amplitudes = []
+        for amplitude_dict in amplitudes_list:
+            amplitude = Amplitude()
+            allowed_keys = amplitude.__dict__.keys()
+            for key, item in amplitude_dict.items():
+                if key in allowed_keys:
+                    amplitude.__setattr__(key, item)
+                else:
+                    raise AttributeError(self.key_error_message(key, amplitude))
+            self.amplitudes.append(amplitude)
+
     def set_bcs(self, bcs_list: List) -> None:
         self.bcs = []
         for bc_dict in bcs_list:
             bc = BC()
             allowed_keys = bc.__dict__.keys()
             for key, item in bc_dict.items():
                 if key in allowed_keys:
@@ -176,52 +194,14 @@
             for key, item in output_dict.items():
                 if key in allowed_keys:
                     output.__setattr__(key, item)
                 else:
                     raise AttributeError(self.key_error_message(key, output))
             self.outputs.append(output)
 
-    def set_nodes_from_gmsh(self):
-        gmsh_path = Path(self.mesh.file)
-        if gmsh_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
-            abs_gmsh_file = gmsh_path
-        else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
-            abs_gmsh_file = self.work_path.joinpath(gmsh_path)
-        self.nodes = NodeSet()
-        self.nodes.read_gmsh_file(abs_gmsh_file)
-        self.nodes.update_indices()
-
-    def set_elements_from_gmsh(self):
-        gmsh_path = Path(self.mesh.file)
-        if gmsh_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
-            abs_gmsh_file = gmsh_path
-        else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
-            abs_gmsh_file = self.work_path.joinpath(gmsh_path)
-        self.elements = ElementSet()
-        self.elements.read_gmsh_file(abs_gmsh_file, self.sections)
-
-    def set_nodes_from_abaqus(self):
-        inp_path = Path(self.mesh.file)
-        if inp_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
-            abs_inp_path = inp_path
-        else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
-            abs_inp_path = self.work_path.joinpath(inp_path)
-        self.nodes = NodeSet()
-        self.nodes.read_inp_file(abs_inp_path)
-        self.nodes.update_indices()
-
-    def set_elements_from_abaqus(self):
-        inp_path = Path(self.mesh.file)
-        if inp_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
-            abs_inp_file = inp_path
-        else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
-            abs_inp_file = self.work_path.joinpath(inp_path)
-        self.elements = ElementSet()
-        self.elements.read_inp_file(abs_inp_file, self.sections)
-
     @staticmethod
     def key_error_message(key: Any, obj: Any) -> str:
         return error_style(f'{key} is not an allowable attribute keyword of {type(obj).__name__}')
 
     def read_file(self, filename: Union[Path, str]) -> None:
         """
         读取 .toml 格式的配置文件。
@@ -258,14 +238,18 @@
             dofs_dict = self.toml['dof']
             self.set_dofs(dofs_dict)
 
         if 'materials' in toml_keys:
             materials_list = self.toml['materials']
             self.set_materials(materials_list)
 
+        if 'amplitudes' in toml_keys:
+            amplitudes_list = self.toml['amplitudes']
+            self.set_amplitudes(amplitudes_list)
+
         if 'bcs' in toml_keys:
             bcs_list = self.toml['bcs']
             self.set_bcs(bcs_list)
 
         if 'solver' in toml_keys:
             solver_dict = self.toml['solver']
             self.set_solver(solver_dict)
```

### Comparing `pyfem-0.0.9/src/pyfem/io/Section.py` & `pyfem-0.1.0/src/pyfem/io/Section.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from typing import Optional, List
 
 from pyfem.utils.visualization import object_dict_to_string
 
 
 class Section:
     def __init__(self) -> None:
```

### Comparing `pyfem-0.0.9/src/pyfem/io/Solver.py` & `pyfem-0.1.0/src/pyfem/io/Output.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from pyfem.utils.visualization import object_dict_to_string
 
 
-class Solver:
+class Output:
     def __init__(self) -> None:
         self.type: str = None  # type: ignore
-        self.option: str = None  # type: ignore
-        self.total_time: float = 1.0
-        self.start_time: float = 0.0
-        self.max_increment: int = 100
-        self.initial_dtime: float = 1.0
-        self.max_dtime: float = 1.0
-        self.min_dtime: float = 0.001
-        self.dtype: str = 'float64'
+        self.field_outputs: str = None  # type: ignore
+        self.on_screen: bool = None  # type: ignore
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
 
 if __name__ == "__main__":
-    solver = Solver()
-    print(solver.__dict__.keys())
-    print(solver)
-    print(solver.to_string())
+    output = Output()
+    print(output.__dict__.keys())
+    print(output)
+    print(output.to_string())
```

### Comparing `pyfem-0.0.9/src/pyfem/io/arguments.py` & `pyfem-0.1.0/src/pyfem/io/arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 import sys
 from argparse import ArgumentParser, Namespace, SUPPRESS
 
 
 def get_arguments() -> Namespace:
     logo = r"""
                      ____             
@@ -31,15 +35,15 @@
 
     # 添加帮助选项
     parser.add_argument('-h', '--help', action='help', default=SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='pyfem 0.0.9')
+                        version='pyfem 0.1.0')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
         print('--------------------------------------')
```

### Comparing `pyfem-0.0.9/src/pyfem/io/write_vtk.py` & `pyfem-0.1.0/src/pyfem/io/write_vtk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from xml.etree.ElementTree import ElementTree, Element, SubElement
 
 from pyfem.assembly.Assembly import Assembly
 
 
 def write_vtk(assembly: Assembly):
     props = assembly.props
     timer = assembly.timer
-    dimension = props.nodes.dimension
+    dimension = props.mesh_data.dimension
 
     root = Element("VTKFile", {
         "type": "UnstructuredGrid",
         "version": "0.1",
         "byte_order": "LittleEndian"
     })
 
     ugrid = SubElement(root, "UnstructuredGrid")
     piece = SubElement(ugrid, "Piece", {
-        "NumberOfPoints": str(len(props.nodes)),
-        "NumberOfCells": str(len(props.elements))
+        "NumberOfPoints": str(len(props.mesh_data.nodes)),
+        "NumberOfCells": str(len(props.mesh_data.elements))
     })
 
     # 添加节点数据
     point_data = SubElement(piece, "PointData")
     temp = SubElement(point_data, "DataArray", {
         "type": "Float64",
         "Name": "Temperature",
         "NumberOfComponents": "1",
         "format": "ascii"
     })
     temp.text = ""
-    for _ in props.nodes.items():
+    for _ in props.mesh_data.nodes:
         temp.text += "0.0\n"  # 在这里添加具体的场量数值
 
     disp = SubElement(point_data, "DataArray", {
         "type": "Float64",
         "Name": "Displacement",
         "NumberOfComponents": "3",
         "format": "ascii"
@@ -63,15 +67,15 @@
     points = SubElement(piece, "Points")
     node_coords = SubElement(points, "DataArray", {
         "type": "Float64",
         "NumberOfComponents": "3",
         "format": "ascii"
     })
     node_coords.text = ""
-    for _, coord in props.nodes.items():
+    for coord in props.mesh_data.nodes:
         if dimension == 2:
             node_coords.text += " ".join("{:.6f}".format(c) for c in coord) + " 0.0\n"
         elif dimension == 3:
             node_coords.text += " ".join("{:.6f}".format(c) for c in coord) + "\n"
         else:
             raise NotImplementedError
 
@@ -92,15 +96,15 @@
         "Name": "types",
         "format": "ascii"
     })
     conn_elem.text = ""
     offset_elem.text = ""
     types_elem.text = ""
     offset = 0
-    for _, connectivity in props.elements.items():
+    for connectivity in props.mesh_data.elements:
         conn_elem.text += " ".join(str(node_id) for node_id in connectivity) + "\n"
         offset += len(connectivity)
         offset_elem.text += "{}\n".format(offset)
         if dimension == 2:
             types_elem.text += "9\n"
         elif dimension == 3:
             types_elem.text += "12\n"  # 12表示六面体单元类型
```

### Comparing `pyfem-0.0.9/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.1.0/src/pyfem/materials/BaseMaterial.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 
 class BaseMaterial:
     def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
         self.material: Material = material
         self.dimension: int = dimension
         self.option: Optional[str] = option
         self.ddsdde: ndarray = empty(0)
-        self.variable: ndarray = empty(0)
+        self.output: Dict[str, ndarray] = {}
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
-    def get_tangent(self, state_variable: Dict[str, ndarray],
+    def get_tangent(self, variable: Dict[str, ndarray],
+                    state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
-                    state: ndarray,
-                    dstate: ndarray,
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
-                    timer: Timer) -> Tuple[ndarray, ndarray]:
-        return self.ddsdde, self.variable
+                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
+        return self.ddsdde, self.output
```

### Comparing `pyfem-0.0.9/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.1.0/src/pyfem/materials/ElasticIsotropic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from typing import Optional, Tuple, Dict
 
-from numpy import array, outer, diag, float64, ndarray, dot
+from numpy import array, outer, diag, ndarray, dot
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
@@ -28,27 +28,27 @@
             if self.dimension == 3:
                 self.option = None
             self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
         else:
             error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
             raise NotImplementedError(error_style(error_msg))
 
-    def get_tangent(self, state_variable: Dict[str, ndarray],
+    def get_tangent(self, variable: Dict[str, ndarray],
+                    state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
-                    state: ndarray,
-                    dstate: ndarray,
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
-                    timer: Timer) -> Tuple[ndarray, ndarray]:
-        strain = state
+                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
+        strain = variable['strain']
         stress = dot(self.ddsdde, strain)
-        return self.ddsdde, stress
+        output = {'stress': stress}
+        return self.ddsdde, output
 
 
 def get_lame_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> Tuple[float, float]:
     r"""
     Compute Lamé parameters from Young's modulus and Poisson's ratio.
 
     The relationship between Lamé parameters and Young's modulus, Poisson's
```

### Comparing `pyfem-0.0.9/src/pyfem/materials/PlasticIsotropicHardening.py` & `pyfem-0.1.0/src/pyfem/materials/PlasticIsotropicHardening.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-"""
-
-"""
-from typing import Optional
-
-from pyfem.io.Material import Material
-from pyfem.materials.BaseMaterial import BaseMaterial
-from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
-from pyfem.utils.colors import error_style
-
-
-class PlasticIsotropicHardening(BaseMaterial):
-    allowed_option = ['PlaneStress', 'PlaneStrain', None]
-
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
-        super().__init__(material, dimension, option)
-        self.create_tangent()
-
-    def create_tangent(self):
-        young = self.material.data[0]
-        poisson = self.material.data[1]
-
-        if self.option in self.allowed_option:
-            if self.dimension == 3:
-                self.option = None
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
-        else:
-            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
-            raise NotImplementedError(error_style(error_msg))
-
-
-if __name__ == "__main__":
-    from pyfem.Job import Job
-
-    job = Job(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-
-    material_data = PlasticIsotropicHardening(job.props.materials[0], 3)
-    print(material_data.to_string())
+# -*- coding: utf-8 -*-
+"""
+
+"""
+from typing import Optional
+
+from pyfem.io.Material import Material
+from pyfem.materials.BaseMaterial import BaseMaterial
+from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
+from pyfem.utils.colors import error_style
+
+
+class PlasticIsotropicHardening(BaseMaterial):
+    allowed_option = ['PlaneStress', 'PlaneStrain', None]
+
+    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
+        super().__init__(material, dimension, option)
+        self.create_tangent()
+
+    def create_tangent(self):
+        young = self.material.data[0]
+        poisson = self.material.data[1]
+
+        if self.option in self.allowed_option:
+            if self.dimension == 3:
+                self.option = None
+            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
+        else:
+            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
+            raise NotImplementedError(error_style(error_msg))
+
+
+if __name__ == "__main__":
+    from pyfem.Job import Job
+
+    job = Job(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+
+    material_data = PlasticIsotropicHardening(job.props.materials[0], 3)
+    print(material_data.to_string())
```

### Comparing `pyfem-0.0.9/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.1.0/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
 from typing import Optional, Dict, Tuple
 
-from numpy import zeros, ndarray, dot, sqrt, outer
+from numpy import zeros, ndarray, dot, sqrt, outer, insert, delete
 
 from pyfem.fem.Timer import Timer
+from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
 from pyfem.utils.colors import error_style
-from pyfem.fem.constants import DTYPE
 
 
 class PlasticKinematicHardening(BaseMaterial):
     allowed_option = ['PlaneStress', 'PlaneStrain', 'Volume', None]
 
     def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
         super().__init__(material, dimension, option)
@@ -37,41 +37,67 @@
             if self.dimension == 3:
                 self.option = None
             self.ddsdde = get_stiffness_from_young_poisson(self.dimension, self.young, self.poisson, self.option)
         else:
             error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
             raise NotImplementedError(error_style(error_msg))
 
-    def get_tangent(self, state_variable: Dict[str, ndarray],
+    def get_tangent(self, variable: Dict[str, ndarray],
+                    state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
-                    state: ndarray,
-                    dstate: ndarray,
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
-                    timer: Timer) -> Tuple[ndarray, ndarray]:
+                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
 
         if state_variable == {}:
             state_variable['elastic_strain'] = zeros(ntens, dtype=DTYPE)
             state_variable['plastic_strain'] = zeros(ntens, dtype=DTYPE)
             state_variable['back_stress'] = zeros(ntens, dtype=DTYPE)
             state_variable['stress'] = zeros(ntens, dtype=DTYPE)
 
         elastic_strain = deepcopy(state_variable['elastic_strain'])
         plastic_strain = deepcopy(state_variable['plastic_strain'])
         back_stress = deepcopy(state_variable['back_stress'])
         stress = deepcopy(state_variable['stress'])
 
-        dstrain = dstate
+        dstrain = variable['dstrain']
+
+        E = self.young
+        nu = self.poisson
+
+        if self.option == 'PlaneStrain':
+            dstrain = insert(dstrain, 2, 0)
+        elif self.option == 'PlaneStress':
+            dstrain = insert(dstrain, 2, -nu / (1 - nu) * (dstrain[0] + dstrain[1]))
+
         elastic_strain += dstrain
-        ddsdde = self.ddsdde
+
+        ddsdde = zeros((ntens, ntens), dtype=DTYPE)
+
+        lam = E * nu / ((1.0 + nu) * (1.0 - 2.0 * nu))
+        mu = E / (2.0 * (1.0 + nu))
+
+        ddsdde[:ndi, :ndi] += lam
+        for i in range(ndi):
+            ddsdde[i, i] += 2 * mu
+        for i in range(ndi, ntens):
+            ddsdde[i, i] += mu
+
         stress += dot(ddsdde, dstrain)
-        smises = get_smises(stress - back_stress)
+        s = stress - back_stress
+        smises = get_smises(s)
+
+        # if element_id == 0 and igp == 0:
+        #     print(ddsdde)
+        #     print(dstrain)
+        #     print(stress)
+        #     print(dot(ddsdde, dstrain))
 
         if smises > (1.0 + self.tolerance) * self.yield_stress:
             hydrostatic_stress = sum(stress[:ndi]) / 3.0
             flow = stress - back_stress
             flow[:ndi] = flow[:ndi] - hydrostatic_stress
             flow *= 1.0 / smises
 
@@ -83,44 +109,63 @@
 
             plastic_strain[ndi:] += 3.0 * flow[ndi:] * delta_p
             elastic_strain[ndi:] -= 3.0 * flow[ndi:] * delta_p
 
             stress = back_stress + flow * self.yield_stress
             stress[:ndi] += hydrostatic_stress
 
+            # if element_id == 0 and igp == 0:
+            #     print(stress)
+
             EFFG = self.EG * (self.yield_stress + self.hard * delta_p) / smises
             EFFG2 = 2.0 * EFFG
             EFFG3 = 3.0 * EFFG
             EFFLAM = (self.EBULK3 - EFFG2) / 3.0
             EFFHRD = self.EG3 * self.hard / (self.EG3 + self.hard) - EFFG3
 
-            ddsdde = zeros(shape=(ntens, ntens))
+            ddsdde = zeros(shape=(ntens, ntens), dtype=DTYPE)
             ddsdde[:ndi, :ndi] = EFFLAM
 
             for i in range(ndi):
                 ddsdde[i, i] += EFFG2
 
             for i in range(ndi, ntens):
                 ddsdde[i, i] += EFFG
 
             ddsdde += EFFHRD * outer(flow, flow)
 
+        # if element_id == 0 and igp == 0:
+        #     print(stress)
+
         state_variable_new['elastic_strain'] = elastic_strain
         state_variable_new['plastic_strain'] = plastic_strain
         state_variable_new['back_stress'] = back_stress
         state_variable_new['stress'] = stress
 
-        return ddsdde, stress
+        if self.option == 'PlaneStrain':
+            ddsdde = delete(delete(ddsdde, 2, axis=0), 2, axis=1)
+            stress = delete(stress, 2)
+        elif self.option == 'PlaneStress':
+            ddsdde = delete(delete(ddsdde, 2, axis=0), 2, axis=1)
+            ddsdde[0, 0] -= lam * lam / (lam + 2 * mu)
+            ddsdde[0, 1] -= lam * lam / (lam + 2 * mu)
+            ddsdde[1, 0] -= lam * lam / (lam + 2 * mu)
+            ddsdde[1, 1] -= lam * lam / (lam + 2 * mu)
+            stress = delete(stress, 2)
+
+        output = {'stress': stress}
+
+        return ddsdde, output
 
 
 def get_smises(s: ndarray) -> float:
     if len(s) == 3:
         smises = sqrt(s[0] ** 2 + s[1] ** 2 - s[0] * s[1] + 3 * s[2] ** 2)
         return float(smises)
-    elif len(s) == 6:
+    elif len(s) >= 3:
         smises = (s[0] - s[1]) ** 2 + (s[1] - s[2]) ** 2 + (s[2] - s[0]) ** 2
         smises += 6 * sum([i ** 2 for i in s[3:]])
         smises = sqrt(0.5 * smises)
         return float(smises)
     else:
         raise NotImplementedError(error_style(f'unsupported stress dimension {len(s)}'))
```

### Comparing `pyfem-0.0.9/src/pyfem/materials/get_material_data.py` & `pyfem-0.1.0/src/pyfem/materials/get_material_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 """
 from typing import Optional
 
 from pyfem.io.Material import Material
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import ElasticIsotropic
 from pyfem.materials.PlasticKinematicHardening import PlasticKinematicHardening
+from pyfem.materials.ViscoElasticMaxwell import ViscoElasticMaxwell
 from pyfem.utils.colors import error_style
 
 material_data_dict = {
     'ElasticIsotropic': ElasticIsotropic,
     'PlasticKinematicHardening': PlasticKinematicHardening,
+    'ViscoElasticMaxwell': ViscoElasticMaxwell
 }
 
 
 def get_material_data(material: Material, dimension: int, option: Optional[str] = None) -> BaseMaterial:
     class_name = f'{material.category}{material.type}'.strip().replace(' ', '')
 
     if class_name in material_data_dict:
```

### Comparing `pyfem-0.0.9/src/pyfem/mesh/ElementSet.py` & `pyfem-0.1.0/src/pyfem/mesh/ElementSet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import os
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from copy import deepcopy
 from pathlib import Path
 from typing import List, Any, Dict, Union
 
 import meshio  # type: ignore
 import numpy as np
 
@@ -67,20 +70,24 @@
         从 ABAQUS inp文件中读取单元集合。
         使用meshio库读取inp文件，并根据给定的sections列表提取指定的单元集合。
         遍历读取的网格的单元集合字典，并将符合条件的单元添加到单元集合中。
         """
         # logger.info(f"Reading elements from {file_name}")
         mesh = meshio.read(file_name, file_format="abaqus")
 
+        for cell in mesh.cells:
+            print(cell.dim, cell.type, cell.data)
+
         assigned_element_set = []
         for section in sections:
             assigned_element_set += section.element_sets
 
         assembly_element_id = 0
         for cell_name, cell_dict in mesh.cell_sets_dict.items():
+
             if cell_name != 'gmsh:bounding_entities' and cell_name in assigned_element_set:
                 for mesh_type, element_ids in cell_dict.items():
                     for element_id in element_ids:
                         connectivity = deepcopy(mesh.cells_dict[mesh_type][element_id])
                         self.add_item_by_element_id(assembly_element_id, cell_name, connectivity)
                         assembly_element_id += 1
 
@@ -95,22 +102,24 @@
         else:
             self.element_sets[element_set_name].append(element_id)
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
-    props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-
-    os.chdir(r'F:\Github\pyfem\examples\rectangle')
+    # props = Properties()
+    # props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+    #
+    # os.chdir(r'F:\Github\pyfem\examples\rectangle')
+    #
+    # elements = ElementSet()
+    # elements.read_gmsh_file('rectangle4.msh', props.sections)
+    # elements.show()
 
-    elements = ElementSet()
-    elements.read_gmsh_file('rectangle4.msh', props.sections)
-    elements.show()
+    props = Properties()
+    props.read_file(r'F:\Github\pyfem\examples\quad_tria\quad_tria.toml')
 
-    # os.chdir(r'F:\Github\pyfem\examples\abaqus')
+    # os.chdir(r'F:\Github\pyfem\examples\quad_tria')
     #
     # elements = ElementSet()
-    # elements.read_inp_file('Job-1.inp', props.sections)
-    # # elements.get_dof_types()
+    # elements.read_inp_file('quad_tria.inp', props.sections)
     # elements.show()
```

### Comparing `pyfem-0.0.9/src/pyfem/mesh/NodeSet.py` & `pyfem-0.1.0/src/pyfem/mesh/NodeSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 import os
 from pathlib import Path
 from typing import List, Dict, Union
 
 import meshio  # type: ignore
 from numpy import array, ndarray
 
+from pyfem.fem.constants import DTYPE
 from pyfem.utils.IntKeyDict import IntKeyDict
 from pyfem.utils.logger import get_logger
 from pyfem.utils.wrappers import show_running_time
-from pyfem.fem.constants import DTYPE
 
 logger = get_logger()
 
 
 class NodeSet(IntKeyDict):
 
     def __init__(self) -> None:
@@ -122,14 +126,14 @@
     # # nodes.read_gmsh_file('rectangle100.msh')
     # nodes.read_gmsh_file('rectangle10000.msh')
     # # print(nodes.dimension)
     # # print(nodes.node_sets)
     # print(nodes.get_coords_by_ids([0, 1, 2]))
     # nodes.show()
 
-    os.chdir(r'F:\Github\pyfem\examples\specimen')
-    nodes.read_inp_file('Job-1.inp')
+    os.chdir(r'F:\Github\pyfem\examples\quad_tria')
+    nodes.read_inp_file('quad_tria.inp')
     nodes.show()
     print(nodes.dimension)
     print(nodes.node_sets)
     print(nodes.get_coords_by_ids([0, 1, 2]).dtype)
     # nodes.show()
```

### Comparing `pyfem-0.0.9/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.1.0/src/pyfem/solvers/LinearSolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 """
 
 """
 from numpy import empty
 from scipy.sparse.linalg import spsolve  # type: ignore
 
 from pyfem.assembly.Assembly import Assembly
+from pyfem.fem.constants import DTYPE
 from pyfem.io.Solver import Solver
 from pyfem.io.write_vtk import write_vtk
-from pyfem.fem.constants import DTYPE
 from pyfem.solvers.BaseSolver import BaseSolver
-from pyfem.utils.wrappers import show_running_time
 
 
 class LinearSolver(BaseSolver):
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
-        super().__init__(assembly, solver)
+        super().__init__()
         self.assembly: Assembly = assembly
         self.solver: Solver = solver
         self.dof_solution = empty(0, dtype=DTYPE)
         self.PENALTY = 1.0e16
 
     def run(self) -> None:
         self.solve()
```

### Comparing `pyfem-0.0.9/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.1.0/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 from copy import deepcopy
 
 from numpy import zeros
 from numpy.linalg import norm
 from scipy.sparse.linalg import splu  # type: ignore
 
 from pyfem.assembly.Assembly import Assembly
+from pyfem.fem.constants import DTYPE
 from pyfem.io.Solver import Solver
 from pyfem.io.write_vtk import write_vtk, write_pvd
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.utils.colors import error_style
 from pyfem.utils.colors import info_style
-from pyfem.utils.wrappers import show_running_time
-from pyfem.fem.constants import DTYPE
 
 
 class NonlinearSolver(BaseSolver):
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
-        super().__init__(assembly, solver)
+        super().__init__()
         self.assembly: Assembly = assembly
         self.solver: Solver = solver
         self.dof_solution = zeros(self.assembly.total_dof_number)
         self.PENALTY = 1.0e16
         self.FORCE_TOL = 1.0e-6
         self.MAX_NITER = 32
 
     def run(self) -> None:
-        self.Newton_Raphson_solve()
+        if self.assembly.props.solver.option in ['', 'NewtonRaphson', None]:
+            self.Newton_Raphson_solve()
+        elif self.assembly.props.solver.option == 'InitialTangent':
+            self.initial_tangent_solve()
 
-    @show_running_time
-    def initial_tangent_solve(self) -> None:
+    def Newton_Raphson_solve(self) -> None:
         timer = self.assembly.timer
-
         timer.total_time = self.solver.total_time
         timer.dtime = self.solver.initial_dtime
         timer.time0 = self.solver.start_time
         timer.increment = 0
         timer.frame_ids.append(0)
 
         self.assembly.update_element_field_variables()
@@ -48,38 +48,38 @@
         for increment in range(1, self.solver.max_increment):
 
             timer.time1 = timer.time0 + timer.dtime
             timer.increment = increment
 
             print(info_style(f'increment = {increment}, time = {timer.time1}'))
 
-            self.assembly.ddof_solution = zeros(self.assembly.total_dof_number)
+            self.assembly.ddof_solution = zeros(self.assembly.total_dof_number, dtype=DTYPE)
 
             is_convergence = False
             for niter in range(self.MAX_NITER):
+                self.assembly.assembly_global_stiffness()
+                fint = self.assembly.fint
+                rhs = deepcopy(self.assembly.fext)
                 if niter == 0:
-                    self.assembly.assembly_global_stiffness()
-                    fint = self.assembly.fint
-                    rhs = deepcopy(self.assembly.fext)
                     for bc_data in self.assembly.bc_data_list:
                         for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
                             self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
-                            rhs[dof_id] += dof_value * timer.dtime / timer.total_time * self.PENALTY
-                    LU = splu(self.assembly.global_stiffness)
+                            rhs[dof_id] += dof_value * (bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(
+                                timer.time0)) * self.PENALTY
                 else:
-                    fint = self.assembly.fint
-                    rhs = deepcopy(self.assembly.fext)
                     for bc_data in self.assembly.bc_data_list:
                         for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
+                            self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
                             rhs[dof_id] = 0.0 * self.PENALTY
 
+                LU = splu(self.assembly.global_stiffness)
                 da = LU.solve(rhs - fint)
 
                 self.assembly.ddof_solution += da
-                self.assembly.update_element_data_without_stiffness()
+                self.assembly.update_element_data()
                 self.assembly.assembly_fint()
 
                 f_residual = self.assembly.fext - self.assembly.fint
                 f_residual[self.assembly.bc_dof_ids] = 0
                 f_residual = norm(f_residual)
 
                 print(f'  niter = {niter}, force residual = {f_residual}')
@@ -105,16 +105,17 @@
             if timer.is_done():
                 write_pvd(self.assembly)
                 break
 
         if not timer.is_done():
             raise NotImplementedError(error_style('maximum increment is reached'))
 
-    def Newton_Raphson_solve(self) -> None:
+    def initial_tangent_solve(self) -> None:
         timer = self.assembly.timer
+
         timer.total_time = self.solver.total_time
         timer.dtime = self.solver.initial_dtime
         timer.time0 = self.solver.start_time
         timer.increment = 0
         timer.frame_ids.append(0)
 
         self.assembly.update_element_field_variables()
@@ -124,37 +125,39 @@
         for increment in range(1, self.solver.max_increment):
 
             timer.time1 = timer.time0 + timer.dtime
             timer.increment = increment
 
             print(info_style(f'increment = {increment}, time = {timer.time1}'))
 
-            self.assembly.ddof_solution = zeros(self.assembly.total_dof_number, dtype=DTYPE)
+            self.assembly.ddof_solution = zeros(self.assembly.total_dof_number)
 
             is_convergence = False
             for niter in range(self.MAX_NITER):
-                self.assembly.assembly_global_stiffness()
-                fint = self.assembly.fint
-                rhs = deepcopy(self.assembly.fext)
                 if niter == 0:
+                    self.assembly.assembly_global_stiffness()
+                    fint = self.assembly.fint
+                    rhs = deepcopy(self.assembly.fext)
                     for bc_data in self.assembly.bc_data_list:
                         for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
                             self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
-                            rhs[dof_id] += dof_value * timer.dtime / timer.total_time * self.PENALTY
+                            rhs[dof_id] += dof_value * (bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(
+                                timer.time0)) * self.PENALTY
+                    LU = splu(self.assembly.global_stiffness)
                 else:
+                    fint = self.assembly.fint
+                    rhs = deepcopy(self.assembly.fext)
                     for bc_data in self.assembly.bc_data_list:
                         for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
-                            self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
                             rhs[dof_id] = 0.0 * self.PENALTY
 
-                LU = splu(self.assembly.global_stiffness)
                 da = LU.solve(rhs - fint)
 
                 self.assembly.ddof_solution += da
-                self.assembly.update_element_data()
+                self.assembly.update_element_data_without_stiffness()
                 self.assembly.assembly_fint()
 
                 f_residual = self.assembly.fext - self.assembly.fint
                 f_residual[self.assembly.bc_dof_ids] = 0
                 f_residual = norm(f_residual)
 
                 print(f'  niter = {niter}, force residual = {f_residual}')
```

### Comparing `pyfem-0.0.9/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.1.0/src/pyfem/solvers/get_solver_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Solver import Solver
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.solvers.LinearSolver import LinearSolver
 from pyfem.solvers.NonlinearSolver import NonlinearSolver
 from pyfem.utils.colors import error_style
```

### Comparing `pyfem-0.0.9/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.1.0/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem/utils/colors.py` & `pyfem-0.1.0/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem/utils/logger.py` & `pyfem-0.1.0/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem/utils/visualization.py` & `pyfem-0.1.0/src/pyfem/utils/visualization.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,7 +42,20 @@
         elif isinstance(item, ndarray):
             msg += '  ' * level + GREEN + f'|- {key}: ' + END + f'{type(item)} with shape = {item.shape} \n'
         elif key == 'global_stiffness':
             msg += '  ' * level + GREEN + f'|- {key}: ' + END + f'{type(item)} with shape = {item.shape} \n'
         else:
             msg += '  ' * level + GREEN + f'|- {key}: ' + END + f'{item}\n'
     return msg[:-1]
+
+
+def object_slots_to_string_ndarray(obj, level: int = 1) -> str:
+    msg = BLUE + obj.__str__() + END
+    msg += '\n'
+    for key in obj.__slots__:
+        item = obj.__getattribute__(key)
+        if isinstance(item, ndarray):
+            msg += '  ' * level + GREEN + f'|- {key}: ' + END + f'{type(item)} with shape = {item.shape} \n'
+            msg += insert_spaces(5 + (level - 1) * 2, f'{item}') + '\n'
+        else:
+            msg += '  ' * level + GREEN + f'|- {key}: ' + END + f'{item}\n'
+    return msg[:-1]
```

### Comparing `pyfem-0.0.9/src/pyfem/utils/wrappers.py` & `pyfem-0.1.0/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.9/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.1.0/src/pyfem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.9
+Version: 0.1.0
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.0.9/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.1.0/src/pyfem.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,37 @@
 src/pyfem/__main__.py
 src/pyfem.egg-info/PKG-INFO
 src/pyfem.egg-info/SOURCES.txt
 src/pyfem.egg-info/dependency_links.txt
 src/pyfem.egg-info/entry_points.txt
 src/pyfem.egg-info/requires.txt
 src/pyfem.egg-info/top_level.txt
+src/pyfem/amplitude/BaseAmplitude.py
+src/pyfem/amplitude/TabularAmplitude.py
+src/pyfem/amplitude/__init__.py
+src/pyfem/amplitude/get_amplitude_data.py
 src/pyfem/assembly/Assembly.py
 src/pyfem/assembly/__init__.py
 src/pyfem/bc/BaseBC.py
 src/pyfem/bc/DirichletBC.py
+src/pyfem/bc/NeumannBC.py
 src/pyfem/bc/__init__.py
 src/pyfem/bc/get_bc_data.py
 src/pyfem/elements/BaseElement.py
 src/pyfem/elements/IsoElementDiagram.py
 src/pyfem/elements/IsoElementShape.py
 src/pyfem/elements/SolidPlaneSmallStrain.py
 src/pyfem/elements/SolidVolumeSmallStrain.py
 src/pyfem/elements/__init__.py
 src/pyfem/elements/get_element_data.py
 src/pyfem/elements/get_iso_element_type.py
 src/pyfem/fem/Timer.py
 src/pyfem/fem/__init__.py
 src/pyfem/fem/constants.py
+src/pyfem/io/Amplitude.py
 src/pyfem/io/BC.py
 src/pyfem/io/Dof.py
 src/pyfem/io/Material.py
 src/pyfem/io/Mesh.py
 src/pyfem/io/Output.py
 src/pyfem/io/Properties.py
 src/pyfem/io/Section.py
@@ -38,18 +44,19 @@
 src/pyfem/io/__init__.py
 src/pyfem/io/arguments.py
 src/pyfem/io/write_vtk.py
 src/pyfem/materials/BaseMaterial.py
 src/pyfem/materials/ElasticIsotropic.py
 src/pyfem/materials/PlasticIsotropicHardening.py
 src/pyfem/materials/PlasticKinematicHardening.py
+src/pyfem/materials/ViscoElasticMaxwell.py
 src/pyfem/materials/__init__.py
 src/pyfem/materials/get_material_data.py
-src/pyfem/materials/run.py
 src/pyfem/mesh/ElementSet.py
+src/pyfem/mesh/MeshData.py
 src/pyfem/mesh/NodeSet.py
 src/pyfem/mesh/__init__.py
 src/pyfem/solvers/BaseSolver.py
 src/pyfem/solvers/LinearSolver.py
 src/pyfem/solvers/NonlinearSolver.py
 src/pyfem/solvers/__init__.py
 src/pyfem/solvers/get_solver_data.py
```

