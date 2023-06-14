# Comparing `tmp/amshan-2.1.1.tar.gz` & `tmp/amshan-2021.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amshan-2.1.1.tar", last modified: Wed Jun 14 20:39:27 2023, max compression
+gzip compressed data, was "amshan-2021.12.1.tar", last modified: Tue Dec 14 20:46:46 2021, max compression
```

## Comparing `amshan-2.1.1.tar` & `amshan-2021.12.1.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:39:27.129478 amshan-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 20:39:16.000000 amshan-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-14 20:39:27.129478 amshan-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-14 20:39:16.000000 amshan-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:39:27.125478 amshan-2.1.1/amshan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-14 20:39:27.000000 amshan-2.1.1/amshan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-14 20:39:27.000000 amshan-2.1.1/amshan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:39:27.000000 amshan-2.1.1/amshan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 20:39:27.000000 amshan-2.1.1/amshan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 20:39:27.000000 amshan-2.1.1/amshan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:39:27.129478 amshan-2.1.1/han/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 20:39:16.000000 amshan-2.1.1/han/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-14 20:39:16.000000 amshan-2.1.1/han/aidon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-14 20:39:16.000000 amshan-2.1.1/han/autodecoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-14 20:39:16.000000 amshan-2.1.1/han/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-14 20:39:16.000000 amshan-2.1.1/han/cosem.py
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-06-14 20:39:16.000000 amshan-2.1.1/han/dlde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-14 20:39:16.000000 amshan-2.1.1/han/fastframecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-06-14 20:39:16.000000 amshan-2.1.1/han/hdlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-14 20:39:16.000000 amshan-2.1.1/han/kaifa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-14 20:39:16.000000 amshan-2.1.1/han/kamstrup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-06-14 20:39:16.000000 amshan-2.1.1/han/meter_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-14 20:39:16.000000 amshan-2.1.1/han/obis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-14 20:39:16.000000 amshan-2.1.1/han/obis_map.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:39:16.000000 amshan-2.1.1/han/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-14 20:39:16.000000 amshan-2.1.1/han/serial_connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-14 20:39:16.000000 amshan-2.1.1/han/tcp_connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 20:39:27.129478 amshan-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-14 20:39:16.000000 amshan-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 20:46:46.927153 amshan-2021.12.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-12-14 20:46:32.000000 amshan-2021.12.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6531 2021-12-14 20:46:46.927153 amshan-2021.12.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5890 2021-12-14 20:46:32.000000 amshan-2021.12.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 20:46:46.927153 amshan-2021.12.1/amshan/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2912 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/aidon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2135 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/autodecoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7854 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/cosem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/fastframecheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16219 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/hdlc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4420 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/kaifa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/kamstrup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14147 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/meter_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2570 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/obis_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/serial_connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1885 2021-12-14 20:46:32.000000 amshan-2021.12.1/amshan/tcp_connection_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 20:46:46.927153 amshan-2021.12.1/amshan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6531 2021-12-14 20:46:46.000000 amshan-2021.12.1/amshan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-12-14 20:46:46.000000 amshan-2021.12.1/amshan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 20:46:46.000000 amshan-2021.12.1/amshan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-14 20:46:46.000000 amshan-2021.12.1/amshan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-14 20:46:46.000000 amshan-2021.12.1/amshan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-12-14 20:46:46.927153 amshan-2021.12.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-12-14 20:46:32.000000 amshan-2021.12.1/setup.py
```

### Comparing `amshan-2.1.1/LICENSE` & `amshan-2021.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amshan-2.1.1/PKG-INFO` & `amshan-2021.12.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 Metadata-Version: 2.1
 Name: amshan
-Version: 2.1.1
-Summary: Decode P1 and MBUS (Meter Bus) DLMS data. Special support for norwegian and swedish meters.
+Version: 2021.12.1
+Summary: Decode MBUS (Meter Bus) data with special support for norwegian AMS-smart meters (HAN port)
 Home-page: https://github.com/toreamun/amshan
 Author: Tore Amundsen
 Author-email: tore@amundsen.org
-Keywords: meter,han,ams,p1,mbus,aidon,kaifa,kamstrup,dlms,cosem,hdlc,fast frame check
+License: UNKNOWN
+Keywords: meter,han,ams,mbus,aidon,kaifa,kamstrup,cosem,hdlc,fast frame check
 Platform: POSIX
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: serial
 License-File: LICENSE
 
 [![GitHub Release](https://img.shields.io/github/release/toreamun/amshan?style=for-the-badge)](https://github.com/toreamun/amshan/releases)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/toreamun/amshan.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/toreamun/amshan/context:python)
 [![License](https://img.shields.io/github/license/toreamun/amshan?style=for-the-badge)](LICENSE)
 
 ![Project Maintenance](https://img.shields.io/badge/maintainer-Tore%20Amundsen%20%40toreamun-blue.svg?style=for-the-badge)
 [![buy me a coffee](https://img.shields.io/badge/If%20you%20like%20it-Buy%20me%20a%20coffee-orange.svg?style=for-the-badge)](https://www.buymeacoffee.com/toreamun)
 
 # AMSHAN
 
-Package to help decode smart power meter data stream of IEC 62056-21 Mode D P1 or DLMS/Cosem HDLC frames used by MBUS (Meter Bus). The package can both help reading frames of meter data and/or decoding them.
+Package to help decode smart power meter data stream of Cosem HDLC frames used by MBUS (Meter Bus). The package can both help reading frames of meter data and/or decoding them.
 
-The package has special support for DLMS formats used by Aidon, Kaifa and Kamstrup smart meteres (HAN) in Norway (See https://www.nek.no/info-ams-han-utviklere/) and Sweden. The Swedish P1 format format is also supported.
+The package has special support for formats used by Aidon, Kaifa and Kamstrum smart meteres (HAN) in Norway. See https://www.nek.no/info-ams-han-utviklere/
 
 ## Reading asynchronous from a stream of data
 
-SmartMeterMessagePayloadProtocol can be used to read smart meter P1 date readout (ascii) or MBUS HDLC (binary) frames asynchronous. The content of each mdssage (no headers and control characters) is passed as bytes to a Queue. Headers are checked and checksum validated, and only content from non empty frames with expected length (only DLMS) and checksum is passed to the queue.
+SmartMeterFrameContentProtocol can be used to read smart meter MBUS HDLC frames asynchronous. The content of each frame (no headers and control characters) is passed as bytes to a Queue. HDLC frame headers are checked and checksum validated, and only content from non empty frames with expected length and checksum is passed to the queue.
 
-SmartMeterMessageProtocol can be used to read smart meter P1 data readout (ascii) or MBUS HDLC frames asynchronous. The complete message is sent to a Queue as an instance of as subclass of MeterReaderBase. Frames are not validated. This class is a more low level alternative to SmartMeterMessagePayloadProtocol. This type has to be used to get the meter type from P1 readouts as this is part of the message "header".
+SmartMeterFrameProtocol can be used to read smart meter MBUS HDLC frames asynchronous. The complete fram is sent to a Queue as an instance of HdlcFrame. Frames are not validated. This class is a more low level alternative to SmartMeterFrameContentProtocol.
 
-Both SmartMeterMessagePayloadProtocol and SmartMeterMessageProtocol is a [Python asyncio protocol](https://docs.python.org/3/library/asyncio-protocol.html#protocols). Protocols support different types of transports like network and serial.
+Both SmartMeterFrameContentProtocol and SmartMeterFrameProtocol is a [Python asyncio protocol](https://docs.python.org/3/library/asyncio-protocol.html#protocols). Protocols support different types of transports like network and serial.
 
-It is recommended to use provided ConnectionManager and connection factories to read the data stream.
+It is recommended to use provided ConnectionManager and connection factories to read MBus meter data stream.
 
 ### Create protocol using transport
 
-Pass a factory for the selected protocol (SmartMeterMessagePayloadProtocol or SmartMeterMessageProtocol) to a utility function of your selected transport (e.g., EventLoop.create_connection() for TCP/IP or serial_asyncio.create_serial_connection() for serial).
+Pass a factory for the selected protocol (SmartMeterFrameContentProtocol or SmartMeterFrameProtocol) to a utility function of your selected transport (e.g., EventLoop.create_connection() for TCP/IP or serial_asyncio.create_serial_connection() for serial).
 
 Serial example:
 
 ```python
-transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessagePayloadProtocol(queue, [ModeDReader]), url = "/dev/tty01")
+transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameContentProtocol(queue), url = "/dev/tty01")
 ```
 
 Serial example:
 
 ```python
-transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessagePayloadProtocol(queue, [ModeDReader]), url = "/dev/tty01")
+transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameContentProtocol(queue), url = "/dev/tty01")
 ```
 
 ### Create protocol using provided factories
 
 Multiple factories are provided to create a protocol as an alternative to using selected transports create function as above. Use [serial_connection_factory](serial_connection_factory.py) for serial and [tcp_connection_factory](tcp_connection_factory) for TCP/IP.
 
-| Factory module            | SmartMeterMessageProtocol                  | SmartMeterMessagePayloadProtocol        |
-| ------------------------- | ------------------------------------------ | --------------------------------------- |
-| serial_connection_factory | create_serial_message_payload_connection() | create_serial_message_connection()      |
-| tcp_connection_factory    | create_tcp_message_connection()            | create_tcp_message_payload_connection() |
+| Factory module            | SmartMeterFrameProtocol                  | SmartMeterFrameContentProtocol   |
+| ------------------------- | ---------------------------------------- | -------------------------------- |
+| serial_connection_factory | create_serial_frame_content_connection() | create_serial_frame_connection() |
+| tcp_connection_factory    | create_tcp_frame_content_connection()    | create_tcp_frame_connection()    |
 
-Example of creating a SmartMeterMessagePayloadProtocol serial connection on device /dev/ttyUSB0:
+Example of creating a SmartMeterFrameContentProtocol serial connection on device /dev/ttyUSB0:
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-transport, protocol = await create_serial_frame_content_connection(queue, loop, None, url="/dev/ttyUSB0", baudrate=2400, parity=N)
+transport, protocol = await create_serial_frame_content_connection(queue, loop, url="/dev/ttyUSB0", baudrate=2400, parity=N)
 ```
 
-Example of creating a SmartMeterMessageProtocol protocol TCP/IP connection to host 192.168.1.1 on port 1234:
+Example of creating a SmartMeterFrameProtocol protocol TCP/IP connection to host 192.168.1.1 on port 1234:
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-transport, protocol = await create_tcp_frame_connection(queue, loop, None, "192.168.1.1", 1234)
+transport, protocol = await create_tcp_frame_connection(queue, loop, "192.168.1.1", 1234)
 ```
 
 See [reader_async.py](reader_async.py) for a complete example.
 
 ### Create resilient connection with ConnectionManager
 
 ConnectionManager maintain connection and reconnect if connection is lost. A back-off retry strategy is used when reconnecting, and a simple circuit breaker is used for lost connection.
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-connection_manager = ConnectionManager(lambda: create_serial_message_connection(queue, loop, None, url="/dev/ttyUSB0", baudrate=2400, parity=N))
+connection_manager = ConnectionManager(lambda: create_serial_frame_content_connection(queue, loop, url="/dev/ttyUSB0", baudrate=2400, parity=N))
 await connection_manager.connect_loop()
 ```
 
 See [reader_async.py](amshan/reader_async.py) for a complete example.
 
-## Parse P1 readouts directly from raw bytes
-
-dlde.ModeDReader can be used to read readout by readout from bytes. Call read() to read readouts as more bytes become available. The function takes bytes as an argument and returns a list of DataReadout (the list can be empty). The function can receive incomplete readout in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete readout are found and returned. You should check if returned readouts are valid with readout.is_valid before using them.
-
 ## Parse frames directly from raw bytes
 
-hdlc.HdlcFrameReader can be used to read frame by frame from bytes. Call read() to read frames as more bytes become available. The function takes bytes as an argument and returns a list of HdlcFrame (the list can be empty). The function can receive incomplete frames in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete frames are found and returned. You should check if returned frames are valid with frame.is_valid before using them.
+hdlc.HdlcFrameReader can be used to read frame by frame from bytes. Call read() to read frames as more bytes become available. The function takes bytes as an argument and returns a list of HdlcFrame (the list can be empty). The function can receive incomplete frames in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete frames are found and returned. You should check if returned frames are valid with frame.is_good_ffc and frame.is_expected_length before using them.
 
-# Decode norwegian and swedish messages
+# Decode norwegian HAN port frames
 
-P1 readout and MBUS frames using the norwegian or swedish DMLS AMS format can be parsed into meter specific objects or decoded into a common dictionary. Modules exists for P1 (generic format), Aidon, Kaifa and Kamstrup meters, but the easiest is to use [autodecoder.AutoDecode](han/autodecode.py) to automatically detect meter type and decode the frame into a dictionary. The dictionay content is as far as possible common between meters. Possible dictionary keys kan be found as constants in [obis_map.py](han/obis_map.py).
+MBUS frames using the norwegian AMS format can be parsed into meter specific objects or decoded into a common dictionary. Modules exists for Aidon, Kaifa and Kamstrup meters, but the easiest is to use [autodecoder.AutoDecode](amshan/autodecode.py) to automatically detect meter type and decode the frame into a dictionary. The dictionay content is as far as possible common between meters. Possible dictionary keys kan be found as constants in [obis_map.py](amshan/obis_map.py).
 
 Example:
 
 ```python
 decoder = AutoDecoder()
 frame = bytes.fromhex("e6e700" "0f" "40000000" "00" "0101" "020309060100010700ff060000011802020f00161b")
 decoded = decoder.decode_frame_content(frame)
 ```
+
+
```

### Comparing `amshan-2.1.1/README.md` & `amshan-2021.12.1/amshan.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,115 @@
+Metadata-Version: 2.1
+Name: amshan
+Version: 2021.12.1
+Summary: Decode MBUS (Meter Bus) data with special support for norwegian AMS-smart meters (HAN port)
+Home-page: https://github.com/toreamun/amshan
+Author: Tore Amundsen
+Author-email: tore@amundsen.org
+License: UNKNOWN
+Keywords: meter,han,ams,mbus,aidon,kaifa,kamstrup,cosem,hdlc,fast frame check
+Platform: POSIX
+Platform: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: serial
+License-File: LICENSE
+
 [![GitHub Release](https://img.shields.io/github/release/toreamun/amshan?style=for-the-badge)](https://github.com/toreamun/amshan/releases)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/toreamun/amshan.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/toreamun/amshan/context:python)
 [![License](https://img.shields.io/github/license/toreamun/amshan?style=for-the-badge)](LICENSE)
 
 ![Project Maintenance](https://img.shields.io/badge/maintainer-Tore%20Amundsen%20%40toreamun-blue.svg?style=for-the-badge)
 [![buy me a coffee](https://img.shields.io/badge/If%20you%20like%20it-Buy%20me%20a%20coffee-orange.svg?style=for-the-badge)](https://www.buymeacoffee.com/toreamun)
 
 # AMSHAN
 
-Package to help decode smart power meter data stream of IEC 62056-21 Mode D P1 or DLMS/Cosem HDLC frames used by MBUS (Meter Bus). The package can both help reading frames of meter data and/or decoding them.
+Package to help decode smart power meter data stream of Cosem HDLC frames used by MBUS (Meter Bus). The package can both help reading frames of meter data and/or decoding them.
 
-The package has special support for DLMS formats used by Aidon, Kaifa and Kamstrup smart meteres (HAN) in Norway (See https://www.nek.no/info-ams-han-utviklere/) and Sweden. The Swedish P1 format format is also supported.
+The package has special support for formats used by Aidon, Kaifa and Kamstrum smart meteres (HAN) in Norway. See https://www.nek.no/info-ams-han-utviklere/
 
 ## Reading asynchronous from a stream of data
 
-SmartMeterMessagePayloadProtocol can be used to read smart meter P1 date readout (ascii) or MBUS HDLC (binary) frames asynchronous. The content of each mdssage (no headers and control characters) is passed as bytes to a Queue. Headers are checked and checksum validated, and only content from non empty frames with expected length (only DLMS) and checksum is passed to the queue.
+SmartMeterFrameContentProtocol can be used to read smart meter MBUS HDLC frames asynchronous. The content of each frame (no headers and control characters) is passed as bytes to a Queue. HDLC frame headers are checked and checksum validated, and only content from non empty frames with expected length and checksum is passed to the queue.
 
-SmartMeterMessageProtocol can be used to read smart meter P1 data readout (ascii) or MBUS HDLC frames asynchronous. The complete message is sent to a Queue as an instance of as subclass of MeterReaderBase. Frames are not validated. This class is a more low level alternative to SmartMeterMessagePayloadProtocol. This type has to be used to get the meter type from P1 readouts as this is part of the message "header".
+SmartMeterFrameProtocol can be used to read smart meter MBUS HDLC frames asynchronous. The complete fram is sent to a Queue as an instance of HdlcFrame. Frames are not validated. This class is a more low level alternative to SmartMeterFrameContentProtocol.
 
-Both SmartMeterMessagePayloadProtocol and SmartMeterMessageProtocol is a [Python asyncio protocol](https://docs.python.org/3/library/asyncio-protocol.html#protocols). Protocols support different types of transports like network and serial.
+Both SmartMeterFrameContentProtocol and SmartMeterFrameProtocol is a [Python asyncio protocol](https://docs.python.org/3/library/asyncio-protocol.html#protocols). Protocols support different types of transports like network and serial.
 
-It is recommended to use provided ConnectionManager and connection factories to read the data stream.
+It is recommended to use provided ConnectionManager and connection factories to read MBus meter data stream.
 
 ### Create protocol using transport
 
-Pass a factory for the selected protocol (SmartMeterMessagePayloadProtocol or SmartMeterMessageProtocol) to a utility function of your selected transport (e.g., EventLoop.create_connection() for TCP/IP or serial_asyncio.create_serial_connection() for serial).
+Pass a factory for the selected protocol (SmartMeterFrameContentProtocol or SmartMeterFrameProtocol) to a utility function of your selected transport (e.g., EventLoop.create_connection() for TCP/IP or serial_asyncio.create_serial_connection() for serial).
 
 Serial example:
 
 ```python
-transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessagePayloadProtocol(queue, [ModeDReader]), url = "/dev/tty01")
+transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameContentProtocol(queue), url = "/dev/tty01")
 ```
 
 Serial example:
 
 ```python
-transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessagePayloadProtocol(queue, [ModeDReader]), url = "/dev/tty01")
+transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameContentProtocol(queue), url = "/dev/tty01")
 ```
 
 ### Create protocol using provided factories
 
 Multiple factories are provided to create a protocol as an alternative to using selected transports create function as above. Use [serial_connection_factory](serial_connection_factory.py) for serial and [tcp_connection_factory](tcp_connection_factory) for TCP/IP.
 
-| Factory module            | SmartMeterMessageProtocol                  | SmartMeterMessagePayloadProtocol        |
-| ------------------------- | ------------------------------------------ | --------------------------------------- |
-| serial_connection_factory | create_serial_message_payload_connection() | create_serial_message_connection()      |
-| tcp_connection_factory    | create_tcp_message_connection()            | create_tcp_message_payload_connection() |
+| Factory module            | SmartMeterFrameProtocol                  | SmartMeterFrameContentProtocol   |
+| ------------------------- | ---------------------------------------- | -------------------------------- |
+| serial_connection_factory | create_serial_frame_content_connection() | create_serial_frame_connection() |
+| tcp_connection_factory    | create_tcp_frame_content_connection()    | create_tcp_frame_connection()    |
 
-Example of creating a SmartMeterMessagePayloadProtocol serial connection on device /dev/ttyUSB0:
+Example of creating a SmartMeterFrameContentProtocol serial connection on device /dev/ttyUSB0:
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-transport, protocol = await create_serial_frame_content_connection(queue, loop, None, url="/dev/ttyUSB0", baudrate=2400, parity=N)
+transport, protocol = await create_serial_frame_content_connection(queue, loop, url="/dev/ttyUSB0", baudrate=2400, parity=N)
 ```
 
-Example of creating a SmartMeterMessageProtocol protocol TCP/IP connection to host 192.168.1.1 on port 1234:
+Example of creating a SmartMeterFrameProtocol protocol TCP/IP connection to host 192.168.1.1 on port 1234:
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-transport, protocol = await create_tcp_frame_connection(queue, loop, None, "192.168.1.1", 1234)
+transport, protocol = await create_tcp_frame_connection(queue, loop, "192.168.1.1", 1234)
 ```
 
 See [reader_async.py](reader_async.py) for a complete example.
 
 ### Create resilient connection with ConnectionManager
 
 ConnectionManager maintain connection and reconnect if connection is lost. A back-off retry strategy is used when reconnecting, and a simple circuit breaker is used for lost connection.
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-connection_manager = ConnectionManager(lambda: create_serial_message_connection(queue, loop, None, url="/dev/ttyUSB0", baudrate=2400, parity=N))
+connection_manager = ConnectionManager(lambda: create_serial_frame_content_connection(queue, loop, url="/dev/ttyUSB0", baudrate=2400, parity=N))
 await connection_manager.connect_loop()
 ```
 
 See [reader_async.py](amshan/reader_async.py) for a complete example.
 
-## Parse P1 readouts directly from raw bytes
-
-dlde.ModeDReader can be used to read readout by readout from bytes. Call read() to read readouts as more bytes become available. The function takes bytes as an argument and returns a list of DataReadout (the list can be empty). The function can receive incomplete readout in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete readout are found and returned. You should check if returned readouts are valid with readout.is_valid before using them.
-
 ## Parse frames directly from raw bytes
 
-hdlc.HdlcFrameReader can be used to read frame by frame from bytes. Call read() to read frames as more bytes become available. The function takes bytes as an argument and returns a list of HdlcFrame (the list can be empty). The function can receive incomplete frames in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete frames are found and returned. You should check if returned frames are valid with frame.is_valid before using them.
+hdlc.HdlcFrameReader can be used to read frame by frame from bytes. Call read() to read frames as more bytes become available. The function takes bytes as an argument and returns a list of HdlcFrame (the list can be empty). The function can receive incomplete frames in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete frames are found and returned. You should check if returned frames are valid with frame.is_good_ffc and frame.is_expected_length before using them.
 
-# Decode norwegian and swedish messages
+# Decode norwegian HAN port frames
 
-P1 readout and MBUS frames using the norwegian or swedish DMLS AMS format can be parsed into meter specific objects or decoded into a common dictionary. Modules exists for P1 (generic format), Aidon, Kaifa and Kamstrup meters, but the easiest is to use [autodecoder.AutoDecode](han/autodecode.py) to automatically detect meter type and decode the frame into a dictionary. The dictionay content is as far as possible common between meters. Possible dictionary keys kan be found as constants in [obis_map.py](han/obis_map.py).
+MBUS frames using the norwegian AMS format can be parsed into meter specific objects or decoded into a common dictionary. Modules exists for Aidon, Kaifa and Kamstrup meters, but the easiest is to use [autodecoder.AutoDecode](amshan/autodecode.py) to automatically detect meter type and decode the frame into a dictionary. The dictionay content is as far as possible common between meters. Possible dictionary keys kan be found as constants in [obis_map.py](amshan/obis_map.py).
 
 Example:
 
 ```python
 decoder = AutoDecoder()
 frame = bytes.fromhex("e6e700" "0f" "40000000" "00" "0101" "020309060100010700ff060000011802020f00161b")
 decoded = decoder.decode_frame_content(frame)
 ```
+
+
```

### Comparing `amshan-2.1.1/amshan.egg-info/PKG-INFO` & `amshan-2021.12.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,93 @@
-Metadata-Version: 2.1
-Name: amshan
-Version: 2.1.1
-Summary: Decode P1 and MBUS (Meter Bus) DLMS data. Special support for norwegian and swedish meters.
-Home-page: https://github.com/toreamun/amshan
-Author: Tore Amundsen
-Author-email: tore@amundsen.org
-Keywords: meter,han,ams,p1,mbus,aidon,kaifa,kamstrup,dlms,cosem,hdlc,fast frame check
-Platform: POSIX
-Platform: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: serial
-License-File: LICENSE
-
 [![GitHub Release](https://img.shields.io/github/release/toreamun/amshan?style=for-the-badge)](https://github.com/toreamun/amshan/releases)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/toreamun/amshan.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/toreamun/amshan/context:python)
 [![License](https://img.shields.io/github/license/toreamun/amshan?style=for-the-badge)](LICENSE)
 
 ![Project Maintenance](https://img.shields.io/badge/maintainer-Tore%20Amundsen%20%40toreamun-blue.svg?style=for-the-badge)
 [![buy me a coffee](https://img.shields.io/badge/If%20you%20like%20it-Buy%20me%20a%20coffee-orange.svg?style=for-the-badge)](https://www.buymeacoffee.com/toreamun)
 
 # AMSHAN
 
-Package to help decode smart power meter data stream of IEC 62056-21 Mode D P1 or DLMS/Cosem HDLC frames used by MBUS (Meter Bus). The package can both help reading frames of meter data and/or decoding them.
+Package to help decode smart power meter data stream of Cosem HDLC frames used by MBUS (Meter Bus). The package can both help reading frames of meter data and/or decoding them.
 
-The package has special support for DLMS formats used by Aidon, Kaifa and Kamstrup smart meteres (HAN) in Norway (See https://www.nek.no/info-ams-han-utviklere/) and Sweden. The Swedish P1 format format is also supported.
+The package has special support for formats used by Aidon, Kaifa and Kamstrum smart meteres (HAN) in Norway. See https://www.nek.no/info-ams-han-utviklere/
 
 ## Reading asynchronous from a stream of data
 
-SmartMeterMessagePayloadProtocol can be used to read smart meter P1 date readout (ascii) or MBUS HDLC (binary) frames asynchronous. The content of each mdssage (no headers and control characters) is passed as bytes to a Queue. Headers are checked and checksum validated, and only content from non empty frames with expected length (only DLMS) and checksum is passed to the queue.
+SmartMeterFrameContentProtocol can be used to read smart meter MBUS HDLC frames asynchronous. The content of each frame (no headers and control characters) is passed as bytes to a Queue. HDLC frame headers are checked and checksum validated, and only content from non empty frames with expected length and checksum is passed to the queue.
 
-SmartMeterMessageProtocol can be used to read smart meter P1 data readout (ascii) or MBUS HDLC frames asynchronous. The complete message is sent to a Queue as an instance of as subclass of MeterReaderBase. Frames are not validated. This class is a more low level alternative to SmartMeterMessagePayloadProtocol. This type has to be used to get the meter type from P1 readouts as this is part of the message "header".
+SmartMeterFrameProtocol can be used to read smart meter MBUS HDLC frames asynchronous. The complete fram is sent to a Queue as an instance of HdlcFrame. Frames are not validated. This class is a more low level alternative to SmartMeterFrameContentProtocol.
 
-Both SmartMeterMessagePayloadProtocol and SmartMeterMessageProtocol is a [Python asyncio protocol](https://docs.python.org/3/library/asyncio-protocol.html#protocols). Protocols support different types of transports like network and serial.
+Both SmartMeterFrameContentProtocol and SmartMeterFrameProtocol is a [Python asyncio protocol](https://docs.python.org/3/library/asyncio-protocol.html#protocols). Protocols support different types of transports like network and serial.
 
-It is recommended to use provided ConnectionManager and connection factories to read the data stream.
+It is recommended to use provided ConnectionManager and connection factories to read MBus meter data stream.
 
 ### Create protocol using transport
 
-Pass a factory for the selected protocol (SmartMeterMessagePayloadProtocol or SmartMeterMessageProtocol) to a utility function of your selected transport (e.g., EventLoop.create_connection() for TCP/IP or serial_asyncio.create_serial_connection() for serial).
+Pass a factory for the selected protocol (SmartMeterFrameContentProtocol or SmartMeterFrameProtocol) to a utility function of your selected transport (e.g., EventLoop.create_connection() for TCP/IP or serial_asyncio.create_serial_connection() for serial).
 
 Serial example:
 
 ```python
-transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessagePayloadProtocol(queue, [ModeDReader]), url = "/dev/tty01")
+transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameContentProtocol(queue), url = "/dev/tty01")
 ```
 
 Serial example:
 
 ```python
-transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessagePayloadProtocol(queue, [ModeDReader]), url = "/dev/tty01")
+transport, protocol = await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameContentProtocol(queue), url = "/dev/tty01")
 ```
 
 ### Create protocol using provided factories
 
 Multiple factories are provided to create a protocol as an alternative to using selected transports create function as above. Use [serial_connection_factory](serial_connection_factory.py) for serial and [tcp_connection_factory](tcp_connection_factory) for TCP/IP.
 
-| Factory module            | SmartMeterMessageProtocol                  | SmartMeterMessagePayloadProtocol        |
-| ------------------------- | ------------------------------------------ | --------------------------------------- |
-| serial_connection_factory | create_serial_message_payload_connection() | create_serial_message_connection()      |
-| tcp_connection_factory    | create_tcp_message_connection()            | create_tcp_message_payload_connection() |
+| Factory module            | SmartMeterFrameProtocol                  | SmartMeterFrameContentProtocol   |
+| ------------------------- | ---------------------------------------- | -------------------------------- |
+| serial_connection_factory | create_serial_frame_content_connection() | create_serial_frame_connection() |
+| tcp_connection_factory    | create_tcp_frame_content_connection()    | create_tcp_frame_connection()    |
 
-Example of creating a SmartMeterMessagePayloadProtocol serial connection on device /dev/ttyUSB0:
+Example of creating a SmartMeterFrameContentProtocol serial connection on device /dev/ttyUSB0:
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-transport, protocol = await create_serial_frame_content_connection(queue, loop, None, url="/dev/ttyUSB0", baudrate=2400, parity=N)
+transport, protocol = await create_serial_frame_content_connection(queue, loop, url="/dev/ttyUSB0", baudrate=2400, parity=N)
 ```
 
-Example of creating a SmartMeterMessageProtocol protocol TCP/IP connection to host 192.168.1.1 on port 1234:
+Example of creating a SmartMeterFrameProtocol protocol TCP/IP connection to host 192.168.1.1 on port 1234:
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-transport, protocol = await create_tcp_frame_connection(queue, loop, None, "192.168.1.1", 1234)
+transport, protocol = await create_tcp_frame_connection(queue, loop, "192.168.1.1", 1234)
 ```
 
 See [reader_async.py](reader_async.py) for a complete example.
 
 ### Create resilient connection with ConnectionManager
 
 ConnectionManager maintain connection and reconnect if connection is lost. A back-off retry strategy is used when reconnecting, and a simple circuit breaker is used for lost connection.
 
 ```python
 queue = Queue()
 loop = asyncio.get_event_loop()
-connection_manager = ConnectionManager(lambda: create_serial_message_connection(queue, loop, None, url="/dev/ttyUSB0", baudrate=2400, parity=N))
+connection_manager = ConnectionManager(lambda: create_serial_frame_content_connection(queue, loop, url="/dev/ttyUSB0", baudrate=2400, parity=N))
 await connection_manager.connect_loop()
 ```
 
 See [reader_async.py](amshan/reader_async.py) for a complete example.
 
-## Parse P1 readouts directly from raw bytes
-
-dlde.ModeDReader can be used to read readout by readout from bytes. Call read() to read readouts as more bytes become available. The function takes bytes as an argument and returns a list of DataReadout (the list can be empty). The function can receive incomplete readout in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete readout are found and returned. You should check if returned readouts are valid with readout.is_valid before using them.
-
 ## Parse frames directly from raw bytes
 
-hdlc.HdlcFrameReader can be used to read frame by frame from bytes. Call read() to read frames as more bytes become available. The function takes bytes as an argument and returns a list of HdlcFrame (the list can be empty). The function can receive incomplete frames in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete frames are found and returned. You should check if returned frames are valid with frame.is_valid before using them.
+hdlc.HdlcFrameReader can be used to read frame by frame from bytes. Call read() to read frames as more bytes become available. The function takes bytes as an argument and returns a list of HdlcFrame (the list can be empty). The function can receive incomplete frames in the buffer input and add incomplete data to an internal buffer. The buffer is schrinked when complete frames are found and returned. You should check if returned frames are valid with frame.is_good_ffc and frame.is_expected_length before using them.
 
-# Decode norwegian and swedish messages
+# Decode norwegian HAN port frames
 
-P1 readout and MBUS frames using the norwegian or swedish DMLS AMS format can be parsed into meter specific objects or decoded into a common dictionary. Modules exists for P1 (generic format), Aidon, Kaifa and Kamstrup meters, but the easiest is to use [autodecoder.AutoDecode](han/autodecode.py) to automatically detect meter type and decode the frame into a dictionary. The dictionay content is as far as possible common between meters. Possible dictionary keys kan be found as constants in [obis_map.py](han/obis_map.py).
+MBUS frames using the norwegian AMS format can be parsed into meter specific objects or decoded into a common dictionary. Modules exists for Aidon, Kaifa and Kamstrup meters, but the easiest is to use [autodecoder.AutoDecode](amshan/autodecode.py) to automatically detect meter type and decode the frame into a dictionary. The dictionay content is as far as possible common between meters. Possible dictionary keys kan be found as constants in [obis_map.py](amshan/obis_map.py).
 
 Example:
 
 ```python
 decoder = AutoDecoder()
 frame = bytes.fromhex("e6e700" "0f" "40000000" "00" "0101" "020309060100010700ff060000011802020f00161b")
 decoded = decoder.decode_frame_content(frame)
```

### Comparing `amshan-2.1.1/han/cosem.py` & `amshan-2021.12.1/amshan/cosem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """Contruct declarations for some COSEM types and structures."""
-# pylint: disable=protected-access
-from __future__ import annotations
-
 import datetime
 from decimal import Decimal
 from typing import Any
 
 import construct  # type: ignore
 
 # See COSEM blue Book table 2 (Common data types) in section 4.1.5 Common data types
@@ -52,14 +49,31 @@
 
 ObisCode = construct.ExprAdapter(
     construct.Int8ub[6],
     decoder=lambda obj, ctx: ".".join(f"{b}" for b in obj),
     encoder=lambda obj, ctx: [int(part) for part in obj.split(".")],
 )
 
+
+def _type_code_to_type(
+    type_code: construct.Enum,
+) -> Any:
+    return construct.Switch(
+        type_code,
+        {
+            CommonDataTypes.integer: Integer,
+            CommonDataTypes.long: Long,
+            CommonDataTypes.long_unsigned: LongUnsigned,
+            CommonDataTypes.double_long_unsigned: DoubleLongUnsigned,
+            CommonDataTypes.visible_string: VisibleString,
+        },
+        default=construct.Error,
+    )
+
+
 OptionalDateTimeByte = construct.ExprAdapter(
     construct.Int8ub,
     decoder=lambda obj, ctx: obj if obj != 0xFF else None,
     encoder=lambda obj, ctx: obj if obj is not None else 0xFF,
 )
 
 # See COSEM blue Book section 4.1.6.1 Date and time formats
@@ -74,52 +88,26 @@
     "second" / OptionalDateTimeByte,
     "hundredths_of_second" / OptionalDateTimeByte,
     "deviation"
     / construct.ExprAdapter(
         construct.Int16sb,
         decoder=lambda obj, ctx: obj if obj != -0x8000 else None,
         encoder=lambda obj, ctx: obj if obj is not None else -0x8000,
-    )
-    * ("Range -720...+720 in minutes of local time to UTC. 0x8000 = not specified"),
+    ),
     "clock_status_byte" / construct.Peek(OptionalDateTimeByte),
     "clock_status"
     / construct.If(
         construct.this.clock_status_byte != 0xFF,
         construct.BitStruct(
-            "invalid_value"
-            / construct.BitsInteger(1)
-            * (
-                "Time could not be recovered after an incident. Detailed conditions are "
-                "manufacturer specific (for example after the power to the clock has been "
-                "interrupted). For a valid status, bit 0 shall not be set if bit 1 is set."
-            ),
-            "doubtful_value"
-            / construct.BitsInteger(1)
-            * (
-                "Time could be recovered after an incident but the value cannot be guaranteed. "
-                "Detailed conditions are manufacturer specific. For a valid status, bit 1 shall "
-                "not be set if bit 0 is set."
-            ),
-            "different_clock_base"
-            / construct.BitsInteger(1)
-            * (
-                "Bit is set if the basic timing information for the clock at the actual moment "
-                "is taken from a timing source different from the source specified in clock_base."
-            ),
-            "invalid_clock_status"
-            / construct.BitsInteger(1)
-            * (
-                "This bit indicates that at least one bit of the clock status is invalid. "
-                "Some bits may be correct. The exact meaning shall be explained in the "
-                "manufacturer's documentation."
-            ),
+            "invalid_value" / construct.BitsInteger(1),
+            "doubtful_value" / construct.BitsInteger(1),
+            "different_clock_base" / construct.BitsInteger(1),
+            "invalid_clock_status" / construct.BitsInteger(1),
             construct.BitsInteger(3),
-            "daylight_saving_active"
-            / construct.BitsInteger(1)
-            * "Flag set to true: the transmitted time contains the daylight saving deviation (summer time).",
+            "daylight_saving_active" / construct.BitsInteger(1),
         ),
     ),
     construct.If(construct.this.clock_status_byte == 0xFF, construct.Int8ub),
     "datetime"
     / construct.Computed(
         lambda ctx: datetime.datetime(
             ctx.year,
@@ -127,55 +115,23 @@
             ctx.day_of_month,
             ctx.hour,
             ctx.minute,
             ctx.second,
             ctx.hundredths_of_second * 10000
             if ctx.hundredths_of_second is not None
             else 0,
-            datetime.timezone(datetime.timedelta(minutes=ctx.deviation * -1))
+            datetime.timezone(datetime.timedelta(minutes=ctx.deviation))
             if ctx.deviation is not None
             else None,
         )
     ),
 )
 
-NullData: construct.Struct = construct.Struct(
-    "_null_peek" / construct.Peek(CommonDataTypes),
-    "value"
-    / construct.If(
-        CommonDataTypes.null_data == construct.this._null_peek,
-        construct.GreedyRange(
-            construct.Const(CommonDataTypes.null_data, CommonDataTypes)
-        ),
-    ),
-)
-
-
 # field types
 
-
-def _type_code_to_type(
-    type_code: construct.Enum,
-) -> Any:
-    """Map COSEM common data type codes to type."""
-    return construct.Switch(
-        type_code,
-        {
-            CommonDataTypes.null_data: NullData,
-            CommonDataTypes.integer: Integer,
-            CommonDataTypes.long: Long,
-            CommonDataTypes.long_unsigned: LongUnsigned,
-            CommonDataTypes.double_long_unsigned: DoubleLongUnsigned,
-            CommonDataTypes.octet_string: construct.Select(DateTime, OctedStringText),
-            CommonDataTypes.visible_string: VisibleString,
-        },
-        default=construct.Error,
-    )
-
-
 Field = construct.FocusedSeq(
     "value",
     "content_type" / CommonDataTypes,
     "value" / _type_code_to_type(construct.this.content_type),
 )
 
 ObisCodeOctedStringField = construct.FocusedSeq(
@@ -247,38 +203,35 @@
         lambda ctx: ctx.content_type
         in (CommonDataTypes.null_data, CommonDataTypes.octet_string)
     ),
     "value"
     / construct.If(construct.this.content_type != CommonDataTypes.null_data, DateTime),
 )
 
-
 LongInvokeIdAndPriority = construct.BitStruct(
-    "invoke_id" / construct.BitsInteger(24),
+    "invoke-id" / construct.BitsInteger(24),
     construct.Padding(4),
-    "self_descriptive"
+    "self-descriptive"
     / construct.Enum(construct.BitsInteger(1), NotSelfDescriptive=0, SelfDescriptive=1),
-    "processing_option"
+    "processing-option"
     / construct.Enum(construct.BitsInteger(1), ContinueOnError=0, BreakOnError=1),
-    "service_class"
+    "service-class"
     / construct.Enum(construct.BitsInteger(1), Unconfirmed=0, Confirmed=1),
     "priority" / construct.Enum(construct.BitsInteger(1), Normal=0, High=1),
 )
 
-ApduTag = construct.Enum(construct.Int8ub, data_notification=0x0F)
-
 
-def _get_apdu_struct(notification_body: construct.Struct) -> construct.Struct:
+def _get_apdpu_struct(notification_body: construct.Struct) -> construct.Struct:
     return construct.Struct(
-        "Tag" / ApduTag,
+        "Tag" / construct.Int8ub,
         "LongInvokeIdAndPriority" / LongInvokeIdAndPriority,
         "_datetimestartbyte" / construct.Peek(CommonDataTypes),
         "DateTime"
         / construct.Switch(
-            construct.this._datetimestartbyte,
+            construct.this._datetimestartbyte,  # pylint: disable=protected-access
             {
                 CommonDataTypes.null_data: construct.Byte,
                 CommonDataTypes.octet_string: DateTimeField,
             },
             default=DateTime,
         ),
         "notification_body" / notification_body,
@@ -287,9 +240,9 @@
 
 def get_llc_pdu_struct(notification_body: construct.Struct) -> construct.Struct:
     """Get a LLC PDU struct wrapping supplied notification body."""
     return construct.Struct(
         "dsap" / construct.Int8ub,
         "ssap" / construct.Int8ub,
         "control" / construct.Int8ub,
-        "information" / _get_apdu_struct(notification_body),
+        "information" / _get_apdpu_struct(notification_body),
     )
```

### Comparing `amshan-2.1.1/han/fastframecheck.py` & `amshan-2021.12.1/amshan/fastframecheck.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Compute or check checksum using a 16-bit Fast Frame Check Sequence (FCS) derived from RFC1662."""
-from __future__ import annotations
+from typing import List
 
 
-def _compute_fcs_16_crc_table() -> list[int]:
+def _compute_fcs_16_crc_table() -> List[int]:
     """Generate a FCS-16 table."""
     polynomial = 0x8408  # The FCS-16 generator polynomial: x**0 + x**5 + x**12 + x**16.
     crc_table = [] * 256
     for byte in range(256):
         crc = 0
         for _ in range(8):
             if (byte ^ crc) & 1:
```

### Comparing `amshan-2.1.1/han/hdlc.py` & `amshan-2021.12.1/amshan/hdlc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,190 +1,187 @@
 """Use this module to read HDLC frames."""
-from __future__ import annotations
-
 import logging
-from typing import cast
+from typing import List, Optional, cast
 
-from han import fastframecheck
-from han.common import MeterMessageBase, MeterMessageType, MeterReaderBase
+from amshan import fastframecheck
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class HdlcFrameHeader:
     """The start (header) of an HdlcFrame."""
 
-    def __init__(self, frame: HdlcFrame) -> None:
+    def __init__(self, frame: "HdlcFrame") -> None:
         """
         Initialize header.
 
         Used by parent frame.
         """
         self._frame: HdlcFrame = frame
-        self._control_position: int | None = None
-        self._is_header_good: bool | None = None
+        self._control_position: Optional[int] = None
+        self._is_header_good: Optional[bool] = None
 
     def update(self) -> None:
         """Update fields when more frame data has been read. Used by parent HdlcFrame."""
         if self._control_position is None and len(self._frame) > 3:
             self._control_position = self._get_control_field_position()
 
         if self._control_position is not None:
             if self._is_header_good is None:
                 if len(self._frame) == self._control_position + 3:
                     self._is_header_good = self._frame.is_good_ffc
 
     @property
-    def frame_format(self) -> int | None:
+    def frame_format(self) -> Optional[int]:
         """Return the value of frame format if the value has been read."""
         # The length of the frame format field is two bytes. It consists of three sub-fields referred to as the Format
         # type sub-field (4 bit), the Segmentation bit (S, 1 bit) and the frame length sub-field (11 bit).
         if len(self._frame) >= 2:
-            return self._frame.as_bytes[0] << 8 | self._frame.as_bytes[1]
+            return self._frame.frame_data[0] << 8 | self._frame.frame_data[1]
         return None
 
     @property
-    def frame_format_type(self) -> int | None:
+    def frame_format_type(self) -> Optional[int]:
         """Return the value of frame format type sub-field when frame format has been read."""
         if self.frame_format is not None:
             return (self.frame_format >> 12) & 0b1111
         return None
 
     @property
-    def segmentation(self) -> bool | None:
+    def segmentation(self) -> Optional[bool]:
         """Return the value of frame format Segmentation flag when frame format has been read."""
         if self.frame_format is not None:
             return ((self.frame_format >> 11) & 0x1) == 0x1
         return None
 
     @property
-    def frame_length(self) -> int | None:
+    def frame_length(self) -> Optional[int]:
         """
         Return the value of frame format length sub-field when frame format has been read.
 
         The value of the frame length subfield is the count of octets in the frame
         excluding the opening and closing frame flag sequences.
         """
         if self.frame_format is not None:
             return self.frame_format & 0b11111111111
         return None
 
     @property
-    def destination_address(self) -> bytes | None:
+    def destination_address(self) -> Optional[bytes]:
         """
         Return the value of destination address when the field has been read.
 
         Depending on the direction of the data transfer, both the client and the server addresses can
         be destination or source addresses.
 
         The client address shall always be expressed on one byte.
         """
         if len(self._frame) >= 2:
             return self._get_address(2)
         return None
 
     @property
-    def source_address(self) -> bytes | None:
+    def source_address(self) -> Optional[bytes]:
         """
         Return the value of source address when the field has been read.
 
         Depending on the direction of the data transfer, both the client and the server addresses can
         be destination or source addresses.
 
         The client address shall always be expressed on one byte.
         """
         destination_adr = self.destination_address
         if destination_adr is not None:
             return self._get_address(2 + len(destination_adr))
         return None
 
     @property
-    def control(self) -> int | None:
+    def control(self) -> Optional[int]:
         """
         Return the value of control field when the field has been read.
 
         It indicates the type of commands or responses,
         and contains sequence numbers, where appropriate (frames I, RR and RNR).
         """
         is_available = (
             self._control_position is not None
             and len(self._frame) > self._control_position
         )
         if is_available:
-            return self._frame.as_bytes[cast(int, self._control_position)]
+            return self._frame.frame_data[cast(int, self._control_position)]
         return None
 
     @property
-    def header_check_sequence(self) -> int | None:
+    def header_check_sequence(self) -> Optional[int]:
         """
         Header check sequence (HCS) field when the field has been read.
 
         This check sequence is applied to only the header,
         i.e., the bits between the opening flag sequence and the header check sequence.
         """
         is_available = (
             self._control_position is not None
             and len(self._frame) > self._control_position + 2
         )
         if is_available:
             return (
-                self._frame.as_bytes[cast(int, self._control_position) + 1] << 8
-                | self._frame.as_bytes[cast(int, self._control_position) + 2]
+                self._frame.frame_data[cast(int, self._control_position) + 1] << 8
+                | self._frame.frame_data[cast(int, self._control_position) + 2]
             )
         return None
 
     @property
-    def information_position(self) -> int | None:
+    def information_position(self) -> Optional[int]:
         """
         Information field position when the field position is known and is available.
 
         Frames that do not have an information field or have an empty information field,
         e.g., as with some supervisory frames, do not contain an HCS and FCS, only an FCS.
         """
         if self._control_position is not None:
             return self._control_position + 3
         return None
 
-    def _get_address(self, position: int) -> bytes | None:
+    def _get_address(self, position: int) -> Optional[bytes]:
         """Get variable length address from position."""
         # As specified in ISO/IEC 13239:2002, 4.7.1, The address field range can be extended by reserving the first
         # transmitted bit (low-order) of each address octet which would then be set to binary zero to indicate that
         # the following octet is an extension of the address field. The format of the extended octet(s) shall be the
         # same as that of the first octet. Thus, the address field may be recursively extended. The last octet of an
         # address field is indicted by setting the low-order bit to binary one.
 
         if len(self._frame) > position:
             adr = bytearray()
 
             i = position
-            frame_data = self._frame.as_bytes
+            frame_data = self._frame.frame_data
             while True:
                 if i >= len(self._frame):
                     return None
 
                 current = frame_data[i]
                 adr.append(current)
 
                 if (current & 0x01) == 0x01:
                     return bytes(adr)
 
                 i += 1
 
         return None
 
-    def _get_control_field_position(self) -> int | None:
+    def _get_control_field_position(self) -> Optional[int]:
         destination_adr = self.destination_address
         if destination_adr is not None:
             source_adr = self.source_address
             if source_adr is not None:
                 return 2 + len(destination_adr) + len(source_adr)
         return None
 
 
-class HdlcFrame(MeterMessageBase):
+class HdlcFrame:
     """
     Use this class to read HDLC frames by calling append for each byte.
 
     is_good is true when checksum is ok. This can be the case both when header is read
     and when done reading information.
     """
 
@@ -209,34 +206,15 @@
     def append(self, byte: int) -> None:
         """Append byte to frame."""
         self._frame_data.append(byte)
         self._ffc.update(byte)
         self._header.update()
 
     @property
-    def message_type(self) -> MeterMessageType:
-        """Return MeterMessageType of message."""
-        return MeterMessageType.HDLC_DLMS
-
-    @property
-    def is_valid(self) -> bool:
-        """Return True when valitation (checksum etc.) is successfull."""
-        if self.is_good_ffc and self.is_expected_length:
-            return True
-
-        _LOGGER.warning(
-            "Got invalid frame (is_good_ffc = %s, is_expected_length = %s): %s",
-            self.is_good_ffc,
-            self.is_expected_length,
-            self.as_bytes.hex(),
-        )
-        return False
-
-    @property
-    def as_bytes(self) -> bytes:
+    def frame_data(self) -> bytes:
         """
         Return frame data bytes.
 
         Data has been unescaped when the reader uses octet frame stuffing (see constructor).
         """
         return bytes(self._frame_data)
 
@@ -256,34 +234,34 @@
 
     @property
     def header(self) -> HdlcFrameHeader:
         """Frame header."""
         return self._header
 
     @property
-    def frame_check_sequence(self) -> int | None:
+    def frame_check_sequence(self) -> Optional[int]:
         """Frame check sequence if complete frame has been read. None or invalid number if not."""
         if self._header.information_position is not None:
             if len(self._frame_data) >= self._header.information_position:
                 return (
                     self._frame_data[len(self._frame_data) - 2] << 8
                     | self._frame_data[len(self._frame_data) - 1]
                 )
         return None
 
     @property
-    def payload(self) -> bytes | None:
-        """Information field (the payload) when the field has been read and is available."""
+    def information(self) -> Optional[bytes]:
+        """Information field when the field has been read and is available."""
         info_position = self._header.information_position
         if info_position is not None and len(self._frame_data) > info_position:
             return bytes(self._frame_data[info_position:-2])
         return None
 
 
-class HdlcFrameReader(MeterReaderBase[HdlcFrame]):
+class HdlcFrameReader:
     """Use this class to HDLC-frames as stream of bytes."""
 
     # The Control Escape octet is defined as binary 01111101 (hexadecimal 0x7d)
     CONTROL_ESCAPE: int = 0x7D
 
     # The Flag Sequence indicates the beginning or end of a frame.
     # The octet stream is examined on an octet-by-octet basis for the value 01111110 (hexadecimal 0x7e).
@@ -298,34 +276,34 @@
         :param use_octet_stuffing: true to use octet stuffing (0x7D as escape octet)
         """
         self._use_octet_stuffing = use_octet_stuffing
         self._use_abort_sequence = use_abort_sequence
         self._unescape_next = False
         self._buffer = _ReaderBuffer()
         self._raw_frame_data = bytearray()
-        self._frame: HdlcFrame | None = None
+        self._frame: Optional[HdlcFrame] = None
 
     @property
     def unescape_next(self) -> bool:
         """Return True if octet stuffing is used and next octet is escaped and must be unescaped."""
         return self._unescape_next
 
     @property
     def is_in_hunt_mode(self) -> bool:
         """Return True when reader is hunting for start of frame."""
         return self._frame is None
 
-    def read(self, data_chunk: bytes) -> list[HdlcFrame]:
+    def read(self, data_chunk: bytes) -> List[HdlcFrame]:
         """
         Call this function to read chunks of bytes.
 
         :param data_chunk: next bytes to parsed.
         :return: frame when a frame is complete (both with correct and incorrect checksum).
         """
-        frames_received: list[HdlcFrame] = []
+        frames_received: List[HdlcFrame] = []
 
         self._buffer.extend(data_chunk)
 
         if self._frame is None:  # in hunt mode
             self._buffer.trim_buffer_to_flag_or_end()
 
         while self._buffer.is_available:
```

### Comparing `amshan-2.1.1/han/kamstrup.py` & `amshan-2021.12.1/amshan/kamstrup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Decoding support for Kamstrup meters."""
 # pylint: disable=protected-access
-from __future__ import annotations
-
 from datetime import datetime
+from typing import Dict, Union
 
 import construct  # type: ignore
 
-from han import cosem, obis_map
-from han.obis import Obis
+from amshan import cosem, obis_map
 
 Element: construct.Struct = construct.Struct(
     "_element_type" / construct.Peek(cosem.CommonDataTypes),
     "obis"
     / construct.If(
         cosem.CommonDataTypes.octet_string == construct.this._element_type,
         cosem.ObisCodeOctedStringField,
@@ -19,105 +17,65 @@
     "value_type" / construct.Peek(cosem.CommonDataTypes),
     "value"
     / construct.IfThenElse(
         cosem.CommonDataTypes.octet_string == construct.this.value_type,
         cosem.DateTimeField,
         cosem.Field,
     ),
-    "_NullData" / cosem.NullData,  # trim null-data between elements
 )
 
 NotificationBody: construct.Struct = construct.Struct(
     construct.Const(
         cosem.CommonDataTypes.structure, cosem.CommonDataTypes
     ),  # expect structure
     "length" / construct.Int8ub,
     "list_items" / construct.GreedyRange(Element),
 )
 
 LlcPdu: construct.Struct = cosem.get_llc_pdu_struct(NotificationBody)
 
-_field_scaling_standard = {
-    "1.1.31.7.0.255": -2,  # IL1
-    "1.1.51.7.0.255": -2,  # IL2
-    "1.1.71.7.0.255": -2,  # IL3
-    "1.1.1.8.0.255": 1,  # A14
-    "1.1.2.8.0.255": 1,  # A23
-    "1.1.3.8.0.255": 1,  # R12
-    "1.1.4.8.0.255": 1,  # R34
-}
-
-_field_scaling_ct_meter = {
-    "1.1.31.7.0.255": -3,  # IL1
-    "1.1.51.7.0.255": -3,  # IL2
-    "1.1.71.7.0.255": -3,  # IL3
-    "1.1.1.8.0.255": 1,  # A14
-    "1.1.2.8.0.255": 1,  # A23
-    "1.1.3.8.0.255": 1,  # R12
-    "1.1.4.8.0.255": 1,  # R34
+_field_scaling = {
+    "1.1.31.7.0.255": -2,
+    "1.1.51.7.0.255": -2,
+    "1.1.71.7.0.255": -2,
 }
 
 
-def _normalize_parsed_items(
-    list_items: construct.ListContainer,
-) -> dict[str, str | int | float | datetime]:
-    dictionary: dict[str, str | int | float | datetime] = {
-        obis_map.FIELD_METER_MANUFACTURER: "Kamstrup",
+def normalize_parsed_frame(
+    frame: construct.Struct,
+) -> Dict[str, Union[str, int, float, datetime]]:
+    """Convert data from meters construct structure to a dictionary with common key names."""
+    dictionary = {
+        obis_map.NEK_HAN_FIELD_METER_MANUFACTURER: "Kamstrup",
+        obis_map.NEK_HAN_FIELD_METER_DATETIME: frame.information.DateTime.datetime,
     }
 
-    meter_type = next((x for x in list_items if x.obis == "1.1.96.1.1.256"), None)
-    is_ct_meter = meter_type is not None and meter_type.startswith("685")
-    field_scaling = _field_scaling_ct_meter if is_ct_meter else _field_scaling_standard
-
+    list_items = frame.information.notification_body.list_items
     for measure in list_items:
         # list version is the only element without obis code
         element_name = (
-            obis_map.obis_name_map[Obis.from_string(measure.obis).to_group_cdr_str()]
+            obis_map.obis_name_map[measure.obis]
             if measure.obis
-            else obis_map.FIELD_OBIS_LIST_VER_ID
+            else obis_map.NEK_HAN_FIELD_OBIS_LIST_VER_ID
         )
 
-        if element_name == obis_map.FIELD_METER_DATETIME:
+        if element_name == obis_map.NEK_HAN_FIELD_METER_DATETIME:
             dictionary[element_name] = measure.value.datetime
         else:
             if isinstance(measure.value, int):
-                scale = field_scaling.get(measure.obis, None)
+                scale = _field_scaling.get(measure.obis, None)
                 if scale:
-                    dictionary[element_name] = measure.value * (10**scale)
+                    dictionary[element_name] = measure.value * (10 ** scale)
                 else:
                     dictionary[element_name] = measure.value
             else:
                 dictionary[element_name] = measure.value
 
     return dictionary
 
 
-def normalize_parsed_frame(
-    frame: construct.Struct,
-) -> dict[str, str | int | float | datetime]:
-    """Convert data from meters construct structure to a dictionary with common key names."""
-    dictionary = _normalize_parsed_items(frame.information.notification_body.list_items)
-    dictionary[obis_map.FIELD_METER_DATETIME] = frame.information.DateTime.datetime
-    return dictionary
-
-
-def normalize_parsed_notification(
-    notification: construct.Struct,
-) -> dict[str, str | int | float | datetime]:
-    """Convert data from meters construct structure to a dictionary with common key names."""
-    return _normalize_parsed_items(notification.list_items)
-
-
 def decode_frame_content(
     frame_content: bytes,
-) -> dict[str, str | int | float | datetime]:
+) -> Dict[str, Union[str, int, float, datetime]]:
     """Decode meter LLC PDU frame content as a dictionary."""
     parsed = LlcPdu.parse(frame_content)
     return normalize_parsed_frame(parsed)
-
-
-def decode_notification_body(
-    notification_body: bytes,
-) -> dict[str, str | int | float | datetime]:
-    """Decode meter APDU notification body as a dictionary."""
-    parsed = NotificationBody.parse(notification_body)
-    return normalize_parsed_notification(parsed)
```

### Comparing `amshan-2.1.1/han/meter_connection.py` & `amshan-2021.12.1/amshan/meter_connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Async meter connection module."""
-from __future__ import annotations
-
 import datetime
 import logging
 from abc import ABCMeta, abstractmethod
 from asyncio import (
     FIRST_COMPLETED,
     BaseTransport,
     CancelledError,
     Event,
     Future,
     Protocol,
     Queue,
     iscoroutinefunction,
-    sleep,
     wait,
-    create_task,
-    ensure_future,
+    sleep,
 )
-from typing import Awaitable, Callable, ClassVar, Sequence, Tuple
+from typing import Awaitable, Callable, ClassVar, Optional, Tuple
 
-from han.common import MeterMessageBase, MeterReaderBase
+from amshan import hdlc
+from amshan.hdlc import HdlcFrame
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class BackOffStrategy(metaclass=ABCMeta):
     """
     Back-off strategy base class.
@@ -70,39 +67,43 @@
     def current_delay_sec(self) -> int:
         """Return current back-off delay in seconds."""
         return self._delay if self._delay < self.max_delay else self.max_delay
 
 
 class SmartMeterBaseProtocol(Protocol, metaclass=ABCMeta):
     """
-    Network protocol base class that reads smart meter messages from a stream.
+    Network protocol base class that reads smart meter frames from a stream.
 
-    Sub classes must implement message_received().
+    Sub classes must implement frame_received().
     """
 
     # Total number of this class that has been created.
     # The number is used when initializing trace id for new instances.
     total_instance_counter: ClassVar[int] = 0
 
     def __init__(
         self,
-        reader_candidates: Sequence[MeterReaderBase],
+        frame_reader: Optional[hdlc.HdlcFrameReader] = None,
     ) -> None:
         """
         Initialize SmartMeterProtocol.
 
-        :param reader_candidates: message reader candidates.
+        :param frame_reader: optional frame reader.
+        A frame reader with both octet stuffing and abort sequence disabled is created if None.
         """
         super().__init__()
         self._done: Future[None] = Future()
         self.instance_id: int = SmartMeterBaseProtocol.total_instance_counter
-        self._reader_candidates = list(reader_candidates)
-        self._selected_reader: MeterReaderBase | None = None
-        self._transport: BaseTransport | None = None
-        self._transport_info: str | None = None
+        self._frame_reader = (
+            frame_reader
+            if frame_reader
+            else hdlc.HdlcFrameReader(use_octet_stuffing=False, use_abort_sequence=True)
+        )
+        self._transport: Optional[BaseTransport] = None
+        self._transport_info: Optional[str] = None
         SmartMeterBaseProtocol.total_instance_counter += 1
 
     @property
     def done(self) -> Awaitable[None]:
         """Return Awaitable that can be used to wait for connection to be lost or closed."""
         return self._done
 
@@ -130,15 +131,15 @@
         """
         self._transport = transport
         self._set_transport_info()
         _LOGGER.info(
             "%s: Smart meter connected to %s", self._instance_id(), self._transport_info
         )
 
-    def connection_lost(self, exc: Exception | None) -> None:
+    def connection_lost(self, exc: Optional[Exception]) -> None:
         """
         Signal that the transport connected to this protocol instance has been lost or closed.
 
         Called when the connection is lost or closed.
         The argument is an exception object or None (the latter
         meaning a regular EOF is received or the connection was
         aborted or closed).
@@ -171,139 +172,126 @@
                     "lost" if exc else "closed",
                     ex,
                 )
 
         self._done.set_result(None)
 
     def data_received(self, data: bytes) -> None:
-        """Receive data from the transport and put messages(s) on the queue if messages(s) are ready."""
-        if self._selected_reader:
-            messages = self._selected_reader.read(data)
-            for msg in messages:
-                self.message_received(msg)
-        else:
-            for reader in self._reader_candidates:
-                messages = reader.read(data)
-                for msg in messages:
-                    if msg.is_valid:
-                        self._selected_reader = reader
-                        self._reader_candidates.clear()
-                        _LOGGER.info("Reader %s selected.", reader)
-                        break
-                if self._selected_reader:
-                    for msg in messages:
-                        self.message_received(msg)
-                    break
+        """Receive data from the transport and put frame(s) on the queue if frame(s) are complete."""
+        frames = self._frame_reader.read(data)
+        for frame in frames:
+            self.frame_received(frame)
 
     @abstractmethod
-    def message_received(self, message: MeterMessageBase) -> None:
-        """Message is received from the transport."""
+    def frame_received(self, frame: HdlcFrame) -> None:
+        """Frame is received from the transport."""
 
     def eof_received(self) -> bool:
         """
         Return False to close the transport.
 
-        Called when the other end signals it won't send any more data.
+        Called when the other end signals it won’t send any more data.
         """
         _LOGGER.debug(
-            "%s: eof_received - the other end (%s) signaled it won't send any more data. Close transport",
+            "%s: eof_received - the other end (%s) signaled it won’t send any more data. Close transport",
             self._instance_id(),
             self._transport_info,
         )
 
         # return false to close transport.
         return False
 
     def _instance_id(self) -> str:
         return f"{self.__class__.__name__}[{self.instance_id}]"
 
 
-class SmartMeterMessageProtocol(SmartMeterBaseProtocol):
+# pylint: disable=too-many-instance-attributes
+
+
+class SmartMeterFrameProtocol(SmartMeterBaseProtocol):
     """
-    Network protocol that reads smart meter messages from a stream and forwards them to a queue.
+    Network protocol that reads smart meter frames from a stream and forwards them to a queue.
 
     When the user wants to requests a transport to use with this protocol,
-    they pass a SmartMeterMessageProtocol factory to a utility function (e.g.,
+    they pass a SmartMeterFrameProtocol factory to a utility function (e.g.,
     EventLoop.create_connection() or serial_asyncio.create_serial_connection).
 
     Example:
-        await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessageProtocol(queue), [ModeDReader()], url = "/dev/tty01")
+        await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameProtocol(queue), url = "/dev/tty01")
     """
 
     def __init__(
         self,
-        destination_queue: Queue[MeterMessageBase],
-        reader_candidates: Sequence[MeterReaderBase],
+        destination_queue: "Queue[hdlc.HdlcFrame]",
+        frame_reader: Optional[hdlc.HdlcFrameReader] = None,
     ) -> None:
         """
-        Initialize SmartMeterMessageProtocol.
+        Initialize SmartMeterProtocol.
 
-        :param destination_queue: destination queue for received messages.
-        :param reader_candidates: message reader candidates.
+        :param destination_queue: destination queue for decoded frames.
+        :param frame_reader: optional frame reader.
+        A frame reader with both octet stuffing and abort sequence disabled is created if None.
         """
-        super().__init__(reader_candidates)
-        self.queue: Queue[MeterMessageBase] = destination_queue
+        super().__init__(frame_reader)
+        self.queue: Queue[HdlcFrame] = destination_queue
 
-    def message_received(self, message: MeterMessageBase) -> None:
-        """Received message is passed on to the queue."""
-        self.queue.put_nowait(message)
+    def frame_received(self, frame: HdlcFrame) -> None:
+        """Frame is passed on to the queue."""
+        self.queue.put_nowait(frame)
 
 
-class SmartMeterMessagePayloadProtocol(SmartMeterBaseProtocol):
+class SmartMeterFrameContentProtocol(SmartMeterBaseProtocol):
     """
-    Network protocol that reads smart meter messages from a stream and forwards their payload to a queue.
+    Network protocol that reads smart meter frames from a stream and forwards their content to a queue.
 
     When the user wants to requests a transport to use with this protocol,
-    they pass a SmartMeterMessagePayloadProtocol factory to a utility function (e.g.,
+    they pass a SmartMeterFrameContentProtocol factory to a utility function (e.g.,
     EventLoop.create_connection() or serial_asyncio.create_serial_connection).
 
     Example:
-        await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterMessagePayloadProtocol(queue), [ModeDReader()] url = "/dev/tty01")
+        await serial_asyncio.create_serial_connection(loop, lambda: SmartMeterFrameContentProtocol(queue), url = "/dev/tty01")
     """
 
     def __init__(
         self,
-        destination_queue: Queue[bytes],
-        reader_candidates: Sequence[MeterReaderBase],
+        destination_queue: "Queue[bytes]",
+        frame_reader: Optional[hdlc.HdlcFrameReader] = None,
     ) -> None:
         """
-        Initialize SmartMeterMessagePayloadProtocol.
+        Initialize SmartMeterProtocol.
 
-        :param destination_queue: destination queue for received messages payloads.
-        :param reader_candidates: message reader candidates.
+        :param destination_queue: destination queue for decoded frames.
+        :param frame_reader: optional frame reader.
+        A frame reader with both octet stuffing and abort sequence disabled is created if None.
         """
-        super().__init__(reader_candidates)
+        super().__init__(frame_reader)
         self.queue: Queue[bytes] = destination_queue
 
-    def message_received(self, message: MeterMessageBase) -> None:
+    def frame_received(self, frame: HdlcFrame) -> None:
         """
-        Message is received and its payload is passed on to the queue.
+        Frame is received and its content is passed on to the queue.
 
-        Only payload from non empty payloads of valid messages (check sum etc.) is passed on
+        Only content from non empty frames with expected length and checksum is passed on.
         """
-        payload = message.payload
-        if message.is_valid:
-            if payload is not None and len(payload) > 0:
-                self.queue.put_nowait(payload)
+        if frame.is_good_ffc and frame.is_expected_length:
+            frame_content = frame.information
+            if frame_content:
+                self.queue.put_nowait(frame_content)
             else:
-                _LOGGER.debug("Got empty message.")
+                _LOGGER.debug("Got empty frame")
         else:
-            _LOGGER.warning(
-                "Got invalid message: %s",
-                message.as_bytes.hex() if message.as_bytes else "<empty>",
-            )
+            _LOGGER.warning("Got invalid frame: %s", frame.frame_data.hex())
 
 
 MeterTransportProtocol = Tuple[BaseTransport, SmartMeterBaseProtocol]
 
 AsyncConnectionFactory = Callable[[], Awaitable[MeterTransportProtocol]]
 
 
 class ConnectionManager:
-    # pylint: disable=too-many-instance-attributes
     """
     Maintain connection and reconnect if connection is lost.
 
     Reconnecting uses a back-off retry strategy, and has a simple circuit breaker for connection lost.
     """
 
     DEFAULT_CONNECTION_LOST_BACK_OFF_THRESHOLD: int = 5
@@ -318,26 +306,26 @@
 
         :param connection_factory: A factory function that returns a Transport and SmartMeterProtocol tuple.
         """
         if not iscoroutinefunction(connection_factory):
             raise ValueError("Factory must be awaitable.")
 
         self._connection_factory: AsyncConnectionFactory = connection_factory
-        self._connection: MeterTransportProtocol | None = None
+        self._connection: Optional[MeterTransportProtocol] = None
         self._is_closing: Event = Event()
 
         self.back_off_connect_error: BackOffStrategy = ExponentialBackOff()
 
         self.connection_lost_back_off_threshold: int = (
             ConnectionManager.DEFAULT_CONNECTION_LOST_BACK_OFF_SLEEP_SEC
         )
         self.connection_lost_back_off_sleep_sec: int = (
             ConnectionManager.DEFAULT_CONNECTION_LOST_BACK_OFF_SLEEP_SEC
         )
-        self._connection_lost_last_time: datetime.datetime | None = None
+        self._connection_lost_last_time: Optional[datetime.datetime] = None
         self._connection_lost_sleep_before_reconnect: bool = False
 
     def close(self) -> None:
         """Close current connection, if any, and stop reconnecting."""
         self._is_closing.set()
         if self._connection:
             _LOGGER.info("Close connection and abort connect loop")
@@ -348,27 +336,23 @@
     async def connect_loop(self) -> None:
         """
         Connect to meter using connection factory, and keep reconnecting if connection is lost.
 
         The connection is not reconnected on connection loss if close() was called on this instance.
         """
         while not self._is_closing.is_set():
-            connect_task = create_task(self._try_connect())
-            closing_task = create_task(self._is_closing.wait())
             await wait(
-                (connect_task, closing_task),
+                (self._try_connect(), self._is_closing.wait()),
                 return_when=FIRST_COMPLETED,
             )
 
             if self._connection:
                 _, protocol = self._connection
-                done_task = ensure_future(protocol.done)
-                closing_task2 = create_task(self._is_closing.wait())
                 await wait(
-                    (done_task, closing_task2),
+                    (protocol.done, self._is_closing.wait()),
                     return_when=FIRST_COMPLETED,
                 )
 
                 if not self._is_closing.is_set():
                     _LOGGER.warning("Connection lost")
                     self._update_connection_lost_circuit_breaker()
 
@@ -416,13 +400,13 @@
         if not self._is_closing.is_set():
             try:
                 _LOGGER.debug("Try to connect")
                 self._connection = await self._connection_factory()
 
                 self.back_off_connect_error.reset()
             except CancelledError:
-                _LOGGER.debug("The operation was cancelled")
+                _LOGGER.debug("The operation was cencelled")
                 raise
             except Exception as ex:  # pylint: disable=broad-except
                 self._connection = None
                 self.back_off_connect_error.failure()
                 _LOGGER.warning("Error connecting: %s", ex)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `amshan-2.1.1/han/serial_connection_factory.py` & `amshan-2021.12.1/amshan/serial_connection_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,64 @@
 """Serial connection factory."""
-from __future__ import annotations
-
-from asyncio import Queue  # pylint: disable=unused-import
 from asyncio import AbstractEventLoop, get_event_loop
-from typing import Sequence, cast
+from asyncio import Queue  # pylint: disable=unused-import
+from typing import Optional, cast
 
 import serial_asyncio  # type: ignore
 
-from han.common import MeterMessageBase  # pylint: disable=unused-import
-from han.common import MeterReaderBase
-from han.dlde import ModeDReader
-from han.hdlc import HdlcFrameReader
-from han.meter_connection import (
+from amshan.hdlc import HdlcFrame  # pylint: disable=unused-import
+from amshan.meter_connection import (
     MeterTransportProtocol,
-    SmartMeterMessagePayloadProtocol,
-    SmartMeterMessageProtocol,
+    SmartMeterFrameContentProtocol,
+    SmartMeterFrameProtocol,
 )
 
 
-async def create_serial_message_connection(
-    queue: "Queue[MeterMessageBase]",
-    loop: AbstractEventLoop | None,
-    readers: Sequence[MeterReaderBase] | None,
+async def create_serial_frame_connection(
+    queue: "Queue[HdlcFrame]",
+    loop: Optional[AbstractEventLoop],
     *args,
     **kwargs,
 ) -> MeterTransportProtocol:
     """
-    Create serial connection using SmartMeterMessageProtocol.
+    Create serial connection using SmartMeterFrameProtocol.
 
-    :param queue: Queue for received data readouts
+    :param queue: Queue for received frames
     :param loop: The event handler
-    :param readers: message reader(s). Passing None means all.
     :param args: Passed to serial_asyncio.create_serial_connection and further to serial.Serial init function
     :param kwargs: Passed to serial_asyncio.create_serial_connection and further the serial.Serial init function
     :return: Tuple of transport and protocol
     """
     return cast(
         MeterTransportProtocol,
         await serial_asyncio.create_serial_connection(
             loop if loop else get_event_loop(),
-            lambda: SmartMeterMessageProtocol(
-                queue,
-                readers
-                if readers
-                else [
-                    HdlcFrameReader(use_octet_stuffing=False, use_abort_sequence=True),
-                    ModeDReader(),
-                ],
-            ),
+            lambda: SmartMeterFrameProtocol(queue),
             *args,
             **kwargs,
         ),
     )
 
 
-async def create_serial_message_payload_connection(
+async def create_serial_frame_content_connection(
     queue: "Queue[bytes]",
-    loop: AbstractEventLoop | None,
-    readers: Sequence[MeterReaderBase] | None,
+    loop: Optional[AbstractEventLoop],
     *args,
     **kwargs,
 ) -> MeterTransportProtocol:
-    """Create serial connection using SmartMeterMessagePayloadProtocol.
+    """Create serial connection using SmartMeterFrameContentProtocol.
 
-    :param queue: Queue for received data readout content
+    :param queue: Queue for received frames
     :param loop: The event handler
-    :param readers: message reader(s). Passing None means all.
     :param args: Passed to serial_asyncio.create_serial_connection and further to serial.Serial init function
     :param kwargs: Passed to serial_asyncio.create_serial_connection and further the serial.Serial init function
     :return: Tuple of transport and protocol
     """
     return cast(
         MeterTransportProtocol,
         await serial_asyncio.create_serial_connection(
             loop if loop else get_event_loop(),
-            lambda: SmartMeterMessagePayloadProtocol(
-                queue,
-                readers
-                if readers
-                else [
-                    HdlcFrameReader(use_octet_stuffing=False, use_abort_sequence=True),
-                    ModeDReader(),
-                ],
-            ),
+            lambda: SmartMeterFrameContentProtocol(queue),
             *args,
             **kwargs,
         ),
     )
```

### Comparing `amshan-2.1.1/han/tcp_connection_factory.py` & `amshan-2021.12.1/amshan/tcp_connection_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,63 @@
 """TCP/IP connection factory."""
-from __future__ import annotations
-
-from asyncio import Queue  # pylint: disable=unused-import
 from asyncio import AbstractEventLoop, BaseProtocol, get_event_loop
-from typing import Sequence, cast
+from asyncio import Queue  # pylint: disable=unused-import
+from typing import Optional, cast
 
-from han.common import MeterMessageBase  # pylint: disable=unused-import
-from han.common import MeterReaderBase
-from han.dlde import ModeDReader
-from han.hdlc import HdlcFrameReader
-from han.meter_connection import (
+from amshan.hdlc import HdlcFrame  # pylint: disable=unused-import
+from amshan.meter_connection import (
     MeterTransportProtocol,
-    SmartMeterMessagePayloadProtocol,
-    SmartMeterMessageProtocol,
+    SmartMeterFrameContentProtocol,
+    SmartMeterFrameProtocol,
 )
 
 
-async def create_tcp_message_connection(
-    queue: "Queue[MeterMessageBase]",
-    loop: AbstractEventLoop | None,
-    readers: Sequence[MeterReaderBase] | None,
+async def create_tcp_frame_connection(
+    queue: "Queue[HdlcFrame]",
+    loop: Optional[AbstractEventLoop],
     *args,
     **kwargs,
 ) -> MeterTransportProtocol:
     """
-    Create TCP connection using SmartMeterMessageProtocol.
+    Create TCP connection using SmartMeterFrameProtocol.
 
-    :param queue: Queue for received data readouts
+    :param queue: Queue for received frames
     :param loop: The event handler
-    :param readers: message reader(s).
     :param args: Passed to the loop.create_connection
     :param kwargs: Passed to the loop.create_connection
     :return: Tuple of transport and protocol
     """
     loop = loop if loop else get_event_loop()
     return cast(
         MeterTransportProtocol,
         await loop.create_connection(
-            lambda: cast(
-                BaseProtocol,
-                SmartMeterMessageProtocol(
-                    queue,
-                    readers
-                    if readers
-                    else [
-                        HdlcFrameReader(
-                            use_octet_stuffing=False, use_abort_sequence=True
-                        ),
-                        ModeDReader(),
-                    ],
-                ),
-            ),
+            lambda: cast(BaseProtocol, SmartMeterFrameProtocol(queue)),
             *args,
             **kwargs,
         ),
     )
 
 
-async def create_tcp_message_payload_connection(
+async def create_tcp_frame_content_connection(
     queue: "Queue[bytes]",
-    loop: AbstractEventLoop | None,
-    readers: Sequence[MeterReaderBase] | None,
+    loop: Optional[AbstractEventLoop],
     *args,
     **kwargs,
 ) -> MeterTransportProtocol:
     """
-    Create TCP connection using SmartMeterMessagePayloadProtocol.
+    Create TCP connection using SmartMeterFrameContentProtocol.
 
-    :param queue: Queue for received data readout content
+    :param queue: Queue for received frames
     :param loop: The event handler
-    :param readers: message reader(s).
     :param args: Passed to the loop.create_connection
     :param kwargs: Passed to the loop.create_connection
     :return: Tuple of transport and protocol
     """
     loop = loop if loop else get_event_loop()
     return cast(
         MeterTransportProtocol,
         await loop.create_connection(
-            lambda: cast(
-                BaseProtocol,
-                SmartMeterMessagePayloadProtocol(
-                    queue,
-                    readers
-                    if readers
-                    else [
-                        HdlcFrameReader(
-                            use_octet_stuffing=False, use_abort_sequence=True
-                        ),
-                        ModeDReader(),
-                    ],
-                ),
-            ),
+            lambda: cast(BaseProtocol, SmartMeterFrameContentProtocol(queue)),
             *args,
             **kwargs,
         ),
     )
```

### Comparing `amshan-2.1.1/setup.py` & `amshan-2021.12.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,40 +2,38 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="amshan",
-    version="2.1.1",
+    version="2021.12.1",
     author="Tore Amundsen",
     author_email="tore@amundsen.org",
-    description="Decode P1 and MBUS (Meter Bus) DLMS data. Special support for norwegian and swedish meters.",
+    description="Decode MBUS (Meter Bus) data with special support for norwegian AMS-smart meters (HAN port)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms=["POSIX", "Windows"],
     url="https://github.com/toreamun/amshan",
-    packages=["han"],
-    package_data={"han": ["py.typed"]},
+    packages=["amshan"],
+    package_data={"amshan": ["py.typed"]},
     keywords=[
         "meter",
         "han",
         "ams",
-        "p1",
         "mbus",
         "aidon",
         "kaifa",
         "kamstrup",
-        "dlms",
         "cosem",
         "hdlc",
         "fast frame check",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.6",
     install_requires=["construct"],
     extras_require={"serial": ["pyserial-asyncio>=0.4"]},
 )
```

