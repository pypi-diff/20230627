# Comparing `tmp/openterrace-0.0.6.tar.gz` & `tmp/openterrace-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openterrace-0.0.6.tar", max compression
+gzip compressed data, was "openterrace-0.0.7.tar", max compression
```

## Comparing `openterrace-0.0.6.tar` & `openterrace-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    35146 2023-03-08 10:37:50.784306 openterrace-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1452 2023-03-08 10:37:50.784306 openterrace-0.0.6/README.md
--rw-r--r--   0        0        0       91 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/__init__.py
--rw-r--r--   0        0        0     2117 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/analytical_functions.py
--rw-r--r--   0        0        0     3021 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/bed_substances/ATS58.py
--rw-r--r--   0        0        0      210 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/bed_substances/__init__.py
--rw-r--r--   0        0        0     1653 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/bed_substances/magnetite.py
--rw-r--r--   0        0        0     1661 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/bed_substances/swedish_diabase.py
--rw-r--r--   0        0        0      210 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/boundary_conditions/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/boundary_conditions/fixedValue.py
--rw-r--r--   0        0        0        0 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/boundary_conditions/timeVaryingFixedValue.py
--rw-r--r--   0        0        0        0 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/boundary_conditions/zeroGradient.py
--rw-r--r--   0        0        0      210 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/convection_schemes/__init__.py
--rw-r--r--   0        0        0      477 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/convection_schemes/upwind_1d.py
--rw-r--r--   0        0        0      210 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/diffusion_schemes/__init__.py
--rw-r--r--   0        0        0      498 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/diffusion_schemes/central_difference_1d.py
--rw-r--r--   0        0        0      210 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/domains/__init__.py
--rw-r--r--   0        0        0     1395 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/domains/block_1d.py
--rw-r--r--   0        0        0     1449 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/domains/cylinder_1d.py
--rw-r--r--   0        0        0     1773 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/domains/hollow_sphere_1d.py
--rw-r--r--   0        0        0     1119 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/domains/lumped.py
--rw-r--r--   0        0        0     1511 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/domains/sphere_1d.py
--rw-r--r--   0        0        0      210 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/fluid_substances/__init__.py
--rw-r--r--   0        0        0     3077 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/fluid_substances/air.py
--rw-r--r--   0        0        0     3250 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/fluid_substances/water.py
--rw-r--r--   0        0        0    14154 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/openterrace.py
--rw-r--r--   0        0        0      210 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/postprocessing/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/postprocessing/animation.py
--rw-r--r--   0        0        0        6 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/postprocessing/panda_dataframe.py
--rw-r--r--   0        0        0     3450 2023-03-08 10:37:50.796306 openterrace-0.0.6/openterrace/tests/test_diffusion.py
--rw-r--r--   0        0        0     1169 2023-03-08 10:38:10.604015 openterrace-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 openterrace-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35146 2023-06-27 11:14:01.697152 openterrace-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1452 2023-06-27 11:14:01.697152 openterrace-0.0.7/README.md
+-rw-r--r--   0        0        0       91 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/__init__.py
+-rw-r--r--   0        0        0     2360 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/analytical_functions.py
+-rw-r--r--   0        0        0     3021 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/bed_substances/ATS58.py
+-rw-r--r--   0        0        0      210 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/bed_substances/__init__.py
+-rw-r--r--   0        0        0     1653 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/bed_substances/magnetite.py
+-rw-r--r--   0        0        0     1661 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/bed_substances/swedish_diabase.py
+-rw-r--r--   0        0        0      210 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/boundary_conditions/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/boundary_conditions/fixedValue.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/boundary_conditions/timeVaryingFixedValue.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/boundary_conditions/zeroGradient.py
+-rw-r--r--   0        0        0      210 2023-06-27 11:14:01.705151 openterrace-0.0.7/openterrace/convection_schemes/__init__.py
+-rw-r--r--   0        0        0      477 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/convection_schemes/upwind_1d.py
+-rw-r--r--   0        0        0      210 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/diffusion_schemes/__init__.py
+-rw-r--r--   0        0        0      498 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/diffusion_schemes/central_difference_1d.py
+-rw-r--r--   0        0        0      210 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/domains/__init__.py
+-rw-r--r--   0        0        0     1400 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/domains/block_1d.py
+-rw-r--r--   0        0        0     1449 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/domains/cylinder_1d.py
+-rw-r--r--   0        0        0     1773 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/domains/hollow_sphere_1d.py
+-rw-r--r--   0        0        0     1128 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/domains/lumped.py
+-rw-r--r--   0        0        0     1511 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/domains/sphere_1d.py
+-rw-r--r--   0        0        0      210 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/fluid_substances/__init__.py
+-rw-r--r--   0        0        0     3077 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/fluid_substances/air.py
+-rw-r--r--   0        0        0     3250 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/fluid_substances/water.py
+-rw-r--r--   0        0        0    15255 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/openterrace.py
+-rw-r--r--   0        0        0      210 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/postprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/postprocessing/animation.py
+-rw-r--r--   0        0        0        6 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/postprocessing/panda_dataframe.py
+-rw-r--r--   0        0        0     3609 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/tests/old.py
+-rw-r--r--   0        0        0     5621 2023-06-27 11:14:01.709151 openterrace-0.0.7/openterrace/tests/test_functions.py
+-rw-r--r--   0        0        0     1169 2023-06-27 11:14:20.077136 openterrace-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 openterrace-0.0.7/PKG-INFO
```

### Comparing `openterrace-0.0.6/LICENSE.txt` & `openterrace-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/README.md` & `openterrace-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/analytical_functions.py` & `openterrace-0.0.7/openterrace/analytical_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 import numpy as np
 from scipy.optimize import brentq
 
-def analytical_wall(Bi:float, Fo:float, n:int):
+def analytical_step(X:float, n=int):
+    y_H_arr = np.linspace(0,1,n)
+    theta_arr = np.zeros(n)
+    
+    indices = [i for i,y_H in enumerate(y_H_arr) if y_H >= X]
+    theta_arr[indices] = 1
+    return y_H_arr, theta_arr
+
+def analytical_diffusion_wall(Bi:float, Fo:float, n:int):
     def theta_fcn(Bi:float, Fo:float, r_r0:float, n_terms:int=100):
         def lambda_fcn(Bi, i):
             left = np.pi*i
             right = left + np.pi/2 - 1e-12
             return brentq(lambda x: x*np.tan(x)-Bi, left, right)
 
         theta = 0
@@ -22,15 +30,15 @@
     theta_arr = []
     x_x0_arr = np.linspace(0,1,n)
     for x_x0 in x_x0_arr:
         theta = theta_fcn(Bi, Fo, x_x0)
         theta_arr.append(theta)
     return x_x0_arr, theta_arr
 
-def analytical_sphere(Bi:float, Fo:float, n:int):
+def analytical_diffusion_sphere(Bi:float, Fo:float, n:int):
     def theta_fcn(Bi:float, Fo:float, r_r0:float, n_terms:int=100):
         def lambda_fcn(Bi, i):
             left = np.pi*(i) + 1e-12
             right = np.pi*(i+1) - 1e-12
             return brentq(lambda x: 1-x/np.tan(x)-Bi, left, right)
 
         theta = 0
```

### Comparing `openterrace-0.0.6/openterrace/bed_substances/ATS58.py` & `openterrace-0.0.7/openterrace/bed_substances/ATS58.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/bed_substances/magnetite.py` & `openterrace-0.0.7/openterrace/bed_substances/magnetite.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/bed_substances/swedish_diabase.py` & `openterrace-0.0.7/openterrace/bed_substances/swedish_diabase.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/domains/block_1d.py` & `openterrace-0.0.7/openterrace/domains/block_1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 def shape(vars):
     """Shape function.
 
     Args:
         vars (list): List of arguments
     """
+    
     n = vars['n']
     return np.array([n])
 
 def dx(vars):
     """Node spacing function.
 
     Args:
```

### Comparing `openterrace-0.0.6/openterrace/domains/cylinder_1d.py` & `openterrace-0.0.7/openterrace/domains/cylinder_1d.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/domains/hollow_sphere_1d.py` & `openterrace-0.0.7/openterrace/domains/hollow_sphere_1d.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/domains/lumped.py` & `openterrace-0.0.7/openterrace/domains/lumped.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 def A(vars):
     """Cross-sectional area for faces of node.
 
     Args:
         vars (list): List of arguments
     """
 
-    return (np.repeat(0,1), np.repeat(0,1))
+    A = vars['A']
+    return np.array([[0,0],[0,A]])
 
 def V(vars):
     """Volume of node element.
 
     Args:
         vars (list): List of arguments
     """
```

### Comparing `openterrace-0.0.6/openterrace/domains/sphere_1d.py` & `openterrace-0.0.7/openterrace/domains/sphere_1d.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/fluid_substances/air.py` & `openterrace-0.0.7/openterrace/fluid_substances/air.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Data for atmospheric air.
 
 Reference 1: Eric W. Lemmon, Richard T. Jacobsen, Steven G. Penoncello, and Daniel G. Friend. Thermodynamic Properties of Air and Mixtures of Nitrogen, Argon, and Oxygen from 60 to 2000 K at Pressures to 2000 MPa. J. Phys. Chem. Ref. Data, 29(3):331–385, 2000. doi:10.1063/1.1285884.
 Reference 2: E. W. Lemmon and R. T Jacobsen. Viscosity and Thermal Conductivity Equations for Nitrogen, Oxygen, Argon, and Air. Int. J. Thermophys., 25(1):21–69, 2004. doi:10.1023/B:IJOT.0000022327.04529.f3.
 """
 
 def h(T:float) -> float:
-    """Mass specific enthalpy as function of temperature at 1 atm (fit valid between 273.15 K to 2000 K).
+    """Mass specific enthalpy as function of temperature at 1 atm (fit valid between 273.15 K to 1000 K).
 
     Args:
         T (float): Temperature in K
 
     Returns:
         Mass specific enthalpy in J/kg
     """
```

### Comparing `openterrace-0.0.6/openterrace/fluid_substances/water.py` & `openterrace-0.0.7/openterrace/fluid_substances/water.py`

 * *Files identical despite different names*

### Comparing `openterrace-0.0.6/openterrace/openterrace.py` & `openterrace-0.0.7/openterrace/openterrace.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,59 +3,68 @@
 from . import bed_substances
 from . import domains
 from . import diffusion_schemes
 from . import convection_schemes
 from . import boundary_conditions
 
 # Import common Python modules
-import sys
 import tqdm
 import numpy as np
 import matplotlib
+import datetime
 matplotlib.use('agg')
 import matplotlib.pyplot as plt
 import matplotlib.animation as anim
 
 class Simulate:
     """OpenTerrace class."""
-    def __init__(self, t_end:float=None, dt:float=None, n_fluid:int=50, n_bed:int=5):
+    def __init__(self, t_end:float=None, dt:float=None, sim_name:str=None):
         """Initialise with various control parameters.
 
         Args:
             t_end (float): End time in s
             dt (float): Time step size in s
-            n_fluid (int): Number of discretisations for fluid phase
-            n_bed (int): Number of discretisations for bed phase
         """
         self.t_start = 0
         self.t_end = t_end
         self.dt = dt
-        self.fluid = self.Phase(n=n_fluid, n2=1, _type='fluid')
-        self.bed = self.Phase(n=n_bed, n2=n_fluid, _type='bed')
-        self.sources = []
-        self.coupling = False
-        self.saved_data = []
-        self.output_animation_flag = False
-        self.save_flag = []
+        self.coupling = []
+        self.flag_coupling = False
+        self.sim_name = sim_name
         
     class Phase:
+        instances = []
         """Main class to define either the fluid or bed phase."""
-        def __init__(self, n:int=None, n2:int=None, _type:str=None):
+        def __init__(self, n:int=None, n_other:int=1, type:str=None):
+            """Initialise a phase with number of control points and type.
+
+            Args:
+                n_self (int): Number of discretisations for the given phase
+                n_other (int): Number of discretisations for the other phase
+                type (str): Type of phase
+            """
+            self.__class__.instances.append(self)
             self.n = n
-            self.n2 = n2
-            self._type = _type
+            self.n_other = n_other
+            
+            self.phi = 1
+
             self.bcs = []
             self.sources = []
-            self.postprocess = []
-            self.phi = 1
-            self._valid_inputs(_type)
 
-        def _valid_inputs(self, _type:str):
+            self._flag_save_data = False
+ 
+            self.type = type
+            self._valid_inputs(type)
+
+        def _valid_inputs(self, type:str=None):
+            """Gets valid domain and substances depending on type of phase.
+            """
             self.valid_domains = globals()['domains'].__all__
-            self.valid_substances = globals()[self._type+'_substances'].__all__
+            self.valid_substances = globals()[type+'_substances'].__all__
 
         def select_substance_on_the_fly(self, cp:float=None, rho:float=None, k:float=None):
             """Defines and selects a new substance on-the-fly. This is useful for defining a substance for testing purposes with temperature independent properties.
 
             Args:
                 cp (float): Specific heat capacity in J/(kg K)
                 rho (float): Density in kg/m^3
@@ -75,16 +84,16 @@
 
             Args:
                 substance (str): Substance name
             """
             if not substance:
                 raise Exception("Keyword 'substance' not specified.")
             if not substance in self.valid_substances:
-                raise Exception(substance+" specified as "+self._type+" substance. Valid "+self._type+" substances are:", self.valid_substances)
-            self.fcns = getattr(globals()[self._type+'_substances'], substance)
+                raise Exception(substance+" specified as "+self.type+" substance. Valid "+self.type+" substances are:", self.valid_substances)
+            self.fcns = getattr(globals()[self.type+'_substances'], substance)
 
         def select_domain_shape(self, domain:str=None, **kwargs):
             """Select domain shape and initialise constants."""
             kwargs['n'] = self.n
             if not domain:
                 raise Exception("Keyword 'domain' not specified.")
             if not domain in globals()['domains'].__all__:
@@ -103,15 +112,15 @@
             self.domain.V = self.domain.V*phi
             self.phi = phi
 
         def select_schemes(self, diff:str=None, conv:str=None):
             """Imports the specified diffusion and convection schemes."""
 
             if self.domain.type == 'lumped':
-                raise Exception("'lumped' has been selected as domain type. Please don't try discretising it.")
+                raise Exception("'lumped' has been selected as domain type. Please don't specify a discretisation scheme.")
 
             if diff is not None:
                 try:
                     self.diff = getattr(getattr(globals()['diffusion_schemes'], diff), diff)
                 except:
                     raise Exception("Diffusion scheme \'"+diff+"\' specified. Valid options for diffusion schemes are:", diffusion_schemes.__all__)
 
@@ -120,18 +129,18 @@
                     self.conv = getattr(getattr(globals()['convection_schemes'], conv), conv)
                 except:
                     raise Exception("Convection scheme \'"+conv+"\' specified. Valid options for convection schemes are:", convection_schemes.__all__)
 
         def select_initial_conditions(self, T:float=None, mdot:float=None):
             """Initialises temperature and massflow fields"""
             if T is not None:
-                self.T = np.tile(T,(np.append(self.n2,self.domain.shape)))
+                self.T = np.tile(T,(np.append(self.n_other,self.domain.shape)))
                 self.h = self.fcns.h(self.T)
             if mdot is not None:
-                self.mdot = np.tile(mdot,(np.append(self.n2,self.domain.shape)))
+                self.mdot = np.tile(mdot,(np.append(self.n_other,self.domain.shape)))
             self.T = self.fcns.T(self.h)
             self.rho = self.fcns.rho(self.h)
             self.cp = self.fcns.cp(self.h)
             self.k = self.fcns.k(self.h)
             self.D = np.zeros(((2,)+(self.T.shape)))
             self.F = np.zeros(((2,)+(self.T.shape)))
             self.S = np.zeros(self.T.shape)
@@ -157,14 +166,73 @@
             if kwargs['source_type'] == 'thermal_resistance':
                 required = ['R','T_inf', 'position']
                 for var in required:
                     if not var in kwargs:
                         raise Exception("Keyword \'"+var+"\' not specified for source of type \'"+kwargs['source_type']+"\'")
             self.sources.append(kwargs)
 
+        def select_output(self, times:list[float]=None, parameters:list[str]=None):
+            class Data(object):
+                pass
+            self.data = Data()
+            self.data.time = np.array(times)
+            self.data.parameters = parameters
+            for parameter in parameters:
+                setattr(self.data,parameter,np.zeros((len(times), self.n_other, self.n)))
+                self._flag_save_data = True
+                self._q = 0
+
+        def _save_data(self, t:float=None):
+            if self._flag_save_data:
+                if t in self.data.time:
+                    self.data.time[self._q] = t
+                    for parameter in self.data.parameters: 
+                        getattr(self.data,parameter)[self._q] = getattr(self,parameter)
+                        self._q = self._q+1
+
+        def _create_plot(self, sim_name=None):
+            for parameter in self.data.parameters:
+                filename='OpenTerrace_'+sim_name+'_'+datetime.datetime.now().strftime("%Y-%m-%d_%H%M")+'_'+self.type+'_'+parameter+'.png'
+                fig, ax = plt.subplots()
+                fig.tight_layout(pad=2)
+
+                ax.plot(self.domain.node_pos, np.mean(getattr(self.data,parameter),1).transpose())
+                plt.grid()
+                plt.xlabel('Position (m)')
+                plt.ylabel('$%s_{%s}$' % (parameter, self.type))
+                plt.legend(['$\it{t}$ = '+str(s)+' s' for s in getattr(self.data,'time')], loc='lower right')
+                plt.savefig(filename)
+                
+
+        def _create_animation(self):
+            def _update(frame):
+                x = xdata
+                y = ydata[frame]
+                ax.clear()
+                ax.set_xlim(xmin, xmax)
+                ax.set_ylim(ymin, ymax)
+                ax.set_xlabel('Position (m)')
+                ax.set_ylabel('Temperature (C)')
+                ax.grid()
+                ax.plot(x, y.T-273.15, color = '#4cae4f')
+                ax.text(.05, .95, 'Simulated with OpenTerrace', ha='left', va='top', transform=ax.transAxes, color = '#4cae4f',
+                    bbox=dict(facecolor='white',boxstyle="square,pad=0.5", alpha=0.5))
+                ax.set_title('Time: ' + str(np.round(self.saved_time_data[frame], decimals=2)) + ' s')
+
+            for parameter in self.data.parameters:
+                fig, ax = plt.subplots()
+                fig.tight_layout(pad=2)
+                ymin = np.min(ydata)-273.15
+                ymax = np.max(ydata)-273.15
+                xmin = np.min(xdata)
+                xmax = np.max(xdata)
+
+                ani = anim.FuncAnimation(fig, _update, frames=np.arange(int(np.floor(self.t_end/(self.dt*self.save_int)))))
+                ani.save(self.file_name+'_'+phase+'.gif', writer=anim.PillowWriter(fps=10),progress_callback=lambda i, n: print(f'{phase}: saving animation frame {i}/{n}'))
+
         def _update_properties(self):
             """Updates properties based on specific enthalpy"""
             self.T = self.fcns.T(self.h)
             self.rho = self.fcns.rho(self.h)
             self.cp = self.fcns.cp(self.h)
 
             if hasattr(self, 'diff'):
@@ -172,127 +240,67 @@
                 self.D[0,:,:] = self.k*self.domain.A[0]/self.domain.dx
                 self.D[1,:,:] = self.k*self.domain.A[1]/self.domain.dx
 
             if hasattr(self, 'conv'):
                 self.F[0,:,:] = self.mdot*self.cp
                 self.F[1,:,:] = self.mdot*self.cp
 
-        def _update_boundary_nodes(self, t, dt):
+        def _update_boundary_nodes(self, t:float=None, dt:float=None):
             """Update boundary nodes"""
             for bc in self.bcs:
                 if bc['type'] == 'dirichlet':
                     self.h[bc['position']] = self.fcns.h(bc['value'])
                 if bc['type'] == 'dirichlet_timevarying':
                     self.h[bc['position']] = self.fcns.h(np.interp(t,bc['value'][:,0],bc['value'][:,1]))
                 if bc['type'] == 'neumann':
                     if bc['position'] == np.s_[:,0]:
                         self.h[bc['position']] = self.h[bc['position']] + (2*self.T[:,1]*self.D[1,:,0] - 2*self.T[:,0]*self.D[1,:,0] - self.F[0,:,1]*self.T[:,1] + self.F[1,:,0]*self.T[:,0]) / (self.rho[:,0]*self.domain.V[0])*dt
                     if bc['position'] == np.s_[:,-1]:
                         self.h[bc['position']] = self.h[bc['position']] + (2*self.T[:,-2]*self.D[0,:,-1] - 2*self.T[:,-1]*self.D[0,:,-1] + self.F[1,:,-2]*self.T[:,-2] - self.F[0,:,-1]*self.T[:,-1]) / (self.rho[:,-1]*self.domain.V[-1])*dt
 
-        def _update_source(self, dt):
+        def _update_source(self, dt:float=None):
             for source in self.sources:
                 if source['source_type'] == 'thermal_resistance':
                     self.h[source['position']] = self.h[source['position']] + (2/source['R'] * (source['T_inf']-self.T[source['position']])) / (self.rho[source['position']]*self.domain.V[source['position'][1]])*dt
 
-        def _solve_equations(self, t, dt):
+        def _solve_equations(self, t:float=None, dt:float=None):
             self._update_boundary_nodes(t, dt)
             if hasattr(self, 'diff'):
                 self.h = self.h + self.diff(self.T, self.D)/(self.rho*self.domain.V)*dt
             if hasattr(self, 'conv'):
                 self.h = self.h + self.conv(self.T, self.F)/(self.rho*self.domain.V)*dt
             if self.sources is not None:
                 self._update_source(dt)
 
-        def select_output(self, output_type:str=None, times:list[float]=None, file_name:str='openterrace_animation_'):
-            self.postprocess.append({'type': output_type, 'time': np.array(times), 'data': np.zeros((len(times), self.n)), 'file_name': file_name})
-
-        def _prepare_output(self, t_start, t_end, dt):
-            for pp in self.postprocess:
-                print(pp)
-
-    def select_coupling(self, h_coeff=None, h_value=None):
-        self.coupling = True
-        valid_h_coeff = ['constant']
-        if h_coeff not in valid_h_coeff:
-            raise Exception("h_coeff \'"+h_coeff+"\' specified. Valid options for h_coeff are:", valid_h_coeff)
-        if h_coeff == 'constant':
-            self.h_value = h_value
-
-    def _couple(self):
-        Q = self.h_value*self.bed.domain.A[-1][-1]*(self.fluid.T[0]-self.bed.T[:,-1])*self.dt
-        self.bed.h[:,-1] = self.bed.h[:,-1] + Q/(self.bed.rho[:,-1]*self.bed.domain.V[-1])
-        self.fluid.h[0] = self.fluid.h[0] - (1-self.fluid.phi)*(self.fluid.domain.V/self.fluid.phi) / np.sum(self.bed.domain.V) * Q/(self.fluid.rho*self.fluid.domain.V)
-
-    def _create_animation(self, phase=None, xdata=None, ydata=None):
-        fig, ax = plt.subplots()
-        fig.tight_layout(pad=2)
-        ymin = np.min(ydata)-273.15
-        ymax = np.max(ydata)-273.15
-        xmin = np.min(xdata)
-        xmax = np.max(xdata)
-
-        def _update(frame):
-            x = xdata
-            y = ydata[frame]
-            ax.clear()
-            ax.set_xlim(xmin, xmax)
-            ax.set_ylim(ymin, ymax)
-            ax.set_xlabel('Position (m)')
-            ax.set_ylabel('Temperature (C)')
-            ax.grid()
-            ax.plot(x, y.T-273.15, color = '#4cae4f')
-            ax.text(.05, .95, 'Simulated with OpenTerrace', ha='left', va='top', transform=ax.transAxes, color = '#4cae4f',
-                bbox=dict(facecolor='white',boxstyle="square,pad=0.5", alpha=0.5))
-            ax.set_title('Time: ' + str(np.round(self.saved_time_data[frame], decimals=2)) + ' s')
+    def select_coupling(self, fluid_phase:int=None, bed_phase:int=None, h_exp:str=None, h_value:float=None):
+        valid_h_exp = ['constant']
+        if h_exp not in valid_h_exp:
+            raise Exception("h_exp \'"+h_exp+"\' specified. Valid options for h_exp are:", valid_h_exp)
+        
+        self.coupling.append({"fluid_phase":fluid_phase, "bed_phase":bed_phase, "h_exp":h_exp, "h_value":h_value})
+        self.flag_coupling = True
 
-        ani = anim.FuncAnimation(fig, _update, frames=np.arange(int(np.floor(self.t_end/(self.dt*self.save_int)))))
-        ani.save(self.file_name+'_'+phase+'.gif', writer=anim.PillowWriter(fps=10),progress_callback=lambda i, n: print(f'{phase}: saving animation frame {i}/{n}'))
+    def _coupling(self):
+        for couple in self.coupling:
+            Q = couple['h_value']*self.Phase.instances[couple['bed_phase']].domain.A[-1][-1]*(self.Phase.instances[couple['fluid_phase']].T[0]-self.Phase.instances[couple['bed_phase']].T[:,-1])*self.dt
+            self.Phase.instances[couple['bed_phase']].h[:,-1] = self.Phase.instances[couple['bed_phase']].h[:,-1] + Q/(self.Phase.instances[couple['bed_phase']].rho[:,-1] * self.Phase.instances[couple['bed_phase']].domain.V[-1])
+            self.Phase.instances[couple['fluid_phase']].h[0] = self.Phase.instances[couple['fluid_phase']].h[0] - (1-self.Phase.instances[couple['fluid_phase']].phi)*(self.Phase.instances[couple['fluid_phase']].domain.V * self.Phase.instances[couple['fluid_phase']].phi) / np.sum(self.Phase.instances[couple['bed_phase']].domain.V) * Q/(self.Phase.instances[couple['fluid_phase']].rho*self.Phase.instances[couple['fluid_phase']].domain.V)
 
     def run_simulation(self):
         """This is the function full of magic."""
-
-        if self.fluid.postprocess:
-            self.fluid._prepare_output(self.t_start, self.t_end, self.dt)
-
-        if self.bed.postprocess:
-            self.bed._prepare_output(self.t_start, self.t_end, self.dt)
-        #         self.fluid._prepare_output(self.t_start, self.t_end, self.dt)
-
-        # if hasattr(self.bed, 'postprocess'):
-        #     if self.bed.postprocess:
-        #         self.bed._prepare_output(self.t_start, self.t_end, self.dt)
-
-        # sys.exit()
-
-        i = 0
-        for t in tqdm.tqdm(np.arange(self.t_start, self.t_end, self.dt)):
-            if hasattr(self.fluid, 'T'):
-                self.fluid._solve_equations(t, self.dt)
-                self.fluid._update_properties()
-                if self.fluid.postprocess:
-                    pass
-                    
-            if hasattr(self.bed, 'T'):
-                self.bed._solve_equations(t, self.dt)
-                self.bed._update_properties()
-
-            if self.coupling:
-                self._couple()
-
-            if hasattr(self.fluid, 'animation_output_flag'):
-
-
-
-                if np.mod(i, self.save_int) == 0:
-                    self.saved_time_data[int(i/self.save_int)] = t
-                    if hasattr(self.bed, 'T'):
-                        self.saved_bed_data[int(i/self.save_int),:,:] = self.bed.T
-                    if hasattr(self.fluid, 'T'):
-                        self.saved_fluid_data[int(i/self.save_int),:] = self.fluid.T
-            i = i+1
-
-        if self.output_animation_flag:
-            if hasattr(self.bed, 'T'):
-                self._create_animation(phase='bed', xdata=self.bed.domain.node_pos, ydata=self.saved_bed_data)
-            if hasattr(self.fluid, 'T'):
-                self._create_animation(phase='fluid', xdata=self.fluid.domain.node_pos, ydata=self.saved_fluid_data)
+        for t in tqdm.tqdm(np.arange(self.t_start, self.t_end+self.dt, self.dt)):
+            for phase_instance in self.Phase.instances:
+                phase_instance._solve_equations(t, self.dt)
+                phase_instance._update_properties()
+                phase_instance._save_data(t)
+            if self.flag_coupling:
+                self._coupling()
+
+    def generate_plots(self):
+        for phase_instance in self.Phase.instances:
+            if phase_instance._flag_save_data:
+                phase_instance._create_plot(self.sim_name)
+
+    def generate_animations(self):
+        for phase_instance in self.Phase.instances:
+            if phase_instance._flag_save_data:
+                phase_instance._create_animation()
```

### Comparing `openterrace-0.0.6/openterrace/tests/test_diffusion.py` & `openterrace-0.0.7/openterrace/tests/old.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import openterrace
 import numpy as np
 import matplotlib.pyplot as plt
+import datetime
+import pathlib
+
+print(pathlib.Path(__file__).parent.resolve())
 
 def test_diffusion_sphere():
     n = 50
     t_end = 200
 
     Lc = 0.025
     T_init = 0
     T_inf = 100
     h = 200
     cp = 4179
     rho = 993
     k = 0.627
 
-    ot = openterrace.Simulate(t_end=t_end, dt=1e-2, n_bed=n)
+    ot = openterrace.Simulate(t_end=t_end, dt=1e-2)
+    ot.bed = ot.Phase(n=n, type='bed')
     ot.bed.select_substance_on_the_fly(cp=cp, rho=rho, k=k)
     ot.bed.select_domain_shape(domain='sphere_1d', R=Lc)
     ot.bed.select_schemes(diff='central_difference_1d')
     ot.bed.select_initial_conditions(T=T_init)
     ot.bed.select_bc(bc_type='neumann', parameter='T', position=(slice(None, None, None), 0))
     ot.bed.select_bc(bc_type='neumann', parameter='T', position=(slice(None, None, None), -1))
     ot.bed.select_source_term(source_type='thermal_resistance', R=1/(h*4*np.pi*Lc**2), T_inf=T_inf, position=(slice(None, None, None), -1))
     ot.run_simulation()
 
     Bi = h*Lc/k
     Fo = k/(rho*cp)*t_end/Lc**2
 
-    r_r0_ana, theta_ana = openterrace.analytical_sphere(Bi, Fo, n)
+    r_r0_ana, theta_ana = openterrace.analytical_diffusion_sphere(Bi, Fo, n)
     r_r0_num, theta_num = ot.bed.domain.node_pos/(ot.bed.domain.node_pos[-1]-ot.bed.domain.node_pos[0]), (ot.bed.T[0,:]-T_inf)/(T_init-T_inf)
 
     plt.plot(r_r0_num, theta_num,'s', label='OpenTerrace', color = '#4cae4f')
     plt.plot(r_r0_ana, theta_ana,'k', label='Analytical')
     plt.xlim([0, 1])
     plt.ylim([0, 1])
     plt.grid()
@@ -52,28 +57,29 @@
     T_inf = 100
     h = 200
     cp = 4179
     rho = 993
     k = 0.627
     A = 1
 
-    ot = openterrace.Simulate(t_end=t_end, dt=1e-2, n_bed=n)
+    ot = openterrace.Simulate(t_end=t_end, dt=1e-2)
+    ot.bed = ot.Phase(n=n, type='bed')
     ot.bed.select_substance_on_the_fly(cp=cp, rho=rho, k=k)
     ot.bed.select_domain_shape(domain='block_1d', L=Lc, A=A)
     ot.bed.select_schemes(diff='central_difference_1d')
     ot.bed.select_initial_conditions(T=T_init)
     ot.bed.select_bc(bc_type='neumann', parameter='T', position=(slice(None, None, None), 0))
     ot.bed.select_bc(bc_type='neumann', parameter='T', position=(slice(None, None, None), -1))
     ot.bed.select_source_term(source_type='thermal_resistance', R=1/(h*A), T_inf=T_inf, position=(slice(None, None, None), -1))
     ot.run_simulation()
 
     Bi = h*Lc/k
     Fo = k/(rho*cp)*t_end/Lc**2
 
-    x_x0_ana, theta_ana = openterrace.analytical_wall(Bi, Fo, n)
+    x_x0_ana, theta_ana = openterrace.analytical_diffusion_wall(Bi, Fo, n)
     x_x0_num, theta_num = ot.bed.domain.node_pos/(ot.bed.domain.node_pos[-1]-ot.bed.domain.node_pos[0]), (ot.bed.T[0,:]-T_inf)/(T_init-T_inf)
 
     plt.plot(x_x0_num, theta_num,'s', label='OpenTerrace', color = '#4cae4f')
     plt.plot(x_x0_ana, theta_ana,'k', label='Analytical')
     plt.xlim([0, 1])
     plt.ylim([0, 1])
     plt.grid()
```

### Comparing `openterrace-0.0.6/pyproject.toml` & `openterrace-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openterrace"
 description = "OpenTerrace is a pure Python framework for thermal energy storage packed bed simulations"
-version = "v0.0.6"
+version = "v0.0.7"
 authors = [
     "Jakob Hærvig"
 ]
 readme = "README.md"
 license = "MIT"
 
 packages = [
```

### Comparing `openterrace-0.0.6/PKG-INFO` & `openterrace-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openterrace
-Version: 0.0.6
+Version: 0.0.7
 Summary: OpenTerrace is a pure Python framework for thermal energy storage packed bed simulations
 Home-page: https://github.com/OpenTerrace/openterrace-python
 License: MIT
 Author: Jakob Hærvig
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

