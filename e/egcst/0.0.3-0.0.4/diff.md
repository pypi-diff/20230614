# Comparing `tmp/egcst-0.0.3.tar.gz` & `tmp/egcst-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egcst-0.0.3.tar", last modified: Wed Jun 14 00:46:51 2023, max compression
+gzip compressed data, was "egcst-0.0.4.tar", last modified: Wed Jun 14 19:09:51 2023, max compression
```

## Comparing `egcst-0.0.3.tar` & `egcst-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:46:51.212230 egcst-0.0.3/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:46:51.212406 egcst-0.0.3/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)     2319 2023-06-14 00:46:10.000000 egcst-0.0.3/README.md
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:46:51.207759 egcst-0.0.3/egcst/
--rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.3/egcst/__init__.py
--rw-r--r--   0 sasha      (502) staff       (20)    10467 2023-06-13 23:11:39.000000 egcst-0.0.3/egcst/core.py
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:46:51.211834 egcst-0.0.3/egcst.egg-info/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-14 00:46:51.000000 egcst-0.0.3/egcst.egg-info/SOURCES.txt
--rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/dependency_links.txt
--rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/requires.txt
--rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/top_level.txt
--rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-14 00:46:51.213116 egcst-0.0.3/setup.cfg
--rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-14 00:45:11.000000 egcst-0.0.3/setup.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 19:09:51.839719 egcst-0.0.4/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 19:09:51.839994 egcst-0.0.4/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)     2230 2023-06-14 19:06:51.000000 egcst-0.0.4/README.md
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 19:09:51.834608 egcst-0.0.4/egcst/
+-rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.4/egcst/__init__.py
+-rw-r--r--   0 sasha      (502) staff       (20)    12442 2023-06-14 18:59:37.000000 egcst-0.0.4/egcst/core.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 19:09:51.839026 egcst-0.0.4/egcst.egg-info/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/requires.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-14 19:09:51.841619 egcst-0.0.4/setup.cfg
+-rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-14 19:00:13.000000 egcst-0.0.4/setup.py
```

### Comparing `egcst-0.0.3/README.md` & `egcst-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Python package _egcst_
 This Python package helps to perform triangulation for engineering geological cross-sections.
 
 # Installation
 This Python package is uploaded to the PyPI repository and therefore can be installed with `pip install egcst` command line instruction and updated (this is critical at this early stage of development) with `pip install egcst --upgrade`.
 
 # Polygon data format to feed
-The only class `CrossSection()` of this package, when initiated, is expected to read an input text file that contains the polygons with unique geological characteristics in the following format: each polygon is placed on an individual line in the file with vertices' coordinates following one another separated with tabulation characters with x and y coordinates separated with a comma. The expected default name for this input file is `input.txt`. The object of the class `CrossSection()`, when initiated, can accept the optional argument `input_file_name` with another name for this input file. Another optional argument is `min_step`, which determines the approximate step for the triangulation grid. Its default value is 0.04, which is too small for certain input units and may dramatically slow the triangulation.
+The only class `CrossSection()` of this package, when initiated, is expected to read an input text file that contains the polygons with unique geological characteristics in the following format: each polygon is placed on an individual line in the file with vertices' coordinates following one another separated with tabulation characters with x and y coordinates separated with a comma. The expected default name for this input file is `input.txt`. The object of the class `CrossSection()`, when initiated, can accept the optional argument `input_file_name` with another name for this input file. Another optional argument is `min_step`, which determines the approximate step for the triangulation grid. Its default value is 0.5.
 
 # Dependencies
 This package depends on the standard Python module `sys` as well as the non-standard Python modules `numpy`, `matplotlib`, `shapely`, `ground`, and `sect`.
 
 # How to use it
 Very easy. The package has only one class `CrossSection()`, which is initiated with the input text file containing the coordinates for the polygons of the  engineering geological cross-section. This class has only 5 'public' methods: `.draw_blank()`, `.triangulate()`, `.save_triangles()`, `.draw_triangles()`, `.do_everything()`, which (except for the last one) are expected to be called in this order (and never repeated for the same object).<br/> The illustration of how to use this package can be found in the attached file [egcst_illustration.ipybn](https://github.com/yuryatin/egcst/blob/main/egcst_illustration.ipynb) .<br/> Briefly this can be expressed like this:
 ```python
```

### Comparing `egcst-0.0.3/egcst/core.py` & `egcst-0.0.4/egcst/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 import matplotlib.colors as mcolors
 from shapely.geometry import Polygon as sly_Polygon
 from shapely.geometry import Point as sly_Point
 
 from ground.base import get_context
 from sect.triangulation import Triangulation
 context = get_context()
-Contour, Point, sect_Polygon = context.contour_cls, context.point_cls, context.polygon_cls
+sect_Contour, sect_Point, sect_Polygon = context.contour_cls, context.point_cls, context.polygon_cls
 
 
 class CrossSection():
     def __init__(self,
-                 min_step=0.04,
+                 min_step=0.5,
                  input_file_name='input.txt'):
+        self.triangulated = False
+        self.triangles_saved = False
         self.min_step = min_step
         self.input_file_name = input_file_name
         with open(self.input_file_name) as f:
             self.data = f.readlines()
 
         self.polygons = list()
         for p_n, row in enumerate(self.data):
@@ -125,15 +127,15 @@
         for point in self.new_points:
             p_attribution = list()
             for i_p, p in enumerate(self.polygons):
                 if sly_Polygon(p).contains(sly_Point(point)):
                     p_attribution.append(i_p)
             try:
                 self.new_point_attribution[min(p_attribution, key=self.nesting_dict.get)].append(
-                    Point(point[0], point[1]))
+                    sect_Point(point[0], point[1]))
             except:
                 pass
 
     def draw_blank(self, fig_blank_file_name='output_blank.png'):
         self.color_indeces = list(range(len(mcolors.CSS4_COLORS)))
         fig, ax = plt.subplots()
         for i_c, p in enumerate(self.polygons):
@@ -143,27 +145,32 @@
         ax.scatter(self.new_x, self.new_y, s=3, c='g')
         ax.axis('equal')
         ax.legend(loc='lower center', ncol=self.n_polygons)
         dpi = fig.get_dpi()
         plt.savefig(fig_blank_file_name, dpi=dpi*3)
 
     def triangulate(self):
+        if self.triangulated:
+            print("You may not call the .triangulate() on this instance of the class CrossSection more than once. You have already called it once. If you intend to repeat a triangulation for this cross-section, you need to create a new instance of the class CrossSection and call .triangulate() on it.")
+            return
+        
+        self.triangulated = True
         for i_p in range(self.n_polygons):
             if 1 in self.nesting_matrix[i_p, :] and -1 in self.nesting_matrix[i_p, :]:
                 for j_p in np.where(self.nesting_matrix[i_p, :] == 1)[0]:
                     for k_p in np.where(self.nesting_matrix[i_p, :] == -1)[0]:
                         self.nesting_matrix[j_p,
                                             k_p] = self.nesting_matrix[k_p, j_p] = 0
 
         self.c_list = list()
         for p in self.polygons:
             p_list = list()
             for point in p:
-                p_list.append(Point(point[0], point[1]))
-            self.c_list.append(Contour(p_list[:-1]))
+                p_list.append(sect_Point(point[0], point[1]))
+            self.c_list.append(sect_Contour(p_list[:-1]))
 
         self.p_list = list()
         for i_c, c in enumerate(self.c_list):
             nested = list()
             for k_p in np.where(self.nesting_matrix[i_c, :] == 1)[0]:
                 nested.append(self.c_list[k_p])
             self.p_list.append(sect_Polygon(c, nested))
@@ -177,16 +184,27 @@
             print("The polygon #%2d has been triangulated" % (i_p + 1))
             stdout.flush()
 
     def save_triangles(self,
                        output_file_name_triangles='triangles.txt',
                        output_file_name_points='points.txt',
                        output_file_name='output.txt'):
-        self.the_all_points = np.concatenate(
-            (self.all_points, self.new_points))
+        if self.triangles_saved:
+            print("You may not call the .save_triangles() on this instance of the class CrossSection more than once. You have already called it once. If you intend to save triangles again for this cross-section after triangulation, you need to create a new instance of the class CrossSection, to call .triangulate() to triangulate it and then to call .save_triangles() on it.")
+            return
+        
+        if not self.triangulated:
+            print("You are trying to save triangles while you have not yet triangulated the cross-section for this instance of the classCrossSection. So you need to first call .triangulate() and then to call .save_triangles() to save the triangles you will have gotten.")
+            return
+        
+        self.triangles_saved = True
+        if self.new_points:
+            self.the_all_points = np.concatenate((self.all_points, self.new_points))
+        else:
+            self.the_all_points = np.copy(self.all_points)
         self.new_array = list()
         count = -1
         with open(output_file_name, 'w') as f:
             for i_z, z in self.tri_sect.items():
                 for _tri in z:
                     count += 1
                     f.write("%d\t" % (count + 1))
@@ -206,14 +224,22 @@
 
         with open(output_file_name_triangles, 'w') as f:
             for i_tri, _tri in enumerate(self.new_array):
                 f.write("%d\t%d\t%d\t%d\n" %
                         (i_tri + 1, _tri[0] + 1, _tri[1] + 1, _tri[2] + 1))
 
     def draw_triangles(self, fig_triangles_file_name='output_triangles.png'):
+        if not self.triangulated:
+            print("You are trying to draw triangles while you have not yet triangulated the cross-section for this instance of the classCrossSection nor saved those trianlges. So you need to first call .triangulate(), then to call .save_triangles(), and then to call this method.")
+            return
+        
+        if not self.triangles_saved:
+            print("You may not call the .draw_triangles() on this instance of the class CrossSection before you saved the triangles by calling the .save_triangles() method.")
+            return
+        
         fig, ax = plt.subplots()
         for i_c, p in enumerate(self.polygons):
             ax.add_patch(Polygon(np.array(p), alpha=0.2, facecolor=list(
                 mcolors.CSS4_COLORS.values())[self.color_indeces[i_c+12]], label="%2d" % (i_c+1)))
         ax.scatter(self.all_x, self.all_y, s=20, c='r')
         plt.triplot(
             self.the_all_points[:, 0], self.the_all_points[:, 1], self.new_array, linewidth=0.7)
```

### Comparing `egcst-0.0.3/setup.py` & `egcst-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
     name = 'egcst',
     packages = ['egcst'],
-    version = '0.0.3',
+    version = '0.0.4',
     license = 'MIT',
     description = 'This package performs triangulation for engineering geological cross-sections',
     url = 'https://github.com/yuryatin/egcst',
-    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.3.tar.gz',
+    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.4.tar.gz',
     keywords = ['engineering', 'geological', 'cross', 'sections', 'mapping', 'triangulation', 'delaunay'],
     classifiers = [],
     install_requires = ['numpy', 'matplotlib', 'shapely', 'ground', 'sect']
 )
```

