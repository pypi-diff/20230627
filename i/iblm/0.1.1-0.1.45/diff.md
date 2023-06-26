# Comparing `tmp/iblm-0.1.1.tar.gz` & `tmp/iblm-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iblm-0.1.1.tar", max compression
+gzip compressed data, was "iblm-0.1.45.tar", max compression
```

## Comparing `iblm-0.1.1.tar` & `iblm-0.1.45.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-06-07 12:40:58.888840 iblm-0.1.1/LICENSE
--rw-r--r--   0        0        0      643 2023-06-07 14:56:45.740106 iblm-0.1.1/README.md
--rw-r--r--   0        0        0      404 2023-06-22 14:31:09.323608 iblm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      203 2023-06-22 14:01:16.003155 iblm-0.1.1/src/iblm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 15:10:29.105686 iblm-0.1.1/src/iblm/ibbagging/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 15:10:11.765225 iblm-0.1.1/src/iblm/ibboosting/__init__.py
--rw-r--r--   0        0        0     4843 2023-06-07 17:06:15.194104 iblm-0.1.1/src/iblm/ibboosting/ibboosting_classifier.py
--rw-r--r--   0        0        0        0 2023-06-07 19:26:52.021636 iblm-0.1.1/src/iblm/iblmodel/__init__.py
--rw-r--r--   0        0        0     4848 2023-06-09 18:01:15.259584 iblm-0.1.1/src/iblm/iblmodel/iblm_classifier.py
--rw-r--r--   0        0        0     4835 2023-06-07 15:17:27.793056 iblm-0.1.1/src/iblm/iblmodel/iblm_regressor.py
--rw-r--r--   0        0        0        0 2023-06-14 18:02:51.818510 iblm-0.1.1/src/iblm/iclmodel/__init__.py
--rw-r--r--   0        0        0     4698 2023-06-14 18:09:08.467661 iblm-0.1.1/src/iblm/iclmodel/icl_classifier.py
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 iblm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-07 12:40:58.888840 iblm-0.1.45/LICENSE
+-rw-r--r--   0        0        0     1813 2023-06-26 14:42:26.100130 iblm-0.1.45/README.md
+-rw-r--r--   0        0        0      519 2023-06-26 20:16:13.486261 iblm-0.1.45/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-06-25 22:32:03.071956 iblm-0.1.45/src/iblm/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:10:29.105686 iblm-0.1.45/src/iblm/ibbagging/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:10:11.765225 iblm-0.1.45/src/iblm/ibboosting/__init__.py
+-rw-r--r--   0        0        0     4843 2023-06-07 17:06:15.194104 iblm-0.1.45/src/iblm/ibboosting/ibboosting_classifier.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:26:52.021636 iblm-0.1.45/src/iblm/iblmodel/__init__.py
+-rw-r--r--   0        0        0     4420 2023-06-26 18:36:25.225642 iblm-0.1.45/src/iblm/iblmodel/iblm_classifier.py
+-rw-r--r--   0        0        0     4667 2023-06-26 14:34:12.336205 iblm-0.1.45/src/iblm/iblmodel/iblm_regressor.py
+-rw-r--r--   0        0        0     1668 2023-06-26 19:18:53.706468 iblm-0.1.45/src/iblm/iblmodel/prompt/20230627.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:02:51.818510 iblm-0.1.45/src/iblm/iclmodel/__init__.py
+-rw-r--r--   0        0        0     1984 2023-06-26 21:24:21.558654 iblm-0.1.45/src/iblm/iclmodel/icl_classifier.py
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 iblm-0.1.45/PKG-INFO
```

### Comparing `iblm-0.1.1/LICENSE` & `iblm-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `iblm-0.1.1/src/iblm/ibboosting/ibboosting_classifier.py` & `iblm-0.1.45/src/iblm/ibboosting/ibboosting_classifier.py`

 * *Files identical despite different names*

### Comparing `iblm-0.1.1/src/iblm/iblmodel/iblm_classifier.py` & `iblm-0.1.45/src/iblm/iblmodel/iblm_regressor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-from langchain.llms import OpenAI
 from langchain.callbacks import get_openai_callback
 import re
 
 import numpy as np
 
 import warnings
 warnings.filterwarnings('ignore')
 
 
-class IBLMClassifier():
+class IBLMRegressor():
     def __init__(
         self, 
-        llm_model_name, 
+        llm_model, 
         params
         ):
-        self.llm_model_name = llm_model_name
-        self.llm_model = OpenAI(temperature=0, model_name = self.llm_model_name)
-
-        #self.llm_model = llm_model,
+        self.llm_model = llm_model
         self.columns_name = params['columns_name']
         self.model_code = None
 
 
     def fit(self, x, y, model_name, file_path=None):
         print("> Start of model creating.")
         df = x.copy()
@@ -30,15 +26,14 @@
 
         # Determine whether binary or multivalued classification is used
         if len(df['target'].unique()) == 2:
             task_type = 'binary classification'
             output_code = 'y = 1 / (1 + np.exp(-y))'
         else:
             task_type = 'multi-class classification'
-            output_code = ''
 
         # Obtaining data types
         data_type = ', '.join(df.dtypes.astype(str))
 
 
 
         # Create a string dataset
@@ -60,49 +55,50 @@
             col_name = ', '.join(df.columns.astype(str))
             col_option = 'df.columns = range(df.shape[1])'
 
 
 
         create_prompt = """
         Please create your code in compliance with all of the following conditions. Output should be code only. Do not enclose the output in ``python ``` or the like.
-        ・Analyze the following large amount of data and create a code to accurately predict the probability that the "target" is 1.
+        ・Analyze the large amount of data below and create a {task_type_} code to accurately predict "target".
         ------------------
         {dataset_str_}
         ------------------
         ・Each data type is as follows. If necessary, you can change the data type.
-        ------------------
-        {data_type_}
-        ------------------
-        ・The column names, in order, are as follows {col_name_}
-        ・Think and code the logic to predict probability values based on the data without using a machine learning model.
-        ・Please make your predictions as accurate as possible.
-        ・Predicting probability values as finely as possible increases overall accuracy.
+        ・Create code that can make predictions about new data based on logic from large amounts of input data without using machine learning models.
+        ・If input is available, the column names below should also be used to help make decisions when creating the predictive model. Column Name:{col_name_}
+        ・Create a code like the following. Do not change the input or output format.
         ・If {col_option_} is not blank, add it after 'df = x.copy()'.
         ・You do not need to provide examples.
-        ・Create a code like the following.
         ------------------
         import numpy as np
+
         def predict(x):
             df = x.copy()
+
             output = []
             for index, row in df.iterrows():
-                # Do not change the code before this point.
-                # Please describe the process required to make the prediction below.
 
 
-                # Do not change the code after this point.
+                # Feature creation and data preprocessing
+
+
+                {output_code_}
                 output.append(y)
-            return np.array(output)
+
+            output = np.array(output)
+                
+            return output
         """.format(
-            #task_type_ = task_type,
+            task_type_ = task_type,
             dataset_str_ = dataset_str,
-            data_type_ = data_type,
+            model_name_ = model_name,
             col_name_ = col_name,
             col_option_ = col_option,
-            #output_code_ = output_code
+            output_code_ = output_code
             )
 
         #print(create_prompt)
 
         with get_openai_callback() as cb:
             model_code = self.llm_model(create_prompt)
             print(cb)
@@ -120,17 +116,22 @@
 
     def predict(self, x):
         if self.model_code is None:
             raise Exception("You must train the model before predicting!")
 
         code = self.model_code
 
+        # = re.search(r'def (\w+)', function_string).group(1)
+        #code = self.model_code + '\n'# + f'model = model({x})'
         exec(code, globals())
 
+        #model = namespace["code"]
+        
         y = predict(x)
+
         return y
 
 
 
 
     def interpret(self):
         if self.model_code is None:
```

