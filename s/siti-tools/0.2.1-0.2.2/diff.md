# Comparing `tmp/siti-tools-0.2.1.tar.gz` & `tmp/siti-tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siti-tools-0.2.1.tar", last modified: Fri May 13 15:10:40 2022, max compression
+gzip compressed data, was "siti-tools-0.2.2.tar", last modified: Tue Jun 27 18:59:26 2023, max compression
```

## Comparing `siti-tools-0.2.1.tar` & `siti-tools-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2022-05-13 15:10:40.422652 siti-tools-0.2.1/
--rw-rw-r--   0 werner    (1000) werner    (1000)     1086 2022-05-03 11:24:12.000000 siti-tools-0.2.1/LICENSE
--rw-rw-r--   0 werner    (1000) werner    (1000)    18042 2022-05-13 15:10:40.422652 siti-tools-0.2.1/PKG-INFO
--rw-rw-r--   0 werner    (1000) werner    (1000)    14210 2022-05-13 15:06:19.000000 siti-tools-0.2.1/README.md
--rw-rw-r--   0 werner    (1000) werner    (1000)      568 2022-05-13 15:10:37.000000 siti-tools-0.2.1/pyproject.toml
--rw-rw-r--   0 werner    (1000) werner    (1000)       38 2022-05-13 15:10:40.422652 siti-tools-0.2.1/setup.cfg
--rwxrwxr-x   0 werner    (1000) werner    (1000)     1854 2022-05-13 15:08:04.000000 siti-tools-0.2.1/setup.py
-drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2022-05-13 15:10:40.422652 siti-tools-0.2.1/siti_tools/
--rw-rw-r--   0 werner    (1000) werner    (1000)       22 2022-05-13 15:10:37.000000 siti-tools-0.2.1/siti_tools/__init__.py
--rw-rw-r--   0 werner    (1000) werner    (1000)     9638 2022-05-13 15:06:18.000000 siti-tools-0.2.1/siti_tools/__main__.py
--rw-rw-r--   0 werner    (1000) werner    (1000)     3059 2022-05-03 11:24:12.000000 siti-tools-0.2.1/siti_tools/file.py
--rw-rw-r--   0 werner    (1000) werner    (1000)      864 2022-05-03 11:24:12.000000 siti-tools-0.2.1/siti_tools/log.py
--rw-rw-r--   0 werner    (1000) werner    (1000)    27823 2022-05-13 15:06:18.000000 siti-tools-0.2.1/siti_tools/siti.py
-drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2022-05-13 15:10:40.422652 siti-tools-0.2.1/siti_tools.egg-info/
--rw-rw-r--   0 werner    (1000) werner    (1000)    18042 2022-05-13 15:10:40.000000 siti-tools-0.2.1/siti_tools.egg-info/PKG-INFO
--rw-rw-r--   0 werner    (1000) werner    (1000)      415 2022-05-13 15:10:40.000000 siti-tools-0.2.1/siti_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 werner    (1000) werner    (1000)        1 2022-05-13 15:10:40.000000 siti-tools-0.2.1/siti_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 werner    (1000) werner    (1000)       57 2022-05-13 15:10:40.000000 siti-tools-0.2.1/siti_tools.egg-info/entry_points.txt
--rw-rw-r--   0 werner    (1000) werner    (1000)        1 2022-03-14 12:48:36.000000 siti-tools-0.2.1/siti_tools.egg-info/not-zip-safe
--rw-rw-r--   0 werner    (1000) werner    (1000)       29 2022-05-13 15:10:40.000000 siti-tools-0.2.1/siti_tools.egg-info/requires.txt
--rw-rw-r--   0 werner    (1000) werner    (1000)       11 2022-05-13 15:10:40.000000 siti-tools-0.2.1/siti_tools.egg-info/top_level.txt
-drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2022-05-13 15:10:40.422652 siti-tools-0.2.1/test/
--rwxrwxr-x   0 werner    (1000) werner    (1000)    19102 2022-05-03 11:24:12.000000 siti-tools-0.2.1/test/test.py
--rwxrwxr-x   0 werner    (1000) werner    (1000)     1717 2022-05-03 11:24:12.000000 siti-tools-0.2.1/test/test_decode.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-27 18:59:26.915407 siti-tools-0.2.2/
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2022-09-14 19:11:00.000000 siti-tools-0.2.2/LICENSE
+-rw-r--r--   0 werner     (501) staff       (20)    19401 2023-06-27 18:59:26.915205 siti-tools-0.2.2/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)    15355 2023-06-27 18:56:20.000000 siti-tools-0.2.2/README.md
+-rw-r--r--   0 werner     (501) staff       (20)      567 2023-06-27 18:57:11.000000 siti-tools-0.2.2/pyproject.toml
+-rw-r--r--   0 werner     (501) staff       (20)       38 2023-06-27 18:59:26.915453 siti-tools-0.2.2/setup.cfg
+-rwxr-xr-x   0 werner     (501) staff       (20)     1854 2022-09-14 19:11:00.000000 siti-tools-0.2.2/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-27 18:59:26.912552 siti-tools-0.2.2/siti_tools/
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-06-27 18:56:47.000000 siti-tools-0.2.2/siti_tools/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     9846 2022-09-14 19:11:02.000000 siti-tools-0.2.2/siti_tools/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)     3234 2022-09-14 19:11:00.000000 siti-tools-0.2.2/siti_tools/file.py
+-rw-r--r--   0 werner     (501) staff       (20)      864 2022-09-14 19:11:00.000000 siti-tools-0.2.2/siti_tools/log.py
+-rw-r--r--   0 werner     (501) staff       (20)    27823 2022-09-14 19:11:00.000000 siti-tools-0.2.2/siti_tools/siti.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-27 18:59:26.914251 siti-tools-0.2.2/siti_tools.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    19401 2023-06-27 18:59:26.000000 siti-tools-0.2.2/siti_tools.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      415 2023-06-27 18:59:26.000000 siti-tools-0.2.2/siti_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-06-27 18:59:26.000000 siti-tools-0.2.2/siti_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       56 2023-06-27 18:59:26.000000 siti-tools-0.2.2/siti_tools.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-08 09:46:29.000000 siti-tools-0.2.2/siti_tools.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)       29 2023-06-27 18:59:26.000000 siti-tools-0.2.2/siti_tools.egg-info/requires.txt
+-rw-r--r--   0 werner     (501) staff       (20)       11 2023-06-27 18:59:26.000000 siti-tools-0.2.2/siti_tools.egg-info/top_level.txt
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-27 18:59:26.914770 siti-tools-0.2.2/test/
+-rwxr-xr-x   0 werner     (501) staff       (20)    19102 2022-09-14 19:11:00.000000 siti-tools-0.2.2/test/test.py
+-rwxr-xr-x   0 werner     (501) staff       (20)     1869 2023-06-27 18:46:17.000000 siti-tools-0.2.2/test/test_decode.py
```

### Comparing `siti-tools-0.2.1/LICENSE` & `siti-tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `siti-tools-0.2.1/PKG-INFO` & `siti-tools-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: siti-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Functions to calculate Spatial Information / Temporal Information according to ITU-T P.910
 Home-page: https://github.com/VQEG/siti-tools
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: video,spatial information,temporal information
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Video
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -32,35 +31,30 @@
 
 Contents:
 
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Command Line Usage](#command-line-usage)
-    - [Usage for > 8-bit Content](#usage-for--8-bit-content)
-    - [Full vs. Limited Range](#full-vs-limited-range)
-    - [HDR Usage](#hdr-usage)
   - [Detailed Options](#detailed-options)
   - [Output](#output)
   - [API Usage](#api-usage)
 - [Testing](#testing)
 - [About](#about)
   - [What is SI/TI?](#what-is-siti)
-    - [Spatial Information](#spatial-information)
-    - [Temporal information](#temporal-information)
   - [What is the purpose of this activity?](#what-is-the-purpose-of-this-activity)
   - [Contributors](#contributors)
   - [Acknowledgements](#acknowledgements)
   - [Related Projects](#related-projects)
   - [License](#license)
 
 ## Requirements
 
 - Python 3.8 or higher
-- FFmpeg 4.x libraries (to run `pyav`) — this does not work yet with FFmpeg 5.x, see https://github.com/PyAV-Org/PyAV/issues/817
+- FFmpeg libraries (v5 or higher)
 
 Under Ubuntu, to get ffmpeg libraries:
 
     sudo apt update -qq && \
     sudo apt install \
       libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev \
       libavfilter-dev libswscale-dev libavresample-dev
@@ -88,16 +82,30 @@
 
 ```
 siti-tools /path/to/input/file.mp4
 ```
 
 to run the tool. It will print JSON output containing info about SI/TI values and other statistics to `stdout`.
 
+You can pass any video file with a container that can be read by FFmpeg. For YUV files, see below.
+
 This works for 8-bit standard dynamic range (SDR) content, which will apply to most input files. However, this tool does not automatically handle input that is not 8-bit SDR content. For more info on that, see below.
 
+#### Usage with YUV files
+
+We don't recommend working with raw YUV files, as they do not carry the metadata required to decode them. Use Y4M files or any other container format that can be read by FFmpeg.
+
+To convert YUV into Y4M, use the basic command:
+
+```bash
+ffmpeg -f rawvideo -pix_fmt yuv420p -framerate 24 -video_size 1920x1080 -i input.yuv -c:v copy output.y4m
+```
+
+Adapt the parameters to your input file (i.e., the pixel format, framerate, and resolution).
+
 #### Usage for > 8-bit Content
 
 To deal with input with more than 8-bit, you can choose the bit depth:
 
 ```
 siti-tools /path/to/input/file.mov --bit-depth 10
 ```
@@ -192,15 +200,23 @@
 PU21 options:
   --pu21-mode {banding,banding_glare,peaks,peaks_glare}
                         Specify mode for PU21 (default: banding)
 ```
 
 ### Output
 
-The tool will output a valid JSON object on `stdout`, with SI and TI scores contained in an array. Note that the first frame has no TI value by definition, so a file with two frames would produce the following output:
+The tool will output a valid JSON object on `stdout`, with SI and TI scores contained in an array.
+
+To redirect the output to a file, use shell redirection:
+
+```bash
+siti-tools input1.mp4 > input1.json
+```
+
+Note that the first frame has no TI value by definition, so a file with two frames would produce the following output:
 
 ```json
 {
     "si": [
         4.678114135021466,
         4.690539260164495
     ],
@@ -227,14 +243,45 @@
 In the `settings` key, you will find information on how the calculation was done. This is useful for allowing values to be reproduced. You can use these settings for further calculation runs. For instance, if you want to use the settings used for `input1` for `input2`, run the following:
 
 ```
 siti-tools input1.mp4 > input1.json
 siti-tools input2.mp4 --settings input1.json > input2.json
 ```
 
+You can also generate CSV output, which will contain fewer columns but is easier to parse.
+
+```bash
+siti-tools input1.mp4 --format csv > input1.csv
+siti-tools input2.mp4 --settings input1.json --format csv > input2.csv
+```
+
+The output might look like this:
+
+```
+input_file,n,si,ti
+foreman_cif.y4m,1,39.342,
+foreman_cif.y4m,2,39.229,5.007
+foreman_cif.y4m,3,39.224,5.291
+foreman_cif.y4m,4,39.458,5.08
+foreman_cif.y4m,5,39.212,4.854
+foreman_cif.y4m,6,39.214,4.22
+foreman_cif.y4m,7,39.26,3.95
+foreman_cif.y4m,8,39.351,4.267
+foreman_cif.y4m,9,39.349,4.915
+foreman_cif.y4m,10,39.504,4.77
+```
+
+Note that the first TI value is empty by definition.
+
+There is also a handy conversion utility to help you convert JSON to CSV files after you have calculated the scores.
+
+```bash
+utils/json-to-csv.py input.json input.csv
+```
+
 ### API Usage
 
 The tools expose the calculation functions via an API.
 
 For instance, you can directly use the SI/TI functions:
 
 ```python
@@ -380,14 +427,29 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.2.2 (2023-06-27)
+
+* Update dependencies.
+
+* Update test decode function.
+
+* Explain usage with YUV files.
+
+* Add version support to CLI.
+
+* Add utility for converting JSON output to CSV.
+
+* Error on unsupported frame formats.
+
+
 ## v0.2.1 (2022-05-13)
 
 * Fix console script installation.
 
 * Fix link in setup.py.
 
 * Update README.
@@ -583,9 +645,7 @@
 * Improve README.
 
 * Initial commit.
 
 * Initial commit.
 
 
-
-
```

### Comparing `siti-tools-0.2.1/README.md` & `siti-tools-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,35 +10,30 @@
 
 Contents:
 
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Command Line Usage](#command-line-usage)
-    - [Usage for > 8-bit Content](#usage-for--8-bit-content)
-    - [Full vs. Limited Range](#full-vs-limited-range)
-    - [HDR Usage](#hdr-usage)
   - [Detailed Options](#detailed-options)
   - [Output](#output)
   - [API Usage](#api-usage)
 - [Testing](#testing)
 - [About](#about)
   - [What is SI/TI?](#what-is-siti)
-    - [Spatial Information](#spatial-information)
-    - [Temporal information](#temporal-information)
   - [What is the purpose of this activity?](#what-is-the-purpose-of-this-activity)
   - [Contributors](#contributors)
   - [Acknowledgements](#acknowledgements)
   - [Related Projects](#related-projects)
   - [License](#license)
 
 ## Requirements
 
 - Python 3.8 or higher
-- FFmpeg 4.x libraries (to run `pyav`) — this does not work yet with FFmpeg 5.x, see https://github.com/PyAV-Org/PyAV/issues/817
+- FFmpeg libraries (v5 or higher)
 
 Under Ubuntu, to get ffmpeg libraries:
 
     sudo apt update -qq && \
     sudo apt install \
       libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev \
       libavfilter-dev libswscale-dev libavresample-dev
@@ -66,16 +61,30 @@
 
 ```
 siti-tools /path/to/input/file.mp4
 ```
 
 to run the tool. It will print JSON output containing info about SI/TI values and other statistics to `stdout`.
 
+You can pass any video file with a container that can be read by FFmpeg. For YUV files, see below.
+
 This works for 8-bit standard dynamic range (SDR) content, which will apply to most input files. However, this tool does not automatically handle input that is not 8-bit SDR content. For more info on that, see below.
 
+#### Usage with YUV files
+
+We don't recommend working with raw YUV files, as they do not carry the metadata required to decode them. Use Y4M files or any other container format that can be read by FFmpeg.
+
+To convert YUV into Y4M, use the basic command:
+
+```bash
+ffmpeg -f rawvideo -pix_fmt yuv420p -framerate 24 -video_size 1920x1080 -i input.yuv -c:v copy output.y4m
+```
+
+Adapt the parameters to your input file (i.e., the pixel format, framerate, and resolution).
+
 #### Usage for > 8-bit Content
 
 To deal with input with more than 8-bit, you can choose the bit depth:
 
 ```
 siti-tools /path/to/input/file.mov --bit-depth 10
 ```
@@ -170,15 +179,23 @@
 PU21 options:
   --pu21-mode {banding,banding_glare,peaks,peaks_glare}
                         Specify mode for PU21 (default: banding)
 ```
 
 ### Output
 
-The tool will output a valid JSON object on `stdout`, with SI and TI scores contained in an array. Note that the first frame has no TI value by definition, so a file with two frames would produce the following output:
+The tool will output a valid JSON object on `stdout`, with SI and TI scores contained in an array.
+
+To redirect the output to a file, use shell redirection:
+
+```bash
+siti-tools input1.mp4 > input1.json
+```
+
+Note that the first frame has no TI value by definition, so a file with two frames would produce the following output:
 
 ```json
 {
     "si": [
         4.678114135021466,
         4.690539260164495
     ],
@@ -205,14 +222,45 @@
 In the `settings` key, you will find information on how the calculation was done. This is useful for allowing values to be reproduced. You can use these settings for further calculation runs. For instance, if you want to use the settings used for `input1` for `input2`, run the following:
 
 ```
 siti-tools input1.mp4 > input1.json
 siti-tools input2.mp4 --settings input1.json > input2.json
 ```
 
+You can also generate CSV output, which will contain fewer columns but is easier to parse.
+
+```bash
+siti-tools input1.mp4 --format csv > input1.csv
+siti-tools input2.mp4 --settings input1.json --format csv > input2.csv
+```
+
+The output might look like this:
+
+```
+input_file,n,si,ti
+foreman_cif.y4m,1,39.342,
+foreman_cif.y4m,2,39.229,5.007
+foreman_cif.y4m,3,39.224,5.291
+foreman_cif.y4m,4,39.458,5.08
+foreman_cif.y4m,5,39.212,4.854
+foreman_cif.y4m,6,39.214,4.22
+foreman_cif.y4m,7,39.26,3.95
+foreman_cif.y4m,8,39.351,4.267
+foreman_cif.y4m,9,39.349,4.915
+foreman_cif.y4m,10,39.504,4.77
+```
+
+Note that the first TI value is empty by definition.
+
+There is also a handy conversion utility to help you convert JSON to CSV files after you have calculated the scores.
+
+```bash
+utils/json-to-csv.py input.json input.csv
+```
+
 ### API Usage
 
 The tools expose the calculation functions via an API.
 
 For instance, you can directly use the SI/TI functions:
 
 ```python
```

### Comparing `siti-tools-0.2.1/pyproject.toml` & `siti-tools-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "siti-tools"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Werner Robitza <werner.robitza@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
-numpy = "~=1.22.2"
-scipy = "~=1.8.0"
-av = "~=8.1.0"
-tqdm = "~=4.62.3"
-plotille = "~=4.0.1"
+python = "^3.8.1,<3.12"
+numpy = "~1.23.5"
+scipy = "~1.10.1"
+av = "~10.0.0"
+tqdm = "~4.65.0"
+plotille = "~5.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.1"
+pytest = "^7.4.0"
 flake8 = "^4.0.1"
-black = "^22.3.0"
-requests = "^2.27.1"
+black = "^23.3.0"
+requests = "^2.31.0"
 pytest-xdist = "^2.5.0"
 
 [tool.poetry.scripts]
 siti-tools = 'siti_tools.__main__:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `siti-tools-0.2.1/setup.py` & `siti-tools-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `siti-tools-0.2.1/siti_tools/__main__.py` & `siti-tools-0.2.2/siti_tools/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # SOFTWARE.
 
 import argparse
 import json
 import logging
 import sys
 from tqdm import tqdm
+from . import __version__ as prog_version
 from .log import CustomLogFormatter
 from .siti import (
     CalculationDomain,
     ColorRange,
     EotfFunction,
     HdrMode,
     Pu21Mode,
@@ -81,15 +82,19 @@
 
     logger.addHandler(ch)
 
     return logger
 
 
 def main():
-    parser = argparse.ArgumentParser(prog="siti-tools", formatter_class=CustomArgsFormatter)
+    parser = argparse.ArgumentParser(
+        prog="siti-tools",
+        description=f"siti-tools v{prog_version}",
+        formatter_class=CustomArgsFormatter
+    )
 
     group_io = parser.add_argument_group("input/output")
     group_io.add_argument(
         "input",
         help="Input file, can be Y4M or file in FFmpeg-readable container",
         type=str,
     )
@@ -125,14 +130,17 @@
         "--show-histogram",
         action="store_true",
         help="Show a histogram for the first frame (computation-intensive, implies --verbose)",
     )
     group_io.add_argument(
         "-q", "--quiet", action="store_true", help="Do not show progress bar"
     )
+    group_io.add_argument(
+        "--version", action="version", version=prog_version
+    )
 
     group_general = parser.add_argument_group("Video/SI options")
     group_general.add_argument(
         "-c",
         "--calculation-domain",
         help="Select calculation domain",
         type=CalculationDomain,
```

### Comparing `siti-tools-0.2.1/siti_tools/file.py` & `siti-tools-0.2.2/siti_tools/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,20 @@
     if not len(container.streams.video):
         raise RuntimeError("No video streams found!")
 
     for frame in container.decode(video=0):
         # FIXME: this has been determined experimentally, not sure if it is the
         # correct way to do that -- the return values seem correct for a white/black
         # checkerboard pattern
-        if "p10" in str(frame.format):
+        if "yuv" not in str(frame.format.name):
+            raise RuntimeError(f"Decoding not yet possible for format {frame.format.name}! Only YUV is supported.")
+
+        if "p10" in str(frame.format.name):
             datatype = np.uint16
-        elif "p12" in str(frame.format):
+        elif "p12" in str(frame.format.name):
             datatype = np.uint16
         else:
             datatype = np.uint8
 
         try:
             yield (
                 # The code commented out below does the "standard" conversion of YUV
```

### Comparing `siti-tools-0.2.1/siti_tools/log.py` & `siti-tools-0.2.2/siti_tools/log.py`

 * *Files identical despite different names*

### Comparing `siti-tools-0.2.1/siti_tools/siti.py` & `siti-tools-0.2.2/siti_tools/siti.py`

 * *Files identical despite different names*

### Comparing `siti-tools-0.2.1/siti_tools.egg-info/PKG-INFO` & `siti-tools-0.2.2/siti_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: siti-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Functions to calculate Spatial Information / Temporal Information according to ITU-T P.910
 Home-page: https://github.com/VQEG/siti-tools
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: video,spatial information,temporal information
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Video
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -32,35 +31,30 @@
 
 Contents:
 
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Command Line Usage](#command-line-usage)
-    - [Usage for > 8-bit Content](#usage-for--8-bit-content)
-    - [Full vs. Limited Range](#full-vs-limited-range)
-    - [HDR Usage](#hdr-usage)
   - [Detailed Options](#detailed-options)
   - [Output](#output)
   - [API Usage](#api-usage)
 - [Testing](#testing)
 - [About](#about)
   - [What is SI/TI?](#what-is-siti)
-    - [Spatial Information](#spatial-information)
-    - [Temporal information](#temporal-information)
   - [What is the purpose of this activity?](#what-is-the-purpose-of-this-activity)
   - [Contributors](#contributors)
   - [Acknowledgements](#acknowledgements)
   - [Related Projects](#related-projects)
   - [License](#license)
 
 ## Requirements
 
 - Python 3.8 or higher
-- FFmpeg 4.x libraries (to run `pyav`) — this does not work yet with FFmpeg 5.x, see https://github.com/PyAV-Org/PyAV/issues/817
+- FFmpeg libraries (v5 or higher)
 
 Under Ubuntu, to get ffmpeg libraries:
 
     sudo apt update -qq && \
     sudo apt install \
       libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev \
       libavfilter-dev libswscale-dev libavresample-dev
@@ -88,16 +82,30 @@
 
 ```
 siti-tools /path/to/input/file.mp4
 ```
 
 to run the tool. It will print JSON output containing info about SI/TI values and other statistics to `stdout`.
 
+You can pass any video file with a container that can be read by FFmpeg. For YUV files, see below.
+
 This works for 8-bit standard dynamic range (SDR) content, which will apply to most input files. However, this tool does not automatically handle input that is not 8-bit SDR content. For more info on that, see below.
 
+#### Usage with YUV files
+
+We don't recommend working with raw YUV files, as they do not carry the metadata required to decode them. Use Y4M files or any other container format that can be read by FFmpeg.
+
+To convert YUV into Y4M, use the basic command:
+
+```bash
+ffmpeg -f rawvideo -pix_fmt yuv420p -framerate 24 -video_size 1920x1080 -i input.yuv -c:v copy output.y4m
+```
+
+Adapt the parameters to your input file (i.e., the pixel format, framerate, and resolution).
+
 #### Usage for > 8-bit Content
 
 To deal with input with more than 8-bit, you can choose the bit depth:
 
 ```
 siti-tools /path/to/input/file.mov --bit-depth 10
 ```
@@ -192,15 +200,23 @@
 PU21 options:
   --pu21-mode {banding,banding_glare,peaks,peaks_glare}
                         Specify mode for PU21 (default: banding)
 ```
 
 ### Output
 
-The tool will output a valid JSON object on `stdout`, with SI and TI scores contained in an array. Note that the first frame has no TI value by definition, so a file with two frames would produce the following output:
+The tool will output a valid JSON object on `stdout`, with SI and TI scores contained in an array.
+
+To redirect the output to a file, use shell redirection:
+
+```bash
+siti-tools input1.mp4 > input1.json
+```
+
+Note that the first frame has no TI value by definition, so a file with two frames would produce the following output:
 
 ```json
 {
     "si": [
         4.678114135021466,
         4.690539260164495
     ],
@@ -227,14 +243,45 @@
 In the `settings` key, you will find information on how the calculation was done. This is useful for allowing values to be reproduced. You can use these settings for further calculation runs. For instance, if you want to use the settings used for `input1` for `input2`, run the following:
 
 ```
 siti-tools input1.mp4 > input1.json
 siti-tools input2.mp4 --settings input1.json > input2.json
 ```
 
+You can also generate CSV output, which will contain fewer columns but is easier to parse.
+
+```bash
+siti-tools input1.mp4 --format csv > input1.csv
+siti-tools input2.mp4 --settings input1.json --format csv > input2.csv
+```
+
+The output might look like this:
+
+```
+input_file,n,si,ti
+foreman_cif.y4m,1,39.342,
+foreman_cif.y4m,2,39.229,5.007
+foreman_cif.y4m,3,39.224,5.291
+foreman_cif.y4m,4,39.458,5.08
+foreman_cif.y4m,5,39.212,4.854
+foreman_cif.y4m,6,39.214,4.22
+foreman_cif.y4m,7,39.26,3.95
+foreman_cif.y4m,8,39.351,4.267
+foreman_cif.y4m,9,39.349,4.915
+foreman_cif.y4m,10,39.504,4.77
+```
+
+Note that the first TI value is empty by definition.
+
+There is also a handy conversion utility to help you convert JSON to CSV files after you have calculated the scores.
+
+```bash
+utils/json-to-csv.py input.json input.csv
+```
+
 ### API Usage
 
 The tools expose the calculation functions via an API.
 
 For instance, you can directly use the SI/TI functions:
 
 ```python
@@ -380,14 +427,29 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.2.2 (2023-06-27)
+
+* Update dependencies.
+
+* Update test decode function.
+
+* Explain usage with YUV files.
+
+* Add version support to CLI.
+
+* Add utility for converting JSON output to CSV.
+
+* Error on unsupported frame formats.
+
+
 ## v0.2.1 (2022-05-13)
 
 * Fix console script installation.
 
 * Fix link in setup.py.
 
 * Update README.
@@ -583,9 +645,7 @@
 * Improve README.
 
 * Initial commit.
 
 * Initial commit.
 
 
-
-
```

### Comparing `siti-tools-0.2.1/test/test.py` & `siti-tools-0.2.2/test/test.py`

 * *Files identical despite different names*

### Comparing `siti-tools-0.2.1/test/test_decode.py` & `siti-tools-0.2.2/test/test_decode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python3
 #
 # Verify output of PyAV with limited/full range content
+import glob
+
 import av
 import numpy as np
 
+
 # generate with:
 # ffmpeg -y -f lavfi -i testsrc=size=320x240 -filter:v "scale=in_range=limited:out_range=limited,signalstats,metadata=mode=print" -frames:v 3 -pix_fmt yuv420p videos/limited-range.y4m
 # ffmpeg -y -f lavfi -i testsrc=size=320x240 -filter:v "scale=in_range=limited:out_range=full,signalstats,metadata=mode=print" -frames:v 3 -pix_fmt yuv420p videos/full-range.y4m
 def useful_array(plane, bytes_per_pixel=1):
     total_line_size = abs(plane.line_size)
     useful_line_size = plane.width * bytes_per_pixel
     arr = np.frombuffer(plane, np.uint8)
@@ -15,35 +18,40 @@
         arr = arr.reshape(-1, total_line_size)[:, 0:useful_line_size].reshape(-1)
     return arr
 
 
 def decode_and_print(input_file, bitdepth=8):
     print(input_file)
     container = av.open(input_file)
-    breakpoint()
 
     if bitdepth == 8:
         datatype = np.uint8
     elif bitdepth > 8:
         datatype = np.uint16
     else:
         raise RuntimeError
 
     for idx, frame in enumerate(container.decode(video=0)):
         frame_data = (
             np.frombuffer(frame.planes[0], datatype)
+            .reshape(frame.height, frame.width)
+            .astype("int")
             # useful_array(frame.planes[0])
-            .reshape(frame.height, frame.width).astype("int")
         )
-        print(f"frame {idx} -- min: {np.min(frame_data)}, max: {np.max(frame_data)}")
+        print(
+            f"frame {idx} ({frame.width}x{frame.height}) -- min: {np.min(frame_data)}, max: {np.max(frame_data)}"
+        )
     print()
 
 
 # decode_and_print("videos/limited-range.y4m")
 
 # decode_and_print("videos/full-range.y4m")
 
 # decode_and_print("videos/checkerboard-8x8.y4m")
 
 # decode_and_print("videos/checkerboard-8x8-10bpp-limited.y4m", bitdepth=10)
 
-decode_and_print("videos/checkerboard-8x8-10bpp.y4m", bitdepth=10)
+# decode_and_print("videos/checkerboard-8x8-10bpp.y4m", bitdepth=10)
+
+for video in glob.glob("videos/test-*p.y4m"):
+    decode_and_print(video, bitdepth=8)
```

