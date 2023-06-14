# Comparing `tmp/qsm-forward-0.4.tar.gz` & `tmp/qsm-forward-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm-forward-0.4.tar", last modified: Wed Jun 14 05:55:46 2023, max compression
+gzip compressed data, was "qsm-forward-0.5.tar", last modified: Wed Jun 14 06:57:44 2023, max compression
```

## Comparing `qsm-forward-0.4.tar` & `qsm-forward-0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.4/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:55:46.437987 qsm-forward-0.4/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.4/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-14 05:55:09.000000 qsm-forward-0.4/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      465 2023-06-14 05:36:03.000000 qsm-forward-0.4/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    19256 2023-06-14 05:34:06.000000 qsm-forward-0.4/qsm_forward/qsm_forward.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 05:55:46.437987 qsm-forward-0.4/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-14 05:36:21.000000 qsm-forward-0.4/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.4/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.5/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 06:57:44.977896 qsm-forward-0.5/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.5/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-14 06:55:50.000000 qsm-forward-0.5/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      465 2023-06-14 05:36:03.000000 qsm-forward-0.5/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    19754 2023-06-14 06:54:44.000000 qsm-forward-0.5/qsm_forward/qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 06:57:44.977896 qsm-forward-0.5/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-14 06:55:36.000000 qsm-forward-0.5/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.5/tests/test_qsm_forward.py
```

### Comparing `qsm-forward-0.4/LICENSE` & `qsm-forward-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.4/PKG-INFO` & `qsm-forward-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.4
+Version: 0.5
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.4/README.md` & `qsm-forward-0.5/README.md`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.4/pyproject.toml` & `qsm-forward-0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm-forward"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm-forward-0.4/qsm_forward/qsm_forward.py` & `qsm-forward-0.5/qsm_forward/qsm_forward.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from dipy.denoise.gibbs import gibbs_removal
 from nilearn.image import resample_img
 
 import json
 import os
 import nibabel as nib
 import numpy as np
-import qsm_forward
 
 # Default parameters for tissue
 default_tissue_params = {
     "chi_path" : "ChiModelMIX_noCalc.nii.gz",
     "M0_path" : "M0.nii.gz",
     "R1_path" : "R1.nii.gz",
     "R2star_path" : "R2star.nii.gz",
@@ -30,15 +29,16 @@
     "Run" : 1,                      # Run number
     "TR" : 50e-3,                   # Repetition time (in seconds)
     "TEs" : np.array([ 4e-3, 12e-3, 20e-3, 28e-3 ]), # Echo times (in seconds)
     "flip_angle" : 15,              # Flip angle (in degrees)
     "B0" : 7,                       # Magnetic field strength (in Tesla)
     "B0_dir" : np.array([0, 0, 1]), # B0 field direction
     "phase_offset" : 0,             # Phase offset (in radians)
-    "shimm" : False,                # Boolean to control shimming
+    "generate_phase_offset": True,  # Boolean to control phase offset generation
+    "generate_shim_field" : True,   # Boolean to control shim field generation
     "voxel_size" : np.array([1.0, 1.0, 1.0]), # Voxel size (in mm)
     "peak_snr" : np.inf             # Peak signal-to-noise ratio
 }
 
 def generate_bids(tissue_params, recon_params, bids_dir):
     """
     Generate T2*-weighted MRI signals and save the outputs in the BIDS-compliant format.
@@ -71,68 +71,75 @@
     session_dir = os.path.join(bids_dir, f"sub-{recon_params['Subject']}", f"ses-{recon_params['Session']}")
     os.makedirs(os.path.join(session_dir, 'anat'), exist_ok=True)
     os.makedirs(os.path.join(session_dir, 'extra_data'), exist_ok=True)
 
     # image-space resizing
     chi_nii = nib.load(tissue_params['chi_path'])
     print("Image-space resizing of chi...")
-    chi_downsampled_nii = qsm_forward.resize(chi_nii, recon_params['voxel_size'])
-    nib.save(chi_downsampled_nii, filename=os.path.join(session_dir, "extra_data", "chi.nii"))
-    print("Image-space cropping of brain mask...")
-    mask_downsampled_nii = qsm_forward.resize(nib.load(tissue_params['mask_path']), recon_params['voxel_size'], 'nearest')
-    nib.save(mask_downsampled_nii, filename=os.path.join(session_dir, "extra_data", "brain-mask.nii"))
-    del mask_downsampled_nii
-    print("Image-space cropping of segmentation...")
-    seg_downsampled_nii = qsm_forward.resize(nib.load(tissue_params['seg_path']), recon_params['voxel_size'], 'nearest')
-    nib.save(seg_downsampled_nii, filename=os.path.join(session_dir, "extra_data", "segmentation.nii"))
-    del seg_downsampled_nii
+    chi_downsampled_nii = resize(chi_nii, recon_params['voxel_size'])
+    nib.save(chi_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_chi.nii"))
+    if os.path.exists(str(tissue_params['mask_path'])):
+        print("Image-space cropping of mask...")
+        mask_downsampled_nii = resize(nib.load(tissue_params['mask_path']), recon_params['voxel_size'], 'nearest')
+        nib.save(mask_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_mask.nii"))
+        del mask_downsampled_nii
+    if os.path.exists(str(tissue_params['seg_path'])):
+        print("Image-space cropping of segmentation...")
+        seg_downsampled_nii = resize(nib.load(tissue_params['seg_path']), recon_params['voxel_size'], 'nearest')
+        nib.save(seg_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_segmentation.nii"))
+        del seg_downsampled_nii
 
     # calculate field
     print("Computing field model...")
     chi = chi_nii.get_fdata()
-    field = qsm_forward.generate_field(chi)
+    field = generate_field(chi)
     del chi
 
     # simulate shim field
-    print("Computing shim fields...")
-    brain_mask = nib.load(tissue_params['mask_path']).get_fdata()
-    _, field, _ = qsm_forward.generate_shimmed_field(field, brain_mask, order=2)
+    mask = nib.load(tissue_params['mask_path']).get_fdata() if os.path.exists(tissue_params['mask_path']) else np.ones(field.shape)
+    if recon_params['generate_shim_field']:
+        print("Computing shim fields...")
+        _, field, _ = generate_shimmed_field(field, mask, order=2)
 
     # phase offset
-    print("Computing phase offset...")
-    M0 = nib.load(tissue_params['M0_path']).get_fdata()
-    phase_offset = qsm_forward.generate_phase_offset(M0, brain_mask, M0.shape)
-    del brain_mask
+    M0 = nib.load(tissue_params['M0_path']).get_fdata() if os.path.exists(tissue_params['M0_path']) else np.ones(field.shape) * mask
+    if recon_params['generate_phase_offset']:
+        print("Computing phase offset...")
+        phase_offset = recon_params['phase_offset'] + generate_phase_offset(M0, mask, M0.shape)
 
     # signal model
     multiecho = len(recon_params['TEs']) > 1
+    R1 = nib.load(tissue_params['R1_path']).get_fdata() if os.path.exists(tissue_params['R1_path']) else np.ones(field.shape) * mask
+    R2star = nib.load(tissue_params['R2star_path']).get_fdata() if os.path.exists(tissue_params['R2star_path']) else np.ones(field.shape) * mask
+    del mask
     for i in range(len(recon_params['TEs'])):
         print(f"Computing MR signal for echo {i+1}...")
         recon_name_i = f"{recon_name}_echo-{i+1}" if multiecho else recon_name
-        sigHR = qsm_forward.generate_signal(
+
+        sigHR = generate_signal(
             field=field,
             B0=recon_params['B0'],
             TR=recon_params['TR'],
             TE=recon_params['TEs'][i],
             flip_angle=recon_params['flip_angle'],
             phase_offset=phase_offset,
-            R1=nib.load(tissue_params['R1_path']).get_fdata(),
-            R2star=nib.load(tissue_params['R2star_path']).get_fdata(),
-            M0=nib.load(tissue_params['M0_path']).get_fdata()
+            R1=R1,
+            R2star=R2star,
+            M0=M0
         )
     
         # k-space cropping of sigHR
         print(f"k-space cropping of MR signal for echo {i+1}...")
         resolution = np.array(np.round((np.array(chi_nii.header.get_zooms()) / recon_params['voxel_size']) * np.array(chi_nii.header.get_data_shape())), dtype=int)
-        sigHR_cropped = qsm_forward.crop_kspace(sigHR, resolution)
+        sigHR_cropped = crop_kspace(sigHR, resolution)
         del sigHR
 
         # noise
         print(f"Simulating noise for echo {i+1}...")
-        sigHR_cropped_noisy = qsm_forward.add_noise(sigHR_cropped, peak_snr=recon_params['peak_snr'])
+        sigHR_cropped_noisy = add_noise(sigHR_cropped, peak_snr=recon_params['peak_snr'])
         del sigHR_cropped
 
         # save nifti images
         mag_filename = f"{recon_name_i}_part-mag" + ("_MEGRE" if multiecho else "_T2starw")
         phs_filename = f"{recon_name_i}_part-phase" + ("_MEGRE" if multiecho else "_T2starw")
         nib.save(nib.Nifti1Image(dataobj=np.abs(sigHR_cropped_noisy), affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{mag_filename}.nii"))
         nib.save(nib.Nifti1Image(dataobj=np.angle(sigHR_cropped_noisy), affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{phs_filename}.nii"))
@@ -177,24 +184,24 @@
     chitemp = np.ones(2 * dims) * chi[-1, -1, -1]
     chitemp[:dims[0], :dims[1], :dims[2]] = chi
     field = np.real(np.fft.ifftn(np.fft.fftn(chitemp) * D))
     field = field[:dims[0], :dims[1], :dims[2]]
 
     return field
 
-def generate_phase_offset(M0, brain_mask, dims):
+def generate_phase_offset(M0, mask, dims):
     """
     Generate a suitable phase offset.
 
     Parameters
     ----------
     M0 : numpy.ndarray
         The initial magnetization.
-    brain_mask : numpy.ndarray
-        A binary mask that indicates the region of the brain.
+    mask : numpy.ndarray
+        A binary mask that indicates the internal region of interest.
     dims : tuple of int
         The dimensions of the input image.
 
     Returns
     -------
     numpy.ndarray
         The phase offset of the input image.
@@ -207,31 +214,31 @@
         np.arange(1, dims[1]+1)-c[1],
         np.arange(1, dims[0]+1)-c[0],
         np.arange(1, dims[2]+1)-c[2]
     )
     
     temp = (x/w[1])**2 + (y/w[0])**2 + (z/w[2])**2
     
-    max_temp = np.max(temp[brain_mask != 0])
-    min_temp = np.min(temp[brain_mask != 0])
+    max_temp = np.max(temp[mask != 0])
+    min_temp = np.min(temp[mask != 0])
     
     phase_offset = -temp / (max_temp - min_temp) * np.pi
 
     return phase_offset
 
 
-def generate_shimmed_field(field, brain_mask, order=2):
+def generate_shimmed_field(field, mask, order=2):
     """
     Simulate field shimming by fitting the field with second- and third-order Legendre polynomials.
 
     Parameters
     ----------
     field : numpy.ndarray
         3D array representing the magnetic field to fit.
-    brain_mask : numpy.ndarray
+    mask : numpy.ndarray
         3D binary array. Must be the same shape as `field`. A True value at a coordinate will 
         include that point in the fit.
     order : int, optional
         The order of the polynomial to fit. Must be 0, 1, or 2. Default is 2.
 
     Returns
     -------
@@ -241,22 +248,22 @@
         3D array representing the residuals of the fit.
     b : numpy.ndarray
         1D array representing the coefficients of the fitted polynomial.
 
     Raises
     ------
     ValueError
-        If `field` and `brain_mask` shapes are not the same.
+        If `field` and `mask` shapes are not the same.
     """
 
     dim = field.shape
     
     ## for volume fitting
-    #brain_mask = np.ones(brain_mask.shape)
-    indices = np.nonzero(brain_mask)
+    #mask = np.ones(mask.shape)
+    indices = np.nonzero(mask)
     x1, y1, z1 = indices
     R = field[indices]
     b = None
     
     if len(indices[0]) > (3*order)**2:
         model = _create_model(x1, y1, z1, dim, order)
         b = np.linalg.pinv(model) @ R
@@ -270,15 +277,15 @@
         Fit = model @ b
         del model
         
         FIT3D = Fit.reshape(dim)
         Residuals = (field-FIT3D)
     else:
         FIT3D = np.zeros_like(field)
-        Residuals = (field-FIT3D) * brain_mask
+        Residuals = (field-FIT3D) * mask
     
     return FIT3D, Residuals, b
 
 def generate_signal(field, B0=3, TR=1, TE=30e-3, flip_angle=90, phase_offset=0, R1=1, R2star=50, M0=1):
     """
     Compute the MRI signal based on the given parameters.
```

### Comparing `qsm-forward-0.4/qsm_forward.egg-info/PKG-INFO` & `qsm-forward-0.5/qsm_forward.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.4
+Version: 0.5
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.4/setup.py` & `qsm-forward-0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm-forward',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

