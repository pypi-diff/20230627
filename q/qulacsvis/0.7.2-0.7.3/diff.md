# Comparing `tmp/qulacsvis-0.7.2.tar.gz` & `tmp/qulacsvis-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulacsvis-0.7.2.tar", max compression
+gzip compressed data, was "qulacsvis-0.7.3.tar", max compression
```

## Comparing `qulacsvis-0.7.2.tar` & `qulacsvis-0.7.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/LICENSE
--rw-r--r--   0        0        0     4131 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/README.md
--rw-r--r--   0        0        0     1063 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/models/__init__.py
--rw-r--r--   0        0        0     3297 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/models/circuit.py
--rw-r--r--   0        0        0        0 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/qulacs/__init__.py
--rw-r--r--   0        0        0      732 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/qulacs/circuit.py
--rw-r--r--   0        0        0        0 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/utils/__init__.py
--rw-r--r--   0        0        0     2720 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/utils/gate.py
--rw-r--r--   0        0        0     3894 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/utils/latex.py
--rw-r--r--   0        0        0      243 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/__init__.py
--rw-r--r--   0        0        0     4571 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/circuit_drawer.py
--rw-r--r--   0        0        0      603 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/circuit_parser.py
--rw-r--r--   0        0        0     9211 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/latex.py
--rw-r--r--   0        0        0    16211 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/matplotlib.py
--rw-r--r--   0        0        0    34165 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/text.py
--rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 qulacsvis-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4131 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/README.md
+-rw-r--r--   0        0        0     1063 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/models/__init__.py
+-rw-r--r--   0        0        0     3297 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/models/circuit.py
+-rw-r--r--   0        0        0        0 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/qulacs/__init__.py
+-rw-r--r--   0        0        0      732 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/qulacs/circuit.py
+-rw-r--r--   0        0        0        0 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/utils/__init__.py
+-rw-r--r--   0        0        0     2720 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/utils/gate.py
+-rw-r--r--   0        0        0     3894 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/utils/latex.py
+-rw-r--r--   0        0        0      243 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/visualization/__init__.py
+-rw-r--r--   0        0        0     4571 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/visualization/circuit_drawer.py
+-rw-r--r--   0        0        0      603 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/visualization/circuit_parser.py
+-rw-r--r--   0        0        0     9302 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/visualization/latex.py
+-rw-r--r--   0        0        0    17654 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/visualization/matplotlib.py
+-rw-r--r--   0        0        0    34165 2023-06-27 06:14:33.528414 qulacsvis-0.7.3/qulacsvis/visualization/text.py
+-rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 qulacsvis-0.7.3/PKG-INFO
```

### Comparing `qulacsvis-0.7.2/LICENSE` & `qulacsvis-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/README.md` & `qulacsvis-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/pyproject.toml` & `qulacsvis-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qulacsvis"
-version = "0.7.2"
+version = "0.7.3"
 readme = "README.md"
 description = "visualizers for qulacs"
 repository = "https://github.com/Qulacs-Osaka/qulacs-visualizer"
 homepage = "https://github.com/Qulacs-Osaka/qulacs-visualizer"
 documentation = "https://qulacs-osaka.github.io/qulacs-visualizer"
 authors = ["Qulacs-Osaka <you@example.com>"]
 license = "MIT"
```

### Comparing `qulacsvis-0.7.2/qulacsvis/models/circuit.py` & `qulacsvis-0.7.3/qulacsvis/models/circuit.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/qulacsvis/qulacs/circuit.py` & `qulacsvis-0.7.3/qulacsvis/qulacs/circuit.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/qulacsvis/utils/gate.py` & `qulacsvis-0.7.3/qulacsvis/utils/gate.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/qulacsvis/utils/latex.py` & `qulacsvis-0.7.3/qulacsvis/utils/latex.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/qulacsvis/visualization/circuit_drawer.py` & `qulacsvis-0.7.3/qulacsvis/visualization/circuit_drawer.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/qulacsvis/visualization/circuit_parser.py` & `qulacsvis-0.7.3/qulacsvis/visualization/circuit_parser.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/qulacsvis/visualization/latex.py` & `qulacsvis-0.7.3/qulacsvis/visualization/latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,11 +241,15 @@
         Parameters
         ----------
         layer_latex : List[str]
             Array containing the string of the gate of the layer currently of interest
         gate : GateData
             The gate data to be drawn.
         """
-        gate_qcircuit_style = r"\gate{" + to_latex_style(gate.name) + "}"
+        try:
+            gate_qcircuit_style = r"\gate{" + to_latex_style(gate.name) + "}"
+        except KeyError:
+            gate_qcircuit_style = r"\gate{UDF}"
+
         target_bit = gate.target_bits[0]
         layer_latex[target_bit] = gate_qcircuit_style
         self._control_bits(layer_latex, gate.control_bit_infos, target_bit)
```

### Comparing `qulacsvis-0.7.2/qulacsvis/visualization/matplotlib.py` & `qulacsvis-0.7.3/qulacsvis/visualization/matplotlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,37 @@
     "module://matplotlib_inline.backend_inline",
     "nbAgg",
 }
 
 GATE_DEFAULT_WIDTH = 1.0
 GATE_DEFAULT_HEIGHT = 1.5
 
-GATE_MARGIN_RIGHT: Final[float] = 0.5
-GATE_MARGIN_LEFT: Final[float] = 0.5
-GATE_MARGIN_BOTTOM: Final[float] = 0.5
-GATE_MARGIN_TOP: Final[float] = 0.5
+GATE_MARGIN_RIGHT: Final[float] = 0.25
+GATE_MARGIN_LEFT: Final[float] = 0.25
+GATE_MARGIN_BOTTOM: Final[float] = 0.25
+GATE_MARGIN_TOP: Final[float] = 0.25
+
+CIRCUIT_MARGIN = 0.5
 
 PORDER_LINE: Final[int] = 2
 PORDER_GATE: Final[int] = 3
 PORDER_TEXT: Final[int] = 4
 
 
+def _calc_gate_width(gate: GateData) -> float:
+    width = GATE_DEFAULT_WIDTH
+    try:
+        to_latex_style(gate.name)
+    except KeyError:
+        char_width = 0.2
+        width += (len(gate.name) - 3) * char_width
+
+    return width
+
+
 class MPLCircuitlDrawer:
     """
     Drawing a circuit using Matplotlib.
 
     Parameters
     ----------
     circuit : CircuitData
@@ -79,14 +92,32 @@
         self._figure.subplots_adjust(left=0, right=1, bottom=0, top=1)
         self._ax = self._figure.add_subplot(111)
         self._ax.set_aspect("equal")
         self._ax.axis("off")
 
         self._circuit = circuit
         self._fig_scale_factor = scale
+        self._layer_width: List[float] = []
+
+    def _calc_layer_width(self) -> None:
+        circuit_qubit_count = self._circuit.qubit_count
+        circuit_layer_count = self._circuit.layer_count
+
+        for layer in range(circuit_layer_count):
+            max_width = 0.0
+
+            for qubit in range(circuit_qubit_count):
+                gate = self._circuit.gates[qubit][layer]
+                max_width = max(max_width, _calc_gate_width(gate))
+
+            self._layer_width.append(max_width)
+
+        # When the input is an empty quantum circuit
+        if self._layer_width == []:
+            self._layer_width = [GATE_DEFAULT_WIDTH]
 
     def draw(
         self, *, debug: bool = False, filename: Optional[str] = None
     ) -> matplotlib.figure.Figure:
         """
         Draw the circuit.
 
@@ -104,54 +135,57 @@
         """
         if debug:
             self._ax.axis("on")
             self._ax.grid()
 
         circuit_qubit_count = self._circuit.qubit_count
         circuit_layer_count = self._circuit.layer_count
-        layer_width = [GATE_DEFAULT_WIDTH for _ in range(circuit_layer_count)]
-        # When the input is an empty quantum circuit
-        if layer_width == []:
-            layer_width = [GATE_DEFAULT_WIDTH]
+
+        self._calc_layer_width()
+
         # X/Y coordinates of the area where the circuit will be drawn.
         # Used to resize the figure.
         # In particular, the X coordinate is also used
         # as the right end (max_x) and left end (min_x) coordinates of the circuit wire.
         circuit_max_x = (
-            sum(layer_width)
-            + circuit_layer_count * GATE_MARGIN_RIGHT
-            - layer_width[0] / 2
+            sum(self._layer_width)
+            + circuit_layer_count * (GATE_MARGIN_RIGHT + GATE_MARGIN_LEFT)
+            - self._layer_width[0] / 2
         )
-        circuit_min_x = -layer_width[0] / 2 - GATE_MARGIN_LEFT
+        circuit_min_x = -self._layer_width[0] / 2 - GATE_MARGIN_LEFT - GATE_MARGIN_RIGHT
         circuit_max_y = (
-            circuit_qubit_count * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
+            circuit_qubit_count
+            * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_TOP + GATE_MARGIN_BOTTOM)
+            - GATE_MARGIN_TOP
             - GATE_MARGIN_BOTTOM
             - GATE_DEFAULT_HEIGHT / 2
         )
 
         # Determine the size of the figure (drawing size of the circuit + margins)
         QUBIT_LABEL_WIDTH = 2
         self._ax.set_xlim(
-            circuit_min_x - QUBIT_LABEL_WIDTH, circuit_max_x + GATE_MARGIN_RIGHT
+            circuit_min_x - QUBIT_LABEL_WIDTH, circuit_max_x + CIRCUIT_MARGIN
         )
         self._ax.set_ylim(
-            circuit_max_y + GATE_MARGIN_BOTTOM,
-            -GATE_DEFAULT_HEIGHT / 2 - GATE_MARGIN_TOP,
+            circuit_max_y + CIRCUIT_MARGIN,
+            -GATE_DEFAULT_HEIGHT / 2 - CIRCUIT_MARGIN,
         )
 
         # Enlarge/reduce the shape while keeping the aspect ratio
         fig_width = abs(self._ax.get_xlim()[1] - self._ax.get_xlim()[0])
         fig_heigth = abs(self._ax.get_ylim()[1] - self._ax.get_ylim()[0])
         self._figure.set_size_inches(
             fig_width * self._fig_scale_factor, fig_heigth * self._fig_scale_factor
         )
 
         # Draw a Qubit label for the number of Qubits in the quantum circuit and a wire
         for qubit in range(circuit_qubit_count):
-            line_ypos = qubit * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
+            line_ypos = qubit * (
+                GATE_DEFAULT_HEIGHT + GATE_MARGIN_TOP + GATE_MARGIN_BOTTOM
+            )
             self._text(
                 circuit_min_x - 1,
                 line_ypos,
                 r"$q_{" + str(qubit) + r"}$",
                 fontsize=30,
             )
 
@@ -166,15 +200,18 @@
         # x-coordinate of the layer currently being drawn
         layer_xpos = 0.0
 
         # Draw a gate for each layer
         for layer in range(circuit_layer_count):
             for qubit in range(circuit_qubit_count):
                 gate = self._circuit.gates[qubit][layer]
-                qubit_ypos = qubit * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
+                qubit_ypos = qubit * (
+                    GATE_DEFAULT_HEIGHT + GATE_MARGIN_TOP + GATE_MARGIN_BOTTOM
+                )
+
                 if gate.name == "ghost":
                     continue
                 elif gate.name == "wire":
                     continue
                 elif gate.name == "CNOT":
                     self._cnot(gate, (layer_xpos, qubit_ypos))
                 elif gate.name == "Toffoli":
@@ -183,15 +220,20 @@
                     self._swap(gate, (layer_xpos, qubit_ypos))
                 elif len(gate.target_bits) > 1:
                     self._multi_gate(gate, (layer_xpos, qubit_ypos))
                 else:
                     self._gate_with_size(gate, (layer_xpos, qubit_ypos), 1)
 
             # Determine the x-coordinate of the next layer
-            layer_xpos += layer_width[layer] + GATE_MARGIN_RIGHT
+            if layer < circuit_layer_count - 1:
+                layer_xpos += (
+                    (self._layer_width[layer] + self._layer_width[layer + 1]) * 0.5
+                    + GATE_MARGIN_RIGHT
+                    + GATE_MARGIN_LEFT
+                )
 
         if filename:
             self._figure.savefig(
                 filename,
                 # need some options?
             )
 
@@ -304,30 +346,32 @@
         xy : Tuple[float, float]
             The position of the gate with the smallest index among the target bits.
         multi_gate_size : int
             The size of the gate.
         """
 
         xpos, ypos = xy
+        gate_width = _calc_gate_width(gate)
+
         # Find the midpoint of the y-coordinate of the gate with size
         ypos = (
             ypos
             + (
                 ypos
-                + (multi_gate_size - 1) * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
+                + (multi_gate_size - 1)
+                * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM + GATE_MARGIN_TOP)
             )
         ) * 0.5
-        multi_gate_height = (
-            GATE_DEFAULT_HEIGHT * multi_gate_size
-            + GATE_MARGIN_BOTTOM * (multi_gate_size - 1)
-        )
+        multi_gate_height = GATE_DEFAULT_HEIGHT * multi_gate_size + (
+            GATE_MARGIN_BOTTOM + GATE_MARGIN_TOP
+        ) * (multi_gate_size - 1)
         box = patches.Rectangle(
             # The gate is centered.
-            xy=(xpos - 0.5 * GATE_DEFAULT_WIDTH, ypos - 0.5 * multi_gate_height),
-            width=GATE_DEFAULT_WIDTH,
+            xy=(xpos - 0.5 * gate_width, ypos - 0.5 * multi_gate_height),
+            width=gate_width,
             height=multi_gate_height,
             facecolor="w",
             edgecolor="k",
             linewidth=2.4,
             zorder=PORDER_GATE,
         )
         self._ax.add_patch(box)
@@ -359,25 +403,31 @@
 
         multi_gate_data = GateData(gate.name)
 
         groups_of_adjacent_gates = grouping_adjacent_gates(gate.target_bits)
 
         for i, adjacent_gates in enumerate(groups_of_adjacent_gates):
             group_x = xpos
-            group_y = adjacent_gates[0] * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
+            group_y = adjacent_gates[0] * (
+                GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM + GATE_MARGIN_TOP
+            )
             self._gate_with_size(
                 multi_gate_data, (group_x, group_y), len(adjacent_gates)
             )
             if i == 0:
                 # Show the name only for the first group (multi_gate) and hide the rest
                 multi_gate_data.name = ""
 
         # Gray line connecting the gates
-        ypos = min(gate.target_bits) * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
-        to_ypos = max(gate.target_bits) * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
+        ypos = min(gate.target_bits) * (
+            GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM + GATE_MARGIN_TOP
+        )
+        to_ypos = max(gate.target_bits) * (
+            GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM + GATE_MARGIN_TOP
+        )
         self._line((xpos, ypos), (xpos, to_ypos), lw=10, lc="gray")
 
         self._control_bits(gate.control_bit_infos, (xpos, ypos))
 
     def _cnot(self, gate: GateData, xy: Tuple[float, float]) -> None:
         """
         Draw a CNOT gate.
@@ -449,15 +499,17 @@
             The control bits to be drawn.
         xy_from : Tuple[float, float]
             The position of the gate from which the control bits are connected.
         """
 
         for info in control_bit_infos:
             control_bit = info.index
-            to_ypos = control_bit * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_RIGHT)
+            to_ypos = control_bit * (
+                GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM + GATE_MARGIN_TOP
+            )
             to_xpos = xy_from[0]
 
             self._line(
                 xy_from,
                 (to_xpos, to_ypos),
             )
             if info.control_value == 0:
@@ -492,15 +544,17 @@
             The position of the gate with the smaller index among the target bits.
         """
 
         xpos, ypos = xy
         TARGET_QUBIT_MARK_SIZE: Final[float] = 0.2
 
         for target_bit in gate.target_bits:
-            to_ypos = target_bit * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_RIGHT)
+            to_ypos = target_bit * (
+                GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM + GATE_MARGIN_TOP
+            )
             self._line(
                 (xpos, ypos),
                 (xpos, to_ypos),
             )
             # draw target qubit's "x" mark
             # \
             self._line(
```

### Comparing `qulacsvis-0.7.2/qulacsvis/visualization/text.py` & `qulacsvis-0.7.3/qulacsvis/visualization/text.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.2/PKG-INFO` & `qulacsvis-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacsvis
-Version: 0.7.2
+Version: 0.7.3
 Summary: visualizers for qulacs
 Home-page: https://github.com/Qulacs-Osaka/qulacs-visualizer
 License: MIT
 Author: Qulacs-Osaka
 Author-email: you@example.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

