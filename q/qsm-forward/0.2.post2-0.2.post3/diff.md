# Comparing `tmp/qsm_forward-0.2.post2.tar.gz` & `tmp/qsm-forward-0.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm_forward-0.2.post2.tar", last modified: Wed Jun 14 02:05:05 2023, max compression
+gzip compressed data, was "qsm-forward-0.2.post3.tar", last modified: Wed Jun 14 04:08:19 2023, max compression
```

## Comparing `qsm_forward-0.2.post2.tar` & `qsm-forward-0.2.post3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm_forward-0.2.post2/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      752 2023-06-14 02:03:58.000000 qsm_forward-0.2.post2/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.001659 qsm_forward-0.2.post2/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      397 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    11985 2023-06-14 02:03:24.000000 qsm_forward-0.2.post2/qsm_forward/qsm_forward.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)     8139 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/qsm_forward/visualisation.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      321 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       67 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      916 2023-06-14 02:04:09.000000 qsm_forward-0.2.post2/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:08:19.004811 qsm-forward-0.2.post3/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.2.post3/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 04:08:19.004811 qsm-forward-0.2.post3/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.2.post3/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      752 2023-06-14 03:32:43.000000 qsm-forward-0.2.post3/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:08:19.004811 qsm-forward-0.2.post3/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      425 2023-06-14 04:06:28.000000 qsm-forward-0.2.post3/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    12015 2023-06-14 04:07:21.000000 qsm-forward-0.2.post3/qsm_forward/qsm_forward.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     8139 2023-06-12 05:17:28.000000 qsm-forward-0.2.post3/qsm_forward/visualisation.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:08:19.004811 qsm-forward-0.2.post3/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 04:08:18.000000 qsm-forward-0.2.post3/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      321 2023-06-14 04:08:18.000000 qsm-forward-0.2.post3/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 04:08:18.000000 qsm-forward-0.2.post3/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 04:08:18.000000 qsm-forward-0.2.post3/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 04:08:18.000000 qsm-forward-0.2.post3/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 04:08:19.004811 qsm-forward-0.2.post3/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      814 2023-06-14 03:31:54.000000 qsm-forward-0.2.post3/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:08:19.004811 qsm-forward-0.2.post3/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.2.post3/tests/test_qsm_forward.py
```

### Comparing `qsm_forward-0.2.post2/LICENSE` & `qsm-forward-0.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2.post2/PKG-INFO` & `qsm-forward-0.2.post3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qsm_forward
-Version: 0.2.post2
+Name: qsm-forward
+Version: 0.2.post3
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm_forward-0.2.post2/README.md` & `qsm-forward-0.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2.post2/pyproject.toml` & `qsm-forward-0.2.post3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "qsm_forward"
-version = "0.2-2"
+name = "qsm-forward"
+version = "0.2-3"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm_forward-0.2.post2/qsm_forward/qsm_forward.py` & `qsm-forward-0.2.post3/qsm_forward/qsm_forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from dipy.denoise.gibbs import gibbs_removal
 from nilearn.image import resample_img
 
-def forward_convolution(chi):
+def generate_field(chi):
     """
     Perform the forward convolution operation.
 
     This function performs the forward convolution step of the QSM simulation.
 
     Parameters
     ----------
@@ -25,111 +25,88 @@
     chitemp = np.ones(2 * dims) * chi[-1, -1, -1]
     chitemp[:dims[0], :dims[1], :dims[2]] = chi
     field = np.real(np.fft.ifftn(np.fft.fftn(chitemp) * D))
     field = field[:dims[0], :dims[1], :dims[2]]
 
     return field
 
-def signal_model(field, B0=3, TR=1, TE=30e-3, flip_angle=90, phase_offset=0, R1=1, R2star=50, M0=1):
+def generate_phase_offset(M0, brain_mask, dims):
     """
-    Compute the MRI signal based on the given parameters.
+    Generate a suitable phase offset.
 
     Parameters
     ----------
-    field : numpy.ndarray
-        The magnetic field distribution.
-    B0 : float, optional
-        The main magnetic field strength. Default is 3.
-    TR : float, optional
-        The repetition time. Default is 1.
-    TE : float, optional
-        The echo time. Default is 30e-3.
-    flip_angle : float, optional
-        The flip angle in degrees. Default is 90.
-    phase_offset : float, optional
-        The phase offset. Default is 0.
-    R1 : float or numpy.ndarray, optional
-        The longitudinal relaxation rate. Can be a single value or a 3D numpy array. Default is 1.
-    R2star : float or numpy.ndarray, optional
-        The effective transverse relaxation rate. Can be a single value or a 3D numpy array. Default is 50.
-    M0 : float or numpy.ndarray, optional
-        The equilibrium magnetization. Can be a single value or a 3D numpy array. Default is 1.
+    M0 : numpy.ndarray
+        The initial magnetization.
+    brain_mask : numpy.ndarray
+        A binary mask that indicates the region of the brain.
+    dims : tuple of int
+        The dimensions of the input image.
 
     Returns
     -------
     numpy.ndarray
-        The computed MRI signal.
-
-    """
-
-    sigHR = M0 * np.exp(1j * (2 * np.pi * field * B0 * 42.58 * TE + phase_offset)) * np.exp(-TE * R2star) \
-        * (1 - np.exp(-TR * R1)) * np.sin(np.deg2rad(flip_angle)) / (1 - np.cos(np.deg2rad(flip_angle)) * np.exp(-TR * R1))
-    sigHR[np.isnan(sigHR)] = 0
-
-    return sigHR
+        The phase offset of the input image.
 
-def add_noise(sig, peak_snr=np.inf):
     """
-    Add complex Gaussian noise to a signal.
-
-    Parameters
-    ----------
-    sig : numpy.ndarray
-        The input signal to which noise will be added.
-    peak_snr : float, optional
-        The peak signal-to-noise ratio, by default np.inf
 
-    Returns
-    -------
-    numpy.ndarray
-        The input signal with added noise.
-
-    """
+    c, w = _center_of_mass(M0)
+    
+    x, y, z = np.meshgrid(
+        np.arange(1, dims[1]+1)-c[1],
+        np.arange(1, dims[0]+1)-c[0],
+        np.arange(1, dims[2]+1)-c[2]
+    )
+    
+    temp = (x/w[1])**2 + (y/w[0])**2 + (z/w[2])**2
+    
+    max_temp = np.max(temp[brain_mask != 0])
+    min_temp = np.min(temp[brain_mask != 0])
+    
+    phase_offset = -temp / (max_temp - min_temp) * np.pi
 
-    noise = np.random.randn(*sig.shape) + 1j * np.random.randn(*sig.shape)
-    sig_noisy = sig + (noise * np.max(np.abs(sig))) / peak_snr
-    return sig_noisy
+    return phase_offset
 
 
-def poly_fit_shim_like(volume, brain_mask, order=2):
+def generate_shimmed_field(field, brain_mask, order=2):
     """
-    Perform a polynomial fit of the given order to a volume using a binary brain mask to select points.
+    Simulate field shimming by fitting the field with second- and third-order Legendre polynomials.
 
     Parameters
     ----------
-    volume : numpy.ndarray
-        3D array representing the volume to fit.
+    field : numpy.ndarray
+        3D array representing the magnetic field to fit.
     brain_mask : numpy.ndarray
-        3D binary array. Must be the same shape as `volume`. A True value at a coordinate will 
+        3D binary array. Must be the same shape as `field`. A True value at a coordinate will 
         include that point in the fit.
     order : int, optional
         The order of the polynomial to fit. Must be 0, 1, or 2. Default is 2.
 
     Returns
     -------
     FIT3D : numpy.ndarray
-        3D array representing the fitted volume.
+        3D array representing the fitted field.
     Residuals : numpy.ndarray
         3D array representing the residuals of the fit.
     b : numpy.ndarray
         1D array representing the coefficients of the fitted polynomial.
 
     Raises
     ------
     ValueError
-        If `volume` and `brain_mask` shapes are not the same.
+        If `field` and `brain_mask` shapes are not the same.
     """
 
-    dim = volume.shape
+    dim = field.shape
     
     ## for volume fitting
     #brain_mask = np.ones(brain_mask.shape)
     indices = np.nonzero(brain_mask)
     x1, y1, z1 = indices
-    R = volume[indices]
+    R = field[indices]
     b = None
     
     if len(indices[0]) > (3*order)**2:
         model = _create_model(x1, y1, z1, dim, order)
         b = np.linalg.pinv(model) @ R
         temp = R - model @ b
         del model, R
@@ -138,62 +115,85 @@
         x1, y1, z1 = [ind.flatten() for ind in indices]
         model = _create_model(x1, y1, z1, dim, order)
         
         Fit = model @ b
         del model
         
         FIT3D = Fit.reshape(dim)
-        Residuals = (volume-FIT3D)
+        Residuals = (field-FIT3D)
     else:
-        FIT3D = np.zeros_like(volume)
-        Residuals = (volume-FIT3D) * brain_mask
+        FIT3D = np.zeros_like(field)
+        Residuals = (field-FIT3D) * brain_mask
     
     return FIT3D, Residuals, b
 
-def compute_phase_offset(M0, brain_mask, dims):
+def generate_signal(field, B0=3, TR=1, TE=30e-3, flip_angle=90, phase_offset=0, R1=1, R2star=50, M0=1):
     """
-    Compute the phase offset of an image.
+    Compute the MRI signal based on the given parameters.
 
     Parameters
     ----------
-    M0 : numpy.ndarray
-        The input image.
-    brain_mask : numpy.ndarray
-        A binary mask that indicates the region of the brain.
-    dims : tuple of int
-        The dimensions of the input image.
+    field : numpy.ndarray
+        The magnetic field distribution.
+    B0 : float, optional
+        The main magnetic field strength. Default is 3.
+    TR : float, optional
+        The repetition time. Default is 1.
+    TE : float, optional
+        The echo time. Default is 30e-3.
+    flip_angle : float, optional
+        The flip angle in degrees. Default is 90.
+    phase_offset : float, optional
+        The phase offset. Default is 0.
+    R1 : float or numpy.ndarray, optional
+        The longitudinal relaxation rate. Can be a single value or a 3D numpy array. Default is 1.
+    R2star : float or numpy.ndarray, optional
+        The effective transverse relaxation rate. Can be a single value or a 3D numpy array. Default is 50.
+    M0 : float or numpy.ndarray, optional
+        The equilibrium magnetization. Can be a single value or a 3D numpy array. Default is 1.
 
     Returns
     -------
     numpy.ndarray
-        The phase offset of the input image.
+        The computed MRI signal.
 
     """
 
-    c, w = _center_of_mass(M0)
-    
-    x, y, z = np.meshgrid(
-        np.arange(1, dims[1]+1)-c[1],
-        np.arange(1, dims[0]+1)-c[0],
-        np.arange(1, dims[2]+1)-c[2]
-    )
-    
-    temp = (x/w[1])**2 + (y/w[0])**2 + (z/w[2])**2
-    
-    max_temp = np.max(temp[brain_mask != 0])
-    min_temp = np.min(temp[brain_mask != 0])
-    
-    phase_offset = -temp / (max_temp - min_temp) * np.pi
+    sigHR = M0 * np.exp(1j * (2 * np.pi * field * B0 * 42.58 * TE + phase_offset)) * np.exp(-TE * R2star) \
+        * (1 - np.exp(-TR * R1)) * np.sin(np.deg2rad(flip_angle)) / (1 - np.cos(np.deg2rad(flip_angle)) * np.exp(-TR * R1))
+    sigHR[np.isnan(sigHR)] = 0
 
-    return phase_offset
+    return sigHR
+
+def add_noise(sig, peak_snr=np.inf):
+    """
+    Add complex Gaussian noise to a signal.
+
+    Parameters
+    ----------
+    sig : numpy.ndarray
+        The input signal to which noise will be added.
+    peak_snr : float, optional
+        The peak signal-to-noise ratio, by default np.inf
+
+    Returns
+    -------
+    numpy.ndarray
+        The input signal with added noise.
+
+    """
+
+    noise = np.random.randn(*sig.shape) + 1j * np.random.randn(*sig.shape)
+    sig_noisy = sig + (noise * np.max(np.abs(sig))) / peak_snr
+    return sig_noisy
 
 
 def resize(nii, voxel_size):
     """
-    Resize a Nifti image.
+    Resize a Nifti image to a voxel size.
 
     Parameters
     ----------
     nii : nibabel.nifti1.Nifti1Image
         The input Nifti image.
     voxel_size : list of float
         The desired voxel size after resizing.
@@ -212,15 +212,15 @@
         nii,
         target_affine=target_affine,
         target_shape=target_shape,
         interpolation='nearest'
     )
 
 
-def crop(x, shape):
+def crop_imagespace(x, shape):
     """
     Crop a nD matrix around its center.
 
     Parameters
     ----------
     x : numpy.ndarray
         The input n-dimensional matrix.
@@ -245,15 +245,15 @@
     for n in range(s.size):
         start = np.floor_divide(m[n], 2) + np.ceil(-s[n] / 2)
         end = np.floor_divide(m[n], 2) + np.ceil(s[n] / 2)
         idx.append(slice(int(start), int(end)))
     res = x[tuple(idx)]
     return res
 
-def kspace_crop(volume, dims, scaling=False, gibbs_correction=True):
+def crop_kspace(volume, dims, scaling=False, gibbs_correction=True):
     """
     Crop a 3D volume in k-space and apply optional scaling and Gibbs ringing correction.
 
     Parameters
     ----------
     volume : numpy.ndarray
         The input 3D volume.
```

### Comparing `qsm_forward-0.2.post2/qsm_forward/visualisation.py` & `qsm-forward-0.2.post3/qsm_forward/visualisation.py`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2.post2/qsm_forward.egg-info/PKG-INFO` & `qsm-forward-0.2.post3/qsm_forward.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.2.post2
+Version: 0.2.post3
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm_forward-0.2.post2/setup.py` & `qsm-forward-0.2.post3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='qsm_forward',
-    version='0.2-2',
+    name='qsm-forward',
+    version='0.2-3',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'numpy',
-        'matplotlib',
-        'nibabel',
         'nilearn',
-        'ipykernel',
-        'scikit-image',
-        'dipy',
-        'torch'
+        'dipy'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
 )
+
```

