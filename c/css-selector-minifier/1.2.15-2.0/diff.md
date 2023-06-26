# Comparing `tmp/css_selector_minifier-1.2.15.tar.gz` & `tmp/css_selector_minifier-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "css_selector_minifier-1.2.15.tar", last modified: Sat Apr  1 00:47:41 2023, max compression
+gzip compressed data, was "css_selector_minifier-2.0.tar", last modified: Mon Jun 26 22:00:15 2023, max compression
```

## Comparing `css_selector_minifier-1.2.15.tar` & `css_selector_minifier-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 00:47:41.392528 css_selector_minifier-1.2.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-01 00:47:24.000000 css_selector_minifier-1.2.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-01 00:47:41.392528 css_selector_minifier-1.2.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-01 00:47:24.000000 css_selector_minifier-1.2.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 00:47:41.392528 css_selector_minifier-1.2.15/css_selector_minifier/
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-04-01 00:47:24.000000 css_selector_minifier-1.2.15/css_selector_minifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 00:47:41.392528 css_selector_minifier-1.2.15/css_selector_minifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-01 00:47:41.000000 css_selector_minifier-1.2.15/css_selector_minifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-01 00:47:41.000000 css_selector_minifier-1.2.15/css_selector_minifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 00:47:41.000000 css_selector_minifier-1.2.15/css_selector_minifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-01 00:47:41.000000 css_selector_minifier-1.2.15/css_selector_minifier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 00:47:41.392528 css_selector_minifier-1.2.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-01 00:47:24.000000 css_selector_minifier-1.2.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:00:15.962192 css_selector_minifier-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 22:00:04.000000 css_selector_minifier-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-26 22:00:15.962192 css_selector_minifier-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-26 22:00:04.000000 css_selector_minifier-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:00:15.962192 css_selector_minifier-2.0/css_selector_minifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-26 22:00:04.000000 css_selector_minifier-2.0/css_selector_minifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:00:15.962192 css_selector_minifier-2.0/css_selector_minifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-26 22:00:15.000000 css_selector_minifier-2.0/css_selector_minifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 22:00:15.000000 css_selector_minifier-2.0/css_selector_minifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:00:15.000000 css_selector_minifier-2.0/css_selector_minifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 22:00:15.000000 css_selector_minifier-2.0/css_selector_minifier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:00:15.962192 css_selector_minifier-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-26 22:00:04.000000 css_selector_minifier-2.0/setup.py
```

### Comparing `css_selector_minifier-1.2.15/LICENSE` & `css_selector_minifier-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `css_selector_minifier-1.2.15/PKG-INFO` & `css_selector_minifier-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: css_selector_minifier
-Version: 1.2.15
+Version: 2.0
 Summary: Minify css selectors in css, html, js files.
 Author: 0x1618 aka ctrlshifti (Maksymilian Sawicz)
 Author-email: <max.sawicz@gmail.com>
 Keywords: python,css,html,js,minify,css selectors,selector,selectors,minify css selectors
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `css_selector_minifier-1.2.15/README.md` & `css_selector_minifier-2.0/README.md`

 * *Files identical despite different names*

### Comparing `css_selector_minifier-1.2.15/css_selector_minifier/__init__.py` & `css_selector_minifier-2.0/css_selector_minifier/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,27 +23,31 @@
 	Args:
 		css (list): List of CSS file paths to be minified.
 		html (list): List of HTML file paths to be checked for CSS selectors to be minified.
 		js (list): List of JS file paths to be checked for CSS selectors to be minified.
 		start_prefix (str): Prefix added at the start of the selector to be minified.
 		end_prefix (str): Prefix added at the end of the selector to be minified.
 		min_letters (int): Minimum number of letters in the minified selector.
+		start_selector (str): Unique prefix that you want to put at the start of the minifed selector.
+		end_selector (str): Unique prefix that you want to put at the end of the minifed selector.
 
 	Raises:
 		ValueError: If `min_letters` is zero or negative.
 
 	Attributes:
 		prefix (dict): Dictionary containing start and end prefixes.
 		css (list): List of CSS file paths to be minified.
 		css_selectors (set): Set of unique CSS selectors found in `css` files.
 		name_map (dict): Dictionary containing mapping of CSS selectors with their minified counterparts.
 		html (list): List of HTML file paths to be checked for CSS selectors to be minified.
 		js (list): List of JS file paths to be checked for CSS selectors to be minified.
 		min_letters (int): Minimum number of letters in the minified selector.
 		regex_pattern (str): Regular expression pattern to match CSS selectors.
+		start_selector (str): Unique prefix that you want to put at the start of the minifed selector.
+		end_selector (str): Unique prefix that you want to put at the end of the minifed selector.
 
 	Methods:
 		Get_All_CSS_Selectors(self) -> set:
 			Returns a set of unique CSS selectors found in `css` files.
 
 		Generate_Minifed_Selectors(self) -> generator:
 			Returns a generator object which yields a series of minified selectors.
@@ -55,29 +59,31 @@
 			Replaces all CSS selectors in `css`, `html` and `js` files with their minified counterparts.
 			If `backup` is True, creates a backup of the original files before making changes.
 
 		Minify(self, backup=True) -> None:
 			Perfoms minification using above functions.
 	"""
 
-	def __init__(self, css=None, html=None, js=None, start_prefix='-s-', end_prefix='-e-', min_letters=1):
+	def __init__(self, css=None, html=None, js=None, start_prefix='-s-', end_prefix='-e-', min_letters=1, start_selector='', end_selector=''):
 		self.prefix = {
 			'start-prefix': start_prefix,
 			'end-prefix': end_prefix
 		}
 
 		self.css = css if css else []
 		self.css_selectors = set()
 		self.name_map = {}
 		self.html = html if html else []
 		self.js = js if js else []
 
 		self.min_letters = min_letters
+		self.start_selector = start_selector
+		self.end_selector = end_selector
 
-		self.regex_pattern = rf'^.*[.#]{self.prefix["start-prefix"]}.*{self.prefix["end-prefix"]}'
+		self.regex_pattern = rf'([.#])({self.prefix["start-prefix"]}[a-zA-Z0-9_-]+{self.prefix["end-prefix"]})'
 
 		if self.min_letters <= 0:
 			raise ValueError("min_letters cannot be equal to 0 or less than 0")
 
 	def Get_All_CSS_Selectors(self) -> set:
 		"""
 		Returns a set of unique CSS selectors found in `css` files.
@@ -88,14 +94,15 @@
 
 		paths = self.css
 
 		for path in paths:
 			with open(path, 'rb') as css_file:
 				css = css_file.read().decode()
 				for selector in re.findall(self.regex_pattern, css, re.MULTILINE):
+					selector = ''.join(selector)
 					selectors = filter(lambda selector: selector != '', selector.replace(',', '').split(' '))
 					for selector in selectors:
 						selector = selector.replace('\t', '')
 						if not re.search(self.regex_pattern, selector):
 							continue
 						self.css_selectors.add(selector)
 
@@ -122,15 +129,15 @@
 
 		Returns:
 			dict: Dictionary containing mapping of CSS selectors with their minified counterparts.
 		"""
 
 		generator = self.Generate_Minifed_Selectors()
 		for selector in self.css_selectors:
-			self.name_map[selector] = selector[0] + ''.join(next(generator))
+			self.name_map[selector] = selector[0] + self.start_selector + ''.join(next(generator)) + self.end_selector
 
 		return self.name_map
 
 	def Replace_CSS_Selectors_With_Minifed(self, backup=True) -> None:
 		"""
 		Replaces all CSS selectors in `css`, `html` and `js` files with their minified counterparts.
 		If `backup` is True, creates a backup of the original files before making changes.
@@ -138,31 +145,31 @@
 		Args:
 			backup (bool, optional): Whether to create a backup of the original files before making changes. Defaults to True.
 		Returns:
 			None
 		"""
 
 		for path in self.css + self.html + self.js:
-			with open(path, 'ab+') as file:
+			with open(path, 'a+', encoding='utf-8') as file:
 				file.seek(0)
-				new_css = file.read().decode()
+				new_css = file.read()
 
 				for old_selector, new_selector in self.name_map.items():
 					if path.split('.')[-1] in ['html', 'js']:
 						old_selector = ''.join(list(old_selector)[1:])
 						new_selector = ''.join(list(new_selector)[1:])
 						new_css = new_css.replace(old_selector, new_selector)
 					else:
 						new_css = new_css.replace(old_selector, new_selector)
 
 				if backup:
 					copyfile(path, path + f'-{time()}.bak')
 
 				file.truncate(0)
-				file.write(new_css.encode())
+				file.write(new_css)
 	
 	def Minify(self, backup=True) -> None:
 		"""
 		Perform minification.
 
 		Args:
 			backup (bool, optional): Whether to create a backup of the original files before making changes. Defaults to True.
@@ -171,17 +178,20 @@
 		"""
 
 		self.Get_All_CSS_Selectors()
 		self.Generate_Map_For_CSS_Selectors()
 		self.Replace_CSS_Selectors_With_Minifed(backup=backup)
 
 if __name__ == "__main__":
+	import glob
 	m = Minify_CSS_Names(
-		css=['src/style.css'],
-		html=['src/index.html'],
-		js=['src/main.js'],
+		css=['main.css'],
+		html=[],
+		js=[],
 		start_prefix='-s-',
 		end_prefix='-e-',
-		min_letters=2
+		min_letters=2,
+		start_selector='l',
+		end_selector='s'
 	)
 
 	m.Minify()
```

### Comparing `css_selector_minifier-1.2.15/css_selector_minifier.egg-info/PKG-INFO` & `css_selector_minifier-2.0/css_selector_minifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: css-selector-minifier
-Version: 1.2.15
+Version: 2.0
 Summary: Minify css selectors in css, html, js files.
 Author: 0x1618 aka ctrlshifti (Maksymilian Sawicz)
 Author-email: <max.sawicz@gmail.com>
 Keywords: python,css,html,js,minify,css selectors,selector,selectors,minify css selectors
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `css_selector_minifier-1.2.15/setup.py` & `css_selector_minifier-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '1.2.15'
+VERSION = '2.0'
 DESCRIPTION = 'Minify css selectors in css, html, js files.'
 LONG_DESCRIPTION = 'A package that allows you to easily minify css selectors in css, html, js files.'
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # Setting up
```

