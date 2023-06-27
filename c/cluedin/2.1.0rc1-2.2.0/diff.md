# Comparing `tmp/cluedin-2.1.0rc1.tar.gz` & `tmp/cluedin-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-2.1.0rc1.tar", max compression
+gzip compressed data, was "cluedin-2.2.0.tar", max compression
```

## Comparing `cluedin-2.1.0rc1.tar` & `cluedin-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1093 2023-05-01 19:58:59.989579 cluedin-2.1.0rc1/LICENSE
--rw-r--r--   0        0        0     6887 2023-05-21 13:07:36.800967 cluedin-2.1.0rc1/cluedin/README.md
--rw-r--r--   0        0        0      214 2023-05-21 12:33:01.908448 cluedin-2.1.0rc1/cluedin/__init__.py
--rw-r--r--   0        0        0     9727 2023-05-20 19:26:50.338507 cluedin-2.1.0rc1/cluedin/account.py
--rw-r--r--   0        0        0     5735 2023-05-14 19:14:24.796902 cluedin-2.1.0rc1/cluedin/context.py
--rw-r--r--   0        0        0     1450 2023-05-21 13:07:14.463017 cluedin-2.1.0rc1/cluedin/entity.py
--rw-r--r--   0        0        0      119 2023-05-14 19:14:24.797006 cluedin-2.1.0rc1/cluedin/env.py
--rw-r--r--   0        0        0     2061 2023-05-14 19:14:24.797108 cluedin-2.1.0rc1/cluedin/gql.py
--rw-r--r--   0        0        0      492 2023-05-14 19:14:24.797191 cluedin-2.1.0rc1/cluedin/jwt.py
--rw-r--r--   0        0        0     3853 2023-05-14 19:14:24.797279 cluedin-2.1.0rc1/cluedin/public.py
--rw-r--r--   0        0        0      669 2023-05-20 19:54:13.830640 cluedin-2.1.0rc1/cluedin/vocab.py
--rw-r--r--   0        0        0      573 2023-05-21 14:27:36.205692 cluedin-2.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7588 1970-01-01 00:00:00.000000 cluedin-2.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-01 19:58:59.989579 cluedin-2.2.0/LICENSE
+-rw-r--r--   0        0        0     7051 2023-06-27 11:16:45.871386 cluedin-2.2.0/cluedin/README.md
+-rw-r--r--   0        0        0      214 2023-05-24 19:51:29.865108 cluedin-2.2.0/cluedin/__init__.py
+-rw-r--r--   0        0        0     9727 2023-05-24 19:51:29.865577 cluedin-2.2.0/cluedin/account.py
+-rw-r--r--   0        0        0     5889 2023-06-27 11:32:41.598029 cluedin-2.2.0/cluedin/context.py
+-rw-r--r--   0        0        0     1450 2023-05-24 19:51:29.865763 cluedin-2.2.0/cluedin/entity.py
+-rw-r--r--   0        0        0      119 2023-05-14 19:14:24.797006 cluedin-2.2.0/cluedin/env.py
+-rw-r--r--   0        0        0     2950 2023-06-27 11:33:27.536376 cluedin-2.2.0/cluedin/gql.py
+-rw-r--r--   0        0        0      492 2023-05-14 19:14:24.797191 cluedin-2.2.0/cluedin/jwt.py
+-rw-r--r--   0        0        0     3853 2023-05-14 19:14:24.797279 cluedin-2.2.0/cluedin/public.py
+-rw-r--r--   0        0        0      669 2023-05-24 19:51:29.866765 cluedin-2.2.0/cluedin/vocab.py
+-rw-r--r--   0        0        0      570 2023-06-27 11:15:36.182802 cluedin-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 cluedin-2.2.0/PKG-INFO
```

### Comparing `cluedin-2.1.0rc1/LICENSE` & `cluedin-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0rc1/cluedin/README.md` & `cluedin-2.2.0/cluedin/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 
 - `cluedin.entity.get_entity_blob(context: Context, entity_id: str) -> str` – returns an entity blob by ID.
 - `cluedin.entity.get_entity_as_clue(context: Context, entity_id: str) -> str` – returns an entity as a clue by ID.
 
 ### GraphQL
 
 - `cluedin.gql.gql(context: Context, query: str, variables: dict = None) -> dict` – sends a GraphQL request and returns a response.
+- `cluedin.gql.org_gql(context: Context, query: str, variables: dict = None) -> dict` – sends a GraphQL request to Organization endpoint and returns a response.
 - `cluedin.gql.entries(context: Context, query: str, variables: dict = None) -> list` – returns entries from a GraphQL search query. If cursor is requested in the GraphQL query (see the example above and tests), then it proceeds to next pages to return all results.
 
 ### JWT
 
 - `cluedin.jwt.get_jwt_payload(jwt: str) -> dict` – parses a JWT (JSON Web Token, a.k.a. access token or API token), and returns its payload serialized into a `dict`.
 
 ### Public API
```

### Comparing `cluedin-2.1.0rc1/cluedin/account.py` & `cluedin-2.2.0/cluedin/account.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0rc1/cluedin/context.py` & `cluedin-2.2.0/cluedin/context.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                  user_email: str,
                  user_password: str,
                  protocol: str = 'https',
                  access_token: str = None,
                  org_url: str = None,
                  auth_url: str = None,
                  api_url: str = None,
-                 gql_url: str = None,
+                 gql_org_url: str = None,
                  gql_api_url: str = None,
                  public_api_url: str = None,
                  verify_tls: bool = True) -> None:
         self.domain = domain
         self.org_name = org_name
         self.user_email = user_email
         self.user_password = user_password
@@ -41,29 +41,29 @@
             self.auth_url = auth_url
 
         if api_url is None:
             self.api_url = f'{self.org_url}/api/api'
         else:
             self.api_url = api_url
 
-        if gql_url is None:
-            self.gql_url = f'{self.org_url}/graphql'
+        if gql_org_url is None:
+            self.gql_org_url = f'{self.org_url}/graphql'
         else:
-            self.gql_url = gql_url
+            self.gql_org_url = gql_org_url
 
         if gql_api_url is None:
             self.gql_api_url = f'{self.api_url}/graphql'
         else:
             self.gql_api_url = gql_api_url
 
         if public_api_url is None:
             self.public_api_url = f'{self.org_url}/public/api'
         else:
             self.public_api_url = public_api_url
-            
+
         self.verify_tls = verify_tls
 
     @classmethod
     def from_dict(cls, context_dict: dict):
         """Create a Context object from a dictionary.
 
         Args:
@@ -77,15 +77,15 @@
         user_email: str = None
         user_password: str = None
         protocol: str = None
         access_token: str = None
         org_url: str = None
         auth_url: str = None
         api_url: str = None
-        gql_url: str = None
+        gql_org_url: str = None
         gql_api_url: str = None
         public_api_url: str = None
         verify_tls: bool = True
 
         if 'domain' in context_dict:
             domain = context_dict['domain']
 
@@ -111,16 +111,20 @@
 
         if 'auth_url' in context_dict:
             auth_url = context_dict['auth_url']
 
         if 'api_url' in context_dict:
             api_url = context_dict['api_url']
 
+        # TODO: Remove in v3.0.0
         if 'gql_url' in context_dict:
-            gql_url = context_dict['gql_url']
+            gql_org_url = context_dict['gql_url']
+
+        if 'gql_org_url' in context_dict:
+            gql_org_url = context_dict['gql_org_url']
 
         if 'gql_api_url' in context_dict:
             gql_api_url = context_dict['gql_api_url']
 
         if 'public_api_url' in context_dict:
             public_api_url = context_dict['public_api_url']
 
@@ -132,15 +136,15 @@
                    org_name=org_name,
                    user_email=user_email,
                    user_password=user_password,
                    access_token=access_token,
                    org_url=org_url,
                    auth_url=auth_url,
                    api_url=api_url,
-                   gql_url=gql_url,
+                   gql_org_url=gql_org_url,
                    gql_api_url=gql_api_url,
                    public_api_url=public_api_url,
                    verify_tls=verify_tls)
 
     @staticmethod
     def from_json_file(file_path: str):
         """Create a Context object from a JSON file.
```

### Comparing `cluedin-2.1.0rc1/cluedin/entity.py` & `cluedin-2.2.0/cluedin/entity.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0rc1/cluedin/gql.py` & `cluedin-2.2.0/cluedin/gql.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,52 @@
 
     if not response.ok:
         response.raise_for_status()
 
     return response.json()
 
 
+def org_gql(context: Context, query: str, variables: dict = None) -> dict:
+    """Send a GraphQL query to CluedIn Organization endpoint.
+
+    Args:
+        context (Context): Context object.
+        query (str): GraphQL query.
+        variables (dict, optional): A dicrionary of variables to be used in the query.
+            Defaults to {}.
+
+    Returns:
+        dict: JSON response.
+    """
+    headers = {
+        'Authorization': f'Bearer {context.access_token}'
+    }
+
+    if variables is None:
+        variables = {}
+
+    json = {
+        'query': query,
+        'variables': variables
+    }
+
+    response = requests.post(
+        url=context.gql_org_url,
+        json=json,
+        headers=headers,
+        timeout=CLUEDIN_REQUEST_TIMEOUT_IN_SECONDS,
+        verify=context.verify_tls
+    )
+
+    if not response.ok:
+        response.raise_for_status()
+
+    return response.json()
+
+
 def entries(context: Context, query: str, variables: dict = None) -> list:
     """Get entries from a GraphQL query. This function is a generator.
         It uses the cursor to get the next page of entries.
 
     Args:
         context (Context): Context object.
         query (str): GraphQL query.
```

### Comparing `cluedin-2.1.0rc1/cluedin/public.py` & `cluedin-2.2.0/cluedin/public.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0rc1/cluedin/vocab.py` & `cluedin-2.2.0/cluedin/vocab.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0rc1/pyproject.toml` & `cluedin-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cluedin"
-version = "2.1.0rc1"
+version = "2.2.0"
 description = "A Python client for CluedIn API."
 authors = ["Roman Klimenko <romaklimenko@gmail.com>"]
 readme = "cluedin/README.md"
 license = "MIT"
 keywords = ["cluedin", "mdm", "master data management"]
 maintainers = ["Roman Klimenko <romaklimenko@gmail.com>"]
 homepage = "https://github.com/romaklimenko/cluedin"
```

### Comparing `cluedin-2.1.0rc1/PKG-INFO` & `cluedin-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluedin
-Version: 2.1.0rc1
+Version: 2.2.0
 Summary: A Python client for CluedIn API.
 Home-page: https://github.com/romaklimenko/cluedin
 License: MIT
 Keywords: cluedin,mdm,master data management
 Author: Roman Klimenko
 Author-email: romaklimenko@gmail.com
 Maintainer: Roman Klimenko
@@ -163,14 +163,15 @@
 
 - `cluedin.entity.get_entity_blob(context: Context, entity_id: str) -> str` – returns an entity blob by ID.
 - `cluedin.entity.get_entity_as_clue(context: Context, entity_id: str) -> str` – returns an entity as a clue by ID.
 
 ### GraphQL
 
 - `cluedin.gql.gql(context: Context, query: str, variables: dict = None) -> dict` – sends a GraphQL request and returns a response.
+- `cluedin.gql.org_gql(context: Context, query: str, variables: dict = None) -> dict` – sends a GraphQL request to Organization endpoint and returns a response.
 - `cluedin.gql.entries(context: Context, query: str, variables: dict = None) -> list` – returns entries from a GraphQL search query. If cursor is requested in the GraphQL query (see the example above and tests), then it proceeds to next pages to return all results.
 
 ### JWT
 
 - `cluedin.jwt.get_jwt_payload(jwt: str) -> dict` – parses a JWT (JSON Web Token, a.k.a. access token or API token), and returns its payload serialized into a `dict`.
 
 ### Public API
```

