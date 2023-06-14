# Comparing `tmp/gamutrf-0.5.8.tar.gz` & `tmp/gamutrf-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamutrf-0.5.8.tar", max compression
+gzip compressed data, was "gamutrf-0.5.9.tar", max compression
```

## Comparing `gamutrf-0.5.8.tar` & `gamutrf-0.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11373 2023-01-11 04:17:13.741856 gamutrf-0.5.8/LICENSE
--rw-r--r--   0        0        0    10849 2023-01-11 04:17:13.741856 gamutrf-0.5.8/README.md
--rw-r--r--   0        0        0       75 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/__init__.py
--rw-r--r--   0        0        0     1018 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/__main__.py
--rwxr-xr-x   0        0        0    10832 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/api.py
--rwxr-xr-x   0        0        0     1967 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/birdseye_rssi.py
--rwxr-xr-x   0        0        0     4153 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/freqxlator.py
--rwxr-xr-x   0        0        0     3673 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/grscan.py
--rwxr-xr-x   0        0        0     3376 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/grsource.py
--rwxr-xr-x   0        0        0     3013 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/mqtt_reporter.py
--rwxr-xr-x   0        0        0     2525 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/sample_reader.py
--rwxr-xr-x   0        0        0     2100 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/samples2raw.py
--rwxr-xr-x   0        0        0     5068 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/scan.py
--rwxr-xr-x   0        0        0     6492 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/scan2mp4.py
--rwxr-xr-x   0        0        0     2688 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/scan2rtlpow.py
--rwxr-xr-x   0        0        0    12294 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/sdr_recorder.py
--rwxr-xr-x   0        0        0    21260 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/sigfinder.py
--rwxr-xr-x   0        0        0     7925 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/sigwindows.py
--rwxr-xr-x   0        0        0    11549 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/specgram.py
--rwxr-xr-x   0        0        0     3155 2023-01-11 04:17:13.745856 gamutrf-0.5.8/gamutrf/utils.py
--rw-r--r--   0        0        0     1361 2023-01-11 04:17:13.749857 gamutrf-0.5.8/pyproject.toml
--rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 gamutrf-0.5.8/setup.py
--rw-r--r--   0        0        0    12056 1970-01-01 00:00:00.000000 gamutrf-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11373 2023-01-29 01:59:28.979806 gamutrf-0.5.9/LICENSE
+-rw-r--r--   0        0        0    10849 2023-01-29 01:59:28.979806 gamutrf-0.5.9/README.md
+-rw-r--r--   0        0        0       75 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/__init__.py
+-rw-r--r--   0        0        0     1018 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/__main__.py
+-rwxr-xr-x   0        0        0    10832 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/api.py
+-rwxr-xr-x   0        0        0     1967 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/birdseye_rssi.py
+-rwxr-xr-x   0        0        0     4153 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/freqxlator.py
+-rwxr-xr-x   0        0        0     3966 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/grscan.py
+-rwxr-xr-x   0        0        0     3376 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/grsource.py
+-rwxr-xr-x   0        0        0     3013 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/mqtt_reporter.py
+-rwxr-xr-x   0        0        0     2525 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/sample_reader.py
+-rwxr-xr-x   0        0        0     2100 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/samples2raw.py
+-rwxr-xr-x   0        0        0     5328 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/scan.py
+-rwxr-xr-x   0        0        0     6492 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/scan2mp4.py
+-rwxr-xr-x   0        0        0     2688 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/scan2rtlpow.py
+-rwxr-xr-x   0        0        0    12294 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/sdr_recorder.py
+-rwxr-xr-x   0        0        0    21645 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/sigfinder.py
+-rwxr-xr-x   0        0        0     7925 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/sigwindows.py
+-rwxr-xr-x   0        0        0    11549 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/specgram.py
+-rwxr-xr-x   0        0        0     3155 2023-01-29 01:59:28.983806 gamutrf-0.5.9/gamutrf/utils.py
+-rw-r--r--   0        0        0     1360 2023-01-29 01:59:28.983806 gamutrf-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 gamutrf-0.5.9/setup.py
+-rw-r--r--   0        0        0    12056 1970-01-01 00:00:00.000000 gamutrf-0.5.9/PKG-INFO
```

### Comparing `gamutrf-0.5.8/LICENSE` & `gamutrf-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/README.md` & `gamutrf-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/__main__.py` & `gamutrf-0.5.9/gamutrf/__main__.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/api.py` & `gamutrf-0.5.9/gamutrf/api.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/birdseye_rssi.py` & `gamutrf-0.5.9/gamutrf/birdseye_rssi.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/freqxlator.py` & `gamutrf-0.5.9/gamutrf/freqxlator.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/grscan.py` & `gamutrf-0.5.9/gamutrf/grscan.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         samp_rate=4.096e6,
         sweep_sec=30,
         logaddr="0.0.0.0",  # nosec
         logport=8001,
         sdr="ettus",
         sdrargs=None,
         fft_size=1024,
+        tune_overlap=0.5,
+        tune_step_fft=0,
         iqtlabs=None,
     ):
         gr.top_block.__init__(self, "scan", catch_exceptions=True)
 
         ##################################################
         # Parameters
         ##################################################
@@ -57,21 +59,26 @@
             center_freq=freq_start,
             sdrargs=sdrargs,
         )
 
         self.retune_fft = None
         if iqtlabs:
             freq_range = freq_end - freq_start
-            tune_step_hz = int(samp_rate / 2)
-            target_retune_hz = freq_range / self.sweep_sec / tune_step_hz
-            fft_rate = int(samp_rate / fft_size)
-            tune_step_fft = int(fft_rate / target_retune_hz)
-            logging.info(
-                f"tuning across {freq_range/1e6}MHz in {self.sweep_sec}s, requires retuning at {target_retune_hz}Hz in {tune_step_hz/1e6}MHz steps"
-            )
+            tune_step_hz = int(samp_rate * tune_overlap)
+            if tune_step_fft:
+                logging.info(
+                    f"retuning across {freq_range/1e6}MHz every {tune_step_fft} FFTs"
+                )
+            else:
+                target_retune_hz = freq_range / self.sweep_sec / tune_step_hz
+                fft_rate = int(samp_rate / fft_size)
+                tune_step_fft = int(fft_rate / target_retune_hz)
+                logging.info(
+                    f"retuning across {freq_range/1e6}MHz in {self.sweep_sec}s, requires retuning at {target_retune_hz}Hz in {tune_step_hz/1e6}MHz steps ({tune_step_fft} FFTs)"
+                )
             self.retune_fft = iqtlabs.retune_fft(
                 "rx_freq",
                 fft_size,
                 int(samp_rate),
                 int(freq_start),
                 int(freq_end),
                 tune_step_hz,
```

### Comparing `gamutrf-0.5.8/gamutrf/grsource.py` & `gamutrf-0.5.9/gamutrf/grsource.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/mqtt_reporter.py` & `gamutrf-0.5.9/gamutrf/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/sample_reader.py` & `gamutrf-0.5.9/gamutrf/sample_reader.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/samples2raw.py` & `gamutrf-0.5.9/gamutrf/samples2raw.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/scan.py` & `gamutrf-0.5.9/gamutrf/scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,19 +60,26 @@
         type=eng_float,
         default=eng_notation.num_to_str(float(4.096e6)),
         help="Set samp_rate [default=%(default)r]",
     )
     parser.add_argument(
         "--sweep-sec",
         dest="sweep_sec",
-        type=intx,
+        type=float,
         default=30,
         help="Set sweep_sec [default=%(default)r]",
     )
     parser.add_argument(
+        "--tune-step-fft",
+        dest="tune_step_fft",
+        type=int,
+        default=0,
+        help="tune FFT step (0 is use sweep_sec) [default=%(default)r]",
+    )
+    parser.add_argument(
         "--nfft",
         dest="nfft",
         type=int,
         default=2048,
         help="FFTI size [default=%(default)r]",
     )
     parser.add_argument(
@@ -114,19 +121,19 @@
         "--updatetimeout",
         dest="updatetimeout",
         type=int,
         default=10,
         help="seconds to wait for healthy freq updates",
     )
     parser.add_argument(
-        "--retune-intervals",
-        dest="retune_intervals",
-        type=int,
-        default=1,
-        help="if > 1, then schedule future retuning events in batches",
+        "--tuneoverlap",
+        dest="tuneoverlap",
+        type=float,
+        default=0.5,
+        help="multiple of samp_rate when retuning",
     )
     return parser
 
 
 def main():
     logging.basicConfig(level=logging.DEBUG, format="%(asctime)s %(message)s")
     options = argument_parser().parse_args()
@@ -163,14 +170,16 @@
         samp_rate=options.samp_rate,
         sweep_sec=options.sweep_sec,
         logaddr=options.logaddr,
         logport=options.logport,
         sdr=options.sdr,
         sdrargs=options.sdrargs,
         fft_size=options.nfft,
+        tune_overlap=options.tuneoverlap,
+        tune_step_fft=options.tune_step_fft,
         iqtlabs=iqtlabs,
     )
 
     def sig_handler(_sig=None, _frame=None):
         tb.stop()
         tb.wait()
         sys.exit(0)
```

### Comparing `gamutrf-0.5.8/gamutrf/scan2mp4.py` & `gamutrf-0.5.9/gamutrf/scan2mp4.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/scan2rtlpow.py` & `gamutrf-0.5.9/gamutrf/scan2rtlpow.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/sdr_recorder.py` & `gamutrf-0.5.9/gamutrf/sdr_recorder.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/sigfinder.py` & `gamutrf-0.5.9/gamutrf/sigfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from gamutrf.sigwindows import graph_fft_peaks
 from gamutrf.sigwindows import parse_freq_excluded
 from gamutrf.sigwindows import scipy_find_sig_windows
 from gamutrf.utils import rotate_file_n, SCAN_FRES
 
 MB = int(1.024e6)
 FFT_BUFFER_TIME = 1
-BUFF_FILE = "/dev/shm/scanfftbuffer.txt.zst"  # nosec
+BUFF_FILE = "scanfftbuffer.txt.zst"  # nosec
 PEAK_TRIGGER = int(os.environ.get("PEAK_TRIGGER", "0"))
 PIN_TRIGGER = int(os.environ.get("PIN_TRIGGER", "17"))
 if PEAK_TRIGGER == 1:
     import RPi.GPIO as GPIO
 
     GPIO.setmode(GPIO.BCM)
     GPIO.setup(PIN_TRIGGER, GPIO.OUT)
@@ -463,17 +463,18 @@
                         packets_sent += 1
                         last_packet_sent_time = now
                         break
         os.rename(tmp_buff_file, buff_file)
 
 
 def find_signals(args, prom_vars):
+    buff_file = os.path.join(args.buff_path, BUFF_FILE)
     with concurrent.futures.ProcessPoolExecutor(2) as executor:
-        proxy_result = executor.submit(fft_proxy, args, BUFF_FILE)
-        process_fft_lines(args, prom_vars, BUFF_FILE, executor, proxy_result)
+        proxy_result = executor.submit(fft_proxy, args, buff_file)
+        process_fft_lines(args, prom_vars, buff_file, executor, proxy_result)
 
 
 def argument_parser():
     parser = argparse.ArgumentParser(
         description="watch a scan UDP stream and find signals"
     )
     parser.add_argument(
@@ -555,14 +556,21 @@
         "--promport",
         dest="promport",
         type=int,
         default=9000,
         help="Prometheus client port",
     )
     parser.add_argument(
+        "--port",
+        dest="port",
+        type=int,
+        default=80,
+        help="control webserver port",
+    )
+    parser.add_argument(
         "--freq-end",
         dest="freq_end",
         type=float,
         default=float(1e9),
         help="Set freq_end [default=%(default)r]",
     )
     parser.add_argument(
@@ -596,15 +604,21 @@
     parser.add_argument(
         "--running_fft_secs",
         dest="running_fft_secs",
         type=int,
         default=900,
         help="Number of seconds for running FFT average",
     )
-
+    parser.add_argument(
+        "--buff_path",
+        dest="buff_path",
+        type=str,
+        default="/dev/shm",  # nosec
+        help="Path for FFT buffer file",
+    )
     return parser
 
 
 def main():
     parser = argument_parser()
     args = parser.parse_args()
 
@@ -622,8 +636,8 @@
     app = falcon.App()
     scanner_form = ScannerForm()
     result = Result()
     active_requests = ActiveRequests()
     app.add_route("/", scanner_form)
     app.add_route("/result", result)
     app.add_route("/requests", active_requests)
-    bjoern.run(app, "0.0.0.0", 80)
+    bjoern.run(app, "0.0.0.0", args.port)  # nosec
```

### Comparing `gamutrf-0.5.8/gamutrf/sigwindows.py` & `gamutrf-0.5.9/gamutrf/sigwindows.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/specgram.py` & `gamutrf-0.5.9/gamutrf/specgram.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/gamutrf/utils.py` & `gamutrf-0.5.9/gamutrf/utils.py`

 * *Files identical despite different names*

### Comparing `gamutrf-0.5.8/pyproject.toml` & `gamutrf-0.5.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gamutrf"
-version = "0.5.8"
+version = "0.5.9"
 description = "An orchestrated SDR scanner"
 authors = ["cglewis <clewis@iqt.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "gamutrf" },
 ]
@@ -13,36 +13,36 @@
 python = ">=3.8 <3.11"
 bjoern = "3.2.2"
 falcon = "3.1.1"
 falcon-cors = "1.1.7"
 gpsd-py3 = "0.3.0"
 httpx = "0.23.3"
 Jinja2 = "3.1.2"
-matplotlib = "3.6.2"
+matplotlib = "3.6.3"
 numpy = "1.24.1"
 paho-mqtt = "1.6.1"
-pandas = "1.5.2"
-prometheus_client = "0.15.0"
-requests = "2.28.1"
+pandas = "1.5.3"
+prometheus_client = "0.16.0"
+requests = "2.28.2"
 "RPi.GPIO" = "0.7.1"
 schedule = "1.1.0"
 scipy = "1.10.0"
-sigmf = "1.0.0"
+sigmf = "1.1.0"
 zstandard = "0.19.0"
 pycairo = "^1.21.0"
 cairocffi = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
 attrs = "22.2.0"
 black = "22.12.0"
 docker = "6.0.1"
 pylint = "2.15.10"
-pytest = "7.2.0"
+pytest = "7.2.1"
 pytest-cov = "4.0.0"
-pytype = "2022.12.15"
+pytype = "2023.1.17"
 
 [tool.poetry.scripts]
 gamutrf-api = 'gamutrf.__main__:api'
 gamutrf-freqxlator = 'gamutrf.__main__:freqxlator'
 gamutrf-samples2raw = 'gamutrf.__main__:samples2raw'
 gamutrf-scan = 'gamutrf.__main__:scan'
 gamutrf-scan2mp4 = 'gamutrf.__main__:scan2mp4'
```

### Comparing `gamutrf-0.5.8/setup.py` & `gamutrf-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,39 +12,39 @@
  'RPi.GPIO==0.7.1',
  'bjoern==3.2.2',
  'cairocffi>=1.3.0,<2.0.0',
  'falcon-cors==1.1.7',
  'falcon==3.1.1',
  'gpsd-py3==0.3.0',
  'httpx==0.23.3',
- 'matplotlib==3.6.2',
+ 'matplotlib==3.6.3',
  'numpy==1.24.1',
  'paho-mqtt==1.6.1',
- 'pandas==1.5.2',
- 'prometheus_client==0.15.0',
+ 'pandas==1.5.3',
+ 'prometheus_client==0.16.0',
  'pycairo>=1.21.0,<2.0.0',
- 'requests==2.28.1',
+ 'requests==2.28.2',
  'schedule==1.1.0',
  'scipy==1.10.0',
- 'sigmf==1.0.0',
+ 'sigmf==1.1.0',
  'zstandard==0.19.0']
 
 entry_points = \
 {'console_scripts': ['gamutrf-api = gamutrf.__main__:api',
                      'gamutrf-freqxlator = gamutrf.__main__:freqxlator',
                      'gamutrf-samples2raw = gamutrf.__main__:samples2raw',
                      'gamutrf-scan = gamutrf.__main__:scan',
                      'gamutrf-scan2mp4 = gamutrf.__main__:scan2mp4',
                      'gamutrf-scan2rtlpow = gamutrf.__main__:scan2rtlpow',
                      'gamutrf-sigfinder = gamutrf.__main__:sigfinder',
                      'gamutrf-specgram = gamutrf.__main__:specgram']}
 
 setup_kwargs = {
     'name': 'gamutrf',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'An orchestrated SDR scanner',
     'long_description': '# gamutRF\n\nAn SDR orchestrated scanner and collector.\n\ngamutRF is a system enabling a compact network of one or more modest machines (such as Pi4s), each with their own USB SDR (such as an Ettus\nB200mini or a BladeRF XA9), to operate collectively as a configurable wideband scanner and I/Q sample recorder.\n\nA gamutRF "orchestrator" machine can scan 0.1GHz to 6GHz in 30 seconds to identify signals, and then command potentially many gamutRF "workers" to make I/Q sample recordings for later analysis.\n\ngamutRF provides tools to work with I/Q sample recordings, and to also record GPS location/compass metadata for the system itself. gamutRF typically runs on networks of Raspberry Pi4s, but can also run on x86 machines, and is based on gnuradio.\n\nSee also [instructions on how to build a gamutRF system](BUILD.md).\n\n## Scanner theory of operation\n\ngamutRF\'s scanner function is split across two Docker containers which are both run on the orchestrator. The `gamutrf` (scanner) container connects to the SDR and sweeps over a configured frequency range in 30s, while sampling at 8.192Msps (all default values which can be changed).\n\nThe samples are sent to a [streaming FFT gnuradio block](https://github.com/iqtlabs/gr-iqtlabs) which emits 2048 FFT points which are served over ZMQ to the `sigfinder` container (see below). The FFT block needs to know when the SDR has been retuned to a new frequency, so it uses a gnuradio timestamp and frequency tag provided by the gnuradio UHD driver upon retuning. This tag functionality has been added to the Soapy driver in a gnuradio fork which is part of gamutRF, so that other SDRs may be used as scanners.\n\nThe `sigfinder` container consumes these FFT points from ZMQ, does some noise processing (correcting FFT points to be in frequency order, computing mean power over 10kHz, and then a rolling mean over 1MHz) and then submits them to [scipy.signals.find_peaks](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.find_peaks.html).\n\nIf workers have been provisioned, the orchestrator will then command the workers to make an approximately 10 second I/Q recording at approximately 20Msps of each signal. Each signal peak is assigned a 20MHz bin, which means that if a signal is repeatedly detected with some frequency variation, the assigned recording bin will be constant, and if multiple signals are detected within 20MHz they can be collected simultaneously. A worker by default records at a higher sample rate than the bin size, so that 20MHz signal margins can be recorded.\n\nAs there will almost certainly be more signals than workers available, the orchestrator will prioritize signals that it least often observed over a configurable number of scanner cycles. It is possible to configure this to `off` so that the recording choice will be random. It is also possible to configure the workers to tell the orchestrator to exclude that worker from certain frequency ranges (if for example the worker SDR cannot handle some part of the frequency spectrum scanned).\n\n## Operating gamutRF\n\nSee the [build doc](BUILD.md)\n\n### SDR/scanner/sigfinder command line options\n\nWhile there are other options, these options primarily influence gamutRF\'s scanner functionality.\n\n#### scanner\n\n| Option | Description |\n| -- | -- |\n| --freq-start and --freq-end | Start and end of frequency range to scan in Hz (also used by sigfinger) |\n| --igain | SDR input gain in dB |\n| --samp-rate | Number of samples/sec |\n| --sweep-sec | Time to sweep frequency range in seconds |\n| --nfft | Number of FFT points |\n\n##### sigfinder\n\n| Option | Description |\n| -- | -- |\n| --width | Minimum width of a peak to be detected in 0.01MHz increments (passed to scipy find_peaks()) |\n| --prominence | Minimum prominence of a peak to be detected (passed to scipy find_peaks()) |\n| --threshold | Minimum threshold in dB of a peak to be detected (passed to scipy find_peaks()) |\n| --bin_width | Bin width in MHz |\n| --max_raw_power | Maximum valid raw power value at each FFT point |\n| --history | Number of scanner cycles over which to prioritize recording of least often observed peaks |\n| --record_bw_msps | Number of samples per second in units of 1024^2 (generally larger than bin size to record signal margins) |\n| --record_secs | Length of time to record I/Q samples in seconds |\n| --fftlog | Log raw output of CSV to this file, which will be rotated every --rotatesecs |\n| --fftgraph | Graph the most recent FFT signal and peaks to this PNG file (will keep the last --nfftgraph versions) |\n\n### Manually initiating worker actions\n\nThe orchestrator has a web interface on port 80. You can use this to command a worker to start an I/Q sample recording or start a RSSI stream.\n\n## Working with worker I/Q recordings\n\nWorkers make recordings that are compressed with zstandard, and are typically in complex number, int16 format, and include the center frequency and sample rate that the recording was made with. gamutRF tools can generally work with such files directly, but other tools require the recordings to be converted (see below).\n\n### Generating a spectrogram of a recording\n\ngamutRF provides a tool to convert a recording or directory of recordings into a spectrogram. For example, to convert all I/Q recordings in /tmp:\n\n```docker run -ti -v /tmp:/tmp iqtlabs/gamutrf gamutrf-specgram /tmp```\n\nUse the ```--help``` option to change how the spectogram is generated (for example, to change the sample rate).\n\n### Translating recordings to "gnuradio" format\n\nMost SDR tools by convention take an uncompressed raw binary file as input, of [gnuradio type complex](https://blog.sdr.hu/grblocks/types.html). The user must explicitly specify to most SDR tools what sample rate the file was made at to correctly process it. gamutRF provides a tool that converts a gamutRF I/Q recording (which may be compressed) to an uncompressed binary file. For example:\n\n```\ndocker run -v /tmp:/tmp -ti iqtlabs/gamutrf gamutrf-samples2raw /tmp/gamutrf_recording_ettus_directional_gain70_1234_100000000Hz_20971520sps.s16.zst\n```\n\n### Reviewing a recording interactively in gqrx\n\n[gqrx](https://gqrx.dk/) is a multiplatform open source tool that allows some basic SDR operations like visualizing or audio demodulating an I/Q sample recording (see the [github releases page](https://github.com/gqrx-sdr/gqrx/releases), for a MacOS .dmg file). To use gqrx with a gamutRF recording, first translate the recording to gnuradio format (see above). Then open gqrx.\n\n* Select ```Complex Sampled (I/Q) File```\n* Set ```Input rate``` to be the same as the gamutRF sample rate (e.g. from the recording file name,\n```gamutrf_recording_ettus_directional_gain70_1234_100000000Hz_20971520sps.raw```, set ```Input rate``` to 20971520, and also edit ```rate=``` in ```Device string``` to be 20971520)\n* Set ``Bandwidth`` to 0\n* Edit ```Device string``` to set the ```file=``` to be the path to the recording.\n* Set ```Decimation``` to None.\n* Finally select ```OK``` and then ```play``` from the gqrx interface to watch the recording play.\n\n### Reducing recording sample rate\n\nYou may want to reduce the sample rate of a recording or re-center it with respect to frequency (e.g. to use another demodulator tool that doesn\'t support a high sample rate). gamutRF provides the ```freqxlator``` tool to do this.\n\n* Translate your gamutRF recording to gnuradio format (see above).\n* Use ```freqxlator``` to create a new recording at a lower sample rate, potentially with a different center frequency.\n\nFor example, to reduce a recording made with gamutRF\'s default sample rate to 1/10th the rate while adjusting the center frequency down by 1MHz, use:\n\n```docker run -ti iqtlabs/gamutrf gamutrf-freqxlator --samp-rate 20971520 --center -1e6 --dec 10 gamutrf_recording_gain70_1234_100000000Hz_20971520sps.raw gamutrf_recording_gain70_1234_100000000Hz_2097152sps.raw```\n\n### Demodulating AM/FM audio from a recording\n\ngamutRF provides a tool to demodulate AM/FM audio from a recording as an example use case.\n\n* Use the ```freqxlator``` tool to make a new recording at no more than 1Msps and has the frequency to be demodulated centered.\n* Use the ```airspyfm``` tool to demodulate audio to a WAV file.\n\nFor example, to decode an FM recording which must be at the center frequency of a recording:\n\n```docker run -v /tmp:/tmp -ti iqtlabs/gamutrf-airspyfm -m fm -t filesource -c filename=/tmp/gamutrf_recording_gain70_1234_100000000Hz_2097152sps.raw,raw,format=FLOAT,srate=2097152 -F /tmp/out.wav```\n\nRun:\n\n```docker run -ti iqtlabs/gamutrf-airspyfm -h```\n\nTo view other options.\n\n## Scanner testing\n\nCurrently, the scanner ```gain``` and sigfinder ```threshold``` must be set manually for the general RF environment (e.g. noisy/many signals versus quiet/few signals).\nTo establish the correct values and to confirm the scanner is working, initiate a scan over the 2.2-2.6GHz range. As the 2.4GHz spectrum is very busy with legacy WiFi\nand BlueTooth, the probability of seeing signals is high. If in an environment without BlueTooth or WiFi, an alternative is the FM broadcast band (88MHz to 108MHz).\n\nTo begin, commence scanning with just the scanner and sigfinder containers:\n\n```\n$ VOL_PREFIX=/tmp FREQ_START=2.2e9 FREQ_END=2.6e9 docker-compose -f orchestrator.yml up gamutrf sigfinder\n```\n\nWatch for ```/tmp/fft.png``` to appear, which should contain strong signals similar to this example:\n\n![2.4G example](fft24test.png)\n\nIf no or only small peaks appear which are not marked as peaks, increase ```gain``` (e.g., from 40 to 45) until peaks are detected.\n\nIf no peaks appear still, check antenna cabling, or choose a different scan range where signals are expected in your environment.\n\nIf peaks appear but are consistently not marked, decrease ```theshold``` (e.g. -25 to -35). If too many peaks are detected (noise detected as peaks), raise ```threshold.```\n\n## Troubleshooting\n\n#### Containers won\'t start using Ettus SDRs\n\nYou may see ```[ERROR] [USB] USB open failed: insufficient permissions``` on initial startup with Ettus SDRs. These devices download firmware and switch USB identities when first powered up. Restart the affected container to work around this.\n\n#### "O"s or warnings about overflows in SDR containers\n\n* Ensure your hardware can support the I/Q sample rate you have configured (gamutRF has been tested on Pi4 at 20Msps, which is the default recording rate). Also ensure your recording medium (e.g. flash drive, USB hard disk) is not timing out or blocking.\n* If using a Pi4, make sure you are using active cooling and an adequate power supply (no CPU throttling), and you are using a "blue" USB3 port.\n\n#### Scanner repeatedly logs "mean tuning step is greater than --samp-rate/2"\n\n* ```--sweep-sec``` may be too low (fast), or ```--samp-rate``` may be too low, causing non-overlapping FFT windows between retuning points.\n',
     'author': 'cglewis',
     'author_email': 'clewis@iqt.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `gamutrf-0.5.8/PKG-INFO` & `gamutrf-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamutrf
-Version: 0.5.8
+Version: 0.5.9
 Summary: An orchestrated SDR scanner
 License: Apache-2.0
 Author: cglewis
 Author-email: clewis@iqt.org
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,24 +15,24 @@
 Requires-Dist: RPi.GPIO (==0.7.1)
 Requires-Dist: bjoern (==3.2.2)
 Requires-Dist: cairocffi (>=1.3.0,<2.0.0)
 Requires-Dist: falcon (==3.1.1)
 Requires-Dist: falcon-cors (==1.1.7)
 Requires-Dist: gpsd-py3 (==0.3.0)
 Requires-Dist: httpx (==0.23.3)
-Requires-Dist: matplotlib (==3.6.2)
+Requires-Dist: matplotlib (==3.6.3)
 Requires-Dist: numpy (==1.24.1)
 Requires-Dist: paho-mqtt (==1.6.1)
-Requires-Dist: pandas (==1.5.2)
-Requires-Dist: prometheus_client (==0.15.0)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: prometheus_client (==0.16.0)
 Requires-Dist: pycairo (>=1.21.0,<2.0.0)
-Requires-Dist: requests (==2.28.1)
+Requires-Dist: requests (==2.28.2)
 Requires-Dist: schedule (==1.1.0)
 Requires-Dist: scipy (==1.10.0)
-Requires-Dist: sigmf (==1.0.0)
+Requires-Dist: sigmf (==1.1.0)
 Requires-Dist: zstandard (==0.19.0)
 Project-URL: homepage, https://github.com/IQTLabs/gamutRF
 Description-Content-Type: text/markdown
 
 # gamutRF
 
 An SDR orchestrated scanner and collector.
```

