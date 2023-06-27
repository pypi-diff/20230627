# Comparing `tmp/SimpliPyTEM-1.0.5.tar.gz` & `tmp/SimpliPyTEM-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpliPyTEM-1.0.5.tar", last modified: Mon Apr 17 09:37:50 2023, max compression
+gzip compressed data, was "SimpliPyTEM-1.0.6.tar", last modified: Tue Jun 27 15:39:05 2023, max compression
```

## Comparing `SimpliPyTEM-1.0.5.tar` & `SimpliPyTEM-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-04-17 09:37:50.541139 SimpliPyTEM-1.0.5/
--rw-r--r--   0 gabriel    (501) staff       (20)    35149 2023-01-20 17:02:41.000000 SimpliPyTEM-1.0.5/LICENSE
--rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-04-17 09:37:50.540743 SimpliPyTEM-1.0.5/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)     2373 2023-04-03 10:12:55.000000 SimpliPyTEM-1.0.5/README.md
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-04-17 09:37:50.525413 SimpliPyTEM-1.0.5/SimpliPyTEM/
--rw-r--r--   0 gabriel    (501) staff       (20)    10120 2023-04-04 10:53:05.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/App_functions.py
--rw-r--r--   0 gabriel    (501) staff       (20)    85128 2023-04-03 08:57:45.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/MicroVideo_class.py
--rw-r--r--   0 gabriel    (501) staff       (20)    71639 2023-04-03 08:57:45.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Micrograph_class.py
--rw-r--r--   0 gabriel    (501) staff       (20)     3320 2023-03-20 17:44:55.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Motion_correction.py
--rw-r--r--   0 gabriel    (501) staff       (20)     7567 2023-04-17 09:25:52.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/PDF_generator.py
--rw-r--r--   0 gabriel    (501) staff       (20)    18705 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_analysis.py
--rw-r--r--   0 gabriel    (501) staff       (20)     4875 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_tracking.py
--rwxr-xr-x   0 gabriel    (501) staff       (20)    22560 2023-04-17 09:11:44.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/SimpliPyTEM_GUI.py
--rw-r--r--   0 gabriel    (501) staff       (20)     7182 2023-03-20 17:44:55.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/html_writer.py
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-04-17 09:37:50.540197 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/
--rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)      517 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel    (501) staff       (20)        1 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       69 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/entry_points.txt
--rw-r--r--   0 gabriel    (501) staff       (20)      166 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/requires.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       12 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/top_level.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       38 2023-04-17 09:37:50.541262 SimpliPyTEM-1.0.5/setup.cfg
--rw-r--r--   0 gabriel    (501) staff       (20)     2106 2023-04-17 09:34:20.000000 SimpliPyTEM-1.0.5/setup.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-06-27 15:39:05.533205 SimpliPyTEM-1.0.6/
+-rw-r--r--   0 gabriel    (501) staff       (20)    35149 2023-01-20 17:02:41.000000 SimpliPyTEM-1.0.6/LICENSE
+-rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-06-27 15:39:05.532871 SimpliPyTEM-1.0.6/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)     2373 2023-04-03 10:12:55.000000 SimpliPyTEM-1.0.6/README.md
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-06-27 15:39:05.524594 SimpliPyTEM-1.0.6/SimpliPyTEM/
+-rw-r--r--   0 gabriel    (501) staff       (20)     4267 2023-05-24 11:02:21.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/App_functions.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    88246 2023-05-31 17:12:48.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/MicroVideo_class.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    74806 2023-06-26 13:33:53.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Micrograph_class.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     3407 2023-05-23 12:31:46.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Motion_correction.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     7491 2023-05-23 12:31:57.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/PDF_generator.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    19160 2023-06-08 16:26:21.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_analysis.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     4836 2023-05-23 12:31:57.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_tracking.py
+-rwxr-xr-x   0 gabriel    (501) staff       (20)    27247 2023-06-07 15:24:10.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/SimpliPyTEM_GUI.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     7463 2023-06-07 15:23:27.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/html_writer.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-06-27 15:39:05.532416 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/
+-rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)      517 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)        1 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       69 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/entry_points.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)      276 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/requires.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       12 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/top_level.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       38 2023-06-27 15:39:05.533303 SimpliPyTEM-1.0.6/setup.cfg
+-rw-r--r--   0 gabriel    (501) staff       (20)     2216 2023-05-24 11:37:38.000000 SimpliPyTEM-1.0.6/setup.py
```

### Comparing `SimpliPyTEM-1.0.5/LICENSE` & `SimpliPyTEM-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.5/PKG-INFO` & `SimpliPyTEM-1.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpliPyTEM
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package to simplify the processing and analysis of TEM and in situ TEM images and videos
 Home-page: https://github/gabriel-ing/Micrograph-analysis-scripts
 Author: Gabriel Ing
 Author-email: ucbtgrb@ucl.ac.uk
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SimpliPyTEM-1.0.5/README.md` & `SimpliPyTEM-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/MicroVideo_class.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/MicroVideo_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1270 +1,1374 @@
-import cv2 as cv
-import ncempy.io as nci
+import argparse
 import os
+import subprocess as sb
+import time
+from copy import deepcopy
+
 import cv2 as cv
+import matplotlib.animation as animation
 import matplotlib.pyplot as plt
-from matplotlib import font_manager
-from PIL import Image, ImageOps, ImageFont, ImageDraw, ImageFilter
-import numpy as np 
-import time
-import argparse
 import mrcfile
-import subprocess as sb
+import ncempy.io as nci
+import numpy as np
+import pandas as pd
 import tifffile
-from copy import deepcopy
+from matplotlib import font_manager
 from moviepy.editor import ImageSequenceClip
-from SimpliPyTEM.Micrograph_class import *
-import matplotlib.animation as animation
-import pandas as pd
+from PIL import Image, ImageDraw, ImageFilter, ImageFont, ImageOps
 
+from SimpliPyTEM.Micrograph_class import Micrograph, default_image_pipeline, make_outdir
 
 plt.gray()
 
-class MicroVideo: 
-    '''
-    A class holding video data and various methods to edit the frames. 
+
+class MicroVideo:
+    """
+    A class holding video data and various methods to edit the frames.
 
     Attributes
     ----------
     filename:str
         The file name opened (blank if not opened in object)
     pixel_size:float
         The pixel size in the image, should be initialised when opening data assuming the pixel size is included, if not can easily be altered
     pixel_unit:str
         The unit of the pixel size
     metadata_tags:dict
         The metadata of the file should be stored in this dictionary (works with digital micrograph files)
     shape:tuple
-        The shape of the video (nframes, y, x) 
+        The shape of the video (nframes, y, x)
     x:int
         The size of the x axis in the image
-    y:int    
+    y:int
         The size of the y axis in the image
     frames:numpy array
         The video data
 
-
     List of functions in MicroVideo
     -------------------------------
     Imports:
         open_dm - Opening digital micrograph files
-
         open_video - Opening a .mp4 or .avi video files
-
         open_array - Loading a numpy array
-
     Saving:
         save_tif_stack
-
         save_tif_sequence
-
         write_video - save .mp4 or .avi version of the video
-
         write_image - save video frame or video average as an image
-
     Basic functions:
         bin - reduce size of xy axis by binning pixels, factor is specified in call
-
         convert_to_8bit - converts to 8bit video by scaling pixel values between 0-255.
-
         make_scalebar - creates suitably sized scalebar
-
         Average_frames - averages frames in groups of n
-
         Running_average - performs a running average of the video
-
         reset_xy - reset the object x, y and shape attributes upon change of video, useful if video is cropped.
-
     Contrast enhancement:
         clip_contrast - enhances contrast by making a percentage of values saturated (absolute black/white) and scaling the rest of the pixels between these (my preferred contrast enhancement)
-
         enhance_contrast - enhances contrast based on alpha (contrast), beta (brightness) and gamma (non-linear contrast) values
-
         eqHist - equalises histogram, ensuring even converage of pixel values from 0-255
-
         Normalise_video - normalises contrast between frames of the video
-
     Metadata (currently relies on dm3/dm4 metadata):
         show_metadata - shows all metadata tags and values
-
         get_mag - prints and returns magnification (indicated and actual)
-
         get_voltage - prints and returns voltage
-
         get_exposure - prints and returns frame rate, exposure time
-
         get_date_time - prints aquisition date and time
-
     Image filters:
         gaussian_filter
-
         median_filter
-
         low_pass_filter
-
         weiner_filter
-
         non_local_means_filter
-
     Plotting:
         imshow - plots still image (either single frame or average) of video
-
         plot_histogram - plots the histogram of the video
-
         show_video - shows video in a jupyter notebook (very slow)
-
     Other functions:
         Sidebyside - Sticks two videos together so they play side by side.
-
         motioncorrect_vid - Uses motioncor2 to align the video frames (requires motioncor exectutable to be set)
 
-        
 
 
-    '''
+
+    """
+
     def __init__(self, filename=None):
-        if filename: 
+        if filename:
             self.log = []
-            self.video=True
-            self.pixel_size= 1
-            self.pixel_unit = 'pixels'
+            self.video = True
+            self.pixel_size = 1
+            self.pixel_unit = "pixels"
             self.filename = filename
             self.open_file(filename)
         else:
-            self.filename = ''
-            #self.image='Undefined'
-            self.pixel_size= 1
-            self.pixel_unit = 'pixels'
+            self.filename = ""
+            # self.image='Undefined'
+            self.pixel_size = 1
+            self.pixel_unit = "pixels"
             self.log = []
-            self.video=True
-        '''-------------------------------------------------------------------------------------------------------------------------------------------
+            self.video = True
+        """-------------------------------------------------------------------------------------------------------------------------------------------
         SECTION: IMPORT IMAGES
 
             can be imported as dm3, dm4, mrc, **numpy array or tifs ** add the tifs 
             need to add numpy and tif functionality
 
 
-        '''
-    
+        """
 
     def open_dm(self, file, pixelcorrection=True):
-        '''
-        Imports digital micrograph files into the micrograph object, initialising all the default attributes required, including saving the metadata into self.metadata_tags. 
-        By default, video dm files (dose fractionations) will be summed to create a single image file, there is also an option (video_average) to use the first frame only. 
-        
+        """
+        Imports digital micrograph files into the micrograph object, initialising all the default attributes required, including saving the metadata into self.metadata_tags.
+        By default, video dm files (dose fractionations) will be summed to create a single image file, there is also an option (video_average) to use the first frame only.
+
         Some DM files have 'hot pixels' which have anomalously high signal due to detector malfunction, these often lead to contrast issues.
         To correct for this any pixel which has a higher value than the mean value + (20 x standard deviation) is set to the mean pixel value, this is on by default but can be turned off using pixel_correction=False
-        
+
         This uses the ncempy.io.dm package to read DM files, more information can be found here: https://openncem.readthedocs.io/en/latest/ncempy.io.html
 
 
         Parameters
         ----------
             file : str
-                The name of the dm file to open. The path to the file can also be included if it is not in the same directory. 
+                The name of the dm file to open. The path to the file can also be included if it is not in the same directory.
 
-            pixel_correction: bool 
-                Set anomalous 'hot' pixels to the image mean, anomalous pixels defined as image_mean + 20*image_standard_deviation. Default is on (True). 
+            pixel_correction: bool
+                Set anomalous 'hot' pixels to the image mean, anomalous pixels defined as image_mean + 20*image_standard_deviation. Default is on (True).
 
-        '''
+        """
         dm_input = nci.dm.dmReader(file)
-        #if len(dm_input['data'].shape)==2:
+        # if len(dm_input['data'].shape)==2:
         #    image = dm_input['data']
         #    dm = '_Image_'
 
         # at the moment it automatically averages a video into a single image. This will be changed soon to allow for video analysis.
-        if len(dm_input['data'].shape)==3:
-            self.frames = dm_input['data']
-            #image = np.average(images, axis=0)
-            dm='_Video_'
-        else:
-            print('Error, {} is not a video, consider using Micrograph() class unless you are running open_series'.format(file))
+        if len(dm_input["data"].shape) == 3:
+            self.frames = dm_input["data"]
+            # image = np.average(images, axis=0)
+            dm = "_Video_"
+        else:
+            print(
+                "Error, {} is not a video, consider using Micrograph() class unless you are running open_series".format(
+                    file
+                )
+            )
         dmfile = nci.dm.fileDM(file)
-        self.metadata_tags =dmfile.allTags
-        if '.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Frame Exposure' in self.metadata_tags:
-            self.fps = 1/float(self.metadata_tags['.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Frame Exposure']) 
-        #extract x and y shapes
+        self.metadata_tags = dmfile.allTags
+        if (
+            ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Frame Exposure"
+            in self.metadata_tags
+        ):
+            self.fps = 1 / float(
+                self.metadata_tags[
+                    ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Frame Exposure"
+                ]
+            )
+        # extract x and y shapes
         self.x = self.frames[0].shape[1]
         self.y = self.frames[0].shape[0]
 
-        pixel_size=float(dm_input['pixelSize'][-1])
-        #print(type(pixel_size))
-        #print(pixel_size,type(pixel_size))
-        pixel_unit = dm_input['pixelUnit'][-1]
+        pixel_size = float(dm_input["pixelSize"][-1])
+        # print(type(pixel_size))
+        # print(pixel_size,type(pixel_size))
+        pixel_unit = dm_input["pixelUnit"][-1]
         self.filename = file
-        self.pixel_size= pixel_size
+        self.pixel_size = pixel_size
         self.pixel_unit = pixel_unit
-        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default. 
-        #This line removes any giant outliers (bright pixels) from the images
-        #print(self.frames[self.frames>self.frames.mean()+self.frames.std()*50])
-        
-        #self.frames = np.flip(self.frames,axis=1)
+        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default.
+        # This line removes any giant outliers (bright pixels) from the images
+        # print(self.frames[self.frames>self.frames.mean()+self.frames.std()*50])
+
+        # self.frames = np.flip(self.frames,axis=1)
         if pixelcorrection:
-            self.frames[self.frames>self.frames.mean()+self.frames.std()*8]=0
-        
-        self.frames=  self.frames.astype('float32')
-        #for frame in self.frames:
+            self.frames[self.frames > self.frames.mean() + self.frames.std() * 8] = 0
+
+        self.frames = self.frames.astype("float32")
+        # for frame in self.frames:
         #    frame = frame.astype('float32')
         self.shape = self.frames.shape
-        print(file + ' opened as a MicroVideo object')
+        print(file + " opened as a MicroVideo object")
 
-#       #return image, x, y, pixel_size, pixel_unit
+    #       #return image, x, y, pixel_size, pixel_unit
 
     def open_mrc(self, file):
-        mrc= mrcfile.open(file)
+        mrc = mrcfile.open(file)
         print(mrc.voxel_size)
         voxel_size = mrc.voxel_size
 
-        self.pixel_size = float(str(voxel_size).split(',')[0].strip('('))
+        self.pixel_size = float(str(voxel_size).split(",")[0].strip("("))
         self.frames = mrc.data
         self.frames.setflags(write=1)
         self.frames = np.flip(self.frames, axis=1)
 
         self.x = self.frames.shape[1]
         self.y = self.frames.shape[0]
-        self.pixel_unit='nm'
+        self.pixel_unit = "nm"
         self.filename = file
 
-        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default. 
+        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default.
         for frame in self.frames:
-            frame = frame.astype('float32')
+            frame = frame.astype("float32")
 
-    def open_video(self, filename,pixel_size=1,pixel_unit='pixels',):
-        '''
+    def open_video(
+        self,
+        filename,
+        pixel_size=1,
+        pixel_unit="pixels",
+    ):
+        """
         Loads video files (eg. mp4 and avi, unsure if others will work) into microvideo object.
         The pixel size is not taken from the video by default, and so it should be included in the command, else the default of 1nm/pixel is used. This can be addedd later using video.pixel_size= {new pixel size}
-        
+
         Parameters
         ----------
 
             filename: str
                 Name of the video file to open
             pixel_size: float
                 Size of one pixel (eg. 1nm/pixel), optionall.
             pixel_unit: str
                 Unit for the pixel_size
 
-        '''
+        """
 
         cap = cv.VideoCapture(filename)
-        frames= []
-        self.filename = '.'.join(filename.split('.')[:-1])
+        frames = []
+        self.filename = ".".join(filename.split(".")[:-1])
         while cap.isOpened():
-            ret, frame =cap.read()
-            
-            #print(ret, frame)
+            ret, frame = cap.read()
+
+            # print(ret, frame)
             if not ret:
                 print("Can't receive frame (stream end?). Exiting ...")
                 break
-            #print(frame.shape)
+            # print(frame.shape)
             frame = cv.cvtColor(frame, cv.COLOR_BGR2GRAY)
-            #plt.imshow(frame)
-            #cv.imshow('frame',frame)
-            if cv.waitKey(1)==ord('q'):
+            # plt.imshow(frame)
+            # cv.imshow('frame',frame)
+            if cv.waitKey(1) == ord("q"):
                 break
             frames.append(frame)
-            #print(len(frames))
+            # print(len(frames))
         self.frames = np.array(frames)
-        print('{} frames loaded as micrograph object'.format(len(self.frames)))
-        print('As format is avi, the pixelsize is not loaded automatically, please set this using micrograph.pixel_size = n')
+        print("{} frames loaded as micrograph object".format(len(self.frames)))
+        print(
+            "As format is avi, the pixelsize is not loaded automatically, please set this using micrograph.pixel_size = n"
+        )
         cap.release()
         self.reset_xy()
-        self.pixel_size=pixel_size
-        self.pixel_unit=pixel_unit
-
-
-
+        self.pixel_size = pixel_size
+        self.pixel_unit = pixel_unit
 
-    def open_array(self, arr, pixelsize=1,pixelunit='nm', filename='Loaded_array'):
-        '''
+    def open_array(self, arr, pixelsize=1, pixelunit="nm", filename="Loaded_array"):
+        """
         Loads a numpy array into the microvideo object, allowing use of all the other available methods. Filename, pixel size and pixel unit should be given in the call, defaults of 1nm/pixel allow this to be avoided but correct pixel size should be loaded if a scalebar is required (as well as certain other functions)
-        
-        '''
+
+        """
         print(arr.shape)
-        if len(arr.shape)!=3:
-            print('Error, this doesnt appear to be an image stack, please double check!')
-            return 1 
-
-        self.frames = arr 
-        self.pixel_size=pixelsize
-        self.pixel_unit=pixelunit
-        self.filename=filename
+        if len(arr.shape) != 3:
+            print(
+                "Error, this doesnt appear to be an image stack, please double check!"
+            )
+            return 1
+
+        self.frames = arr
+        self.pixel_size = pixelsize
+        self.pixel_unit = pixelunit
+        self.filename = filename
         self.reset_xy()
 
-       
     def open_series(self, frames):
-        '''
-        Hasn't exactly been tested but should work! 
-        '''
+        """
+        Hasn't exactly been tested but should work!
+        """
         self.open_dm(frame[0])
         new_frames = []
         for frame in frames[1:]:
             next_frame = nci.dm.dmReader(frame)
             new_frames.append(next_frame)
         self.frames = np.array(new_frames)
 
     def open_file(self, filename):
-        if filename[-4:]=='.dm3' or filename[-4:]=='.dm4':
+        if filename[-4:] == ".dm3" or filename[-4:] == ".dm4":
             self.open_dm(filename)
-        elif filename[-4:]=='.mrc':
+        elif filename[-4:] == ".mrc":
             self.open_mrc(filename)
         else:
             self.open_video(filename)
 
     def reset_xy(self):
-        '''
+        """
         Resets the image attributes for the x, y and shape of the image. Used by the binning method and is also useful following cropping of the micrograph
 
-        '''
+        """
         self.x = self.frames[0].shape[1]
         self.y = self.frames[0].shape[0]
         self.shape = self.frames.shape
 
-
-    '''-----------------------------------------------------------
+    """-----------------------------------------------------------
 
     SECTION: SAVING
 
 
 
-    '''
+    """
+
     def save_tif_stack(self, name=None, outdir=None):
-        '''
+        """
         Saves the video as a single, multi-image tif file (stack). Files saved in current condition so if an 8bit tif is required, run video.convert_to_8bit() before use.
         These can be useful for viewing editted video in imageJ
-        
+
         Parameters
         ----------
             name:str
                 Prefix for the outputted filename.
 
             outdir:str
                 The output directory for the files, if this directory doesn't exist (in the cwd) a new one will be created.
 
         Outputs
         -------
 
             Saves a multi-image tif stack into the output directory listed (cwd is default)
 
-        '''
+        """
 
         if name:
-            if name[-4:]!='.tif':
-                name+='.tif'        
+            if name[-4:] != ".tif":
+                name += ".tif"
         else:
-            name = '.'.join(self.filename.split('.')[:-1])+'.tif'    
-        
-        if pixel_unit!='nm':
-            pu = 'um'
-        else:
-            pu='nm'
+            name = ".".join(self.filename.split(".")[:-1]) + ".tif"
 
+        if self.pixel_unit != "nm":
+            pu = "um"
+        else:
+            pu = "nm"
 
         if outdir:
             make_outdir(outdir)
-            name = outdir+'/'+name
-        tifffile.imsave(name, self.frames,imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':pu})
-
+            name = outdir + "/" + name
+        tifffile.imsave(
+            name,
+            self.frames,
+            imagej=True,
+            resolution=(1 / self.pixel_size, 1 / self.pixel_size),
+            metadata={"unit": pu},
+        )
 
     def save_tif_sequence(self, name=None, outdir=None):
-        '''        
+        """
         Saves each frame of the video as a tif, this is saved in the current format, so if an 8bit tif is required, run video.convert_to_8bit() before use.
-        nameand outdir can be included to give a name (prefix) and  the output directory. 
-        
+        nameand outdir can be included to give a name (prefix) and  the output directory.
+
         Parameters
         ----------
             name:str
                 Prefix for the outputted filenames.
 
             outdir:str
                 The output directory for the files, if this directory doesn't exist (in the cwd) a new one will be created.
 
         Outputs
         -------
 
             Saves a sequence of Tif files into the output directory listed (cwd is default)
 
-        '''
+        """
         if name:
-            if name[-4:]=='.tif':
-                name= name.strip('.tif')
-        else: 
-            name = '.'.join(self.filename.split('.')[:1]) 
+            if name[-4:] == ".tif":
+                name = name.strip(".tif")
+        else:
+            name = ".".join(self.filename.split(".")[:1])
 
         if outdir:
             make_outdir(outdir)
-            name = outdir+'/'+name
+            name = outdir + "/" + name
 
-        if self.pixel_unit!='nm':
-            pu = 'um'
+        if self.pixel_unit != "nm":
+            pu = "um"
         else:
-            pu='nm'
+            pu = "nm"
 
         for i in range(len(self.frames)):
-            j=4-len(str(i))
-            zeros = '0000'
-            count = str(zeros[:j])+str(i)
-            savename = name+'_{}'.format(count)+'.tif'
-            tifffile.imsave(savename, self.frames[i],imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':pu, 'Labels':'{}/{} -{}'.format(i, len(self.frames),self.filename)})
-
-    def save_gif(self, fps=5,**kwargs ):
-
-        if 'name' in kwargs:
-            name = kwargs['name']
-            if name[-4:]!='.gif':
-                name= name+'.gif'
-        else: 
-            name = '.'.join(self.filename.split('.')[:1])+'.gif' 
-
-        if 'outdir' in kwargs:
-            outdir = str(kwargs['outdir'])
-            if outdir not in os.listdir('.') and outdir!='.':
+            j = 4 - len(str(i))
+            zeros = "0000"
+            count = str(zeros[:j]) + str(i)
+            savename = name + "_{}".format(count) + ".tif"
+            tifffile.imsave(
+                savename,
+                self.frames[i],
+                imagej=True,
+                resolution=(1 / self.pixel_size, 1 / self.pixel_size),
+                metadata={
+                    "unit": pu,
+                    "Labels": "{}/{} -{}".format(i, len(self.frames), self.filename),
+                },
+            )
+
+    def save_gif(self, fps=5, **kwargs):
+        if "name" in kwargs:
+            name = kwargs["name"]
+            if name[-4:] != ".gif":
+                name = name + ".gif"
+        else:
+            name = ".".join(self.filename.split(".")[:1]) + ".gif"
+
+        if "outdir" in kwargs:
+            outdir = str(kwargs["outdir"])
+            if outdir not in os.listdir(".") and outdir != ".":
                 os.mkdir(outdir)
-            name = outdir+'/'+name
+            name = outdir + "/" + name
 
         from moviepy.editor import ImageSequenceClip
-        arr = video.frames    
+
+        arr = video.frames
         arr = np.expand_dims(arr, 3)
         clip = ImageSequenceClip(list(arrex), fps=fps)
         clip.to_videofile(name, fps)
-    
 
     def write_video(self, name=None, outdir=None, fps=None):
-        '''
+        """
         This allows saving as an mp4 or a raw avi file (imageJ compatible)
 
         Parameters
         ----------
             name:str
-                Output filename. Outputted files can be in mp4 or uncompressed avi (imageJ readable) filetypes (mp4 by default), this is denoted by the suffix of the name. 
+                Output filename. Outputted files can be in mp4 or uncompressed avi (imageJ readable) filetypes (mp4 by default), this is denoted by the suffix of the name.
 
             outdir:str
                 The output directory for the files, if this directory doesn't exist (in the cwd) a new one will be created.
 
             fps:int
                 Optionally the output movie frame rate can be added (in frames per second)
         Outputs
         -------
 
             Saves a sequence of Tif files into the output directory listed (cwd is default)
-        '''    
+        """
         if name:
-            #name = kwargs['name']
-            if name[-4:]!='.mp4' and name[-4:]!='.avi':
-                name= name+'.mp4'
-                outformat='mp4'
-            elif name[-4:]=='.avi':
-                outformat = 'avi'   
+            # name = kwargs['name']
+            if name[-4:] != ".mp4" and name[-4:] != ".avi":
+                name = name + ".mp4"
+                outformat = "mp4"
+            elif name[-4:] == ".avi":
+                outformat = "avi"
             else:
-                outformat='.mp4'    
-        else: 
-            name = '.'.join(self.filename.split('.')[:-1])+'.mp4' 
-            outformat='mp4'
+                outformat = ".mp4"
+        else:
+            name = ".".join(self.filename.split(".")[:-1]) + ".mp4"
+            outformat = "mp4"
 
         if outdir:
             make_outdir(outdir)
-            name = outdir+'/'+name
-        
-        if not fps and hasattr(self,'fps'):
-            fps= self.fps    
+            name = outdir + "/" + name
+
+        if not fps and hasattr(self, "fps"):
+            fps = self.fps
         elif not fps:
-            fps=10
+            fps = 10
 
         outvid = []
         for frame in self.frames:
             frame = cv.cvtColor(frame, cv.COLOR_GRAY2BGR)
             outvid.append(frame)
         outvid = np.array(outvid)
-        
+
         clip = ImageSequenceClip(list(outvid), fps=fps)
-        #print(clip)
-        if outformat=='avi':
-            clip.write_videofile(name,codec='rawvideo', fps=fps)
+        # print(clip)
+        if outformat == "avi":
+            clip.write_videofile(name, codec="rawvideo", fps=fps)
         else:
             clip.write_videofile(name, fps=fps)
-                
-    def write_image(self, name=None, ftype='jpg', average=True, framenumber=0, outdir=None):
-        '''
-        Saves the image in a .jpg or .tif file for display or use with other programs. 
+
+    def write_image(
+        self, name=None, ftype="jpg", average=True, framenumber=0, outdir=None
+    ):
+        """
+        Saves the image in a .jpg or .tif file for display or use with other programs.
 
         Parameters
         ----------
             name: str
-                Filename for saved image. Ending with either .jpg or .tif will define the format of the image, alternatively ftype argument can be used. 
-                This is optional, without including a name the name of the original file opened will be used. 
+                Filename for saved image. Ending with either .jpg or .tif will define the format of the image, alternatively ftype argument can be used.
+                This is optional, without including a name the name of the original file opened will be used.
 
             ftype: str
-                Optional. Filetype of output image, either 'jpg' or 'tif' (default jpg), this is better defined using the suffix of the name. 
+                Optional. Filetype of output image, either 'jpg' or 'tif' (default jpg), this is better defined using the suffix of the name.
                 Saving as a tif will save in whatever format it is currently in - this can be a 32-bit or 8-bit image, using convert_to_8bit() will ensure that latter.
 
             outdir: str
                 Keyword argument (usage: outdir='/path/to/directory'). This defines the output location of the saved image, use a path relative to the current directory or an absolute path.
                 The final directory in the path will be made if it does not already exist.
-            
+
             average:bool
                 Do you want to save an image of the average of the video? True or False (y/n)
 
             framenumber:int
                 If not saving the average (average=False), this chooses which frame to save - index starts at zero and negative numbers count from the end
 
-        '''
-
+        """
 
         if outdir:
             make_outdir(outdir)
-            name =outdir+'/'+name    
-        print('Start name :', name)
+            name = outdir + "/" + name
+        print("Start name :", name)
         if name:
-                print('if name : ',name)
-                if name[-4:]=='.jpg':
-                    ftype='jpg'
-                    name=name[:-4]
-                elif name[-4:]=='.tif':
-                    ftype='tif' 
-                    name = name[:-4]   
-                if len(name.split('.'))>2:
-                    name='.'.join(name.split('.')[:-1])
-                    print('if len name: ', name)
-                    print('.'.join(name.split('.')[:-1]))
-        else:
-                name = '.'.join(self.filename.split('.')[:-1])
-                print('else_name = ',name)
-        #try:
+            print("if name : ", name)
+            if name[-4:] == ".jpg":
+                ftype = "jpg"
+                name = name[:-4]
+            elif name[-4:] == ".tif":
+                ftype = "tif"
+                name = name[:-4]
+            if len(name.split(".")) > 2:
+                name = ".".join(name.split(".")[:-1])
+                print("if len name: ", name)
+                print(".".join(name.split(".")[:-1]))
+        else:
+            name = ".".join(self.filename.split(".")[:-1])
+            print("else_name = ", name)
+        # try:
         #    name += '_'+self.scalebar_size+'scale.{}'.format(ftype)
-        #except AttributeError:
-        name+='.'+ftype
-        #if self.foldername!='':
+        # except AttributeError:
+        name += "." + ftype
+        # if self.foldername!='':
         #        name = '/'+self.foldername.strip('/n') + '/' + name.split('/')[-1]
-        #if self.foldername=='':
+        # if self.foldername=='':
         #    newname = self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
-        #else:
+        # else:
         #    newname = self.foldername.strip('\n') + '/' +self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
         if average:
             image = np.sum(self.frames, axis=0)
 
         else:
             image = self.frames[framenumber]
 
-        if ftype=='jpg':
-            if image.max()!=255 or image.min()!=0:
+        if ftype == "jpg":
+            if image.max() != 255 or image.min() != 0:
                 print(image.max(), image.min())
-                image= (image - image.min())*(1/(image.max()-image.min())*255)
-                image = image.astype('uint8')
-                print('converting to 8bit')
-            cv.imwrite(name,image)
-        elif ftype=='tif':
-            tifffile.imsave(name, image,imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':self.pixel_unit})
+                image = (image - image.min()) * (1 / (image.max() - image.min()) * 255)
+                image = image.astype("uint8")
+                print("converting to 8bit")
+            cv.imwrite(name, image)
+        elif ftype == "tif":
+            tifffile.imsave(
+                name,
+                image,
+                imagej=True,
+                resolution=(1 / self.pixel_size, 1 / self.pixel_size),
+                metadata={"unit": self.pixel_unit},
+            )
 
-        #self.pil_image.save(name, quality=self.quality)
-        print(name, 'Done!')
+        # self.pil_image.save(name, quality=self.quality)
+        print(name, "Done!")
+
+    def write_mrc(self, name=None, outdir=None, overwrite=False):
+        """
+        Function to save video as an mrc file. Currently Metadata is not supported.
+        """
+
+        if name:
+            # print('if name : ',name)
+            if len(name.split(".")) > 2:
+                name = ".".join(name.split(".")[:-1])
+                print(".".join(name.split(".")[:-1]))
+        else:
+            name = ".".join(self.filename.split(".")[:-1])
+
+        if name[-4:] != ".mrc":
+            name += ".mrc"
+
+        if outdir:
+            make_outdir(outdir)
+            name = outdir + "/" + name
+
+        with mrcfile.new(name, overwrite=overwrite) as mrc:
+            mrc.set_data(self.frames)
 
     def toMicrograph(self):
-        '''
+        """
         Returns a micrograph object with the average of the image so the video average can be treated as a single image
-        
+
         Returns
         -------
 
             micrograph:Micrograph
                 Micrograph object with the same metadata and an average of all the image frames.
 
-        '''
+        """
         im = Micrograph()
         for key in self.__dict__.keys():
-            if key!= 'frames':
+            if key != "frames":
                 setattr(im, key, self.__dict__[key])
         im.image = np.sum(self.frames, 0)
         return im
-        '''-----------------------------------------------------------------------------------------------------------------------
+        """-----------------------------------------------------------------------------------------------------------------------
         SECTION: BASIC FUNCTIONS
 
             add_frames : this sums all the frames of a video together if the frames are saved individually, input is a list of frames, can be generated using the group frames method in the motioncorrection section 
             convert to 8bit: this is important to create a easily openable and lower filesize output image good for viewing. 
 
 
-        '''
+        """
+
     def convert_to_8bit(self):
-        '''Returns a microvideo object with the image scaled between 0 and 255 (an 8-bit image). Improves contrast, reduces data size and is a more usable image format than higher bit rates. 
-        
+        """Returns a microvideo object with the image scaled between 0 and 255 (an 8-bit image). Improves contrast, reduces data size and is a more usable image format than higher bit rates.
+
         Returns
         -------
             MicroVideo8bit : MicroVideo
                 A copy of the microvideo object with the image scaled between 0 and 255
-        '''
+        """
         #  this will scale the pixels to between 0 and 255, this will automatically scale the image to its max and min
         vid8bit = deepcopy(self)
-        vid8bit.frames= (self.frames - self.frames.min())*(1/(self.frames.max()-self.frames.min())*255)
-        vid8bit.frames = vid8bit.frames.astype('uint8')
-        #print(self.frames.dtype)
-        #for i in range(len(self.frames)):
+        vid8bit.frames = (self.frames - self.frames.min()) * (
+            1 / (self.frames.max() - self.frames.min()) * 255
+        )
+        vid8bit.frames = vid8bit.frames.astype("uint8")
+        # print(self.frames.dtype)
+        # for i in range(len(self.frames)):
         #    self.frames[i] = ((self.frames[i] - self.frames.min()) * (1/(self.frames.max() - self.frames[i].min()) * 255)).astype('uint8')
-        vid8bit.log.append('convert_to_8bit()')
+        vid8bit.log.append("convert_to_8bit()")
         return vid8bit
-    
+
     def bin(self, value=2):
         """
         This function applies binning to the frames in a micrograph object, reducing their size by a specified factor.
-    
+
         Parameters
         ----------
         value : int
             The factor by which to reduce the size of the frames. The default value is 2.
-    
+
         Returns
         -------
         Microvideo_binned: MicroVideo
             A new microvideo object with the binned frames.
         """
-        i=0
+        i = 0
         frames = []
         for frame in self.frames:
-
-            frame = cv.resize(frame, (int(frame.shape[0]/value), int(frame.shape[1]/value)), interpolation=cv.INTER_CUBIC)
+            frame = cv.resize(
+                frame,
+                (int(frame.shape[1] / value), int(frame.shape[0] / value)),
+                interpolation=cv.INTER_CUBIC,
+            )
             frames.append(frame)
-            i+=1
+            i += 1
         binned = deepcopy(self)
-        binned.frames=np.array(frames)
-        #print(self.frames.shape)
-        binned.pixel_size= self.pixel_size*value
+        binned.frames = np.array(frames)
+        # print(self.frames.shape)
+        binned.pixel_size = self.pixel_size * value
         binned.reset_xy()
-        binned.log.append('binned()')
+        binned.log.append("binned()")
         return binned
 
-
-
-
     def clip_contrast(self, saturation=0.2, maxvalue=None, minvalue=None):
         """
-        Function for enhancing the contrast in an image by clipping the histogram between two values. 
+        Function for enhancing the contrast in an image by clipping the histogram between two values.
         These values can be defined directly or can be automatically decided using a saturation value, which the is percentage of the pixels above or below this value.
-        I.e, if there are 1,000,000 pixels in an image and the saturation value is 0.1, the method searches the value for which only 0.1% or 1000 pixels are above/below. 
+        I.e, if there are 1,000,000 pixels in an image and the saturation value is 0.1, the method searches the value for which only 0.1% or 1000 pixels are above/below.
         These values then become the new minimum and maximum of the image, and are scaled to between 0 and 255.
-        
+
         This method will automatically convert to 8 bit (scale between 0 and 255), if this is an issue raise and it can be changed in future versions.
 
         Parameters
         ----------
 
             saturation: Float
                 The percentage cutoff above/below which the pixels are set to zero/255, default is 0.5% of pixels
 
             maxvalue: int
-                The maximum value that is being clipped (to be decided from histogram). Optional. 
+                The maximum value that is being clipped (to be decided from histogram). Optional.
 
             minvalue: int
-                The minimum value that is being clipped (to be decided from histogram). Optional. 
+                The minimum value that is being clipped (to be decided from histogram). Optional.
 
         Returns
         -------
 
             Contrast_enhanced_microvideo : Microvideo
                 Return a copy of the object with the contrast clipped at either end of the image
 
         Usage
         -----
 
             MicrovideoContrastClipped = video.clip_contrast(saturation=1)
-            
-            or 
+
+            or
 
             MicrovideoContrastClipped = video.clip_contrast(maxvalue=220, minvalue=20)
 
         """
-        new_vid  = self.convert_to_8bit()
-        #print(new_vid)
-        #print(new_vid.frames)
-        
+        new_vid = self.convert_to_8bit()
+        # print(new_vid)
+        # print(new_vid.frames)
+
         if not maxvalue:
-            print('Saturation = ',saturation)
-            maxvalue=np.percentile(new_vid.frames, 100-saturation)
-            print('Maxmium value : ',maxvalue)
+            print("Saturation = ", saturation)
+            maxvalue = np.percentile(new_vid.frames, 100 - saturation)
+            print("Maxmium value : ", maxvalue)
         if not minvalue:
-            minvalue= np.percentile(new_vid.frames, saturation)
-            print('Minimum value : ',minvalue)
-        frames =new_vid.frames.astype(np.int16)    
+            minvalue = np.percentile(new_vid.frames, saturation)
+            print("Minimum value : ", minvalue)
+        frames = new_vid.frames.astype(np.int16)
         print(maxvalue, minvalue)
-        new_vid.frames = (frames - minvalue)*(255/(maxvalue-minvalue))
-        new_vid.frames[new_vid.frames>255]=255
-        new_vid.frames[new_vid.frames<0]=0
+        new_vid.frames = (frames - minvalue) * (255 / (maxvalue - minvalue))
+        new_vid.frames[new_vid.frames > 255] = 255
+        new_vid.frames[new_vid.frames < 0] = 0
         new_vid.frames = new_vid.frames.astype(np.uint8)
-        new_vid.log.append('clip_contrast()')
+        new_vid.log.append("clip_contrast()")
         return new_vid
 
-
     # This, much like the filters below returns the enhanced version as a new object, I have made it this way to allow tuning of alpha and beta.
     def enhance_contrast(self, alpha=1.3, beta=1.1, gamma=1):
-        '''
-        Function for enhancing contrast. This uses the OpenCV methods detailed here: https://docs.opencv.org/3.4/d3/dc1/tutorial_basic_linear_transform.html. 
-        There are 3 input values which define contast controls: alpha, beta and gamma, the gamma value is optional. 
-        
+        """
+        Function for enhancing contrast. This uses the OpenCV methods detailed here: https://docs.opencv.org/3.4/d3/dc1/tutorial_basic_linear_transform.html.
+        There are 3 input values which define contast controls: alpha, beta and gamma, the gamma value is optional.
+
         Parameters
         ----------
 
             alpha:float
-                Basic contrast control, usually in the range of 1-3. The histogram is streched. 
+                Basic contrast control, usually in the range of 1-3. The histogram is streched.
 
             beta: int (or float)
                 Brightness control, this will add the value to every pixel in the image, only really has an effect with 8-bit images (and any pixels above 255 will be clipped to this)
-            
+
             gamma:float
                 Non-linear contrast control, values between 0-1 makes images brighter (particularly the dark areas), while values >1 darken the image(particularly the bright areas)
-                Optional, if included image will be converted to 8 bit. 
+                Optional, if included image will be converted to 8 bit.
 
-        Returns 
+        Returns
         -------
 
             Contrast_enhanced_microvidoe : MicroVideo
                 Return a copy of the object with the contrast enhanced.
-        '''
+        """
 
         enhanced_object = deepcopy(self)
         for i in range(len(enhanced_object.frames)):
-            #print(enhanced_object.frames.dtype)
-            enhanced_object.frames[i] = cv.convertScaleAbs(enhanced_object.frames[i], alpha=alpha, beta=beta)
-
-        #print(enhanced_object.frames[0].dtype)
-        if enhanced_object.frames[i].dtype=='uint8' and gamma!=1:
-            LUT =np.empty((1,256), np.uint8)
+            # print(enhanced_object.frames.dtype)
+            enhanced_object.frames[i] = cv.convertScaleAbs(
+                enhanced_object.frames[i], alpha=alpha, beta=beta
+            )
+
+        # print(enhanced_object.frames[0].dtype)
+        if enhanced_object.frames[i].dtype == "uint8" and gamma != 1:
+            LUT = np.empty((1, 256), np.uint8)
             for i in range(256):
-                LUT[0, i]=np.clip(pow(i/255.0,gamma)*255.0, 0, 255)
-            res =cv.LUT(enhanced_object.frames, LUT) 
-            print('Gamma adjusted...')
+                LUT[0, i] = np.clip(pow(i / 255.0, gamma) * 255.0, 0, 255)
+            res = cv.LUT(enhanced_object.frames, LUT)
+            print("Gamma adjusted...")
             enhanced_object.frames = res
-        #enhanced_object.image = enhanced_image
-        enhanced_object.log.append('enhance_contrast()')
+        # enhanced_object.image = enhanced_image
+        enhanced_object.log.append("enhance_contrast()")
         return enhanced_object
 
     def eqHist(self):
-        '''
-        Spreads the contrast across complete range of values, leading to an evened, flattened histogram. This can be very effective at enhancing midtones in images with very bright or very dark patches. 
-        
+        """
+        Spreads the contrast across complete range of values, leading to an evened, flattened histogram. This can be very effective at enhancing midtones in images with very bright or very dark patches.
+
         Returns
         -------
             Contrast_enhanced_microvideo : MicroVideo
                 Return a copy of the object with the contrast enhanced.
 
-        '''
-        enhanced_object=deepcopy(self)
+        """
+        enhanced_object = deepcopy(self)
         enhanced_object = enhanced_object.convert_to_8bit()
         for i in range(len(enhanced_object.frames)):
             enhanced_object.frames[i] = cv.equalizeHist(enhanced_object.frames[i])
-        enhanced_object.log.append('eqHist()')
+        enhanced_object.log.append("eqHist()")
         return enhanced_object
 
     def __len__(self):
         return self.frames.shape[0]
 
-    def Normalise_video(self, normtype='mean'):
-        '''
+    def normalise_video(self, normtype="mean"):
+        """
         Normalises the video frames to have equal contrast, either through  mean or median normalisation
-            
+
         Parameters
         ----------
-            
+
             normtype:str
-                options are mean or median - changes the type of normalisation, either the mean of each frame  is equal or the median of each frame is equal. 
+                options are mean or median - changes the type of normalisation, either the mean of each frame  is equal or the median of each frame is equal.
 
 
         Returns
         -------
-            
+
             Normalised_microvideo: MicroVideo
                 Returns  a normalised copy of the original object.
 
-        '''
-
+        """
+        dtype = self.frames.dtype
         norm_frames = []
-        normtypes = ['median', 'mean']
+        normtypes = ["median", "mean"]
         if normtype not in normtypes:
-            raise Exception('this normalisation type is not supported, currently only median or mean are supported')
-        elif normtype=='mean':
+            raise Exception(
+                "this normalisation type is not supported, currently only median or mean are supported"
+            )
+        elif normtype == "mean":
             vid_norm = np.mean(self.frames)
-        elif normtype=='median':
+        elif normtype == "median":
             vid_norm = np.median(self.frames)
 
-        #vid_median= np.median(self.frames)
-        
+        # vid_median= np.median(self.frames)
+
         norm_object = deepcopy(self)
         for frame in self.frames:
-            
-            if normtype=='mean':
+            if normtype == "mean":
                 frame_norm = np.mean(self.frames)
-            elif normtype=='median':
+            elif normtype == "median":
                 frame_norm = np.median(self.frames)
-            #frame_median = np.median(self.frames)
-            norm_frames.append(frame*vid_norm/frame_norm)
-        norm_object.frames =  np.array(norm_frames)
-        norm_object.log.append('Normalise_video()')
+            # frame_median = np.median(self.frames)
+            norm_frames.append(frame * vid_norm / frame_norm)
+        norm_object.frames = np.array(norm_frames)
+        norm_object.log.append("normalise_video()")
+        norm_object.frames = norm_object.frames.astype(dtype)
         return norm_object
 
-    def local_normalisation(self,numpatches, padding=15, pad=False, normalise_all=True):
-        '''
-        Normalises contrast across the video frames, ensuring even contrast throughout. 
+    def local_normalisation(
+        self, numpatches, padding=15, pad=False, normalise_all=True
+    ):
+        """
+        Normalises contrast across the video frames, ensuring even contrast throughout.
         frames are taken and split into patches, following which the median of the patches ('local median') is compared to the median of the video ('global median').
-        The patch (local area) is then normalised using the medians (patch = patch* global_median/local_medium) leading to a uniform contrast in the video frame and video itself. 
+        The patch (local area) is then normalised using the medians (patch = patch* global_median/local_medium) leading to a uniform contrast in the video frame and video itself.
+
+        The patch median was chosen so there would be less effect if there is a large dark/bright particle, however if this is too large compared with the patch size it will affect the resulting contrast.
 
-        The patch median was chosen so there would be less effect if there is a large dark/bright particle, however if this is too large compared with the patch size it will affect the resulting contrast. 
-        
         Padding can be applied which will greatly reduce edge artefacts. However doing this well will greatly increase the run time.
         Note: if there is a black region (eg. edge of beam or grid) in the image this may lead to bad results.
 
         Parameters
         ----------
 
             numpatches:int
-                The number of patches on each axis to split the image into, ie image is split into n x n patches and these are given the same median 
+                The number of patches on each axis to split the image into, ie image is split into n x n patches and these are given the same median
 
             padding: int
                 percentage overlap between patches (only used if pad=True)
-            
+
             pad:bool
-                Setting to true reduces edge artifacts from the patches of the image, however it also greatly increases processing time. 
+                Setting to true reduces edge artifacts from the patches of the image, however it also greatly increases processing time.
 
         Returns
         -------
 
             new_vid: Micrograph
                 Copy of the MicroVideo object with a video that has normalised contrast
-        '''
+        """
         new_vid = deepcopy(self)
-        
-        #Create patches
-        xconst = int(new_vid.frames.shape[1]/numpatches)
-        yconst = int(new_vid.frames.shape[2]/numpatches)
-        x_coords = [i*xconst for i in range(numpatches)]
-        y_coords = [i*yconst for i in range(numpatches)]
+
+        # Create patches
+        xconst = int(new_vid.frames.shape[1] / numpatches)
+        yconst = int(new_vid.frames.shape[2] / numpatches)
+        x_coords = [i * xconst for i in range(numpatches)]
+        y_coords = [i * yconst for i in range(numpatches)]
         patch_coords = list(itertools.product(x_coords, y_coords))
-        
-        
+
         if normalise_all:
             global_median = np.median(new_vid.frames)
         else:
-            global_median=None
-        new_frames= []
+            global_median = None
+        new_frames = []
         for frame in new_vid.frames:
-            
-            new_frame = self.local_normalisation_frame(frame, global_median,patch_coords, pad, padding, xconst, yconst )
-            #print(new_frame)
+            new_frame = self.local_normalisation_frame(
+                frame, global_median, patch_coords, pad, padding, xconst, yconst
+            )
+            # print(new_frame)
             new_frames.append(new_frame)
-        new_vid.frames= np.array(new_frames)
-        new_vid.log.append('local_normalisation')
-        return new_vid    
-        
-            
-            
-            
-            
-    def local_normalisation_frame(self,frame,global_median, patch_coords, pad, padding, xconst, yconst):
-        '''
-        Function to perform local normalisation on each frame. This function is called by the local_normalisation() function and can be ignored for users. 
-        '''
+        new_vid.frames = np.array(new_frames)
+        new_vid.log.append("local_normalisation")
+        return new_vid
+
+    def local_normalisation_frame(
+        self, frame, global_median, patch_coords, pad, padding, xconst, yconst
+    ):
+        """
+        Function to perform local normalisation on each frame. This function is called by the local_normalisation() function and can be ignored for users.
+        """
         if pad:
             arrs = []
         else:
-            padding=0
-                
-        if global_median==None:
+            padding = 0
+
+        if global_median == None:
             global_median = np.median(frame)
-            
-        for coord in patch_coords:
 
+        for coord in patch_coords:
             x_low = coord[0]
-            x_high = coord[0]+xconst+int((padding/100)*xconst)
+            x_high = coord[0] + xconst + int((padding / 100) * xconst)
             y_low = coord[1]
-            y_high = coord[1]+yconst+int((padding/100)*yconst)
-
+            y_high = coord[1] + yconst + int((padding / 100) * yconst)
 
             local_patch = frame[x_low:x_high, y_low:y_high]
             local_median = np.median(local_patch)
-            local_patch = local_patch*global_median/local_median
-                
+            local_patch = local_patch * global_median / local_median
+
             if pad:
-                    #Creates arrays for each coordinate and sets the patch equal to the normalise local patch, the rest are zeros
-                    #print(coord)
-                empty_arr = np.zeros_like(frame, dtype='float32')
-                    #Set all values to not-a-number
-                    #print(empty_arr.dtype)
-                empty_arr[:]=np.nan
-                    #Set patch in empty array 
-                empty_arr[x_low:x_high, y_low:y_high]=local_patch
+                # Creates arrays for each coordinate and sets the patch equal to the normalise local patch, the rest are zeros
+                # print(coord)
+                empty_arr = np.zeros_like(frame, dtype="float32")
+                # Set all values to not-a-number
+                # print(empty_arr.dtype)
+                empty_arr[:] = np.nan
+                # Set patch in empty array
+                empty_arr[x_low:x_high, y_low:y_high] = local_patch
                 arrs.append(empty_arr)
-            else:    
-                frame[x_low:x_high, y_low:y_high]=local_patch
-                    
-            
+            else:
+                frame[x_low:x_high, y_low:y_high] = local_patch
+
         if pad:
-                #Creates array of arrays
+            # Creates array of arrays
             arrs = np.array(arrs)
-                #Creates mean of array (ignoring not-a-number values)
+            # Creates mean of array (ignoring not-a-number values)
             new_arr = np.nanmean(arrs, axis=0)
             return new_arr
-                
+
         else:
-                #print(frame)
-            return frame 
-    
-    '''--------------------------------------------------------------------------------
+            # print(frame)
+            return frame
+
+    """--------------------------------------------------------------------------------
     SECTION: METADATA
 
         If a dm file has been opened, the metadata is saved in MicroVideo.metadata_tags, this is unformatted and awkward to use
         but all the raw data can be found. These methods allow easy extraction of some key metadata items: mag, voltage,
         exposure and aquisition date/time. 
-    '''
+    """
+
     def show_metadata(self):
-        '''
-        prints the metadata tags, this can be useful for finding the names of metadata features within the metadata.tags file. 
+        """
+        prints the metadata tags, this can be useful for finding the names of metadata features within the metadata.tags file.
 
-        '''
+        """
         for tag in self.metadata_tags:
-            print('{} : {}\n'.format(tag, self.metadata_tags[tag]))
-
+            print("{} : {}\n".format(tag, self.metadata_tags[tag]))
 
     def get_mag(self):
-        '''
-                
+        """
+
         Returns Micrograph magnifications (indicated and actual) and saves them as microvideo attributes (microscope.indicated_mag, microscope.actual_mag)
 
         Returns
         -------
 
             indicated_mag:float
                 Indicated magnification (i.e. what the microscope tells you the mag is) for the image
             actual_mag: float
-                Actual magnification of the image at the camera. 
-        
-        '''
+                Actual magnification of the image at the camera.
+
+        """
         try:
-            self.indicated_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Indicated Magnification']
+            self.indicated_mag = self.metadata_tags[
+                ".ImageList.2.ImageTags.Microscope Info.Indicated Magnification"
+            ]
         except KeyError:
-            try:    
-                self.indicated_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Formatted Indicated Mag']
+            try:
+                self.indicated_mag = self.metadata_tags[
+                    ".ImageList.2.ImageTags.Microscope Info.Formatted Indicated Mag"
+                ]
             except KeyError:
-                print('Sorry, indicated mag could not be found, try searching for it manually with the show_metadata method')
-        try:   
-            self.actual_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Actual Magnification']
+                print(
+                    "Sorry, indicated mag could not be found, try searching for it manually with the show_metadata method"
+                )
+        try:
+            self.actual_mag = self.metadata_tags[
+                ".ImageList.2.ImageTags.Microscope Info.Actual Magnification"
+            ]
         except KeyError:
-                try:
-                    actual_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Formatted Actual Mag']
-                except:
-                    print('Sorry, indicated mag could not be found, try searching for it manually with the show_metadata method')
-        
-        if hasattr(self, 'actual_mag') and hasattr(self, 'indicated_mag'):
-            #print('Indicated mag: {}'.format(self.indicated_mag))
-            #print('Actual mag: {}'.format(self.actual_mag))
+            try:
+                actual_mag = self.metadata_tags[
+                    ".ImageList.2.ImageTags.Microscope Info.Formatted Actual Mag"
+                ]
+            except:
+                print(
+                    "Sorry, indicated mag could not be found, try searching for it manually with the show_metadata method"
+                )
+
+        if hasattr(self, "actual_mag") and hasattr(self, "indicated_mag"):
+            # print('Indicated mag: {}'.format(self.indicated_mag))
+            # print('Actual mag: {}'.format(self.actual_mag))
             return self.indicated_mag, self.actual_mag
 
     def get_voltage(self):
-        '''
+        """
         Returns voltage and saves is as micrograph attribute
 
         Returns
         -------
 
             Voltage:int
                 Microscope voltage for the image
-        '''        
-        self.voltage = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Voltage']
+        """
+        self.voltage = self.metadata_tags[
+            ".ImageList.2.ImageTags.Microscope Info.Voltage"
+        ]
         return self.voltage
 
     def get_exposure(self, print_values=True):
-        '''
+        """
         Prints and returns the frame rate, exposure time per frame, imaging time and number of frames.
 
         Returns
         -------
 
             fps:int
                 Frame rate of the video in frames per second
 
             Imaging_time:int
                 The total imaging time for the video. s
-        '''
-        #print('Frame rate : {}fps'.format(self.fps))
-        #print('Exposure time per frame: {}s '.format(1/self.fps))
-        if print_values==True:
-            print('Frame rate : {}fps'.format(self.fps))
-            print('Exposure time per frame: {}s '.format(1/self.fps))
-            print('Imaging time: {}s'.format(self.metadata_tags['.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)']))
-            print('Number of frames: {}'.format(self.frames.shape[0]))
-        return self.fps, self.metadata_tags['.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)']
-
-    def get_date_time(self): 
-        '''
-        Prints and returns the aquisition date and time for the image. 
+        """
+        # print('Frame rate : {}fps'.format(self.fps))
+        # print('Exposure time per frame: {}s '.format(1/self.fps))
+        if print_values == True:
+            print("Frame rate : {}fps".format(self.fps))
+            print("Exposure time per frame: {}s ".format(1 / self.fps))
+            print(
+                "Imaging time: {}s".format(
+                    self.metadata_tags[
+                        ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)"
+                    ]
+                )
+            )
+            print("Number of frames: {}".format(self.frames.shape[0]))
+        return (
+            self.fps,
+            self.metadata_tags[
+                ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)"
+            ],
+        )
+
+    def get_date_time(self):
+        """
+        Prints and returns the aquisition date and time for the image.
 
         Returns
         -------
 
             AqDate:str
                 Date on which the micrograph was captured
             AqTime:str
                 Time at which the micrograph was captured
-        '''
-        self.AqDate = self.metadata_tags['.ImageList.2.ImageTags.DataBar.Acquisition Date']
-        self.AqTime = self.metadata_tags['.ImageList.2.ImageTags.DataBar.Acquisition Time']
-        #print('Date: {} '.format(self.AqDate))
-        #print('Time {} '.format(self.AqTime))
+        """
+        self.AqDate = self.metadata_tags[
+            ".ImageList.2.ImageTags.DataBar.Acquisition Date"
+        ]
+        self.AqTime = self.metadata_tags[
+            ".ImageList.2.ImageTags.DataBar.Acquisition Time"
+        ]
+        # print('Date: {} '.format(self.AqDate))
+        # print('Time {} '.format(self.AqTime))
         return self.AqDate, self.AqTime
 
-    def export_metadata(self,name=None, outdir='.'):
-        '''
-        '''
+    def export_metadata(self, name=None, outdir="."):
+        """ """
         make_outdir(outdir)
-        
-        dt = self.get_date_time()
-        date_time = pd.to_datetime(dt[0]+' '+dt[1])
 
-        metadata = {'Image name':self.filename, 'Indicated Magnification':self.get_mag()[0], 'Actual Magnifiation':self.get_mag()[1],  'Date':str(date_time.date()),'Time':str(date_time.time()), 'Pixel size':self.pixel_size,'Pixel unit':self.pixel_unit, 'Exposure Time (s)':self.get_exposure(print_values=False)[1], 'Voltage':self.get_voltage(), 'Size (px)':'{}x{}'.format(self.shape[1],self.shape[2]),'Video':self.video, 'Frame Rate (fps)':self.fps,  'Number of frames':self.frames.shape[0]}        
-        #print(metadata)
+        dt = self.get_date_time()
+        date_time = pd.to_datetime(dt[0] + " " + dt[1])
 
+        metadata = {
+            "Image name": self.filename,
+            "Indicated Magnification": self.get_mag()[0],
+            "Actual Magnifiation": self.get_mag()[1],
+            "Date": str(date_time.date()),
+            "Time": str(date_time.time()),
+            "Pixel size": self.pixel_size,
+            "Pixel unit": self.pixel_unit,
+            "Exposure Time (s)": self.get_exposure(print_values=False)[1],
+            "Voltage": self.get_voltage(),
+            "Size (px)": "{}x{}".format(self.shape[1], self.shape[2]),
+            "Video": self.video,
+            "Frame Rate (fps)": self.fps,
+            "Number of frames": self.frames.shape[0],
+        }
+        # print(metadata)
 
         df = pd.DataFrame(metadata, index=[0])
-        
+
         if name in os.listdir(outdir):
-            old_df = pd.read_csv(outdir+'/'+name)
+            old_df = pd.read_csv(outdir + "/" + name)
             new_df = pd.concat([old_df, df], ignore_index=True)
-            new_df.sort_values(by=['Date', 'Time'], inplace=True)
-            new_df.to_csv(outdir+'/'+name, index=False)
+            new_df.sort_values(by=["Date", "Time"], inplace=True)
+            new_df.to_csv(outdir + "/" + name, index=False)
         else:
-            df.to_csv(outdir+'/'+name,index=False)
-    '''-----------------------------------------------------------------------------------------------------------------------
+            df.to_csv(outdir + "/" + name, index=False)
+
+    """-----------------------------------------------------------------------------------------------------------------------
     SECTION: SCALEBAR
 
         Adds well-sized scalebar to the image. use make_scalebar function for use. 
 
 
 
 
-    '''
+    """
 
     def change_scale_unit(self, new_unit, scaling_factor=None):
-        '''
-        Function to change the unit of the scale in the image. The method is built to allow easy transfer between nanometers ('nm') and microns ('µm'), however can be used to give any new unit providing a scaling factor to multiply the current value by is included. 
+        """
+        Function to change the unit of the scale in the image. The method is built to allow easy transfer between nanometers ('nm') and microns ('µm'), however can be used to give any new unit providing a scaling factor to multiply the current value by is included.
 
         Parameters
         ----------
 
             new_unit : str
                 The new unit for the scale, commonly 'nm' or 'µm'
 
             scaling_factor: int/float
                 The value to multiply the current value by to give the new scale. This isnt necessary with 'µm'/'nm' transitions, but without it any other change will change unit only.
 
-        '''
-        if new_unit==self.pixel_unit:
-            
-            print('The unit is already {}! Skipping file.'.format(new_unit))
-        elif new_unit=='nm' and self.pixel_unit=='µm':
-            self.pixel_size*=1000
-            self.pixel_unit='nm'
-        elif new_unit!='nm' and new_unit!='µm':
-            self.pixel_unit=new_unit
+        """
+        if new_unit == self.pixel_unit:
+            print("The unit is already {}! Skipping file.".format(new_unit))
+        elif new_unit == "nm" and self.pixel_unit == "µm":
+            self.pixel_size *= 1000
+            self.pixel_unit = "nm"
+        elif new_unit != "nm" and new_unit != "µm":
+            self.pixel_unit = new_unit
 
-            if scaling_factor !=None:
-                self.pixel_size*=scaling_factor
+            if scaling_factor != None:
+                self.pixel_size *= scaling_factor
             else:
-                print('Setting new scale unit but not changing the value, please include a scaling factor to also change the value.')
-        elif new_unit=='µm' and self.pixel_unit=='nm':
-            self.pixel_size= self.pixel_size/1000
-            self.pixel_unit='µm'
+                print(
+                    "Setting new scale unit but not changing the value, please include a scaling factor to also change the value."
+                )
+        elif new_unit == "µm" and self.pixel_unit == "nm":
+            self.pixel_size = self.pixel_size / 1000
+            self.pixel_unit = "µm"
+
+        elif (
+            self.pixel_unit not in ["µm", "nm"]
+            and new_unit in ["µm", "nm"]
+            and scaling_factor == None
+        ):
+            print(
+                "Error! You want to switch to {} but the transition from {} is not naturally supported, please include a scaling factor (even if its just 1) to ensure correct conversion.".format(
+                    new_unit, self.pixel_unit
+                )
+            )
+        elif (
+            self.pixel_unit not in ["µm", "nm"]
+            and new_unit in ["µm", "nm"]
+            and scaling_factor != None
+        ):
+            self.pixel_size *= scaling_factor
+            self.pixel_unit = new_unit
+
+        else:
+            print(
+                "Not sure how we got here! Check inputs and try again - if genuine error, raise an issue on github!"
+            )
 
-        elif self.pixel_unit not in ['µm', 'nm'] and new_unit in ['µm','nm'] and scaling_factor==None:
-            print("Error! You want to switch to {} but the transition from {} is not naturally supported, please include a scaling factor (even if its just 1) to ensure correct conversion.".format(new_unit,self.pixel_unit))
-        elif self.pixel_unit not in ['µm', 'nm'] and new_unit in ['µm','nm'] and scaling_factor!=None:
-            self.pixel_size*=scaling_factor
-            self.pixel_unit=new_unit
-
-        else:
-            print('Not sure how we got here! Check inputs and try again - if genuine error, raise an issue on github!')
-
-        self.log.append('change_scale_unit({},{})'.format(new_unit, scaling_factor))
+        self.log.append("change_scale_unit({},{})".format(new_unit, scaling_factor))
 
     def set_scale(self, pixels, dist, unit):
-        '''
+        """
         Set the scale in the image with a measurement (number of pixels and size, with unit)
-        
+
         Parameters
         ----------
-        
+
             pixels : int/float
                 Number of pixels measured
 
             dist : int/float
                 Distance measured
             unit : str
                 Unit of measurement
 
-        '''
-        self.pixel_size=dist/pixels
-        self.pixel_unit=unit
+        """
+        self.pixel_size = dist / pixels
+        self.pixel_unit = unit
 
     def choose_scalebar_size(self):
-        '''
+        """
         Function for choosing scalebar size, called through make_scalebar(), not a standalone function.
 
         Returns
         -------
             scalebar_x: int
-                x coordinate for the scalebar 
+                x coordinate for the scalebar
             scalebar_y: int
-                y coordinate for the scalebar 
+                y coordinate for the scalebar
             width:int
                 width of scalebar
             height:int
                 height of the scalebar
             scalebar_size:int (or float)
                 Size of the scalebar in scaled units (pixel_unit)
-        '''
-        y,x = self.frames.shape[1], self.frames.shape[2]
-        
-        #make coordinates for the scalebar, currently set to y-12.5%,x-5% of image size from the bottom right corner 
-        #of the image to bottom left of the scalebar - change this by editing /20 and /7.5 values (this just looked good to me)
-        scalebar_y = y-int(y/25)
-        scalebar_x = x-int(x/6.5)
-        #print(x,scalebar_x)
-
-        #possible scalebar sizes are given here, if its >500nm it should be in unit micron
-        
-        possible_sizes = [0.5, 1,2,5,10,25,50,100,250,500,1000]
-        
-        #to select sizes, iterate through possible sizes, if the width of the resulting scalebar (n*pixelsize) 
-        #is over 15% of the image size, the size is chose, if none are over 15% of image size
-        #the largest size is chosen as default
+        """
+        y, x = self.frames.shape[1], self.frames.shape[2]
+
+        # make coordinates for the scalebar, currently set to y-12.5%,x-5% of image size from the bottom right corner
+        # of the image to bottom left of the scalebar - change this by editing /20 and /7.5 values (this just looked good to me)
+        scalebar_y = y - int(y / 25)
+        scalebar_x = x - int(x / 6.5)
+        # print(x,scalebar_x)
+
+        # possible scalebar sizes are given here, if its >500nm it should be in unit micron
+
+        possible_sizes = [0.5, 1, 2, 5, 10, 25, 50, 100, 250, 500, 1000]
+
+        # to select sizes, iterate through possible sizes, if the width of the resulting scalebar (n*pixelsize)
+        # is over 15% of the image size, the size is chose, if none are over 15% of image size
+        # the largest size is chosen as default
         for n in possible_sizes:
-            width = int(n*1/self.pixel_size)
-            #print(n, image.shape([0]/10)
-            if width>(x/16):
+            width = int(n * 1 / self.pixel_size)
+            # print(n, image.shape([0]/10)
+            if width > (x / 16):
                 break
-        
-        # This if statement checks whether the scalebar is too close to the edge or bigger than the size. 
+
+        # This if statement checks whether the scalebar is too close to the edge or bigger than the size.
         # This should ensure it is at least one 100th of the image width away from the edge.
 
-        if scalebar_x+width>=x:
+        if scalebar_x + width >= x:
             print(True)
-            diff = x - scalebar_x+width
-            scalebar_x=scalebar_x-diff - x/100
-        elif scalebar_x+width+x/100 > x:
-            scalebar_x=scalebar_x-x/100
-
-        #choose height of scalebar (default is scalebar width/6), convert width into an integer
-        height = int(y/60)
-        width = int(width)   
+            diff = x - scalebar_x + width
+            scalebar_x = scalebar_x - diff - x / 100
+        elif scalebar_x + width + x / 100 > x:
+            scalebar_x = scalebar_x - x / 100
+
+        # choose height of scalebar (default is scalebar width/6), convert width into an integer
+        height = int(y / 60)
+        width = int(width)
         scalebar_x = int(scalebar_x)
         scalebar_y = int(scalebar_y)
         scalebar_size = n
-        #return int(scalebar_x/xybin), int(scalebar_y/xybin), int(height/xybin), int(width/xybin), n
+        # return int(scalebar_x/xybin), int(scalebar_y/xybin), int(height/xybin), int(width/xybin), n
         return scalebar_x, scalebar_y, width, height, scalebar_size
 
-
-
-
-    def choose_scalebar_color(self,color,scalebar_x, scalebar_y , width, height):
-        '''
+    def choose_scalebar_color(self, color, scalebar_x, scalebar_y, width, height):
+        """
         Function for choosing the scalebar color and returns the pixelvalue and text color for the annotation.
         Called through make_scalebar(), not a standalone function
-        '''
-        if color=='black':
+        """
+        if color == "black":
             pixvalue = 0
-            textcolor = 'black'
-        elif color=='white':
+            textcolor = "black"
+        elif color == "white":
             pixvalue = 255
-            textcolor='white'
-        elif color=='grey':
+            textcolor = "white"
+        elif color == "grey":
             pixvalue = 150
-            textcolor='grey'
-        else: #default is black, unless it is a particularly dark area - if the mean pixvalue of the scale bar region is significantly less than the overall image mean, the scalebar will be white
-            
-            if np.mean(self.frames[0][scalebar_y:scalebar_y+height,scalebar_x:scalebar_x+width])<np.mean(self.frames[0])/1.5:
+            textcolor = "grey"
+        else:  # default is black, unless it is a particularly dark area - if the mean pixvalue of the scale bar region is significantly less than the overall image mean, the scalebar will be white
+            if (
+                np.mean(
+                    self.frames[0][
+                        scalebar_y : scalebar_y + height,
+                        scalebar_x : scalebar_x + width,
+                    ]
+                )
+                < np.mean(self.frames[0]) / 1.5
+            ):
                 pixvalue = 255
-                textcolor='white'
+                textcolor = "white"
             else:
                 pixvalue = 0
-                textcolor = 'black'
-        #add scalebar (set pixels to color) 
-
-        return pixvalue, textcolor        
+                textcolor = "black"
+        # add scalebar (set pixels to color)
 
+        return pixvalue, textcolor
 
-    def make_scalebar(self, texton=True, color='Auto', fontsize='M'):
-        '''
-        Automated method to create a scalebar of a suitable size, shape and color. Returns a new object with a scalebar. 
+    def make_scalebar(self, texton=True, color="Auto", fontsize="M"):
+        """
+        Automated method to create a scalebar of a suitable size, shape and color. Returns a new object with a scalebar.
         The color will be selected between black and white based on mean value of the region of the scalebar compared to the mean value of the whole video. To override this the color can be defined as black white or grey.
-        This will work best for 8-bit images, as the scalebar will be given values of 0 or 255. 
+        This will work best for 8-bit images, as the scalebar will be given values of 0 or 255.
 
         You can change the fontsize of the scalebar label with the fontsize option, this is medium ('M') by default but can be made larger or smaller ('S','L', 'XL'), if none of these look good to you, you can choose the fontsize by entering an integer instead of these options. For reference, the fontsize given by these values (calculated based on image size) is printed.
-        
+
         Parameters
         ----------
 
             color : str
                 The color of the scalebar, the options are 'white'. 'black' or 'grey'
             texton : bool
                 Text can be turned off using texton=False, the selected size of the scalebar can be accessed using micrograph.scalebar_size
             fontsize: str
-                Choose the fontsize from S,M,L,XL or give an integer value 
+                Choose the fontsize from S,M,L,XL or give an integer value
         Returns
         -------
             Micrograph_object_with_scalebar: Micrograph
                 Copy of the micrograph object with a scale bar.
-        '''
-        #print(pixvalue, textcolor)
+        """
+        # print(pixvalue, textcolor)
         vidSB = deepcopy(self)
-        scalebar_x, scalebar_y , width, height, scalebar_size = self.choose_scalebar_size()
-        pixvalue, textcolor = self.choose_scalebar_color(color,scalebar_x, scalebar_y , width, height)
-        textposition = ((scalebar_x+width/2),scalebar_y-5)
-
-        if fontsize=='M':
-            fontsize=int(scalebar_x/(22))
-        elif fontsize=='L':
-            fontsize=int(scalebar_x/(18))
-        elif fontsize=='XL':
-            fontsize=int(scalebar_x/(15))
-        elif fontsize=='S':
-            fontsize=int(scalebar_x/(27))
-
+        (
+            scalebar_x,
+            scalebar_y,
+            width,
+            height,
+            scalebar_size,
+        ) = self.choose_scalebar_size()
+        pixvalue, textcolor = self.choose_scalebar_color(
+            color, scalebar_x, scalebar_y, width, height
+        )
+        textposition = ((scalebar_x + width / 2), scalebar_y - 5)
+
+        if fontsize == "M":
+            fontsize = int(scalebar_x / (22))
+        elif fontsize == "L":
+            fontsize = int(scalebar_x / (18))
+        elif fontsize == "XL":
+            fontsize = int(scalebar_x / (15))
+        elif fontsize == "S":
+            fontsize = int(scalebar_x / (27))
 
         for i in range(len(self.frames)):
-            #print(self.frames[i])
-            vidSB.frames[i][scalebar_y:scalebar_y+height,scalebar_x:scalebar_x+width]=pixvalue
-            
-            
-            
-            #if pixel_unit!='nm':
-             #   Utext = str(n)+u'\u00b5'+ 'm'
-              #  text = str(n)+'microns'
-            #else:
-            vidSB.scalebar_size = '{}{}'.format(scalebar_size,vidSB.pixel_unit) 
-             
+            # print(self.frames[i])
+            vidSB.frames[i][
+                scalebar_y : scalebar_y + height, scalebar_x : scalebar_x + width
+            ] = pixvalue
+
+            # if pixel_unit!='nm':
+            #   Utext = str(n)+u'\u00b5'+ 'm'
+            #  text = str(n)+'microns'
+            # else:
+            vidSB.scalebar_size = "{}{}".format(scalebar_size, vidSB.pixel_unit)
 
             pil_image = Image.fromarray(vidSB.frames[i])
 
-            if texton==True:
-                #print('TEXTON!')
-                draw = ImageDraw.Draw(pil_image)        
-                    
-                #fontsize=int(vidSB.scalebar_x/(25))
+            if texton == True:
+                # print('TEXTON!')
+                draw = ImageDraw.Draw(pil_image)
+
+                # fontsize=int(vidSB.scalebar_x/(25))
                 try:
-                    file = font_manager.findfont('Helvetica')
+                    file = font_manager.findfont("Helvetica")
                     font = ImageFont.truetype(file, fontsize)
                 except:
-                    font_search = font_manager.FontProperties(family='sans-serif', weight='normal')
+                    font_search = font_manager.FontProperties(
+                        family="sans-serif", weight="normal"
+                    )
                     file = font_manager.findfont(font_search)
                     font = ImageFont.truetype(file, fontsize)
 
-                draw.text(textposition, vidSB.scalebar_size, anchor ='mb', fill=textcolor, font=font, stroke_width=1)
-                vidSB.frames[i] = np.array(pil_image)    
+                draw.text(
+                    textposition,
+                    vidSB.scalebar_size,
+                    anchor="mb",
+                    fill=textcolor,
+                    font=font,
+                    stroke_width=1,
+                )
+                vidSB.frames[i] = np.array(pil_image)
             else:
-                print('The scalebar added is {}'.format(vidSB.scalebar_size))
-        print('Fontsize:',fontsize)
-        vidSB.log.append('make_scalebar()')
+                print("The scalebar added is {}".format(vidSB.scalebar_size))
+        print("Fontsize:", fontsize)
+        vidSB.log.append("make_scalebar()")
         return vidSB
 
-
-    '''------------------------------------------------------------------------------------------------------------------------
+    """------------------------------------------------------------------------------------------------------------------------
         SECTION: IMAGE FILTERS
         These are filters to improve the visibility of features or decrease the noise levels. Included features are 
             
             - Median filter: performs a median filter with kernal size defined in the call (default is 3)
             - Gaussian filter: performs a Gaussian filter with kernal size defined in the call (default is 3)
             - Weiner filter: performs a Weiner filter with kernal size defined in the call (default is 5)
             - Low pass filter: performs a 2D fourier transform of the image and removes the  
@@ -1274,809 +1378,864 @@
     Therefore to use: 
 
         filtered_micrograph = micrograph.gaussian_filter()
         plt.imshow(filtered_micrograph.image)
         filtered_micrograph.make_scalebar()
 
 
-    '''
+    """
+
     def low_pass_filter(self, radius):
-        '''
+        """
         This low pass filters the image. The pixel size is used to scale the radius to whatever the pixel unit is (ie radius 10 is 10nm/10um)
         If pixelsize is undefined the radius will refer to pixels only
-        
+
         Parameters
         ----------
 
             radius : int (or potentially float)
-                The effects of this vary depending on if the pixelsize is defined in self.pixel_size.: 
-                     - Assuming your micrograph object has a pixel size defined, the filter works by removing any features smaller than the size you input as a parameter (the unit is the same as the pixelsize), A larger number yields a stronger filter, if it is too large, you won't see any features. 
+                The effects of this vary depending on if the pixelsize is defined in self.pixel_size.:
+                     - Assuming your micrograph object has a pixel size defined, the filter works by removing any features smaller than the size you input as a parameter (the unit is the same as the pixelsize), A larger number yields a stronger filter, if it is too large, you won't see any features.
                     Effective filter sizes depends on features and magnification, so with something between 1-5 and tune it to your needs.
                     - If your micrograph is missing a pixelsize the size input will be the radius of a circle kept in the power spectrum. Here the input number does the inverse - a smaller number leads to stronger filter. In this case, much larger numbers will be needed, 50 is a good starting value.
-        
+
         Returns
         -------
                 Low_pass_filtered_object :MicroVideo
-                    Low pass filtered copy of the microvideo object.          
+                    Low pass filtered copy of the microvideo object.
+
+        """
+        # print(N)
+        N = self.frames[0].shape[0]
+        if (
+            type(self.pixel_size) == int
+            or type(self.pixel_size) == float
+            and self.pixel_size != 0
+        ):
+            radius = int((N * self.pixel_size) / radius)
 
-        '''    
-        #print(N)
-        N=self.frames[0].shape[0]
-        if type(self.pixel_size)==int or type(self.pixel_size)==float and self.pixel_size!=0:
-            radius=int((N*self.pixel_size)/radius)
-        
         filtered_object = deepcopy(self)
         for i in range(len(filtered_object.frames)):
             fft = np.fft.fft2(filtered_object.frames[i])
             fshift = np.fft.fftshift(fft)
             magnitude_spectrum = np.log(np.abs(fshift))
-            crow, ccol = int(self.y/2), int(self.x/2)
-            fshift_filtered=np.copy(fshift)
+            crow, ccol = int(self.y / 2), int(self.x / 2)
+            fshift_filtered = np.copy(fshift)
             mask = np.zeros_like(self.frames[i])
 
-            mask = cv.circle(cv.UMat(mask), (crow, ccol),radius*2, 1, -1) 
-            #print(fshift_filtered)
+            mask = cv.circle(cv.UMat(mask), (crow, ccol), radius * 2, 1, -1)
+            # print(fshift_filtered)
             mask = mask.get()
-            fcomplex = fshift[:,:]*1j
-            fshift_filtered = mask*fcomplex
+            fcomplex = fshift[:, :] * 1j
+            fshift_filtered = mask * fcomplex
             f_filtered_shifted = np.fft.fftshift(fshift_filtered)
-            #magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
+            # magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
             inv_image = np.fft.ifft2(f_filtered_shifted)
             filtered_object.frames[i] = np.abs(inv_image)
             filtered_object.frames[i] -= filtered_object.frames[i].min()
-        filtered_object.log.append('low_pass_filter({})'.format(radius))
+        filtered_object.log.append("low_pass_filter({})".format(radius))
         return filtered_object
 
     def median_filter(self, kernal=3):
-        '''
+        """
         Returns a median filtered copy of the Microvideo object, kernal size defined in the call (default is 3)
 
             Parameters
             ----------
                 kernal:int
                     The n x n kernal for median filter is defined here, must be an odd integer
 
             Returns
             -------
                 Median_filtered_object :Microvideo
                     Median filtered copy of Microvideo object with median filtered image
-        '''
+        """
         filtered_object = deepcopy(self)
         for i in range(len(filtered_object.frames)):
-            filtered_object.frames[i] = cv.medianBlur(filtered_object.frames[i],kernal)
-        filtered_object.log.append('median_filter({})'.format(kernal))
+            filtered_object.frames[i] = cv.medianBlur(filtered_object.frames[i], kernal)
+        filtered_object.log.append("median_filter({})".format(kernal))
         return filtered_object
 
     def weiner_filter(self, kernal=5):
-        '''
+        """
         Returns a Weiner filtered copy of the Microvideo object, kernal size defined in the call (default is 5)
 
             Parameters
             ----------
 
                 n :int
                     The n x n kernal for Weiner filter is defined here, must be an odd integer
 
             Returns
             -------
 
                 Weiner_filtered_object : Microvideo
-                    Weiner filtered copy of Microvideo object 
-        '''
+                    Weiner filtered copy of Microvideo object
+        """
 
         from scipy.signal import wiener
+
         filtered_object = deepcopy(self)
         for i in range(len(filtered_object.frames)):
-            filtered_object.frames[i] = wiener(filtered_object.frames[i], (kernal, kernal))
-        weiner_filter.log.append('weiner_filter({})'.format(kernal))
+            filtered_object.frames[i] = wiener(
+                filtered_object.frames[i], (kernal, kernal)
+            )
+        weiner_filter.log.append("weiner_filter({})".format(kernal))
         return filtered_object
 
     def NLM_filter(self, h=5):
-
-        '''
-        Returns a non-local means filtered copy of the Microvideo, filter strength is defined in the call. 
+        """
+        Returns a non-local means filtered copy of the Microvideo, filter strength is defined in the call.
         More information on non-local means filtering can be found here: https://docs.opencv.org/3.4/d5/d69/tutorial_py_non_local_means.html
 
             Parameters
             ----------
                 h:int
                     Defines the strength of the Non-local means filter, default is 5
             Returns
             -------
                 nlm_filtered_object : Microvideo
                     Non-local means filtered copy of the Microvideo object
-        '''
+        """
 
         filtered_object = deepcopy(self)
         for i in range(len(filtered_object.frames)):
-            filtered_object.frames[i] = cv.fastNlMeansDenoising(np.uint8(filtered_object.frames[i]), h)
-        
-        filtered_object.log.append('NLM_filter({})'.format(h))
+            filtered_object.frames[i] = cv.fastNlMeansDenoising(
+                np.uint8(filtered_object.frames[i]), h
+            )
+
+        filtered_object.log.append("NLM_filter({})".format(h))
         return filtered_object
 
     def gaussian_filter(self, kernal=3):
-        '''
+        """
         Returns a Gaussian filtered copy of the micrograph object, kernal size defined in the call (default is 3)
 
             Parameters
             ----------
                 n:int
                     The n x n kernal for median filter is defined here, *must be an odd integer*
 
             Returns
             -------
                 Gaussian_filtered_object :Micrograph
                     Gaussian filtered copy of micrograph object with gaussian filtered image
-        '''
-        if len(self.frames.shape)!=3:
-
-            raise Exception('There should be 3 axis for this, erroring here.')
-        swapped = np.swapaxes(self.frames, 0,2)
-        #print(kernal)
-        swapped = cv.GaussianBlur(swapped, (kernal,kernal), 0)
+        """
+        if len(self.frames.shape) != 3:
+            raise Exception("There should be 3 axis for this, erroring here.")
+        swapped = np.swapaxes(self.frames, 0, 2)
+        # print(kernal)
+        swapped = cv.GaussianBlur(swapped, (kernal, kernal), 0)
         swapped = np.swapaxes(swapped, 0, 2)
 
-        filtered_object = deepcopy(self)        
+        filtered_object = deepcopy(self)
         filtered_object.frames = swapped
-        filtered_object.log.append('gaussian_filter({})'.format(kernal))
+        filtered_object.log.append("gaussian_filter({})".format(kernal))
         return filtered_object
 
+    def topaz_denoise(
+        self,
+        model="unet",
+        use_cuda=True,
+        lowpass=0,
+        cutoff=0,
+        gaus=None,
+        inv_gaus=None,
+        deconvolve=False,
+        deconv_patch=1,
+        patch_size=1024,
+        padding=200,
+        normalize=False,
+    ):
+        """
+        Denoise micrograph with topaz denoiser.
 
-
-    def topaz_denoise(self, model='unet', use_cuda=True, lowpass=0, cutoff=0, \
-                gaus=None,inv_gaus=None ,deconvolve=False,deconv_patch=1, \
-                patch_size=1024, padding=200, normalize=False):
-        '''
-        Denoise micrograph with topaz denoiser. 
-
-        Topaz (https://doi.org/10.1038/s41467-020-18952-1) is a pre-trained implementation of the deeplearning based noise2noise method (https://doi.org/10.48550/arXiv.1803.04189). 
+        Topaz (https://doi.org/10.1038/s41467-020-18952-1) is a pre-trained implementation of the deeplearning based noise2noise method (https://doi.org/10.48550/arXiv.1803.04189).
         It has been specifically trained on cryo-EM datasets but works pretty well for dryTEM and liquid-TEM images and videos. It is very effective at reducing noise and enhancing lower resolution features, although is not necessarily trustworthy for high resolution data.
-        Use with caution, but it is a powerful method. 
-        
-        Best to only perform on a machine with high RAM and ideally a CUDA GPU, as can take a long time with lesser computers. 
+        Use with caution, but it is a powerful method.
+
+        Best to only perform on a machine with high RAM and ideally a CUDA GPU, as can take a long time with lesser computers.
         If topaz is not installed, simply type `pip install topaz-em` into the command line.
 
-        Unfortunately bespoke training is not currently included in SimpliPyTEM, so please use Topaz to train your own model. 
+        Unfortunately bespoke training is not currently included in SimpliPyTEM, so please use Topaz to train your own model.
 
         Parameters
         ----------
             The parameters here are not required for running with default options, these are available through the topaz code and thus documentation for more advanced options can be found in topaz documentation (https://github.com/tbepler/topaz/, https://topaz-em.readthedocs.io/en/latest/?badge=latest)
-            The important parameters are which model is used, and whether to use a cuda GPU: 
+            The important parameters are which model is used, and whether to use a cuda GPU:
 
             model: str
                 Which topaz denoising model is used, options are ['unet', 'unet-small', 'fcnn', 'affine', 'unet-v0.2.1']
             use_cuda: bool
-                Use CUDA gpu(s)? true or false. 
-            
-            
+                Use CUDA gpu(s)? true or false.
 
 
-        '''
-        
-        from topaz.commands import denoise
+
+
+        """
+
         import topaz.denoise as dn
-        
+        from topaz.commands import denoise
+
         frames = self.frames.copy()
-        frames = frames.astype('float32')
+        frames = frames.astype("float32")
 
         im_denoised = deepcopy(self)
-        denoised_frames = [] 
+        denoised_frames = []
 
-        if gaus!= None and gaus>0:
+        if gaus != None and gaus > 0:
             gaus = dn.GaussianDenoise(gaus)
             if use_cuda:
                 gaus.cuda()
         else:
             gaus = None
-            
-        if inv_gaus!= None and inv_gaus>0:
+
+        if inv_gaus != None and inv_gaus > 0:
             inv_gaus = dn.InvGaussianFilter(inv_gaus)
             if use_cuda:
                 inv_gaus.cuda()
         else:
             inv_gaus = None
-        
-
 
         model = dn.load_model(model)
         if use_cuda:
             model.cuda()
 
         for frame in frames:
-            output = denoise.denoise_image(frame, [model], lowpass=lowpass, cutoff=cutoff, gaus=gaus,\
-                                           inv_gaus=inv_gaus ,deconvolve=deconvolve,deconv_patch=deconv_patch,\
-                                           patch_size=1024, padding=200, normalize=False, use_cuda=use_cuda)
+            output = denoise.denoise_image(
+                frame,
+                [model],
+                lowpass=lowpass,
+                cutoff=cutoff,
+                gaus=gaus,
+                inv_gaus=inv_gaus,
+                deconvolve=deconvolve,
+                deconv_patch=deconv_patch,
+                patch_size=1024,
+                padding=200,
+                normalize=False,
+                use_cuda=use_cuda,
+            )
             denoised_frames.append(output)
         im_denoised.frames = np.array(denoised_frames)
 
         return im_denoised
 
-
-    '''
+    """
     ------------------------------------------------------------------------------------------------------------
     Section Visualising images
 
     used for plotting images using matplotlib. Functions very basic so only meant for rapid use, for better figures write own function or use save command
 
-    '''
+    """
+
     def imshow(self, title=None, vmax=None, vmin=None, framenumber=0, average=False):
-        '''
-        Method to view the video as a static image. This method completely uses matplotlib's imshow function to show the image, however this allows control of display with a single command. 
+        """
+        Method to view the video as a static image. This method completely uses matplotlib's imshow function to show the image, however this allows control of display with a single command.
 
-        This method allows control of the title, whether the image is averaged, which frame is plotted and the maximum and minimum values plotted. 
+        This method allows control of the title, whether the image is averaged, which frame is plotted and the maximum and minimum values plotted.
 
         Parameters
         ----------
-            
+
             title:str
-                This gives a title to the plot. 
+                This gives a title to the plot.
 
             vmax:int or float
-                The maximum value in the image such that any value above vmax is white. 
-            
+                The maximum value in the image such that any value above vmax is white.
+
             vmin: int or float
                 The minimum value in the image such that any value below vmin is black.
-            
+
             framenumber: int
                 The index of the frame to be shown (starting from zero, minus numbers can also count from the final frame, i.e -1 is the final frame). If the frame number is out of range, an IndexError is raised.
 
-            average: bool 
+            average: bool
                 Setting to True shows an average of all the frames of the video rather than individual frame number
 
 
-        '''
+        """
 
         if average:
-            av =  np.sum(self.frames, axis=0)
+            av = np.sum(self.frames, axis=0)
 
         if not vmax:
             if not average:
                 vmax = np.max(self.frames)
             else:
                 vmax = np.max(av)
         if not vmin:
             if not average:
                 vmin = np.min(self.frames)
             else:
-                vmin = np.min(av)        
-
+                vmin = np.min(av)
 
-        plt.subplots(figsize=(20,10))
+        plt.subplots(figsize=(20, 10))
         if title:
             plt.title(title, fontsize=30)
         if average:
             plt.imshow(av, vmax=vmax, vmin=vmin)
         else:
             plt.imshow(self.frames[framenumber], vmax=vmax, vmin=vmin)
         plt.show()
 
-    def imshow_pair(self,other_image, title1='', title2='', average=True):
-        '''
-        Basic function for plotting 2 stills from videos side by side. this 
+    def imshow_pair(self, other_image, title1="", title2="", average=True):
+        """
+        Basic function for plotting 2 stills from videos side by side. this
 
 
-        '''
-        fig, ax = plt.subplots(1,2, figsize=(50,30))
+        """
+        fig, ax = plt.subplots(1, 2, figsize=(50, 30))
         ax[0].imshow(self.frames[0])
-        if title1!='':
+        if title1 != "":
             ax[0].set_title(title1, fontsize=30)
-        
+
         ax[1].imshow(other_image)
-        if title2!='':
+        if title2 != "":
             ax[1].set_title(title2, fontsize=30)
         plt.show()
 
-
     def Sidebyside(self, Video2):
-        '''
+        """
         Joins a second video (in the form of a numpy array) to the original video, allowing them to be played side by side.
 
         Parameters
         ----------
 
             Video2:np array
                 The second video to add to the original video
 
         Returns
         -------
             sidebyside:MicroVideo
                 Copy of the original video with the second video grafted onto the side.
-        '''
-        #Add video as numpy stack (Z,Y,X ) 
-        #print(Video1.shape)
-        z1,y1,x1 = self.frames.shape
-        z2, y2, x2=Video2.shape
-        sidebyside = np.zeros((max(z1,z2), max(y1,y2), x1+x2),dtype='uint8')
-
-        # this was put here to invert the masked video, DO this BEFORE calling function. 
-        #masksinv=cv.bitwise_not(np.array(masks))
-        sidebyside[:, :, :x1] =self.frames
-
-        sidebyside[:, :, x1:] =Video2[:,:,:]
-        #plt.imshow(sidebyside[0], cmap='magma')
-        #plt.show()
-        sidebyside_object =deep_copy(self)
+        """
+        # Add video as numpy stack (Z,Y,X )
+        # print(Video1.shape)
+        z1, y1, x1 = self.frames.shape
+        z2, y2, x2 = Video2.shape
+        sidebyside = np.zeros((max(z1, z2), max(y1, y2), x1 + x2), dtype="uint8")
+
+        # this was put here to invert the masked video, DO this BEFORE calling function.
+        # masksinv=cv.bitwise_not(np.array(masks))
+        sidebyside[:, :, :x1] = self.frames
+
+        sidebyside[:, :, x1:] = Video2[:, :, :]
+        # plt.imshow(sidebyside[0], cmap='magma')
+        # plt.show()
+        sidebyside_object = deep_copy(self)
         sidebyside_object.frames = sidebyside
-        return sidebyside    
+        return sidebyside
 
-    def plot_histogram(self, sidebyside=False, imAverage=True, histAverage=False, vmax=None, vmin=None):
-        '''
+    def plot_histogram(
+        self, sidebyside=False, imAverage=True, histAverage=False, vmax=None, vmin=None
+    ):
+        """
         Plots the histogram of the video (or average of the video), this an be accompanied by either the first frame of the video or the sum of the video frames.
 
         Parameters
         ----------
             sidebyside:bool
                 plots the histogram beside a still image of the video - either first frame or image sum
-            
-            imAverage:bool 
+
+            imAverage:bool
                 if plotting a still, this determines whether the still is the video sum (average) or the first frame, true for video sum.
 
             histAverage:bool
                 Plot the histogram of the average frame? (True) or the histogram of the whole video (False)
 
              vmax:int or float
-                The maximum value in the sidebyside plotted image such that any value above vmax is white. 
-            
+                The maximum value in the sidebyside plotted image such that any value above vmax is white.
+
             vmin: int or float
                 The minimum value in the sidebyside plotted image such that any value below vmin is black.
-                       
+
         Output
         ------
 
             Plots the histogram of the video, can have a video still beside the histogram.
 
 
-        '''
-            #evalute the vmaxes depending on imAverage
+        """
+        # evalute the vmaxes depending on imAverage
         if imAverage or histAverage:
-            av =  np.sum(self.frames, axis=0)
+            av = np.sum(self.frames, axis=0)
 
         if sidebyside:
             if not vmax:
                 if not imAverage:
                     vmax = np.max(self.frames)
                 else:
                     vmax = np.max(av)
             if not vmin:
                 if not imAverage:
                     vmin = np.min(self.frames)
                 else:
-                    vmin = np.min(av)        
+                    vmin = np.min(av)
 
-            fig, ax = plt.subplots(1,2, figsize=(30,15))
-            ax[1].tick_params(axis='x', labelsize=25)
-            ax[1].tick_params(axis='y', labelsize=25)
-            
-            #plot image
+            fig, ax = plt.subplots(1, 2, figsize=(30, 15))
+            ax[1].tick_params(axis="x", labelsize=25)
+            ax[1].tick_params(axis="y", labelsize=25)
+
+            # plot image
             if imAverage:
-                ax[0].imshow(av, vmax=vmax,vmin=vmin) 
+                ax[0].imshow(av, vmax=vmax, vmin=vmin)
             else:
-                ax[0].imshow(self.frames[0],vmax=vmax,vmin=vmin)
-
+                ax[0].imshow(self.frames[0], vmax=vmax, vmin=vmin)
 
             if histAverage:
-                ax[1].hist(av.ravel(),100)
+                ax[1].hist(av.ravel(), 100)
             else:
-                if self.frames.dtype == 'unit8':
-                    ax[1].hist(self.frames.ravel(), 256, [0,256])
+                if self.frames.dtype == "unit8":
+                    ax[1].hist(self.frames.ravel(), 256, [0, 256])
                 else:
                     ax[1].hist(self.frames.ravel(), 100)
-            ax[1].set_xlabel('Pixel Values', fontsize=30)
-            ax[1].set_ylabel('Frequency',fontsize=30)
-
+            ax[1].set_xlabel("Pixel Values", fontsize=30)
+            ax[1].set_ylabel("Frequency", fontsize=30)
 
         else:
-            fig,ax = plt.subplots(1,1, figsize=(5,5))
-            #ax.tick_params(axis='x', labelsize=25)
-            #ax.tick_params(axis='y', labelsize=25)
+            fig, ax = plt.subplots(1, 1, figsize=(5, 5))
+            # ax.tick_params(axis='x', labelsize=25)
+            # ax.tick_params(axis='y', labelsize=25)
             if histAverage:
-                plt.hist(av.ravel(),100)
-            else: 
-                if self.frames.dtype == 'unit8':
-                        plt.hist(self.frames.ravel(), 256, [0,256])
-                    
+                plt.hist(av.ravel(), 100)
+            else:
+                if self.frames.dtype == "unit8":
+                    plt.hist(self.frames.ravel(), 256, [0, 256])
+
                 else:
                     plt.hist(self.frames.ravel(), 100)
 
-
         plt.show()
 
     def show_video(self, width=500, fps=None, loop=0):
-        '''
-        Method to show the video within a jupyter notebook. 
-        
+        """
+        Method to show the video within a jupyter notebook.
+
         Parameters
         ----------
 
             fps: int
-                The frame rate of the video show (in frames per second), default is to take it from the metadata, and failing that show it at 10fps. 
+                The frame rate of the video show (in frames per second), default is to take it from the metadata, and failing that show it at 10fps.
+
+            width:int
+                The width of the video shown
 
-            width:int  
-                The width of the video shown  
-            
             loop:int
-                Set to 1 to make the video automatically loop. 
-    
+                Set to 1 to make the video automatically loop.
+
 
 
-        '''
-        if not fps and hasattr(self, 'fps'):
-            fps=self.fps
-        elif not fps and not hasattr(self, 'fps'):
-            fps=10
+        """
+        if not fps and hasattr(self, "fps"):
+            fps = self.fps
+        elif not fps and not hasattr(self, "fps"):
+            fps = 10
 
-        outvid = [] 
+        outvid = []
         for frame in self.frames:
-            frame=cv.cvtColor(frame, cv.COLOR_GRAY2BGR)
+            frame = cv.cvtColor(frame, cv.COLOR_GRAY2BGR)
             outvid.append(frame)
         outvid = np.array(outvid)
         clip = ImageSequenceClip(list(outvid), fps=fps)
         return clip.ipython_display(width=width, loop=loop)
 
-    '''------------------------------------------
+    """------------------------------------------
     SECTION: VIDEO SPECIFIC METHODS
 
-    '''
+    """
+
     def Average_frames(self, groupsize, keep_remainder=False):
-        '''
+        """
         Sums frames in groups, reducing the number of frames and the time resolution but increases contrast.
-        
+
         Parameters
         ----------
             Groupsize:int
-                Number of frames per group to average. Best as a multiple of the number of frames, else the final group will be the remainder (ie a 25 frame video split into groups of 10 will have 3 output frames: 1-10,11-20, 21-25 ). 
-            
+                Number of frames per group to average. Best as a multiple of the number of frames, else the final group will be the remainder (ie a 25 frame video split into groups of 10 will have 3 output frames: 1-10,11-20, 21-25 ).
+
             keep_remainder: bool
                 Set to false to ignore the remainder when averaging (eg a 25 frame video split into sets of 10 leads to 2 frames, with the final 5 frames of the original being abandonned.)
 
         Returns
         -------
             SummedMicroVideo: Microvideo
                 Copy of the original video object with frames averaged in groups of {groupsize}
-        '''
+        """
 
         newframes = []
         for x in range(0, len(self.frames), groupsize):
-            if x+groupsize>len(self.frames):
-
-                frame = np.sum(self.frames[x:len(self.frames)],axis=0)
+            if x + groupsize > len(self.frames):
+                frame = np.sum(self.frames[x : len(self.frames)], axis=0)
             else:
-                frame = np.sum(self.frames[x:x+groupsize],axis=0)    
+                frame = np.sum(self.frames[x : x + groupsize], axis=0)
             newframes.append(frame)
-        averaged_object=deepcopy(self)    
-        if len(self.frames)%groupsize!=0 and not keep_remainder:
-            newframes=newframes[:-1]
-        averaged_object.frames=np.array(newframes)
+        averaged_object = deepcopy(self)
+        if len(self.frames) % groupsize != 0 and not keep_remainder:
+            newframes = newframes[:-1]
+        averaged_object.frames = np.array(newframes)
         averaged_object.reset_xy()
-        averaged_object.log.append('Average_frames({})'.format(groupsize))
+        averaged_object.log.append("Average_frames({})".format(groupsize))
         return averaged_object
 
-
     def Running_average(self, groupsize):
-        '''
-        Sums frames in group of {groupsize} in a running or rolling average fashion - in this case these groups overlap with only a single frame offset, meaning the resulting video has (n - groupsize) frames. 
+        """
+        Sums frames in group of {groupsize} in a running or rolling average fashion - in this case these groups overlap with only a single frame offset, meaning the resulting video has (n - groupsize) frames.
 
         Parameters
         ----------
             Groupsize:int
-                Number of frames per group to average. Best as a multiple of the number of frames, else the final group will be the remainder (ie a 25 frame video split into groups of 10 will have 3 output frames: 1-10,11-20, 21-25 ). 
+                Number of frames per group to average. Best as a multiple of the number of frames, else the final group will be the remainder (ie a 25 frame video split into groups of 10 will have 3 output frames: 1-10,11-20, 21-25 ).
         Returns
         -------
             RunningAveragedMicrovideo:Microvideo
                 Copy of the original video object with frames averaged into groups of {groupsize} with a 1 frame offset between frames
-        '''
+        """
         averaged_video = []
-        for i in range(0, len(self.frames)-groupsize):
-            frame_group = self.frames[i:i+groupsize]
+        for i in range(0, len(self.frames) - groupsize):
+            frame_group = self.frames[i : i + groupsize]
             av_frame_group = np.sum(frame_group, axis=0)
             averaged_video.append(av_frame_group)
         averaged_object = deepcopy(self)
-        averaged_object.frames=np.array(averaged_video)    
+        averaged_object.frames = np.array(averaged_video)
         averaged_object.reset_xy()
-        averaged_object.log.append('Running_average({})'.format(groupsize))
+        averaged_object.log.append("Running_average({})".format(groupsize))
         return averaged_object
 
-    '''---------------------------------
+    """---------------------------------
     SECTION MOTION CORRECTION
     
     This defines using motioncor2 to align video frames, these frames either need to be saved individually, in which case the function group_frames is needed on the image set before use
     Motioncorrect_video works on a dm4 file, converts it to mrc and then runs motioncor on this image stack. 
 
 
-    '''        
+    """
 
     def motioncorrect_vid(self, vid_output=False):
-        '''
-        This is tricky to use but can be incredibly effective, motioncorrecting LTEM videos can dramatically improve the signal to noise ratio of outputted averages. 
-        Here I use the publically available software motioncor2, which can be downloaded from here: https://emcore.ucsf.edu/ucsf-software which can correct for motion within the video. 
+        """
+        This is tricky to use but can be incredibly effective, motioncorrecting LTEM videos can dramatically improve the signal to noise ratio of outputted averages.
+        Here I use the publically available software motioncor2, which can be downloaded from here: https://emcore.ucsf.edu/ucsf-software which can correct for motion within the video.
 
-        In order to use this function, you need to download this software, and then set a path to the executable, note that several versions will be downloaded so ensure you use the correct one for your CUDA setup, I believe CUDA is required for this. 
+        In order to use this function, you need to download this software, and then set a path to the executable, note that several versions will be downloaded so ensure you use the correct one for your CUDA setup, I believe CUDA is required for this.
 
-        to set the executable, open terminal and type: 
-            ```export MOTIONCOR2_PATH='PATH/TO/EXECUTABLE'``` 
+        to set the executable, open terminal and type:
+            ```export MOTIONCOR2_PATH='PATH/TO/EXECUTABLE'```
 
-        to give an example of what this looks like, this is how it looks on my computer: 
+        to give an example of what this looks like, this is how it looks on my computer:
 
             ```export MOTIONCOR2_PATH='/home/Gabriel/Downloads/MotionCor2_1.4.4/MotionCor2_1.4.4_Cuda113-08-11-2021'```
 
         You can also set the executable directly from an ipython workbook by running `os.environ['MOTIONCOR2_PATH']='~/Downloads/MotionCor2_1.4.4/MotionCor2_1.4.4_Cuda113-08-11-2021'`
 
         To avoid needing to do this for every new terminal opened, add this line to your .bashrc file in your home directory (you can use the terminal text editor nano for this: ```nano ~/.bashrc```)
 
-        After doing this, the function should hopefully work, just use: 
-            
+        After doing this, the function should hopefully work, just use:
+
             video=MicroVideo()
             video.open_dm('myfile.dm4')
             motioncorrected_vid = video.motioncorrect_vid()
 
 
         Parameters
         ----------
 
             vid_output:bool
                 Do you want to output a video or just an average image? Image (False) is used for SimpliPyTEM-GUI, Video (True) produces far more data but gives more useful results.
 
         Returns
         -------
 
-            MotionCorrected_video_object: 
+            MotionCorrected_video_object:
 
-        '''
+        """
 
         original_cwd = os.getcwd()
-        tifname = 'OutIntermediateTiff.tif'
-        outname= '.'.join(self.filename.split('.')[:-1])+'Motion_corrected.mrc'
-        print('outname = ', outname)
-        outname = outname.split('/')[-1]
-
-        if '/' in self.filename:
-            directory='/'.join(self.filename.split('/')[:-1])
-        else:
-            directory=os.getcwd() 
-        os.chdir(directory)   
-        print('cwd = ', os.getcwd())
-        MCor_path = os.environ.get('MOTIONCOR2_PATH')
+        tifname = "OutIntermediate.mrc"
+        outname = ".".join(self.filename.split(".")[:-1]) + "Motion_corrected.mrc"
+        outname = outname.replace(" ", "_")
+        print("outname = ", outname)
+        outname = outname.split("/")[-1]
+
+        if "/" in self.filename:
+            directory = "/".join(self.filename.split("/")[:-1])
+        else:
+            directory = os.getcwd()
+        os.chdir(directory)
+        print("cwd = ", os.getcwd())
+        MCor_path = os.environ.get("MOTIONCOR2_PATH")
         if MCor_path:
             if vid_output:
-                command = '{} -InTiff {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixlSize {} -OutStack 1'.format(MCor_path, tifname, outname, self.pixel_size*10)
-                MC_vid=deepcopy(self)
-                inname = '.'.join(outname.split('.')[:-1])+'_Stk.mrc'
+                command = "{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixlSize {} -OutStack 1".format(
+                    MCor_path, tifname, outname, self.pixel_size * 10
+                )
+                MC_vid = deepcopy(self)
+                inname = ".".join(outname.split(".")[:-1]) + "_Stk.mrc"
             else:
-                command = '{} -InTiff {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixlSize {}'.format(MCor_path, tifname, outname, self.pixel_size*10)
+                command = "{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixlSize {}".format(
+                    MCor_path, tifname, outname, self.pixel_size * 10
+                )
                 MC_vid = Micrograph()
-                inname = '.'.join(outname.split('.')[:-1])+'.mrc'
-            self.save_tif_stack(name=tifname)
+                inname = ".".join(outname.split(".")[:-1]) + ".mrc"
+            self.write_mrc(name=tifname, overwrite=True)
             sb.call(command, shell=True, cwd=os.getcwd())
         else:
-            print('Sorry, the motioncor2 exectuable is not defined and so cannot be run. Please give the executable using "export MOTIONCOR2_PATH=\'PATH/TO/EXECUTABLE\'" (or on windows: "setx MY_EXECUTABLE_PATH \'path/to/executable\'") for more info, please see documentation  ')
+            print(
+                "Sorry, the motioncor2 exectuable is not defined and so cannot be run. Please give the executable using \"export MOTIONCOR2_PATH='PATH/TO/EXECUTABLE'\" (or on windows: \"setx MY_EXECUTABLE_PATH 'path/to/executable'\") for more info, please see documentation  "
+            )
             return 1
 
-       
         try:
             MC_vid.open_mrc(inname)
         except FileNotFoundError:
-            print("The file isn't found - this usually appears to be a motioncor2 issue, sometimes it fails to save an image as a stack for some unknown reason (likely to do with filesize), maybe try decreasing the size by binning/averaging?")
+            print(
+                "The file isn't found - this usually appears to be a motioncor2 issue, sometimes it fails to save an image as a stack for some unknown reason (likely to do with filesize), maybe try decreasing the size by binning/averaging?"
+            )
             return 1
         MC_vid.metadata_tags = self.metadata_tags
         MC_vid.pixel_size = self.pixel_size
-        MC_vid.pixel_unit=self.pixel_unit
+        MC_vid.pixel_unit = self.pixel_unit
         MC_vid.fps = self.fps
-        MC_vid.filename = self.filename+'_MotionCorrected'
-        os.remove('OutIntermediateTiff.tif')
+        MC_vid.filename = self.filename + "_MotionCorrected"
+        os.remove(tifname)
         os.chdir(original_cwd)
-        MC_vid.log.append('motioncorrect_vid()')
+        MC_vid.log.append("motioncorrect_vid()")
         return MC_vid
 
-
-    def display_fft(self, average=True, ret=False,vmax=None, vmin=None):
-        '''
-        Function to see the 2D Fourier transform of the video. 
+    def display_fft(self, average=True, ret=False, vmax=None, vmin=None):
+        """
+        Function to see the 2D Fourier transform of the video.
 
         Parameters
         ----------
 
-            Average:bool 
-                Do you want to see a powerspectrum for the average of the video? True or False (default=True) if true, it will be displayed automatically unless the `ret` paraameter is used to return it as a new micrograph object. 
+            Average:bool
+                Do you want to see a powerspectrum for the average of the video? True or False (default=True) if true, it will be displayed automatically unless the `ret` paraameter is used to return it as a new micrograph object.
 
 
             vmax: int/float
                 The 'white value' when plotting the power spectrum, such that anything above this value is set to white.
-            
+
             vmin: int/float
                 The 'black value' when plotting the power spectrum, such that anything below this value is set to black.
-            
-            ret: bool 
+
+            ret: bool
                 Set to true if you want to return a copy of the fft as a micrograph object. Only works if average=True, if average=False, a new object will always be returned.
 
         Returns
         -------
 
-            If ret==True and average=True, a new micrograph object is returned with the power spectrum of the average of the video as the micrograph.image attribute, from here the same functions can be used 
-            
-            if Average==False, a new MicroVideo object is returned with the powerspectrum of each frame sa the .frames attribute. 
+            If ret==True and average=True, a new micrograph object is returned with the power spectrum of the average of the video as the micrograph.image attribute, from here the same functions can be used
+
+            if Average==False, a new MicroVideo object is returned with the powerspectrum of each frame sa the .frames attribute.
 
 
-        '''
+        """
         if average:
             av = np.sum(self.frames, axis=0)
             fft = np.fft.fft2(av)
-            fshift=np.fft.fftshift(fft)
-            magnitude_spectrum=np.log(np.abs(fshift))
-            magnitude_spectrum= magnitude_spectrum.astype(np.float32)
-            
+            fshift = np.fft.fftshift(fft)
+            magnitude_spectrum = np.log(np.abs(fshift))
+            magnitude_spectrum = magnitude_spectrum.astype(np.float32)
+
             if not vmax:
                 vmax = magnitude_spectrum.max()
             if not vmin:
                 vmin = magnitude_spectrum.min()
 
             if ret:
-             
                 fft_ob = Micrograph()
                 fft_ob.image = magnitude_spectrum
                 fft_ob.reset_xy()
-                filename = self.filename.split('.')[:-1]
-                filename.append('_FFT')
+                filename = self.filename.split(".")[:-1]
+                filename.append("_FFT")
                 fft_ob.filename = filename
                 return fft_ob
             else:
-                plt.figure(figsize=(20,20))
+                plt.figure(figsize=(20, 20))
                 plt.imshow(magnitude_spectrum, vmin=vmin, vmax=vmax)
                 plt.show()
         else:
-            fft_frames = [] 
+            fft_frames = []
             for frame in self.frames:
-                fft=np.fft.fft2(frame)
-                fshift=np.fft.fftshift(fft)
-                magnitude_spectrum=np.log(np.abs(fshift))
-                magnitude_spectrum=magnitude_spectrum.astype(np.float32)
+                fft = np.fft.fft2(frame)
+                fshift = np.fft.fftshift(fft)
+                magnitude_spectrum = np.log(np.abs(fshift))
+                magnitude_spectrum = magnitude_spectrum.astype(np.float32)
                 fft_frames.append(magnitude_spectrum)
             fft_ob = MicroVideo()
             fft_ob.frames = np.array(fft_frames)
             fft_ob.reset_xy()
-            filename = self.filename.split('.')[:-1]
-            filename.append('_FFT')
+            filename = self.filename.split(".")[:-1]
+            filename.append("_FFT")
             fft_ob.filename = filename
             return fft_ob
 
 
-# I had to move default pipeline outside of the class because the filters make a new instance of the class and I didnt want to multiply the number of instances in memory. 
+# I had to move default pipeline outside of the class because the filters make a new instance of the class and I didnt want to multiply the number of instances in memory.
 # Use: default_pipeline(micrograph)
-def default_video_pipeline(filename, output_type,medfilter=0, gaussfilter=3, scalebar=True,  xybin=2, color='Auto',\
-    Average_frames=2,save_metadata=True, metadata_name='metadata.csv', outdir='.', name=None, topaz_denoise=False, denoise_with_cuda=False):
-    '''
+def default_video_pipeline(
+    filename,
+    vid_type,
+    contrast_enhance=True,
+    medfilter=0,
+    gaussfilter=3,
+    scalebar=True,
+    xybin=2,
+    color="Auto",
+    Average_frames=2,
+    save_metadata=True,
+    metadata_name="metadata.csv",
+    outdir=".",
+    name=None,
+    topaz_denoise=False,
+    denoise_with_cuda=False,
+    im_type = 'jpg'
+):
+    """
     Use to automate default filtering, scalebar adding, binning,frame averaging and saving.
 
-    From a coding point of view this function is a bit of a mess with if...elif...else statements so I should clear it up at some point. 
+    From a coding point of view this function is a bit of a mess with if...elif...else statements so I should clear it up at some point.
 
     Parameters
     ----------
 
         filename: str
-            The filename of the .dm3 or .dm4 file to open 
+            The filename of the .dm3 or .dm4 file to open
         output type: str
             This needs to be one of the following: ['Save Tif Stack', 'Save Tif Sequence', 'Save Video as .mp4', 'Save video as .avi', 'Save MotionCorrected Average']. To save as an average, use default_image_pipeline (Micrograph_class module).
         medfilter: int
             Kernal value for a median filter to apply, zero is no filter
         gaussfilter: int
             Kernal for a gaussian filter to apply, zero is no filter
         xybin: int
             value by which the image is binned (reduced size) on both the x and y axis
         scalebar:bool
             True for adding scalebar, False for not adding scalebar
         Average_frames: int
-            Average this number of frames together, only used for saving as video options. 
+            Average this number of frames together, only used for saving as video options.
         topaz_denoise: bool
             Denoise with topaz? True (default) or False (default)
         denoise_with_cuda: bool
-            If denoising with topaz, use CUDA gpu for this? If availble this will dramatically increase speed. 
+            If denoising with topaz, use CUDA gpu for this? If availble this will dramatically increase speed.
 
     Outputs
     -------
 
         Performs filtering etc as parameters suggest, saves it in format defined in output_type.
 
-    '''
+    """
 
-    print('Processing :',filename)
+    print("Processing :", filename)
 
     MicroVideo_object = MicroVideo(filename)
-    
-    if save_metadata==True and filename[-4:-1]=='.dm':
-        MicroVideo_object.export_metadata(metadata_name,outdir)
-
-    #print(MicroVideo_object)
-    if not name:
-        name = '.'.join(MicroVideo_object.filename.split('.')[:-1])
-
 
+    if save_metadata == True and filename[-4:-1] == ".dm":
+        MicroVideo_object.export_metadata(metadata_name, outdir)
 
+    # print(MicroVideo_object)
+    if not name:
+        name = ".".join(MicroVideo_object.filename.split(".")[:-1])
 
-    if output_type=='Save MotionCorrected Average':
+    if vid_type == "Save MotionCorrected Average":
         MCor_im = MicroVideo_object.motioncorrect_vid()
         if topaz_denoise:
             Mcor_im = Mcor_im.topaz_denoise(use_cuda=denoise_with_cuda)
 
-        if MCor_im==1:
-            default_image_pipeline(filename, xybin = xybin, medfilter=medfilter, gaussfilter=gaussfilter,outdir=output_folder_name)
+        if MCor_im == 1:
+            default_image_pipeline(
+                filename,
+                output_type=im_type,
+                xybin=xybin,
+                medfilter=medfilter,
+                gaussfilter=gaussfilter,
+                outdir=outdir,
+            )
             return 1
-        #aved =  MCor_vid.toMicrograph()
+        # aved =  MCor_vid.toMicrograph()
         print(medfilter, type(medfilter))
-        if medfilter!=0:
-            MCor_im= MCor_im.median_filter(int(medfilter))
-        if gaussfilter!=0:
+        if medfilter != 0:
+            MCor_im = MCor_im.median_filter(int(medfilter))
+        if gaussfilter != 0:
             MCor_im = MCor_im.gaussian_filter(gaussfilter)
 
-        if xybin!=0 and xybin!=1:
+        if xybin != 0 and xybin != 1:
             MCor_im = MCor_im.bin(xybin)
-        MCor_im = MCor_im.clip_contrast()
-        if scalebar==True:
+        if contrast_enhance:
+            MCor_im = MCor_im.clip_contrast()
+        if scalebar == True:
             MCor_im = MCor_im.make_scalebar()
 
-        MCor_im.write_image(name, outdir=outdir+'/Images')
+        MCor_im.write_image(name, outdir=outdir + "/Images", ftype=im_type)
 
     else:
-        if xybin!= 0 and xybin!=1:
+        if xybin != 0 and xybin != 1:
             MicroVideo_object = MicroVideo_object.bin(xybin)
 
         if topaz_denoise:
-            MicroVideo_object = MicroVideo_object.topaz_denoise(use_cuda=denoise_with_cuda)
+            MicroVideo_object = MicroVideo_object.topaz_denoise(
+                use_cuda=denoise_with_cuda
+            )
 
-        if type(medfilter)==int and medfilter!=0: 
+        if type(medfilter) == int and medfilter != 0:
             MicroVideo_object = MicroVideo_object.median_filter(medfilter)
-        
-        if type(gaussfilter)==int and gaussfilter!=0:  
-            MicroVideo_object = MicroVideo_object.gaussian_filter(gaussfilter)
 
+        if type(gaussfilter) == int and gaussfilter != 0:
+            MicroVideo_object = MicroVideo_object.gaussian_filter(gaussfilter)
 
         if not name:
-            name = '.'.join(MicroVideo_object.filename.split('.')[:1])
-        #MicroVideo_object.bin(xybin)
-        
-        if output_type=='Save Video as .mp4' or output_type=='Save Video as .avi':
-            if Average_frames!= 0 and Average_frames!=1:
-                MicroVideo_object=MicroVideo_object.Average_frames(Average_frames,keep_remainder=False)
-            print('Saving {} as video'.format(filename))
+            name = ".".join(MicroVideo_object.filename.split(".")[:1])
+        # MicroVideo_object.bin(xybin)
+
+        if vid_type == "Save Video as .mp4" or vid_type == "Save Video as .avi":
+            if Average_frames != 0 and Average_frames != 1:
+                MicroVideo_object = MicroVideo_object.Average_frames(
+                    Average_frames, keep_remainder=False
+                )
+            print("Saving {} as video".format(filename))
+            if contrast_enhance:
+                MicroVideo_object = MicroVideo_object.clip_contrast()
             MicroVideo_object.convert_to_8bit()
-            MicroVideo_object = MicroVideo_object.clip_contrast()
-            if scalebar==True:
-                MicroVideo_object=MicroVideo_object.make_scalebar(color=color)
-            name = name+output_type[-4:]
-        
-            MicroVideo_object.write_video(name=name,outdir=outdir+'/Videos')
-  
-                
-        elif output_type=='Save Tif Stack':
-            if scalebar==True:
-                MicroVideo_object=MicroVideo_object.make_scalebar(color=color)
-                #MicroVideo_object = MicroVideo_object.clip_contrast()
-            MicroVideo_object.save_tif_stack(name=name, outdir=outdir+'/Videos')
-
-        elif output_type=='Save Tif Sequence':
-            if scalebar==True:
-                MicroVideo_object= MicroVideo_object.make_scalebar(color=color)
-                #MicroVideo_object = MicroVideo_object.clip_contrast()
 
-            MicroVideo_object.save_tif_sequence(name=name, outdir=outdir+'/Videos')
+            if scalebar == True:
+                MicroVideo_object = MicroVideo_object.make_scalebar(color=color)
+            name = name + vid_type[-4:]
+
+            MicroVideo_object.write_video(name=name, outdir=outdir + "/Videos")
 
+        elif vid_type == "Save Tif Stack":
+            if scalebar == True:
+                MicroVideo_object = MicroVideo_object.make_scalebar(color=color)
+            if contrast_enhance:
+                MicroVideo_object = MicroVideo_object.clip_contrast()
+            MicroVideo_object.save_tif_stack(name=name, outdir=outdir + "/Videos")
+
+        elif vid_type == "Save Tif Sequence":
+            if scalebar == True:
+                MicroVideo_object = MicroVideo_object.make_scalebar(color=color)
+                # MicroVideo_object = MicroVideo_object.clip_contrast()
+            if contrast_enhance:
+                MicroVideo_object = MicroVideo_object.clip_contrast()
+            MicroVideo_object.save_tif_sequence(name=name, outdir=outdir + "/Videos")
 
         else:
-            print('Error "{}" is not an acceptable output type.'.format(output_type))
+            print('Error "{}" is not an acceptable output type.'.format(vid_type))
+
 
-#def group_frames( frames):
+# def group_frames( frames):
 #    prefixes = []
- #   prefix_set=set()
- #   frames.sort()
- #   tups = []
- #   organised_dict= {}
- #   for file in frames:
+#   prefix_set=set()
+#   frames.sort()
+#   tups = []
+#   organised_dict= {}
+#   for file in frames:
 #        file2 = file[:-4]
-  #      end = file2[-9:]
- #       ids = end.split('-')
-  #      vid_id = ids[0]
-  #      frame_id = ids[1]
- #       tups.append((file, vid_id, frame_id))
- #       prefix_set.add(vid_id)
-        
- #   for prefix in prefix_set: 
- #       images_per_prefix = [x[0] for x in tups if x[1]==prefix]
- #       organised_dict[prefix]=images_per_prefix
-   #     return organised_dict
+#      end = file2[-9:]
+#       ids = end.split('-')
+#      vid_id = ids[0]
+#      frame_id = ids[1]
+#       tups.append((file, vid_id, frame_id))
+#       prefix_set.add(vid_id)
+
+#   for prefix in prefix_set:
+#       images_per_prefix = [x[0] for x in tups if x[1]==prefix]
+#       organised_dict[prefix]=images_per_prefix
+#     return organised_dict
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/Micrograph_class.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/Micrograph_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import cv2 as cv
-import ncempy.io as nci
+import argparse
+import itertools
 import os
+import subprocess as sb
+import time
+from copy import deepcopy
+
 import cv2 as cv
 import matplotlib.pyplot as plt
-from matplotlib import font_manager
-from PIL import Image, ImageOps, ImageFont, ImageDraw, ImageFilter
-import numpy as np 
-import time
-import argparse
 import mrcfile
-import subprocess as sb
-from copy import deepcopy
-from scipy.signal import wiener
+import ncempy.io as nci
+import numpy as np
 import pandas as pd
 import tifffile
-import itertools
-
+from matplotlib import font_manager
+from PIL import Image, ImageDraw, ImageFilter, ImageFont, ImageOps
+from scipy.signal import wiener
 
 plt.gray()
 
-class Micrograph: 
-    '''
-    A class holding the micrograph image data along with associated parameters and methods. This makes processing microscope images easier as it collects data and methods into a single place. 
-    The majority of image handling methods here comes from OpenCV, the functions often have more options/parameters, as a result making them both more powerful and more complicated. 
-    This package aims to simplify and automate these functions, however if more functionality is required, I recommend using OpenCV (https://docs.opencv.org/4.x/) as a starting point for your image analysis. 
-    ... 
+
+class Micrograph:
+    """
+    A class holding the micrograph image data along with associated parameters and methods. This makes processing microscope images easier as it collects data and methods into a single place.
+    The majority of image handling methods here comes from OpenCV, the functions often have more options/parameters, as a result making them both more powerful and more complicated.
+    This package aims to simplify and automate these functions, however if more functionality is required, I recommend using OpenCV (https://docs.opencv.org/4.x/) as a starting point for your image analysis.
+    ...
     Attributes
     ----------
     filename:str
         The file name opened (blank if not opened in object)
     pixel_size:float
         The pixel size in the image, should be initialised when opening data assuming the pixel size is included, if not can easily be altered
     pixel_unit:str
         The unit of the pixel size
     metadata_tags:dict
         The metadata of the file should be stored in this dictionary (works with digital micrograph files)
     shape:tuple
-        The shape of the image 
+        The shape of the image
     x:int
         The size of the x axis in the image
-    y:int    
+    y:int
         The size of the y axis in the image
     image: np array
         The image data
 
 
     List of Functions
     -----------------
@@ -105,858 +105,946 @@
 
         show_pair - plots two images side by side
 
     Others:
         display_fft - get the 2D fourier transform of the image.
 
 
-    '''
+    """
+
     def __init__(self, filename=None):
         if filename:
-            self.video=False
-            self.nframes=1
+            self.video = False
+            self.nframes = 1
             self.filename = filename
             self.open_file(filename)
-            self.log = []            
+            self.log = []
         else:
-            self.filename = ''
-            self.image='Undefined'
-            self.pixel_size= 'Undefined'
+            self.filename = ""
+            self.image = "Undefined"
+            self.pixel_size = "Undefined"
             self.log = []
-            self.video=False
-            self.nframes=1
-
-
-
+            self.video = False
+            self.nframes = 1
 
     def open_dm(self, file, video_average=True, pixel_correction=True):
-        '''
-        Imports digital micrograph files into the micrograph object, initialising all the default attributes required, including saving the metadata into self.metadata_tags. 
-        By default, video dm files (dose fractionations) will be summed to create a single image file, there is also an option (video_average) to use the first frame only. 
-        
+        """
+        Imports digital micrograph files into the micrograph object, initialising all the default attributes required, including saving the metadata into self.metadata_tags.
+        By default, video dm files (dose fractionations) will be summed to create a single image file, there is also an option (video_average) to use the first frame only.
+
         Some DM files have 'hot pixels' which have anomalously high signal due to detector malfunction, these often lead to contrast issues.
         To correct for this any pixel which has a higher value than the mean value + (20 x standard deviation) is set to the mean pixel value, this is on by default but can be turned off using pixel_correction=False
-        
+
         This uses the ncempy.io.dm package to read DM files, more information can be found here: https://openncem.readthedocs.io/en/latest/ncempy.io.html
 
 
         Parameters
         ----------
             file : str
-                The name of the dm file to open. The path to the file can also be included if it is not in the same directory. 
+                The name of the dm file to open. The path to the file can also be included if it is not in the same directory.
 
             video_average : bool
                 If file is a video, this controls whether to output an average (sum) of all the frames or the first frame. Default is to average the video (True), change to False to output a single frame
 
-            pixel_correction: bool 
-                Set anomalous 'hot' pixels to the image mean, anomalous pixels defined as image_mean + 20*image_standard_deviation. Default is on (True). 
+            pixel_correction: bool
+                Set anomalous 'hot' pixels to the image mean, anomalous pixels defined as image_mean + 20*image_standard_deviation. Default is on (True).
 
-        '''
+        """
         dm_input = nci.dm.dmReader(file)
-        if len(dm_input['data'].shape)==2:
-            self.image = dm_input['data']
-            
+        if len(dm_input["data"].shape) == 2:
+            self.image = dm_input["data"]
 
         # at the moment it automatically averages a video into a single image. This will be changed soon to allow for video analysis.
-        elif len(dm_input['data'].shape)==3:
-            print('{} is an image stack, averaging frames together, if you would open as a video, please us MicroVideo object'.format(file))
-            self.nframes=dm_input['data'].shape[0]
+        elif len(dm_input["data"].shape) == 3:
+            print(
+                "{} is an image stack, averaging frames together, if you would open as a video, please us MicroVideo object".format(
+                    file
+                )
+            )
+            self.nframes = dm_input["data"].shape[0]
             if video_average:
-
-                images = dm_input['data']
-                self.image= np.sum(images, axis=0)
+                images = dm_input["data"]
+                self.image = np.sum(images, axis=0)
             else:
-                self.image=dm_input['data'][0]
-            self.video=True
+                self.image = dm_input["data"][0]
+            self.video = True
 
         dmfile = nci.dm.fileDM(file)
-        self.metadata_tags =dmfile.allTags        
-        #extract x and y shapes
-        
-        #self.image = np.flip(self.image, axis=0)
+        self.metadata_tags = dmfile.allTags
+        # extract x and y shapes
+
+        # self.image = np.flip(self.image, axis=0)
         self.x = self.image.shape[1]
-        self.pixel_unit = dm_input['pixelUnit'][-1]
+        self.pixel_unit = dm_input["pixelUnit"][-1]
         self.y = self.image.shape[0]
-        self.pixel_size=float(dm_input['pixelSize'][-1])
-        #print(pixel_size,type(pixel_size))
+        self.pixel_size = float(dm_input["pixelSize"][-1])
+        # print(pixel_size,type(pixel_size))
         self.original_image = self.image
         self.filename = file
-        #self.pixel_size= float(pixel_size)
-        #self.pixel_unit = pixel_unit
-
+        # self.pixel_size= float(pixel_size)
+        # self.pixel_unit = pixel_unit
 
-        
-        #this line removes dead pixels which are super bright (any pixel which is more than mean+25*stddeviation
+        # this line removes dead pixels which are super bright (any pixel which is more than mean+25*stddeviation
         if pixel_correction:
-            self.image[self.image>self.image.mean()+self.image.std()*20]=self.image.mean()
-        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default. 
-        self.image = self.image.astype('float32')
+            self.image[
+                self.image > self.image.mean() + self.image.std() * 20
+            ] = self.image.mean()
+        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default.
+        self.image = self.image.astype("float32")
         #       #return image, x, y, pixel_size, pixel_unit
-        self.shape=self.image.shape
-        print('{} opened as a Micrograph object'.format(file))
+        self.shape = self.image.shape
+        print("{} opened as a Micrograph object".format(file))
 
     def open_mrc(self, file, pixel_correction=True):
-        '''
-        Imports MRC image files into the Micrograph object. 
+        """
+        Imports MRC image files into the Micrograph object.
 
         Parameters
         ----------
             file : str
-                The name of an MRC file to open, the path to the file can also be included. 
-        '''
+                The name of an MRC file to open, the path to the file can also be included.
+        """
 
-        mrc= mrcfile.open(file)
+        mrc = mrcfile.open(file)
         print(mrc.voxel_size)
         voxel_size = mrc.voxel_size
-        self.pixel_size = float(str(voxel_size).split(',')[0].strip('('))
+        self.pixel_size = float(str(voxel_size).split(",")[0].strip("("))
         self.image = mrc.data
         self.image.setflags(write=1)
         self.x = self.image.shape[1]
         self.y = self.image.shape[0]
-        #self.image = np.flip(self.image, axis=0)
-        self.pixel_unit='nm'
+        self.image = np.flip(self.image, axis=0)
+        self.pixel_unit = "nm"
         self.filename = file
         if pixel_correction:
-            self.image[self.image>self.image.mean()+self.image.std()*20]=self.image.mean()
-        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default. 
-        self.image = self.image.astype('float32')
-        self.shape=self.image.shape
+            self.image[
+                self.image > self.image.mean() + self.image.std() * 20
+            ] = self.image.mean()
+        # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default.
+        self.image = self.image.astype("float32")
+        self.shape = self.image.shape
         self.original_image = self.image
 
-    ##write a hyperspy opening function 
+    ##write a hyperspy opening function
 
     def open_image(self, filename, pixel_size=None, pixel_unit=None):
-        '''
+        """
         Open a jpg, png or tif file into the micrograph object. If the tif has any metadata tags, these should be saved into the metadata_tags and will then be accessible with .show_metadata()
         The pixel size is likely to be included somewhere within the metadata and may be loaded, but the name of the tags are not always constant, and so this may need to be searched in  the .show_metadata output.
-        
+
         Parameters
         ----------
 
             filename: str
                 Name of image file to load into the object
             pixel_size: float
                 The pixel size in the image, not necessary but can be included here, can also be loaded with set_scale()
             pixel_unit: str
                 The unit for the pixel size included.
-        '''
+        """
 
-        if filename[-3:].lower()=='jpg' or filename[-3:]=='png':
-            #Load file as grayscale image
+        if filename[-3:].lower() == "jpg" or filename[-3:] == "png":
+            # Load file as grayscale image
             self.image = cv.imread(filename, 0)
             if type(self.image) is None:
                 raise FileNotFoundError
-        if filename[-3:] in ['tiff', 'tif', 'TIF', 'TIFF']:
+        if filename[-3:] in ["tiff", "tif", "TIF", "TIFF"]:
             with tifffile.TiffFile(filename) as tif:
                 self.metadata_tags = {}
                 self.image = tif.asarray()
                 for page in tif.pages:
                     for tag in page.tags:
                         self.metadata_tags[tag.name] = tag.value
 
-            if 'XResolution' in self.metadata_tags:
-                if self.metadata_tags['XResolution']==self.metadata_tags['YResolution']:
+            if "XResolution" in self.metadata_tags:
+                if (
+                    self.metadata_tags["XResolution"]
+                    == self.metadata_tags["YResolution"]
+                ):
                     try:
-                        self.pixel_size = 1/(self.metadata_tags['XResolution'][0] / self.metadata_tags['XResolution'][1])
+                        self.pixel_size = 1 / (
+                            self.metadata_tags["XResolution"][0]
+                            / self.metadata_tags["XResolution"][1]
+                        )
                     except:
                         pass
 
-            if 'unit' in self.metadata_tags:
-                if self.metadata_tags['unit']=='micron':
-                    self.pixel_unit = 'µm'
-                elif self.metadata_tags['unit']=='nm':
-                    self.pixel_unit='nm'
+            if "unit" in self.metadata_tags:
+                if self.metadata_tags["unit"] == "micron":
+                    self.pixel_unit = "µm"
+                elif self.metadata_tags["unit"] == "nm":
+                    self.pixel_unit = "nm"
 
-        self.filename=filename
+        self.filename = filename
         self.reset_xy()
 
         if pixel_size:
-            self.pixel_size=pixel_size
+            self.pixel_size = pixel_size
         else:
-            self.pixel_size=1
-        if pixel_unit: 
-            self.pixel_unit=pixel_unit
+            self.pixel_size = 1
+        if pixel_unit:
+            self.pixel_unit = pixel_unit
         else:
-            self.pixel_unit='pixels'
+            self.pixel_unit = "pixels"
 
         self.original_image = self.image
 
+    def open_array(
+        self, array, pixel_size=None, pixel_unit=None, name="Default_image_name"
+    ):
+        """
+        Opens np array into micrograph object.
 
-    def open_array(self, array, pixel_size=None, pixel_unit=None, name='Default_image_name'):
-        '''
-        Opens np array into micrograph object. 
-        
         Parameters
         ----------
 
             array:  numpy array
-                The image data in the form of a numpy array 
+                The image data in the form of a numpy array
 
             pixel_size: float
                 The pixel size in the image, not necessary but can be included here, can also be loaded with set_scale()
             pixel_unit: str
                 The unit for the pixel size included.
             name: str
-                The name for the image (becomes micrograph.filename attribute)     
-        '''
+                The name for the image (becomes micrograph.filename attribute)
+        """
 
-        self.image = array 
+        self.image = array
         self.reset_xy()
         self.filename = name
         if pixel_size:
-            self.pixel_size=pixel_size
+            self.pixel_size = pixel_size
         if pixel_unit:
-            self.pixel_unit=pixel_unit
+            self.pixel_unit = pixel_unit
 
         self.original_image = self.image
 
     def open_file(self, filename):
-        if filename[-4:]=='.dm3' or filename[-4:]=='.dm4':
+        if filename[-4:] == ".dm3" or filename[-4:] == ".dm4":
             self.open_dm(filename)
-        elif filename[-4:]=='.mrc':
+        elif filename[-4:] == ".mrc":
             self.open_mrc(filename)
-        elif filename[-4:].lower() in ['.jpg', '.png', '.tif', 'tiff']:
+        elif filename[-4:].lower() in [".jpg", ".png", ".tif", "tiff"]:
             self.open_image(filename)
-        elif filename[-4:].lower() in ['.mp4', '.avi', '.mov']:
+        elif filename[-4:].lower() in [".mp4", ".avi", ".mov"]:
             self.open_video(filename)
 
-
-    def open_video(self, filename,pixel_size=1,pixel_unit='pixels',):
-        '''
+    def open_video(
+        self,
+        filename,
+        pixel_size=1,
+        pixel_unit="pixels",
+    ):
+        """
         Loads video files (eg. mp4 and avi, unsure if others will work) into microvideo object.
         The pixel size is not taken from the video by default, and so it should be included in the command, else the default of 1nm/pixel is used. This can be addedd later using video.pixel_size= {new pixel size}
-        
+
         Parameters
         ----------
 
             filename: str
                 Name of the video file to open
             pixel_size: float
                 Size of one pixel (eg. 1nm/pixel), optionall.
             pixel_unit: str
                 Unit for the pixel_size
 
-        '''
+        """
 
         cap = cv.VideoCapture(filename)
-        frames= []
-        self.filename = '.'.join(filename.split('.')[:-1])
+        frames = []
+        self.filename = ".".join(filename.split(".")[:-1])
         while cap.isOpened():
-            ret, frame =cap.read()
-            
-            #print(ret, frame)
+            ret, frame = cap.read()
+
+            # print(ret, frame)
             if not ret:
                 print("Can't receive frame (stream end?). Exiting ...")
                 break
-            #print(frame.shape)
+            # print(frame.shape)
             frame = cv.cvtColor(frame, cv.COLOR_BGR2GRAY)
-            #plt.imshow(frame)
-            #cv.imshow('frame',frame)
-            if cv.waitKey(1)==ord('q'):
+            # plt.imshow(frame)
+            # cv.imshow('frame',frame)
+            if cv.waitKey(1) == ord("q"):
                 break
             frames.append(frame)
-            #print(len(frames))
+            # print(len(frames))
         frames = np.array(frames)
         self.image = np.sum(frames, axis=0)
-        self.image = self.image.astype('float32')
+        self.image = self.image.astype("float32")
         print(self.image)
-        print('{} frames loaded as an average'.format(len(frames)))
-        #print('As format is avi, the pixelsize is not loaded automatically, please set this using micrograph.pixel_size = n')
+        print("{} frames loaded as an average".format(len(frames)))
+        # print('As format is avi, the pixelsize is not loaded automatically, please set this using micrograph.pixel_size = n')
         cap.release()
         self.reset_xy()
-        self.pixel_size=pixel_size
-        self.pixel_unit=pixel_unit
+        self.pixel_size = pixel_size
+        self.pixel_unit = pixel_unit
 
-
-    def write_image(self, name=None, ftype='jpg',outdir=None):
-        '''
-        Saves the image in a .jpg or .tif file for display or use with other programs. 
+    def write_image(self, name=None, ftype="jpg", outdir=None, bit8=False):
+        """
+        Saves the image in a .jpg or .tif file for display or use with other programs.
 
         Parameters
         ----------
             name: str
-                Filename for saved image. Ending with either .jpg or .tif will define the format of the image, alternatively ftype argument can be used. 
-                This is optional, without including a name the name of the original file opened will be used. 
+                Filename for saved image. Ending with either .jpg or .tif will define the format of the image, alternatively ftype argument can be used.
+                This is optional, without including a name the name of the original file opened will be used.
 
             ftype: str
-                Optional. Filetype of output image, either 'jpg' or 'tif' (default jpg), this is better defined using the suffix of the name. 
-                Saving as a tif will save in whatever format it is currently in - this can be a 32-bit or 8-bit image, using convert_to_8bit() will ensure that latter.
+                Optional. Filetype of output image, either 'jpg' or 'tif' (default jpg), this is better defined using the suffix of the name.
+                Saving as a tif will save in whatever format it is currently in - this can be a 32-bit or 8-bit image, using 'tif 8-bit' or bit8=True ensures its the latter.
+            bit8: bool
+                save tif as 8-bit image? Set to False if you want a full size (32-bit) image
 
             outdir: str
                 Keyword argument (usage: outdir='/path/to/directory'). This defines the output location of the saved image, use a path relative to the current directory or an absolute path.
                 The final directory in the path will be made if it does not already exist.
-        ''' 
-        if outdir:
-            make_outdir(outdir)
-            name = outdir+'/'+name
-        #print('Start name :', name)
+        """
+
+        # print('Start name :', name)
         if name:
-                #print('if name : ',name)
-                if name[-4:]=='.jpg':
-                    ftype='jpg'
-                    name = name[:-4]
-                elif name[-4:]=='.tif':
-                    ftype='tif'    
-                    name = name[:-4]
-
-                if len(name.split('.'))>=2 and name[-4]=='.':
-                    name='.'.join(name.split('.')[:-1])
-                    #print('if len name: ', name)
-                    #print('.'.join(name.split('.')[:-1]))
+            # print('if name : ',name)
+            if name[-4:] == ".jpg":
+                ftype = "jpg"
+                name = name[:-4]
+            elif name[-4:] == ".tif":
+                ftype = "tif"
+                name = name[:-4]
+
+            if len(name.split(".")) >= 2 and name[-4] == ".":
+                name = ".".join(name.split(".")[:-1])
+                # print('if len name: ', name)
+                # print('.'.join(name.split('.')[:-1]))
         else:
-                name = '.'.join(self.filename.split('.')[:-1])
-                name+='.'+ftype
-                #print('else_name = ',name)
-        #try:
-        #    name += '_'+self.scalebar_size.replace('µ','u')+'scale.{}'.format(ftype)
-        #except AttributeError:
-        
-        #if self.foldername!='':
-        #        name = '/'+self.foldername.strip('/n') + '/' + name.split('/')[-1]
-        #if self.foldername=='':
-        #    newname = self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
-        #else:
-        #    newname = self.foldername.strip('\n') + '/' +self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
-        
-        name+='.'+ftype
-        if self.pixel_unit=='µm':
-            pixel_unit='um'
+            name = ".".join(self.filename.split(".")[:-1])
+
+
+        if outdir:
+            make_outdir(outdir)
+            name = outdir + "/" + name
+            # print('else_name = ',name)
+
+        name += "." + ftype[:3]
+        if self.pixel_unit == "µm":
+            pixel_unit = "um"
         else:
-            pixel_unit=self.pixel_unit
+            pixel_unit = self.pixel_unit
 
-        if ftype=='jpg':
-            if self.image.max()!=255 or self.image.min()!=0:
+        if ftype == "jpg":
+            if self.image.max() != 255 or self.image.min() != 0:
                 print(self.image.max(), self.image.min())
                 self = self.convert_to_8bit()
-                print('converting to 8bit')
-            cv.imwrite(name,self.image)
+                print("converting to 8bit")
+            cv.imwrite(name, self.image)
 
-        elif ftype=='tif':
-            metadata= self.metadata_tags
-            metadata['unit':pixel_unit]
-            tifffile.imsave(name, self.image,imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata=metadata)
+        elif ftype[:3] == "tif":
+            if not hasattr(self, 'metadata_tags'):
+                self.metadata_tags={'Pixel Size':self.pixel_size, 'unit':'Pixel unit'}
+            metadata = self.metadata_tags
+            metadata["unit"]=pixel_unit
+            if ftype=='tif 8-bit' or bit8==True:
+                self = self.convert_to_8bit()
+            delkeys = []
+            for key in metadata.keys():
 
-        #self.pil_image.save(name, quality=self.quality)
-        print(name, 'Done!')
+                if isinstance(metadata[key], str):
+                    if '\xb5' in metadata[key]:
+                        metadata[key]=metadata[key].replace('µ','u')
+                        print('replaced')
+
+                    else:
+                        metadata[key]=metadata[key].encode('ascii', 'ignore').decode('ascii')
+                if '\xb5' in key:
+                    nkey=key.replace('µ','u')
+                    #metadata[nkey]=metadata[key]
+                    delkeys.append((key, nkey))
+                if '\xf8' in key:
+                    nkey = key.replace('\xf8','_')
+                    delkeys.append((key, nkey))
+            for keys in delkeys:
+                metadata[keys[1]]=metadata[keys[0]]
+                del metadata[keys[0]]
+            
+
+            
+            try:
+                tifffile.imsave(
+                    name,
+                    self.image,
+                    imagej=True,
+                    resolution=(1 / self.pixel_size, 1 / self.pixel_size),
+                    metadata=metadata,
+
+                )
+            except UnicodeEncodeError:
+                print('Metadata contains unconverted unicode (in one of the tag keys), metadata not being saved.')
+                tifffile.imsave(
+                    name,
+                    self.image,
+                    imagej=True,
+                    resolution=(1 / self.pixel_size, 1 / self.pixel_size),
+                )
+
+        print(name, "Done!")
 
         #    def average_video(self):
         #       self.image = np.average(image, axis=0)
-    
+
+
     def reset_xy(self):
-        '''
+        """
         Resets the image attributes for the x, y and shape of the image. Used by the binning method and is also useful following cropping of the micrograph
 
-        '''
+        """
         self.x = self.image.shape[1]
         self.y = self.image.shape[0]
         self.shape = self.image.shape
 
     def revert_to_original(self):
-        '''
+        """
         When an image is loaded, the original image is saved as a separate attribute, this function resets the image to original.
-        
-        '''
+
+        """
         self.image = self.original_image
         self.reset_xy()
-        
-    '''-----------------------------------------------------------------------------------------------------------------------
+
+    """-----------------------------------------------------------------------------------------------------------------------
         SECTION: BASIC FUNCTIONS
 
             add_frames : this sums all the frames of a video together if the frames are saved individually, input is a list of frames, can be generated using the group frames method in the motioncorrection section 
             convert to 8bit: this is important to create a easily openable and lower filesize output image good for viewing. 
 
 
-    '''
+    """
+
     def convert_to_8bit(self):
-        ''' 
-        Returns a micrograph object with the image scaled between 0 and 255 (an 8-bit image). Improves contrast and is a more usable image format than higher bits. 
-        
+        """
+        Returns a micrograph object with the image scaled between 0 and 255 (an 8-bit image). Improves contrast and is a more usable image format than higher bits.
+
         Returns
         -------
             Micrograph8bit : Micrograph
                 A copy of the micrograph object with the image scaled between 0 and 255
 
-        '''
+        """
         image8bit = deepcopy(self)
-        image8bit.image = ((self.image - self.image.min()) * (1/(self.image.max() - self.image.min()) * 255))
-        image8bit.image = image8bit.image.astype('uint8')
+        image8bit.image = (self.image - self.image.min()) * (
+            1 / (self.image.max() - self.image.min()) * 255
+        )
+        image8bit.image = image8bit.image.astype("uint8")
         return image8bit
 
-
     def bin(self, value=2):
-        '''
+        """
         This bins (reduces size) of the image on the x and y dimensions by the selected value (e.g. a 4000x4000 pixels image goes to 2000x2000 pixels with a value of 2)
 
         Parameters
         ----------
             value:int
                 The scale by which to reduce the image size on each dimension. This is normally kept to powers of 2 but any number (including floating point numbers) should work.
         Returns
         -------
             Binned_image:Micrograph
                 Copy of micrograph object with reduced image size
 
-        '''
+        """
         binned_image = deepcopy(self)
-        binned_image.image = cv.resize(self.image, (int(self.image.shape[1]/value), int(self.image.shape[0]/value)), interpolation=cv.INTER_CUBIC) 
-        binned_image.pixel_size= binned_image.pixel_size*value
+        binned_image.image = cv.resize(
+            self.image,
+            (int(self.image.shape[1] / value), int(self.image.shape[0] / value)),
+            interpolation=cv.INTER_CUBIC,
+        )
+        binned_image.pixel_size = binned_image.pixel_size * value
         binned_image.reset_xy()
         return binned_image
 
     def add_frames(self, frames):
-        '''
-        This is used to create a sum of a series of frames where each frame is a saved in a separate .dm file. 
+        """
+        This is used to create a sum of a series of frames where each frame is a saved in a separate .dm file.
 
         Parameters
         ----------
             frames:list
                 A series of frames (name or path+name) to add to the original frame
 
         Output
         ------
-            Adds the frames to the existing frame, self.image is now an average of all the frames. 
+            Adds the frames to the existing frame, self.image is now an average of all the frames.
 
-        '''
+        """
 
         for frame in frames:
             next_frame = nci.dm.dmReader(frame)
-            self.image = self.image + next_frame['data']
+            self.image = self.image + next_frame["data"]
 
     # This, much like the filters below returns the enhanced version as a new object, I have made it this way to allow tuning of alpha and beta.
-    
 
     def clip_contrast(self, saturation=0.2, maxvalue=None, minvalue=None):
         """
-        Function for enhancing the contrast in an image by clipping the histogram between two values. 
+        Function for enhancing the contrast in an image by clipping the histogram between two values.
         These values can be defined directly or can be automatically decided using a saturation value, which the is percentage of the pixels above or below this value.
-        I.e, if there are 1,000,000 pixels in an image and the saturation value is 0.1, the method searches the value for which only 0.1% or 1000 pixels are above/below. 
+        I.e, if there are 1,000,000 pixels in an image and the saturation value is 0.1, the method searches the value for which only 0.1% or 1000 pixels are above/below.
         These values then become the new minimum and maximum of the image, and are scaled to between 0 and 255.
-        
+
         This method will automatically convert to 8 bit (scale between 0 and 255), if this is an issue raise and it can be changed in future versions.
 
         Parameters
         ----------
 
             saturation: Float
                 The percentage cutoff above/below which the pixels are set to zero/255, default is 0.5% of pixels
 
             maxvalue: int
-                The maximum value that is being clipped (to be decided from histogram). Optional. 
+                The maximum value that is being clipped (to be decided from histogram). Optional.
 
             minvalue: int
-                The minimum value that is being clipped (to be decided from histogram). Optional. 
+                The minimum value that is being clipped (to be decided from histogram). Optional.
 
         Returns
         -------
 
             Contrast_enhanced_micrograph : Micrograph
                 Return a copy of the object with the contrast clipped at either end of the image
 
         Usage
         -----
 
             MicrographContrastClipped = micrograph.clip_contrast(saturation=1)
-            
-            or 
+
+            or
 
             MicrographContrastClipped = micrograph.clip_contrast(maxvalue=220, minvalue=20)
 
         """
-        new_im  = self.convert_to_8bit()
-        
-        if not maxvalue:
+        new_im = self.convert_to_8bit()
 
-            print('Saturation = ',saturation)
-            maxvalue = np.percentile(new_im.image, 100-saturation)
-            print('Maxmium value : ',maxvalue)
+        if not maxvalue:
+            print("Saturation = ", saturation)
+            maxvalue = np.percentile(new_im.image, 100 - saturation)
+            print("Maxmium value : ", maxvalue)
         if not minvalue:
             minvalue = np.percentile(new_im.image, saturation)
-            print('Minimum value : ', minvalue)
-        image =new_im.image.astype(np.int16)    
-        new_im.image = (image - minvalue)*(255/(maxvalue-minvalue))
-        new_im.image[new_im.image>255]=255
-        new_im.image[new_im.image<0]=0
+            print("Minimum value : ", minvalue)
+        image = new_im.image.astype(np.int16)
+        new_im.image = (image - minvalue) * (255 / (maxvalue - minvalue))
+        new_im.image[new_im.image > 255] = 255
+        new_im.image[new_im.image < 0] = 0
         new_im.image = new_im.image.astype(np.uint8)
 
-        new_im.log.append('clip_contrast()')
+        new_im.log.append("clip_contrast()")
         return new_im
 
+    def enhance_contrast(self, alpha=1.5, beta=0, gamma=""):
+        """
+        Function for enhancing contrast. This uses the OpenCV methods detailed here: https://docs.opencv.org/3.4/d3/dc1/tutorial_basic_linear_transform.html.
+        There are 3 input values which define contast controls: alpha, beta and gamma, the gamma value is optional.
 
-    def enhance_contrast(self, alpha=1.5, beta=0, gamma=''):
-        '''
-        Function for enhancing contrast. This uses the OpenCV methods detailed here: https://docs.opencv.org/3.4/d3/dc1/tutorial_basic_linear_transform.html. 
-        There are 3 input values which define contast controls: alpha, beta and gamma, the gamma value is optional. 
-        
         Parameters
         ----------
 
             alpha:float
-                Basic contrast control, usually in the range of 1-3. The histogram is streched. 
+                Basic contrast control, usually in the range of 1-3. The histogram is stretched.
 
             beta: int (or float)
                 Brightness control, this will add the value to every pixel in the image, only really has an effect with 8-bit images (and any pixels above 255 will be clipped to this)
-            
+
             gamma:float
                 Non-linear contrast control, values between 0-1 makes images brighter (particularly the dark areas), while values >1 darken the image(particularly the bright areas)
-                Optional, if included image will be converted to 8 bit. 
+                Optional, if included image will be converted to 8 bit.
 
-        Returns 
+        Returns
         -------
 
             Contrast_enhanced_micrograph : Micrograph
                 Return a copy of the object with the contrast enhanced.
-        '''
+        """
         enhanced_image = cv.convertScaleAbs(self.image, alpha=alpha, beta=beta)
-        #print(self.image.dtype)
-        
-        #enhanced_image = cv.equalizeHist(enhanced_image)
+        # print(self.image.dtype)
+
+        # enhanced_image = cv.equalizeHist(enhanced_image)
         enhanced_object = deepcopy(self)
         enhanced_object.image = enhanced_image
-        if type(gamma)==float or type(gamma)==int:
-            if enhanced_object.image.dtype!='uint8':
-                enhanced_objec=enhanced_object.convert_to_8bit()
-            LUT =np.empty((1,256), np.uint8)
+        if type(gamma) == float or type(gamma) == int:
+            if enhanced_object.image.dtype != "uint8":
+                enhanced_objec = enhanced_object.convert_to_8bit()
+            LUT = np.empty((1, 256), np.uint8)
             for i in range(256):
-                LUT[0, i]=np.clip(pow(i/255.0,gamma)*255.0, 0, 255)
-            res =cv.LUT(enhanced_object.image, LUT) 
-            print('Gamma adjusted...')
-        if self.image.dtype=='uint8':
-            enhanced_image[enhanced_image>255]=255
+                LUT[0, i] = np.clip(pow(i / 255.0, gamma) * 255.0, 0, 255)
+            res = cv.LUT(enhanced_object.image, LUT)
+            print("Gamma adjusted...")
+        if self.image.dtype == "uint8":
+            enhanced_image[enhanced_image > 255] = 255
 
-        enhanced_object.log.append('enhanced_object()')
+        enhanced_object.log.append("enhanced_object()")
         return enhanced_object
 
     def eqHist(self):
-        '''
-        Spreads the contrast across a range of values, leading to an evened, flattened histogram. This can be very effective at enhancing midtones in images with very bright or very dark patches. 
-        
+        """
+        Spreads the contrast across a range of values, leading to an evened, flattened histogram. This can be very effective at enhancing midtones in images with very bright or very dark patches.
+
         Returns
         -------
             Contrast_enhanced_micrograph : Micrograph
                 Return a copy of the object with the contrast enhanced.
 
-        '''
+        """
         enhanced_object = deepcopy(self)
         enhanced_object = enhanced_object.convert_to_8bit()
         enhanced_object.image = cv.equalizeHist(enhanced_object.image)
-        enhanced_object.log.append('eqHist()')
+        enhanced_object.log.append("eqHist()")
         return enhanced_object
 
-
-    def local_normalisation(self,numpatches, padding=15, pad=True):
+    def local_normalisation(self, numpatches, padding=15, pad=True):
         """
-        Normalises contrast across the image, ensuring even contrast throughout. 
+        Normalises contrast across the image, ensuring even contrast throughout.
         Image is taken and split into patches, following which the median of the patches ('local median') is compared to the median of the image ('global median').
-        The patch (local area) is then normalised using the medians (patch = patch* global_median/local_medium) leading to a uniform contrast in the image. 
+        The patch (local area) is then normalised using the medians (patch = patch* global_median/local_medium) leading to a uniform contrast in the image.
+
+        The patch median was chosen so there would be less effect if there is a large dark/bright particle, however if this is too large compared with the patch size it will affect the resulting contrast.
 
-        The patch median was chosen so there would be less effect if there is a large dark/bright particle, however if this is too large compared with the patch size it will affect the resulting contrast. 
-        
         Padding can be applied which will greatly reduce edge artefacts. However doing this well will greatly increase the run time.
         Note: if there is a black region (eg. edge of beam or grid) in the image this may lead to bad results.
 
         Parameters
         ----------
 
             numpatches:int
-                The number of patches on each axis to split the image into, ie image is split into n x n patches and these are given the same median 
+                The number of patches on each axis to split the image into, ie image is split into n x n patches and these are given the same median
 
             padding: int
                 percentage overlap between patches (only used if pad=True)
-            
+
             pad:bool
-                Setting to true reduces edge artifacts from the patches of the image, however it also greatly increases processing time. 
+                Setting to true reduces edge artifacts from the patches of the image, however it also greatly increases processing time.
 
         Returns
         -------
 
             new_im: Micrograph
-                Copy of the object with an image that has been locally normalised 
-                
+                Copy of the object with an image that has been locally normalised
+
         """
         new_im = deepcopy(self)
         if pad:
             arrs = []
         else:
-            padding=0
-        xconst = int(new_im.image.shape[0]/numpatches)
-        yconst = int(new_im.image.shape[1]/numpatches)
-        x_coords = [i*xconst for i in range(numpatches)]
-        y_coords = [i*yconst for i in range(numpatches)]
+            padding = 0
+        xconst = int(new_im.image.shape[0] / numpatches)
+        yconst = int(new_im.image.shape[1] / numpatches)
+        x_coords = [i * xconst for i in range(numpatches)]
+        y_coords = [i * yconst for i in range(numpatches)]
         patch_coords = list(itertools.product(x_coords, y_coords))
         global_median = np.median(new_im.image)
         for coord in patch_coords:
-            
             x_low = coord[0]
-            x_high = coord[0]+xconst+int((padding/100)*xconst)
+            x_high = coord[0] + xconst + int((padding / 100) * xconst)
             y_low = coord[1]
-            y_high = coord[1]+yconst+int((padding/100)*yconst)
-            
-            #local_mean = new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)].mean()
-            #.mean()
+            y_high = coord[1] + yconst + int((padding / 100) * yconst)
+
+            # local_mean = new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)].mean()
+            # .mean()
             local_patch = new_im.image[x_low:x_high, y_low:y_high]
             local_median = np.median(local_patch)
-            local_patch = local_patch*global_median/local_median
+            local_patch = local_patch * global_median / local_median
 
             if pad:
-                empty_arr = np.zeros_like(new_im.image, dtype='float32')
-                empty_arr[:]=np.nan
-                empty_arr[x_low:x_high, y_low:y_high]=local_patch
+                empty_arr = np.zeros_like(new_im.image, dtype="float32")
+                empty_arr[:] = np.nan
+                empty_arr[x_low:x_high, y_low:y_high] = local_patch
                 arrs.append(empty_arr)
-            else:    
-                new_im.image[x_low:x_high, y_low:y_high]=local_patch
-        new_im.log.append('local_normalisation')
+            else:
+                new_im.image[x_low:x_high, y_low:y_high] = local_patch
+        new_im.log.append("local_normalisation")
         if pad:
             arrs = np.array(arrs)
             new_arr = np.nanmean(arrs, axis=0)
-            new_im.image= new_arr
+            new_im.image = new_arr
             return new_im
-            #new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)]= new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)]*(image.mean()/new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)].mean())
-        #if numpatches>2:
+            # new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)]= new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)]*(image.mean()/new_im[coord[0]-xconst:int(coord[0]+xconst*padding), coord[1]-yconst:int(coord[1]+yconst*padding)].mean())
+        # if numpatches>2:
         #    new_im = normalise_across_image(new_im, numpatches-1, padding)
         else:
             return new_im
 
-    '''-----------------------------------------------------------------------------------------------------------------------
+    """-----------------------------------------------------------------------------------------------------------------------
     SECTION: SCALEBAR
 
         Adds well-sized scalebar to the image. use make_scalebar function for use. 
 
 
 
 
-    '''
+    """
+
     def change_scale_unit(self, new_unit, scaling_factor=None):
-        '''
-        Function to change the unit of the scale in the image. The method is built to allow easy transfer between nanometers ('nm') and microns ('µm'), however can be used to give any new unit providing a scaling factor to multiply the current value by is included. 
+        """
+        Function to change the unit of the scale in the image. The method is built to allow easy transfer between nanometers ('nm') and microns ('µm'), however can be used to give any new unit providing a scaling factor to multiply the current value by is included.
 
         Parameters
         ----------
 
             new_unit : str
                 The new unit for the scale, commonly 'nm' or 'µm'
 
             scaling_factor: int/float
                 The value to multiply the current value by to give the new scale. This isnt necessary with 'µm'/'nm' transitions, but without it any other change will change unit only.
 
-        '''
-        if new_unit==self.pixel_unit:
-
-            print('The unit is already {}! Skipping file.'.format(new_unit))
-        elif new_unit=='nm' and self.pixel_unit=='µm':
-            self.pixel_size*=1000
-            self.pixel_unit='nm'
-        elif new_unit!='nm' and new_unit!='µm':
-            self.pixel_unit=new_unit
+        """
+        if new_unit == self.pixel_unit:
+            print("The unit is already {}! Skipping file.".format(new_unit))
+        elif new_unit == "nm" and self.pixel_unit == "µm":
+            self.pixel_size *= 1000
+            self.pixel_unit = "nm"
+        elif new_unit != "nm" and new_unit != "µm":
+            self.pixel_unit = new_unit
 
-            if scaling_factor !=None:
-                self.pixel_size*=scaling_factor
+            if scaling_factor != None:
+                self.pixel_size *= scaling_factor
             else:
-                print('Setting new scale unit but not changing the value, please include a scaling factor to also change the value.')
-        elif new_unit=='µm' and self.pixel_unit=='nm':
-            self.pixel_size= self.pixel_size/1000
-            self.pixel_unit='µm'
-
-        elif self.pixel_unit not in ['µm', 'nm'] and new_unit in ['µm','nm'] and scaling_factor==None:
-            print("Error! You want to switch to {} but the transition from {} is not naturally supported, please include a scaling factor (even if its just 1) to ensure correct conversion.".format(new_unit,self.pixel_unit))
-        elif self.pixel_unit not in ['µm', 'nm'] and new_unit in ['µm','nm'] and scaling_factor!=None:
-            self.pixel_size*=scaling_factor
-            self.pixel_unit=new_unit
+                print(
+                    "Setting new scale unit but not changing the value, please include a scaling factor to also change the value."
+                )
+        elif new_unit == "µm" and self.pixel_unit == "nm":
+            self.pixel_size = self.pixel_size / 1000
+            self.pixel_unit = "µm"
+
+        elif (
+            self.pixel_unit not in ["µm", "nm"]
+            and new_unit in ["µm", "nm"]
+            and scaling_factor == None
+        ):
+            print(
+                "Error! You want to switch to {} but the transition from {} is not naturally supported, please include a scaling factor (even if its just 1) to ensure correct conversion.".format(
+                    new_unit, self.pixel_unit
+                )
+            )
+        elif (
+            self.pixel_unit not in ["µm", "nm"]
+            and new_unit in ["µm", "nm"]
+            and scaling_factor != None
+        ):
+            self.pixel_size *= scaling_factor
+            self.pixel_unit = new_unit
 
         else:
-            print('Not sure how we got here! Check inputs and try again - if genuine error, raise an issue on github!')
-        self.log.append('change_scale_unit({}, {})'.format(new_unit, scaling_factor))
+            print(
+                "Not sure how we got here! Check inputs and try again - if genuine error, raise an issue on github!"
+            )
+        self.log.append("change_scale_unit({}, {})".format(new_unit, scaling_factor))
 
     def set_scale(self, pixels, dist, unit):
-        '''
+        """
         Set the scale in the image with a measurement (number of pixels and size, with unit)
-        
+
         Parameters
         ----------
-        
+
             pixels : int/float
                 Number of pixels measured
 
             dist : int/float
                 Distance measured
             unit : str
                 Unit of measurement
 
-        '''
-        self.pixel_size=dist/pixels
-        self.pixel_unit=unit
-        self.log.append('set_scale({},{},{})'.format(pixels, dist, unit))
+        """
+        self.pixel_size = dist / pixels
+        self.pixel_unit = unit
+        self.log.append("set_scale({},{},{})".format(pixels, dist, unit))
 
     def choose_scalebar_size(self):
-        '''
+        """
         Function for choosing scalebar size, called through make_scalebar(), not a standalone function.
 
         Returns
         -------
             scalebar_x: int
-                x coordinate for the scalebar 
+                x coordinate for the scalebar
             scalebar_y: int
-                y coordinate for the scalebar 
+                y coordinate for the scalebar
             width:int
                 width of scalebar
             height:int
                 height of the scalebar
             scalebar_size:int (or float)
                 Size of the scalebar in scaled units (pixel_unit)
-        '''
-        y,x = self.image.shape
-        
-        #make coordinates for the scalebar, currently set to y-12.5%,x-5% of image size from the bottom right corner 
-        #of the image to bottom left of the scalebar - change this by editing /20 and /7.5 values (this just looked good to me)
-        scalebar_y = y-int(y/25)
-        scalebar_x = x-int(x/6.5)
-        #print(x,scalebar_x)
-
-        #possible scalebar sizes are given here, if its >500nm it should be in unit micron
-        
-        possible_sizes = [0.5, 1,2,5,10,25,50,100,250,500,1000]
-        
-        #to select sizes, iterate through possible sizes, if the width of the resulting scalebar (n*pixelsize) 
-        #is over 15% of the image size, the size is chose, if none are over 15% of image size
-        #the largest size is chosen as default
+        """
+        y, x = self.image.shape
+
+        # make coordinates for the scalebar, currently set to y-12.5%,x-5% of image size from the bottom right corner
+        # of the image to bottom left of the scalebar - change this by editing /20 and /7.5 values (this just looked good to me)
+        scalebar_y = y - int(y / 25)
+        scalebar_x = x - int(x / 6.5)
+        # print(x,scalebar_x)
+
+        # possible scalebar sizes are given here, if its >500nm it should be in unit micron
+
+        possible_sizes = [0.5, 1, 2, 5, 10, 25, 50, 100, 250, 500, 1000]
+
+        # to select sizes, iterate through possible sizes, if the width of the resulting scalebar (n*pixelsize)
+        # is over 15% of the image size, the size is chose, if none are over 15% of image size
+        # the largest size is chosen as default
         for n in possible_sizes:
-            width = int(n*1/self.pixel_size)
-            #print(n, image.shape([0]/10)
-            if width>(x/15):
+            width = int(n * 1 / self.pixel_size)
+            # print(n, image.shape([0]/10)
+            if width > (x / 15):
                 break
-        
-        # This if statement checks whether the scalebar is too close to the edge or bigger than the size. 
+
+        # This if statement checks whether the scalebar is too close to the edge or bigger than the size.
         # This should ensure it is at least one 100th of the image width away from the edge.
 
-        if scalebar_x+width>=x:
+        if scalebar_x + width >= x:
             print(True)
-            diff = x - scalebar_x+width
-            scalebar_x=scalebar_x-diff - x/100
-        elif scalebar_x+width+x/100 > x:
-            scalebar_x=scalebar_x-x/100
-
-        #choose height of scalebar (default is scalebar width/6), convert width into an integer
-        height = int(y/60)
-        width = int(width)   
+            diff = x - scalebar_x + width
+            scalebar_x = scalebar_x - diff - x / 100
+        elif scalebar_x + width + x / 100 > x:
+            scalebar_x = scalebar_x - x / 100
+
+        # choose height of scalebar (default is scalebar width/6), convert width into an integer
+        height = int(y / 60)
+        width = int(width)
         scalebar_x = int(scalebar_x)
         scalebar_y = int(scalebar_y)
         scalebar_size = n
-        #return int(scalebar_x/xybin), int(scalebar_y/xybin), int(height/xybin), int(width/xybin), n
+        # return int(scalebar_x/xybin), int(scalebar_y/xybin), int(height/xybin), int(width/xybin), n
         return scalebar_x, scalebar_y, width, height, scalebar_size
 
-
-    def choose_scalebar_color(self,color, scalebar_x, scalebar_y, width, height):
-        '''
+    def choose_scalebar_color(self, color, scalebar_x, scalebar_y, width, height):
+        """
         Chooses the scalebar color and returns the pixelvalue and text color for the annotation. parameters are most of the outputs from choose_scalebar_size()
 
 
         Parameters
         ----------
 
             scalebar_x: int
-                x coordinate for the scalebar 
+                x coordinate for the scalebar
             scalebar_y: int
-                y coordinate for the scalebar 
+                y coordinate for the scalebar
             width:int
                 width of scalebar
             height:int
                 height of the scalebar
             scalebar_size:int (or float)
                 Size of the scalebar in scaled units (pixel_unit)
-        '''
-        if color=='black' or self.image.dtype!='uint8':
+        """
+        if color == "black" or self.image.dtype != "uint8":
             pixvalue = 0
-            textcolor = 'black'
-        elif color=='white':
+            textcolor = "black"
+        elif color == "white":
             pixvalue = 255
-            textcolor='white'
-        elif color=='grey':
+            textcolor = "white"
+        elif color == "grey":
             pixvalue = 150
-            textcolor='grey'
-        else: #default is black, unless it is a particularly dark area - if the mean pixvalue of the scale bar region is significantly less than the overall image mean, the scalebar will be white
-            
-            if np.mean(self.image[scalebar_y:scalebar_y+height,scalebar_x:scalebar_x+width])<np.mean(self.image)/1.5:
+            textcolor = "grey"
+        else:  # default is black, unless it is a particularly dark area - if the mean pixvalue of the scale bar region is significantly less than the overall image mean, the scalebar will be white
+            if (
+                np.mean(
+                    self.image[
+                        scalebar_y : scalebar_y + height,
+                        scalebar_x : scalebar_x + width,
+                    ]
+                )
+                < np.mean(self.image) / 1.5
+            ):
                 pixvalue = 255
-                textcolor='white'
+                textcolor = "white"
             else:
                 pixvalue = 0
-                textcolor = 'black'
-        #add scalebar (set pixels to color) 
+                textcolor = "black"
+        # add scalebar (set pixels to color)
 
-        return pixvalue, textcolor        
+        return pixvalue, textcolor
 
-
-    def make_scalebar(self, texton = True, color='Auto', fontsize='M'):
-        '''
-        Automated method to create a scalebar of a suitable size, shape and color. Returns a new object with a scalebar. 
+    def make_scalebar(self, texton=True, color="Auto", fontsize="M"):
+        """
+        Automated method to create a scalebar of a suitable size, shape and color. Returns a new object with a scalebar.
         The color will be selected between black and white based on mean value of the region of the scalebar compared to the mean value of the whole video. To override this the color can be defined as black white or grey.
-        This will work best for 8-bit images, as the scalebar will be given values of 0 or 255. 
-        
+        This will work best for 8-bit images, as the scalebar will be given values of 0 or 255.
+
         Parameters
         ----------
 
             color : str
                 The color of the scalebar, the options are 'white'. 'black' or 'grey'
             texton : bool
                 Text can be turned off using texton=False, the selected size of the scalebar can be accessed using micrograph.scalebar_size
             fontsize : str or int
-                Can choose S, M, L, XL for size of the text on the scalebar, or an integer value for size. 
+                Can choose S, M, L, XL for size of the text on the scalebar, or an integer value for size.
 
         Returns
         -------
             Micrograph_object_with_scalebar: Micrograph
                 Copy of the micrograph object with a scale bar.
-        '''
+        """
 
         micrograph_SB = deepcopy(self)
-        scalebar_x, scalebar_y , width, height, scalebar_size = self.choose_scalebar_size()
-        
-        pixvalue, textcolor = self.choose_scalebar_color(color,scalebar_x, scalebar_y , width, height)
-
-        micrograph_SB.image[scalebar_y:scalebar_y+height,scalebar_x:scalebar_x+width]=pixvalue
-        
-        textposition = ((scalebar_x+width/2),scalebar_y-5)
-        
-        #if pixel_unit!='nm':
-         #   Utext = str(n)+u'\u00b5'+ 'm'
-          #  text = str(n)+'microns'
-        #else:
-        micrograph_SB.scalebar_size = '{}{}'.format(scalebar_size,self.pixel_unit) 
-         
+        (
+            scalebar_x,
+            scalebar_y,
+            width,
+            height,
+            scalebar_size,
+        ) = self.choose_scalebar_size()
+
+        pixvalue, textcolor = self.choose_scalebar_color(
+            color, scalebar_x, scalebar_y, width, height
+        )
+
+        micrograph_SB.image[
+            scalebar_y : scalebar_y + height, scalebar_x : scalebar_x + width
+        ] = pixvalue
+
+        textposition = ((scalebar_x + width / 2), scalebar_y - 5)
+
+        # if pixel_unit!='nm':
+        #   Utext = str(n)+u'\u00b5'+ 'm'
+        #  text = str(n)+'microns'
+        # else:
+        micrograph_SB.scalebar_size = "{}{}".format(scalebar_size, self.pixel_unit)
 
         pil_image = Image.fromarray(micrograph_SB.image)
 
-        if texton==True:
-            #print('textoff')
-            if fontsize=='M':
-                fontsize=int(scalebar_x/(25))
-            elif fontsize=='L':
-                fontsize=int(scalebar_x/(20))
-            elif fontsize=='XL':
-                fontsize=int(scalebar_x/(17))
-            elif fontsize=='S':
-                fontsize=int(scalebar_x/(30))
+        if texton == True:
+            # print('textoff')
+            if fontsize == "M":
+                fontsize = int(scalebar_x / (25))
+            elif fontsize == "L":
+                fontsize = int(scalebar_x / (20))
+            elif fontsize == "XL":
+                fontsize = int(scalebar_x / (17))
+            elif fontsize == "S":
+                fontsize = int(scalebar_x / (30))
             print(fontsize)
-            draw = ImageDraw.Draw(pil_image)        
-            
-            #fontsize=int(scalebar_x/(25))
+            draw = ImageDraw.Draw(pil_image)
+
+            # fontsize=int(scalebar_x/(25))
             try:
-                file = font_manager.findfont('Helvetica')
+                file = font_manager.findfont("Helvetica")
                 font = ImageFont.truetype(file, fontsize)
             except:
-                font_search = font_manager.FontProperties(family='sans-serif', weight='normal')
+                font_search = font_manager.FontProperties(
+                    family="sans-serif", weight="normal"
+                )
                 file = font_manager.findfont(font_search)
                 font = ImageFont.truetype(file, fontsize)
-            draw.text(textposition, micrograph_SB.scalebar_size, anchor ='mb', fill=textcolor, font=font, stroke_width=1)
-            micrograph_SB.image = np.array(pil_image)    
+            draw.text(
+                textposition,
+                micrograph_SB.scalebar_size,
+                anchor="mb",
+                fill=textcolor,
+                font=font,
+                stroke_width=1,
+            )
+            micrograph_SB.image = np.array(pil_image)
 
-        micrograph_SB.log.append('make_scalebar()')
+        micrograph_SB.log.append("make_scalebar()")
         return micrograph_SB
 
-
-    '''------------------------------------------------------------------------------------------------------------------------
+    """------------------------------------------------------------------------------------------------------------------------
         SECTION: IMAGE FILTERS
         These are filters to improve the visibility of features or decrease the noise levels. Included features are 
             
             - Median filter: performs a median filter with kernal size defined in the call (default is 3)
             - Gaussian filter: performs a Gaussian filter with kernal size defined in the call (default is 3)
             - Weiner filter: performs a Weiner filter with kernal size defined in the call (default is 5)
             - Low pass filter: performs a 2D fourier transform of the image and removes the  features at higher resolutions than the radius 
@@ -966,787 +1054,878 @@
     Therefore to use: 
 
         filtered_micrograph = micrograph.gaussian_filter()
         plt.imshow(filtered_micrograph.image)
         filtered_micrograph.make_scalebar()
 
 
-    '''
+    """
+
     def low_pass_filter(self, radius):
-        '''
+        """
         This low pass filters the image. The pixel size is used to scale the radius to whatever the pixel unit is (ie radius 10 is 10nm/10um)
         If pixelsize is undefined the radius will refer to pixels only
-        
+
         Parameters
         ----------
 
             radius : int (or potentially float)
-                The effects of this vary depending on if the pixelsize is defined in self.pixel_size.: 
-                     - Assuming your micrograph object has a pixel size defined, the filter works by removing any features smaller than the size you input as a parameter (the unit is the same as the pixelsize), A larger number yields a stronger filter, if it is too large, you won't see any features. 
+                The effects of this vary depending on if the pixelsize is defined in self.pixel_size.:
+                     - Assuming your micrograph object has a pixel size defined, the filter works by removing any features smaller than the size you input as a parameter (the unit is the same as the pixelsize), A larger number yields a stronger filter, if it is too large, you won't see any features.
                     Effective filter sizes depends on features and magnification, so with something between 1-5 and tune it to your needs.
                     - If your micrograph is missing a pixelsize the size input will be the radius of a circle kept in the power spectrum. Here the input number does the inverse - a smaller number leads to stronger filter. In this case, much larger numbers will be needed, 50 is a good starting value.
-        
+
         Returns
         -------
                 Low_pass_filtered_object :Micrograph
-                    Low pass filtered copy of micrograph object.          
+                    Low pass filtered copy of micrograph object.
+
+        """
+        N = self.image.shape[0]
+        if (
+            type(self.pixel_size) == int
+            or type(self.pixel_size) == float
+            and self.pixel_size != 0
+        ):
+            radius = int((N * self.pixel_size) / radius)
 
-        '''    
-        N=self.image.shape[0]
-        if type(self.pixel_size)==int or type(self.pixel_size)==float and self.pixel_size!=0:
-            radius=int((N*self.pixel_size)/radius)
-        
-            
         fft = np.fft.fft2(self.image)
         fshift = np.fft.fftshift(fft)
         magnitude_spectrum = np.log(np.abs(fshift))
         rows, cols = self.image.shape
-        crow, ccol = int(rows/2), int(cols/2)
-        fshift_filtered=np.copy(fshift)
+        crow, ccol = int(rows / 2), int(cols / 2)
+        fshift_filtered = np.copy(fshift)
         mask = np.zeros_like(self.image)
 
-        mask = cv.circle(cv.UMat(mask), (crow, ccol),radius*2, 1, -1) 
-        #print(fshift_filtered)
+        mask = cv.circle(cv.UMat(mask), (crow, ccol), radius * 2, 1, -1)
+        # print(fshift_filtered)
         mask = mask.get()
-        fcomplex = fshift[:,:]*1j
-        fshift_filtered = mask*fcomplex
+        fcomplex = fshift[:, :] * 1j
+        fshift_filtered = mask * fcomplex
         f_filtered_shifted = np.fft.fftshift(fshift_filtered)
-        #magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
+        # magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
         inv_image = np.fft.ifft2(f_filtered_shifted)
         filtered_image = np.abs(inv_image)
         filtered_image -= filtered_image.min()
         filtered_object = deepcopy(self)
         filtered_object.image = filtered_image
 
-        filtered_object.log.append('low_pass_filter({})'.format(radius))
+        filtered_object.log.append("low_pass_filter({})".format(radius))
         return filtered_object
 
     def median_filter(self, kernal=3):
-        '''
+        """
         Returns a median filtered copy of the micrograph object, kernal size defined in the call (default is 3)
 
             Parameters
             ----------
                 kernal:int
                     The n x n kernal for median filter is defined here, must be an odd integer
 
             Returns
             -------
                 Median_filtered_object :Micrograph
                     Median filtered copy of micrograph object with median filtered image
-        '''
-        filtered_image = cv.medianBlur(self.image,kernal)
+        """
+        filtered_image = cv.medianBlur(self.image, kernal)
         filtered_object = deepcopy(self)
         filtered_object.image = filtered_image
-        filtered_object.log.append('median_filter()')
+        filtered_object.log.append("median_filter()")
         return filtered_object
 
     def weiner_filter(self, kernal=5):
-        '''
+        """
         Returns a Weiner filtered copy of the micrograph object, kernal size defined in the call (default is 5)
 
             Parameters
             ----------
 
                 n :int
                     The n x n kernal for Weiner filter is defined here, must be an odd integer
 
             Returns
             -------
 
                 Weiner_filtered_object : Micrograph
-                    Weiner filtered copy of micrograph object 
-        '''
+                    Weiner filtered copy of micrograph object
+        """
         filtered_image = wiener(self.image, (kernal, kernal))
         filtered_object = deepcopy(self)
         filtered_object.image = filtered_image
-        filtered_object.log.append('weiner_filter()')
+        filtered_object.log.append("wiener_filter()")
         return filtered_object
 
     def nlm_filter(self, h=5):
-        '''
-        Returns a non-local means filtered copy of the micrograph, filter strength is defined in the call. 
+        """
+        Returns a non-local means filtered copy of the micrograph, filter strength is defined in the call.
         More information on non-local means filtering can be found here: https://docs.opencv.org/3.4/d5/d69/tutorial_py_non_local_means.html
 
             Parameters
             ----------
                 h:int
                     Defines the strength of the Non-local means filter, default is 5
             Returns
             -------
                 nlm_filtered_object : Micrograph
                     Non-local means filtered copy of the micrograph object
-        '''
+        """
         filtered_image = cv.fastNlMeansDenoising(np.uint8(self.image), h)
         filtered_object = deepcopy(self)
         filtered_object.image = filtered_image
-        filtered_object.log.append('nlm_filter()')
+        filtered_object.log.append("nlm_filter()")
         return filtered_object
 
     def gaussian_filter(self, kernal=3):
-        '''
+        """
         Returns a Gaussian filtered copy of the micrograph object, kernal size defined in the call (default is 3)
 
             Parameters
             ----------
                 n:int
                     The n x n kernal for median filter is defined here, *must be an odd integer*
 
             Returns
             -------
                 Gaussian_filtered_object :Micrograph
                     Gaussian filtered copy of micrograph object with gaussian filtered image
-        '''
-        filtered_image = cv.GaussianBlur(self.image, (kernal,kernal),0)
+        """
+        filtered_image = cv.GaussianBlur(self.image, (kernal, kernal), 0)
         filtered_object = deepcopy(self)
         filtered_object.image = filtered_image
-        filtered_object.log.append('gaussian_filter()')
+        filtered_object.log.append("gaussian_filter()")
 
         return filtered_object
 
+    def topaz_denoise(
+        self,
+        model="unet",
+        use_cuda=False,
+        lowpass=0,
+        cutoff=0,
+        gaus=None,
+        inv_gaus=None,
+        deconvolve=False,
+        deconv_patch=1,
+        patch_size=1024,
+        padding=200,
+        normalize=False,
+    ):
+        """
+        Denoise micrograph with topaz denoiser.
 
-    def topaz_denoise(self, model='unet', use_cuda=False, lowpass=0, cutoff=0, \
-                gaus=None,inv_gaus=None ,deconvolve=False,deconv_patch=1, \
-                patch_size=1024, padding=200, normalize=False):
-        '''
-        Denoise micrograph with topaz denoiser. 
-
-        Topaz (https://doi.org/10.1038/s41467-020-18952-1) is a pre-trained implementation of the deeplearning based noise2noise method (https://doi.org/10.48550/arXiv.1803.04189). 
+        Topaz (https://doi.org/10.1038/s41467-020-18952-1) is a pre-trained implementation of the deeplearning based noise2noise method (https://doi.org/10.48550/arXiv.1803.04189).
         It has been specifically trained on cryo-EM datasets but works pretty well for dryTEM and liquid-TEM images and videos. It is very effective at reducing noise and enhancing lower resolution features, although is not necessarily trustworthy for high resolution data.
-        Use with caution, but it is a powerful method. 
-        
-        Best to only perform on a machine with high RAM and ideally a CUDA GPU, as can take a long time with lesser computers. 
+        Use with caution, but it is a powerful method.
+
+        Best to only perform on a machine with high RAM and ideally a CUDA GPU, as can take a long time with lesser computers.
         If topaz is not installed, simply type `pip install topaz-em` into the command line.
 
-        Unfortunately bespoke training is not currently included in SimpliPyTEM, so please use Topaz to train your own model. 
+        Unfortunately bespoke training is not currently included in SimpliPyTEM, so please use Topaz to train your own model.
 
         Parameters
         ----------
             The parameters here are not required for running with default options, these are available through the topaz code and thus documentation for more advanced options can be found in topaz documentation (https://github.com/tbepler/topaz/, https://topaz-em.readthedocs.io/en/latest/?badge=latest)
-            The important parameters are which model is used, and whether to use a cuda GPU: 
+            The important parameters are which model is used, and whether to use a cuda GPU:
 
             model: str
                 Which topaz denoising model is used, options are ['unet', 'unet-small', 'fcnn', 'affine', 'unet-v0.2.1']
             use_cuda: bool
-                Use CUDA gpu(s)? true or false. 
-            
-            
+                Use CUDA gpu(s)? true or false.
+
+
         Topaz Parameters
         ----------------
 
-            These are parameters 
+            These are parameters
 
 
-        '''
-        
-        from topaz.commands import denoise
+        """
+
         import topaz.denoise as dn
-        
+        from topaz.commands import denoise
+
         mic = self.image.copy()
-        mic = mic.astype('float32')
+        mic = mic.astype("float32")
 
         im_denoised = deepcopy(self)
 
         mic = im_denoised.image
-        mic = mic.astype('float32')
-
+        mic = mic.astype("float32")
 
-        if gaus!= None and gaus>0:
+        if gaus != None and gaus > 0:
             gaus = dn.GaussianDenoise(gaus)
             if use_cuda:
                 gaus.cuda()
         else:
             gaus = None
-            
-        if inv_gaus!= None and inv_gaus>0:
+
+        if inv_gaus != None and inv_gaus > 0:
             inv_gaus = dn.InvGaussianFilter(inv_gaus)
             if use_cuda:
                 inv_gaus.cuda()
         else:
             inv_gaus = None
-        
 
         model = dn.load_model(model)
         if use_cuda:
             model.cuda()
-        output = denoise.denoise_image(mic, [model], lowpass=lowpass, cutoff=cutoff, gaus=gaus,\
-                                       inv_gaus=inv_gaus ,deconvolve=deconvolve,deconv_patch=deconv_patch,\
-                                       patch_size=1024, padding=200, normalize=False, use_cuda=use_cuda)
-        
+        output = denoise.denoise_image(
+            mic,
+            [model],
+            lowpass=lowpass,
+            cutoff=cutoff,
+            gaus=gaus,
+            inv_gaus=inv_gaus,
+            deconvolve=deconvolve,
+            deconv_patch=deconv_patch,
+            patch_size=1024,
+            padding=200,
+            normalize=False,
+            use_cuda=use_cuda,
+        )
+
         im_denoised.image = output
 
         return im_denoised
 
-
-
-    '''
+    """
     ------------------------------------------------------------------------------------------------------------
     Section Visualising images
 
     used for plotting images using matplotlib. Functions very basic so only meant for rapid use, for better figures write own function or use save command
 
-    '''
-    def imshow(self, title='', vmax=None, vmin=None):
-        '''
+    """
+
+    def imshow(self, title="", vmax=None, vmin=None):
+        """
         Basic function for plotting the micrograph image
 
         Parameters
         ----------
 
             title:str
-                Optional title to be added to the plot 
-            
+                Optional title to be added to the plot
+
             vmax: int/float
                 The 'white value' when plotting the image, such that anything above this value is set to white.
-            
+
             vmin: int/float
                 The 'black value' when plotting the image, such that anything below this value is set to black.
-        '''
-        plt.subplots(figsize=(20,10))
+        """
+        plt.subplots(figsize=(20, 10))
 
         if not vmax:
             vmax = self.image.max()
         if not vmin:
             vmin = self.image.min()
 
-
         plt.imshow(self.image, vmax=vmax, vmin=vmin)
-        if title!='':
+        if title != "":
             plt.title(title, fontsize=20)
         plt.show()
 
-    def show_pair(self,other_image, title1='', title2=''):
-        '''
-        Basic function for plotting pairs of images for comparison 
+    def show_pair(self, other_image, title1="", title2=""):
+        """
+        Basic function for plotting pairs of images for comparison
 
         Parameters
         ----------
             other_image : 2D Numpy array
                 Second image of the plot - if using Micrograph object remember to use micrograph.image
             title1 : str
                 Title for the first image (the object being used to plot the images) - Optional
             title2 : str
-                Title for the second image - Optional 
+                Title for the second image - Optional
 
-        '''
+        """
 
-        if str(type(other_image))=="<class 'SimpliPyTEM.Micrograph_class.Micrograph'>":
+        if (
+            str(type(other_image))
+            == "<class 'SimpliPyTEM.Micrograph_class.Micrograph'>"
+        ):
             other_image = other_image.image
-        fig, ax = plt.subplots(1,2, figsize=(20,10))
+        fig, ax = plt.subplots(1, 2, figsize=(20, 10))
         ax[0].imshow(self.image)
-        if title1!='':
+        if title1 != "":
             ax[0].set_title(title1, fontsize=20)
 
         ax[1].imshow(other_image)
-        if title2!='':
+        if title2 != "":
             ax[1].set_title(title2, fontsize=20)
         plt.show()
 
     def plot_histogram(self, sidebyside=False, vmax=None, vmin=None):
-        '''
+        """
         Function to plot a histogram of the image values. This can be done on its own or side by side with the image.
-        
+
         Parameters
         ----------
             sidebyside:bool
                 Show the image next to the histogram? True or False (default is False)
 
             vmax: int/float
                 The 'white value' when plotting the image, such that anything above this value is set to white.
-            
+
             vmin: int/float
                 The 'black value' when plotting the image, such that anything below this value is set to black.
 
-    
-        '''
-        if sidebyside:
 
+        """
+        if sidebyside:
             if not vmax:
                 vmax = self.image.max()
             if not vmin:
                 vmin = self.image.min()
 
-            fig, ax = plt.subplots(1,2, figsize=(20,10))
+            fig, ax = plt.subplots(1, 2, figsize=(20, 10))
             ax[0].imshow(self.image, vmax=vmax, vmin=vmin)
-            ax[0].tick_params(axis='x', labelsize=20)
-            ax[0].tick_params(axis='y', labelsize=20)
-            if self.image.dtype == 'unit8':
-                ax[1].hist(self.image.ravel(), 256, [0,256])
+            ax[0].tick_params(axis="x", labelsize=20)
+            ax[0].tick_params(axis="y", labelsize=20)
+            if self.image.dtype == "unit8":
+                ax[1].hist(self.image.ravel(), 256, [0, 256])
             else:
                 ax[1].hist(self.image.ravel(), 100)
-            ax[1].set_xlabel('Pixel Values', fontsize=20)
-            ax[1].set_ylabel('Frequency',fontsize=20)
-            ax[1].tick_params(axis='x', labelsize=20)
-            ax[1].tick_params(axis='y', labelsize=20)
+            ax[1].set_xlabel("Pixel Values", fontsize=20)
+            ax[1].set_ylabel("Frequency", fontsize=20)
+            ax[1].tick_params(axis="x", labelsize=20)
+            ax[1].tick_params(axis="y", labelsize=20)
         else:
-            plt.figure(figsize=(8,5))
-            if self.image.dtype == 'unit8':
-                plt.hist(self.image.ravel(), 256, [0,256])
+            plt.figure(figsize=(8, 5))
+            if self.image.dtype == "unit8":
+                plt.hist(self.image.ravel(), 256, [0, 256])
             else:
                 plt.hist(self.image.ravel(), 100)
-            plt.xlabel('Pixel Values', fontsize=15)
-            plt.ylabel('Frequency',fontsize=15)
+            plt.xlabel("Pixel Values", fontsize=15)
+            plt.ylabel("Frequency", fontsize=15)
 
         plt.show()
 
-
-    def display_fft(self,sidebyside=False, vmax=None,vmin=None, ret=False):
-        '''
+    def display_fft(self, sidebyside=False, vmax=None, vmin=None, ret=False):
+        """
         Function to display or return the power-spectrum, or 2D fourier transform of the image. This can be useful to observe any periodic features, eg lattace lines, or Thon rings resulting from the contrast transfer function in the microscope.
 
 
         Parameters
         ----------
 
-            sidebyside:bool 
+            sidebyside:bool
                 Do you want to display the power spectrum next to the image? default is yes (True), change to False to see fft only
 
             vmax: int/float
                 The 'white value' when plotting the power spectrum, such that anything above this value is set to white.
-            
+
             vmin: int/float
                 The 'black value' when plotting the power spectrum, such that anything below this value is set to black.
-            
-            ret: bool 
+
+            ret: bool
                 Set to true if you want to return a copy of the fft as a micrograph object (with the fft as the .image parameter)
 
         Returns
         -------
 
-            If ret==True, a new micrograph object is returned with the power spectrum as the image, from here the same functions can be used 
+            If ret==True, a new micrograph object is returned with the power spectrum as the image, from here the same functions can be used
 
-        '''
+        """
         fft = np.fft.fft2(self.image)
         fshift = np.fft.fftshift(fft)
         magnitude_spectrum = np.log(np.abs(fshift))
         magnitude_spectrum = magnitude_spectrum.astype(np.float32)
 
-
         if not vmax:
             vmax = magnitude_spectrum.max()
         if not vmin:
             vmin = magnitude_spectrum.min()
-        #print(magnitude_spectrum.dtype)
-
-        if ret==True: 
+        # print(magnitude_spectrum.dtype)
 
+        if ret == True:
             fft_ob = Micrograph()
             fft_ob.image = magnitude_spectrum
-            filename = self.filename.split('.')[:-1]
-            filename.append('_FFT')
+            filename = self.filename.split(".")[:-1]
+            filename.append("_FFT")
             fft_ob.filename = filename
             return fft_ob
 
         if sidebyside:
-            fig,ax= plt.subplots(1,2, figsize=(30,20))
+            fig, ax = plt.subplots(1, 2, figsize=(30, 20))
             ax[0].imshow(self.image)
-            ax[0].set_title('Image')
+            ax[0].set_title("Image")
             ax[1].imshow(magnitude_spectrum, vmin=vmin, vmax=vmax)
-            ax[1].set_title('Power spectrum')
+            ax[1].set_title("Power spectrum")
             plt.show()
         else:
-            plt.figure(figsize=(20,20))
+            plt.figure(figsize=(20, 20))
             plt.imshow(magnitude_spectrum, vmin=vmin, vmax=vmax)
             plt.show()
 
-
-
-    '''--------------------------------------------------------------------------------
+    """--------------------------------------------------------------------------------
     SECTION: METADATA
 
         If a dm file has been opened, the metadata is saved in MicroVideo.metadata_tags, this is unformatted and awkward to use
         but all the raw data can be found. These methods allow easy extraction of some key metadata items: mag, voltage,
         exposure and aquisition date/time. 
-    '''
+    """
+
     def show_metadata(self):
-        '''
-        prints the metadata tags, this can be useful for finding the names of metadata features within the metadata.tags file. 
+        """
+        prints the metadata tags, this can be useful for finding the names of metadata features within the metadata.tags file.
 
-        '''
+        """
         for tag in self.metadata_tags:
-            print('{} : {}\n'.format(tag, self.metadata_tags[tag]))
-
+            print("{} : {}\n".format(tag, self.metadata_tags[tag]))
 
     def get_mag(self):
-        '''
-                
+        """
+
         Returns Micrograph magnifications (indicated and actual) and saves them as micrograph attributes (microscope.indicated_mag, microscope.actual_mag)
 
         Returns
         -------
 
             indicated_mag:float
                 Indicated magnification (i.e. what the microscope tells you the mag is) for the image
             actual_mag: float
-                Actual magnification of the image at the camera. 
-        
-        '''
+                Actual magnification of the image at the camera.
+
+        """
 
         try:
-            self.indicated_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Indicated Magnification']
+            self.indicated_mag = self.metadata_tags[
+                ".ImageList.2.ImageTags.Microscope Info.Indicated Magnification"
+            ]
         except KeyError:
             try:
-                self.indicated_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Formatted Indicated Mag']
-                  
+                self.indicated_mag = self.metadata_tags[
+                    ".ImageList.2.ImageTags.Microscope Info.Formatted Indicated Mag"
+                ]
+
             except KeyError:
-                print('Sorry, indicated mag cannot be located in tags, please find manually using .show_metadata()')
-        
+                print(
+                    "Sorry, indicated mag cannot be located in tags, please find manually using .show_metadata()"
+                )
+
         try:
-            self.actual_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Actual Magnification']
+            self.actual_mag = self.metadata_tags[
+                ".ImageList.2.ImageTags.Microscope Info.Actual Magnification"
+            ]
         except KeyError:
             try:
-                self.actual_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Formatted Actual Mag']
+                self.actual_mag = self.metadata_tags[
+                    ".ImageList.2.ImageTags.Microscope Info.Formatted Actual Mag"
+                ]
             except KeyError:
-                print('Sorry, actual mag cannot be located in tags, please find manually using .show_metadata()')
-
-
-        #self.indicated_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Indicated Magnification']
-        if hasattr(self, 'indicated_mag') and hasattr(self, 'actual_mag'):
-            #print('Indicated mag: {}'.format(self.indicated_mag))
-            #print('Actual mag: {}'.format(self.actual_mag))
+                print(
+                    "Sorry, actual mag cannot be located in tags, please find manually using .show_metadata()"
+                )
+
+        # self.indicated_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Indicated Magnification']
+        if hasattr(self, "indicated_mag") and hasattr(self, "actual_mag"):
+            # print('Indicated mag: {}'.format(self.indicated_mag))
+            # print('Actual mag: {}'.format(self.actual_mag))
             return self.indicated_mag, self.actual_mag
         else:
             return -1, -1
 
     def get_voltage(self):
-        '''
+        """
         Returns voltage and saves is as micrograph attribute
 
         Returns
         -------
 
             Voltage:int
                 Microscope voltage for the image
-        '''
+        """
         try:
-            self.voltage = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Voltage']
+            self.voltage = self.metadata_tags[
+                ".ImageList.2.ImageTags.Microscope Info.Voltage"
+            ]
             return self.voltage
         except KeyError:
-            print('Voltage was not found')
+            print("Voltage was not found")
             return -1
 
     def get_exposure(self):
-        '''
-        Prints and returns the exposure time for the image. 
+        """
+        Prints and returns the exposure time for the image.
 
         Returns
         -------
 
             exposure:int
                 Capture time for the image
-        '''
-        #print('Frame rate : {}fps'.format(self.fps))
-        #print('Exposure time per frame: {}s '.format(1/self.fps))
-        #print('Imaging time: {}s'.format(self.metadata_tags['.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)']))
+        """
+        # print('Frame rate : {}fps'.format(self.fps))
+        # print('Exposure time per frame: {}s '.format(1/self.fps))
+        # print('Imaging time: {}s'.format(self.metadata_tags['.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)']))
         try:
-            self.exposure = self.metadata_tags['.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)']
+            self.exposure = self.metadata_tags[
+                ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)"
+            ]
             return self.exposure
         except KeyError:
             return -1
 
-    def get_date_time(self): 
-        '''
-        Prints and returns the aquisition date and time for the image. 
+    def get_date_time(self):
+        """
+        Prints and returns the aquisition date and time for the image.
 
         Returns
         -------
 
             AqDate:str
                 Date on which the micrograph was captured
             AqTime:str
                 Time at which the micrograph was captured
-        '''
+        """
         try:
-            self.AqDate = self.metadata_tags['.ImageList.2.ImageTags.DataBar.Acquisition Date']
-            self.AqTime = self.metadata_tags['.ImageList.2.ImageTags.DataBar.Acquisition Time']
+            self.AqDate = self.metadata_tags[
+                ".ImageList.2.ImageTags.DataBar.Acquisition Date"
+            ]
+            self.AqTime = self.metadata_tags[
+                ".ImageList.2.ImageTags.DataBar.Acquisition Time"
+            ]
             return self.AqDate, self.AqTime
         except:
-            return 'UNK', 'UNK'
-        #print('Date: {} '.format(self.AqDate))
-        #print('Time {} '.format(self.AqTime))
-
+            return "UNK", "UNK"
+        # print('Date: {} '.format(self.AqDate))
+        # print('Time {} '.format(self.AqTime))
 
-
-    def export_metadata(self,name=None, outdir='.'):
-        
+    def export_metadata(self, name=None, outdir="."):
         make_outdir(outdir)
 
-
         if not name:
-            name='metadata.csv'
+            name = "metadata.csv"
 
         dt = self.get_date_time()
-        date_time = pd.to_datetime(dt[0]+' '+dt[1])
-    
-        metadata = {'Image name':self.filename, 'Indicated Magnification':self.get_mag()[0], 'Actual Magnifiation':self.get_mag()[1],  'Date':str(date_time.date()),'Time':str(date_time.time()), 'Pixel size':self.pixel_size,'Pixel unit':self.pixel_unit, 'Exposure Time (s)':self.get_exposure(), 'Voltage':self.get_voltage(), 'Size (px)':'{}x{}'.format(self.shape[1],self.shape[0]),'Video':self.video, 'Frame Rate (fps)':False,  'Number of frames':self.nframes}        
-        
+        date_time = pd.to_datetime(dt[0] + " " + dt[1])
+
+        metadata = {
+            "Image name": self.filename,
+            "Indicated Magnification": self.get_mag()[0],
+            "Actual Magnifiation": self.get_mag()[1],
+            "Date": str(date_time.date()),
+            "Time": str(date_time.time()),
+            "Pixel size": self.pixel_size,
+            "Pixel unit": self.pixel_unit,
+            "Exposure Time (s)": self.get_exposure(),
+            "Voltage": self.get_voltage(),
+            "Size (px)": "{}x{}".format(self.shape[1], self.shape[0]),
+            "Video": self.video,
+            "Frame Rate (fps)": False,
+            "Number of frames": self.nframes,
+        }
+
         df = pd.DataFrame(metadata, index=[0])
         if name in os.listdir(outdir):
-            old_df = pd.read_csv(outdir+'/'+name)
+            old_df = pd.read_csv(outdir + "/" + name)
             new_df = pd.concat([old_df, df], ignore_index=True)
-            new_df.sort_values(by=['Date', 'Time'], inplace=True)
-            new_df.to_csv(outdir+'/'+name, index=False)
+            new_df.sort_values(by=["Date", "Time"], inplace=True)
+            new_df.to_csv(outdir + "/" + name, index=False)
         else:
-            df.to_csv(outdir+'/'+name,index=False)
+            df.to_csv(outdir + "/" + name, index=False)
 
-    '''---------------------------------
+    """---------------------------------
     SECTION MOTION CORRECTION
 
     This defines using motioncor2 to align video frames, these frames either need to be saved individually, in which case the function group_frames is needed on the image set before use
     Motioncorrect_video works on a dm4 file, converts it to mrc and then runs motioncor on this image stack. 
 
 
-    '''        
+    """
+
     def motioncor_frames(self, frames_dict):
-        '''
+        """
         Advanced method which requires editing the code to use. Uses Motioncor2 to motion correct a series of frames and output a number of motion corrected images as a micrograph object
-        
+
         Parameters
         ----------
             frames_dict:dict
                 A dictionary of videos and frames in the directory which will be motion corrected, this is created by the 'group_frames()' function
-        
+
         This actually wont work well (will only open the final vid in the frames dictionary). Depreciated function.
-        '''
+        """
 
         for vid in frames_dict:
             frames = frames_dict[vid]
-            outfile = '_'.join(frames[0].split('-')[:-1])+'.mrc'
-            outfile_aligned = '_'.join(frames[0].split('.')[:-1])+'_aligned.mrc'
+            outfile = "_".join(frames[0].split("-")[:-1]) + ".mrc"
+            outfile_aligned = "_".join(frames[0].split(".")[:-1]) + "_aligned.mrc"
             pixelsize = nci.dm.fileDM(frames[0]).scale[2]
-            sb.call('dm2mrc *{}-* {} '.format(vid, outfile), shell=True, cwd=os.getcwd())
-            MCor_path = os.environ.get('MOTIONCOR2_PATH')
+            sb.call(
+                "dm2mrc *{}-* {} ".format(vid, outfile), shell=True, cwd=os.getcwd()
+            )
+            MCor_path = os.environ.get("MOTIONCOR2_PATH")
             if path:
-                motion_cor_command = '{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixSize {} '.format(MCor_path,  outfile, outfile_aligned, pixelsize)
+                motion_cor_command = "{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixSize {} ".format(
+                    MCor_path, outfile, outfile_aligned, pixelsize
+                )
                 sb.call(motion_cor_command, shell=True, cwd=os.getcwd())
 
             else:
-                print('Sorry, the motioncor2 exectuable is not defined and so cannot be run. Please give the executable using "export MOTIONCOR2_PATH=\'PATH/TO/EXECUTABLE\'" for more info, please see documentation  ')
+                print(
+                    "Sorry, the motioncor2 exectuable is not defined and so cannot be run. Please give the executable using \"export MOTIONCOR2_PATH='PATH/TO/EXECUTABLE'\" for more info, please see documentation  "
+                )
                 return 1
-            #motion_cor_command = '{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixSize {} '.format(MOTION_COR_EXECUTABLE,  outfile, outfile_aligned, pixelsize)
-            #sb.call(motion_cor_command, shell=True, cwd=os.getcwd())
+            # motion_cor_command = '{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixSize {} '.format(MOTION_COR_EXECUTABLE,  outfile, outfile_aligned, pixelsize)
+            # sb.call(motion_cor_command, shell=True, cwd=os.getcwd())
             os.remove(outfile)
-            self.open_mrc(outfile_aligned)  
+            self.open_mrc(outfile_aligned)
 
     def motioncorrect_video(self, file):
-        ''' 
+        """
         Advanced method which requires editing the source code to use. Uses Motioncor2 to motion correct a video and output a motion corrected image as a micrograph object
-        
-        This function first converts the dm3 to an mrc file, followed by using motioncor by the exectuable defined in motion_cor_command - change this executible to use. 
-        
+
+        This function first converts the dm3 to an mrc file, followed by using motioncor by the exectuable defined in motion_cor_command - change this executible to use.
+
         An aligned mrc file should be saved in the directory and automatically opened in this Micrograph object.
         Parameters
         ----------
             filename:str
                 The filename to motion correct
-        '''
-        outfile = '_'.join(file.split('.')[:-1])+'.mrc'
-        outfile_aligned = '_'.join(file.split('.')[:-1])+'_aligned.mrc'
+        """
+        outfile = "_".join(file.split(".")[:-1]) + ".mrc"
+        outfile_aligned = "_".join(file.split(".")[:-1]) + "_aligned.mrc"
         pixelsize = nci.dm.fileDM(file).scale[2]
-        #print(pixelsize)
-        #sb.call('dm2mrc {} {} '.format(file, outfile), shell=True, cwd=os.getcwd())
+        # print(pixelsize)
+        # sb.call('dm2mrc {} {} '.format(file, outfile), shell=True, cwd=os.getcwd())
         self.save_tif_stack()
-        MCor_path = os.environ.get('MOTIONCOR2_PATH')
+        MCor_path = os.environ.get("MOTIONCOR2_PATH")
         if MCor_path:
-            motion_cor_command = '{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixSize {} '.format(MCor_path,  outfile, outfile_aligned, pixelsize)
+            motion_cor_command = "{} -InMrc {} -OutMrc {} -Iter 10 -Tol 0.5 -Throw 1 -Kv 200 -PixSize {} ".format(
+                MCor_path, outfile, outfile_aligned, pixelsize
+            )
             sb.call(motion_cor_command, shell=True, cwd=os.getcwd())
 
         else:
-            print('Sorry, the motioncor2 exectuable is not defined and so cannot be run. Please give the executable using "export MOTIONCOR2_PATH=\'PATH/TO/EXECUTABLE\'" (or on windows: "setx MY_EXECUTABLE_PATH \'path/to/executable\'") for more info, please see documentation  ')
+            print(
+                "Sorry, the motioncor2 exectuable is not defined and so cannot be run. Please give the executable using \"export MOTIONCOR2_PATH='PATH/TO/EXECUTABLE'\" (or on windows: \"setx MY_EXECUTABLE_PATH 'path/to/executable'\") for more info, please see documentation  "
+            )
             return 1
         os.remove(outfile)
-        self.open_mrc(outfile_aligned)            
-
-     
-
-
-
-
+        self.open_mrc(outfile_aligned)
 
 
-
-# I had to move default pipeline outside of the class because the filters make a new instance of the class and I didnt want to multiply the number of instances in memory. 
+# I had to move default pipeline outside of the class because the filters make a new instance of the class and I didnt want to multiply the number of instances in memory.
 # Use: default_pipeline(micrograph)
-def default_image_pipeline(filename,  name='', medfilter=3, gaussfilter=0, scalebar=True, texton = True, xybin=2, color='Auto', outdir='.',save_metadata=True, metadata_name='metadata.csv',topaz_denoise=False, denoise_with_cuda=False):
-    '''
+def default_image_pipeline(
+    filename,
+    output_type='jpg',
+    name="",
+    contrast_enhance=True,
+    medfilter=3,
+    gaussfilter=0,
+    scalebar=True,
+    texton=True,
+    xybin=2,
+    color="Auto",
+    outdir=".",
+    save_metadata=True,
+    metadata_name="metadata.csv",
+    topaz_denoise=False,
+    denoise_with_cuda=False,
+):
+    """
     Default pipeline to process image, add scalebar, filter, bin and save the image, speeding up automation.
-    
+
     Parameters
     ----------
         Filename:str
             Filename of image to process
 
         name:str
             Name of the saved image
 
-        medfilter:int 
-            The kernal size for a median filter on the image, default is 3, use 0 for no median filter, otherwise must be odd. 
+        output_type: str
+            Decides file format of saved image. Currently supported are jpg, tif (8-bit) and tif (32-bit)
+
+        medfilter:int
+            The kernal size for a median filter on the image, default is 3, use 0 for no median filter, otherwise must be odd.
 
         gaussfilter:int
-            The kernal size for a gaussian filter on the image, default is off (0), must be odd. 
+            The kernal size for a gaussian filter on the image, default is off (0), must be odd.
 
         scalebar:bool
-            Turns the scale bar on/off (default is on), use scalebar=False to turn off. 
+            Turns the scale bar on/off (default is on), use scalebar=False to turn off.
 
 
         texton:bool
             Turns the text on the scalebar on or off (default is on)
-         
+
         xybin:int
             Bins the image (x/y) axis
 
         color:str
             Chooses scalebar color 'black', 'white' or 'grey'
 
         topaz_denoise: bool
             Denoise with topaz? True (default) or False (default)
 
         denoise_with_cuda: bool
-            If denoising with topaz, use CUDA gpu for this? If availble this will dramatically increase speed. 
-    '''
+            If denoising with topaz, use CUDA gpu for this? If availble this will dramatically increase speed.
+    """
     Micrograph_object = Micrograph(filename)
 
-    if '/' in Micrograph_object.filename:
-        Micrograph_object.filename=Micrograph_object.filename.split('/')[-1]
+    if "/" in Micrograph_object.filename:
+        Micrograph_object.filename = Micrograph_object.filename.split("/")[-1]
 
-    if save_metadata==True and filename[-4:-1]=='.dm':
-        Micrograph_object.export_metadata(name=metadata_name, outdir=outdir) 
+    if save_metadata == True and filename[-4:-1] == ".dm":
+        Micrograph_object.export_metadata(name=metadata_name, outdir=outdir)
 
     if topaz_denoise:
         Micrograph_object = Micrograph_object.topaz_denoise(use_cuda=denoise_with_cuda)
 
-    if type(medfilter)==int and medfilter!=0: 
+    if type(medfilter) == int and medfilter != 0:
         Micrograph_object = Micrograph_object.median_filter(medfilter)
-    
-    if type(gaussfilter)==int and gaussfilter!=0:  
+
+    if type(gaussfilter) == int and gaussfilter != 0:
         Micrograph_object = Micrograph_object.gaussian_filter(medfilter)
 
-    if xybin!= 0 and xybin!=1:
+    if xybin != 0 and xybin != 1:
         Micrograph_object = Micrograph_object.bin(xybin)
 
-    if name !='':
+    if name != "":
         name = name
     else:
-        name = '.'.join(Micrograph_object.filename.split('.')[:-1])
-        #print(filename)
-    #if 'outdir' in kwargs:
-    #print('name=',name)
-    #Micrograph_object = Micrograph_object.enhance_contrast()
-    Micrograph_object=Micrograph_object.convert_to_8bit()
-    Micrograph_object = Micrograph_object.clip_contrast() 
-    if scalebar==True:
+        name = ".".join(Micrograph_object.filename.split(".")[:-1])
+        # print(filename)
+    # if 'outdir' in kwargs:
+    # print('name=',name)
+    # Micrograph_object = Micrograph_object.enhance_contrast()
+    #Micrograph_object = Micrograph_object.convert_to_8bit()
+    if contrast_enhance: 
+        Micrograph_object = Micrograph_object.clip_contrast()
+    if scalebar == True:
         Micrograph_object = Micrograph_object.make_scalebar(texton=texton, color=color)
 
-    
-    Micrograph_object.write_image(name=name,outdir=outdir+'/Images')
+    Micrograph_object.write_image(name=name, outdir=outdir + "/Images", ftype= output_type)
 
-    #Micrograph_object.save_image(outname=name)
+    # Micrograph_object.save_image(outname=name)
 
-def default_pipeline_class(Micrograph_object ,name=None, medfilter=3, gaussfilter=0, scalebar=True, texton = True, xybin=2, color='Auto',outdir='.', topaz_denoise=False, denoise_with_cuda=False):
 
-    '''
+def default_pipeline_class(
+    Micrograph_object,
+    name=None,
+    medfilter=3,
+    gaussfilter=0,
+    scalebar=True,
+    texton=True,
+    xybin=2,
+    color="Auto",
+    outdir=".",
+    topaz_denoise=False,
+    denoise_with_cuda=False,
+):
+    """
     Default pipeline to process from a Micrograph_object, add scalebar, filter, bin and save the image, speeding up automation.
-    
+
     Parameters
     ----------
         Filename:str
             Filename of image to process
 
         name:str
             Name of the saved image
 
-        medfilter:int 
-            The kernal size for a median filter on the image, default is 3, use 0 for no median filter, otherwise must be odd. 
+        medfilter:int
+            The kernal size for a median filter on the image, default is 3, use 0 for no median filter, otherwise must be odd.
 
         gaussfilter:int
-            The kernal size for a gaussian filter on the image, default is off (0), must be odd. 
+            The kernal size for a gaussian filter on the image, default is off (0), must be odd.
 
         scalebar:bool
-            Turns the scale bar on/off (default is on), use scalebar=False to turn off. 
+            Turns the scale bar on/off (default is on), use scalebar=False to turn off.
 
 
         texton:bool
             Turns the text on the scalebar on or off (default is on)
-         
+
         xybin:int
             Bins the image (x/y) axis
 
         color:str
             Chooses scalebar color 'black', 'white' or 'grey'
 
         topaz_denoise: bool
             Denoise with topaz? True (default) or False (default)
 
         denoise_with_cuda: bool
-            If denoising with topaz, use CUDA gpu for this? If availble this will dramatically increase speed. 
+            If denoising with topaz, use CUDA gpu for this? If availble this will dramatically increase speed.
+
 
-        
-    '''
+    """
     if topaz_denoise:
         Micrograph_object = Micrograph_object.topaz_denoise(use_cuda=denoise_with_cuda)
 
-    if type(medfilter)==int and medfilter!=0: 
+    if type(medfilter) == int and medfilter != 0:
         Micrograph_object = Micrograph_object.median_filter(medfilter)
-    
-    if type(gaussfilter)==int and gaussfilter!=0:  
+
+    if type(gaussfilter) == int and gaussfilter != 0:
         Micrograph_object = Micrograph_object.gaussian_filter(medfilter)
 
-    if xybin!= 0 and xybin!=1:
+    if xybin != 0 and xybin != 1:
         Micrograph_object = Micrograph_object.bin(xybin)
 
     if name:
         name = name
     else:
         print(Micrograph_object.filename)
-        name = '.'.join(Micrograph_object.filename.split('.')[:-1])
+        name = ".".join(Micrograph_object.filename.split(".")[:-1])
         print(name)
-        #print(filename)
-    #if 'outdir' in kwargs:
-    #print('name=',name)
-    #Micrograph_object = Micrograph_object.enhance_contrast()
-    Micrograph_object=Micrograph_object.convert_to_8bit()
+        # print(filename)
+    # if 'outdir' in kwargs:
+    # print('name=',name)
+    # Micrograph_object = Micrograph_object.enhance_contrast()
+    Micrograph_object = Micrograph_object.convert_to_8bit()
     Micrograph_object = Micrograph_object.clip_contrast()
     if scalebar:
         Micrograph_object = Micrograph_object.make_scalebar(texton=texton, color=color)
 
+    Micrograph_object.write_image(name=name, outdir=outdir)
 
-    Micrograph_object.write_image(name=name,outdir=outdir)
+    # Micrograph_object.save_image(outname=name)
 
-    #Micrograph_object.save_image(outname=name)
 
 def group_frames(frames):
     prefixes = []
-    prefix_set=set()
+    prefix_set = set()
     frames.sort()
     tups = []
-    organised_dict= {}
+    organised_dict = {}
     for file in frames:
         file2 = file[:-4]
         end = file2[-9:]
-        ids = end.split('-')
+        ids = end.split("-")
         vid_id = ids[0]
         frame_id = ids[1]
         tups.append((file, vid_id, frame_id))
         prefix_set.add(vid_id)
 
-    for prefix in prefix_set: 
-        images_per_prefix = [x[0] for x in tups if x[1]==prefix]
-        organised_dict[prefix]=images_per_prefix
+    for prefix in prefix_set:
+        images_per_prefix = [x[0] for x in tups if x[1] == prefix]
+        organised_dict[prefix] = images_per_prefix
         return organised_dict
 
+
 def make_outdir(outdir):
-    if outdir==None:
+    if outdir == None:
         return 0
 
-    elif '/' in outdir:
-        split = outdir.split('/')
+    elif "/" in outdir:
+        split = outdir.split("/")
         new_dir = split[-1]
-        current_dir = '/'.join(split[:-1])
+        current_dir = "/".join(split[:-1])
 
-        if new_dir not in os.listdir(current_dir) and new_dir.lower() not in [x.lower() for x in os.listdir(current_dir)]:
+        if new_dir not in os.listdir(current_dir) and new_dir.lower() not in [
+            x.lower() for x in os.listdir(current_dir)
+        ]:
             os.mkdir(outdir)
-    elif outdir=='.':
+    elif outdir == ".":
         return 0
-    else: 
-        if outdir not in os.listdir('.'):
+    else:
+        if outdir not in os.listdir("."):
             os.mkdir(outdir)
 
+
+def get_files(pattern, directory="."):
+    return [directory + "/" + x for x in os.listdir(directory) if pattern in x]
+
+
+
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/Motion_correction.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/Motion_correction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,98 @@
-
 import cv2 as cv
-import numpy as np 
+import numpy as np
+
 
 def find_shift(frame1, frame2, crop=3700):
-    if len(frame1.shape)==3:
-        #print(frame1, frame2)
-        frame1=np.sum(frame1, axis=0)
-        #print(frame1.shape)
-    frame1[frame1>frame1.mean()+4*frame1.std()]=frame1.mean()
-    frame2[frame2>frame1.mean()+4*frame1.std()] = frame2.mean()
+    if len(frame1.shape) == 3:
+        # print(frame1, frame2)
+        frame1 = np.sum(frame1, axis=0)
+        # print(frame1.shape)
+    frame1[frame1 > frame1.mean() + 4 * frame1.std()] = frame1.mean()
+    frame2[frame2 > frame1.mean() + 4 * frame1.std()] = frame2.mean()
     frame1_cropped = frame1[:crop, :crop]
     frame2_cropped = frame2[:crop, :crop]
-    
-    #frame1_cropped =cv.resize(frame1_cropped, (int(frame1_cropped.shape[0]/2), int(frame1_cropped.shape[1]/2)), interpolation=cv.INTER_CUBIC)
-    #frame2_cropped =cv.resize(frame2_cropped, (int(frame2_cropped.shape[0]/2), int(frame2_cropped.shape[1]/2)), interpolation=cv.INTER_CUBIC)
-    center = (int(frame1_cropped.shape[0]/2), int( frame1_cropped.shape[1]/2))
-    
-    #mask = np.zeros_like(frame1_cropped)
-    #mask= cv.circle(mask,center, LP_radius*2,1,-1)
-    
+
+    # frame1_cropped =cv.resize(frame1_cropped, (int(frame1_cropped.shape[0]/2), int(frame1_cropped.shape[1]/2)), interpolation=cv.INTER_CUBIC)
+    # frame2_cropped =cv.resize(frame2_cropped, (int(frame2_cropped.shape[0]/2), int(frame2_cropped.shape[1]/2)), interpolation=cv.INTER_CUBIC)
+    center = (int(frame1_cropped.shape[0] / 2), int(frame1_cropped.shape[1] / 2))
+
+    # mask = np.zeros_like(frame1_cropped)
+    # mask= cv.circle(mask,center, LP_radius*2,1,-1)
+
     fft1 = cv.dft(frame1_cropped.astype(np.float32), flags=cv.DFT_COMPLEX_OUTPUT)
     fft2 = cv.dft(frame2_cropped.astype(np.float32), flags=cv.DFT_COMPLEX_OUTPUT)
     fft1_shf = np.fft.fftshift(fft1)
     fft2_shf = np.fft.fftshift(fft2)
-    
-    #mask = np.zeros_like(fft1)
-    #mask= cv.circle(mask,center, LP_radius*2,1,-1)
-    #print(fft1_shf.shape)
-    #fft1_filtered = mask*fft1_shf
-    #fft2_filtered = mask*fft2_shf
-    
-    
-    fft1_shf_cplx = fft1_shf[:,:,0]+1j*fft1_shf[:,:,1]
-    fft2_shf_cplx = fft2_shf[:,:,0]+1j*fft2_shf[:,:,1]
 
-    
+    # mask = np.zeros_like(fft1)
+    # mask= cv.circle(mask,center, LP_radius*2,1,-1)
+    # print(fft1_shf.shape)
+    # fft1_filtered = mask*fft1_shf
+    # fft2_filtered = mask*fft2_shf
+
+    fft1_shf_cplx = fft1_shf[:, :, 0] + 1j * fft1_shf[:, :, 1]
+    fft2_shf_cplx = fft2_shf[:, :, 0] + 1j * fft2_shf[:, :, 1]
+
     fft1_shf_abs = np.abs(fft1_shf_cplx)
     fft2_shf_abs = np.abs(fft2_shf_cplx)
-    total_abs = fft1_shf_abs*fft2_shf_abs
-    
-    p_real = (np.real(fft1_shf_cplx)*np.real(fft2_shf_cplx)+np.imag(fft1_shf_cplx)*np.imag(fft2_shf_cplx))/total_abs
-    p_imag = (np.imag(fft1_shf_cplx)*np.real(fft2_shf_cplx)+np.real(fft1_shf_cplx)*np.imag(fft2_shf_cplx))/total_abs
-    p_complex = p_real + 1j*p_imag
+    total_abs = fft1_shf_abs * fft2_shf_abs
+
+    p_real = (
+        np.real(fft1_shf_cplx) * np.real(fft2_shf_cplx)
+        + np.imag(fft1_shf_cplx) * np.imag(fft2_shf_cplx)
+    ) / total_abs
+    p_imag = (
+        np.imag(fft1_shf_cplx) * np.real(fft2_shf_cplx)
+        + np.real(fft1_shf_cplx) * np.imag(fft2_shf_cplx)
+    ) / total_abs
+    p_complex = p_real + 1j * p_imag
     p_inverse = np.abs(np.fft.ifft2(p_complex))
-    #print(p_inverse)
+    # print(p_inverse)
     max_val = np.max(p_inverse)
-    #print(max_val)
-    
-    shifts = np.where(p_inverse==max_val)
+    # print(max_val)
+
+    shifts = np.where(p_inverse == max_val)
     print(shifts)
     shift_x = shifts[0][0]
     shift_y = shifts[1][0]
-    if shift_x==0:
-        p_inverse[shift_x, shift_y]=0
-        print('shift=0')
-        shifts=np.where(p_inverse==np.max(p_inverse))
+    if shift_x == 0:
+        p_inverse[shift_x, shift_y] = 0
+        print("shift=0")
+        shifts = np.where(p_inverse == np.max(p_inverse))
         print(shifts)
         shift_x = shifts[0][0]
         shift_y = shifts[1][0]
     return shift_x, shift_y
 
+
 def shift_elements(arr, shifts, fill_value):
-    '''
+    """
     shifts an array by set values, with the remaining values being set to 'fill_value'
-    shifts are entered in format of [y,x] and will shift with up and left being the negative direction. 
+    shifts are entered in format of [y,x] and will shift with up and left being the negative direction.
     This was designed to work with the find_shifts() function above, however this appears to be problematic (I think it doesn't shift in negative directions correctly).
-    aligning based on particle coordinates should work. 
-    
-    '''
+    aligning based on particle coordinates should work.
+
+    """
     result = np.full_like(arr, fill_value)
     y = shifts[0]
-    if y>0:
+    if y > 0:
         result[y:] = arr[:-y]
-    elif y<0: 
-        #print('Here')
-        #result[x]=fill_value
-        result[:y]=arr[-y:]
+    elif y < 0:
+        # print('Here')
+        # result[x]=fill_value
+        result[:y] = arr[-y:]
     else:
-        result =arr
-    #print(result)   
+        result = arr
+    # print(result)
     r2 = np.full_like(result, fill_value)
-    #print(r2)
+    # print(r2)
     x = shifts[1]
-    #print(y)
-    if x>0:
-        r2[:,x:]=result[:,:-x]
-    elif x<0:
-        
-        r2[:, :x]=result[:, -x:] 
+    # print(y)
+    if x > 0:
+        r2[:, x:] = result[:, :-x]
+    elif x < 0:
+        r2[:, :x] = result[:, -x:]
     else:
-        r2=result
-    #print(result)
-    return r2    
+        r2 = result
+    # print(result)
+    return r2
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/PDF_generator.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/PDF_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,216 +1,214 @@
-
-from fpdf import FPDF
-import os
 import itertools
 import math
+import os
 
+from fpdf import FPDF
 
 
-def pdf_generator(images, title, notes, directory='',max_num=9):
-    '''
-    Function for generating a pdf file showing images, this aims to make it easier to examine, evaluate and share images from a TEM session by putting them in a single document. 
+def pdf_generator(images, title, notes, directory="", max_num=9):
+    """
+    Function for generating a pdf file showing images, this aims to make it easier to examine, evaluate and share images from a TEM session by putting them in a single document.
 
     Parameters
     ----------
 
         images: list
-            A list of images to place in the pdf document. This can be easily created with a generator function, eg. images = [x for x in os.listdir('PATH/TO/DIRECTORY') if x[-3:]=='jpg'] 
-    
+            A list of images to place in the pdf document. This can be easily created with a generator function, eg. images = [x for x in os.listdir('PATH/TO/DIRECTORY') if x[-3:]=='jpg']
+
         title: str
             A title for the experiment
 
         notes: str
             Experimental notes, need to be kept fairly short (a few sentances max), these will be placed on the first page.
 
         directory: str
             If being run outside of the directory containing the images, the path to the directory needs to be included here, by default it assumes the same directory.
 
         max_num: int
-            The maximum number of images to include on a single pdf page, this can be 1,4,6 or 9 (default). Smaller number means larger images (but longer document) 
+            The maximum number of images to include on a single pdf page, this can be 1,4,6 or 9 (default). Smaller number means larger images (but longer document)
 
     Output
     ------
 
-        Saves a pdf document under the name {title}.pdf with the images contained within the list. 
-    '''
-    if ' ' in title: 
-        filename = title.replace(' ', '_')+'.pdf'
-    elif '_' in title:
-        filename = str(title)+'.pdf'
-        title = title.replace('_', ' ')
-    elif title == '':
-        filename = 'out.pdf'
-    else: 
-        filename = title+'.pdf' 
+        Saves a pdf document under the name {title}.pdf with the images contained within the list.
+    """
+    if " " in title:
+        filename = title.replace(" ", "_") + ".pdf"
+    elif "_" in title:
+        filename = str(title) + ".pdf"
+        title = title.replace("_", " ")
+    elif title == "":
+        filename = "out.pdf"
+    else:
+        filename = title + ".pdf"
 
-    pdf = FPDF(orientation='P',unit='pt', format='A4')
+    pdf = FPDF(orientation="P", unit="pt", format="A4")
     pdf.add_page()
-    pdf.set_font('Arial', 'B', 16)
-    pdf.cell(540, 10, title, align='C')
-    pdf.set_font('Arial','', 10)
-    pdf.set_xy(20, 50 )
+    pdf.set_font("Arial", "B", 16)
+    pdf.cell(540, 10, title, align="C")
+    pdf.set_font("Arial", "", 10)
+    pdf.set_xy(20, 50)
 
-    pdf.multi_cell(0, 12,notes)
+    pdf.multi_cell(0, 12, notes)
     if directory:
-        images = [directory+'/'+image for image in images]
+        images = [directory + "/" + image for image in images]
     i = 0
     grouped_images = group_images(images)
     group_number = 0
 
-
     for prefix in grouped_images:
-        i=0
+        i = 0
 
         group = grouped_images[prefix]
         print(prefix)
-        if group_number !=0:
+        if group_number != 0:
             pdf.add_page()
 
-        #pdf.set_xy(10, 100)
-        #pdf.set_font('Arial', 'B', 14)
-        #xsample_name = 'Sample name: {}'.format(' '.join(prefix.split('_')))
-        #pdf.cell(540, 10, sample_name, align='C')
-        pagenum =0
+        # pdf.set_xy(10, 100)
+        # pdf.set_font('Arial', 'B', 14)
+        # xsample_name = 'Sample name: {}'.format(' '.join(prefix.split('_')))
+        # pdf.cell(540, 10, sample_name, align='C')
+        pagenum = 0
 
-        group_size= len(group)
+        group_size = len(group)
 
-        
         # this if group decides how many images to put per page based on the number of images total.
 
-        if group_size<2:
+        if group_size < 2:
             num = 1
-        elif group_size<5 or group_size==7 or group_size ==8:
-            num =4 
-        elif group_size<7 or group_size ==10 or group_size==11 or group_size==12:
-            num=6
+        elif group_size < 5 or group_size == 7 or group_size == 8:
+            num = 4
+        elif group_size < 7 or group_size == 10 or group_size == 11 or group_size == 12:
+            num = 6
         else:
-            num=9   
+            num = 9
 
-        
-        if num==6:
+        if num == 6:
             pdf.set_xy(10, 100)
         else:
-            pdf.set_xy(10,120)          
-        pdf.set_font('Arial', 'B', 14)
-        sample_name = 'Sample name: {}'.format(' '.join(prefix.split('_')))
-        pdf.cell(540, 10, sample_name, align='C')   
-        #This line gets the coordinates using the  
-        
+            pdf.set_xy(10, 120)
+        pdf.set_font("Arial", "B", 14)
+        sample_name = "Sample name: {}".format(" ".join(prefix.split("_")))
+        pdf.cell(540, 10, sample_name, align="C")
+        # This line gets the coordinates using the
+
         image_coords, cap_coords, size = return_coords(num)
         print(image_coords, cap_coords, size)
 
         for i in range(len(group)):
-                    
-            j =i-(pagenum*num)
+            j = i - (pagenum * num)
 
-            pdf.image(group[i],image_coords[j][0], image_coords[j][1], size )
-                   
+            pdf.image(group[i], image_coords[j][0], image_coords[j][1], size)
 
             im_id, im_preview = find_number(group[i])
-            pdf.set_xy(cap_coords[j][0],cap_coords[j][1])
-            pdf.cell(10,10,im_id )
-            #pdf.cell
-                #i+=1
-                #print(j)
-    
-            #this deals with making a new page when all the images are on the previous page.
-
-            if (i+1)%num==0 and num!=1 and i+1!=group_size:
-                print('yes')
-                pagenum+=1
+            pdf.set_xy(cap_coords[j][0], cap_coords[j][1])
+            pdf.cell(10, 10, im_id)
+            # pdf.cell
+            # i+=1
+            # print(j)
+
+            # this deals with making a new page when all the images are on the previous page.
+
+            if (i + 1) % num == 0 and num != 1 and i + 1 != group_size:
+                print("yes")
+                pagenum += 1
                 pdf.add_page()
                 pdf.set_xy(10, 100)
-                pdf.cell(540, 10, sample_name, align='C')
+                pdf.cell(540, 10, sample_name, align="C")
 
-        group_number+=1
-    pdf.output(filename,'F')
+        group_number += 1
+    pdf.output(filename, "F")
+
+    print("PDF generated!")
 
-    print('PDF generated!')
 
 def find_number(string):
-    '''
-    Function to find the idenfication number of the images so they can be  labelled in the pdf. 
+    """
+    Function to find the idenfication number of the images so they can be  labelled in the pdf.
 
     Parameters
     ----------
         string: str
             Filename which contains the image number
 
     Returns
     -------
 
         im_id:str
-            The ID number of the image 
+            The ID number of the image
 
         prefix:str
-            The prefix to the image id - normally contains details about the sample. 
+            The prefix to the image id - normally contains details about the sample.
+
 
-    
-    '''
-    nstring= string.replace('.', '_')
-    lstring = nstring.split('_')
-    #print(lstring)
+    """
+    nstring = string.replace(".", "_")
+    lstring = nstring.split("_")
+    # print(lstring)
     success = False
     for item in lstring:
-        if len(item)==4 and item.isdigit():
-                im_id = item
-                ind = lstring.index(im_id)
-                #print(ind)
-                success=True
-    if success==False:
+        if len(item) == 4 and item.isdigit():
+            im_id = item
+            ind = lstring.index(im_id)
+            # print(ind)
+            success = True
+    if success == False:
         ind = -2
         im_id = lstring[ind]
 
-    prefix = ' '.join(lstring[:ind])
-    #print(success)
+    prefix = " ".join(lstring[:ind])
+    # print(success)
     return im_id, prefix
-#print(im_prefix)
+
+
+# print(im_prefix)
+
 
 def group_images(images):
-    '''
-    Sorts a number of images into a dictionary with images separated by the sample name, these can then be separated onto different pages. 
+    """
+    Sorts a number of images into a dictionary with images separated by the sample name, these can then be separated onto different pages.
 
     Parameters
     ----------
 
         images:list
             List of images (by filename)
 
-    Returns 
+    Returns
     -------
 
         organised_dict:dict
             Dictionary containing the sample names (image prefixes) as the keys and a list of images with  that name as the value.
-    '''
+    """
 
     prefixes = []
-    prefix_set=set()
+    prefix_set = set()
     images.sort()
     tups = []
     for image in images:
         im_id, im_prefix = find_number(image)
-        
+
         prefix_set.add(im_prefix)
         tup = image, im_id, im_prefix
         tups.append(tup)
 
-    organised_dict= {}
+    organised_dict = {}
     prefix_set = sorted(prefix_set)
     for prefix in prefix_set:
+        # im_id, im_prefix = find_number(image)
 
-        #im_id, im_prefix = find_number(image)
+        images_per_prefix = [x[0] for x in tups if x[2] == prefix]
+        organised_dict[prefix] = images_per_prefix
 
-        images_per_prefix =[x[0] for x in tups if x[2]==prefix]
-        organised_dict[prefix]=images_per_prefix
-  
     return organised_dict
 
+
 def return_coords(max_num):
-    '''
+    """
     Gives the coordinates for the images & captions, and the size of the images depending on the number per page.
 
     Parameters
     ----------
         max_num:int
             The number of images per page.
 
@@ -218,60 +216,57 @@
     -------
         Image_coords:list
             The coordinates for each image on the page
 
         cap_coords:list
             The coordinates for each caption on the page
 
-        size:int 
+        size:int
             The size of the images.
-    '''
-    if max_num==1:
+    """
+    if max_num == 1:
         imx = [15]
         imy = [178]
         capx = [271]
         capy = [755]
         size = 570
-    
-    elif max_num==4:
+
+    elif max_num == 4:
         imx = [10, 300]
         imy = [149, 475]
-       
-        capx = [123,431]
-        capy = [442,768]
+
+        capx = [123, 431]
+        capy = [442, 768]
         size = 280
-        #capy = [422,754]
-#        size = 284
+        # capy = [422,754]
+    #        size = 284
 
-    elif max_num==6:
-        imx = [68,358]
-        imy = [123,360, 598]
+    elif max_num == 6:
+        imx = [68, 358]
+        imy = [123, 360, 598]
         capx = [13, 307]
         capy = [255, 463, 700]
         size = 227
-    elif max_num==9:
-        
+    elif max_num == 9:
         imx = [12, 205, 398]
-        imy= [146, 361, 576]
-        
+        imy = [146, 361, 576]
 
-        capx = [85,280, 473]
+        capx = [85, 280, 473]
         capy = [335, 550, 764]
         size = 180
-    else: 
-        print('Input not valid, returning default')
-                
+    else:
+        print("Input not valid, returning default")
+
         imx = [12, 205, 398]
-        imy= [146, 361, 576]
-        capx = [85,280, 473]
+        imy = [146, 361, 576]
+        capx = [85, 280, 473]
         capy = [335, 550, 764]
         size = 180
-    cap_coords=list(itertools.product(capx, capy))
-    image_coords = list(itertools.product(imx,imy))
-    return image_coords, cap_coords, size 
-
-if __name__=='__main__':
-    images = [x for x in os.listdir('.') if x[-3:]=='jpg']      
+    cap_coords = list(itertools.product(capx, capy))
+    image_coords = list(itertools.product(imx, imy))
+    return image_coords, cap_coords, size
 
-    pdf_generator(images, 'New_attempt', 'Hello world')
 
+if __name__ == "__main__":
+    images = [x for x in os.listdir(".") if x[-3:] == "jpg"]
 
+    pdf_generator(images, "New_attempt", "Hello world")
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_analysis.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,491 +1,526 @@
-from SimpliPyTEM.Micrograph_class import *
-from SimpliPyTEM.MicroVideo_class import *
+import math
+
+import imutils
+from imutils import contours
 from moviepy.editor import ImageSequenceClip
 from skimage import measure
-from imutils import contours
-import imutils
-import math
+import cv2 as cv
+import numpy as np 
+import pandas as pd 
+from SimpliPyTEM.Micrograph_class import Micrograph
+from SimpliPyTEM.MicroVideo_class import MicroVideo
 
-'''
+"""
 MAIN FUNCTIONS
-'''
+"""
+
 
 def Threshold(image, threshold, brightfield=True):
-    '''
+    """
     Threshold the image to a particular value, such that below that value goes to black and above that value goes to white.
-    
+
     Parameters
     ----------
         image:numpy array
             The image to be thresholded
 
         threshold: int
             The threshold value
 
     returns
     -------
         thresh:numpy array
-            The thresholded image 
+            The thresholded image
 
-    '''
+    """
 
-
-    imG=cv.GaussianBlur(image, (5,5),0)
-    #croppedThresh[croppedThresh<90] = 0
-    #croppedThresh[croppedThresh>90]=255
+    imG = cv.GaussianBlur(image, (5, 5), 0)
+    # croppedThresh[croppedThresh<90] = 0
+    # croppedThresh[croppedThresh>90]=255
     ret, thresh = cv.threshold(imG, threshold, 255, cv.THRESH_BINARY)
-    thresh = cv.erode(thresh, None,iterations=1)
-    thresh = cv.dilate(thresh, None,iterations=1)
-    thresh = thresh.astype('uint8')
-    if brightfield==True:
-        thresh=cv.bitwise_not(thresh)
-    return thresh#,res
-
-
-def Find_contours(thresh, minsize=200, complex_coords=False, maxsize=100000, remove_edges=True, labelled=False):
-    '''
-    Finds the contours (or edges) of the particles in the image 
+    thresh = cv.erode(thresh, None, iterations=1)
+    thresh = cv.dilate(thresh, None, iterations=1)
+    thresh = thresh.astype("uint8")
+    if brightfield == True:
+        thresh = cv.bitwise_not(thresh)
+    return thresh  # ,res
+
+
+def Find_contours(
+    thresh,
+    minsize=200,
+    complex_coords=False,
+    maxsize=100000,
+    remove_edges=True,
+    labelled=False,
+):
+    """
+    Finds the contours (or edges) of the particles in the image
 
     In doing so, this also filters the particles by minimum and maximum size (in number of pixels total area) and removes any particles which are on the edge of the image.
 
     Parameters
     ----------
 
         thresh:numpy array
             The thresholded image, can be produced with threshold(). Can also use a pre-labelled image (labelled=True)
-        
+
         minsize:int
             The minimum area (in pixels) for a particle to be considered a particle
 
         minsize:int
             The maximum area (in pixels) for a particle to be considered a particle
 
-        complex_coords:bool 
-            Whether to use cv.CHAIN_APPROX_SIMPLE or cv.CHAIN_APPROX_NONE in the contours. Complex_coords = False (off, chain_approx_simple) simplifies the bounding coordinates leading to less total coordinates, this is faster to process. Full coordinates (complex_coords=True) allows more detailed measurements across the particle, however will take longer. 
+        complex_coords:bool
+            Whether to use cv.CHAIN_APPROX_SIMPLE or cv.CHAIN_APPROX_NONE in the contours. Complex_coords = False (off, chain_approx_simple) simplifies the bounding coordinates leading to less total coordinates, this is faster to process. Full coordinates (complex_coords=True) allows more detailed measurements across the particle, however will take longer.
 
         labelled: bool
-            If you want to use a labelled image (rather than thresholded) set to true. Labelled image should have the pixels lablled a specific number for each particle 
+            If you want to use a labelled image (rather than thresholded) set to true. Labelled image should have the pixels lablled a specific number for each particle
     Returns
     -------
-        contours_im:list 
-            This is a list of arrays with coordinates which bound each particle selected in the image. This is used in downstream processing. 
+        contours_im:list
+            This is a list of arrays with coordinates which bound each particle selected in the image. This is used in downstream processing.
 
         mask:numpy array
-            Binary image showing the particles selected in white and the background in black. 
+            Binary image showing the particles selected in white and the background in black.
 
-    '''
+    """
 
-    #plt.imshow(thresh)
-    #plt.show()
-    #labels =measure.label(thresh, neighbors=8, background=0)
-    if labelled!=True:
+    # plt.imshow(thresh)
+    # plt.show()
+    # labels =measure.label(thresh, neighbors=8, background=0)
+    if labelled != True:
         cnts, hier = cv.findContours(thresh, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
         for cnt in cnts:
-            cv.drawContours(thresh, [cnt], 0,255,-1)
-        labels =measure.label(thresh,background=0)
-    else: 
-        labels=thresh
-    mask = np.zeros(thresh.shape, dtype='uint8')
-    
-    
+            cv.drawContours(thresh, [cnt], 0, 255, -1)
+        labels = measure.label(thresh, background=0)
+    else:
+        labels = thresh
+    mask = np.zeros(thresh.shape, dtype="uint8")
 
     for label in np.unique(labels):
-        if label==0:
+        if label == 0:
             continue
-        label_mask = np.zeros(thresh.shape, dtype='uint8')
-        label_mask[labels==label]=255
-        #particle_data['Radius']=255
+        label_mask = np.zeros(thresh.shape, dtype="uint8")
+        label_mask[labels == label] = 255
+        # particle_data['Radius']=255
         num_pixels = cv.countNonZero(label_mask)
-        #if num_pixels>min_size:
+        # if num_pixels>min_size:
         #    mask = cv.add(mask, label_mas
-        coords = np.where(label_mask>0)
+        coords = np.where(label_mask > 0)
 
-        #Filter out anything touching the edges
-        #if remove_edges and not any([0 in coords[0], thresh.shape[0]-1 in coords[0],thresh.shape[1]-1 in coords[1], 0 in coords[1]]):
+        # Filter out anything touching the edges
+        # if remove_edges and not any([0 in coords[0], thresh.shape[0]-1 in coords[0],thresh.shape[1]-1 in coords[1], 0 in coords[1]]):
 
-        if not any([0 in coords[0], thresh.shape[0]-1 in coords[0],thresh.shape[1]-1 in coords[1], 0 in coords[1],num_pixels<minsize, num_pixels>maxsize]) and remove_edges:
-                #print(coords)
-                mask = cv.add(mask, label_mask)
-        elif remove_edges==False and num_pixels> minsize and num_pixels<maxsize:
-                #print(coords)
-                mask = cv.add(mask, label_mask)
+        if (
+            not any(
+                [
+                    0 in coords[0],
+                    thresh.shape[0] - 1 in coords[0],
+                    thresh.shape[1] - 1 in coords[1],
+                    0 in coords[1],
+                    num_pixels < minsize,
+                    num_pixels > maxsize,
+                ]
+            )
+            and remove_edges
+        ):
+            # print(coords)
+            mask = cv.add(mask, label_mask)
+        elif remove_edges == False and num_pixels > minsize and num_pixels < maxsize:
+            # print(coords)
+            mask = cv.add(mask, label_mask)
     if complex_coords:
-        contours_im = cv.findContours(mask.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE)
+        contours_im = cv.findContours(
+            mask.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE
+        )
     else:
-        contours_im = cv.findContours(mask.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
-    #for cnt in contours_im:
-    #print(contours_im)
+        contours_im = cv.findContours(
+            mask.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE
+        )
+    # for cnt in contours_im:
+    # print(contours_im)
     contours_im = imutils.grab_contours(contours_im)
     try:
         contours_im = contours.sort_contours(contours_im)[0]
     except ValueError:
-        print('Theres a ValueError! This is commonly because no particles are selected in the video.  Try raising the threshold value, or ')
-    #print(contours_im)
-    #plt.imshow(labels)
-    #for labell in np.unique(labels)
+        print(
+            "Theres a ValueError! This is commonly because no particles are selected in the video.  Try raising the threshold value, or "
+        )
+    # print(contours_im)
+    # plt.imshow(labels)
+    # for labell in np.unique(labels)
     return contours_im, mask
 
 
-
-
-    
-def Collect_particle_data(contours_im, pixel_size, multimeasure=False ):    
-    '''
+def Collect_particle_data(contours_im, pixel_size, multimeasure=False):
+    """
     This collects a number of data sets from the contours_im outputted by the find_contours function. Complex measurement of particle size can be done with multimeasure (it measures the distance across each particle at multiple points and then includes max, min, mean and std of these measurements)
 
-    Data collected for each particle in this function: 
+    Data collected for each particle in this function:
         Area - The area of the particle in the image
         Centroid - The center point coordinate of the particle (x, y)
         Aspect ratio - ratio between minimum and maximum length of particle
         Circularity - The area of the particle divided by the area of a circle that completely bounds the particle, giving a value for how circular it is (or how much of a circle it fills)
         width - The width of the smallest possible rectangle that could fully contain the particle
         Height - The height of the smallest possible rectangle that could fully contain the particle
-        radius - The radius of the smallest possible circle that could fully contain the particle. 
+        radius - The radius of the smallest possible circle that could fully contain the particle.
         Major-Minor Ratio  - the ratio between width and height
 
-        Multimeasure specific: 
+        Multimeasure specific:
 
-            Max-diameter 
+            Max-diameter
             Min-diameter
             Mean-diameter
             Stddev-diameter
-            Number of measurements  - the number of measurements across the particle to give the above diameter values. 
+            Number of measurements  - the number of measurements across the particle to give the above diameter values.
 
-        particle_data = { 'Area':area_particle, 'Centroid':centroid_particle, 
-                     'Aspect_ratio':aspect_ratio_particle, 'Perimeter':perimeter_particle, 'Circularity':circularity_particle, 
-                     'Width':width_particle, 'Height':height_particle, 'Radius':radius_particle, 'Major-Minor Ratio':MajorMinorRatio} 
+        particle_data = { 'Area':area_particle, 'Centroid':centroid_particle,
+                     'Aspect_ratio':aspect_ratio_particle, 'Perimeter':perimeter_particle, 'Circularity':circularity_particle,
+                     'Width':width_particle, 'Height':height_particle, 'Radius':radius_particle, 'Major-Minor Ratio':MajorMinorRatio}
 
     Parameters
     ----------
- 
+
         contours_im:list
             As generated from find_contours()
         pixel_size:float
-            Pixel size in the image, the same unit is used in the output data so not important here but worth keeping an eye on. 
+            Pixel size in the image, the same unit is used in the output data so not important here but worth keeping an eye on.
         multimeasure:bool
-            Whether to measure the distance across the particle many times, this can give an idea of the variation in shape and a better measure of diameter, but also  significantly increases runtime. 
-    
+            Whether to measure the distance across the particle many times, this can give an idea of the variation in shape and a better measure of diameter, but also  significantly increases runtime.
+
     Returns
     -------
         particle_data:dict
             A dictionary containing the data collected (with keys describing what the data is)
-    '''
-    num_particle= len(contours_im)
-    #print(num_particle)
-
+    """
+    num_particle = len(contours_im)
+    # print(num_particle)
 
     # this parameter computes the maximum length of a particle i.e. maximum distance between two point of a contour
-    #max_length_particle = np.zeros([num_particle, 1], dtype=float)
+    # max_length_particle = np.zeros([num_particle, 1], dtype=float)
     # this parameter computes the areas of  particles
-    #area_particle = np.zeros([num_particle, 1], dtype=float)
-    area_particle=[]
+    # area_particle = np.zeros([num_particle, 1], dtype=float)
+    area_particle = []
     # this parameter computes the center of the mass of  particles
-    centroid_x_particle =[]
+    centroid_x_particle = []
     centroid_y_particle = []
     centroid_particle = []
     # this parameter computes the ratio between maximum and minimum length of a particle
     aspect_ratio_particle = []
     # this parameter computes the perimeter of particles
     perimeter_particle = []
     # this parameter computes the perimeter of particles
-    #circularity_particle = np.zeros([num_particle, 1], dtype=float)
-    circularity_particle=[]
-    #width_particle =np.zeros([num_particle, 1], dtype = float)
-    #height_particle = np.zeros([num_particle, 1], dtype = float)
+    # circularity_particle = np.zeros([num_particle, 1], dtype=float)
+    circularity_particle = []
+    # width_particle =np.zeros([num_particle, 1], dtype = float)
+    # height_particle = np.zeros([num_particle, 1], dtype = float)
     width_particle = []
     height_particle = []
-    radius_particle= []
-    #meanradius_particle=np.zeros([num_particle, 1],dtype = float)
+    radius_particle = []
+    # meanradius_particle=np.zeros([num_particle, 1],dtype = float)
     MajorMinorRatio = []
 
     if multimeasure:
-        maxlength  = []
+        maxlength = []
         minlength = []
-        meanlength= []
-        stddev_length= [] 
+        meanlength = []
+        stddev_length = []
         measurements = []
-    for (i, c) in enumerate(contours_im):
-        #print(i,c)
+    for i, c in enumerate(contours_im):
+        # print(i,c)
         moment_contour = cv.moments(c)
-        centroid_x=(moment_contour['m10']/moment_contour['m00'])
-        centroid_y=(moment_contour['m01']/moment_contour['m00'])
+        centroid_x = moment_contour["m10"] / moment_contour["m00"]
+        centroid_y = moment_contour["m01"] / moment_contour["m00"]
         centroid_x_particle.append(centroid_x)
         centroid_y_particle.append(centroid_y)
         centroid_particle.append((centroid_x, centroid_y))
-        area = cv.contourArea(c)*pixel_size**2
+        area = cv.contourArea(c) * pixel_size**2
         area_particle.append(area)
-        #meanradius_particle = area__particle[i, 0]
-
+        # meanradius_particle = area__particle[i, 0]
 
-        perimeter_particle.append(cv.arcLength(c, True)*pixel_size)
+        perimeter_particle.append(cv.arcLength(c, True) * pixel_size)
         min_rectangle = cv.minAreaRect(c)
-        #print(min_rectangle)
-        #circularity_particle = 
+        # print(min_rectangle)
+        # circularity_particle =
         width_height = min_rectangle[1]
-        #print(width, height)
-        #width_particle[i, 0]= width*pixel_size
-        #height_particle[i, 0] = height*pixel_size
+        # print(width, height)
+        # width_particle[i, 0]= width*pixel_size
+        # height_particle[i, 0] = height*pixel_size
         height = max(width_height)
         width = min(width_height)
-        width_particle.append(width*pixel_size)
-        height_particle.append(height*pixel_size)
-        MajMinRat = height/width
+        width_particle.append(width * pixel_size)
+        height_particle.append(height * pixel_size)
+        MajMinRat = height / width
         MajorMinorRatio.append(MajMinRat)
         ((cx, cy), radius) = cv.minEnclosingCircle(c)
-        radius_particle.append(radius*pixel_size)
-        circularity_particle.append(area/(np.pi*radius*radius*pixel_size**2))
+        radius_particle.append(radius * pixel_size)
+        circularity_particle.append(area / (np.pi * radius * radius * pixel_size**2))
         box = cv.boxPoints(min_rectangle)
-        box=np.int0(box)
+        box = np.int0(box)
 
-        if multimeasure: 
-            dists,coords = multiMeasure_particle(c, (centroid_x,centroid_y))
-            maxlength.append(max(dists)*pixel_size)
-            minlength.append(min(dists)*pixel_size)
-            meanlength.append(np.mean(dists)*pixel_size)
-            stddev_length.append(np.std(dists)*pixel_size)
+        if multimeasure:
+            dists, coords = multiMeasure_particle(c, (centroid_x, centroid_y))
+            maxlength.append(max(dists) * pixel_size)
+            minlength.append(min(dists) * pixel_size)
+            meanlength.append(np.mean(dists) * pixel_size)
+            stddev_length.append(np.std(dists) * pixel_size)
             measurements.append(len(dists))
-    
 
-    particle_data = { 'Area':area_particle, 'Centroid':centroid_particle, 'Centroid_x':centroid_x_particle, 'Centroid_y':centroid_y_particle,
-                      'Perimeter':perimeter_particle, 'Circularity':circularity_particle, 
-                     'Width':width_particle, 'Height':height_particle, 'Radius':radius_particle, 'Major-Minor Ratio':MajorMinorRatio}  
+    particle_data = {
+        "Area": area_particle,
+        "Centroid": centroid_particle,
+        "Centroid_x": centroid_x_particle,
+        "Centroid_y": centroid_y_particle,
+        "Perimeter": perimeter_particle,
+        "Circularity": circularity_particle,
+        "Width": width_particle,
+        "Height": height_particle,
+        "Radius": radius_particle,
+        "Major-Minor Ratio": MajorMinorRatio,
+    }
     if multimeasure:
-        particle_data['Min diameter'] = minlength
-        particle_data['Max diameter'] = maxlength
-        particle_data['Mean diameter'] = meanlength
-        particle_data['Stddev diameter']=stddev_length
-        particle_data['Measurements']=measurements
-    #print(particle_data)
+        particle_data["Min diameter"] = minlength
+        particle_data["Max diameter"] = maxlength
+        particle_data["Mean diameter"] = meanlength
+        particle_data["Stddev diameter"] = stddev_length
+        particle_data["Measurements"] = measurements
+    # print(particle_data)
     return particle_data
 
-#particle_data=  Collect_particle_data(contours_im, 0.112)
-#print(particle_data['Height'])
-#print(np.mean(particle_data['Height']))
 
-'''
+# particle_data=  Collect_particle_data(contours_im, 0.112)
+# print(particle_data['Height'])
+# print(np.mean(particle_data['Height']))
+
+"""
 PLOT RADIUS DATA
-'''
-#print(np.array(widths))
-#widths_list = [x for i in widths for x in i]
+"""
+
+
+# print(np.array(widths))
+# widths_list = [x for i in widths for x in i]
 def Flatten_list(l):
-    '''
+    """
     Simple function to make a single list from a list of lists, useful for combining data from different frames
 
     Parameters
     ----------
 
         l: list of list of lists
-            These can be created if from the particle_analysis_video function or if you do particle analysis of multiple frames, the data from these can be combined with this function. 
+            These can be created if from the particle_analysis_video function or if you do particle analysis of multiple frames, the data from these can be combined with this function.
     Returns
     -------
-        single list of values 
-    '''
+        single list of values
+    """
     return [x for i in l for x in i]
-    
+
+
 def Convert_to_single_dict(l, combine_data=False):
-    '''
+    """
     Take a list of dictionaries and convert to a single dictionary. This can keep data per image or combine the data from each image, as per requirements
 
     Parameters
     ----------
 
         l: list
             List of dictionaries containing particle data for each image
 
         combine_data:bool
             Do you want the data from each frame separated or together? True for together
-    '''
+    """
     # make an new empty dictionary
     alldata_dict = {}
-    
+
     # Get the keys of the dictionaries
-    
+
     keys = list(l[0].keys())
-    
-    #Create empty options for each key value
+
+    # Create empty options for each key value
     for key in l[0].keys():
-            alldata_dict[key]= [] 
-    
-    #Append the data from each dataset into the new dictionary
+        alldata_dict[key] = []
+
+    # Append the data from each dataset into the new dictionary
     for dset in l:
         for key in dset:
             alldata_dict[key].append(dset[key])
-            
-    alldata_dict['Image number']=[]
+
+    alldata_dict["Image number"] = []
     for x in range(len(l)):
-         alldata_dict['Image number'].append(([x for i in range(len(l[x][key]))]))
+        alldata_dict["Image number"].append(([x for i in range(len(l[x][key]))]))
     if combine_data:
-        
         for key in alldata_dict.keys():
             alldata_dict[key] = Flatten_list(alldata_dict[key])
 
-
-
     return alldata_dict
 
 
 def Sidebyside(Video1, Video2):
-
-    '''
+    """
     Stitches two videos together side by side - (good for comparing masks and originals)
 
     Parameters
     ----------
         Video1:numpy array
             Lefthand video
-        Video2:numpy array 
+        Video2:numpy array
             Righthand video
     Returns
     -------
-        sidebyside: numpy array 
-            Single videos where the two videos play side by side 
-    '''
-    #Videos need to be the same shape. Add video as numpy stack (Z,Y,X ) 
+        sidebyside: numpy array
+            Single videos where the two videos play side by side
+    """
+    # Videos need to be the same shape. Add video as numpy stack (Z,Y,X )
     print(Video1.shape)
-    z1,y1,x1 = Video1.shape
-    z2, y2, x2=Video2.shape
-    sidebyside = np.zeros((max(z1,z2), max(y1,y2), x1+x2),dtype='uint8')
-
-    # this was put here to invert the masked video, DO this BEFORE calling function. 
-    #masksinv=cv.bitwise_not(np.array(masks))
-    sidebyside[:, :, :x1] =Video1
-
-    sidebyside[:, :, x1:] =Video2[:,:,:]
-    #plt.imshow(sidebyside[0], cmap='magma')
-    #plt.show()
+    z1, y1, x1 = Video1.shape
+    z2, y2, x2 = Video2.shape
+    sidebyside = np.zeros((max(z1, z2), max(y1, y2), x1 + x2), dtype="uint8")
+
+    # this was put here to invert the masked video, DO this BEFORE calling function.
+    # masksinv=cv.bitwise_not(np.array(masks))
+    sidebyside[:, :, :x1] = Video1
+
+    sidebyside[:, :, x1:] = Video2[:, :, :]
+    # plt.imshow(sidebyside[0], cmap='magma')
+    # plt.show()
     return sidebyside
 
-def Particle_analysis(image, threshold, minsize, pixel_size,multimeasure=False):
-    '''
+
+def Particle_analysis(image, threshold, minsize, pixel_size, multimeasure=False):
+    """
     Do the thresholding, contours finding and data collection all in one to collect data from the particles  in an image
-    
+
     Parameters
     ----------
-        image:numpy array 
+        image:numpy array
             The image to analyse
         threshold:int
             The threshold pixel value
         minsize:int
-            minimum area of particles 
+            minimum area of particles
         pixel_size:float
-            Pixel size in the image, normally in nanometers but this unit is kept in the resulting data so it doesnt matter. 
+            Pixel size in the image, normally in nanometers but this unit is kept in the resulting data so it doesnt matter.
         Multimeasure:bool
-            Whether to measure the distance across the particle many times, this can give an idea of the variation in shape and a better measure of diameter, but also  significantly increases runtime. 
-    
+            Whether to measure the distance across the particle many times, this can give an idea of the variation in shape and a better measure of diameter, but also  significantly increases runtime.
+
     Returns
     -------
-        mask:numpy array 
+        mask:numpy array
             A binary image showing the particles selected in white.
 
         particle_data:dict
             A dictionary containing the data collected (with keys describing what the data is)
-    '''
+    """
 
     thresh = Threshold(image, threshold)
     contours_im, mask = Find_contours(thresh, minsize)
     particle_data = Collect_particle_data(contours_im, pixel_size, multimeasure)
     return mask, particle_data
 
-def Particle_analysis_video(video,threshold, minsize,pixel_size, multimeasure=False):
-    '''
-    Runs the particle analysis for every frame in a video and creates a dictionary with a list of lists (data from each frame) as the value.  
+
+def Particle_analysis_video(video, threshold, minsize, pixel_size, multimeasure=False):
+    """
+    Runs the particle analysis for every frame in a video and creates a dictionary with a list of lists (data from each frame) as the value.
 
     Parameters
     ----------
-        video:numpy array 
+        video:numpy array
             The video to analyse
         threshold:int
             The threshold pixel value
         minsize:int
-            minimum area of particles 
+            minimum area of particles
         pixel_size:float
-            Pixel size in the image, normally in nanometers but this unit is kept in the resulting data so it doesnt matter. 
+            Pixel size in the image, normally in nanometers but this unit is kept in the resulting data so it doesnt matter.
         Multimeasure:bool
-            Whether to measure the distance across the particle many times, this can give an idea of the variation in shape and a better measure of diameter, but also  significantly increases runtime. 
-    
+            Whether to measure the distance across the particle many times, this can give an idea of the variation in shape and a better measure of diameter, but also  significantly increases runtime.
+
     Returns
     -------
-        mask:numpy array 
+        mask:numpy array
             A binary video showing the particles selected in white.
 
         particle_data:dict
             A dictionary containing the data collected (with keys describing what the data is)
-    '''
-    masks =[]
+    """
+    masks = []
 
-    #video_data ={'Max_length':[], 'Area':[], 'Centroid':[], 
-    #                 'Aspect_ratio':[], 'Perimeter':[], 'Circularity':[], 
-    #                 'Width':[], 'Height':[], 'Radius':[], 'Major-Minor Ratio':[]}  
-    
-    #if multimeasure:
+    # video_data ={'Max_length':[], 'Area':[], 'Centroid':[],
+    #                 'Aspect_ratio':[], 'Perimeter':[], 'Circularity':[],
+    #                 'Width':[], 'Height':[], 'Radius':[], 'Major-Minor Ratio':[]}
+
+    # if multimeasure:
     #    video_data['Min diameter'] = []
     #    video_data['Max diameter'] = []
     #    video_data['Mean diameter'] = []
     #    video_data['Stddev diameter']=[]
     #    video_data['Measurements']=[]
-    #print(particle_data)
+    # print(particle_data)
     video_data = {}
-    
+
     i = 0
-    
+
     for frame in video:
-        mask, data =Particle_analysis(frame, threshold, minsize,pixel_size, multimeasure)
+        mask, data = Particle_analysis(
+            frame, threshold, minsize, pixel_size, multimeasure
+        )
         masks.append(mask)
-        
-        if i==0: 
+
+        if i == 0:
             for key in data.keys():
-                video_data[key]=[]
-            i=1
+                video_data[key] = []
+            i = 1
 
         for key in data:
             video_data[key].append(data[key])
 
     masks = np.array(masks)
     return masks, video_data
 
+
 def multiMeasure_particle(particle_contours, centroid):
-    '''
+    """
     Measures the diameter of the particle at multiple points around the particle by seeing if the angle between any two points on the perimeter and the center of the particle is 180 +/- 1 degree.
 
     Parameters
     ----------
         particle_contours: list
             A list of the coordinates bounding the particle (each list within contours_im)
 
         centroid: array
-            The central coordinate of the particle. 
+            The central coordinate of the particle.
 
     returns
     -------
         distances: list
             A list  of the diameters measured
-        coordinates 
+        coordinates
             The pairs of coordinates measured (point1, center point, point2)
-    '''
+    """
     distances = []
     coords = []
     c = centroid
-    count=0
-    #print(c)
-    #print(contours_im[0])
+    count = 0
+    # print(c)
+    # print(contours_im[0])
     for P1 in particle_contours:
-        #print(P1[0])
+        # print(P1[0])
         for P2 in particle_contours:
-            #print(P1[0][0],P1[0][1],P2[0][1],c[0],P2[0][1] )
-            #print('P1: ', P1)
-            #print('P2: ', P2)
-            #print('c: ', c)
-            ba = P1[0]-c
-            bc = P2[0]-c
+            # print(P1[0][0],P1[0][1],P2[0][1],c[0],P2[0][1] )
+            # print('P1: ', P1)
+            # print('P2: ', P2)
+            # print('c: ', c)
+            ba = P1[0] - c
+            bc = P2[0] - c
 
-            cosine_angle = np.dot(ba,bc)/(np.linalg.norm(ba)*np.linalg.norm(bc))
+            cosine_angle = np.dot(ba, bc) / (np.linalg.norm(ba) * np.linalg.norm(bc))
             angle = np.degrees(np.arccos(cosine_angle))
 
-            if 179<angle<181:
-                #print(angle)
-                count +=1
-                #d = np.linalg.norm(P1[0], P2[0])
-                d = math.hypot(P1[0][0]-P2[0][0], P1[0][1]-P2[0][1])
-                coords.append((P1[0],c, P2[0]))
+            if 179 < angle < 181:
+                # print(angle)
+                count += 1
+                # d = np.linalg.norm(P1[0], P2[0])
+                d = math.hypot(P1[0][0] - P2[0][0], P1[0][1] - P2[0][1])
+                coords.append((P1[0], c, P2[0]))
                 distances.append(d)
     return distances, coords
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_tracking.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_tracking.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,138 @@
+import pandas as pd
 from scipy.spatial import distance as dist
+
 from SimpliPyTEM.Thresholding import *
-import pandas as pd
+
 
 class particle:
-    def __init__(self, centroid,frame_number, frame_index):
-        
+    def __init__(self, centroid, frame_number, frame_index):
         self.current_coordinate = centroid
         self.coordinates = [centroid]
         self.distances = [0]
-        self.pixelsize=None
-        self.frame_numbers= [frame_number]
+        self.pixelsize = None
+        self.frame_numbers = [frame_number]
         self.frame_indices = [frame_index]
-        
+
     def update_coordinate(self, coordinate, frame_num, frame_index):
         self.distances.append(dist.euclidean(self.current_coordinate, coordinate))
         self.coordinates.append(coordinate)
         self.current_coordinate = coordinate
         self.frame_numbers.append(frame_num)
         self.frame_indices.append(frame_index)
-    
+
     def length(self):
         return len(self.coordinates)
-    
+
     def __len__(self):
         return len(self.coordinates)
-    
+
     def mean_distance(self):
         mean = np.mean(self.distances)
         if self.pixelsize:
-            mean=self.pixelsize*mean
+            mean = self.pixelsize * mean
         return mean
-    
+
     def total_displacement(self):
         d = dist.euclidean(self.distances[0], self.current_coordinate)
         if self.pixelsize:
-            d= d*self.pixelsize
+            d = d * self.pixelsize
         return d
-    
+
     def get_area(self, data):
         areas = []
         for x in range(len(self.frame_numbers)):
-            area = data['Area'][self.frame_numbers[x]][self.frame_indices[x]]
+            area = data["Area"][self.frame_numbers[x]][self.frame_indices[x]]
             areas.append(area)
         return area
 
     def get_height_widths(self, data):
-        widths, heights = [], [] 
+        widths, heights = [], []
         for x in range(len(self.frame_numbers)):
-            width = data['Width'][self.frame_numbers[x]][self.frame_indices[x]]
-            height = data['Height'][self.frame_numbers[x]][self.frame_indices[x]]
+            width = data["Width"][self.frame_numbers[x]][self.frame_indices[x]]
+            height = data["Height"][self.frame_numbers[x]][self.frame_indices[x]]
             widths.append(width)
             heights.append(height)
-            
-        return widths, heights    
-    
+
+        return widths, heights
+
     def get_feature(self, data, feature_key):
         property_list = []
-       
+
         y_list = []
         for x in range(len(self.frame_numbers)):
-            #print(x, len(self.frame_numbers), len(self.frame_indices))
+            # print(x, len(self.frame_numbers), len(self.frame_indices))
             prop = data[feature_key][self.frame_numbers[x]][self.frame_indices[x]]
-            if type(prop)==np.ndarray and len(prop)==1:
+            if type(prop) == np.ndarray and len(prop) == 1:
                 property_list.append(float(prop))
-            elif type(prop)==np.ndarray and len(prop)==2:
+            elif type(prop) == np.ndarray and len(prop) == 2:
                 property_list.append(prop[0])
                 y_list.append(prop[1])
             else:
                 property_list.append(prop)
         if y_list:
             return property_list, y_list
         else:
             return property_list
-    
+
     def get_feature_data(self, data):
         df = pd.DataFrame()
-        df['Frame number']=self.frame_numbers
+        df["Frame number"] = self.frame_numbers
         for key in data.keys():
             props = self.get_feature(data, key)
-            if type(props)!=tuple:
-                df[key]= props
-            elif type(props)==tuple and key=='Centroid':
-                df['Centroid_x']=props[0]
-                df['Centroid_y']=props[1]
+            if type(props) != tuple:
+                df[key] = props
+            elif type(props) == tuple and key == "Centroid":
+                df["Centroid_x"] = props[0]
+                df["Centroid_y"] = props[1]
         if self.pixelsize:
-            df['Displacement']=self.distances*pixelsize
+            df["Displacement"] = self.distances * pixelsize
         else:
-            df['Displacement (pix)']=self.distances
+            df["Displacement (pix)"] = self.distances
         self.data_full = df
         return df
 
 
 def get_particles(data, min_dist):
-    # create the list of particles 
+    # create the list of particles
     particle_list = []
-    #It needs a list of current coordinates, I think this has to go here: 
+    # It needs a list of current coordinates, I think this has to go here:
     coordinate_list = []
-    
+
     # This is finding the centroids from the data, as this is the key value. This actually needs to be changed because I've changed it to centroid_x and centroid_y by default.
 
-    centroids = data['Centroid']
+    centroids = data["Centroid"]
 
-    #Compare the distances between the particles in two adjacent frames 
-    for x in range(len(centroids)-1):
-        dists = dist.cdist(centroids[x], centroids[x+1])
-        connectedx, connectedy = np.where(dists<min_dist)
+    # Compare the distances between the particles in two adjacent frames
+    for x in range(len(centroids) - 1):
+        dists = dist.cdist(centroids[x], centroids[x + 1])
+        connectedx, connectedy = np.where(dists < min_dist)
         connected = list(zip(connectedx, connectedy))
-        #print(connected)
-        
+        # print(connected)
+
         for i in connected:
-            #print(i)
+            # print(i)
             coord1 = tuple(centroids[x][i[0]])
-            coord2 = tuple(centroids[x+1][i[1]])
-            #print(coord1, coord2)
-            
+            coord2 = tuple(centroids[x + 1][i[1]])
+            # print(coord1, coord2)
+
             if coord1 not in coordinate_list:
                 p = particle(coord1, x, i[0])
-                p.update_coordinate(coord2, x+1,i[1])
+                p.update_coordinate(coord2, x + 1, i[1])
                 particle_list.append(p)
                 coordinate_list.append(coord2)
             elif coord1 in coordinate_list:
                 ind = coordinate_list.index(coord1)
-                particle_list[ind].update_coordinate(coord2,x+1,i[1])
-                coordinate_list[ind]=coord2
+                particle_list[ind].update_coordinate(coord2, x + 1, i[1])
+                coordinate_list[ind] = coord2
 
     return particle_list
 
 
 def extract_features(particle_list, data, features_list):
-    extracted_features ={}
+    extracted_features = {}
     for feature in features_list:
-        extracted_features[feature]=[]
+        extracted_features[feature] = []
     for p in particle_list:
         df = p.get_feature_data()
         for feature in features_list:
-          extracted_features
-          
+            extracted_features
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/SimpliPyTEM_GUI.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/SimpliPyTEM_GUI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,581 +1,764 @@
 #! /usr/bin/env python3
 import os
-from PyQt5.QtCore import QCoreApplication, Qt
-from PyQt5.QtWidgets import (QApplication, QLabel, QPushButton, QVBoxLayout, QWidget, QHBoxLayout,
-                             QFileDialog, QTextEdit, QTextBrowser, QComboBox, QCheckBox, QMainWindow,QGridLayout,QFileDialog,QLineEdit,QButtonGroup)
-from PyQt5.QtGui import QFont
 import sys
-from SimpliPyTEM.App_functions import * 
-from SimpliPyTEM.PDF_generator import *
-from SimpliPyTEM.html_writer import *
-import threading 
-
+import threading
+import time
+from PyQt6.QtCore import QCoreApplication, Qt
+from PyQt6.QtGui import QFont
+from PyQt6.QtWidgets import (QApplication, QButtonGroup, QCheckBox, QComboBox,
+                             QFileDialog, QGridLayout, QHBoxLayout, QLabel,
+                             QLineEdit, QMainWindow, QPushButton, QTextBrowser,
+                             QTextEdit, QVBoxLayout, QWidget)
+
+from SimpliPyTEM.App_functions import video_processing, isvideo, frames_processing, get_files_from_pattern
+from SimpliPyTEM.html_writer import write_html, write_css, get_files_html
+from SimpliPyTEM.PDF_generator import pdf_generator
+from SimpliPyTEM.Micrograph_class import default_image_pipeline
 
 class MainApplication(QWidget):
     def __init__(self):
         super().__init__()
-        #Qt.AlignHCenter
-
-        self.setGeometry(500, 500, 100,400)
-        self.setWindowTitle('SimpliPyTEM-GUI')
-        
-        self.title = QLabel('SimpliPyTEM-GUI',self)
-        self.title.setObjectName("title")
-        #app.setStyleSheet("QLabel, QCheckBox{font-size: 16pt;}")
-
-
+        # Qt.AlignHCenter
 
+        self.setGeometry(500, 500, 100, 400)
+        self.setWindowTitle("SimpliPyTEM-GUI")
 
-        self.folderlabel = QLabel('Process a folder, a file or \nliveprocessing a folder:')
-        #label.setLayout(layout)
-        #self.label2 = QLabel('Choose whether to process a file, a folder, or live during an imaging session',self)
-        self.title.setAlignment(Qt.AlignCenter)
-
+        self.title = QLabel("SimpliPyTEM-GUI", self)
+        self.title.setObjectName("title")
+        # app.setStyleSheet("QLabel, QCheckBox{font-size: 16pt;}")
 
+        self.folderlabel = QLabel(
+            "Process a folder, a file or \nliveprocessing a folder:"
+        )
+        # label.setLayout(layout)
+        # self.label2 = QLabel('Choose whether to process a file, a folder, or live during an imaging session',self)
+        self.title.setAlignment(Qt.AlignmentFlag.AlignHCenter)
 
-        #Live
-        self.live = 'Folder'
+        # Live
+        self.live = "Folder"
         self.live_choice = QComboBox(self)
-        #live_button.clicked.connect(self.liveCommand)
-        choices = ['Folder', 'File', 'Live Processing']
-        self.folder_option=choices[0]
-        self.live_choice.addItems(['Folder', 'File', 'Live Processing'])
+        # live_button.clicked.connect(self.liveCommand)
+        choices = ["Folder", "File", "Live Processing"]
+        self.folder_option = choices[0]
+        self.live_choice.addItems(["Folder", "File", "Live Processing"])
         self.live_choice.currentTextChanged.connect(self.text_changed)
-        #live_choice.setLayout(layout)
-
+        # live_choice.setLayout(layout)
 
         self.folderpath = None
-        self.folderpath_label = QLabel('')
+        self.folderpath_label = QLabel("")
 
         # For giving an input pattern
-        self.filepattern_label = QLabel('Input File Pattern\ne.g. *.tif means all .tif files (default= *.dm*)\n')
+        self.filepattern_label = QLabel(
+            "Input File Pattern\ne.g. *.tif means all .tif files (default= *.dm*)\n"
+        )
         self.filepattern_box = QLineEdit(self)
-
-        #Checkbox for median filter
-        self.med_check = QCheckBox('Median filter',self)
-        #self.med_check.setEnabled(True)
+        
+        #Contrast enhance check box
+        self.contrast_check = QCheckBox('Enhance Contrast', self)
+        self.contrast_check.toggled.connect(self.update_contrast)
+        self.contrast_state = True
+        self.contrast_check.setChecked(True)
+
+        # Checkbox for median filter
+        self.med_check = QCheckBox("Median filter", self)
+        # self.med_check.setEnabled(True)
         self.med_check.toggled.connect(self.updateMed)
-        self.Med_state=True
+        self.Med_state = True
         self.med_check.setChecked(True)
-        #Value choicec for median filter
-        self.med_filter_value= 3
+        # Value choicec for median filter
+        self.med_filter_value = 3
         self.med_choice = QComboBox(self)
-        self.med_choice.addItems(['3', '5', '7','9','11'])
+        self.med_choice.addItems(["3", "5", "7", "9", "11"])
         self.med_choice.currentTextChanged.connect(self.med_int_changed)
 
-
-        #Checkbox for gaussian filter
-        self.gauss_check = QCheckBox('Gaussian Filter', self)
+        # Checkbox for gaussian filter
+        self.gauss_check = QCheckBox("Gaussian Filter", self)
         self.gauss_check.toggled.connect(self.updateGauss)
         self.gauss_check.setChecked(False)
-        self.Gauss_state=False
+        self.Gauss_state = False
 
-        #value for gaussian filter
-        self.gauss_filter_value= 3
+        # value for gaussian filter
+        self.gauss_filter_value = 3
         self.gauss_choice = QComboBox(self)
-        self.gauss_choice.addItems(['3', '5', '7','9','11'])
+        self.gauss_choice.addItems(["3", "5", "7", "9", "11"])
         self.gauss_choice.currentTextChanged.connect(self.gauss_int_changed)
 
-        # Checkbox for bin 
-        self.bin_check = QCheckBox('Bin image', self)
+        # Checkbox for bin
+        self.bin_check = QCheckBox("Bin image", self)
         self.bin_check.toggled.connect(self.updateBin)
         self.bin_check.setChecked(True)
-        self.Bin_state=True
+        self.Bin_state = True
 
-        #Value for bin
+        # Value for bin
         self.bin_value = 2
-        self.bin_choice=QComboBox(self)
-        self.bin_choice.addItems(['2','4','8'])
+        self.bin_choice = QComboBox(self)
+        self.bin_choice.addItems(["2", "4", "8"])
         self.bin_choice.currentTextChanged.connect(self.gauss_int_changed)
 
-        #Checkbox for scalebar
+        # Checkbox for scalebar
         self.scalebar_on = True
-        self.scalebar_check = QCheckBox('Scalebar', self)
+        self.scalebar_check = QCheckBox("Scalebar", self)
         self.scalebar_check.toggled.connect(self.updateScalebar)
         self.scalebar_check.setChecked(True)
 
+        self.output_type_label = QLabel(
+            'Choose image output type:'
+        )
+        # combo box for output image type
+        self.output_type = 'jpg'
+        self.output_choice = QComboBox(self)
+        self.output_choice.addItems(['jpg', 'tif 8-bit', 'tif 32-bit'])
+        self.output_choice.currentTextChanged.connect(self.output_choice_changed)
+
         # Checkbox for topaz_denoise and using cuda GPU
-        
-        self.topaz_label =  QLabel('Use Topaz Denoising? (requires setup, see docs for details) ')
+
+        self.topaz_label = QLabel(
+            "Use Topaz Denoising? (requires setup, see docs for details) "
+        )
 
         self.topaz_on = False
-        self.topaz_check = QCheckBox('Denoise using Topaz', self)
+        self.topaz_check = QCheckBox("Denoise using Topaz", self)
         self.topaz_check.toggled.connect(self.updateTopaz)
         self.topaz_check.setChecked(False)
 
         self.cuda_on = False
-        self.cuda_check = QCheckBox('Use CUDA GPU', self)
+        self.cuda_check = QCheckBox("Use CUDA GPU", self)
         self.cuda_check.toggled.connect(self.updateCuda)
         self.cuda_check.setChecked(False)
 
-
-
         # Choosing output folder name
-        self.output_folder_label = QLabel('Give the output folder a name:')
-        self.output_folder_box =  QLineEdit(self)
-
-
+        self.output_folder_label = QLabel("Give the output folder a name:")
+        self.output_folder_box = QLineEdit(self)
 
-
-        #Video options :
-        self.video_label =  QLabel('If there are videos, choose how video files are handled, else ignore: ')
-        self.video_status='Save Average'
+        # Video options :
+        self.video_label = QLabel(
+            "If there are videos, choose how video files are handled, else ignore: "
+        )
+        self.video_status = "Save Average"
 
         self.video_choice = QComboBox(self)
-        #live_button.clicked.connect(self.liveCommand)
-        videochoices = ['Save Average', 'Save Tif Stack', 'Save Tif Sequence', 'Save Video as .mp4', 'Save video as .avi', 'Save MotionCorrected Average']
-        
+        # live_button.clicked.connect(self.liveCommand)
+        videochoices = [
+            "Save Average",
+            "Save Tif Stack",
+            "Save Tif Sequence",
+            "Save Video as .mp4",
+            "Save video as .avi",
+            "Save MotionCorrected Average",
+        ]
+
         self.video_choice.addItems(videochoices)
         self.video_choice.currentTextChanged.connect(self.video_choice_changed)
 
-
-        self.doc_label1 = QLabel('Document Section')
-        self.doc_label1.setObjectName('doc_label')
-        self.doc_label1.setAlignment(Qt.AlignCenter)
-
-        self.doc_label=QLabel('Following generation of images/videos, use this section to create \n an html or pdf file to display the resulting images:')
-        self.title_box_label = QLabel('Give a title for the experiment:')
+        self.doc_label1 = QLabel("Document Section")
+        self.doc_label1.setObjectName("doc_label")
+        self.doc_label1.setAlignment(Qt.AlignmentFlag.AlignHCenter)
+
+        self.doc_label = QLabel(
+            "Following generation of images/videos, use this section to create \n an html or pdf file to display the resulting images:"
+        )
+        self.title_box_label = QLabel("Give a title for the experiment:")
         self.title_box = QLineEdit()
-        self.notes_box_label=  QLabel('Add some notes here:')
+        self.notes_box_label = QLabel("Add some notes here:")
         self.notes_box = QTextEdit()
 
-
-
-        #Call other functions
+        # Call other functions
         self.make_buttons()
-        #self.video_checkbox_functions()
-        
+        # self.video_checkbox_functions()
+
         self.set_layouts()
         self.add_styles()
         self.set_fonts()
         self.show()
 
     def make_buttons(self):
-        #folder browse button
-        self.FolderBrowse_button = QPushButton('Choose Folder', self)
+        # folder browse button
+        self.FolderBrowse_button = QPushButton("Choose Folder", self)
         self.FolderBrowse_button.clicked.connect(self.FileFolderChooser)
 
-        #self.FolderBrowse_button.setStyleSheet("background-color : White")
+        # self.FolderBrowse_button.setStyleSheet("background-color : White")
 
-        #Run button 
-        self.Run_button = QPushButton('Run!', self)
+        # Run button
+        self.Run_button = QPushButton("Run!", self)
         self.Run_button.clicked.connect(self.RunCommand)
 
-        #html button
-        self.html_button = QPushButton('Make HTML!')
+        # html button
+        self.html_button = QPushButton("Make HTML!")
         self.html_button.clicked.connect(self.html_command)
 
-        #pdf button
-        self.pdf_button  = QPushButton('Make PDF!')
+        # pdf button
+        self.pdf_button = QPushButton("Make PDF!")
         self.pdf_button.clicked.connect(self.pdf_command)
 
-        #stop button
-        self.stopButton = QPushButton('Stop Process')
+        # stop button
+        self.stopButton = QPushButton("Stop Process")
         self.stopButton.clicked.connect(self.stopCommand)
-        self.stopButton.setObjectName('stopButton')
-        self.stopSignal=False
+        self.stopButton.setObjectName("stopButton")
+        self.stopSignal = False
+
     def add_styles(self):
-        #app.setStyleSheet(" QCheckBox{font-size: 14pt;}")
-        #app.setStyleSheet("QPushButton{background-color:White;font-size:16pt;font-weight:500;}")
-        app.setStyleSheet('''*{font-family:"helvetica", serif; font-weight:200} QWidget{background-color:#C2E4E9;} \
+        # app.setStyleSheet(" QCheckBox{font-size: 14pt;}")
+        # app.setStyleSheet("QPushButton{background-color:White;font-size:16pt;font-weight:500;}")
+        app.setStyleSheet(
+            """*{font-family:"helvetica", serif; font-weight:200} QWidget{background-color:#C2E4E9;} \
             QPushButton:hover{background-color: #D8BBEA; color:black;} \
             QPushButton{background-color:white;font-size:16pt;font-weight:500;}  \
             QPushButton.active{background-color:#502673}
             QCheckBox{background-color:white;font-size: 11pt; } \
             QLabel{font-size:12pt;font-weight:400;}\
             QComboBox{background-color:white;font-size:10px;vertical-align:text-top;}\
             QTextEdit{background-color:white;} \
             QLineEdit{background-color:white}\
             #stopButton:hover{background-color:#F2B8D5}\
             QLabel#title{font-size:18pt; font-weight:700;}
             QLabel#doc_label{font-size:15pt; font-weight:600;}
-            ''')
+            """
+        )
 
     def set_fonts(self):
-        #define title font
+        # define title font
         self.titlefont = QFont()
         self.titlefont.setPointSize(20)
-        self.titlefont.setBold(True)  
+        self.titlefont.setBold(True)
         # add title font to title and doc section title
         self.title.setFont(self.titlefont)
         self.doc_label1.setFont(self.titlefont)
 
-
-        #define and set video label font 
+        # define and set video label font
         self.video_labelfont = QFont()
         self.video_labelfont.setPointSize(12)
         self.video_labelfont.setItalic(True)
         self.video_label.setFont(self.video_labelfont)
 
-        #define button font - Easier done in the add_styles method
- 
-
-        #self.button_font = QFont()
-        #self.button_font.setPointSize(16)
-        #self.button_font.setBold(True) 
-        #self.button_font.setItalic(True)
-
-        #set button fonts
-        #self.FolderBrowse_button.setFont(self.button_font)
-        #self.Run_button.setFont(self.button_font)
-        #self.html_button.setFont(self.button_font)
-        #self.pdf_button.setFont(self.button_font)
-
+        # define button font - Easier done in the add_styles method
 
+        # self.button_font = QFont()
+        # self.button_font.setPointSize(16)
+        # self.button_font.setBold(True)
+        # self.button_font.setItalic(True)
+
+        # set button fonts
+        # self.FolderBrowse_button.setFont(self.button_font)
+        # self.Run_button.setFont(self.button_font)
+        # self.html_button.setFont(self.button_font)
+        # self.pdf_button.setFont(self.button_font)
 
     def set_layouts(self):
         self.layout = QGridLayout()
         self.setLayout(self.layout)
-        self.layout.addWidget(self.title,0,0, 1,2)
-        self.layout.addWidget(self.folderlabel,1,0,1,1)
-        self.layout.addWidget(self.live_choice,1,1,1,1)
-        self.layout.addWidget(self.FolderBrowse_button, 2,0,1,2)
-        self.layout.addWidget(self.folderpath_label, 3,0,1,2)
-        self.layout.addWidget(self.filepattern_label,4,0,1,1)
-        self.layout.addWidget(self.filepattern_box,4,1,1,1)
-
-        self.layout.addWidget(self.med_check,5,0,1,1)
-        self.layout.addWidget(self.med_choice,5,1,1,1)
-
-        self.layout.addWidget(self.gauss_check,6,0,1,1)
-        self.layout.addWidget(self.gauss_choice,6,1,1,1)
-        self.layout.addWidget(self.bin_check,7,0,1,1)
-        self.layout.addWidget(self.bin_choice,7,1,1,1)
-
-        self.layout.addWidget(self.scalebar_check, 8,0,1,1)
-
-        self.layout.addWidget(self.topaz_label, 9,0,1,2)        
-        self.layout.addWidget(self.topaz_check, 10,0,1,1)
-        self.layout.addWidget(self.cuda_check, 10,1,1,1)
-
-        self.layout.addWidget(self.output_folder_label, 11,0,1,1)
-        self.layout.addWidget(self.output_folder_box,11,1,1,1)
-
-        self.layout.addWidget(self.video_label, 12,0,1,2)
-        self.layout.addWidget(self.video_choice, 13, 0,1,2)
-        #self.layout.addWidget(self.video_option1,9,0,1,1)
-        #self.layout.addWidget(self.video_option2,9,1,1,1)
-        #self.layout.addWidget(self.video_option3,10,0,1,1)
-        #self.layout.addWidget(self.video_option4,10,1,1,1)
-        self.layout.addWidget(self.Run_button, 15,0,2,2)
-        self.layout.addWidget(self.stopButton, 17,0,1,2)
-        self.layout.addWidget(self.doc_label1, 18,0,1,2)
-        self.layout.addWidget(self.doc_label, 19, 0,1,2)
-        self.layout.addWidget(self.title_box_label, 20, 0,1,1)
-        self.layout.addWidget(self.title_box,21,0,1,2)
-        self.layout.addWidget(self.notes_box_label, 22,0,1,1)
-        self.layout.addWidget(self.notes_box, 23,0,1,3)
-
-        self.layout.addWidget(self.html_button, 27,0,1,1)
-        self.layout.addWidget(self.pdf_button, 27,1,1,1)
+        i = 0
+        self.layout.addWidget(self.title, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.folderlabel, i, 0, 1, 1)
+        self.layout.addWidget(self.live_choice, i, 1, 1, 1)
+        i+=1
+        self.layout.addWidget(self.FolderBrowse_button, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.folderpath_label, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.filepattern_label, i, 0, 1, 1)
+        self.layout.addWidget(self.filepattern_box, i, 1, 1, 1)
+        i+=1
+        self.layout.addWidget(self.contrast_check, i, 0,1,1)
+        i+=1
+        self.layout.addWidget(self.med_check, i, 0, 1, 1)
+        self.layout.addWidget(self.med_choice, i, 1, 1, 1)
+        i+=1
+        self.layout.addWidget(self.gauss_check, i, 0, 1, 1)
+        self.layout.addWidget(self.gauss_choice, i, 1, 1, 1)
+        i+=1
+        self.layout.addWidget(self.bin_check, i, 0, 1, 1)
+        self.layout.addWidget(self.bin_choice, i, 1, 1, 1)
+        i+=1
+        self.layout.addWidget(self.scalebar_check, i, 0, 1, 1)
+        i+=1
+        self.layout.addWidget(self.output_type_label, i,0,1,1)
+        self.layout.addWidget(self.output_choice, i, 1, 1,1)
+        i+=1
+        self.layout.addWidget(self.topaz_label, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.topaz_check, i, 0, 1, 1)
+        self.layout.addWidget(self.cuda_check, i, 1, 1, 1)
+        i+=1
+        self.layout.addWidget(self.output_folder_label, i, 0, 1, 1)
+        self.layout.addWidget(self.output_folder_box, i, 1, 1, 1)
+        i+=1
+        self.layout.addWidget(self.video_label, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.video_choice, i, 0, 1, 2)
+        i+=2
+        # self.layout.addWidget(self.video_option1,9,0,1,1)
+        # self.layout.addWidget(self.video_option2,9,1,1,1)
+        # self.layout.addWidget(self.video_option3,10,0,1,1)
+        # self.layout.addWidget(self.video_option4,10,1,1,1)
+        self.layout.addWidget(self.Run_button, i, 0, 2, 2)
+        i+=2
+        self.layout.addWidget(self.stopButton, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.doc_label1, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.doc_label, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.title_box_label, i, 0, 1, 1)
+        i+=1
+        self.layout.addWidget(self.title_box, i, 0, 1, 2)
+        i+=1
+        self.layout.addWidget(self.notes_box_label, i, 0, 1, 1)
+        i+=1
+        self.layout.addWidget(self.notes_box, i, 0, 1, 3)
+        i+=4
+        self.layout.addWidget(self.html_button, i, 0, 1, 1)
+        self.layout.addWidget(self.pdf_button, i, 1, 1, 1)
 
     def video_checkbox_functions(self):
-                #Video options checkboxes:
+        # Video options checkboxes:
         self.video_group = QButtonGroup()
-        
-        self.video_option1 = QCheckBox('Save Average', self)
-        self.video_option2 = QCheckBox('Save Video as mp4', self)
-        self.video_option3 = QCheckBox('Save Tif Stack', self)
-        self.video_option4 = QCheckBox('Save MotionCorrected average', self)
+
+        self.video_option1 = QCheckBox("Save Average", self)
+        self.video_option2 = QCheckBox("Save Video as mp4", self)
+        self.video_option3 = QCheckBox("Save Tif Stack", self)
+        self.video_option4 = QCheckBox("Save MotionCorrected average", self)
         self.video_group.buttonClicked.connect(self.video_group_func)
-        self.video_status='Save Average'
+        self.video_status = "Save Average"
         self.video_group.addButton(self.video_option1)
         self.video_group.addButton(self.video_option2)
         self.video_group.addButton(self.video_option3)
         self.video_group.addButton(self.video_option4)
 
     def stopCommand(self):
-
-        self.stopSignal=True
-        print('Stopping before next file')
+        self.stopSignal = True
+        print("Stopping before next file")
 
     def eval_stop(self):
-        if self.stopSignal==True:
-            print('Stop signal recieved, exiting now')
-            self.stopSignal=False
+        if self.stopSignal == True:
+            print("Stop signal recieved, exiting now")
+            self.stopSignal = False
             return True
 
-    def text_changed(self, s): # i is an int
-        self.folder_option=s 
-    def med_int_changed(self,i):
-        self.med_filter_value=int(i)
-    def gauss_int_changed(self,i):
-        self.gauss_filter_value=int(i)
-    def bin_int_changed(self,i):
-        self.bin_value=int(i)
-    def updateGauss(self,state):
-        self.Gauss_state=state
-    def updateMed(self,state):
-        self.Med_state=state
-    def updateBin(self,state):
+    def update_contrast(self, state):
+        self.contrast_state=state
+
+    def text_changed(self, s):  # i is an int
+        self.folder_option = s
+
+    def med_int_changed(self, i):
+        self.med_filter_value = int(i)
+
+    def gauss_int_changed(self, i):
+        self.gauss_filter_value = int(i)
+
+    def bin_int_changed(self, i):
+        self.bin_value = int(i)
+
+    def updateGauss(self, state):
+        self.Gauss_state = state
+
+    def updateMed(self, state):
+        self.Med_state = state
+
+    def updateBin(self, state):
         self.Bin_state = state
-    def updateScalebar(self,state):
-        self.scalebar_on=state
+
+    def output_choice_changed(self, s):
+        self.output_type=s
+    def updateScalebar(self, state):
+        self.scalebar_on = state
+
     def video_group_func(self, but):
-        self.video_status = (but.text())
+        self.video_status = but.text()
+
     def video_choice_changed(self, s):
         self.video_status = s
+
     def updateTopaz(self, state):
         self.topaz_on = state
+
     def updateCuda(self, state):
-        self.cuda_on=  state
+        self.cuda_on = state
 
     def FileFolderChooser(self):
-        if self.folder_option=='Folder' or self.folder_option=='Live Processing':
-            self.folderpath = QFileDialog.getExistingDirectory(self, 'Select a Folder')
+        if self.folder_option == "Folder" or self.folder_option == "Live Processing":
+            self.folderpath = QFileDialog.getExistingDirectory(self, "Select a Folder")
         else:
-            self.folderpath = QFileDialog.getOpenFileName(self, 'Select a File')[0]
+            self.folderpath = QFileDialog.getOpenFileName(self, "Select a File")[0]
         self.folderpath_label.setText(self.folderpath)
 
     def html_command(self):
         outdir = self.output_folder_box.text()
 
-        if outdir=='':
-            outdir='.'
+        if outdir == "":
+            outdir = "."
 
-        if self.folderpath=='' or self.folderpath==None:
-            print('Please select a folder/file')
+        if self.folderpath == "" or self.folderpath == None:
+            print("Please select a folder/file")
             return 1
 
         cwd = os.getcwd()
-        os.chdir(self.folderpath+'/'+outdir)
+        os.chdir(self.folderpath + "/" + outdir)
 
         title = self.title_box.text()
-        if title=='':
-            title = 'Default_title'
+        if title == "":
+            title = "Default_title"
         notes = self.notes_box.toPlainText()
-        print('Writing html and css files')
-        try: 
-            image_files, video_files = get_files('Images', 'Videos')
-        except FileNotFoundError: 
-            print('The Images folder was not found, please make sure that the output folder defined above has a folder of images called images.')
+        print("Writing html and css files")
+        try:
+            image_files, video_files = get_files_html("Images", "Videos")
+        except FileNotFoundError:
+            print(
+                "The Images folder was not found, please make sure that the output folder defined above has a folder of images called images."
+            )
             os.chdir(cwd)
             return 1
         print(image_files)
 
         write_html(image_files, video_files, title, notes)
         write_css()
-        print('Done!')
+        print("Done!")
         os.chdir(cwd)
 
     def pdf_command(self):
         outdir = self.output_folder_box.text()
-        if outdir=='':
-            outdir='.'
-
+        if outdir == "":
+            outdir = "."
 
-        if self.folderpath=='' or self.folderpath==None:
-            print('Please select a folder/file')
+        if self.folderpath == "" or self.folderpath == None:
+            print("Please select a folder/file")
             return 1
 
         cwd = os.getcwd()
-        os.chdir(self.folderpath+'/'+outdir)
-
+        os.chdir(self.folderpath + "/" + outdir)
 
         title = self.title_box.text()
         notes = self.notes_box.toPlainText()
-        
+
         print(os.getcwd())
-        print(os.listdir('.'))
-        try: 
-            images = ['Images/'+x for x in os.listdir('Images') if 'jpg' in x]
-        except FileNotFoundError: 
-            print('The Images folder was not found, please make sure that the output folder defined above has a folder of images called images.')
+        print(os.listdir("."))
+        try:
+            images = ["Images/" + x for x in os.listdir("Images") if "jpg" in x]
+        except FileNotFoundError:
+            print(
+                "The Images folder was not found, please make sure that the output folder defined above has a folder of images called images."
+            )
             os.chdir(cwd)
             return 1
         print(images)
         try:
             pdf_generator(images, title, notes)
         except Exception as e:
-            print('Error! Not sure what has happened here')
+            print("Error! Not sure what has happened here")
             print(e)
         os.chdir(cwd)
 
     def RunCommand(self):
-        #print('Gauss=', self.Gauss_state)
-        #print('Med=',self.Med_state)
-        #print('med_value',self.med_filter_value)
-        #print('Bin=',self.Bin_state)
-        #print('Folder:' ,self.folder_option)
-        
-        
-        outdir = self.output_folder_box.text()
-        if outdir=='':
-            outdir='.'
-        elif '\n' in outdir:
-            outdir.replace('\n','')
-
+        # print('Gauss=', self.Gauss_state)
+        # print('Med=',self.Med_state)
+        # print('med_value',self.med_filter_value)
+        # print('Bin=',self.Bin_state)
+        # print('Folder:' ,self.folder_option)
 
-        if self.Med_state==False:
-            self.med_filter_value=0
-        if self.Gauss_state==False:
-            self.gauss_filter_value=0
-        if self.Bin_state==False:
-            self.bin_value=0
+        outdir = self.output_folder_box.text()
+        if outdir == "":
+            outdir = "."
+        elif "\n" in outdir:
+            outdir.replace("\n", "")
+
+        if self.Med_state == False:
+            self.med_filter_value = 0
+        if self.Gauss_state == False:
+            self.gauss_filter_value = 0
+        if self.Bin_state == False:
+            self.bin_value = 0
 
-        if self.folderpath=='' or self.folderpath==None:
-            print('Please select a folder/file')
+        if self.folderpath == "" or self.folderpath == None:
+            print("Please select a folder/file")
             return 1
         print(self.folderpath)
-        
-        try: 
-            if self.folder_option=='Folder':
-                    print('Running folder?')
-                    thread = threading.Thread(target =self.process_folder, args=(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.scalebar_on, self.video_status, self.topaz_on, self.cuda_on ))
-                    thread.start()
-            elif self.folder_option=='File':
-                    print(self.live)    
-                    self.process_file(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.scalebar_on,self.video_status,self.topaz_on, self.cuda_on  )
-            elif self.folder_option =='Live Processing':
-                    #live_process_folder(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.video_status )
-                    print('Live processing')
-                    thread = threading.Thread(target=self.live_process, args=(self.folderpath,outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.scalebar_on,self.video_status,self.topaz_on, self.cuda_on  ))
-                    thread.start()
+        print('Contrast_state', self.contrast_state)
+        try:
+            if self.folder_option == "Folder":
+                print("Running folder?")
+                thread = threading.Thread(
+                    target=self.process_folder,
+                    args=(
+                        self.folderpath,
+                        outdir,
+                        self.output_type,
+                        self.contrast_state,
+                        self.bin_value,
+                        self.med_filter_value,
+                        self.gauss_filter_value,
+                        self.scalebar_on,
+                        self.video_status,
+                        self.topaz_on,
+                        self.cuda_on,
+                    ),
+                )
+                thread.start()
+            elif self.folder_option == "File":
+                print(self.live)
+                self.process_file(
+                    self.folderpath,
+                    outdir,
+                    self.output_type,
+                    self.contrast_state,
+                    self.bin_value,
+                    self.med_filter_value,
+                    self.gauss_filter_value,
+                    self.scalebar_on,
+                    self.video_status,
+                    self.topaz_on,
+                    self.cuda_on,
+                )
+            elif self.folder_option == "Live Processing":
+                # live_process_folder(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.video_status )
+                print("Live processing")
+                thread = threading.Thread(
+                    target=self.live_process,
+                    args=(
+                        self.folderpath,
+                        outdir,
+                        self.output_type,
+                        self.contrast_state,
+                        self.bin_value,
+                        self.med_filter_value,
+                        self.gauss_filter_value,
+                        self.scalebar_on,
+                        self.video_status,
+                        self.topaz_on,
+                        self.cuda_on,
+                    ),
+                )
+                thread.start()
         except Exception as e:
-
-            print('Whoops there is an error, check the terminal and your inputs and try again.')
+            print(
+                "Whoops there is an error, check the terminal and your inputs and try again."
+            )
             print(e)
 
-    def process_folder(self,folder, output_folder_name,xybin, medfilter, gaussian_filter,scalebar_on, video_status, topaz_on, cuda_on):
+    def process_folder(
+        self,
+        folder,
+        output_folder_name,
+        output_type,
+        contrast_state,
+        xybin,
+        medfilter,
+        gaussian_filter,
+        scalebar_on,
+        video_status,
+        topaz_on,
+        cuda_on,
+    ):
         start_time = time.time()
-        print('Processing folder!')
+        print("Processing folder!")
         cwd = os.getcwd()
 
         os.chdir(folder)
 
-#        dm_files = [x for x in os.listdir('.') if x[-4:-1]=='.dm']
-#        dm_vids = [x for x in dm_files if isvideo(x)]
-#        dm_frames = [x for x in dm_files if x[-9]=='-' and x[-13:-9].isdigit() and x[-8:-4].isdigit()]
-#        dm_ims = [x for x in dm_files if x not in dm_vids and x not in dm_frames]   
-
+        #        dm_files = [x for x in os.listdir('.') if x[-4:-1]=='.dm']
+        #        dm_vids = [x for x in dm_files if isvideo(x)]
+        #        dm_frames = [x for x in dm_files if x[-9]=='-' and x[-13:-9].isdigit() and x[-8:-4].isdigit()]
+        #        dm_ims = [x for x in dm_files if x not in dm_vids and x not in dm_frames]
 
         pattern = self.filepattern_box.text()
-        if pattern=='':
-            pattern='*dm*'
+        if pattern == "":
+            pattern = "*dm*"
         im_files, vid_files, dm_frames = get_files_from_pattern(pattern)
 
-        print('Imfiles', im_files)
-        print('Vidfiles', vid_files)
-        print('dm_frames', dm_frames)
+        print("Imfiles", im_files)
+        print("Vidfiles", vid_files)
+        print("dm_frames", dm_frames)
 
-        if output_folder_name not in os.listdir('.') and output_folder_name!='.':
+        if output_folder_name not in os.listdir(".") and output_folder_name != ".":
             os.mkdir(output_folder_name)
 
         for file in vid_files:
             print(self.stopSignal)
             if self.eval_stop():
-                return 1 
-            print('Processing: ', file)
-            video_processing(filename=file,output_folder_name=output_folder_name,xybin=xybin, medfilter=medfilter, gaussian_filter=gaussian_filter,scalebar_on=scalebar_on, video_status=video_status, topaz_denoise=topaz_on, denoise_with_cuda=cuda_on )
+                return 1
+            print("Processing: ", file)
+            video_processing(
+                filename=file,
+                output_folder_name=output_folder_name,
+                output_type=output_type,
+                contrast_enhance=contrast_state,
+                xybin=xybin,
+                medfilter=medfilter,
+                gaussian_filter=gaussian_filter,
+                scalebar_on=scalebar_on,
+                video_status=video_status,
+                topaz_denoise=topaz_on,
+                denoise_with_cuda=cuda_on,
+            )
 
-        for  file in im_files:
+        for file in im_files:
             if self.eval_stop():
-                return 1 
-            default_image_pipeline(file, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,scalebar=scalebar_on,outdir=output_folder_name, topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
-        if len(dm_frames)!=0: 
+                return 1
+            default_image_pipeline(
+                file,
+                output_type=output_type,
+                contrast_enhance=contrast_state,
+                xybin=xybin,
+                medfilter=medfilter,
+                gaussfilter=gaussian_filter,
+                scalebar=scalebar_on,
+                outdir=output_folder_name,
+                topaz_denoise=topaz_on,
+                denoise_with_cuda=cuda_on,
+            )
+        if len(dm_frames) != 0:
             print(dm_frames)
-            frames_processing(dm_frames,output_folder_name,xybin, medfilter, gaussian_filter, video_status )
-        print('All files in folder complete!')  
-        running_time = time.time()-start_time
-        print('Running time for {} images and {} videos: {}'.format(len(im_files),len(vid_files), running_time))
+            frames_processing(
+                dm_frames,
+                output_folder_name,
+                output_type,
+                xybin,
+                medfilter,
+                gaussian_filter,
+                video_status,
+            )
+        print("All files in folder complete!")
+        running_time = time.time() - start_time
+        print(
+            "Running time for {} images and {} videos: {}".format(
+                len(im_files), len(vid_files), running_time
+            )
+        )
         os.chdir(cwd)
 
-
-    def live_process(self, folder, output_folder_name,xybin, medfilter, gaussian_filter, scalebar_on,video_status, topaz_on, cuda_on):
+    def live_process(
+        self,
+        folder,
+        output_folder_name,
+        output_type,
+        contrast_state,
+        xybin,
+        medfilter,
+        gaussian_filter,
+        scalebar_on,
+        video_status,
+        topaz_on,
+        cuda_on,
+    ):
         cwd = os.getcwd()
-        #print('calling function')
+        # print('calling function')
         os.chdir(folder)
-        files = os.listdir('.')
+        files = os.listdir(".")
         file_set = set(files)
         start_time = time.time()
         max_running_time = 3600
-        #print(os.getcwd())
-        if output_folder_name not in os.listdir('.') and output_folder_name!='.':
+        # print(os.getcwd())
+        if output_folder_name not in os.listdir(".") and output_folder_name != ".":
             os.mkdir(output_folder_name)
-        
+
         pattern = self.filepattern_box.text()
-        if pattern=='':
-            pattern='*dm*'
-                
-        possible_filetypes = ['.avi', '.mp4', '.dm3', '.dm4', '.tif', '.jpg', ]
-        
+        if pattern == "":
+            pattern = "*dm*"
+
+        possible_filetypes = [
+            ".avi",
+            ".mp4",
+            ".dm3",
+            ".dm4",
+            ".tif",
+            ".jpg",
+        ]
+
         while True:
             if self.eval_stop():
-                    return 1 
+                return 1
 
             im_files, vid_files, dm_frames = get_files_from_pattern(pattern)
-            
-            for file in im_files+vid_files+dm_frames:
+
+            for file in im_files + vid_files + dm_frames:
                 if file not in file_set:
-                    #print(file)
-                    if file[-4:].lower() in  possible_filetypes:
+                    # print(file)
+                    if file[-4:].lower() in possible_filetypes:
                         # this is to check the file isnt still being written, if it grows in size, it ignores if for now and loops again:
                         currentsize = os.path.getsize(file)
-                        time.sleep(1)      
-                        if os.path.getsize(file)>currentsize:
+                        time.sleep(1)
+                        if os.path.getsize(file) > currentsize:
                             break
 
-
-
-                        if isvideo(file) and video_status!='Save Average':
-                            video_processing(file,output_folder_name,xybin, medfilter, gaussian_filter, scalebar_on=scalebar_on,video_status=video_status,topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
+                        if isvideo(file) and video_status != "Save Average":
+                            video_processing(
+                                file,
+                                output_folder_name,
+                                output_type,
+                                contrast_state,
+                                xybin,
+                                medfilter,
+                                gaussian_filter,
+                                scalebar_on=scalebar_on,
+                                video_status=video_status,
+                                topaz_denoise=topaz_on,
+                                denoise_with_cuda=cuda_on,
+                            )
                         else:
-                            default_image_pipeline(file, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,outdir=output_folder_name,topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
-                    
-                        
+                            default_image_pipeline(
+                                file,
+                                output_type=output_type,
+                                xybin=xybin,
+                                contrast_enhance=contrast_state,
+                                medfilter=medfilter,
+                                gaussfilter=gaussian_filter,
+                                outdir=output_folder_name,
+                                topaz_denoise=topaz_on,
+                                denoise_with_cuda=cuda_on,
+                            )
 
                     file_set.add(file)
-                
+
             running_time = time.time() - start_time
-            print('Running time : {}s'.format(round(running_time,0)))
-            
-            if running_time>max_running_time:
+            print("Running time : {}s".format(round(running_time, 0)))
+
+            if running_time > max_running_time:
                 break
             time.sleep(10)
-            #print('Looping')      
-        print('Time out reached, exiting now')
+            # print('Looping')
+        print("Time out reached, exiting now")
         os.chdir(cwd)
 
-    def process_file(self,folderpath, outdir, bin_value, med_filter_value, gauss_filter_value,scalebar_on, video_status ):
+    def process_file(
+        self,
+        folderpath,
+        outdir,
+        output_type,
+        contrast_state,
+        bin_value,
+        med_filter_value,
+        gauss_filter_value,
+        scalebar_on,
+        video_status,
+    ):
         if isvideo(file):
-            video_processing(folderpath, outdir, xybin =bin_value, medfilter=med_filter_value, gaussian_filter=gauss_filter_value, scalebar_on=scalebar_on,video_status= video_status)
+            video_processing(
+                folderpath,
+                outdir,
+                output_type,
+                contrast_state,
+                xybin=bin_value,
+                medfilter=med_filter_value,
+                gaussian_filter=gauss_filter_value,
+                scalebar_on=scalebar_on,
+                video_status=video_status,
+            )
         else:
-            default_image_pipeline(filename, xybin = xybin, medfilter=med_filter_value, gaussfilter=gauss_filter_value,scalebar=scalebar_on,outdir=outdir)
-
-'''
-class JobRunner(QRunnable):
-
-    signals = WorkerSignals()
-
-    def __init__(self):
-        super().__init__()
-
-        self.is_paused = False
-        self.is_killed = False
-
-    @pyqtSlot()
-    def run(self):
-        for n in range(100):
-            self.signals.progress.emit(n + 1)
-            time.sleep(0.1)
-
-            while self.is_paused:
-                time.sleep(0)
-
-            if self.is_killed:
-                break
+            default_image_pipeline(
+                filename,
+                output_type=output_type,
+                contrast_enhance=contrast_state,
+                xybin=bin_value,
+                medfilter=med_filter_value,
+                gaussfilter=gauss_filter_value,
+                scalebar=scalebar_on,
+                outdir=outdir,
+            )
 
-    def pause(self):
-        self.is_paused = True
 
-    def resume(self):
-        self.is_paused = False
 
-    def kill(self):
-        self.is_killed = True
-'''
-#MainApplication.show()
-#application.exec()
+# MainApplication.show()
+# application.exec()
 app = QApplication(sys.argv)
 ex = MainApplication()
-sys.exit(app.exec_())
+sys.exit(app.exec())
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM/html_writer.py` & `SimpliPyTEM-1.0.6/SimpliPyTEM/html_writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,145 @@
-from airium import Airium
 import os
 
-def write_html(images, videos=None, title='Default_experiment_title', notes='', **kwargs):
-    '''
-    Writes html file containing the images and videos from an experiment so they can be viewed on a webbrowser. This can be preferable over PDFS as the videos can be played. 
-    The images and videos are only linked in this html, so in order to share the page these need to be sent as well. 
+from airium import Airium
+
+
+def write_html(
+    images, videos=None, title="Default_experiment_title", notes="", **kwargs
+):
+    """
+    Writes html file containing the images and videos from an experiment so they can be viewed on a webbrowser. This can be preferable over PDFS as the videos can be played.
+    The images and videos are only linked in this html, so in order to share the page these need to be sent as well.
 
     Parameters
     ----------
         Images:list
             List of images (including their path from the current directory), can be made with get_files()
 
         Videos: list
             List of videos (including their path from the current directory), can be made with get_files()
-        
+
         title:str
             The title for the experiment (name of html doc and title of the resulting page)
-    
+
         notes:str
             Accompanying notes for the experiment, included at the top of the doc.
 
     Output
     ------
         HTML document {title}.html saved in the current working directory. This html document has the images from an experiment as well as playable videos.
-    '''
+    """
     print(images)
-    a =Airium()
-    with a.html(lang='en'):
+    images.sort()
+    videos.sort()
+    a = Airium()
+    with a.html(lang="en"):
         with a.head():
-            a.meta(charset='utf-8', content='width=device-width')
-            a.title(_t='')
-            a.link(href="style.css", rel='stylesheet', type='text/css')
+            a.meta(charset="utf-8", content="width=device-width")
+            a.title(_t="")
+            a.link(href="style.css", rel="stylesheet", type="text/css")
         with a.body():
-            with a.div(klass='banner'):
+            with a.div(klass="banner"):
                 with a.h1():
                     if title:
-                        a(title.replace('_', ' ').strip('.html'))
+                        a(title.replace("_", " ").strip(".html"))
                 with a.h3():
                     a(notes)
             with a.h2():
-                a('Images')
-            with a.ul(klass='Image_group'):
+                a("Images")
+            with a.ul(klass="Image_group"):
                 for image in images:
-
                     print(image)
-                    image_name = image.strip('.jpg').split('/')[-1].replace('_', ' ')
-                    
+                    image_name = image.strip(".jpg").split("/")[-1].replace("_", " ")
+
+                    #                    with a.h3():
+                    #                        a(image.strip('.jpg').split('/')[-1].replace('_', ' '))
 
-    #                    with a.h3():
-    #                        a(image.strip('.jpg').split('/')[-1].replace('_', ' '))
-                    
                     with a.li():
-                        with a.a(href=''):
-                            a.img(src=image, alt=image_name)    
+                        with a.a(href=""):
+                            a.img(src=image, alt=image_name)
                             with a.p():
                                 a(image_name)
-                            a.img(src=image, alt=image_name, klass='preview')    
-            if  videos:
-                with a.div(klass='Videos'):
+                            a.img(src=image, alt=image_name, klass="preview")
+            if videos:
+                with a.div(klass="Videos"):
                     with a.h2():
-                        a('Videos')
-                    with a.ul(klass='Video_group'):
+                        a("Videos")
+                    with a.ul(klass="Video_group"):
                         for video in videos:
                             with a.li():
-
-                                with a.video('controls', width=600,height=600):
+                                with a.video("controls", width=600, height=600):
                                     a.source(src=video, type="video/mp4")
                                 with a.p():
-                                    a(video.strip('.mp4').split('/')[-1].replace('_',' '))
-
-        if 'outdir' in kwargs:
-            outdir = kwargs['outdir']
-            title = outdir + '/' + title
-        title+='.html'
-
-
-    with open(title, 'w') as f:
-        f.write(str(a))        
-
-
-
-def get_files( imagedir, videodir=None, image_pattern='', video_pattern=''):
-    '''
-    Simple method for getting the image and video files. 
+                                    a(
+                                        video.strip(".mp4")
+                                        .split("/")[-1]
+                                        .replace("_", " ")
+                                    )
+
+        if "outdir" in kwargs:
+            outdir = kwargs["outdir"]
+            title = outdir + "/" + title
+        title += ".html"
+
+    with open(title, "w") as f:
+        f.write(str(a))
+
+
+def get_files_html(imagedir, videodir=None, image_pattern="", video_pattern=""):
+    """
+    Simple method for getting the image and video files.
 
     Parameters
     ----------
 
         imagedir:str
             Directory containing the images (jpg, png or tif format)
         videodir:str
             Directory containing videos. Videos must  be .mp4
         image_pattern:str
-            Pattern which the images contain, it is assumed they will be .jpg but if any more specific patterns in the filename are required (E.g. to  only include a single sample) It can be added here. 
+            Pattern which the images contain, it is assumed they will be .jpg but if any more specific patterns in the filename are required (E.g. to  only include a single sample) It can be added here.
         video_pattern:str
-            As image pattern but for videos. 
-        
-    '''
-    #current_dir = os.getcwd()
-    #os.chdir(directory) 
-    image_files = [imagedir+'/'+x for x in os.listdir(imagedir) if x[-3:]=='jpg' or x[-3:]=='tif' or x[-3:]=='png' and image_pattern in x]
-    #print(image_files)
-    if videodir and videodir in os.listdir('.'):
-        video_files = [videodir+'/'+x for x in os.listdir(videodir) if x[-3:]=='mp4' and video_pattern in x]
+            As image pattern but for videos.
+
+    """
+    # current_dir = os.getcwd()
+    # os.chdir(directory)
+    image_files = [
+        imagedir + "/" + x
+        for x in os.listdir(imagedir)
+        if x[-3:] == "jpg" or x[-3:] == "tif" or x[-3:] == "png" and image_pattern in x
+    ]
+    # print(image_files)
+    if videodir and videodir in os.listdir("."):
+        video_files = [
+            videodir + "/" + x
+            for x in os.listdir(videodir)
+            if x[-3:] == "mp4" and video_pattern in x
+        ]
     else:
         video_files = []
-    #print(video_files)
-    #os.chdir(current_dir)
+    # print(video_files)
+    # os.chdir(current_dir)
     return image_files, video_files
 
 
-
-
 def write_css(outdir=None):
-    '''
-    Writes a basic css document called style.css, this is linked in the html generated. This gives it some basic formatting. You may consider making your own css for better formatting. 
+    """
+    Writes a basic css document called style.css, this is linked in the html generated. This gives it some basic formatting. You may consider making your own css for better formatting.
 
-    '''
+    """
 
     if outdir:
-        cssname = outdir+'/style.css'
+        cssname = outdir + "/style.css"
     else:
-        cssname='style.css' 
-    with open(cssname, 'w') as f:
-        f.write('''
+        cssname = "style.css"
+    with open(cssname, "w") as f:
+        f.write(
+            """
 *
 {
     border: 0;
     margin: 0;
     padding: 0;
 }
 
@@ -276,17 +288,19 @@
     float: left;
     padding: 10px 10px 10px 10px;
     position: relative;
     margin: auto;
 
 }
 
-''')
+"""
+        )
+
 
-if __name__=='__main__':
+if __name__ == "__main__":
     directory = os.getcwd()
-    title = input('Give a title for the experiment: ')
-    title=title.replace(' ', '_')
-    images, videos = get_files('Images', 'Videos')
+    title = input("Give a title for the experiment: ")
+    title = title.replace(" ", "_")
+    images, videos = get_files("Images", "Videos")
     print(images)
     write_html(images, videos, title=title)
     write_css()
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/PKG-INFO` & `SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpliPyTEM
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package to simplify the processing and analysis of TEM and in situ TEM images and videos
 Home-page: https://github/gabriel-ing/Micrograph-analysis-scripts
 Author: Gabriel Ing
 Author-email: ucbtgrb@ucl.ac.uk
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/SOURCES.txt` & `SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.5/setup.py` & `SimpliPyTEM-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from setuptools import setup 
 
 setup(
 	name='SimpliPyTEM',
-	version='1.0.5',
+	version='1.0.6',
 	description='A python package to simplify the processing and analysis of TEM and in situ TEM images and videos',
 	long_description='''SimpliPyTEM is a python package to make python-based analysis of Transmission electron microscopy images easier and more approachable. Although TEM is the focus, this could also easily be adapted to other microscopy images. Importantly, SimpliPyTEM is designed to make automated, basic work accessible for beginners (through a simple GUI), while more complicated methods can be accessed through simple python code. This package centers around the image data being held in a Numpy array which makes the image data easy to access for further analysis.
 	This project aims to make use of the rapid automation of image analysis methods available through python while making it approachable for the user.
 	Functions to generate pdf and html files containing images and videos are also included in this package. This allows easy viewing and sharing of all the images/videos taken in an imaging session, making experiment evaluation significantly easier. 
 	For more info, please see: https://micrograph-analysis-scripts.readthedocs.io/en/latest/''',
 	url='https://github/gabriel-ing/Micrograph-analysis-scripts',
 	author='Gabriel Ing',
 	author_email='ucbtgrb@ucl.ac.uk',
 	license = 'GPL-3.0',
 	packages =['SimpliPyTEM'],
 	install_requires=['numpy',
-	 'ncempy',
-	 'Pillow',
-	 'mrcfile',
-	 'moviepy',
-	 'airium',
+	 'ncempy==1.10.0',
+	 'Pillow==9.4.0',
+	 'mrcfile==1.4.3',
+	 'moviepy==1.0.3',
+	 'airium==0.2.5',
 	 'matplotlib',
-	 'opencv-python',
-	 'tifffile',
-	 'notebook',
-	 'scikit-image',
-	 'imutils',
-	 'fpdf',
-	 'PyQt5',
+	 'opencv-python==4.7.0.72',
+	 'tifffile==2023.3.21',
+	 'notebook==7.0.0b2',
+	 'scikit-image==0.20.0',
+	 'imutils==0.5.4',
+	 'fpdf==1.7.2',
+	 'PyQt6==6.5.0',
 	 'sphinx',
 	 'sphinx_rtd_theme',
 	 'nbsphinx',
-	 'pandas',
-	 'seaborn'],
+	 'pandas==1.5.3',
+	 'seaborn==0.12.2'],
 	entry_points={'console_scripts':['SimpliPyTEM-GUI = SimpliPyTEM.SimpliPyTEM_GUI:main']},
 	classifiers=[
 		'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',  
         'Operating System :: POSIX :: Linux',     
         'Programming Language :: Python :: 3',
```

