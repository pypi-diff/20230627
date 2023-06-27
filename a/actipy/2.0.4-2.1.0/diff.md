# Comparing `tmp/actipy-2.0.4.tar.gz` & `tmp/actipy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actipy-2.0.4.tar", last modified: Wed Jun  7 13:58:04 2023, max compression
+gzip compressed data, was "actipy-2.1.0.tar", last modified: Tue Jun 27 17:25:16 2023, max compression
```

## Comparing `actipy-2.0.4.tar` & `actipy-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.769765 actipy-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-07 13:57:51.000000 actipy-2.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 13:57:51.000000 actipy-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-07 13:58:04.769765 actipy-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-07 13:57:51.000000 actipy-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-07 13:57:51.000000 actipy-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:58:04.769765 actipy-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-07 13:57:51.000000 actipy-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.765765 actipy-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.769765 actipy-2.0.4/src/actipy/
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/ActigraphReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/ActigraphReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/AxivityReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/AxivityReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/GENEActivReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/GENEActivReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/NpyWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/NpyWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 13:58:04.769765 actipy-2.0.4/src/actipy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.769765 actipy-2.0.4/src/actipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-07 13:57:51.000000 actipy-2.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.191441 actipy-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-27 17:25:01.000000 actipy-2.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 17:25:01.000000 actipy-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-27 17:25:16.191441 actipy-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-27 17:25:01.000000 actipy-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-27 17:25:01.000000 actipy-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:25:16.191441 actipy-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-27 17:25:01.000000 actipy-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.183441 actipy-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.191441 actipy-2.1.0/src/actipy/
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 17:25:16.191441 actipy-2.1.0/src/actipy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.191441 actipy-2.1.0/src/actipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-27 17:25:01.000000 actipy-2.1.0/versioneer.py
```

### Comparing `actipy-2.0.4/LICENSE.md` & `actipy-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/PKG-INFO` & `actipy-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.0.4
+Version: 2.1.0
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-2.0.4/README.md` & `actipy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/pyproject.toml` & `actipy-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/setup.py` & `actipy-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             "flake8",
             "autopep8",
             "ipython",
             "ipdb",
             "memory-profiler",
             "twine",
             "tomli",
+            "pytest",
         ],
         "docs": [
             "sphinx>=4.2",
             "sphinx_rtd_theme>=1.0",
             "readthedocs-sphinx-search>=0.1",
             "docutils<0.18",
         ]
```

### Comparing `actipy-2.0.4/src/actipy/ActigraphReader.class` & `actipy-2.1.0/src/actipy/ActigraphReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/src/actipy/ActigraphReader.java` & `actipy-2.1.0/src/actipy/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/src/actipy/AxivityReader.class` & `actipy-2.1.0/src/actipy/AxivityReader.class`

 * *Files 11% similar despite different names*

#### procyon -ec {}

```diff
@@ -79,20 +79,21 @@
         byteBuffer.order(ByteOrder.LITTLE_ENDIAN);
         final String string = (char)byteBuffer.get() + "" + (char)byteBuffer.get() + "";
         try {
             if (string.equals("MD")) {
                 return;
             }
             if (string.equals("AX")) {
-                final int n = (int)getUnsignedInt(byteBuffer, 14);
-                final float n2 = (float)((getUnsignedShort(byteBuffer, 20) * 150.0 - 20500.0) / 1000.0);
+                final int intExact = Math.toIntExact(getUnsignedInt(byteBuffer, 14));
+                final float n = (float)Math.pow(10.0, (double)(getUnsignedShort(byteBuffer, 18) & 0x3FF) / 341.0);
+                final float n2 = (float)(((getUnsignedShort(byteBuffer, 20) & 0x3FF) * 150.0 - 20500.0) / 1000.0);
                 final short n3 = (short)(byteBuffer.get(24) & 0xFF);
                 final short n4 = (short)(byteBuffer.get(25) & 0xFF);
                 int unsignedShort = getUnsignedShort(byteBuffer, 28);
-                final long cwaTimestamp = this.getCwaTimestamp(n);
+                final long cwaTimestamp = this.getCwaTimestamp(intExact);
                 short n5 = 0;
                 float sampleRate;
                 float n6;
                 if (n3 == 0) {
                     sampleRate = byteBuffer.getShort(26);
                     n6 = 0.0f;
                 }
@@ -126,15 +127,15 @@
                     n7 = 4;
                 }
                 final int n9 = 480 / n7;
                 if (unsignedShort > n9) {
                     unsignedShort = n9;
                 }
                 if (this.sessionStart == null) {
-                    this.sessionStart = this.getCwaLocalDateTime(n);
+                    this.sessionStart = this.getCwaLocalDateTime(intExact);
                 }
                 for (int j = 0; j < unsignedShort; ++j) {
                     float n10;
                     float n11;
                     float n12;
                     if (n7 == 4) {
                         final long unsignedInt = getUnsignedInt(byteBuffer, 30 + 4 * j);
@@ -148,15 +149,15 @@
                         n12 = byteBuffer.getShort(30 + 2 * n8 * j + 4);
                     }
                     else {
                         n10 = 0.0f;
                         n11 = 0.0f;
                         n12 = 0.0f;
                     }
-                    this.writer.write((Map)toItems((long)((lastBlockTime + j * (lastBlockTime2 - lastBlockTime) / unsignedShort) * 1000.0), n10 / 256.0f, n11 / 256.0f, n12 / 256.0f, n2));
+                    this.writer.write((Map)toItems((long)((lastBlockTime + j * (lastBlockTime2 - lastBlockTime) / unsignedShort) * 1000.0), n10 / 256.0f, n11 / 256.0f, n12 / 256.0f, n2, n));
                 }
             }
         }
         catch (final Exception ex) {
             ++this.errCounter;
             ex.printStackTrace();
         }
@@ -195,31 +196,33 @@
             this.writer.close();
         }
         catch (final Exception ex) {
             ex.printStackTrace();
         }
     }
     
-    private static Map<String, Object> toItems(final long l, final float f, final float f2, final float f3, final float f4) {
+    private static Map<String, Object> toItems(final long l, final float f, final float f2, final float f3, final float f4, final float f5) {
         final HashMap hashMap = new HashMap();
         hashMap.put("time", Long.valueOf(l));
         hashMap.put("x", Float.valueOf(f));
         hashMap.put("y", Float.valueOf(f2));
         hashMap.put("z", Float.valueOf(f3));
         hashMap.put("temperature", Float.valueOf(f4));
+        hashMap.put("light", Float.valueOf(f5));
         return hashMap;
     }
     
-    private static Map<String, Object> toItems(final long n, final double n2, final double n3, final double n4, final double n5) {
-        return toItems(n, (float)n2, (float)n3, (float)n4, (float)n5);
+    private static Map<String, Object> toItems(final long n, final double n2, final double n3, final double n4, final double n5, final float n6) {
+        return toItems(n, (float)n2, (float)n3, (float)n4, (float)n5, n6);
     }
     
     static {
         final LinkedHashMap m = new LinkedHashMap();
         m.put("time", "Long");
         m.put("x", "Float");
         m.put("y", "Float");
         m.put("z", "Float");
         m.put("temperature", "Float");
+        m.put("light", "Float");
         ITEM_NAMES_AND_TYPES = Collections.unmodifiableMap((Map<?, ?>)m);
     }
 }
```

### Comparing `actipy-2.0.4/src/actipy/AxivityReader.java` & `actipy-2.1.0/src/actipy/AxivityReader.java`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     static{
         Map<String, String> itemNamesAndTypes = new LinkedHashMap<String, String>();
         itemNamesAndTypes.put("time", "Long");
         itemNamesAndTypes.put("x", "Float");
         itemNamesAndTypes.put("y", "Float");
         itemNamesAndTypes.put("z", "Float");
         itemNamesAndTypes.put("temperature", "Float");
-        // itemNamesAndTypes.put("lux", "Integer");  // unused for now
+        itemNamesAndTypes.put("light", "Float");
         ITEM_NAMES_AND_TYPES = Collections.unmodifiableMap(itemNamesAndTypes);
     }
 
     private String accFile;
     private String outFile;
     private boolean verbose;
 
@@ -124,17 +124,17 @@
                  * java.time.DateTimeException: Invalid value for MonthOfYear (valid values 1 - 12): 0
                  */
                 // sessionStart = getCwaHeaderLoggingStartTime(block);
 
                 return;
 
             } else if (header.equals("AX")) {
-                int blockTimeInfo = (int) getUnsignedInt(block, 14);
-                // int light = getUnsignedShort(block, 18); // unused for now
-                float temperature = (float) ((getUnsignedShort(block, 20) * 150.0 - 20500) / 1000);
+                int blockTimeInfo = Math.toIntExact(getUnsignedInt(block, 14));
+                float light = (float) Math.pow(10, (getUnsignedShort(block, 18) & 0x3ff) / 341.0);
+                float temperature = (float) (((getUnsignedShort(block, 20) & 0x3ff) * 150.0 - 20500) / 1000);
                 short rateCode = (short) (block.get(24) & 0xff);
                 short numAxesBPS = (short) (block.get(25) & 0xff);
                 int sampleCount = getUnsignedShort(block, 28);
                 long blockTime = getCwaTimestamp(blockTimeInfo);  // Unix seconds
                 double blockStartTime, blockEndTime;
                 short timestampOffset = 0;
                 float offsetStart = 0;
@@ -217,15 +217,15 @@
                     x /= 256;  // to gravity
                     y /= 256;
                     z /= 256;
 
                     t = blockStartTime + (double)i * (blockEndTime - blockStartTime) / sampleCount;
                     t *= 1000;  // secs to millis
 
-                    writer.write(toItems((long) t, x, y, z, temperature));
+                    writer.write(toItems((long) t, x, y, z, temperature, light));
 
                 }
 
                 return;
 
             }
 
@@ -289,25 +289,25 @@
             writer.close();
         } catch (Exception e) {
             e.printStackTrace();
         }
     }
 
 
-    private static Map<String, Object> toItems(long t, float x, float y, float z, float temperature) {
+    private static Map<String, Object> toItems(long t, float x, float y, float z, float temperature, float light) {
         Map<String, Object> items = new HashMap<String, Object>();
         items.put("time", t);
         items.put("x", x);
         items.put("y", y);
         items.put("z", z);
         items.put("temperature", temperature);
-        // items.put("lux", light);
+        items.put("light", light);
         return items;
     }
 
 
-    private static Map<String, Object> toItems(long t, double x, double y, double z, double temperature) {
-        return toItems(t, (float) x, (float) y, (float) z, (float) temperature);
+    private static Map<String, Object> toItems(long t, double x, double y, double z, double temperature, float light) {
+        return toItems(t, (float) x, (float) y, (float) z, (float) temperature, (float) light);
     }
 
 
 }
```

### Comparing `actipy-2.0.4/src/actipy/GENEActivReader.class` & `actipy-2.1.0/src/actipy/GENEActivReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/src/actipy/GENEActivReader.java` & `actipy-2.1.0/src/actipy/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/src/actipy/NpyWriter.class` & `actipy-2.1.0/src/actipy/NpyWriter.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/src/actipy/NpyWriter.java` & `actipy-2.1.0/src/actipy/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/src/actipy/processing.py` & `actipy-2.1.0/src/actipy/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,14 +366,15 @@
             btype = 'lowpass'
             Wn = lowcut / nyq
     else:
         btype = 'lowpass'
         Wn = cutoffs / nyq
     sos = signal.butter(order, Wn, btype=btype, analog=False, output='sos')
     y = signal.sosfiltfilt(sos, x, axis=axis)
+    y = y.astype(x.dtype, copy=False)
 
     return y
 
 
 def chunker(data, chunksize='4h', leeway='0h', fn=None, fntrim=True):
     """ Return chunk generator for a given datetime-indexed DataFrame.
     A `leeway` parameter can be used to obtain overlapping chunks (e.g. leeway='30m').
@@ -413,11 +414,12 @@
 
 
 def npy2df(data):
     """ Convert a numpy structured array to pandas dataframe. Also parse time
     and set as index. This function will avoid copies whenever possible. """
 
     t = pd.to_datetime(data['time'], unit='ms')
-    columns = [c for c in ['x', 'y', 'z', 'temperature'] if c in data.dtype.names]
+    t.name = 'time'
+    columns = [c for c in data.dtype.names if c != 'time']
     data = pd.DataFrame({c: data[c] for c in columns}, index=t, copy=False)
 
     return data
```

### Comparing `actipy-2.0.4/src/actipy/reader.py` & `actipy-2.1.0/src/actipy/reader.py`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/src/actipy.egg-info/PKG-INFO` & `actipy-2.1.0/src/actipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.0.4
+Version: 2.1.0
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-2.0.4/src/actipy.egg-info/SOURCES.txt` & `actipy-2.1.0/src/actipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actipy-2.0.4/versioneer.py` & `actipy-2.1.0/versioneer.py`

 * *Files identical despite different names*

