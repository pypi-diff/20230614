# Comparing `tmp/openflexure_microscope_client-0.1.7.tar.gz` & `tmp/openflexure_microscope_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openflexure_microscope_client-0.1.7.tar", max compression
+gzip compressed data, was "openflexure_microscope_client-0.1.8.tar", max compression
```

## Comparing `openflexure_microscope_client-0.1.7.tar` & `openflexure_microscope_client-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     5892 2022-10-18 10:00:56.191491 openflexure_microscope_client-0.1.7/README.md
--rw-r--r--   0        0        0      182 2022-10-18 10:00:56.191491 openflexure_microscope_client-0.1.7/openflexure_microscope_client/__init__.py
--rw-r--r--   0        0        0    12808 2022-10-18 10:00:56.191491 openflexure_microscope_client-0.1.7/openflexure_microscope_client/microscope_client.py
--rw-r--r--   0        0        0      483 2022-10-18 10:00:56.191491 openflexure_microscope_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6801 1970-01-01 00:00:00.000000 openflexure_microscope_client-0.1.7/setup.py
--rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 openflexure_microscope_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     5892 2023-06-14 08:55:03.134579 openflexure_microscope_client-0.1.8/README.md
+-rw-r--r--   0        0        0      182 2023-06-14 08:55:03.134579 openflexure_microscope_client-0.1.8/openflexure_microscope_client/__init__.py
+-rw-r--r--   0        0        0    15365 2023-06-14 08:55:03.134579 openflexure_microscope_client-0.1.8/openflexure_microscope_client/microscope_client.py
+-rw-r--r--   0        0        0      483 2023-06-14 08:55:03.135579 openflexure_microscope_client-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 openflexure_microscope_client-0.1.8/PKG-INFO
```

### Comparing `openflexure_microscope_client-0.1.7/README.md` & `openflexure_microscope_client-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `openflexure_microscope_client-0.1.7/openflexure_microscope_client/microscope_client.py` & `openflexure_microscope_client-0.1.8/openflexure_microscope_client/microscope_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import json
 import time
 import io
 import PIL.Image
 import numpy as np
 import logging
 import zeroconf
+import os
 
 ACTION_RUNNING_KEYWORDS = ["idle", "pending", "running"]
 ACTION_OUTPUT_KEYS = ["output", "return"]
 
 class MicroscopeClient(object):
     def __init__(self, host, port=5000):
         if isinstance(host, zeroconf.ServiceInfo):
@@ -116,22 +117,24 @@
         return r.json()
 
     def grab_image_raw(self):
         r = requests.get(self.base_uri + "/streams/snapshot")
         r.raise_for_status()
         return r.content
 
-    def capture_image(self, params: dict = None):
-        """Capture an image and return it as a PIL image object"""
+    def capture_image(self):
+        """Capture an image and return it as a PIL image object
+        A RAM capture is only possible with an image from
+        the preview stream.
+        For a higher res image, you'll need to use a combination
+        of capture_image_to_disk and download_from_id"""
         payload = {
             "use_video_port": True,
             "bayer": False,
         }
-        if params:
-            payload.update(params)
         r = requests.post(self.base_uri + "/actions/camera/ram-capture", json=payload, headers={'Accept': 'image/jpeg'})
         r.raise_for_status()
         image = PIL.Image.open(io.BytesIO(r.content))
         return image
 
     def grab_mjpeg(self, timeout, output=None, stop_event=None, max_size=None):
         """Capture the mjpeg stream from the camera"""
@@ -161,51 +164,114 @@
         payload = {
             "use_video_port": True,
             "bayer": False,
             "temporary" :False
         }
         if params:
             payload.update(params)
-        r = requests.post(self.base_uri + "/actions/camera/capture", json=payload)
+        r = self.post_json(self.base_uri + "/actions/camera/capture", payload, wait_on_task=True)
         return r
 
     def grab_image(self):
         """Grab an image from the stream and return as a PIL image object"""
         image = PIL.Image.open(io.BytesIO(self.grab_image_raw()))
         return image
+    
+    def list_capture_ids(self):
+        """List all of the captures on the Pi
+        by their ids"""
+        ids = []
+        data = self.get_json("/captures")
+        for image in data:
+            ids.append(image['id'])
+        return ids
+
+    def delete_image(self, id):
+        """Delete an image on the Pi from 
+        the capture ids"""
+        r = requests.delete(self.base_uri + f"/captures/{id}")
+        return r
 
+    def get_capture_metadata(self, id):
+        """Return the metadata from the
+        capture of the id supplied"""
+        r = requests.get(self.base_uri + f"/captures/{id}")
+        r.raise_for_status()
+        return r.json()
+    
     def grab_image_array(self, ):
         """Grab an image and return it as a numpy ndarray"""
         return np.array(self.grab_image())
 
     def move_and_measure(self, params: dict):
         """Move in z and track the JPEG size against time"""
         return self.extensions["org.openflexure.autofocus"]["move_and_measure"].post_json(params)
 
+    def download_from_id(self, id, folderpath):
+        """Download image from id, and save it (with metadata) in folderpath"""
+        link = self.base_uri
+        r = requests.get(link + "/captures/" + id + "/download/my_image.jpg")
+        r.raise_for_status()
+        im = r.content
+        data = self.get_capture_metadata(id)['metadata']
+
+        file_path = os.path.join(folderpath, data['image']['name'])
+
+        with open(file_path, "wb") as f:
+            f.write(im)
+        return file_path
+
+    def pull_settings(self):
+        """Download the current microscope settings as a JSON"""
+        return self.get_json("/instrument/settings")
+
+    def move_in_pixels(self, x, y):
+        """Move by pixels in the stream (not in the full res image)
+        This is x and y according to the server coordinates;
+        may be more intuitive to think of it as
+        x as y and y as x"""
+        return self.extensions["org.openflexure.camera_stage_mapping"]["move_in_image_coordinates"].post_json({'x':x,'y':y})
+
+    def move_by_percent(self, x, y):
+        """Move by percent of the field of view
+        This is x and y according to the server coordinates;
+        may be more intuitive to think of it as
+        x as y and y as x"""
+        settings = self.pull_settings()
+        fov = settings['camera']['stream_resolution']
+        try:
+            x *= fov[1]/100
+            y *= fov[0]/100
+        except:
+            logging.debug('Invalid keys in move by percent request, expecting "x" and "y"')
+        return self.extensions["org.openflexure.camera_stage_mapping"]["move_in_image_coordinates"].post_json({'x':x,'y':y})
+
     def calibrate_xy(self):
         """Move the stage in X and Y to calibrate stage movements vs camera coordinates
         
         NB this takes around 2 minutes to complete with a 40x objective.  Lower magnification
         may work less well.
         """
         return self.extensions["org.openflexure.camera_stage_mapping"]["calibrate_xy"].post_json()
 
-    def autofocus(self):
+    def autofocus(self, dz = 2000):
         """Move the stage up and down, and pick the sharpest position."""
-        return self.extensions["org.openflexure.autofocus"]["fast_autofocus"].post_json()
+        return self.extensions["org.openflexure.autofocus"]["fast_autofocus"].post_json({'dz':dz})
 
     def laplacian_autofocus(self, params: dict):
         """run a slower autofocus at heights dz respective to the starting point"""
         return self.extensions["org.openflexure.autofocus"]["autofocus"].post_json(params)
 
     def scan(self, params: dict, wait_on_task=True):
         """autofocus_dz: 20 is roughly fine, 30 is roughly medium"""
         return self.extensions["org.openflexure.scan"]["tile"].post_json(params, wait_on_task=wait_on_task)
 
     def grab_image_size(self):
+        """Get the size of the MJPEG
+        stream at the current FOV"""
         file_bytes = io.BytesIO(self.grab_image_raw())
         value = file_bytes.getvalue()
         length_size = len(value)
         return length_size
 
     @property
     def configuration(self):
```

### Comparing `openflexure_microscope_client-0.1.7/setup.py` & `openflexure_microscope_client-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,104 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['openflexure_microscope_client']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pillow>=9.0,<10.0',
- 'numpy>=1.21,<2.0',
- 'requests>=2.28,<3.0',
- 'zeroconf>=0.39,<0.40']
-
-setup_kwargs = {
-    'name': 'openflexure-microscope-client',
-    'version': '0.1.7',
-    'description': 'Python client code for the OpenFlexure Microscope',
-    'long_description': '# A Python client for the OpenFlexure Microscope.  \n\nThe [OpenFlexure Microscope] is most often controlled by two pieces of software - the [OpenFlexure Microscope Server], which is written in Python and runs on the embedded Raspberry Pi, and [OpenFlexure Connect][Connect] which is a graphical interface written in Electron, that can be run either on the Raspberry Pi, or on another computer via a network connection.  However, if you want to write your own scripts to perform particular experiments or protocols, it\'s useful not to have to embed these into the the [OpenFlexure Microscope Server] or package them up as plugins.  This library exists to make it easy to control your microscope from a simple Python script that can run either on the Raspberry Pi, or over the network.  I particularly like to use it from a [Jupyter] notebook on my laptop, because it allows me to plot graphs and display images as I go.\n\n## Installation\n\nThis module can be installed with ``pip install openflexure-microscope-client``, or by cloning the repository and running ``poetry install``.\n\n## Usage\n\n### Connect to your microscope\nYou can connect to the microscope either by specifying a hostname or IP address, or using mDNS.  If your network is relatively simple, and if you can see your microscope in the "nearby devices" section of [Connect], then mDNS is a zero-faff way of connecting to your microscope:\n```python\nimport openflexure_microscope_client as ofm_client\nmicroscope = ofm_client.find_first_microscope()\n```\nIf your network is more complicated, or you know the address of your microscope, you can connect using the hostname or IP address.  By default, your microscope will declare itself as ``microscope.local`` though this also relies on mDNS so if the method above doesn\'t work, ``microscope.local`` may also not work.  \n```python\nmicroscope = ofm_client.MicroscopeClient("example.host.name")\n```\n\n### Check the connection\nUsually, I run a few commands to check my microscope is working properly:\n```python\npos = microscope.position\nstarting_pos = pos.copy()\npos[\'x\'] += 100\nmicroscope.move(pos)\nassert microscope.position == pos\npos[\'x\'] -= 100\nmicroscope.move(pos)\nassert microscope.position == starting_pos\n\n# Check the microscope will autofocus\nret = microscope.autofocus()\n\n# Acquire an image for sanity-checking too\nimage = microscope.grab_image()\nf, ax = plt.subplots(1,1)\nax.imshow(np.array(image))\n#print(image.metadata)\nprint("Active microscope extensions")\nfor k in microscope.extensions.keys():\n    print(k)\n```\nAfter running this block, you should see a list of extensions that are currently active, and a picture taken by the microscope.  Given that we just autofocused, this image should be nice and sharp!\n\n### Basic commands\nThere are a few basic commands built in as methods of the ``MicroscopeClient`` object:\n  * ``position`` is a property that returns a dictionary with ``\'x\'``, ``\'y\'``, and ``\'z\'`` components, giving the position of the stage.\n  * ``get_position_array()`` returns a 3-element ``numpy`` array with the same position in it.\n  * ``move(position)`` accepts either a 3-element array or a dictionary as returned by ``position``, and performs an absolute move\n  * ``move_rel(displacement)`` performs a relative move (i.e. supplying 0 will not move that axis)\n  * ``capture_image()`` will take a new image from the camera and return it as a ``PIL`` image object\n  * ``grab_image()`` will return the next image the camera sends in its MJPEG preview stream (i.e. it\'s quicker but lower quality than ``capture_image()``)\n  * ``grab_image_array()`` returns the image as a ``numpy`` array.\n  * ``autofocus()`` runs the fast autofocus routine, just like clicking the "autofocus" button in [Connect]\n\n### Extensions\nTo run methods provided by the microscope extensions, you can use the ``extensions`` dictionary, to make ``get`` or ``post`` requests:\n```python\nmicroscope.extensions["your.extension.name"]["link_name"].get()\nmicroscope.extensions["your.extension.name"]["link_name"].post_json({"key":"value"})\n```\n\n### Arguments and documentation\nThere is not currently much documentation beyond this README for the Python client.  However, the microscope API is pretty well documented.  This is the place to go to find out the details of what each command does, and what the arguments mean, particularly for any of the commands that take a `payload` argument; that\'s converted to JSON and passed directly to the corresponding HTTP POST request.  Currently, there is a static version of the API documentation linked from the [server readthedocs page], or you can access a live interactive version from `http://microscope.local:5000/api/v2/docs/swagger-ui`, replacing `microscope.local` with the IP or hostname of your microscope.\n\n[server readthedocs page]: https://openflexure-microscope-software.readthedocs.io/en/master/api.html\n\n\n## Development\n### Installation\nThe dependencies are managed using poetry, so once you have cloned the repository, you can set up a virtual environment with ``poetry install``.\n\n### Tests\nThere are some basic tests that can be run using ``pytest``.  This needs to be within the environment installed above, so use ``poetry run pytest``.  These mostly need to connect to a microscope; the easiest way to test this automatically is to build ``openflexure-microscope-server`` and run it locally - this will create a local dummy microscope server.  Some tests will be skipped because they need microscope hardware, but it should at least verify most of the URLs.  Running the tests requires you to have started that server already - it will not be started automatically.\n\n[OpenFlexure Microscope]: https://openflexure.org/projects/microscope/\n[Connect]: https://gitlab.com/openflexure/openflexure-connect\n[OpenFlexure Microscope Server]: https://gitlab.com/openflexure/openflexure-microscope-server/\n[Jupyter]: https://jupyter.org/',
-    'author': 'Richard Bowman',
-    'author_email': 'richard.bowman@cantab.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/openflexure/openflexure-microscope-pyclient/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: openflexure-microscope-client
+Version: 0.1.8
+Summary: Python client code for the OpenFlexure Microscope
+Home-page: https://gitlab.com/openflexure/openflexure-microscope-pyclient/
+License: LGPL-3.0-or-later
+Author: Richard Bowman
+Author-email: richard.bowman@cantab.net
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.0,<10.0)
+Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: zeroconf (>=0.39,<0.40)
+Description-Content-Type: text/markdown
+
+# A Python client for the OpenFlexure Microscope.  
+
+The [OpenFlexure Microscope] is most often controlled by two pieces of software - the [OpenFlexure Microscope Server], which is written in Python and runs on the embedded Raspberry Pi, and [OpenFlexure Connect][Connect] which is a graphical interface written in Electron, that can be run either on the Raspberry Pi, or on another computer via a network connection.  However, if you want to write your own scripts to perform particular experiments or protocols, it's useful not to have to embed these into the the [OpenFlexure Microscope Server] or package them up as plugins.  This library exists to make it easy to control your microscope from a simple Python script that can run either on the Raspberry Pi, or over the network.  I particularly like to use it from a [Jupyter] notebook on my laptop, because it allows me to plot graphs and display images as I go.
+
+## Installation
+
+This module can be installed with ``pip install openflexure-microscope-client``, or by cloning the repository and running ``poetry install``.
+
+## Usage
+
+### Connect to your microscope
+You can connect to the microscope either by specifying a hostname or IP address, or using mDNS.  If your network is relatively simple, and if you can see your microscope in the "nearby devices" section of [Connect], then mDNS is a zero-faff way of connecting to your microscope:
+```python
+import openflexure_microscope_client as ofm_client
+microscope = ofm_client.find_first_microscope()
+```
+If your network is more complicated, or you know the address of your microscope, you can connect using the hostname or IP address.  By default, your microscope will declare itself as ``microscope.local`` though this also relies on mDNS so if the method above doesn't work, ``microscope.local`` may also not work.  
+```python
+microscope = ofm_client.MicroscopeClient("example.host.name")
+```
+
+### Check the connection
+Usually, I run a few commands to check my microscope is working properly:
+```python
+pos = microscope.position
+starting_pos = pos.copy()
+pos['x'] += 100
+microscope.move(pos)
+assert microscope.position == pos
+pos['x'] -= 100
+microscope.move(pos)
+assert microscope.position == starting_pos
+
+# Check the microscope will autofocus
+ret = microscope.autofocus()
+
+# Acquire an image for sanity-checking too
+image = microscope.grab_image()
+f, ax = plt.subplots(1,1)
+ax.imshow(np.array(image))
+#print(image.metadata)
+print("Active microscope extensions")
+for k in microscope.extensions.keys():
+    print(k)
+```
+After running this block, you should see a list of extensions that are currently active, and a picture taken by the microscope.  Given that we just autofocused, this image should be nice and sharp!
+
+### Basic commands
+There are a few basic commands built in as methods of the ``MicroscopeClient`` object:
+  * ``position`` is a property that returns a dictionary with ``'x'``, ``'y'``, and ``'z'`` components, giving the position of the stage.
+  * ``get_position_array()`` returns a 3-element ``numpy`` array with the same position in it.
+  * ``move(position)`` accepts either a 3-element array or a dictionary as returned by ``position``, and performs an absolute move
+  * ``move_rel(displacement)`` performs a relative move (i.e. supplying 0 will not move that axis)
+  * ``capture_image()`` will take a new image from the camera and return it as a ``PIL`` image object
+  * ``grab_image()`` will return the next image the camera sends in its MJPEG preview stream (i.e. it's quicker but lower quality than ``capture_image()``)
+  * ``grab_image_array()`` returns the image as a ``numpy`` array.
+  * ``autofocus()`` runs the fast autofocus routine, just like clicking the "autofocus" button in [Connect]
+
+### Extensions
+To run methods provided by the microscope extensions, you can use the ``extensions`` dictionary, to make ``get`` or ``post`` requests:
+```python
+microscope.extensions["your.extension.name"]["link_name"].get()
+microscope.extensions["your.extension.name"]["link_name"].post_json({"key":"value"})
+```
+
+### Arguments and documentation
+There is not currently much documentation beyond this README for the Python client.  However, the microscope API is pretty well documented.  This is the place to go to find out the details of what each command does, and what the arguments mean, particularly for any of the commands that take a `payload` argument; that's converted to JSON and passed directly to the corresponding HTTP POST request.  Currently, there is a static version of the API documentation linked from the [server readthedocs page], or you can access a live interactive version from `http://microscope.local:5000/api/v2/docs/swagger-ui`, replacing `microscope.local` with the IP or hostname of your microscope.
+
+[server readthedocs page]: https://openflexure-microscope-software.readthedocs.io/en/master/api.html
+
+
+## Development
+### Installation
+The dependencies are managed using poetry, so once you have cloned the repository, you can set up a virtual environment with ``poetry install``.
+
+### Tests
+There are some basic tests that can be run using ``pytest``.  This needs to be within the environment installed above, so use ``poetry run pytest``.  These mostly need to connect to a microscope; the easiest way to test this automatically is to build ``openflexure-microscope-server`` and run it locally - this will create a local dummy microscope server.  Some tests will be skipped because they need microscope hardware, but it should at least verify most of the URLs.  Running the tests requires you to have started that server already - it will not be started automatically.
+
+[OpenFlexure Microscope]: https://openflexure.org/projects/microscope/
+[Connect]: https://gitlab.com/openflexure/openflexure-connect
+[OpenFlexure Microscope Server]: https://gitlab.com/openflexure/openflexure-microscope-server/
+[Jupyter]: https://jupyter.org/
```

