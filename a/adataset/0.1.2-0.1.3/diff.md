# Comparing `tmp/adataset-0.1.2.tar.gz` & `tmp/adataset-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adataset-0.1.2.tar", last modified: Sat Jun 24 03:44:07 2023, max compression
+gzip compressed data, was "adataset-0.1.3.tar", last modified: Tue Jun 27 12:16:20 2023, max compression
```

## Comparing `adataset-0.1.2.tar` & `adataset-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.466546 adataset-0.1.2/
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-24 03:44:07.466371 adataset-0.1.2/PKG-INFO
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3875 2023-05-20 04:47:09.000000 adataset-0.1.2/README.md
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.440810 adataset-0.1.2/adataset/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/__init__.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.436638 adataset-0.1.2/adataset/calibration_meta/
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.442123 adataset-0.1.2/adataset/calibration_meta/camera_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      207 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/camera_params/camera_extrinsics.yaml
--rw-r--r--   0 wangfanghao   (502) staff       (20)      939 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/camera_params/camera_intrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.442797 adataset-0.1.2/adataset/calibration_meta/gnss_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      273 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/gnss_params/ant_imu_leverarm.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.443381 adataset-0.1.2/adataset/calibration_meta/radar_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      203 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/radar_params/radar_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.443968 adataset-0.1.2/adataset/calibration_meta/vehicle_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      115 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/vehicle_params/vehicle_imu_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.445358 adataset-0.1.2/adataset/calibration_meta/velodyne_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)       59 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/velodyne_params/lidar_height.yaml
--rw-r--r--   0 wangfanghao   (502) staff       (20)      214 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/velodyne_params/lidar_novatel_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.453576 adataset-0.1.2/adataset/kitti/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/__init__.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)    12153 2023-06-10 11:44:42.000000 adataset-0.1.2/adataset/kitti/calibration_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1348 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/common.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3626 2023-06-24 03:19:09.000000 adataset-0.1.2/adataset/kitti/dataset_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 11:44:59.000000 adataset-0.1.2/adataset/kitti/geometry.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4198 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/kitti.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1892 2023-06-10 11:45:15.000000 adataset-0.1.2/adataset/kitti/params.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1397 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/pcd_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1579 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/proj_helper.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3861 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/sensor.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4051 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/main.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.458943 adataset-0.1.2/adataset/nuscenes/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/nuscenes/__init__.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)    12194 2023-06-10 11:48:19.000000 adataset-0.1.2/adataset/nuscenes/calibration_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3880 2023-06-24 03:19:48.000000 adataset-0.1.2/adataset/nuscenes/dataset_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 10:39:20.000000 adataset-0.1.2/adataset/nuscenes/geometry.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     6886 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/nuscenes/nuscenes.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     2363 2023-06-10 11:09:08.000000 adataset-0.1.2/adataset/nuscenes/params.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1444 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/nuscenes/pcd_converter.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.466094 adataset-0.1.2/adataset.egg-info/
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/PKG-INFO
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1276 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/SOURCES.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)        1 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/dependency_links.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       48 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/entry_points.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       37 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/requires.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)        9 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/top_level.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       38 2023-06-24 03:44:07.466607 adataset-0.1.2/setup.cfg
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1353 2023-06-24 03:43:46.000000 adataset-0.1.2/setup.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.316887 adataset-0.1.3/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-27 12:16:20.316723 adataset-0.1.3/PKG-INFO
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3875 2023-06-25 02:51:22.000000 adataset-0.1.3/README.md
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.299993 adataset-0.1.3/adataset/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/__init__.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.296281 adataset-0.1.3/adataset/calibration_meta/
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.300695 adataset-0.1.3/adataset/calibration_meta/camera_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      207 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/calibration_meta/camera_params/camera_extrinsics.yaml
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      939 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/calibration_meta/camera_params/camera_intrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.301158 adataset-0.1.3/adataset/calibration_meta/gnss_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      273 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/calibration_meta/gnss_params/ant_imu_leverarm.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.301578 adataset-0.1.3/adataset/calibration_meta/radar_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      203 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/calibration_meta/radar_params/radar_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.301969 adataset-0.1.3/adataset/calibration_meta/vehicle_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      115 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/calibration_meta/vehicle_params/vehicle_imu_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.302857 adataset-0.1.3/adataset/calibration_meta/velodyne_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       59 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/calibration_meta/velodyne_params/lidar_height.yaml
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      214 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/calibration_meta/velodyne_params/lidar_novatel_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.308031 adataset-0.1.3/adataset/kitti/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/kitti/__init__.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)    12783 2023-06-27 11:43:27.000000 adataset-0.1.3/adataset/kitti/calibration_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1348 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/kitti/common.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3607 2023-06-27 11:01:32.000000 adataset-0.1.3/adataset/kitti/dataset_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-25 10:52:15.000000 adataset-0.1.3/adataset/kitti/geometry.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4198 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/kitti/kitti.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1895 2023-06-27 01:08:17.000000 adataset-0.1.3/adataset/kitti/params.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1397 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/kitti/pcd_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1579 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/kitti/proj_helper.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3861 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/kitti/sensor.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4051 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/main.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.311841 adataset-0.1.3/adataset/nuscenes/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/nuscenes/__init__.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)    12984 2023-06-27 12:10:43.000000 adataset-0.1.3/adataset/nuscenes/calibration_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3830 2023-06-27 11:11:00.000000 adataset-0.1.3/adataset/nuscenes/dataset_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-25 10:52:15.000000 adataset-0.1.3/adataset/nuscenes/geometry.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     6886 2023-06-27 06:53:43.000000 adataset-0.1.3/adataset/nuscenes/nuscenes.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     2334 2023-06-27 11:13:02.000000 adataset-0.1.3/adataset/nuscenes/params.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1444 2023-06-25 02:51:22.000000 adataset-0.1.3/adataset/nuscenes/pcd_converter.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-27 12:16:20.316484 adataset-0.1.3/adataset.egg-info/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-27 12:16:19.000000 adataset-0.1.3/adataset.egg-info/PKG-INFO
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1276 2023-06-27 12:16:20.000000 adataset-0.1.3/adataset.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        1 2023-06-27 12:16:19.000000 adataset-0.1.3/adataset.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       48 2023-06-27 12:16:20.000000 adataset-0.1.3/adataset.egg-info/entry_points.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       37 2023-06-27 12:16:20.000000 adataset-0.1.3/adataset.egg-info/requires.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        9 2023-06-27 12:16:20.000000 adataset-0.1.3/adataset.egg-info/top_level.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       38 2023-06-27 12:16:20.316945 adataset-0.1.3/setup.cfg
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1353 2023-06-27 11:44:10.000000 adataset-0.1.3/setup.py
```

### Comparing `adataset-0.1.2/PKG-INFO` & `adataset-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adataset
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dataset conversion to Apollo record tool
 Home-page: https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset
 Author: apollo-team
 Author-email: apollo-support@baidu.com
 Project-URL: Bug Tracker, https://github.com/ApolloAuto/apollo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `adataset-0.1.2/README.md` & `adataset-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/calibration_meta/camera_params/camera_intrinsics.yaml` & `adataset-0.1.3/adataset/calibration_meta/camera_params/camera_intrinsics.yaml`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/kitti/calibration_converter.py` & `adataset-0.1.3/adataset/kitti/calibration_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,19 +47,18 @@
 
 # Frame ID
 CAMERA_FRAME_ID = 'velodyne64'
 RADAR_FRAME_ID = 'novatel'
 LIDAR_FRAME_ID = 'novatel'
 
 
-def _matrix_padding4x4(r_array):
-  transform = np.empty((4, 4))
-  transform[:3,:3] = r_array.reshape((3, 3))
-  transform[:3, 3] = [0, 0, 0]
-  transform[3, :]  = [0, 0, 0, 1]
+def _construct_transform(rotation, translation):
+  transform = np.identity(4)
+  transform[:3, :3] = rotation
+  transform[:3, 3] = translation
   return transform
 
 def load_yaml(file_path):
   """Read content from yaml
 
   Args:
       file_path (str): yaml file
@@ -81,37 +80,38 @@
       file_path (src): file path
       content (dict): yaml object
   """
   with open(file_path, 'w') as f:
     yaml.safe_dump(content, f, sort_keys=False)
 
 
-def gen_camera_extrinsics(camera_name, calibrated_sensor, calibration_file_path):
+def gen_camera_extrinsics(child_frame_id, frame_id, calibrated_sensor,
+        calibration_file_path):
   """Generate camera extrinsic and intrinsic file
 
   Args:
       camera_name (str): camera name
       calibrated_sensor (_type_): kitti calibrated_sensor json object
       calibration_file_path (str): saved path
   """
   # 1. Generate extrinsics
   camera_meta_extrinsics = os.path.join(
     CALIBRATION_META_ROOT, CAMERA_PARAMS_PATH, CAMERA_EXTRINSICS)
   camera_extrinsics = load_yaml(camera_meta_extrinsics)
-  camera_extrinsics['header']['frame_id'] = CAMERA_FRAME_ID
-  camera_extrinsics['child_frame_id'] = camera_name
+  camera_extrinsics['header']['frame_id'] = frame_id
+  camera_extrinsics['child_frame_id'] = child_frame_id
   camera_extrinsics['transform']['translation']['x'] = calibrated_sensor['translation'][0]
   camera_extrinsics['transform']['translation']['y'] = calibrated_sensor['translation'][1]
   camera_extrinsics['transform']['translation']['z'] = calibrated_sensor['translation'][2]
   camera_extrinsics['transform']['rotation']['w'] = calibrated_sensor['rotation'][0]
   camera_extrinsics['transform']['rotation']['x'] = calibrated_sensor['rotation'][1]
   camera_extrinsics['transform']['rotation']['y'] = calibrated_sensor['rotation'][2]
   camera_extrinsics['transform']['rotation']['z'] = calibrated_sensor['rotation'][3]
 
-  file_name = CAMERA_EXTRINSICS.replace('camera', camera_name)
+  file_name = CAMERA_EXTRINSICS.replace('camera', child_frame_id)
   file_path = os.path.join(calibration_file_path, CAMERA_PARAMS_PATH)
   Path(file_path).mkdir(parents=True, exist_ok=True)
 
   camera_extrinsics_file = os.path.join(file_path, file_name)
   save_yaml(camera_extrinsics_file, camera_extrinsics)
 
 
@@ -141,94 +141,100 @@
 
   file_name = CAMERA_INTRINSICS.replace('camera', camera_name)
   file_path = os.path.join(calibration_file_path, CAMERA_PARAMS_PATH)
   camera_intrinsics_file = os.path.join(file_path, file_name)
   save_yaml(camera_intrinsics_file, camera_intrinsics)
 
 
-def gen_radar_params(radar_name, calibrated_sensor, calibration_file_path):
+def gen_radar_params(child_frame_id, frame_id, calibrated_sensor,
+      calibration_file_path):
   """Generate radar extrinsic file
 
   Args:
       radar_name (str): radar name
       calibrated_sensor (_type_): kitti calibrated_sensor json object
       calibration_file_path (_type_): saved path
   """
   radar_meta_extrinsics = os.path.join(
     CALIBRATION_META_ROOT, RADAR_PARAMS_PATH, RADAR_EXTRINSICS)
   radar_extrinsics = load_yaml(radar_meta_extrinsics)
-  radar_extrinsics['header']['frame_id'] = RADAR_FRAME_ID
-  radar_extrinsics['child_frame_id'] = radar_name
+  radar_extrinsics['header']['frame_id'] = frame_id
+  radar_extrinsics['child_frame_id'] = child_frame_id
   radar_extrinsics['transform']['translation']['x'] = calibrated_sensor['translation'][0]
   radar_extrinsics['transform']['translation']['y'] = calibrated_sensor['translation'][1]
   radar_extrinsics['transform']['translation']['z'] = calibrated_sensor['translation'][2]
   radar_extrinsics['transform']['rotation']['w'] = calibrated_sensor['rotation'][0]
   radar_extrinsics['transform']['rotation']['x'] = calibrated_sensor['rotation'][1]
   radar_extrinsics['transform']['rotation']['y'] = calibrated_sensor['rotation'][2]
   radar_extrinsics['transform']['rotation']['z'] = calibrated_sensor['rotation'][3]
 
-  file_name = RADAR_EXTRINSICS.replace('radar', radar_name)
+  file_name = RADAR_EXTRINSICS.replace('radar', child_frame_id)
   file_path = os.path.join(calibration_file_path, RADAR_PARAMS_PATH)
   Path(file_path).mkdir(parents=True, exist_ok=True)
 
   radar_extrinsics_file = os.path.join(file_path, file_name)
   save_yaml(radar_extrinsics_file, radar_extrinsics)
 
 
-def gen_velodyne_params(lidar_name, calibrated_sensor, calibration_file_path):
+def gen_velodyne_params(child_frame_id, frame_id, calibrated_sensor,
+      calibration_file_path):
   """Generate lidar extrinsic file
 
   Args:
       lidar_name (str): lidar name
       calibrated_sensor (_type_): kitti calibrated_sensor json object
       calibration_file_path (str): saved path
   """
   lidar_meta_extrinsics = os.path.join(
     CALIBRATION_META_ROOT, VELODYNE_PARAMS_PATH, LIDAR_NOVATEL_EXTRINSICS)
   lidar_extrinsics = load_yaml(lidar_meta_extrinsics)
-  lidar_extrinsics['header']['frame_id'] = LIDAR_FRAME_ID
-  lidar_extrinsics['child_frame_id'] = lidar_name
+  lidar_extrinsics['header']['frame_id'] = frame_id
+  lidar_extrinsics['child_frame_id'] = child_frame_id
   lidar_extrinsics['transform']['translation']['x'] = calibrated_sensor['translation'][0]
   lidar_extrinsics['transform']['translation']['y'] = calibrated_sensor['translation'][1]
   lidar_extrinsics['transform']['translation']['z'] = calibrated_sensor['translation'][2]
   lidar_extrinsics['transform']['rotation']['w'] = calibrated_sensor['rotation'][0]
   lidar_extrinsics['transform']['rotation']['x'] = calibrated_sensor['rotation'][1]
   lidar_extrinsics['transform']['rotation']['y'] = calibrated_sensor['rotation'][2]
   lidar_extrinsics['transform']['rotation']['z'] = calibrated_sensor['rotation'][3]
 
-  file_name = LIDAR_NOVATEL_EXTRINSICS.replace('lidar', lidar_name)
+  file_name = LIDAR_NOVATEL_EXTRINSICS.replace('lidar', child_frame_id)
   file_path = os.path.join(calibration_file_path, VELODYNE_PARAMS_PATH)
   Path(file_path).mkdir(parents=True, exist_ok=True)
 
   lidar_novatel_extrinsics = os.path.join(file_path, file_name)
   save_yaml(lidar_novatel_extrinsics, lidar_extrinsics)
 
 
-def process_calib_imu_to_velo(dataset_path, calibration_file_path):
+def process_calib_velo_to_imu(dataset_path, calibration_file_path):
   absolute_path = os.path.join(dataset_path, 'calib_imu_to_velo.txt')
   calibrated_sensor = dict()
   with open(absolute_path, 'r') as f:
     lines = f.readlines()
+    # rotation 3x3 matrix
     r = lines[1].lstrip('R:').split()
-    r_array = np.array(r, dtype=np.float32)
+    rotation = np.array(r, dtype=np.float32).reshape((3, 3))
+    # translation 1x3 list
+    t = lines[2].lstrip('T:').split()
+    translation = np.array(t, dtype=np.float32).tolist()
+    imu2lidar = _construct_transform(rotation, translation)
     # Apollo coordinate system conversion
-    # k_imu * imu2lidar = k_lidar
-    # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
-    transform = _matrix_padding4x4(r_array)
-    imu_to_velo = apollo2kitti_imu @ transform @ kitti2apollo_lidar
-    r_array = imu_to_velo[:3,:3]
+    # imu2lidar * k_imu = k_lidar
+    # imu2lidar * apollo2k_imu * apollo_imu = apollo2k_lidar * apollo_lidar
+    imu_to_velo = kitti2apollo_lidar @ imu2lidar @ apollo2kitti_imu
+    velo_to_imu = np.linalg.inv(imu_to_velo)
 
-    roll, pitch, yaw = rotation_matrix_to_euler(r_array)
+    rotation = velo_to_imu[:3, :3]
+    roll, pitch, yaw = rotation_matrix_to_euler(rotation)
     q = Euler(roll, pitch, yaw).to_quaternion()
     calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+    calibrated_sensor['translation'] = velo_to_imu[:3, 3].tolist()
 
-    t = lines[2].lstrip('T:').split()
-    calibrated_sensor['translation'] = np.array(t, dtype=np.float32).tolist()
-
-  gen_velodyne_params('velodyne64', calibrated_sensor, calibration_file_path)
+  gen_velodyne_params('velodyne64', LIDAR_FRAME_ID, calibrated_sensor,
+      calibration_file_path)
 
 
 def process_calib_cam_to_cam(dataset_path, calibration_file_path):
   absolute_path = os.path.join(dataset_path, 'calib_cam_to_cam.txt')
 
   with open(absolute_path, 'r') as f:
     total_lines = f.readlines()
@@ -238,68 +244,77 @@
     lines = total_lines[i*8:(i+1)*8]
     calibrated_sensor = dict()
     s = lines[0][len('S_00:'):].strip().split()
     wh = np.array(s, dtype=np.float32).tolist()
     calibrated_sensor['width'] = wh[0]
     calibrated_sensor['height'] = wh[1]
 
-    k = lines[1][len('S_00:'):].strip().split()
+    k = lines[1][len('K_00:'):].strip().split()
     calibrated_sensor['K'] = np.array(k, dtype=np.float32).tolist()
 
-    d = lines[2][len('S_00:'):].strip().split()
+    d = lines[2][len('D_00:'):].strip().split()
     calibrated_sensor['D'] = np.array(d, dtype=np.float32).tolist()
 
-    r = lines[3][len('S_00:'):].strip().split()
-    r_array = np.array(r, dtype=np.float32)
     # Todo(zero): Need to generate cam to cam external parameters
+    # rotation
+    r = lines[3][len('R_00:'):].strip().split()
+    rotation = np.array(r, dtype=np.float32).reshape((3, 3))
+    # translation
+    t = lines[4][len('T_00:'):].strip().split()
+    translation = np.array(t, dtype=np.float32).tolist()
     # Apollo coordinate system conversion
-    # k_cam * cam2cam = k_cam
-    # apollo_camera * apollo2k_camera * cam2cam = apollo_camera * apollo2k_camera
-    transform = _matrix_padding4x4(r_array)
-    cam_to_cam = apollo2kitti_camera @ transform @ kitti2apollo_camera
-    r_array = cam_to_cam[:3,:3]
+    # cam2cam0 * k_cam1 = k_cam0
+    # cam2cam0 * apollo2k_camera1 * apollo_cam1 = apollo2k_camera0 * apollo_cam0
+    cam2cam0 = _construct_transform(rotation, translation)
+    cam_to_cam0 = kitti2apollo_camera @ cam2cam0 @ apollo2kitti_camera
 
-    roll, pitch, yaw = rotation_matrix_to_euler(r_array)
+    rotation = cam_to_cam0[:3, :3]
+    roll, pitch, yaw = rotation_matrix_to_euler(rotation)
     q = Euler(roll, pitch, yaw).to_quaternion()
     calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+    calibrated_sensor['translation'] = cam_to_cam0[:3, 3].tolist()
 
-    t = lines[4][len('S_00:'):].strip().split()
-    calibrated_sensor['translation'] = np.array(t, dtype=np.float32).tolist()
+    camera_name = 'camera_{:02d}'.format(i)
+    gen_camera_extrinsics(camera_name, 'camera_00', calibrated_sensor,
+        calibration_file_path)
 
     s_rect = lines[5][len('S_rect_01:'):].strip().split()
     s_rect_array = np.array(s_rect, dtype=np.float32).tolist()
     r_rect = lines[6][len('S_rect_01:'):].strip().split()
     r_rect_array = np.array(r_rect, dtype=np.float32).tolist()
     p_rect = lines[7][len('S_rect_01:'):].strip().split()
     p_rect_array = np.array(p_rect, dtype=np.float32).tolist()
 
-    camera_name = 'camera_{:02d}'.format(i)
     gen_camera_intrinsics(camera_name, calibrated_sensor, calibration_file_path)
 
 
-def process_calib_velo_to_cam(dataset_path, calibration_file_path):
+def process_calib_cam_to_velo(dataset_path, calibration_file_path):
   absolute_path = os.path.join(dataset_path, 'calib_velo_to_cam.txt')
   calibrated_sensor = dict()
   with open(absolute_path, 'r') as f:
     lines = f.readlines()
+    # rotation
     r = lines[1].lstrip('R:').split()
-    r_array = np.array(r, dtype=np.float32)
+    rotation = np.array(r, dtype=np.float32).reshape((3, 3))
+    # translation
+    t = lines[2].lstrip('T:').split()
+    translation = np.array(t, dtype=np.float32).tolist()
     # Apollo coordinate system conversion
-    # k_lidar * lidar2cam = k_camera
-    # apollo_lidar * apollo2k_lidar * lidar2cam = apollo_camera * apollo2k_camera
-    transform = _matrix_padding4x4(r_array)
-    velo_to_cam = apollo2kitti_lidar @ transform @ kitti2apollo_camera
-    r_array = velo_to_cam[:3,:3]
+    # velo2cam * k_lidar = k_camera
+    # velo2cam * apollo2k_lidar * apollo_lidar = apollo2k_camera * apollo_camera
+    velo2cam = _construct_transform(rotation, translation)
+    velo_to_cam = kitti2apollo_camera @ velo2cam @ apollo2kitti_lidar
+    cam_to_velo = np.linalg.inv(velo_to_cam)
 
-    roll, pitch, yaw = rotation_matrix_to_euler(r_array)
+    rotation = cam_to_velo[:3, :3]
+    roll, pitch, yaw = rotation_matrix_to_euler(rotation)
     q = Euler(roll, pitch, yaw).to_quaternion()
     calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+    calibrated_sensor['translation'] = cam_to_velo[:3, 3].tolist()
 
-    t = lines[2].lstrip('T:').split()
-    calibrated_sensor['translation'] = np.array(t, dtype=np.float32).tolist()
-
-  gen_camera_extrinsics('camera', calibrated_sensor, calibration_file_path)
+  gen_camera_extrinsics('camera', CAMERA_FRAME_ID, calibrated_sensor,
+      calibration_file_path)
 
 def convert_calibration(dataset_path, calibration_root_path):
-  process_calib_imu_to_velo(dataset_path, calibration_root_path)
-  process_calib_velo_to_cam(dataset_path, calibration_root_path)
+  process_calib_velo_to_imu(dataset_path, calibration_root_path)
+  process_calib_cam_to_velo(dataset_path, calibration_root_path)
   process_calib_cam_to_cam(dataset_path, calibration_root_path)
```

### Comparing `adataset-0.1.2/adataset/kitti/common.py` & `adataset-0.1.3/adataset/kitti/common.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/kitti/dataset_converter.py` & `adataset-0.1.3/adataset/kitti/dataset_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
   PointCloudBuilder,
   LocalizationBuilder,
   TransformBuilder)
 from adataset.kitti.kitti import KITTISchema, KITTI
 from adataset.kitti.geometry import Quaternion, Euler, rotation_matrix_to_euler
 from adataset.kitti.params import (
   kitti2apollo_lidar,
-  kitti2apollo_imu
 )
 
 
 LOCALIZATION_TOPIC = '/apollo/localization/pose'
 TF_TOPIC= '/tf'
```

### Comparing `adataset-0.1.2/adataset/kitti/geometry.py` & `adataset-0.1.3/adataset/kitti/geometry.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/kitti/kitti.py` & `adataset-0.1.3/adataset/kitti/kitti.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/kitti/params.py` & `adataset-0.1.3/adataset/kitti/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 apollo2kitti_lidar = np.array([[1.0000000, 0.0000000, 0.0000000, 0.0000000],
                                [0.0000000, 1.0000000, 0.0000000, 0.0000000],
                                [0.0000000, 0.0000000, 1.0000000, 0.0000000],
                                [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
 
 apollo2kitti_camera = np.array([[1.0000000, 0.0000000, 0.0000000, 0.0000000],
-                               [0.0000000, 1.0000000, 0.0000000, 0.0000000],
-                               [0.0000000, 0.0000000, 1.0000000, 0.0000000],
-                               [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
+                                [0.0000000, 1.0000000, 0.0000000, 0.0000000],
+                                [0.0000000, 0.0000000, 1.0000000, 0.0000000],
+                                [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
 
-apollo2kitti_imu = np.array([[0.0000000, -1.0000000, 0.0000000, 0.0000000],
-                             [1.0000000, 0.0000000, 0.0000000, 0.0000000],
+apollo2kitti_imu = np.array([[0.0000000, 1.0000000, 0.0000000, 0.0000000],
+                             [-1.0000000, 0.0000000, 0.0000000, 0.0000000],
                              [0.0000000, 0.0000000, 1.0000000, 0.0000000],
                              [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
 
 kitti2apollo_lidar = np.linalg.inv(apollo2kitti_lidar)
 kitti2apollo_camera = np.linalg.inv(apollo2kitti_camera)
 kitti2apollo_imu = np.linalg.inv(apollo2kitti_imu)
```

### Comparing `adataset-0.1.2/adataset/kitti/pcd_converter.py` & `adataset-0.1.3/adataset/kitti/pcd_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/kitti/proj_helper.py` & `adataset-0.1.3/adataset/kitti/proj_helper.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/kitti/sensor.py` & `adataset-0.1.3/adataset/kitti/sensor.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/main.py` & `adataset-0.1.3/adataset/main.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/nuscenes/calibration_converter.py` & `adataset-0.1.3/adataset/nuscenes/calibration_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,30 +18,28 @@
 '''Generate apollo calibration files by nuscenes calibration data.'''
 
 import os
 import yaml
 import pkgutil
 import numpy as np
 
-from itertools import chain
 from pathlib import Path
 
 from adataset.nuscenes.nuscenes import NuScenesSchema, NuScenesHelper, NuScenes
 from adataset.nuscenes.geometry import (
   Euler,
   Quaternion,
   euler_to_rotation_matrix,
   rotation_matrix_to_euler
 )
 from adataset.nuscenes.params import (
   apollo2nuscenes_lidar,
-  apollo2nuscenes_imu,
-  nuscenes2apollo_camera,
-  nuscenes2apollo_lidar,
-  nuscenes2apollo_radar,
+  apollo2nuscenes_camera,
+  nuscenes2apollo_imu,
+  apollo2nuscenes_radar,
 )
 
 CALIBRATION_META_ROOT = 'calibration_meta'
 # Lidar meta
 VELODYNE_PARAMS_PATH = 'velodyne_params'
 LIDAR_NOVATEL_EXTRINSICS = 'lidar_novatel_extrinsics.yaml'
 # Camera meta
@@ -53,19 +51,19 @@
 RADAR_EXTRINSICS = 'radar_extrinsics.yaml'
 
 # Frame ID
 CAMERA_FRAME_ID = 'novatel'
 RADAR_FRAME_ID = 'novatel'
 LIDAR_FRAME_ID = 'novatel'
 
-def _construct_transform(r, t):
-  transform = np.empty((4, 4))
-  transform[:3,:3] = r
-  transform[:3, 3] = t
-  transform[3, :]  = [0, 0, 0, 1]
+
+def _construct_transform(rotation, translation):
+  transform = np.identity(4)
+  transform[:3, :3] = rotation
+  transform[:3, 3] = translation
   return transform
 
 def load_yaml(file_path):
   """Read content from yaml
 
   Args:
       file_path (str): yaml file
@@ -87,193 +85,215 @@
       file_path (src): file path
       content (dict): yaml object
   """
   with open(file_path, 'w') as f:
     yaml.safe_dump(content, f, sort_keys=False)
 
 
-def gen_camera_params(camera_name, calibrated_sensor, calibration_file_path):
+def gen_camera_extrinsics(child_frame_id, frame_id, calibrated_sensor,
+        calibration_file_path):
   """Generate camera extrinsic and intrinsic file
 
   Args:
       camera_name (str): camera name
-      calibrated_sensor (_type_): nuscenes calibrated_sensor json object
+      calibrated_sensor (_type_): kitti calibrated_sensor json object
       calibration_file_path (str): saved path
   """
   # 1. Generate extrinsics
   camera_meta_extrinsics = os.path.join(
     CALIBRATION_META_ROOT, CAMERA_PARAMS_PATH, CAMERA_EXTRINSICS)
   camera_extrinsics = load_yaml(camera_meta_extrinsics)
-  camera_extrinsics['header']['frame_id'] = CAMERA_FRAME_ID
-  camera_extrinsics['child_frame_id'] = camera_name
+  camera_extrinsics['header']['frame_id'] = frame_id
+  camera_extrinsics['child_frame_id'] = child_frame_id
   camera_extrinsics['transform']['translation']['x'] = calibrated_sensor['translation'][0]
   camera_extrinsics['transform']['translation']['y'] = calibrated_sensor['translation'][1]
   camera_extrinsics['transform']['translation']['z'] = calibrated_sensor['translation'][2]
   camera_extrinsics['transform']['rotation']['w'] = calibrated_sensor['rotation'][0]
   camera_extrinsics['transform']['rotation']['x'] = calibrated_sensor['rotation'][1]
   camera_extrinsics['transform']['rotation']['y'] = calibrated_sensor['rotation'][2]
   camera_extrinsics['transform']['rotation']['z'] = calibrated_sensor['rotation'][3]
 
-  file_name = CAMERA_EXTRINSICS.replace('camera', camera_name)
+  file_name = CAMERA_EXTRINSICS.replace('camera', child_frame_id)
   file_path = os.path.join(calibration_file_path, CAMERA_PARAMS_PATH)
   Path(file_path).mkdir(parents=True, exist_ok=True)
 
   camera_extrinsics_file = os.path.join(file_path, file_name)
   save_yaml(camera_extrinsics_file, camera_extrinsics)
 
+
+def gen_camera_intrinsics(camera_name, calibrated_sensor, calibration_file_path):
+  """Generate camera extrinsic and intrinsic file
+
+  Args:
+      camera_name (str): camera name
+      calibrated_sensor (_type_): kitti calibrated_sensor json object
+      calibration_file_path (str): saved path
+  """
   # 2. Generate intrinsics
   camera_meta_intrinsics = os.path.join(
     CALIBRATION_META_ROOT, CAMERA_PARAMS_PATH, CAMERA_INTRINSICS)
   camera_intrinsics = load_yaml(camera_meta_intrinsics)
 
-  raw_camera_intrinsic = calibrated_sensor['camera_intrinsic']
   camera_intrinsics['header']['frame_id'] = CAMERA_FRAME_ID
-  camera_intrinsics['K'] = list(chain.from_iterable(raw_camera_intrinsic))
+  if 'height' in calibrated_sensor:
+    camera_intrinsics['height'] = calibrated_sensor['height']
+  if 'width' in calibrated_sensor:
+    camera_intrinsics['width'] = calibrated_sensor['width']
 
-  # Todo(zero): need to complete
-  # camera_intrinsics['D'] =
+  camera_intrinsics['K'] = list(calibrated_sensor['K'])
+  # camera_intrinsics['D'] = list(calibrated_sensor['D'])
   # camera_intrinsics['R'] =
   # camera_intrinsics['P'] =
 
   file_name = CAMERA_INTRINSICS.replace('camera', camera_name)
+  file_path = os.path.join(calibration_file_path, CAMERA_PARAMS_PATH)
   camera_intrinsics_file = os.path.join(file_path, file_name)
   save_yaml(camera_intrinsics_file, camera_intrinsics)
 
 
-def gen_radar_params(radar_name, calibrated_sensor, calibration_file_path):
+def gen_radar_params(child_frame_id, frame_id, calibrated_sensor,
+        calibration_file_path):
   """Generate radar extrinsic file
 
   Args:
       radar_name (str): radar name
       calibrated_sensor (_type_): nuscenes calibrated_sensor json object
       calibration_file_path (_type_): saved path
   """
   radar_meta_extrinsics = os.path.join(
     CALIBRATION_META_ROOT, RADAR_PARAMS_PATH, RADAR_EXTRINSICS)
   radar_extrinsics = load_yaml(radar_meta_extrinsics)
-  radar_extrinsics['header']['frame_id'] = RADAR_FRAME_ID
-  radar_extrinsics['child_frame_id'] = radar_name
+  radar_extrinsics['header']['frame_id'] = frame_id
+  radar_extrinsics['child_frame_id'] = child_frame_id
   radar_extrinsics['transform']['translation']['x'] = calibrated_sensor['translation'][0]
   radar_extrinsics['transform']['translation']['y'] = calibrated_sensor['translation'][1]
   radar_extrinsics['transform']['translation']['z'] = calibrated_sensor['translation'][2]
   radar_extrinsics['transform']['rotation']['w'] = calibrated_sensor['rotation'][0]
   radar_extrinsics['transform']['rotation']['x'] = calibrated_sensor['rotation'][1]
   radar_extrinsics['transform']['rotation']['y'] = calibrated_sensor['rotation'][2]
   radar_extrinsics['transform']['rotation']['z'] = calibrated_sensor['rotation'][3]
 
-  file_name = RADAR_EXTRINSICS.replace('radar', radar_name)
+  file_name = RADAR_EXTRINSICS.replace('radar', child_frame_id)
   file_path = os.path.join(calibration_file_path, RADAR_PARAMS_PATH)
   Path(file_path).mkdir(parents=True, exist_ok=True)
 
   radar_extrinsics_file = os.path.join(file_path, file_name)
   save_yaml(radar_extrinsics_file, radar_extrinsics)
 
 
-def gen_velodyne_params(lidar_name, calibrated_sensor, calibration_file_path):
+def gen_velodyne_params(child_frame_id, frame_id, calibrated_sensor,
+        calibration_file_path):
   """Generate lidar extrinsic file
 
   Args:
       lidar_name (str): lidar name
       calibrated_sensor (_type_): nuscenes calibrated_sensor json object
       calibration_file_path (str): saved path
   """
   lidar_meta_extrinsics = os.path.join(
     CALIBRATION_META_ROOT, VELODYNE_PARAMS_PATH, LIDAR_NOVATEL_EXTRINSICS)
   lidar_extrinsics = load_yaml(lidar_meta_extrinsics)
-  lidar_extrinsics['header']['frame_id'] = LIDAR_FRAME_ID
-  lidar_extrinsics['child_frame_id'] = lidar_name
+  lidar_extrinsics['header']['frame_id'] = frame_id
+  lidar_extrinsics['child_frame_id'] = child_frame_id
   lidar_extrinsics['transform']['translation']['x'] = calibrated_sensor['translation'][0]
   lidar_extrinsics['transform']['translation']['y'] = calibrated_sensor['translation'][1]
   lidar_extrinsics['transform']['translation']['z'] = calibrated_sensor['translation'][2]
   lidar_extrinsics['transform']['rotation']['w'] = calibrated_sensor['rotation'][0]
   lidar_extrinsics['transform']['rotation']['x'] = calibrated_sensor['rotation'][1]
   lidar_extrinsics['transform']['rotation']['y'] = calibrated_sensor['rotation'][2]
   lidar_extrinsics['transform']['rotation']['z'] = calibrated_sensor['rotation'][3]
 
-  file_name = LIDAR_NOVATEL_EXTRINSICS.replace('lidar', lidar_name)
+  file_name = LIDAR_NOVATEL_EXTRINSICS.replace('lidar', child_frame_id)
   file_path = os.path.join(calibration_file_path, VELODYNE_PARAMS_PATH)
   Path(file_path).mkdir(parents=True, exist_ok=True)
 
   lidar_novatel_extrinsics = os.path.join(file_path, file_name)
   save_yaml(lidar_novatel_extrinsics, lidar_extrinsics)
 
 
-def process_calib_imu_to_velo(channel, calibrated_sensor, calibration_file_path):
+def process_calib_velo_to_imu(channel, calibrated_sensor, calibration_file_path):
   qw, qx, qy, qz = calibrated_sensor['rotation']
   q = Quaternion(qw, qx, qy, qz)
   euler = q.to_euler()
   r_matrix = euler_to_rotation_matrix(euler.roll, euler.pitch, euler.yaw)
   # Apollo coordinate system conversion
-  # k_imu * imu2lidar = k_lidar
-  # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
-  transform = _construct_transform(r_matrix, calibrated_sensor['translation'])
-  imu_to_velo = apollo2nuscenes_imu @ transform @ nuscenes2apollo_lidar
-  r_matrix = imu_to_velo[:3,:3]
+  # lidar2imu * n_lidar = n_imu
+  # lidar2imu * apollo2n_lidar * apollo_lidar = apollo2n_imu * apollo_imu
+  lidar2imu = _construct_transform(r_matrix, calibrated_sensor['translation'])
+  velo_to_imu = nuscenes2apollo_imu @ lidar2imu @ apollo2nuscenes_lidar
 
+  r_matrix = velo_to_imu[:3, :3]
   roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
   q = Euler(roll, pitch, yaw).to_quaternion()
   calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+  calibrated_sensor['translation'] = velo_to_imu[:3, 3].tolist()
+  gen_velodyne_params(channel, LIDAR_FRAME_ID, calibrated_sensor, calibration_file_path)
 
-  calibrated_sensor['translation'] = imu_to_velo[:3, 3].tolist()
-  gen_velodyne_params(channel, calibrated_sensor, calibration_file_path)
 
-def process_calib_velo_to_cam(channel, calibrated_sensor, calibration_file_path):
+def process_calib_cam_to_imu(channel, calibrated_sensor, calibration_file_path):
+  # 1. camera extrinsics
   qw, qx, qy, qz = calibrated_sensor['rotation']
   q = Quaternion(qw, qx, qy, qz)
   euler = q.to_euler()
   r_matrix = euler_to_rotation_matrix(euler.roll, euler.pitch, euler.yaw)
   # Apollo coordinate system conversion
-  # k_imu * imu2lidar = k_lidar
-  # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
-  transform = _construct_transform(r_matrix, calibrated_sensor['translation'])
-  velo_to_cam = apollo2nuscenes_lidar @ transform @ nuscenes2apollo_camera
-  r_matrix = velo_to_cam[:3,:3]
+  # cam2imu * n_cam = n_imu
+  # cam2imu * apollo2n_cam * apollo_cam = apollo2n_imu * apollo_imu
+  cam2imu = _construct_transform(r_matrix, calibrated_sensor['translation'])
+  cam_to_imu = nuscenes2apollo_imu @ cam2imu @ apollo2nuscenes_camera
 
+  r_matrix = cam_to_imu[:3,:3]
   roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
   q = Euler(roll, pitch, yaw).to_quaternion()
   calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
+  calibrated_sensor['translation'] = cam_to_imu[:3, 3].tolist()
+  gen_camera_extrinsics(channel, CAMERA_FRAME_ID, calibrated_sensor,
+      calibration_file_path)
+
+  # 2. camera intrinsic
+  calibrated_sensor['width'] = 1920
+  calibrated_sensor['height'] = 1080
 
-  calibrated_sensor['translation'] = velo_to_cam[:3, 3].tolist()
-  gen_radar_params(channel, calibrated_sensor, calibration_file_path)
+  calibrated_sensor['K'] = calibrated_sensor['camera_intrinsic']
+  gen_camera_intrinsics(channel, calibrated_sensor, calibration_file_path)
 
 
-def process_calib_velo_to_radar(channel, calibrated_sensor, calibration_file_path):
+def process_calib_radar_to_imu(channel, calibrated_sensor, calibration_file_path):
   qw, qx, qy, qz = calibrated_sensor['rotation']
   q = Quaternion(qw, qx, qy, qz)
   euler = q.to_euler()
   r_matrix = euler_to_rotation_matrix(euler.roll, euler.pitch, euler.yaw)
   # Apollo coordinate system conversion
-  # k_imu * imu2lidar = k_lidar
-  # apollo_imu * apollo2k_imu * imu2lidar = apollo_lidar * apollo2k_lidar
-  transform = _construct_transform(r_matrix, calibrated_sensor['translation'])
-  velo_to_radar = apollo2nuscenes_lidar @ transform @ nuscenes2apollo_radar
-  r_matrix = velo_to_radar[:3,:3]
+  # radar2imu * n_radar = n_imu
+  # radar2imu * apollo2n_radar * apollo_radar = apollo2n_imu * apollo_imu
+  radar2imu = _construct_transform(r_matrix, calibrated_sensor['translation'])
+  radar_to_imu = nuscenes2apollo_imu @ radar2imu @ apollo2nuscenes_radar
 
+  r_matrix = radar_to_imu[:3, :3]
   roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
   q = Euler(roll, pitch, yaw).to_quaternion()
   calibrated_sensor['rotation'] = [q.w, q.x, q.y, q.z]
-
-  calibrated_sensor['translation'] = velo_to_radar[:3, 3].tolist()
-  gen_radar_params(channel, calibrated_sensor, calibration_file_path)
+  calibrated_sensor['translation'] = radar_to_imu[:3, 3].tolist()
+  gen_radar_params(channel, RADAR_FRAME_ID, calibrated_sensor, calibration_file_path)
 
 
 def gen_sensor_calibration(calibrations, calibration_file_path):
   """Generate camera/radar/lidar extrinsic file and camera intrinsic file
 
   Args:
       calibrations (dict): nuscenes calibrated_sensor json objects
       calibration_file_path (str): saved path
   """
   for channel, calibrated_sensor in calibrations.items():
-    if channel.startswith('CAM'):
-      process_calib_imu_to_velo(channel, calibrated_sensor, calibration_file_path)
-    elif channel.startswith('LIDAR'):
-      process_calib_velo_to_cam(channel, calibrated_sensor, calibration_file_path)
+    if channel.startswith('LIDAR'):
+      process_calib_velo_to_imu(channel, calibrated_sensor, calibration_file_path)
+    elif channel.startswith('CAM'):
+      process_calib_cam_to_imu(channel, calibrated_sensor, calibration_file_path)
     elif channel.startswith('RADAR'):
-      process_calib_velo_to_radar(channel, calibrated_sensor, calibration_file_path)
+      process_calib_radar_to_imu(channel, calibrated_sensor, calibration_file_path)
     else:
       print("Unsupported sensor: {}".format(channel))
 
 
 def dataset_to_calibration(nuscenes, calibration_root_path):
   """Generate sensor calibration
```

### Comparing `adataset-0.1.2/adataset/nuscenes/dataset_converter.py` & `adataset-0.1.3/adataset/nuscenes/dataset_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,17 @@
   PointCloudBuilder,
   LocalizationBuilder,
   TransformBuilder)
 from adataset.nuscenes.nuscenes import NuScenesSchema, NuScenesHelper, NuScenes
 from adataset.nuscenes.geometry import (
   Euler,
   Quaternion,
-  rotation_matrix_to_euler
 )
 from adataset.nuscenes.params import (
   nuscenes2apollo_lidar,
-  nuscenes2apollo_imu,
 )
 
 LOCALIZATION_TOPIC = '/apollo/localization/pose'
 TF_TOPIC= '/tf'
 
 
 def dataset_to_record(nuscenes, record_root_path):
```

### Comparing `adataset-0.1.2/adataset/nuscenes/geometry.py` & `adataset-0.1.3/adataset/nuscenes/geometry.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/nuscenes/nuscenes.py` & `adataset-0.1.3/adataset/nuscenes/nuscenes.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset/nuscenes/params.py` & `adataset-0.1.3/adataset/nuscenes/params.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,33 +14,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###############################################################################
 
 import numpy as np
 
-identity = np.identity(4)
 
-apollo2nuscenes_lidar = np.array([[0.0000000, 1.0000000, 0.0000000, 0.0000000],
-                                  [-1.0000000, 0.0000000, 0.0000000, 0.0000000],
+apollo2nuscenes_lidar = np.array([[0.0000000, -1.0000000, 0.0000000, 0.0000000],
+                                  [1.0000000, 0.0000000, 0.0000000, 0.0000000],
                                   [0.0000000, 0.0000000, 1.0000000, 0.0000000],
                                   [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
 
 apollo2nuscenes_camera = np.array([[1.0000000, 0.0000000, 0.0000000, 0.0000000],
                                    [0.0000000, 1.0000000, 0.0000000, 0.0000000],
                                    [0.0000000, 0.0000000, 1.0000000, 0.0000000],
                                    [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
 
 apollo2nuscenes_radar = np.array([[1.0000000, 0.0000000, 0.0000000, 0.0000000],
-                                   [0.0000000, 1.0000000, 0.0000000, 0.0000000],
-                                   [0.0000000, 0.0000000, 1.0000000, 0.0000000],
-                                   [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
+                                  [0.0000000, 1.0000000, 0.0000000, 0.0000000],
+                                  [0.0000000, 0.0000000, 1.0000000, 0.0000000],
+                                  [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
 
-apollo2nuscenes_imu = np.array([[0.0000000, -1.0000000, 0.0000000, 0.0000000],
-                                [1.0000000, 0.0000000, 0.0000000, 0.0000000],
+apollo2nuscenes_imu = np.array([[0.0000000, 1.0000000, 0.0000000, 0.0000000],
+                                [-1.0000000, 0.0000000, 0.0000000, 0.0000000],
                                 [0.0000000, 0.0000000, 1.0000000, 0.0000000],
                                 [0.0000000, 0.0000000, 0.0000000, 1.0000000]])
 
 nuscenes2apollo_lidar = np.linalg.inv(apollo2nuscenes_lidar)
 nuscenes2apollo_camera = np.linalg.inv(apollo2nuscenes_camera)
 nuscenes2apollo_radar = np.linalg.inv(apollo2nuscenes_radar)
 nuscenes2apollo_imu = np.linalg.inv(apollo2nuscenes_imu)
```

### Comparing `adataset-0.1.2/adataset/nuscenes/pcd_converter.py` & `adataset-0.1.3/adataset/nuscenes/pcd_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/adataset.egg-info/PKG-INFO` & `adataset-0.1.3/adataset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adataset
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dataset conversion to Apollo record tool
 Home-page: https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset
 Author: apollo-team
 Author-email: apollo-support@baidu.com
 Project-URL: Bug Tracker, https://github.com/ApolloAuto/apollo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `adataset-0.1.2/adataset.egg-info/SOURCES.txt` & `adataset-0.1.3/adataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adataset-0.1.2/setup.py` & `adataset-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adataset",
-    version="0.1.2",
+    version="0.1.3",
     author="apollo-team",
     author_email="apollo-support@baidu.com",
     description="Dataset conversion to Apollo record tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset",
     project_urls={
```

