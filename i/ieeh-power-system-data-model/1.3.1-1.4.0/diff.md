# Comparing `tmp/ieeh-power-system-data-model-1.3.1.tar.gz` & `tmp/ieeh-power-system-data-model-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeh-power-system-data-model-1.3.1.tar", last modified: Tue May 23 12:26:16 2023, max compression
+gzip compressed data, was "ieeh-power-system-data-model-1.4.0.tar", last modified: Tue Jun 27 14:03:55 2023, max compression
```

## Comparing `ieeh-power-system-data-model-1.3.1.tar` & `ieeh-power-system-data-model-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      348 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/AUTHORS.md
--rw-r--r--   0        0        0     1568 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/LICENSE
--rw-r--r--   0        0        0     2680 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/README.md
--rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/base.py
--rw-r--r--   0        0        0      579 2023-05-23 12:26:07.077182 ieeh-power-system-data-model-1.3.1/psdm/meta.py
--rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/__init__.py
--rw-r--r--   0        0        0     1047 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/active_power.py
--rw-r--r--   0        0        0     3880 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/case.py
--rw-r--r--   0        0        0     5062 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/controller.py
--rw-r--r--   0        0        0      432 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/external_grid.py
--rw-r--r--   0        0        0      539 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/load.py
--rw-r--r--   0        0        0     1091 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/reactive_power.py
--rw-r--r--   0        0        0      367 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/transformer.py
--rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/__init__.py
--rw-r--r--   0        0        0      491 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/active_power.py
--rw-r--r--   0        0        0     1931 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/branch.py
--rw-r--r--   0        0        0      337 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/characteristic.py
--rw-r--r--   0        0        0      364 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/coupler.py
--rw-r--r--   0        0        0      697 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/external_grid.py
--rw-r--r--   0        0        0     3739 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/load.py
--rw-r--r--   0        0        0     1409 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/load_model.py
--rw-r--r--   0        0        0      320 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/node.py
--rw-r--r--   0        0        0      486 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/reactive_power.py
--rw-r--r--   0        0        0      363 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/switch.py
--rw-r--r--   0        0        0     1011 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/topology.py
--rw-r--r--   0        0        0     2351 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/transformer.py
--rw-r--r--   0        0        0     1081 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/windings.py
--rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology_case/__init__.py
--rw-r--r--   0        0        0      501 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology_case/case.py
--rw-r--r--   0        0        0      399 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology_case/element_state.py
--rw-r--r--   0        0        0     2686 2023-05-23 12:26:07.109185 ieeh-power-system-data-model-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1441 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_active_power.py
--rw-r--r--   0        0        0      659 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_branch.py
--rw-r--r--   0        0        0     8953 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_controller.py
--rw-r--r--   0        0        0     1449 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_reactive_power.py
--rw-r--r--   0        0        0     1606 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_topology_load.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      348 2023-06-27 14:02:54.083710 ieeh-power-system-data-model-1.4.0/AUTHORS.md
+-rw-r--r--   0        0        0     1568 2023-06-27 14:02:54.083710 ieeh-power-system-data-model-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2680 2023-06-27 14:02:54.083710 ieeh-power-system-data-model-1.4.0/README.md
+-rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/__init__.py
+-rw-r--r--   0        0        0     1068 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/base.py
+-rw-r--r--   0        0        0      579 2023-06-27 14:03:46.848663 ieeh-power-system-data-model-1.4.0/psdm/meta.py
+-rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/__init__.py
+-rw-r--r--   0        0        0     1047 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/active_power.py
+-rw-r--r--   0        0        0     3880 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/case.py
+-rw-r--r--   0        0        0     5062 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/controller.py
+-rw-r--r--   0        0        0      432 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/external_grid.py
+-rw-r--r--   0        0        0      539 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/load.py
+-rw-r--r--   0        0        0     1091 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/reactive_power.py
+-rw-r--r--   0        0        0      367 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/transformer.py
+-rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/active_power.py
+-rw-r--r--   0        0        0     1949 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/branch.py
+-rw-r--r--   0        0        0      337 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/characteristic.py
+-rw-r--r--   0        0        0      364 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/coupler.py
+-rw-r--r--   0        0        0      697 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/external_grid.py
+-rw-r--r--   0        0        0      361 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/fuse.py
+-rw-r--r--   0        0        0     4056 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/load.py
+-rw-r--r--   0        0        0     1409 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/load_model.py
+-rw-r--r--   0        0        0      320 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/node.py
+-rw-r--r--   0        0        0      486 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/reactive_power.py
+-rw-r--r--   0        0        0      363 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/switch.py
+-rw-r--r--   0        0        0     1011 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/topology.py
+-rw-r--r--   0        0        0     2351 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/transformer.py
+-rw-r--r--   0        0        0     1081 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/windings.py
+-rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology_case/__init__.py
+-rw-r--r--   0        0        0      501 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology_case/case.py
+-rw-r--r--   0        0        0      399 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology_case/element_state.py
+-rw-r--r--   0        0        0     2686 2023-06-27 14:03:46.872664 ieeh-power-system-data-model-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1441 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_active_power.py
+-rw-r--r--   0        0        0      659 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_branch.py
+-rw-r--r--   0        0        0     8953 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_controller.py
+-rw-r--r--   0        0        0     1449 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_reactive_power.py
+-rw-r--r--   0        0        0     1870 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_topology_load.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.4.0/PKG-INFO
```

### Comparing `ieeh-power-system-data-model-1.3.1/LICENSE` & `ieeh-power-system-data-model-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/README.md` & `ieeh-power-system-data-model-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/base.py` & `ieeh-power-system-data-model-1.4.0/psdm/base.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/active_power.py` & `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/case.py` & `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/case.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/controller.py` & `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/controller.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/load.py` & `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/reactive_power.py` & `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/topology/branch.py` & `ieeh-power-system-data-model-1.4.0/psdm/topology/branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from psdm.base import Base
 from psdm.base import VoltageSystemType
 
 
 class BranchType(Enum):
     LINE = "LINE"
     COUPLER = "COUPLER"
+    FUSE = "FUSE"
 
 
 class Branch(Base):
     node_1: str
     node_2: str
     name: str
     u_n: float  # nominal voltage of the branch connected nodes
```

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/topology/external_grid.py` & `ieeh-power-system-data-model-1.4.0/psdm/topology/external_grid.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/topology/load.py` & `ieeh-power-system-data-model-1.4.0/psdm/topology/load.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,24 @@
 class Phase(enum.Enum):
     A = "A"
     B = "B"
     C = "C"
     N = "N"
 
 
+class PowerType(enum.Enum):
+    AC_APPARENT = "AC_APPARENT"
+    AC_ACTIVE = "AC_ACTIVE"
+    AC_REACTIVE = "AC_REACTIVE"
+    DC = "DC"
+    THERMAL = "THERMAL"
+    GAS = "GAS"
+    MECHANICAL = "MECHANICAL"
+
+
 THRESHOLD = 0.51  # acceptable rounding error (0.5 W) + epsilon for calculation accuracy (0.01 W)
 
 
 def validate_total(values: dict[str, float]) -> dict[str, float]:
     pow_total = values["value_a"] + values["value_b"] + values["value_c"]
     diff = abs(values["value"] - pow_total)
     if diff > THRESHOLD:
@@ -83,34 +93,41 @@
         msg = "Power mismatch: Three-phase power of load is not symmetrical."
         raise ValueError(msg)
 
     return values
 
 
 class RatedPower(Base):
-    value: float = pydantic.Field(..., ge=0)  # rated apparent power; base for p.u. calculation
-    value_a: float = pydantic.Field(..., ge=0)  # rated apparent power (phase a)
-    value_b: float = pydantic.Field(..., ge=0)  # rated apparent power (phase b)
-    value_c: float = pydantic.Field(..., ge=0)  # rated apparent power (phase c)
+    value: float = pydantic.Field(..., ge=0)  # rated power; base for p.u. calculation
+    value_a: float = pydantic.Field(..., ge=0)  # rated power (phase a)
+    value_b: float = pydantic.Field(..., ge=0)  # rated power (phase b)
+    value_c: float = pydantic.Field(..., ge=0)  # rated power (phase c)
     cosphi: float = pydantic.Field(1, ge=0, le=1)  # rated cos(phi) in relation to rated power
     cosphi_a: float = pydantic.Field(1, ge=0, le=1)  # rated cos(phi) (phase a)
     cosphi_b: float = pydantic.Field(1, ge=0, le=1)  # rated cos(phi) (phase b)
     cosphi_c: float = pydantic.Field(1, ge=0, le=1)  # rated cos(phi) (phase c)
+    power_type: PowerType
 
     @pydantic.root_validator(skip_on_failure=True)
     def _validate_total(cls, values: dict[str, float]) -> dict[str, float]:
         return validate_total(values)
 
 
+class ConnectedPhases(Base):
+    phases_a: Sequence[Phase]
+    phases_b: Sequence[Phase]
+    phases_c: Sequence[Phase]
+
+
 class Load(Base):  # including assets of type load and generator
     name: str
     node: str
     u_n: float  # nominal voltage of the connected node
     rated_power: RatedPower
     active_power: ActivePower
     reactive_power: ReactivePower
     type: LoadType  # noqa: A003
-    connected_phases: Sequence[Phase]
+    connected_phases: ConnectedPhases
     system_type: SystemType
     phase_connection_type: PhaseConnectionType
     voltage_system_type: VoltageSystemType
     description: str | None = None
```

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/topology/load_model.py` & `ieeh-power-system-data-model-1.4.0/psdm/topology/load_model.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/topology/topology.py` & `ieeh-power-system-data-model-1.4.0/psdm/topology/topology.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/topology/transformer.py` & `ieeh-power-system-data-model-1.4.0/psdm/topology/transformer.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/psdm/topology/windings.py` & `ieeh-power-system-data-model-1.4.0/psdm/topology/windings.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/pyproject.toml` & `ieeh-power-system-data-model-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "loguru",
     "pydantic",
 ]
 description = "A data model for describing power systems"
 name = "ieeh-power-system-data-model"
 readme = "README.md"
 requires-python = ">=3.10,<3.11"
-version = "1.3.1"
+version = "1.4.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/ieeh-tu-dresden/power-system-data-model"
 
@@ -101,15 +101,15 @@
 
 [tool.black]
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
-version = "1.3.1"
+version = "1.4.0"
 version_files = [
     ".zenodo.json:version",
     "CITATION.cff:cff-version",
     "psdm/meta.py:VERSION",
     "pyproject.toml:version",
 ]
```

### Comparing `ieeh-power-system-data-model-1.3.1/tests/test_active_power.py` & `ieeh-power-system-data-model-1.4.0/tests/test_active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/tests/test_branch.py` & `ieeh-power-system-data-model-1.4.0/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/tests/test_controller.py` & `ieeh-power-system-data-model-1.4.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/tests/test_reactive_power.py` & `ieeh-power-system-data-model-1.4.0/tests/test_reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.1/tests/test_topology_load.py` & `ieeh-power-system-data-model-1.4.0/tests/test_topology_load.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,54 +4,58 @@
 
 from contextlib import nullcontext as does_not_raise
 
 import pydantic
 import pytest
 
 from psdm.topology.load import RatedPower
+from psdm.topology.load import PowerType
 
 
 class TestRatedPower:
     @pytest.mark.parametrize(
         (
             "value",
             "value_a",
             "value_b",
             "value_c",
             "cosphi",
             "cosphi_a",
             "cosphi_b",
             "cosphi_c",
+            "power_type",
             "expectation",
         ),
         [
-            (0, 0, 0, 0, 0, 0, 0, 0, does_not_raise()),
-            (3, 1, 1, 1, 1, 1, 1, 1, does_not_raise()),
-            (4, 2, 1, 1, 1, 1, 1, 1, does_not_raise()),
-            (2, 2, 1, 1, 1, 1, 2, 1, pytest.raises(pydantic.ValidationError)),
-            (2, -2, 1, 1, 1, 1, 1, 1, pytest.raises(pydantic.ValidationError)),
-            (0, -2, 1, 1, 1, 1, 1, 1, pytest.raises(pydantic.ValidationError)),
+            (0, 0, 0, 0, 0, 0, 0, 0, PowerType.AC_APPARENT, does_not_raise()),
+            (3, 1, 1, 1, 1, 1, 1, 1, PowerType.AC_APPARENT, does_not_raise()),
+            (4, 2, 1, 1, 1, 1, 1, 1, PowerType.AC_APPARENT, does_not_raise()),
+            (2, 2, 1, 1, 1, 1, 2, 1, PowerType.AC_APPARENT, pytest.raises(pydantic.ValidationError)),
+            (2, -2, 1, 1, 1, 1, 1, 1, PowerType.AC_APPARENT, pytest.raises(pydantic.ValidationError)),
+            (0, -2, 1, 1, 1, 1, 1, 1, PowerType.AC_APPARENT, pytest.raises(pydantic.ValidationError)),
         ],
     )
     def test_init(  # noqa: PLR0913
         self,
         value,
         value_a,
         value_b,
         value_c,
         cosphi,
         cosphi_a,
         cosphi_b,
         cosphi_c,
+        power_type,
         expectation,
     ) -> None:
         with expectation:
             RatedPower(
                 value=value,
                 value_a=value_a,
                 value_b=value_b,
                 value_c=value_c,
                 cosphi=cosphi,
                 cosphi_a=cosphi_a,
                 cosphi_b=cosphi_b,
                 cosphi_c=cosphi_c,
+                power_type=power_type,
             )
```

### Comparing `ieeh-power-system-data-model-1.3.1/PKG-INFO` & `ieeh-power-system-data-model-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieeh-power-system-data-model
-Version: 1.3.1
+Version: 1.4.0
 Summary: A data model for describing power systems
 Author-email: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>,Laura Fiedler <laura.fiedler1@tu-dresden.de>,Maximilian Schmidt <maximilian.schmidt@tu-dresden.de>,Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 Requires-Python: >=3.10,<3.11
 Project-URL: Source, https://github.com/ieeh-tu-dresden/power-system-data-model
 Description-Content-Type: text/markdown
 
 # IEEH Power System Data Model
```

