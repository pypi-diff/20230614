# Comparing `tmp/xarrayuvecs-0.1.8-py3-none-any.whl.zip` & `tmp/xarrayuvecs-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 171099 bytes, number of entries: 10
+Zip file size: 171100 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      166 b- defN 22-Nov-16 11:09 xarrayuvecs/__init__.py
--rw-r--r--  2.0 unx     2831 b- defN 22-Nov-17 10:22 xarrayuvecs/lut2d.py
+-rw-r--r--  2.0 unx     2831 b- defN 22-Nov-17 18:03 xarrayuvecs/lut2d.py
 -rw-r--r--  2.0 unx     4835 b- defN 22-Nov-17 10:46 xarrayuvecs/odfplot.py
 -rw-r--r--  2.0 unx   536222 b- defN 22-Nov-16 11:09 xarrayuvecs/uniform_dist.py
 -rw-r--r--  2.0 unx    27889 b- defN 22-Nov-17 13:51 xarrayuvecs/uvecs.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Nov-17 17:49 xarrayuvecs-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      840 b- defN 22-Nov-17 17:49 xarrayuvecs-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-17 17:49 xarrayuvecs-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-Nov-17 17:49 xarrayuvecs-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      805 b- defN 22-Nov-17 17:49 xarrayuvecs-0.1.8.dist-info/RECORD
-10 files, 608841 bytes uncompressed, 169735 bytes compressed:  72.1%
+-rw-r--r--  2.0 unx    35149 b- defN 22-Nov-17 18:04 xarrayuvecs-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      840 b- defN 22-Nov-17 18:04 xarrayuvecs-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Nov-17 18:04 xarrayuvecs-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 22-Nov-17 18:04 xarrayuvecs-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      805 b- defN 22-Nov-17 18:04 xarrayuvecs-0.1.9.dist-info/RECORD
+10 files, 608841 bytes uncompressed, 169736 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: xarrayuvecs/uniform_dist.py
 Comment: 
 
 Filename: xarrayuvecs/uvecs.py
 Comment: 
 
-Filename: xarrayuvecs-0.1.8.dist-info/LICENSE
+Filename: xarrayuvecs-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: xarrayuvecs-0.1.8.dist-info/METADATA
+Filename: xarrayuvecs-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xarrayuvecs-0.1.8.dist-info/WHEEL
+Filename: xarrayuvecs-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xarrayuvecs-0.1.8.dist-info/top_level.txt
+Filename: xarrayuvecs-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xarrayuvecs-0.1.8.dist-info/RECORD
+Filename: xarrayuvecs-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xarrayuvecs/lut2d.py

```diff
@@ -91,14 +91,14 @@
     xyz=xr.DataArray(np.dstack([phi,theta]),dims=('y','x','uvecs')).uvecs.xyz()
 
     data=np.dstack([phi,theta,xyz])
 
     data[np.isnan(theta),0]=np.nan
 
     fig=px.imshow(ll)
-    fig.data[0]['hovertemplate']='(phi,theta):(%{customdata[0]:.3f},%{customdata[1]:.3f}) <br> (x,y,z):(%{customdata[2]:.3f},%{customdata[3]:.3f},%{customdata[4]:.3f}) '
+    fig.data[0]['hovertemplate']='(phi,theta):(%{customdata[1]:.3f},%{customdata[2]:.3f}) <br> (x,y,z):(%{customdata[2]:.3f},%{customdata[3]:.3f},%{customdata[4]:.3f}) '
     fig.data[0]['customdata']=data
 
     fig=fig.update_xaxes(visible=False)
     fig=fig.update_yaxes(visible=False)
 
     return fig
```

## Comparing `xarrayuvecs-0.1.8.dist-info/LICENSE` & `xarrayuvecs-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xarrayuvecs-0.1.8.dist-info/METADATA` & `xarrayuvecs-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarrayuvecs
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to work on unit vector that are symmetric (i.e. x is equivalent to -x)
 Home-page: https://gricad-gitlab.univ-grenoble-alpes.fr/mecaiceige/tools/lib_python/xarray_uvecs
 Author: Thomas Chauve
 Author-email: thomas.chauve@univ-grenoble-alpes.fr
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

## Comparing `xarrayuvecs-0.1.8.dist-info/RECORD` & `xarrayuvecs-0.1.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xarrayuvecs/__init__.py,sha256=zybPYhLAfZU98HQa8F9mmKWZ8Rfu9kQUVMJCBkdYGPs,166
-xarrayuvecs/lut2d.py,sha256=GZC1NoiBl9IucncQLMNRYuQP3btDhlcPMtEQGIGmZtI,2831
+xarrayuvecs/lut2d.py,sha256=xfonEejzNjCwOIAHaUKdHNlj7g3PyYHG77sU26ISRGg,2831
 xarrayuvecs/odfplot.py,sha256=nIk9nQsxSRxRzzm_7Daf6pW16yvVMYFIhA3okbFLYz4,4835
 xarrayuvecs/uniform_dist.py,sha256=MQNh-rwye-XnL2_eJtrGnu0ZL6upIY_Bdtdwg6cK7pg,536222
 xarrayuvecs/uvecs.py,sha256=MgyudUnN7LWspQt32csg8iaQOO0pjZyUckuDcfplJrE,27889
-xarrayuvecs-0.1.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-xarrayuvecs-0.1.8.dist-info/METADATA,sha256=sV18-jGYgfSWluXQDoVS7runRfOa1mkbEApB43CG5Ck,840
-xarrayuvecs-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xarrayuvecs-0.1.8.dist-info/top_level.txt,sha256=fj3quk3cPiFOh9jZM-1NSW5qNcQv-udx8nsuI3qYMMA,12
-xarrayuvecs-0.1.8.dist-info/RECORD,,
+xarrayuvecs-0.1.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+xarrayuvecs-0.1.9.dist-info/METADATA,sha256=Xc5ZSnp3lTGtrVYaSxXT-SI1wWq2y2zyZvS2EG7xgg0,840
+xarrayuvecs-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xarrayuvecs-0.1.9.dist-info/top_level.txt,sha256=fj3quk3cPiFOh9jZM-1NSW5qNcQv-udx8nsuI3qYMMA,12
+xarrayuvecs-0.1.9.dist-info/RECORD,,
```

