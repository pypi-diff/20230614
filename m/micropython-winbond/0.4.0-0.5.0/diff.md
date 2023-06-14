# Comparing `tmp/micropython-winbond-0.4.0.tar.gz` & `tmp/micropython-winbond-0.5.0.tar.gz`

## Comparing `micropython-winbond-0.4.0.tar` & `micropython-winbond-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-24 14:21:04.000000 micropython-winbond-0.4.0/micropython_winbond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-24 14:20:56.000000 micropython-winbond-0.4.0/winbond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-24 14:21:04.000000 micropython-winbond-0.4.0/winbond/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-03-24 14:20:56.000000 micropython-winbond-0.4.0/winbond/winbond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-06-14 20:18:41.000000 micropython-winbond-0.5.0/micropython_winbond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 20:18:30.000000 micropython-winbond-0.5.0/winbond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 20:18:40.000000 micropython-winbond-0.5.0/winbond/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-14 20:18:30.000000 micropython-winbond-0.5.0/winbond/winbond.py
```

### Comparing `micropython-winbond-0.4.0/micropython_winbond.egg-info/PKG-INFO` & `micropython-winbond-0.5.0/micropython_winbond.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: micropython-winbond
-Version: 0.4.0
+Version: 0.5.0
 Summary: Simple MicroPython Winbond library
 Home-page: https://github.com/brainelectronics/micropython-winbond
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-winbond/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-winbond
 Keywords: micropython,winbond,library
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MicroPython Winbond Flash
 
 [![Downloads](https://pepy.tech/badge/micropython-winbond)](https://pepy.tech/project/micropython-winbond)
 ![Release](https://img.shields.io/github/v/release/brainelectronics/micropython-winbond?include_prereleases&color=success)
@@ -30,22 +31,22 @@
 [MicroPython Winbond ReadTheDocs][ref-rtd-micropython-winbond] 📚
 
 -----------------------
 
 <!-- MarkdownTOC -->
 
 - [Installation](#installation)
-	- [Install required tools](#install-required-tools)
+    - [Install required tools](#install-required-tools)
 - [Stetup](#stetup)
-	- [Install package with upip](#install-package-with-upip)
-		- [General](#general)
-		- [Specific version](#specific-version)
-		- [Test version](#test-version)
-	- [Manually](#manually)
-		- [Upload files to board](#upload-files-to-board)
+    - [Install package](#install-package)
+        - [General](#general)
+        - [Specific version](#specific-version)
+        - [Test version](#test-version)
+    - [Manually](#manually)
+        - [Upload files to board](#upload-files-to-board)
 - [Usage](#usage)
 - [Credits](#credits)
 
 <!-- /MarkdownTOC -->
 
 ## Installation
 
@@ -76,21 +77,22 @@
 
 ```bash
 rshell --help
 ```
 
 ## Stetup
 
-### Install package with upip
+### Install package
 
-Connect your MicroPython board to a network
+Connect the MicroPython device to a network (if possible)
 
 ```python
 import network
 station = network.WLAN(network.STA_IF)
+station.active(True)
 station.connect('SSID', 'PASSWORD')
 station.isconnected()
 ```
 
 #### General
 
 Install the latest package version of this lib on the MicroPython device
@@ -115,15 +117,16 @@
 import mip
 # install a verions of a specific branch
 mip.install("github:brainelectronics/micropython-winbond", version="feature/add-docs-and-detailed-examples")
 # install a tag version
 mip.install("github:brainelectronics/micropython-winbond", version="0.4.0")
 ```
 
-For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`
+For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`.
+With `upip` always the latest available version will be installed.
 
 ```python
 import upip
 upip.install('micropython-winbond')
 ```
 
 #### Test version
@@ -134,15 +137,16 @@
 will be used.
 
 ```python
 import mip
 mip.install("github:brainelectronics/micropython-winbond", version="0.4.0-rc2.dev4")
 ```
 
-For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`
+For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`.
+With `upip` always the latest available version will be installed.
 
 ```python
 import upip
 # overwrite index_urls to only take artifacts from test.pypi.org
 upip.index_urls = ['https://test.pypi.org/pypi']
 upip.install('micropython-winbond')
 ```
@@ -167,27 +171,28 @@
 Perform the following command inside the `rshell` to copy all files and
 folders to the device
 
 ```bash
 mkdir /pyboard/lib
 mkdir /pyboard/lib/winbond
 
-cp winbond.py /pyboard/lib/winbond
+cp winbond/* /pyboard/lib/winbond
 cp main.py /pyboard/lib/winbond
 cp boot.py /pyboard/lib/winbond
 ```
 
 ## Usage
 
 ```python
 from machine import SPI, Pin
 import os
 from winbond import W25QFlash
 
 # the used SPI and CS pin is setup specific, change accordingly
+# check the boot.py file of this repo for further boards
 flash = W25QFlash(spi=SPI(2), cs=Pin(5), baud=2000000, software_reset=True)
 
 flash_mount_point = '/external'
 
 try:
     os.mount(flash, flash_mount_point)
 except Exception as e:
@@ -221,16 +226,11 @@
 Kudos and big thank you to [crizeo of the MicroPython Forum][ref-crizeo] and
 his [post to use Winbond flash chips][ref-upy-forum-winbond-driver]
 
 <!-- Links -->
 [ref-rtd-micropython-winbond]: https://micropython-winbond.readthedocs.io/en/latest/
 [ref-remote-upy-shell]: https://github.com/dhylands/rshell
 [ref-brainelectronics-test-pypiserver]: https://github.com/brainelectronics/test-pypiserver
-[ref-be32]: https://github.com/brainelectronics/BE32-01/
-[ref-pfalcon-picoweb-sdist-upip]: https://github.com/pfalcon/picoweb/blob/b74428ebdde97ed1795338c13a3bdf05d71366a0/sdist_upip.py
-[ref-test-pypi]: https://test.pypi.org/
-[ref-pypi]: https://pypi.org/
-[ref-invalid-auth-test-pypi]: https://test.pypi.org/help/#invalid-auth
 [ref-crizeo]: https://forum.micropython.org/memberlist.php?mode=viewprofile&u=3067
 [ref-upy-forum-winbond-driver]: https://forum.micropython.org/viewtopic.php?f=16&t=3899&start=10
```

### Comparing `micropython-winbond-0.4.0/winbond/winbond.py` & `micropython-winbond-0.5.0/winbond/winbond.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,19 @@
         :param      cs:              The CS pin object
         :type       cs:              Pin
         :param      baud:            The SCK clock rate
         :type       baud:            int
         :param      software_reset:  Flag to use software reset
         :type       software_reset:  bool
         """
+        self._manufacturer = 0x0
+        self._mem_type = 0
+        self._device_type = 0x0
+        self._capacity = 0
+
         self.cs = cs
         self.spi = spi
         self.cs.init(self.cs.OUT, value=1)
         # highest possible baudrate is 40 MHz for ESP-12
         self.spi.init(baudrate=baud, phase=1, polarity=1)
         self._busy = False
 
@@ -54,20 +59,59 @@
 
         # address length (default: 3 bytes, 32MB+: 4)
         self._ADR_LEN = 3 if (len(bin(self._CAPACITY - 1)) - 2) <= 24 else 4
 
         # setup address mode:
         if self._ADR_LEN == 4:
             if not self._read_status_reg(nr=16):  # not in 4-byte mode
-                print("entering 4-byte address mode")
                 self._await()
                 self.cs(0)
                 self.spi.write(b'\xB7')  # 'Enter 4-Byte Address Mode'
                 self.cs(1)
 
+    @property
+    def capacity(self) -> int:
+        """
+        Get the storage capacity of the flash
+
+        :returns:   Capacity of the flash in bytes
+        :rtype:     int
+        """
+        return self._capacity
+
+    @property
+    def device(self) -> int:
+        """
+        Get the flash device type
+
+        :returns:   Flash device type
+        :rtype:     int
+        """
+        return self._device_type
+
+    @property
+    def manufacturer(self) -> int:
+        """
+        Get the manufacturer ID of the flash
+
+        :returns:   Manufacturer ID of the flash
+        :rtype:     int
+        """
+        return self._manufacturer
+
+    @property
+    def mem_type(self) -> int:
+        """
+        Get the memory type of the flash
+
+        :returns:   Memory type of the flash
+        :rtype:     int
+        """
+        return self._mem_type
+
     def reset(self) -> None:
         """
         Reset the Winbond flash if the device has no hardware reset pin.
 
         See datasheet section 7.2.43 Enable Reset (66h) and Reset (99h)
         Because of the small package and the limitation on the number of pins,
         the W25Q64FV provide a software Reset instruction instead of a
@@ -99,15 +143,14 @@
         self.spi.write(b'\x66')  # 'Enable Reset' command
         self.cs(1)
         self.cs(0)
         self.spi.write(b'\x99')  # 'Reset' command
         self.cs(1)
         time.sleep_us(30)
         self._busy = False
-        # print('Reset performed')
 
     def identify(self) -> None:
         """
         Identify the Winbond chip.
 
         Determine the manufacturer and device ID and raises an error if the
         device is not detected or not supported.
@@ -128,18 +171,19 @@
             raise OSError("device not responding, check wiring. ({}, {}, {})".
                           format(hex(mf), hex(mem_type), hex(cap)))
         if mf != 0xEF or mem_type not in [0x40, 0x60]:
             # Winbond manufacturer, Q25 series memory (tested 0x40 only)
             raise OSError("manufacturer ({}) or memory type ({}) unsupported".
                           format(hex(mf), hex(mem_type)))
 
-        print("manufacturer: {}".format(hex(mf)))               # 0xef
-        print("mem_type: {}".format(mem_type))
-        print("device: {}".format(hex(mem_type << 8 | cap)))    # 0x4016
-        print("capacity: {} bytes".format(self._CAPACITY))      # 4194304 bytes
+        self._manufacturer = hex(mf)
+        self._mem_type = mem_type
+        self._device_type = hex(mem_type << 8 | cap)
+        self._capacity = self._CAPACITY
+
         # return self._CAPACITY  # calculate number of bytes
 
     def get_size(self) -> int:
         """
         Get the flash chip size.
 
         :returns:   The flash size in byte.
@@ -220,15 +264,14 @@
         :type       buf:   list
         :param      addr:  The start address
         :type       addr:  int
         """
         assert addr + len(buf) <= self._CAPACITY, \
             "memory not addressable at %s with range %d (max.: %s)" % \
             (hex(addr), len(buf), hex(self._CAPACITY - 1))
-        # print("read {} bytes starting at {}".format(len(buf), hex(addr)))
 
         self._await()
         self.cs(0)
         # 'Fast Read' (0x03 = default), 0x0C for 4-byte mode command
         self.spi.write(b'\x0C' if self._ADR_LEN == 4 else b'\x0B')
         self.spi.write(addr.to_bytes(self._ADR_LEN, 'big'))
         self.spi.write(b'\xFF')  # dummy byte
@@ -264,15 +307,14 @@
         assert len(buf) % self.PAGE_SIZE == 0, \
             "invalid buffer length: {}".format(len(buf))
         assert not addr & 0xf, \
             "address ({}) not at page start".format(addr)
         assert addr + len(buf) <= self._CAPACITY, \
             ("memory not addressable at {} with range {} (max.: {})".
                 format(hex(addr), len(buf), hex(self._CAPACITY - 1)))
-        # print("write buf[{}] to {} ({})".format(len(buf), hex(addr), addr))
 
         for i in range(0, len(buf), self.PAGE_SIZE):
             self._wren()
             self._await()
             self.cs(0)
             self.spi.write(b'\x02')  # 'Page Program' command
             self.spi.write(addr.to_bytes(self._ADR_LEN, 'big'))
@@ -292,15 +334,14 @@
         :param      blocknum:  The block number
         :type       blocknum:  int
         :param      buf:       The data buffer
         :type       buf:       list
         """
         assert len(buf) == self.BLOCK_SIZE, \
             "invalid block length: {}".format(len(buf))
-        # print("writeblock({}, buf[{}])".format(blocknum, len(buf)))
 
         sector_nr = blocknum // 8
         sector_addr = sector_nr * self.SECTOR_SIZE
         # index of first byte of page in sector (multiple of self.PAGE_SIZE)
         index = (blocknum << 9) & 0xfff
 
         self._read(buf=self._cache, addr=sector_addr)
```

