# Comparing `tmp/texto_transformer-0.0.5.tar.gz` & `tmp/texto_transformer-0.0.6.tar.gz`

## Comparing `texto_transformer-0.0.5.tar` & `texto_transformer-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/requirements.txt
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0   111239 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/notebooks/ExemplosTextoTransformer.ipynb
--rw-r--r--   0        0        0   433294 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/notebooks/TestesTextoTransformer.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/__init__.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_medida.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_mensuradorenum.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_modeloenum.py
--rw-r--r--   0        0        0    28556 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_textotransformer.py
--rw-r--r--   0        0        0    23945 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_textotransformer_numpy.py
--rw-r--r--   0        0        0    14058 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_transformer.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_utiltempo.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/testes/test_utiltexto.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/__init__.py
--rw-r--r--   0        0        0    63721 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/textotransformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/mensurador/__init__.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/mensurador/medidas.py
--rw-r--r--   0        0        0    23551 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/mensurador/mensurador.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/mensurador/mensuradorenum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/modelo/__init__.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/modelo/modeloarguments.py
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/modelo/modeloenum.py
--rw-r--r--   0        0        0    43324 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/modelo/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/pln/__init__.py
--rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/pln/pln.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/util/__init__.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/util/utilambiente.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/util/utilarquivo.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/util/utilconstantes.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/util/utiltempo.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/textotransformer/util/utiltexto.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/LICENSE
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 texto_transformer-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0   114847 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/notebooks/ExemplosTextoTransformer.ipynb
+-rw-r--r--   0        0        0  1868809 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/notebooks/TestesTextoTransformer.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/__init__.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_medida.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_mensuradorenum.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_modeloenum.py
+-rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_textotransformer.py
+-rw-r--r--   0        0        0    23945 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_textotransformer_numpy.py
+-rw-r--r--   0        0        0    14364 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_transformer.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_utiltempo.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/testes/test_utiltexto.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/__init__.py
+-rw-r--r--   0        0        0    65763 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/textotransformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/mensurador/__init__.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/mensurador/medidas.py
+-rw-r--r--   0        0        0    26133 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/mensurador/mensurador.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/mensurador/mensuradorenum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/modelo/__init__.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/modelo/modeloarguments.py
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/modelo/modeloenum.py
+-rw-r--r--   0        0        0    43315 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/modelo/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/pln/__init__.py
+-rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/pln/pln.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/util/__init__.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/util/utilambiente.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/util/utilarquivo.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/util/utilconstantes.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/util/utiltempo.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/textotransformer/util/utiltexto.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 texto_transformer-0.0.6/PKG-INFO
```

### Comparing `texto_transformer-0.0.5/notebooks/ExemplosTextoTransformer.ipynb` & `texto_transformer-0.0.6/notebooks/ExemplosTextoTransformer.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9737535365226336%*

 * *Differences: {"'cells'": "{4: {'metadata': {'executionInfo': {'timestamp': 1687868960700, 'elapsed': 11}}}, 6: "*

 * *            "{'metadata': {'executionInfo': {'timestamp': 1687868980272, 'elapsed': 19582}, "*

 * *            "'outputId': 'aaff1919-2633-48bf-fee1-89192201c892'}, 'outputs': {0: {'text': {insert: "*

 * *            "[(2, '  Downloading texto_transformer-0.0.5-py3-none-any.whl (40 kB)\\n'), (3, "*

 * *            "'\\x1b[2K     \\x1b[90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\\x1b[0m "*

 * *            '\\x1b[32m40.7/40.7 kB\\ […]*

```diff
@@ -38,17 +38,17 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "executionInfo": {
-                    "elapsed": 2,
+                    "elapsed": 11,
                     "status": "ok",
-                    "timestamp": 1687431886444,
+                    "timestamp": 1687868960700,
                     "user": {
                         "displayName": "Osmar Oliveira Braz Junior",
                         "userId": "03010865824982624199"
                     },
                     "user_tz": 180
                 },
                 "id": "jzW-q8W3BxZV"
@@ -78,79 +78,94 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "executionInfo": {
-                    "elapsed": 16212,
+                    "elapsed": 19582,
                     "status": "ok",
-                    "timestamp": 1687431902654,
+                    "timestamp": 1687868980272,
                     "user": {
                         "displayName": "Osmar Oliveira Braz Junior",
                         "userId": "03010865824982624199"
                     },
                     "user_tz": 180
                 },
                 "id": "yYjPb3EMJb63",
-                "outputId": "67a90e5a-81bc-4f69-f6df-0dfb5a028e18"
+                "outputId": "aaff1919-2633-48bf-fee1-89192201c892"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Looking in indexes: https://pypi.org/simple, https://us-python.pkg.dev/colab-wheels/public/simple/\n",
                         "Collecting texto-transformer\n",
-                        "  Downloading texto_transformer-0.0.4-py3-none-any.whl (39 kB)\n",
-                        "Requirement already satisfied: spacy==3.5.2 in /usr/local/lib/python3.10/dist-packages (from texto-transformer) (3.5.2)\n",
+                        "  Downloading texto_transformer-0.0.5-py3-none-any.whl (40 kB)\n",
+                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m40.7/40.7 kB\u001b[0m \u001b[31m3.7 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
+                        "\u001b[?25hRequirement already satisfied: numpy==1.22.4 in /usr/local/lib/python3.10/dist-packages (from texto-transformer) (1.22.4)\n",
+                        "Requirement already satisfied: scipy==1.10.1 in /usr/local/lib/python3.10/dist-packages (from texto-transformer) (1.10.1)\n",
+                        "Collecting spacy==3.5.2 (from texto-transformer)\n",
+                        "  Downloading spacy-3.5.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (6.6 MB)\n",
+                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m6.6/6.6 MB\u001b[0m \u001b[31m52.2 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
+                        "\u001b[?25hRequirement already satisfied: torch==2.0.1 in /usr/local/lib/python3.10/dist-packages (from texto-transformer) (2.0.1+cu118)\n",
                         "Requirement already satisfied: tqdm==4.65.0 in /usr/local/lib/python3.10/dist-packages (from texto-transformer) (4.65.0)\n",
                         "Collecting transformers==4.26.1 (from texto-transformer)\n",
                         "  Downloading transformers-4.26.1-py3-none-any.whl (6.3 MB)\n",
-                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m6.3/6.3 MB\u001b[0m \u001b[31m72.6 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
+                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m6.3/6.3 MB\u001b[0m \u001b[31m91.2 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
                         "\u001b[?25hRequirement already satisfied: spacy-legacy<3.1.0,>=3.0.11 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (3.0.12)\n",
                         "Requirement already satisfied: spacy-loggers<2.0.0,>=1.0.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (1.0.4)\n",
                         "Requirement already satisfied: murmurhash<1.1.0,>=0.28.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (1.0.9)\n",
                         "Requirement already satisfied: cymem<2.1.0,>=2.0.2 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (2.0.7)\n",
                         "Requirement already satisfied: preshed<3.1.0,>=3.0.2 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (3.0.8)\n",
-                        "Requirement already satisfied: thinc<8.2.0,>=8.1.8 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (8.1.9)\n",
-                        "Requirement already satisfied: wasabi<1.2.0,>=0.9.1 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (1.1.1)\n",
+                        "Requirement already satisfied: thinc<8.2.0,>=8.1.8 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (8.1.10)\n",
+                        "Requirement already satisfied: wasabi<1.2.0,>=0.9.1 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (1.1.2)\n",
                         "Requirement already satisfied: srsly<3.0.0,>=2.4.3 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (2.4.6)\n",
                         "Requirement already satisfied: catalogue<2.1.0,>=2.0.6 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (2.0.8)\n",
                         "Requirement already satisfied: typer<0.8.0,>=0.3.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (0.7.0)\n",
-                        "Requirement already satisfied: pathy>=0.10.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (0.10.1)\n",
+                        "Requirement already satisfied: pathy>=0.10.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (0.10.2)\n",
                         "Requirement already satisfied: smart-open<7.0.0,>=5.2.1 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (6.3.0)\n",
-                        "Requirement already satisfied: numpy>=1.15.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (1.22.4)\n",
                         "Requirement already satisfied: requests<3.0.0,>=2.13.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (2.27.1)\n",
-                        "Requirement already satisfied: pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (1.10.7)\n",
+                        "Requirement already satisfied: pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (1.10.9)\n",
                         "Requirement already satisfied: jinja2 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (3.1.2)\n",
                         "Requirement already satisfied: setuptools in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (67.7.2)\n",
                         "Requirement already satisfied: packaging>=20.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (23.1)\n",
                         "Requirement already satisfied: langcodes<4.0.0,>=3.2.0 in /usr/local/lib/python3.10/dist-packages (from spacy==3.5.2->texto-transformer) (3.3.0)\n",
-                        "Requirement already satisfied: filelock in /usr/local/lib/python3.10/dist-packages (from transformers==4.26.1->texto-transformer) (3.12.0)\n",
+                        "Requirement already satisfied: filelock in /usr/local/lib/python3.10/dist-packages (from torch==2.0.1->texto-transformer) (3.12.2)\n",
+                        "Requirement already satisfied: typing-extensions in /usr/local/lib/python3.10/dist-packages (from torch==2.0.1->texto-transformer) (4.6.3)\n",
+                        "Requirement already satisfied: sympy in /usr/local/lib/python3.10/dist-packages (from torch==2.0.1->texto-transformer) (1.11.1)\n",
+                        "Requirement already satisfied: networkx in /usr/local/lib/python3.10/dist-packages (from torch==2.0.1->texto-transformer) (3.1)\n",
+                        "Requirement already satisfied: triton==2.0.0 in /usr/local/lib/python3.10/dist-packages (from torch==2.0.1->texto-transformer) (2.0.0)\n",
                         "Collecting huggingface-hub<1.0,>=0.11.0 (from transformers==4.26.1->texto-transformer)\n",
                         "  Downloading huggingface_hub-0.15.1-py3-none-any.whl (236 kB)\n",
-                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m236.8/236.8 kB\u001b[0m \u001b[31m26.7 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
+                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m236.8/236.8 kB\u001b[0m \u001b[31m25.0 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
                         "\u001b[?25hRequirement already satisfied: pyyaml>=5.1 in /usr/local/lib/python3.10/dist-packages (from transformers==4.26.1->texto-transformer) (6.0)\n",
                         "Requirement already satisfied: regex!=2019.12.17 in /usr/local/lib/python3.10/dist-packages (from transformers==4.26.1->texto-transformer) (2022.10.31)\n",
                         "Collecting tokenizers!=0.11.3,<0.14,>=0.11.1 (from transformers==4.26.1->texto-transformer)\n",
                         "  Downloading tokenizers-0.13.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (7.8 MB)\n",
-                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m7.8/7.8 MB\u001b[0m \u001b[31m100.5 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
-                        "\u001b[?25hRequirement already satisfied: fsspec in /usr/local/lib/python3.10/dist-packages (from huggingface-hub<1.0,>=0.11.0->transformers==4.26.1->texto-transformer) (2023.4.0)\n",
-                        "Requirement already satisfied: typing-extensions>=3.7.4.3 in /usr/local/lib/python3.10/dist-packages (from huggingface-hub<1.0,>=0.11.0->transformers==4.26.1->texto-transformer) (4.5.0)\n",
-                        "Requirement already satisfied: urllib3<1.27,>=1.21.1 in /usr/local/lib/python3.10/dist-packages (from requests<3.0.0,>=2.13.0->spacy==3.5.2->texto-transformer) (1.26.15)\n",
-                        "Requirement already satisfied: certifi>=2017.4.17 in /usr/local/lib/python3.10/dist-packages (from requests<3.0.0,>=2.13.0->spacy==3.5.2->texto-transformer) (2022.12.7)\n",
+                        "\u001b[2K     \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m7.8/7.8 MB\u001b[0m \u001b[31m100.1 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
+                        "\u001b[?25hRequirement already satisfied: cmake in /usr/local/lib/python3.10/dist-packages (from triton==2.0.0->torch==2.0.1->texto-transformer) (3.25.2)\n",
+                        "Requirement already satisfied: lit in /usr/local/lib/python3.10/dist-packages (from triton==2.0.0->torch==2.0.1->texto-transformer) (16.0.6)\n",
+                        "Requirement already satisfied: fsspec in /usr/local/lib/python3.10/dist-packages (from huggingface-hub<1.0,>=0.11.0->transformers==4.26.1->texto-transformer) (2023.6.0)\n",
+                        "Requirement already satisfied: urllib3<1.27,>=1.21.1 in /usr/local/lib/python3.10/dist-packages (from requests<3.0.0,>=2.13.0->spacy==3.5.2->texto-transformer) (1.26.16)\n",
+                        "Requirement already satisfied: certifi>=2017.4.17 in /usr/local/lib/python3.10/dist-packages (from requests<3.0.0,>=2.13.0->spacy==3.5.2->texto-transformer) (2023.5.7)\n",
                         "Requirement already satisfied: charset-normalizer~=2.0.0 in /usr/local/lib/python3.10/dist-packages (from requests<3.0.0,>=2.13.0->spacy==3.5.2->texto-transformer) (2.0.12)\n",
                         "Requirement already satisfied: idna<4,>=2.5 in /usr/local/lib/python3.10/dist-packages (from requests<3.0.0,>=2.13.0->spacy==3.5.2->texto-transformer) (3.4)\n",
                         "Requirement already satisfied: blis<0.8.0,>=0.7.8 in /usr/local/lib/python3.10/dist-packages (from thinc<8.2.0,>=8.1.8->spacy==3.5.2->texto-transformer) (0.7.9)\n",
                         "Requirement already satisfied: confection<1.0.0,>=0.0.1 in /usr/local/lib/python3.10/dist-packages (from thinc<8.2.0,>=8.1.8->spacy==3.5.2->texto-transformer) (0.0.4)\n",
                         "Requirement already satisfied: click<9.0.0,>=7.1.1 in /usr/local/lib/python3.10/dist-packages (from typer<0.8.0,>=0.3.0->spacy==3.5.2->texto-transformer) (8.1.3)\n",
-                        "Requirement already satisfied: MarkupSafe>=2.0 in /usr/local/lib/python3.10/dist-packages (from jinja2->spacy==3.5.2->texto-transformer) (2.1.2)\n",
-                        "Installing collected packages: tokenizers, huggingface-hub, transformers, texto-transformer\n",
-                        "Successfully installed huggingface-hub-0.15.1 texto-transformer-0.0.4 tokenizers-0.13.3 transformers-4.26.1\n"
+                        "Requirement already satisfied: MarkupSafe>=2.0 in /usr/local/lib/python3.10/dist-packages (from jinja2->spacy==3.5.2->texto-transformer) (2.1.3)\n",
+                        "Requirement already satisfied: mpmath>=0.19 in /usr/local/lib/python3.10/dist-packages (from sympy->torch==2.0.1->texto-transformer) (1.3.0)\n",
+                        "Installing collected packages: tokenizers, huggingface-hub, transformers, spacy, texto-transformer\n",
+                        "  Attempting uninstall: spacy\n",
+                        "    Found existing installation: spacy 3.5.3\n",
+                        "    Uninstalling spacy-3.5.3:\n",
+                        "      Successfully uninstalled spacy-3.5.3\n",
+                        "Successfully installed huggingface-hub-0.15.1 spacy-3.5.2 texto-transformer-0.0.5 tokenizers-0.13.3 transformers-4.26.1\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install texto-transformer"
             ]
         },
@@ -176,208 +191,208 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/",
                     "height": 437,
                     "referenced_widgets": [
-                        "e5d0b720b6e44032bdde51abe3ab66ae",
-                        "3d0a7924dd504fe796c231dd9dab6af6",
-                        "984f4e10b03142de846a9b548cd03ee1",
-                        "f1754c9c936f45148eede52269a23cd1",
-                        "3104bf335a73488a98ef16b649b8c7d6",
-                        "54a4f7326fc84bfd96fb078a5b55623a",
-                        "d916021a0e304a63a250f85f1b76c182",
-                        "8e780a80d87d4538b459d54d7fb1098c",
-                        "c008276891df4224b560c41d6270d698",
-                        "65e2f75e1b5c4110bc1296defaf71530",
-                        "a29a1024b0a5466895d09058a06e6600",
-                        "7ad161120f63445193991eb4e7658227",
-                        "1b5fe90ce8124fbca0234e852af12e94",
-                        "62c2599cdcf94002a60d7cc3f7351ac5",
-                        "d32b41f0ee18415ca2b2d6ab50cf5994",
-                        "5a5fcaae6225496eb0e1bccf380aac17",
-                        "7e4188173cda41f981e422535856b7fd",
-                        "d11dfed36a4942ac80987ce576ba6479",
-                        "51d7200dcebe4abe9b107a17caf377ec",
-                        "44a22e12a8e84a5e839ef414084c506e",
-                        "29bcb56493c5469591e22715e08cddd2",
-                        "54ca2b07a0a84f55abe065f3f6bd5f75",
-                        "ef70eda01a6a4e4ea5af1a02bde464fb",
-                        "47159ae7012d42f29457f357a55fe9ba",
-                        "b9d4705480c0452e901f62e63628a1fe",
-                        "7648c248e384496c976936862b74f05c",
-                        "01fc099c040b4d36972dd12335525c78",
-                        "c96f0e33d8c5408bb422ef56ab24c194",
-                        "ab751a87fc9d4bbeb307d167bff5e8ee",
-                        "b6511e1f0a7e4b3fbaf3630ed9c50e0a",
-                        "961eea22ba954cdf9a3dcae667481b1a",
-                        "b7097265ed434613b30a8fe27a864ceb",
-                        "70bcca82fe38413090b8d5663e24a56c",
-                        "387257fbcb1643b786bf0941ae5610cf",
-                        "aca22504983d40a180fece9cee23ea08",
-                        "3a9752ed8c8d4a12b79ddba66910ba72",
-                        "cd8270c931e442d39efb8973fc9e9cd0",
-                        "b03435fa402c410bab6ab02dfb91571f",
-                        "c7b144be7bfb40d295c219e3e93f6779",
-                        "822c56ddf5ae425ebe7bd297c5636c47",
-                        "65e95da4fe534e03a70ed10e4a474fcb",
-                        "bcc947dec8a24623bf924d207b28d0f5",
-                        "da392a60335b4e23b9ef4d9ab7d248a6",
-                        "52f3102280bb46bcbdf8a94df36d9d98",
-                        "0e645da118ca4e8bac47dc125da74f5d",
-                        "6be5065562b9420d90a9c6176b663c24",
-                        "d1dc69952e89475eb9e42adf4a7329b1",
-                        "07188e3eec194e0cba6fcc61cc5f44da",
-                        "9fa6d96a0c514163a6e505a9e4ba2c70",
-                        "a360d88b0ae448be817afed2c73e7a9d",
-                        "e1b5cf95cb64472580f27a973aa2f0bc",
-                        "c5bb3480a51e499692467bc8451775ee",
-                        "e52b2d45ab4547f09ea5f3b9d7995729",
-                        "266be8717bab4d68a59a6e3d1e1d5adc",
-                        "79b539b880fc491fbdb6c22420442c03",
-                        "924a5f514c3c4d0c88905af5e7ec60a4",
-                        "81b9ce3485394ef0bb441437519428be",
-                        "9d6c716b193b4fff8bd7fc106996ec9e",
-                        "9e3af83600794795abd87871c43d0370",
-                        "aad79e9c9eb04d79995c7dd969ad1a78",
-                        "98ee209c9c2045f4b22238f299f63dfb",
-                        "081704f030274e9288f609de308280d2",
-                        "5f621ccb93b54ae5b9e3197e2f8cf9e6",
-                        "ee68c66abaad4c3899ed3ddbf1391ee4",
-                        "5558b2cc33de4af180c5ed17434076c4",
-                        "0dbb03ff73b248d5818248daf81e5f07"
+                        "0ca863afa3b744c58d003a7abb968a01",
+                        "a443b8d2f7cb4986a777309b1588358e",
+                        "206eef0ebab34909b01404dd24aa8cb8",
+                        "981fec6d51ff4eaaa5a85e9dd4da3c13",
+                        "3befee64f555448ea3f58cecfc339a09",
+                        "1039dc32ba9c4383b57b448ffcc86cc9",
+                        "bb5cc90cb8824f6fb3f73bbc694d1ee5",
+                        "9d4a70dc69e349318d5a45f1c6059f4e",
+                        "138782a44372479c854b1ec1ca991a71",
+                        "0e953467cb29441cabf5b3e7bd88eb1c",
+                        "383a6954d36a495e99ee6dcf09683a97",
+                        "884b25c4a5394e729f99806c386ff676",
+                        "88a6c785822d45a7a72c405d1eff1e38",
+                        "bf515b6f22d44135bcd8f4a4ac5ebcaa",
+                        "f7c0e5759f0e425ea4f93f12f772ba6a",
+                        "94a40d35519c4e0c9389fccf8d115945",
+                        "1d40573de1714ffaa9151120015de335",
+                        "00989fc5d7a449c890e15189f85728bf",
+                        "d9dcba12e5b34d1e8731c6d85a1fe9b4",
+                        "7d417f141bc544cb9c18c38fe4615530",
+                        "d6185cc26bc249c08bf045c6d011760e",
+                        "4450c51bc917467f89b85143a4865ede",
+                        "5051db7676454e6a97ae8c04690bf43d",
+                        "0eba1863ded74d2486a5f2e4b8462162",
+                        "2cba5495711e44ff9b5492e58e53ec64",
+                        "841949ec05604cceaa6f136c7c3ab1a7",
+                        "243c6427c32543f99af0da1d93f2b355",
+                        "f05a9b49b93248ccbfca3f564dd68a9a",
+                        "e468da48ef494573a162ffc3e2413fe7",
+                        "6fde3705b86545cf897690b98d3e7f80",
+                        "233a8634c6534a37894db60ede579d10",
+                        "6fe3fec382544e4eae5e001abf1656af",
+                        "8909d8f6125941109b5f793edd60ee92",
+                        "7b7461f039a8467f9f827b28d58bb05e",
+                        "d9a3110c7cc542db8b42e4063b245a88",
+                        "57d017402476458ca812ac885dec609b",
+                        "f82d75cbdc624925a4db4f3a84d7f59c",
+                        "5a3397c35b7e41cf81a5a948606c1fdd",
+                        "4e0a13c7e4014f38bf86f8b1dcbacb5f",
+                        "0c85ba579f434af7914c9147d386ea2b",
+                        "9aff7433559141a588109c80603a0b47",
+                        "d66adb512213416db32c3aeb620e8829",
+                        "f3c0b4deb6a24328ad375b53c68c73ff",
+                        "60a41b950c3647ab82ba65f00865ba69",
+                        "644309d24db54231b6832124952ff213",
+                        "01bbefb6674749f790e833a3adc85400",
+                        "1b0c92c1ebe94bca90e224e0b00ea91f",
+                        "7001e450aa00445caa1610586155ad09",
+                        "187bb32f2ad945949954b74509ab1ad2",
+                        "4d77bf16f68d45829643df3c5c3d0f12",
+                        "bda4d4c295234e119b51978a150b7453",
+                        "4895a332b60f489783152d9280c84f9f",
+                        "07617a884ff145048b9d41068941ee32",
+                        "ba3f45477fa148349ebb67ef00b43430",
+                        "ae8428d2c91545beb5127933c9489626",
+                        "244441e4080849cca316048f8692b2a8",
+                        "c17473326ca2401d96dc4155bd0a0a1d",
+                        "f3215ac2a89447ad83182953eb0b614f",
+                        "83e5803dcdd0494484911ff3a829da5b",
+                        "f4502452877f451aa2b06ec4642187f9",
+                        "fe275efb2bd3462c9c691a252205b068",
+                        "5c265699431f4647a2350e223b9671e4",
+                        "29344f726b7e4e1680c8d9e4a7032a69",
+                        "ac118d13cd05406ca7689d80a7ab8cb3",
+                        "e7f957aedb7a4a48bba1f22769cf0195",
+                        "d1bbff516dab4f98b93d9bb02370f458"
                     ]
                 },
                 "executionInfo": {
-                    "elapsed": 69218,
+                    "elapsed": 76859,
                     "status": "ok",
-                    "timestamp": 1687431971868,
+                    "timestamp": 1687869057127,
                     "user": {
                         "displayName": "Osmar Oliveira Braz Junior",
                         "userId": "03010865824982624199"
                     },
                     "user_tz": 180
                 },
                 "id": "53YA78CmCPQr",
-                "outputId": "f4087888-a4bb-437d-9b68-63f87af18c28"
+                "outputId": "5986084e-0865-4723-d8a5-ab4132b195b9"
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "INFO:numexpr.utils:NumExpr defaulting to 2 threads.\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "e5d0b720b6e44032bdde51abe3ab66ae",
+                            "model_id": "0ca863afa3b744c58d003a7abb968a01",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Downloading (\u2026)lve/main/config.json:   0%|          | 0.00/647 [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "7ad161120f63445193991eb4e7658227",
+                            "model_id": "884b25c4a5394e729f99806c386ff676",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Downloading pytorch_model.bin:   0%|          | 0.00/438M [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Some weights of the model checkpoint at neuralmind/bert-base-portuguese-cased were not used when initializing BertModel: ['cls.predictions.decoder.weight', 'cls.predictions.transform.dense.bias', 'cls.predictions.bias', 'cls.seq_relationship.bias', 'cls.predictions.transform.LayerNorm.bias', 'cls.predictions.transform.dense.weight', 'cls.seq_relationship.weight', 'cls.predictions.transform.LayerNorm.weight']\n",
+                        "Some weights of the model checkpoint at neuralmind/bert-base-portuguese-cased were not used when initializing BertModel: ['cls.seq_relationship.weight', 'cls.predictions.transform.LayerNorm.bias', 'cls.predictions.decoder.weight', 'cls.seq_relationship.bias', 'cls.predictions.transform.LayerNorm.weight', 'cls.predictions.transform.dense.weight', 'cls.predictions.transform.dense.bias', 'cls.predictions.bias']\n",
                         "- This IS expected if you are initializing BertModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).\n",
                         "- This IS NOT expected if you are initializing BertModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "ef70eda01a6a4e4ea5af1a02bde464fb",
+                            "model_id": "5051db7676454e6a97ae8c04690bf43d",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Downloading (\u2026)okenizer_config.json:   0%|          | 0.00/43.0 [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "387257fbcb1643b786bf0941ae5610cf",
+                            "model_id": "7b7461f039a8467f9f827b28d58bb05e",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "Downloading (\u2026)solve/main/vocab.txt: 0.00B [00:00, ?B/s]"
+                            "Downloading (\u2026)solve/main/vocab.txt:   0%|          | 0.00/210k [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "0e645da118ca4e8bac47dc125da74f5d",
+                            "model_id": "644309d24db54231b6832124952ff213",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Downloading (\u2026)in/added_tokens.json:   0%|          | 0.00/2.00 [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "924a5f514c3c4d0c88905af5e7ec60a4",
+                            "model_id": "244441e4080849cca316048f8692b2a8",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Downloading (\u2026)cial_tokens_map.json:   0%|          | 0.00/112 [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "INFO:textotransformer.modelo.transformer:Classe Transformer carregada: ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, camadas_embeddings=2, estrategia_pooling=0, palavra_relevante=0).\n",
-                        "INFO:textotransformer.textotransformer:Utilizando embeddings do modelo da \u00daltima camada(s).\n",
-                        "INFO:textotransformer.util.utilambiente:Download do modelo spaCy pt_core_news_lg realizado!\n",
-                        "INFO:textotransformer.pln.pln:Modelo spaCy vers\u00e3o pt_core_news_lg carregado!\n",
-                        "INFO:textotransformer.pln.pln:Classe PLN carregada: ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, camadas_embeddings=2, estrategia_pooling=0, palavra_relevante=0).\n",
-                        "INFO:textotransformer.mensurador.mensurador:Classe Mensurador carregada: ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, camadas_embeddings=2, estrategia_pooling=0, palavra_relevante=0).\n",
+                        "INFO:textotransformer.modelo.transformer:Classe \"Transformer\" carregada: \"ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, abordagem_extracao_embeddings_camadas=2, estrategia_pooling=0, palavra_relevante=0)\".\n",
+                        "INFO:textotransformer.textotransformer:Utilizando abordagem para extra\u00e7\u00e3o dos embeddings das camadas do transfomer \"\u00daltima\" camada(s).\n",
+                        "INFO:textotransformer.util.utilambiente:Download do modelo spaCy \"pt_core_news_lg\" realizado!\n",
+                        "INFO:textotransformer.pln.pln:Modelo spaCy vers\u00e3o \"pt_core_news_lg\" carregado!\n",
+                        "INFO:textotransformer.pln.pln:Classe \"PLN\" carregada: \"ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, abordagem_extracao_embeddings_camadas=2, estrategia_pooling=0, palavra_relevante=0)\".\n",
+                        "INFO:textotransformer.mensurador.mensurador:Classe \"Mensurador\" carregada: \"ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, abordagem_extracao_embeddings_camadas=2, estrategia_pooling=0, palavra_relevante=0)\".\n",
                         "INFO:textotransformer.textotransformer:Sem GPU dispon\u00edvel, usando CPU.\n",
-                        "INFO:textotransformer.textotransformer:Classe TextoTransformer carregada: ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, camadas_embeddings=2, estrategia_pooling=0, palavra_relevante=0).\n"
+                        "INFO:textotransformer.textotransformer:Classe \"TextoTransformer\" carregada com os par\u00e2metros: \"ModeloArgumentos(max_seq_len=512, pretrained_model_name_or_path='neuralmind/bert-base-portuguese-cased', modelo_spacy='pt_core_news_lg', do_lower_case=False, output_attentions=False, output_hidden_states=True, abordagem_extracao_embeddings_camadas=2, estrategia_pooling=0, palavra_relevante=0)\".\n"
                     ]
                 }
             ],
             "source": [
                 "# Biblioteca texto-transformer\n",
                 "from textotransformer import TextoTransformer\n",
                 "\n",
@@ -391,32 +406,32 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "executionInfo": {
-                    "elapsed": 6,
+                    "elapsed": 11,
                     "status": "ok",
-                    "timestamp": 1687431971869,
+                    "timestamp": 1687869057127,
                     "user": {
                         "displayName": "Osmar Oliveira Braz Junior",
                         "userId": "03010865824982624199"
                     },
                     "user_tz": 180
                 },
                 "id": "X7Att6Otm3Pv",
-                "outputId": "ccfb056e-ca7a-492e-d8a7-aa5553f05497"
+                "outputId": "60eb97fd-c240-46b3-c0aa-a56c4bca245c"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Classe (TextoTransformer) com Transformer BertModel carregada com o modelo neuralmind/bert-base-portuguese-cased e NLP Portuguese carregado com o modelo pt_core_news_lg \n"
+                        "Classe (\"TextoTransformer\") com o Transformer \"BertModel\" carregada com o modelo \"neuralmind/bert-base-portuguese-cased\" e NLP \"Portuguese\" carregada com o modelo \"pt_core_news_lg\" \n"
                     ]
                 }
             ],
             "source": [
                 "print(modelo)"
             ]
         },
@@ -442,25 +457,25 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "executionInfo": {
-                    "elapsed": 629,
+                    "elapsed": 8,
                     "status": "ok",
-                    "timestamp": 1687431972495,
+                    "timestamp": 1687869057127,
                     "user": {
                         "displayName": "Osmar Oliveira Braz Junior",
                         "userId": "03010865824982624199"
                     },
                     "user_tz": 180
                 },
                 "id": "dFTQE2AQa2Mo",
-                "outputId": "3932cf1e-6fac-4a8e-c411-e59ba5dfcc72"
+                "outputId": "211003a8-c533-472c-8a55-2fccdf2040b8"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Texto: Bom Dia, professor.\n",
@@ -1051,36 +1066,37 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "VXymzdTVvDUH"
             },
             "source": [
-                "## 3.2 Recuperando embeddings de texto, senten\u00e7as, palavras e token"
+                "## 3.2 Recuperando embeddings de texto, senten\u00e7as, palavras e token\n",
+                "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "executionInfo": {
-                    "elapsed": 1085,
+                    "elapsed": 1269,
                     "status": "ok",
-                    "timestamp": 1687431973578,
+                    "timestamp": 1687869058392,
                     "user": {
                         "displayName": "Osmar Oliveira Braz Junior",
                         "userId": "03010865824982624199"
                     },
                     "user_tz": 180
                 },
                 "id": "ntwJ5XHMvFJ-",
-                "outputId": "4750162e-5341-4fd2-ae83-9c2d875014e9"
+                "outputId": "57696cf3-3d89-49f0-cc8c-84886f63fa38"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Um texto de tamanho      : 768\n",
@@ -1115,14 +1131,76 @@
                 "print(\"Cada palavra de tamanho  :\",len(embeddings_palavra[0]))\n",
                 "\n",
                 "# Recupera os embeddings dos tokens do texto\n",
                 "embeddings_token = modelo.getEmbeddingToken(texto)\n",
                 "print(\"\\nQuantidade de tokens     :\",len(embeddings_token))\n",
                 "print(\"Cada token de tamanho    :\",len(embeddings_token[0]))"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "eUBGHz4zy6z2"
+            },
+            "source": [
+                "## 3.3 Similaridade de textos"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {
+                "colab": {
+                    "base_uri": "https://localhost:8080/"
+                },
+                "executionInfo": {
+                    "elapsed": 7,
+                    "status": "ok",
+                    "timestamp": 1687869058393,
+                    "user": {
+                        "displayName": "Osmar Oliveira Braz Junior",
+                        "userId": "03010865824982624199"
+                    },
+                    "user_tz": 180
+                },
+                "id": "_qlRUgJ0z6u-",
+                "outputId": "9bd73770-a5ec-4e97-b4eb-50c8df87b9d3"
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        ">>>Sa\u00edda\n",
+                        "similaridadeCosseno(embeddingTexto1,embeddingTexto2) =  0.7183282375335693\n",
+                        "similaridadeCosseno(embeddingTexto1,embeddingTexto3) =  0.5837798714637756\n",
+                        "similaridadeCosseno(embeddingTexto2,embeddingTexto3) =  0.6247625946998596\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from textotransformer.mensurador.medidas import similaridadeCosseno\n",
+                "\n",
+                "texto1 = \"Adoro sorvete de manga.\"\n",
+                "texto2 = \"A manga \u00e9 uma fruta doce.\"\n",
+                "texto3 = \"Sujei a manga da camisa.\"\n",
+                "\n",
+                "embeddingTexto1 = modelo.getEmbeddingTexto(texto1)\n",
+                "embeddingTexto2 = modelo.getEmbeddingTexto(texto2)\n",
+                "embeddingTexto3 = modelo.getEmbeddingTexto(texto3)\n",
+                "\n",
+                "sim12 = similaridadeCosseno(embeddingTexto1, embeddingTexto2)\n",
+                "sim13 = similaridadeCosseno(embeddingTexto1, embeddingTexto3)\n",
+                "sim23 = similaridadeCosseno(embeddingTexto2, embeddingTexto3)\n",
+                "\n",
+                "print(\">>>Sa\u00edda\")\n",
+                "print(\"similaridadeCosseno(embeddingTexto1,embeddingTexto2) = \", sim12)\n",
+                "print(\"similaridadeCosseno(embeddingTexto1,embeddingTexto3) = \", sim13)\n",
+                "print(\"similaridadeCosseno(embeddingTexto2,embeddingTexto3) = \", sim23)"
+            ]
         }
     ],
     "metadata": {
         "colab": {
             "provenance": [
                 {
                     "file_id": "1ZQvuAVwA3IjybezQOXnrXMGAnMyZRuPU",
@@ -1141,161 +1219,177 @@
         },
         "kernelspec": {
             "display_name": "Python 3",
             "name": "python3"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
-                "01fc099c040b4d36972dd12335525c78": {
-                    "model_module": "@jupyter-widgets/base",
-                    "model_module_version": "1.2.0",
-                    "model_name": "LayoutModel",
+                "00989fc5d7a449c890e15189f85728bf": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "DescriptionStyleModel",
                     "state": {
-                        "_model_module": "@jupyter-widgets/base",
-                        "_model_module_version": "1.2.0",
-                        "_model_name": "LayoutModel",
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "DescriptionStyleModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
-                        "_view_name": "LayoutView",
-                        "align_content": null,
-                        "align_items": null,
-                        "align_self": null,
-                        "border": null,
-                        "bottom": null,
-                        "display": null,
-                        "flex": null,
-                        "flex_flow": null,
-                        "grid_area": null,
-                        "grid_auto_columns": null,
-                        "grid_auto_flow": null,
-                        "grid_auto_rows": null,
-                        "grid_column": null,
-                        "grid_gap": null,
-                        "grid_row": null,
-                        "grid_template_areas": null,
-                        "grid_template_columns": null,
-                        "grid_template_rows": null,
-                        "height": null,
-                        "justify_content": null,
-                        "justify_items": null,
-                        "left": null,
-                        "margin": null,
-                        "max_height": null,
-                        "max_width": null,
-                        "min_height": null,
-                        "min_width": null,
-                        "object_fit": null,
-                        "object_position": null,
-                        "order": null,
-                        "overflow": null,
-                        "overflow_x": null,
-                        "overflow_y": null,
-                        "padding": null,
-                        "right": null,
-                        "top": null,
-                        "visibility": null,
-                        "width": null
+                        "_view_name": "StyleView",
+                        "description_width": ""
                     }
                 },
-                "07188e3eec194e0cba6fcc61cc5f44da": {
+                "01bbefb6674749f790e833a3adc85400": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HTMLModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HTMLModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HTMLView",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_266be8717bab4d68a59a6e3d1e1d5adc",
+                        "layout": "IPY_MODEL_4d77bf16f68d45829643df3c5c3d0f12",
                         "placeholder": "\u200b",
-                        "style": "IPY_MODEL_79b539b880fc491fbdb6c22420442c03",
-                        "value": " 2.00/2.00 [00:00&lt;00:00, 40.3B/s]"
+                        "style": "IPY_MODEL_bda4d4c295234e119b51978a150b7453",
+                        "value": "Downloading (\u2026)in/added_tokens.json: 100%"
                     }
                 },
-                "081704f030274e9288f609de308280d2": {
+                "07617a884ff145048b9d41068941ee32": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
-                    "model_name": "DescriptionStyleModel",
+                    "model_name": "ProgressStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
-                        "_model_name": "DescriptionStyleModel",
+                        "_model_name": "ProgressStyleModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
+                        "bar_color": null,
                         "description_width": ""
                     }
                 },
-                "0dbb03ff73b248d5818248daf81e5f07": {
+                "0c85ba579f434af7914c9147d386ea2b": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "DescriptionStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "DescriptionStyleModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
                         "description_width": ""
                     }
                 },
-                "0e645da118ca4e8bac47dc125da74f5d": {
+                "0ca863afa3b744c58d003a7abb968a01": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HBoxModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HBoxModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HBoxView",
                         "box_style": "",
                         "children": [
-                            "IPY_MODEL_6be5065562b9420d90a9c6176b663c24",
-                            "IPY_MODEL_d1dc69952e89475eb9e42adf4a7329b1",
-                            "IPY_MODEL_07188e3eec194e0cba6fcc61cc5f44da"
+                            "IPY_MODEL_a443b8d2f7cb4986a777309b1588358e",
+                            "IPY_MODEL_206eef0ebab34909b01404dd24aa8cb8",
+                            "IPY_MODEL_981fec6d51ff4eaaa5a85e9dd4da3c13"
                         ],
-                        "layout": "IPY_MODEL_9fa6d96a0c514163a6e505a9e4ba2c70"
+                        "layout": "IPY_MODEL_3befee64f555448ea3f58cecfc339a09"
+                    }
+                },
+                "0e953467cb29441cabf5b3e7bd88eb1c": {
+                    "model_module": "@jupyter-widgets/base",
+                    "model_module_version": "1.2.0",
+                    "model_name": "LayoutModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/base",
+                        "_model_module_version": "1.2.0",
+                        "_model_name": "LayoutModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "LayoutView",
+                        "align_content": null,
+                        "align_items": null,
+                        "align_self": null,
+                        "border": null,
+                        "bottom": null,
+                        "display": null,
+                        "flex": null,
+                        "flex_flow": null,
+                        "grid_area": null,
+                        "grid_auto_columns": null,
+                        "grid_auto_flow": null,
+                        "grid_auto_rows": null,
+                        "grid_column": null,
+                        "grid_gap": null,
+                        "grid_row": null,
+                        "grid_template_areas": null,
+                        "grid_template_columns": null,
+                        "grid_template_rows": null,
+                        "height": null,
+                        "justify_content": null,
+                        "justify_items": null,
+                        "left": null,
+                        "margin": null,
+                        "max_height": null,
+                        "max_width": null,
+                        "min_height": null,
+                        "min_width": null,
+                        "object_fit": null,
+                        "object_position": null,
+                        "order": null,
+                        "overflow": null,
+                        "overflow_x": null,
+                        "overflow_y": null,
+                        "padding": null,
+                        "right": null,
+                        "top": null,
+                        "visibility": null,
+                        "width": null
                     }
                 },
-                "1b5fe90ce8124fbca0234e852af12e94": {
+                "0eba1863ded74d2486a5f2e4b8462162": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HTMLModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HTMLModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HTMLView",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_7e4188173cda41f981e422535856b7fd",
+                        "layout": "IPY_MODEL_f05a9b49b93248ccbfca3f564dd68a9a",
                         "placeholder": "\u200b",
-                        "style": "IPY_MODEL_d11dfed36a4942ac80987ce576ba6479",
-                        "value": "Downloading pytorch_model.bin: 100%"
+                        "style": "IPY_MODEL_e468da48ef494573a162ffc3e2413fe7",
+                        "value": "Downloading (\u2026)okenizer_config.json: 100%"
                     }
                 },
-                "266be8717bab4d68a59a6e3d1e1d5adc": {
+                "1039dc32ba9c4383b57b448ffcc86cc9": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1339,15 +1433,31 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "29bcb56493c5469591e22715e08cddd2": {
+                "138782a44372479c854b1ec1ca991a71": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "ProgressStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "ProgressStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "bar_color": null,
+                        "description_width": ""
+                    }
+                },
+                "187bb32f2ad945949954b74509ab1ad2": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1391,15 +1501,39 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "3104bf335a73488a98ef16b649b8c7d6": {
+                "1b0c92c1ebe94bca90e224e0b00ea91f": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "FloatProgressModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "FloatProgressModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "ProgressView",
+                        "bar_style": "success",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_4895a332b60f489783152d9280c84f9f",
+                        "max": 2,
+                        "min": 0,
+                        "orientation": "horizontal",
+                        "style": "IPY_MODEL_07617a884ff145048b9d41068941ee32",
+                        "value": 2
+                    }
+                },
+                "1d40573de1714ffaa9151120015de335": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1443,37 +1577,15 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "387257fbcb1643b786bf0941ae5610cf": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HBoxModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HBoxModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HBoxView",
-                        "box_style": "",
-                        "children": [
-                            "IPY_MODEL_aca22504983d40a180fece9cee23ea08",
-                            "IPY_MODEL_3a9752ed8c8d4a12b79ddba66910ba72",
-                            "IPY_MODEL_cd8270c931e442d39efb8973fc9e9cd0"
-                        ],
-                        "layout": "IPY_MODEL_b03435fa402c410bab6ab02dfb91571f"
-                    }
-                },
-                "3a9752ed8c8d4a12b79ddba66910ba72": {
+                "206eef0ebab34909b01404dd24aa8cb8": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "FloatProgressModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
@@ -1481,44 +1593,23 @@
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "ProgressView",
                         "bar_style": "success",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_65e95da4fe534e03a70ed10e4a474fcb",
-                        "max": 1,
+                        "layout": "IPY_MODEL_9d4a70dc69e349318d5a45f1c6059f4e",
+                        "max": 647,
                         "min": 0,
                         "orientation": "horizontal",
-                        "style": "IPY_MODEL_bcc947dec8a24623bf924d207b28d0f5",
-                        "value": 1
-                    }
-                },
-                "3d0a7924dd504fe796c231dd9dab6af6": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HTMLModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HTMLModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HTMLView",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_54a4f7326fc84bfd96fb078a5b55623a",
-                        "placeholder": "\u200b",
-                        "style": "IPY_MODEL_d916021a0e304a63a250f85f1b76c182",
-                        "value": "Downloading (\u2026)lve/main/config.json: 100%"
+                        "style": "IPY_MODEL_138782a44372479c854b1ec1ca991a71",
+                        "value": 647
                     }
                 },
-                "44a22e12a8e84a5e839ef414084c506e": {
+                "233a8634c6534a37894db60ede579d10": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "ProgressStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "ProgressStyleModel",
@@ -1526,36 +1617,15 @@
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
                         "bar_color": null,
                         "description_width": ""
                     }
                 },
-                "47159ae7012d42f29457f357a55fe9ba": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HTMLModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HTMLModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HTMLView",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_c96f0e33d8c5408bb422ef56ab24c194",
-                        "placeholder": "\u200b",
-                        "style": "IPY_MODEL_ab751a87fc9d4bbeb307d167bff5e8ee",
-                        "value": "Downloading (\u2026)okenizer_config.json: 100%"
-                    }
-                },
-                "51d7200dcebe4abe9b107a17caf377ec": {
+                "243c6427c32543f99af0da1d93f2b355": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1599,30 +1669,37 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "52f3102280bb46bcbdf8a94df36d9d98": {
+                "244441e4080849cca316048f8692b2a8": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
-                    "model_name": "DescriptionStyleModel",
+                    "model_name": "HBoxModel",
                     "state": {
+                        "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
-                        "_model_name": "DescriptionStyleModel",
+                        "_model_name": "HBoxModel",
                         "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "description_width": ""
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HBoxView",
+                        "box_style": "",
+                        "children": [
+                            "IPY_MODEL_c17473326ca2401d96dc4155bd0a0a1d",
+                            "IPY_MODEL_f3215ac2a89447ad83182953eb0b614f",
+                            "IPY_MODEL_83e5803dcdd0494484911ff3a829da5b"
+                        ],
+                        "layout": "IPY_MODEL_f4502452877f451aa2b06ec4642187f9"
                     }
                 },
-                "54a4f7326fc84bfd96fb078a5b55623a": {
+                "29344f726b7e4e1680c8d9e4a7032a69": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1666,30 +1743,54 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "54ca2b07a0a84f55abe065f3f6bd5f75": {
+                "2cba5495711e44ff9b5492e58e53ec64": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "FloatProgressModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "FloatProgressModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "ProgressView",
+                        "bar_style": "success",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_6fde3705b86545cf897690b98d3e7f80",
+                        "max": 43,
+                        "min": 0,
+                        "orientation": "horizontal",
+                        "style": "IPY_MODEL_233a8634c6534a37894db60ede579d10",
+                        "value": 43
+                    }
+                },
+                "383a6954d36a495e99ee6dcf09683a97": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "DescriptionStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "DescriptionStyleModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
                         "description_width": ""
                     }
                 },
-                "5558b2cc33de4af180c5ed17434076c4": {
+                "3befee64f555448ea3f58cecfc339a09": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1733,15 +1834,30 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "5a5fcaae6225496eb0e1bccf380aac17": {
+                "4450c51bc917467f89b85143a4865ede": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "DescriptionStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "DescriptionStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "description_width": ""
+                    }
+                },
+                "4895a332b60f489783152d9280c84f9f": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1785,15 +1901,15 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "5f621ccb93b54ae5b9e3197e2f8cf9e6": {
+                "4d77bf16f68d45829643df3c5c3d0f12": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1837,39 +1953,15 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "62c2599cdcf94002a60d7cc3f7351ac5": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "FloatProgressModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "FloatProgressModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "ProgressView",
-                        "bar_style": "success",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_51d7200dcebe4abe9b107a17caf377ec",
-                        "max": 438235074,
-                        "min": 0,
-                        "orientation": "horizontal",
-                        "style": "IPY_MODEL_44a22e12a8e84a5e839ef414084c506e",
-                        "value": 438235074
-                    }
-                },
-                "65e2f75e1b5c4110bc1296defaf71530": {
+                "4e0a13c7e4014f38bf86f8b1dcbacb5f": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1913,15 +2005,61 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "65e95da4fe534e03a70ed10e4a474fcb": {
+                "5051db7676454e6a97ae8c04690bf43d": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "HBoxModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "HBoxModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HBoxView",
+                        "box_style": "",
+                        "children": [
+                            "IPY_MODEL_0eba1863ded74d2486a5f2e4b8462162",
+                            "IPY_MODEL_2cba5495711e44ff9b5492e58e53ec64",
+                            "IPY_MODEL_841949ec05604cceaa6f136c7c3ab1a7"
+                        ],
+                        "layout": "IPY_MODEL_243c6427c32543f99af0da1d93f2b355"
+                    }
+                },
+                "57d017402476458ca812ac885dec609b": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "FloatProgressModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "FloatProgressModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "ProgressView",
+                        "bar_style": "success",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_9aff7433559141a588109c80603a0b47",
+                        "max": 209528,
+                        "min": 0,
+                        "orientation": "horizontal",
+                        "style": "IPY_MODEL_d66adb512213416db32c3aeb620e8829",
+                        "value": 209528
+                    }
+                },
+                "5a3397c35b7e41cf81a5a948606c1fdd": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -1962,112 +2100,70 @@
                         "overflow": null,
                         "overflow_x": null,
                         "overflow_y": null,
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
-                        "width": "20px"
-                    }
-                },
-                "6be5065562b9420d90a9c6176b663c24": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HTMLModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HTMLModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HTMLView",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_a360d88b0ae448be817afed2c73e7a9d",
-                        "placeholder": "\u200b",
-                        "style": "IPY_MODEL_e1b5cf95cb64472580f27a973aa2f0bc",
-                        "value": "Downloading (\u2026)in/added_tokens.json: 100%"
+                        "width": null
                     }
                 },
-                "70bcca82fe38413090b8d5663e24a56c": {
+                "5c265699431f4647a2350e223b9671e4": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "DescriptionStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "DescriptionStyleModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
                         "description_width": ""
                     }
                 },
-                "7648c248e384496c976936862b74f05c": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HTMLModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HTMLModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HTMLView",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_b7097265ed434613b30a8fe27a864ceb",
-                        "placeholder": "\u200b",
-                        "style": "IPY_MODEL_70bcca82fe38413090b8d5663e24a56c",
-                        "value": " 43.0/43.0 [00:00&lt;00:00, 562B/s]"
-                    }
-                },
-                "79b539b880fc491fbdb6c22420442c03": {
+                "60a41b950c3647ab82ba65f00865ba69": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "DescriptionStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "DescriptionStyleModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
                         "description_width": ""
                     }
                 },
-                "7ad161120f63445193991eb4e7658227": {
+                "644309d24db54231b6832124952ff213": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HBoxModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HBoxModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HBoxView",
                         "box_style": "",
                         "children": [
-                            "IPY_MODEL_1b5fe90ce8124fbca0234e852af12e94",
-                            "IPY_MODEL_62c2599cdcf94002a60d7cc3f7351ac5",
-                            "IPY_MODEL_d32b41f0ee18415ca2b2d6ab50cf5994"
+                            "IPY_MODEL_01bbefb6674749f790e833a3adc85400",
+                            "IPY_MODEL_1b0c92c1ebe94bca90e224e0b00ea91f",
+                            "IPY_MODEL_7001e450aa00445caa1610586155ad09"
                         ],
-                        "layout": "IPY_MODEL_5a5fcaae6225496eb0e1bccf380aac17"
+                        "layout": "IPY_MODEL_187bb32f2ad945949954b74509ab1ad2"
                     }
                 },
-                "7e4188173cda41f981e422535856b7fd": {
+                "6fde3705b86545cf897690b98d3e7f80": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2111,51 +2207,15 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "81b9ce3485394ef0bb441437519428be": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HTMLModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HTMLModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HTMLView",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_98ee209c9c2045f4b22238f299f63dfb",
-                        "placeholder": "\u200b",
-                        "style": "IPY_MODEL_081704f030274e9288f609de308280d2",
-                        "value": "Downloading (\u2026)cial_tokens_map.json: 100%"
-                    }
-                },
-                "822c56ddf5ae425ebe7bd297c5636c47": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "DescriptionStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "DescriptionStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "description_width": ""
-                    }
-                },
-                "8e780a80d87d4538b459d54d7fb1098c": {
+                "6fe3fec382544e4eae5e001abf1656af": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2199,37 +2259,58 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "924a5f514c3c4d0c88905af5e7ec60a4": {
+                "7001e450aa00445caa1610586155ad09": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "HTMLModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "HTMLModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HTMLView",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_ba3f45477fa148349ebb67ef00b43430",
+                        "placeholder": "\u200b",
+                        "style": "IPY_MODEL_ae8428d2c91545beb5127933c9489626",
+                        "value": " 2.00/2.00 [00:00&lt;00:00, 46.4B/s]"
+                    }
+                },
+                "7b7461f039a8467f9f827b28d58bb05e": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HBoxModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HBoxModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HBoxView",
                         "box_style": "",
                         "children": [
-                            "IPY_MODEL_81b9ce3485394ef0bb441437519428be",
-                            "IPY_MODEL_9d6c716b193b4fff8bd7fc106996ec9e",
-                            "IPY_MODEL_9e3af83600794795abd87871c43d0370"
+                            "IPY_MODEL_d9a3110c7cc542db8b42e4063b245a88",
+                            "IPY_MODEL_57d017402476458ca812ac885dec609b",
+                            "IPY_MODEL_f82d75cbdc624925a4db4f3a84d7f59c"
                         ],
-                        "layout": "IPY_MODEL_aad79e9c9eb04d79995c7dd969ad1a78"
+                        "layout": "IPY_MODEL_5a3397c35b7e41cf81a5a948606c1fdd"
                     }
                 },
-                "961eea22ba954cdf9a3dcae667481b1a": {
+                "7d417f141bc544cb9c18c38fe4615530": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "ProgressStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "ProgressStyleModel",
@@ -2237,39 +2318,115 @@
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
                         "bar_color": null,
                         "description_width": ""
                     }
                 },
-                "984f4e10b03142de846a9b548cd03ee1": {
+                "83e5803dcdd0494484911ff3a829da5b": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
-                    "model_name": "FloatProgressModel",
+                    "model_name": "HTMLModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
-                        "_model_name": "FloatProgressModel",
+                        "_model_name": "HTMLModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
-                        "_view_name": "ProgressView",
-                        "bar_style": "success",
+                        "_view_name": "HTMLView",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_8e780a80d87d4538b459d54d7fb1098c",
-                        "max": 647,
-                        "min": 0,
-                        "orientation": "horizontal",
-                        "style": "IPY_MODEL_c008276891df4224b560c41d6270d698",
-                        "value": 647
+                        "layout": "IPY_MODEL_e7f957aedb7a4a48bba1f22769cf0195",
+                        "placeholder": "\u200b",
+                        "style": "IPY_MODEL_d1bbff516dab4f98b93d9bb02370f458",
+                        "value": " 112/112 [00:00&lt;00:00, 3.78kB/s]"
+                    }
+                },
+                "841949ec05604cceaa6f136c7c3ab1a7": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "HTMLModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "HTMLModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HTMLView",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_6fe3fec382544e4eae5e001abf1656af",
+                        "placeholder": "\u200b",
+                        "style": "IPY_MODEL_8909d8f6125941109b5f793edd60ee92",
+                        "value": " 43.0/43.0 [00:00&lt;00:00, 465B/s]"
                     }
                 },
-                "98ee209c9c2045f4b22238f299f63dfb": {
+                "884b25c4a5394e729f99806c386ff676": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "HBoxModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "HBoxModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HBoxView",
+                        "box_style": "",
+                        "children": [
+                            "IPY_MODEL_88a6c785822d45a7a72c405d1eff1e38",
+                            "IPY_MODEL_bf515b6f22d44135bcd8f4a4ac5ebcaa",
+                            "IPY_MODEL_f7c0e5759f0e425ea4f93f12f772ba6a"
+                        ],
+                        "layout": "IPY_MODEL_94a40d35519c4e0c9389fccf8d115945"
+                    }
+                },
+                "88a6c785822d45a7a72c405d1eff1e38": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "HTMLModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "HTMLModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HTMLView",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_1d40573de1714ffaa9151120015de335",
+                        "placeholder": "\u200b",
+                        "style": "IPY_MODEL_00989fc5d7a449c890e15189f85728bf",
+                        "value": "Downloading pytorch_model.bin: 100%"
+                    }
+                },
+                "8909d8f6125941109b5f793edd60ee92": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "DescriptionStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "DescriptionStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "description_width": ""
+                    }
+                },
+                "94a40d35519c4e0c9389fccf8d115945": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2313,60 +2470,36 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "9d6c716b193b4fff8bd7fc106996ec9e": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "FloatProgressModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "FloatProgressModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "ProgressView",
-                        "bar_style": "success",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_5f621ccb93b54ae5b9e3197e2f8cf9e6",
-                        "max": 112,
-                        "min": 0,
-                        "orientation": "horizontal",
-                        "style": "IPY_MODEL_ee68c66abaad4c3899ed3ddbf1391ee4",
-                        "value": 112
-                    }
-                },
-                "9e3af83600794795abd87871c43d0370": {
+                "981fec6d51ff4eaaa5a85e9dd4da3c13": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HTMLModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HTMLModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HTMLView",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_5558b2cc33de4af180c5ed17434076c4",
+                        "layout": "IPY_MODEL_0e953467cb29441cabf5b3e7bd88eb1c",
                         "placeholder": "\u200b",
-                        "style": "IPY_MODEL_0dbb03ff73b248d5818248daf81e5f07",
-                        "value": " 112/112 [00:00&lt;00:00, 2.46kB/s]"
+                        "style": "IPY_MODEL_383a6954d36a495e99ee6dcf09683a97",
+                        "value": " 647/647 [00:00&lt;00:00, 12.9kB/s]"
                     }
                 },
-                "9fa6d96a0c514163a6e505a9e4ba2c70": {
+                "9aff7433559141a588109c80603a0b47": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2410,30 +2543,15 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "a29a1024b0a5466895d09058a06e6600": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "DescriptionStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "DescriptionStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "description_width": ""
-                    }
-                },
-                "a360d88b0ae448be817afed2c73e7a9d": {
+                "9d4a70dc69e349318d5a45f1c6059f4e": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2477,15 +2595,67 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "aad79e9c9eb04d79995c7dd969ad1a78": {
+                "a443b8d2f7cb4986a777309b1588358e": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "HTMLModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "HTMLModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HTMLView",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_1039dc32ba9c4383b57b448ffcc86cc9",
+                        "placeholder": "\u200b",
+                        "style": "IPY_MODEL_bb5cc90cb8824f6fb3f73bbc694d1ee5",
+                        "value": "Downloading (\u2026)lve/main/config.json: 100%"
+                    }
+                },
+                "ac118d13cd05406ca7689d80a7ab8cb3": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "ProgressStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "ProgressStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "bar_color": null,
+                        "description_width": ""
+                    }
+                },
+                "ae8428d2c91545beb5127933c9489626": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "DescriptionStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "DescriptionStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "description_width": ""
+                    }
+                },
+                "ba3f45477fa148349ebb67ef00b43430": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2529,51 +2699,105 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "ab751a87fc9d4bbeb307d167bff5e8ee": {
+                "bb5cc90cb8824f6fb3f73bbc694d1ee5": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "DescriptionStyleModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "DescriptionStyleModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/base",
                         "_view_module_version": "1.2.0",
                         "_view_name": "StyleView",
                         "description_width": ""
                     }
                 },
-                "aca22504983d40a180fece9cee23ea08": {
+                "bda4d4c295234e119b51978a150b7453": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "DescriptionStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "DescriptionStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "description_width": ""
+                    }
+                },
+                "bf515b6f22d44135bcd8f4a4ac5ebcaa": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "FloatProgressModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "FloatProgressModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "ProgressView",
+                        "bar_style": "success",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_d9dcba12e5b34d1e8731c6d85a1fe9b4",
+                        "max": 438235074,
+                        "min": 0,
+                        "orientation": "horizontal",
+                        "style": "IPY_MODEL_7d417f141bc544cb9c18c38fe4615530",
+                        "value": 438235074
+                    }
+                },
+                "c17473326ca2401d96dc4155bd0a0a1d": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HTMLModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HTMLModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HTMLView",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_c7b144be7bfb40d295c219e3e93f6779",
+                        "layout": "IPY_MODEL_fe275efb2bd3462c9c691a252205b068",
                         "placeholder": "\u200b",
-                        "style": "IPY_MODEL_822c56ddf5ae425ebe7bd297c5636c47",
-                        "value": "Downloading (\u2026)solve/main/vocab.txt: "
+                        "style": "IPY_MODEL_5c265699431f4647a2350e223b9671e4",
+                        "value": "Downloading (\u2026)cial_tokens_map.json: 100%"
+                    }
+                },
+                "d1bbff516dab4f98b93d9bb02370f458": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "DescriptionStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "DescriptionStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "description_width": ""
                     }
                 },
-                "b03435fa402c410bab6ab02dfb91571f": {
+                "d6185cc26bc249c08bf045c6d011760e": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2617,15 +2841,52 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "b6511e1f0a7e4b3fbaf3630ed9c50e0a": {
+                "d66adb512213416db32c3aeb620e8829": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "ProgressStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "ProgressStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "bar_color": null,
+                        "description_width": ""
+                    }
+                },
+                "d9a3110c7cc542db8b42e4063b245a88": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "HTMLModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "HTMLModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "HTMLView",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_4e0a13c7e4014f38bf86f8b1dcbacb5f",
+                        "placeholder": "\u200b",
+                        "style": "IPY_MODEL_0c85ba579f434af7914c9147d386ea2b",
+                        "value": "Downloading (\u2026)solve/main/vocab.txt: 100%"
+                    }
+                },
+                "d9dcba12e5b34d1e8731c6d85a1fe9b4": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2669,15 +2930,30 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "b7097265ed434613b30a8fe27a864ceb": {
+                "e468da48ef494573a162ffc3e2413fe7": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "DescriptionStyleModel",
+                    "state": {
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "DescriptionStyleModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/base",
+                        "_view_module_version": "1.2.0",
+                        "_view_name": "StyleView",
+                        "description_width": ""
+                    }
+                },
+                "e7f957aedb7a4a48bba1f22769cf0195": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2721,71 +2997,15 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "b9d4705480c0452e901f62e63628a1fe": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "FloatProgressModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "FloatProgressModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "ProgressView",
-                        "bar_style": "success",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_b6511e1f0a7e4b3fbaf3630ed9c50e0a",
-                        "max": 43,
-                        "min": 0,
-                        "orientation": "horizontal",
-                        "style": "IPY_MODEL_961eea22ba954cdf9a3dcae667481b1a",
-                        "value": 43
-                    }
-                },
-                "bcc947dec8a24623bf924d207b28d0f5": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "ProgressStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "ProgressStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "bar_color": null,
-                        "description_width": ""
-                    }
-                },
-                "c008276891df4224b560c41d6270d698": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "ProgressStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "ProgressStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "bar_color": null,
-                        "description_width": ""
-                    }
-                },
-                "c5bb3480a51e499692467bc8451775ee": {
+                "f05a9b49b93248ccbfca3f564dd68a9a": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2829,15 +3049,39 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "c7b144be7bfb40d295c219e3e93f6779": {
+                "f3215ac2a89447ad83182953eb0b614f": {
+                    "model_module": "@jupyter-widgets/controls",
+                    "model_module_version": "1.5.0",
+                    "model_name": "FloatProgressModel",
+                    "state": {
+                        "_dom_classes": [],
+                        "_model_module": "@jupyter-widgets/controls",
+                        "_model_module_version": "1.5.0",
+                        "_model_name": "FloatProgressModel",
+                        "_view_count": null,
+                        "_view_module": "@jupyter-widgets/controls",
+                        "_view_module_version": "1.5.0",
+                        "_view_name": "ProgressView",
+                        "bar_style": "success",
+                        "description": "",
+                        "description_tooltip": null,
+                        "layout": "IPY_MODEL_29344f726b7e4e1680c8d9e4a7032a69",
+                        "max": 112,
+                        "min": 0,
+                        "orientation": "horizontal",
+                        "style": "IPY_MODEL_ac118d13cd05406ca7689d80a7ab8cb3",
+                        "value": 112
+                    }
+                },
+                "f3c0b4deb6a24328ad375b53c68c73ff": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2881,15 +3125,15 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "c96f0e33d8c5408bb422ef56ab24c194": {
+                "f4502452877f451aa2b06ec4642187f9": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -2933,111 +3177,57 @@
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
                 },
-                "cd8270c931e442d39efb8973fc9e9cd0": {
+                "f7c0e5759f0e425ea4f93f12f772ba6a": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HTMLModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HTMLModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HTMLView",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_da392a60335b4e23b9ef4d9ab7d248a6",
+                        "layout": "IPY_MODEL_d6185cc26bc249c08bf045c6d011760e",
                         "placeholder": "\u200b",
-                        "style": "IPY_MODEL_52f3102280bb46bcbdf8a94df36d9d98",
-                        "value": " 210k/? [00:00&lt;00:00, 2.55MB/s]"
-                    }
-                },
-                "d11dfed36a4942ac80987ce576ba6479": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "DescriptionStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "DescriptionStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "description_width": ""
-                    }
-                },
-                "d1dc69952e89475eb9e42adf4a7329b1": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "FloatProgressModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "FloatProgressModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "ProgressView",
-                        "bar_style": "success",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_c5bb3480a51e499692467bc8451775ee",
-                        "max": 2,
-                        "min": 0,
-                        "orientation": "horizontal",
-                        "style": "IPY_MODEL_e52b2d45ab4547f09ea5f3b9d7995729",
-                        "value": 2
+                        "style": "IPY_MODEL_4450c51bc917467f89b85143a4865ede",
+                        "value": " 438M/438M [00:02&lt;00:00, 139MB/s]"
                     }
                 },
-                "d32b41f0ee18415ca2b2d6ab50cf5994": {
+                "f82d75cbdc624925a4db4f3a84d7f59c": {
                     "model_module": "@jupyter-widgets/controls",
                     "model_module_version": "1.5.0",
                     "model_name": "HTMLModel",
                     "state": {
                         "_dom_classes": [],
                         "_model_module": "@jupyter-widgets/controls",
                         "_model_module_version": "1.5.0",
                         "_model_name": "HTMLModel",
                         "_view_count": null,
                         "_view_module": "@jupyter-widgets/controls",
                         "_view_module_version": "1.5.0",
                         "_view_name": "HTMLView",
                         "description": "",
                         "description_tooltip": null,
-                        "layout": "IPY_MODEL_29bcb56493c5469591e22715e08cddd2",
+                        "layout": "IPY_MODEL_f3c0b4deb6a24328ad375b53c68c73ff",
                         "placeholder": "\u200b",
-                        "style": "IPY_MODEL_54ca2b07a0a84f55abe065f3f6bd5f75",
-                        "value": " 438M/438M [00:03&lt;00:00, 114MB/s]"
+                        "style": "IPY_MODEL_60a41b950c3647ab82ba65f00865ba69",
+                        "value": " 210k/210k [00:00&lt;00:00, 2.95MB/s]"
                     }
                 },
-                "d916021a0e304a63a250f85f1b76c182": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "DescriptionStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "DescriptionStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "description_width": ""
-                    }
-                },
-                "da392a60335b4e23b9ef4d9ab7d248a6": {
+                "fe275efb2bd3462c9c691a252205b068": {
                     "model_module": "@jupyter-widgets/base",
                     "model_module_version": "1.2.0",
                     "model_name": "LayoutModel",
                     "state": {
                         "_model_module": "@jupyter-widgets/base",
                         "_model_module_version": "1.2.0",
                         "_model_name": "LayoutModel",
@@ -3080,126 +3270,14 @@
                         "overflow_y": null,
                         "padding": null,
                         "right": null,
                         "top": null,
                         "visibility": null,
                         "width": null
                     }
-                },
-                "e1b5cf95cb64472580f27a973aa2f0bc": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "DescriptionStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "DescriptionStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "description_width": ""
-                    }
-                },
-                "e52b2d45ab4547f09ea5f3b9d7995729": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "ProgressStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "ProgressStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "bar_color": null,
-                        "description_width": ""
-                    }
-                },
-                "e5d0b720b6e44032bdde51abe3ab66ae": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HBoxModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HBoxModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HBoxView",
-                        "box_style": "",
-                        "children": [
-                            "IPY_MODEL_3d0a7924dd504fe796c231dd9dab6af6",
-                            "IPY_MODEL_984f4e10b03142de846a9b548cd03ee1",
-                            "IPY_MODEL_f1754c9c936f45148eede52269a23cd1"
-                        ],
-                        "layout": "IPY_MODEL_3104bf335a73488a98ef16b649b8c7d6"
-                    }
-                },
-                "ee68c66abaad4c3899ed3ddbf1391ee4": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "ProgressStyleModel",
-                    "state": {
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "ProgressStyleModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/base",
-                        "_view_module_version": "1.2.0",
-                        "_view_name": "StyleView",
-                        "bar_color": null,
-                        "description_width": ""
-                    }
-                },
-                "ef70eda01a6a4e4ea5af1a02bde464fb": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HBoxModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HBoxModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HBoxView",
-                        "box_style": "",
-                        "children": [
-                            "IPY_MODEL_47159ae7012d42f29457f357a55fe9ba",
-                            "IPY_MODEL_b9d4705480c0452e901f62e63628a1fe",
-                            "IPY_MODEL_7648c248e384496c976936862b74f05c"
-                        ],
-                        "layout": "IPY_MODEL_01fc099c040b4d36972dd12335525c78"
-                    }
-                },
-                "f1754c9c936f45148eede52269a23cd1": {
-                    "model_module": "@jupyter-widgets/controls",
-                    "model_module_version": "1.5.0",
-                    "model_name": "HTMLModel",
-                    "state": {
-                        "_dom_classes": [],
-                        "_model_module": "@jupyter-widgets/controls",
-                        "_model_module_version": "1.5.0",
-                        "_model_name": "HTMLModel",
-                        "_view_count": null,
-                        "_view_module": "@jupyter-widgets/controls",
-                        "_view_module_version": "1.5.0",
-                        "_view_name": "HTMLView",
-                        "description": "",
-                        "description_tooltip": null,
-                        "layout": "IPY_MODEL_65e2f75e1b5c4110bc1296defaf71530",
-                        "placeholder": "\u200b",
-                        "style": "IPY_MODEL_a29a1024b0a5466895d09058a06e6600",
-                        "value": " 647/647 [00:00&lt;00:00, 20.3kB/s]"
-                    }
                 }
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `texto_transformer-0.0.5/testes/test_medida.py` & `texto_transformer-0.0.6/testes/test_medida.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/testes/test_mensuradorenum.py` & `texto_transformer-0.0.6/testes/test_mensuradorenum.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/testes/test_modeloenum.py` & `texto_transformer-0.0.6/testes/test_modeloenum.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/testes/test_textotransformer.py` & `texto_transformer-0.0.6/testes/test_textotransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,34 @@
     # Testes getSaidaRede 
     def test_getSaidaRede(self):
         logger.info("Testando o getSaidaRede")
         
         # Valores de entrada                
         texto = "Adoro sorvete de manga."
         
+        # Tokeniza o texto
+        texto_tokenizado = self.modelo.getTransformer().tokenize(texto)
+        
         # Valores de saída
-        saida = self.modelo.getSaidaRede(texto)
+        saida = self.modelo.getSaidaRede(texto_tokenizado)
         
         # Testa o tamanho do dicionário
         self.assertEqual(len(saida), 7) 
         
     # Testes getSaidaRedeCamada
     def test_getSaidaRedeCamada(self):
         logger.info("Testando o getSaidaRedeCamada")
          
         # Valores de entrada       
         texto = "Adoro sorvete de manga."
         
+        texto_tokenizado = self.modelo.getTransformer().tokenize(texto)
+        
         # Valores de saída
-        saida = self.modelo.getSaidaRedeCamada(texto, 2) # Camada 2 - Ultima camada dos transformers
+        saida = self.modelo.getSaidaRedeCamada(texto_tokenizado, 2) # Camada 2 - Ultima camada dos transformers
         
         # Testa o tamanho do dicionário
         self.assertEqual(len(saida), 9)
     
     # Testes getCodificacaoCompleta string
     def test_getCodificacaoCompleta_string(self):
         logger.info("Testando o getCodificacaoCompleta com string")
```

### Comparing `texto_transformer-0.0.5/testes/test_textotransformer_numpy.py` & `texto_transformer-0.0.6/testes/test_textotransformer_numpy.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/testes/test_transformer.py` & `texto_transformer-0.0.6/testes/test_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,16 +127,19 @@
     # Testes getSaidaRede String
     def test_getSaidaRede_string(self):
         logger.info("Testando o getSaidaRede com string")
          
         # Valores de entrada        
         texto = "Adoro sorvete de manga."
         
+        # Tokeniza o texto
+        texto_tokenizado = self.modelo.tokenize(texto)
+        
         # Valores de saída
-        saida = self.modelo.getSaidaRede(texto)
+        saida = self.modelo.getSaidaRede(texto_tokenizado)
         
         # Testa o tamanho do dicionário
         self.assertEqual(len(saida), 7) 
         
         # Testa o nome das chaves
         self.assertTrue("token_embeddings" in saida)
         self.assertTrue("input_ids" in saida)
@@ -174,16 +177,19 @@
     # Testes getSaidaRede Lista de Strings
     def test_getSaidaRede_lista_string(self):
         logger.info("Testando o getSaidaRede com lista de strings")
          
         # Valores de entrada       
         texto = ["Adoro sorvete de manga.","Sujei a manga da camisa."]
         
+        # Tokeniza o texto
+        texto_tokenizado = self.modelo.tokenize(texto)
+        
         # Valores de saída
-        saida = self.modelo.getSaidaRede(texto)
+        saida = self.modelo.getSaidaRede(texto_tokenizado)
         
         # Testa o tamanho do dicionário
         self.assertEqual(len(saida), 7) 
         
         # Testa o nome das chaves
         self.assertTrue("token_embeddings" in saida)
         self.assertTrue("input_ids" in saida)
@@ -229,18 +235,21 @@
     # Testes getSaidaRedeCamada String
     def test_getSaidaRedeCamada_string(self):
         logger.info("Testando o getSaidaRedeCamada com strings")
         
         # Valores de entrada        
         texto = ["Adoro sorvete de manga.","Sujei a manga da camisa."]
         
+        # Tokeniza o texto
+        texto_tokenizado = self.modelo.tokenize(texto)
+        
         # Valores de saída
         # Abordagem extração de embeddings das camadas
         # 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últimas/5-Soma de todas
-        saida = self.modelo.getSaidaRedeCamada(texto, 2)
+        saida = self.modelo.getSaidaRedeCamada(texto_tokenizado, 2)
         
         # Testa o tamanho do dicionário
         self.assertEqual(len(saida), 9) 
         
         # Testa o nome das chaves
         self.assertTrue("token_embeddings" in saida)
         self.assertTrue("input_ids" in saida)
```

### Comparing `texto_transformer-0.0.5/testes/test_utiltempo.py` & `texto_transformer-0.0.6/testes/test_utiltempo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/testes/test_utiltexto.py` & `texto_transformer-0.0.6/testes/test_utiltexto.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/textotransformer.py` & `texto_transformer-0.0.6/textotransformer/textotransformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     estrategia_pooling=0,                       # 0 - MEAN estratégia média / 1 - MAX  estratégia maior
     palavra_relevante=0                         # 0 - Considera todas as palavras das sentenças / 1 - Desconsidera as stopwords / 2 - Considera somente as palavras substantivas
 )
 
 class TextoTransformer:
     
     ''' 
-    Carrega e cria um objeto da classe TextoTransformer para manipular um modelo de linguagem baseado e transformer.
-    Manipula embeddings de tokens, palavras, sentenças e textos.
+    A classe carrega e cria um objeto para manipular um modelo de linguagem baseado e transformer. 
+    Permite recuperar e manipular embeddings recuperados de tokens, palavras, sentenças e textos.
      
     Parâmetros:
        `pretrained_model_name_or_path` - Se for um caminho de arquivo no disco, carrega o modelo a partir desse caminho. Se não for um caminho, ele primeiro faz o download do repositório de modelos do Huggingface com esse nome. Valor default: 'neuralmind/bert-base-portuguese-cased'.                  
-       `modelo_spacy` - Nome do modelo a ser instalado e carregado pela ferramenta de pln spaCy. Valor default 'pt_core_news_lg'.                       
-       `abordagem_extracao_embeddings_camadas` - Especifica a abordagem para a extração dos embeddings das camadas do transformer. Valor default '2'. Valores possíveis: 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últimas/5-Todas.
-       `device` - Dispositivo (como 'cuda' / 'cpu') que deve ser usado para computação. Se none, verifica se uma GPU pode ser usada.
+       `modelo_spacy` - Nome do modelo spaCy a ser instalado e carregado pela ferramenta de pln spaCy. Valor default 'pt_core_news_lg'.
+       `abordagem_extracao_embeddings_camadas` - Especifica a abordagem padrão para a extração dos embeddings das camadas do transformer. Valor default '2'. Valores possíveis: 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últimas/5-Todas.
+       `device` - Dispositivo (como 'cuda' / 'cpu') que deve ser usado para o processamento. Se `None`, verifica se uma GPU pode ser usada. Se a GPU estiver disponível será usada no processamento. Valor default 'None'.
     ''' 
     
     # Construtor da classe
     def __init__(self, pretrained_model_name_or_path: str ="neuralmind/bert-base-portuguese-cased", 
                        modelo_spacy: str ="pt_core_news_lg",
                        abordagem_extracao_embeddings_camadas: int = 2,
                        device = None):
@@ -74,19 +74,14 @@
                     
         # Especifica camadas para recuperar os embeddings
         model_args.abordagem_extracao_embeddings_camadas = abordagem_extracao_embeddings_camadas
       
         # Carrega o spaCy
         self.pln = PLN(modelo_args=model_args)
                         
-        # Constroi um mensurador
-        self.mensurador = Mensurador(modelo_args=model_args, 
-                                     transformer=self.transformer, 
-                                     pln=self.pln)        
-    
         # Verifica se é possível usar GPU
         if device is None:
             if torch.cuda.is_available():    
                 device = "cuda"
                 logger.info("Existem\"{}\" GPU(s) disponíveis.".format(torch.cuda.device_count()))
                 logger.info("Iremos usar a GPU:\"{}\".".format(torch.cuda.get_device_name(0)))
 
@@ -94,15 +89,22 @@
                 device = "cpu"
                 logger.info("Sem GPU disponível, usando CPU.")
             
             # Diz ao PyTorch para usar o dispositvo (GPU ou CPU)
             self._target_device = torch.device(device)
         else:
             # Usa o device informado
+            logger.info("Usando dispositivo informado:\"{}\".".format(device))
             self._target_device = torch.device(device)
+            
+        # Constroi um mensurador
+        self.mensurador = Mensurador(modelo_args=model_args, 
+                                     transformer=self.transformer, 
+                                     pln=self.pln,
+                                     device=self._target_device)
 
         # Mensagem de carregamento da classe
         logger.info("Classe \"{}\" carregada com os parâmetros: \"{}\".".format(self.__class__.__name__, model_args))
     
     # ============================   
     def __repr__(self):
         '''
@@ -164,106 +166,118 @@
                     model_args.palavra_relevante = PalavraRelevante.NOUN.value                    
                 else:
                     logger.info("Não foi especificado uma estratégia de relevância de palavras do texto válida.") 
 
     # ============================
     def getMedidasTexto(self, texto: str, 
                         estrategia_pooling: EstrategiasPooling = EstrategiasPooling.MEAN, 
-                        palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL):
+                        palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL,
+                        converte_para_numpy: bool = True):
         ''' 
         Retorna as medidas de (in)coerência Ccos, Ceuc, Cman do texto.
         
         Parâmetros:
            `texto` - Um texto a ser medido.           
            `estrategia_pooling` - Estratégia de pooling das camadas do transformer.
-           `palavra_relevante` - Estratégia de relevância das palavras do texto.            
+           `palavra_relevante` - Estratégia de relevância das palavras do texto.
+           `converte_para_numpy` - Se verdadeiro, a saída em vetores numpy. Caso contrário, é uma lista de tensores pytorch.
         
         Retorno um dicionário com:
            `cos` - Medida de cos do do texto.
            `euc` - Medida de euc do do texto.
            `man` - Medida de man do do texto.
         ''' 
 
         self._defineEstrategiaPooling(estrategia_pooling)
         self._definePalavraRelevante(palavra_relevante)
         
         saida = self.mensurador.getMedidasComparacaoTexto(texto, 
-                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas)
+                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas,
+                                                          converte_para_numpy=converte_para_numpy)
           
         return saida
     
     # ============================
     def getMedidasTextoCosseno(self, texto: str, 
                                estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN, 
-                               palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL):
+                               palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL,
+                               converte_para_numpy: bool = True):
         ''' 
         Retorna a medida do texto utilizando a medida de similaridade de cosseno.
         
         Parâmetros:
            `texto` - Um texto a ser medido a coerência.           
            `estrategia_pooling` - Estratégia de pooling das camadas do transformer. 
            `palavra_relevante` - Estratégia de relevância das palavras do texto.            
+           `converte_para_numpy` - Se verdadeiro, a saída em vetores numpy. Caso contrário, é uma lista de tensores pytorch.
         
         Retorno:
            `cos` - Medida de cos do do texto.            
         '''         
 
         self._defineEstrategiaPooling(estrategia_pooling)
         self._definePalavraRelevante(palavra_relevante)
         
         saida = self.mensurador.getMedidasComparacaoTexto(texto, 
-                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas)
+                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas,
+                                                          converte_para_numpy=converte_para_numpy)
           
         return saida['cos']
     
     # ============================
     def getMedidasTextoEuclediana(self, texto: str, 
                                   estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN, 
-                                  palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL):
+                                  palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL,
+                                  converte_para_numpy: bool = True):
         ''' 
         Retorna a medida do texto utilizando a medida de distância de Euclidiana.
                  
         Parâmetros:
            `texto` - Um texto a ser mensurado.           
            `estrategia_pooling` - Estratégia de pooling das camadas do transformer.
            `palavra_relevante` - Estratégia de relevância das palavras do texto.            
+           `converte_para_numpy` - Se verdadeiro, a saída em vetores numpy. Caso contrário, é uma lista de tensores pytorch.
         
         Retorno:
            `ceu` - Medida euc do texto.            
         ''' 
         
         self._defineEstrategiaPooling(estrategia_pooling)
         self._definePalavraRelevante(palavra_relevante)
 
         saida = self.mensurador.getMedidasComparacaoTexto(texto,
-                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas)
+                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas,
+                                                          converte_para_numpy=converte_para_numpy)
           
         return saida['euc']      
        
     # ============================
     def getMedidasTextoManhattan(self, texto: str, 
                                  estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN, 
-                                 palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL):
+                                 palavra_relevante: Union[int, PalavraRelevante] = PalavraRelevante.ALL,
+                                 converte_para_numpy: bool = True):
         ''' 
         Retorna a medida do texto utilizando a medida de distância de Manhattan.
                  
         Parâmetros:
            `texto` - Um texto a ser mensurado.           
            `estrategia_pooling` - Estratégia de pooling das camadas do BERT.
            `palavra_relevante` - Estratégia de relevância das palavras do texto.            
+           `converte_para_numpy` - Se verdadeiro, a saída em vetores numpy. Caso contrário, é uma lista de tensores pytorch.
         
         Retorno:
            `man` - Medida  Cman do do texto.            
         ''' 
         
         self._defineEstrategiaPooling(estrategia_pooling)
         self._definePalavraRelevante(palavra_relevante)
         
         saida = self.mensurador.getMedidasComparacaoTexto(texto, 
-                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas)
+                                                          abordagem_extracao_embeddings_camadas=model_args.abordagem_extracao_embeddings_camadas,
+                                                          converte_para_numpy=converte_para_numpy)
           
         return saida['man']
     
     # ============================
     def tokenize(self, texto: Union[str, List[str]]):
         '''
         Tokeniza um texto para submeter ao modelo de linguagem. 
@@ -317,15 +331,16 @@
            `texto` - Texto a ser recuperado os embeddings.
            `abordagem_extracao_embeddings_camadas` - Camada de onde deve ser recupera os embeddings.
 
         Retorno:
            Os embeddings da camada para o texto.
         '''    
 
-        return self.getTransformer().getSaidaRedeCamada(texto, abordagem_extracao_embeddings_camadas=abordagem_extracao_embeddings_camadas)
+        return self.getTransformer().getSaidaRedeCamada(texto, 
+                                                        abordagem_extracao_embeddings_camadas=abordagem_extracao_embeddings_camadas)
 
     # ============================
     def getCodificacaoCompleta(self, texto: Union[str, List[str]],
                                tamanho_lote: int = 32, 
                                mostra_barra_progresso: bool = False,
                                converte_para_numpy: bool = False,
                                device: str = None):
@@ -402,17 +417,14 @@
             
             # Roda o texto através do modelo de linguagem, e coleta todos os estados ocultos produzidos.
             with torch.no_grad():
 
                 # Recupera a saída da rede
                 output_rede = self.getTransformer().getSaidaRede(lote_textos_tokenizados)
 
-                # Lista para os embeddings do texto
-                embeddings = []
-
                 # Percorre todas as saídas(textos) do lote                
                 for i, texto in enumerate(output_rede['texto_original']):      
                 
                     #ultimo_mask_id = len(attention_mask)-1
                     ultimo_mask_id = len(output_rede['attention_mask'][i])-1
                     
                     # Localiza o último token de "attention_mask" igual a 1                    
@@ -435,20 +447,33 @@
         saida['token_embeddings'] = [saida['token_embeddings'][idx] for idx in np.argsort(indice_tamanho_ordenado)]
         saida['input_ids'] = [saida['input_ids'][idx] for idx in np.argsort(indice_tamanho_ordenado)]
         saida['attention_mask'] = [saida['attention_mask'][idx] for idx in np.argsort(indice_tamanho_ordenado)]
         saida['token_type_ids'] = [saida['token_type_ids'][idx] for idx in np.argsort(indice_tamanho_ordenado)]
         saida['tokens_texto_mcl'] = [saida['tokens_texto_mcl'][idx] for idx in np.argsort(indice_tamanho_ordenado)]
         saida['texto_original'] = [saida['texto_original'][idx] for idx in np.argsort(indice_tamanho_ordenado)]
         saida['all_layer_embeddings'] = [saida['all_layer_embeddings'][idx] for idx in np.argsort(indice_tamanho_ordenado)]
-        
+                
+        # Se estiver usando GPU, copia os tensores para a memória do host.
+        if torch.cuda.is_available():
+            
+            # Copiando os tensores para a memória do host.
+            saida['token_embeddings'] = [emb.cpu() for emb in saida['token_embeddings']]
+            
+            # Copiando os tensores para a memória do host.
+            saida['all_layer_embeddings'] = [[[emb.cpu() for emb in camada] for camada in sentenca] for sentenca in saida['all_layer_embeddings']]
+            
         # Converte para numpy
         if converte_para_numpy:
+            
+            # Convertendo para numpy
             saida['token_embeddings'] = [np.array(emb.numpy(), dtype=object) for emb in saida['token_embeddings']]
+                        
+            # Convertendo para numpy
             saida['all_layer_embeddings'] = [[np.array([emb.numpy() for emb in camada], dtype=object) for camada in sentenca] for sentenca in saida['all_layer_embeddings']]
-            # Caso contrário deixa como lista de tensores.
+            # Caso contrário deixa como lista de tensores.            
 
         # Se é uma string remove a lista de lista
         if entrada_eh_string:
             saida['token_embeddings'] = saida['token_embeddings'][0]
             saida['input_ids'] = saida['input_ids'][0]
             saida['attention_mask'] = saida['attention_mask'][0]
             saida['token_type_ids'] = saida['token_type_ids'][0]
@@ -558,14 +583,16 @@
             
             # Converte o parâmetro estrategia_pooling para um objeto da classe EstrategiasPooling
             estrategia_pooling = EstrategiasPooling.converteInt(estrategia_pooling)
 
 
         # Retorna os embeddings de acordo com a estratégia
         if estrategia_pooling == EstrategiasPooling.MEAN:
+            
+            
             return self.getCodificacaoTexto(texto,
                                             tamanho_lote=tamanho_lote,
                                             mostra_barra_progresso=mostra_barra_progresso,
                                             converte_para_numpy=converte_para_numpy,
                                             device=device)['texto_embeddings_MEAN']
         else:
             if estrategia_pooling == EstrategiasPooling.MAX:
@@ -647,15 +674,15 @@
                 embedding_documento_maximo = np.max(embeddings_texto, axis=0)
                                 
             # Acumula a saída do método 
             saida['texto_original'].append(texto_embeddings['texto_original'][i])
             saida['tokens_texto_mcl'].append(tokens_texto_mcl)
             saida['texto_embeddings_MEAN'].append(embedding_documento_media)
             saida['texto_embeddings_MAX'].append(embedding_documento_maximo)
-
+            
         #Se é uma string uma lista com comprimento 1
         if entrada_eh_string:
             saida['texto_original'] = saida['texto_original'][0]
             saida['tokens_texto_mcl'] = saida['tokens_texto_mcl'][0]
             saida['texto_embeddings_MEAN'] = saida['texto_embeddings_MEAN'][0]
             saida['texto_embeddings_MAX'] = saida['texto_embeddings_MAX'][0]
```

### Comparing `texto_transformer-0.0.5/textotransformer/mensurador/medidas.py` & `texto_transformer-0.0.6/textotransformer/mensurador/medidas.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/mensurador/mensurador.py` & `texto_transformer-0.0.6/textotransformer/mensurador/mensurador.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,20 +23,22 @@
     ''' 
     Realiza mensurações em textos.
      
     Parâmetros:
        `modelo_args` - Parâmetros do modelo de linguagem.
        `transformer` - Modelo de linguagem carregado.
        `pln` - Processador de linguagem natural.
+       `device` - Dispositivo (como 'cuda' / 'cpu') que deve ser usado para computação. Se none, verifica se uma GPU pode ser usada.
     ''' 
 
     # Construtor da classe
     def __init__(self, modelo_args: ModeloArgumentos,
                  transformer: Transformer, 
-                 pln: PLN):
+                 pln: PLN,
+                 device: str = None):
     
         # Parâmetros do modelo
         self.model_args = modelo_args
     
         # Recupera o objeto do transformer.
         self.transformer = transformer
     
@@ -45,14 +47,17 @@
     
         # Recupera o tokenizador.     
         self.tokenizer = transformer.getTokenizer()
         
         # Recupera a classe PLN
         self.pln = pln
         
+        # Recupera o dispositivo
+        self._target_device = device
+                
         logger.info("Classe \"{}\" carregada: \"{}\".".format(self.__class__.__name__, modelo_args))
 
     # ============================   
     def __repr__(self):
         '''
         Retorna uma string com descrição do objeto.
         '''
@@ -391,52 +396,100 @@
                 return self.getEmbeddingSentencaEmbeddingTextoCLEAN(embedding_texto, texto, sentenca)
             else:
                 if self.model_args.palavra_relevante == PalavraRelevante.NOUN.value:
                     return self.getEmbeddingSentencaEmbeddingTextoNOUN(embedding_texto, texto, sentenca)
                 else:
                     logger.info("Nenhuma estratégia de relevância de palavras foi especificada.") 
     
-    
     # ============================
-    def getEmbeddingTextoCamada(self, texto, 
-                                abordagem_extracao_embeddings_camadas):
+    def getSaidaRedeMensurador(self, texto,
+                               abordagem_extracao_embeddings_camadas,
+                               device: str = None):
+        
         '''
         Retorna os embeddings do texto de acordo com a abordagem de extração especificada.
         
         Parâmetros:
            `texto` - Texto a ser recuperado os embeddings.
            `abordagem_extracao_embeddings_camadas` - Camada de onde deve ser recupera os embeddings.
+           `device` - Qual torch.device usar para a computação.
 
         Retorno:
            Uma lista com os embeddings do texto de acordo com a abordagem de extração especificada.
         '''
         
+        # Coloca o modelo em modo avaliação
+        self.model.eval()
+        
+        # Se o texto não estiver tokenizado, tokeniza
+        if not isinstance(texto, dict):
+            texto = self.getTransformer().tokenize(texto)
+            
+        # Se não foi especificado um dispositivo, use-o defaul
+        if device is None:
+            device = self._target_device
+     
+        # Adiciona um dispositivo ao modelo
+        self.model.to(device)            
+
+        # Adiciona ao device gpu ou cpu
+        lote_textos_tokenizados = self.getTransformer().batchToDevice(texto, device)            
+        
         # Roda o texto através do modelo de linguagem, e coleta todos os estados ocultos produzidos.
         with torch.no_grad():
+            
+            # Recupera a saída da rede
+            saida = self.getTransformer().getSaidaRedeCamada(lote_textos_tokenizados,
+                                                             abordagem_extracao_embeddings_camadas=abordagem_extracao_embeddings_camadas)
+        
+        return saida
+        
+    # ============================
+    def getEmbeddingTextoCamada(self, texto, 
+                                abordagem_extracao_embeddings_camadas,
+                                converte_para_numpy: bool = True):
+        '''
+        Retorna os embeddings do texto de acordo com a abordagem de extração especificada.
         
-            saida = self.getTransformer().getSaidaRedeCamada(texto,
-                                                            abordagem_extracao_embeddings_camadas=abordagem_extracao_embeddings_camadas)
+        Parâmetros:
+           `texto` - Texto a ser recuperado os embeddings.
+           `abordagem_extracao_embeddings_camadas` - Camada de onde deve ser recupera os embeddings.
+           `converte_para_numpy` - Se verdadeiro, a saída em vetores numpy. Caso contrário, é uma lista de tensores pytorch.
+
+        Retorno:
+           Uma lista com os embeddings do texto de acordo com a abordagem de extração especificada.
+        '''
+        
+        # Roda o texto através do modelo de linguagem, e coleta todos os estados ocultos produzidos.
+        saida = self.getSaidaRedeMensurador(texto,
+                                            abordagem_extracao_embeddings_camadas=abordagem_extracao_embeddings_camadas)
         
         # Remove o lote com [0]
         embedding_texto = saida['embedding_extraido'][0]
         
+        # Desconecta
+        if converte_para_numpy:
+            embedding_texto = embedding_texto.cpu()
+        
         return embedding_texto
 
     # ============================
     def getMedidasComparacaoTexto(self, texto, 
-                                  abordagem_extracao_embeddings_camadas):        
+                                  abordagem_extracao_embeddings_camadas,
+                                  converte_para_numpy: bool = True):
         '''
         Retorna as medidas do texto.
         Considera somente sentenças com pelo menos uma palavra.
         Estratégia de pooling padrão é MEAN(0).
         Palavra relavante padrão é ALL(0).
         
         Parâmetros:
            `texto` - Texto a ser realizado as comparações.
-         'abordagem_extracao_embeddings_camadas' - Camada de onde deve ser recupera os embeddings.
+           `abordagem_extracao_embeddings_camadas` - Camada de onde deve ser recupera os embeddings.
+           `converte_para_numpy` - Se verdadeiro, a saída em vetores numpy. Caso contrário, é uma lista de tensores pytorch.
                  
         Retorno um dicionário com:
            `cos` - Medida de cos do do texto.
            `euc` - Medida de euc do do texto.
            `man` - Medida de man do do texto.
         '''
 
@@ -452,74 +505,75 @@
 
         # Junta a lista de sentenças em um texto(string)
         string_texto = ' '.join(texto)
         #print('string_texto=', string_texto)
 
         # Recupera os embeddings dos tokens das camadas especificadas de acordo com a estratégia especificada para camada          
         embedding_texto = self.getEmbeddingTextoCamada(string_texto,
-                                                       abordagem_extracao_embeddings_camadas=abordagem_extracao_embeddings_camadas)
+                                                       abordagem_extracao_embeddings_camadas=abordagem_extracao_embeddings_camadas,
+                                                       converte_para_numpy=converte_para_numpy)
         #print('embedding_texto=', embedding_texto.shape)
 
         # Acumuladores das medidas entre as sentenças  
-        somaScos = 0
-        somaSeuc = 0
-        somaSman = 0
+        soma_Scos = 0
+        soma_Seuc = 0
+        soma_Sman = 0
 
         # Seleciona os pares de sentença a serem avaliados
-        posSi = 0
-        posSj = posSi + 1
+        pos_si = 0
+        pos_sj = pos_si + 1
 
         #Enquanto o indíce da sentneça posSj(2a sentença) não chegou ao final da quantidade de sentenças
-        while posSj <= (n-1):  
+        while pos_sj <= (n-1):  
 
             # Seleciona as sentenças do texto  
-            Si = texto[posSi]
-            Sj = texto[posSj]
+            Si = texto[pos_si]
+            Sj = texto[pos_sj]
 
             # Recupera os embedding das sentenças Si e Sj do embedding do texto      
             embedding_si = self.getEmbeddingSentencaEmbeddingTexto(embedding_texto, string_texto, Si)
             embedding_sj = self.getEmbeddingSentencaEmbeddingTexto(embedding_texto, string_texto, Sj)
 
             # Verifica se os embeddings sentenças estão preenchidos
             if embedding_si != None and embedding_sj != None:
 
                 # Recupera as medidas entre Si e Sj     
                 ajustado_embedding_si, ajustado_embedding_sj, Scos, Seuc, Sman = self.getMedidasSentencasEmbedding(embedding_si, embedding_sj)
 
                 # Acumula as medidas
-                somaScos = somaScos + Scos
-                somaSeuc = somaSeuc + Seuc
-                somaSman = somaSman + Sman
+                soma_Scos = soma_Scos + Scos
+                soma_Seuc = soma_Seuc + Seuc
+                soma_Sman = soma_Sman + Sman
 
                 # avança para o próximo par de sentenças
-                posSi = posSj
-                posSj = posSj + 1
+                pos_si = pos_sj
+                pos_sj = pos_sj + 1
             else:
                 # Reduz um da quantidade de sentenças pois uma delas está vazia
                 divisor = divisor - 1
                 # Se embedding_si igual a None avanca pos1 e pos2
                 if embedding_si == None:
                     # Avança a posição da sentença posSi para a posSj
-                    posSi = posSj
+                    pos_si = pos_sj
                     # Avança para a próxima sentença de posSj
-                    posSj = posSj + 1        
+                    pos_sj = pos_sj + 1        
                 else:          
                     # Se embeddingSj = None avança somente posJ para a próxima sentença
                     if embedding_sj == None:
-                        posSj = posSj + 1
+                        pos_sj = pos_sj + 1
 
         # Calcula a medida 
         Ccos = 0
         Ceuc = 0
         Cman = 0
 
         if divisor != 0:
-            Ccos = float(somaScos) / float(divisor)
-            Ceuc = float(somaSeuc) / float(divisor)
-            Cman = float(somaSman) / float(divisor)
+            Ccos = float(soma_Scos) / float(divisor)
+            Ceuc = float(soma_Seuc) / float(divisor)
+            Cman = float(soma_Sman) / float(divisor)
 
         # Retorna as medidas em um dicionário
         saida = {}
         saida.update({'cos' : Ccos,
                       'euc' : Ceuc,
                       'man' : Cman})
```

### Comparing `texto_transformer-0.0.5/textotransformer/mensurador/mensuradorenum.py` & `texto_transformer-0.0.6/textotransformer/mensurador/mensuradorenum.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/modelo/modeloarguments.py` & `texto_transformer-0.0.6/textotransformer/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/modelo/modeloenum.py` & `texto_transformer-0.0.6/textotransformer/modelo/modeloenum.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/modelo/transformer.py` & `texto_transformer-0.0.6/textotransformer/modelo/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,38 +242,38 @@
         for tokens in saida['tokens_texto_mcl']:
             if len(tokens) >= 512:
                 logger.info("Utilizando embeddings do modelo de:\"{}\".".format(AbordagemExtracaoEmbeddingsCamadas.converteInt(self.modelo_args.abordagem_extracao_embeddings_camadas).getStr()))
   
         return saida
         
     # ============================           
-    def getSaidaRede(self, texto: Union[str, dict]):
+    def getSaidaRede(self, texto: dict):
         '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings dos tokens do texto. 
+        De um texto preparado(tokenizado) retorna os embeddings dos tokens do texto. 
         O retorno é um dicionário com token_embeddings, input_ids, attention_mask, token_type_ids, 
         tokens_texto_mcl, texto_original  e all_layer_embeddings.
         
         Retorna os embeddings de todas as camadas de um texto.
     
         Parâmetros:
-           `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
+           `texto` - Um texto tokenizado a ser recuperado os embeddings do modelo de linguagem
     
         Retorna um dicionário com as seguintes chaves:
            `token_embeddings` - Uma lista com os embeddings da última camada.
            `input_ids` - Uma lista com os textos indexados.            
            `attention_mask` - Uma lista com os as máscaras de atenção
            `token_type_ids` - Uma lista com os tipos dos tokens.            
            `tokens_texto_mcl` - Uma lista com os textos tokenizados com os tokens especiais.
            `texto_origina`l - Uma lista com os textos originais.
            `all_layer_embeddings` - Uma lista com os embeddings de todas as camadas.
         '''
 
         # Se o texto não estiver tokenizado, tokeniza
-        if not isinstance(texto, dict):
-            texto = self.tokenize(texto)
+        #if not isinstance(texto, dict):
+        #   texto = self.tokenize(texto)
     
         # Recupera o texto preparado pelo tokenizador para envio ao modelo
         dic_texto_tokenizado = {'input_ids': texto['input_ids'],                                 
                                 'attention_mask': texto['attention_mask']}
         
         # Se token_type_ids estiver no texto preparado copia para dicionário
         if 'token_type_ids' in texto:
```

### Comparing `texto_transformer-0.0.5/textotransformer/pln/pln.py` & `texto_transformer-0.0.6/textotransformer/pln/pln.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/util/utilambiente.py` & `texto_transformer-0.0.6/textotransformer/util/utilambiente.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/util/utilarquivo.py` & `texto_transformer-0.0.6/textotransformer/util/utilarquivo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/util/utilconstantes.py` & `texto_transformer-0.0.6/textotransformer/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/util/utiltempo.py` & `texto_transformer-0.0.6/textotransformer/util/utiltempo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/textotransformer/util/utiltexto.py` & `texto_transformer-0.0.6/textotransformer/util/utiltexto.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/LICENSE` & `texto_transformer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.5/README.md` & `texto_transformer-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -96,15 +96,28 @@
 #Cada palavra de tamanho  : 768
 #Quantidade de tokens     : 15
 #Cada token de tamanho    : 768
 ````
 
 **Os exemplos podem ser executados através deste notebook no GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).**
 
-## Métodos principais
+## Classe principal
+
+A classe **TextoTransformer** carrega e cria um objeto para manipular um modelo de linguagem baseado e transformer. Permite recuperar e manipular embeddings recuperados de tokens, palavras, sentenças e textos.
+     
+### Parâmetros inicialização
+
+Aqui os parâmetros a serem especificados para instanciar a classe TextoTransformer.
+
+- `pretrained_model_name_or_path` - Se for um caminho de arquivo no disco, carrega o modelo a partir desse caminho. Se não for um caminho, ele primeiro faz o download do repositório de modelos do Huggingface com esse nome. Valor default: `neuralmind/bert-base-portuguese-cased`.
+- `modelo_spacy` - Nome do modelo spaCy a ser instalado e carregado pela ferramenta de pln spaCy. Valor default 'pt_core_news_lg'.
+- `abordagem_extracao_embeddings_camadas` - Especifica a abordagem padrão para a extração dos embeddings das camadas do transformer. Valor default '2'. Valores possíveis: 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últimas/5-Todas.
+- `device` - Dispositivo (como 'cuda' / 'cpu') que deve ser usado para o processamento. Se `None`, verifica se uma GPU pode ser usada. Se a GPU estiver disponível será usada no processamento. Valor default 'None'.
+    
+### Métodos principais
 
 Aqui os métodos principais para recuperar embeddings de textos, sentenças, palavras e tokens. Os métodos para recuperar os embeddings de textos, sentenças e palavras consolidados podem utilizar as estratégias de pooling média (MEAN) e máximo (MAX) dos embeddings de seus tokens.
 
 - `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling: int)`
     - Retorna uma lista dos embeddings consolidados dos textos.
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
@@ -135,12 +148,11 @@
 
 - transformers==4.26.1
 - spacy==3.5.2
 - tqdm==4.65.0
 - torch==2.0.1
 - scipy==1.10.1
 - numpy==1.22.4
-- scikit-learn=1.2.2
 
 ## Licença
 
 Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

### Comparing `texto_transformer-0.0.5/pyproject.toml` & `texto_transformer-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "texto-transformer"
-version = "0.0.5"
+version = "0.0.6"
 description = "Texto Transformer: Framework para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer"
 readme = "README.md"
 requires-python = ">=3.6.0"
 license = { file = "LICENSE" }
 
 authors = [
     { name = "Osmar de Oliveira Braz Junior", email = "osmar.braz@udesc.br" }
```

### Comparing `texto_transformer-0.0.5/PKG-INFO` & `texto_transformer-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texto-transformer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Texto Transformer: Framework para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer
 Project-URL: repository, https://github.com/osmarbraz/textotransformer/
 Author-email: Osmar de Oliveira Braz Junior <osmar.braz@udesc.br>
 License: MIT License
         
         Copyright (c) 2023 Osmar de Oliveira Braz Junior
         
@@ -139,15 +139,28 @@
 #Cada palavra de tamanho  : 768
 #Quantidade de tokens     : 15
 #Cada token de tamanho    : 768
 ````
 
 **Os exemplos podem ser executados através deste notebook no GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).**
 
-## Métodos principais
+## Classe principal
+
+A classe **TextoTransformer** carrega e cria um objeto para manipular um modelo de linguagem baseado e transformer. Permite recuperar e manipular embeddings recuperados de tokens, palavras, sentenças e textos.
+     
+### Parâmetros inicialização
+
+Aqui os parâmetros a serem especificados para instanciar a classe TextoTransformer.
+
+- `pretrained_model_name_or_path` - Se for um caminho de arquivo no disco, carrega o modelo a partir desse caminho. Se não for um caminho, ele primeiro faz o download do repositório de modelos do Huggingface com esse nome. Valor default: `neuralmind/bert-base-portuguese-cased`.
+- `modelo_spacy` - Nome do modelo spaCy a ser instalado e carregado pela ferramenta de pln spaCy. Valor default 'pt_core_news_lg'.
+- `abordagem_extracao_embeddings_camadas` - Especifica a abordagem padrão para a extração dos embeddings das camadas do transformer. Valor default '2'. Valores possíveis: 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últimas/5-Todas.
+- `device` - Dispositivo (como 'cuda' / 'cpu') que deve ser usado para o processamento. Se `None`, verifica se uma GPU pode ser usada. Se a GPU estiver disponível será usada no processamento. Valor default 'None'.
+    
+### Métodos principais
 
 Aqui os métodos principais para recuperar embeddings de textos, sentenças, palavras e tokens. Os métodos para recuperar os embeddings de textos, sentenças e palavras consolidados podem utilizar as estratégias de pooling média (MEAN) e máximo (MAX) dos embeddings de seus tokens.
 
 - `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling: int)`
     - Retorna uma lista dos embeddings consolidados dos textos.
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
@@ -178,12 +191,11 @@
 
 - transformers==4.26.1
 - spacy==3.5.2
 - tqdm==4.65.0
 - torch==2.0.1
 - scipy==1.10.1
 - numpy==1.22.4
-- scikit-learn=1.2.2
 
 ## Licença
 
 Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

