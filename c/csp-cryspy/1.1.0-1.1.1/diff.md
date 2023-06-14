# Comparing `tmp/csp-cryspy-1.1.0.tar.gz` & `tmp/csp-cryspy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csp-cryspy-1.1.0.tar", last modified: Tue May 16 08:22:18 2023, max compression
+gzip compressed data, was "csp-cryspy-1.1.1.tar", last modified: Wed Jun 14 14:14:14 2023, max compression
```

## Comparing `csp-cryspy-1.1.0.tar` & `csp-cryspy-1.1.1.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.084537 csp-cryspy-1.1.0/
--rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp-cryspy-1.1.0/LICENSE
--rw-r--r--   0 yamashita06   (501) staff       (20)     5562 2023-05-16 08:22:18.084063 csp-cryspy-1.1.0/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     3656 2023-05-16 07:49:41.000000 csp-cryspy-1.1.0/README.md
--rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp-cryspy-1.1.0/pyproject.toml
--rw-r--r--   0 yamashita06   (501) staff       (20)       38 2023-05-16 08:22:18.084663 csp-cryspy-1.1.0/setup.cfg
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.031596 csp-cryspy-1.1.0/src/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.032798 csp-cryspy-1.1.0/src/cryspy/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.037816 csp-cryspy-1.1.0/src/cryspy/BO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2580 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/bo_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6772 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/bo_next_select.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/bo_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4804 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/combo_cryspy.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      688 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/select_descriptor.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.040631 csp-cryspy-1.1.0/src/cryspy/EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3995 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_append.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4870 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_child.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2262 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4765 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_next_gen.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.045247 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    29426 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/crossover.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8526 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/ea_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8533 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/permutation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2858 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/rotation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/select_parents.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/strain.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.048476 csp-cryspy-1.1.0/src/cryspy/IO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/change_input.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1825 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/io_stat.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5567 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/out_results.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4842 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/pkl_data.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    70193 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/IO/read_input.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.050866 csp-cryspy-1.1.0/src/cryspy/LAQA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/calc_score.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1394 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1872 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_next_selection.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1049 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_restart.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.052849 csp-cryspy-1.1.0/src/cryspy/RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.054808 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    28668 2023-04-20 07:19:24.000000 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    19060 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/random_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/rs_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/rs_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.055387 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.056737 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/
--rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3401 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/calc_FP.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.058093 csp-cryspy-1.1.0/src/cryspy/interface/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.059373 csp-cryspy-1.1.0/src/cryspy/interface/ASE/
--rw-r--r--   0 yamashita06   (501) staff       (20)      684 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/ASE/calc_files_ase.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1065 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/ASE/collect_ase.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1915 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/ASE/ctrl_job_ase.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.061995 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      855 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1442 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/collect_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2112 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2859 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.064739 csp-cryspy-1.1.0/src/cryspy/interface/OMX/
--rw-r--r--   0 yamashita06   (501) staff       (20)      752 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/calc_files_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2679 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/collect_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3954 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/ctrl_job_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3119 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.067875 csp-cryspy-1.1.0/src/cryspy/interface/QE/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      703 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/calc_files_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    11215 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/collect_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3856 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/ctrl_job_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2884 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.070543 csp-cryspy-1.1.0/src/cryspy/interface/VASP/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      661 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/calc_files_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9063 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/collect_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3603 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/ctrl_job_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.071927 csp-cryspy-1.1.0/src/cryspy/interface/ext/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/ext/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      428 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/ext/collect_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7127 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/select_code.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.075159 csp-cryspy-1.1.0/src/cryspy/interface/soiap/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      705 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/calc_files_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7477 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/collect_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2173 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/ctrl_job_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2415 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.076857 csp-cryspy-1.1.0/src/cryspy/job/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/job/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    12290 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/job/ctrl_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    30848 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/job/ctrl_job.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.077736 csp-cryspy-1.1.0/src/cryspy/scripts/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/scripts/__init__.py
--rwxr-xr-x   0 yamashita06   (501) staff       (20)     4166 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/scripts/cryspy.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.079384 csp-cryspy-1.1.0/src/cryspy/start/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/start/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5317 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/start/cryspy_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4565 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/start/cryspy_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6664 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/start/gen_init_struc.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.080781 csp-cryspy-1.1.0/src/cryspy/util/
--rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/util/constants.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    15584 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/util/struc_util.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2581 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/util/utility.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.083496 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/
--rw-r--r--   0 yamashita06   (501) staff       (20)     5562 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     3106 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/SOURCES.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/dependency_links.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)       54 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/entry_points.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)       14 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/requires.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)        7 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/top_level.txt
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.989115 csp-cryspy-1.1.1/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp-cryspy-1.1.1/LICENSE
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5616 2023-06-14 14:14:14.988944 csp-cryspy-1.1.1/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3710 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/README.md
+-rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp-cryspy-1.1.1/pyproject.toml
+-rw-r--r--   0 yamashita06   (501) staff       (20)       38 2023-06-14 14:14:14.989160 csp-cryspy-1.1.1/setup.cfg
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.959743 csp-cryspy-1.1.1/src/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.960466 csp-cryspy-1.1.1/src/cryspy/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.962583 csp-cryspy-1.1.1/src/cryspy/BO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2580 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/bo_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6772 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/bo_next_select.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/bo_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4804 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/combo_cryspy.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      688 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/select_descriptor.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.964382 csp-cryspy-1.1.1/src/cryspy/EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3995 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_append.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4870 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_child.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2262 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4765 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_next_gen.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.966935 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    29426 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/crossover.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8526 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/ea_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8533 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/permutation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2858 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/rotation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/select_parents.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/strain.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.968855 csp-cryspy-1.1.1/src/cryspy/IO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/change_input.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1888 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/IO/io_stat.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5567 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/out_results.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4842 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/pkl_data.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    70148 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/IO/read_input.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.970708 csp-cryspy-1.1.1/src/cryspy/LAQA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/calc_score.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1394 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1872 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_next_selection.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1049 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_restart.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.972673 csp-cryspy-1.1.1/src/cryspy/RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.973703 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    28135 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    19060 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/random_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/rs_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/rs_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.974197 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.974953 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3401 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/calc_FP.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.975363 csp-cryspy-1.1.1/src/cryspy/interactive/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/interactive/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.975901 csp-cryspy-1.1.1/src/cryspy/interface/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.976673 csp-cryspy-1.1.1/src/cryspy/interface/ASE/
+-rw-------   0 yamashita06   (501) staff       (20)      684 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/ASE/calc_files_ase.py
+-rw-------   0 yamashita06   (501) staff       (20)     1065 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/ASE/collect_ase.py
+-rw-------   0 yamashita06   (501) staff       (20)     1915 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/ASE/ctrl_job_ase.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.978471 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      855 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/calc_files_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1442 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/collect_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2112 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2859 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.979864 csp-cryspy-1.1.1/src/cryspy/interface/OMX/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      752 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/calc_files_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2679 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/collect_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3954 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/ctrl_job_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3119 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.981396 csp-cryspy-1.1.1/src/cryspy/interface/QE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      703 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/calc_files_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    11215 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/collect_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3856 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/ctrl_job_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2884 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.982743 csp-cryspy-1.1.1/src/cryspy/interface/VASP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      661 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/calc_files_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9063 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/collect_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3603 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/ctrl_job_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.983417 csp-cryspy-1.1.1/src/cryspy/interface/ext/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/ext/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      428 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/ext/collect_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7127 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/select_code.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.984951 csp-cryspy-1.1.1/src/cryspy/interface/soiap/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      705 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/calc_files_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7477 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/collect_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2173 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/ctrl_job_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2415 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.985802 csp-cryspy-1.1.1/src/cryspy/job/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/job/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    12290 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/job/ctrl_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    30846 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/job/ctrl_job.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.986196 csp-cryspy-1.1.1/src/cryspy/scripts/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/scripts/__init__.py
+-rwx------   0 yamashita06   (501) staff       (20)     4166 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/scripts/cryspy.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.987085 csp-cryspy-1.1.1/src/cryspy/start/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/start/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5316 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/start/cryspy_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4565 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/start/cryspy_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6672 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/start/gen_init_struc.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.987862 csp-cryspy-1.1.1/src/cryspy/util/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/util/constants.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    15584 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/util/struc_util.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2581 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/util/utility.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.988728 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/
+-rw-------   0 yamashita06   (501) staff       (20)     5616 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/PKG-INFO
+-rw-------   0 yamashita06   (501) staff       (20)     3141 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/SOURCES.txt
+-rw-------   0 yamashita06   (501) staff       (20)        1 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/dependency_links.txt
+-rw-------   0 yamashita06   (501) staff       (20)       54 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/entry_points.txt
+-rw-------   0 yamashita06   (501) staff       (20)       14 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/requires.txt
+-rw-------   0 yamashita06   (501) staff       (20)        7 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/top_level.txt
```

### Comparing `csp-cryspy-1.1.0/LICENSE` & `csp-cryspy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/PKG-INFO` & `csp-cryspy-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.1.0
+Version: 1.1.1
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -42,17 +42,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.1.0 (2023 May 16)
+version 1.1.1 (2023 June 14)
 
 ## News
+- [2023 June 14] CrySPY 1.1.1 released
+    + bug fix
 - [2023 May 16] CrySPY 1.1.0 released
     + MPI parallelization (optional)
     + New score of LAQA
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
     + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
```

### Comparing `csp-cryspy-1.1.0/README.md` & `csp-cryspy-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.1.0 (2023 May 16)
+version 1.1.1 (2023 June 14)
 
 ## News
+- [2023 June 14] CrySPY 1.1.1 released
+    + bug fix
 - [2023 May 16] CrySPY 1.1.0 released
     + MPI parallelization (optional)
     + New score of LAQA
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
     + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
```

### Comparing `csp-cryspy-1.1.0/pyproject.toml` & `csp-cryspy-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/BO/bo_init.py` & `csp-cryspy-1.1.1/src/cryspy/BO/bo_init.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/BO/bo_next_select.py` & `csp-cryspy-1.1.1/src/cryspy/BO/bo_next_select.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/BO/bo_restart.py` & `csp-cryspy-1.1.1/src/cryspy/BO/bo_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/BO/combo_cryspy.py` & `csp-cryspy-1.1.1/src/cryspy/BO/combo_cryspy.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/BO/select_descriptor.py` & `csp-cryspy-1.1.1/src/cryspy/BO/select_descriptor.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/ea_append.py` & `csp-cryspy-1.1.1/src/cryspy/EA/ea_append.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/ea_child.py` & `csp-cryspy-1.1.1/src/cryspy/EA/ea_child.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/ea_init.py` & `csp-cryspy-1.1.1/src/cryspy/EA/ea_init.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/ea_next_gen.py` & `csp-cryspy-1.1.1/src/cryspy/EA/ea_next_gen.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/crossover.py` & `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/crossover.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/ea_generation.py` & `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/ea_generation.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/permutation.py` & `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/permutation.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/rotation.py` & `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/rotation.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/select_parents.py` & `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/select_parents.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/strain.py` & `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/strain.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/IO/io_stat.py` & `csp-cryspy-1.1.1/src/cryspy/IO/io_stat.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         stat.add_section('QE')
     if rin.calc_code == 'soiap':
         stat.add_section('soiap')
     if rin.calc_code == 'LAMMPS':
         stat.add_section('LAMMPS')
     if rin.calc_code == 'OMX':
         stat.add_section('OMX')
+    if rin.calc_code == 'ASE':
+        stat.add_section('ASE')
     # ----------
     stat.add_section('option')
     stat.add_section('status')
     return stat
 
 
 def stat_read():
```

### Comparing `csp-cryspy-1.1.0/src/cryspy/IO/out_results.py` & `csp-cryspy-1.1.1/src/cryspy/IO/out_results.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/IO/pkl_data.py` & `csp-cryspy-1.1.1/src/cryspy/IO/pkl_data.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/IO/read_input.py` & `csp-cryspy-1.1.1/src/cryspy/IO/read_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,18 +678,17 @@
         force_gamma = False
 
     # ---------- ase
     elif calc_code == 'ASE':
         # ------ global declaration
         global ase_python
         # ------ read input variables
-        try:
-            ase_python = config.get('ASE', 'ase_python')
-        except configparser.NoOptionError:
-            ase_python = 'ase.py'
+        ase_python = config.get('ASE', 'ase_python')
+        kpt_flag = False
+        force_gamma = False
 
     # ---------- ext
     elif calc_code == 'ext':
         kpt_flag = False
 
 
 def _spglist(spgnum):
@@ -870,15 +869,15 @@
             stat.set('LAMMPS', 'lammps_potential',
                      '{}'.format(' '.join(lammps_potential)))
         stat.set('LAMMPS', 'lammps_data', '{}'.format(lammps_data))
 
     # ---------- ASE
     if calc_code == 'ASE':
         stat.set('ASE', 'ase_python', '{}'.format(ase_python))
-    
+
     # ---------- option
     stat.set('option', 'stop_chkpt', '{}'.format(stop_chkpt))
     stat.set('option', 'load_struc_flag', '{}'.format(load_struc_flag))
     stat.set('option', 'stop_next_struc', '{}'.format(stop_next_struc))
     stat.set('option', 'recalc', '{}'.format(' '.join(str(x) for x in recalc)))
     stat.set('option', 'append_struc_ea', '{}'.format(append_struc_ea))
     stat.set('option', 'energy_step_flag', '{}'.format(energy_step_flag))
```

### Comparing `csp-cryspy-1.1.0/src/cryspy/LAQA/calc_score.py` & `csp-cryspy-1.1.1/src/cryspy/LAQA/calc_score.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_init.py` & `csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_init.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_next_selection.py` & `csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_next_selection.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_restart.py` & `csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py` & `csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 class Rnd_struc_gen_pyxtal:
     '''
     Random structure generation using pyxtal
     '''
 
     def __init__(self, mindist):
         self.mindist = mindist
-        self.spg_error = []
 
     def set_mol(self):
         '''
         set molecule files and number of molecules
         '''
         # ----------
         mol_data = []
@@ -76,28 +75,25 @@
         # ---------- loop for structure generattion
         while len(self.init_struc_data) < nstruc:
             # ------ spgnum --> spg
             if rin.spgnum == 'all':
                 spg = random.randint(1, 230)
             else:
                 spg = random.choice(rin.spgnum)
-            if spg in self.spg_error:
-                continue
             # ------ vol_factor
             rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
             # ------ generate structure
             tmp_crystal = pyxtal()
             try:
                 with redirect_stdout(sys.stderr):
                     tmp_crystal.from_random(dim=3, group=spg, species=rin.atype,
                                             numIons=rin.nat, factor=rand_vol,
                                             conventional=False, tm=tolmat)
             except Exception as e:
                 print(e, ':spg = {} retry.'.format(spg), file=sys.stderr, flush=True)
-                self.spg_error.append(spg)
                 continue
             if tmp_crystal.valid:
                 tmp_struc = tmp_crystal.to_pymatgen(resort=False)    # pymatgen Structure format
                 # -- check the number of atoms
                 if not self._check_nat(tmp_struc):
                     # (pyxtal 0.1.4) cryspy adopts "conventional=False",
                     #     which is better for DFT calculation
@@ -138,16 +134,14 @@
                 self.init_struc_data[cid] = tmp_struc
                 print('Structure ID {0:>6} was generated.'
                       ' Space group: {1:>3} --> {2:>3} {3}'.format(
                        cid, spg, spg_num, spg_sym), flush=True)
                 # -- save init_POSCARS
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
-            else:
-                self.spg_error.append(spg)
 
     def gen_struc_mol(self, nstruc, id_offset=0, init_pos_path=None):
         '''
         Generate random molecular crystal structures for given space groups
         one have to run self.set_mol() in advance
         # ---------- args
         nstruc (int): number of generated structures
@@ -184,16 +178,14 @@
         # ---------- loop for structure generattion
         while len(self.init_struc_data) < nstruc:
             # ------ spgnum --> spg
             if rin.spgnum == 'all':
                 spg = random.randint(1, 230)
             else:
                 spg = random.choice(rin.spgnum)
-            if spg in self.spg_error:
-                continue
             rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
             # ------ generate structure
             # -- multiprocess for measures against hangup
             q = Queue()
             p = Process(target=self._mp_mc, args=(tolmat, spg, rin.nmol, rand_vol, q, rin.algo))
             p.start()
             p.join(timeout=rin.timeout_mol)
@@ -215,15 +207,14 @@
                     dums = tmp_q[1]         # dummy element
                     in_dists = tmp_q[2]     # interatomic distance in a molecule
                     mol_dists = tmp_q[3]    # distance between molecules
                 else:
                     tmp_struc = q.get()
                 tmp_valid = q.get()
                 if tmp_struc == 'error':
-                    self.spg_error.append(spg)
                     continue
             if tmp_valid:
                 # -- scale volume
                 if rin.vol_mu is not None:
                     vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
                     vol = vol * tmp_struc.num_sites / rin.natot    # for conv. cell
                     tmp_struc = scale_cell_mol(tmp_struc, self.mol_data, vol)
@@ -315,16 +306,14 @@
                     self.struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
                 print('Structure ID {0:>6} was generated.'
                       ' Space group: {1:>3} --> {2:>3} {3}'.format(
                        cid, spg, spg_num, spg_sym), flush=True)
                 # -- save init_POSCARS
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
-            else:
-                self.spg_error.append(spg)
 
     def gen_struc_mol_break_sym(self, nstruc, mindist_dummy,
                                 id_offset=0, init_pos_path=None):
         '''
         Generate random molecular crystal structures
         one have to run self.set_mol() in advance
         molecules are put a Wyckoff position without consideration of symmetry
@@ -368,28 +357,25 @@
         # ---------- loop for structure generattion
         while len(self.init_struc_data) < nstruc:
             # ------ spgnum --> spg
             if rin.spgnum == 'all':
                 spg = random.randint(1, 230)
             else:
                 spg = random.choice(rin.spgnum)
-            if spg in self.spg_error:
-                continue
             # ------ vol_factor
             rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
             # ------ generate structure
             tmp_crystal = pyxtal()
             try:
                 with redirect_stdout(sys.stderr):
                     tmp_crystal.from_random(dim=3, group=spg, species=atype_dummy,
                                             numIons=rin.nmol, factor=rand_vol,
                                             conventional=False, tm=tolmat)
             except Exception as e:
                 print(e, ':spg = {} retry.'.format(spg), file=sys.stderr, flush=True)
-                self.spg_error.append(spg)
                 continue
             if tmp_crystal.valid:
                 # -- each wyckoff position --> dummy atom
                 dums = []        # dummy atoms
                 dum_pos = []     # internal position of dummy
                 dum_type = {}    # type of dummy
                                  #  e.g. {DummySpecie X00+: 'Rn',
@@ -515,16 +501,14 @@
                     self.struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
                 print('Structure ID {0:>6} was generated.'
                       ' Space group: {1:>3} --> {2:>3} {3}'.format(
                        cid, spg, spg_num, spg_sym), flush=True)
                 # -- save init_POSCARS
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
-            else:
-                self.spg_error.append(spg)
 
     def _set_tol_mat(self, atype, mindist):
         tolmat = Tol_matrix()
         for i, itype in enumerate(atype):
             for j, jtype in enumerate(atype):
                 if i <= j:
                     tolmat.set_tol(itype, jtype, mindist[i][j])
```

### Comparing `csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/random_generation.py` & `csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/random_generation.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/RS/rs_restart.py` & `csp-cryspy-1.1.1/src/cryspy/RS/rs_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/calc_FP.py` & `csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/calc_FP.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/ASE/calc_files_ase.py` & `csp-cryspy-1.1.1/src/cryspy/interface/ASE/calc_files_ase.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/ASE/collect_ase.py` & `csp-cryspy-1.1.1/src/cryspy/interface/ASE/collect_ase.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/ASE/ctrl_job_ase.py` & `csp-cryspy-1.1.1/src/cryspy/interface/ASE/ctrl_job_ase.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py` & `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/calc_files_lammps.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/collect_lammps.py` & `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/collect_lammps.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py` & `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/structure.py` & `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/OMX/calc_files_OMX.py` & `csp-cryspy-1.1.1/src/cryspy/interface/OMX/calc_files_OMX.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/OMX/collect_OMX.py` & `csp-cryspy-1.1.1/src/cryspy/interface/OMX/collect_OMX.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/OMX/ctrl_job_OMX.py` & `csp-cryspy-1.1.1/src/cryspy/interface/OMX/ctrl_job_OMX.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/OMX/structure.py` & `csp-cryspy-1.1.1/src/cryspy/interface/OMX/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/QE/calc_files_qe.py` & `csp-cryspy-1.1.1/src/cryspy/interface/QE/calc_files_qe.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/QE/collect_qe.py` & `csp-cryspy-1.1.1/src/cryspy/interface/QE/collect_qe.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/QE/ctrl_job_qe.py` & `csp-cryspy-1.1.1/src/cryspy/interface/QE/ctrl_job_qe.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/QE/structure.py` & `csp-cryspy-1.1.1/src/cryspy/interface/QE/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/VASP/calc_files_vasp.py` & `csp-cryspy-1.1.1/src/cryspy/interface/VASP/calc_files_vasp.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/VASP/collect_vasp.py` & `csp-cryspy-1.1.1/src/cryspy/interface/VASP/collect_vasp.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/VASP/ctrl_job_vasp.py` & `csp-cryspy-1.1.1/src/cryspy/interface/VASP/ctrl_job_vasp.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/select_code.py` & `csp-cryspy-1.1.1/src/cryspy/interface/select_code.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/soiap/calc_files_soiap.py` & `csp-cryspy-1.1.1/src/cryspy/interface/soiap/calc_files_soiap.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/soiap/collect_soiap.py` & `csp-cryspy-1.1.1/src/cryspy/interface/soiap/collect_soiap.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/soiap/ctrl_job_soiap.py` & `csp-cryspy-1.1.1/src/cryspy/interface/soiap/ctrl_job_soiap.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/interface/soiap/structure.py` & `csp-cryspy-1.1.1/src/cryspy/interface/soiap/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/job/ctrl_ext.py` & `csp-cryspy-1.1.1/src/cryspy/job/ctrl_ext.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/job/ctrl_job.py` & `csp-cryspy-1.1.1/src/cryspy/job/ctrl_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,15 +631,15 @@
         # ---------- check point 3
         if rin.stop_chkpt == 3:
             print('Stop at check point 3: BO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- max_select_bo
         if 0 < rin.max_select_bo <= self.n_selection:
-            print('Reached max_select_bo: {}\n'.format(rin.max_select_bo))
+            print('Reached max_select_bo: {}'.format(rin.max_select_bo))
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- BO
         backup_cryspy()
         bo_data = (self.init_dscrpt_data, self.opt_dscrpt_data,
                    self.bo_mean, self.bo_var, self.bo_score)
         bo_id_data = (self.n_selection, self.id_queueing,
```

### Comparing `csp-cryspy-1.1.0/src/cryspy/scripts/cryspy.py` & `csp-cryspy-1.1.1/src/cryspy/scripts/cryspy.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/start/cryspy_init.py` & `csp-cryspy-1.1.1/src/cryspy/start/cryspy_init.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,8 @@
             stress_step_data = {}
             pkl_data.save_stress_step(stress_step_data)
 
         # ---------- for ext
         if rin.calc_code == 'ext':
             os.makedirs('ext', exist_ok=True)
             with open('ext/stat_job', 'w') as fstat:
-                fstat.write('out\n')
+                fstat.write('out\n')
```

### Comparing `csp-cryspy-1.1.0/src/cryspy/start/cryspy_restart.py` & `csp-cryspy-1.1.1/src/cryspy/start/cryspy_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/start/gen_init_struc.py` & `csp-cryspy-1.1.1/src/cryspy/start/gen_init_struc.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # ---------- mindist
     if mpi_rank == 0:
         print('# ------ mindist', flush=True)
     if mpi_size > 1:
         comm.barrier()
     mindist = set_mindist(rin.mindist, rin.mindist_factor, False, mpi_rank)
 
-    # ---------- nstruc, offset
+    # ---------- nstruc, offset for MPI
     nstruc_list, offset_list = _divide_task(rin.tot_struc, mpi_size, len(init_struc_data))
 
     # ---------- pyxtal
     if not (rin.spgnum == 0 or rin.use_find_wy):
         from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
         rsgx = Rnd_struc_gen_pyxtal(mindist=mindist)
         # ------ crystal
```

### Comparing `csp-cryspy-1.1.0/src/cryspy/util/struc_util.py` & `csp-cryspy-1.1.1/src/cryspy/util/struc_util.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.0/src/cryspy/util/utility.py` & `csp-cryspy-1.1.1/src/cryspy/util/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import shutil
 import subprocess
 
 
 # ---------- functions
 def get_version():
-    return '1.1.0'
+    return '1.1.1'
 
 
 def get_date():
     return datetime.now().strftime("%Y/%m/%d %H:%M:%S")
 
 
 def check_fwpath(fwpath):
```

### Comparing `csp-cryspy-1.1.0/src/csp_cryspy.egg-info/PKG-INFO` & `csp-cryspy-1.1.1/src/csp_cryspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.1.0
+Version: 1.1.1
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -42,17 +42,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.1.0 (2023 May 16)
+version 1.1.1 (2023 June 14)
 
 ## News
+- [2023 June 14] CrySPY 1.1.1 released
+    + bug fix
 - [2023 May 16] CrySPY 1.1.0 released
     + MPI parallelization (optional)
     + New score of LAQA
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
     + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
```

### Comparing `csp-cryspy-1.1.0/src/csp_cryspy.egg-info/SOURCES.txt` & `csp-cryspy-1.1.1/src/csp_cryspy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/cryspy/RS/rs_restart.py
 src/cryspy/RS/gen_struc_RS/__init__.py
 src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
 src/cryspy/RS/gen_struc_RS/random_generation.py
 src/cryspy/calc_dscrpt/__init__.py
 src/cryspy/calc_dscrpt/FP/__init__.py
 src/cryspy/calc_dscrpt/FP/calc_FP.py
+src/cryspy/interactive/__init__.py
 src/cryspy/interface/__init__.py
 src/cryspy/interface/select_code.py
 src/cryspy/interface/ASE/calc_files_ase.py
 src/cryspy/interface/ASE/collect_ase.py
 src/cryspy/interface/ASE/ctrl_job_ase.py
 src/cryspy/interface/LAMMPS/__init__.py
 src/cryspy/interface/LAMMPS/calc_files_lammps.py
```

