# Comparing `tmp/idun_data_models-0.1.2.tar.gz` & `tmp/idun_data_models-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_data_models-0.1.2.tar", max compression
+gzip compressed data, was "idun_data_models-0.2.0.tar", max compression
```

## Comparing `idun_data_models-0.1.2.tar` & `idun_data_models-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      167 2023-05-25 12:59:05.212909 idun_data_models-0.1.2/README.md
--rw-r--r--   0        0        0      194 2023-05-25 12:59:05.212909 idun_data_models-0.1.2/idun_data_models/__init__.py
--rw-r--r--   0        0        0     2430 2023-05-25 12:59:05.212909 idun_data_models-0.1.2/idun_data_models/api_data_model.py
--rw-r--r--   0        0        0      823 2023-05-25 12:59:05.212909 idun_data_models-0.1.2/idun_data_models/device.py
--rw-r--r--   0        0        0       19 2023-05-25 12:59:05.212909 idun_data_models-0.1.2/idun_data_models/parameters.py
--rw-r--r--   0        0        0        0 2023-05-25 12:59:05.212909 idun_data_models-0.1.2/idun_data_models/py.typed
--rw-r--r--   0        0        0      583 2023-05-25 12:59:05.212909 idun_data_models-0.1.2/idun_data_models/serialization.py
--rw-r--r--   0        0        0      498 2023-05-25 12:59:05.216909 idun_data_models-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 idun_data_models-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      167 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/README.md
+-rw-r--r--   0        0        0      448 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/idun_data_models/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/idun_data_models/device.py
+-rw-r--r--   0        0        0      119 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/idun_data_models/parameters.py
+-rw-r--r--   0        0        0        0 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/idun_data_models/py.typed
+-rw-r--r--   0        0        0     3048 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/idun_data_models/rest_data_model.py
+-rw-r--r--   0        0        0      583 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/idun_data_models/serialization.py
+-rw-r--r--   0        0        0     1114 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/idun_data_models/websocket_data_model.py
+-rw-r--r--   0        0        0      495 2023-06-27 18:02:02.512924 idun_data_models-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 idun_data_models-0.2.0/PKG-INFO
```

### Comparing `idun_data_models-0.1.2/idun_data_models/api_data_model.py` & `idun_data_models-0.2.0/idun_data_models/rest_data_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,100 @@
 """
 This module defines data classes that are used by the IDUN Data API, defined with Pydantic.
 """
 
+from enum import Enum
 from datetime import datetime
-from pydantic import root_validator, validator
-from pydantic.dataclasses import dataclass
+from pydantic import BaseModel, root_validator, validator
 from .parameters import MAX_ID_LENGTH
 
 
-@dataclass(frozen=True)
-class Message:
-    """
-    A Message encapsulates encrypted device packets with metadata.
-    The IDUN SDK sends Messages with device data to the IDUN Cloud through the websocket API.
-    """
-    recordingID: str
-    deviceID: str
-    deviceTimestamp: datetime
-    connectionID: str | None = None
-    payload: str | None = None
-    impedance: float | None = None
-
-    # DEPRECATED: these fields will be replaced by explicit API calls
-    stop: bool | None = None
-    "Signal that the frontend sends to stop the recording"
-    recorded: bool | None = None
-    "Signal that the recorder sends to signal that batch processing is complete"
-    enableStreamer: bool | None = None
-    "Signal that the frontend can send to disable live streaming"
-
-    @validator("recordingID", "deviceID", "connectionID")
-    def limit_length(cls, v, field):
-        if v and len(v) > MAX_ID_LENGTH:
-            raise ValueError(f"{field} is too long. Max length: {MAX_ID_LENGTH}")
-        return v
-
-
-@dataclass(frozen=True)
-class DataStreams:
+class DataStreams(BaseModel):
     "Real time data streams available to return to the client"
 
-    bandpass_eeg: bool= False
+    bandpass_eeg: bool = False
     "Enables a stream of bandpass filtered EEG signal"
     # The following options are not yet supported
-    #raw_eeg: bool = False
-    #spectrogram: bool= False
+    # raw_eeg: bool = False
+    # spectrogram: bool= False
 
     @root_validator
     def validate_streaming_modes(cls, values):
         "Forbid invalid streaming mode selection"
         return values
 
-@dataclass(frozen=True)
-class GuardianRecording:
+
+class RecordingConfig(BaseModel):
+    data_stream_subscription: DataStreams | None = None
+    "Subscribe to real time data streams. No data stream by default."
+
+
+class recordingstatus(str, Enum):
+    NOT_STARTED = "NOT_STARTED"
+    ONGOING = "ONGOING"
+    PROCESSING = "PROCESSING"
+    COMPLETED = "COMPLETED"
+    FAILED = "FAILED"
+
+
+class _RecordingStatus(BaseModel):
+    stopped: bool
+    "Is the recording still receiving data?"
+
+
+class RecordingStatusIn(_RecordingStatus):
+    pass
+
+
+class RecordingStatusOut(_RecordingStatus):
+    status: recordingstatus | None = None
+    message: str | None = None
+    "Explanation about the current status"
+    startDeviceTimestamp: datetime | None = None
+    """Device timestamp of the first message in the recording.
+    It is provided by the client, so it can be unreliable for BI purposes.
+    """
+    stopDeviceTimestamp: datetime | None = None
+    """Device timestamp of the last message in the recording.
+    It is provided by the client, so it can be unreliable for BI purposes.
     """
-    A GuardianRecording is a contiguous data capture session of the IDUN Guardian through a specific frontend client.
-    It is part of the IDUN REST API.
+    createdAt: datetime | None = None
+    """Local timestamp of the API at the moment that this recording was created.
     """
+    stoppedAt: datetime | None = None
+    """Local timestamp of the API at the moment that this recording was stopped.
+    """
+
 
+class _Recording(BaseModel):
     recordingID: str
     deviceID: str
     displayName: str
     "User-friendly name used in the UI"
 
-    # Configuration options (should be optional)
-    data_stream_subscription: DataStreams | None = None
-    "Subscribe to real time data streams. No data stream by default."
-
     @validator("recordingID", "deviceID", "displayName")
     def limit_length(cls, v, field):
+        # TODO: validate ID regex
         if len(v) > MAX_ID_LENGTH:
             raise ValueError(f"{field} is too long. Max length: {MAX_ID_LENGTH}")
         return v
+
+
+class RecordingIn(_Recording):
+    """
+    RecordingIn can be used to create/update recordings in the IDUN REST API.
+    A Recording is a contiguous data capture session of the IDUN Guardian through a specific frontend client.
+    """
+
+    config: RecordingConfig | None = None
+
+
+class RecordingOut(_Recording):
+    """
+    RecordingOut is returned by the IDUN REST API to describe existing recordings.
+    A Recording is a contiguous data capture session of the IDUN Guardian through a specific frontend client.
+    """
+
+    status: RecordingStatusOut
+    config: RecordingConfig | None = None
+    cursor: str | None = None
+    "Continue fetching objects from this point onward"
```

### Comparing `idun_data_models-0.1.2/idun_data_models/device.py` & `idun_data_models-0.2.0/idun_data_models/device.py`

 * *Files identical despite different names*

### Comparing `idun_data_models-0.1.2/idun_data_models/serialization.py` & `idun_data_models-0.2.0/idun_data_models/serialization.py`

 * *Files identical despite different names*

### Comparing `idun_data_models-0.1.2/PKG-INFO` & `idun_data_models-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun-data-models
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Author: Konstantinos Samaras-Tsakiris
 Author-email: konstantinos@iduntechnologies.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

