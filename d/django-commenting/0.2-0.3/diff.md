# Comparing `tmp/django-commenting-0.2.tar.gz` & `tmp/django-commenting-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-commenting-0.2.tar", last modified: Sat Jun 24 04:49:42 2023, max compression
+gzip compressed data, was "django-commenting-0.3.tar", last modified: Tue Jun 27 14:23:19 2023, max compression
```

## Comparing `django-commenting-0.2.tar` & `django-commenting-0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 04:49:42.935136 django-commenting-0.2/
--rw-rw-rw-   0        0        0     1577 2023-06-23 14:16:41.000000 django-commenting-0.2/LICENSE
--rw-rw-rw-   0        0        0       77 2023-06-23 14:47:04.000000 django-commenting-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2017 2023-06-24 04:49:42.935136 django-commenting-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-06-24 04:41:09.000000 django-commenting-0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-24 04:49:42.557923 django-commenting-0.2/commenting/
--rw-rw-rw-   0        0        0        0 2023-06-23 06:06:41.000000 django-commenting-0.2/commenting/__init__.py
--rw-rw-rw-   0        0        0      187 2023-06-23 06:23:33.000000 django-commenting-0.2/commenting/admin.py
--rw-rw-rw-   0        0        0      158 2023-06-23 06:06:41.000000 django-commenting-0.2/commenting/apps.py
--rw-rw-rw-   0        0        0      671 2023-06-22 02:50:24.000000 django-commenting-0.2/commenting/forms.py
--rw-rw-rw-   0        0        0      944 2023-06-23 06:26:55.000000 django-commenting-0.2/commenting/models.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:49:42.585884 django-commenting-0.2/commenting/templates/
--rw-rw-rw-   0        0        0     1789 2023-06-23 11:13:54.000000 django-commenting-0.2/commenting/templates/comment-form.html
--rw-rw-rw-   0        0        0     2140 2023-06-23 11:27:06.000000 django-commenting-0.2/commenting/templates/comment.html
-drwxrwxrwx   0        0        0        0 2023-06-24 04:49:42.899121 django-commenting-0.2/commenting/templatetags/
--rw-rw-rw-   0        0        0        0 2023-06-19 14:35:07.000000 django-commenting-0.2/commenting/templatetags/__init__.py
--rw-rw-rw-   0        0        0      619 2023-06-23 10:59:33.000000 django-commenting-0.2/commenting/templatetags/comment_form_tag.py
--rw-rw-rw-   0        0        0      911 2023-06-23 10:57:27.000000 django-commenting-0.2/commenting/templatetags/custom_tags.py
--rw-rw-rw-   0        0        0       63 2023-06-23 06:06:41.000000 django-commenting-0.2/commenting/tests.py
--rw-rw-rw-   0        0        0      351 2023-06-23 11:27:22.000000 django-commenting-0.2/commenting/urls.py
--rw-rw-rw-   0        0        0     2145 2023-06-23 11:28:48.000000 django-commenting-0.2/commenting/views.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:49:42.927123 django-commenting-0.2/django_commenting.egg-info/
--rw-rw-rw-   0        0        0     2017 2023-06-24 04:49:42.000000 django-commenting-0.2/django_commenting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-06-24 04:49:42.000000 django-commenting-0.2/django_commenting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 04:49:42.000000 django-commenting-0.2/django_commenting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 04:49:42.000000 django-commenting-0.2/django_commenting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      972 2023-06-24 04:49:42.936936 django-commenting-0.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-23 14:02:19.000000 django-commenting-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:23:19.797646 django-commenting-0.3/
+-rw-rw-rw-   0        0        0     1577 2023-06-23 14:16:41.000000 django-commenting-0.3/LICENSE
+-rw-rw-rw-   0        0        0       77 2023-06-23 14:47:04.000000 django-commenting-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2017 2023-06-27 14:23:19.797646 django-commenting-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-06-24 04:41:09.000000 django-commenting-0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-27 14:23:19.767653 django-commenting-0.3/commenting/
+-rw-rw-rw-   0        0        0        0 2023-06-23 06:06:41.000000 django-commenting-0.3/commenting/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-06-23 06:23:33.000000 django-commenting-0.3/commenting/admin.py
+-rw-rw-rw-   0        0        0      158 2023-06-23 06:06:41.000000 django-commenting-0.3/commenting/apps.py
+-rw-rw-rw-   0        0        0      671 2023-06-22 02:50:24.000000 django-commenting-0.3/commenting/forms.py
+-rw-rw-rw-   0        0        0      944 2023-06-23 06:26:55.000000 django-commenting-0.3/commenting/models.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:23:19.767653 django-commenting-0.3/commenting/templates/
+-rw-rw-rw-   0        0        0     2284 2023-06-27 14:22:00.000000 django-commenting-0.3/commenting/templates/comment-form.html
+-rw-rw-rw-   0        0        0     2140 2023-06-23 11:27:06.000000 django-commenting-0.3/commenting/templates/comment.html
+drwxrwxrwx   0        0        0        0 2023-06-27 14:23:19.772947 django-commenting-0.3/commenting/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-06-19 14:35:07.000000 django-commenting-0.3/commenting/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      619 2023-06-23 10:59:33.000000 django-commenting-0.3/commenting/templatetags/comment_form_tag.py
+-rw-rw-rw-   0        0        0      911 2023-06-23 10:57:27.000000 django-commenting-0.3/commenting/templatetags/custom_tags.py
+-rw-rw-rw-   0        0        0       63 2023-06-23 06:06:41.000000 django-commenting-0.3/commenting/tests.py
+-rw-rw-rw-   0        0        0      351 2023-06-23 11:27:22.000000 django-commenting-0.3/commenting/urls.py
+-rw-rw-rw-   0        0        0     2114 2023-06-27 14:22:15.000000 django-commenting-0.3/commenting/views.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:23:19.797646 django-commenting-0.3/django_commenting.egg-info/
+-rw-rw-rw-   0        0        0     2017 2023-06-27 14:23:19.000000 django-commenting-0.3/django_commenting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-06-27 14:23:19.000000 django-commenting-0.3/django_commenting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:23:19.000000 django-commenting-0.3/django_commenting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 14:23:19.000000 django-commenting-0.3/django_commenting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      972 2023-06-27 14:23:19.797646 django-commenting-0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-23 14:02:19.000000 django-commenting-0.3/setup.py
```

### Comparing `django-commenting-0.2/LICENSE` & `django-commenting-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/PKG-INFO` & `django-commenting-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-commenting
-Version: 0.2
+Version: 0.3
 Summary: A Django app to add nested commenting feature to the user django application.
 Home-page: https://www.example.com/
 Author: Marvin
 Author-email: aviavi@gmail.com
 License: MIT
 Keywords: Django,commenting,nested comments
 Classifier: Environment :: Web Environment
```

### Comparing `django-commenting-0.2/README.rst` & `django-commenting-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/commenting/forms.py` & `django-commenting-0.3/commenting/forms.py`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/commenting/models.py` & `django-commenting-0.3/commenting/models.py`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/commenting/templates/comment-form.html` & `django-commenting-0.3/commenting/templates/comment-form.html`

 * *Files 17% similar despite different names*

```diff
@@ -56,8 +56,22 @@
       No comments yet
   <!-- design this -->
   {% else %}
       {% for comment in comments %}
           {% include 'comment.html' with comment=comment replyobject=object %}
       {% endfor %}
   {% endif %}
-  </section>
+  </section>
+  <script>
+    function handleReply(response_id) {
+    const reply_form_container = document.querySelector(`#reply-form-container-${response_id}`)
+    if (reply_form_container) {
+        reply_form_container.style.display = 'block';
+    }
+}
+function handleCancel(response_id) {
+    const reply_form_container = document.querySelector(`#reply-form-container-${response_id}`)
+    if (reply_form_container) {
+        reply_form_container.style.display = 'none';
+    }
+}
+    </script>
```

### Comparing `django-commenting-0.2/commenting/templates/comment.html` & `django-commenting-0.3/commenting/templates/comment.html`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/commenting/templatetags/comment_form_tag.py` & `django-commenting-0.3/commenting/templatetags/comment_form_tag.py`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/commenting/templatetags/custom_tags.py` & `django-commenting-0.3/commenting/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/commenting/views.py` & `django-commenting-0.3/commenting/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             new_comment = comment_form.save(commit=False)
             new_comment.content_type = content_type
             new_comment.object_id = object_id
             new_comment.save()
             # absolutepath = request.build_absolute_uri()
             absolutepath = request.META.get('HTTP_REFERER')
             path =  absolutepath+'#'+str(new_comment.id)
-        return redirect('commenting:successpage', path=path)
+        return redirect(path)
     return redirect(absolutepath)
 
 
 def postreply(request):
     if request.method == "POST":
         form = CommentForm(request.POST)
         model_name = request.POST.get('model_name')
```

### Comparing `django-commenting-0.2/django_commenting.egg-info/PKG-INFO` & `django-commenting-0.3/django_commenting.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-commenting
-Version: 0.2
+Version: 0.3
 Summary: A Django app to add nested commenting feature to the user django application.
 Home-page: https://www.example.com/
 Author: Marvin
 Author-email: aviavi@gmail.com
 License: MIT
 Keywords: Django,commenting,nested comments
 Classifier: Environment :: Web Environment
```

### Comparing `django-commenting-0.2/django_commenting.egg-info/SOURCES.txt` & `django-commenting-0.3/django_commenting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-commenting-0.2/setup.cfg` & `django-commenting-0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 636f 6d6d 656e   = django-commen
 00000020: 7469 6e67 0d0a 7665 7273 696f 6e20 3d20  ting..version = 
-00000030: 302e 320d 0a64 6573 6372 6970 7469 6f6e  0.2..description
+00000030: 302e 330d 0a64 6573 6372 6970 7469 6f6e  0.3..description
 00000040: 203d 2041 2044 6a61 6e67 6f20 6170 7020   = A Django app 
 00000050: 746f 2061 6464 206e 6573 7465 6420 636f  to add nested co
 00000060: 6d6d 656e 7469 6e67 2066 6561 7475 7265  mmenting feature
 00000070: 2074 6f20 7468 6520 7573 6572 2064 6a61   to the user dja
 00000080: 6e67 6f20 6170 706c 6963 6174 696f 6e2e  ngo application.
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 000000a0: 6f6e 203d 2066 696c 653a 5245 4144 4d45  on = file:README
```

