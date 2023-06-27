# Comparing `tmp/basic-pitch-0.2.5.tar.gz` & `tmp/basic-pitch-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic-pitch-0.2.5.tar", last modified: Fri May 19 16:52:46 2023, max compression
+gzip compressed data, was "basic-pitch-0.2.6.tar", last modified: Tue Jun 27 17:52:25 2023, max compression
```

## Comparing `basic-pitch-0.2.5.tar` & `basic-pitch-0.2.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/OWNERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/commandline_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/nnaudio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/note_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.497214 basic-pitch-0.2.5/basic_pitch/saved_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.497214 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/
--rw-r--r--   0 runner    (1001) docker     (123)  1084140 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/
--rw-r--r--   0 runner    (1001) docker     (123)   219309 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   802472 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/resources/vocadito_10.wav
--rw-r--r--   0 runner    (1001) docker     (123)  1075892 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/resources/vocadito_14.wav
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/test_note_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.824170 basic-pitch-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/OWNERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 17:52:25.824170 basic-pitch-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.816170 basic-pitch-0.2.6/basic_pitch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/commandline_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.820170 basic-pitch-0.2.6/basic_pitch/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/layers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/layers/nnaudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/layers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.816170 basic-pitch-0.2.6/basic_pitch/saved_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.816170 basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.820170 basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/
+-rw-r--r--   0 runner    (1001) docker     (123)  1084140 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.820170 basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)   219309 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.816170 basic-pitch-0.2.6/basic_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 17:52:25.000000 basic-pitch-0.2.6/basic_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-27 17:52:25.000000 basic-pitch-0.2.6/basic_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:52:25.000000 basic-pitch-0.2.6/basic_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 17:52:25.000000 basic-pitch-0.2.6/basic_pitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:52:25.000000 basic-pitch-0.2.6/basic_pitch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 17:52:25.000000 basic-pitch-0.2.6/basic_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 17:52:25.000000 basic-pitch-0.2.6/basic_pitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-27 17:52:25.824170 basic-pitch-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.820170 basic-pitch-0.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:52:25.820170 basic-pitch-0.2.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   802472 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/tests/resources/vocadito_10.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  1075892 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/tests/resources/vocadito_14.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/tests/test_note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-27 17:52:11.000000 basic-pitch-0.2.6/tox.ini
```

### Comparing `basic-pitch-0.2.5/CODE_OF_CONDUCT.md` & `basic-pitch-0.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/CONTRIBUTING.md` & `basic-pitch-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/LICENSE` & `basic-pitch-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/NOTICE` & `basic-pitch-0.2.6/NOTICE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/OWNERS.md` & `basic-pitch-0.2.6/OWNERS.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/PKG-INFO` & `basic-pitch-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.2.5
+Version: 0.2.6
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Home-page: https://github.com/spotify/basic-pitch
 Author: Spotify
 Author-email: basic-pitch@spotify.com
 Maintainer: Spotify
 Maintainer-email: basic-pitch@spotify.com
 License: Apache 2.0
```

### Comparing `basic-pitch-0.2.5/README.md` & `basic-pitch-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/SECURITY.md` & `basic-pitch-0.2.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/__init__.py` & `basic-pitch-0.2.6/basic_pitch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pathlib
 
 __author__ = "Spotify"
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __email__ = "basic-pitch@spotify.com"
 __demowebsite__ = "https://basicpitch.io"
 __description__ = "Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection."
 __url__ = "https://github.com/spotify/basic-pitch"
 
 ICASSP_2022_MODEL_PATH = pathlib.Path(__file__).parent / "saved_models/icassp_2022/nmp"
```

### Comparing `basic-pitch-0.2.5/basic_pitch/commandline_printing.py` & `basic-pitch-0.2.6/basic_pitch/commandline_printing.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/constants.py` & `basic-pitch-0.2.6/basic_pitch/constants.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/inference.py` & `basic-pitch-0.2.6/basic_pitch/inference.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/layers/math.py` & `basic-pitch-0.2.6/basic_pitch/layers/math.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/layers/nnaudio.py` & `basic-pitch-0.2.6/basic_pitch/layers/nnaudio.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/layers/signal.py` & `basic-pitch-0.2.6/basic_pitch/layers/signal.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/models.py` & `basic-pitch-0.2.6/basic_pitch/models.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/nn.py` & `basic-pitch-0.2.6/basic_pitch/nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/note_creation.py` & `basic-pitch-0.2.6/basic_pitch/note_creation.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/predict.py` & `basic-pitch-0.2.6/basic_pitch/predict.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb` & `basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001` & `basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index` & `basic-pitch-0.2.6/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/basic_pitch.egg-info/PKG-INFO` & `basic-pitch-0.2.6/basic_pitch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.2.5
+Version: 0.2.6
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Home-page: https://github.com/spotify/basic-pitch
 Author: Spotify
 Author-email: basic-pitch@spotify.com
 Maintainer: Spotify
 Maintainer-email: basic-pitch@spotify.com
 License: Apache 2.0
```

### Comparing `basic-pitch-0.2.5/basic_pitch.egg-info/SOURCES.txt` & `basic-pitch-0.2.6/basic_pitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/setup.cfg` & `basic-pitch-0.2.6/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.5
+current_version = 0.2.6
 commit = True
 tag = True
 
 [metadata]
 name = basic-pitch
 version = attr: basic_pitch.__version__
 description = Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
@@ -35,16 +35,16 @@
 install_requires = 
 	librosa>=0.8.0
 	mir_eval>=0.6
 	numpy<1.24,>=1.18
 	pretty_midi>=0.2.9
 	resampy>=0.2.2
 	scipy>=1.4.1
-	tensorflow>=2.4.1,<2.12; platform_machine != 'arm64'
-	tensorflow-macos>=2.4.1,<2.12; platform_machine == 'arm64'
+	tensorflow>=2.4.1; platform_machine != 'arm64'
+	tensorflow-macos>=2.4.1; platform_machine == 'arm64'
 	typing_extensions
 
 [options.entry_points]
 console_scripts = 
 	basic-pitch = basic_pitch.predict:main
 
 [options.extras_require]
```

### Comparing `basic-pitch-0.2.5/setup.py` & `basic-pitch-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/tests/resources/vocadito_10.wav` & `basic-pitch-0.2.6/tests/resources/vocadito_10.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/tests/resources/vocadito_14.wav` & `basic-pitch-0.2.6/tests/resources/vocadito_14.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/tests/test_inference.py` & `basic-pitch-0.2.6/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/tests/test_nn.py` & `basic-pitch-0.2.6/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/tests/test_note_creation.py` & `basic-pitch-0.2.6/tests/test_note_creation.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.5/tox.ini` & `basic-pitch-0.2.6/tox.ini`

 * *Files identical despite different names*

