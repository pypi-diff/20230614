# Comparing `tmp/nanoqnt-0.2.0rc2.tar.gz` & `tmp/nanoqnt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoqnt-0.2.0rc2.tar", max compression
+gzip compressed data, was "nanoqnt-0.2.1.tar", max compression
```

## Comparing `nanoqnt-0.2.0rc2.tar` & `nanoqnt-0.2.1.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0       43 2023-06-12 12:02:24.897116 nanoqnt-0.2.0rc2/README.md
--rw-r--r--   0        0        0        0 2023-01-02 14:34:22.063965 nanoqnt-0.2.0rc2/nanoqnt/__init__.py
--rw-r--r--   0        0        0     4154 2023-06-12 12:02:24.898367 nanoqnt-0.2.0rc2/nanoqnt/dispertech-logo.ico
--rw-r--r--   0        0        0      820 2023-06-12 12:02:24.899141 nanoqnt-0.2.0rc2/nanoqnt/main.py
--rw-r--r--   0        0        0        0 2022-12-20 12:52:00.514018 nanoqnt-0.2.0rc2/nanoqnt/model/__init__.py
--rw-r--r--   0        0        0    13247 2023-06-12 12:02:24.899813 nanoqnt-0.2.0rc2/nanoqnt/model/analyze_nanoqnt.py
--rw-r--r--   0        0        0      280 2023-06-12 12:02:24.900270 nanoqnt-0.2.0rc2/nanoqnt/model/decorators.py
--rw-r--r--   0        0        0       34 2023-06-12 12:02:24.900680 nanoqnt-0.2.0rc2/nanoqnt/model/exceptions.py
--rw-r--r--   0        0        0      385 2023-06-12 12:02:24.901046 nanoqnt-0.2.0rc2/nanoqnt/stage_main.py
--rw-r--r--   0        0        0      351 2023-06-12 12:02:24.901498 nanoqnt-0.2.0rc2/nanoqnt/util/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-12 12:02:24.901860 nanoqnt-0.2.0rc2/nanoqnt/util/make_hdf5.py
--rw-r--r--   0        0        0     3759 2022-03-16 14:59:30.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
--rw-r--r--   0        0        0     4715 2022-03-16 14:59:22.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11814 - Atom.svg
--rw-r--r--   0        0        0     3727 2022-03-16 14:59:14.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11815 - Battery.svg
--rw-r--r--   0        0        0     5275 2022-03-16 14:59:06.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
--rw-r--r--   0        0        0     2802 2022-03-16 14:58:58.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
--rw-r--r--   0        0        0     4637 2022-03-16 14:58:50.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
--rw-r--r--   0        0        0     1936 2022-03-16 14:58:44.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
--rw-r--r--   0        0        0     2442 2022-03-16 14:58:36.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
--rw-r--r--   0        0        0     2191 2022-03-16 14:58:28.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
--rw-r--r--   0        0        0     2594 2022-03-16 14:58:22.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11822 - Collision.svg
--rw-r--r--   0        0        0     2347 2022-03-16 14:58:14.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
--rw-r--r--   0        0        0     2347 2022-03-16 14:58:04.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
--rw-r--r--   0        0        0     2710 2022-03-16 14:57:56.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
--rw-r--r--   0        0        0     3426 2022-03-16 15:19:36.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
--rw-r--r--   0        0        0     3508 2022-03-16 14:57:38.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
--rw-r--r--   0        0        0     3527 2022-03-16 14:57:30.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11828 - Energy.svg
--rw-r--r--   0        0        0     1821 2022-03-16 14:57:22.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11829 - Flask.svg
--rw-r--r--   0        0        0     4901 2022-03-16 14:57:14.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11830 - Float.svg
--rw-r--r--   0        0        0     1522 2022-03-16 14:57:06.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
--rw-r--r--   0        0        0     8697 2022-03-16 14:56:58.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11832 - Force.svg
--rw-r--r--   0        0        0     3310 2022-03-16 14:56:48.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11833 - Formula.svg
--rw-r--r--   0        0        0     2416 2022-03-16 14:56:40.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11834 - Gears.svg
--rw-r--r--   0        0        0     4479 2022-03-16 14:56:32.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
--rw-r--r--   0        0        0     4165 2022-03-16 14:56:24.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
--rw-r--r--   0        0        0     3653 2022-03-16 14:56:16.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
--rw-r--r--   0        0        0     2013 2022-03-16 14:56:08.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
--rw-r--r--   0        0        0     2576 2022-03-16 14:56:00.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
--rw-r--r--   0        0        0     5579 2022-03-16 14:55:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
--rw-r--r--   0        0        0     3646 2022-03-16 14:55:46.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
--rw-r--r--   0        0        0     1706 2022-03-16 14:55:38.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
--rw-r--r--   0        0        0     3307 2022-03-16 14:55:32.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
--rw-r--r--   0        0        0     2707 2022-03-16 14:55:24.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11844 - Motion.svg
--rw-r--r--   0        0        0     1163 2022-03-16 14:55:18.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
--rw-r--r--   0        0        0     5179 2022-03-16 14:55:10.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
--rw-r--r--   0        0        0     2264 2022-03-16 14:55:02.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
--rw-r--r--   0        0        0     4868 2022-03-16 14:54:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11848 - Planet.svg
--rw-r--r--   0        0        0     9381 2022-03-16 14:54:44.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
--rw-r--r--   0        0        0      806 2022-03-16 14:54:36.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11850 - Power.svg
--rw-r--r--   0        0        0     2581 2022-03-16 14:54:28.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11851 - Press.svg
--rw-r--r--   0        0        0     3090 2022-03-16 14:54:20.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11852 - Proton.svg
--rw-r--r--   0        0        0     2528 2022-03-16 14:54:12.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
--rw-r--r--   0        0        0     4144 2022-03-16 14:54:04.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
--rw-r--r--   0        0        0     3109 2022-03-16 14:53:56.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
--rw-r--r--   0        0        0     2481 2022-03-16 14:53:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
--rw-r--r--   0        0        0     3390 2022-03-16 14:53:52.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
--rw-r--r--   0        0        0     2463 2022-03-16 14:53:50.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
--rw-r--r--   0        0        0     2156 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
--rw-r--r--   0        0        0     2552 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
--rw-r--r--   0        0        0     2816 2022-03-16 15:41:46.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11861 - Waves.svg
--rw-r--r--   0        0        0     3799 2022-03-16 14:53:44.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
--rw-r--r--   0        0        0       43 2022-12-20 12:57:18.786580 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Icons.qrc
--rw-r--r--   0        0        0      342 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Open Folder.svg
--rw-r--r--   0        0        0      559 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Save.svg
--rw-r--r--   0        0        0      215 2020-07-27 20:54:42.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/open.svg
--rw-r--r--   0        0        0     2193 2023-06-12 12:02:24.902373 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/channel_selector.ui
--rw-r--r--   0        0        0    14859 2023-06-12 12:02:24.902919 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/data_exploration.ui
--rw-r--r--   0        0        0     5564 2023-06-12 12:02:24.903391 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/particles_widget.ui
--rw-r--r--   0        0        0     3367 2023-01-26 21:32:32.021169 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/scan_control.ui
--rw-r--r--   0        0        0       62 2023-06-12 12:02:24.903693 nanoqnt-0.2.0rc2/nanoqnt/view/__init__.py
--rw-r--r--   0        0        0      848 2023-06-12 12:02:24.903942 nanoqnt-0.2.0rc2/nanoqnt/view/channel_selector.py
--rw-r--r--   0        0        0    11311 2023-06-12 12:02:24.904324 nanoqnt-0.2.0rc2/nanoqnt/view/main_window.py
--rw-r--r--   0        0        0     1947 2023-06-12 12:02:24.904552 nanoqnt-0.2.0rc2/nanoqnt/view/particle_widget.py
--rw-r--r--   0        0        0     1359 2023-06-12 12:02:24.904821 nanoqnt-0.2.0rc2/nanoqnt/view/stage_control.py
--rw-r--r--   0        0        0      515 2023-06-12 12:29:11.995279 nanoqnt-0.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 nanoqnt-0.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-06-14 12:31:39.675046 nanoqnt-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0      648 2023-06-14 14:20:59.156275 nanoqnt-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-01-02 14:34:22.063965 nanoqnt-0.2.1/nanoqnt/__init__.py
+-rw-r--r--   0        0        0     4154 2023-06-12 12:02:24.898367 nanoqnt-0.2.1/nanoqnt/dispertech-logo.ico
+-rw-r--r--   0        0        0     1189 2023-06-14 13:42:06.609945 nanoqnt-0.2.1/nanoqnt/main.py
+-rw-r--r--   0        0        0        0 2022-12-20 12:52:00.514018 nanoqnt-0.2.1/nanoqnt/model/__init__.py
+-rw-r--r--   0        0        0    15541 2023-06-14 14:52:26.989817 nanoqnt-0.2.1/nanoqnt/model/analyze_nanoqnt.py
+-rw-r--r--   0        0        0      280 2023-06-12 12:02:24.900270 nanoqnt-0.2.1/nanoqnt/model/decorators.py
+-rw-r--r--   0        0        0       34 2023-06-12 12:02:24.900680 nanoqnt-0.2.1/nanoqnt/model/exceptions.py
+-rw-r--r--   0        0        0      385 2023-06-12 12:02:24.901046 nanoqnt-0.2.1/nanoqnt/stage_main.py
+-rw-r--r--   0        0        0      351 2023-06-12 12:02:24.901498 nanoqnt-0.2.1/nanoqnt/util/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-12 12:02:24.901860 nanoqnt-0.2.1/nanoqnt/util/make_hdf5.py
+-rw-r--r--   0        0        0     3759 2022-03-16 14:59:30.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
+-rw-r--r--   0        0        0     4715 2022-03-16 14:59:22.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11814 - Atom.svg
+-rw-r--r--   0        0        0     3727 2022-03-16 14:59:14.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11815 - Battery.svg
+-rw-r--r--   0        0        0     5275 2022-03-16 14:59:06.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
+-rw-r--r--   0        0        0     2802 2022-03-16 14:58:58.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
+-rw-r--r--   0        0        0     4637 2022-03-16 14:58:50.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
+-rw-r--r--   0        0        0     1936 2022-03-16 14:58:44.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
+-rw-r--r--   0        0        0     2442 2022-03-16 14:58:36.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
+-rw-r--r--   0        0        0     2191 2022-03-16 14:58:28.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
+-rw-r--r--   0        0        0     2594 2022-03-16 14:58:22.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11822 - Collision.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:14.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:04.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
+-rw-r--r--   0        0        0     2710 2022-03-16 14:57:56.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
+-rw-r--r--   0        0        0     3426 2022-03-16 15:19:36.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
+-rw-r--r--   0        0        0     3508 2022-03-16 14:57:38.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
+-rw-r--r--   0        0        0     3527 2022-03-16 14:57:30.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11828 - Energy.svg
+-rw-r--r--   0        0        0     1821 2022-03-16 14:57:22.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11829 - Flask.svg
+-rw-r--r--   0        0        0     4901 2022-03-16 14:57:14.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11830 - Float.svg
+-rw-r--r--   0        0        0     1522 2022-03-16 14:57:06.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
+-rw-r--r--   0        0        0     8697 2022-03-16 14:56:58.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11832 - Force.svg
+-rw-r--r--   0        0        0     3310 2022-03-16 14:56:48.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11833 - Formula.svg
+-rw-r--r--   0        0        0     2416 2022-03-16 14:56:40.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11834 - Gears.svg
+-rw-r--r--   0        0        0     4479 2022-03-16 14:56:32.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
+-rw-r--r--   0        0        0     4165 2022-03-16 14:56:24.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
+-rw-r--r--   0        0        0     3653 2022-03-16 14:56:16.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
+-rw-r--r--   0        0        0     2013 2022-03-16 14:56:08.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
+-rw-r--r--   0        0        0     2576 2022-03-16 14:56:00.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
+-rw-r--r--   0        0        0     5579 2022-03-16 14:55:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
+-rw-r--r--   0        0        0     3646 2022-03-16 14:55:46.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
+-rw-r--r--   0        0        0     1706 2022-03-16 14:55:38.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
+-rw-r--r--   0        0        0     3307 2022-03-16 14:55:32.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
+-rw-r--r--   0        0        0     2707 2022-03-16 14:55:24.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11844 - Motion.svg
+-rw-r--r--   0        0        0     1163 2022-03-16 14:55:18.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
+-rw-r--r--   0        0        0     5179 2022-03-16 14:55:10.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
+-rw-r--r--   0        0        0     2264 2022-03-16 14:55:02.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
+-rw-r--r--   0        0        0     4868 2022-03-16 14:54:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11848 - Planet.svg
+-rw-r--r--   0        0        0     9381 2022-03-16 14:54:44.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
+-rw-r--r--   0        0        0      806 2022-03-16 14:54:36.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11850 - Power.svg
+-rw-r--r--   0        0        0     2581 2022-03-16 14:54:28.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11851 - Press.svg
+-rw-r--r--   0        0        0     3090 2022-03-16 14:54:20.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11852 - Proton.svg
+-rw-r--r--   0        0        0     2528 2022-03-16 14:54:12.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
+-rw-r--r--   0        0        0     4144 2022-03-16 14:54:04.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
+-rw-r--r--   0        0        0     3109 2022-03-16 14:53:56.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
+-rw-r--r--   0        0        0     2481 2022-03-16 14:53:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
+-rw-r--r--   0        0        0     3390 2022-03-16 14:53:52.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
+-rw-r--r--   0        0        0     2463 2022-03-16 14:53:50.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
+-rw-r--r--   0        0        0     2156 2022-03-16 14:53:48.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
+-rw-r--r--   0        0        0     2552 2022-03-16 14:53:48.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
+-rw-r--r--   0        0        0     2816 2022-03-16 15:41:46.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11861 - Waves.svg
+-rw-r--r--   0        0        0     3799 2022-03-16 14:53:44.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
+-rw-r--r--   0        0        0       43 2022-12-20 12:57:18.786580 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Icons.qrc
+-rw-r--r--   0        0        0      342 2022-11-15 12:55:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Open Folder.svg
+-rw-r--r--   0        0        0      559 2022-11-15 12:55:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Save.svg
+-rw-r--r--   0        0        0      215 2020-07-27 20:54:42.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/open.svg
+-rw-r--r--   0        0        0     2193 2023-06-12 12:02:24.902373 nanoqnt-0.2.1/nanoqnt/view/GUI/channel_selector.ui
+-rw-r--r--   0        0        0    14862 2023-06-14 14:24:59.072757 nanoqnt-0.2.1/nanoqnt/view/GUI/data_exploration.ui
+-rw-r--r--   0        0        0     5565 2023-06-14 14:20:12.278524 nanoqnt-0.2.1/nanoqnt/view/GUI/particles_widget.ui
+-rw-r--r--   0        0        0     3367 2023-01-26 21:32:32.021169 nanoqnt-0.2.1/nanoqnt/view/GUI/scan_control.ui
+-rw-r--r--   0        0        0       62 2023-06-12 12:02:24.903693 nanoqnt-0.2.1/nanoqnt/view/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-12 12:02:24.903942 nanoqnt-0.2.1/nanoqnt/view/channel_selector.py
+-rw-r--r--   0        0        0    11374 2023-06-14 14:56:09.181506 nanoqnt-0.2.1/nanoqnt/view/main_window.py
+-rw-r--r--   0        0        0     1947 2023-06-12 12:02:24.904552 nanoqnt-0.2.1/nanoqnt/view/particle_widget.py
+-rw-r--r--   0        0        0     1359 2023-06-12 12:02:24.904821 nanoqnt-0.2.1/nanoqnt/view/stage_control.py
+-rw-r--r--   0        0        0     1448 2023-06-14 14:57:22.497703 nanoqnt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 nanoqnt-0.2.1/PKG-INFO
```

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/dispertech-logo.ico` & `nanoqnt-0.2.1/nanoqnt/dispertech-logo.ico`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/model/analyze_nanoqnt.py` & `nanoqnt-0.2.1/nanoqnt/model/analyze_nanoqnt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import json
+import logging
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import pims as pims
-import skimage
 import trackpy as tp
 import yaml
 from scipy.spatial import KDTree
 from skimage import morphology
 from skimage.measure import label, regionprops_table
 from trackpy.find import where_close
 from trackpy.utils import pandas_concat
 
+logger = logging.getLogger(__name__)
+
 
 class AnalyzeNanoQNT:
     def __init__(self):
         self.filename = None
         self.data = None
         self.metadata = {}
         self.particle_df = []
         self.particles = pd.DataFrame()
         self.num_frames = 0
         self.find_settings = {}
         self.filename = Path.home()
-        self.concentration = 0  # pcles/ml
+        self.concentration = {}  # pcles/ml
         self.linked_particles = None
         self.total_num_particles = 0
         self.summarized_particles = None
 
         self.ignore_edge_pixels = 8
 
         self.num_channels = 1
         self.channels_data = {}
+        self.channels_names = []
         self.bkg = None
 
+
     def open(self, filename):
         """ Opens the file with the data. Normally a multi-tiff file, but it can be adapted to other formats.
         It also looks for the comments.txt file (create by uManager) in order to load some metadata
 
         :param filename: The full-path to the file to be opened
         """
         self.filename = Path(filename)
@@ -64,14 +68,15 @@
             self.metadata['uManager'] = {'comments': 'file not found'}
 
         try:
             comment = self.metadata['uManager']['map']['General annotation']['scalar']['comments']['scalar']
             start = comment.index('(') + 1
             end = comment.index(')')
             self.num_channels = len(comment[start:end].split(' '))
+            self.channels_names = [i for i in range(self.num_channels)]
         except:
             pass
 
     def find_particles(self, frame_num, diameter, minmass, method='mask'):
         """ Finds particles in a given frame and stores the data frame in a list indexed by the frame number.
 
         :param int frame_num: The number of the frame (0-indexed) to analyze
@@ -103,15 +108,15 @@
             df = pd.DataFrame(props).rename(columns={'centroid-0': 'y', 'centroid-1': 'x', 'intensity_mean': 'mass'})
             to_drop = where_close(df[['x', 'y']], separation=diameter * 2, intensity=df['mass'])
             df = df.drop(to_drop)
             df = df.loc[df['y'] >= self.ignore_edge_pixels]
             self.particle_df[frame_num] = df
             return df
 
-    def find_all_particles(self, frames_no, diameter, minmass, method='python'):
+    def find_all_particles(self, frames_no, diameter, minmass, method='numba'):
         """ Finds all the particles in a given range of frames. If the data has multiple channels, then it can handle
         different settings for each one. In that case, diameter and minmass must be iterables and in the appropriate
         order, i.e., the first setting will be for the first channel, etc.
 
         The data is structured as a dictionary, where each channel is a different key, and then the localizations are
         stored as a pandas dataframe.
 
@@ -151,28 +156,26 @@
                     real_frame = frame * self.num_channels + channel
                     df = self.find_particles(real_frame, diameter[channel], minmass[channel], method='mask')
                     df['frame'] = frame
                     all_features.append(df)
                 self.particles[channel] = pandas_concat(all_features).reset_index(drop=True)
             return self.particles
 
-        ## For the python or numba methods, only 1-channel data is available
-        if self.num_channels > 1:
-            raise Exception("Trackpy-based methods only work with 1-channel data for the time being")
-
-        self.particles[0] = tp.batch(self.data[frames_no[0]:frames_no[1]],
-                                     diameter[0],
-                                     minmass=minmass[0],
-                                     characterize=False,
-                                     preprocess=False,
-                                     processes='auto',
-                                     engine=method)
-        self.particles[0]['intensity'] = np.nan
-
-        return self.particles
+        for channel in range(self.num_channels):
+            data = np.array(self.data[frames_no[0] * self.num_channels + channel:frames_no[
+                                                                                     1] * self.num_channels + channel:self.num_channels])
+            data = [data[i, ...] for i in range(data.shape[0])]
+
+            self.particles[channel] = tp.batch(data,
+                                               diameter[channel],
+                                               minmass=minmass[channel],
+                                               characterize=False,
+                                               preprocess=False,
+                                               processes='auto',
+                                               engine=method)
 
     def link_particles(self, search_radius, memory=0, min_frames=0):
         self.linked_particles = {}
         for channel in range(self.num_channels):
             self.linked_particles[channel] = tp.link(self.particles[channel], search_radius, memory=memory)
             self.linked_particles[channel] = tp.filter_stubs(self.linked_particles[channel], min_frames)
 
@@ -182,22 +185,36 @@
             'memory': memory
             })
 
     def calculate_intensities(self):
         """Calculates the intensities of the linked particles assuming they were the product of the mask method.
         The methods that rely on the trackpy algorithm already include the intensity.
         """
+        self.summary_data = {}
+        intensity_columns = [f'i_{channel}' for channel in range(self.num_channels)]
+
+        if (engine := self.metadata.get('engine')) == 'python' or engine == 'numba':
+            logger.info('Using the trackpy intensities')
+            for channel in range(self.num_channels):
+                self.summary_data[channel] = self.linked_particles[channel].groupby('particle').mean()
+                self.summary_data[channel]['frame'] = self.summary_data[channel]['frame'].astype('int')
+                self.summary_data[channel]['x'] = self.summary_data[channel]['x'].astype('int')
+                self.summary_data[channel]['y'] = self.summary_data[channel]['y'].astype('int')
+                for colum in intensity_columns:
+                    self.summary_data[channel][colum] = np.nan
+                self.summary_data[channel][f'i_{channel}'] = self.summary_data[channel]['mass']
+                self.summary_data[channel] = self.summary_data[channel].reset_index(drop=True)
+            return
+
         fit_size = 10
         x_fit = np.linspace(0, 2 * fit_size, 2 * fit_size + 1)
         y_fit = np.linspace(0, 2 * fit_size, 2 * fit_size + 1)
         x_fit, y_fit = np.meshgrid(x_fit, y_fit)
         initial_guess = (200, fit_size, fit_size, 2, 2, 200)
 
-        self.summary_data = {}
-        intensity_columns = [f'i_{channel}' for channel in range(self.num_channels)]
         for channel in range(self.num_channels):
             self.summary_data[channel] = pd.DataFrame(columns=['particle', 'frame', 'x', 'y'] + intensity_columns)
 
             for p in self.linked_particles[channel]['particle'].unique():
                 pcle = self.linked_particles[channel].loc[self.linked_particles[channel]['particle'] == p]
                 ix = pcle['mass'].idxmax()
                 x = int(pcle.loc[ix]['y'])
@@ -227,47 +244,72 @@
                 self.summary_data[channel] = pd.concat((self.summary_data[channel], df), ignore_index=True)
             self.summary_data[channel] = self.summary_data[channel].reset_index(drop=True)
 
     def multi_color_link(self):  # TODO: Add max frame distance as a parameter instead of fixing it to 5
         """ Find the same particles in every channel and add the intensity information on each """
         kd_trees = {}
         for channel in range(self.num_channels):
-            kd_trees[channel] = KDTree(np.array(self.summary_data[channel][['x', 'y']]))
+            kd_trees[channel] = KDTree(np.array(self.summary_data[channel][['x', 'y', 'frame']]))
 
         for channel in range(self.num_channels):
             for channel_2 in range(channel + 1, self.num_channels):
                 for ix, p in self.summary_data[channel].iterrows():
-                    dist, ind = kd_trees[channel_2].query((p['x'], p['y']), p=2, distance_upper_bound=15)
+                    dist, ind = kd_trees[channel_2].query((p['x'], p['y'], p['frame']), p=2, distance_upper_bound=15)
                     if ind == kd_trees[channel_2].n:
                         continue
                     if abs(self.summary_data[channel_2].loc[ind]['frame'] - p['frame']) > 5:
-                        print('Frames too far apart with ', ix, p['x'], p['y'], p['frame'])
+                        logger.info('Frames too far apart with ', ix, p['x'], p['y'], p['frame'])
                         continue
                     self.summary_data[channel].loc[ix, f'i_{channel_2}'] = \
                         self.summary_data[channel_2].loc[ind][f'i_{channel_2}']
                     self.summary_data[channel_2].loc[ind, f'i_{channel}'] = p[f'i_{channel}']
 
     def save_all_data(self, filename):
         self.linked_particles.to_csv(str(filename))
 
     def save_data(self, filename):
         """ Saves only the most important information to the file: particle and intensity information.
         """
+
+        if len(self.channels_names) != self.num_channels:
+            self.channels_names = [i for i in range(self.num_channels)]
+
         if not type(filename) is Path:
             filename = Path(filename)
 
         for i in range(self.num_channels):
             stem = filename.stem
             file_name = filename.with_stem(f'{stem}_{i}')
             self.summary_data[i].to_csv(str(file_name))
 
+        # Exporting summary data
+        with open(filename.with_suffix('.md'), 'w') as f:
+            info = ""
+            for channel in range(self.num_channels):
+                info += f"# Channel {self.channels_names[channel]}\n\n"
+                info += f" - *Found particles*: {len(self.summary_data[channel])}\n"
+                if self.num_channels > 1:
+                    for sub_channel in range(self.num_channels):
+                        info += f" - Particles also in *{self.channels_names[sub_channel]}*: " \
+                                f"{len(self.summary_data[channel][f'i_{sub_channel}'].dropna())}\n"
+                info += f" - *Concentration*: {self.concentration.get(channel, 0):.2E} pcles/ml"
+                info += '\n\n'
+            f.write(info)
+
         with open(filename.with_suffix('.yml'), 'w') as f:
             yaml.dump(self.metadata, f)
 
     def calculate_concentration(self, step_size=5):
+        """ Calculates the concentration on each channel in the dataset. After linking the particles,
+        the concentration is calculated by simply counting the number of detections and dividing by the volume. The
+        volume is derived from the field of view (given a magnification and sensor size) and the third dimension from
+        the number of steps and the step size.
+
+        TODO: Real-space FOV is hard-coded (as well as the region in the edges of the image that is discarded).
+        """
         self.total_num_particles = {}
         self.concentration = {}
         if self.linked_particles is None:
             return
         fraction_sensor_used = (2048 - self.ignore_edge_pixels) / 2048
         field_of_view = fraction_sensor_used * (13.3 / 20) ** 2  # (Sensor size/magnification) # mm2
         for channel in range(self.num_channels):
@@ -276,14 +318,7 @@
             volume = volume / 1000  # in ml
             num_particles = len(self.linked_particles[channel].groupby('particle').sum())
 
             self.total_num_particles[channel] = num_particles
             self.concentration[channel] = num_particles / volume
 
         self.metadata.update({'concentration': self.concentration})
-
-    def calculate_background(self, frames_no=None, num_frames=10, sigma=200):
-        if frames_no is None:
-            average = np.mean(self.data[:num_frames], 0)
-        else:
-            average = np.mean(self.data[frames_no[0]:frames_no[1]], 0)
-        self.bkg = skimage.filters.gaussian(average, sigma=sigma)
```

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/util/make_hdf5.py` & `nanoqnt-0.2.1/nanoqnt/util/make_hdf5.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11814 - Atom.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11814 - Atom.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11815 - Battery.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11815 - Battery.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11816 - Orbit.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11817 - Beaker.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11819 - Bounce.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11820 - Caliper.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11821 - Catapult.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11822 - Collision.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11822 - Collision.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11828 - Energy.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11828 - Energy.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11829 - Flask.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11829 - Flask.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11830 - Float.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11830 - Float.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11832 - Force.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11832 - Force.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11833 - Formula.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11833 - Formula.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11834 - Gears.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11834 - Gears.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11835 - Gravity.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11837 - Histogram.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11839 - Magnet.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11841 - Metronome.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11843 - Molecule.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11844 - Motion.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11844 - Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11848 - Planet.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11848 - Planet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11850 - Power.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11850 - Power.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11851 - Press.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11851 - Press.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11852 - Proton.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11852 - Proton.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11853 - Pulley.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11854 - Reflection.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11855 - Resistor.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11856 - Rolling.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11857 - Rotate.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11859 - Temperature.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11861 - Waves.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11861 - Waves.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Save.svg` & `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Save.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/channel_selector.ui` & `nanoqnt-0.2.1/nanoqnt/view/GUI/channel_selector.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/data_exploration.ui` & `nanoqnt-0.2.1/nanoqnt/view/GUI/data_exploration.ui`

 * *Files 0% similar despite different names*

#### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/data_exploration.ui` & `nanoqnt-0.2.1/nanoqnt/view/GUI/data_exploration.ui`

```diff
@@ -98,20 +98,20 @@
               <item row="3" column="1">
                 <widget class="QComboBox" name="engine_box">
                   <property name="toolTip">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;If installed, numba is preferred&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                   <item>
                     <property name="text">
-                      <string>mask</string>
+                      <string>numba</string>
                     </property>
                   </item>
                   <item>
                     <property name="text">
-                      <string>numba</string>
+                      <string>mask</string>
                     </property>
                   </item>
                   <item>
                     <property name="text">
                       <string>python</string>
                     </property>
                   </item>
@@ -330,31 +330,31 @@
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="action_open"/>
         <addaction name="action_save_data"/>
         <addaction name="action_export_all_data"/>
       </widget>
-      <widget class="QMenu" name="menuAnaysis">
+      <widget class="QMenu" name="menuAnalysis">
         <property name="title">
-          <string>Anaysis</string>
+          <string>Analysis</string>
         </property>
         <addaction name="action_calculate_bkg"/>
         <addaction name="action_show_bkg"/>
         <addaction name="action_data_frame"/>
       </widget>
       <widget class="QMenu" name="menuHelp">
         <property name="title">
           <string>Help</string>
         </property>
         <addaction name="action_about"/>
         <addaction name="actionGo_to_documentation"/>
       </widget>
       <addaction name="menuFile"/>
-      <addaction name="menuAnaysis"/>
+      <addaction name="menuAnalysis"/>
       <addaction name="menuHelp"/>
     </widget>
     <action name="action_open">
       <property name="icon">
         <iconset>
           <normaloff>Icons/Open Folder.svg</normaloff>
           Icons/Open Folder.svg
```

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/particles_widget.ui` & `nanoqnt-0.2.1/nanoqnt/view/GUI/particles_widget.ui`

 * *Files 1% similar despite different names*

#### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/particles_widget.ui` & `nanoqnt-0.2.1/nanoqnt/view/GUI/particles_widget.ui`

```diff
@@ -56,15 +56,15 @@
             </item>
             <item row="1" column="0">
               <widget class="QLineEdit" name="size_line">
                 <property name="toolTip">
                   <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Approximate size of the particles in pixels&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                 </property>
                 <property name="text">
-                  <string>15</string>
+                  <string>7</string>
                 </property>
               </widget>
             </item>
             <item row="1" column="3">
               <widget class="QLineEdit" name="min_mass_line">
                 <property name="sizePolicy">
                   <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
@@ -78,15 +78,15 @@
                     <height>0</height>
                   </size>
                 </property>
                 <property name="toolTip">
                   <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum intensity to apply as a threshold&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                 </property>
                 <property name="text">
-                  <string>130</string>
+                  <string>10000</string>
                 </property>
               </widget>
             </item>
             <item row="1" column="4">
               <widget class="QLineEdit" name="found_particles_line">
                 <property name="enabled">
                   <bool>false</bool>
```

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/scan_control.ui` & `nanoqnt-0.2.1/nanoqnt/view/GUI/scan_control.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/channel_selector.py` & `nanoqnt-0.2.1/nanoqnt/view/channel_selector.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/main_window.py` & `nanoqnt-0.2.1/nanoqnt/view/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 
         if filename is not None:
             self.analyze_model.save_data(filename)
 
     def channels_updated(self):
         self.analyze_model.num_channels = self.channel_widget.channel_box.currentIndex() + 1
         self.channel_names = [line.text() for line in self.channel_widget.channels]
+        self.analyze_model.channels_names = self.channel_names
 
         self.nanoqnt_images = [ParticleWidget() for _ in range(self.analyze_model.num_channels)]
 
         plot_layout = self.video_widget.layout()
         for i in reversed(range(plot_layout.count())):
             plot_layout.itemAt(i).widget().setParent(None)
```

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/particle_widget.py` & `nanoqnt-0.2.1/nanoqnt/view/particle_widget.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc2/nanoqnt/view/stage_control.py` & `nanoqnt-0.2.1/nanoqnt/view/stage_control.py`

 * *Files identical despite different names*

