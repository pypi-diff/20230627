# Comparing `tmp/lantana-2.6.6.tar.gz` & `tmp/lantana-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lantana-2.6.6.tar", last modified: Sun May 21 07:10:25 2023, max compression
+gzip compressed data, was "dist\lantana-2.7.0.tar", last modified: Tue Jun 27 12:49:59 2023, max compression
```

## Comparing `lantana-2.6.6.tar` & `lantana-2.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/
-drwxrwxrwx   0        0        0        0 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana/
--rw-rw-rw-   0        0        0      547 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/404.html
--rw-rw-rw-   0        0        0     8998 2023-05-21 07:10:20.000000 lantana-2.6.6/lantana/base.html
--rw-rw-rw-   0        0        0      306 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/breadcrumb.html
-drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana/css/
--rw-rw-rw-   0        0        0   210062 2023-05-21 06:29:23.000000 lantana-2.6.6/lantana/css/bootstrap-dark.min.css
--rw-rw-rw-   0        0        0    83555 2023-05-21 06:33:38.000000 lantana-2.6.6/lantana/css/bootstrap-icons.min.css
--rw-rw-rw-   0        0        0   155850 2023-05-21 06:31:31.000000 lantana-2.6.6/lantana/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     1152 2023-05-21 06:34:35.000000 lantana-2.6.6/lantana/css/default.min.css
--rw-rw-rw-   0        0        0     2705 2023-03-05 11:56:33.000000 lantana-2.6.6/lantana/css/theme.css
--rw-rw-rw-   0        0        0     1927 2023-05-21 06:35:24.000000 lantana-2.6.6/lantana/css/vs.min.css
-drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana/extensions/
--rw-rw-rw-   0        0        0     3125 2023-03-08 12:20:00.000000 lantana-2.6.6/lantana/extensions/mdx_cards.py
--rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.6.6/lantana/extensions/mdx_embedly.py
--rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.6.6/lantana/extensions/mdx_wsid.py
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/extensions/__init__.py
--rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/favicon.png
--rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/favicon.svg
-drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana/js/
--rw-rw-rw-   0        0        0    78749 2023-05-21 06:58:58.000000 lantana-2.6.6/lantana/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.6.6/lantana/js/highlight.min.js
--rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.6.6/lantana/js/jquery-3.6.1.slim.min.js
--rw-rw-rw-   0        0        0     5746 2023-03-05 11:57:02.000000 lantana-2.6.6/lantana/js/theme.js
--rw-rw-rw-   0        0        0     5285 2023-01-15 11:10:45.000000 lantana-2.6.6/lantana/main.html
--rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.6.6/lantana/mkdocs_theme.yml
--rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.6.6/lantana/nav.html
--rw-rw-rw-   0        0        0      536 2022-11-07 12:37:39.000000 lantana-2.6.6/lantana/sitemap.html
--rw-rw-rw-   0        0        0     1994 2023-05-21 07:00:03.000000 lantana-2.6.6/lantana/statics.html
--rw-rw-rw-   0        0        0      368 2023-02-16 13:48:35.000000 lantana-2.6.6/lantana/toc.html
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.6.6/lantana/__init__.py
--rw-rw-rw-   0        0        0     2682 2022-12-01 09:12:15.000000 lantana-2.6.6/lantana/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 07:10:25.000000 lantana-2.6.6/lantana.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      279 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      266 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/requires.txt
--rw-rw-rw-   0        0        0      927 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 07:10:24.000000 lantana-2.6.6/lantana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0      266 2023-05-21 07:10:25.000000 lantana-2.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.6.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 07:10:25.000000 lantana-2.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1129 2023-05-21 07:00:00.000000 lantana-2.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:49:59.000000 lantana-2.7.0/
+drwxrwxrwx   0        0        0        0 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana/
+-rw-rw-rw-   0        0        0      547 2022-10-28 12:09:36.000000 lantana-2.7.0/lantana/404.html
+-rw-rw-rw-   0        0        0     9085 2023-06-27 12:30:23.000000 lantana-2.7.0/lantana/base.html
+-rw-rw-rw-   0        0        0      306 2022-10-28 12:09:36.000000 lantana-2.7.0/lantana/breadcrumb.html
+drwxrwxrwx   0        0        0        0 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana/css/
+-rw-rw-rw-   0        0        0   210062 2023-05-21 06:29:23.000000 lantana-2.7.0/lantana/css/bootstrap-dark.min.css
+-rw-rw-rw-   0        0        0    83555 2023-05-21 06:33:38.000000 lantana-2.7.0/lantana/css/bootstrap-icons.min.css
+-rw-rw-rw-   0        0        0   155850 2023-05-21 06:31:31.000000 lantana-2.7.0/lantana/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1152 2023-05-21 06:34:35.000000 lantana-2.7.0/lantana/css/default.min.css
+-rw-rw-rw-   0        0        0     2705 2023-03-05 11:56:33.000000 lantana-2.7.0/lantana/css/theme.css
+-rw-rw-rw-   0        0        0     1927 2023-05-21 06:35:24.000000 lantana-2.7.0/lantana/css/vs.min.css
+drwxrwxrwx   0        0        0        0 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana/extensions/
+-rw-rw-rw-   0        0        0     3367 2023-06-27 12:47:44.000000 lantana-2.7.0/lantana/extensions/mdx_cards.py
+-rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.7.0/lantana/extensions/mdx_embedly.py
+-rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.7.0/lantana/extensions/mdx_wsid.py
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.7.0/lantana/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.7.0/lantana/favicon.png
+-rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.7.0/lantana/favicon.svg
+drwxrwxrwx   0        0        0        0 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana/js/
+-rw-rw-rw-   0        0        0    78749 2023-05-21 06:58:58.000000 lantana-2.7.0/lantana/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.7.0/lantana/js/highlight.min.js
+-rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.7.0/lantana/js/jquery-3.6.1.slim.min.js
+-rw-rw-rw-   0        0        0     5746 2023-03-05 11:57:02.000000 lantana-2.7.0/lantana/js/theme.js
+-rw-rw-rw-   0        0        0     5285 2023-01-15 11:10:45.000000 lantana-2.7.0/lantana/main.html
+-rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.7.0/lantana/mkdocs_theme.yml
+-rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.7.0/lantana/nav.html
+-rw-rw-rw-   0        0        0      536 2022-11-07 12:37:39.000000 lantana-2.7.0/lantana/sitemap.html
+-rw-rw-rw-   0        0        0     1994 2023-06-27 12:49:10.000000 lantana-2.7.0/lantana/statics.html
+-rw-rw-rw-   0        0        0      368 2023-02-16 13:48:35.000000 lantana-2.7.0/lantana/toc.html
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.7.0/lantana/__init__.py
+-rw-rw-rw-   0        0        0     2682 2022-12-01 09:12:15.000000 lantana-2.7.0/lantana/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      279 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      266 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      927 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 12:49:59.000000 lantana-2.7.0/lantana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      266 2023-06-27 12:49:59.000000 lantana-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:49:59.000000 lantana-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2023-06-27 12:49:25.000000 lantana-2.7.0/setup.py
```

### Comparing `lantana-2.6.6/lantana/404.html` & `lantana-2.7.0/lantana/404.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/base.html` & `lantana-2.7.0/lantana/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -65,40 +65,41 @@
 
   {% block extrahead %}
   {% endblock %}
 </head>
 <body>
   {% if not config.disable_header %}
     <header>
-    <nav class="navbar navbar-expand-sm navbar-toggleable-sm  border-bottom box-shadow mb-3">
+    <nav class="navbar navbar-expand-sm navbar-toggleable-sm  border-bottom box-shadow mb-3 {% if config.disable_header_when_printing %} print-hide {% endif %}">
       <div class="container">
           <a class="navbar-brand text-body" asp-area="" href="{{ "/"|url }}">
             {% if config.logo %}
             <img class="img-structure" src="{{ config.logo|url }}" alt="{{ config.site_name }}" width="28" height="28"/>
             {% endif%}
             {% if config.header_name %}
               {{ config.header_name }}
             {% else %}
               {{ config.site_name }}
             {% endif %}
           </a>
-          <div class="navbar-collapse collapse d-sm-inline-flex justify-content-between print-hide">
-              <p></p>
+          <div class="print-hide">
+          <div class="navbar-collapse collapse d-sm-inline-flex justify-content-between">
               <div class="d-none d-md-flex input-group mb-3" style="max-width: 300px;">
               {% if config.visible_search!=false %}
                   <input class="form-control me-2" type="search" id="searchbox" accesskey="/" placeholder="{{ config.site_name }}で検索" aria-label="検索"/>
                   <button class="btn btn-outline-secondary" type="button" onclick="search(false);">
                       <i class="bi bi-search"></i>
                   </button>
                   {% endif %}
               </div>
           </div>
+          </div>
       </div>
   </nav>
-  <nav class="navbar border-bottom box-shadow mb-3 d-md-none  print-hide">
+  <nav class="navbar border-bottom box-shadow mb-3 d-md-none print-hide">
     <div class="container">
         <div class="navbar-collapse d-flex">
           <p>
             <div class="d-flex input-group mb-3">
               {% if page and page.meta.disable_nav %}
               <!-- NAV -->
               {% else %}
```

### Comparing `lantana-2.6.6/lantana/css/bootstrap-dark.min.css` & `lantana-2.7.0/lantana/css/bootstrap-dark.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/css/bootstrap-icons.min.css` & `lantana-2.7.0/lantana/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/css/bootstrap.min.css` & `lantana-2.7.0/lantana/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/css/default.min.css` & `lantana-2.7.0/lantana/css/default.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/css/theme.css` & `lantana-2.7.0/lantana/css/theme.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/css/vs.min.css` & `lantana-2.7.0/lantana/css/vs.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/extensions/mdx_cards.py` & `lantana-2.7.0/lantana/extensions/mdx_cards.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,29 +30,37 @@
         if not filename.endswith(index_filename):
             card=Card()
             card.title = read_property(filename,'title')
             card.summary = read_property(filename,'summary')
             card.date = read_property(filename,'date')
             card.author = read_property(filename,'author')
             card.order = read_property(filename,'order',filename)
-            card.content_dir = filename.lstrip('docs/').rstrip('.md')
+            card.content_dir = remove_filename(filename)
             card.dir_title=dir_title
             cards.append(card)
     
     cards = natsorted(cards,key=lambda x:x.order)
     cards.reverse()
 
     html = '<div class="container-fluid">\n'
     for card in cards:
         html += '    <div class="row mb-3 card">\n'
         html += get_card_element(card.title, card.content_dir,card.summary,card.date,card.author,card.dir_title)
         html += '    </div>\n'
     html += '</div>'
     return html
 
+def remove_filename(filename):
+    """
+        docs/***.mdのようなファイル名を**のみに切り出す関数
+    """
+    filename = filename.replace("docs/","",1)
+    filename=filename[::-1].replace("dm.","",1)
+    return filename[::-1]
+
 def read_property(filename,key,default=""):
     """記事や.pagesファイルからプロパティを読みだす関数
     
     filename=ファイル名、key=プロパティの名前
     """
     with open(filename, "r", encoding="utf-8") as f:
         search=re.search(key+'\ *:\ *(.+)*\n*', f.read())
```

#### html2text {}

```diff
@@ -7,22 +7,25 @@
 get_thumbnail_element(dir, index_filename='index.md',pages_filename='.pages'):
 dir_title=read_property(f'docs/{dir}/{pages_filename}','title') filenames =
 natsorted(glob.glob(f'docs/{dir}/*.md')) cards=list() for i, filename in
 enumerate(filenames): if not filename.endswith(index_filename): card=Card()
 card.title = read_property(filename,'title') card.summary = read_property
 (filename,'summary') card.date = read_property(filename,'date') card.author =
 read_property(filename,'author') card.order = read_property
-(filename,'order',filename) card.content_dir = filename.lstrip('docs/').rstrip
-('.md') card.dir_title=dir_title cards.append(card) cards = natsorted
-(cards,key=lambda x:x.order) cards.reverse() html = '
+(filename,'order',filename) card.content_dir = remove_filename(filename)
+card.dir_title=dir_title cards.append(card) cards = natsorted(cards,key=lambda
+x:x.order) cards.reverse() html = '
 \n' for card in cards: html += '
 \n' html += get_card_element(card.title,
 card.content_dir,card.summary,card.date,card.author,card.dir_title) html += '
 \n' html += '
-' return html def read_property(filename,key,default=""):
+' return html def remove_filename(filename): """ docs/
+***.mdã®ãããªãã¡ã¤ã«åã**ã®ã¿ã«åãåºãé¢æ° """ filename
+= filename.replace("docs/","",1) filename=filename[::-1].replace("dm.","",1)
+return filename[::-1] def read_property(filename,key,default=""):
 """è¨äºã.pagesãã¡ã¤ã«ãããã­ããã£ãèª­ã¿ã ãé¢æ°
 filename=ãã¡ã¤ã«åãkey=ãã­ããã£ã®åå """ with open(filename,
 "r", encoding="utf-8") as f: search=re.search(key+'\ *:\ *(.+)*\n*', f.read())
 if search != None: return search.group(1) else: return default def
 get_card_element(title, dir,summary,date,author,dir_title): card = '' card +=
 f'
 {dir_title}
```

### Comparing `lantana-2.6.6/lantana/extensions/mdx_embedly.py` & `lantana-2.7.0/lantana/extensions/mdx_embedly.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/extensions/mdx_wsid.py` & `lantana-2.7.0/lantana/extensions/mdx_wsid.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/favicon.png` & `lantana-2.7.0/lantana/favicon.png`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/favicon.svg` & `lantana-2.7.0/lantana/favicon.svg`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/js/bootstrap.bundle.min.js` & `lantana-2.7.0/lantana/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/js/highlight.min.js` & `lantana-2.7.0/lantana/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/js/jquery-3.6.1.slim.min.js` & `lantana-2.7.0/lantana/js/jquery-3.6.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/js/theme.js` & `lantana-2.7.0/lantana/js/theme.js`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/main.html` & `lantana-2.7.0/lantana/main.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/nav.html` & `lantana-2.7.0/lantana/nav.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/sitemap.html` & `lantana-2.7.0/lantana/sitemap.html`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana/statics.html` & `lantana-2.7.0/lantana/statics.html`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       <tr>
         <th scope="row">リポジトリ</th>
         <td colspan="2"><a href="{{ config.repo_url }}">{% if config.repo_name %}{{ config.repo_name }}{% else %}{{ config.repo_url }}{% endif %}</a></td>
       </tr>
       {% endif %}
       <tr>
         <th scope="row">Lantanaのバージョン</th>
-        <td>WSOFT Lantana v2.6.6(tapioca)</td>
+        <td>WSOFT Lantana v2.7.0(tapioca)</td>
       </tr>
       <tr>
         <th scope="row">MkDocsのバージョン</th>
         <td>{{ mkdocs_version }}</td>
       </tr>
     </tbody>
   </table>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
                                         }}
 è¨äºã®ç·æ°          {{ ns.cnt }}
 ãµã¤ãã®æçµæ{{ build_date_utc }}
 ãµã¤ãã®ä½è    {{ config.author }}
                                         {%_if_config.repo_name_%}{
 ãªãã¸ããª          {_config.repo_name_}}{%_else_%}{
                                         {_config.repo_url_}}{%_endif_%}
-Lantanaã®ãã¼ã¸ã§ã�WSOFT Lantana v2.6.6
+Lantanaã®ãã¼ã¸ã§ã�WSOFT Lantana v2.7.0
                                         (tapioca)
 MkDocsã®ãã¼ã¸ã§ã{{ mkdocs_version }}
 Lantana
 Copyright 2022 WSOFT. All rights reserved.
 Lantanaã¯MkDocsããã®ä»ã®ãªã¼ãã³ã½ã¼ã¹
 ã½ããã¦ã§ã¢ã«ãã£ã¦å®ç¾ãã¾ããã
 Lantanaã®ãã¼ã ãã¼ã¸/GitHubãªãã¸ããª/WSOFTã®ãµã¤ã
```

### Comparing `lantana-2.6.6/lantana/__main__.py` & `lantana-2.7.0/lantana/__main__.py`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/lantana.egg-info/SOURCES.txt` & `lantana-2.7.0/lantana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/README.md` & `lantana-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `lantana-2.6.6/setup.py` & `lantana-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.6.6'
+VERSION = '2.7.0'
 
 setup(
     name="lantana",
     version=VERSION,
     url='http://wsoft-project.github.io/lantana/',
     license='MIT',
     description='Bootstrap theme for MkDocs',
```

