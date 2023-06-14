# Comparing `tmp/openhomedevice-2.0.2.tar.gz` & `tmp/openhomedevice-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhomedevice-2.0.2.tar", last modified: Wed Apr 13 22:57:23 2022, max compression
+gzip compressed data, was "openhomedevice-2.1.tar", last modified: Wed Jun 14 19:58:16 2023, max compression
```

## Comparing `openhomedevice-2.0.2.tar` & `openhomedevice-2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2022-04-13 22:57:23.231451 openhomedevice-2.0.2/
--rw-r--r--   0 barry     (1000) barry     (1000)     6783 2022-04-13 22:57:23.231451 openhomedevice-2.0.2/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     4794 2022-02-18 23:58:29.000000 openhomedevice-2.0.2/README.md
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2022-04-13 22:57:23.227451 openhomedevice-2.0.2/openhomedevice/
--rw-r--r--   0 barry     (1000) barry     (1000)       43 2022-02-18 23:58:29.000000 openhomedevice-2.0.2/openhomedevice/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)     9700 2022-04-13 22:51:01.000000 openhomedevice-2.0.2/openhomedevice/device.py
--rw-r--r--   0 barry     (1000) barry     (1000)     6482 2022-02-18 23:58:29.000000 openhomedevice-2.0.2/openhomedevice/didl_lite.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2022-04-13 22:57:23.231451 openhomedevice-2.0.2/openhomedevice.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     6783 2022-04-13 22:57:23.000000 openhomedevice-2.0.2/openhomedevice.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      297 2022-04-13 22:57:23.000000 openhomedevice-2.0.2/openhomedevice.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2022-04-13 22:57:23.000000 openhomedevice-2.0.2/openhomedevice.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       36 2022-04-13 22:57:23.000000 openhomedevice-2.0.2/openhomedevice.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       15 2022-04-13 22:57:23.000000 openhomedevice-2.0.2/openhomedevice.egg-info/top_level.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       79 2022-04-13 22:57:23.235451 openhomedevice-2.0.2/setup.cfg
--rw-r--r--   0 barry     (1000) barry     (1000)      918 2022-04-13 22:28:30.000000 openhomedevice-2.0.2/setup.py
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-14 19:58:16.480407 openhomedevice-2.1/
+-rw-r--r--   0 barry      (502) staff       (20)     1076 2023-06-12 20:59:11.000000 openhomedevice-2.1/LICENSE.txt
+-rw-r--r--   0 barry      (502) staff       (20)     7141 2023-06-14 19:58:16.480531 openhomedevice-2.1/PKG-INFO
+-rw-r--r--   0 barry      (502) staff       (20)     6493 2023-06-14 19:55:10.000000 openhomedevice-2.1/README.md
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-14 19:58:16.478311 openhomedevice-2.1/openhomedevice/
+-rw-r--r--   0 barry      (502) staff       (20)       43 2023-06-12 20:59:11.000000 openhomedevice-2.1/openhomedevice/__init__.py
+-rw-r--r--   0 barry      (502) staff       (20)    10323 2023-06-14 19:50:16.000000 openhomedevice-2.1/openhomedevice/device.py
+-rw-r--r--   0 barry      (502) staff       (20)     6482 2023-06-12 20:59:11.000000 openhomedevice-2.1/openhomedevice/didl_lite.py
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-14 19:58:16.480157 openhomedevice-2.1/openhomedevice.egg-info/
+-rw-r--r--   0 barry      (502) staff       (20)     7141 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/PKG-INFO
+-rw-r--r--   0 barry      (502) staff       (20)      309 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/SOURCES.txt
+-rw-r--r--   0 barry      (502) staff       (20)        1 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/dependency_links.txt
+-rw-r--r--   0 barry      (502) staff       (20)       36 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/requires.txt
+-rw-r--r--   0 barry      (502) staff       (20)       15 2023-06-14 19:58:16.000000 openhomedevice-2.1/openhomedevice.egg-info/top_level.txt
+-rw-r--r--   0 barry      (502) staff       (20)       79 2023-06-14 19:58:16.480980 openhomedevice-2.1/setup.cfg
+-rw-r--r--   0 barry      (502) staff       (20)      914 2023-06-14 18:34:31.000000 openhomedevice-2.1/setup.py
```

### Comparing `openhomedevice-2.0.2/PKG-INFO` & `openhomedevice-2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,186 +1,236 @@
-Metadata-Version: 2.1
-Name: openhomedevice
-Version: 2.0.2
-Summary: Provides an API for requesting information from an Openhome device
-Home-page: https://github.com/bazwilliams/openhomedevice
-Author: Barry John Williams
-Author-email: barry@bjw.me.uk
-License: UNKNOWN
-Download-URL: https://github.com/bazwilliams/openhomedevice/tarball/2.0.1
-Description: # openhomedevice
-        
-        Library to provide an API to an existing openhome device. The device needs to have been discovered first by something like netdisco (https://github.com/home-assistant/netdisco).
-        
-        The underlying UPnP client library used is https://github.com/StevenLooman/async_upnp_client
-        
-        * Tested against [Linn Products Ltd](https://www.linn.co.uk/uk/) devices running Davaar 80 (thought expected to work on earlier variants)
-        * Tested against [OpenHome Player](http://openhome.org/) devices
-        
-        ## Installation
-        
-        `pip install openhomedevice`
-        
-        ## API
-        
-        ### Constructor
-        
-        ```python
-        device = Device(location)
-        await device.init()
-        ```
-        
-        ### Methods
-        
-        #### Control
-        
-        ```python
-            await set_standby(standbyRequested) #bool
-            await play() #starts playback
-            await play_media(track_details) #start playing `track_details`
-            await stop() #stops playback
-            await pause() #pauses playback
-            await skip(offset) #positive or negative integer
-            await set_volume(volume_level) #positive number
-            await increase_volume() #increase volume by 1
-            await decrease_volume() #decrease volume by 1
-            await set_mute(muteRequested) #bool
-            await set_source(index) #positive integer (use Sources() for indices)
-            await invoke_pin(index) #positive integer (use Pins() for indices)
-        ```
-        
-        #### Informational
-        
-        ```python
-            uuid() #Unique identifier
-            await name() #Name of device
-            await room() #Name of room
-            await is_in_standby() #returns true if in standby
-            await transport_state() #returns one of Stopped, Playing, Paused or Buffering.
-            volume_enabled #property true if the volume service is available
-            await volume_level() #returns the volume setting or None if disabled
-            await is_muted() #returns true if muted or None if disabled
-            await source() #returns the currently connected source as a dictionary
-            await sources() #returns an array of source dictionaries with indices
-            await track_info() #returns a track dictionary
-            await pins() #returns an array of pin dictionaries with indices
-            pins_enabled #property true if the pins service is available
-        ```
-        
-        ##### Source Response
-        
-        ```python
-        {
-            'type': 'Playlist',
-            'name': 'Playlist'
-        }
-        ```
-        
-        ##### Sources Response
-        
-        ```python
-        [
-            { 'index': 0, 'type': 'Playlist', 'name': 'Playlist' },
-            { 'index': 1, 'type': 'Radio', 'name': 'Radio' },
-            { 'index': 3, 'type': 'Receiver', 'name': 'Songcast' },
-            { 'index': 6, 'type': 'Analog', 'name': 'Front Aux' }
-        ]
-        ```
-        
-        ##### Pins Response
-        
-        ```python
-        [
-          {'index': 1, 'title': 'Playstation 4', 'artworkUri': 'external:///source?type=Hdmi&systemName=HDMI3'}
-          {'index': 4, 'title': 'Classic FM', 'artworkUri': 'http://cdn-profiles.tunein.com/s8439/images/logoq.png?t=1'}
-          {'index': 6, 'title': 'Chillout Playlist', 'artworkUri': 'http://media/artwork/chillout-playlist.png'}
-        ]
-        ```
-        
-        ##### TrackInfo Response
-        
-        ```python
-        {
-          "mimeType": "http-get:*:audio/x-flac:DLNA.ORG_OP=01;DLNA.ORG_FLAGS=01700000000000000000000000000000",
-          "rating": None,
-          "performer": [
-            "Fahmi Alqhai, Performer - Johann Sebastian Bach, Composer"
-          ],
-          "bitDepth": 16,
-          "channels": 2,
-          "disc": None,
-          "composer": [],
-          "year": 2017,
-          "duration": 460,
-          "author": [],
-          "albumArtist": [],
-          "type": "object.item.audioItem.musicTrack",
-          "narrator": [],
-          "description": None,
-          "conductor": [],
-          "albumArtwork": "http://static.qobuz.com/images/covers/58/20/8424562332058_600.jpg",
-          "track": 2,
-          "tracks": None,
-          "artwork": None,
-          "genre": [
-            "Klassiek"
-          ],
-          "publisher": "Glossa",
-          "albumGenre": [
-            "Klassiek"
-          ],
-          "artist": [
-            "Fahmi Alqhai"
-          ],
-          "bitRate": None,
-          "albumTitle": "The Bach Album",
-          "uri": "http://192.168.0.110:58050/stream/audio/b362f0f7a1ff33b176bcf2adde75af96.flac",
-          "discs": None,
-          "published": None,
-          "title": "Violin Sonata No. 2 in A Minor, BWV 1003 (Arr. for Viola da gamba) : Violin Sonata No. 2 in A Minor, BWV 1003 (Arr. for Viola da gamba): II. Fuga",
-          "sampleRate": 44100
-        }
-        ```
-        
-        ##### Playing A Track
-        
-        Use this to play a short audio track, a podcast Uri or radio station Uri. The audio will be played using the radio source of the device. The `trackDetails` object should be the same as the one described in the `TrackInfo` section above.
-        
-        ```python
-            trackDetails = {}
-            trackDetails["uri"] = "http://opml.radiotime.com/Tune.ashx?id=s122119"
-            trackDetails["title"] = 'Linn Radio (Eclectic Music)'
-            trackDetails["albumArtwork"] = 'http://cdn-radiotime-logos.tunein.com/s122119q.png'
-        
-            openhomeDevice.PlayMedia(trackDetails)
-        ```
-        
-        ## Example
-        
-        ```python
-        python3 demo.py
-        ```
-        
-        ## Running Tests
-        
-        ```bash
-        PYTHONPATH=. pytest ./tests/*
-        ```
-        
-        ## Uploading Package
-        
-        Following guide from https://packaging.python.org/tutorials/packaging-projects/
-        
-        Update version in `setup.py`
-        
-        ```sh
-        python3 setup.py sdist
-        twine upload dist/*
-        ```
-        
-Keywords: upnp,dlna,openhome,linn,ds,music,render,async
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# openhomedevice
+
+Library to provide an API to an existing openhome device. The device needs to have been discovered first by something like netdisco (https://github.com/home-assistant/netdisco).
+
+The underlying UPnP client library used is https://github.com/StevenLooman/async_upnp_client
+
+* Tested against [Linn Products Ltd](https://www.linn.co.uk/uk/) devices running Davaar 80 (thought expected to work on earlier variants)
+* Tested against [OpenHome Player](http://openhome.org/) devices
+
+## Installation
+
+`pip install openhomedevice`
+
+## API
+
+### Constructor
+
+```python
+device = Device(location)
+await device.init()
+```
+
+### Methods
+
+#### Control
+
+```python
+    await set_standby(standbyRequested) #bool
+    await play() #starts playback
+    await play_media(track_details) #start playing `track_details`
+    await stop() #stops playback
+    await pause() #pauses playback
+    await skip(offset) #positive or negative integer
+    await set_volume(volume_level) #positive number
+    await increase_volume() #increase volume by 1
+    await decrease_volume() #decrease volume by 1
+    await set_mute(muteRequested) #bool
+    await set_source(index) #positive integer (use Sources() for indices)
+    await invoke_pin(index) #positive integer (use Pins() for indices)
+```
+
+#### Firmware
+
+```python
+    await check_latest_firmware() #check for the latest firmware
+    await update_firmware() #update the device firmware
+    await software_status() #returns a dictionary with information about the current software
+```
+
+#### Informational
+
+```python
+    uuid() #Unique identifier
+    await name() #Name of device
+    await room() #Name of room
+    await is_in_standby() #returns true if in standby
+    await transport_state() #returns one of Stopped, Playing, Paused or Buffering.
+    volume_enabled #property true if the volume service is available
+    await volume_level() #returns the volume setting or None if disabled
+    await is_muted() #returns true if muted or None if disabled
+    await source() #returns the currently connected source as a dictionary
+    await sources() #returns an array of source dictionaries with indices
+    await track_info() #returns a track dictionary
+    await pins() #returns an array of pin dictionaries with indices
+    pins_enabled #property true if the pins service is available
+```
+
+##### Source Response
+
+```python
+{
+    'type': 'Playlist',
+    'name': 'Playlist'
+}
+```
+
+##### Sources Response
+
+```python
+[
+    { 'index': 0, 'type': 'Playlist', 'name': 'Playlist' },
+    { 'index': 1, 'type': 'Radio', 'name': 'Radio' },
+    { 'index': 3, 'type': 'Receiver', 'name': 'Songcast' },
+    { 'index': 6, 'type': 'Analog', 'name': 'Front Aux' }
+]
+```
+
+##### Pins Response
+
+```python
+[
+  {'index': 1, 'title': 'Playstation 4', 'artworkUri': 'external:///source?type=Hdmi&systemName=HDMI3'}
+  {'index': 4, 'title': 'Classic FM', 'artworkUri': 'http://cdn-profiles.tunein.com/s8439/images/logoq.png?t=1'}
+  {'index': 6, 'title': 'Chillout Playlist', 'artworkUri': 'http://media/artwork/chillout-playlist.png'}
+]
+```
+
+##### TrackInfo Response
+
+```python
+{
+  "mimeType": "http-get:*:audio/x-flac:DLNA.ORG_OP=01;DLNA.ORG_FLAGS=01700000000000000000000000000000",
+  "rating": None,
+  "performer": [
+    "Fahmi Alqhai, Performer - Johann Sebastian Bach, Composer"
+  ],
+  "bitDepth": 16,
+  "channels": 2,
+  "disc": None,
+  "composer": [],
+  "year": 2017,
+  "duration": 460,
+  "author": [],
+  "albumArtist": [],
+  "type": "object.item.audioItem.musicTrack",
+  "narrator": [],
+  "description": None,
+  "conductor": [],
+  "albumArtwork": "http://static.qobuz.com/images/covers/58/20/8424562332058_600.jpg",
+  "track": 2,
+  "tracks": None,
+  "artwork": None,
+  "genre": [
+    "Klassiek"
+  ],
+  "publisher": "Glossa",
+  "albumGenre": [
+    "Klassiek"
+  ],
+  "artist": [
+    "Fahmi Alqhai"
+  ],
+  "bitRate": None,
+  "albumTitle": "The Bach Album",
+  "uri": "http://192.168.0.110:58050/stream/audio/b362f0f7a1ff33b176bcf2adde75af96.flac",
+  "discs": None,
+  "published": None,
+  "title": "Violin Sonata No. 2 in A Minor, BWV 1003 (Arr. for Viola da gamba) : Violin Sonata No. 2 in A Minor, BWV 1003 (Arr. for Viola da gamba): II. Fuga",
+  "sampleRate": 44100
+}
+```
+
+##### SoftwareStatus response
+
+When an update is available:
+
+```python
+{
+   "status":"update_available",
+   "current_software":{
+      "version":"4.99.491",
+      "topic":"main",
+      "channel":"release"
+   },
+   "update_info":{
+      "legal":{
+         "licenseurl":"http://products.linn.co.uk/VersionInfo/licenseV2.txt",
+         "privacyurl":"https://www.linn.co.uk/privacy",
+         "privacyuri":"https://products.linn.co.uk/VersionInfo/PrivacyV1.json",
+         "privacyversion":1
+      },
+      "releasenotesuri":"http://docs.linn.co.uk/wiki/index.php/ReleaseNotes",
+      "updates":[
+         {
+            "channel":"release",
+            "date":"07 Jun 2023 12:29:48",
+            "description":"Release build version 4.100.502 (07 Jun 2023 12:29:48)",
+            "exaktlink":"3",
+            "manifest":"https://cloud.linn.co.uk/update/components/836/4.100.502/manifest.json",
+            "topic":"main",
+            "variant":"836",
+            "version":"4.100.502"
+         }
+      ],
+      "exaktUpdates":[]
+   }
+}
+```
+
+When the system is on the latest firmware:
+
+```python
+{
+   "status":"on_latest",
+   "current_software":{
+      "version":"4.100.502",
+      "topic":"main",
+      "channel":"release"
+   }
+}
+```
+
+##### Upgrading Firmware
+
+Use this to check if an update is required and then instruct the device to apply it
+
+```python
+    await openhomeDevice.check_latest_firmware()
+    await openhomeDevice.update_firmware()
+```
+
+##### Playing A Track
+
+Use this to play a short audio track, a podcast Uri or radio station Uri. The audio will be played using the radio source of the device. The `trackDetails` object should be the same as the one described in the `TrackInfo` section above.
+
+```python
+    track_details = {}
+    track_details["uri"] = "http://opml.radiotime.com/Tune.ashx?id=s122119"
+    track_details["title"] = 'Linn Radio (Eclectic Music)'
+    track_details["albumArtwork"] = 'http://cdn-radiotime-logos.tunein.com/s122119q.png'
+
+    openhomeDevice.PlayMedia(track_details)
+```
+
+## Example
+
+```python
+python3 demo.py
+```
+
+## Running Tests
+
+```bash
+PYTHONPATH=. pytest ./tests/*
+```
+
+## Uploading Package
+
+Following guide from https://packaging.python.org/tutorials/packaging-projects/
+
+Update version in `setup.py`
+
+```sh
+python3 setup.py sdist
+twine upload dist/*
+```
```

### Comparing `openhomedevice-2.0.2/openhomedevice/device.py` & `openhomedevice-2.1/openhomedevice/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             "urn:av-openhome-org:serviceId:Playlist"
         )
         self.info_service = self.device.service_id("urn:av-openhome-org:serviceId:Info")
         self.pins_service = self.device.service_id("urn:av-openhome-org:serviceId:Pins")
         self.radio_service = self.device.service_id(
             "urn:av-openhome-org:serviceId:Radio"
         )
+        self.update_service = self.device.service_id("urn:linn-co-uk:serviceId:Update")
 
     async def init(self):
         requester = AiohttpRequester()
         factory = UpnpFactory(requester)
         self.device = await factory.async_create_device(self.location)
         self.setup_services()
 
@@ -262,7 +263,22 @@
                 }
                 pins.append(pin)
         return pins
 
     async def invoke_pin(self, pin_id):
         if self.pins_enabled:
             await self.pins_service.action("InvokeIndex").async_call(Index=(pin_id - 1))
+
+    async def software_status(self):
+        if self.update_service:
+            action = self.update_service.action("GetSoftwareStatus")
+            result = await action.async_call()
+            return json.loads(result["SoftwareStatus"])
+
+    async def check_latest_firmware(self):
+        if self.update_service:
+            action = await self.update_service.action("CheckNow").async_call()
+
+    async def update_firmware(self):
+        if self.update_service:
+            await self.update_service.action("Apply").async_call()
+
```

### Comparing `openhomedevice-2.0.2/openhomedevice/didl_lite.py` & `openhomedevice-2.1/openhomedevice/didl_lite.py`

 * *Files identical despite different names*

### Comparing `openhomedevice-2.0.2/setup.py` & `openhomedevice-2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'openhomedevice',
-  version = '2.0.2',
+  version = '2.1',
   author = 'Barry John Williams',
   author_email = 'barry@bjw.me.uk',
   description='Provides an API for requesting information from an Openhome device',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/bazwilliams/openhomedevice',
   packages=setuptools.find_packages(),
-  download_url = 'https://github.com/bazwilliams/openhomedevice/tarball/2.0.1',
+  download_url = 'https://github.com/bazwilliams/openhomedevice/tarball/2.1',
   keywords = ['upnp', 'dlna', 'openhome', 'linn', 'ds', 'music', 'render', 'async'],
   install_requires = ['async_upnp_client>=0.27', 'lxml>=4.8.0'],
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

