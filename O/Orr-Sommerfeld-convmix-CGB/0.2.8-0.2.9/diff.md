# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.2.8.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.2.9.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.2.8.tar` & `orr_sommerfeld_convmix_cgb-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/LICENSE
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    12059 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.9/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.9/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.9/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.9/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.8/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.2.9/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,30 +271,31 @@
         #Expresión de u
         u= (1j*alpha*dot(D,v)/k2) + dot(beta/k2,eta)
         #Expresión de w
         w=((beta*u)-eta)/alpha
     # Falta agregar la presion 
     return  v,u,w,tita
 def normalizacion(v,u,w,tita):
-    vr=v.real
-    vi=v.imag
-    #Busca el valor de màxima norma de u
-    norm= vr*vr+vi*vi
-    i=np.where(abs(norm) == np.max(norm))
-    #Para ese valor máximo, multiplico por un complejo c=a+bj/su fase sea cero y su norma sea 1
-    a=vr[i]/norm[i]
-    b=-vi[i]/norm[i]
-    #a=vi[i]/sqrt(norm[i])
-    #b=-v[i]**2/(vr[i]*sqrt(norm[i]))
-    c= a + (1j*b)   
-    #Luego normalizo todas las autofunciones con el c hallado
-    v=c*v
-    u=c*u
-    w=c*w
-    tita=c*tita
+    if any(v):
+	    vr=v.real
+	    vi=v.imag
+	    #Busca el valor de màxima norma de u
+	    norm= vr*vr+vi*vi
+	    i=np.where(abs(norm) == np.max(norm))
+	    #Para ese valor máximo, multiplico por un complejo c=a+bj/su fase sea cero y su norma sea 1
+	    a=vr[i]/norm[i]
+	    b=-vi[i]/norm[i]
+	    #a=vi[i]/sqrt(norm[i])
+	    #b=-v[i]**2/(vr[i]*sqrt(norm[i]))
+	    c= a + (1j*b)   
+	    #Luego normalizo todas las autofunciones con el c hallado
+	    v=c*v
+	    u=c*u
+	    w=c*w
+	    tita=c*tita
     v= (hstack(( [0.],v , [0.])))
     u= (hstack(( [0.],u , [0.])))
     w= (hstack(( [0.],w , [0.])))
     tita= (hstack(( [0.],tita , [0.])))
     return v,u,w,tita  
 def grafica_autofunciones(N,Ra,Pr,Re,alpha,beta):
     #plt.style.use('ggplot')
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.8/LICENSE` & `orr_sommerfeld_convmix_cgb-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.8/README.md` & `orr_sommerfeld_convmix_cgb-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.8/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.8/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.2.8
+Version: 0.2.9
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Project-URL: Source Code, https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

