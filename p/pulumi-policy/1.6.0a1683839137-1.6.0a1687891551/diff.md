# Comparing `tmp/pulumi_policy-1.6.0a1683839137-py2.py3-none-any.whl.zip` & `tmp/pulumi_policy-1.6.0a1687891551-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15498 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1483 b- defN 23-May-11 21:15 pulumi_policy/__init__.py
--rw-r--r--  2.0 unx     3849 b- defN 23-May-11 21:15 pulumi_policy/deserialize.py
--rw-r--r--  2.0 unx    39992 b- defN 23-May-11 21:15 pulumi_policy/policy.py
--rw-r--r--  2.0 unx     6833 b- defN 23-May-11 21:15 pulumi_policy/proxy.py
--rw-r--r--  2.0 unx       22 b- defN 23-May-11 21:15 pulumi_policy/pulumiplugin.json
--rw-r--r--  2.0 unx        0 b- defN 23-May-11 21:15 pulumi_policy/py.typed
--rw-r--r--  2.0 unx      634 b- defN 23-May-11 21:15 pulumi_policy/version.py
--rw-r--r--  2.0 unx     2339 b- defN 23-May-11 21:15 pulumi_policy-1.6.0a1683839137.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-11 21:15 pulumi_policy-1.6.0a1683839137.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-11 21:15 pulumi_policy-1.6.0a1683839137.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      936 b- defN 23-May-11 21:15 pulumi_policy-1.6.0a1683839137.dist-info/RECORD
-11 files, 56212 bytes uncompressed, 13898 bytes compressed:  75.3%
+Zip file size: 15502 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1483 b- defN 23-Jun-27 18:47 pulumi_policy/__init__.py
+-rw-r--r--  2.0 unx     3849 b- defN 23-Jun-27 18:47 pulumi_policy/deserialize.py
+-rw-r--r--  2.0 unx    39992 b- defN 23-Jun-27 18:47 pulumi_policy/policy.py
+-rw-r--r--  2.0 unx     6833 b- defN 23-Jun-27 18:47 pulumi_policy/proxy.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-27 18:47 pulumi_policy/pulumiplugin.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 18:47 pulumi_policy/py.typed
+-rw-r--r--  2.0 unx      634 b- defN 23-Jun-27 18:47 pulumi_policy/version.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Jun-27 18:47 pulumi_policy-1.6.0a1687891551.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-27 18:47 pulumi_policy-1.6.0a1687891551.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-27 18:47 pulumi_policy-1.6.0a1687891551.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      936 b- defN 23-Jun-27 18:47 pulumi_policy-1.6.0a1687891551.dist-info/RECORD
+11 files, 56212 bytes uncompressed, 13902 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pulumi_policy/py.typed
 Comment: 
 
 Filename: pulumi_policy/version.py
 Comment: 
 
-Filename: pulumi_policy-1.6.0a1683839137.dist-info/METADATA
+Filename: pulumi_policy-1.6.0a1687891551.dist-info/METADATA
 Comment: 
 
-Filename: pulumi_policy-1.6.0a1683839137.dist-info/WHEEL
+Filename: pulumi_policy-1.6.0a1687891551.dist-info/WHEEL
 Comment: 
 
-Filename: pulumi_policy-1.6.0a1683839137.dist-info/top_level.txt
+Filename: pulumi_policy-1.6.0a1687891551.dist-info/top_level.txt
 Comment: 
 
-Filename: pulumi_policy-1.6.0a1683839137.dist-info/RECORD
+Filename: pulumi_policy-1.6.0a1687891551.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pulumi_policy/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = "1.6.0-alpha.1683839137+8cef30d0"
+VERSION = "1.6.0-alpha.1687891551+603b3ea5"
```

## Comparing `pulumi_policy-1.6.0a1683839137.dist-info/METADATA` & `pulumi_policy-1.6.0a1687891551.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-policy
-Version: 1.6.0a1683839137
+Version: 1.6.0a1687891551
 Summary: Pulumi's Policy Python SDK
 Home-page: https://github.com/pulumi/pulumi-policy
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: pulumi (<4.0.0,>=3.0.0)
 Requires-Dist: protobuf (>=3.6.0)
 Requires-Dist: grpcio (>=1.9.1)
```

## Comparing `pulumi_policy-1.6.0a1683839137.dist-info/RECORD` & `pulumi_policy-1.6.0a1687891551.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pulumi_policy/__init__.py,sha256=K99pGM6N3NaP7j-FTt2oyoxHfYSmpgUXmwp-cenYV7Y,1483
 pulumi_policy/deserialize.py,sha256=DHI6Ssbv-Z4-znbQONTX_s2ylvx_l0fYKakBO3ajsgw,3849
 pulumi_policy/policy.py,sha256=6nHRfPGjR6_FaT_JcoavmHccGUfUO_GWZ_y3Lfekirw,39992
 pulumi_policy/proxy.py,sha256=RMFCa72PjZ_fPSRWkCCcafDmzHQUpixfny4MQbuYH5U,6833
 pulumi_policy/pulumiplugin.json,sha256=-N5Rzo52OzMKvgqLH1JxqCkgtQ0y9JyJy0SQHEHbw24,22
 pulumi_policy/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pulumi_policy/version.py,sha256=MFzRReDRGxppP3AKlvP8mrRr8Ru4m0bnZ6Q4f02m3_E,634
-pulumi_policy-1.6.0a1683839137.dist-info/METADATA,sha256=kOzbtb1ktPmPAufGj2jtnAye97K1E2m3pNaiCl4X3so,2339
-pulumi_policy-1.6.0a1683839137.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pulumi_policy-1.6.0a1683839137.dist-info/top_level.txt,sha256=Kple_6YMrdhwu7WmTNRlUqrt9Hoy368SVBiYRCF5B2k,14
-pulumi_policy-1.6.0a1683839137.dist-info/RECORD,,
+pulumi_policy/version.py,sha256=dXHQBs7MOgsf_POFm7qYXQbllqISaLfZcyE7dlmc-rA,634
+pulumi_policy-1.6.0a1687891551.dist-info/METADATA,sha256=zExk1PwV8swYIzN-Sbt0o6_9nHNIBAiIUgeHWle3uvE,2339
+pulumi_policy-1.6.0a1687891551.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pulumi_policy-1.6.0a1687891551.dist-info/top_level.txt,sha256=Kple_6YMrdhwu7WmTNRlUqrt9Hoy368SVBiYRCF5B2k,14
+pulumi_policy-1.6.0a1687891551.dist-info/RECORD,,
```

