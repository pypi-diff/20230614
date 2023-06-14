# Comparing `tmp/stb-tester-33.0.0.tar.gz` & `tmp/stb-tester-33.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stb-tester-33.0.0.tar", last modified: Thu Jul 21 18:12:49 2022, max compression
+gzip compressed data, was "stb-tester-33.1.0.tar", last modified: Mon Jul 25 17:17:18 2022, max compression
```

## Comparing `stb-tester-33.0.0.tar` & `stb-tester-33.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2022-07-21 18:12:49.432769 stb-tester-33.0.0/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       80 2021-10-13 08:25:58.000000 stb-tester-33.0.0/MANIFEST.in
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1598 2022-07-21 18:12:49.432769 stb-tester-33.0.0/PKG-INFO
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       38 2022-07-21 18:12:49.432769 stb-tester-33.0.0/setup.cfg
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1852 2022-07-21 18:07:21.000000 stb-tester-33.0.0/setup.py
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2022-07-21 18:12:49.432769 stb-tester-33.0.0/stb_tester.egg-info/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1598 2022-07-21 18:12:49.000000 stb-tester-33.0.0/stb_tester.egg-info/PKG-INFO
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      261 2022-07-21 18:12:49.000000 stb-tester-33.0.0/stb_tester.egg-info/SOURCES.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        1 2022-07-21 18:12:49.000000 stb-tester-33.0.0/stb_tester.egg-info/dependency_links.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       16 2022-07-21 18:12:49.000000 stb-tester-33.0.0/stb_tester.egg-info/requires.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        5 2022-07-21 18:12:49.000000 stb-tester-33.0.0/stb_tester.egg-info/top_level.txt
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2022-07-21 18:12:49.432769 stb-tester-33.0.0/stbt/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    30712 2022-07-21 12:29:19.000000 stb-tester-33.0.0/stbt/__init__.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      708 2022-06-25 08:00:03.000000 stb-tester-33.0.0/stbt/audio.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     5740 2022-06-30 10:55:57.000000 stb-tester-33.0.0/stbt/prometheus.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       73 2022-06-25 08:00:03.000000 stb-tester-33.0.0/stbt/pylint_plugin.py
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2022-07-25 17:17:18.752384 stb-tester-33.1.0/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       80 2021-10-13 08:25:58.000000 stb-tester-33.1.0/MANIFEST.in
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1598 2022-07-25 17:17:18.752384 stb-tester-33.1.0/PKG-INFO
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       38 2022-07-25 17:17:18.752384 stb-tester-33.1.0/setup.cfg
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1852 2022-07-25 17:01:25.000000 stb-tester-33.1.0/setup.py
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2022-07-25 17:17:18.748384 stb-tester-33.1.0/stb_tester.egg-info/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1598 2022-07-25 17:17:18.000000 stb-tester-33.1.0/stb_tester.egg-info/PKG-INFO
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      261 2022-07-25 17:17:18.000000 stb-tester-33.1.0/stb_tester.egg-info/SOURCES.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        1 2022-07-25 17:17:18.000000 stb-tester-33.1.0/stb_tester.egg-info/dependency_links.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       16 2022-07-25 17:17:18.000000 stb-tester-33.1.0/stb_tester.egg-info/requires.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        5 2022-07-25 17:17:18.000000 stb-tester-33.1.0/stb_tester.egg-info/top_level.txt
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2022-07-25 17:17:18.752384 stb-tester-33.1.0/stbt/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    31468 2022-07-25 17:01:25.000000 stb-tester-33.1.0/stbt/__init__.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      708 2022-06-25 08:00:03.000000 stb-tester-33.1.0/stbt/audio.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     5740 2022-06-30 10:55:57.000000 stb-tester-33.1.0/stbt/prometheus.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       73 2022-06-25 08:00:03.000000 stb-tester-33.1.0/stbt/pylint_plugin.py
```

### Comparing `stb-tester-33.0.0/PKG-INFO` & `stb-tester-33.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stb-tester
-Version: 33.0.0
+Version: 33.1.0
 Summary: Automated GUI testing for Set-Top Boxes
 Home-page: https://stb-tester.com
 Author: Stb-tester.com Ltd.
 Author-email: support@stb-tester.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `stb-tester-33.0.0/setup.py` & `stb-tester-33.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 autocompletion, but without a working implementation.
 
 [Stb-tester Platform]: https://stb-tester.com
 """
 
 setuptools.setup(
     name="stb-tester",
-    version="33.0.0",
+    version="33.1.0",
     author="Stb-tester.com Ltd.",
     author_email="support@stb-tester.com",
     description="Automated GUI testing for Set-Top Boxes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://stb-tester.com",
     packages=["stbt"],
```

### Comparing `stb-tester-33.0.0/stb_tester.egg-info/PKG-INFO` & `stb-tester-33.1.0/stb_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stb-tester
-Version: 33.0.0
+Version: 33.1.0
 Summary: Automated GUI testing for Set-Top Boxes
 Home-page: https://stb-tester.com
 Author: Stb-tester.com Ltd.
 Author-email: support@stb-tester.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `stb-tester-33.0.0/stbt/__init__.py` & `stb-tester-33.1.0/stbt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     "find_regions_by_color",
     "find_selection_from_background",
     "FIRST_FRAME_TIME",
     "get_rms_volume",
     "measure_av_sync",
     "play_audio_file",
     "prometheus",
+    "RmsVolumeResult",
     "Roku",
     "segment",
     "stop_job",
     "TEST_PACK_ROOT",
     "VolumeChangeDirection",
     "VolumeChangeTimeout",
     "wait_for_volume_change",
@@ -204,15 +205,15 @@
     :return: An iterator yielding `AudioChunk` objects
     :rtype: Iterator[AudioChunk]
     """
     _raise_premium("audio_chunks")
     return iter([AudioChunk((4800,), dtype=numpy.float32)])
 
 
-def get_rms_volume(duration_secs=3, stream=None):
+def get_rms_volume(duration_secs=3, stream=None) -> "RmsVolumeResult":
     """Calculate the average `RMS`_ volume of the audio over the given duration.
 
     For example, to check that your mute button works::
 
         stbt.press('KEY_MUTE')
         time.sleep(1)  # <- give it some time to take effect
         assert get_rms_volume().amplitude < 0.001  # -60 dB
@@ -224,35 +225,55 @@
 
     :type stream: Iterator[AudioChunk]
     :param stream: Audio stream to measure. Defaults to ``audio_chunks()``.
 
     :raises ZeroDivisionError: If ``duration_secs`` is shorter than one sample
         or ``stream`` contains no samples.
 
-    :returns:
-        An object with the following attributes:
-
-        * **amplitude** (*float*) – The RMS amplitude over the specified
-          window. This is a value between 0.0 (absolute silence) and 1.0 (a
-          full-range square wave).
-
-        * **time** (*float*) – The start of the window, as number of seconds
-          since the unix epoch (1970-01-01T00:00Z). This is compatible with
-          ``time.time()`` and ``stbt.Frame.time``.
-
-        * **duration_secs** (*float*) – The window size, in seconds. Typically
-          this will be the same as passed into ``get_rms_volume()``.
+    :rtype: RmsVolumeResult
 
     .. _RMS: https://en.wikipedia.org/wiki/Root_mean_square
     """
     _raise_premium("get_rms_volume")
-    return _RmsVolumeResult(0.0, 0.0, 0.0)
+    return RmsVolumeResult(0.0, 0.0, 0.0)
+
+
+class RmsVolumeResult(
+        namedtuple('RmsVolumeResult', 'time duration_secs amplitude')):
+    """The result from `get_rms_volume`.
+
+    :ivar float amplitude: The `RMS`_ amplitude over the specified window. This
+      is a value between 0.0 (absolute silence) and 1.0 (a full-range square
+      wave).
 
+    :ivar float time: The start of the window, as number of seconds since the
+      unix epoch (1970-01-01T00:00Z). This is compatible with ``time.time()``
+      and ``stbt.Frame.time``.
 
-_RmsVolumeResult = namedtuple('RmsVolumeResult', 'time duration_secs amplitude')
+    :ivar int|float duration_secs: The window size in seconds, as given to
+      `get_rms_volume`.
+    """
+
+    def dBov(self, noise_floor_amplitude=0.0003) -> float:
+        """The RMS amplitude converted to `dBov`_.
+
+        Decibels are a logarithmic measurement; human perception of loudness is
+        also logarithmic, so decibels are a useful way to measure loudness.
+
+        This is a value between -70 (silence, or near silence) and 0 (the
+        loudest possible signal, a full-scale square wave).
+
+        :param noise_floor_amplitude: This is used to avoid `ZeroDivisionError`
+            exceptions. We consider 0 amplitude to be this non-zero value
+            instead. It defaults to ~0.0003 (-70dBov).
+
+        .. _dBov: https://en.wikipedia.org/wiki/DBFS
+        """
+        import math
+        return 20 * math.log10(max(self.amplitude, noise_floor_amplitude))
 
 
 class VolumeChangeDirection(IntEnum):
     LOUDER = 1
     QUIETER = -1
 
     # For nicer formatting of `wait_for_volume_change` signature in generated
@@ -263,15 +284,16 @@
 
 class VolumeChangeTimeout(AssertionError):
     pass
 
 
 def wait_for_volume_change(
         direction=VolumeChangeDirection.LOUDER, stream=None,
-        window_size_secs=0., threshold_db=0., noise_floor=0.0, timeout_secs=0.):
+        window_size_secs=0.400, threshold_db=10.,
+        noise_floor_amplitude=0.0003, timeout_secs=10):
 
     """Wait for changes in the RMS audio volume.
 
     This can be used to listen for the start of content, or for bleeps and
     bloops when navigating the UI. It returns after the first significant
     volume change. This function tries hard to give accurate timestamps for
     when the volume changed. It works best for sudden changes like a beep.
@@ -325,17 +347,17 @@
         ``direction=VolumeChangeDirection.QUIETER`` the RMS volume must fall by
         10 dB.
 
     :type noise_floor_amplitude: float
     :param noise_floor_amplitude: This is used to avoid `ZeroDivisionError`
         exceptions.  The change from an amplitude of 0 to 0.1 is ∞ dB.
         This isn't very practical to deal with so we consider 0 amplitude to be
-        this non-zero ``noise_floor_amplitude`` instead. It defaults to ~0.0003
-        (-70dBov). Increase this value if there is some sort of background
-        noise that you want to ignore.
+        this non-zero value instead. It defaults to ~0.0003 (-70dBov). Increase
+        this value if there is some sort of background noise that you want to
+        ignore.
 
     :type timeout_secs: float
     :param timeout_secs: Timeout in seconds. If no significant volume change is
         found within this time, `VolumeChangeTimeout` will be raised and your
         test will fail.
 
     :raises VolumeChangeTimeout: If no volume change is detected before
@@ -343,18 +365,18 @@
 
     :returns:
         An object with the following attributes:
 
         * **direction** (`VolumeChangeDirection`) – This will be either
           ``VolumeChangeDirection.LOUDER`` or ``VolumeChangeDirection.QUIETER``
           as given to ``wait_for_volume_change``.
-        * **rms_before** (see `get_rms_volume`) – The RMS volume averaged over
+        * **rms_before** (`RmsVolumeResult`) – The RMS volume averaged over
           the window immediately before the volume change. Use
           ``result.rms_before.amplitude`` to get the RMS amplitude as a float.
-        * **rms_after** (see `get_rms_volume`) – The RMS volume averaged over
+        * **rms_after** (`RmsVolumeResult`) – The RMS volume averaged over
           the window immediately after the volume change.
         * **difference_db** (*float*) – Ratio between ``rms_after`` and
           ``rms_before``, in decibels.
         * **difference_amplitude** (*float*) – Absolute difference between the
           ``rms_after`` and ``rms_before``. This is a number in the range -1.0
           to +1.0.
         * **time** (*float*) – The time of the volume change, as number of
@@ -362,16 +384,16 @@
           format used by the Python standard library function ``time.time()``
           and ``stbt.Frame.time``.
         * **window_size_secs** (*float*) – The size of the window over which
           the volume was averaged, in seconds.
     """
     _raise_premium("wait_for_volume_change")
     return _VolumeChangeResult(VolumeChangeDirection.LOUDER,
-                               _RmsVolumeResult(0.0, 0.0, 0.0),
-                               _RmsVolumeResult(0.0, 0.0, 0.0),
+                               RmsVolumeResult(0.0, 0.0, 0.0),
+                               RmsVolumeResult(0.0, 0.0, 0.0),
                                0.0, 0.0, 0.0, 0.)
 
 
 _VolumeChangeResult = namedtuple(
     '_VolumeChangeResult',
     "direction rms_before rms_after difference_db difference_amplitude time "
     "window_size_secs")
@@ -817,15 +839,15 @@
                 ...
 
         .. _debug console: https://developer.roku.com/en-gb/docs/developer-program/debugging/debugging-channels.md
         """
         _raise_premium("Roku")
         yield
 
-    def query_apps(self) -> dict[str, str]:
+    def query_apps(self) -> Dict[str, str]:
         """Returns a dict of ``application_id: name`` with all the apps
         installed on the Roku device.
         """
         _raise_premium("Roku")
         return {}
 
     def launch_app(self, id_or_name) -> None:
```

### Comparing `stb-tester-33.0.0/stbt/audio.py` & `stb-tester-33.1.0/stbt/audio.py`

 * *Files identical despite different names*

### Comparing `stb-tester-33.0.0/stbt/prometheus.py` & `stb-tester-33.1.0/stbt/prometheus.py`

 * *Files identical despite different names*

