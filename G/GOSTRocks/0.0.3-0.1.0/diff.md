# Comparing `tmp/GOSTRocks-0.0.3-py2.py3-none-any.whl.zip` & `tmp/GOSTRocks-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,17 @@
-Zip file size: 22999 bytes, number of entries: 11
+Zip file size: 24498 bytes, number of entries: 15
 -rw-r-----  2.0 unx        0 b- defN 20-Nov-03 12:23 GOSTRocks/__init__.py
--rw-r-----  2.0 unx    10173 b- defN 22-May-04 23:00 GOSTRocks/metadataMisc.py
--rw-r-----  2.0 unx    11209 b- defN 22-Mar-16 01:48 GOSTRocks/misc.py
--rw-r-----  2.0 unx     2835 b- defN 22-Apr-13 21:24 GOSTRocks/ntlMisc.py
--rw-r-----  2.0 unx    17398 b- defN 20-Nov-03 12:23 GOSTRocks/osmMisc.py
--rw-r-----  2.0 unx    24446 b- defN 22-May-26 14:26 GOSTRocks/rasterMisc.py
--rw-r-----  2.0 unx     1076 b- defN 22-May-26 14:31 GOSTRocks-0.0.3.dist-info/LICENSE
--rw-r-----  2.0 unx      934 b- defN 22-May-26 14:31 GOSTRocks-0.0.3.dist-info/METADATA
--rw-r-----  2.0 unx      110 b- defN 22-May-26 14:31 GOSTRocks-0.0.3.dist-info/WHEEL
--rw-r-----  2.0 unx       10 b- defN 22-May-26 14:31 GOSTRocks-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      865 b- defN 22-May-26 14:31 GOSTRocks-0.0.3.dist-info/RECORD
-11 files, 69056 bytes uncompressed, 21551 bytes compressed:  68.8%
+-rw-r-----  2.0 unx      213 b- defN 23-Jan-23 15:08 GOSTRocks/awsMisc.py
+-rw-r-----  2.0 unx     2871 b- defN 23-Jun-27 12:45 GOSTRocks/dataMisc.py
+-rw-r-----  2.0 unx     1026 b- defN 23-Feb-13 15:43 GOSTRocks/ghslMisc.py
+-rw-r-----  2.0 unx     5791 b- defN 23-Jun-26 19:24 GOSTRocks/mapMisc.py
+-rw-r-----  2.0 unx    10993 b- defN 23-Jun-27 12:47 GOSTRocks/metadataMisc.py
+-rw-r-----  2.0 unx     7173 b- defN 23-Jun-27 12:51 GOSTRocks/misc.py
+-rw-r-----  2.0 unx     3707 b- defN 23-Jun-26 19:29 GOSTRocks/ntlMisc.py
+-rw-r-----  2.0 unx    14072 b- defN 23-Jun-26 19:36 GOSTRocks/osmMisc.py
+-rw-r-----  2.0 unx    21372 b- defN 23-Jun-27 12:27 GOSTRocks/rasterMisc.py
+-rw-r-----  2.0 unx     1076 b- defN 23-Jun-27 14:50 GOSTRocks-0.1.0.dist-info/LICENSE
+-rw-r-----  2.0 unx     1349 b- defN 23-Jun-27 14:50 GOSTRocks-0.1.0.dist-info/METADATA
+-rw-r-----  2.0 unx       92 b- defN 23-Jun-27 14:50 GOSTRocks-0.1.0.dist-info/WHEEL
+-rw-r-----  2.0 unx       10 b- defN 23-Jun-27 14:50 GOSTRocks-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1173 b- defN 23-Jun-27 14:50 GOSTRocks-0.1.0.dist-info/RECORD
+15 files, 70918 bytes uncompressed, 22582 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,10 +1,22 @@
 Filename: GOSTRocks/__init__.py
 Comment: 
 
+Filename: GOSTRocks/awsMisc.py
+Comment: 
+
+Filename: GOSTRocks/dataMisc.py
+Comment: 
+
+Filename: GOSTRocks/ghslMisc.py
+Comment: 
+
+Filename: GOSTRocks/mapMisc.py
+Comment: 
+
 Filename: GOSTRocks/metadataMisc.py
 Comment: 
 
 Filename: GOSTRocks/misc.py
 Comment: 
 
 Filename: GOSTRocks/ntlMisc.py
@@ -12,23 +24,23 @@
 
 Filename: GOSTRocks/osmMisc.py
 Comment: 
 
 Filename: GOSTRocks/rasterMisc.py
 Comment: 
 
-Filename: GOSTRocks-0.0.3.dist-info/LICENSE
+Filename: GOSTRocks-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: GOSTRocks-0.0.3.dist-info/METADATA
+Filename: GOSTRocks-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: GOSTRocks-0.0.3.dist-info/WHEEL
+Filename: GOSTRocks-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: GOSTRocks-0.0.3.dist-info/top_level.txt
+Filename: GOSTRocks-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: GOSTRocks-0.0.3.dist-info/RECORD
+Filename: GOSTRocks-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## GOSTRocks/metadataMisc.py

```diff
@@ -1,49 +1,53 @@
-import os, re, json, logging
+import os, logging
 
-import geojson
 import rasterio # v1.0.21 (latest v1.2.10)
-import fiona # v1.8.4 (latest v1.8.21)
 
-import numpy as np # v1.18.1 (latest v1.21.5)
 import pandas as pd # v1.0.3 (latest v1.4.1)
 import geopandas as gpd # v0.6.3 (latest v0.10.2)
 
 import seaborn as sns
-import matplotlib # v3.2.1 (latest v3.5.1)
-import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
 
 from rasterio.plot import show
-from shapely.geometry import shape, GeometryCollection
+from shapely.geometry import shape
 from shapely.wkt import loads
-from matplotlib import colors
-from tqdm.notebook import tqdm
+from tqdm import tqdm
 from pyproj.crs.crs import CRS
 
 try:
     import arcpy # v2.6
     from arcgis.features import GeoAccessor, GeoSeriesAccessor
 except:
-    print("Could not import arcgis libraries")
+    print("METADATA Library: Could not import arcgis libraries")
     
 vector_file_types = ['.shp','.kml','.geojson']
-raster_file_types = ['.tif','.tiff','.geotiff','.geotif']
+raster_file_types = ['.TIF','.tif','.tiff','.geotiff','.geotif']
 
 
 ### TODO: 
 # 1. Add searching through ESRI geodatabases
 # 2. Add support to include tables (xlsx, csv)
    
 class metadata_gost:
     ''' Create standardized metadata for folders of geospatial data
     '''
     
     def __init__(self, input_dir, output_dir, type="Folder"):
+        """ Create standardized metadata for folders of geospatial data
+
+        :param input_dir: Folder to search for geospatial layers
+        :type input_dir: str
+        :param output_dir: Where to create output metadata files
+        :type output_dir: str
+        :param type: What we are searching, defaults to "Folder"
+        :type type: str, optional
+        """
         self.input_dir = input_dir
+        if not os.path.exists(input_dir):
+            raise(ValueError("Input directory does not exist"))
         self.output_dir = output_dir
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
         
     def get_layers(self):
         ''' Iterate through self.input_dir and get list of vector and raster data '''
         vector_files = []
@@ -74,21 +78,19 @@
                      'owner name':owner,
                      'owner email':email}
         base_pd = pd.DataFrame([base_info]).transpose()
         if layer_metadata is None:
            layer_metadata = self.metaPD
         if field_metadata is None:
            field_metadata = self.fieldsPD
-         
+        
         with pd.ExcelWriter(out_file, engine='openpyxl', mode='w', if_sheet_exists='replace') as writer:
            base_pd.to_excel(writer, 'dataset info', encoding='utf8')
            layer_metadata.to_excel(writer, 'layer_summaries', encoding='utf8')
-           if field_metadata:
-               field_metadata.to_excel(writer, 'field_summaries', encoding='utf8')
-        
+           field_metadata.to_excel(writer, 'field_summaries', encoding='utf8')
     
     def generate_metadata(self, vector_files=None, raster_files=None):
         ''' Generate metadata for vector and raster files
         
         Args:
             vector_files [optional, list] - list of paths to vector_files, if none, defaults to list generated through get_list_of_layers
             raster_files [optional, list] - list of paths to raster_files, if none, defaults to list generated through get_list_of_layers
@@ -127,23 +129,23 @@
         if raster_files is None:
             raster_files = self.raster_files
             
         metadata = []
         field_defs = []
         for vector_file in vector_files:            
             try:
-                cur_meta = vector_file_metadata(vector_file)
+                cur_meta = vector_file_metadata(vector_file, in_folder=self.input_dir)
                 metadata.append(cur_meta.get_metadata())
                 field_defs.append(cur_meta.get_field_summaries())
             except:
-                logging.error(f"Cannot log {raster_file}")
+                logging.error(f"Cannot log {vector_file}")
             
         for raster_file in raster_files:
             try:
-                cur_meta = raster_file_metadata(raster_file)
+                cur_meta = raster_file_metadata(raster_file, in_folder=self.input_dir)
                 metadata.append(cur_meta.get_metadata())
             except:
                 logging.error(f"Cannot log {raster_file}")
             
         metaPD = pd.DataFrame(metadata)
         metaPD['layer_label'] = ''
         metaPD['description'] = ''
@@ -162,21 +164,28 @@
             except:
                 final = cur_pd
         try:
             fieldsPD = final.reset_index()
             self.fieldsPD = fieldsPD
         except:
             fieldsPD = None
-            self.fieldsPD = None            
+            self.fieldsPD = None  
+        self.metaPD.sort_values(['folder',"layer_name"], inplace=True)
+        self.fieldsPD.sort_values(["layer_name", "field_name"], inplace=True)
+        
         return({'metadata':metaPD, 'fields':fieldsPD})            
 
 class raster_file_metadata:
-    def __init__(self, path):
+    def __init__(self, path, in_folder=''):
         self.path = path
         self.layer_name = os.path.splitext((os.path.basename(path)))[0]
+        if in_folder == '':
+            self.dir_name = os.path.dirname(path)
+        else:
+            self.dir_name = os.path.dirname(path).replace(in_folder, '')
         self.data_type = "Raster"
         
         curR = rasterio.open(path)
         
         cur_crs = CRS.from_wkt(curR.crs.wkt)        
         self.crs_name = cur_crs.name
         self.crs_code = curR.crs.to_epsg()
@@ -196,29 +205,35 @@
         self.min_lon = b[0]
         self.min_lat = b[1]
         self.max_lon = b[2]
         self.max_lat = b[3]        
         
     def get_metadata(self):
         return({'layer_name': self.layer_name, 
+                'folder': self.dir_name,
                 'data_type': self.data_type, 
                 'crs_name': self.crs_name, 'crs_code': self.crs_code, 
                 'num_dimensions': self.num_dimensions,
                 'min_lon': self.min_lon, 
                 'max_lon': self.max_lon, 
                 'min_lat': self.min_lat, 
                 'max_lat': self.max_lat, 
                 'raster_width': self.raster_width,
                 'raster_height': self.raster_height,
                 'raster_res': self.raster_res})
               
 class vector_file_metadata:
-    def __init__(self, path):
+    def __init__(self, path, in_folder=''):
         self.path = path
+        self.in_folder = ''
         self.layer_name = os.path.splitext((os.path.basename(path)))[0]
+        if in_folder == '':
+            self.dir_name = os.path.dirname(path)
+        else:
+            self.dir_name = os.path.dirname(path).replace(in_folder, '')
         self.data_type = "Vector"
         
         curD = gpd.read_file(path)
         self.curD = curD
         self.crs_name = curD.crs.name
         self.crs_code = curD.crs.to_epsg()
         self.num_dimensions = curD.shape[1]
```

## GOSTRocks/misc.py

```diff
@@ -1,153 +1,84 @@
-import os, sys, time, math, subprocess, inspect, json, glob, logging
+import time, math, logging
 
 import geopandas as gpd
 import pandas as pd
-import shapely
-import fiona 
-import pyproj
-import rasterio
-import numpy
-import ogr
+import numpy as np
 
-from collections import Counter
 from math import ceil
-from rtree import index
-from shapely.geometry import shape, Point, Polygon
-from affine import Affine
-from rasterio.features import rasterize
+from shapely.geometry import Point, Polygon
 
 wgs84 = {'init':'epsg:4326'}
 
-def loggingInfo():
-    logging.basicConfig(format='%(asctime)s:%(levelname)s: %(message)s', level=logging.INFO)
+def loggingInfo(lvl = logging.INFO):
+    """ Set logging settings to info (default) and print useful information
+
+    :param lvl: logging level for setting, defaults to logging.INFO
+    :type lvl: logging.INFO
+    """
+    logging.basicConfig(format='%(asctime)s:%(levelname)s: %(message)s', level=lvl)
 
-def renameDir(dir):
-    '''
-    Renames all files in a directory
-    Used to add .dat to all ENVI files, but not their headers
-    '''
-    for f in os.listdir(dir):
-        title = os.path.basename(pathAndFilename)
-        os.rename(pathAndFilename, os.path.join(dir, "%s.dat" % title))
-
-def listFiles(inFolder, pattern):
-    outFiles = []
-    for f in os.listdir(inFolder):
-        if f.endswith(pattern):
-            outFiles.append(os.path.join(inFolder, f))
-        elif os.path.isdir(os.path.join(inFolder, f)):
-            outFiles = outFiles + listFiles(os.path.join(inFolder, f), pattern)
-    return(outFiles)
 
-'''prints the time along with the message'''
 def tPrint(s):
+    '''prints the time along with the message'''
     print("%s\t%s" % (time.strftime("%H:%M:%S"), s))
 
 def round_to_1(x):
     return(round(x, -int(math.floor(math.log10(x)))))
 
-# Create an interable range made with decimal point steps
 def drange(start, stop, step):
+    ''' Create an interable range made with decimal point steps '''
     r = start
     while r < stop:
         yield r
         r += step    
-'''
-Get the index of a specific [val] within a list of histogram values
-'''
-def getHistIndex(hIdx, val, maxVal=2000):
+
+def getHistIndex(hIdx, val):
+    """ Get the index of a specific [val] within a list of histogram values
+
+    :param hIdx: list of values (from histogram calculation)
+    :type hIdx: list of numbers
+    :param val: value to search for
+    :type val: number
+    :return: index in hIdx where val falls
+    :rtype: int
+    """
+    lastH = 0
     for h in range(0, len(hIdx)):
         curH = hIdx[h]
         if curH > val:
             return(lastH)        
         lastH = h
     return(len(hIdx) -1)
 
-'''
-Convert a list of values into a percent of total 
-'''    
+def listSum(inD):
+    """get sum of values in list
+
+    :param inD: list of numbers
+    :type inD: list
+    """
+    total = 0
+    for x in inD:
+        total += x
+    return(total)
+
 def getHistPer(inD):
+    ''' Convert a list of values into a percent of total 
+    
+    :param inD: list of values
+    :type inD: list of numbers
+    :return: list of values of same length of inD.
+    :rtype: list of float
+    '''  
     tSum = listSum(inD)
     for hIdx in range(0,len(inD)):
         inD[hIdx] = inD[hIdx] / tSum
     return(inD)
-    
-
-def generateVRT(inFiles, outVRT, 
-        gdalVRTfunction=r"C:\Python27\ArcGIS10.3\Lib\site-packages\osgeo\gdalbuildvrt.exe", fileList="C:/Temp/VRTList.txt"):
-    vrtFile = open(fileList, 'w')
-    for f in inFiles:
-        vrtFile.write("%s\n" % f)
-    vrtFile.close()
-    subprocess.call("%s -input_file_list %s %s" % (gdalVRTfunction, fileList, outVRT))
-    os.remove(fileList)
-    
-def getUrbanParams():
-    thisFolder = os.path.realpath(os.path.abspath(os.path.split(inspect.getfile( inspect.currentframe() ))[0]))
-    inputParameters = "%s/Urban/urbanParameters.json" % thisFolder
-    with open(inputParameters, 'r') as data_file:                 
-        jsonParams = json.load(data_file)
-    return jsonParams
-    
-def getParams():
-    '''
-    '''
-    thisFolder = os.path.realpath(os.path.abspath(os.path.split(inspect.getfile( inspect.currentframe() ))[0]))
-    inputParameters = "%s/importantParameters.json" % thisFolder    
-    with open(inputParameters, 'r') as data_file:                 
-        jsonParams = json.load(data_file)
-    return jsonParams
-    
-def selectByIntersection(allAdmin, inD, exact=False):
-    ''' Select features from allAdmin that intersect inD
-    allAdmin [shapely geometry] - describes the feature of interest
-    inD [geopandas dataframe] - features to be intersected
-    exact (optional) [boolean] - perform exact geometry match, default is False, which
-                                 will only calculate bounding box intersection
-    RETURNS [geopandas dataframe] - subset of inD that intersects allAdmin
-    EXAMPLE:
-        inS = gpd.read_file(sourceFile)   
-        inD = gpd.read_file(intersectingFile)        
-        if inS.crs != inD.crs:
-            inS = inS.to_crs(inD.crs)
-        allAdmin = shapely.ops.cascaded_union(MultiPolygon(inS['geometry'].tolist()))
-        selectByIntersection(allAdmin, inD, exact=False)
-    TODO: Projection checks
-    '''
-    #Read the source boundaries into an rtree opbject
-    idxAdmin = index.Index()    
-    try:
-        for i, shape in enumerate(allAdmin):
-            idxAdmin.insert(i, shape.bounds)
-    except:
-        idxAdmin.insert(0, allAdmin.bounds)
-    #Enumerate through the intersecting file
-    intersectingList = []
-    for i, row in inD.iterrows():
-        interSection = list(idxAdmin.intersection(row['geometry'].bounds))
-        if len(interSection):
-            intersectingList.append(row)
-            
-    returnDF = gpd.GeoDataFrame(intersectingList) 
-    returnDF.crs = inD.crs
-    
-    if exact:
-        selData = []
-        for j, origRow in returnDF.iterrows():    
-            xx = allAdmin.intersects(origRow['geometry'])
-            print ("%s - %s" % (j, xx))
-            if xx:
-                selData.append(origRow)
-            returnDF = gpd.GeoDataFrame(selData) 
-    return returnDF
 
 def tabulateUnq(unqResults, verbose=False, columnPrefix="c"):
-    cnt = 0
-    tResults = len(unqResults)
     allVals = []
     for r in unqResults:
         allVals.append(r[0].tolist())
     flattened = [val for sublist in allVals for val in sublist] 
     unq = np.unique(np.array(flattened)).tolist()
     #unqCols = ["c_%s" % xxx for xxx in unq]
     allRes = []
@@ -156,40 +87,52 @@
             curRes = [0] * len(unq)
             for idx in range(0, len(r[0].tolist())):
                 curRes[unq.index(r[0].tolist()[idx])] = r[1].tolist()[idx]
         except:
             print (r)
         allRes.append(curRes)
     return pd.DataFrame(allRes, columns=["%s_%s" % (columnPrefix, xxx) for xxx in unq])    
-
-def get_box(row, col, l, r, b, t, gridWidth, gridHeight):
-    ll = Point(l + (row * gridWidth), b + (col + gridHeight))
-    ul = Point(l + (row * gridWidth), t + (col + gridHeight))
-    ur = Point(r + (row * gridWidth), t + (col + gridHeight))
-    lr = Point(r + (row * gridWidth), b + (col + gridHeight))
-    box = Polygon([ll, ul, ur, lr, ll])
-    return(box)
-
-def get_point(row, col, l, r, b, t, gridWidth, gridHeight):
-    pt = Point((l+r)/2 + (col*gridWidth), (t+b)/2  - (row * gridHeight))
-    return(pt)    
-
-def createFishnet_gdf(inD, outFile, type='POLY'):
-    ''' create a fishnet for each polygon in an input dataframe
-    '''
-    if res.geometry[0].type != "Polygon":
-        raise(ValueError("Input dataframe must be Polygonal"))
     
 def createFishnet(xmin,xmax,ymin,ymax,gridHeight,gridWidth,type='POLY',crsNum=4326,outputGridfn=''):
-    ''' Create a fishnet shapefile inside the defined coordinates 
-    outputGridfn: output shapefile to hold the grid
-    xmin,xmax,ymin,ymax: coordinates for the extent of the fishnet
-    gridHeight,gridWidth: dimensions of the grid cells in the outpout fishnet
-    '''    
-   # convert sys.argv to float
+    """ Create a fishnet shapefile inside the defined coordinates
+
+    :param xmin: minimum longitude
+    :type xmin: float
+    :param xmax: maximum longitude
+    :type xmax: float
+    :param ymin: minimum latitude
+    :type ymin: float
+    :param ymax: maximum latitude
+    :type ymax: float
+    :param gridHeight: resolution of the grid cells in crsNum units
+    :type gridHeight: float
+    :param gridWidth: resolution of the grid cells in crsNum units
+    :type gridWidth: float
+    :param type: geometry type of output fishnet, defaults to 'POLY'
+    :type type: str, optional
+    :param crsNum: units of output crs, defaults to 4326
+    :type crsNum: int, optional
+    :param outputGridfn: path for output shapefile, defaults to '', which creates no shapefile
+    :type outputGridfn: str, optional
+    :return: geodataframe of fishnet
+    :rtype: gpd.GeoDataFrame
+    """
+    
+    def get_box(row, col, l, r, b, t, gridWidth, gridHeight):
+        ll = Point(l + (row * gridWidth), b + (col + gridHeight))
+        ul = Point(l + (row * gridWidth), t + (col + gridHeight))
+        ur = Point(r + (row * gridWidth), t + (col + gridHeight))
+        lr = Point(r + (row * gridWidth), b + (col + gridHeight))
+        box = Polygon([ll, ul, ur, lr, ll])
+        return(box)
+
+    def get_point(row, col, l, r, b, t, gridWidth, gridHeight):
+        pt = Point((l+r)/2 + (col*gridWidth), (t+b)/2  - (row * gridHeight))
+        return(pt)    
+    # convert sys.argv to float
     xmin = float(xmin)
     xmax = float(xmax)
 
     ymin = float(ymin)
     ymax = float(ymax)
     gridWidth = float(gridWidth)
     gridHeight = float(gridHeight)
@@ -214,62 +157,21 @@
                 box = get_point(rowIdx, colIdx, ringXleftOrigin, ringXrightOrigin, ringYbottomOrigin, ringYtopOrigin, gridWidth, gridHeight)
             all_res.append([rowIdx, colIdx, box])
     res = gpd.GeoDataFrame(pd.DataFrame(all_res, columns=['rowIdx', 'colIdx', 'geometry']), geometry='geometry', crs=f'epsg:{crsNum}')
     if outputGridfn != '':
         res.to_file(outputGridfn)
     return(res)
 
-def getVIIRSFiles(baseFolder=r"R:\GLOBAL\NTL\VIIRS", years="all", months="all", tile=-1, retType="images"):
-    '''
-    Get list of VIIRS files based on input filtering
-    '''  
-    returnList = {}
-    for root, dirs, files in os.walk(baseFolder):
-        for f in files:
-            if f[-3:] == "tif":
-                curNames = root.split("\\")
-                try:
-                    tile = curNames[5]
-                    date = curNames[4]
-                    if "vcmcfg_v10" in f or "vcm-orm-ntl" in f:
-                        if "avg_rade9" in f:
-                            try:
-                                returnList[date].append(os.path.join(root, f))
-                            except:
-                                returnList[date] = [os.path.join(root, f)]
-                except:
-                    pass
-    return(returnList)
-
-def getNTLFiles(baseFolder=r"Q:\GLOBAL\NTL\DMSP", years="all", months="all", tile=-1, retType="images"):
-    '''
-    Get list of VIIRS files based on input filtering
-    '''  
-    returnList = {}
-    for root, dirs, files in os.walk(baseFolder):
-        for f in files:
-            if f[-3:] == "tif":
-                curNames = root.split(".")
-                try:
-                    date = curNames[0]
-                    if "_ElvidgeCorrected_gt3" in f or "_Corrected" in f:
-                        try:
-                            returnList[date].append(os.path.join(root, f))
-                        except:
-                            returnList[date] = [os.path.join(root, f)]
-                except:
-                    pass
-    return(returnList)
-
 def explodeGDF(indf):
     ''' Convert geodataframe with multi-part polygons to one with single part polygons
-    INPUT
-    indf [Geopandas geodataframe]
-    RETURNS
-    [Geopandas geodataframe]
+    
+    :param indf: input geodataframe to explode
+    :type indf: gpd.GeoDataFrame
+    :return: exploded geodaatframe
+    :rtype: gpd.GeoDataFrame
     '''
     outdf = gpd.GeoDataFrame(columns=indf.columns)
     outdf.crs = indf.crs
     for idx, row in indf.iterrows():
         row.geometry.type
         if row.geometry.type in ["Polygon", "Point"]:
             outdf = outdf.append(row,ignore_index=True)
@@ -281,19 +183,18 @@
                 multdf.loc[geom,'geometry'] = row.geometry[geom]
             outdf = outdf.append(multdf,ignore_index=True)
     return(outdf)
 
 def project_UTM(inD):
     ''' Project an input data frame to UTM coordinates.
     
-    INPUT
-    inputDF [geopandas data frame]
-    
-    RETURNS
-    [geopandas data frame]    
+    :param inD: input geodataframe to explode
+    :type inD: gpd.GeoDataFrame
+    :return: exploded geodaatframe
+    :rtype: gpd.GeoDataFrame
     '''
     import utm
     
     #get UTM zones for upper right and lower left of input dataframe
     
     
     if inD.crs != {'init': 'epsg:4326'}:
```

## GOSTRocks/ntlMisc.py

```diff
@@ -1,24 +1,39 @@
-import sys, os, inspect, logging, json
-import rasterio, boto3
+import sys, os, inspect
+import rasterio
 
 import pandas as pd
-import geopandas as gpd
 import numpy as np
+import xarray as xr
+import matplotlib.pyplot as plt
+
+curPath = os.path.realpath(os.path.abspath(os.path.split(inspect.getfile( inspect.currentframe() ))[0]))
+if not curPath in sys.path:
+    sys.path.append(curPath)
+
+from dataMisc import aws_search_ntl
+from misc import tPrint
+import rasterMisc as rMisc
 
 def map_viirs(cur_file, out_file='', class_bins = [-10,0.5,1,2,3,5,10,15,20,30,40,50], text_x=0, text_y=5, dpi=100):
-    ''' create map of viirs data
-    
-    INPUT
-        cur_file [string] - path to input geotif
-        [optional] out_file [string] - path to create output image
-        [optional] class_bins [list numbers] - breaks for applying colour ramp
-        [optional] text_x [int] - position on map to position year text (left to right)
-        [optional] text_y [int] - position on map to position year text (top to bottom)
-    '''
+    """Map VIIRS nighttime lights imagery, optionally create output image
+
+    :param cur_file: path to input geotiff
+    :type cur_file: string
+    :param out_file: path to create output image, defaults to '' which does not create a file
+    :type out_file: str, optional
+    :param class_bins: breaks for applying colour ramp, defaults to [-10,0.5,1,2,3,5,10,15,20,30,40,50]
+    :type class_bins: list, optional
+    :param text_x: position on map to position year text (left to right), defaults to 0
+    :type text_x: int, optional
+    :param text_y: position on map to position year text (top to bottom), defaults to 5
+    :type text_y: int, optional
+    :param dpi: dotes per inch for output image, defaults to 100
+    :type dpi: int, optional
+    """
     # extract the year from the file name
     year = cur_file.split("_")[-1][:4]
     
     # Open the VIIRS data and reclassify 
     inR = rasterio.open(cur_file)
     inD = inR.read() 
     inC = xr.apply_ufunc(np.digitize,inD,class_bins)
@@ -38,44 +53,47 @@
         #plt.imsave(out_file, inC[0,:,:], cmap=plt.get_cmap('magma'))
         plt.imshow(inC[0,:,:], cmap=plt.get_cmap('magma'))
         fig.savefig(out_file, dpi=dpi, bbox_inches='tight', pad_inches=0)
     else:
         # https://matplotlib.org/stable/tutorials/colors/colormaps.html
         plt.imshow(inC[0,:,:], cmap=plt.get_cmap('magma'))
 
-def find_monthly_ntl(bucket='wbgdecinternal-ntl', prefix='NTL/VIIRS/Annual/VIIRS_ANNUAL_EOG'):
-    ''' Get list of NTL files in AWS
-    
-    INPUT
-    bucket [string, optional] - bucket to search for imagery
-    prefix [string, optional] - prefix storing images. Default is annual composites from EOG, choose "NTL/VIIRS" for monthly
     
+def run_zonal(inD, ntl_files=[], minval=0.1, verbose=False, calc_sd=True):
+    """ Run zonal statistics against a series of nighttime lights files
+
+    :param inD: input geopandas dataframe in which to summarize results
+    :type inD: gpd.GeoDataFrames
+    :param ntl_files: list of ntl files to summarize, defaults to [] which will search for all files in the s3 bucket using datMisc.aws_search_ntl()
+    :type ntl_files: list, optional
+    :param minval: Minimum value to summarize in nighttime lights, defaults to 0.1 which means all values below this become 0
+    :type minval: float, optional
+    :param verbose: print additional information, defaults to False
+    :type verbose: bool, optional
+    :param calc_sd: _description_, defaults to True
+    :type calc_sd: bool, optional
+    """
+    
+    ''' run zonal stats on all ntl files
+    INPUT 
+        inD [geopandas dataframe]
+        
     RETURNS
-    [pandas dataframe]
+        pandas dataframe
     '''
-
-    s3client = boto3.client('s3')
-    
-    # Loop through the S3 bucket and get all the keys for files that are .tif 
-    more_results = True
-    try:
-        del(token)
-    except:
-        pass
-    loops = 0
-    good_res = []
-    while more_results:
-        print(f"Completed loop: {loops}")
-        if loops > 0:
-            objects = s3client.list_objects_v2(Bucket=bucket, Prefix=prefix, ContinuationToken=token)
-        else:
-            objects = s3client.list_objects_v2(Bucket=bucket, Prefix=prefix)
-        more_results = objects['IsTruncated']
-        if more_results:
-            token = objects['NextContinuationToken']
-        loops += 1
-        for res in objects['Contents']:
-            if res['Key'].endswith('.tif'):
-                good_res.append(f"s3://{bucket}/{res['Key']}")
+    if len(ntl_files) == 0:
+        ntl_files = aws_search_ntl()
+        
+    for ntl_file in ntl_files:
+        name = ntl_file.split("/")[-1].split("_")[2][:8]
+        if verbose:
+            tPrint(name)
+        inR = rasterio.open(ntl_file)
+        ntl_res = rMisc.zonalStats(inD, inR, minVal=minval, calc_sd=calc_sd) 
+        out_cols = ['SUM','MIN','MAX','MEAN']
+        if calc_sd:
+            out_cols.append("SD")
+        ntl_df = pd.DataFrame(ntl_res, columns=out_cols)
+        inD[f'ntl_{name}_SUM'] = ntl_df['SUM']
+    return(inD)
     
-    return(good_res)
```

## GOSTRocks/osmMisc.py

```diff
@@ -1,26 +1,15 @@
-###############################################################################
-# Summarize OSM roads lengths
-# Charles Fox, July 2018
-# Purpose: summarize road lengths within features in defined shapefile
-###############################################################################
-
-import os, sys, time, subprocess, argparse, logging
-
-import GOSTnets as gn
-#from . import OSMNX_POIs
+import subprocess, argparse, logging
 
 import geopandas as gpd
 import osmnx as ox
 import pandas as pd
-import networkx as nx
 
 from shapely.geometry import box
-#import misc
-
+from GOSTRocks import misc
 
 # Highway features are reclassified to 4 OSMLR classes for simplification and standardization
 #   https://mapzen.com/blog/osmlr-2nd-technical-preview/
 OSMLR_Classes = {
 "motorway":"OSMLR level 1",
 "motorway_link":"OSMLR level 1",
 "trunk":"OSMLR level 1",
@@ -97,16 +86,15 @@
         ''' Read input osmpbf, extract all buildings and spit out to shapefile
         INPUT
         inPbf [string] - path to input pbf
         outFile [string] - path to output shapefile
         '''
         baseCommand = r"{osmCommand} --read-pbf {inPbf} --tf accept-ways building=*".format(
             osmCommand = self.osmosisCommand,
-            inPbf = inPbf, 
-            outPbf = outFile)
+            inPbf = inPbf)
         if len(bounds) > 0:
             baseCommand = "{baseCommand} --bounding-box top={top} left={left} bottom={bottom} right={right}".format(
                 baseCommand=baseCommand,
                 top    = bounds[3],
                 left   = bounds[0],
                 bottom = bounds[1],
                 right  = bounds[2])
@@ -169,16 +157,15 @@
                     highwayVals.append(key)
             except:
                 pass
         allCommands = ",".join(highwayVals)
         baseCommand = r"{osmCmd} --read-pbf {inPbf} --tf accept-ways highway={highwayCommand} --used-node".format(
             osmCmd = self.osmosisCommand, 
             inPbf=inPbf, 
-            highwayCommand=allCommands, 
-            outPbf=outOSM)
+            highwayCommand=allCommands)
         
         if len(bounds) > 0:
             baseCommand = "{baseCommand} --bounding-box top={top} left={left} bottom={bottom} right={right}".format(
                 baseCommand=baseCommand,
                 top    = bounds[3],
                 left   = bounds[0],
                 bottom = bounds[1],
@@ -191,77 +178,15 @@
             return(baseCommand)
         else:
             with open(self.tempFile, 'w') as outFile:
                 outFile.write(baseCommand)
             subprocess.call([self.tempFile], shell=True)
         
 
-#grid = gpd.read_file(r"Q:\AFRICA\COD\Projects\Shohei_Poverty_Kinshasa\ADMIN\PSUs\bati_ilot_quartier.shp")
-#outFolder = r"Q:\AFRICA\COD\Projects\Shohei_Poverty_Kinshasa\ADMIN"
-def downloadBaseData(grid, outFolder, amenities=True):
-    '''Download OSM based data using OSMNX - roads, schools, hospitals, and churches.
-    
-    INPUT
-    grid [geopandas dataFrame] - area to download in
-    outFolder [string] - place to write output
-    RETURNS
-    dictionary of [geopandas]
-    '''
-    toReturn = {}
-    roadsFile = os.path.join(outFolder, "OSM_Roads.shp")
-    if not os.path.exists(roadsFile):
-        bbox = box(grid.bounds.minx.min(), grid.bounds.miny.min(), grid.bounds.maxx.max(), grid.bounds.maxy.max())
-        #Download road network
-        G = ox.graph_from_polygon(bbox, network_type='drive_service')
-        roads = gn.edge_gdf_from_graph(G)
-        roads['highway'] = roads.highway.astype(str)
-        roads['OSMLR'] = roads.highway.map(OSMLR_Classes)
-        roads['oneway'] = roads.oneway.astype(int)   
-        '''
-        for badKeys in ['access', 'bridge','junction', 'lanes','oneway', 'osmid', 'ref', 'service','tunnel','width','stnode','endnode','name']:
-            try:
-                roads = roads.drop([badKeys],axis=1)
-            except:
-                print("Could not drop %s" % badKeys)
-        '''
-        try:        
-            roads.to_file(roadsFile)
-        except:
-            print("Could not write output")
-    else:
-        roads = pd.read_file
-    toReturn['Roads'] = roads
-        
-    if amenities:    
-        #Download Schools
-        schools = OSMNX_POIs.AmenityObject('Health', bbox, ['clinic','pharmacy','hospital','health'], "C:/Temp")
-        schools = schools.GenerateOSMPOIs()
-        schools = schools.RemoveDupes(0.005, roads.crs)
-        schools = schools.prepForMA()
-        schools.to_csv(os.path.join(outFolder, "OSM_Health.csv"), encoding='utf-8')
-        toReturn['Schools'] = schools
-        
-        #Download Hospitals
-        health = OSMNX_POIs.AmenityObject('Education', bbox, ['school','university','secondary school', 'kindergarten', 'college'], "C:/Temp")
-        health = health.GenerateOSMPOIs()
-        health = health.RemoveDupes(0.005, roads.crs)
-        health = health.prepForMA()
-        health.to_csv(os.path.join(outFolder, "OSM_Schools.csv"), encoding='utf-8')  
-        toReturn['Health'] = health
-        
-        #Download Churches
-        placeOfWorship = OSMNX_POIs.AmenityObject('Churches', bbox, ['place_of_worship'], "C:/Temp")
-        placeOfWorship = placeOfWorship.GenerateOSMPOIs()
-        placeOfWorship = placeOfWorship.RemoveDupes(0.005, roads.crs)
-        placeOfWorship = placeOfWorship.prepForMA()
-        placeOfWorship.to_csv(os.path.join(outFolder, "OSM_Churches.csv"), encoding='utf-8') 
-        toReturn['placeOfWorship'] = placeOfWorship
-        
-    return(toReturn)
-    
+   
 def summarizeOSM(grid, verbose=True, roadsOnly=False):
     ''' Summarizes OSM road length within each feature in the input grid
     
     ---variables---
     grid [GeoDataframe] - each feature will have the length of all roads summarized
 
     --- To Do ---
@@ -321,15 +246,16 @@
     INPUT
     inOSM [string] - path to OSM pbf to convert
     layer [string] - data layer to extract. Select from lines, points, multipolygons, multilinestrings
     
     RETURNS
     [geopandas data frame]
     '''
-    import ogr, geojson, json
+    import geojson, json
+    from osgeo import ogr
     from shapely.geometry import shape
     
     driver=ogr.GetDriverByName('OSM')
     data = driver.Open(inOSM)
     layer = data.GetLayer(layer)
     features=[x for x in layer]
     def loadOSMjson(x):
@@ -348,22 +274,21 @@
             pass
         x.pop("properties", None)
         x.pop("other_tags", None)
         return(x)
     
     allFeats = [loadOSMjson(feat.ExportToJson(as_object=True)) for feat in features]
     inR = pd.DataFrame(allFeats)
-    inR = gpd.GeoDataFrame(inR, geometry='geometry')
-    inR.crs = {'init': 'epsg:4326'}
+    inR = gpd.GeoDataFrame(inR, geometry='geometry', crs=4326)    
     try:
         inR = misc.project_UTM(inR)
     except:
-        inR = inR.to_crs({'init':'epsg:3857'})
+        inR = inR.to_crs(3857)
     inR['Length'] = inR['geometry'].apply(lambda x: x.length)
-    inR = inR.to_crs({'init':'epsg:4326'})
+    inR = inR.to_crs(4326)
     return (inR)
     
 if __name__ == "__main__":
     exampleText =  '''
     #Extract OSMLR level 1 and 2 roads from pbf
     python osmMisc.py -i Q:\AFRICA\MRT\INFRA\mauritania-latest_20190103.osm.pbf -o Q:\AFRICA\MRT\INFRA\mauritania-latest_20190103_OSMLR12.osm.pbf -OSMLR 1 2 -OSMExtract
```

## GOSTRocks/rasterMisc.py

```diff
@@ -1,68 +1,92 @@
-################################################################################
-# Miscellaneous Raster functions
-# Benjamin Stewart, September 2018
-# Purpose: Collect a number of useful raster functions in one place
-################################################################################
-
-import sys, os, inspect, logging, json
-import rasterio, affine, pyproj
+import sys, os, inspect, json
+import rasterio, pyproj
 
 import pandas as pd
 import geopandas as gpd
 import numpy as np
-import matplotlib.pyplot as plt
-import xarray as xr
-import rioxarray as rxr
-
-from matplotlib.colors import ListedColormap, BoundaryNorm
-from collections import Counter
-from shapely.geometry import box
+
+from shapely.geometry import box, shape
 from shapely import wkt
 from affine import Affine
 from rasterio import features
 from rasterio.mask import mask
 from rasterio.features import rasterize, MergeAlg
 from rasterio.warp import reproject, Resampling
-from rasterio import MemoryFile
+from rasterio.io import MemoryFile
 from contextlib import contextmanager
 
 import seaborn as sns
-import shapely
 sns.set(font_scale=1.5, style="whitegrid")
 
 curPath = os.path.realpath(os.path.abspath(os.path.split(inspect.getfile( inspect.currentframe() ))[0]))
 if not curPath in sys.path:
     sys.path.append(curPath)
 
 from misc import tPrint
 
 @contextmanager
 def create_rasterio_inmemory(src, curData):
     '''Create a rasterio object in memory from a numpy array 
     
-    :param dictionary src: - data dictionary describing the rasterio template i.e. - rasterio.open().profile
-    :param numpy array curData: - numpy array from which to create rasterio object
+    :param src: data dictionary describing the rasterio template i.e. - rasterio.open().profile
+    :type src: rasterio metadata dictionary 
+    :param curData: numpy array from which to create rasterio object
+    :type curData: numpy array
     '''
     with MemoryFile() as memFile:
         with memFile.open(**src) as dataset:
-            dataset.write(curData)
+            try:
+                dataset.write(curData)
+            except:
+                dataset.write_band(1, curData)
             del curData
         
         with memFile.open() as dataset:
-            yield(dataset)
+            yield dataset
+                
+def vectorize_raster(inR):# TODO out_file='', smooth=False, smooth_window=3, bad_vals=None):
+    ''' convert input raster data to a geodatframe
+    
+    :param inR: input raster data to vectorize
+    :type inR: rasterio.datasetReader 
+    '''
+    
+    data = inR.read()
+    ## TODO add smoothing option
+    #if smooth:
+    ## TODO add bad value filtering
+    idx = 0
+    all_vals = []
+    for cShape, value in features.shapes(data, transform=inR.transform):
+        all_vals.append([idx, value, shape(cShape)])
+        # shape(geojson.loads(json.dumps(cShape)))
+        idx += 1
+        
+    return(gpd.GeoDataFrame(all_vals, columns=['idx', 'value', 'geometry'], geometry='geometry', crs=inR.crs))
             
-def clipRaster(inR, inD, outFile, crop=True):
-    ''' Clip input raster
-    INPUT
-    [rasterio object] inR = rasterio.open(r"Q:/GLOBAL/POP&DEMO/GHS/BETA/FULL/MT/MT.vrt")
-    [geopandas object]inD = gpd.read_file(r"Q:\WORKINGPROJECTS\CityScan\Data\CityExtents\Conotou_AOI.shp")
-    [string]          outFile = r"Q:\WORKINGPROJECTS\CityScan\Data\CityExtents\Conotou_AOI\MappingData\GHSL.tif"
-    [Boolean] crop [default True] clip to exact extent of shape (True) or to bounding box (False)
 
+""" TODO
+def project_raster(inR, crs):
+    ''' 
+    '''
+"""            
+def clipRaster(inR, inD, outFile='', crop=True):
+    ''' Clip input raster
+    
+    :param inR: rasterio object to clip
+    :type inR: rasterio.DatasetReader
+    :param inD: geopandas polygonal dataframe to use for clip clip extent based on crop param
+    :type inD: geopandas.GeoDataFrame
+    :param outFile: string path to write output raster, default is '' which writes nothing
+    :type outFile: string
+    :param crop: determine wether to clip based on bounding box (False) or unary_union (True). Default is True
+    :type crop: Boolean
+    :return: array of [numpy array of data, and rasterio metadata]
+    :rtype: array
     '''
     if inD.crs != inR.crs:
         inD = inD.to_crs(inR.crs)
         inD = inD.buffer(0)
     out_meta = inR.meta.copy()
     def getFeatures(gdf):
         #Function to parse features from GeoDataFrame in such a manner that rasterio wants them
@@ -74,37 +98,43 @@
     
     coords = getFeatures(tD)
     out_img, out_transform = mask(inR, shapes=coords, crop=True)
     out_meta.update({"driver": "GTiff",
                      "height": out_img.shape[1],
                      "width": out_img.shape[2],
                      "transform": out_transform})
-    with rasterio.open(outFile, "w", **out_meta) as dest:
-        dest.write(out_img)
-
-def rasterizeDataFrame(inD, outFile, idField='', templateRaster='', templateMeta = '', nCells=0, res=0, mergeAlg="REPLACE", re_proj=False):
-    ''' Convert input geopandas dataframe into a raster file
-        inD = gpd.read_file(r"C:\Temp\TFRecord\Data\Training Data\test3_training.shp")
-        templateRaster=r"C:\Temp\TFRecord\Data\Training Data\test3.tif"
-        idField = 'ID2'
-        outFile = templateRaster.replace(".tif", "_labels.tif")
-
-    INPUT VARIABLES
-        inD [geopandas DataFrame]
-        outFile [string] - path for creating output file
-    OPTIONAL
-        idField [string] - field to rasterize, sets everything to 1 otherwise
-        templateRaster [string] - raster upon which to base raster creation
-        templateMeta [dictionary] - raster metadata used to create output raster
-        nCells [number] - number of cells in width and height
-        res [number] - resolution of output raster in units of the crs
-        re_proj [Boolean] - option to reproject inD to templateRaster if CRS do not match
-    RETURNS
-        [dict of [dict] and [numpy array]] - metadata used to create output raster and burned raster values
-    '''
+    if outFile != '':
+        with rasterio.open(outFile, "w", **out_meta) as dest:
+            dest.write(out_img)
+    return([out_img, out_meta])
+
+def rasterizeDataFrame(inD, outFile='', idField='', templateRaster='', templateMeta = '', nCells=0, res=0, mergeAlg="REPLACE", re_proj=False):
+    """ Convert input geopandas dataframe into a raster file
+
+    :param inD: input data frame to rasterize
+    :type inD: gpd.GeoDataFrame
+    :param outFile: output file to create from rasterized dataframe, defaults to '' which creates no file
+    :type outFile: string
+    :param idField: field in inD to rasterize, defaults to '' which sets everything to 1
+    :type idField: str, optional
+    :param templateRaster: raster upon which to base raster creation, defaults to ''. If no template is provided, nCells or res need to be defined
+    :type templateRaster: str, optional
+    :param templateMeta: raster metadata used to create output raster, defaults to ''. If no template is provided, nCells or res need to be defined
+    :type templateMeta: str, optional
+    :param nCells: number of cells in width and height, defaults to 0
+    :type nCells: int, optional
+    :param res: resolution of output raster in units of the crs, defaults to 0
+    :type res: int, optional
+    :param mergeAlg: Method of aggregating overlapping features, defaults to "REPLACE"; options are "REPLACE" or "ADD"
+    :type mergeAlg: str, optional
+    :param re_proj: option to reproject inD to templateRaster if CRS do not match, defaults to False
+    :type re_proj: bool, optional
+    :return:  dict of metadata used to create output raster and burned raster values
+    :rtype: dict of {'meta':new raster metadata, 'vals': values in new raster}
+    """
     ###Parameter checking
     if nCells <=0 and res <=0 and templateRaster == '' and templateMeta =='':
         raise(ValueError("Must define one of nCells or res"))
     if nCells > 0 and res > 0 and templateRaster == ''  and templateMeta =='':
         raise(ValueError("Cannot define both nCells and res"))
 
     #Set VALUE field equal to idField
@@ -119,15 +149,15 @@
     elif mergeAlg == "ADD":
         mAlg = MergeAlg.add
     else:
         raise(ValueError("MergeAlg must be one of REPLACE or ADD"))
         
     if templateRaster != '':
         inR = rasterio.open(templateRaster)
-        cMeta = inR.meta.copy()
+        cMeta = inR.profile.copy()
         cMeta.update(count=1)
         nTransform = cMeta['transform']
         if inD.crs != inR.crs:
             if not re_proj:
                 raise(ValueError("input CRS do not match: inD - %s, templateRaster - %s" % (inD.crs, inR.crs)))
             inD = inD.to_crs(inR.crs)
     elif templateMeta != '':
@@ -136,57 +166,50 @@
         if inD.crs != cMeta['crs']:
             if not re_proj:
                 raise(ValueError("input CRS do not match: inD - %s, templateRaster - %s" % (inD.crs, inR.crs)))
             inD = inD.to_crs(cMeta['crs'])
     else:
         bounds = inD.total_bounds
         if nCells > 0:
-            cellWidth  = (bounds[2] - bounds[0]) / nCells
-            cellHeight = ((bounds[3] - bounds[1]) / nCells) * -1
             height = nCells
             width = nCells
         if res > 0:
-            cellWidth = res
-            cellHeight = res
             height = int(round((bounds[3] - bounds[1]) / res))
             width =  int(round((bounds[2] - bounds[0]) / res))
 
         b = inD.total_bounds
         nTransform = rasterio.transform.from_bounds(b[0], b[1], b[2], b[3], width, height)
         if inD.crs.__class__ == pyproj.crs.crs.CRS:
             crs = {'init':'epsg:%s' % inD.crs.to_epsg()}
         else:
             crs = inD.crs
-        print(crs)
         cMeta = {'count':1, 'crs': crs, 'dtype':inD['VALUE'].dtype, 'driver':'GTiff',
                  'transform':nTransform, 'height':height, 'width':width}
     shapes = ((row.geometry,row.VALUE) for idx, row in inD.iterrows())
     burned = features.rasterize(shapes=shapes, out_shape=(cMeta['height'], cMeta['width']), transform=nTransform, dtype=cMeta['dtype'], merge_alg=mAlg)
     try:
         with rasterio.open(outFile, 'w', **cMeta) as out:
             out.write_band(1, burned)
         return({'meta':cMeta, 'vals': burned})
     except:
         print("Error writing raster")
         return({'meta':cMeta, 'vals': burned})
 
-def polygonizeArray(data, b, curRaster):
-    '''
-    Convert input array to a geodataframe defined by the boundary as the b object
-    INPUT
-    array [numpy array]
-    curRaster [rasterio object] - template raster object
-    RETURNS
-    geopandas dataframe
-    DEBUGGING
-    window = ((float(lr[0]), float(ul[0])), (float(ul[1]), float(lr[1])+1))
-    data = curRaster.read(bandNum, window=window, masked = True)
-    outArray.to_csv("C:/temp/FUBAR.csv")
-    '''
+def polygonizeArray(data, curRaster):
+    """ Convert input array (data) to a geodataframe
+
+    :param data: numpy array of raster data. ie - rasterio.open().read()
+    :type data: np.array
+    :param curRaster: template raster object
+    :type curRaster: rasterio.DatasetReader
+    :return: geodataframe with columns row, col, val, geometry
+    :rtype: gpd.GeoDataFrame
+    """
     #Calculate resolution of cells
+    b = curRaster.bounds
     ll = curRaster.xy(*curRaster.index(*b[0:2]),"ll")
     xmin = ll[0]
     ymin = ll[1]
     xRes = curRaster.res[0]
     yRes = curRaster.res[1]
     crs = curRaster.crs
     #create a dataframe equal to the size of the array
@@ -194,17 +217,19 @@
     outArray['id'] = list(range(0, (data.shape[0] * data.shape[1])))
     rowVals = []
     colVals = []
     actualvals = []
     for row in range(0,data.shape[0]):
         for col in range(0,data.shape[1]):
             rowVals.append(row)
-            colVals.append(col)            
+            colVals.append(col)
+            actualvals.append(data[row,col])            
     outArray['row'] = rowVals
     outArray['col'] = colVals
+    outArray['vals'] = actualvals
     #Create a polygon covering each cell
     def getPolygon(x):
         llX = xmin + (xRes * x['col'])
         llY = ymin + (yRes * x['row'])
         A = "%s %s" % (llX, llY)
         B = "%s %s" % (llX, llY + yRes)
         C = "%s %s" % (llX + xRes, llY + yRes)
@@ -212,35 +237,50 @@
         return(wkt.loads("POLYGON((%s,%s,%s,%s,%s))" % (A,B,C,D,A)))
     outArray['geometry'] = outArray.apply(getPolygon, axis=1)
     outGeo = gpd.GeoDataFrame(outArray, geometry="geometry")
     outGeo.crs = crs
     return(outGeo)
     
 def zonalStats(inShp, inRaster, bandNum=1, mask_A = None, reProj = False, minVal = '', maxVal = '',
-                verbose=False , rastType='N', unqVals=[], weighted=False, allTouched=False):
-    ''' Run zonal statistics against an input shapefile. Returns array of SUM, MIN, MAX, and MEAN
+                verbose=False , rastType='N', unqVals=[], weighted=False, allTouched=False, calc_sd=False, return_df=False):
+    """ Run zonal statistics against an input shapefile. Returns array of SUM, MIN, MAX, and MEAN
 
-    INPUT VARIABLES
-    inShp [string or geopandas object] - path to input shapefile
-    inRaster [string or rasterio object] - path to input raster
-
-    OPTIONAL
-    bandNum [integer] - band in raster to analyze
-    reProj [boolean] -  whether to reproject data to match, if not, raise an error
-    minVal/maxVal [number] - if defined, will only calculate statistics on values above or below this number
-    verbose [boolean] - whether to be loud with technical updates
-    rastType [string N or C] - N is numeric and C is categorical. Categorical returns counts of numbers
-    unqVals [array of numbers] - used in categorical zonal statistics, tabulates all these numbers, will report 0 counts
-    mask_A [numpy boolean mask] - mask the desired band using an identical shape boolean mask. Useful for doing conditional zonal stats
-    weighted [boolean] - apply weighted zonal calculations. This will determine the % overlap for each
-        cell in the defined AOI. Will apply weights in calculations of numerical statistics
-    
-    RETURNS
-    array of arrays, one for each feature in inShp
-    '''
+    :param inShp: input geospatial data to summarize raster
+    :type inShp: string path to file of gpd.GeoDataFrame
+    :param inRaster: input raster to summarize
+    :type inRaster: string path to file or rasterio.DatasetReader
+    :param bandNum: band in raster to analyze, defaults to 1
+    :type bandNum: int, optional
+    :param mask_A: mask the raster data using an identical shaped boolean mask, defaults to None
+    :type mask_A: np.array, optional
+    :param reProj: whether to reproject data to match, if not, raise a ValueError if CRS mismatch between inShp and inRaster, defaults to False
+    :type reProj: bool, optional
+    :param minVal: if defined, will only calculate statistics on values above this number, defaults to ''
+    :type minVal: number, optional
+    :param maxVal: if defined, will only calculate statistics on values below this number, defaults to ''
+    :type maxVal: number, optional
+    :param verbose: provide additional text updates, defaults to False
+    :type verbose: bool, optional
+    :param rastType: Type of raster, defaults to 'N' as numerical or 'C' as categorical. If 'C' is used, you should provide unqVals
+    :type rastType: str, optional
+    :param unqVals: List of unique values to search for in raster, defaults to []
+    :type unqVals: list of int, optional
+    :param weighted: apply weighted zonal calculations. This will determine the % overlap for each
+        raster cell in the defined AOI. Will apply weights in calculations of numerical statistics, defaults to False
+    :type weighted: bool, optional
+    :param allTouched: whether to include all cells touched in raster calculation, passed to rasterio rasterize function, defaults to False
+    :type allTouched: bool, optional
+    :param calc_sd: include the standard deviation in calculation, defaults to False
+    :type calc_sd: bool, optional
+    :param return_df: if true, return result as data frame; defaults to False
+    :type return_df: boolean, optional
+    :raises ValueError: If CRS mismatch between inShp and inRaster
+    :return: array of zonal results - one entry for every feature in inShp. Each entry is SUM, MIN, MAX, MEAN, SD (optional)
+    :rtype: array
+    """
     if isinstance(inShp, str):
         inVector = gpd.read_file(inShp)
     else:
         inVector = inShp
     if isinstance(inRaster, str):
         curRaster = rasterio.open(inRaster, 'r')
     else:
@@ -292,15 +332,23 @@
                     rGrid['newArea'] = rGrid.intersection(geometry).area
                     #Store the percent overlap 
                     rGrid['w'] = rGrid['newArea']/rGrid['gArea']
                     newData = data
                     for idx, row in rGrid.iterrows():
                         newData[row['row'], row['col']] = data[row['row'], row['col']] * row['w']
                     data = newData
-                    
+                
+                '''
+                # Mask out no-data in data array
+                if 'nodata' in curRaster.profile.keys():
+                    no_data_val = curRaster.profile['nodata']
+                    #data[data == no_data_val] = np.nan
+                    data[data == no_data_val] = 0
+                '''
+                
                 # create an affine transform for the subset data
                 t = curRaster.transform
                 shifted_affine = Affine(t.a, t.b, t.c+ul[1]*t.a, t.d, t.e, t.f+lr[0]*t.e)
 
                 # rasterize the geometry
                 mask = rasterize(
                     [(geometry, 0)],
@@ -322,42 +370,56 @@
                             results = [np.nansum(masked_data), np.nanmin(masked_data), 
                                        np.nanmax(masked_data), np.nanmean(masked_data)]
                         else :
                             results = [-1, -1, -1, -1]
                     else:
                         results = [np.nansum(masked_data), np.nanmin(masked_data), 
                                    np.nanmax(masked_data), np.nanmean(masked_data)]
+                    if calc_sd:
+                        try:
+                            results.append(np.std(masked_data))
+                        except:
+                            results.append(-1)
                 if rastType == 'C':
-                    if len(unqVals) > 0:
-                        xx = dict(Counter(data.flatten()))
+                    if len(unqVals) > 0:             
+                        masked_unq = np.unique(masked_data, return_counts=True)
+                        xx = dict(list(zip(masked_unq[0], masked_unq[1]))[:-1])
                         results = [xx.get(i, 0) for i in unqVals]
                     else:
                         results = np.unique(masked_data, return_counts=True)
                 outputData.append(results)
             except Exception as e:
                 if verbose:
-                    print(e)
+                    print(e)                    
                 if rastType == 'N':
                     outputData.append([-1, -1, -1, -1])
                 else:
                     outputData.append([-1 for x in unqVals])
         except:
             print("Error processing %s" % fCount)
-    return outputData
+    if return_df:
+        cols = ["SUM","MIN","MAX","MEAN"]
+        if calc_sd:
+            cols.append("SD")
+        outputData = pd.DataFrame(outputData, columns=cols)
+    return(outputData)
 
 def standardizeInputRasters(inR1, inR2, inR1_outFile='', resampling_type="nearest"):
     ''' Standardize inR1 to inR2: changes crs, extent, and resolution.
 
-    Inputs:
-    inR1, inR2 [rasterio raster object]
-    [optional] inR1_outFile [string] - output file for creating inR1 standardized to inR2
-    [optional] data_type [string ['C','N']]
-    
-    Returns:
-    [list] - [numpy array, raster metadata]
+    :param inR1: rasterio object for raster to be modified
+    :type inR1: ratserio.DatasetReader
+    :param inR2: rasterio object to be standardized to
+    :type inR12 ratserio.DatasetReader
+    :param inR1_outfile: path to create output raster file of standardized inR1, default is '', which means nothing is written
+    :type inR1: string
+    :param resampling_type: how to perfrom spatial resampling; options are nearest (default), cubic, or sum
+    :type resampling_type: string
+    :return: array of numpy array, and rasterio metadata
+    :rtype: array
     '''
     if inR1.crs != inR2.crs:
         bounds = gpd.GeoDataFrame(pd.DataFrame([[1, box(*inR2.bounds)]], columns=["ID","geometry"]), geometry='geometry', crs=inR2.crs)
         bounds = bounds.to_crs(inR1.crs)
         b2 = bounds.total_bounds
         boxJSON = [{'type': 'Polygon', 'coordinates': [[[b2[0], b2[1]],[b2[0], b2[3]],[b2[2], b2[3]],[b2[2], b2[1]],[b2[0], b2[1]]]]}]
     else:
@@ -385,24 +447,24 @@
                      "crs": inR2.crs})
     if inR1_outFile != "":
         with rasterio.open(inR1_outFile, "w", **out_meta) as dest:
             dest.write(newArr.astype(out_meta['dtype']))
     return([newArr.astype(out_meta['dtype']), out_meta])
 
 def jaccardIndex(inR1, inR2):
-    '''Calculate the jaccard index on two binary input raster objects
-
-    Reference: https://en.wikipedia.org/wiki/Jaccard_index
+    """ Calculate the jaccard index on two binary input raster objects; Reference: https://en.wikipedia.org/wiki/Jaccard_index
 
-    Inputs:
-    inR1/inR2[rasterio raster object] - these need to be the same size
-
-    Returns:
-    index [ float ]
-    '''
+    :param inR1: binary rasterio raster object to compare; needs to be same shape as inR2
+    :type inR1: rasterio.DatasetReader
+    :param inR2: binary rasterio raster object to compare; needs to be same shape as inR1
+    :type inR2: rasterio.DatasetReader
+    :raises ValueError: if inR1 and inR2 are different shapes
+    :return: index comparing similarity of input raster datasets
+    :rtype: float
+    """
     if inR1.shape != inR2.shape:
         print(inR1.shape)
         print(inR2.shape)
         raise ValueError("Shape of input rasters do not match")
     #Add the two rasters together and get the unique tabulation
     inC = inR1.read() + inR2.read()
     xx = np.unique(inC, return_counts=True)
@@ -414,116 +476,8 @@
     #   1 - Only one area defines it as urban
     #   2 - Both areas define cell as urban
     # Jaccard is ratio of 2 / 1+2
     try:
         jIdx = outDict[2] / float(outDict[2] + outDict[1])
         return jIdx
     except:
-        return -1
-
-def groupJaccard(oFile, sFiles):
-    with open(oFile, 'w') as output:
-        for bFile in sFiles:
-            inR2 = rasterio.open(bFile)
-            for cFile in sFiles:
-                if bFile != cFile:
-                    logging.info("Processing %s and %s" % (os.path.basename(bFile), os.path.basename(cFile)))
-                    inR1 = rasterio.open(cFile)
-                    curIndex = jaccardIndex(inR2, inR1)
-                    output.write("%s,%s,%s\n" % (os.path.basename(bFile), os.path.basename(cFile), curIndex))
-
-class zonalResult(object):
-    def __init__(self, inputPath, fileType, fieldToCopy='ALL', fieldAction= 'REPLACE', fieldNames=''):
-        '''
-        INPUT
-            inputPath [string] - path to the input zonal stats results
-            fileTpe [string] - 'C' or 'N', for use in processing fields
-            [optional] fieldToCopy [string] - field name type to extract from numerical fields, can be a regex expression
-            [optional] fieldAction [string] - 'REPLACE' or 'JOIN'. REPLACE will replace output names with the variable
-                fieldNames. JOIN will join fieldNames to each of the existing zonal results fields
-            [optional] field_names [string] - either a list of field names to give to output, or prefix to join to each field               
-        '''
-        self.inputPath = inputPath
-        self.inValues = pd.read_csv(inputPath)
-        self.fileType = fileType
-        #Extract specific fields
-        self.inValues = self.inValues.drop(self.inValues.filter(regex="Unnamed").columns, axis=1)
-        if fieldToCopy != 'ALL':
-            #Search columns for defined field
-            self.inValues = self.inValues.filter(regex="|".join(fieldToCopy))
-        if fieldNames != '':
-            if fieldAction == 'REPLACE':
-                self.inValues.columns = fieldNames
-            if fieldAction == 'JOIN':
-                self.inValues.columns = ["%s_%s" % (fieldNames, c) for c in self.inValues.columns]
-    def __str__(self):
-        return("%s: %s" % (os.path.basename(self.inputPath), "|".join(self.inValues.columns)))
-
-def runAllJaccard():
-    inAI_file = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\AI\d150t60pop50l.tif"
-    inHD_file = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\Clusters\hd_clusters.tif"
-    inURB_file = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\Clusters\urban_clusters.tif"
-    inNTL1_file = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\NTLs\NTL_Extents_80.tif"
-    inNTL2_file = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\NTLs\NTL_Extents_25.tif"
-    inDuranton10 = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\Duranton\Duranton_10_binary.tif"
-    inDuranton7 = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\Duranton\Duranton_7_binary.tif"
-    allFiles = [inHD_file, inURB_file, inAI_file, inDuranton10, inDuranton7, inNTL2_file, inNTL1_file]
-
-    outputFile = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\Jaccard_Comparison.csv"
-    baliShp = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\Java_and_Bali.shp"
-    baliGeom = gpd.read_file(baliShp)
-    notBaliShp = r"Q:\WORKINGPROJECTS\Indonesia_Urbanization\UrbanComparison\ForBen\Not_Bali_norJAVA.shp"
-    notBaliGeom = gpd.read_file(notBaliShp)
-
-    #Standardize all input layers to the same baseline - inNTL1_file
-    inR1 = rasterio.open(inNTL1_file)
-    standardFiles = []
-
-    logging.info("Standardizing input files")
-    for inFile in allFiles:
-        inR2 = rasterio.open(inFile)
-        cFileOut = inFile.replace(".tif", "_standard.tif")
-        standardFiles.append(cFileOut)
-        if not os.path.exists(cFileOut):
-            standardizeInputRasters(inR2, inR1, cFileOut)
-
-    # Clip standard rasters to BALI, and then eliminate BALI
-    baliFiles = []
-    notBaliFiles = []
-    for inFile in standardFiles:
-        baliFile = inFile.replace(".tif", "_Bali.tif")
-        baliFiles.append(baliFile)
-        notBaliFile = inFile.replace(".tif", "_NotBali.tif")
-        notBaliFiles.append(notBaliFile)
-        logging.info(baliFile)
-        if not os.path.exists(baliFile):
-            curR = rasterio.open(inFile)
-            if baliGeom.crs != curR.crs:
-                baliGeom = baliGeom.to_crs(curR.crs)
-            #Generate mask for Bali and Java
-            baliGeoms = ((g, 1) for g in baliGeom['geometry'])
-            baliMask = features.rasterize(baliGeoms, out_shape=curR.shape, transform=curR.transform)
-            #Identify only Bali and Java
-            baliImage = baliMask * curR.read()
-            #Identify everythin else
-            notBaliMask = np.abs(baliMask.astype("int8") - 1).astype("uint8")
-            notBaliImage = notBaliMask * curR.read()
-            #Write Bali Results
-            with rasterio.open(baliFile, 'w', **curR.meta) as dst:
-                dst.write(baliImage)
-            #Write not Bali Results
-            with rasterio.open(notBaliFile, 'w', **curR.meta) as dst:
-                dst.write(notBaliImage)
-    groupJaccard(outputFile, standardFiles)
-    groupJaccard(outputFile.replace(".csv", "_Bali.csv"), baliFiles)
-    groupJaccard(outputFile.replace(".csv", "_NotBali.csv"), notBaliFiles)
-
-if __name__ == "__main__":
-    exampleText = '''
-    python rasterMisc.py -gdalbuildvrt -outFile Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID-FD-5.vrt -file_list Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-1.tif Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-2.tif Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-3.tif Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-4.tif Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-5.tif Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-6.tif Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-7.tif Q:\GLOBAL\HYDRO\SSBN_Flooding\indonesia\ID_fluvial_defended\ID-FD-5-8.tif
-    '''
-    parser.add_argument("-gdalbuildvrt", dest="BUILDVRT", action="store_true", help="Build a VRT from input rasters")
-    parser.add_argument("-file_list", dest="GDALFILES", nargs='+', action="store_true", help="List of files to build VRT from")
-    parser.add_argument("-outFile", dest="VRTOUT", nargs='+', action="store_true", help="output vrt file")
-
-    args = parser.parse_args()
-    logging.basicConfig(level=logging.INFO)
+        return -1
```

## Comparing `GOSTRocks-0.0.3.dist-info/LICENSE` & `GOSTRocks-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `GOSTRocks-0.0.3.dist-info/METADATA` & `GOSTRocks-0.1.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 Metadata-Version: 2.1
 Name: GOSTRocks
-Version: 0.0.3
+Version: 0.1.0
 Summary: Miscellaneous geospatial functions concerning vector, raster, and network analysis
 Home-page: https://github.com/bpstewar/gostrocks
 Author: Benjamin P. Stewart
-License: MIT
-Platform: UNKNOWN
+Author-email: "Benjamin P. Stewart" <ben.gis.stewart@gmail.com>
+Project-URL: Homepage, https://github.com/bpstewar/gostrocks
+Project-URL: Bug Tracker, https://github.com/bpstewar/gostrocks/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rasterio
 Requires-Dist: geopandas
 Requires-Dist: pandas
+Requires-Dist: numexpr (>2.6.8)
 Requires-Dist: numpy
-Requires-Dist: osmnx
-Requires-Dist: GOSTNets
-Requires-Dist: scikit-image
 Requires-Dist: pyproj
 Requires-Dist: ogr
-Requires-Dist: rtree
-Requires-Dist: networkx
-Requires-Dist: xarray
-Requires-Dist: rioxarray
 Requires-Dist: seaborn
+Requires-Dist: boto3
+Requires-Dist: botocore
+Requires-Dist: contextily
+Requires-Dist: matplotlib
+Requires-Dist: tqdm
+Requires-Dist: xarray
+Requires-Dist: osmnx
+Requires-Dist: affine
+Requires-Dist: PyOpenSSL (>=23.2)
 
 # GOSTRocks
 Geospatial tools from the World Bank GOST team (mostly Ben).
 
 # Installation
 ```
 $ pip install GOSTRocks
 ```
 
 Future releases and information can be built from the setup.py here, but pip will contain the most recent stable version
 
 # Examples
 ...see the notebooks in the github repo
-
-
```

