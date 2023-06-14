# Comparing `tmp/pyhalo-0.2.7.tar.gz` & `tmp/pyhalo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.7.tar", last modified: Sat Jun 10 17:52:09 2023, max compression
+gzip compressed data, was "pyhalo-0.2.8.tar", last modified: Wed Jun 14 15:40:38 2023, max compression
```

## Comparing `pyhalo-0.2.7.tar` & `pyhalo-0.2.8.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.671340 pyhalo-0.2.7/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.7/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.7/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.7/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.7/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.7/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-10 17:52:09.670659 pyhalo-0.2.7/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.7/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.565345 pyhalo-0.2.7/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.7/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.7/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.577395 pyhalo-0.2.7/pyHalo/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.584871 pyhalo-0.2.7/pyHalo/Cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.7/pyHalo/Cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Cosmology/cosmology.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Cosmology/geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.589746 pyhalo-0.2.7/pyHalo/Halos/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.599882 pyhalo-0.2.7/pyHalo/Halos/HaloModels/
--rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/NFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/PTMass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/PsuedoJaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFWemulator.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/ULDM.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/generalized_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.7/pyHalo/Halos/HaloModels/powerlaw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.7/pyHalo/Halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-06-10 17:05:16.000000 pyhalo-0.2.7/pyHalo/Halos/concentration.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.7/pyHalo/Halos/halo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/lens_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-10 01:21:15.000000 pyhalo-0.2.7/pyHalo/Halos/tidal_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Halos/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.610087 pyhalo-0.2.7/pyHalo/Rendering/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.617359 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/density_peaks.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-06-10 17:27:13.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/mass_function_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2285 2023-06-09 20:28:33.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/stucker.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.623072 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.7/pyHalo/Rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/correlated_structure.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/halo_population.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.7/pyHalo/Rendering/line_of_sight.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/rendering_class_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.7/pyHalo/Rendering/subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/Rendering/two_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.7/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3061 2023-06-09 21:04:32.000000 pyhalo-0.2.7/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4769 2023-06-10 17:07:58.000000 pyhalo-0.2.7/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8338 2023-06-10 16:58:29.000000 pyhalo-0.2.7/pyHalo/plotting_routines.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    52889 2023-06-10 17:09:44.000000 pyhalo-0.2.7/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.7/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.7/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1448 2023-06-09 21:04:32.000000 pyhalo-0.2.7/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.7/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.582986 pyhalo-0.2.7/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     4043 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.7/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-10 17:52:09.000000 pyhalo-0.2.7/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-10 17:51:37.000000 pyhalo-0.2.7/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-10 17:52:09.671532 pyhalo-0.2.7/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.7/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.636345 pyhalo-0.2.7/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.7/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1858 2023-06-10 01:03:10.000000 pyhalo-0.2.7/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.640788 pyhalo-0.2.7/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.7/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.653923 pyhalo-0.2.7/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.7/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.7/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.7/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.7/tests/test_halos/test_powerlaw_profile.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.7/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.7/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      917 2023-06-10 17:50:52.000000 pyhalo-0.2.7/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1153 2023-06-10 17:27:13.000000 pyhalo-0.2.7/tests/test_plotting.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3384 2023-06-10 01:27:42.000000 pyhalo-0.2.7/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.659579 pyhalo-0.2.7/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.7/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.665346 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10932 2023-06-09 19:49:01.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3776 2023-06-09 22:32:59.000000 pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_stucker.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-10 17:52:09.669292 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.7/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.7/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.7/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.738269 pyhalo-0.2.8/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.8/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.8/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.8/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.8/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-14 15:40:38.737576 pyhalo-0.2.8/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.8/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.529179 pyhalo-0.2.8/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.8/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.545109 pyhalo-0.2.8/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.554355 pyhalo-0.2.8/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.8/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.558920 pyhalo-0.2.8/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.565753 pyhalo-0.2.8/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.8/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-06-10 17:05:16.000000 pyhalo-0.2.8/pyHalo/Halos/concentration.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.8/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-10 01:21:15.000000 pyhalo-0.2.8/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.571260 pyhalo-0.2.8/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.576717 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-06-10 17:27:13.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2285 2023-06-09 20:28:33.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.580167 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.8/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.8/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.8/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      157 2023-06-14 15:39:35.000000 pyhalo-0.2.8/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3061 2023-06-09 21:04:32.000000 pyhalo-0.2.8/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3872 2023-06-13 07:05:17.000000 pyhalo-0.2.8/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8338 2023-06-10 16:58:29.000000 pyhalo-0.2.8/pyHalo/plotting_routines.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    55312 2023-06-13 19:50:28.000000 pyhalo-0.2.8/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.8/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1448 2023-06-09 21:04:32.000000 pyhalo-0.2.8/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.8/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.552416 pyhalo-0.2.8/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4043 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.8/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-14 15:40:10.000000 pyhalo-0.2.8/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-14 15:40:38.738460 pyhalo-0.2.8/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.8/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.628376 pyhalo-0.2.8/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.8/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1858 2023-06-10 01:03:10.000000 pyhalo-0.2.8/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.638108 pyhalo-0.2.8/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.8/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.718651 pyhalo-0.2.8/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.8/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.8/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.8/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.8/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.8/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.8/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      917 2023-06-10 17:50:52.000000 pyhalo-0.2.8/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1153 2023-06-10 17:27:13.000000 pyhalo-0.2.8/tests/test_plotting.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3384 2023-06-10 01:27:42.000000 pyhalo-0.2.8/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.724126 pyhalo-0.2.8/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.8/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.728980 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10932 2023-06-09 19:49:01.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3776 2023-06-09 22:32:59.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.735653 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.8/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.8/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.7/CONTRIBUTING.rst` & `pyhalo-0.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/LICENSE` & `pyhalo-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/PKG-INFO` & `pyhalo-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.7/README.rst` & `pyhalo-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/docs/Makefile` & `pyhalo-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/docs/conf.py` & `pyhalo-0.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/docs/installation.rst` & `pyhalo-0.2.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/docs/make.bat` & `pyhalo-0.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Cosmology/cosmology.py` & `pyhalo-0.2.8/pyHalo/Cosmology/cosmology.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Cosmology/geometry.py` & `pyhalo-0.2.8/pyHalo/Cosmology/geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/NFW.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/NFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/PTMass.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/PTMass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/PsuedoJaffe.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/PsuedoJaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFW.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/TNFWemulator.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFWemulator.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/ULDM.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/ULDM.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/gaussian.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/generalized_nfw.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/generalized_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/HaloModels/powerlaw.py` & `pyhalo-0.2.8/pyHalo/Halos/HaloModels/powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/concentration.py` & `pyhalo-0.2.8/pyHalo/Halos/concentration.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/halo_base.py` & `pyhalo-0.2.8/pyHalo/Halos/halo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/lens_cosmo.py` & `pyhalo-0.2.8/pyHalo/Halos/lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/tidal_truncation.py` & `pyhalo-0.2.8/pyHalo/Halos/tidal_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Halos/util.py` & `pyhalo-0.2.8/pyHalo/Halos/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/delta_function.py` & `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/density_peaks.py` & `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/density_peaks.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/mass_function_base.py` & `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/mass_function_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/stucker.py` & `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/stucker.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/MassFunctions/util.py` & `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/correlated.py` & `pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/nfw.py` & `pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/SpatialDistributions/uniform.py` & `pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/correlated_structure.py` & `pyhalo-0.2.8/pyHalo/Rendering/correlated_structure.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/halo_population.py` & `pyhalo-0.2.8/pyHalo/Rendering/halo_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/line_of_sight.py` & `pyhalo-0.2.8/pyHalo/Rendering/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/rendering_class_base.py` & `pyhalo-0.2.8/pyHalo/Rendering/rendering_class_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/subhalos.py` & `pyhalo-0.2.8/pyHalo/Rendering/subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/Rendering/two_halo.py` & `pyhalo-0.2.8/pyHalo/Rendering/two_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/concentration_models.py` & `pyhalo-0.2.8/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/defaults.py` & `pyhalo-0.2.8/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/mass_function_models.py` & `pyhalo-0.2.8/pyHalo/mass_function_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         return WDMPowerLaw, kwargs_model_out
     elif model_name == 'POWER_LAW_TURNOVER':
         return ShethTormenTurnover, kwargs_model_out
     elif model_name == 'SHMF_MIXED_WDM_TURNOVER':
         return MixedWDMPowerLaw, kwargs_model_out
     elif model_name == 'MIXED_WDM_TURNOVER':
         return ShethTormenMixedWDM, kwargs_model_out
-    elif model_name == 'STUCKER_SHMF':
+    elif model_name in ['STUCKER_SHMF', 'STUCKER']:
         if 'dlogT_dlogk' not in kwargs_model.keys():
             raise Exception('Must specify |dlogT_dlogk| (absolute value of the ' \
             'logarithmic derivative of the transfer function) when using the STUCKER model.)')
         if 'a_wdm' in kwargs_model.keys():
             raise Exception('Cannot specify a_wdm with the Stucker model.')
         if 'b_wdm' in kwargs_model.keys():
             raise Exception('Cannot specify b_wdm with the Stucker model.')
@@ -71,29 +71,15 @@
             raise Exception('Cannot specify c_wdm with the Stucker model.')
         from pyHalo.Rendering.MassFunctions.stucker import stucker_suppression_params
         a_wdm, b_wdm, c_wdm = stucker_suppression_params(kwargs_model_out['dlogT_dlogk'])
         kwargs_model_out['a_wdm'] = a_wdm
         kwargs_model_out['b_wdm'] = b_wdm
         kwargs_model_out['c_wdm'] = c_wdm
         del kwargs_model_out['dlogT_dlogk']
-        return WDMPowerLaw, kwargs_model_out
-    elif model_name == 'STUCKER':
-        if 'dlogT_dlogk' not in kwargs_model.keys():
-            raise Exception('Must specify |dlogT_dlogk| (absolute value of the ' \
-            'logarithmic derivative of the transfer function) when using the STUCKER model.)')
-        if 'a_wdm' in kwargs_model.keys():
-            raise Exception('Cannot specify a_wdm with the Stucker model.')
-        if 'b_wdm' in kwargs_model.keys():
-            raise Exception('Cannot specify b_wdm with the Stucker model.')
-        if 'c_wdm' in kwargs_model.keys():
-            raise Exception('Cannot specify c_wdm with the Stucker model.')
-        from pyHalo.Rendering.MassFunctions.stucker import stucker_suppression_params
-        a_wdm, b_wdm, c_wdm = stucker_suppression_params(kwargs_model_out['dlogT_dlogk'])
-        kwargs_model_out['a_wdm'] = a_wdm
-        kwargs_model_out['b_wdm'] = b_wdm
-        kwargs_model_out['c_wdm'] = c_wdm
-        del kwargs_model_out['dlogT_dlogk']
-        return ShethTormenTurnover, kwargs_model_out
+        if model_name == 'STUCKER':
+            return ShethTormenTurnover, kwargs_model_out
+        else:
+            return WDMPowerLaw, kwargs_model_out
     else:
         raise Exception('model name '+str(model_name)+' not recognized')
```

### Comparing `pyhalo-0.2.7/pyHalo/plotting_routines.py` & `pyhalo-0.2.8/pyHalo/plotting_routines.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/preset_models.py` & `pyhalo-0.2.8/pyHalo/preset_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -672,37 +672,56 @@
                   'log_m_host': log_m_host, 'r_tidal': r_tidal, 'LOS_normalization': LOS_normalization,
                   'geometry_type': geometry_type, 'kwargs_cosmo': kwargs_cosmo,
                   'kwargs_density_profile': kwargs_density_profile
                   }
     return WDM(**kwargs_wdm)
 
 def WDMGeneral(z_lens, z_source, log_mc, dlogT_dlogk, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
+        truncation_model_subhalos='TRUNCATION_MEAN_DENSITY', kwargs_truncation_model_subhalos={},
+        truncation_model_fieldhalos='SPLASHBACK', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
         LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
         mdef_subhalos='TNFW', mdef_field_halos='TNFW', kwargs_density_profile={}):
 
     """
+    This preset model implements a generalized treatment of warm dark matter, or any theory that produces a cutoff in
+    the linear matter power spectrum. One additional free parameter is added to parameterize the cutoff in the matter
+     power spectrum, dlogT_dlogk, which is the absolute value of the logarithmic derivative of the transfer function
+     evaluated at k_1/2, the wavenumber corresponding to the half-mode mass (or log_mc).
+
+     In this model, halo concentrations are computed following the formalism suggeesteed by Schneider et al. (2012) and
+     Ludlow et al. (2016), in which the central density of a halo more or less is fully determined by the formation time.
+
+     The mass function is computed from dlogT_dlogk based on the prescription by Stucker et al. (2021)
+     https://arxiv.org/pdf/2109.09760.pdf
 
     :param z_lens: the lens redshift
-    :param z_source:
-    :param log_mc:
-    :param dlogT_dlogk:
-    :param sigma_sub:
-    :param log_mlow:
-    :param log_mhigh:
-    :param shmf_log_slope:
-    :param cone_opening_angle_arcsec:
-    :param log_m_host:
-    :param r_tidal:
-    :param LOS_normalization:
-    :param geometry_type:
-    :param kwargs_cosmo:
-    :param mdef_subhalos:
-    :param mdef_field_halos:
-    :param kwargs_density_profile:
+    :param z_source: source redshift
+    :param log_mc: the log (base 10) of the half-mode mass
+    :param dlogT_dlogk: the absolute value of the logarithmic derivative of the transfer function at k_1/2; the model
+    is calibrated for values between ~1 and ~3
+    :param sigma_sub: amplitude of the subhalo mass function
+    :param log_mlow: minimum halo mass to render
+    :param log_mhigh: maximum halo mass to render
+    :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
+    :param kwargs_truncation_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
+    complete list
+    :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
+    :param shmf_log_slope: logarithmic slope of the subhalo mass function
+    :param cone_opening_angle_arcsec: the opening angle of the rendering volume
+    :param log_m_host: the log (base 10) of the host halo mass
+    :param r_tidal: the core size in units of the scale radius of the host halo; subhalos are rendered uniformly in 3D
+    inside this radius
+    :param LOS_normalization: the amplitude of the LOS mass function relative to Sheth-Tormen
+    :param geometry_type: CONE, DOUBLE_CONE, CYLINDER - sets the geometry of the rendering volume
+    :param kwargs_cosmo: keyword arguments to set cosmology
+    :param mdef_subhalos: mass definition for subhalos
+    :param mdef_field_halos: mass definition for field halos
+    :param kwargs_density_profile: keyword arguments for the density profile
     :return:
     """
     # FIRST WE CREATE AN INSTANCE OF PYHALO, WHICH SETS THE COSMOLOGY
     pyhalo = pyHalo(z_lens, z_source, kwargs_cosmo)
     # WE ALSO SPECIFY THE GEOMETRY OF THE RENDERING VOLUME
     geometry = Geometry(pyhalo.cosmology, z_lens, z_source,
                         cone_opening_angle_arcsec, geometry_type)
@@ -712,22 +731,21 @@
     fieldhalo_spatial_distribution = LensConeUniform
 
     kwargs_model_dlogT_dlogk = {'dlogT_dlogk': dlogT_dlogk}
     mass_function_model_subhalos, kwargs_mfunc_subs = preset_mass_function_models('STUCKER_SHMF', kwargs_model_dlogT_dlogk)
     mass_function_model_fieldhalos, kwargs_mfunc_field = preset_mass_function_models('STUCKER', kwargs_model_dlogT_dlogk)
 
     # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
-    truncation_model_subhalos = 'TRUNCATION_MEAN_DENSITY'
-    truncation_model_fieldhalos = 'SPLASHBACK'
-
-    model_subhalos, kwargs_truncation_model_subhalos = truncation_models(truncation_model_subhalos)
+    model_subhalos, kwargs_truncation_model_subhalos = truncation_models(truncation_model_subhalos,
+                                                                         kwargs_truncation_model_subhalos)
     kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
     truncation_model_subhalos = model_subhalos(**kwargs_truncation_model_subhalos)
 
-    model_fieldhalos, kwargs_truncation_model_fieldhalos = truncation_models(truncation_model_fieldhalos)
+    model_fieldhalos, kwargs_truncation_model_fieldhalos = truncation_models(truncation_model_fieldhalos,
+                                                                             kwargs_truncation_model_fieldhalos)
     kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
     truncation_model_fieldhalos = model_fieldhalos(**kwargs_truncation_model_fieldhalos)
 
     # SET THE CONCENTRATION-MASS RELATION FOR SUBHALOS AND FIELD HALOS
     concentration_model = 'FROM_FORMATION_HISTORY'
     model_subhalos, kwargs_concentration_model_subhalos = preset_concentration_models(concentration_model,
                                                                                       kwargs_model_dlogT_dlogk)
```

### Comparing `pyhalo-0.2.7/pyHalo/pyhalo.py` & `pyhalo-0.2.8/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/realization_extensions.py` & `pyhalo-0.2.8/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/single_realization.py` & `pyhalo-0.2.8/pyHalo/single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/truncation_models.py` & `pyhalo-0.2.8/pyHalo/truncation_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo/utilities.py` & `pyhalo-0.2.8/pyHalo/utilities.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.8/pyHalo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.7/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.8/pyHalo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/pyproject.toml` & `pyhalo-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.7/setup.py` & `pyhalo-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_concentration_models.py` & `pyhalo-0.2.8/tests/test_concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.8/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.8/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.8/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.8/tests/test_halos/test_adiabatic_tides.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.8/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.8/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.8/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.8/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.8/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.8/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.8/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_powerlaw_profile.py` & `pyhalo-0.2.8/tests/test_halos/test_powerlaw_profile.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.8/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_truncation.py` & `pyhalo-0.2.8/tests/test_halos/test_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_uldm.py` & `pyhalo-0.2.8/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_halos/test_util.py` & `pyhalo-0.2.8/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_mass_function_models.py` & `pyhalo-0.2.8/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_plotting.py` & `pyhalo-0.2.8/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_preset_models.py` & `pyhalo-0.2.8/tests/test_preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_pyhalo_base.py` & `pyhalo-0.2.8/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_realization_extensions.py` & `pyhalo-0.2.8/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.8/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_los.py` & `pyhalo-0.2.8/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_mass_functions/test_stucker.py` & `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_stucker.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_population.py` & `pyhalo-0.2.8/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.8/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_single_realization.py` & `pyhalo-0.2.8/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.7/tests/test_utilities.py` & `pyhalo-0.2.8/tests/test_utilities.py`

 * *Files identical despite different names*

