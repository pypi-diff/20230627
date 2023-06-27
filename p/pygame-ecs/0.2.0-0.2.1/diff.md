# Comparing `tmp/pygame_ecs-0.2.0.tar.gz` & `tmp/pygame_ecs-0.2.1.tar.gz`

## Comparing `pygame_ecs-0.2.0.tar` & `pygame_ecs-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/.gitattributes
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/entity.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/exceptions.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/components/base_component.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/managers/component_manager.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/managers/entity_manager.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/managers/system_manager.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/systems/base_system.py
--rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/circle.png
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/draw_test.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/particle_test_cpu.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/particle_test_gpu.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/speed_test.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/tester.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/LICENSE
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/README.md
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/.gitattributes
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/entity.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/exceptions.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/components/base_component.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/managers/component_manager.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/managers/entity_manager.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/managers/system_manager.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/systems/base_system.py
+-rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/circle.png
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/draw_test.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/particle_test_cpu.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/particle_test_gpu.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/speed_test.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/tester.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/README.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/PKG-INFO
```

### Comparing `pygame_ecs-0.2.0/pygame_ecs/managers/component_manager.py` & `pygame_ecs-0.2.1/pygame_ecs/managers/component_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.0/pygame_ecs/managers/entity_manager.py` & `pygame_ecs-0.2.1/pygame_ecs/managers/entity_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 
 
 class EntityManager:
     def __init__(self) -> None:
         self.count = 0
         self.dead_entities: list[Entity] = []
 
-    def add_entity(self, component_manager: ComponentManager):
+    def add_entity(self):
         if len(self.dead_entities) > 0:
-            entity = Entity(self.dead_entities.pop())
+            entity = self.dead_entities.pop()
         else:
             entity = Entity(self.count)
             self.count += 1
         return entity
 
     def kill_entity(self, component_manager: ComponentManager, entity: Entity):
         self.dead_entities.append(entity)
         for component_type in component_manager.components.keys():
-            del component_manager.components[component_type][entity]
+            try:
+                del component_manager.components[component_type][entity]
+            except KeyError:
+                pass
```

### Comparing `pygame_ecs-0.2.0/pygame_ecs/managers/system_manager.py` & `pygame_ecs-0.2.1/pygame_ecs/managers/system_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.0/pygame_ecs/systems/base_system.py` & `pygame_ecs-0.2.1/pygame_ecs/systems/base_system.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.0/test/circle.png` & `pygame_ecs-0.2.1/test/circle.png`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.0/test/draw_test.py` & `pygame_ecs-0.2.1/test/draw_test.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.0/test/particle_test_cpu.py` & `pygame_ecs-0.2.1/test/particle_test_cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             )
             radius = random.randint(2, 12)
             color = [random.randint(0, 255) for _ in range(3)]
             vel = pygame.math.Vector2(
                 (random.random() - 0.5) * 400 / 1000,
                 (random.random() - 0.5) * 400 / 1000,
             )
-            entity = self.entity_manager.add_entity(self.component_manager)
+            entity = self.entity_manager.add_entity()
             self.component_manager.add_component(entity, Position(center[0], center[1]))
             self.component_manager.add_component(entity, BallRenderer(radius, color))
             if random.randint(0, 1):
                 self.component_manager.add_component(entity, Velocity(vel))
             self.entities.append(entity)
 
     def draw(self):
```

### Comparing `pygame_ecs-0.2.0/test/particle_test_gpu.py` & `pygame_ecs-0.2.1/test/particle_test_gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     radius = random.randint(5, 15)
     color = [random.randint(0, 255) for _ in range(3)]
     color.append(255)
     vel = pygame.math.Vector2(
         (random.random() - 0.5) * 400 / 1000,
         (random.random() - 0.5) * 400 / 1000,
     )
-    entity = entity_manager.add_entity(component_manager)
+    entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
     if random.randint(0, 1):
         component_manager.add_component(entity, Velocity(vel))
     component_manager.add_component(entity, BallRenderer(radius, color))
     entities.append(entity)
```

### Comparing `pygame_ecs-0.2.0/test/speed_test.py` & `pygame_ecs-0.2.1/test/speed_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from timeit import timeit
 import pygame_ecs
 import random
 from sys import argv
 
-cmds = argv[1]
+try:
+    cmds = argv[1]
+except IndexError:
+    cmds = "perfect"
 
 WIDTH = 800
 HEIGHT = 800
 ENTITY_AMOUNT = 1_000 * 5
 
 
 class Position(pygame_ecs.BaseComponent):
@@ -40,32 +43,52 @@
 
 
 entities = []
 entity_manager = pygame_ecs.EntityManager()
 component_manager = pygame_ecs.ComponentManager()
 system_manager = pygame_ecs.SystemManager()
 ball_physics = BallPhysics()
-
 component_manager.init_components()
 
 for _ in range(ENTITY_AMOUNT):
     center = (
         random.randint(0, WIDTH),
         random.randint(0, HEIGHT),
     )
     radius = random.randint(2, 12)
     color = [random.randint(0, 255) for _ in range(3)]
     vel = [
         (random.random() - 0.5) * 400 / 1000,
         (random.random() - 0.5) * 400 / 1000,
     ]
-    entity = entity_manager.add_entity(component_manager)
+    entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
     if cmds[0] != "perfect":
         component_manager.add_component(entity, Velocity(vel))
     entities.append(entity)
 
+for _ in range(1_000):
+    ent = entities[random.randint(0, len(entities) - 1)]
+    entity_manager.kill_entity(component_manager, ent)
+    entities.remove(ent)
+
+for _ in range(2_000):  # ensure that killing and then spawning entities doesnt break anything
+    center = (
+        random.randint(0, WIDTH),
+        random.randint(0, HEIGHT),
+    )
+    radius = random.randint(2, 12)
+    color = [random.randint(0, 255) for _ in range(3)]
+    vel = [
+        (random.random() - 0.5) * 400 / 1000,
+        (random.random() - 0.5) * 400 / 1000,
+    ]
+    entity = entity_manager.add_entity()
+    component_manager.add_component(entity, Position(center[0], center[1]))
+    if cmds[0] != "perfect":
+        component_manager.add_component(entity, Velocity(vel))
+    entities.append(entity)
 
 REPEAT = 1_000
 
 res = timeit(lambda: system_manager.update_entities(entities, component_manager, ball_physics), number=REPEAT)  # type: ignore
-print(f"Took {res/REPEAT} roughly for each frame, using {ENTITY_AMOUNT} entities")
+print(f"Took {res/REPEAT} roughly for each frame, using {len(entities)} entities")
```

### Comparing `pygame_ecs-0.2.0/.gitignore` & `pygame_ecs-0.2.1/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintainted in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
-.VSCodeCounter/
+.VSCodeCounter/
+.vscode/
```

### Comparing `pygame_ecs-0.2.0/LICENSE` & `pygame_ecs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.0/README.md` & `pygame_ecs-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.0/pyproject.toml` & `pygame_ecs-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "pygame_ecs"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Notenlish", email="71970100+Notenlish@users.noreply.github.com" },
 ]
 description = "Pure Python, simple to use Entity Component System(ECS) for pygame"
 packages=["pygame_ecs", "pygame_ecs.components", "pygame_ecs.managers", "pygame_ecs.systems"]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pygame_ecs-0.2.0/PKG-INFO` & `pygame_ecs-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_ecs
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pure Python, simple to use Entity Component System(ECS) for pygame
 Project-URL: Homepage, https://github.com/Notenlish/pygame_ecs
 Project-URL: Bug Tracker, https://github.com/Notenlish/pygame_ecs/issues
 Author-email: Notenlish <71970100+Notenlish@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ECS,component,ecs,entity,entity component system,pygame,pygame-ce,pygame_ecs,system
```

