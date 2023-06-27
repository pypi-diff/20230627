# Comparing `tmp/hipal_mixin_scrud-1.0.4.tar.gz` & `tmp/hipal_mixin_scrud-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hipal_mixin_scrud-1.0.4.tar", last modified: Thu Jun 22 18:36:34 2023, max compression
+gzip compressed data, was "dist\hipal_mixin_scrud-1.0.5.tar", last modified: Tue Jun 27 19:43:21 2023, max compression
```

## Comparing `hipal_mixin_scrud-1.0.4.tar` & `hipal_mixin_scrud-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.691867 hipal_mixin_scrud-1.0.4/
--rw-rw-rw-   0        0        0     5283 2023-06-22 18:36:34.690866 hipal_mixin_scrud-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3835 2023-06-22 18:34:44.000000 hipal_mixin_scrud-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.655990 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.676867 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/__init__.py
--rw-rw-rw-   0        0        0     5808 2023-06-22 17:44:55.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/generator.py
--rw-rw-rw-   0        0        0     3366 2023-06-22 17:45:00.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/mixin_list.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.682866 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/__init__.py
--rw-rw-rw-   0        0        0      255 2023-06-22 17:45:04.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/operators.py
--rw-rw-rw-   0        0        0       82 2023-06-22 17:45:06.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/sorts.py
--rw-rw-rw-   0        0        0     4691 2023-06-22 17:44:49.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/mixin.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.688867 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/__init__.py
--rw-rw-rw-   0        0        0      352 2023-06-22 17:45:08.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/paginate_params.py
--rw-rw-rw-   0        0        0      364 2023-06-22 17:45:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/pagination_base.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.671866 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/
--rw-rw-rw-   0        0        0     5283 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      621 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 18:36:34.692866 hipal_mixin_scrud-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-06-22 18:36:14.000000 hipal_mixin_scrud-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.368118 hipal_mixin_scrud-1.0.5/
+-rw-rw-rw-   0        0        0     4285 2023-06-27 19:43:21.359118 hipal_mixin_scrud-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3860 2023-06-27 19:42:51.000000 hipal_mixin_scrud-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.292091 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud.egg-info/
+-rw-rw-rw-   0        0        0     4285 2023-06-27 19:43:21.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2023-06-27 19:43:21.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 19:43:21.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-27 19:43:21.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-27 19:43:21.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.296091 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.327178 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/crud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/crud/__init__.py
+-rw-rw-rw-   0        0        0     5686 2023-06-27 19:39:37.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/crud/generator.py
+-rw-rw-rw-   0        0        0     3486 2023-06-27 19:40:20.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/crud/mixin_list.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.333175 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/enums/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/enums/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-06-22 17:45:04.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/enums/operators.py
+-rw-rw-rw-   0        0        0       82 2023-06-22 17:45:06.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/enums/sorts.py
+-rw-rw-rw-   0        0        0     4966 2023-06-27 18:13:40.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.341176 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/schemas/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/schemas/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-06-27 19:40:36.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/schemas/paginate_params.py
+-rw-rw-rw-   0        0        0      364 2023-06-27 19:40:37.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/schemas/pagination_base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.346175 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-23 18:53:11.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:43:21.354176 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/tests/factory_test/
+-rw-rw-rw-   0        0        0        0 2023-06-23 18:57:52.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/tests/factory_test/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-06-27 19:40:44.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/tests/factory_test/person.py
+-rw-rw-rw-   0        0        0     4506 2023-06-27 19:38:37.000000 hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/tests/test_mixin_paginate.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 19:43:21.369118 hipal_mixin_scrud-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-06-27 19:41:34.000000 hipal_mixin_scrud-1.0.5/setup.py
```

### Comparing `hipal_mixin_scrud-1.0.4/PKG-INFO` & `hipal_mixin_scrud-1.0.5/hipal_mixin_scrud.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,134 @@
 Metadata-Version: 2.1
-Name: hipal_mixin_scrud
-Version: 1.0.4
+Name: hipal-mixin-scrud
+Version: 1.0.5
 Summary: Libreria para crud basica.
 Home-page: http://git.hipal.com.co/libraries/ms-mixins/-/tree/feature/mixins
 Author: Hipal
 Author-email: desarrollo@hipal.com.co
-License: UNKNOWN
-Description: 
-        # Hipal Mixin Scrud
-        
-        Libreria para generar rutas generales para una crud basica
-        
-        Instalacion
-        ---------
-        ```pip install hipal-mixin-scrud```
-        
-        Como usar
-        ---------
-        Para usar la libreria se debe importar la instancia "MixinCrud" para luego en su constructor enviarle los argumentos necesarios, ejemplo:
-        
-        ```
-        from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
-        from db.db_session import db_session
-        from models.user import User
-        
-        from hipal_mixin_scrud.mixin import MixinCrud
-        
-        users_router = MixinCrud(
-            schema=UserSchema,
-            db_session=db_session,
-            model=User,
-            prefix="/users",
-            create_schema=CreateUserSchema,
-            update_schema=UpdateUserSchema
-        )
-        ```
-        donde:
-        - **schema**: Sera el schema principal para listar o paginar los datos
-        - **db_session**: La session de la base de datos otorgada por el motor implementado mediante sqlalchemy
-        - **model**: El modelo con el que se hara la crud basica
-        - **prefix**: La raiz de los endpoints
-        - **create_schema**: El schema con el que se mapearan los datos para crear los registros en el modelo
-        - **update_schema**: El schema con el que se mapearan los datos para la actualizacion de un registro existente del modelo
-        
-        Uso Avanzado
-        ---------
-        Si se requiere tener mas control de las rutas generadas, se tiene lo siguiente:
-        
-        Para especificar que rutas se requieren y cuales no, se hace uso de 5 parametros:
-        - has_update
-        - has_get_list
-        - has_delete_one
-        - has_create
-        - has_get_one
-        
-        Por defecto todas estan en "True", y reciben booleanos para indicar si se genera la ruta o no:
-        ```
-        from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
-        from db.db_session import db_session
-        from models.user import User
-        
-        from hipal_mixin_scrud.mixin import MixinCrud
-        
-        users_router = MixinCrud(
-            schema=UserSchema,
-            db_session=db_session,
-            model=User,
-            prefix="/users",
-            create_schema=CreateUserSchema,
-            update_schema=UpdateUserSchema,
-            has_update=False,
-            has_get_list=True,
-            has_delete_one=False,
-            has_create=False,
-            has_get_one=True,
-        )
-        ```
-        
-        Para especificar una "query prefija" es decir, una query por defecto que se concatenara con la query final en toda la CRUD principal, hacemos uso del parametro: **query**, Ejemplo:
-        
-        ```
-        from fastapi import Request
-        from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
-        from db.db_session import db_session
-        from models.user import User
-        
-        from hipal_mixin_scrud.mixin import MixinCrud
-        
-        
-        def default_query(
-            request: Request,
-        ):
-            account_id = request.headers.get("account_id")
-            profile_id = request.headers.get("profile_id")
-        
-            query = db_session.query(User).filter(User.id > 0)
-        
-            return query
-        
-        users_router = MixinCrud(
-            schema=UserSchema,
-            db_session=db_session,
-            model=User,
-            prefix="/users",
-            create_schema=CreateUserSchema,
-            update_schema=UpdateUserSchema,
-            query=default_query
-        )
-        ```
-        
-        El parametro query es opcional, y en caso de que se requiera recibira una funcion que como obligacion debera recibir por argument "request" y tendra que devolver la query que se requiera.
-        
-        Paginación
-        ---------
-        
-        Para generar una paginacion es exactamente igual a lo dicho anteriormente, Sin embargo, recibe algunos parametros opcionales los cuales sirven para:
-        
-        - **offset**: Recibe el numero de la posicion del registro donde se requiere empezar a ver 
-        - **limit**: Limite de registros a visualizar
-        - **search**: Lista de campos con su valor a buscar separados por ; ejemplo: name=alan;company=Gooogle
-        - **sort**: ASC o DESC para especificar si se requiere el orden descendente o ascendente
-        - **sort_field**: Nombre del campo por el cual se requiere ordenar
-        
-        Adicionalmente se podra user "users_router" para generar las rutas como generalmente las conocemos:
-        
-        ```
-        @users_router.get("/me", response_model=UserSchema)
-        def endpoint() -> UserSchema:
-            return {"msg":"prueba"}
-        ```
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+
+
+# Hipal Mixin Scrud
+
+Libreria para generar rutas generales para una crud basica con el orm de SQLAlchemy
+
+Instalacion
+---------
+```pip install hipal-mixin-scrud```
+
+Como usar
+---------
+Para usar la libreria se debe importar la instancia "MixinCrud" para luego en su constructor enviarle los argumentos necesarios.
+ejemplo:
+
+```
+from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
+from db.db_session import db_session
+from models.user import User
+
+from hipal_mixin_scrud.mixin import MixinCrud
+
+users_router = MixinCrud(
+    schema=UserSchema,
+    db_session=db_session,
+    model=User,
+    prefix="/users",
+    create_schema=CreateUserSchema,
+    update_schema=UpdateUserSchema
+)
+```
+donde:
+- **schema**: Sera el schema principal para listar o paginar los datos
+- **db_session**: La session de la base de datos otorgada por el motor implementado mediante sqlalchemy
+- **model**: El modelo con el que se hara la crud basica
+- **prefix**: La raiz de los endpoints
+- **create_schema**: El schema con el que se mapearan los datos para crear los registros en el modelo
+- **update_schema**: El schema con el que se mapearan los datos para la actualizacion de un registro existente del modelo
+
+Uso Avanzado
+---------
+Si se requiere tener mas control de las rutas generadas, se tiene lo siguiente:
+
+Para especificar que rutas se requieren y cuales no, se hace uso de 5 parametros:
+- has_update
+- has_get_list
+- has_delete_one
+- has_create
+- has_get_one
+
+Por defecto todas estan en "True", y reciben booleanos para indicar si se genera la ruta o no:
+```
+from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
+from db.db_session import db_session
+from models.user import User
+
+from hipal_mixin_scrud.mixin import MixinCrud
+
+users_router = MixinCrud(
+    schema=UserSchema,
+    db_session=db_session,
+    model=User,
+    prefix="/users",
+    create_schema=CreateUserSchema,
+    update_schema=UpdateUserSchema,
+    has_update=False,
+    has_get_list=True,
+    has_delete_one=False,
+    has_create=False,
+    has_get_one=True,
+)
+```
+
+Para especificar una "query prefija" es decir, una query por defecto que se concatenara con la query final en toda la CRUD principal, hacemos uso del parametro: **query**, Ejemplo:
+
+```
+from fastapi import Request
+from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
+from db.db_session import db_session
+from models.user import User
+
+from hipal_mixin_scrud.mixin import MixinCrud
+
+
+def default_query(
+    request: Request,
+):
+    account_id = request.headers.get("account_id")
+    profile_id = request.headers.get("profile_id")
+
+    query = db_session.query(User).filter(User.id > 0)
+
+    return query
+
+users_router = MixinCrud(
+    schema=UserSchema,
+    db_session=db_session,
+    model=User,
+    prefix="/users",
+    create_schema=CreateUserSchema,
+    update_schema=UpdateUserSchema,
+    query=default_query
+)
+```
+
+El parametro query es opcional, y en caso de que se requiera recibira una funcion que como obligacion debera recibir por argument "request" y tendra que devolver la query que se requiera.
+
+Paginación
+---------
+
+Para generar una paginacion es exactamente igual a lo dicho anteriormente, Sin embargo, recibe algunos parametros opcionales los cuales sirven para:
+
+- **offset**: Recibe el numero de la posicion del registro donde se requiere empezar a ver 
+- **limit**: Limite de registros a visualizar
+- **search**: Lista de campos con su valor a buscar separados por ; ejemplo: name=alan;company=Gooogle
+- **sort**: ASC o DESC para especificar si se requiere el orden descendente o ascendente
+- **sort_field**: Nombre del campo por el cual se requiere ordenar
+
+Adicionalmente se podra user "users_router" para generar las rutas como generalmente las conocemos:
+
+```
+@users_router.get("/me", response_model=UserSchema)
+def endpoint() -> UserSchema:
+    return {"msg":"prueba"}
+```
```

### Comparing `hipal_mixin_scrud-1.0.4/README.md` & `hipal_mixin_scrud-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 
 # Hipal Mixin Scrud
 
-Libreria para generar rutas generales para una crud basica
+Libreria para generar rutas generales para una crud basica con el orm de SQLAlchemy
 
 Instalacion
 ---------
 ```pip install hipal-mixin-scrud```
 
 Como usar
 ---------
-Para usar la libreria se debe importar la instancia "MixinCrud" para luego en su constructor enviarle los argumentos necesarios, ejemplo:
+Para usar la libreria se debe importar la instancia "MixinCrud" para luego en su constructor enviarle los argumentos necesarios.
+ejemplo:
 
 ```
 from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
 from db.db_session import db_session
 from models.user import User
 
 from hipal_mixin_scrud.mixin import MixinCrud
```

### Comparing `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/generator.py` & `hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/crud/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from fastapi import APIRouter, Depends, HTTPException
+# lib
 from typing import Any, Callable, List, Optional, Sequence, TypeVar, Union
-from typing import Type
-from typing import Generic
+from abc import ABC, abstractmethod
+from pydantic import create_model
 from pydantic import BaseModel
+from typing import Generic
+from typing import Type
+
+# fastapi
+from fastapi import APIRouter, Depends, HTTPException
+
+# sqlalchemy
 from sqlalchemy.orm import Session
-from sqlalchemy.orm import Query
-from hipal_mixin_scrud.schemas.pagination_base import PaginationBase
-from pydantic import create_model
 
-from abc import ABC, abstractmethod
+# app
+from schemas.pagination_base import PaginationBase
 
 T = TypeVar("T", bound=BaseModel)
 
 DEPENDENCIES = Optional[Sequence[Depends]]
 
 
 class MixinGenerator(Generic[T], APIRouter, ABC):
@@ -50,25 +55,23 @@
         model,
         db_session: Session,
         schema: Type[T],
         prefix: Optional[str] = None,
         tags: Optional[List[str]] = None,
         create_schema: Optional[BaseModel] = None,
         update_schema: Optional[BaseModel] = None,
-        query_model_paginate: Optional[Query] = None,
         has_get_list: bool = True,
         has_update: bool = True,
         has_create: bool = True,
         has_get_one: bool = True,
         has_delete_one: bool = True,
         **kwargs: Any,
     ) -> None:
         self.model = model
         self.db_session = db_session
-        self.query_model_paginate = query_model_paginate
         self.schema = schema
         self._pk: str = self._pk if hasattr(self, "_pk") else "id"
         self.create_schema = (
             create_schema
             if create_schema
             else self.schema_factory(self.schema, pk_field_name=self._pk, name="Create")
         )
```

### Comparing `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/mixin_list.py` & `hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/crud/mixin_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+# lib
+from pydantic import BaseModel
+from typing import Type
 import math
+
+# fastapi
 from fastapi import HTTPException
-from typing import Type
-from pydantic import BaseModel
+
+# sqlalchemy
+from sqlalchemy.orm import declarative_base
 from sqlalchemy import String, cast, or_
 from sqlalchemy.orm import Session
 from sqlalchemy.orm import Query
-from sqlalchemy.orm import declarative_base
 
-from hipal_mixin_scrud.schemas.paginate_params import PaginateParams
+# app
+from schemas.paginate_params import PaginateParams
 
 
 class ListModelMixin:
     """
     List a queryset.
     """
 
@@ -22,35 +28,29 @@
         db_session: Session,
         model: Type[Base],
         squema: BaseModel,
         path: str,
         paginate_params: PaginateParams = PaginateParams(),
         query_model: Query = None,
     ):
+
         query = db_session.query(model) if query_model is None else query_model
 
         if paginate_params.offset < 0:
             raise HTTPException(
                 status_code=400,
                 detail="Offset debe ser positivo.",
             )
 
         if paginate_params.limit < 1:
             raise HTTPException(
                 status_code=400,
                 detail="Limite debe ser mayor que 0.",
             )
 
-        order_by = getattr(model, "created_at")
-        order_by = order_by.desc()
-
-        if paginate_params.sort:
-            order_by = getattr(model, paginate_params.sort_field)
-            order_by = getattr(order_by, paginate_params.sort.value)()
-
         if paginate_params.search:
             SEPARATOR = ";"
             OPERATOR = "="
 
             filters = paginate_params.search.split(SEPARATOR)
             filters_sql = []
 
@@ -61,14 +61,24 @@
 
                 filter = cast(field, String).ilike(f"%{search_value}%")
 
                 filters_sql.append(filter)
 
             query = query.filter(or_(*filters_sql))
 
+        order_by = None
+        
+        if hasattr(model, "created_at"):
+            order_by = getattr(model, "created_at")
+            order_by = order_by.desc()
+
+        if paginate_params.sort:
+            order_by = getattr(model, paginate_params.sort_field)
+            order_by = getattr(order_by, paginate_params.sort.value)()
+
         query = query.order_by(order_by)
         paginate_model = query.limit(paginate_params.limit).offset(
             paginate_params.offset
         )
         total_pages = math.ceil(query.count() / paginate_params.limit)
         total_items = query.count()
 
@@ -95,9 +105,9 @@
                         f"?offset={total_pages}"
                         f"&limit={paginate_params.limit}"
                     ),
                 },
             },
             "data": [squema.from_orm(row) for row in paginate_model.all()],
         }
-
+        
         return obj
```

### Comparing `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/mixin.py` & `hipal_mixin_scrud-1.0.5/hipal_mixin_scrud_t/mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from fastapi import Depends, HTTPException, Request, Response
-from typing import Any, Callable, List, Optional, Sequence, TypeVar
+from typing import Any, Callable, Dict, List, Optional, Sequence, TypeVar
 from typing import Type
 from pydantic import BaseModel
 from types import FunctionType
 from sqlalchemy.orm import Query
 from sqlalchemy.orm import Session
 
-from hipal_mixin_scrud.crud.generator import MixinGenerator
-from hipal_mixin_scrud.crud.mixin_list import ListModelMixin
-from hipal_mixin_scrud.schemas.paginate_params import PaginateParams
+from crud.generator import MixinGenerator
+from crud.mixin_list import ListModelMixin
+from schemas.paginate_params import PaginateParams
 from sqlalchemy.ext.declarative import DeclarativeMeta as Model
 
 T = TypeVar("T", bound=BaseModel)
 DEPENDENCIES = Optional[Sequence[Depends]]
 
 
 class MixinCrud(MixinGenerator, ListModelMixin):
@@ -26,22 +26,24 @@
         db_session: Session,
         schema: Type[T],
         query: Optional[FunctionType] = None,
         prefix: Optional[str] = None,
         tags: Optional[List[str]] = None,
         create_schema: Optional[BaseModel] = None,
         update_schema: Optional[BaseModel] = None,
+        error_messages: Optional[Dict] = None,
         has_get_list: bool = True,
         has_update: bool = True,
         has_create: bool = True,
         has_get_one: bool = True,
         has_delete_one: bool = True,
         **kwargs: Any,
     ) -> None:
         self.query = query
+        self.error_messages = error_messages
 
         super().__init__(
             model=model,
             db_session=db_session,
             schema=schema,
             prefix=prefix,
             tags=tags,
@@ -51,84 +53,95 @@
             has_update=has_update,
             has_create=has_create,
             has_get_one=has_get_one,
             has_delete_one=has_delete_one,
             **kwargs,
         )
 
+    def get_message(self, http_code):
+        
+        error_mesages = self.error_messages if self.error_messages else {
+            "not_found": "Recurso no encontrado.",
+            "already_exists": "El dato ya existe.",
+        }
+        
+        return error_mesages.get(http_code)
+    
     def _fk_fields(self, model: Model):
         foreign_keys = [c.key for c in model.__table__.c if c.foreign_keys]
         return foreign_keys
 
     def _get_one_db(self, item_id, query: Query = None):
         item = (
             query.filter(getattr(self.model, self._pk) == item_id).first()
             if self.query
             else self.db_session.query(self.model)
             .filter(getattr(self.model, self._pk) == item_id)
             .first()
         )
+        
+        msg_response = self.get_message("not_found")
 
         if not item:
-            raise HTTPException(404, "Recurso no encontrado")
+            raise HTTPException(404, msg_response)
 
         return item
 
     def _get_paginate(self, *args: Any, **kwargs: Any):
         def route(
             request: Request,
             paginate_params: PaginateParams = Depends(),
         ):
+
             query = None
 
             if self.query:
                 query = self.query(request)
 
             path = request.url._url.split("?")[0]
             return self.paginate(
                 db_session=self.db_session,
                 model=self.model,
                 paginate_params=paginate_params,
                 squema=self.schema,
                 path=path,
                 query_model=query,
             )
+    
 
         return route
 
     def _get_one(self, *args: Any, **kwargs: Any):
         def route(request: Request, item_id):
             query = None
             if self.query:
                 query = self.query(request)
             return self._get_one_db(item_id, query)
 
         return route
 
     def _create(self, *args: Any, **kwargs: Any):
         def route(model: self.create_schema):
+
             db_model = self.model(**model.dict())
             self.db_session.add(db_model)
             self.db_session.commit()
             self.db_session.refresh(db_model)
+
             return db_model
 
         return route
 
     def _update(self, *args: Any, **kwargs: Any):
         def route(
-            request: Request,
             item_id,
             model: self.update_schema,
         ):
-            query = None
-            if self.query:
-                query = self.query(request)
 
-            db_model = self._get_one_db(item_id, query)
+            db_model = self._get_one_db(item_id)
 
             for key, value in model.dict(exclude={self._pk}).items():
                 if hasattr(db_model, key):
                     setattr(db_model, key, value)
 
             self.db_session.commit()
             self.db_session.refresh(db_model)
```

### Comparing `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/PKG-INFO` & `hipal_mixin_scrud-1.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,134 @@
 Metadata-Version: 2.1
-Name: hipal-mixin-scrud
-Version: 1.0.4
+Name: hipal_mixin_scrud
+Version: 1.0.5
 Summary: Libreria para crud basica.
 Home-page: http://git.hipal.com.co/libraries/ms-mixins/-/tree/feature/mixins
 Author: Hipal
 Author-email: desarrollo@hipal.com.co
-License: UNKNOWN
-Description: 
-        # Hipal Mixin Scrud
-        
-        Libreria para generar rutas generales para una crud basica
-        
-        Instalacion
-        ---------
-        ```pip install hipal-mixin-scrud```
-        
-        Como usar
-        ---------
-        Para usar la libreria se debe importar la instancia "MixinCrud" para luego en su constructor enviarle los argumentos necesarios, ejemplo:
-        
-        ```
-        from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
-        from db.db_session import db_session
-        from models.user import User
-        
-        from hipal_mixin_scrud.mixin import MixinCrud
-        
-        users_router = MixinCrud(
-            schema=UserSchema,
-            db_session=db_session,
-            model=User,
-            prefix="/users",
-            create_schema=CreateUserSchema,
-            update_schema=UpdateUserSchema
-        )
-        ```
-        donde:
-        - **schema**: Sera el schema principal para listar o paginar los datos
-        - **db_session**: La session de la base de datos otorgada por el motor implementado mediante sqlalchemy
-        - **model**: El modelo con el que se hara la crud basica
-        - **prefix**: La raiz de los endpoints
-        - **create_schema**: El schema con el que se mapearan los datos para crear los registros en el modelo
-        - **update_schema**: El schema con el que se mapearan los datos para la actualizacion de un registro existente del modelo
-        
-        Uso Avanzado
-        ---------
-        Si se requiere tener mas control de las rutas generadas, se tiene lo siguiente:
-        
-        Para especificar que rutas se requieren y cuales no, se hace uso de 5 parametros:
-        - has_update
-        - has_get_list
-        - has_delete_one
-        - has_create
-        - has_get_one
-        
-        Por defecto todas estan en "True", y reciben booleanos para indicar si se genera la ruta o no:
-        ```
-        from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
-        from db.db_session import db_session
-        from models.user import User
-        
-        from hipal_mixin_scrud.mixin import MixinCrud
-        
-        users_router = MixinCrud(
-            schema=UserSchema,
-            db_session=db_session,
-            model=User,
-            prefix="/users",
-            create_schema=CreateUserSchema,
-            update_schema=UpdateUserSchema,
-            has_update=False,
-            has_get_list=True,
-            has_delete_one=False,
-            has_create=False,
-            has_get_one=True,
-        )
-        ```
-        
-        Para especificar una "query prefija" es decir, una query por defecto que se concatenara con la query final en toda la CRUD principal, hacemos uso del parametro: **query**, Ejemplo:
-        
-        ```
-        from fastapi import Request
-        from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
-        from db.db_session import db_session
-        from models.user import User
-        
-        from hipal_mixin_scrud.mixin import MixinCrud
-        
-        
-        def default_query(
-            request: Request,
-        ):
-            account_id = request.headers.get("account_id")
-            profile_id = request.headers.get("profile_id")
-        
-            query = db_session.query(User).filter(User.id > 0)
-        
-            return query
-        
-        users_router = MixinCrud(
-            schema=UserSchema,
-            db_session=db_session,
-            model=User,
-            prefix="/users",
-            create_schema=CreateUserSchema,
-            update_schema=UpdateUserSchema,
-            query=default_query
-        )
-        ```
-        
-        El parametro query es opcional, y en caso de que se requiera recibira una funcion que como obligacion debera recibir por argument "request" y tendra que devolver la query que se requiera.
-        
-        Paginación
-        ---------
-        
-        Para generar una paginacion es exactamente igual a lo dicho anteriormente, Sin embargo, recibe algunos parametros opcionales los cuales sirven para:
-        
-        - **offset**: Recibe el numero de la posicion del registro donde se requiere empezar a ver 
-        - **limit**: Limite de registros a visualizar
-        - **search**: Lista de campos con su valor a buscar separados por ; ejemplo: name=alan;company=Gooogle
-        - **sort**: ASC o DESC para especificar si se requiere el orden descendente o ascendente
-        - **sort_field**: Nombre del campo por el cual se requiere ordenar
-        
-        Adicionalmente se podra user "users_router" para generar las rutas como generalmente las conocemos:
-        
-        ```
-        @users_router.get("/me", response_model=UserSchema)
-        def endpoint() -> UserSchema:
-            return {"msg":"prueba"}
-        ```
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+
+
+# Hipal Mixin Scrud
+
+Libreria para generar rutas generales para una crud basica con el orm de SQLAlchemy
+
+Instalacion
+---------
+```pip install hipal-mixin-scrud```
+
+Como usar
+---------
+Para usar la libreria se debe importar la instancia "MixinCrud" para luego en su constructor enviarle los argumentos necesarios.
+ejemplo:
+
+```
+from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
+from db.db_session import db_session
+from models.user import User
+
+from hipal_mixin_scrud.mixin import MixinCrud
+
+users_router = MixinCrud(
+    schema=UserSchema,
+    db_session=db_session,
+    model=User,
+    prefix="/users",
+    create_schema=CreateUserSchema,
+    update_schema=UpdateUserSchema
+)
+```
+donde:
+- **schema**: Sera el schema principal para listar o paginar los datos
+- **db_session**: La session de la base de datos otorgada por el motor implementado mediante sqlalchemy
+- **model**: El modelo con el que se hara la crud basica
+- **prefix**: La raiz de los endpoints
+- **create_schema**: El schema con el que se mapearan los datos para crear los registros en el modelo
+- **update_schema**: El schema con el que se mapearan los datos para la actualizacion de un registro existente del modelo
+
+Uso Avanzado
+---------
+Si se requiere tener mas control de las rutas generadas, se tiene lo siguiente:
+
+Para especificar que rutas se requieren y cuales no, se hace uso de 5 parametros:
+- has_update
+- has_get_list
+- has_delete_one
+- has_create
+- has_get_one
+
+Por defecto todas estan en "True", y reciben booleanos para indicar si se genera la ruta o no:
+```
+from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
+from db.db_session import db_session
+from models.user import User
+
+from hipal_mixin_scrud.mixin import MixinCrud
+
+users_router = MixinCrud(
+    schema=UserSchema,
+    db_session=db_session,
+    model=User,
+    prefix="/users",
+    create_schema=CreateUserSchema,
+    update_schema=UpdateUserSchema,
+    has_update=False,
+    has_get_list=True,
+    has_delete_one=False,
+    has_create=False,
+    has_get_one=True,
+)
+```
+
+Para especificar una "query prefija" es decir, una query por defecto que se concatenara con la query final en toda la CRUD principal, hacemos uso del parametro: **query**, Ejemplo:
+
+```
+from fastapi import Request
+from schemas import UserSchema, CreateUserSchema, UpdateUserSchema
+from db.db_session import db_session
+from models.user import User
+
+from hipal_mixin_scrud.mixin import MixinCrud
+
+
+def default_query(
+    request: Request,
+):
+    account_id = request.headers.get("account_id")
+    profile_id = request.headers.get("profile_id")
+
+    query = db_session.query(User).filter(User.id > 0)
+
+    return query
+
+users_router = MixinCrud(
+    schema=UserSchema,
+    db_session=db_session,
+    model=User,
+    prefix="/users",
+    create_schema=CreateUserSchema,
+    update_schema=UpdateUserSchema,
+    query=default_query
+)
+```
+
+El parametro query es opcional, y en caso de que se requiera recibira una funcion que como obligacion debera recibir por argument "request" y tendra que devolver la query que se requiera.
+
+Paginación
+---------
+
+Para generar una paginacion es exactamente igual a lo dicho anteriormente, Sin embargo, recibe algunos parametros opcionales los cuales sirven para:
+
+- **offset**: Recibe el numero de la posicion del registro donde se requiere empezar a ver 
+- **limit**: Limite de registros a visualizar
+- **search**: Lista de campos con su valor a buscar separados por ; ejemplo: name=alan;company=Gooogle
+- **sort**: ASC o DESC para especificar si se requiere el orden descendente o ascendente
+- **sort_field**: Nombre del campo por el cual se requiere ordenar
+
+Adicionalmente se podra user "users_router" para generar las rutas como generalmente las conocemos:
+
+```
+@users_router.get("/me", response_model=UserSchema)
+def endpoint() -> UserSchema:
+    return {"msg":"prueba"}
+```
```

### Comparing `hipal_mixin_scrud-1.0.4/setup.py` & `hipal_mixin_scrud-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Lee el contenido del archivo README.md
 readme_path = Path(__file__).parent / "README.md"
 with open(readme_path, "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name="hipal_mixin_scrud",
-    version="1.0.4",
+    version="1.0.5",
     description="Libreria para crud basica.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.9",
     install_requires=[
         "pydantic==1.10.7",
```

