# Comparing `tmp/pepdbagent-0.4.1.tar.gz` & `tmp/pepdbagent-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.4.1.tar", last modified: Fri Jun  9 20:50:34 2023, max compression
+gzip compressed data, was "pepdbagent-0.4.2.tar", last modified: Tue Jun 27 16:01:41 2023, max compression
```

## Comparing `pepdbagent-0.4.1.tar` & `pepdbagent-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:34.416576 pepdbagent-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-09 20:50:34.416576 pepdbagent-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:34.412576 pepdbagent-0.4.1/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:34.412576 pepdbagent-0.4.1/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:34.412576 pepdbagent-0.4.1/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-09 20:50:34.000000 pepdbagent-0.4.1/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-09 20:50:34.000000 pepdbagent-0.4.1/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:50:34.000000 pepdbagent-0.4.1/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 20:50:34.000000 pepdbagent-0.4.1/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 20:50:34.000000 pepdbagent-0.4.1/pepdbagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:34.416576 pepdbagent-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:50:34.416576 pepdbagent-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:34.416576 pepdbagent-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-09 20:50:25.000000 pepdbagent-0.4.1/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.4.1/LICENSE.txt` & `pepdbagent-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/PKG-INFO` & `pepdbagent-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.4.1/README.md` & `pepdbagent-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/pepdbagent/db_utils.py` & `pepdbagent-0.4.2/pepdbagent/db_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Result,
     Select,
     String,
     event,
     select,
     TIMESTAMP,
 )
-from sqlalchemy.dialects.postgresql import JSONB
+from sqlalchemy.dialects.postgresql import JSON
 from sqlalchemy.engine import URL, create_engine
 from sqlalchemy.exc import ProgrammingError
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.orm import (
     DeclarativeBase,
     Mapped,
     Session,
@@ -35,17 +35,17 @@
 
 
 @compiles(BIGSERIAL, POSTGRES_DIALECT)
 def compile_bigserial_pg(type_, compiler, **kw):
     return "BIGSERIAL"
 
 
-@compiles(JSONB, POSTGRES_DIALECT)
+@compiles(JSON, POSTGRES_DIALECT)
 def compile_jsonb_pg(type_, compiler, **kw):
-    return "JSONB"
+    return "JSON"
 
 
 class Base(DeclarativeBase):
     type_annotation_map = {datetime.datetime: TIMESTAMP(timezone=True)}
 
 
 @event.listens_for(Base.metadata, "after_create")
@@ -63,15 +63,15 @@
     __tablename__ = "projects"
 
     id: Mapped[int] = mapped_column(BIGSERIAL, server_default=FetchedValue())
     namespace: Mapped[str] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column(primary_key=True)
     tag: Mapped[str] = mapped_column(primary_key=True)
     digest: Mapped[str] = mapped_column(String(32))
-    project_value: Mapped[dict] = mapped_column(JSONB, server_default=FetchedValue())
+    project_value: Mapped[dict] = mapped_column(JSON, server_default=FetchedValue())
     private: Mapped[bool]
     number_of_samples: Mapped[int]
     submission_date: Mapped[datetime.datetime]
     last_update_date: Mapped[datetime.datetime]
     pep_schema: Mapped[Optional[str]]
 
     __table_args__ = (PrimaryKeyConstraint("namespace", "name", "tag", name="id"),)
```

### Comparing `pepdbagent-0.4.1/pepdbagent/exceptions.py` & `pepdbagent-0.4.2/pepdbagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/pepdbagent/models.py` & `pepdbagent-0.4.2/pepdbagent/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,10 +106,16 @@
 
     @validator("tag", "name")
     def value_must_be_lowercase(cls, v):
         if v:
             return v.lower()
         return v
 
+    @validator("tag", "name")
+    def value_should_not_contain_question(cls, v):
+        if "?" in v:
+            return ValueError("Question mark (?) is prohibited in name and tag.")
+        return v
+
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
```

### Comparing `pepdbagent-0.4.1/pepdbagent/modules/annotation.py` & `pepdbagent-0.4.2/pepdbagent/modules/annotation.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/pepdbagent/modules/namespace.py` & `pepdbagent-0.4.2/pepdbagent/modules/namespace.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/pepdbagent/modules/project.py` & `pepdbagent-0.4.2/pepdbagent/modules/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,20 +186,22 @@
         :param pep_schema: assign PEP to a specific schema. [DefaultL: None]
         :param overwrite: if project exists overwrite the project, otherwise upload it.
             [Default: False - project won't be overwritten if it exists in db]
         :param update_only: if project exists overwrite it, otherwise do nothing.  [Default: False]
         :return: None
         """
         proj_dict = project.to_dict(extended=True)
+        proj_dict["_config"]["description"] = project.description
 
         namespace = namespace.lower()
         if name:
             name = name.lower()
             proj_name = name
             proj_dict["name"] = name
+            proj_dict["_config"]["name"] = project.name
         elif proj_dict["name"]:
             proj_name = proj_dict["name"].lower()
         else:
             raise ValueError(f"Name of the project wasn't provided. Project will not be uploaded.")
 
         proj_digest = create_digest(proj_dict)
         number_of_samples = len(project.samples)
@@ -377,16 +379,19 @@
          :param update_values: UpdateItems (pydantic class) with
             updating values
         :return: unified update dict
         """
         update_final = UpdateModel()
 
         if update_values.project_value is not None:
+            proj_dict = update_values.project_value.to_dict(extended=True)
+            proj_dict["_config"]["description"] = proj_dict["description"]
+            proj_dict["_config"]["name"] = proj_dict["name"]
             update_final = UpdateModel(
-                project_value=update_values.project_value.to_dict(extended=True),
+                project_value=proj_dict,
                 name=update_values.project_value.name,
                 digest=create_digest(update_values.project_value.to_dict(extended=True)),
                 last_update_date=datetime.datetime.now(datetime.timezone.utc),
                 number_of_samples=len(update_values.project_value.samples),
             )
 
         if update_values.tag is not None:
```

### Comparing `pepdbagent-0.4.1/pepdbagent/pepdbagent.py` & `pepdbagent-0.4.2/pepdbagent/pepdbagent.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/pepdbagent/utils.py` & `pepdbagent-0.4.2/pepdbagent/utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.4.2/pepdbagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.4.1/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.4.2/pepdbagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/setup.py` & `pepdbagent-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/tests/conftest.py` & `pepdbagent-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.1/tests/test_pepagent.py` & `pepdbagent-0.4.2/tests/test_pepagent.py`

 * *Files identical despite different names*

