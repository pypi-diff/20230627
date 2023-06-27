# Comparing `tmp/pygame_ecs-0.2.2.tar.gz` & `tmp/pygame_ecs-0.2.3.tar.gz`

## Comparing `pygame_ecs-0.2.2.tar` & `pygame_ecs-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/.gitattributes
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/entity.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/exceptions.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/components/base_component.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/managers/component_manager.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/managers/entity_manager.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/managers/system_manager.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/systems/base_system.py
--rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/circle.png
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/draw_test.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/particle_test_cpu.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/particle_test_gpu.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/speed_test.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/tester.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/LICENSE
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/README.md
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/.gitattributes
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/entity.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/exceptions.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/components/base_component.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/managers/component_manager.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/managers/entity_manager.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/managers/system_manager.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pygame_ecs/systems/base_system.py
+-rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/test/circle.png
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/test/draw_test.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/test/particle_test_cpu.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/test/particle_test_gpu.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/test/speed_test.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/test/tester.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/README.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 pygame_ecs-0.2.3/PKG-INFO
```

### Comparing `pygame_ecs-0.2.2/pygame_ecs/managers/component_manager.py` & `pygame_ecs-0.2.3/pygame_ecs/managers/component_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/pygame_ecs/managers/entity_manager.py` & `pygame_ecs-0.2.3/pygame_ecs/managers/entity_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/pygame_ecs/managers/system_manager.py` & `pygame_ecs-0.2.3/pygame_ecs/managers/system_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/pygame_ecs/systems/base_system.py` & `pygame_ecs-0.2.3/pygame_ecs/systems/base_system.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/test/circle.png` & `pygame_ecs-0.2.3/test/circle.png`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/test/draw_test.py` & `pygame_ecs-0.2.3/test/draw_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     )
     radius = random.randint(4, 18)
     color = [random.randint(0, 255) for _ in range(3)]
     vel = pygame.math.Vector2(
         (random.random() - 0.5) * 400 / 1000,
         (random.random() - 0.5) * 400 / 1000,
     )
-    entity = entity_manager.add_entity(component_manager)
+    entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
     component_manager.add_component(entity, BallRenderer(radius, color))
     entities.append(entity)
 
 while True:
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
```

### Comparing `pygame_ecs-0.2.2/test/particle_test_cpu.py` & `pygame_ecs-0.2.3/test/particle_test_cpu.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/test/particle_test_gpu.py` & `pygame_ecs-0.2.3/test/particle_test_gpu.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/test/speed_test.py` & `pygame_ecs-0.2.3/test/speed_test.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/.gitignore` & `pygame_ecs-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/LICENSE` & `pygame_ecs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.2/README.md` & `pygame_ecs-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     )
     radius = random.randint(4, 18)
     color = [random.randint(0, 255) for _ in range(3)]
     vel = pygame.math.Vector2(
         (random.random() - 0.5) * 400 / 1000,
         (random.random() - 0.5) * 400 / 1000,
     )
-    entity = entity_manager.add_entity(component_manager)
+    entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
     component_manager.add_component(entity, BallRenderer(radius, color))
     entities.append(entity)
 
 while True:
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
```

### Comparing `pygame_ecs-0.2.2/pyproject.toml` & `pygame_ecs-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "pygame_ecs"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Notenlish", email="71970100+Notenlish@users.noreply.github.com" },
 ]
 description = "Pure Python, simple to use Entity Component System(ECS) for pygame"
 packages=["pygame_ecs", "pygame_ecs.components", "pygame_ecs.managers", "pygame_ecs.systems"]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pygame_ecs-0.2.2/PKG-INFO` & `pygame_ecs-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_ecs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Pure Python, simple to use Entity Component System(ECS) for pygame
 Project-URL: Homepage, https://github.com/Notenlish/pygame_ecs
 Project-URL: Bug Tracker, https://github.com/Notenlish/pygame_ecs/issues
 Author-email: Notenlish <71970100+Notenlish@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ECS,component,ecs,entity,entity component system,pygame,pygame-ce,pygame_ecs,system
@@ -126,15 +126,15 @@
     )
     radius = random.randint(4, 18)
     color = [random.randint(0, 255) for _ in range(3)]
     vel = pygame.math.Vector2(
         (random.random() - 0.5) * 400 / 1000,
         (random.random() - 0.5) * 400 / 1000,
     )
-    entity = entity_manager.add_entity(component_manager)
+    entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
     component_manager.add_component(entity, BallRenderer(radius, color))
     entities.append(entity)
 
 while True:
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
```

