# Comparing `tmp/resbaz-0.0.3.tar.gz` & `tmp/resbaz-0.0.4.tar.gz`

## Comparing `resbaz-0.0.3.tar` & `resbaz-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 resbaz-0.0.3/src/resbaz/__init__.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 resbaz-0.0.3/src/resbaz/certificate.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 resbaz-0.0.3/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 resbaz-0.0.3/LICENSE
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 resbaz-0.0.3/README.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 resbaz-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 resbaz-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 resbaz-0.0.4/src/resbaz/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 resbaz-0.0.4/src/resbaz/certificate.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 resbaz-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 resbaz-0.0.4/LICENSE
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 resbaz-0.0.4/README.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 resbaz-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 resbaz-0.0.4/PKG-INFO
```

### Comparing `resbaz-0.0.3/src/resbaz/certificate.py` & `resbaz-0.0.4/src/resbaz/certificate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-def get_certificate(name):
-  from PIL import Image, ImageDraw, ImageFont
-  import pandas as pd
-  from google.colab import files
-  import os
-  os.system("wget https://dl.dropboxusercontent.com/s/mxgxuqe9ejptl2k/Certificate.png -O Certificate.png --quiet")
-  os.system("https://dl.dropboxusercontent.com/s/hpd7246qdczd5wq/bellania.ttf?dl=0 -O bellania.ttf --quiet")
-  url = "https://drive.google.com/uc?export=download&id=1MUlHNAjZ_n40ciSW4f0enZgnz2AG5ilI"
-  form = pd.read_excel(url)
-  name_list = form['Name'].to_list()
-  if name in name_list:
-    im = Image.open("Certificate.png")
-    d = ImageDraw.Draw(im)
-    # location = (360, 350)
-    W, H = (960, 750)
-    # text_color = (0, 0, 0)
-    font = ImageFont.truetype("bellania.ttf", 25)
-    w,h = font.getsize(name)
-    d.text(((W-w)/2,(H-h)/2), name, font=font, fill="black")
-    # d.text(location, name, fill=text_color, font=font)
-    im.save(f"certificate_{name}.pdf")
-    print(f"Congratulations {name}, your certificate is ready!")
-    files.download(f"certificate_{name}.pdf")
-  else:
-    print("Sorry, the name you entered is not in the spreadsheet.")
+def get_certificate(name):
+  from PIL import Image, ImageDraw, ImageFont
+  import pandas as pd
+  from google.colab import files
+  import os
+  os.system("wget https://dl.dropboxusercontent.com/s/mxgxuqe9ejptl2k/Certificate.png -O Certificate.png --quiet")
+  os.system("wget https://dl.dropboxusercontent.com/s/hpd7246qdczd5wq/bellania.ttf?dl=0 -O bellania.ttf --quiet")
+  url = "https://drive.google.com/uc?export=download&id=1MUlHNAjZ_n40ciSW4f0enZgnz2AG5ilI"
+  form = pd.read_excel(url)
+  name_list = form['Name'].to_list()
+  if name in name_list:
+    im = Image.open("Certificate.png")
+    d = ImageDraw.Draw(im)
+    # location = (360, 350)
+    W, H = (960, 750)
+    # text_color = (0, 0, 0)
+    font = ImageFont.truetype("bellania.ttf", 25)
+    w,h = font.getsize(name)
+    d.text(((W-w)/2,(H-h)/2), name, font=font, fill="black")
+    # d.text(location, name, fill=text_color, font=font)
+    im.save(f"certificate_{name}.pdf")
+    print(f"Congratulations {name}, your certificate is ready!")
+    files.download(f"certificate_{name}.pdf")
+  else:
+    print("Sorry, the name you entered is not in the spreadsheet.")
```

### Comparing `resbaz-0.0.3/.gitignore` & `resbaz-0.0.4/.gitignore`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+pip-wheel-metadata/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
```

### Comparing `resbaz-0.0.3/LICENSE` & `resbaz-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `resbaz-0.0.3/PKG-INFO` & `resbaz-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resbaz
-Version: 0.0.3
+Version: 0.0.4
 Summary: ResBaz example package
 Project-URL: Homepage, https://resbaz.auckland.ac.nz/
 Author-email: Victor Gambarini <victor.gambarini@auckland.ac.nz>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

