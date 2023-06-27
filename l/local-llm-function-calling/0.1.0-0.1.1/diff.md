# Comparing `tmp/local_llm_function_calling-0.1.0.tar.gz` & `tmp/local_llm_function_calling-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_llm_function_calling-0.1.0.tar", max compression
+gzip compressed data, was "local_llm_function_calling-0.1.1.tar", max compression
```

## Comparing `local_llm_function_calling-0.1.0.tar` & `local_llm_function_calling-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2419 2023-06-27 11:02:02.687775 local_llm_function_calling-0.1.0/README.md
--rw-r--r--   0        0        0      306 2023-06-27 10:56:05.853586 local_llm_function_calling-0.1.0/local_llm_function_calling/__init__.py
--rw-r--r--   0        0        0     5999 2023-06-27 10:59:41.930783 local_llm_function_calling-0.1.0/local_llm_function_calling/generator.py
--rw-r--r--   0        0        0     3950 2023-06-27 09:38:19.333497 local_llm_function_calling-0.1.0/local_llm_function_calling/prompter.py
--rw-r--r--   0        0        0      416 2023-06-27 11:04:28.005924 local_llm_function_calling-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2842 1970-01-01 00:00:00.000000 local_llm_function_calling-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2455 2023-06-27 12:00:57.538028 local_llm_function_calling-0.1.1/README.md
+-rw-r--r--   0        0        0      306 2023-06-27 10:56:05.853586 local_llm_function_calling-0.1.1/local_llm_function_calling/__init__.py
+-rw-r--r--   0        0        0     7090 2023-06-27 12:19:02.425382 local_llm_function_calling-0.1.1/local_llm_function_calling/generator.py
+-rw-r--r--   0        0        0     3950 2023-06-27 09:38:19.333497 local_llm_function_calling-0.1.1/local_llm_function_calling/prompter.py
+-rw-r--r--   0        0        0      416 2023-06-27 12:21:36.314534 local_llm_function_calling-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 local_llm_function_calling-0.1.1/PKG-INFO
```

### Comparing `local_llm_function_calling-0.1.0/README.md` & `local_llm_function_calling-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
         "description": "Get the current weather in a given location",
         "parameters": {
             "type": "object",
             "properties": {
                 "location": {
                     "type": "string",
                     "description": "The city and state, e.g. San Francisco, CA",
+                    "maxLength": 20,
                 },
                 "unit": {"type": "string", "enum": ["celsius", "fahrenheit"]},
             },
             "required": ["location"],
         },
     }
 ]
 
 # Initialize the generator with the Hugging Face model, tokenizer, and functions
 generator = Generator(functions, "gpt2")
 
 # Generate text using a prompt
 function_call = generator.generate("What is the weather like today in Brooklyn?")
 print(function_call)
-
 ```
 
 ## Extending and Customizing
 
 To extend or customize the prompt structure, you can subclass the `TextPrompter` class. This allows you to modify the prompt generation process according to your specific requirements.
```

### Comparing `local_llm_function_calling-0.1.0/local_llm_function_calling/generator.py` & `local_llm_function_calling-0.1.1/local_llm_function_calling/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 import json_schema_enforcer
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from .prompter import CompletionModelPrompter, FunctionCall, FunctionType, TextPrompter
 
 
+class SequenceTooLong(Exception):
+    """The sequence is too long to generate"""
+
+
 class Generator:
     """Generate the function call based on the schema"""
 
     def __init__(
         self,
         functions: list[FunctionType],
         model: AutoModelForCausalLM | str,
@@ -44,15 +48,17 @@
         Args:
             prompt (str): The prompt to use
 
         Yields:
             str: The tokens sorted by their likelihood
         """
         inputs = self.tokenizer(prompt, return_tensors="pt")
-        gen_tokens = model.generate(
+        if inputs["input_ids"].shape[1] >= self.model.config.n_positions:
+            raise SequenceTooLong()
+        gen_tokens = self.model.generate(
             **inputs,
             output_scores=True,
             return_dict_in_generate=True,
             max_new_tokens=1,
             pad_token_id=self.tokenizer.eos_token_id
         )
         tokens_rated = gen_tokens.scores[0].argsort(descending=True)[0]
@@ -117,23 +123,32 @@
         Returns:
             str: The function to call
         """
         if function_call is None:
             return self._choose_function(prompt)
         return function_call
 
-    def generate_arguments(self, prompt: str, function_call: str) -> str:
+    def generate_arguments(
+        self,
+        prompt: str,
+        function_call: str,
+        max_new_tokens: int | None = None,
+        max_length: int | None = None,
+    ) -> str:
         """Generate the arguments for the function
 
         Args:
             prompt (str): The prompt to use
             function_call (str): The function to call
+            max_new_tokens (int | None): The maximum number of tokens to generate
+            max_length (int | None): The maximum length of the generated sequence
 
         Returns:
-            str: The arguments for the function
+            str: The arguments for the function, as a JSON string
+                (may not be complete)
         """
         config = json_schema_enforcer.StyleConfig(True, 4, True, 0, 0)
         parser = json_schema_enforcer.parser_for_schema(
             [
                 function
                 for function in self.functions
                 if function["name"] == function_call
@@ -141,27 +156,44 @@
                 "parameters"
             ]  # type: ignore
         )
         if parser is None:
             raise ValueError("No parser found for arguments")
         prefix = self.prompter.prompt(prompt, self.functions, function_call)
         generated = ""
+        generated_tokens = 0
         while True:
-            for token in self.get_sorted_tokens(prefix + generated):
-                validated = parser.validate(generated + token, style_config=config)
-                if validated.valid:
-                    if validated.end_index is not None:
-                        return (generated + token)[: validated.end_index]
-                    generated += token
-                    break
+            try:
+                for token in self.get_sorted_tokens(prefix + generated):
+                    validated = parser.validate(generated + token, style_config=config)
+                    if validated.valid:
+                        if validated.end_index is not None:
+                            return (generated + token)[: validated.end_index]
+                        generated += token
+                        break
+            except SequenceTooLong:
+                return generated
+            generated_tokens += 1
+            if max_new_tokens is not None and generated_tokens >= max_new_tokens:
+                return generated
+            if max_length is not None and len(generated) >= max_length:
+                return generated
 
-    def generate(self, prompt: str, function_call: str | None = None) -> FunctionCall:
+    def generate(
+        self,
+        prompt: str,
+        function_call: str | None = None,
+        max_length: int | None = None,
+        max_new_tokens: int | None = None,
+    ) -> FunctionCall:
         """Generate the function call
 
         Args:
             prompt (str): The prompt to use
             function_call (str | None): The function call to use.
                 Will be generated if not provided.
         """
         function_name = self.choose_function(prompt, function_call)
-        arguments = self.generate_arguments(prompt, function_name)
+        arguments = self.generate_arguments(
+            prompt, function_name, max_new_tokens, max_length
+        )
         return {"name": function_name, "parameters": arguments}
```

### Comparing `local_llm_function_calling-0.1.0/local_llm_function_calling/prompter.py` & `local_llm_function_calling-0.1.1/local_llm_function_calling/prompter.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.0/PKG-INFO` & `local_llm_function_calling-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-llm-function-calling
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: json-schema-enforcer (>=0.1.0,<0.2.0)
@@ -47,28 +47,28 @@
         "description": "Get the current weather in a given location",
         "parameters": {
             "type": "object",
             "properties": {
                 "location": {
                     "type": "string",
                     "description": "The city and state, e.g. San Francisco, CA",
+                    "maxLength": 20,
                 },
                 "unit": {"type": "string", "enum": ["celsius", "fahrenheit"]},
             },
             "required": ["location"],
         },
     }
 ]
 
 # Initialize the generator with the Hugging Face model, tokenizer, and functions
 generator = Generator(functions, "gpt2")
 
 # Generate text using a prompt
 function_call = generator.generate("What is the weather like today in Brooklyn?")
 print(function_call)
-
 ```
 
 ## Extending and Customizing
 
 To extend or customize the prompt structure, you can subclass the `TextPrompter` class. This allows you to modify the prompt generation process according to your specific requirements.
```

