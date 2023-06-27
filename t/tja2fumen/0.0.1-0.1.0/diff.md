# Comparing `tmp/tja2fumen-0.0.1.tar.gz` & `tmp/tja2fumen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.0.1.tar", last modified: Sun Jun  4 19:27:41 2023, max compression
+gzip compressed data, was "tja2fumen-0.1.0.tar", last modified: Tue Jun 27 01:15:29 2023, max compression
```

## Comparing `tja2fumen-0.0.1.tar` & `tja2fumen-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.963748 tja2fumen-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-06-04 16:36:23.000000 tja2fumen-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4390 2023-06-04 19:27:41.962749 tja2fumen-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-06-04 19:27:00.000000 tja2fumen-0.0.1/README.md
--rw-rw-rw-   0        0        0      720 2023-06-04 19:27:19.000000 tja2fumen-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 19:27:41.963748 tja2fumen-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       96 2023-06-04 15:18:33.000000 tja2fumen-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.922466 tja2fumen-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.937436 tja2fumen-0.0.1/src/tja2fumen/
--rw-rw-rw-   0        0        0     1178 2023-06-04 16:30:47.000000 tja2fumen-0.0.1/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-06-04 16:25:40.000000 tja2fumen-0.0.1/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    11608 2023-06-04 18:47:43.000000 tja2fumen-0.0.1/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    20666 2023-06-04 16:25:40.000000 tja2fumen-0.0.1/src/tja2fumen/parsers.py
--rw-rw-rw-   0        0        0    13964 2023-06-04 18:47:43.000000 tja2fumen-0.0.1/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2851 2023-06-04 16:25:40.000000 tja2fumen-0.0.1/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.960375 tja2fumen-0.0.1/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4390 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 01:15:29.106199 tja2fumen-0.1.0/
+-rw-rw-rw-   0        0        0     1083 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4390 2023-06-27 01:15:29.106199 tja2fumen-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/README.md
+-rw-rw-rw-   0        0        0      720 2023-06-27 01:15:16.000000 tja2fumen-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 01:15:29.106199 tja2fumen-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:15:29.074922 tja2fumen-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 01:15:29.090563 tja2fumen-0.1.0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1609 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     4430 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    12255 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    20582 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/src/tja2fumen/parsers.py
+-rw-rw-rw-   0        0        0     3864 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2847 2023-06-27 01:14:40.000000 tja2fumen-0.1.0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:15:29.090563 tja2fumen-0.1.0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4390 2023-06-27 01:15:29.000000 tja2fumen-0.1.0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-06-27 01:15:29.000000 tja2fumen-0.1.0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 01:15:29.000000 tja2fumen-0.1.0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-27 01:15:29.000000 tja2fumen-0.1.0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 01:15:29.000000 tja2fumen-0.1.0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 01:15:29.000000 tja2fumen-0.1.0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.0.1/LICENSE.txt` & `tja2fumen-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.1/PKG-INFO` & `tja2fumen-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.0.1
+Version: 0.1.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.0.1/README.md` & `tja2fumen-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.1/pyproject.toml` & `tja2fumen-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.0.1"
+version = "0.1.0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.0.1/src/tja2fumen/converters.py` & `tja2fumen-0.1.0/src/tja2fumen/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from copy import deepcopy
 
-from tja2fumen.utils import computeSoulGaugeByte
-from tja2fumen.constants import TJA_NOTE_TYPES, DIFFICULTY_BYTES, unknownHeaderSample
+from tja2fumen.utils import computeSoulGaugeBytes
+from tja2fumen.constants import TJA_NOTE_TYPES, DIFFICULTY_BYTES, sampleHeaderMetadata, simpleHeaders
 
 # Filler metadata that the `writeFumen` function expects
+# TODO: Determine how to properly set the item byte (https://github.com/vivaria/tja2fumen/issues/17)
 default_note = {'type': '', 'pos': 0.0, 'item': 0, 'padding': 0.0,
                 'scoreInit': 0, 'scoreDiff': 0, 'duration': 0.0}
 default_branch = {'length': 0, 'padding': 0, 'speed': 1.0}
 default_measure = {
     'bpm': 0.0,
     'fumenOffset': 0.0,
     'gogo': False,
-    'hidden': True,
+    'barline': True,
     'padding1': 0,
     'branchInfo': [-1, -1, -1, -1, -1, -1],
     'padding2': 0,
     'normal': deepcopy(default_branch),
     'advanced': deepcopy(default_branch),
     'master': deepcopy(default_branch)
 }
@@ -38,14 +39,15 @@
     if it has multiple BPM changes within a measure.
 
     In the future, this logic should probably be moved into the TJA parser itself.
     """
     currentBPM = 0
     currentScroll = 1.0
     currentGogo = False
+    currentBarline = True
 
     measuresCorrected = []
     for measure in tja['measures']:
         # Step 1: Combine notes and events
         notes = [{'pos': i, 'type': 'note', 'value': TJA_NOTE_TYPES[note]}
                  for i, note in enumerate(measure['data']) if note != '0']
         events = [{'pos': e['position'], 'type': e['name'], 'value': e['value']}
@@ -59,40 +61,41 @@
                     combined.append(notes.pop(0))
             elif events:
                 combined.append(events.pop(0))
             elif notes:
                 combined.append(notes.pop(0))
 
         # Step 2: Split measure into submeasure
-        measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo,
+        measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo, 'barline': currentBarline,
                        'subdivisions': len(measure['data']), 'pos_start': 0, 'pos_end': 0,
                        'time_sig': measure['length'], 'data': []}
         for data in combined:
             if data['type'] == 'note':
                 measure_cur['data'].append(data)
             elif data['type'] == 'bpm':
                 currentBPM = float(data['value'])
                 # Case 1: BPM change at the start of a measure; just change BPM
                 if data['pos'] == 0:
                     measure_cur['bpm'] = currentBPM
                 # Case 2: BPM change mid-measure, so start a new sub-measure
                 else:
                     measure_cur['pos_end'] = data['pos']
                     measuresCorrected.append(measure_cur)
-                    measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo,
+                    measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo, 'barline': currentBarline,
                                    'subdivisions': len(measure['data']), 'pos_start': data['pos'], 'pos_end': 0,
                                    'time_sig': measure['length'], 'data': []}
             elif data['type'] == 'scroll':
                 currentScroll = data['value']
                 measure_cur['scroll'] = currentScroll
             elif data['type'] == 'gogo':
-                currentGogo = bool(data['value'])
+                currentGogo = bool(int(data['value']))
                 measure_cur['gogo'] = currentGogo
             elif data['type'] == 'barline':
-                pass
+                currentBarline = bool(int(data['value']))
+                measure_cur['barline'] = currentBarline
             else:
                 print(f"Unexpected event type: {data['type']}")
         measure_cur['pos_end'] = len(measure['data'])
         measuresCorrected.append(measure_cur)
 
     return measuresCorrected
 
@@ -132,21 +135,22 @@
                 tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
                 tjaConverted['measures'][-1]['fumenOffset'] = tjaOffset - measureDuration
             # Use the previous measure's offset plus the previous duration to compute the current measure's offset
             measureOffsetPrev = tjaConverted['measures'][-1]['fumenOffset']
             measureFumen['fumenOffset'] = measureOffsetPrev + measureDurationPrev
         measureDurationPrev = measureDuration
 
-        # Best guess at what 'hidden' status means for each measure:
-        # - 'True' means the measure lands on a barline (i.e. most measures)
-        # - 'False' means that the measure is between barlines. For example:
-        #     1. Measures before the first barline
+        # Best guess at what 'barline' status means for each measure:
+        # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
+        # - 'False' means that the measure doesn't land on a barline, and thus barline should be hidden.
+        #   For example:
+        #     1. Measures where #BARLINEOFF has been set
         #     2. Sub-measures that don't fall on the barline
-        if idx_m == 0 or (measureRatio != 1.0 and measureTJA['pos_start'] != 0):
-            measureFumen['hidden'] = False
+        if measureTJA['barline'] is False or (measureRatio != 1.0 and measureTJA['pos_start'] != 0):
+            measureFumen['barline'] = False
 
         # Create note dictionaries based on TJA measure data (containing 0's plus 1/2/3/4/etc. for notes)
         note_counter = 0
         for idx_d, data in enumerate(measureTJA['data']):
             if data['type'] == 'note':
                 # Note positions must be calculated using the base measure duration (that uses a single BPM value)
                 # (In other words, note positions do not take into account any mid-measure BPM change adjustments.)
@@ -202,19 +206,24 @@
                 currentDrumroll['multimeasure'] = True
             else:
                 currentDrumroll['duration'] += measureDurationBase
 
         total_notes += note_counter
 
     # Take a stock header metadata sample and add song-specific metadata
-    headerMetadata = unknownHeaderSample
+    headerMetadata = sampleHeaderMetadata
     headerMetadata[8] = DIFFICULTY_BYTES[tja['metadata']['course']][0]
     headerMetadata[9] = DIFFICULTY_BYTES[tja['metadata']['course']][1]
-    headerMetadata[20] = computeSoulGaugeByte(total_notes)
-    tjaConverted['headerUnknown'] = b"".join(i.to_bytes(1, 'little') for i in headerMetadata)
+    headerMetadata[20], headerMetadata[21] = computeSoulGaugeBytes(
+        n_notes=total_notes,
+        difficulty=tja['metadata']['course'],
+        stars=tja['metadata']['level']
+    )
+    tjaConverted['headerMetadata'] = b"".join(i.to_bytes(1, 'little') for i in headerMetadata)
+    tjaConverted['headerPadding'] = simpleHeaders[0]  # Use a basic, known set of header bytes
     tjaConverted['order'] = '<'
     tjaConverted['length'] = len(tjaConverted['measures'])
     tjaConverted['unknownMetadata'] = 0
     tjaConverted['branches'] = False
     tjaConverted['scoreInit'] = tja['scoreInit']
     tjaConverted['scoreDiff'] = tja['scoreDiff']
```

### Comparing `tja2fumen-0.0.1/src/tja2fumen/parsers.py` & `tja2fumen-0.1.0/src/tja2fumen/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import os
 import re
 
-from tja2fumen.utils import readStruct, getBool, shortHex, nameValue, debugPrint, checkValidHeader
+from tja2fumen.utils import readStruct, getBool, shortHex, nameValue, debugPrint
 from tja2fumen.constants import (
     # TJA constants
     HEADER_GLOBAL, HEADER_COURSE, BRANCH_COMMANDS, MEASURE_COMMANDS, COMMAND, NORMALIZE_COURSE,
     # Fumen constants
     branchNames, noteTypes
 )
 
 
 ########################################################################################################################
 # TJA-parsing functions ( Original source: https://github.com/WHMHammer/tja-tools/blob/master/src/js/parseTJA.js)
 ########################################################################################################################
 
 
-def parseTJA(tja):
+def parseTJA(fnameTJA):
+    try:
+        tja = open(fnameTJA, "r", encoding="utf-8-sig")
+    except UnicodeDecodeError:
+        tja = open(fnameTJA, "r", encoding="shift-jis")
+
     # Split into lines
     lines = tja.read().splitlines()
     lines = [line for line in lines if line.strip()]  # Discard empty lines
 
     # Line by line
     headers = {}
     courses = {}
@@ -283,21 +288,16 @@
     """
     if type(fumenFile) is str:
         file = open(fumenFile, "rb")
     else:
         file = fumenFile
     size = os.fstat(file.fileno()).st_size
 
-    # Check for valid fumen header (first 432 bytes) using valid byte substrings
-    fumenHeader = file.read(432)
-    if not checkValidHeader(fumenHeader):
-        debugPrint(f"Invalid header!")
-    # Read the next 80 bytes, which contains unknown information
-    fumenHeaderUnknown = file.read(80)
-    # validateHeaderMetadata(fumenHeaderUnknown)
+    # Fetch the header bytes
+    fumenHeader = file.read(512)
 
     # Determine:
     #   - The byte order (big or little endian)
     #   - The total number of measures from byte 0x200 (decimal 512)
     if byteOrder:
         order = ">" if byteOrder == "big" else "<"
         totalMeasures = readStruct(file, order, format_string="I", seek=0x200)[0]
@@ -307,22 +307,24 @@
         measuresLittle = readStruct(file, order="", format_string="<I", seek=0x200)[0]
         if measuresBig < measuresLittle:
             order = ">"
             totalMeasures = measuresBig
         else:
             order = "<"
             totalMeasures = measuresLittle
-    unknownMetadata = readStruct(file, order, format_string="I", seek=0x204)[0]
 
     # Initialize the dict that will contain the chart information
     song = {'measures': []}
-    song['header'] = fumenHeader
-    song['headerUnknown'] = fumenHeaderUnknown
+    song['headerPadding'] = fumenHeader[:432]
+    song['headerMetadata'] = fumenHeader[-80:]
     song['order'] = order
     song["length"] = totalMeasures
+
+    # I am unsure what byte this represents
+    unknownMetadata = readStruct(file, order, format_string="I", seek=0x204)[0]
     song["unknownMetadata"] = unknownMetadata
 
     # Determine whether the song has branches from byte 0x1b0 (decimal 432)
     hasBranches = getBool(readStruct(file, order, format_string="B", seek=0x1b0)[0])
     song["branches"] = hasBranches
 
     # Print general debug metadata about the song
@@ -337,15 +339,15 @@
     file.seek(0x208)
     for measureNumber in range(totalMeasures):
         # Parse the measure data using the following `format_string`:
         #   "ffBBHiiiiiii" (12 format characters, 40 bytes per measure)
         #     - 'f': BPM              (represented by one float (4 bytes))
         #     - 'f': fumenOffset      (represented by one float (4 bytes))
         #     - 'B': gogo             (represented by one unsigned char (1 byte))
-        #     - 'B': hidden           (represented by one unsigned char (1 byte))
+        #     - 'B': barline           (represented by one unsigned char (1 byte))
         #     - 'H': <padding>        (represented by one unsigned short (2 bytes))
         #     - 'iiiiii': branchInfo  (represented by six integers (24 bytes))
         #     - 'i': <padding>        (represented by one integer (4 bytes)
         measureStruct = readStruct(file, order, format_string="ffBBHiiiiiii")
 
         # Create the measure dictionary using the newly-parsed measure data
         measure = {}
@@ -354,15 +356,15 @@
         # if measureNumber == 0:
         #     measure["offset"] = measure["fumenOffset"] + 240000 / measure["bpm"]
         # else:
         #     prev = song['measures'][measureNumber - 1]
         #     measure["offset"] = ((prev["offset"] + measure["fumenOffset"] + 240000) /
         #                          (measure["bpm"] - prev["fumenOffset"] - 240000 / prev["bpm"]))
         measure["gogo"] = getBool(measureStruct[2])
-        measure["hidden"] = getBool(measureStruct[3])
+        measure["barline"] = getBool(measureStruct[3])
         measure["padding1"] = measureStruct[4]
         measure["branchInfo"] = list(measureStruct[5:11])
         measure["padding2"] = measureStruct[11]
 
         # Iterate through the three branch types
         for branchNumber in range(len(branchNames)):
             # Parse the measure data using the following `format_string`:
```

### Comparing `tja2fumen-0.0.1/src/tja2fumen/writers.py` & `tja2fumen-0.1.0/src/tja2fumen/writers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from tja2fumen.utils import writeStruct, putBool
-from tja2fumen.constants import simpleHeaders, branchNames, typeNotes
+from tja2fumen.constants import branchNames, typeNotes
 
 
 def writeFumen(file, song):
     # Fetch the byte order (little/big endian)
     order = song['order']
 
     # Write the header
-    file.write(simpleHeaders[0])       # Write known, valid header
-    file.write(song['headerUnknown'])  # Write unknown header
+    file.write(song['headerPadding'])   # Write header padding bytes
+    file.write(song['headerMetadata'])  # Write header metadata bytes
 
     # Preallocate space in the file
     len_metadata = 8
     len_measures = 0
     for measureNumber in range(song['length']):
         len_measures += 40
         measure = song['measures'][measureNumber]
@@ -31,15 +31,15 @@
     writeStruct(file, order, format_string="I", value_list=[song['length']], seek=0x200)
     writeStruct(file, order, format_string="I", value_list=[song['unknownMetadata']], seek=0x204)
 
     # Write measure data
     file.seek(0x208)
     for measureNumber in range(song['length']):
         measure = song['measures'][measureNumber]
-        measureStruct = [measure['bpm'], measure['fumenOffset'], int(measure['gogo']), int(measure['hidden'])]
+        measureStruct = [measure['bpm'], measure['fumenOffset'], int(measure['gogo']), int(measure['barline'])]
         measureStruct.extend([measure['padding1']] + measure['branchInfo'] + [measure['padding2']])
         writeStruct(file, order, format_string="ffBBHiiiiiii", value_list=measureStruct)
 
         for branchNumber in range(len(branchNames)):
             branch = measure[branchNames[branchNumber]]
             branchStruct = [branch['length'], branch['padding'], branch['speed']]
             writeStruct(file, order, format_string="HHf", value_list=branchStruct)
```

### Comparing `tja2fumen-0.0.1/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.1.0/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.0.1
+Version: 0.1.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

