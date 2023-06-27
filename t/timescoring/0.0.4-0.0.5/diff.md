# Comparing `tmp/timescoring-0.0.4.tar.gz` & `tmp/timescoring-0.0.5.tar.gz`

## Comparing `timescoring-0.0.4.tar` & `timescoring-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 timescoring-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 timescoring-0.0.4/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 timescoring-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/annotations.py
--rw-r--r--   0        0        0     9221 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/scoring.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/visualization.py
--rw-r--r--   0        0        0    12973 2020-02-02 00:00:00.000000 timescoring-0.0.4/tests/test.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 timescoring-0.0.4/LICENSE
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 timescoring-0.0.4/README.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 timescoring-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 timescoring-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 timescoring-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 timescoring-0.0.5/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 timescoring-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timescoring-0.0.5/src/timescoring/__init__.py
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 timescoring-0.0.5/src/timescoring/annotations.py
+-rw-r--r--   0        0        0     9221 2020-02-02 00:00:00.000000 timescoring-0.0.5/src/timescoring/scoring.py
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 timescoring-0.0.5/src/timescoring/visualization.py
+-rw-r--r--   0        0        0    13482 2020-02-02 00:00:00.000000 timescoring-0.0.5/tests/test.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 timescoring-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 timescoring-0.0.5/README.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 timescoring-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 timescoring-0.0.5/PKG-INFO
```

### Comparing `timescoring-0.0.4/.github/workflows/python-app.yml` & `timescoring-0.0.5/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.4/.github/workflows/python-publish.yml` & `timescoring-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.4/src/timescoring/annotations.py` & `timescoring-0.0.5/src/timescoring/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             events = list()
             tmpEnd = []
             # Find transitions
             start_i = np.where(np.diff(np.array(data, dtype=int)) == 1)[0]
             end_i = np.where(np.diff(np.array(data, dtype=int)) == -1)[0]
 
             # No transitions and first sample is positive -> event is duration of file
-            if len(start_i) == 0 and data[0]:
+            if len(start_i) == 0 and len(end_i) == 0 and data[0]:
                 events.append((0, len(data) / fs))
             else:
                 # Edge effect - First sample is an event
                 if data[0]:
                     events.append((0, (end_i[0] + 1) / fs))
                     end_i = np.delete(end_i, 0)
                 # Edge effect - Last event runs until end of file
```

### Comparing `timescoring-0.0.4/src/timescoring/scoring.py` & `timescoring-0.0.5/src/timescoring/scoring.py`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.4/src/timescoring/visualization.py` & `timescoring-0.0.5/src/timescoring/visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,30 +106,30 @@
     # Plot REF TP & FN
     for event in score.ref.events:
         # TP
         if np.any(score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
             color = 'tab:green'
         else:
             color = 'tab:purple'
-        _plotEvent([event[0], event[1] - (1 / score.fs)], [1, 1], color, ax,
+        _plotEvent([event[0], event[1] - (1 / ref.fs)], [1, 1], color, ax,
                    [max(0, event[0] - param.toleranceStart), min(time[-1], event[1] + param.toleranceEnd - (1 / ref.fs))])
 
     # Plot HYP TP & FP
     for event in score.hyp.events:
         # FP
         if np.all(~score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
-            _plotEvent([event[0], event[1] - (1 / score.fs)], [0.5, 0.5], 'tab:red', ax)
+            _plotEvent([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5], 'tab:red', ax)
         # TP
         elif np.all(score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
-            ax.plot([event[0], event[1] - (1 / score.fs)], [0.5, 0.5],
+            ax.plot([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5],
                     color='tab:green', linewidth=5, solid_capstyle='butt', linestyle='solid')
         # Mix TP, FP
         else:
-            _plotEvent([event[0], event[1] - (1 / score.fs)], [0.5, 0.5], 'tab:red', ax, zorder=1.7)
-            ax.plot([event[0], event[1] - (1 / score.fs)], [0.5, 0.5],
+            _plotEvent([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5], 'tab:red', ax, zorder=1.7)
+            ax.plot([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5],
                     color='tab:green', linewidth=5, solid_capstyle='butt', linestyle=(0, (2, 2)))
 
     # Text
     plt.title('Event Scoring')
 
     ax.set_yticks([0.3, 0.8], ['HYP', 'REF'])
     _scale_time_xaxis(ax)
```

### Comparing `timescoring-0.0.4/tests/test.py` & `timescoring-0.0.5/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,33 @@
         TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'Simple events')
 
         # Event == File duration
         mask = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
         events = [(0.0, 1.0)]
         TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'Event = file duration')
 
-        # Event at start
+        # Event at start - single events
+        mask = [1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
+        events = [(0.0, 0.4)]
+        TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'event at start - single events')
+
+        # Event at end - single events
+        mask = [0, 0, 0, 0, 0, 0, 0, 1, 1, 1]
+        events = [(0.7, 1.)]
+        TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'event at end - single events')
+
+        # Event at start - multiple events
         mask = [1, 1, 1, 1, 0, 0, 1, 0, 0, 0]
         events = [(0.0, 0.4), (0.6, 0.7)]
-        TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'event at start')
+        TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'event at start - multiple events')
 
-        # Event at end
+        # Event at end - multiple events
         mask = [0, 1, 1, 0, 0, 0, 0, 1, 1, 1]
         events = [(0.1, 0.3), (0.7, 1.)]
-        TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'event at end')
+        TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'event at end - multiple events')
 
         # Event at start and end
         mask = [1, 1, 1, 0, 0, 0, 0, 1, 0, 1]
         events = [(0.0, 0.3), (0.7, 0.8), (0.9, 1.0)]
         TestAnnotation.checkMaskEvents(mask, events, fs, numSamples, 'event at start and end')
```

### Comparing `timescoring-0.0.4/LICENSE` & `timescoring-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.4/README.md` & `timescoring-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.4/pyproject.toml` & `timescoring-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "timescoring"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jonathan Dan", email="jonathan.dan@epfl.ch" },
   { name="Una Pale", email="una.pale@epfl.ch" },
   { name="PEDESITE" }
 ]
 description = "Library for measuring performance of time series classification"
 readme = "README.md"
```

### Comparing `timescoring-0.0.4/PKG-INFO` & `timescoring-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timescoring
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for measuring performance of time series classification
 Project-URL: Homepage, https://github.com/esl-epfl/epilepsy_performance_metrics
 Project-URL: Bug Tracker, https://github.com/esl-epfl/epilepsy_performance_metrics/issues
 Author: PEDESITE
 Author-email: Jonathan Dan <jonathan.dan@epfl.ch>, Una Pale <una.pale@epfl.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

