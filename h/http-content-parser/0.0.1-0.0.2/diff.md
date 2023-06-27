# Comparing `tmp/http_content_parser-0.0.1.tar.gz` & `tmp/http_content_parser-0.0.2.tar.gz`

## Comparing `http_content_parser-0.0.1.tar` & `http_content_parser-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/src/http_content_parser/__init__.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/src/http_content_parser/curl_parser.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/src/http_content_parser/generate_api_file.py
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/src/http_content_parser/openapi_parser.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/src/http_content_parser/postman_parser.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/src/http_content_parser/req_data.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/src/http_content_parser/swagger2_parser.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/LICENSE
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/src/http_content_parser/__init__.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/src/http_content_parser/curl_parser.py
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/src/http_content_parser/generate_api_file.py
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/src/http_content_parser/openapi_parser.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/src/http_content_parser/postman_parser.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/src/http_content_parser/req_data.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/src/http_content_parser/swagger2_parser.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/LICENSE
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.2/PKG-INFO
```

### Comparing `http_content_parser-0.0.1/src/http_content_parser/curl_parser.py` & `http_content_parser-0.0.2/src/http_content_parser/curl_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.1/src/http_content_parser/generate_api_file.py` & `http_content_parser-0.0.2/src/http_content_parser/generate_api_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,16 @@
             req_data.body = api_info['body']
             req_data.query_param = json.dumps(api_info['query_param'])
             req_data.original_url = api_info['url']
             req_data.method = api_info['method'].lower()
             req_data.temp_api_label = self.convert_swagger2_path(
                 api_info['path'].split('/'), '_').replace('{', '').replace('}', '') + "_" + api_info['method'].lower()
             self.write_api_content_to_yaml(yaml_file, req_data)
+        # remove duplicate key
+        self.remove_duplicate_key_for_yaml(yaml_file)
 
     def produce_api_yaml_for_curl(self, curl_file, yaml_file, curl_filter=None):
         curl_parser = CurlParser()
         with open(curl_file, 'rt') as f:
             lines = f.readlines()
             line_num_array = curl_parser.get_curl_line_num_scope(lines=lines)
             for r in line_num_array:
@@ -42,14 +44,16 @@
                     split_url['url_path']) + template.method
                 template.header = json.dumps(template.header)
                 template.query_param = json.dumps(split_url['url_params'])
                 split_url_origin = curl_parser.split_url(
                     template.original_url, '/')
                 template.path = split_url_origin['url_path'][:-1]
                 self.write_api_content_to_yaml(yaml_file, template)
+        # remove duplicate key
+        self.remove_duplicate_key_for_yaml(yaml_file)
 
     def produce_api_yaml_for_swagger2(self, swagger2_dict, yaml_file):
         swagger_parser = Swagger2Parser(swagger2_dict)
         api_dict = swagger_parser.get_swagger_api_info()
         if not api_dict:
             print('check your swagger json')
             return
@@ -63,14 +67,16 @@
             req_data.query_param = json.dumps(path_info['query_param'])
             req_data.path_param = json.dumps(path_info['path_param'])
             req_data.response = json.dumps(path_info.get('response', {}))
             # swagger中body第一层和第二层key重复,只取第二层后的数据
             for _, v in path_info['body_param'].items():
                 req_data.body = json.dumps(v)
             self.write_api_content_to_yaml(yaml_file, req_data)
+        # remove duplicate key
+        self.remove_duplicate_key_for_yaml(yaml_file)
 
     def produce_api_yaml_for_openapi3(self, openapi_dict, yaml_file):
         if not openapi_dict:
             print('openapi dict is null')
             return
         parser = OpenApiParser(openapi_dict)
         api_dict = parser.get_open_api_info()
@@ -85,14 +91,16 @@
                 path.split('/'), '_').replace('{', '').replace('}', '')
             req_data.method = path.split('/')[-1]
             req_data.query_param = json.dumps(path_info['query_param'])
             req_data.path_param = json.dumps(path_info['path_param'])
             req_data.response = json.dumps(path_info.get('response', {}))
             req_data.body = json.dumps(path_info['body_param'])
             self.write_api_content_to_yaml(yaml_file, req_data)
+        # remove duplicate key
+        self.remove_duplicate_key_for_yaml(yaml_file)
 
     def convert_swagger2_path(self, path_list, split_char):
         if not path_list:
             return ''
         url_path = ''
         for u in path_list:
             if u:
@@ -102,14 +110,26 @@
     def replace_api_label_chars(self, string):
         pattern = r'[+@?=.]'  # 定义要匹配的特殊字符模式
         replacement = '_'  # 替换为的字符串
 
         new_string = re.sub(pattern, replacement, string)
         return new_string
 
+    def remove_duplicate_key_for_yaml(self, api_yaml_file_path):
+        with open(api_yaml_file_path, 'r') as f:
+            data = yaml.safe_load(f)
+        unique_data = {}
+        if data:
+            for k, v in data.items():
+                if k not in unique_data:
+                    unique_data[k] = v
+
+        with open(api_yaml_file_path, 'w') as f:
+            yaml.dump(unique_data, f)
+
     def write_api_content_to_yaml(self, file, template: ReqData):
         api_obj = {}
         yaml_obj = {}
         with open(file, 'at') as f:
             api_obj['original_url'] = template.original_url
             api_obj['path'] = template.path
             api_obj['query_param'] = template.query_param
```

### Comparing `http_content_parser-0.0.1/src/http_content_parser/openapi_parser.py` & `http_content_parser-0.0.2/src/http_content_parser/openapi_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.1/src/http_content_parser/postman_parser.py` & `http_content_parser-0.0.2/src/http_content_parser/postman_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.1/src/http_content_parser/req_data.py` & `http_content_parser-0.0.2/src/http_content_parser/req_data.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.1/src/http_content_parser/swagger2_parser.py` & `http_content_parser-0.0.2/src/http_content_parser/swagger2_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.1/LICENSE` & `http_content_parser-0.0.2/LICENSE`

 * *Files identical despite different names*

