# Comparing `tmp/pygame_ecs-0.2.1.tar.gz` & `tmp/pygame_ecs-0.2.2.tar.gz`

## Comparing `pygame_ecs-0.2.1.tar` & `pygame_ecs-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/.gitattributes
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/entity.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/exceptions.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/components/base_component.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/managers/component_manager.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/managers/entity_manager.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/managers/system_manager.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pygame_ecs/systems/base_system.py
--rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/circle.png
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/draw_test.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/particle_test_cpu.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/particle_test_gpu.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/speed_test.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/test/tester.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/LICENSE
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/README.md
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pygame_ecs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/.gitattributes
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/entity.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/exceptions.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/components/base_component.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/managers/component_manager.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/managers/entity_manager.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/managers/system_manager.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pygame_ecs/systems/base_system.py
+-rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/circle.png
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/draw_test.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/particle_test_cpu.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/particle_test_gpu.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/speed_test.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/test/tester.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/README.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 pygame_ecs-0.2.2/PKG-INFO
```

### Comparing `pygame_ecs-0.2.1/pygame_ecs/managers/component_manager.py` & `pygame_ecs-0.2.2/pygame_ecs/managers/component_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/pygame_ecs/managers/entity_manager.py` & `pygame_ecs-0.2.2/pygame_ecs/managers/entity_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/pygame_ecs/managers/system_manager.py` & `pygame_ecs-0.2.2/pygame_ecs/managers/system_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/pygame_ecs/systems/base_system.py` & `pygame_ecs-0.2.2/pygame_ecs/systems/base_system.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/test/circle.png` & `pygame_ecs-0.2.2/test/circle.png`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/test/draw_test.py` & `pygame_ecs-0.2.2/test/draw_test.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/test/particle_test_cpu.py` & `pygame_ecs-0.2.2/test/particle_test_cpu.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/test/particle_test_gpu.py` & `pygame_ecs-0.2.2/test/particle_test_gpu.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/test/speed_test.py` & `pygame_ecs-0.2.2/test/speed_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from timeit import timeit
 import pygame_ecs
 import random
 from sys import argv
 
 try:
     cmds = argv[1]
+    if cmds != "perfect":
+        cmds = "imperfect"
 except IndexError:
     cmds = "perfect"
 
 WIDTH = 800
 HEIGHT = 800
 ENTITY_AMOUNT = 1_000 * 5
 
@@ -58,37 +60,41 @@
     color = [random.randint(0, 255) for _ in range(3)]
     vel = [
         (random.random() - 0.5) * 400 / 1000,
         (random.random() - 0.5) * 400 / 1000,
     ]
     entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
-    if cmds[0] != "perfect":
+    if cmds[0] == "imperfect":
         component_manager.add_component(entity, Velocity(vel))
     entities.append(entity)
 
 for _ in range(1_000):
     ent = entities[random.randint(0, len(entities) - 1)]
     entity_manager.kill_entity(component_manager, ent)
     entities.remove(ent)
 
-for _ in range(2_000):  # ensure that killing and then spawning entities doesnt break anything
+for _ in range(
+    2_000
+):  # ensure that killing and then spawning entities doesnt break anything
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
     entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
-    if cmds[0] != "perfect":
+    if cmds[0] == "imperfect":
         component_manager.add_component(entity, Velocity(vel))
     entities.append(entity)
 
 REPEAT = 1_000
 
 res = timeit(lambda: system_manager.update_entities(entities, component_manager, ball_physics), number=REPEAT)  # type: ignore
-print(f"Took {res/REPEAT} roughly for each frame, using {len(entities)} entities")
+print(
+    f"Took {res/REPEAT} roughly for each frame, using {len(entities)} entities, setting: {cmds}"
+)
```

### Comparing `pygame_ecs-0.2.1/.gitignore` & `pygame_ecs-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/LICENSE` & `pygame_ecs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.1/README.md` & `pygame_ecs-0.2.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,126 @@
-# Pygame_ecs
-
-An Pure Python, simple to use ECS library for pygame.
-
-## How it works
-
-Entities are just saved as integers
-
-```python
-entity = entity_manager.add_entity(component_manager)
-```
-
-Components are just classes that hold data
-
-```python
-class Position(pygame_ecs.BaseComponent):
-    def __init__(self, x: int, y: int):
-        super().__init__()
-        self.x = x
-        self.y = y
-```
-
-Systems are just classes that hold logic
-
-```python
-
-class BallPhysics(pygame_ecs.BaseSystem):
-    def __init__(self, screen) -> None:
-        super().__init__(required_component_types=[Position, Velocity])
-        self.dt = 0
-        self.screen = screen
-
-    def update(self, entity_components):
-        pos: Position = entity_components[Position]  # type: ignore
-        vel: Velocity = entity_components[Velocity]  # type: ignore
-        pos.x += vel.vec.x * self.dt  # type: ignore
-        pos.y += vel.vec.y * self.dt  # type: ignore
-        if pos.x > WIDTH or pos.x < 0:
-            vel.vec.x *= -1
-        if pos.y > HEIGHT or pos.y < 0:
-            vel.vec.y *= -1
-
-
-```
-
-## Example Usage
-```py
-
-import pygame
-import pygame_ecs
-import random
-
-class Position(pygame_ecs.BaseComponent):
-    def __init__(self, x: int, y: int):
-        super().__init__()
-        self.x = x
-        self.y = y
-
-class BallRenderer(pygame_ecs.BaseComponent):
-    def __init__(self, radius: int, color) -> None:
-        super().__init__()
-        self.radius = radius
-        self.color = color
-
-class BallDrawSystem(pygame_ecs.BaseSystem):
-    def __init__(self, screen) -> None:
-        super().__init__(required_component_types=[Position, BallRenderer])
-        self.screen = screen
-
-    def update(self, entity_components):
-        pos: Position = entity_components[Position]
-        ball_renderer: BallRenderer = entity_components[BallRenderer]
-        pygame.draw.circle(
-            self.screen, ball_renderer.color, (pos.x, pos.y), ball_renderer.radius
-        )
-
-screen = pygame.display.set_mode((800, 600))
-clock = pygame.time.Clock()
-
-entity_manager = pygame_ecs.EntityManager()
-component_manager = pygame_ecs.ComponentManager()
-system_manager = pygame_ecs.SystemManager()
-ball_draw_system = BallDrawSystem(screen)
-component_manager.init_components()
-
-entities = []
-for _ in range(100):
-    center = (
-        random.randint(0, screen.get_width()),
-        random.randint(0, screen.get_height()),
-    )
-    radius = random.randint(4, 18)
-    color = [random.randint(0, 255) for _ in range(3)]
-    vel = pygame.math.Vector2(
-        (random.random() - 0.5) * 400 / 1000,
-        (random.random() - 0.5) * 400 / 1000,
-    )
-    entity = entity_manager.add_entity(component_manager)
-    component_manager.add_component(entity, Position(center[0], center[1]))
-    component_manager.add_component(entity, BallRenderer(radius, color))
-    entities.append(entity)
-
-while True:
-    for event in pygame.event.get():
-        if event.type == pygame.QUIT:
-            raise SystemExit
-
-    system_manager.update_entities(entities, component_manager, ball_draw_system)
-    pygame.display.update()
-    clock.tick(60)
-    pygame.display.set_caption(f"FPS: {clock.get_fps()}")
-```
-
-# Credits
-
-I'd like to give credit to https://www.youtube.com/watch?v=71RSWVyOMEY and https://github.com/seanfisk/ecs
-As well as `dickerdackel` from pgc server and `SamieZaurus#8030` from UnitOfTime's server.
+# Pygame_ecs
+
+An Pure Python, simple to use ECS library for pygame.
+
+## How it works
+
+Create an entity
+
+```python
+entities = []
+entity = entity_manager.add_entity(component_manager)
+entities.append(entity)
+```
+
+You can delete an entity like this:
+```python
+    entity = entities[random.randint(0, len(entities) - 1)]
+    entity_manager.kill_entity(component_manager, entity)
+    entities.remove(entity)
+```
+
+Components are just classes that hold data
+
+```python
+class Position(pygame_ecs.BaseComponent):
+    def __init__(self, x: int, y: int):
+        super().__init__()
+        self.x = x
+        self.y = y
+```
+
+Systems are just classes that hold logic
+
+```python
+
+class BallPhysics(pygame_ecs.BaseSystem):
+    def __init__(self, screen) -> None:
+        super().__init__(required_component_types=[Position, Velocity])
+        self.dt = 0
+        self.screen = screen
+
+    def update(self, entity_components):
+        pos: Position = entity_components[Position]
+        vel: Velocity = entity_components[Velocity]
+        pos.x += vel.vec.x * self.dt
+        pos.y += vel.vec.y * self.dt
+        if pos.x > WIDTH or pos.x < 0:
+            vel.vec.x *= -1
+        if pos.y > HEIGHT or pos.y < 0:
+            vel.vec.y *= -1
+
+
+```
+
+## Example Usage
+```py
+
+import pygame
+import pygame_ecs
+import random
+
+class Position(pygame_ecs.BaseComponent):
+    def __init__(self, x: int, y: int):
+        super().__init__()
+        self.x = x
+        self.y = y
+
+class BallRenderer(pygame_ecs.BaseComponent):
+    def __init__(self, radius: int, color) -> None:
+        super().__init__()
+        self.radius = radius
+        self.color = color
+
+class BallDrawSystem(pygame_ecs.BaseSystem):
+    def __init__(self, screen) -> None:
+        super().__init__(required_component_types=[Position, BallRenderer])
+        self.screen = screen
+
+    def update(self, entity_components):
+        pos: Position = entity_components[Position]
+        ball_renderer: BallRenderer = entity_components[BallRenderer]
+        pygame.draw.circle(
+            self.screen, ball_renderer.color, (pos.x, pos.y), ball_renderer.radius
+        )
+
+screen = pygame.display.set_mode((800, 600))
+clock = pygame.time.Clock()
+
+entity_manager = pygame_ecs.EntityManager()
+component_manager = pygame_ecs.ComponentManager()
+system_manager = pygame_ecs.SystemManager()
+ball_draw_system = BallDrawSystem(screen)
+component_manager.init_components()
+
+entities = []
+for _ in range(100):
+    center = (
+        random.randint(0, screen.get_width()),
+        random.randint(0, screen.get_height()),
+    )
+    radius = random.randint(4, 18)
+    color = [random.randint(0, 255) for _ in range(3)]
+    vel = pygame.math.Vector2(
+        (random.random() - 0.5) * 400 / 1000,
+        (random.random() - 0.5) * 400 / 1000,
+    )
+    entity = entity_manager.add_entity(component_manager)
+    component_manager.add_component(entity, Position(center[0], center[1]))
+    component_manager.add_component(entity, BallRenderer(radius, color))
+    entities.append(entity)
+
+while True:
+    for event in pygame.event.get():
+        if event.type == pygame.QUIT:
+            raise SystemExit
+
+    system_manager.update_entities(entities, component_manager, ball_draw_system)
+    pygame.display.update()
+    clock.tick(60)
+    pygame.display.set_caption(f"FPS: {clock.get_fps()}")
+```
+
+## Credits
+
+I'd like to give credit to https://www.youtube.com/watch?v=71RSWVyOMEY and https://github.com/seanfisk/ecs
+As well as `dickerdackel` from pgc server and `SamieZaurus#8030` from UnitOfTime's server.
```

### Comparing `pygame_ecs-0.2.1/pyproject.toml` & `pygame_ecs-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "pygame_ecs"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Notenlish", email="71970100+Notenlish@users.noreply.github.com" },
 ]
 description = "Pure Python, simple to use Entity Component System(ECS) for pygame"
 packages=["pygame_ecs", "pygame_ecs.components", "pygame_ecs.managers", "pygame_ecs.systems"]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pygame_ecs-0.2.1/PKG-INFO` & `pygame_ecs-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_ecs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pure Python, simple to use Entity Component System(ECS) for pygame
 Project-URL: Homepage, https://github.com/Notenlish/pygame_ecs
 Project-URL: Bug Tracker, https://github.com/Notenlish/pygame_ecs/issues
 Author-email: Notenlish <71970100+Notenlish@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ECS,component,ecs,entity,entity component system,pygame,pygame-ce,pygame_ecs,system
@@ -26,18 +26,27 @@
 
 # Pygame_ecs
 
 An Pure Python, simple to use ECS library for pygame.
 
 ## How it works
 
-Entities are just saved as integers
+Create an entity
 
 ```python
+entities = []
 entity = entity_manager.add_entity(component_manager)
+entities.append(entity)
+```
+
+You can delete an entity like this:
+```python
+    entity = entities[random.randint(0, len(entities) - 1)]
+    entity_manager.kill_entity(component_manager, entity)
+    entities.remove(entity)
 ```
 
 Components are just classes that hold data
 
 ```python
 class Position(pygame_ecs.BaseComponent):
     def __init__(self, x: int, y: int):
@@ -53,18 +62,18 @@
 class BallPhysics(pygame_ecs.BaseSystem):
     def __init__(self, screen) -> None:
         super().__init__(required_component_types=[Position, Velocity])
         self.dt = 0
         self.screen = screen
 
     def update(self, entity_components):
-        pos: Position = entity_components[Position]  # type: ignore
-        vel: Velocity = entity_components[Velocity]  # type: ignore
-        pos.x += vel.vec.x * self.dt  # type: ignore
-        pos.y += vel.vec.y * self.dt  # type: ignore
+        pos: Position = entity_components[Position]
+        vel: Velocity = entity_components[Velocity]
+        pos.x += vel.vec.x * self.dt
+        pos.y += vel.vec.y * self.dt
         if pos.x > WIDTH or pos.x < 0:
             vel.vec.x *= -1
         if pos.y > HEIGHT or pos.y < 0:
             vel.vec.y *= -1
 
 
 ```
@@ -133,11 +142,11 @@
 
     system_manager.update_entities(entities, component_manager, ball_draw_system)
     pygame.display.update()
     clock.tick(60)
     pygame.display.set_caption(f"FPS: {clock.get_fps()}")
 ```
 
-# Credits
+## Credits
 
 I'd like to give credit to https://www.youtube.com/watch?v=71RSWVyOMEY and https://github.com/seanfisk/ecs
 As well as `dickerdackel` from pgc server and `SamieZaurus#8030` from UnitOfTime's server.
```

