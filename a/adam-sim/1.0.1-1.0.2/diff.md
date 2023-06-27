# Comparing `tmp/adam_sim-1.0.1.tar.gz` & `tmp/adam_sim-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_sim-1.0.1.tar", last modified: Mon May 29 15:40:50 2023, max compression
+gzip compressed data, was "adam_sim-1.0.2.tar", last modified: Tue Jun 27 09:58:39 2023, max compression
```

## Comparing `adam_sim-1.0.1.tar` & `adam_sim-1.0.2.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.095546 adam_sim-1.0.1/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1063 2023-05-29 15:34:07.000000 adam_sim-1.0.1/LICENSE
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3532 2023-05-29 15:40:50.095546 adam_sim-1.0.1/PKG-INFO
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2887 2023-05-29 15:34:07.000000 adam_sim-1.0.1/README.md
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.075654 adam_sim-1.0.1/adam_sim/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       40 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.075654 adam_sim-1.0.1/adam_sim/core/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      815 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/core/topics.yaml
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/entities/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      353 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3134 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/acceleration.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     6411 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/configuration.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3065 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/point.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2351 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/system.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1665 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/vector.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2782 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/velocity.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      121 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       23 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     7765 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/adam.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       57 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      352 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/adam_repository_factory.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      116 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       53 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      929 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       63 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1225 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      853 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2491 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      952 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     5817 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     5832 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   306784 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    64184 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     6084 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     6284 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    48684 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   234684 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   514984 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   983584 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)  1147584 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   307884 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   953184 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)  3570434 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41884 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   174484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   953184 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)  3570434 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   461284 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41884 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   174484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   483484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)  1619484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   483484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)  1619484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   483484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)  1619484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1043 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    73373 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/light-gray-floor-tile.png
--rw-rw-r--   0 vistor    (1001) vistor    (1001)   196878 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/metal.png
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      442 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/simulated_adam_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/entities/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       32 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/entities/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      703 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/entities/adam_info.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       44 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      352 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/repository/adam_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/use_cases/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       27 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1384 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/use_cases/viewer.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       23 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      427 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/base.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       57 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      352 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/base_repository_factory.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      116 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       53 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      666 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       63 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      640 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/entities/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       32 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/entities/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      475 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/entities/base_info.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       44 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      403 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/repository/base_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/data_manager/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       38 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/data_manager/data/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    20048 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/data/configurations_test.csv
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     5901 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/data/end_effector_positions_test.csv
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3330 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/data_manager.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       37 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       71 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      328 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       76 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2010 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       31 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1947 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       78 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2011 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       31 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1949 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       86 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3634 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       48 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     4434 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       88 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3643 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       48 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     4439 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      667 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/manipulator_repository_factory.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/entities/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       79 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/entities/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1698 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/entities/collision.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1008 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/entities/manipulator_info.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2528 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/manipulator.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/repository/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       58 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/repository/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1103 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/repository/manipulator_repository.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       73 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3761 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/control_visualizer.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     5109 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/farm.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.075654 adam_sim-1.0.1/adam_sim.egg-info/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     3532 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/PKG-INFO
--rw-rw-r--   0 vistor    (1001) vistor    (1001)    10053 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/SOURCES.txt
--rw-rw-r--   0 vistor    (1001) vistor    (1001)        1 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/dependency_links.txt
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       75 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/requires.txt
--rw-rw-r--   0 vistor    (1001) vistor    (1001)        9 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/top_level.txt
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      930 2023-05-29 15:40:24.000000 adam_sim-1.0.1/pyproject.toml
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       38 2023-05-29 15:40:50.095546 adam_sim-1.0.1/setup.cfg
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.095546 adam_sim-1.0.1/tests/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      743 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_basic_usage.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1541 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_collisions.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      494 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_configuration.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      344 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_control.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1021 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_data_manager.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      116 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_export_scene.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      752 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_farm.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      604 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_real_communication.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      854 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_returning_info.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      533 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_velocity.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1063 2023-04-12 06:42:52.000000 adam_sim-1.0.2/LICENSE
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3532 2023-06-27 09:58:39.138201 adam_sim-1.0.2/PKG-INFO
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2887 2023-04-14 09:53:02.000000 adam_sim-1.0.2/README.md
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.122202 adam_sim-1.0.2/adam_sim/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       40 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.122202 adam_sim-1.0.2/adam_sim/core/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      815 2023-04-17 10:50:13.000000 adam_sim-1.0.2/adam_sim/core/topics.yaml
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.122202 adam_sim-1.0.2/adam_sim/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      353 2023-04-13 11:45:34.000000 adam_sim-1.0.2/adam_sim/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3134 2023-04-13 11:45:06.000000 adam_sim-1.0.2/adam_sim/entities/acceleration.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     6411 2023-04-19 11:37:53.000000 adam_sim-1.0.2/adam_sim/entities/configuration.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3642 2023-06-27 08:31:45.000000 adam_sim-1.0.2/adam_sim/entities/point.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2351 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/entities/system.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3543 2023-06-27 08:34:35.000000 adam_sim-1.0.2/adam_sim/entities/vector.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2782 2023-04-13 11:36:34.000000 adam_sim-1.0.2/adam_sim/entities/velocity.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.122202 adam_sim-1.0.2/adam_sim/features/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      121 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.126202 adam_sim-1.0.2/adam_sim/features/adam/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       23 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     7765 2023-04-20 13:03:37.000000 adam_sim-1.0.2/adam_sim/features/adam/adam.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.126202 adam_sim-1.0.2/adam_sim/features/adam/communication/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       57 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/adam_repository_factory.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.126202 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.126202 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/real_adam_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       53 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/real_adam_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      929 2023-04-20 13:05:27.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.126202 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       63 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.126202 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.126202 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1225 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      853 2023-04-12 10:53:15.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2491 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      952 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     5817 2023-04-12 10:29:53.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     5832 2023-04-12 10:30:17.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   306784 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    64184 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     6084 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1484 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     6284 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    48684 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   234684 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   514984 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   983584 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1147584 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   307884 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-04-12 10:28:03.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   461284 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1043 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    73373 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/light-gray-floor-tile.png
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   196878 2023-04-12 10:28:04.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/metal.png
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      442 2023-04-20 13:08:10.000000 adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/simulated_adam_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/adam/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      703 2023-04-18 10:04:19.000000 adam_sim-1.0.2/adam_sim/features/adam/entities/adam_info.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/adam/repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       44 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-20 13:04:57.000000 adam_sim-1.0.2/adam_sim/features/adam/repository/adam_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/adam/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       27 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1384 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/adam/use_cases/viewer.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/base/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       23 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      427 2023-04-19 09:57:15.000000 adam_sim-1.0.2/adam_sim/features/base/base.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/base/communication/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       57 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/communication/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/communication/base_repository_factory.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/real_base_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       53 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/real_base_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      666 2023-04-20 13:11:50.000000 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/simulated_base_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       63 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/simulated_base_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      640 2023-04-20 13:12:00.000000 adam_sim-1.0.2/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/base/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      475 2023-04-13 12:23:56.000000 adam_sim-1.0.2/adam_sim/features/base/entities/base_info.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.134201 adam_sim-1.0.2/adam_sim/features/base/repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       44 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/base/repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      403 2023-04-20 13:08:40.000000 adam_sim-1.0.2/adam_sim/features/base/repository/base_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/data_manager/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/data_manager/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/data_manager/data/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    20048 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/data_manager/data/configurations_test.csv
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     5901 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/data_manager/data/end_effector_positions_test.csv
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3330 2023-04-19 07:32:30.000000 adam_sim-1.0.2/adam_sim/features/data_manager/data_manager.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       37 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       71 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      328 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       76 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2010 2023-04-20 13:01:18.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       31 2023-04-18 07:57:00.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1947 2023-04-22 11:00:16.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       78 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2011 2023-04-22 10:57:14.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       31 2023-04-22 10:57:33.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1949 2023-04-22 10:59:24.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       86 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3634 2023-04-20 13:00:00.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       48 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     4434 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       88 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3643 2023-04-20 13:00:17.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       48 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     4439 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      667 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/communication/manipulator_repository_factory.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       79 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1698 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/entities/collision.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1008 2023-04-13 11:47:19.000000 adam_sim-1.0.2/adam_sim/features/manipulator/entities/manipulator_info.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3424 2023-06-27 08:41:22.000000 adam_sim-1.0.2/adam_sim/features/manipulator/manipulator.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       58 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1103 2023-04-20 12:59:27.000000 adam_sim-1.0.2/adam_sim/features/manipulator/repository/manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/adam_sim/features/manipulator/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       73 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3761 2023-04-12 06:42:52.000000 adam_sim-1.0.2/adam_sim/features/manipulator/use_cases/control_visualizer.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     4958 2023-06-27 09:54:26.000000 adam_sim-1.0.2/adam_sim/features/manipulator/use_cases/farm.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.122202 adam_sim-1.0.2/adam_sim.egg-info/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3532 2023-06-27 09:58:39.000000 adam_sim-1.0.2/adam_sim.egg-info/PKG-INFO
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    10053 2023-06-27 09:58:39.000000 adam_sim-1.0.2/adam_sim.egg-info/SOURCES.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)        1 2023-06-27 09:58:39.000000 adam_sim-1.0.2/adam_sim.egg-info/dependency_links.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       75 2023-06-27 09:58:39.000000 adam_sim-1.0.2/adam_sim.egg-info/requires.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)        9 2023-06-27 09:58:39.000000 adam_sim-1.0.2/adam_sim.egg-info/top_level.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      930 2023-06-27 09:58:18.000000 adam_sim-1.0.2/pyproject.toml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-06-27 09:58:39.138201 adam_sim-1.0.2/setup.cfg
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-06-27 09:58:39.138201 adam_sim-1.0.2/tests/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      743 2023-04-13 10:35:02.000000 adam_sim-1.0.2/tests/test_basic_usage.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1541 2023-04-13 11:22:46.000000 adam_sim-1.0.2/tests/test_collisions.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      494 2023-04-19 11:02:01.000000 adam_sim-1.0.2/tests/test_configuration.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      344 2023-04-13 10:42:23.000000 adam_sim-1.0.2/tests/test_control.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1021 2023-04-19 08:23:30.000000 adam_sim-1.0.2/tests/test_data_manager.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-13 11:20:44.000000 adam_sim-1.0.2/tests/test_export_scene.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1295 2023-06-27 09:50:54.000000 adam_sim-1.0.2/tests/test_farm.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      604 2023-04-20 14:31:17.000000 adam_sim-1.0.2/tests/test_real_communication.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      854 2023-04-13 11:59:15.000000 adam_sim-1.0.2/tests/test_returning_info.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      533 2023-04-13 12:17:49.000000 adam_sim-1.0.2/tests/test_velocity.py
```

### Comparing `adam_sim-1.0.1/LICENSE` & `adam_sim-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/PKG-INFO` & `adam_sim-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam_sim
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simulator of ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots UR3 of 6 DoF each.
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/adam_simulator
 Project-URL: Bug Tracker, https://github.com/vistormu/adam_simulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adam_sim Version: 1.0.1 Summary: A simulator of
+Metadata-Version: 2.1 Name: adam_sim Version: 1.0.2 Summary: A simulator of
 ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator
 consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots
 UR3 of 6 DoF each. Author: Vistor Project-URL: Homepage, https://github.com/
 vistormu/adam_simulator Project-URL: Bug Tracker, https://github.com/vistormu/
 adam_simulator/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
```

### Comparing `adam_sim-1.0.1/README.md` & `adam_sim-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/core/topics.yaml` & `adam_sim-1.0.2/adam_sim/core/topics.yaml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/entities/acceleration.py` & `adam_sim-1.0.2/adam_sim/entities/acceleration.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/entities/configuration.py` & `adam_sim-1.0.2/adam_sim/entities/configuration.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/entities/point.py` & `adam_sim-1.0.2/adam_sim/entities/point.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,26 @@
     y : float
         the y value of the point
     z : float
         the z value of the point
 
     Methods
     -------
+    round:
+        rounds the point to the specified number of decimal places
+    norm:
+        calculates the norm of the point
+    to_numpy:
+        converts the point to a numpy array
+    to_list:
+        converts the point to a list
+    from_numpy:
+        converts a numpy array to a point
+    from_list:
+        converts a list to a point
     """
     x: float
     y: float
     z: float
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self.x}, {self.y}, {self.z})'
@@ -64,14 +76,25 @@
         Returns
         -------
         out : ~.entities.Point
             the rounded point
         '''
         return Point(round(self.x, n), round(self.y, n), round(self.z, n))
 
+    def norm(self) -> float:
+        '''
+        calculates the norm of the point
+
+        Returns
+        -------
+        out : float
+            the norm of the point
+        '''
+        return np.linalg.norm(self).astype(float)
+
     def to_numpy(self) -> np.ndarray:
         '''
         converts the point to a numpy array
 
         Returns
         -------
         out : numpy.ndarray
```

### Comparing `adam_sim-1.0.1/adam_sim/entities/system.py` & `adam_sim-1.0.2/adam_sim/entities/system.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/entities/velocity.py` & `adam_sim-1.0.2/adam_sim/entities/velocity.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/adam.py` & `adam_sim-1.0.2/adam_sim/features/adam/adam.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/light-gray-floor-tile.png` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/light-gray-floor-tile.png`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/metal.png` & `adam_sim-1.0.2/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/metal.png`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/entities/adam_info.py` & `adam_sim-1.0.2/adam_sim/features/adam/entities/adam_info.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/adam/use_cases/viewer.py` & `adam_sim-1.0.2/adam_sim/features/adam/use_cases/viewer.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py` & `adam_sim-1.0.2/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py` & `adam_sim-1.0.2/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/data_manager/data/configurations_test.csv` & `adam_sim-1.0.2/adam_sim/features/data_manager/data/configurations_test.csv`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/data_manager/data/end_effector_positions_test.csv` & `adam_sim-1.0.2/adam_sim/features/data_manager/data/end_effector_positions_test.csv`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/data_manager/data_manager.py` & `adam_sim-1.0.2/adam_sim/features/data_manager/data_manager.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/communication/manipulator_repository_factory.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/communication/manipulator_repository_factory.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/entities/collision.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/entities/collision.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/entities/manipulator_info.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/entities/manipulator_info.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/manipulator.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/manipulator.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,33 +17,51 @@
         sets the manipulator to the specified configuration
 
     set_velocity_to:
         sets the manipulator velocity to the specified vector
 
     control:
         control the manipulator via an interface
-    ''' 
+    '''
+
     def _init_repository(self, id: str, *args, **kwargs) -> None:
+        self._id: str = id
         self._repository: ManipulatorRepository = get_manipulator_repository(id)
         self._control_visualizer: ControlVisualizer = ControlVisualizer(id)
-        
+
         self._repository.init(*args, **kwargs)
 
-    def move_to(self, point: Point) -> None:
+    def move_to(self,
+                target: System,
+                tolerance: float = 0.01,
+                max_iterations: int = 5,
+                consider_orientation: bool = False,
+                ) -> None:
         '''
         moves the manipulator to the specified position
 
         Parameters
         ----------
-        point : ~.entities.Point
-            the position to move the manipulator's end effector to
+        target : ~.entities.System
+            the target position of the manipulator's end effector
+        tolerance : float, optional
+            the tolerance of the manipulator's end effector position, by default 0.01
+        max_iterations : int, optional
+            the maximum number of iterations, by default 5
+        consider_orientation : bool, optional
+            whether to consider the orientation of the target, by default False
         '''
         systems: list[System] = self._repository.get_systems()
-        target: System = System(point, systems[-1].x_axis, systems[-1].y_axis, systems[-1].z_axis)
-        configuration: Configuration | None = Farm.iterate(systems, target)
+        configuration: Configuration | None = Farm.iterate(systems=systems,
+                                                           target=target,
+                                                           tolerance=tolerance,
+                                                           max_iterations=max_iterations,
+                                                           consider_orientation=consider_orientation,
+                                                           manipulator=self._id,
+                                                           )
 
         if configuration is None:
             return
 
         self._repository.set_configuration(configuration)
 
     def set_to(self, configuration: Configuration) -> None:
@@ -56,24 +74,22 @@
             the configuration of the manipulator
         '''
         self._repository.set_configuration(configuration)
 
     def set_velocity_to(self, velocity: Velocity) -> None:
         '''
         sets the manipulator velocity to the specified vector
-        
+
         Parameters
         ----------
         velocity : ~.entities.Velocity
             the velocity of the manipulator
         '''
         self._repository.set_velocity(velocity)
 
     def control(self) -> None:
         '''
         control the manipulator via an interface
         '''
         self._control_visualizer.init(self._repository.get_configuration())
-        
+
         self._repository.set_configuration(self._control_visualizer.get())
-        
-
```

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/repository/manipulator_repository.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/repository/manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/control_visualizer.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/use_cases/control_visualizer.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/farm.py` & `adam_sim-1.0.2/adam_sim/features/manipulator/use_cases/farm.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,49 +3,53 @@
 from ....entities import System, Point, Vector, Configuration
 
 a: list[float] = [-1.0, 0.0, 0.24365, 0.21325, 0.0, 0.0, 0.0]
 d: list[float] = [-1.0, 0.1519, 0.0, 0.0, 0.11235, 0.08535, 0.0819]
 alpha: list[float] = [-1.0, -np.pi/2, 0.0, 0.0, -np.pi/2, np.pi/2, 0.0]
 base_to: int = 3
 
-MAX_ITERATIONS: int = 20
-TOLERANCE: float = 0.0005
-
 
 class Farm:
     @classmethod
-    def iterate(cls, systems: list[System], target: System) -> Configuration | None:
+    def iterate(cls,
+                systems: list[System],
+                target: System,
+                tolerance: float,
+                max_iterations: int,
+                consider_orientation: bool,
+                manipulator: str,
+                ) -> Configuration | None:
         new_configuration: Configuration | None = None
+        base: System = systems[0]
+
+        for _ in range(1, max_iterations+1):
+            end_effector: System = systems[-1]
 
-        distance: float = np.linalg.norm(target.position-systems[-1].position).astype(float)
-        for _ in range(1, MAX_ITERATIONS+1):
-            # Termination condition
-            if distance <= TOLERANCE:
+            distance: float = (target.position - end_effector.position).norm()
+            if distance <= tolerance:
                 break
 
-            # Perform iteration
-            backward_systems: list[System] = cls.backward(systems, target)
-            forward_systems, new_configuration = cls.forward(backward_systems, systems[0])
-
-            # Update variables
-            target = System(target.position, forward_systems[-1].x_axis, forward_systems[-1].y_axis, forward_systems[-1].z_axis)
-            distance: float = np.linalg.norm(target.position-systems[-1].position).astype(float)
-
-            # if new_configuration.q3 > 0.0:
-            #     new_configuration = Configuration(new_configuration.q1,
-            #                                       new_configuration.q2 + new_configuration.q3,
-            #                                       -new_configuration.q3,
-            #                                       new_configuration.q4,
-            #                                       new_configuration.q5,
-            #                                       new_configuration.q6)
+            if not consider_orientation:
+                target = System(target.position, *end_effector[1:])
+
+            systems = cls.target_to_base(systems, target)
+            systems, new_configuration = cls.base_to_target(systems, base)
+
+            if new_configuration.q3 < 0.0 and manipulator == 'left_simulated':
+                new_configuration = Configuration(new_configuration.q1,
+                                                  new_configuration.q2 + new_configuration.q3,
+                                                  -new_configuration.q3,
+                                                  new_configuration.q4,
+                                                  new_configuration.q5,
+                                                  new_configuration.q6)
 
         return new_configuration
 
     @staticmethod
-    def backward(systems: list[System], target: System) -> list[System]:
+    def target_to_base(systems: list[System], target: System) -> list[System]:
         # Initialize lists
         p: list[Point] = [system.position for system in systems]
         x: list[Vector] = [system.x_axis for system in systems]
         y: list[Vector] = [system.y_axis for system in systems]
         z: list[Vector] = [system.z_axis for system in systems]
 
         new_p: list[Point] = [systems[0].position] + [target.position]*(len(p)-1)
@@ -53,44 +57,41 @@
         new_y: list[Vector] = [systems[0].y_axis] + [target.y_axis]*(len(y)-1)
         new_z: list[Vector] = [systems[0].z_axis] + [target.z_axis]*(len(z)-1)
 
         for i in reversed(range(0, len(p)-1)):
             new_z[i] = new_y[i+1]*np.sin(alpha[i+1]) + new_z[i+1]*np.cos(alpha[i+1])
             new_p[i] = new_p[i+1] - Point(*new_x[i+1])*a[i+1] - Point(*new_y[i+1])*d[i+1]*np.sin(alpha[i+1]) - Point(*new_z[i+1])*d[i+1]*np.cos(alpha[i+1])
 
-            lamb: int = np.sign(np.abs(a[i]+d[i])).astype(int)
-
-            j: int = i + lamb - 2
-            v: np.ndarray = np.array(p[j] - new_p[i]) - np.dot(p[j] - new_p[i], new_z[i])*np.array(new_z[i])
+            v: np.ndarray = np.array(p[i-1] - new_p[i]) - np.dot(p[i-1] - new_p[i], new_z[i])*np.array(new_z[i])
 
-            mu = lamb*np.sign(-a[i]-d[i]*np.sin(alpha[i])) + (1-lamb)*np.sign(np.dot(v, x[i]))
+            mu = np.sign(-a[i]-d[i]*np.sin(alpha[i]))
             phi: int = np.abs(np.sign(d[i])).astype(int)
 
             new_x[i] = Vector(*((1-phi)*mu*v + phi*mu*np.cross(v, new_z[i]))).normalize()
             new_y[i] = Vector(*((1-phi)*mu*np.cross(new_z[i], v) + phi*mu*v)).normalize()
 
         return [System(p_i, x_i, y_i, z_i) for (p_i, x_i, y_i, z_i) in zip(new_p, new_x, new_y, new_z)]
 
     @ staticmethod
-    def forward(systems: list[System], base: System) -> tuple[list[System], Configuration]:
+    def base_to_target(systems: list[System], base: System) -> tuple[list[System], Configuration]:
         # Initialize lists
         p: list[Point] = [oriented_point.position for oriented_point in systems]
         x: list[Vector] = [oriented_point.x_axis for oriented_point in systems]
         y: list[Vector] = [oriented_point.y_axis for oriented_point in systems]
         z: list[Vector] = [oriented_point.z_axis for oriented_point in systems]
 
         theta: list[float] = [0.0]*(len(p))
 
         new_p: list[Point] = [base.position]*len(p)
         new_x: list[Vector] = [base.x_axis]*len(x)
         new_y: list[Vector] = [base.y_axis]*len(y)
         new_z: list[Vector] = [base.z_axis]*len(z)
 
         for i in range(1, len(p)):
-            u: np.ndarray = np.sign(np.dot(x[i], p[base_to] - new_p[i-1]))*np.array(p[base_to] - new_p[i-1]) if i == 1 and base_to != 0 else np.array(x[i])
+            u: np.ndarray = np.sign(np.dot(x[i], p[base_to] - new_p[i-1]))*np.array(p[base_to] - new_p[i-1]) if i == 1 else np.array(x[i])
 
             new_x[i] = Vector(*(u-np.dot(u, new_z[i-1])*new_z[i-1])).normalize()
 
             theta[i] = float(np.arctan2(np.dot(np.cross(new_x[i-1], new_x[i]), new_z[i-1]), np.dot(new_x[i], new_x[i-1])))
 
             new_p[i] = new_p[i-1] + Point(*new_x[i-1])*a[i]*np.cos(theta[i]) + Point(*new_y[i-1])*a[i]*np.sin(theta[i]) + Point(*new_z[i-1])*d[i]
             new_y[i] = (new_x[i-1]*(-np.cos(alpha[i])*np.sin(theta[i])) + new_y[i-1]*np.cos(alpha[i])*np.cos(theta[i]) + new_z[i-1]*np.sin(alpha[i])).normalize()
```

### Comparing `adam_sim-1.0.1/adam_sim.egg-info/PKG-INFO` & `adam_sim-1.0.2/adam_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-sim
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simulator of ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots UR3 of 6 DoF each.
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/adam_simulator
 Project-URL: Bug Tracker, https://github.com/vistormu/adam_simulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adam-sim Version: 1.0.1 Summary: A simulator of
+Metadata-Version: 2.1 Name: adam-sim Version: 1.0.2 Summary: A simulator of
 ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator
 consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots
 UR3 of 6 DoF each. Author: Vistor Project-URL: Homepage, https://github.com/
 vistormu/adam_simulator Project-URL: Bug Tracker, https://github.com/vistormu/
 adam_simulator/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
```

### Comparing `adam_sim-1.0.1/adam_sim.egg-info/SOURCES.txt` & `adam_sim-1.0.2/adam_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/pyproject.toml` & `adam_sim-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adam_sim"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name = "Vistor" }]
 description = "A simulator of ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots UR3 of 6 DoF each."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `adam_sim-1.0.1/tests/test_basic_usage.py` & `adam_sim-1.0.2/tests/test_basic_usage.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/tests/test_collisions.py` & `adam_sim-1.0.2/tests/test_collisions.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/tests/test_data_manager.py` & `adam_sim-1.0.2/tests/test_data_manager.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/tests/test_real_communication.py` & `adam_sim-1.0.2/tests/test_real_communication.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/tests/test_returning_info.py` & `adam_sim-1.0.2/tests/test_returning_info.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.1/tests/test_velocity.py` & `adam_sim-1.0.2/tests/test_velocity.py`

 * *Files identical despite different names*

