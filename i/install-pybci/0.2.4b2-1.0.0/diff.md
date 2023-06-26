# Comparing `tmp/install-pybci-0.2.4b2.tar.gz` & `tmp/install-pybci-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.4b2.tar", last modified: Fri Jun 23 14:39:37 2023, max compression
+gzip compressed data, was "install-pybci-1.0.0.tar", last modified: Mon Jun 26 22:54:26 2023, max compression
```

## Comparing `install-pybci-0.2.4b2.tar` & `install-pybci-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/OptimisedDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:54:26.217618 install-pybci-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 22:53:45.000000 install-pybci-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 22:53:45.000000 install-pybci-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-26 22:54:26.217618 install-pybci-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-06-26 22:53:45.000000 install-pybci-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:54:26.213618 install-pybci-1.0.0/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-26 22:54:26.000000 install-pybci-1.0.0/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 22:54:26.000000 install-pybci-1.0.0/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:54:26.000000 install-pybci-1.0.0/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 22:54:26.000000 install-pybci-1.0.0/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 22:54:26.000000 install-pybci-1.0.0/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:54:26.213618 install-pybci-1.0.0/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:54:26.213618 install-pybci-1.0.0/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:54:26.217618 install-pybci-1.0.0/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/ThreadClasses/OptimisedDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:54:26.217618 install-pybci-1.0.0/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20072 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 22:53:45.000000 install-pybci-1.0.0/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:54:26.217618 install-pybci-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-26 22:53:45.000000 install-pybci-1.0.0/setup.py
```

### Comparing `install-pybci-0.2.4b2/LICENSE` & `install-pybci-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/PKG-INFO` & `install-pybci-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.4b2
+Version: 1.0.0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, Pytorch, SciKit-Learn and Tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -78,19 +78,8 @@
 ## Background Information
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
-## ToDo!
-- ~~Update ReadTheDocs!~~
-- ~~Finish arduino hand grasp demo and video.~~
-- Tst and likely Fix multimodal after new data thread creation
-- ~~Combine multiple data streams for multi modal bci!~~
-- ~~Add pytorch compatibility!~~ 
-- ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
-- ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
-- ~~Levels of print debug (info, error, none)~~
-- ~~Retrieve feature data~~
-
-## Curently in Beta, come back in a few days for updates!
+## Any issues, recommendations, pull-requests and suggestions are welcome and encouraged!
```

### Comparing `install-pybci-0.2.4b2/README.md` & `install-pybci-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,19 +48,8 @@
 ## Background Information
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
-## ToDo!
-- ~~Update ReadTheDocs!~~
-- ~~Finish arduino hand grasp demo and video.~~
-- Tst and likely Fix multimodal after new data thread creation
-- ~~Combine multiple data streams for multi modal bci!~~
-- ~~Add pytorch compatibility!~~ 
-- ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
-- ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
-- ~~Levels of print debug (info, error, none)~~
-- ~~Retrieve feature data~~
-
-## Curently in Beta, come back in a few days for updates!
+## Any issues, recommendations, pull-requests and suggestions are welcome and encouraged!
```

### Comparing `install-pybci-0.2.4b2/install_pybci.egg-info/PKG-INFO` & `install-pybci-1.0.0/install_pybci.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.4b2
+Version: 1.0.0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, Pytorch, SciKit-Learn and Tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -78,19 +78,8 @@
 ## Background Information
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
-## ToDo!
-- ~~Update ReadTheDocs!~~
-- ~~Finish arduino hand grasp demo and video.~~
-- Tst and likely Fix multimodal after new data thread creation
-- ~~Combine multiple data streams for multi modal bci!~~
-- ~~Add pytorch compatibility!~~ 
-- ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
-- ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
-- ~~Levels of print debug (info, error, none)~~
-- ~~Retrieve feature data~~
-
-## Curently in Beta, come back in a few days for updates!
+## Any issues, recommendations, pull-requests and suggestions are welcome and encouraged!
```

### Comparing `install-pybci-0.2.4b2/install_pybci.egg-info/SOURCES.txt` & `install-pybci-1.0.0/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/Configuration/EpochSettings.py` & `install-pybci-1.0.0/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-1.0.0/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-1.0.0/pybci/ThreadClasses/ClassifierThread.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 
 class ClassifierThread(threading.Thread):
     features = np.array([])#[]
     targets = np.array([])
     mode = "train"
     guess = " "
-    epochCountsc = {} 
+    #epochCountsc = {} 
     def __init__(self, closeEvent,trainTestEvent, featureQueueTest,featureQueueTrain, classifierInfoQueue, classifierInfoRetrieveEvent, 
                  classifierGuessMarkerQueue, classifierGuessMarkerEvent, queryFeaturesQueue, queryFeaturesEvent,
                  logger = Logger(Logger.INFO), numStreamDevices = 1,
                  minRequiredEpochs = 10, clf = None, model = None, torchModel = None):
         super().__init__()
         self.trainTestEvent = trainTestEvent # responsible for tolling between train and test mode
         self.closeEvent = closeEvent # responsible for cosing threads
@@ -26,43 +26,46 @@
         self.classifierGuessMarkerEvent = classifierGuessMarkerEvent
         self.queryFeaturesQueue = queryFeaturesQueue
         self.queryFeaturesEvent = queryFeaturesEvent
         self.numStreamDevices = numStreamDevices
         self.logger = logger
 
     def run(self):
+        epochCountsc={}
         if self.numStreamDevices > 1:
             tempdatatrain = {}
             tempdatatest = {}
         while not self.closeEvent.is_set():
             if self.trainTestEvent.is_set(): # We're training!
                 if self.featureQueueTrain.empty():
-                    if len(self.epochCountsc) > 1: # check if there is more then one test condition
-                        minNumKeyEpochs = min([self.epochCountsc[key][1] for key in self.epochCountsc]) # check minimum viable number of training eochs have been obtained
+                    if len(epochCountsc) > 1: # check if there is more then one test condition
+                        minNumKeyEpochs = min([epochCountsc[key][1] for key in epochCountsc]) # check minimum viable number of training eochs have been obtained
                         if minNumKeyEpochs < self.minRequiredEpochs:
                             pass
                         else: 
                             start = time.time()
                             self.classifier.TrainModel(self.features, self.targets)
                             if (self.logger.level == Logger.TIMING):
                                 end = time.time()
                                 self.logger.log(Logger.TIMING, f" classifier training time {end - start}")
                     if self.classifierGuessMarkerEvent.is_set():
                         self.classifierGuessMarkerQueue.put(self.guess)
                 else:
                     try:
-                        featuresSingle, devCount, target, self.epochCountsc = self.featureQueueTrain.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
-                        
+                        featuresSingle, devCount, target, epochCountsc = self.featureQueueTrain.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
                         if self.numStreamDevices > 1: # Collects multiple data strems feature sets and synchronise here
                             tempdatatrain[devCount] = featuresSingle
                             if len(tempdatatrain) == self.numStreamDevices:
-                                flattened_list = [item for sublist in tempdatatrain.values() for item in sublist]
+                                flattened_list = np.array([item for sublist in tempdatatrain.values() for item in sublist])
                                 tempdatatrain = {}
                                 self.targets = np.append(self.targets, [target], axis = 0)
-                                self.features = np.append(self.features, [flattened_list], axis = 0)
+                                #self.features = np.append(self.features, [flattened_list], axis = 0)
+                                if self.features.shape[0] == 0:
+                                    self.features = self.features.reshape((0,) + flattened_list.shape)
+                                self.features = np.append(self.features, [flattened_list], axis=0)
                             # need to check if all device data is captured, then flatten and append  
                         else: # Only one device to collect from
                             if self.features.shape[0] == 0:
                                 self.features = self.features.reshape((0,) + featuresSingle.shape)
                             self.targets = np.append(self.targets, [target], axis = 0)
                             self.features = np.append(self.features, [featuresSingle], axis = 0)
                     except queue.Empty:
@@ -70,25 +73,23 @@
             else: # We're testing!
                 try:
                     featuresSingle, devCount = self.featureQueueTest.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
                     if self.numStreamDevices > 1:
                         tempdatatest[devCount] = featuresSingle
                         if len(tempdatatest) == self.numStreamDevices:
                             flattened_list = []
-                            for value in tempdatatest.values():
-                                flattened_list.extend(value)
+                            flattened_list = np.array([item for sublist in tempdatatest.values() for item in sublist])
                             tempdatatest = {}
                             start = time.time()
                             self.guess = self.classifier.TestModel(flattened_list)
                             if (self.logger.level == Logger.TIMING):
                                 end = time.time()
                                 self.logger.log(Logger.TIMING, f" classifier testing time {end - start}")
                     else:
                         start = time.time()
-                        #print(featuresSingle)
                         self.guess = self.classifier.TestModel(featuresSingle)
                         if (self.logger.level == Logger.TIMING):
                             end = time.time()
                             self.logger.log(Logger.TIMING, f" classifier testing time {end - start}")
                     if self.classifierGuessMarkerEvent.is_set():
                         self.classifierGuessMarkerQueue.put(self.guess)
                 except queue.Empty:
```

### Comparing `install-pybci-0.2.4b2/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-1.0.0/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-1.0.0/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import threading, queue, time
 from ..Utils.FeatureExtractor import GenericFeatureExtractor
 from ..Utils.Logger import Logger
 from ..Configuration.EpochSettings import GlobalEpochSettings
+import copy
+
 class FeatureProcessorThread(threading.Thread):
     tempDeviceEpochLogger = []
     def __init__(self, closeEvent, trainTestEvent, dataQueueTrain,dataQueueTest,
                 featureQueueTest,featureQueueTrain,  totalDevices,markerCountRetrieveEvent,markerCountQueue, customEpochSettings = {}, 
                 globalEpochSettings = GlobalEpochSettings(),logger = Logger(Logger.INFO), 
                 featureExtractor = GenericFeatureExtractor()):
         super().__init__()
@@ -40,15 +42,15 @@
                     start = time.time()
                     features = self.featureExtractor.ProcessFeatures(dataFIFOs, sr, target) # allows custom epoch class to be passed
                     if (self.logger.level == Logger.TIMING):
                         end = time.time()
                         self.logger.log(Logger.TIMING, f" Feature Extraction time {end - start}")
                         if (end-start) >self.globalWindowSettings.windowLength:
                             self.logger.log(Logger.WARNING, f" Feature Extraction time > globalEpochSetting.windowLength, will create lag in classification output. Recommended to reduce channels, smapling rate, and features or reduce feature computational complexity.")
-                    self.featureQueueTrain.put( [features, devCount, target, self.epochCounts] )
+                    self.featureQueueTrain.put( [features, devCount, target, dict(self.epochCounts)] )
                 except queue.Empty:
                     pass
             else:
                 try:
                     dataFIFOs, sr, devCount = self.dataQueueTest.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, ]
                     start = time.time()
                     features = self.featureExtractor.ProcessFeatures(dataFIFOs, sr, None)
```

### Comparing `install-pybci-0.2.4b2/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-1.0.0/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/ThreadClasses/OptimisedDataReceiverThread.py` & `install-pybci-1.0.0/pybci/ThreadClasses/OptimisedDataReceiverThread.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         self.dataQueueTrain = dataQueueTrain
         self.dataQueueTest = dataQueueTest
         self.dataStreamInlet = dataStreamInlet
         self.customEpochSettings = customEpochSettings
         self.globalEpochSettings = globalEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.sr = maxExpectedSampleRate
-        #self.dataType = dataStreamInlet.info().type()
         self.devCount = devCount # used for tracking which device is sending data to feature extractor
         
     def run(self):
         chCount = self.dataStreamInlet.info().channel_count()
         maxTime = (self.globalEpochSettings.tmin + self.globalEpochSettings.tmax)
         if len(self.customEpochSettings.keys()) > 0: # min time used for max_samples and temp array,  maxTime used for longest epochs and permanentDataBuffers
             if max([self.customEpochSettings[x].tmin + self.customEpochSettings[x].tmax for x in self.customEpochSettings]) > maxTime:
@@ -38,25 +37,21 @@
             window_overlap = self.globalEpochSettings.windowOverlap
         else:
             window_length = self.globalEpochSettings.tmin+self.globalEpochSettings.tmax
         minfifoLength = int(self.sr * window_length * (1-self.globalEpochSettings.windowOverlap)) #  sets global window length with overlap as factor for minimum delay in test mode
         dataBuffers = np.zeros((minfifoLength,chCount))
         chs_to_drop = np.ones(chCount, dtype=bool)
         chs_to_drop[self.streamChsDropDict] = False
-        #print(chs_to_drop)
         fifoLength = int(self.sr * (maxTime+20)) # adds twenty seconds to give more timestamps when buffering  (assuming devices dont timeout for longer then 20.0 seconds, migth be worth making configurable)
         permanentDataBuffers = np.zeros((fifoLength, chCount - len(self.streamChsDropDict)))
         permanentTimestampBuffer = np.zeros(fifoLength)
         next_window_time = 0 # sets testing mode window time, duration based on windowlength and overlap
         while not self.closeEvent.is_set():
             _, timestamps = self.dataStreamInlet.pull_chunk(timeout=0.0, max_samples=dataBuffers.shape[0], dest_obj=dataBuffers) # optimised method of getting data to pull_sample, dest_obj saves memory re-allocation
             if timestamps:
-                #print(timestamps)
-                #if self.markerReceived:
-                #    print(self.markerTimestamp)
                 if len(self.streamChsDropDict) == 0:
                     dataBufferView = dataBuffers[:len(timestamps), :] # [:, :len(timestamps)]
                 else:
                     dataBufferView = dataBuffers[:len(timestamps), chs_to_drop] # [:, :len(timestamps)]
                 permanentDataBuffers = np.roll(permanentDataBuffers, shift=-len(timestamps), axis=0)
                 permanentTimestampBuffer = np.roll(permanentTimestampBuffer, shift=-len(timestamps))
                 permanentDataBuffers[-len(timestamps):,:] = dataBufferView
```

### Comparing `install-pybci-0.2.4b2/pybci/Utils/Classifier.py` & `install-pybci-1.0.0/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/Utils/FeatureExtractor.py` & `install-pybci-1.0.0/pybci/Utils/FeatureExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,24 @@
                 l += 1
                 features[(ch* self.numFeatures)+l] = np.sqrt(np.mean(np.array(epoch[:,ch])**2))
             if self.featureChoices.variance: # variance
                 l += 1    
                 features[(ch* self.numFeatures)+l] =  np.var(epoch[:,ch])
             if self.featureChoices.meanAbs: # Mean Absolute Value 
                 l += 1
-                features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c) for c in epoch[:,ch]])/len(epoch[:,ch])
+                try:
+                    features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c) for c in epoch[:,ch]])/len(epoch[:,ch])
+                except:
+                    features[(ch* self.numFeatures)+l] = 0
             if self.featureChoices.waveformLength: # waveformLength
                 l += 1
-                features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c-epoch[inum,ch]) for inum, c in enumerate(epoch[1:,ch])])
+                try:    
+                    features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c-epoch[inum,ch]) for inum, c in enumerate(epoch[1:,ch])])
+                except:
+                    features[(ch* self.numFeatures)+l] = 0
             if self.featureChoices.zeroCross: # zeroCross
                 l += 1
                 features[(ch* self.numFeatures)+l] = sum([1 if c*epoch[inum+1,ch]<0 else 0 for inum, c in enumerate(epoch[:-1,ch])])
             if self.featureChoices.slopeSignChange: # slopeSignChange
                 l += 1    
                 ssc = sum([1 if (c-epoch[inum+1,ch])*(c-epoch[inum+1,ch])>=0.1 else 0 for inum, c in enumerate(epoch[:-1,ch])])
                 features[(ch* self.numFeatures)+l] = ssc
```

### Comparing `install-pybci-0.2.4b2/pybci/Utils/LSLScanner.py` & `install-pybci-1.0.0/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/Utils/Logger.py` & `install-pybci-1.0.0/pybci/Utils/Logger.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b2/pybci/pybci.py` & `install-pybci-1.0.0/pybci/pybci.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,30 +228,32 @@
             #    if stream.info().name() in self.streamChsDropDict.keys():
             #        dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
             #                                self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
             #    else:
             #        dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
             #                                self.globalEpochSettings, len(self.dataThreads))
             #else: # cold be desirable to capture samples only relative to timestammps with async, so maybe make this configurable?
-            if stream.info().nominal_srate() == 0:
-                if stream.info().name() in self.streamChsDropDict.keys(): ## all use optimised now (pull_chunk and timestamp relative)
-                    #print(self.streamChsDropDict[stream.info().name()])
-                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
-                else:
-                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads))
+            #if stream.info().nominal_srate() == 0:
+            print(len(self.dataThreads))
+            print(stream.info().name())
+            if stream.info().name() in self.streamChsDropDict.keys(): ## all use optimised now (pull_chunk and timestamp relative)
+                #print(self.streamChsDropDict[stream.info().name()])
+                dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+                                        self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
             else:
-                if stream.info().name() in self.streamChsDropDict.keys(): ## all use optimised now (pull_chunk and timestamp relative)
-                    #print(self.streamChsDropDict[stream.info().name()])
-                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()], maxExpectedSampleRate = stream.info().nominal_srate())
-                else:
-                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads),maxExpectedSampleRate = stream.info().nominal_srate())
+                dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+                                        self.globalEpochSettings, len(self.dataThreads))
+            #else:
+            #    if stream.info().name() in self.streamChsDropDict.keys(): ## all use optimised now (pull_chunk and timestamp relative)
+            #        #print(self.streamChsDropDict[stream.info().name()])
+            #        dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+            #                                self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()], maxExpectedSampleRate = stream.info().nominal_srate())
+            #    else:
+            #        dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+            #                                self.globalEpochSettings, len(self.dataThreads),maxExpectedSampleRate = stream.info().nominal_srate())
             dt.start()
             self.dataThreads.append(dt)
             if stream.info().name() in self.streamCustomFeatureExtract.keys():
                 self.ft = FeatureProcessorThread(self.closeEvent,self.trainTestEvent, self.dataQueueTrain, self.dataQueueTest,
                                                 self.featureQueueTest,self.featureQueueTrain, len(self.dataStreams),
                                                 self.markerCountRetrieveEvent, self.markerCountQueue,logger=self.logger,
                                                 featureExtractor = self.streamCustomFeatureExtract[stream.info().name()],
```

### Comparing `install-pybci-0.2.4b2/setup.py` & `install-pybci-1.0.0/setup.py`

 * *Files identical despite different names*

