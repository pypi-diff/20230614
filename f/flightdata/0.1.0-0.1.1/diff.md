# Comparing `tmp/flightdata-0.1.0.tar.gz` & `tmp/flightdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightdata-0.1.0.tar", last modified: Wed Mar  1 19:07:25 2023, max compression
+gzip compressed data, was "flightdata-0.1.1.tar", last modified: Wed Jun 14 09:40:50 2023, max compression
```

## Comparing `flightdata-0.1.0.tar` & `flightdata-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:07:25.299802 flightdata-0.1.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     7632 2023-03-01 17:16:16.000000 flightdata-0.1.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     4298 2023-03-01 19:07:25.299802 flightdata-0.1.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     4018 2022-12-20 14:21:12.000000 flightdata-0.1.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:07:25.289802 flightdata-0.1.0/flightdata/
--rw-r--r--   0 tom       (1000) tom       (1000)       62 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:07:25.299802 flightdata-0.1.0/flightdata/config/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/config/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/config/ardupilot.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8826 2023-03-01 17:31:10.000000 flightdata-0.1.0/flightdata/data.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:07:25.299802 flightdata-0.1.0/flightdata/field_mapping/
--rw-r--r--   0 tom       (1000) tom       (1000)      309 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/field_mapping/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4776 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/field_mapping/ardupilot_ekfv2.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4426 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/field_mapping/ardupilot_ekfv3.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1968 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/field_mapping/fc_json_2_1.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6127 2022-12-20 14:21:12.000000 flightdata-0.1.0/flightdata/fields.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:07:25.299802 flightdata-0.1.0/flightdata.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     4298 2023-03-01 19:07:25.000000 flightdata-0.1.0/flightdata.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      512 2023-03-01 19:07:25.000000 flightdata-0.1.0/flightdata.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-03-01 19:07:25.000000 flightdata-0.1.0/flightdata.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-03-01 19:07:25.000000 flightdata-0.1.0/flightdata.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-03-01 19:07:25.000000 flightdata-0.1.0/flightdata.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      402 2023-03-01 19:07:25.299802 flightdata-0.1.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      672 2023-03-01 17:10:27.000000 flightdata-0.1.0/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:07:25.299802 flightdata-0.1.0/test/
--rw-r--r--   0 tom       (1000) tom       (1000)     4091 2022-12-20 14:21:13.000000 flightdata-0.1.0/test/test_data.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:40:50.637548 flightdata-0.1.1/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 15:54:19.000000 flightdata-0.1.1/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4298 2023-06-14 09:40:50.637548 flightdata-0.1.1/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4018 2023-03-28 15:54:19.000000 flightdata-0.1.1/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:40:50.637548 flightdata-0.1.1/flightdata/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       62 2023-03-28 15:54:19.000000 flightdata-0.1.1/flightdata/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:40:50.637548 flightdata-0.1.1/flightdata/config/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-03-28 15:54:19.000000 flightdata-0.1.1/flightdata/config/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1034 2023-03-28 15:54:19.000000 flightdata-0.1.1/flightdata/config/ardupilot.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     9122 2023-06-05 21:20:49.000000 flightdata-0.1.1/flightdata/data.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:40:50.637548 flightdata-0.1.1/flightdata/field_mapping/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      309 2023-03-28 15:54:19.000000 flightdata-0.1.1/flightdata/field_mapping/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4416 2023-06-05 21:20:49.000000 flightdata-0.1.1/flightdata/field_mapping/ardupilot.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4776 2023-03-28 15:54:19.000000 flightdata-0.1.1/flightdata/field_mapping/ardupilot_ekfv2.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4426 2023-03-28 15:54:19.000000 flightdata-0.1.1/flightdata/field_mapping/ardupilot_ekfv3.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1968 2023-03-28 15:54:19.000000 flightdata-0.1.1/flightdata/field_mapping/fc_json_2_1.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5101 2023-05-21 13:09:46.000000 flightdata-0.1.1/flightdata/fields.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:40:50.637548 flightdata-0.1.1/flightdata.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4298 2023-06-14 09:40:50.000000 flightdata-0.1.1/flightdata.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      573 2023-06-14 09:40:50.000000 flightdata-0.1.1/flightdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 09:40:50.000000 flightdata-0.1.1/flightdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       39 2023-06-14 09:40:50.000000 flightdata-0.1.1/flightdata.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       11 2023-06-14 09:40:50.000000 flightdata-0.1.1/flightdata.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-06-14 09:40:50.637548 flightdata-0.1.1/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      672 2023-03-28 15:54:19.000000 flightdata-0.1.1/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:40:50.637548 flightdata-0.1.1/test/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      155 2023-06-05 21:20:49.000000 flightdata-0.1.1/test/test_ardupilot.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4224 2023-05-21 13:14:11.000000 flightdata-0.1.1/test/test_data.py
```

### Comparing `flightdata-0.1.0/LICENSE` & `flightdata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flightdata-0.1.0/PKG-INFO` & `flightdata-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Module for handling UAV flight log data
 Home-page: https://github.com/PyFlightCoach/FlightData
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightdata-0.1.0/README.md` & `flightdata-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flightdata-0.1.0/flightdata/config/ardupilot.py` & `flightdata-0.1.1/flightdata/config/ardupilot.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.1.0/flightdata/data.py` & `flightdata-0.1.1/flightdata/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from enum import Enum
 
 from ardupilot_log_reader.reader import Ardupilot
 
 from .fields import Fields, CIDTypes
 from .field_mapping import get_ardupilot_mapping
 from .field_mapping.fc_json_2_1 import fc_json_2_1_io_info
-from geometry import GPS, Point, Quaternion
-from geometry.gps import GPS
+from geometry import GPS, Point, Quaternion, PX
+from pathlib import Path
+
 
 fdict = Fields.to_dict()
 
 class Flight(object):
     def __init__(self, data, parameters: List = None, zero_time_offset: float = 0):
         self.data = data
         self.parameters = parameters
@@ -35,80 +36,87 @@
         self._origin = None
 
     def flying_only(self, minalt=5, minv=10):
         vs = abs(Point(self.read_fields(Fields.VELOCITY)))
         above_ground = self.data.loc[(self.data.position_z <= -minalt) & (vs > minv)]
         return self[above_ground.index[0]:above_ground.index[-1]]
 
-
     def __getattr__(self, name):
         if name in Fields.all_names:
             return self.data[name]
         if name.upper() in fdict.keys():
             return self.read_fields(fdict[name.upper()])
 
     def __getitem__(self, sli):
         if isinstance(sli, int) or isinstance(sli, float):
-            return self.data.iloc[self.data.index.get_loc(sli, method="nearest")]
+            return self.data.iloc[self.data.index.get_loc(sli)]
         else:
             return Flight(self.data.loc[sli], self.parameters, self.zero_time)
 
+    def slice_raw_t(self, sli):
+        inds = self.data.reset_index().set_index("time_flight")["time_index"].loc[sli].to_numpy()#set_index("t", drop=False).columns
+
+        return Flight(self.data.loc[inds], self.parameters, self.zero_time)
+        
+
+
     def to_csv(self, filename):
         self.data.to_csv(filename)
         return filename
 
     @staticmethod
     def from_csv(filename):
         data = pd.read_csv(filename)
         data.index = data[Fields.TIME.names[0]].copy()
         data.index.name = 'time_index'
         return Flight(data)
 
     @staticmethod
-    def from_log(log_path, additional_fields=None):
+    def from_log(log_path, *args):
         """Constructor from an ardupilot bin file.
             fields are renamed and units converted to the tool fields defined in ./fields.py
             The input fields, read from the log are specified in ./mapping 
 
             Args:
                 log_path (str): [description]
         """
         
-        _field_request = ['XKF1', 'XKQ1', 'NKF1', 'NKQ1', 'NKF2', 'XKF2', 'ARSP', 'GPS', 'RCIN', 'RCOU', 'IMU', 'BARO', 'MODE', 'RPM', 'MAG', 'BAT', 'BAT2']
-        if additional_fields:
-            _field_request += additional_fields
-        _parser = Ardupilot(log_path, types=_field_request,zero_time_base=True)
+        _field_request = ['POS', 'ATT', 'ACC', 'GYRO', 'IMU', 'ARSP', 'GPS', 'RCIN', 'RCOU', 'BARO', 'MODE', 'RPM', 'MAG', 'BAT', 'BAT2']
+        if isinstance(log_path, Path):
+            log_path = str(log_path)
+        _parser = Ardupilot(log_path, types=_field_request+list(args))#,zero_time_base=True)
         fulldf = _parser.join_logs(_field_request)
-
+        
         return Flight.convert_df(
             fulldf,
             get_ardupilot_mapping(_parser.parms['AHRS_EKF_TYPE']),
             _parser.parms
         )
 
     @staticmethod
     def convert_df(fulldf, ioinfo, parms):
         # expand the dataframe to include all the columns listed in the io_info instance
-        input_data = fulldf.get(list(set(fulldf.columns.to_list())
-                                     & set(ioinfo.io_names)))
+        input_data = fulldf.get(
+            list(
+                set(fulldf.columns.to_list()) & set(ioinfo.io_names)
+        ))
 
         # Generate a reordered io instance to match the columns in the dataframe
         _fewer_io_info = ioinfo.subset(input_data.columns.to_list())
 
         _data = input_data * _fewer_io_info.factors_to_base  # do the unit conversion
         _data.columns = _fewer_io_info.base_names  # rename the columns
 
         # add the missing tool columns
         missing_cols = pd.DataFrame(
-            columns=list(set(Fields.all_names()) - set(_data.columns.to_list())) + [Fields.TIME.names[0]]
+            columns=list(set(Fields.all_names) - set(_data.columns.to_list())) + [Fields.TIME.names[0]]
         )
         output_data = _data.merge(missing_cols, on=Fields.TIME.names[0], how='left')
 
-        # set the first time in the index to 0
-        output_data.index = _data[Fields.TIME.names[0]].copy()
+        output_data = output_data.set_index(Fields.TIME.names[0], drop=False)
         output_data.index.name = 'time_index'
 
         return Flight(output_data, parms)
 
     @staticmethod
     def from_fc_json(fc_json):
         df = pd.DataFrame.from_dict(fc_json['data'])
@@ -157,26 +165,28 @@
     def origin(self) -> GPS:
         """the latitude and longitude of the origin (first pos in log)
 
         Returns:
             dict: origin GPS
         """
         if self._origin is None:
-            allgps = self.read_fields(Fields.GLOBALPOSITION)
-
-            self._origin = GPS(*allgps.iloc[0])
+            self._origin = GPS(*self.read_fields(Fields.GLOBALPOSITION).loc[self.gps_ready_time()])
         return self._origin
 
+    def gps_ready_time(self):
+        gps = self.read_fields(Fields.GLOBALPOSITION)
+        gps = gps.loc[~(gps==0).all(axis=1)].dropna()
+        return gps.iloc[0].name
 
     def imu_ready_time(self):
-        qs = Quaternion(self.read_fields(Fields.QUATERNION))
-        if np.any(pd.isna(qs)):
-            qs = Quaternion.from_euler(Point(self.read_fields(Fields.ATTITUDE)))
-        df = qs.transform_point(Point(1, 0, 0)).to_pandas(index=self.data.index)
-        return df.loc[(df.x!=1.0) | (df.y!=0.0) | (df.z!=0.0)].iloc[20].name
+        qs = Quaternion.from_euler(Point(self.read_fields(Fields.ATTITUDE)))
+        df = qs.transform_point(PX(1)).to_pandas(index=self.data.index)
+        att_ready = df.loc[(df.x!=1.0) | (df.y!=0.0) | (df.z!=0.0)].iloc[0].name
+
+        return max(self.gps_ready_time(), att_ready)
 
     def subset(self, start_time: float, end_time: float):
         """generate a subset between the specified times
 
         Args:
             start_time (float): the start of the subset, 0 for the start of the dataset
             end_time (float): end of the subset, -1 for the end of the flight
@@ -208,15 +218,15 @@
     def unique_identifier(self) -> str:
         """Return a string to identify this flight that is very unlikely to be the same as a different flight
 
         Returns:
             str: flight identifier
         """
         _ftemp = Flight(self.data.loc[self.data.position_z < -10])
-        return "{}_{:.8f}_{:.6f}_{:.6f}".format(len(_ftemp.data), _ftemp.duration, *self.origin.to_list())
+        return "{}_{:.8f}_{:.6f}_{:.6f}".format(len(_ftemp.data), _ftemp.duration, *self.origin.data[0])
 
     def describe(self):
         info = dict(
             duration = self.duration,
             origin_gps = self.origin.to_dict(),
             last_gps_ = GPS(*self.read_fields(Fields.GLOBALPOSITION).iloc[-1]).to_dict(),
             average_gps = GPS(*self.read_fields(Fields.GLOBALPOSITION).mean()).to_dict(),
```

### Comparing `flightdata-0.1.0/flightdata/field_mapping/ardupilot_ekfv2.py` & `flightdata-0.1.1/flightdata/field_mapping/ardupilot_ekfv2.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.1.0/flightdata/field_mapping/ardupilot_ekfv3.py` & `flightdata-0.1.1/flightdata/field_mapping/ardupilot_ekfv3.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.1.0/flightdata/field_mapping/fc_json_2_1.py` & `flightdata-0.1.1/flightdata/field_mapping/fc_json_2_1.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.1.0/flightdata/fields.py` & `flightdata-0.1.1/flightdata/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 
 from pint import UnitRegistry, DimensionalityError
 from typing import Dict, List
+from itertools import chain
+
 ureg = UnitRegistry()
 
 
 _field_list = []
 
 # TODO rewrite all this, allow multiple units per field. better to look more like /flightdata/mapping/ardupilot_ekfv3.py
 class CIDTypes():
@@ -71,102 +73,49 @@
     VELOCITY = Field('velocity', ureg.meter / ureg.second, 3, description='velocity data (earth frame)', names=['x', 'y', 'z'])
     WIND = Field('wind', ureg.meter / ureg.second, 2, description='wind in earth frame', names=['x', 'y'])
     RPM = Field('rpm', 1 / ureg.minute, 2, description='motor rpm')
     MAGNETOMETER = Field('magnetometer', 1, 3, description='mag field strength n, e, d')
     PRESSURE = Field('pressure', ureg.pascal, 1) 
     TEMPERATURE = Field('temperature', ureg.kelvin, 1) 
     
-    @staticmethod
-    def all():
-        return _field_list
-
-    @staticmethod
-    def all_names():
-        _all_names = []
-        for field in _field_list:
-            _all_names += field.names
-        return _all_names
+    all = _field_list
+    all_names = list(chain(*[field.names for field in _field_list]))
 
     @staticmethod
     def some_names(fields):
-        if isinstance(fields, list):
-            _some_names = []
-            for field in fields:
-                _some_names += field.names
-            return _some_names
-        else:
-            return fields.names
+        return [field.names for field in fields] if isinstance(fields, list) else fields.names
 
     @staticmethod
     def to_dict():
         return {field.name: field.names for field in _field_list}
 
 
 class MappedField(object):
     def __init__(self, field, position, name, unit):
         super().__init__()
-        self._field = field
-        self._position = position
-        self._name = name
-        self._unit = unit
-        self._base_factor = None
-
-    @property
-    def field(self):
-        return self._field
-
-    @property
-    def position(self):
-        return self._position
-
-    @property
-    def unit(self):
-        return self._unit
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def base_factor(self):
-        if not self._base_factor:
-            try:
-                self._base_factor = float(self.unit) / float(self.field.unit)
-            except DimensionalityError:
-                quantity = 1 * self.unit
-                self._base_factor = quantity.to(self.field.unit).magnitude
-        return self._base_factor
+        self.field = field
+        self.position = position
+        self.name = name
+        self.unit = unit
+        try:
+            self.base_factor = float(self.unit) / float(self.field.unit)
+        except DimensionalityError:
+            self.base_factor = (1 * self.unit).to(self.field.unit).magnitude
 
 
 class FieldIOInfo(object):
     def __init__(self, field_maps: Dict[str, MappedField]):
         self._field_maps = field_maps
 
-        self._io_names = []
-        self._base_names = []
-        self._factors_to_base = []
-        self._factors_to_field = []
+        self.io_names = []
+        self.base_names = []
+        self.factors_to_base = []
+        self.factors_to_field = []
 
         for key, value in self._field_maps.items():
-            self._io_names.append(key)
-            self._base_names.append(value.field.names[value.position])
-            self._factors_to_base.append(value.base_factor)
-            self._factors_to_field.append(1 / value.base_factor)
-
-    @property
-    def io_names(self):
-        return self._io_names
-
-    @property
-    def base_names(self):
-        return self._base_names
-
-    @property
-    def factors_to_base(self) -> List[float]:
-        return self._factors_to_base
-
-    @property
-    def factors_to_field(self) -> List[float]:
-        return self._factors_to_field
+            self.io_names.append(key)
+            self.base_names.append(value.field.names[value.position])
+            self.factors_to_base.append(value.base_factor)
+            self.factors_to_field.append(1 / value.base_factor)
 
     def subset(self, less_base_names):
         return FieldIOInfo({x: self._field_maps[x] for x in less_base_names if x in self._field_maps})
```

### Comparing `flightdata-0.1.0/flightdata.egg-info/PKG-INFO` & `flightdata-0.1.1/flightdata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Module for handling UAV flight log data
 Home-page: https://github.com/PyFlightCoach/FlightData
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightdata-0.1.0/flightdata.egg-info/SOURCES.txt` & `flightdata-0.1.1/flightdata.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,11 +9,13 @@
 flightdata.egg-info/SOURCES.txt
 flightdata.egg-info/dependency_links.txt
 flightdata.egg-info/requires.txt
 flightdata.egg-info/top_level.txt
 flightdata/config/__init__.py
 flightdata/config/ardupilot.py
 flightdata/field_mapping/__init__.py
+flightdata/field_mapping/ardupilot.py
 flightdata/field_mapping/ardupilot_ekfv2.py
 flightdata/field_mapping/ardupilot_ekfv3.py
 flightdata/field_mapping/fc_json_2_1.py
+test/test_ardupilot.py
 test/test_data.py
```

### Comparing `flightdata-0.1.0/setup.py` & `flightdata-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.1.0/test/test_data.py` & `flightdata-0.1.1/test/test_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         self.assertEqual(len(vals1), 1)
     
     def test_to_from_csv(self):
         flight = Flight.from_log('test/ekfv3_test.BIN')
         flight.to_csv('temp.csv')
         flight2 = Flight.from_csv('temp.csv')
         os.remove('temp.csv')
-        self.assertAlmostEqual(flight2.duration, flight.duration)
-        self.assertAlmostEqual(flight2.zero_time, flight.zero_time)
+        self.assertAlmostEqual(flight2.duration, flight.duration, 4)
+        self.assertAlmostEqual(flight2.zero_time, flight.zero_time, 4)
    
     def test_missing_arsp(self):
         flight = Flight.from_log('test/00000150.BIN')
         self.assertGreater(flight.duration, 500)
 
     def test_quaternions(self):
         flight = Flight.from_log('test/00000150.BIN')
@@ -106,7 +106,13 @@
 
 
     def test_flying_only(self):
         flt = self.flight.flying_only()
         assert isinstance(flt, Flight)
         assert flt.duration < self.flight.duration
         assert flt[0].position_z < -5
+
+
+
+def test_timestamp():
+    fl = Flight.from_log("test/test_inputs/00000129.BIN")
+    assert fl.data.time_flight.iloc[0] > 1e6
```

