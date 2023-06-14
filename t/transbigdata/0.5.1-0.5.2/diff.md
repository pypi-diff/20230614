# Comparing `tmp/transbigdata-0.5.1.tar.gz` & `tmp/transbigdata-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transbigdata-0.5.1.tar", last modified: Tue Jun  6 08:32:09 2023, max compression
+gzip compressed data, was "transbigdata-0.5.2.tar", last modified: Wed Jun 14 10:33:44 2023, max compression
```

## Comparing `transbigdata-0.5.1.tar` & `transbigdata-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.661062 transbigdata-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-06 08:31:56.000000 transbigdata-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 08:31:56.000000 transbigdata-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-06 08:32:09.661062 transbigdata-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-06-06 08:31:56.000000 transbigdata-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:32:09.661062 transbigdata-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 08:31:57.000000 transbigdata-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.653062 transbigdata-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.657062 transbigdata-0.5.1/src/transbigdata/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/bikedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/busgps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/gisprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    49157 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/mobilephonedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/odprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/plotmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/taxigps.py
--rw-r--r--   0 runner    (1001) docker     (123)    31846 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/traj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25663 2023-06-06 08:31:57.000000 transbigdata-0.5.1/src/transbigdata/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:09.657062 transbigdata-0.5.1/transbigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 08:32:09.000000 transbigdata-0.5.1/transbigdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:44.188849 transbigdata-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-14 10:33:32.000000 transbigdata-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 10:33:32.000000 transbigdata-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-14 10:33:44.184849 transbigdata-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-06-14 10:33:32.000000 transbigdata-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:33:44.188849 transbigdata-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-14 10:33:32.000000 transbigdata-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:44.184849 transbigdata-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:44.184849 transbigdata-0.5.2/src/transbigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/bikedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/busgps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/gisprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49157 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/mobilephonedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/odprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/plotmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/taxigps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34471 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/traj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25663 2023-06-14 10:33:32.000000 transbigdata-0.5.2/src/transbigdata/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:44.184849 transbigdata-0.5.2/transbigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-14 10:33:44.000000 transbigdata-0.5.2/transbigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 10:33:44.000000 transbigdata-0.5.2/transbigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:33:44.000000 transbigdata-0.5.2/transbigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 10:33:44.000000 transbigdata-0.5.2/transbigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 10:33:44.000000 transbigdata-0.5.2/transbigdata.egg-info/top_level.txt
```

### Comparing `transbigdata-0.5.1/LICENSE` & `transbigdata-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/PKG-INFO` & `transbigdata-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transbigdata
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python package developed for transportation spatio-temporal big data processing and analysis.
 Home-page: https://github.com/ni1o1/transbigdata
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/transbigdata/issues
 Classifier: Operating System :: OS Independent
```

### Comparing `transbigdata-0.5.1/README.md` & `transbigdata-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/setup.py` & `transbigdata-0.5.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="transbigdata",
-    version="0.5.1",
+    version="0.5.2",
     author="Qing Yu",
     author_email="qingyu0815@foxmail.com",
     description="A Python package developed for transportation spatio-temporal big data processing and analysis.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/ni1o1/transbigdata",
```

### Comparing `transbigdata-0.5.1/src/transbigdata/__init__.py` & `transbigdata-0.5.2/src/transbigdata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 __author__ = 'Qing Yu <yuq@sustech.edu.cn>'
 
 # module level doc-string
 __doc__ = """
 TransBigData - A Python package develop for transportation spatio-temporal big
 data processing, analysis and visualization.
 =====================================================================
@@ -154,14 +154,15 @@
     traj_slice,
     traj_smooth,
     traj_segment,
     traj_densify,
     traj_sparsify,
     traj_stay_move,
     traj_to_linestring,
+    traj_length
 )
 
 from transbigdata.utils import (
     dumpjson
 )
 
 from transbigdata.quality import (
```

### Comparing `transbigdata-0.5.1/src/transbigdata/activity.py` & `transbigdata-0.5.2/src/transbigdata/activity.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/bikedata.py` & `transbigdata-0.5.2/src/transbigdata/bikedata.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/busgps.py` & `transbigdata-0.5.2/src/transbigdata/busgps.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/coordinates.py` & `transbigdata-0.5.2/src/transbigdata/coordinates.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/crawler.py` & `transbigdata-0.5.2/src/transbigdata/crawler.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/gisprocess.py` & `transbigdata-0.5.2/src/transbigdata/gisprocess.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/grids.py` & `transbigdata-0.5.2/src/transbigdata/grids.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/metro.py` & `transbigdata-0.5.2/src/transbigdata/metro.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/mobilephonedata.py` & `transbigdata-0.5.2/src/transbigdata/mobilephonedata.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/odprocess.py` & `transbigdata-0.5.2/src/transbigdata/odprocess.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/plotmap.py` & `transbigdata-0.5.2/src/transbigdata/plotmap.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/preprocess.py` & `transbigdata-0.5.2/src/transbigdata/preprocess.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/quality.py` & `transbigdata-0.5.2/src/transbigdata/quality.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/taxigps.py` & `transbigdata-0.5.2/src/transbigdata/taxigps.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/traj.py` & `transbigdata-0.5.2/src/transbigdata/traj.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,59 @@
 import osmnx as ox
 from .coordinates import getdistance
 from .gisprocess import ckdnearest_line
 import numpy as np
 from pykalman import KalmanFilter
 from pyproj import CRS
 
+def traj_length(move_points,col = [ 'lon', 'lat','moveid'],method = 'Haversine'):
+    '''
+    Calculate Trajectory Length.
+    Input the trajectory point data and calculate the length of each trajectory in meters.
+
+    Parameters
+    ----------
+    move_points: DataFrame
+        Trajectory point data, which includes trajectory id, longitude, latitude, etc. Different trajectories are distinguished by trajectory id, and trajectory points are arranged in time order.
+    col: list
+        Column names of the trajectory point data, in the order of [longitude, latitude, trajectory id]
+    method: str
+        The method of calculating the trajectory length, optional 'Haversine' or 'Project', default is 'Haversine' using the haversine formula to calculate spherical distance, 'Project' transforms the data into a projected coordinate system to calculate plane distance.
+
+    Returns
+    -------
+    move_trajs: DataFrame
+        Trajectory length data, including two columns of trajectory id and trajectory length, the unit is meters.
+    '''
+    [lon, lat,moveid] = col
+    if method == 'Project':
+        move_trajs = traj_to_linestring(move_points, col=[lon, lat,moveid])
+        # 将轨迹转换为投影坐标系，以便计算轨迹长度
+        # epsg代号2414为北京54坐标系下经度在112.5度到115.5度范围内的投影坐标系
+        move_trajs.crs = 'epsg:4326'
+        epsg = CRS.from_proj4("+proj=aeqd +lat_0="+str(move_points[lat].mean())+" +lon_0="+str(move_points[lon].mean())+" +datum=WGS84")
+        move_trajs_proj = move_trajs.to_crs(epsg)
+        # 计算每一条轨迹的长度
+        move_trajs['length'] = move_trajs_proj.length
+    elif method == 'Haversine':
+        # 对每一轨迹段计算长度
+        move_trajs = move_points.copy()
+        moveids = move_points[moveid].drop_duplicates()
+        # 将下一行的坐标平移至同一行，方便进行列运算
+        move_trajs[lon+'_next'] = move_trajs[lon].shift(-1)
+        move_trajs[lat+'_next'] = move_trajs[lat].shift(-1)
+        # 还需确保计算的是同一条轨迹的坐标点
+        move_trajs[moveid+'_next'] = move_trajs[moveid].shift(-1)
+        move_trajs = move_trajs[move_trajs[moveid]==move_trajs[moveid+'_next']]
+        # 计算每两点之间的长度，并统计整条轨迹的长度
+        move_trajs['length'] = getdistance(move_trajs[lon],move_trajs[lat],move_trajs[lon+'_next'],move_trajs[lat+'_next'])
+        move_trajs = move_trajs.groupby(moveid)['length'].sum().reset_index()
+        move_trajs = pd.merge(moveids,move_trajs,on = moveid,how = 'left').fillna(0)
+    return move_trajs
+
 def traj_smooth(data,col = ['id','time','lon', 'lat'],proj = False,process_noise_std = 0.5, measurement_noise_std = 1):
     '''
     Smooth Trajectory Using Kalman Filter.
 
     Parameters
     ----------
     data: DataFrame
```

### Comparing `transbigdata-0.5.1/src/transbigdata/utils.py` & `transbigdata-0.5.2/src/transbigdata/utils.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/src/transbigdata/visualization.py` & `transbigdata-0.5.2/src/transbigdata/visualization.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.5.1/transbigdata.egg-info/PKG-INFO` & `transbigdata-0.5.2/transbigdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transbigdata
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python package developed for transportation spatio-temporal big data processing and analysis.
 Home-page: https://github.com/ni1o1/transbigdata
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/transbigdata/issues
 Classifier: Operating System :: OS Independent
```

### Comparing `transbigdata-0.5.1/transbigdata.egg-info/SOURCES.txt` & `transbigdata-0.5.2/transbigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

