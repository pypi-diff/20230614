# Comparing `tmp/ShuaiToolBox-1.1.1.tar.gz` & `tmp/ShuaiToolBox-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ShuaiToolBox-1.1.1.tar", last modified: Tue Jun 13 07:31:59 2023, max compression
+gzip compressed data, was "dist\ShuaiToolBox-1.1.2.tar", last modified: Wed Jun 14 01:59:53 2023, max compression
```

## Comparing `ShuaiToolBox-1.1.1.tar` & `ShuaiToolBox-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/
--rw-rw-rw-   0        0        0      199 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/
--rw-rw-rw-   0        0        0     2617 2021-09-13 13:48:20.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/FindContours.py
--rw-rw-rw-   0        0        0    13825 2023-06-13 07:05:00.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/VideoPro.py
--rw-rw-rw-   0        0        0     8052 2023-06-13 07:04:46.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/VideoProList.py
--rw-rw-rw-   0        0        0      161 2023-06-13 07:22:54.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/__init__.py
--rw-rw-rw-   0        0        0     1028 2022-12-21 14:44:22.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/cv_plugin.py
--rw-rw-rw-   0        0        0     2136 2021-08-31 08:12:37.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/cv_vdopro.py
--rw-rw-rw-   0        0        0     7798 2023-06-13 03:55:53.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/opencv_Functions.py
--rw-rw-rw-   0        0        0     1635 2023-06-13 05:48:13.000000 ShuaiToolBox-1.1.1/ShuaiToolBox/py_plugin.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/ShuaiToolBox.egg-info/
--rw-rw-rw-   0        0        0      199 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/ShuaiToolBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/ShuaiToolBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/ShuaiToolBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/ShuaiToolBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 07:31:59.000000 ShuaiToolBox-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-13 07:30:01.000000 ShuaiToolBox-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/
+-rw-rw-rw-   0        0        0      199 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/
+-rw-rw-rw-   0        0        0    12679 2023-06-13 09:51:02.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/EORmodule.py
+-rw-rw-rw-   0        0        0     2526 2023-06-13 08:11:37.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/FindContours.py
+-rw-rw-rw-   0        0        0    13782 2023-06-13 08:11:14.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/VideoPro.py
+-rw-rw-rw-   0        0        0     8658 2023-06-14 01:55:09.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/VideoProList.py
+-rw-rw-rw-   0        0        0      187 2023-06-13 09:22:13.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/__init__.py
+-rw-rw-rw-   0        0        0     1026 2023-06-13 08:21:34.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/cv_plugin.py
+-rw-rw-rw-   0        0        0     2119 2023-06-13 08:06:47.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/cv_vdopro.py
+-rw-rw-rw-   0        0        0     8687 2023-06-14 01:59:16.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/opencv_Functions.py
+-rw-rw-rw-   0        0        0     1635 2023-06-13 07:56:00.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/py_plugin.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-06-13 07:56:32.000000 ShuaiToolBox-1.1.2/setup.py
```

### Comparing `ShuaiToolBox-1.1.1/ShuaiToolBox/FindContours.py` & `ShuaiToolBox-1.1.2/ShuaiToolBox/FindContours.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-from __future__ import division
 import cv2
-#import numpy as np
 import copy
 import time
 
-
-# img = cv2.imread(r'D:\1.jpg')
-
 def ContoursFilterByMouse(images):
     # Get image
     image = copy.copy(images)
     # init the window
     WindowName = 'Image'
     cv2.namedWindow(WindowName)
     cv2.imshow(WindowName, image)
```

### Comparing `ShuaiToolBox-1.1.1/ShuaiToolBox/VideoPro.py` & `ShuaiToolBox-1.1.2/ShuaiToolBox/VideoPro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import multiprocessing as mp
-
-from cv_plugin import *
-from cv_vdopro import *
-from FindContours import *
-import numpy as np
-import opencv_Functions as cvFun
+from .cv_plugin import *
+from .cv_vdopro import *
+from .FindContours import *
+from .opencv_Functions import GetIndex,cv_GenImage
 
 # 根据颜色上下限对图像进行二值化处理
 def color_seperate(image, lower_hsv, upper_hsv):
     hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)  # 对目标图像进行色彩空间转换
     # 依据设定的上下限对目标图像进行二值化转换,在区间内的为1，不在区间内的为0
     mask = cv2.inRange(hsv, lowerb=lower_hsv, upperb=upper_hsv)
     # dst = cv.bitwise_and(image, image, mask=mask)    #将二值化图像与原图进行“与”操作；实际是提取前两个frame 的“与”结果，然后输出mask 为1的部分
@@ -182,15 +179,15 @@
     for c in Cliplist:
         # Get Index
         _from=c.start_i
         _to=c.end_i
         _IndexFrom=Videos[_from].FPS*(c.start_min*60+c.start_sec)
         _IndexTo = Videos[_to].FPS * (c.end_min * 60 + c.end_sec)
         _clip=[_from,_to,_IndexFrom,_IndexTo]
-        _VideoIndex,_FrameIndex=cvFun.GetIndex(_FrameCount,_clip,FrameSpace)
+        _VideoIndex,_FrameIndex=GetIndex(_FrameCount,_clip,FrameSpace)
 
         Clip_Cap = []
         Clip_frames = []
 
         for i in range(len(_VideoIndex)):
             vdo=Videos[_VideoIndex[i]]
             VdoCap=cv2.VideoCapture(vdo.path)
@@ -207,15 +204,15 @@
                 # cv2.waitKey(0)
                 if ret:
                     Clip_frames.append(frame)
                     temp_capture.GetFrame(frame)
                     record_frame=frame
                 else:
                     print('------------Lost one frame at No. '+str(frame_num)+'/'+str(len(_FrameIndex[i]))+'-------------')
-                    blank=cvFun.cv_GenImage(record_frame)
+                    blank=cv_GenImage(record_frame)
                     Clip_frames.append(blank)
                 Clip_Cap.append(temp_capture)
                 frame_num=frame_num+1
 
             VdoCap.release()
         Frames.extend(Clip_frames)
         Captures.extend(Clip_Cap)
```

### Comparing `ShuaiToolBox-1.1.1/ShuaiToolBox/VideoProList.py` & `ShuaiToolBox-1.1.2/ShuaiToolBox/VideoProList.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys,os
 sys.path.append(r"D:\OneDrive - pku.edu.cn\000 Doing\DataFlux")
 
 import cv2
 import paddlehub as hub
-from VideoPro import *
+from .VideoPro import *
 import imageio
-import opencv_Functions as cvFun
+from .opencv_Functions import *
 
 class process():
     def __init__(self,_path,_videos,_Times,_Cliplist):
         self.path=_path
         self.videos=_videos
         self.Times=_Times
         self.Cliplist=_Cliplist
@@ -87,14 +87,28 @@
 
 def GetCapture(path,videos,Times,Cliplist):
     frames, _ = GetFrameIndex2(Cliplist, videos, Times)
     #frames, _ = GetFrameIndex2(Cliplist, videos, 25*60*Times)
     #frames, _ = GetFrameIndex2(Cliplist, videos, 25*Times)
     outpath = os.path.dirname(path[0]) + '\\Capture\\'
     #outpath=r'G:\ConvecDiss in CloseSys\Test\2022.11.18 WaterBulk\Capture\\'
+    if not os.path.exists(outpath):
+        os.makedirs(outpath)
+    i = 0
+    for fr in frames:
+        #cv2.imwrite(outpath+'t='+str(i*Times)+' min.jpg',fr)
+        cv_imsave(fr,outpath+'t='+str(i*Times)+' s','.jpg')#
+        i += 1
+
+def GetCapture(path,videos,Times,Cliplist):
+    frames, _ = GetFrameIndex2(Cliplist, videos, Times)
+    #frames, _ = GetFrameIndex2(Cliplist, videos, 25*60*Times)
+    #frames, _ = GetFrameIndex2(Cliplist, videos, 25*Times)
+    outpath = os.path.dirname(path[0]) + '\\Capture\\'
+    #outpath=r'G:\ConvecDiss in CloseSys\Test\2022.11.18 WaterBulk\Capture\\'
     if not os.path.exists(outpath):
         os.makedirs(outpath)
     i = 0
     for fr in frames:
         #cv2.imwrite(outpath+'t='+str(i*Times)+' min.jpg',fr)
         cv_imsave(fr,outpath+'t='+str(i*Times)+' s','.jpg')#
         i += 1
```

### Comparing `ShuaiToolBox-1.1.1/ShuaiToolBox/cv_plugin.py` & `ShuaiToolBox-1.1.2/ShuaiToolBox/cv_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import cv2
 import numpy as np
 
-
 def cv_imread(img_path):
     cv_img = cv2.imdecode(np.fromfile(img_path, dtype=np.uint8), -1)
     #cv_img = cv2.cvtColor(cv_img, cv2.COLOR_RGB2BGR)
     return cv_img
 
 def cv_imsave(image, img_path, img_ext):
     # img_ext: .jpg/.png
```

### Comparing `ShuaiToolBox-1.1.1/ShuaiToolBox/cv_vdopro.py` & `ShuaiToolBox-1.1.2/ShuaiToolBox/cv_vdopro.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import cv_plugin
-from py_plugin import *
+from .py_plugin import *
 
 import operator
 import cv2
 import time
 import os
```

### Comparing `ShuaiToolBox-1.1.1/ShuaiToolBox/opencv_Functions.py` & `ShuaiToolBox-1.1.2/ShuaiToolBox/opencv_Functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import cv2
 import imageio
-#import ffmpeg
-import numpy as np
 import copy
-from cv_plugin import *
+from .cv_plugin import *
 
 
 def GetIndex(Framelist,Clip,space):
 
     _start=Clip[0]
     _end=Clip[1]
     _startInd=Clip[2]
@@ -167,14 +164,39 @@
         video = cv2.VideoWriter(path, cv2.VideoWriter_fourcc('P', 'I', 'M', 'I'), fps, size)
     elif format == '.avi':
         video = cv2.VideoWriter(path, cv2.VideoWriter_fourcc('X', 'V', 'I', 'D'), fps, size)
 
     return video
 
 
+# ---------------------------Image process Alogo.----------------------------------------------------------------
+
+def rotateImg(img):
+    imgInfo = img.shape
+    height= imgInfo[0]
+    width = imgInfo[1]
+    deep = imgInfo[2]
+    matRotate = cv2.getRotationMatrix2D((width*0.5, height*0.5), 0, 180) # 旋转变化矩阵
+    dst = cv2.warpAffine(img, matRotate, (width,height))  #旋转
+    return dst
+
+def evenLight(img,size,channel='gray'):
+    clahe = cv2.createCLAHE(clipLimit=5, tileGridSize=(size,size))
+    gray=[]
+    if channel=='h' or channel=='s' or channel=='v':
+        hsv=cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
+        h,s,v=cv2.split(hsv)
+        exec('gray = clahe.apply('+channel+')')
+    elif channel=='b' or channel=='g' or channel=='r':
+        b,g,r=cv2.split(img)
+        exec('gray = clahe.apply('+channel+')')
+    else:
+        gray=cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+    return gray
+
 
 # import ffmpeg
 # import numpy
 # import cv2
 # import sys
 # import random
 #
```

### Comparing `ShuaiToolBox-1.1.1/ShuaiToolBox/py_plugin.py` & `ShuaiToolBox-1.1.2/ShuaiToolBox/py_plugin.py`

 * *Files identical despite different names*

