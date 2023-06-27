# Comparing `tmp/flask_lambda_python36-0.1.0-py36-none-any.whl.zip` & `tmp/flask_lambda_python36-0.1.1-py36-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 3527 bytes, number of entries: 5
--rw-r--r--  2.0 unx     3867 b- defN 18-Apr-10 16:28 flask_lambda.py
--rw-r--r--  2.0 unx       13 b- defN 18-Apr-10 16:43 flask_lambda_python36-0.1.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx       93 b- defN 18-Apr-10 16:43 flask_lambda_python36-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     1657 b- defN 18-Apr-10 16:43 flask_lambda_python36-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      431 b- defN 18-Apr-10 16:43 flask_lambda_python36-0.1.0.dist-info/RECORD
-5 files, 6061 bytes uncompressed, 2727 bytes compressed:  55.0%
+Zip file size: 7257 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     3772 b- defN 23-Jun-27 14:12 flask_lambda.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-27 14:37 flask_lambda_python36-0.1.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      750 b- defN 23-Jun-27 14:37 flask_lambda_python36-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       93 b- defN 23-Jun-27 14:37 flask_lambda_python36-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jun-27 14:37 flask_lambda_python36-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      528 b- defN 23-Jun-27 14:37 flask_lambda_python36-0.1.1.dist-info/RECORD
+6 files, 16513 bytes uncompressed, 6291 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
 Filename: flask_lambda.py
 Comment: 
 
-Filename: flask_lambda_python36-0.1.0.dist-info/top_level.txt
+Filename: flask_lambda_python36-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: flask_lambda_python36-0.1.0.dist-info/WHEEL
+Filename: flask_lambda_python36-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: flask_lambda_python36-0.1.0.dist-info/METADATA
+Filename: flask_lambda_python36-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: flask_lambda_python36-0.1.0.dist-info/RECORD
+Filename: flask_lambda_python36-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: flask_lambda_python36-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_lambda.py

```diff
@@ -12,30 +12,22 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import sys
 
-try:
-    from urllib import urlencode
-except ImportError:
-    from urllib.parse import urlencode
+from io import StringIO
+from urllib.parse import urlencode
 
 from flask import Flask
-
-try:
-    from cStringIO import StringIO
-except ImportError:
-    try:
-        from StringIO import StringIO
-    except ImportError:
-        from io import StringIO
-
-from werkzeug.wrappers import BaseRequest
+try: # werkzeug <= 2.0.3
+    from werkzeug.wrappers import BaseRequest
+except: # werkzeug > 2.1
+    from werkzeug.wrappers import Request as BaseRequest
 
 
 __version__ = '0.0.4'
 
 
 def make_environ(event):
     environ = {}
@@ -52,30 +44,32 @@
         environ[http_hdr_name] = hdr_value
 
     qs = event['queryStringParameters']
 
     environ['REQUEST_METHOD'] = event['httpMethod']
     environ['PATH_INFO'] = event['path']
     environ['QUERY_STRING'] = urlencode(qs) if qs else ''
-    environ['REMOTE_ADDR'] = event['requestContext']['identity']['sourceIp']
+
+    environ['REMOTE_ADDR'] = environ.get('X_FORWARDED_FOR')
+
     environ['HOST'] = '{}:{}'.format(
         environ.get('HTTP_HOST', ''),
         environ.get('HTTP_X_FORWARDED_PORT', ''),
     )
     environ['SCRIPT_NAME'] = ''
     environ['SERVER_NAME'] = 'SERVER_NAME'
 
-    environ['SERVER_PORT'] = environ['HTTP_X_FORWARDED_PORT']
+    environ['SERVER_PORT'] = environ.get('HTTP_X_FORWARDED_PORT', '')
     environ['SERVER_PROTOCOL'] = 'HTTP/1.1'
 
     environ['CONTENT_LENGTH'] = str(
         len(event['body']) if event['body'] else ''
     )
 
-    environ['wsgi.url_scheme'] = environ['HTTP_X_FORWARDED_PROTO']
+    environ['wsgi.url_scheme'] = environ.get('HTTP_X_FORWARDED_PROTO')
     environ['wsgi.input'] = StringIO(event['body'] or '')
     environ['wsgi.version'] = (1, 0)
     environ['wsgi.errors'] = sys.stderr
     environ['wsgi.multithread'] = False
     environ['wsgi.run_once'] = True
     environ['wsgi.multiprocess'] = False
```

