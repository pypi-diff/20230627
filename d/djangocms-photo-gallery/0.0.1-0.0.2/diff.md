# Comparing `tmp/djangocms_photo_gallery-0.0.1.tar.gz` & `tmp/djangocms_photo_gallery-0.0.2.tar.gz`

## Comparing `djangocms_photo_gallery-0.0.1.tar` & `djangocms_photo_gallery-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/.idea/djangocms-photo-gallery.iml
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/admin.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/apps.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/cms_apps.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/cms_plugins.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/models.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/tests.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/urls.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/views.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/.gitignore
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/djangocms-photo-gallery.iml
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/misc.xml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/modules.xml
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/workspace.xml
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/migrations/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/album_list.html
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/plugins/album.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/README.md
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/djangocms-photo-gallery.iml
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/README.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/admin.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/apps.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/cms_apps.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/cms_plugins.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/models.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/tests.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/urls.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/views.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/.gitignore
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/djangocms-photo-gallery.iml
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/misc.xml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/modules.xml
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/workspace.xml
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/migrations/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/album_list.html
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/plugins/album.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/README.md
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/PKG-INFO
```

### Comparing `djangocms_photo_gallery-0.0.1/.idea/djangocms-photo-gallery.iml` & `djangocms_photo_gallery-0.0.2/.idea/djangocms-photo-gallery.iml`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/.idea/misc.xml` & `djangocms_photo_gallery-0.0.2/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/.idea/workspace.xml` & `djangocms_photo_gallery-0.0.2/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `djangocms_photo_gallery-0.0.1/.idea/workspace.xml` & `djangocms_photo_gallery-0.0.2/.idea/workspace.xml`

```diff
@@ -39,15 +39,15 @@
       <changelist id="bcf82a1e-0546-482c-a9dc-afe82c16d027" name="Changes" comment=""/>
       <created>1687875341053</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1687875341053</updated>
       <workItem from="1687875342222" duration="93000"/>
       <workItem from="1687875441137" duration="6829000"/>
-      <workItem from="1687882901824" duration="146000"/>
+      <workItem from="1687882901824" duration="1820000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsContentAnnotationSettings">
```

### Comparing `djangocms_photo_gallery-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `djangocms_photo_gallery-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/README.md` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/models.py` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/djangocms-photo-gallery.iml` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/djangocms-photo-gallery.iml`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/misc.xml` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/workspace.xml` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/.idea/inspectionProfiles/Project_Default.xml` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/migrations/0001_initial.py` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html` & `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/LICENSE.txt` & `djangocms_photo_gallery-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.1/pyproject.toml` & `djangocms_photo_gallery-0.0.2/pyproject.toml`

 * *Files identical despite different names*

