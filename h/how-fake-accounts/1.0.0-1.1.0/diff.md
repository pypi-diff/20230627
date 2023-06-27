# Comparing `tmp/how_fake_accounts-1.0.0.tar.gz` & `tmp/how_fake_accounts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "how_fake_accounts-1.0.0.tar", last modified: Tue Jun 27 14:04:14 2023, max compression
+gzip compressed data, was "how_fake_accounts-1.1.0.tar", last modified: Tue Jun 27 15:04:39 2023, max compression
```

## Comparing `how_fake_accounts-1.0.0.tar` & `how_fake_accounts-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 14:04:14.334226 how_fake_accounts-1.0.0/
--rw-r--r--   0 joaonogueira   (501) staff       (20)      891 2023-06-27 14:04:14.334062 how_fake_accounts-1.0.0/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      743 2023-06-27 14:00:41.000000 how_fake_accounts-1.0.0/README.md
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 14:04:14.332607 how_fake_accounts-1.0.0/how_fake_accounts/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       23 2023-06-27 14:03:58.000000 how_fake_accounts-1.0.0/how_fake_accounts/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      862 2023-06-27 14:01:49.000000 how_fake_accounts-1.0.0/how_fake_accounts/__main__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     1268 2023-06-27 14:03:20.000000 how_fake_accounts-1.0.0/how_fake_accounts/core.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 14:04:14.333855 how_fake_accounts-1.0.0/how_fake_accounts.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)      891 2023-06-27 14:04:14.000000 how_fake_accounts-1.0.0/how_fake_accounts.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      352 2023-06-27 14:04:14.000000 how_fake_accounts-1.0.0/how_fake_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-06-27 14:04:14.000000 how_fake_accounts-1.0.0/how_fake_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       61 2023-06-27 14:04:14.000000 how_fake_accounts-1.0.0/how_fake_accounts.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-06-27 14:04:14.000000 how_fake_accounts-1.0.0/how_fake_accounts.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       18 2023-06-27 14:04:14.000000 how_fake_accounts-1.0.0/how_fake_accounts.egg-info/top_level.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-06-27 14:04:14.334276 how_fake_accounts-1.0.0/setup.cfg
--rw-r--r--   0 joaonogueira   (501) staff       (20)      441 2023-06-27 14:03:43.000000 how_fake_accounts-1.0.0/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 15:04:39.400591 how_fake_accounts-1.1.0/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1306 2023-06-27 15:04:39.400398 how_fake_accounts-1.1.0/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1158 2023-06-27 14:17:43.000000 how_fake_accounts-1.1.0/README.md
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 15:04:39.398563 how_fake_accounts-1.1.0/how_fake_accounts/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       45 2023-06-27 15:03:01.000000 how_fake_accounts-1.1.0/how_fake_accounts/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      862 2023-06-27 14:01:49.000000 how_fake_accounts-1.1.0/how_fake_accounts/__main__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1368 2023-06-27 15:01:34.000000 how_fake_accounts-1.1.0/how_fake_accounts/core.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 15:04:39.400083 how_fake_accounts-1.1.0/how_fake_accounts.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1306 2023-06-27 15:04:39.000000 how_fake_accounts-1.1.0/how_fake_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      352 2023-06-27 15:04:39.000000 how_fake_accounts-1.1.0/how_fake_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-06-27 15:04:39.000000 how_fake_accounts-1.1.0/how_fake_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       61 2023-06-27 15:04:39.000000 how_fake_accounts-1.1.0/how_fake_accounts.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-06-27 15:04:39.000000 how_fake_accounts-1.1.0/how_fake_accounts.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       18 2023-06-27 15:04:39.000000 how_fake_accounts-1.1.0/how_fake_accounts.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-06-27 15:04:39.400646 how_fake_accounts-1.1.0/setup.cfg
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      441 2023-06-27 15:03:08.000000 how_fake_accounts-1.1.0/setup.py
```

### Comparing `how_fake_accounts-1.0.0/PKG-INFO` & `how_fake_accounts-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: how_fake_accounts
-Version: 1.0.0
+Version: 1.1.0
 Author: João Nogueira
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # How Fake Accounts
 
-Pacote python criado para gerar contas fakes, para o primeiro desafio do bootcamp de engenharia de dados da How.
+Pacote python criado para gerar contas fakes, para o primeiro desafio do bootcamp de engenharia de dados da How. O pacote é a implementação de um provider customizado do [Faker](https://faker.readthedocs.io/en/master/#), conforme sugerido em https://faker.readthedocs.io/en/master/#how-to-create-a-provider.
+
+As contas feitas simulam o cadastro de usuários em um aplicativo e contém as seguintes informações para cada usuário cadastrado:
+
+- nome
+- email
+- número de telefone
+- cpf
+- data de nascimento
+- endereço
+- emprego
 
 ## How to install
 
 ```bash
 pip install how-fake-accounts
 ```
 
@@ -20,15 +30,15 @@
 We have mainly two ways to use the package:
 - as a package itself, to be imported in python scripts
 - as a command line interface
 
 ### Package Interface
 
 ```python
-from how_fake_accounts.core import fake
+from how_fake_accounts import fake
 
 # generate 10 random accounts
 accounts = fake.generate_accounts(10)
 print(accounts)
 fake.save_locally(accounts)
 ```
```

### Comparing `how_fake_accounts-1.0.0/how_fake_accounts/__main__.py` & `how_fake_accounts-1.1.0/how_fake_accounts/__main__.py`

 * *Files identical despite different names*

### Comparing `how_fake_accounts-1.0.0/how_fake_accounts/core.py` & `how_fake_accounts-1.1.0/how_fake_accounts/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 fake = Faker('pt_BR')
 
 class GenerateAccountsProvider(BaseProvider):
     def generate_accounts(self, n_accounts=10):
         accounts = []
         for i in range(n_accounts):
             accounts.append({
+                'registration_date': str(fake.date_time_between(start_date='-1y', end_date='now')),
                 'name': fake.name(),
                 'email': fake.email(),
                 'phone': fake.cellphone_number(),
                 'cpf': fake.cpf(),
                 'birth_date': fake.date_of_birth(),
                 'address': fake.address(),
                 'job': fake.job()
```

### Comparing `how_fake_accounts-1.0.0/how_fake_accounts.egg-info/PKG-INFO` & `how_fake_accounts-1.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 2.1
-Name: how-fake-accounts
-Version: 1.0.0
-Author: João Nogueira
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # How Fake Accounts
 
-Pacote python criado para gerar contas fakes, para o primeiro desafio do bootcamp de engenharia de dados da How.
+Pacote python criado para gerar contas fakes, para o primeiro desafio do bootcamp de engenharia de dados da How. O pacote é a implementação de um provider customizado do [Faker](https://faker.readthedocs.io/en/master/#), conforme sugerido em https://faker.readthedocs.io/en/master/#how-to-create-a-provider.
+
+As contas feitas simulam o cadastro de usuários em um aplicativo e contém as seguintes informações para cada usuário cadastrado:
+
+- nome
+- email
+- número de telefone
+- cpf
+- data de nascimento
+- endereço
+- emprego
 
 ## How to install
 
 ```bash
 pip install how-fake-accounts
 ```
 
@@ -20,15 +23,15 @@
 We have mainly two ways to use the package:
 - as a package itself, to be imported in python scripts
 - as a command line interface
 
 ### Package Interface
 
 ```python
-from how_fake_accounts.core import fake
+from how_fake_accounts import fake
 
 # generate 10 random accounts
 accounts = fake.generate_accounts(10)
 print(accounts)
 fake.save_locally(accounts)
 ```
```

