# Comparing `tmp/boundaryscheme-2.1.tar.gz` & `tmp/boundaryscheme-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boundaryscheme-2.1.tar", last modified: Mon Jun  5 13:40:12 2023, max compression
+gzip compressed data, was "dist/boundaryscheme-2.2.tar", last modified: Wed Jun 14 14:39:06 2023, max compression
```

## Comparing `boundaryscheme-2.1.tar` & `boundaryscheme-2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1833 2023-06-05 13:40:12.000000 boundaryscheme-2.1/PKG-INFO
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/tests/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-2.1/tests/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       61 2023-06-05 07:51:32.000000 boundaryscheme-2.1/tests/test_import.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1833 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/PKG-INFO
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/SOURCES.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/requires.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/top_level.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/dependency_links.txt
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     1221 2023-06-05 13:37:51.000000 boundaryscheme-2.1/README.md
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-05 13:29:30.000000 boundaryscheme-2.1/setup.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/examples/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-2.1/examples/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1995 2023-06-04 15:20:10.000000 boundaryscheme-2.1/examples/draw_detKLcurve.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1401 2023-05-31 17:06:49.000000 boundaryscheme-2.1/examples/draw_nbrzerosdetKL.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      925 2023-05-31 17:06:37.000000 boundaryscheme-2.1/examples/draw_symbol.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme/
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-2.1/boundaryscheme/boundaries.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-06-05 13:39:33.000000 boundaryscheme-2.1/boundaryscheme/__init__.py
--rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-2.1/boundaryscheme/utils.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    20955 2023-06-05 07:40:10.000000 boundaryscheme-2.1/boundaryscheme/schemes.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-2.1/boundaryscheme/complex_winding_number.py
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    23173 2023-06-04 15:21:40.000000 boundaryscheme-2.1/boundaryscheme/pyplot.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-05 13:40:12.000000 boundaryscheme-2.1/setup.cfg
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4480 2023-06-14 14:39:06.000000 boundaryscheme-2.2/PKG-INFO
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/tests/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-2.2/tests/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       62 2023-06-14 13:22:07.000000 boundaryscheme-2.2/tests/test_import.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4480 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/PKG-INFO
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/SOURCES.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/requires.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/top_level.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/dependency_links.txt
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     3380 2023-06-14 13:18:38.000000 boundaryscheme-2.2/README.md
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-14 14:38:10.000000 boundaryscheme-2.2/setup.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/examples/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-2.2/examples/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2049 2023-06-14 13:22:07.000000 boundaryscheme-2.2/examples/draw_detKLcurve.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1385 2023-06-14 13:22:07.000000 boundaryscheme-2.2/examples/draw_nbrzerosdetKL.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      909 2023-06-14 13:22:07.000000 boundaryscheme-2.2/examples/draw_symbol.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme/
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-2.2/boundaryscheme/boundaries.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-06-14 14:38:15.000000 boundaryscheme-2.2/boundaryscheme/__init__.py
+-rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-2.2/boundaryscheme/utils.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    19750 2023-06-14 13:22:07.000000 boundaryscheme-2.2/boundaryscheme/schemes.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-2.2/boundaryscheme/complex_winding_number.py
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    22644 2023-06-14 13:22:07.000000 boundaryscheme-2.2/boundaryscheme/pyplot.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-14 14:39:06.000000 boundaryscheme-2.2/setup.cfg
```

### Comparing `boundaryscheme-2.1/boundaryscheme.egg-info/SOURCES.txt` & `boundaryscheme-2.2/boundaryscheme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.1/setup.py` & `boundaryscheme-2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 def read_from(filename):
     with open(filename) as fp:
         return fp.read()
 
 
 def get_version():
-    data = read_from(rel_file('boundaryscheme', '__init__.py'))
+    data = read_from(rel_file("boundaryscheme", "__init__.py"))
     return re.search(r"__version__ = '([^']+)'", data).group(1)
 
 
 def get_requirements():
-    data = read_from(rel_file('requirements.txt'))
+    data = read_from(rel_file("requirements.txt"))
     lines = map(lambda s: s.strip(), data.splitlines())
     return list(filter(None, lines))
 
 
 setup(
-    name='boundaryscheme',
+    name="boundaryscheme",
     version=get_version(),
     description="This library implements Kreiss-Lopatinskii determinant for numerical scheme with boundary",
-    long_description=read_from('README.md'),
-    long_description_content_type='text/markdown',
-    author='Pierre Le Barbenchon',
+    long_description=read_from("README.md"),
+    long_description_content_type="text/markdown",
+    author="Pierre Le Barbenchon",
     packages=find_packages(),
     install_requires=get_requirements(),
 )
```

### Comparing `boundaryscheme-2.1/examples/draw_detKLcurve.py` & `boundaryscheme-2.2/examples/draw_detKLcurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 
 if __name__ == "__main__":
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda = 1.4"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = 1.4)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda in [1.4, 0.7, 1] with sigma = 0.4"""
-    bsplt.detKLplot(BeamWarming, SILW(2, 3), lamb=np.array([1.4, 0.7, 1]), sigma=0)
+    # bsplt.detKLplot(BeamWarming, SILW(2, 3), lamb=np.array([1.4, 0.7, 1]), sigma=0)
+
+    bsplt.detKLplot(LaxWendroff(5), SILW(2, 3), lambdacursor=True)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda = 1 with sigma in [-0.2, 0, 0.1,0.4]"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = 1, sigma = np.array([-0.2, 0, 0.1,0.4]))
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda in [1.4, 0.7] with sigma in [-0.2, 0, 0.4]"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = [1.4, 0.7], sigma = np.array([-0.2, 0, 0.4]))
 
@@ -32,9 +34,7 @@
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = 1.4, sigmacursor = True)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming with a cursor for lambda between 0 and the CFL condition"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lambdacursor = True)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming with a cursor for lambda between 0 and the CFL condition and a cursor for sigma between -0.5 and 0.5"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lambdacursor = True, sigmacursor = True)
-
-    plt.show()
```

### Comparing `boundaryscheme-2.1/examples/draw_nbrzerosdetKL.py` & `boundaryscheme-2.2/examples/draw_nbrzerosdetKL.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,9 +23,7 @@
     # bsplt.nbrzerosdetKL(BeamWarming,  SILW(2,3),lamb = np.array([1.4,1.7]), nparam = 150)
 
     """plot the number of zeros of Kreiss-Lopatinskii determinant of BeamWarming with several boundary conditions"""
     bsplt.nbrzerosdetKL(BeamWarming, [SILW(1, 3), SILW(2, 3), SILW(2, 4), SILW(3, 4), DDJ(3, 0), DDJ(3, 1)], nlambda=60)
 
     """plot the number of zeros of Kreiss-Lopatinskii determinant of BeamWarming with SILW(2,3) with respect to lambda and sigma"""
     # bsplt.nbrzerosdetKL(BeamWarming, SILW(2,3), sigma=True, nlambda=40, nsigma = 20)
-
-    plt.show()
```

### Comparing `boundaryscheme-2.1/examples/draw_symbol.py` & `boundaryscheme-2.2/examples/draw_symbol.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,7 @@
     # bsplt.symbolplot(BeamWarming, [0.7,1.4, 1.8], lambdacursor = True)
 
     """plot the BeamWarming symbol curve for lambda = 1.4"""
     # bsplt.symbolplot(BeamWarming, 1.4)
 
     """plot the BeamWarming symbol curves for lambda in [0.7, 1, 1.6]"""
     # bsplt.symbolplot(BeamWarming, np.array([0.7, 1, 1.6]))
-
-    plt.show()
```

### Comparing `boundaryscheme-2.1/boundaryscheme/boundaries.py` & `boundaryscheme-2.2/boundaryscheme/boundaries.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.1/boundaryscheme/utils.py` & `boundaryscheme-2.2/boundaryscheme/utils.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.1/boundaryscheme/schemes.py` & `boundaryscheme-2.2/boundaryscheme/schemes.py`

 * *Files 3% similar despite different names*

```diff
@@ -336,42 +336,14 @@
         super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
 
     def shortname(self):
         """Name method"""
         return "Upwind"
 
 
-class LaxWendroff(Scheme):
-    """This is a class to represent the Lax-Wendroff scheme (of order 2).
-
-    :param lamb: The Courant number, i.e  a.dt/dx where "a" is the velocity, "dt" the time discretization and "dx" the space discretization
-    :type lamb: float
-    :param boundary: Boundary condition, defaults to Dirichlet()
-    :type boundary: class:`Boundary`, optional
-    :param sigma: Gap between the mesh and the boundary condition, defaults to 0
-    :type sigma: float, optional
-    """
-
-    def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
-        """Constructor method"""
-        self.sigma = sigma
-        self.lamb = lamb
-        coeff1 = -(lamb - lamb**2) / 2
-        coeff2 = 1 - lamb**2
-        coeff3 = (lamb**2 + lamb) / 2
-        self.inter = np.array([coeff3, coeff2, coeff1])
-        self.center = 1
-        self.CFL = 1
-        super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
-
-    def shortname(self):
-        """Name method"""
-        return "LaxWendroff"
-
-
 class LaxFriedrichs(Scheme):
     """This is a class to represent the Lax-Friedrichs scheme.
 
     :param lamb: The Courant number, i.e  a.dt/dx where "a" is the velocity, "dt" the time discretization and "dx" the space discretization
     :type lamb: float
     :param boundary: Boundary condition, defaults to Dirichlet()
     :type boundary: class:`Boundary`, optional
@@ -477,48 +449,46 @@
         super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
 
     def shortname(self):
         """Name method"""
         return "Dissipative"
 
 
-class LW(Scheme):
-    """This is a class to represent a Lax-Wendroff scheme of any order.
-
-    :param lamb: The Courant number, i.e  a.dt/dx where "a" is the velocity, "dt" the time discretization and "dx" the space discretization
-    :type lamb: float
-    :param boundary: Boundary condition, defaults to Dirichlet()
-    :type boundary: class:`Boundary`, optional
-    :param sigma: Gap between the mesh and the boundary condition, defaults to 0
-    :type sigma: float, optional
+def LaxWendroff(order=2):
+    """
+    This is a function which create the class of LaxWendroff scheme at order 'order'
     :param order: Order of the Lax-Wendroff scheme, defaults to 2
     :type order: int, optional
     """
 
-    allordersschem = [None, None, Lwconstructor(2)]
+    class LW(Scheme):
+        """This is a class to represent a Lax-Wendroff scheme of any order.
 
-    def __init__(self, lamb, boundary=Dirichlet(), sigma=0, order=2, **kwargs):
-        """Constructor method"""
-        self.sigma = sigma
-        self.order = order
-        self.lamb = lamb
-        n = len(LW.allordersschem) - 1
-        if order > n:
-            for i in range(order - n):
-                LW.allordersschem.append(None)
-            LW.allordersschem[order] = Lwconstructor(order)
-        if LW.allordersschem[order] == None:
-            LW.allordersschem[order] = Lwconstructor(order)
-        self.inter, self.center = LW.allordersschem[order](lamb)
-        self.CFL = 1
-        super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
+        :param lamb: The Courant number, i.e  a.dt/dx where "a" is the velocity, "dt" the time discretization and "dx" the space discretization
+        :type lamb: float
+        :param boundary: Boundary condition, defaults to Dirichlet()
+        :type boundary: class:`Boundary`, optional
+        :param sigma: Gap between the mesh and the boundary condition, defaults to 0
+        :type sigma: float, optional
+        """
+
+        def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
+            """Constructor method"""
+            self.sigma = sigma
+            self.order = order
+            self.lamb = lamb
+            self.inter, self.center = Lwconstructor(order)(lamb)
+            self.CFL = 1
+            super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
+
+        def shortname(self):
+            """Name method"""
+            return f"Lax Wendroff {self.order}"
 
-    def shortname(self):
-        """Name method"""
-        return f"Lax Wendroff {self.order}"
+    return LW
 
 
 # class LeapFrog(Scheme):
 #     raise NotImplementedError('')
 
 
 # class CrankNicholson(Scheme):
```

### Comparing `boundaryscheme-2.1/boundaryscheme/complex_winding_number.py` & `boundaryscheme-2.2/boundaryscheme/complex_winding_number.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.1/boundaryscheme/pyplot.py` & `boundaryscheme-2.2/boundaryscheme/pyplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     """
     ax = plt.subplot()
     Param, Det = schem.detKL(n_param, parametrization_bool)
     ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2)
     ax.axvline(x=0, color="0.5")
     ax.axhline(y=0, color="0.5")
     ax.axis("equal")
-    return ax
+    plt.show()
 
 
-def detKLplot(schem, left_bound=Dirichlet(), lamb=None, sigma=0, lambdacursor=False, sigmacursor=False, nparam=300, parametrization_bool=True, order=2, fig_size=(6, 4)):
+def detKLplot(schem, left_bound=Dirichlet(), lamb=None, sigma=0, lambdacursor=False, sigmacursor=False, nparam=300, parametrization_bool=True, fig_size=(6, 4)):
     """Computes the Kreiss-Lopatinskii determinant curve for different lambdas and different sigmas or with cursor(s)
 
     :param schem: Scheme depending on a parameter lambda
     :type schem: class:`Scheme`
     :param left_bound: Left boundary of the class Boundary, defaults to Dirichlet()
     :type left_bound: class:`Boundary`, optional
     :param lamb: A value lambda or a numpy.ndarray of several values of lambda (lambda is the Courant number a.dt/dx), defaults to None
@@ -52,16 +52,14 @@
     :type lambdacursor: bool, optional
     :param sigmacursor: Boolean to indicate the use of a cursor for sigma's moving among the sigma values, defaults to False
     :type sigmacursor: bool, optional
     :param n_param: Size of the discretization of the unit circle, defaults to 300
     :type n_param: int, optional
     :param parametrization_bool: True to have a refinment close to the origin, False to have a uniform discretization of the unit circle, defaults to True
     :type parametrization_bool: bool, optional
-    :param order: Order of the scheme (for Lax-Wendroff scheme), defaults to 2
-    :type order: int, optional
     :param fig_size: Size of the figure, defaults to (6,4)
     :type fig_size: (int,int), optional
     :return: the Kreiss-Lopatinskii curve for the scheme
     :rtype: plot object
     """
     if lamb is None:
         lamb = np.array([schem(1).CFL])
@@ -71,38 +69,38 @@
         sigma = np.array([sigma], dtype=float)
     if sigmacursor == False:
         if lambdacursor == False:
             if len(sigma) == 1:
                 lamb = np.sort(lamb)
                 fig, ax = plt.subplots(figsize=fig_size)
                 for l in lamb:
-                    S = schem(l, left_bound, order=order, sigma=sigma[0])
+                    S = schem(l, left_bound, sigma=sigma[0])
                     Param, Det = S.detKL(nparam, parametrization_bool)
                     ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, label=f"$\lambda$ = " + str(l))
                 ax.axvline(x=0, color="0.5")
                 ax.axhline(y=0, color="0.5")
                 ax.legend(loc="best")
                 plt.title("Symbol of " + S.name(boundary_bool=True, sigma_bool=True, lambda_bool=False))
             elif len(lamb) == 1:
                 sigma = np.sort(sigma)
                 fig, ax = plt.subplots(figsize=fig_size)
                 for sig in sigma:
-                    S = schem(lamb[0], left_bound, order=order, sigma=sig)
+                    S = schem(lamb[0], left_bound, sigma=sig)
                     Param, Det = S.detKL(nparam, parametrization_bool)
                     ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, label=f"$\sigma$ = " + str(sig))
                 ax.axvline(x=0, color="0.5")
                 ax.axhline(y=0, color="0.5")
                 ax.legend(loc="best")
                 plt.title("Symbol of " + S.name(boundary_bool=True, sigma_bool=False, lambda_bool=True))
             else:
                 sigma = np.sort(sigma)
                 fig, ax = plt.subplots(figsize=fig_size)
                 for l in lamb:
                     for sig in sigma:
-                        S = schem(l, left_bound, order=order, sigma=sig)
+                        S = schem(l, left_bound, sigma=sig)
                         Param, Det = S.detKL(nparam, parametrization_bool)
                         ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, label=f"$\lambda$ = " + str(l) + f"et $\sigma$ = " + str(sig))
                 ax.axvline(x=0, color="0.5")
                 ax.axhline(y=0, color="0.5")
                 ax.legend(loc="best")
                 plt.title("Symbol of " + S.name(boundary_bool=True, sigma_bool=False, lambda_bool=False))
         else:
@@ -113,21 +111,21 @@
                 lambmin = 0.001
             else:
                 lambmin = np.min(lamb)
 
             lamb0 = (lambmax + lambmin) / 2
             fig = plt.figure(1, figsize=(10, 8))
             plt.title("DKL curve of " + schem(1, left_bound, sigma=sigma[0]).name(boundary_bool=True, sigma_bool=True))
-            ax = fig.add_subplot(111)
+            ax = fig.add_subplot(111, label="cursor1")
             fig.subplots_adjust(left=0.25, bottom=0.25)
             ax.set_xlim(-3, 3)
             ax.axis("equal")
 
             def calc_det(l):
-                S = schem(l, left_bound, sigma=sigma[0], order=order)
+                S = schem(l, left_bound, sigma=sigma[0])
                 return S.detKL(nparam, parametrization_bool)[1]
 
             Det = calc_det(lamb0)
             [line] = ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, color="red")
             ax.axvline(x=0, color="0.5")
             ax.axhline(y=0, color="0.5")
             ax.axis("equal")
@@ -168,21 +166,21 @@
             sigmin = np.min(sigma)
         if lambdacursor == False:
             if len(lamb) > 1:
                 raise TypeError("With a sigma cursor, lambda has to be a single value")
             sigma0 = (sigmax + sigmin) / 2
             fig = plt.figure(1, figsize=(10, 8))
             plt.title("DKL curve of " + schem(lamb[0], left_bound).name(boundary_bool=True, lambda_bool=True))
-            ax = fig.add_subplot(111)
+            ax = fig.add_subplot(111, label="cursor2")
             fig.subplots_adjust(left=0.25, bottom=0.25)
             ax.set_xlim(-3, 3)
             ax.axis("equal")
 
             def calc_det(sig):
-                S = schem(lamb[0], left_bound, sigma=sig, order=order)
+                S = schem(lamb[0], left_bound, sigma=sig)
                 return S.detKL(nparam, parametrization_bool)[1]
 
             Det = calc_det(sigma0)
             [line] = ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, color="red")
             ax.axvline(x=0, color="0.5")
             ax.axhline(y=0, color="0.5")
             ax.axis("equal")
@@ -222,21 +220,21 @@
                 lambmin = np.min(lamb)
 
             sigma0 = (sigmax + sigmin) / 2
             lamb0 = (lambmin + lambmax) / 2
 
             fig = plt.figure(1, figsize=(10, 8))
             plt.title("DKL curve of " + schem(1, left_bound).name(boundary_bool=True))
-            ax = fig.add_subplot(111)
+            ax = fig.add_subplot(111, label="cursor3")
             fig.subplots_adjust(left=0.25, bottom=0.25)
             ax.set_xlim(-3, 3)
             ax.axis("equal")
 
             def calc_det(l, sigm):
-                S = schem(l, left_bound, sigma=sigm, order=order)
+                S = schem(l, left_bound, sigma=sigm)
                 return S.detKL(nparam, parametrization_bool)[1]
 
             Det = calc_det(lamb0, sigma0)
             [line] = ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, color="red")
             plt.axvline(x=0, color="0.5")
             plt.axhline(y=0, color="0.5")
 
@@ -272,39 +270,37 @@
 
             def reset(event):
                 lambda_slider.reset()
                 sigma_slider.reset()
 
             button.on_clicked(reset)
 
-    return ax
+    plt.show()
 
 
-def symbolplot(schem, lamb=None, order=2, lambdacursor=False, nparam=300, fig_size=(10, 8)):
+def symbolplot(schem, lamb=None, lambdacursor=False, nparam=300, fig_size=(10, 8)):
     """Computes the Kreiss-Lopatinskii determinant curve for different lambdas and different sigmas or with cursor(s)
 
     :param schem: Scheme depending on a parameter lambda
     :type schem: class:`Scheme`
     :param lamb: A value lambda or a numpy.ndarray of several values of lambda (lambda is the Courant number a.dt/dx), defaults to None
     :type lamb: int or float or list or numpy.ndarray, optional
-    :param order: Order of the scheme (for Lax-Wendroff scheme), defaults to 2
-    :type order: int, optional
     :param lambdacursor: Boolean to indicate the use of a cursor for lambda's moving among the lamb values, defaults to False
     :type lambdacursor: bool, optional
     :param nparam: Size of the discretization of the unit circle, defaults to 300
     :type nparam: int, optional
     :param fig_size: Size of the figure, defaults to (10,8)
     :type fig_size: (int,int), optional
     :return: the symbol curve of the scheme
     :rtype: plot object
     """
     if lambdacursor == False:
         fig, ax = plt.subplots(figsize=fig_size)
         if isinstance(lamb, (int, float)):
-            S = schem(lamb, order=order)
+            S = schem(lamb)
             X, Y = S.symbol(nparam)
             T = np.linspace(0, 7, 1000)
 
             plt.ylim(-1, 1)
             plt.xlim(-1, 1)
             ax.plot(np.cos(T), np.sin(T), "--", color="black", label="unit circle")
             ax.plot(X, Y, linewidth=2, label="symbol")
@@ -312,15 +308,15 @@
             ax.legend(loc="best")
             plt.title("Symbol of " + S.name(lambda_bool=True))
         else:
             assert (type(lamb) == np.ndarray and lamb.ndim == 1) or type(lamb) == list
             plt.ylim(-1, 1)
             plt.xlim(-1, 1)
             for l in lamb:
-                S = schem(l, order=order)
+                S = schem(l)
                 X, Y = S.symbol(nparam)
                 ax.plot(X, Y, linewidth=2, label=f"$\lambda = $ {l}")
             T = np.linspace(0, 7, 1000)
             ax.plot(np.cos(T), np.sin(T), "--", color="black", label="unit circle")
             ax.axis("equal")
             ax.legend(loc="upper left")
             plt.title("Symbol of " + S.name(lambda_bool=False))
@@ -328,29 +324,29 @@
     else:
         if lamb == None:
             lamb = schem(1).CFL
         if isinstance(lamb, (int, float)):
             lamb = np.array([lamb], dtype=float)
         fig = plt.figure(1, figsize=(10, 8))
         plt.title("Symbol of " + schem(1).name(lambda_bool=False))
-        ax = fig.add_subplot(111)
+        ax = fig.add_subplot(111, label="cursor4")
         fig.subplots_adjust(left=0.25, bottom=0.25)
         ax.set_xlim(-3, 3)
         ax.axis("equal")
 
         if len(lamb) == 1:
             lamb0 = lamb[0] / 2
         else:
             lamb0 = (np.min(lamb) + np.max(lamb)) / 2
 
         Param = np.linspace(0, 1, nparam)
         Param = np.cos(2 * pi * Param) + 1j * np.sin(2 * pi * Param)
         Theta = np.linspace(0, 2 * pi, 500)
 
-        X, Y = schem(lamb0, order=order).symbol(nparam)
+        X, Y = schem(lamb0).symbol(nparam)
         [line] = ax.plot(X, Y, linewidth=2, label="symbol")
         [cible] = ax.plot(np.cos(Theta), np.sin(Theta), "--", color="black", label="unit circle")
         ax.legend(loc="best")
         ax.set_xlim(-6, 2)
         ax.axis("equal")
         if len(lamb) == 1:
             minvalue = 0.0001
@@ -365,15 +361,15 @@
             label="lambda",
             valmin=minvalue,
             valmax=maxvalue,
             valinit=lamb0,
         )
 
         def update(val):
-            S = schem(lambda_slider.val, order=order)
+            S = schem(lambda_slider.val)
             X, Y = S.symbol(nparam)
             line.set_xdata(X)
             line.set_ydata(Y)
             fig.canvas.draw_idle()
 
         # register the update function with each slider
         lambda_slider.on_changed(update)
@@ -382,32 +378,30 @@
         resetax = plt.axes([0.8, 0.025, 0.1, 0.04])
         button = Button(resetax, "Reset", hovercolor="0.975")
 
         def reset(event):
             lambda_slider.reset()
 
         button.on_clicked(reset)
-    return ax
+    plt.show()
 
 
-def nbrzerosdetKL(schem, left_bound=Dirichlet(), lamb=None, sigma=0, order=2, nparam=100, nlambda=200, nsigma=30, parametrization_bool=True, fig_size=(15, 7), fontsize=18):
+def nbrzerosdetKL(schem, left_bound=Dirichlet(), lamb=None, sigma=0, nparam=100, nlambda=200, nsigma=30, parametrization_bool=True, fig_size=(15, 7), fontsize=18):
     """Computes the number of zeros of the Kreiss-Lopatinskii determinant for different boundary conditions, for different lambdas or/and for different sigmas
 
     .. seealso:: for more details and examples, see [Boutin, Le Barbenchon, Seguin, 2023 : Stability of finite difference schemes for the hyperbolic initial boundary value problem by winding number computations]
 
     :param schem: Scheme depending on a parameter lambda
     :type schem: class:`Scheme`
     :param left_bound: Left boundary of the class Boundary, defaults to Dirichlet()
     :type left_bound: class:`Boundary` or list of class:`Boundary`, optional
     :param lamb: A value lambda or a numpy.ndarray of several values of lambda (lambda is the Courant number a.dt/dx), defaults to None
     :type lamb: int or float or list or numpy.ndarray, optional
     :param sigma: Gap between the mesh and the boundary condition, defaults to 0
     :type sigma: int or float or list or numpy.ndarray, optional
-    :param order: Order of the scheme (for Lax-Wendroff scheme), defaults to 2
-    :type order: int, optional
     :param nparam: Size of the discretization of the unit circle for the Kreiss-Lopatinskii curve, defaults to 100
     :type nparam: int, optional
     :param nlambda: Size of the discretization of the lambda's, defaults to 200
     :type nlambda: int, optional
     :param nsigma: Size of the discretization of the sigma's, defaults to 30
     :type nsigma: int, optional
     :param parametrization_bool: True to have a refinment close to the origin, False to have a uniform discretization of the unit circle, defaults to True
@@ -433,27 +427,27 @@
         else:
             lambmin = min(lamb)
             lambmax = max(lamb)
     lambdas = np.linspace(lambmin, lambmax, nlambda)
     if isinstance(left_bound, list) or (isinstance(left_bound, np.ndarray) and left_bound.ndim == 1):
         n = len(left_bound)
         fig, axs = plt.subplots(nrows=n, ncols=1, figsize=fig_size)
-        axs[0].set_title(f"Number of zeros of KL determinant for {schem(1/2, order = order, sigma=sigma).name(sigma_bool=True)} with respect to $\lambda$")
+        axs[0].set_title(f"Number of zeros of KL determinant for {schem(1/2, sigma=sigma).name(sigma_bool=True)} with respect to $\lambda$")
         for i, bound in enumerate(left_bound):
             if i == n - 1:
                 axs[i].set_xlabel("$\lambda$")
             else:
                 axs[i].xaxis.set_ticklabels([])
             axs[i].set_xlim(lambmin, lambmax)
             axs[i].set_ylim(0, 1)
             axs[i].yaxis.set_ticks([])
             axs[i].set_ylabel(bound.name())
             WindingNumbers = []
             for l in lambdas:
-                S = schem(l, bound, sigma=sigma, order=order)
+                S = schem(l, bound, sigma=sigma)
                 Param, Det = S.detKL(nparam, parametrization_bool)
                 WindingNumbers.append(Indice(Det))
             separator = []
             value = []
             for j in range(len(WindingNumbers) - 1):
                 if WindingNumbers[j] != WindingNumbers[j + 1]:
                     separator.append((lambdas[j] + lambdas[j + 1]) / 2)
@@ -467,45 +461,43 @@
                         axs[i].plot([separator[j], separator[j]], [0, 1], color="black")
                         axs[i].text(separator[0] / 2, 0.5, value[j], horizontalalignment="center", verticalalignment="center", fontsize=fontsize)
                     elif j == len(separator):
                         axs[i].text((separator[j - 1] + lambmax) / 2, 0.5, value[j], horizontalalignment="center", verticalalignment="center", fontsize=fontsize)
                     else:
                         axs[i].plot([separator[j], separator[j]], [0, 1], color="black")
                         axs[i].text((separator[j] + separator[j - 1]) / 2, 0.5, value[j], horizontalalignment="center", verticalalignment="center", fontsize=fontsize)
-        return axs
+        plt.show()
     else:
         fig, ax = plt.subplots(figsize=fig_size)
         if isinstance(sigma, (int, float)) and not isinstance(sigma, bool):
             WindingNumbers = []
             for l in lambdas:
-                S = schem(l, left_bound, sigma=sigma, order=order)
+                S = schem(l, left_bound, sigma=sigma)
                 Param, Det = S.detKL(nparam, parametrization_bool)
                 WindingNumbers.append(Indice(Det))
             ax.plot(lambdas, S.r - np.array(WindingNumbers))
-            plt.title(
-                f"Number of zeros of KL determinant for {schem(1/2,left_bound, order = order, sigma=sigma).name(boundary_bool = True, sigma_bool = True, lambda_bool = False)} with respect to $\lambda$"
-            )
+            plt.title(f"Number of zeros of KL determinant for {schem(1/2,left_bound, sigma=sigma).name(boundary_bool = True, sigma_bool = True, lambda_bool = False)} with respect to $\lambda$")
         else:
             if sigma:
                 sigmin = -1 / 2
                 sigmax = 1 / 2
             else:
                 sigmax = max(sigma)
                 sigmin = min(sigma)
 
             sigmas = np.linspace(sigmin, sigmax, nsigma)
             WindingNumbers = np.zeros((nsigma, nlambda))
             for i, l in enumerate(lambdas):
                 for j, sig in enumerate(sigmas):
-                    S = schem(l, left_bound, sigma=sig, order=order)
+                    S = schem(l, left_bound, sigma=sig)
                     Param, Det = S.detKL(nparam, parametrization_bool)
                     WindingNumbers[j, i] = Indice(Det)
             data = S.r - WindingNumbers
             sigmas, lambdas = np.meshgrid(lambdas, sigmas)
             plt.contourf(sigmas, lambdas, data)
             plt.colorbar()
             plt.title(
-                f"Number of zeros of KL determinant for {schem(1/2,left_bound, order = order, sigma=sigma).name(boundary_bool = True, sigma_bool = False, lambda_bool = False)} with respect to $\lambda$ and $\sigma$"
+                f"Number of zeros of KL determinant for {schem(1/2,left_bound, sigma=sigma).name(boundary_bool = True, sigma_bool = False, lambda_bool = False)} with respect to $\lambda$ and $\sigma$"
             )
             plt.xlabel("$\lambda$")
             plt.ylabel("$\sigma$")
-        return ax
+        plt.show()
```

