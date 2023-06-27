# Comparing `tmp/bambooai-0.3.6.tar.gz` & `tmp/bambooai-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.3.6.tar", last modified: Fri Jun 23 00:51:09 2023, max compression
+gzip compressed data, was "bambooai-0.3.7.tar", last modified: Tue Jun 27 07:28:37 2023, max compression
```

## Comparing `bambooai-0.3.6.tar` & `bambooai-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 00:51:09.482377 bambooai-0.3.6/
--rw-rw-rw-   0        0        0     7966 2023-06-23 00:51:09.481581 bambooai-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     7430 2023-06-18 06:44:01.000000 bambooai-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 00:51:09.447726 bambooai-0.3.6/bambooai/
--rw-rw-rw-   0        0        0       79 2023-06-18 06:42:14.000000 bambooai-0.3.6/bambooai/__init__.py
--rw-rw-rw-   0        0        0    26472 2023-06-23 00:45:25.000000 bambooai-0.3.6/bambooai/bambooai.py
--rw-rw-rw-   0        0        0     1309 2023-06-22 23:44:14.000000 bambooai-0.3.6/bambooai/func_calls.py
--rw-rw-rw-   0        0        0     5939 2023-06-22 23:42:27.000000 bambooai-0.3.6/bambooai/prompts.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:51:09.479730 bambooai-0.3.6/bambooai.egg-info/
--rw-rw-rw-   0        0        0     7966 2023-06-23 00:51:09.000000 bambooai-0.3.6/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-23 00:51:09.000000 bambooai-0.3.6/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 00:51:09.000000 bambooai-0.3.6/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-23 00:51:09.000000 bambooai-0.3.6/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 00:51:09.000000 bambooai-0.3.6/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 00:51:09.482471 bambooai-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-06-23 00:44:00.000000 bambooai-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:28:37.163458 bambooai-0.3.7/
+-rw-rw-rw-   0        0        0     7870 2023-06-27 07:28:37.162956 bambooai-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7317 2023-06-27 07:25:47.000000 bambooai-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:28:37.126161 bambooai-0.3.7/bambooai/
+-rw-rw-rw-   0        0        0      107 2023-06-27 07:23:09.000000 bambooai-0.3.7/bambooai/__init__.py
+-rw-rw-rw-   0        0        0    31816 2023-06-27 07:22:25.000000 bambooai-0.3.7/bambooai/bambooai.py
+-rw-rw-rw-   0        0        0     1309 2023-06-22 23:44:14.000000 bambooai-0.3.7/bambooai/func_calls.py
+-rw-rw-rw-   0        0        0     5817 2023-06-24 13:34:56.000000 bambooai-0.3.7/bambooai/prompts.py
+-rw-rw-rw-   0        0        0     4189 2023-06-27 02:19:42.000000 bambooai-0.3.7/bambooai/qa_retrieval.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:28:37.161111 bambooai-0.3.7/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     7870 2023-06-27 07:28:37.000000 bambooai-0.3.7/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-27 07:28:37.000000 bambooai-0.3.7/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:28:37.000000 bambooai-0.3.7/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-27 07:28:37.000000 bambooai-0.3.7/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 07:28:37.000000 bambooai-0.3.7/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:28:37.164046 bambooai-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-27 07:23:56.000000 bambooai-0.3.7/setup.py
```

### Comparing `bambooai-0.3.6/PKG-INFO` & `bambooai-0.3.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.6
+Version: 0.3.7
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -14,43 +14,58 @@
 # BambooAI
 A lightweight library that leverages Language Models (LLMs) to enable natural language interactions, allowing you to converse with your pandas DataFrames.
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
-My primary goal was to build a library that acts as a steadfast companion for analysts of all skill levels, rather than acting as the analyst itself. This library simplifies the intricate process of data analysis and visualization, serving to streamline the user's workflow. It's been crafted with a focus on user-friendliness, efficiency, and adaptability, enabling it to cater to a wide range of users and their unique analytical needs. By functioning as an aid rather than the main analyst, this library not only facilitates smoother operations but also empowers users to effectively employ their analytical skills, enhancing their overall productivity.
+My main goal was to create a tool to help analysts at all levels, not to replace them. This library makes data analysis and visualization easier, helping to improve workflows. It's designed to be easy to use, efficient, and adaptable to different users' needs. As a supportive tool, not the main operator, it helps users apply their own analytical skills more effectively and increase their productivity.
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
 https://github.com/pgalko/BambooAI/assets/39939157/2d8e4a9f-29c4-438b-8c13-126a05065ef8
 
 ## How it works
 
-- The user begins by starting the BambooAI agent.
-- BambooAI subsequently checks if a question has been provided:
-  - If a question is available, it continues to the next step.
-  - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
-- Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents a summary in the form of numbered task list.
-- The agent then replaces the original question with the task list from the previous step and sends this as a prompt to the OpenAI API for code generation.
-- The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
-  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
-- The received code is then executed to generate an answer or a visualization:
-  - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
-  - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
-- The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
-- Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
- 
-**Flow chart:**
+The BambooAI agent operates through several key steps to interact with users and generate responses:
+
+**1. Initiation**
+- The user starts the BambooAI agent.
+- If there's no input question, the agent prompts the user to either input a question or type 'exit' to terminate the program.
+
+**2. Task Evaluation**
+- The agent stores the received question and utilizes the Language Learning Model (LLM) to evaluate and categorize it.
+- The LLM determines whether the question necessitates a narrative response, additional information, or can be resolved using code.
+
+**3. Dynamic Prompt Build**
+- If code can resolve the question, the agent formulates an algorithm expressed as a task list.
+- The original question is modified to align with this algorithm. The agent conducts a semantic search for similar questions.
+- Any matching questions found are appended to the prompt as examples, and GPT-3 is used to generate code based on the algorithm.
+
+**4. Debugging, Execution, and Error Correction**
+- If the generated code needs debugging, GPT-4 is engaged.
+- The code is executed, and if errors occur, the agent logs the error message and refers it to the LLM (GPT-3 or GPT-4, depending on the settings) for correction.
+- This process continues until successful code execution.
+
+**5. Results, Ranking, and Knowledge Base Build**
+- Post successful execution, GPT-4 is used to rank the answer.
+- If the rank surpasses a set threshold, the question, answer, code, and rank are stored in the Pinecone vector database.
+- Regardless of the rank, the final answer or visualization is formatted and presented to the user.
+
+**6. Human Feedback and Loop Continuation**
+- The agent seeks feedback from the user.
+- If the user validates the auto-generated ranking, the question/answer pair is stored in the vector database.
+- If not, a new execution loop begins.
+
+Throughout this process, the agent continuously solicits user input, stores messages for context, and generates and executes code to ensure optimal results. Various AI models and a vector database are employed in this process to provide accurate and helpful responses to user's questions.
 
-![](images/flow_chart_3.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -61,26 +76,26 @@
 Parameters
 
 ```
 df: pd.DataFrame - Dataframe(Required)
 
 max_conversations: int - Number of "user:assistant" conversation pairs to keep in memory for a context. Default=2
 
-llm: str - Base LLM model. Default = gpt-3.5-turbo
+llm: str - Base LLM model. Default = gpt-3.5-turbo-0613
 
 llm_switch: bool - If True, the agent will switch to gpt-4 after error
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
-rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+vector_db: bool - If True, each answer will first be ranked from 1 to 10. If the rank surpasses a certain threshold (8), the corresponding question (vectorised), answer, code, and rank (metadata) are all stored in the Pinecone database. Each time a new question is asked, these records will be searched. If the similarity score is above 0.9, they will be offered as examples and included in the prompt (in a one-shot learning scenario)
 
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
 
-e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True)
+e.g. bamboo = BambooAI(df, debug=True, vector_db=True, llm_switch=True, exploratory=True)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -100,16 +115,19 @@
 bamboo = BambooAI(df)
 bamboo.pd_agent_converse("Calculate 30, 50, 75 and 90 percentiles of the heart rate column")
 ```
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
-The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
-The key can be obtained from here: https://platform.openai.com/account/api-keys
+The library requires an OpenAI API account and the API key to connect to OpenAI LLMs. The OpenAI API key needs to be stored in a ```OPENAI_API_KEY``` environment variable.
+The key can be obtained from here: https://platform.openai.com/account/api-keys.
+
+The Pincone vector db is optional. If you don want to use it, you dont need to do anything. If you have an account with Pinecone and would like to use the knowledge base and ranking features, you will be required to setup ```PINECONE_API_KEY``` and ```PINECONE_ENV``` envirnoment variables, and set the 'vector_db' parameter to True. The vector db index is created upon first execution.
+
 
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 - Supported models: gpt-3.5-turbo, gpt-3.5-turbo-613, gpt-3.5-turbo-16k, gpt-4, gpt-4-0613.
@@ -117,12 +135,11 @@
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
-- Add Knowledge Base in a vector DB. A matching(similar) Q:A pairs will be used as a context/reference for subsequent questions to improve the accuracy and relevancy.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.3.6/README.md` & `bambooai-0.3.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 # BambooAI
 A lightweight library that leverages Language Models (LLMs) to enable natural language interactions, allowing you to converse with your pandas DataFrames.
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
-My primary goal was to build a library that acts as a steadfast companion for analysts of all skill levels, rather than acting as the analyst itself. This library simplifies the intricate process of data analysis and visualization, serving to streamline the user's workflow. It's been crafted with a focus on user-friendliness, efficiency, and adaptability, enabling it to cater to a wide range of users and their unique analytical needs. By functioning as an aid rather than the main analyst, this library not only facilitates smoother operations but also empowers users to effectively employ their analytical skills, enhancing their overall productivity.
+My main goal was to create a tool to help analysts at all levels, not to replace them. This library makes data analysis and visualization easier, helping to improve workflows. It's designed to be easy to use, efficient, and adaptable to different users' needs. As a supportive tool, not the main operator, it helps users apply their own analytical skills more effectively and increase their productivity.
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
 https://github.com/pgalko/BambooAI/assets/39939157/2d8e4a9f-29c4-438b-8c13-126a05065ef8
 
 ## How it works
 
-- The user begins by starting the BambooAI agent.
-- BambooAI subsequently checks if a question has been provided:
-  - If a question is available, it continues to the next step.
-  - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
-- Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents a summary in the form of numbered task list.
-- The agent then replaces the original question with the task list from the previous step and sends this as a prompt to the OpenAI API for code generation.
-- The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
-  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
-- The received code is then executed to generate an answer or a visualization:
-  - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
-  - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
-- The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
-- Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
- 
-**Flow chart:**
+The BambooAI agent operates through several key steps to interact with users and generate responses:
+
+**1. Initiation**
+- The user starts the BambooAI agent.
+- If there's no input question, the agent prompts the user to either input a question or type 'exit' to terminate the program.
+
+**2. Task Evaluation**
+- The agent stores the received question and utilizes the Language Learning Model (LLM) to evaluate and categorize it.
+- The LLM determines whether the question necessitates a narrative response, additional information, or can be resolved using code.
+
+**3. Dynamic Prompt Build**
+- If code can resolve the question, the agent formulates an algorithm expressed as a task list.
+- The original question is modified to align with this algorithm. The agent conducts a semantic search for similar questions.
+- Any matching questions found are appended to the prompt as examples, and GPT-3 is used to generate code based on the algorithm.
+
+**4. Debugging, Execution, and Error Correction**
+- If the generated code needs debugging, GPT-4 is engaged.
+- The code is executed, and if errors occur, the agent logs the error message and refers it to the LLM (GPT-3 or GPT-4, depending on the settings) for correction.
+- This process continues until successful code execution.
+
+**5. Results, Ranking, and Knowledge Base Build**
+- Post successful execution, GPT-4 is used to rank the answer.
+- If the rank surpasses a set threshold, the question, answer, code, and rank are stored in the Pinecone vector database.
+- Regardless of the rank, the final answer or visualization is formatted and presented to the user.
+
+**6. Human Feedback and Loop Continuation**
+- The agent seeks feedback from the user.
+- If the user validates the auto-generated ranking, the question/answer pair is stored in the vector database.
+- If not, a new execution loop begins.
+
+Throughout this process, the agent continuously solicits user input, stores messages for context, and generates and executes code to ensure optimal results. Various AI models and a vector database are employed in this process to provide accurate and helpful responses to user's questions.
 
-![](images/flow_chart_3.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -48,26 +63,26 @@
 Parameters
 
 ```
 df: pd.DataFrame - Dataframe(Required)
 
 max_conversations: int - Number of "user:assistant" conversation pairs to keep in memory for a context. Default=2
 
-llm: str - Base LLM model. Default = gpt-3.5-turbo
+llm: str - Base LLM model. Default = gpt-3.5-turbo-0613
 
 llm_switch: bool - If True, the agent will switch to gpt-4 after error
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
-rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+vector_db: bool - If True, each answer will first be ranked from 1 to 10. If the rank surpasses a certain threshold (8), the corresponding question (vectorised), answer, code, and rank (metadata) are all stored in the Pinecone database. Each time a new question is asked, these records will be searched. If the similarity score is above 0.9, they will be offered as examples and included in the prompt (in a one-shot learning scenario)
 
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
 
-e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True)
+e.g. bamboo = BambooAI(df, debug=True, vector_db=True, llm_switch=True, exploratory=True)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -87,16 +102,19 @@
 bamboo = BambooAI(df)
 bamboo.pd_agent_converse("Calculate 30, 50, 75 and 90 percentiles of the heart rate column")
 ```
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
-The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
-The key can be obtained from here: https://platform.openai.com/account/api-keys
+The library requires an OpenAI API account and the API key to connect to OpenAI LLMs. The OpenAI API key needs to be stored in a ```OPENAI_API_KEY``` environment variable.
+The key can be obtained from here: https://platform.openai.com/account/api-keys.
+
+The Pincone vector db is optional. If you don want to use it, you dont need to do anything. If you have an account with Pinecone and would like to use the knowledge base and ranking features, you will be required to setup ```PINECONE_API_KEY``` and ```PINECONE_ENV``` envirnoment variables, and set the 'vector_db' parameter to True. The vector db index is created upon first execution.
+
 
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 - Supported models: gpt-3.5-turbo, gpt-3.5-turbo-613, gpt-3.5-turbo-16k, gpt-4, gpt-4-0613.
@@ -104,10 +122,9 @@
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
-- Add Knowledge Base in a vector DB. A matching(similar) Q:A pairs will be used as a context/reference for subsequent questions to improve the accuracy and relevancy.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.3.6/bambooai/bambooai.py` & `bambooai-0.3.7/bambooai/bambooai.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,1643 +13,1977 @@
 000000c0: 642c 2063 7072 696e 740d 0a66 726f 6d20  d, cprint..from 
 000000d0: 4950 7974 686f 6e2e 6469 7370 6c61 7920  IPython.display 
 000000e0: 696d 706f 7274 2064 6973 706c 6179 2c20  import display, 
 000000f0: 496d 6167 652c 2048 544d 4c0d 0a69 6d70  Image, HTML..imp
 00000100: 6f72 7420 7761 726e 696e 6773 0d0a 7761  ort warnings..wa
 00000110: 726e 696e 6773 2e66 696c 7465 7277 6172  rnings.filterwar
 00000120: 6e69 6e67 7328 2769 676e 6f72 6527 290d  nings('ignore').
-00000130: 0a23 5275 6e6e 696e 6720 6173 2061 2073  .#Running as a s
-00000140: 6372 6970 740d 0a23 696d 706f 7274 2070  cript..#import p
-00000150: 726f 6d70 7473 0d0a 2369 6d70 6f72 7420  rompts..#import 
-00000160: 6675 6e63 5f63 616c 6c73 0d0a 2352 756e  func_calls..#Run
-00000170: 6e69 6e67 2061 7320 6120 7061 636b 6167  ning as a packag
-00000180: 650d 0a66 726f 6d20 2e20 696d 706f 7274  e..from . import
-00000190: 2070 726f 6d70 7473 0d0a 6672 6f6d 202e   prompts..from .
-000001a0: 2069 6d70 6f72 7420 6675 6e63 5f63 616c   import func_cal
-000001b0: 6c73 0d0a 0d0a 636c 6173 7320 4261 6d62  ls....class Bamb
-000001c0: 6f6f 4149 3a0d 0a20 2020 2064 6566 205f  ooAI:..    def _
-000001d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6466  _init__(self, df
-000001e0: 3a20 7064 2e44 6174 6146 7261 6d65 2c0d  : pd.DataFrame,.
-000001f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000200: 2020 6d61 785f 636f 6e76 6572 7361 7469    max_conversati
-00000210: 6f6e 733a 2069 6e74 203d 2034 2c0d 0a20  ons: int = 4,.. 
-00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000230: 6c6c 6d3a 2073 7472 203d 2027 6770 742d  llm: str = 'gpt-
-00000240: 332e 352d 7475 7262 6f2d 3036 3133 272c  3.5-turbo-0613',
-00000250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000260: 2020 206c 6c6d 5f66 756e 633a 2073 7472     llm_func: str
-00000270: 203d 2027 6770 742d 332e 352d 7475 7262   = 'gpt-3.5-turb
-00000280: 6f2d 3036 3133 272c 0d0a 2020 2020 2020  o-0613',..      
-00000290: 2020 2020 2020 2020 2020 206c 6c6d 5f31             llm_1
-000002a0: 366b 3a20 7374 7220 3d20 2767 7074 2d33  6k: str = 'gpt-3
-000002b0: 2e35 2d74 7572 626f 2d31 366b 272c 0d0a  .5-turbo-16k',..
+00000130: 0a0d 0a23 5275 6e6e 696e 6720 6173 2061  ...#Running as a
+00000140: 2073 6372 6970 740d 0a23 696d 706f 7274   script..#import
+00000150: 2070 726f 6d70 7473 0d0a 2369 6d70 6f72   prompts..#impor
+00000160: 7420 6675 6e63 5f63 616c 6c73 0d0a 2369  t func_calls..#i
+00000170: 6d70 6f72 7420 7161 5f72 6574 7269 6576  mport qa_retriev
+00000180: 616c 0d0a 0d0a 2352 756e 6e69 6e67 2061  al....#Running a
+00000190: 7320 6120 7061 636b 6167 650d 0a66 726f  s a package..fro
+000001a0: 6d20 2e20 696d 706f 7274 2070 726f 6d70  m . import promp
+000001b0: 7473 0d0a 6672 6f6d 202e 2069 6d70 6f72  ts..from . impor
+000001c0: 7420 6675 6e63 5f63 616c 6c73 0d0a 6672  t func_calls..fr
+000001d0: 6f6d 202e 2069 6d70 6f72 7420 7161 5f72  om . import qa_r
+000001e0: 6574 7269 6576 616c 0d0a 0d0a 636c 6173  etrieval....clas
+000001f0: 7320 4261 6d62 6f6f 4149 3a0d 0a20 2020  s BambooAI:..   
+00000200: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000210: 6c66 2c20 6466 3a20 7064 2e44 6174 6146  lf, df: pd.DataF
+00000220: 7261 6d65 2c0d 0a20 2020 2020 2020 2020  rame,..         
+00000230: 2020 2020 2020 2020 6d61 785f 636f 6e76          max_conv
+00000240: 6572 7361 7469 6f6e 733a 2069 6e74 203d  ersations: int =
+00000250: 2034 2c0d 0a20 2020 2020 2020 2020 2020   4,..           
+00000260: 2020 2020 2020 6c6c 6d3a 2073 7472 203d        llm: str =
+00000270: 2027 6770 742d 332e 352d 7475 7262 6f2d   'gpt-3.5-turbo-
+00000280: 3036 3133 272c 0d0a 2020 2020 2020 2020  0613',..        
+00000290: 2020 2020 2020 2020 206c 6c6d 5f66 756e           llm_fun
+000002a0: 633a 2073 7472 203d 2027 6770 742d 332e  c: str = 'gpt-3.
+000002b0: 352d 7475 7262 6f2d 3036 3133 272c 0d0a  5-turbo-0613',..
 000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 206c 6c6d 5f67 7074 343a 2073 7472 203d   llm_gpt4: str =
-000002e0: 2027 6770 742d 342d 3036 3133 272c 0d0a   'gpt-4-0613',..
-000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000300: 2064 6562 7567 3a20 626f 6f6c 203d 2046   debug: bool = F
-00000310: 616c 7365 2c20 0d0a 2020 2020 2020 2020  alse, ..        
-00000320: 2020 2020 2020 2020 2072 616e 6b3a 2062           rank: b
-00000330: 6f6f 6c20 3d20 4661 6c73 652c 200d 0a20  ool = False, .. 
-00000340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000350: 6c6c 6d5f 7377 6974 6368 3a20 626f 6f6c  llm_switch: bool
-00000360: 203d 2046 616c 7365 2c20 0d0a 2020 2020   = False, ..    
-00000370: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-00000380: 6c6f 7261 746f 7279 3a20 626f 6f6c 203d  loratory: bool =
-00000390: 2054 7275 652c 200d 0a20 2020 2020 2020   True, ..       
-000003a0: 2020 2020 2020 2020 2020 293a 0d0a 0d0a            ):....
-000003b0: 2020 2020 2020 2020 7365 6c66 2e41 5049          self.API
-000003c0: 5f4b 4559 203d 206f 732e 656e 7669 726f  _KEY = os.enviro
-000003d0: 6e2e 6765 7428 274f 5045 4e41 495f 4150  n.get('OPENAI_AP
-000003e0: 495f 4b45 5927 290d 0a20 2020 2020 2020  I_KEY')..       
-000003f0: 2073 656c 662e 4d41 585f 4552 524f 525f   self.MAX_ERROR_
-00000400: 434f 5252 4543 5449 4f4e 5320 3d20 350d  CORRECTIONS = 5.
-00000410: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
-00000420: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-00000430: 7220 6f66 2071 7565 7374 696f 6e2f 616e  r of question/an
-00000440: 7377 6572 2070 6169 7273 2074 6f20 6265  swer pairs to be
-00000450: 206b 6570 7420 696e 2074 6865 2063 6f6e   kept in the con
-00000460: 7665 7273 6174 696f 6e20 6d65 6d6d 6f72  versation memmor
-00000470: 790d 0a20 2020 2020 2020 2073 656c 662e  y..        self.
-00000480: 4d41 585f 434f 4e56 4552 5341 5449 4f4e  MAX_CONVERSATION
-00000490: 5320 3d20 286d 6178 5f63 6f6e 7665 7273  S = (max_convers
-000004a0: 6174 696f 6e73 2a32 2920 2d20 310d 0a20  ations*2) - 1.. 
-000004b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000004c0: 2023 2053 746f 7265 2074 6865 206f 7269   # Store the ori
-000004d0: 6769 6e61 6c20 6461 7461 6672 616d 652e  ginal dataframe.
-000004e0: 2054 6869 7320 7769 6c6c 2062 6520 7573   This will be us
-000004f0: 6564 2074 6f20 7265 7365 7420 7468 6520  ed to reset the 
-00000500: 6461 7461 6672 616d 6520 6265 666f 7265  dataframe before
-00000510: 2065 7865 6375 7469 6e67 2074 6865 2063   executing the c
-00000520: 6f64 650d 0a20 2020 2020 2020 2073 656c  ode..        sel
-00000530: 662e 6f72 6967 696e 616c 5f64 6620 3d20  f.original_df = 
-00000540: 6466 0d0a 2020 2020 2020 2020 7365 6c66  df..        self
-00000550: 2e64 6620 3d20 6466 2e63 6f70 7928 2920  .df = df.copy() 
-00000560: 2023 206d 616b 6520 6120 636f 7079 206f   # make a copy o
-00000570: 6620 7468 6520 6461 7461 6672 616d 650d  f the dataframe.
-00000580: 0a20 2020 2020 2020 2073 656c 662e 6466  .        self.df
-00000590: 5f68 6561 6420 3d20 7365 6c66 2e6f 7269  _head = self.ori
-000005a0: 6769 6e61 6c5f 6466 2e68 6561 6428 3129  ginal_df.head(1)
-000005b0: 0d0a 0d0a 2020 2020 2020 2020 2320 4c4c  ....        # LL
-000005c0: 4d73 0d0a 2020 2020 2020 2020 7365 6c66  Ms..        self
-000005d0: 2e6c 6c6d 203d 206c 6c6d 0d0a 2020 2020  .llm = llm..    
-000005e0: 2020 2020 7365 6c66 2e6c 6c6d 5f66 756e      self.llm_fun
-000005f0: 6320 3d20 6c6c 6d5f 6675 6e63 0d0a 2020  c = llm_func..  
-00000600: 2020 2020 2020 7365 6c66 2e6c 6c6d 5f31        self.llm_1
-00000610: 366b 203d 206c 6c6d 5f31 366b 0d0a 2020  6k = llm_16k..  
-00000620: 2020 2020 2020 7365 6c66 2e6c 6c6d 5f67        self.llm_g
-00000630: 7074 3420 3d20 6c6c 6d5f 6770 7434 0d0a  pt4 = llm_gpt4..
-00000640: 0d0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-00000650: 7468 6520 6465 6275 6720 6d6f 6465 2e20  the debug mode. 
-00000660: 5468 6973 206d 6f64 6520 6973 2054 7275  This mode is Tru
-00000670: 6520 7768 656e 2079 6f75 2077 616e 7420  e when you want 
-00000680: 7468 6520 6d6f 6465 6c20 746f 2064 6562  the model to deb
-00000690: 7567 2074 6865 2063 6f64 6520 616e 6420  ug the code and 
-000006a0: 636f 7272 6563 7420 6974 2e0d 0a20 2020  correct it...   
-000006b0: 2020 2020 2073 656c 662e 6465 6275 6720       self.debug 
-000006c0: 3d20 6465 6275 670d 0a20 2020 2020 2020  = debug..       
-000006d0: 2023 2053 6574 2074 6865 206c 6c6d 5f73   # Set the llm_s
-000006e0: 7769 7463 6820 6d6f 6465 2e20 5468 6973  witch mode. This
-000006f0: 206d 6f64 6520 6973 2054 7275 6520 7768   mode is True wh
-00000700: 656e 2079 6f75 2077 616e 7420 7468 6520  en you want the 
-00000710: 6d6f 6465 6c20 746f 2073 7769 7463 6820  model to switch 
-00000720: 746f 2067 7074 2d34 2066 6f72 2064 6562  to gpt-4 for deb
-00000730: 7567 6769 6e67 2c20 6572 726f 7220 636f  ugging, error co
-00000740: 7272 6563 7469 6f6e 2061 6e64 2072 616e  rrection and ran
-00000750: 6b69 6e67 2e0d 0a20 2020 2020 2020 2073  king...        s
-00000760: 656c 662e 6c6c 6d5f 7377 6974 6368 203d  elf.llm_switch =
-00000770: 206c 6c6d 5f73 7769 7463 680d 0a20 2020   llm_switch..   
-00000780: 2020 2020 2023 2053 6574 2074 6865 2072       # Set the r
-00000790: 616e 6b20 6d6f 6465 2e20 5468 6973 206d  ank mode. This m
-000007a0: 6f64 6520 6973 2054 7275 6520 7768 656e  ode is True when
-000007b0: 2079 6f75 2077 616e 7420 7468 6520 6d6f   you want the mo
-000007c0: 6465 6c20 746f 2072 616e 6b20 7468 6520  del to rank the 
-000007d0: 6765 6e65 7261 7465 6420 636f 6465 2e0d  generated code..
-000007e0: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
-000007f0: 6e6b 203d 2072 616e 6b0d 0a0d 0a20 2020  nk = rank....   
-00000800: 2020 2020 2023 2053 6574 2074 6865 2065       # Set the e
-00000810: 7870 6c6f 7261 746f 7279 206d 6f64 652e  xploratory mode.
-00000820: 2054 6869 7320 6d6f 6465 2069 7320 5472   This mode is Tr
-00000830: 7565 2077 6865 6e20 796f 7520 7761 6e74  ue when you want
-00000840: 2074 6865 206d 6f64 656c 2074 6f20 6576   the model to ev
-00000850: 616c 7561 7465 2074 6865 206f 7269 6769  aluate the origi
-00000860: 6e61 6c20 7072 6f6d 7074 2061 6e64 2062  nal prompt and b
-00000870: 7265 616b 2069 7420 646f 776e 2069 6e20  reak it down in 
-00000880: 616c 676f 7269 7468 6d2e 0d0a 2020 2020  algorithm...    
-00000890: 2020 2020 7365 6c66 2e65 7870 6c6f 7261      self.explora
-000008a0: 746f 7279 203d 2065 7870 6c6f 7261 746f  tory = explorato
-000008b0: 7279 0d0a 2020 2020 2020 2020 0d0a 2020  ry..        ..  
-000008c0: 2020 2020 2020 2320 5072 6f6d 7074 730d        # Prompts.
-000008d0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-000008e0: 736b 5f65 7661 6c75 6174 696f 6e20 3d20  sk_evaluation = 
-000008f0: 7072 6f6d 7074 732e 7461 736b 5f65 7661  prompts.task_eva
-00000900: 6c75 6174 696f 6e0d 0a20 2020 2020 2020  luation..       
-00000910: 2073 656c 662e 7379 7374 656d 5f74 6173   self.system_tas
-00000920: 6b20 3d20 7072 6f6d 7074 732e 7379 7374  k = prompts.syst
-00000930: 656d 5f74 6173 6b0d 0a20 2020 2020 2020  em_task..       
-00000940: 2073 656c 662e 7573 6572 5f74 6173 6b20   self.user_task 
-00000950: 3d20 7072 6f6d 7074 732e 7573 6572 5f74  = prompts.user_t
-00000960: 6173 6b0d 0a20 2020 2020 2020 2073 656c  ask..        sel
-00000970: 662e 6572 726f 725f 636f 7272 6563 745f  f.error_correct_
-00000980: 7461 736b 203d 2070 726f 6d70 7473 2e65  task = prompts.e
-00000990: 7272 6f72 5f63 6f72 7265 6374 5f74 6173  rror_correct_tas
-000009a0: 6b0d 0a20 2020 2020 2020 2073 656c 662e  k..        self.
-000009b0: 6465 6275 675f 636f 6465 5f74 6173 6b20  debug_code_task 
-000009c0: 3d20 7072 6f6d 7074 732e 6465 6275 675f  = prompts.debug_
-000009d0: 636f 6465 5f74 6173 6b20 200d 0a20 2020  code_task  ..   
-000009e0: 2020 2020 2073 656c 662e 7261 6e6b 5f61       self.rank_a
-000009f0: 6e73 7765 7220 3d20 7072 6f6d 7074 732e  nswer = prompts.
-00000a00: 7261 6e6b 5f61 6e73 7765 720d 0a20 2020  rank_answer..   
-00000a10: 2020 2020 2073 656c 662e 736f 6c75 7469       self.soluti
-00000a20: 6f6e 5f69 6e73 6967 6874 7320 3d20 7072  on_insights = pr
-00000a30: 6f6d 7074 732e 736f 6c75 7469 6f6e 5f69  ompts.solution_i
-00000a40: 6e73 6967 6874 730d 0a0d 0a20 2020 2020  nsights....     
-00000a50: 2020 2023 2046 756e 6374 696f 6e73 0d0a     # Functions..
-00000a60: 2020 2020 2020 2020 7365 6c66 2e74 6173          self.tas
-00000a70: 6b5f 6576 616c 5f66 756e 6374 696f 6e20  k_eval_function 
-00000a80: 3d20 6675 6e63 5f63 616c 6c73 2e74 6173  = func_calls.tas
-00000a90: 6b5f 6576 616c 5f66 756e 6374 696f 6e0d  k_eval_function.
-00000aa0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00000ab0: 7369 6768 7473 5f66 756e 6374 696f 6e20  sights_function 
-00000ac0: 3d20 6675 6e63 5f63 616c 6c73 2e73 6f6c  = func_calls.sol
-00000ad0: 7574 696f 6e5f 696e 7369 6768 7473 5f66  ution_insights_f
-00000ae0: 756e 6374 696f 6e0d 0a20 2020 2020 2020  unction..       
-00000af0: 200d 0a20 2020 2020 2020 206f 7065 6e61   ..        opena
-00000b00: 692e 6170 695f 6b65 7920 3d20 7365 6c66  i.api_key = self
-00000b10: 2e41 5049 5f4b 4559 0d0a 0d0a 2020 2020  .API_KEY....    
-00000b20: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
-00000b30: 2074 6865 2074 6f74 616c 2074 6f6b 656e   the total token
-00000b40: 7320 7573 6564 206c 6973 742e 2054 6869  s used list. Thi
-00000b50: 7320 6c69 7374 2077 696c 6c20 6265 2075  s list will be u
-00000b60: 7365 6420 746f 206b 6565 7020 7472 6163  sed to keep trac
-00000b70: 6b20 6f66 2074 6865 2074 6f74 616c 2074  k of the total t
-00000b80: 6f6b 656e 7320 7573 6564 2062 7920 7468  okens used by th
-00000b90: 6520 6d6f 6465 6c0d 0a20 2020 2020 2020  e model..       
-00000ba0: 2073 656c 662e 746f 7461 6c5f 746f 6b65   self.total_toke
-00000bb0: 6e73 5f75 7365 6420 3d20 5b5d 0d0a 0d0a  ns_used = []....
-00000bc0: 2020 2020 6465 6620 6c6c 6d5f 6361 6c6c      def llm_call
-00000bd0: 2873 656c 662c 206d 6573 7361 6765 733a  (self, messages:
-00000be0: 2073 7472 2c20 7465 6d70 6572 6174 7572   str, temperatur
-00000bf0: 653a 2066 6c6f 6174 203d 2030 2c20 6d61  e: float = 0, ma
-00000c00: 785f 746f 6b65 6e73 3a20 696e 7420 3d20  x_tokens: int = 
-00000c10: 3130 3030 2c20 6c6c 6d5f 6361 7363 6164  1000, llm_cascad
-00000c20: 653a 2062 6f6f 6c20 3d20 4661 6c73 6529  e: bool = False)
-00000c30: 3a0d 0a20 2020 2020 2020 206d 6f64 656c  :..        model
-00000c40: 203d 2073 656c 662e 6c6c 6d0d 0a20 2020   = self.llm..   
-00000c50: 2020 2020 2069 6620 6c6c 6d5f 6361 7363       if llm_casc
-00000c60: 6164 653a 0d0a 2020 2020 2020 2020 2020  ade:..          
-00000c70: 2020 6d6f 6465 6c20 3d20 7365 6c66 2e6c    model = self.l
-00000c80: 6c6d 5f67 7074 340d 0a20 2020 2020 2020  lm_gpt4..       
-00000c90: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00000ca0: 2020 2072 6573 706f 6e73 6520 3d20 6f70     response = op
-00000cb0: 656e 6169 2e43 6861 7443 6f6d 706c 6574  enai.ChatComplet
-00000cc0: 696f 6e2e 6372 6561 7465 280d 0a20 2020  ion.create(..   
-00000cd0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00000ce0: 656c 3d6d 6f64 656c 2c0d 0a20 2020 2020  el=model,..     
-00000cf0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00000d00: 6765 733d 6d65 7373 6167 6573 2c0d 0a20  ges=messages,.. 
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000d20: 656d 7065 7261 7475 7265 3d74 656d 7065  emperature=tempe
-00000d30: 7261 7475 7265 2c0d 0a20 2020 2020 2020  rature,..       
-00000d40: 2020 2020 2020 2020 206d 6178 5f74 6f6b           max_tok
-00000d50: 656e 733d 6d61 785f 746f 6b65 6e73 2c0d  ens=max_tokens,.
-00000d60: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00000d70: 2020 2020 2020 2020 6578 6365 7074 206f          except o
-00000d80: 7065 6e61 692e 6572 726f 722e 5261 7465  penai.error.Rate
-00000d90: 4c69 6d69 7445 7272 6f72 3a0d 0a20 2020  LimitError:..   
-00000da0: 2020 2020 2020 2020 2070 7269 6e74 280d           print(.
-00000db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000dc0: 2022 5468 6520 4f70 656e 4149 2041 5049   "The OpenAI API
-00000dd0: 2072 6174 6520 6c69 6d69 7420 6861 7320   rate limit has 
-00000de0: 6265 656e 2065 7863 6565 6465 642e 2057  been exceeded. W
-00000df0: 6169 7469 6e67 2031 3020 7365 636f 6e64  aiting 10 second
-00000e00: 7320 616e 6420 7472 7969 6e67 2061 6761  s and trying aga
-00000e10: 696e 2e22 0d0a 2020 2020 2020 2020 2020  in."..          
-00000e20: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00000e30: 2074 696d 652e 736c 6565 7028 3130 290d   time.sleep(10).
-00000e40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00000e50: 706f 6e73 6520 3d20 6f70 656e 6169 2e43  ponse = openai.C
-00000e60: 6861 7443 6f6d 706c 6574 696f 6e2e 6372  hatCompletion.cr
-00000e70: 6561 7465 280d 0a20 2020 2020 2020 2020  eate(..         
-00000e80: 2020 2020 2020 206d 6f64 656c 3d6d 6f64         model=mod
-00000e90: 656c 2c0d 0a20 2020 2020 2020 2020 2020  el,..           
-00000ea0: 2020 2020 206d 6573 7361 6765 733d 6d65       messages=me
-00000eb0: 7373 6167 6573 2c0d 0a20 2020 2020 2020  ssages,..       
-00000ec0: 2020 2020 2020 2020 2074 656d 7065 7261           tempera
-00000ed0: 7475 7265 3d74 656d 7065 7261 7475 7265  ture=temperature
-00000ee0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000ef0: 2020 206d 6178 5f74 6f6b 656e 733d 6d61     max_tokens=ma
-00000f00: 785f 746f 6b65 6e73 2c0d 0a20 2020 2020  x_tokens,..     
-00000f10: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00000f20: 2020 2320 4578 6365 6564 6564 2074 6865    # Exceeded the
-00000f30: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
-00000f40: 6f66 2074 6f6b 656e 7320 616c 6c6f 7765  of tokens allowe
-00000f50: 6420 6279 2074 6865 2041 5049 0d0a 2020  d by the API..  
-00000f60: 2020 2020 2020 6578 6365 7074 206f 7065        except ope
-00000f70: 6e61 692e 6572 726f 722e 496e 7661 6c69  nai.error.Invali
-00000f80: 6452 6571 7565 7374 4572 726f 723a 0d0a  dRequestError:..
-00000f90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00000fa0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-00000fb0: 2020 2020 2254 6865 204f 7065 6e41 4920      "The OpenAI 
-00000fc0: 4150 4920 6d61 7869 6d75 6d20 746f 6b65  API maximum toke
-00000fd0: 6e73 206c 696d 6974 2068 6173 2062 6565  ns limit has bee
-00000fe0: 6e20 6578 6365 6564 6564 2e20 5377 6974  n exceeded. Swit
-00000ff0: 6368 696e 6720 746f 2061 2031 364b 206d  ching to a 16K m
-00001000: 6f64 656c 2e22 0d0a 2020 2020 2020 2020  odel."..        
-00001010: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00001020: 2020 2072 6573 706f 6e73 6520 3d20 6f70     response = op
-00001030: 656e 6169 2e43 6861 7443 6f6d 706c 6574  enai.ChatComplet
-00001040: 696f 6e2e 6372 6561 7465 280d 0a20 2020  ion.create(..   
-00001050: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00001060: 656c 3d73 656c 662e 6c6c 6d5f 3136 6b2c  el=self.llm_16k,
-00001070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001080: 2020 6d65 7373 6167 6573 3d6d 6573 7361    messages=messa
-00001090: 6765 732c 0d0a 2020 2020 2020 2020 2020  ges,..          
-000010a0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-000010b0: 653d 7465 6d70 6572 6174 7572 652c 0d0a  e=temperature,..
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 6d61 785f 746f 6b65 6e73 3d6d 6178 5f74  max_tokens=max_t
-000010e0: 6f6b 656e 732c 0d0a 2020 2020 2020 2020  okens,..        
-000010f0: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
-00001100: 2063 6f6e 7465 6e74 203d 2072 6573 706f   content = respo
-00001110: 6e73 652e 6368 6f69 6365 735b 305d 2e6d  nse.choices[0].m
-00001120: 6573 7361 6765 2e63 6f6e 7465 6e74 2e73  essage.content.s
-00001130: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
-00001140: 746f 6b65 6e73 5f75 7365 6420 3d20 7265  tokens_used = re
-00001150: 7370 6f6e 7365 2e75 7361 6765 2e74 6f74  sponse.usage.tot
-00001160: 616c 5f74 6f6b 656e 730d 0a0d 0a20 2020  al_tokens....   
-00001170: 2020 2020 2072 6574 7572 6e20 636f 6e74       return cont
-00001180: 656e 742c 2074 6f6b 656e 735f 7573 6564  ent, tokens_used
-00001190: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-000011a0: 6c6c 6d5f 6675 6e63 5f63 616c 6c28 7365  llm_func_call(se
-000011b0: 6c66 2c20 6d65 7373 6167 6573 2c20 6675  lf, messages, fu
-000011c0: 6e63 7469 6f6e 732c 2066 756e 6374 696f  nctions, functio
-000011d0: 6e5f 6e61 6d65 293a 0d0a 2020 2020 2020  n_name):..      
-000011e0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000011f0: 2020 2020 7265 7370 6f6e 7365 203d 206f      response = o
-00001200: 7065 6e61 692e 4368 6174 436f 6d70 6c65  penai.ChatComple
-00001210: 7469 6f6e 2e63 7265 6174 6528 0d0a 2020  tion.create(..  
-00001220: 2020 2020 2020 2020 2020 6d6f 6465 6c20            model 
-00001230: 3d20 7365 6c66 2e6c 6c6d 5f66 756e 632c  = self.llm_func,
-00001240: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
-00001250: 7373 6167 6573 3d6d 6573 7361 6765 732c  ssages=messages,
-00001260: 0d0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
-00001270: 6e63 7469 6f6e 733d 6675 6e63 7469 6f6e  nctions=function
-00001280: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00001290: 6675 6e63 7469 6f6e 5f63 616c 6c20 3d20  function_call = 
-000012a0: 6675 6e63 7469 6f6e 5f6e 616d 652c 0d0a  function_name,..
-000012b0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000012c0: 6572 6174 7572 653d 302c 0d0a 2020 2020  erature=0,..    
-000012d0: 2020 2020 2020 2020 6d61 785f 746f 6b65          max_toke
-000012e0: 6e73 203d 2037 3030 2c20 0d0a 2020 2020  ns = 700, ..    
-000012f0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00001300: 2020 2065 7863 6570 7420 6f70 656e 6169     except openai
-00001310: 2e65 7272 6f72 2e52 6174 654c 696d 6974  .error.RateLimit
-00001320: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-00001330: 2020 2020 7072 696e 7428 0d0a 2020 2020      print(..    
-00001340: 2020 2020 2020 2020 2020 2020 2254 6865              "The
-00001350: 204f 7065 6e41 4920 4150 4920 7261 7465   OpenAI API rate
-00001360: 206c 696d 6974 2068 6173 2062 6565 6e20   limit has been 
-00001370: 6578 6365 6564 6564 2e20 5761 6974 696e  exceeded. Waitin
-00001380: 6720 3130 2073 6563 6f6e 6473 2061 6e64  g 10 seconds and
-00001390: 2074 7279 696e 6720 6167 6169 6e2e 220d   trying again.".
-000013a0: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-000013b0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-000013c0: 2e73 6c65 6570 2831 3029 0d0a 2020 2020  .sleep(10)..    
-000013d0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000013e0: 203d 206f 7065 6e61 692e 4368 6174 436f   = openai.ChatCo
-000013f0: 6d70 6c65 7469 6f6e 2e63 7265 6174 6528  mpletion.create(
-00001400: 0d0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
-00001410: 6465 6c20 3d20 7365 6c66 2e6c 6c6d 5f66  del = self.llm_f
-00001420: 756e 632c 0d0a 2020 2020 2020 2020 2020  unc,..          
-00001430: 2020 6d65 7373 6167 6573 3d6d 6573 7361    messages=messa
-00001440: 6765 732c 0d0a 2020 2020 2020 2020 2020  ges,..          
-00001450: 2020 6675 6e63 7469 6f6e 733d 6675 6e63    functions=func
-00001460: 7469 6f6e 732c 0d0a 2020 2020 2020 2020  tions,..        
-00001470: 2020 2020 6675 6e63 7469 6f6e 5f63 616c      function_cal
-00001480: 6c20 3d20 6675 6e63 7469 6f6e 5f6e 616d  l = function_nam
-00001490: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000014a0: 7465 6d70 6572 6174 7572 653d 302c 0d0a  temperature=0,..
-000014b0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-000014c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000014d0: 2066 6e5f 6e61 6d65 203d 2072 6573 706f   fn_name = respo
-000014e0: 6e73 652e 6368 6f69 6365 735b 305d 2e6d  nse.choices[0].m
-000014f0: 6573 7361 6765 5b22 6675 6e63 7469 6f6e  essage["function
-00001500: 5f63 616c 6c22 5d2e 6e61 6d65 0d0a 2020  _call"].name..  
-00001510: 2020 2020 2020 6172 6775 6d65 6e74 7320        arguments 
-00001520: 3d20 7265 7370 6f6e 7365 2e63 686f 6963  = response.choic
-00001530: 6573 5b30 5d2e 6d65 7373 6167 655b 2266  es[0].message["f
-00001540: 756e 6374 696f 6e5f 6361 6c6c 225d 2e61  unction_call"].a
-00001550: 7267 756d 656e 7473 0d0a 2020 2020 2020  rguments..      
-00001560: 2020 746f 6b65 6e73 5f75 7365 6420 3d20    tokens_used = 
-00001570: 7265 7370 6f6e 7365 2e75 7361 6765 2e74  response.usage.t
-00001580: 6f74 616c 5f74 6f6b 656e 730d 0a0d 0a20  otal_tokens.... 
-00001590: 2020 2020 2020 2072 6574 7572 6e20 666e         return fn
-000015a0: 5f6e 616d 652c 6172 6775 6d65 6e74 732c  _name,arguments,
-000015b0: 746f 6b65 6e73 5f75 7365 640d 0a0d 0a20  tokens_used.... 
-000015c0: 2020 200d 0a20 2020 2023 2046 756e 6374     ..    # Funct
-000015d0: 696f 6e73 2074 6f20 7361 6e69 7469 7a65  ions to sanitize
-000015e0: 2074 6865 206f 7574 7075 7420 6672 6f6d   the output from
-000015f0: 2074 6865 204c 4c4d 0d0a 2020 2020 6465   the LLM..    de
-00001600: 6620 5f65 7874 7261 6374 5f63 6f64 6528  f _extract_code(
-00001610: 7365 6c66 2c72 6573 706f 6e73 653a 2073  self,response: s
-00001620: 7472 2c20 7365 7061 7261 746f 723a 2073  tr, separator: s
-00001630: 7472 203d 2022 6060 6022 2920 2d3e 2073  tr = "```") -> s
-00001640: 7472 3a0d 0a0d 0a20 2020 2020 2020 2023  tr:....        #
-00001650: 2044 6566 696e 6520 6120 626c 6163 6b6c   Define a blackl
-00001660: 6973 7420 6f66 2050 7974 686f 6e20 6b65  ist of Python ke
-00001670: 7977 6f72 6473 2061 6e64 2066 756e 6374  ywords and funct
-00001680: 696f 6e73 2074 6861 7420 6172 6520 6e6f  ions that are no
-00001690: 7420 616c 6c6f 7765 640d 0a20 2020 2020  t allowed..     
-000016a0: 2020 2062 6c61 636b 6c69 7374 203d 205b     blacklist = [
-000016b0: 276f 7327 2c27 7375 6270 726f 6365 7373  'os','subprocess
-000016c0: 272c 2773 7973 272c 2765 7661 6c27 2c27  ','sys','eval','
-000016d0: 6578 6563 272c 2766 696c 6527 2c27 736f  exec','file','so
-000016e0: 636b 6574 272c 2775 726c 6c69 6227 2c0d  cket','urllib',.
-000016f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001700: 2020 2020 2027 7368 7574 696c 272c 2770       'shutil','p
-00001710: 6963 6b6c 6527 2c27 6374 7970 6573 272c  ickle','ctypes',
-00001720: 276d 756c 7469 7072 6f63 6573 7369 6e67  'multiprocessing
-00001730: 272c 2774 656d 7066 696c 6527 2c27 676c  ','tempfile','gl
-00001740: 6f62 272c 2763 6f64 6527 2c27 7074 7927  ob','code','pty'
-00001750: 2c27 636f 6d6d 616e 6473 272c 0d0a 2020  ,'commands',..  
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2020 2772 6571 7565 7374 7327 2c27 6367    'requests','cg
-00001780: 6927 2c27 6367 6974 6227 2c27 786d 6c2e  i','cgitb','xml.
-00001790: 6574 7265 652e 456c 656d 656e 7454 7265  etree.ElementTre
-000017a0: 6527 2c27 6275 696c 7469 6e73 270d 0a20  e','builtins'.. 
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
-000017d0: 2320 5365 6172 6368 2066 6f72 2061 2070  # Search for a p
-000017e0: 6174 7465 726e 2062 6574 7765 656e 203c  attern between <
-000017f0: 636f 6465 3e20 616e 6420 3c2f 636f 6465  code> and </code
-00001800: 3e20 696e 2074 6865 2065 7874 7261 6374  > in the extract
-00001810: 6564 2063 6f64 650d 0a20 2020 2020 2020  ed code..       
-00001820: 206d 6174 6368 203d 2072 652e 7365 6172   match = re.sear
-00001830: 6368 2872 223c 636f 6465 3e28 2e2a 293c  ch(r"<code>(.*)<
-00001840: 2f63 6f64 653e 222c 2072 6573 706f 6e73  /code>", respons
-00001850: 652c 2072 652e 444f 5441 4c4c 290d 0a20  e, re.DOTALL).. 
-00001860: 2020 2020 2020 2069 6620 6d61 7463 683a         if match:
-00001870: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00001880: 4966 2061 206d 6174 6368 2069 7320 666f  If a match is fo
-00001890: 756e 642c 2065 7874 7261 6374 2074 6865  und, extract the
-000018a0: 2063 6f64 6520 6265 7477 6565 6e20 3c63   code between <c
-000018b0: 6f64 653e 2061 6e64 203c 2f63 6f64 653e  ode> and </code>
-000018c0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-000018d0: 6465 203d 206d 6174 6368 2e67 726f 7570  de = match.group
-000018e0: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
-000018f0: 2023 2049 6620 7468 6520 7265 7370 6f6e   # If the respon
-00001900: 7365 2063 6f6e 7461 696e 7320 7468 6520  se contains the 
-00001910: 7365 7061 7261 746f 722c 2065 7874 7261  separator, extra
-00001920: 6374 2074 6865 2063 6f64 6520 626c 6f63  ct the code bloc
-00001930: 6b20 6265 7477 6565 6e20 7468 6520 7365  k between the se
-00001940: 7061 7261 746f 7273 0d0a 2020 2020 2020  parators..      
-00001950: 2020 2020 2020 6966 206c 656e 2863 6f64        if len(cod
-00001960: 652e 7370 6c69 7428 7365 7061 7261 746f  e.split(separato
-00001970: 7229 2920 3e20 313a 0d0a 2020 2020 2020  r)) > 1:..      
-00001980: 2020 2020 2020 2020 2020 636f 6465 203d            code =
-00001990: 2063 6f64 652e 7370 6c69 7428 7365 7061   code.split(sepa
-000019a0: 7261 746f 7229 5b31 5d0d 0a0d 0a20 2020  rator)[1]....   
-000019b0: 2020 2020 2023 2049 6620 7468 6520 7265       # If the re
-000019c0: 7370 6f6e 7365 2063 6f6e 7461 696e 7320  sponse contains 
-000019d0: 7468 6520 7365 7061 7261 746f 722c 2065  the separator, e
-000019e0: 7874 7261 6374 2074 6865 2063 6f64 6520  xtract the code 
-000019f0: 626c 6f63 6b20 6265 7477 6565 6e20 7468  block between th
-00001a00: 6520 7365 7061 7261 746f 7273 0d0a 2020  e separators..  
-00001a10: 2020 2020 2020 6966 206c 656e 2872 6573        if len(res
-00001a20: 706f 6e73 652e 7370 6c69 7428 7365 7061  ponse.split(sepa
-00001a30: 7261 746f 7229 2920 3e20 313a 0d0a 2020  rator)) > 1:..  
-00001a40: 2020 2020 2020 2020 2020 636f 6465 203d            code =
-00001a50: 2072 6573 706f 6e73 652e 7370 6c69 7428   response.split(
-00001a60: 7365 7061 7261 746f 7229 5b31 5d0d 0a20  separator)[1].. 
-00001a70: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00001a80: 2020 2020 2023 2052 656d 6f76 6520 7468       # Remove th
-00001a90: 6520 2270 7974 686f 6e22 206f 7220 2270  e "python" or "p
-00001aa0: 7922 2070 7265 6669 7820 6966 2070 7265  y" prefix if pre
-00001ab0: 7365 6e74 0d0a 2020 2020 2020 2020 6966  sent..        if
-00001ac0: 2072 652e 6d61 7463 6828 7222 5e28 7079   re.match(r"^(py
-00001ad0: 7468 6f6e 7c70 7929 222c 2063 6f64 6529  thon|py)", code)
-00001ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
-00001af0: 6f64 6520 3d20 7265 2e73 7562 2872 225e  ode = re.sub(r"^
-00001b00: 2870 7974 686f 6e7c 7079 2922 2c20 2222  (python|py)", ""
-00001b10: 2c20 636f 6465 290d 0a20 2020 2020 2020  , code)..       
-00001b20: 2023 2049 6620 7468 6520 636f 6465 2069   # If the code i
-00001b30: 7320 6265 7477 6565 6e20 7369 6e67 6c65  s between single
-00001b40: 2062 6163 6b74 6963 6b73 2c20 6578 7472   backticks, extr
-00001b50: 6163 7420 7468 6520 636f 6465 2062 6574  act the code bet
-00001b60: 7765 656e 2074 6865 6d0d 0a20 2020 2020  ween them..     
-00001b70: 2020 2069 6620 7265 2e6d 6174 6368 2872     if re.match(r
-00001b80: 225e 602e 2a60 2422 2c20 636f 6465 293a  "^`.*`$", code):
-00001b90: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00001ba0: 6465 203d 2072 652e 7375 6228 7222 5e60  de = re.sub(r"^`
-00001bb0: 282e 2a29 6024 222c 2072 225c 3122 2c20  (.*)`$", r"\1", 
-00001bc0: 636f 6465 290d 0a0d 0a20 2020 2020 2020  code)....       
-00001bd0: 2023 2052 656d 6f76 6520 616e 7920 696e   # Remove any in
-00001be0: 7374 616e 6365 7320 6f66 2022 6466 203d  stances of "df =
-00001bf0: 2070 642e 7265 6164 5f63 7376 2827 6669   pd.read_csv('fi
-00001c00: 6c65 6e61 6d65 2e63 7376 2729 2220 6672  lename.csv')" fr
-00001c10: 6f6d 2074 6865 2063 6f64 650d 0a20 2020  om the code..   
-00001c20: 2020 2020 2063 6f64 6520 3d20 7265 2e73       code = re.s
-00001c30: 7562 2872 2264 665c 732a 3d5c 732a 7064  ub(r"df\s*=\s*pd
-00001c40: 5c2e 7265 6164 5f63 7376 5c28 272e 2a3f  \.read_csv\('.*?
-00001c50: 2728 2c2e 2a29 3f5c 2922 2c20 2222 2c20  '(,.*)?\)", "", 
-00001c60: 636f 6465 290d 0a0d 0a20 2020 2020 2020  code)....       
-00001c70: 2023 2044 6566 696e 6520 7468 6520 7265   # Define the re
-00001c80: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
-00001c90: 2070 6174 7465 726e 2074 6f20 6d61 7463   pattern to matc
-00001ca0: 6820 7468 6520 626c 6163 6b6c 6973 7420  h the blacklist 
-00001cb0: 6974 656d 730d 0a20 2020 2020 2020 2070  items..        p
-00001cc0: 6174 7465 726e 203d 2072 225e 282e 2a5c  attern = r"^(.*\
-00001cd0: 6228 2220 2b20 227c 222e 6a6f 696e 2862  b(" + "|".join(b
-00001ce0: 6c61 636b 6c69 7374 2920 2b20 7222 295c  lacklist) + r")\
-00001cf0: 622e 2a29 2422 0d0a 0d0a 2020 2020 2020  b.*)$"....      
-00001d00: 2020 2320 5265 706c 6163 6520 7468 6520    # Replace the 
-00001d10: 626c 6163 6b6c 6973 7420 6974 656d 7320  blacklist items 
-00001d20: 7769 7468 2063 6f6d 6d65 6e74 730d 0a20  with comments.. 
-00001d30: 2020 2020 2020 2063 6f64 6520 3d20 7265         code = re
-00001d40: 2e73 7562 2870 6174 7465 726e 2c20 7222  .sub(pattern, r"
-00001d50: 2320 6e6f 7420 616c 6c6f 7765 6420 5c31  # not allowed \1
-00001d60: 222c 2063 6f64 652c 2066 6c61 6773 3d72  ", code, flags=r
-00001d70: 652e 4d55 4c54 494c 494e 4529 0d0a 0d0a  e.MULTILINE)....
-00001d80: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-00001d90: 2074 6865 2063 6c65 616e 6564 2061 6e64   the cleaned and
-00001da0: 2065 7874 7261 6374 6564 2063 6f64 650d   extracted code.
-00001db0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001dc0: 636f 6465 2e73 7472 6970 2829 0d0a 2020  code.strip()..  
-00001dd0: 2020 0d0a 2020 2020 6465 6620 5f65 7874    ..    def _ext
-00001de0: 7261 6374 5f72 616e 6b28 7365 6c66 2c72  ract_rank(self,r
-00001df0: 6573 706f 6e73 653a 2073 7472 2920 2d3e  esponse: str) ->
-00001e00: 2073 7472 3a0d 0a0d 0a20 2020 2020 2020   str:....       
-00001e10: 2023 2053 6561 7263 6820 666f 7220 6120   # Search for a 
-00001e20: 7061 7474 6572 6e20 6265 7477 6565 6e20  pattern between 
-00001e30: 3c72 616e 6b3e 2061 6e64 203c 2f72 616e  <rank> and </ran
-00001e40: 6b3e 2069 6e20 7468 6520 7265 7370 6f6e  k> in the respon
-00001e50: 7365 0d0a 2020 2020 2020 2020 6d61 7463  se..        matc
-00001e60: 6820 3d20 7265 2e73 6561 7263 6828 7222  h = re.search(r"
-00001e70: 3c72 616e 6b3e 282e 2a29 3c2f 7261 6e6b  <rank>(.*)</rank
-00001e80: 3e22 2c20 7265 7370 6f6e 7365 290d 0a20  >", response).. 
-00001e90: 2020 2020 2020 2069 6620 6d61 7463 683a         if match:
-00001ea0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00001eb0: 4966 2061 206d 6174 6368 2069 7320 666f  If a match is fo
-00001ec0: 756e 642c 2065 7874 7261 6374 2074 6865  und, extract the
-00001ed0: 2072 616e 6b20 6265 7477 6565 6e20 3c72   rank between <r
-00001ee0: 616e 6b3e 2061 6e64 203c 2f72 616e 6b3e  ank> and </rank>
-00001ef0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00001f00: 6e6b 203d 206d 6174 6368 2e67 726f 7570  nk = match.group
-00001f10: 2831 290d 0a20 2020 2020 2020 2065 6c73  (1)..        els
-00001f20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001f30: 7261 6e6b 203d 2022 220d 0a0d 0a20 2020  rank = ""....   
-00001f40: 2020 2020 2023 2052 6574 7572 6e20 7468       # Return th
-00001f50: 6520 636c 6561 6e65 6420 616e 6420 6578  e cleaned and ex
-00001f60: 7472 6163 7465 6420 636f 6465 0d0a 2020  tracted code..  
-00001f70: 2020 2020 2020 7265 7475 726e 2072 616e        return ran
-00001f80: 6b2e 7374 7269 7028 290d 0a20 2020 200d  k.strip()..    .
-00001f90: 0a20 2020 2064 6566 2074 6173 6b5f 6576  .    def task_ev
-00001fa0: 616c 2873 656c 662c 2065 7661 6c5f 6d65  al(self, eval_me
-00001fb0: 7373 6167 6573 293a 0d0a 0d0a 2020 2020  ssages):....    
-00001fc0: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
-00001fd0: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
-00001fe0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00001ff0: 2320 4a75 7079 7465 7220 6e6f 7465 626f  # Jupyter notebo
-00002000: 6f6b 206f 7220 6970 7974 686f 6e0d 0a20  ok or ipython.. 
-00002010: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00002020: 6179 2848 544d 4c28 6627 3c70 2073 7479  ay(HTML(f'<p sty
-00002030: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
-00002040: 613b 223e 5c6e 4361 6c6c 696e 6720 4d6f  a;">\nCalling Mo
-00002050: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 5f66  del: {self.llm_f
-00002060: 756e 637d 3c2f 703e 2729 290d 0a20 2020  unc}</p>'))..   
-00002070: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00002080: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
-00002090: 796c 653d 2263 6f6c 6f72 3a6d 6167 656e  yle="color:magen
-000020a0: 7461 3b22 3e54 7279 696e 6720 746f 2064  ta;">Trying to d
-000020b0: 6574 6572 6d69 6e65 2074 6865 2062 6573  etermine the bes
-000020c0: 7420 6d65 7468 6f64 2074 6f20 616e 7377  t method to answ
-000020d0: 6572 2079 6f75 7220 7175 6573 7469 6f6e  er your question
-000020e0: 2c20 706c 6561 7365 2077 6169 742e 2e2e  , please wait...
-000020f0: 3c2f 623e 3c2f 703e 3c62 723e 2729 290d  </b></p><br>')).
-00002100: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00002110: 2020 2020 2020 2020 2020 2020 2320 4f74              # Ot
-00002120: 6865 7220 656e 7669 726f 6e6d 656e 7420  her environment 
-00002130: 286c 696b 6520 7465 726d 696e 616c 290d  (like terminal).
-00002140: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00002150: 6e74 2863 6f6c 6f72 6564 2866 225c 6e3e  nt(colored(f"\n>
-00002160: 3e20 4361 6c6c 696e 6720 4d6f 6465 6c3a  > Calling Model:
-00002170: 207b 7365 6c66 2e6c 6c6d 5f66 756e 637d   {self.llm_func}
-00002180: 222c 2022 6d61 6765 6e74 6122 2929 0d0a  ", "magenta"))..
-00002190: 2020 2020 2020 2020 2020 2020 6370 7269              cpri
-000021a0: 6e74 2866 225c 6e3e 3e20 5472 7969 6e67  nt(f"\n>> Trying
-000021b0: 2074 6f20 6465 7465 726d 696e 6520 7468   to determine th
-000021c0: 6520 6265 7374 206d 6574 686f 6420 746f  e best method to
-000021d0: 2061 6e73 7765 7220 796f 7572 2071 7565   answer your que
-000021e0: 7374 696f 6e2c 2070 6c65 6173 6520 7761  stion, please wa
-000021f0: 6974 2e2e 2e5c 6e22 2c20 276d 6167 656e  it...\n", 'magen
-00002200: 7461 272c 2061 7474 7273 3d5b 2762 6f6c  ta', attrs=['bol
-00002210: 6427 5d29 0d0a 0d0a 2020 2020 2020 2020  d'])....        
-00002220: 2320 4361 6c6c 204f 7065 6e41 4920 4150  # Call OpenAI AP
-00002230: 490d 0a20 2020 2020 2020 2066 756e 6374  I..        funct
-00002240: 696f 6e5f 6e61 6d65 203d 207b 226e 616d  ion_name = {"nam
-00002250: 6522 3a20 2251 415f 5265 7370 6f6e 7365  e": "QA_Response
-00002260: 227d 0d0a 2020 2020 2020 2020 666e 5f6e  "}..        fn_n
-00002270: 616d 652c 2061 7267 756d 656e 7473 2c20  ame, arguments, 
-00002280: 746f 6b65 6e73 5f75 7365 6420 3d20 7365  tokens_used = se
-00002290: 6c66 2e6c 6c6d 5f66 756e 635f 6361 6c6c  lf.llm_func_call
-000022a0: 2865 7661 6c5f 6d65 7373 6167 6573 2c73  (eval_messages,s
-000022b0: 656c 662e 7461 736b 5f65 7661 6c5f 6675  elf.task_eval_fu
-000022c0: 6e63 7469 6f6e 2c20 6675 6e63 7469 6f6e  nction, function
-000022d0: 5f6e 616d 6529 0d0a 0d0a 2020 2020 2020  _name)....      
-000022e0: 2020 2320 5061 7273 6520 7468 6520 4a53    # Parse the JS
-000022f0: 4f4e 2073 7472 696e 6720 746f 2061 2050  ON string to a P
-00002300: 7974 686f 6e20 6469 6374 0d0a 2020 2020  ython dict..    
-00002310: 2020 2020 6172 6775 6d65 6e74 735f 6469      arguments_di
-00002320: 6374 203d 206a 736f 6e2e 6c6f 6164 7328  ct = json.loads(
-00002330: 6172 6775 6d65 6e74 732c 2073 7472 6963  arguments, stric
-00002340: 743d 4661 6c73 6529 0d0a 0d0a 2020 2020  t=False)....    
-00002350: 2020 2020 2320 5265 7472 6965 7665 2076      # Retrieve v
-00002360: 616c 7565 730d 0a20 2020 2020 2020 2065  alues..        e
-00002370: 7661 6c5f 616e 7377 6572 203d 2061 7267  val_answer = arg
-00002380: 756d 656e 7473 5f64 6963 745b 2261 6e73  uments_dict["ans
-00002390: 7765 7222 5d0d 0a20 2020 2020 2020 2065  wer"]..        e
-000023a0: 7661 6c5f 616e 7377 6572 5f74 7970 6520  val_answer_type 
-000023b0: 3d20 6172 6775 6d65 6e74 735f 6469 6374  = arguments_dict
-000023c0: 5b22 616e 7377 6572 5f74 7970 6522 5d0d  ["answer_type"].
-000023d0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-000023e0: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-000023f0: 642e 6170 7065 6e64 2874 6f6b 656e 735f  d.append(tokens_
-00002400: 7573 6564 290d 0a0d 0a20 2020 2020 2020  used)....       
-00002410: 2072 6574 7572 6e20 6172 6775 6d65 6e74   return argument
-00002420: 732c 2066 6e5f 6e61 6d65 2c20 6576 616c  s, fn_name, eval
-00002430: 5f61 6e73 7765 722c 2065 7661 6c5f 616e  _answer, eval_an
-00002440: 7377 6572 5f74 7970 650d 0a0d 0a20 2020  swer_type....   
-00002450: 2064 6566 2064 6562 7567 5f63 6f64 6528   def debug_code(
-00002460: 7365 6c66 2c63 6f64 652c 7175 6573 7469  self,code,questi
-00002470: 6f6e 2c20 6c6c 6d5f 6361 7363 6164 653d  on, llm_cascade=
-00002480: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
-00002490: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-000024a0: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
-000024b0: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
-000024c0: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
-000024d0: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
-000024e0: 0d0a 2020 2020 2020 2020 6465 6275 675f  ..        debug_
-000024f0: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
-00002500: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
-00002510: 636f 6e74 656e 7422 3a20 7365 6c66 2e64  content": self.d
-00002520: 6562 7567 5f63 6f64 655f 7461 736b 2e66  ebug_code_task.f
-00002530: 6f72 6d61 7428 636f 6465 2c71 7565 7374  ormat(code,quest
-00002540: 696f 6e29 7d5d 0d0a 0d0a 2020 2020 2020  ion)}]....      
-00002550: 2020 7573 696e 675f 6d6f 6465 6c20 3d20    using_model = 
-00002560: 7365 6c66 2e6c 6c6d 0d0a 2020 2020 2020  self.llm..      
-00002570: 2020 6966 206c 6c6d 5f63 6173 6361 6465    if llm_cascade
-00002580: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
-00002590: 7369 6e67 5f6d 6f64 656c 203d 2073 656c  sing_model = sel
-000025a0: 662e 6c6c 6d5f 6770 7434 0d0a 0d0a 2020  f.llm_gpt4....  
-000025b0: 2020 2020 2020 6966 2027 6970 796b 6572        if 'ipyker
-000025c0: 6e65 6c27 2069 6e20 7379 732e 6d6f 6475  nel' in sys.modu
-000025d0: 6c65 733a 0d0a 2020 2020 2020 2020 2020  les:..          
-000025e0: 2020 2320 4a75 7079 7465 7220 6e6f 7465    # Jupyter note
-000025f0: 626f 6f6b 206f 7220 6970 7974 686f 6e0d  book or ipython.
-00002600: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00002610: 706c 6179 2848 544d 4c28 6627 3c70 2073  play(HTML(f'<p s
-00002620: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
-00002630: 6e74 613b 223e 5c6e 4361 6c6c 696e 6720  nta;">\nCalling 
-00002640: 4d6f 6465 6c3a 207b 7573 696e 675f 6d6f  Model: {using_mo
-00002650: 6465 6c7d 3c2f 703e 2729 290d 0a20 2020  del}</p>'))..   
-00002660: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00002670: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
-00002680: 796c 653d 2263 6f6c 6f72 3a6d 6167 656e  yle="color:magen
-00002690: 7461 3b22 3e49 2068 6176 6520 7265 6365  ta;">I have rece
-000026a0: 6976 6564 2074 6865 2066 6972 7374 2076  ived the first v
-000026b0: 6572 7369 6f6e 206f 6620 7468 6520 636f  ersion of the co
-000026c0: 6465 2e20 4920 616d 2073 656e 6469 6e67  de. I am sending
-000026d0: 2069 7420 6261 636b 2074 6f20 4c4c 4d20   it back to LLM 
-000026e0: 746f 2067 6574 2069 7420 6368 6563 6b65  to get it checke
-000026f0: 6420 666f 7220 616e 7920 6572 726f 7273  d for any errors
-00002700: 2c20 6275 6773 206f 7220 696e 636f 6e73  , bugs or incons
-00002710: 6973 7465 6e63 6965 732c 2061 6e64 2063  istencies, and c
-00002720: 6f72 7265 6374 696f 6e20 6966 206e 6563  orrection if nec
-00002730: 6573 7361 7279 2e20 506c 6561 7365 2077  essary. Please w
-00002740: 6169 742e 2e2e 3c2f 623e 3c2f 703e 3c62  ait...</b></p><b
-00002750: 723e 2729 290d 0a20 2020 2020 2020 2065  r>'))..        e
-00002760: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00002770: 2020 2320 4f74 6865 7220 656e 7669 726f    # Other enviro
-00002780: 6e6d 656e 7420 286c 696b 6520 7465 726d  nment (like term
-00002790: 696e 616c 290d 0a20 2020 2020 2020 2020  inal)..         
-000027a0: 2020 2070 7269 6e74 2863 6f6c 6f72 6564     print(colored
-000027b0: 2866 225c 6e3e 3e20 4361 6c6c 696e 6720  (f"\n>> Calling 
-000027c0: 4d6f 6465 6c3a 207b 7573 696e 675f 6d6f  Model: {using_mo
-000027d0: 6465 6c7d 222c 2022 6d61 6765 6e74 6122  del}", "magenta"
-000027e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000027f0: 6370 7269 6e74 2866 225c 6e3e 3e20 4920  cprint(f"\n>> I 
-00002800: 6861 7665 2072 6563 6569 7665 6420 7468  have received th
-00002810: 6520 6669 7273 7420 7665 7273 696f 6e20  e first version 
-00002820: 6f66 2074 6865 2063 6f64 652e 2049 2061  of the code. I a
-00002830: 6d20 7365 6e64 696e 6720 6974 2062 6163  m sending it bac
-00002840: 6b20 746f 204c 4c4d 2074 6f20 6765 7420  k to LLM to get 
-00002850: 6974 2063 6865 636b 6564 2066 6f72 2061  it checked for a
-00002860: 6e79 2065 7272 6f72 732c 2062 7567 7320  ny errors, bugs 
-00002870: 6f72 2069 6e63 6f6e 7369 7374 656e 6369  or inconsistenci
-00002880: 6573 2c20 616e 6420 636f 7272 6563 7469  es, and correcti
-00002890: 6f6e 2069 6620 6e65 6365 7373 6172 792e  on if necessary.
-000028a0: 2050 6c65 6173 6520 7761 6974 2e2e 2e5c   Please wait...\
-000028b0: 6e22 2c20 276d 6167 656e 7461 272c 2061  n", 'magenta', a
-000028c0: 7474 7273 3d5b 2762 6f6c 6427 5d29 0d0a  ttrs=['bold'])..
-000028d0: 0d0a 2020 2020 2020 2020 2320 4675 6e63  ..        # Func
-000028e0: 7469 6f6e 2074 6f20 6469 7370 6c61 7920  tion to display 
-000028f0: 7265 7375 6c74 7320 6e69 6365 6c79 0d0a  results nicely..
-00002900: 2020 2020 2020 2020 6465 6620 6469 7370          def disp
-00002910: 6c61 795f 7461 736b 2829 3a0d 0a20 2020  lay_task():..   
-00002920: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
-00002930: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
-00002940: 6f64 756c 6573 3a0d 0a20 2020 2020 2020  odules:..       
-00002950: 2020 2020 2020 2020 2023 204a 7570 7974           # Jupyt
-00002960: 6572 206e 6f74 6562 6f6f 6b20 6f72 2069  er notebook or i
-00002970: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
-00002980: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00002990: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
-000029a0: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
-000029b0: 613b 223e 4920 6861 7665 2066 696e 6973  a;">I have finis
-000029c0: 6865 6420 6465 6275 6767 696e 6720 7468  hed debugging th
-000029d0: 6520 636f 6465 2c20 616e 6420 7769 6c6c  e code, and will
-000029e0: 206e 6f77 2070 726f 6365 6564 2074 6f20   now proceed to 
-000029f0: 7468 6520 6578 6563 7574 696f 6e2e 2e2e  the execution...
-00002a00: 3c2f 623e 3c2f 703e 3c62 723e 2729 290d  </b></p><br>')).
-00002a10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00002a20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002a30: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
-00002a40: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
-00002a50: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
-00002a60: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-00002a70: 6622 5c6e 3e3e 2049 2068 6176 6520 6669  f"\n>> I have fi
-00002a80: 6e69 7368 6564 2064 6562 7567 6769 6e67  nished debugging
-00002a90: 2074 6865 2063 6f64 652c 2061 6e64 2077   the code, and w
-00002aa0: 696c 6c20 6e6f 7720 7072 6f63 6565 6420  ill now proceed 
-00002ab0: 746f 2074 6865 2065 7865 6375 7469 6f6e  to the execution
-00002ac0: 2e2e 2e5c 6e22 2c20 276d 6167 656e 7461  ...\n", 'magenta
-00002ad0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
-00002ae0: 5d29 0d0a 0d0a 2020 2020 2020 2020 2320  ])....        # 
-00002af0: 4361 6c6c 2074 6865 204f 7065 6e41 4920  Call the OpenAI 
-00002b00: 4150 490d 0a20 2020 2020 2020 206c 6c6d  API..        llm
-00002b10: 5f72 6573 706f 6e73 652c 2074 6f6b 656e  _response, token
-00002b20: 735f 7573 6564 203d 2073 656c 662e 6c6c  s_used = self.ll
-00002b30: 6d5f 6361 6c6c 2864 6562 7567 5f6d 6573  m_call(debug_mes
-00002b40: 7361 6765 732c 7465 6d70 6572 6174 7572  sages,temperatur
-00002b50: 653d 302c 6c6c 6d5f 6361 7363 6164 653d  e=0,llm_cascade=
-00002b60: 6c6c 6d5f 6361 7363 6164 6529 2023 2068  llm_cascade) # h
-00002b70: 6967 6865 7220 7465 6d70 6572 6174 7572  igher temperatur
-00002b80: 6520 7265 7375 6c74 7320 696e 206d 6f72  e results in mor
-00002b90: 6520 2263 7265 6174 6976 6522 2061 6e73  e "creative" ans
-00002ba0: 7765 7273 2028 736f 6d65 7469 6d65 7320  wers (sometimes 
-00002bb0: 746f 6f20 6372 6561 7469 7665 203a 2d29  too creative :-)
-00002bc0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00002bd0: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
-00002be0: 6865 2063 6f64 6520 6672 6f6d 2074 6865  he code from the
-00002bf0: 2041 5049 2072 6573 706f 6e73 650d 0a20   API response.. 
-00002c00: 2020 2020 2020 2064 6562 7567 6765 645f         debugged_
-00002c10: 636f 6465 203d 2073 656c 662e 5f65 7874  code = self._ext
-00002c20: 7261 6374 5f63 6f64 6528 6c6c 6d5f 7265  ract_code(llm_re
-00002c30: 7370 6f6e 7365 2920 2020 2020 2020 0d0a  sponse)       ..
-00002c40: 2020 2020 2020 2020 6469 7370 6c61 795f          display_
-00002c50: 7461 736b 2829 0d0a 0d0a 2020 2020 2020  task()....      
-00002c60: 2020 7365 6c66 2e74 6f74 616c 5f74 6f6b    self.total_tok
-00002c70: 656e 735f 7573 6564 2e61 7070 656e 6428  ens_used.append(
-00002c80: 746f 6b65 6e73 5f75 7365 6429 0d0a 0d0a  tokens_used)....
-00002c90: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00002ca0: 6562 7567 6765 645f 636f 6465 0d0a 0d0a  ebugged_code....
-00002cb0: 2020 2020 6465 6620 7261 6e6b 5f63 6f64      def rank_cod
-00002cc0: 6528 7365 6c66 2c63 6f64 652c 7175 6573  e(self,code,ques
-00002cd0: 7469 6f6e 2c6c 6c6d 5f63 6173 6361 6465  tion,llm_cascade
-00002ce0: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
-00002cf0: 2020 2320 496e 6974 6961 6c69 7a65 2074    # Initialize t
-00002d00: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
-00002d10: 2077 6974 6820 6120 7379 7374 656d 206d   with a system m
-00002d20: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
-00002d30: 6720 7468 6520 7461 736b 2070 726f 6d70  g the task promp
-00002d40: 740d 0a20 2020 2020 2020 2072 616e 6b5f  t..        rank_
-00002d50: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
-00002d60: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
-00002d70: 636f 6e74 656e 7422 3a20 7365 6c66 2e72  content": self.r
-00002d80: 616e 6b5f 616e 7377 6572 2e66 6f72 6d61  ank_answer.forma
-00002d90: 7428 636f 6465 2c71 7565 7374 696f 6e29  t(code,question)
-00002da0: 7d5d 0d0a 0d0a 2020 2020 2020 2020 7573  }]....        us
-00002db0: 696e 675f 6d6f 6465 6c20 3d20 7365 6c66  ing_model = self
-00002dc0: 2e6c 6c6d 0d0a 2020 2020 2020 2020 6966  .llm..        if
-00002dd0: 206c 6c6d 5f63 6173 6361 6465 3a0d 0a20   llm_cascade:.. 
-00002de0: 2020 2020 2020 2020 2020 2075 7369 6e67             using
-00002df0: 5f6d 6f64 656c 203d 2073 656c 662e 6c6c  _model = self.ll
-00002e00: 6d5f 6770 7434 0d0a 0d0a 2020 2020 2020  m_gpt4....      
-00002e10: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
-00002e20: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
-00002e30: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00002e40: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
-00002e50: 206f 7220 6970 7974 686f 6e0d 0a20 2020   or ipython..   
-00002e60: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00002e70: 2848 544d 4c28 6627 3c70 2073 7479 6c65  (HTML(f'<p style
-00002e80: 3d22 636f 6c6f 723a 6d61 6765 6e74 613b  ="color:magenta;
-00002e90: 223e 5c6e 4361 6c6c 696e 6720 4d6f 6465  ">\nCalling Mode
-00002ea0: 6c3a 207b 7573 696e 675f 6d6f 6465 6c7d  l: {using_model}
-00002eb0: 3c2f 703e 2729 290d 0a20 2020 2020 2020  </p>'))..       
-00002ec0: 2020 2020 2064 6973 706c 6179 2848 544d       display(HTM
-00002ed0: 4c28 6627 3c70 3e3c 6220 7374 796c 653d  L(f'<p><b style=
-00002ee0: 2263 6f6c 6f72 3a6d 6167 656e 7461 3b22  "color:magenta;"
-00002ef0: 3e49 2061 6d20 676f 696e 6720 746f 2065  >I am going to e
-00002f00: 7661 6c75 6174 6520 616e 6420 7261 6e6b  valuate and rank
-00002f10: 2074 6865 2061 6e73 7765 722e 2050 6c65   the answer. Ple
-00002f20: 6173 6520 7761 6974 2e2e 2e3c 2f62 3e3c  ase wait...</b><
-00002f30: 2f70 3e3c 6272 3e27 2929 0d0a 2020 2020  /p><br>'))..    
-00002f40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00002f50: 2020 2020 2020 2023 204f 7468 6572 2065         # Other e
-00002f60: 6e76 6972 6f6e 6d65 6e74 2028 6c69 6b65  nvironment (like
-00002f70: 2074 6572 6d69 6e61 6c29 0d0a 2020 2020   terminal)..    
-00002f80: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
-00002f90: 6c6f 7265 6428 6622 5c6e 3e3e 2043 616c  lored(f"\n>> Cal
-00002fa0: 6c69 6e67 204d 6f64 656c 3a20 7b75 7369  ling Model: {usi
-00002fb0: 6e67 5f6d 6f64 656c 7d22 2c20 226d 6167  ng_model}", "mag
-00002fc0: 656e 7461 2229 290d 0a20 2020 2020 2020  enta"))..       
-00002fd0: 2020 2020 2063 7072 696e 7428 6622 5c6e       cprint(f"\n
-00002fe0: 3e3e 2049 2061 6d20 676f 696e 6720 746f  >> I am going to
-00002ff0: 2065 7661 6c75 6174 6520 616e 6420 7261   evaluate and ra
-00003000: 6e6b 2074 6865 2061 6e73 7765 722e 2050  nk the answer. P
-00003010: 6c65 6173 6520 7761 6974 2e2e 5c6e 222c  lease wait..\n",
-00003020: 2027 6d61 6765 6e74 6127 2c20 6174 7472   'magenta', attr
-00003030: 733d 5b27 626f 6c64 275d 290d 0a0d 0a20  s=['bold']).... 
-00003040: 2020 2020 2020 2023 2043 616c 6c20 7468         # Call th
-00003050: 6520 4f70 656e 4149 2041 5049 200d 0a20  e OpenAI API .. 
-00003060: 2020 2020 2020 206c 6c6d 5f72 6573 706f         llm_respo
-00003070: 6e73 652c 2074 6f6b 656e 735f 7573 6564  nse, tokens_used
-00003080: 203d 2073 656c 662e 6c6c 6d5f 6361 6c6c   = self.llm_call
-00003090: 2872 616e 6b5f 6d65 7373 6167 6573 2c6c  (rank_messages,l
-000030a0: 6c6d 5f63 6173 6361 6465 3d6c 6c6d 5f63  lm_cascade=llm_c
-000030b0: 6173 6361 6465 290d 0a0d 0a20 2020 2020  ascade)....     
-000030c0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
-000030d0: 2063 6f64 6520 6672 6f6d 2074 6865 2041   code from the A
-000030e0: 5049 2072 6573 706f 6e73 650d 0a20 2020  PI response..   
-000030f0: 2020 2020 2072 616e 6b20 3d20 7365 6c66       rank = self
-00003100: 2e5f 6578 7472 6163 745f 7261 6e6b 286c  ._extract_rank(l
-00003110: 6c6d 5f72 6573 706f 6e73 6529 2020 2020  lm_response)    
-00003120: 2020 200d 0a0d 0a20 2020 2020 2020 2073     ....        s
-00003130: 656c 662e 746f 7461 6c5f 746f 6b65 6e73  elf.total_tokens
-00003140: 5f75 7365 642e 6170 7065 6e64 2874 6f6b  _used.append(tok
-00003150: 656e 735f 7573 6564 290d 0a0d 0a20 2020  ens_used)....   
-00003160: 2020 2020 2072 6574 7572 6e20 7261 6e6b       return rank
-00003170: 0d0a 0d0a 2020 2020 6465 6620 7064 5f61  ....    def pd_a
-00003180: 6765 6e74 5f63 6f6e 7665 7273 6528 7365  gent_converse(se
-00003190: 6c66 2c20 7175 6573 7469 6f6e 3d4e 6f6e  lf, question=Non
-000031a0: 6529 3a0d 0a20 2020 2020 2020 2023 2046  e):..        # F
-000031b0: 756e 6374 696f 6e73 2074 6f20 6469 7370  unctions to disp
-000031c0: 6c61 7920 7265 7375 6c74 7320 6e69 6365  lay results nice
-000031d0: 6c79 0d0a 2020 2020 2020 2020 6465 6620  ly..        def 
-000031e0: 6469 7370 6c61 795f 7265 7375 6c74 7328  display_results(
-000031f0: 616e 7377 6572 2c20 636f 6465 2c20 7261  answer, code, ra
-00003200: 6e6b 2c20 746f 7461 6c5f 746f 6b65 6e73  nk, total_tokens
-00003210: 5f75 7365 645f 7375 6d29 3a0d 0a20 2020  _used_sum):..   
-00003220: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
-00003230: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
-00003240: 6f64 756c 6573 3a20 2020 2020 0d0a 2020  odules:     ..  
-00003250: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003260: 2061 6e73 7765 7220 6973 206e 6f74 204e   answer is not N
-00003270: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00003280: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
-00003290: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
-000032a0: 7479 6c65 3d22 636f 6c6f 723a 626c 7565  tyle="color:blue
-000032b0: 3b22 3e49 206e 6f77 2068 6176 6520 7468  ;">I now have th
-000032c0: 6520 6669 6e61 6c20 616e 7377 6572 3a3c  e final answer:<
-000032d0: 2f62 3e3c 6272 3e3c 7072 6520 7374 796c  /b><br><pre styl
-000032e0: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b20  e="color:black; 
-000032f0: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
-00003300: 2d77 7261 703b 2066 6f6e 742d 7765 6967  -wrap; font-weig
-00003310: 6874 3a20 626f 6c64 3b22 3e7b 616e 7377  ht: bold;">{answ
-00003320: 6572 7d3c 2f70 7265 3e3c 2f70 3e3c 6272  er}</pre></p><br
-00003330: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
-00003340: 2020 2020 2020 6966 2063 6f64 6520 6973        if code is
-00003350: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003370: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
-00003380: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
-00003390: 723a 626c 7565 3b22 3e48 6572 6520 6973  r:blue;">Here is
-000033a0: 2074 6865 2066 696e 616c 2063 6f64 6520   the final code 
-000033b0: 7468 6174 2061 6363 6f6d 706c 6973 6865  that accomplishe
-000033c0: 7320 7468 6520 7461 736b 3a3c 2f62 3e3c  s the task:</b><
-000033d0: 6272 3e3c 7072 6520 7374 796c 653d 2263  br><pre style="c
-000033e0: 6f6c 6f72 3a23 3535 3535 3535 3b22 3e7b  olor:#555555;">{
-000033f0: 636f 6465 7d3c 2f70 7265 3e3c 2f70 3e3c  code}</pre></p><
-00003400: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
-00003410: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003420: 7261 6e6b 2061 6e64 2072 616e 6b20 6973  rank and rank is
-00003430: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003450: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
-00003460: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
-00003470: 723a 626c 7565 3b22 3e52 616e 6b3a 3c2f  r:blue;">Rank:</
-00003480: 623e 3c62 723e 3c73 7061 6e20 7374 796c  b><br><span styl
-00003490: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b22  e="color:black;"
-000034a0: 3e7b 7261 6e6b 7d3c 2f73 7061 6e3e 3c2f  >{rank}</span></
-000034b0: 703e 3c62 723e 2729 290d 0a20 2020 2020  p><br>'))..     
-000034c0: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-000034d0: 6179 2848 544d 4c28 6627 3c70 3e3c 6220  ay(HTML(f'<p><b 
-000034e0: 7374 796c 653d 2263 6f6c 6f72 3a62 6c75  style="color:blu
-000034f0: 653b 223e 546f 7461 6c20 546f 6b65 6e73  e;">Total Tokens
-00003500: 2055 7365 643a 3c2f 623e 3c62 723e 3c73   Used:</b><br><s
-00003510: 7061 6e20 7374 796c 653d 2263 6f6c 6f72  pan style="color
-00003520: 3a62 6c61 636b 3b22 3e7b 746f 7461 6c5f  :black;">{total_
-00003530: 746f 6b65 6e73 5f75 7365 645f 7375 6d7d  tokens_used_sum}
-00003540: 3c2f 7370 616e 3e3c 2f70 3e3c 6272 3e27  </span></p><br>'
-00003550: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00003560: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00003570: 2020 2020 2020 2069 6620 616e 7377 6572         if answer
-00003580: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 2020 2063 7072 696e 7428 6622 5c6e 3e3e     cprint(f"\n>>
-000035b0: 2049 206e 6f77 2068 6176 6520 7468 6520   I now have the 
-000035c0: 6669 6e61 6c20 616e 7377 6572 3a5c 6e7b  final answer:\n{
-000035d0: 616e 7377 6572 7d5c 6e22 2c20 2767 7265  answer}\n", 'gre
-000035e0: 656e 272c 2061 7474 7273 3d5b 2762 6f6c  en', attrs=['bol
-000035f0: 6427 5d29 0d0a 2020 2020 2020 2020 2020  d'])..          
-00003600: 2020 2020 2020 6966 2063 6f64 6520 6973        if code is
-00003610: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 6370 7269 6e74 2866 223e 3e20 4865 7265  cprint(f">> Here
-00003640: 2069 7320 7468 6520 6669 6e61 6c20 636f   is the final co
-00003650: 6465 2074 6861 7420 6163 636f 6d70 6c69  de that accompli
-00003660: 7368 6573 2074 6865 2074 6173 6b3a 5c6e  shes the task:\n
-00003670: 7b63 6f64 657d 5c6e 222c 2027 6772 6565  {code}\n", 'gree
-00003680: 6e27 2c20 6174 7472 733d 5b27 626f 6c64  n', attrs=['bold
-00003690: 275d 290d 0a20 2020 2020 2020 2020 2020  '])..           
-000036a0: 2020 2020 2069 6620 7365 6c66 2e72 616e       if self.ran
-000036b0: 6b20 616e 6420 7261 6e6b 2069 7320 6e6f  k and rank is no
-000036c0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000036d0: 2020 2020 2020 2020 2020 2020 2063 7072               cpr
-000036e0: 696e 7428 6622 3e3e 2052 616e 6b3a 5c6e  int(f">> Rank:\n
-000036f0: 7b72 616e 6b7d 5c6e 222c 2027 6772 6565  {rank}\n", 'gree
-00003700: 6e27 2c20 6174 7472 733d 5b27 626f 6c64  n', attrs=['bold
-00003710: 275d 290d 0a20 2020 2020 2020 2020 2020  '])..           
-00003720: 2020 2020 2063 7072 696e 7428 6622 3e3e       cprint(f">>
-00003730: 2054 6f74 616c 2074 6f6b 656e 7320 7573   Total tokens us
-00003740: 6564 3a5c 6e7b 746f 7461 6c5f 746f 6b65  ed:\n{total_toke
-00003750: 6e73 5f75 7365 645f 7375 6d7d 5c6e 222c  ns_used_sum}\n",
-00003760: 2027 7965 6c6c 6f77 272c 2061 7474 7273   'yellow', attrs
-00003770: 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a 2020  =['bold'])....  
-00003780: 2020 2020 2020 6465 6620 6469 7370 6c61        def displa
-00003790: 795f 6576 616c 2874 6173 6b5f 6576 616c  y_eval(task_eval
-000037a0: 2c20 7469 746c 652c 2074 6f74 616c 5f74  , title, total_t
-000037b0: 6f6b 656e 735f 7573 6564 5f73 756d 293a  okens_used_sum):
-000037c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000037d0: 2027 6970 796b 6572 6e65 6c27 2069 6e20   'ipykernel' in 
-000037e0: 7379 732e 6d6f 6475 6c65 733a 0d0a 2020  sys.modules:..  
-000037f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003800: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
-00003810: 206f 7220 6970 7974 686f 6e0d 0a20 2020   or ipython..   
-00003820: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00003830: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
-00003840: 6220 7374 796c 653d 2263 6f6c 6f72 3a62  b style="color:b
-00003850: 6c75 653b 223e 7b74 6974 6c65 7d3c 2f62  lue;">{title}</b
-00003860: 3e3c 6272 3e3c 7072 6520 7374 796c 653d  ><br><pre style=
-00003870: 2263 6f6c 6f72 3a62 6c61 636b 3b20 7768  "color:black; wh
-00003880: 6974 652d 7370 6163 653a 2070 7265 2d77  ite-space: pre-w
-00003890: 7261 703b 2066 6f6e 742d 7765 6967 6874  rap; font-weight
-000038a0: 3a20 626f 6c64 3b22 3e7b 7461 736b 5f65  : bold;">{task_e
-000038b0: 7661 6c7d 3c2f 7072 653e 3c2f 703e 3c62  val}</pre></p><b
-000038c0: 723e 2729 290d 0a20 2020 2020 2020 2020  r>'))..         
-000038d0: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-000038e0: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-000038f0: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
-00003900: 546f 7461 6c20 546f 6b65 6e73 2055 7365  Total Tokens Use
-00003910: 643a 3c2f 623e 3c62 723e 3c73 7061 6e20  d:</b><br><span 
-00003920: 7374 796c 653d 2263 6f6c 6f72 3a62 6c61  style="color:bla
-00003930: 636b 3b22 3e7b 746f 7461 6c5f 746f 6b65  ck;">{total_toke
-00003940: 6e73 5f75 7365 645f 7375 6d7d 3c2f 7370  ns_used_sum}</sp
-00003950: 616e 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  an></p><br>'))..
-00003960: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00003970: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003980: 2020 2023 204f 7468 6572 2065 6e76 6972     # Other envir
-00003990: 6f6e 6d65 6e74 2028 6c69 6b65 2074 6572  onment (like ter
-000039a0: 6d69 6e61 6c29 0d0a 2020 2020 2020 2020  minal)..        
-000039b0: 2020 2020 2020 2020 6370 7269 6e74 2866          cprint(f
-000039c0: 225c 6e3e 3e20 7b74 6974 6c65 7d5c 6e7b  "\n>> {title}\n{
-000039d0: 7461 736b 5f65 7661 6c7d 5c6e 222c 2027  task_eval}\n", '
-000039e0: 6d61 6765 6e74 6127 2c20 6174 7472 733d  magenta', attrs=
-000039f0: 5b27 626f 6c64 275d 290d 0a20 2020 2020  ['bold'])..     
-00003a00: 2020 2020 2020 2020 2020 2063 7072 696e             cprin
-00003a10: 7428 6622 3e3e 2054 6f74 616c 2074 6f6b  t(f">> Total tok
-00003a20: 656e 7320 7573 6564 3a5c 6e7b 746f 7461  ens used:\n{tota
-00003a30: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
-00003a40: 6d7d 5c6e 222c 2027 7965 6c6c 6f77 272c  m}\n", 'yellow',
-00003a50: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
-00003a60: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00003a70: 2020 2020 2320 4966 2061 2071 7565 7374      # If a quest
-00003a80: 696f 6e20 6973 2070 726f 7669 6465 642c  ion is provided,
-00003a90: 2073 6b69 7020 7468 6520 696e 7075 7420   skip the input 
-00003aa0: 7072 6f6d 7074 0d0a 2020 2020 2020 2020  prompt..        
-00003ab0: 6966 2071 7565 7374 696f 6e20 6973 206e  if question is n
-00003ac0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00003ad0: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
-00003ae0: 7a65 2074 6865 206d 6573 7361 6765 7320  ze the messages 
-00003af0: 6c69 7374 2077 6974 6820 6120 7379 7374  list with a syst
-00003b00: 656d 206d 6573 7361 6765 2063 6f6e 7461  em message conta
-00003b10: 696e 696e 6720 7468 6520 7461 736b 2070  ining the task p
-00003b20: 726f 6d70 740d 0a20 2020 2020 2020 2020  rompt..         
-00003b30: 2020 206d 6573 7361 6765 7320 3d20 5b7b     messages = [{
-00003b40: 2272 6f6c 6522 3a20 2273 7973 7465 6d22  "role": "system"
-00003b50: 2c20 2263 6f6e 7465 6e74 223a 2073 656c  , "content": sel
-00003b60: 662e 7379 7374 656d 5f74 6173 6b2e 666f  f.system_task.fo
-00003b70: 726d 6174 2871 7565 7374 696f 6e29 7d5d  rmat(question)}]
-00003b80: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00003b90: 496e 6974 6961 6c69 7a65 2074 6865 206d  Initialize the m
-00003ba0: 6573 7361 6765 7320 6c69 7374 2077 6974  essages list wit
-00003bb0: 6820 6120 7379 7374 656d 206d 6573 7361  h a system messa
-00003bc0: 6765 2063 6f6e 7461 696e 696e 6720 7468  ge containing th
-00003bd0: 6520 7461 736b 2070 726f 6d70 740d 0a20  e task prompt.. 
-00003be0: 2020 2020 2020 2020 2020 2065 7661 6c5f             eval_
-00003bf0: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
-00003c00: 6c65 223a 2022 7573 6572 222c 2022 636f  le": "user", "co
-00003c10: 6e74 656e 7422 3a20 7365 6c66 2e74 6173  ntent": self.tas
-00003c20: 6b5f 6576 616c 7561 7469 6f6e 2e66 6f72  k_evaluation.for
-00003c30: 6d61 7428 7175 6573 7469 6f6e 2c20 7365  mat(question, se
-00003c40: 6c66 2e64 665f 6865 6164 297d 5d0d 0a0d  lf.df_head)}]...
-00003c50: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-00003c60: 616c 6c20 7468 6520 7461 736b 5f65 7661  all the task_eva
-00003c70: 6c20 6d65 7468 6f64 2077 6974 6820 7468  l method with th
-00003c80: 6520 7573 6572 2773 2071 7565 7374 696f  e user's questio
-00003c90: 6e20 6966 2074 6865 2065 7870 6c6f 7261  n if the explora
-00003ca0: 746f 7279 206d 6f64 6520 6973 2054 7275  tory mode is Tru
-00003cb0: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00003cc0: 6620 7365 6c66 2e65 7870 6c6f 7261 746f  f self.explorato
-00003cd0: 7279 2069 7320 5472 7565 3a0d 0a20 2020  ry is True:..   
-00003ce0: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00003cf0: 756d 656e 7473 2c20 666e 5f6e 616d 652c  uments, fn_name,
-00003d00: 2074 6173 6b5f 6576 616c 2c20 7461 736b   task_eval, task
-00003d10: 5f74 7970 6520 3d20 7365 6c66 2e74 6173  _type = self.tas
-00003d20: 6b5f 6576 616c 2865 7661 6c5f 6d65 7373  k_eval(eval_mess
-00003d30: 6167 6573 290d 0a20 2020 2020 2020 2020  ages)..         
-00003d40: 2020 2020 2020 2074 6f74 616c 5f74 6f6b         total_tok
-00003d50: 656e 735f 7573 6564 5f73 756d 203d 2073  ens_used_sum = s
-00003d60: 756d 2873 656c 662e 746f 7461 6c5f 746f  um(self.total_to
-00003d70: 6b65 6e73 5f75 7365 6429 0d0a 2020 2020  kens_used)..    
-00003d80: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00003d90: 6173 6b5f 7479 7065 203d 3d20 276e 6172  ask_type == 'nar
-00003da0: 7261 7469 7665 273a 0d0a 2020 2020 2020  rative':..      
-00003db0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00003dc0: 746c 6520 3d20 2748 6572 6520 6973 2074  tle = 'Here is t
-00003dd0: 6865 2061 6e73 7765 7220 746f 2079 6f75  he answer to you
-00003de0: 7220 7175 6573 7469 6f6e 3a27 2020 2020  r question:'    
-00003df0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00003e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003e10: 2020 2020 2064 6973 706c 6179 5f65 7661       display_eva
-00003e20: 6c28 7461 736b 5f65 7661 6c2c 2074 6974  l(task_eval, tit
-00003e30: 6c65 2c20 746f 7461 6c5f 746f 6b65 6e73  le, total_tokens
-00003e40: 5f75 7365 645f 7375 6d29 0d0a 2020 2020  _used_sum)..    
-00003e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e60: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
-00003e70: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e90: 2020 2074 6974 6c65 203d 2027 4865 7265     title = 'Here
-00003ea0: 2069 7320 7468 6520 7365 7175 656e 6365   is the sequence
-00003eb0: 206f 6620 7374 6570 7320 7265 7175 6972   of steps requir
-00003ec0: 6564 2074 6f20 636f 6d70 6c65 7465 2074  ed to complete t
-00003ed0: 6865 2074 6173 6b3a 270d 0a20 2020 2020  he task:'..     
-00003ee0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00003ef0: 6173 6b20 3d20 7461 736b 5f65 7661 6c0d  ask = task_eval.
+000002d0: 206c 6c6d 5f31 366b 3a20 7374 7220 3d20   llm_16k: str = 
+000002e0: 2767 7074 2d33 2e35 2d74 7572 626f 2d31  'gpt-3.5-turbo-1
+000002f0: 366b 272c 0d0a 2020 2020 2020 2020 2020  6k',..          
+00000300: 2020 2020 2020 206c 6c6d 5f67 7074 343a         llm_gpt4:
+00000310: 2073 7472 203d 2027 6770 742d 342d 3036   str = 'gpt-4-06
+00000320: 3133 272c 0d0a 2020 2020 2020 2020 2020  13',..          
+00000330: 2020 2020 2020 2064 6562 7567 3a20 626f         debug: bo
+00000340: 6f6c 203d 2046 616c 7365 2c20 0d0a 2020  ol = False, ..  
+00000350: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00000360: 6563 746f 725f 6462 3a20 626f 6f6c 203d  ector_db: bool =
+00000370: 2046 616c 7365 2c20 0d0a 2020 2020 2020   False, ..      
+00000380: 2020 2020 2020 2020 2020 206c 6c6d 5f73             llm_s
+00000390: 7769 7463 683a 2062 6f6f 6c20 3d20 4661  witch: bool = Fa
+000003a0: 6c73 652c 200d 0a20 2020 2020 2020 2020  lse, ..         
+000003b0: 2020 2020 2020 2020 6578 706c 6f72 6174          explorat
+000003c0: 6f72 793a 2062 6f6f 6c20 3d20 5472 7565  ory: bool = True
+000003d0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+000003e0: 2020 2020 2029 3a0d 0a0d 0a20 2020 2020       ):....     
+000003f0: 2020 2073 656c 662e 4150 495f 4b45 5920     self.API_KEY 
+00000400: 3d20 6f73 2e65 6e76 6972 6f6e 2e67 6574  = os.environ.get
+00000410: 2827 4f50 454e 4149 5f41 5049 5f4b 4559  ('OPENAI_API_KEY
+00000420: 2729 0d0a 0d0a 2020 2020 2020 2020 2320  ')....        # 
+00000430: 4368 6563 6b20 6966 2074 6865 204f 5045  Check if the OPE
+00000440: 4e41 495f 4150 495f 4b45 5920 656e 7669  NAI_API_KEY envi
+00000450: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00000460: 2069 7320 7365 740d 0a20 2020 2020 2020   is set..       
+00000470: 2069 6620 6e6f 7420 7365 6c66 2e41 5049   if not self.API
+00000480: 5f4b 4559 3a0d 0a20 2020 2020 2020 2020  _KEY:..         
+00000490: 2020 2072 6169 7365 2045 6e76 6972 6f6e     raise Environ
+000004a0: 6d65 6e74 4572 726f 7228 224f 5045 4e41  mentError("OPENA
+000004b0: 495f 4150 495f 4b45 5920 656e 7669 726f  I_API_KEY enviro
+000004c0: 6e6d 656e 7420 7661 7269 6162 6c65 206e  nment variable n
+000004d0: 6f74 2066 6f75 6e64 2e22 290d 0a20 2020  ot found.")..   
+000004e0: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+000004f0: 2043 6865 636b 2069 6620 7468 6520 5049   Check if the PI
+00000500: 4e45 434f 4e45 5f41 5049 5f4b 4559 2061  NECONE_API_KEY a
+00000510: 6e64 2050 494e 4543 4f4e 455f 454e 5620  nd PINECONE_ENV 
+00000520: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00000530: 6162 6c65 7320 6172 6520 7365 7420 6966  ables are set if
+00000540: 2076 6563 746f 725f 6462 2069 7320 5472   vector_db is Tr
+00000550: 7565 0d0a 2020 2020 2020 2020 6966 2076  ue..        if v
+00000560: 6563 746f 725f 6462 3a0d 0a20 2020 2020  ector_db:..     
+00000570: 2020 2020 2020 2050 494e 4543 4f4e 455f         PINECONE_
+00000580: 4150 495f 4b45 5920 3d20 6f73 2e67 6574  API_KEY = os.get
+00000590: 656e 7628 2750 494e 4543 4f4e 455f 4150  env('PINECONE_AP
+000005a0: 495f 4b45 5927 290d 0a20 2020 2020 2020  I_KEY')..       
+000005b0: 2020 2020 2050 494e 4543 4f4e 455f 454e       PINECONE_EN
+000005c0: 5620 3d20 6f73 2e67 6574 656e 7628 2750  V = os.getenv('P
+000005d0: 494e 4543 4f4e 455f 454e 5627 290d 0a20  INECONE_ENV').. 
+000005e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000005f0: 2020 2020 2020 2020 2069 6620 5049 4e45           if PINE
+00000600: 434f 4e45 5f41 5049 5f4b 4559 2069 7320  CONE_API_KEY is 
+00000610: 4e6f 6e65 206f 7220 5049 4e45 434f 4e45  None or PINECONE
+00000620: 5f45 4e56 2069 7320 4e6f 6e65 3a0d 0a20  _ENV is None:.. 
+00000630: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00000640: 7269 6e74 2822 5761 726e 696e 673a 2050  rint("Warning: P
+00000650: 494e 4543 4f4e 455f 4150 495f 4b45 5920  INECONE_API_KEY 
+00000660: 6f72 2050 494e 4543 4f4e 455f 454e 5620  or PINECONE_ENV 
+00000670: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00000680: 6162 6c65 206e 6f74 2066 6f75 6e64 2e20  able not found. 
+00000690: 4469 7361 626c 696e 6720 7665 6374 6f72  Disabling vector
+000006a0: 5f64 622e 2229 0d0a 2020 2020 2020 2020  _db.")..        
+000006b0: 2020 2020 2020 2020 7665 6374 6f72 5f64          vector_d
+000006c0: 6220 3d20 4661 6c73 650d 0a0d 0a20 2020  b = False....   
+000006d0: 2020 2020 2073 656c 662e 4d41 585f 4552       self.MAX_ER
+000006e0: 524f 525f 434f 5252 4543 5449 4f4e 5320  ROR_CORRECTIONS 
+000006f0: 3d20 350d 0a20 2020 2020 2020 2023 2053  = 5..        # S
+00000700: 6574 2074 6865 206d 6178 696d 756d 206e  et the maximum n
+00000710: 756d 6265 7220 6f66 2071 7565 7374 696f  umber of questio
+00000720: 6e2f 616e 7377 6572 2070 6169 7273 2074  n/answer pairs t
+00000730: 6f20 6265 206b 6570 7420 696e 2074 6865  o be kept in the
+00000740: 2063 6f6e 7665 7273 6174 696f 6e20 6d65   conversation me
+00000750: 6d6d 6f72 790d 0a20 2020 2020 2020 2073  mmory..        s
+00000760: 656c 662e 4d41 585f 434f 4e56 4552 5341  elf.MAX_CONVERSA
+00000770: 5449 4f4e 5320 3d20 286d 6178 5f63 6f6e  TIONS = (max_con
+00000780: 7665 7273 6174 696f 6e73 2a32 2920 2d20  versations*2) - 
+00000790: 310d 0a20 2020 2020 2020 200d 0a20 2020  1..        ..   
+000007a0: 2020 2020 2023 2053 746f 7265 2074 6865       # Store the
+000007b0: 206f 7269 6769 6e61 6c20 6461 7461 6672   original datafr
+000007c0: 616d 652e 2054 6869 7320 7769 6c6c 2062  ame. This will b
+000007d0: 6520 7573 6564 2074 6f20 7265 7365 7420  e used to reset 
+000007e0: 7468 6520 6461 7461 6672 616d 6520 6265  the dataframe be
+000007f0: 666f 7265 2065 7865 6375 7469 6e67 2074  fore executing t
+00000800: 6865 2063 6f64 650d 0a20 2020 2020 2020  he code..       
+00000810: 2073 656c 662e 6f72 6967 696e 616c 5f64   self.original_d
+00000820: 6620 3d20 6466 0d0a 2020 2020 2020 2020  f = df..        
+00000830: 7365 6c66 2e64 6620 3d20 6466 2e63 6f70  self.df = df.cop
+00000840: 7928 2920 2023 206d 616b 6520 6120 636f  y()  # make a co
+00000850: 7079 206f 6620 7468 6520 6461 7461 6672  py of the datafr
+00000860: 616d 650d 0a20 2020 2020 2020 2073 656c  ame..        sel
+00000870: 662e 6466 5f68 6561 6420 3d20 7365 6c66  f.df_head = self
+00000880: 2e6f 7269 6769 6e61 6c5f 6466 2e68 6561  .original_df.hea
+00000890: 6428 3129 0d0a 2020 2020 2020 2020 7365  d(1)..        se
+000008a0: 6c66 2e64 665f 636f 6c75 6d6e 7320 3d20  lf.df_columns = 
+000008b0: 7365 6c66 2e64 662e 636f 6c75 6d6e 732e  self.df.columns.
+000008c0: 746f 6c69 7374 2829 0d0a 0d0a 2020 2020  tolist()....    
+000008d0: 2020 2020 2320 4c4c 4d73 0d0a 2020 2020      # LLMs..    
+000008e0: 2020 2020 7365 6c66 2e6c 6c6d 203d 206c      self.llm = l
+000008f0: 6c6d 0d0a 2020 2020 2020 2020 7365 6c66  lm..        self
+00000900: 2e6c 6c6d 5f66 756e 6320 3d20 6c6c 6d5f  .llm_func = llm_
+00000910: 6675 6e63 0d0a 2020 2020 2020 2020 7365  func..        se
+00000920: 6c66 2e6c 6c6d 5f31 366b 203d 206c 6c6d  lf.llm_16k = llm
+00000930: 5f31 366b 0d0a 2020 2020 2020 2020 7365  _16k..        se
+00000940: 6c66 2e6c 6c6d 5f67 7074 3420 3d20 6c6c  lf.llm_gpt4 = ll
+00000950: 6d5f 6770 7434 0d0a 0d0a 2020 2020 2020  m_gpt4....      
+00000960: 2020 2320 5365 7420 7468 6520 6465 6275    # Set the debu
+00000970: 6720 6d6f 6465 2e20 5468 6973 206d 6f64  g mode. This mod
+00000980: 6520 6973 2054 7275 6520 7768 656e 2079  e is True when y
+00000990: 6f75 2077 616e 7420 7468 6520 6d6f 6465  ou want the mode
+000009a0: 6c20 746f 2064 6562 7567 2074 6865 2063  l to debug the c
+000009b0: 6f64 6520 616e 6420 636f 7272 6563 7420  ode and correct 
+000009c0: 6974 2e0d 0a20 2020 2020 2020 2073 656c  it...        sel
+000009d0: 662e 6465 6275 6720 3d20 6465 6275 670d  f.debug = debug.
+000009e0: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
+000009f0: 6865 206c 6c6d 5f73 7769 7463 6820 6d6f  he llm_switch mo
+00000a00: 6465 2e20 5468 6973 206d 6f64 6520 6973  de. This mode is
+00000a10: 2054 7275 6520 7768 656e 2079 6f75 2077   True when you w
+00000a20: 616e 7420 7468 6520 6d6f 6465 6c20 746f  ant the model to
+00000a30: 2073 7769 7463 6820 746f 2067 7074 2d34   switch to gpt-4
+00000a40: 2066 6f72 2064 6562 7567 6769 6e67 2c20   for debugging, 
+00000a50: 6572 726f 7220 636f 7272 6563 7469 6f6e  error correction
+00000a60: 2061 6e64 2072 616e 6b69 6e67 2e0d 0a20   and ranking... 
+00000a70: 2020 2020 2020 2073 656c 662e 6c6c 6d5f         self.llm_
+00000a80: 7377 6974 6368 203d 206c 6c6d 5f73 7769  switch = llm_swi
+00000a90: 7463 680d 0a20 2020 2020 2020 2023 2053  tch..        # S
+00000aa0: 6574 2074 6865 2072 616e 6b20 6d6f 6465  et the rank mode
+00000ab0: 2e20 5468 6973 206d 6f64 6520 6973 2054  . This mode is T
+00000ac0: 7275 6520 7768 656e 2079 6f75 2077 616e  rue when you wan
+00000ad0: 7420 7468 6520 6d6f 6465 6c20 746f 2072  t the model to r
+00000ae0: 616e 6b20 7468 6520 6765 6e65 7261 7465  ank the generate
+00000af0: 6420 636f 6465 2e0d 0a20 2020 2020 2020  d code...       
+00000b00: 2073 656c 662e 7665 6374 6f72 5f64 6220   self.vector_db 
+00000b10: 3d20 7665 6374 6f72 5f64 620d 0a0d 0a20  = vector_db.... 
+00000b20: 2020 2020 2020 2023 2053 6574 2074 6865         # Set the
+00000b30: 2065 7870 6c6f 7261 746f 7279 206d 6f64   exploratory mod
+00000b40: 652e 2054 6869 7320 6d6f 6465 2069 7320  e. This mode is 
+00000b50: 5472 7565 2077 6865 6e20 796f 7520 7761  True when you wa
+00000b60: 6e74 2074 6865 206d 6f64 656c 2074 6f20  nt the model to 
+00000b70: 6576 616c 7561 7465 2074 6865 206f 7269  evaluate the ori
+00000b80: 6769 6e61 6c20 7072 6f6d 7074 2061 6e64  ginal prompt and
+00000b90: 2062 7265 616b 2069 7420 646f 776e 2069   break it down i
+00000ba0: 6e20 616c 676f 7269 7468 6d2e 0d0a 2020  n algorithm...  
+00000bb0: 2020 2020 2020 7365 6c66 2e65 7870 6c6f        self.explo
+00000bc0: 7261 746f 7279 203d 2065 7870 6c6f 7261  ratory = explora
+00000bd0: 746f 7279 0d0a 2020 2020 2020 2020 0d0a  tory..        ..
+00000be0: 2020 2020 2020 2020 2320 5072 6f6d 7074          # Prompt
+00000bf0: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+00000c00: 6465 6661 756c 745f 6578 616d 706c 655f  default_example_
+00000c10: 6f75 7470 7574 203d 2070 726f 6d70 7473  output = prompts
+00000c20: 2e65 7861 6d70 6c65 5f6f 7574 7075 740d  .example_output.
+00000c30: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00000c40: 736b 5f65 7661 6c75 6174 696f 6e20 3d20  sk_evaluation = 
+00000c50: 7072 6f6d 7074 732e 7461 736b 5f65 7661  prompts.task_eva
+00000c60: 6c75 6174 696f 6e0d 0a20 2020 2020 2020  luation..       
+00000c70: 2073 656c 662e 7379 7374 656d 5f74 6173   self.system_tas
+00000c80: 6b20 3d20 7072 6f6d 7074 732e 7379 7374  k = prompts.syst
+00000c90: 656d 5f74 6173 6b0d 0a20 2020 2020 2020  em_task..       
+00000ca0: 2073 656c 662e 7573 6572 5f74 6173 6b20   self.user_task 
+00000cb0: 3d20 7072 6f6d 7074 732e 7573 6572 5f74  = prompts.user_t
+00000cc0: 6173 6b0d 0a20 2020 2020 2020 2073 656c  ask..        sel
+00000cd0: 662e 6572 726f 725f 636f 7272 6563 745f  f.error_correct_
+00000ce0: 7461 736b 203d 2070 726f 6d70 7473 2e65  task = prompts.e
+00000cf0: 7272 6f72 5f63 6f72 7265 6374 5f74 6173  rror_correct_tas
+00000d00: 6b0d 0a20 2020 2020 2020 2073 656c 662e  k..        self.
+00000d10: 6465 6275 675f 636f 6465 5f74 6173 6b20  debug_code_task 
+00000d20: 3d20 7072 6f6d 7074 732e 6465 6275 675f  = prompts.debug_
+00000d30: 636f 6465 5f74 6173 6b20 200d 0a20 2020  code_task  ..   
+00000d40: 2020 2020 2073 656c 662e 7261 6e6b 5f61       self.rank_a
+00000d50: 6e73 7765 7220 3d20 7072 6f6d 7074 732e  nswer = prompts.
+00000d60: 7261 6e6b 5f61 6e73 7765 720d 0a20 2020  rank_answer..   
+00000d70: 2020 2020 2073 656c 662e 736f 6c75 7469       self.soluti
+00000d80: 6f6e 5f69 6e73 6967 6874 7320 3d20 7072  on_insights = pr
+00000d90: 6f6d 7074 732e 736f 6c75 7469 6f6e 5f69  ompts.solution_i
+00000da0: 6e73 6967 6874 730d 0a0d 0a20 2020 2020  nsights....     
+00000db0: 2020 2023 2046 756e 6374 696f 6e73 0d0a     # Functions..
+00000dc0: 2020 2020 2020 2020 7365 6c66 2e74 6173          self.tas
+00000dd0: 6b5f 6576 616c 5f66 756e 6374 696f 6e20  k_eval_function 
+00000de0: 3d20 6675 6e63 5f63 616c 6c73 2e74 6173  = func_calls.tas
+00000df0: 6b5f 6576 616c 5f66 756e 6374 696f 6e0d  k_eval_function.
+00000e00: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00000e10: 7369 6768 7473 5f66 756e 6374 696f 6e20  sights_function 
+00000e20: 3d20 6675 6e63 5f63 616c 6c73 2e73 6f6c  = func_calls.sol
+00000e30: 7574 696f 6e5f 696e 7369 6768 7473 5f66  ution_insights_f
+00000e40: 756e 6374 696f 6e0d 0a0d 0a20 2020 2020  unction....     
+00000e50: 2020 2023 2051 4120 5265 7472 6965 7661     # QA Retrieva
+00000e60: 6c0d 0a20 2020 2020 2020 2073 656c 662e  l..        self.
+00000e70: 6164 645f 7175 6573 7469 6f6e 5f61 6e73  add_question_ans
+00000e80: 7765 725f 7061 6972 203d 2071 615f 7265  wer_pair = qa_re
+00000e90: 7472 6965 7661 6c2e 6164 645f 7175 6573  trieval.add_ques
+00000ea0: 7469 6f6e 5f61 6e73 7765 725f 7061 6972  tion_answer_pair
+00000eb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+00000ec0: 6574 7269 6576 655f 616e 7377 6572 203d  etrieve_answer =
+00000ed0: 2071 615f 7265 7472 6965 7661 6c2e 7265   qa_retrieval.re
+00000ee0: 7472 6965 7665 5f61 6e73 7765 720d 0a20  trieve_answer.. 
+00000ef0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00000f00: 206f 7065 6e61 692e 6170 695f 6b65 7920   openai.api_key 
+00000f10: 3d20 7365 6c66 2e41 5049 5f4b 4559 0d0a  = self.API_KEY..
+00000f20: 0d0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
+00000f30: 6961 6c69 7a65 2074 6865 2074 6f74 616c  ialize the total
+00000f40: 2074 6f6b 656e 7320 7573 6564 206c 6973   tokens used lis
+00000f50: 742e 2054 6869 7320 6c69 7374 2077 696c  t. This list wil
+00000f60: 6c20 6265 2075 7365 6420 746f 206b 6565  l be used to kee
+00000f70: 7020 7472 6163 6b20 6f66 2074 6865 2074  p track of the t
+00000f80: 6f74 616c 2074 6f6b 656e 7320 7573 6564  otal tokens used
+00000f90: 2062 7920 7468 6520 6d6f 6465 6c0d 0a20   by the model.. 
+00000fa0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+00000fb0: 6c5f 746f 6b65 6e73 5f75 7365 6420 3d20  l_tokens_used = 
+00000fc0: 5b5d 0d0a 0d0a 2020 2020 6465 6620 6c6c  []....    def ll
+00000fd0: 6d5f 6361 6c6c 2873 656c 662c 206d 6573  m_call(self, mes
+00000fe0: 7361 6765 733a 2073 7472 2c20 7465 6d70  sages: str, temp
+00000ff0: 6572 6174 7572 653a 2066 6c6f 6174 203d  erature: float =
+00001000: 2030 2c20 6d61 785f 746f 6b65 6e73 3a20   0, max_tokens: 
+00001010: 696e 7420 3d20 3130 3030 2c20 6c6c 6d5f  int = 1000, llm_
+00001020: 6361 7363 6164 653a 2062 6f6f 6c20 3d20  cascade: bool = 
+00001030: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00001040: 206d 6f64 656c 203d 2073 656c 662e 6c6c   model = self.ll
+00001050: 6d0d 0a20 2020 2020 2020 2069 6620 6c6c  m..        if ll
+00001060: 6d5f 6361 7363 6164 653a 0d0a 2020 2020  m_cascade:..    
+00001070: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
+00001080: 7365 6c66 2e6c 6c6d 5f67 7074 340d 0a20  self.llm_gpt4.. 
+00001090: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+000010a0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+000010b0: 6520 3d20 6f70 656e 6169 2e43 6861 7443  e = openai.ChatC
+000010c0: 6f6d 706c 6574 696f 6e2e 6372 6561 7465  ompletion.create
+000010d0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000010e0: 2020 206d 6f64 656c 3d6d 6f64 656c 2c0d     model=model,.
+000010f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001100: 206d 6573 7361 6765 733d 6d65 7373 6167   messages=messag
+00001110: 6573 2c0d 0a20 2020 2020 2020 2020 2020  es,..           
+00001120: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
+00001130: 3d74 656d 7065 7261 7475 7265 2c0d 0a20  =temperature,.. 
+00001140: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00001150: 6178 5f74 6f6b 656e 733d 6d61 785f 746f  ax_tokens=max_to
+00001160: 6b65 6e73 2c0d 0a20 2020 2020 2020 2020  kens,..         
+00001170: 2020 2029 0d0a 2020 2020 2020 2020 6578     )..        ex
+00001180: 6365 7074 206f 7065 6e61 692e 6572 726f  cept openai.erro
+00001190: 722e 5261 7465 4c69 6d69 7445 7272 6f72  r.RateLimitError
+000011a0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+000011b0: 7269 6e74 280d 0a20 2020 2020 2020 2020  rint(..         
+000011c0: 2020 2020 2020 2022 5468 6520 4f70 656e         "The Open
+000011d0: 4149 2041 5049 2072 6174 6520 6c69 6d69  AI API rate limi
+000011e0: 7420 6861 7320 6265 656e 2065 7863 6565  t has been excee
+000011f0: 6465 642e 2057 6169 7469 6e67 2031 3020  ded. Waiting 10 
+00001200: 7365 636f 6e64 7320 616e 6420 7472 7969  seconds and tryi
+00001210: 6e67 2061 6761 696e 2e22 0d0a 2020 2020  ng again."..    
+00001220: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00001230: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00001240: 7028 3130 290d 0a20 2020 2020 2020 2020  p(10)..         
+00001250: 2020 2072 6573 706f 6e73 6520 3d20 6f70     response = op
+00001260: 656e 6169 2e43 6861 7443 6f6d 706c 6574  enai.ChatComplet
+00001270: 696f 6e2e 6372 6561 7465 280d 0a20 2020  ion.create(..   
+00001280: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00001290: 656c 3d6d 6f64 656c 2c0d 0a20 2020 2020  el=model,..     
+000012a0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+000012b0: 6765 733d 6d65 7373 6167 6573 2c0d 0a20  ges=messages,.. 
+000012c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000012d0: 656d 7065 7261 7475 7265 3d74 656d 7065  emperature=tempe
+000012e0: 7261 7475 7265 2c0d 0a20 2020 2020 2020  rature,..       
+000012f0: 2020 2020 2020 2020 206d 6178 5f74 6f6b           max_tok
+00001300: 656e 733d 6d61 785f 746f 6b65 6e73 2c0d  ens=max_tokens,.
+00001310: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00001320: 2020 2020 2020 2020 2320 4578 6365 6564          # Exceed
+00001330: 6564 2074 6865 206d 6178 696d 756d 206e  ed the maximum n
+00001340: 756d 6265 7220 6f66 2074 6f6b 656e 7320  umber of tokens 
+00001350: 616c 6c6f 7765 6420 6279 2074 6865 2041  allowed by the A
+00001360: 5049 0d0a 2020 2020 2020 2020 6578 6365  PI..        exce
+00001370: 7074 206f 7065 6e61 692e 6572 726f 722e  pt openai.error.
+00001380: 496e 7661 6c69 6452 6571 7565 7374 4572  InvalidRequestEr
+00001390: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+000013a0: 2020 7072 696e 7428 0d0a 2020 2020 2020    print(..      
+000013b0: 2020 2020 2020 2020 2020 2254 6865 204f            "The O
+000013c0: 7065 6e41 4920 4150 4920 6d61 7869 6d75  penAI API maximu
+000013d0: 6d20 746f 6b65 6e73 206c 696d 6974 2068  m tokens limit h
+000013e0: 6173 2062 6565 6e20 6578 6365 6564 6564  as been exceeded
+000013f0: 2e20 5377 6974 6368 696e 6720 746f 2061  . Switching to a
+00001400: 2031 364b 206d 6f64 656c 2e22 0d0a 2020   16K model."..  
+00001410: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00001420: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00001430: 6520 3d20 6f70 656e 6169 2e43 6861 7443  e = openai.ChatC
+00001440: 6f6d 706c 6574 696f 6e2e 6372 6561 7465  ompletion.create
+00001450: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00001460: 2020 206d 6f64 656c 3d73 656c 662e 6c6c     model=self.ll
+00001470: 6d5f 3136 6b2c 0d0a 2020 2020 2020 2020  m_16k,..        
+00001480: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+00001490: 3d6d 6573 7361 6765 732c 0d0a 2020 2020  =messages,..    
+000014a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+000014b0: 6572 6174 7572 653d 7465 6d70 6572 6174  erature=temperat
+000014c0: 7572 652c 0d0a 2020 2020 2020 2020 2020  ure,..          
+000014d0: 2020 2020 2020 6d61 785f 746f 6b65 6e73        max_tokens
+000014e0: 3d6d 6178 5f74 6f6b 656e 732c 0d0a 2020  =max_tokens,..  
+000014f0: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+00001500: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
+00001510: 2072 6573 706f 6e73 652e 6368 6f69 6365   response.choice
+00001520: 735b 305d 2e6d 6573 7361 6765 2e63 6f6e  s[0].message.con
+00001530: 7465 6e74 2e73 7472 6970 2829 0d0a 2020  tent.strip()..  
+00001540: 2020 2020 2020 746f 6b65 6e73 5f75 7365        tokens_use
+00001550: 6420 3d20 7265 7370 6f6e 7365 2e75 7361  d = response.usa
+00001560: 6765 2e74 6f74 616c 5f74 6f6b 656e 730d  ge.total_tokens.
+00001570: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00001580: 6e20 636f 6e74 656e 742c 2074 6f6b 656e  n content, token
+00001590: 735f 7573 6564 0d0a 2020 2020 0d0a 2020  s_used..    ..  
+000015a0: 2020 6465 6620 6c6c 6d5f 6675 6e63 5f63    def llm_func_c
+000015b0: 616c 6c28 7365 6c66 2c20 6d65 7373 6167  all(self, messag
+000015c0: 6573 2c20 6675 6e63 7469 6f6e 732c 2066  es, functions, f
+000015d0: 756e 6374 696f 6e5f 6e61 6d65 293a 0d0a  unction_name):..
+000015e0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+000015f0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+00001600: 7365 203d 206f 7065 6e61 692e 4368 6174  se = openai.Chat
+00001610: 436f 6d70 6c65 7469 6f6e 2e63 7265 6174  Completion.creat
+00001620: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+00001630: 6d6f 6465 6c20 3d20 7365 6c66 2e6c 6c6d  model = self.llm
+00001640: 5f66 756e 632c 0d0a 2020 2020 2020 2020  _func,..        
+00001650: 2020 2020 6d65 7373 6167 6573 3d6d 6573      messages=mes
+00001660: 7361 6765 732c 0d0a 2020 2020 2020 2020  sages,..        
+00001670: 2020 2020 6675 6e63 7469 6f6e 733d 6675      functions=fu
+00001680: 6e63 7469 6f6e 732c 0d0a 2020 2020 2020  nctions,..      
+00001690: 2020 2020 2020 6675 6e63 7469 6f6e 5f63        function_c
+000016a0: 616c 6c20 3d20 6675 6e63 7469 6f6e 5f6e  all = function_n
+000016b0: 616d 652c 0d0a 2020 2020 2020 2020 2020  ame,..          
+000016c0: 2020 7465 6d70 6572 6174 7572 653d 302c    temperature=0,
+000016d0: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+000016e0: 785f 746f 6b65 6e73 203d 2037 3030 2c20  x_tokens = 700, 
+000016f0: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00001700: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00001710: 6f70 656e 6169 2e65 7272 6f72 2e52 6174  openai.error.Rat
+00001720: 654c 696d 6974 4572 726f 723a 0d0a 2020  eLimitError:..  
+00001730: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00001740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001750: 2020 2254 6865 204f 7065 6e41 4920 4150    "The OpenAI AP
+00001760: 4920 7261 7465 206c 696d 6974 2068 6173  I rate limit has
+00001770: 2062 6565 6e20 6578 6365 6564 6564 2e20   been exceeded. 
+00001780: 5761 6974 696e 6720 3130 2073 6563 6f6e  Waiting 10 secon
+00001790: 6473 2061 6e64 2074 7279 696e 6720 6167  ds and trying ag
+000017a0: 6169 6e2e 220d 0a20 2020 2020 2020 2020  ain."..         
+000017b0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+000017c0: 2020 7469 6d65 2e73 6c65 6570 2831 3029    time.sleep(10)
+000017d0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000017e0: 7370 6f6e 7365 203d 206f 7065 6e61 692e  sponse = openai.
+000017f0: 4368 6174 436f 6d70 6c65 7469 6f6e 2e63  ChatCompletion.c
+00001800: 7265 6174 6528 0d0a 2020 2020 2020 2020  reate(..        
+00001810: 2020 2020 6d6f 6465 6c20 3d20 7365 6c66      model = self
+00001820: 2e6c 6c6d 5f66 756e 632c 0d0a 2020 2020  .llm_func,..    
+00001830: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+00001840: 3d6d 6573 7361 6765 732c 0d0a 2020 2020  =messages,..    
+00001850: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
+00001860: 733d 6675 6e63 7469 6f6e 732c 0d0a 2020  s=functions,..  
+00001870: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+00001880: 6f6e 5f63 616c 6c20 3d20 6675 6e63 7469  on_call = functi
+00001890: 6f6e 5f6e 616d 652c 0d0a 2020 2020 2020  on_name,..      
+000018a0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
+000018b0: 653d 302c 0d0a 2020 2020 2020 2020 2020  e=0,..          
+000018c0: 2020 290d 0a20 2020 2020 2020 200d 0a20    )..        .. 
+000018d0: 2020 2020 2020 2066 6e5f 6e61 6d65 203d         fn_name =
+000018e0: 2072 6573 706f 6e73 652e 6368 6f69 6365   response.choice
+000018f0: 735b 305d 2e6d 6573 7361 6765 5b22 6675  s[0].message["fu
+00001900: 6e63 7469 6f6e 5f63 616c 6c22 5d2e 6e61  nction_call"].na
+00001910: 6d65 0d0a 2020 2020 2020 2020 6172 6775  me..        argu
+00001920: 6d65 6e74 7320 3d20 7265 7370 6f6e 7365  ments = response
+00001930: 2e63 686f 6963 6573 5b30 5d2e 6d65 7373  .choices[0].mess
+00001940: 6167 655b 2266 756e 6374 696f 6e5f 6361  age["function_ca
+00001950: 6c6c 225d 2e61 7267 756d 656e 7473 0d0a  ll"].arguments..
+00001960: 2020 2020 2020 2020 746f 6b65 6e73 5f75          tokens_u
+00001970: 7365 6420 3d20 7265 7370 6f6e 7365 2e75  sed = response.u
+00001980: 7361 6765 2e74 6f74 616c 5f74 6f6b 656e  sage.total_token
+00001990: 730d 0a0d 0a20 2020 2020 2020 2072 6574  s....        ret
+000019a0: 7572 6e20 666e 5f6e 616d 652c 6172 6775  urn fn_name,argu
+000019b0: 6d65 6e74 732c 746f 6b65 6e73 5f75 7365  ments,tokens_use
+000019c0: 640d 0a0d 0a20 2020 200d 0a20 2020 2023  d....    ..    #
+000019d0: 2046 756e 6374 696f 6e73 2074 6f20 7361   Functions to sa
+000019e0: 6e69 7469 7a65 2074 6865 206f 7574 7075  nitize the outpu
+000019f0: 7420 6672 6f6d 2074 6865 204c 4c4d 0d0a  t from the LLM..
+00001a00: 2020 2020 6465 6620 5f65 7874 7261 6374      def _extract
+00001a10: 5f63 6f64 6528 7365 6c66 2c72 6573 706f  _code(self,respo
+00001a20: 6e73 653a 2073 7472 2c20 7365 7061 7261  nse: str, separa
+00001a30: 746f 723a 2073 7472 203d 2022 6060 6022  tor: str = "```"
+00001a40: 2920 2d3e 2073 7472 3a0d 0a0d 0a20 2020  ) -> str:....   
+00001a50: 2020 2020 2023 2044 6566 696e 6520 6120       # Define a 
+00001a60: 626c 6163 6b6c 6973 7420 6f66 2050 7974  blacklist of Pyt
+00001a70: 686f 6e20 6b65 7977 6f72 6473 2061 6e64  hon keywords and
+00001a80: 2066 756e 6374 696f 6e73 2074 6861 7420   functions that 
+00001a90: 6172 6520 6e6f 7420 616c 6c6f 7765 640d  are not allowed.
+00001aa0: 0a20 2020 2020 2020 2062 6c61 636b 6c69  .        blackli
+00001ab0: 7374 203d 205b 276f 7327 2c27 7375 6270  st = ['os','subp
+00001ac0: 726f 6365 7373 272c 2773 7973 272c 2765  rocess','sys','e
+00001ad0: 7661 6c27 2c27 6578 6563 272c 2766 696c  val','exec','fil
+00001ae0: 6527 2c27 736f 636b 6574 272c 2775 726c  e','socket','url
+00001af0: 6c69 6227 2c0d 0a20 2020 2020 2020 2020  lib',..         
+00001b00: 2020 2020 2020 2020 2020 2027 7368 7574             'shut
+00001b10: 696c 272c 2770 6963 6b6c 6527 2c27 6374  il','pickle','ct
+00001b20: 7970 6573 272c 276d 756c 7469 7072 6f63  ypes','multiproc
+00001b30: 6573 7369 6e67 272c 2774 656d 7066 696c  essing','tempfil
+00001b40: 6527 2c27 676c 6f62 272c 2763 6f64 6527  e','glob','code'
+00001b50: 2c27 7074 7927 2c27 636f 6d6d 616e 6473  ,'pty','commands
+00001b60: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001b70: 2020 2020 2020 2020 2772 6571 7565 7374          'request
+00001b80: 7327 2c27 6367 6927 2c27 6367 6974 6227  s','cgi','cgitb'
+00001b90: 2c27 786d 6c2e 6574 7265 652e 456c 656d  ,'xml.etree.Elem
+00001ba0: 656e 7454 7265 6527 2c27 6275 696c 7469  entTree','builti
+00001bb0: 6e73 270d 0a20 2020 2020 2020 2020 2020  ns'..           
+00001bc0: 2020 2020 2020 2020 205d 0d0a 0d0a 2020           ]....  
+00001bd0: 2020 2020 2020 2320 5365 6172 6368 2066        # Search f
+00001be0: 6f72 2061 2070 6174 7465 726e 2062 6574  or a pattern bet
+00001bf0: 7765 656e 203c 636f 6465 3e20 616e 6420  ween <code> and 
+00001c00: 3c2f 636f 6465 3e20 696e 2074 6865 2065  </code> in the e
+00001c10: 7874 7261 6374 6564 2063 6f64 650d 0a20  xtracted code.. 
+00001c20: 2020 2020 2020 206d 6174 6368 203d 2072         match = r
+00001c30: 652e 7365 6172 6368 2872 223c 636f 6465  e.search(r"<code
+00001c40: 3e28 2e2a 293c 2f63 6f64 653e 222c 2072  >(.*)</code>", r
+00001c50: 6573 706f 6e73 652c 2072 652e 444f 5441  esponse, re.DOTA
+00001c60: 4c4c 290d 0a20 2020 2020 2020 2069 6620  LL)..        if 
+00001c70: 6d61 7463 683a 0d0a 2020 2020 2020 2020  match:..        
+00001c80: 2020 2020 2320 4966 2061 206d 6174 6368      # If a match
+00001c90: 2069 7320 666f 756e 642c 2065 7874 7261   is found, extra
+00001ca0: 6374 2074 6865 2063 6f64 6520 6265 7477  ct the code betw
+00001cb0: 6565 6e20 3c63 6f64 653e 2061 6e64 203c  een <code> and <
+00001cc0: 2f63 6f64 653e 0d0a 2020 2020 2020 2020  /code>..        
+00001cd0: 2020 2020 636f 6465 203d 206d 6174 6368      code = match
+00001ce0: 2e67 726f 7570 2831 290d 0a20 2020 2020  .group(1)..     
+00001cf0: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
+00001d00: 7265 7370 6f6e 7365 2063 6f6e 7461 696e  response contain
+00001d10: 7320 7468 6520 7365 7061 7261 746f 722c  s the separator,
+00001d20: 2065 7874 7261 6374 2074 6865 2063 6f64   extract the cod
+00001d30: 6520 626c 6f63 6b20 6265 7477 6565 6e20  e block between 
+00001d40: 7468 6520 7365 7061 7261 746f 7273 0d0a  the separators..
+00001d50: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00001d60: 656e 2863 6f64 652e 7370 6c69 7428 7365  en(code.split(se
+00001d70: 7061 7261 746f 7229 2920 3e20 313a 0d0a  parator)) > 1:..
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 636f 6465 203d 2063 6f64 652e 7370 6c69  code = code.spli
+00001da0: 7428 7365 7061 7261 746f 7229 5b31 5d0d  t(separator)[1].
+00001db0: 0a0d 0a20 2020 2020 2020 2023 2049 6620  ...        # If 
+00001dc0: 7468 6520 7265 7370 6f6e 7365 2063 6f6e  the response con
+00001dd0: 7461 696e 7320 7468 6520 7365 7061 7261  tains the separa
+00001de0: 746f 722c 2065 7874 7261 6374 2074 6865  tor, extract the
+00001df0: 2063 6f64 6520 626c 6f63 6b20 6265 7477   code block betw
+00001e00: 6565 6e20 7468 6520 7365 7061 7261 746f  een the separato
+00001e10: 7273 0d0a 2020 2020 2020 2020 6966 206c  rs..        if l
+00001e20: 656e 2872 6573 706f 6e73 652e 7370 6c69  en(response.spli
+00001e30: 7428 7365 7061 7261 746f 7229 2920 3e20  t(separator)) > 
+00001e40: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+00001e50: 636f 6465 203d 2072 6573 706f 6e73 652e  code = response.
+00001e60: 7370 6c69 7428 7365 7061 7261 746f 7229  split(separator)
+00001e70: 5b31 5d0d 0a20 2020 2020 2020 2020 2020  [1]..           
+00001e80: 200d 0a20 2020 2020 2020 2023 2052 656d   ..        # Rem
+00001e90: 6f76 6520 7468 6520 2270 7974 686f 6e22  ove the "python"
+00001ea0: 206f 7220 2270 7922 2070 7265 6669 7820   or "py" prefix 
+00001eb0: 6966 2070 7265 7365 6e74 0d0a 2020 2020  if present..    
+00001ec0: 2020 2020 6966 2072 652e 6d61 7463 6828      if re.match(
+00001ed0: 7222 5e28 7079 7468 6f6e 7c70 7929 222c  r"^(python|py)",
+00001ee0: 2063 6f64 6529 3a0d 0a20 2020 2020 2020   code):..       
+00001ef0: 2020 2020 2063 6f64 6520 3d20 7265 2e73       code = re.s
+00001f00: 7562 2872 225e 2870 7974 686f 6e7c 7079  ub(r"^(python|py
+00001f10: 2922 2c20 2222 2c20 636f 6465 290d 0a20  )", "", code).. 
+00001f20: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
+00001f30: 636f 6465 2069 7320 6265 7477 6565 6e20  code is between 
+00001f40: 7369 6e67 6c65 2062 6163 6b74 6963 6b73  single backticks
+00001f50: 2c20 6578 7472 6163 7420 7468 6520 636f  , extract the co
+00001f60: 6465 2062 6574 7765 656e 2074 6865 6d0d  de between them.
+00001f70: 0a20 2020 2020 2020 2069 6620 7265 2e6d  .        if re.m
+00001f80: 6174 6368 2872 225e 602e 2a60 2422 2c20  atch(r"^`.*`$", 
+00001f90: 636f 6465 293a 0d0a 2020 2020 2020 2020  code):..        
+00001fa0: 2020 2020 636f 6465 203d 2072 652e 7375      code = re.su
+00001fb0: 6228 7222 5e60 282e 2a29 6024 222c 2072  b(r"^`(.*)`$", r
+00001fc0: 225c 3122 2c20 636f 6465 290d 0a0d 0a20  "\1", code).... 
+00001fd0: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
+00001fe0: 616e 7920 696e 7374 616e 6365 7320 6f66  any instances of
+00001ff0: 2022 6466 203d 2070 642e 7265 6164 5f63   "df = pd.read_c
+00002000: 7376 2827 6669 6c65 6e61 6d65 2e63 7376  sv('filename.csv
+00002010: 2729 2220 6672 6f6d 2074 6865 2063 6f64  ')" from the cod
+00002020: 650d 0a20 2020 2020 2020 2063 6f64 6520  e..        code 
+00002030: 3d20 7265 2e73 7562 2872 2264 665c 732a  = re.sub(r"df\s*
+00002040: 3d5c 732a 7064 5c2e 7265 6164 5f63 7376  =\s*pd\.read_csv
+00002050: 5c28 272e 2a3f 2728 2c2e 2a29 3f5c 2922  \('.*?'(,.*)?\)"
+00002060: 2c20 2222 2c20 636f 6465 290d 0a0d 0a20  , "", code).... 
+00002070: 2020 2020 2020 2023 2044 6566 696e 6520         # Define 
+00002080: 7468 6520 7265 6775 6c61 7220 6578 7072  the regular expr
+00002090: 6573 7369 6f6e 2070 6174 7465 726e 2074  ession pattern t
+000020a0: 6f20 6d61 7463 6820 7468 6520 626c 6163  o match the blac
+000020b0: 6b6c 6973 7420 6974 656d 730d 0a20 2020  klist items..   
+000020c0: 2020 2020 2070 6174 7465 726e 203d 2072       pattern = r
+000020d0: 225e 282e 2a5c 6228 2220 2b20 227c 222e  "^(.*\b(" + "|".
+000020e0: 6a6f 696e 2862 6c61 636b 6c69 7374 2920  join(blacklist) 
+000020f0: 2b20 7222 295c 622e 2a29 2422 0d0a 0d0a  + r")\b.*)$"....
+00002100: 2020 2020 2020 2020 2320 5265 706c 6163          # Replac
+00002110: 6520 7468 6520 626c 6163 6b6c 6973 7420  e the blacklist 
+00002120: 6974 656d 7320 7769 7468 2063 6f6d 6d65  items with comme
+00002130: 6e74 730d 0a20 2020 2020 2020 2063 6f64  nts..        cod
+00002140: 6520 3d20 7265 2e73 7562 2870 6174 7465  e = re.sub(patte
+00002150: 726e 2c20 7222 2320 6e6f 7420 616c 6c6f  rn, r"# not allo
+00002160: 7765 6420 5c31 222c 2063 6f64 652c 2066  wed \1", code, f
+00002170: 6c61 6773 3d72 652e 4d55 4c54 494c 494e  lags=re.MULTILIN
+00002180: 4529 0d0a 0d0a 2020 2020 2020 2020 2320  E)....        # 
+00002190: 5265 7475 726e 2074 6865 2063 6c65 616e  Return the clean
+000021a0: 6564 2061 6e64 2065 7874 7261 6374 6564  ed and extracted
+000021b0: 2063 6f64 650d 0a20 2020 2020 2020 2072   code..        r
+000021c0: 6574 7572 6e20 636f 6465 2e73 7472 6970  eturn code.strip
+000021d0: 2829 0d0a 2020 2020 0d0a 2020 2020 6465  ()..    ..    de
+000021e0: 6620 5f65 7874 7261 6374 5f72 616e 6b28  f _extract_rank(
+000021f0: 7365 6c66 2c72 6573 706f 6e73 653a 2073  self,response: s
+00002200: 7472 2920 2d3e 2073 7472 3a0d 0a0d 0a20  tr) -> str:.... 
+00002210: 2020 2020 2020 2023 2053 6561 7263 6820         # Search 
+00002220: 666f 7220 6120 7061 7474 6572 6e20 6265  for a pattern be
+00002230: 7477 6565 6e20 3c72 616e 6b3e 2061 6e64  tween <rank> and
+00002240: 203c 2f72 616e 6b3e 2069 6e20 7468 6520   </rank> in the 
+00002250: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00002260: 2020 6d61 7463 6820 3d20 7265 2e73 6561    match = re.sea
+00002270: 7263 6828 7222 3c72 616e 6b3e 282e 2a29  rch(r"<rank>(.*)
+00002280: 3c2f 7261 6e6b 3e22 2c20 7265 7370 6f6e  </rank>", respon
+00002290: 7365 290d 0a20 2020 2020 2020 2069 6620  se)..        if 
+000022a0: 6d61 7463 683a 0d0a 2020 2020 2020 2020  match:..        
+000022b0: 2020 2020 2320 4966 2061 206d 6174 6368      # If a match
+000022c0: 2069 7320 666f 756e 642c 2065 7874 7261   is found, extra
+000022d0: 6374 2074 6865 2072 616e 6b20 6265 7477  ct the rank betw
+000022e0: 6565 6e20 3c72 616e 6b3e 2061 6e64 203c  een <rank> and <
+000022f0: 2f72 616e 6b3e 0d0a 2020 2020 2020 2020  /rank>..        
+00002300: 2020 2020 7261 6e6b 203d 206d 6174 6368      rank = match
+00002310: 2e67 726f 7570 2831 290d 0a20 2020 2020  .group(1)..     
+00002320: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00002330: 2020 2020 2020 7261 6e6b 203d 2022 220d        rank = "".
+00002340: 0a0d 0a20 2020 2020 2020 2023 2052 6574  ...        # Ret
+00002350: 7572 6e20 7468 6520 636c 6561 6e65 6420  urn the cleaned 
+00002360: 616e 6420 6578 7472 6163 7465 6420 636f  and extracted co
+00002370: 6465 0d0a 2020 2020 2020 2020 7265 7475  de..        retu
+00002380: 726e 2072 616e 6b2e 7374 7269 7028 290d  rn rank.strip().
+00002390: 0a20 2020 200d 0a20 2020 2023 2046 756e  .    ..    # Fun
+000023a0: 6374 696f 6e20 746f 2072 656d 6f76 6520  ction to remove 
+000023b0: 6578 616d 706c 6573 2066 726f 6d20 6d65  examples from me
+000023c0: 7373 6167 6573 2077 6865 6e20 6e6f 206c  ssages when no l
+000023d0: 6f6e 6765 7220 6e65 6564 6564 0d0a 2020  onger needed..  
+000023e0: 2020 6465 6620 5f72 656d 6f76 655f 6578    def _remove_ex
+000023f0: 616d 706c 6573 2873 656c 662c 6d65 7373  amples(self,mess
+00002400: 6167 6573 3a20 7374 7229 202d 3e20 7374  ages: str) -> st
+00002410: 723a 0d0a 2020 2020 2020 2020 2320 4465  r:..        # De
+00002420: 6669 6e65 2074 6865 2072 6567 756c 6172  fine the regular
+00002430: 2065 7870 7265 7373 696f 6e20 7061 7474   expression patt
+00002440: 6572 6e0d 0a20 2020 2020 2020 2070 6174  ern..        pat
+00002450: 7465 726e 203d 2027 4578 616d 706c 6520  tern = 'Example 
+00002460: 4f75 7470 7574 3a5c 732a 3c63 6f64 653e  Output:\s*<code>
+00002470: 2e2a 3f3c 2f63 6f64 653e 5c73 2a27 0d0a  .*?</code>\s*'..
+00002480: 0d0a 2020 2020 2020 2020 2320 4974 6572  ..        # Iter
+00002490: 6174 6520 6f76 6572 2074 6865 206c 6973  ate over the lis
+000024a0: 7420 6f66 2064 6963 7469 6f6e 6172 6965  t of dictionarie
+000024b0: 730d 0a20 2020 2020 2020 2066 6f72 2064  s..        for d
+000024c0: 6963 7420 696e 206d 6573 7361 6765 733a  ict in messages:
+000024d0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000024e0: 4163 6365 7373 2061 6e64 2063 6c65 616e  Access and clean
+000024f0: 2075 7020 2763 6f6e 7465 6e74 2720 6669   up 'content' fi
+00002500: 656c 640d 0a20 2020 2020 2020 2020 2020  eld..           
+00002510: 2069 6620 6469 6374 2e67 6574 2827 726f   if dict.get('ro
+00002520: 6c65 2729 203d 3d20 2775 7365 7227 2061  le') == 'user' a
+00002530: 6e64 2027 636f 6e74 656e 7427 2069 6e20  nd 'content' in 
+00002540: 6469 6374 3a0d 0a20 2020 2020 2020 2020  dict:..         
+00002550: 2020 2020 2020 2064 6963 745b 2763 6f6e         dict['con
+00002560: 7465 6e74 275d 203d 2072 652e 7375 6228  tent'] = re.sub(
+00002570: 7061 7474 6572 6e2c 2027 272c 2064 6963  pattern, '', dic
+00002580: 745b 2763 6f6e 7465 6e74 275d 2c20 666c  t['content'], fl
+00002590: 6167 733d 7265 2e44 4f54 414c 4c29 0d0a  ags=re.DOTALL)..
+000025a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000025b0: 206d 6573 7361 6765 730d 0a20 2020 200d   messages..    .
+000025c0: 0a20 2020 2064 6566 2074 6173 6b5f 6576  .    def task_ev
+000025d0: 616c 2873 656c 662c 2065 7661 6c5f 6d65  al(self, eval_me
+000025e0: 7373 6167 6573 293a 0d0a 0d0a 2020 2020  ssages):....    
+000025f0: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
+00002600: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
+00002610: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00002620: 2320 4a75 7079 7465 7220 6e6f 7465 626f  # Jupyter notebo
+00002630: 6f6b 206f 7220 6970 7974 686f 6e0d 0a20  ok or ipython.. 
+00002640: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00002650: 6179 2848 544d 4c28 6627 3c70 2073 7479  ay(HTML(f'<p sty
+00002660: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
+00002670: 613b 223e 5c6e 4361 6c6c 696e 6720 4d6f  a;">\nCalling Mo
+00002680: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 5f66  del: {self.llm_f
+00002690: 756e 637d 3c2f 703e 2729 290d 0a20 2020  unc}</p>'))..   
+000026a0: 2020 2020 2020 2020 2064 6973 706c 6179           display
+000026b0: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
+000026c0: 796c 653d 2263 6f6c 6f72 3a6d 6167 656e  yle="color:magen
+000026d0: 7461 3b22 3e54 7279 696e 6720 746f 2064  ta;">Trying to d
+000026e0: 6574 6572 6d69 6e65 2074 6865 2062 6573  etermine the bes
+000026f0: 7420 6d65 7468 6f64 2074 6f20 616e 7377  t method to answ
+00002700: 6572 2079 6f75 7220 7175 6573 7469 6f6e  er your question
+00002710: 2c20 706c 6561 7365 2077 6169 742e 2e2e  , please wait...
+00002720: 3c2f 623e 3c2f 703e 3c62 723e 2729 290d  </b></p><br>')).
+00002730: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00002740: 2020 2020 2020 2020 2020 2020 2320 4f74              # Ot
+00002750: 6865 7220 656e 7669 726f 6e6d 656e 7420  her environment 
+00002760: 286c 696b 6520 7465 726d 696e 616c 290d  (like terminal).
+00002770: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00002780: 6e74 2863 6f6c 6f72 6564 2866 225c 6e3e  nt(colored(f"\n>
+00002790: 3e20 4361 6c6c 696e 6720 4d6f 6465 6c3a  > Calling Model:
+000027a0: 207b 7365 6c66 2e6c 6c6d 5f66 756e 637d   {self.llm_func}
+000027b0: 222c 2022 6d61 6765 6e74 6122 2929 0d0a  ", "magenta"))..
+000027c0: 2020 2020 2020 2020 2020 2020 6370 7269              cpri
+000027d0: 6e74 2866 225c 6e3e 3e20 5472 7969 6e67  nt(f"\n>> Trying
+000027e0: 2074 6f20 6465 7465 726d 696e 6520 7468   to determine th
+000027f0: 6520 6265 7374 206d 6574 686f 6420 746f  e best method to
+00002800: 2061 6e73 7765 7220 796f 7572 2071 7565   answer your que
+00002810: 7374 696f 6e2c 2070 6c65 6173 6520 7761  stion, please wa
+00002820: 6974 2e2e 2e5c 6e22 2c20 276d 6167 656e  it...\n", 'magen
+00002830: 7461 272c 2061 7474 7273 3d5b 2762 6f6c  ta', attrs=['bol
+00002840: 6427 5d29 0d0a 0d0a 2020 2020 2020 2020  d'])....        
+00002850: 2320 4361 6c6c 204f 7065 6e41 4920 4150  # Call OpenAI AP
+00002860: 490d 0a20 2020 2020 2020 2066 756e 6374  I..        funct
+00002870: 696f 6e5f 6e61 6d65 203d 207b 226e 616d  ion_name = {"nam
+00002880: 6522 3a20 2251 415f 5265 7370 6f6e 7365  e": "QA_Response
+00002890: 227d 0d0a 2020 2020 2020 2020 666e 5f6e  "}..        fn_n
+000028a0: 616d 652c 2061 7267 756d 656e 7473 2c20  ame, arguments, 
+000028b0: 746f 6b65 6e73 5f75 7365 6420 3d20 7365  tokens_used = se
+000028c0: 6c66 2e6c 6c6d 5f66 756e 635f 6361 6c6c  lf.llm_func_call
+000028d0: 2865 7661 6c5f 6d65 7373 6167 6573 2c73  (eval_messages,s
+000028e0: 656c 662e 7461 736b 5f65 7661 6c5f 6675  elf.task_eval_fu
+000028f0: 6e63 7469 6f6e 2c20 6675 6e63 7469 6f6e  nction, function
+00002900: 5f6e 616d 6529 0d0a 0d0a 2020 2020 2020  _name)....      
+00002910: 2020 2320 5061 7273 6520 7468 6520 4a53    # Parse the JS
+00002920: 4f4e 2073 7472 696e 6720 746f 2061 2050  ON string to a P
+00002930: 7974 686f 6e20 6469 6374 0d0a 2020 2020  ython dict..    
+00002940: 2020 2020 6172 6775 6d65 6e74 735f 6469      arguments_di
+00002950: 6374 203d 206a 736f 6e2e 6c6f 6164 7328  ct = json.loads(
+00002960: 6172 6775 6d65 6e74 732c 2073 7472 6963  arguments, stric
+00002970: 743d 4661 6c73 6529 0d0a 0d0a 2020 2020  t=False)....    
+00002980: 2020 2020 2320 5265 7472 6965 7665 2076      # Retrieve v
+00002990: 616c 7565 730d 0a20 2020 2020 2020 2065  alues..        e
+000029a0: 7661 6c5f 616e 7377 6572 203d 2061 7267  val_answer = arg
+000029b0: 756d 656e 7473 5f64 6963 745b 2261 6e73  uments_dict["ans
+000029c0: 7765 7222 5d0d 0a20 2020 2020 2020 2065  wer"]..        e
+000029d0: 7661 6c5f 616e 7377 6572 5f74 7970 6520  val_answer_type 
+000029e0: 3d20 6172 6775 6d65 6e74 735f 6469 6374  = arguments_dict
+000029f0: 5b22 616e 7377 6572 5f74 7970 6522 5d0d  ["answer_type"].
+00002a00: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00002a10: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+00002a20: 642e 6170 7065 6e64 2874 6f6b 656e 735f  d.append(tokens_
+00002a30: 7573 6564 290d 0a0d 0a20 2020 2020 2020  used)....       
+00002a40: 2072 6574 7572 6e20 6172 6775 6d65 6e74   return argument
+00002a50: 732c 2066 6e5f 6e61 6d65 2c20 6576 616c  s, fn_name, eval
+00002a60: 5f61 6e73 7765 722c 2065 7661 6c5f 616e  _answer, eval_an
+00002a70: 7377 6572 5f74 7970 650d 0a0d 0a20 2020  swer_type....   
+00002a80: 2064 6566 2064 6562 7567 5f63 6f64 6528   def debug_code(
+00002a90: 7365 6c66 2c63 6f64 652c 7175 6573 7469  self,code,questi
+00002aa0: 6f6e 2c20 6c6c 6d5f 6361 7363 6164 653d  on, llm_cascade=
+00002ab0: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00002ac0: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
+00002ad0: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
+00002ae0: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
+00002af0: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
+00002b00: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
+00002b10: 0d0a 2020 2020 2020 2020 6465 6275 675f  ..        debug_
+00002b20: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
+00002b30: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
+00002b40: 636f 6e74 656e 7422 3a20 7365 6c66 2e64  content": self.d
+00002b50: 6562 7567 5f63 6f64 655f 7461 736b 2e66  ebug_code_task.f
+00002b60: 6f72 6d61 7428 636f 6465 2c71 7565 7374  ormat(code,quest
+00002b70: 696f 6e29 7d5d 0d0a 0d0a 2020 2020 2020  ion)}]....      
+00002b80: 2020 7573 696e 675f 6d6f 6465 6c20 3d20    using_model = 
+00002b90: 7365 6c66 2e6c 6c6d 0d0a 2020 2020 2020  self.llm..      
+00002ba0: 2020 6966 206c 6c6d 5f63 6173 6361 6465    if llm_cascade
+00002bb0: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
+00002bc0: 7369 6e67 5f6d 6f64 656c 203d 2073 656c  sing_model = sel
+00002bd0: 662e 6c6c 6d5f 6770 7434 0d0a 0d0a 2020  f.llm_gpt4....  
+00002be0: 2020 2020 2020 6966 2027 6970 796b 6572        if 'ipyker
+00002bf0: 6e65 6c27 2069 6e20 7379 732e 6d6f 6475  nel' in sys.modu
+00002c00: 6c65 733a 0d0a 2020 2020 2020 2020 2020  les:..          
+00002c10: 2020 2320 4a75 7079 7465 7220 6e6f 7465    # Jupyter note
+00002c20: 626f 6f6b 206f 7220 6970 7974 686f 6e0d  book or ipython.
+00002c30: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00002c40: 706c 6179 2848 544d 4c28 6627 3c70 2073  play(HTML(f'<p s
+00002c50: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
+00002c60: 6e74 613b 223e 5c6e 4361 6c6c 696e 6720  nta;">\nCalling 
+00002c70: 4d6f 6465 6c3a 207b 7573 696e 675f 6d6f  Model: {using_mo
+00002c80: 6465 6c7d 3c2f 703e 2729 290d 0a20 2020  del}</p>'))..   
+00002c90: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00002ca0: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
+00002cb0: 796c 653d 2263 6f6c 6f72 3a6d 6167 656e  yle="color:magen
+00002cc0: 7461 3b22 3e49 2068 6176 6520 7265 6365  ta;">I have rece
+00002cd0: 6976 6564 2074 6865 2066 6972 7374 2076  ived the first v
+00002ce0: 6572 7369 6f6e 206f 6620 7468 6520 636f  ersion of the co
+00002cf0: 6465 2e20 4920 616d 2073 656e 6469 6e67  de. I am sending
+00002d00: 2069 7420 6261 636b 2074 6f20 4c4c 4d20   it back to LLM 
+00002d10: 746f 2067 6574 2069 7420 6368 6563 6b65  to get it checke
+00002d20: 6420 666f 7220 616e 7920 6572 726f 7273  d for any errors
+00002d30: 2c20 6275 6773 206f 7220 696e 636f 6e73  , bugs or incons
+00002d40: 6973 7465 6e63 6965 732c 2061 6e64 2063  istencies, and c
+00002d50: 6f72 7265 6374 696f 6e20 6966 206e 6563  orrection if nec
+00002d60: 6573 7361 7279 2e20 506c 6561 7365 2077  essary. Please w
+00002d70: 6169 742e 2e2e 3c2f 623e 3c2f 703e 3c62  ait...</b></p><b
+00002d80: 723e 2729 290d 0a20 2020 2020 2020 2065  r>'))..        e
+00002d90: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00002da0: 2020 2320 4f74 6865 7220 656e 7669 726f    # Other enviro
+00002db0: 6e6d 656e 7420 286c 696b 6520 7465 726d  nment (like term
+00002dc0: 696e 616c 290d 0a20 2020 2020 2020 2020  inal)..         
+00002dd0: 2020 2070 7269 6e74 2863 6f6c 6f72 6564     print(colored
+00002de0: 2866 225c 6e3e 3e20 4361 6c6c 696e 6720  (f"\n>> Calling 
+00002df0: 4d6f 6465 6c3a 207b 7573 696e 675f 6d6f  Model: {using_mo
+00002e00: 6465 6c7d 222c 2022 6d61 6765 6e74 6122  del}", "magenta"
+00002e10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00002e20: 6370 7269 6e74 2866 225c 6e3e 3e20 4920  cprint(f"\n>> I 
+00002e30: 6861 7665 2072 6563 6569 7665 6420 7468  have received th
+00002e40: 6520 6669 7273 7420 7665 7273 696f 6e20  e first version 
+00002e50: 6f66 2074 6865 2063 6f64 652e 2049 2061  of the code. I a
+00002e60: 6d20 7365 6e64 696e 6720 6974 2062 6163  m sending it bac
+00002e70: 6b20 746f 204c 4c4d 2074 6f20 6765 7420  k to LLM to get 
+00002e80: 6974 2063 6865 636b 6564 2066 6f72 2061  it checked for a
+00002e90: 6e79 2065 7272 6f72 732c 2062 7567 7320  ny errors, bugs 
+00002ea0: 6f72 2069 6e63 6f6e 7369 7374 656e 6369  or inconsistenci
+00002eb0: 6573 2c20 616e 6420 636f 7272 6563 7469  es, and correcti
+00002ec0: 6f6e 2069 6620 6e65 6365 7373 6172 792e  on if necessary.
+00002ed0: 2050 6c65 6173 6520 7761 6974 2e2e 2e5c   Please wait...\
+00002ee0: 6e22 2c20 276d 6167 656e 7461 272c 2061  n", 'magenta', a
+00002ef0: 7474 7273 3d5b 2762 6f6c 6427 5d29 0d0a  ttrs=['bold'])..
+00002f00: 0d0a 2020 2020 2020 2020 2320 4675 6e63  ..        # Func
+00002f10: 7469 6f6e 2074 6f20 6469 7370 6c61 7920  tion to display 
+00002f20: 7265 7375 6c74 7320 6e69 6365 6c79 0d0a  results nicely..
+00002f30: 2020 2020 2020 2020 6465 6620 6469 7370          def disp
+00002f40: 6c61 795f 7461 736b 2829 3a0d 0a20 2020  lay_task():..   
+00002f50: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
+00002f60: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
+00002f70: 6f64 756c 6573 3a0d 0a20 2020 2020 2020  odules:..       
+00002f80: 2020 2020 2020 2020 2023 204a 7570 7974           # Jupyt
+00002f90: 6572 206e 6f74 6562 6f6f 6b20 6f72 2069  er notebook or i
+00002fa0: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
+00002fb0: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
+00002fc0: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
+00002fd0: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
+00002fe0: 613b 223e 4920 6861 7665 2066 696e 6973  a;">I have finis
+00002ff0: 6865 6420 6465 6275 6767 696e 6720 7468  hed debugging th
+00003000: 6520 636f 6465 2c20 616e 6420 7769 6c6c  e code, and will
+00003010: 206e 6f77 2070 726f 6365 6564 2074 6f20   now proceed to 
+00003020: 7468 6520 6578 6563 7574 696f 6e2e 2e2e  the execution...
+00003030: 3c2f 623e 3c2f 703e 3c62 723e 2729 290d  </b></p><br>')).
+00003040: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00003050: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003060: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
+00003070: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
+00003080: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
+00003090: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
+000030a0: 6622 5c6e 3e3e 2049 2068 6176 6520 6669  f"\n>> I have fi
+000030b0: 6e69 7368 6564 2064 6562 7567 6769 6e67  nished debugging
+000030c0: 2074 6865 2063 6f64 652c 2061 6e64 2077   the code, and w
+000030d0: 696c 6c20 6e6f 7720 7072 6f63 6565 6420  ill now proceed 
+000030e0: 746f 2074 6865 2065 7865 6375 7469 6f6e  to the execution
+000030f0: 2e2e 2e5c 6e22 2c20 276d 6167 656e 7461  ...\n", 'magenta
+00003100: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
+00003110: 5d29 0d0a 0d0a 2020 2020 2020 2020 2320  ])....        # 
+00003120: 4361 6c6c 2074 6865 204f 7065 6e41 4920  Call the OpenAI 
+00003130: 4150 490d 0a20 2020 2020 2020 206c 6c6d  API..        llm
+00003140: 5f72 6573 706f 6e73 652c 2074 6f6b 656e  _response, token
+00003150: 735f 7573 6564 203d 2073 656c 662e 6c6c  s_used = self.ll
+00003160: 6d5f 6361 6c6c 2864 6562 7567 5f6d 6573  m_call(debug_mes
+00003170: 7361 6765 732c 7465 6d70 6572 6174 7572  sages,temperatur
+00003180: 653d 302c 6c6c 6d5f 6361 7363 6164 653d  e=0,llm_cascade=
+00003190: 6c6c 6d5f 6361 7363 6164 6529 2023 2068  llm_cascade) # h
+000031a0: 6967 6865 7220 7465 6d70 6572 6174 7572  igher temperatur
+000031b0: 6520 7265 7375 6c74 7320 696e 206d 6f72  e results in mor
+000031c0: 6520 2263 7265 6174 6976 6522 2061 6e73  e "creative" ans
+000031d0: 7765 7273 2028 736f 6d65 7469 6d65 7320  wers (sometimes 
+000031e0: 746f 6f20 6372 6561 7469 7665 203a 2d29  too creative :-)
+000031f0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00003200: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
+00003210: 6865 2063 6f64 6520 6672 6f6d 2074 6865  he code from the
+00003220: 2041 5049 2072 6573 706f 6e73 650d 0a20   API response.. 
+00003230: 2020 2020 2020 2064 6562 7567 6765 645f         debugged_
+00003240: 636f 6465 203d 2073 656c 662e 5f65 7874  code = self._ext
+00003250: 7261 6374 5f63 6f64 6528 6c6c 6d5f 7265  ract_code(llm_re
+00003260: 7370 6f6e 7365 2920 2020 2020 2020 0d0a  sponse)       ..
+00003270: 2020 2020 2020 2020 6469 7370 6c61 795f          display_
+00003280: 7461 736b 2829 0d0a 0d0a 2020 2020 2020  task()....      
+00003290: 2020 7365 6c66 2e74 6f74 616c 5f74 6f6b    self.total_tok
+000032a0: 656e 735f 7573 6564 2e61 7070 656e 6428  ens_used.append(
+000032b0: 746f 6b65 6e73 5f75 7365 6429 0d0a 0d0a  tokens_used)....
+000032c0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+000032d0: 6562 7567 6765 645f 636f 6465 0d0a 0d0a  ebugged_code....
+000032e0: 2020 2020 6465 6620 7261 6e6b 5f63 6f64      def rank_cod
+000032f0: 6528 7365 6c66 2c63 6f64 652c 7175 6573  e(self,code,ques
+00003300: 7469 6f6e 2c6c 6c6d 5f63 6173 6361 6465  tion,llm_cascade
+00003310: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
+00003320: 2020 2320 496e 6974 6961 6c69 7a65 2074    # Initialize t
+00003330: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
+00003340: 2077 6974 6820 6120 7379 7374 656d 206d   with a system m
+00003350: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
+00003360: 6720 7468 6520 7461 736b 2070 726f 6d70  g the task promp
+00003370: 740d 0a20 2020 2020 2020 2072 616e 6b5f  t..        rank_
+00003380: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
+00003390: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
+000033a0: 636f 6e74 656e 7422 3a20 7365 6c66 2e72  content": self.r
+000033b0: 616e 6b5f 616e 7377 6572 2e66 6f72 6d61  ank_answer.forma
+000033c0: 7428 636f 6465 2c71 7565 7374 696f 6e29  t(code,question)
+000033d0: 7d5d 0d0a 0d0a 2020 2020 2020 2020 7573  }]....        us
+000033e0: 696e 675f 6d6f 6465 6c20 3d20 7365 6c66  ing_model = self
+000033f0: 2e6c 6c6d 0d0a 2020 2020 2020 2020 6966  .llm..        if
+00003400: 206c 6c6d 5f63 6173 6361 6465 3a0d 0a20   llm_cascade:.. 
+00003410: 2020 2020 2020 2020 2020 2075 7369 6e67             using
+00003420: 5f6d 6f64 656c 203d 2073 656c 662e 6c6c  _model = self.ll
+00003430: 6d5f 6770 7434 0d0a 0d0a 2020 2020 2020  m_gpt4....      
+00003440: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
+00003450: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
+00003460: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00003470: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
+00003480: 206f 7220 6970 7974 686f 6e0d 0a20 2020   or ipython..   
+00003490: 2020 2020 2020 2020 2064 6973 706c 6179           display
+000034a0: 2848 544d 4c28 6627 3c70 2073 7479 6c65  (HTML(f'<p style
+000034b0: 3d22 636f 6c6f 723a 6d61 6765 6e74 613b  ="color:magenta;
+000034c0: 223e 5c6e 4361 6c6c 696e 6720 4d6f 6465  ">\nCalling Mode
+000034d0: 6c3a 207b 7573 696e 675f 6d6f 6465 6c7d  l: {using_model}
+000034e0: 3c2f 703e 2729 290d 0a20 2020 2020 2020  </p>'))..       
+000034f0: 2020 2020 2064 6973 706c 6179 2848 544d       display(HTM
+00003500: 4c28 6627 3c70 3e3c 6220 7374 796c 653d  L(f'<p><b style=
+00003510: 2263 6f6c 6f72 3a6d 6167 656e 7461 3b22  "color:magenta;"
+00003520: 3e49 2061 6d20 676f 696e 6720 746f 2065  >I am going to e
+00003530: 7661 6c75 6174 6520 616e 6420 7261 6e6b  valuate and rank
+00003540: 2074 6865 2061 6e73 7765 722e 2050 6c65   the answer. Ple
+00003550: 6173 6520 7761 6974 2e2e 2e3c 2f62 3e3c  ase wait...</b><
+00003560: 2f70 3e3c 6272 3e27 2929 0d0a 2020 2020  /p><br>'))..    
+00003570: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00003580: 2020 2020 2020 2023 204f 7468 6572 2065         # Other e
+00003590: 6e76 6972 6f6e 6d65 6e74 2028 6c69 6b65  nvironment (like
+000035a0: 2074 6572 6d69 6e61 6c29 0d0a 2020 2020   terminal)..    
+000035b0: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
+000035c0: 6c6f 7265 6428 6622 5c6e 3e3e 2043 616c  lored(f"\n>> Cal
+000035d0: 6c69 6e67 204d 6f64 656c 3a20 7b75 7369  ling Model: {usi
+000035e0: 6e67 5f6d 6f64 656c 7d22 2c20 226d 6167  ng_model}", "mag
+000035f0: 656e 7461 2229 290d 0a20 2020 2020 2020  enta"))..       
+00003600: 2020 2020 2063 7072 696e 7428 6622 5c6e       cprint(f"\n
+00003610: 3e3e 2049 2061 6d20 676f 696e 6720 746f  >> I am going to
+00003620: 2065 7661 6c75 6174 6520 616e 6420 7261   evaluate and ra
+00003630: 6e6b 2074 6865 2061 6e73 7765 722e 2050  nk the answer. P
+00003640: 6c65 6173 6520 7761 6974 2e2e 5c6e 222c  lease wait..\n",
+00003650: 2027 6d61 6765 6e74 6127 2c20 6174 7472   'magenta', attr
+00003660: 733d 5b27 626f 6c64 275d 290d 0a0d 0a20  s=['bold']).... 
+00003670: 2020 2020 2020 2023 2043 616c 6c20 7468         # Call th
+00003680: 6520 4f70 656e 4149 2041 5049 200d 0a20  e OpenAI API .. 
+00003690: 2020 2020 2020 206c 6c6d 5f72 6573 706f         llm_respo
+000036a0: 6e73 652c 2074 6f6b 656e 735f 7573 6564  nse, tokens_used
+000036b0: 203d 2073 656c 662e 6c6c 6d5f 6361 6c6c   = self.llm_call
+000036c0: 2872 616e 6b5f 6d65 7373 6167 6573 2c6c  (rank_messages,l
+000036d0: 6c6d 5f63 6173 6361 6465 3d6c 6c6d 5f63  lm_cascade=llm_c
+000036e0: 6173 6361 6465 290d 0a0d 0a20 2020 2020  ascade)....     
+000036f0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
+00003700: 2072 616e 6b20 6672 6f6d 2074 6865 2041   rank from the A
+00003710: 5049 2072 6573 706f 6e73 650d 0a20 2020  PI response..   
+00003720: 2020 2020 2072 616e 6b20 3d20 7365 6c66       rank = self
+00003730: 2e5f 6578 7472 6163 745f 7261 6e6b 286c  ._extract_rank(l
+00003740: 6c6d 5f72 6573 706f 6e73 6529 2020 2020  lm_response)    
+00003750: 2020 200d 0a0d 0a20 2020 2020 2020 2073     ....        s
+00003760: 656c 662e 746f 7461 6c5f 746f 6b65 6e73  elf.total_tokens
+00003770: 5f75 7365 642e 6170 7065 6e64 2874 6f6b  _used.append(tok
+00003780: 656e 735f 7573 6564 290d 0a0d 0a20 2020  ens_used)....   
+00003790: 2020 2020 2072 6574 7572 6e20 7261 6e6b       return rank
+000037a0: 0d0a 0d0a 2020 2020 6465 6620 7064 5f61  ....    def pd_a
+000037b0: 6765 6e74 5f63 6f6e 7665 7273 6528 7365  gent_converse(se
+000037c0: 6c66 2c20 7175 6573 7469 6f6e 3d4e 6f6e  lf, question=Non
+000037d0: 6529 3a0d 0a20 2020 2020 2020 2023 2046  e):..        # F
+000037e0: 756e 6374 696f 6e73 2074 6f20 6469 7370  unctions to disp
+000037f0: 6c61 7920 7265 7375 6c74 7320 6e69 6365  lay results nice
+00003800: 6c79 0d0a 2020 2020 2020 2020 6465 6620  ly..        def 
+00003810: 6469 7370 6c61 795f 7265 7375 6c74 7328  display_results(
+00003820: 616e 7377 6572 2c20 636f 6465 2c20 7261  answer, code, ra
+00003830: 6e6b 2c20 746f 7461 6c5f 746f 6b65 6e73  nk, total_tokens
+00003840: 5f75 7365 645f 7375 6d29 3a0d 0a20 2020  _used_sum):..   
+00003850: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
+00003860: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
+00003870: 6f64 756c 6573 3a20 2020 2020 0d0a 2020  odules:     ..  
+00003880: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003890: 2061 6e73 7765 7220 6973 206e 6f74 204e   answer is not N
+000038a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000038b0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+000038c0: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
+000038d0: 7479 6c65 3d22 636f 6c6f 723a 626c 7565  tyle="color:blue
+000038e0: 3b22 3e49 206e 6f77 2068 6176 6520 7468  ;">I now have th
+000038f0: 6520 6669 6e61 6c20 616e 7377 6572 3a3c  e final answer:<
+00003900: 2f62 3e3c 6272 3e3c 7072 6520 7374 796c  /b><br><pre styl
+00003910: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b20  e="color:black; 
+00003920: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
+00003930: 2d77 7261 703b 2066 6f6e 742d 7765 6967  -wrap; font-weig
+00003940: 6874 3a20 626f 6c64 3b22 3e7b 616e 7377  ht: bold;">{answ
+00003950: 6572 7d3c 2f70 7265 3e3c 2f70 3e3c 6272  er}</pre></p><br
+00003960: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
+00003970: 2020 2020 2020 6966 2063 6f64 6520 6973        if code is
+00003980: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+000039b0: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+000039c0: 723a 626c 7565 3b22 3e48 6572 6520 6973  r:blue;">Here is
+000039d0: 2074 6865 2066 696e 616c 2063 6f64 6520   the final code 
+000039e0: 7468 6174 2061 6363 6f6d 706c 6973 6865  that accomplishe
+000039f0: 7320 7468 6520 7461 736b 3a3c 2f62 3e3c  s the task:</b><
+00003a00: 6272 3e3c 7072 6520 7374 796c 653d 2263  br><pre style="c
+00003a10: 6f6c 6f72 3a23 3535 3535 3535 3b22 3e7b  olor:#555555;">{
+00003a20: 636f 6465 7d3c 2f70 7265 3e3c 2f70 3e3c  code}</pre></p><
+00003a30: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
+00003a40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003a50: 7665 6374 6f72 5f64 6220 616e 6420 7261  vector_db and ra
+00003a60: 6e6b 2069 7320 6e6f 7420 4e6f 6e65 3a0d  nk is not None:.
+00003a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a80: 2020 2020 2064 6973 706c 6179 2848 544d       display(HTM
+00003a90: 4c28 6627 3c70 3e3c 6220 7374 796c 653d  L(f'<p><b style=
+00003aa0: 2263 6f6c 6f72 3a62 6c75 653b 223e 5261  "color:blue;">Ra
+00003ab0: 6e6b 3a3c 2f62 3e3c 6272 3e3c 7370 616e  nk:</b><br><span
+00003ac0: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
+00003ad0: 6163 6b3b 223e 7b72 616e 6b7d 3c2f 7370  ack;">{rank}</sp
+00003ae0: 616e 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  an></p><br>'))..
+00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b00: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00003b10: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+00003b20: 723a 626c 7565 3b22 3e54 6f74 616c 2054  r:blue;">Total T
+00003b30: 6f6b 656e 7320 5573 6564 3a3c 2f62 3e3c  okens Used:</b><
+00003b40: 6272 3e3c 7370 616e 2073 7479 6c65 3d22  br><span style="
+00003b50: 636f 6c6f 723a 626c 6163 6b3b 223e 7b74  color:black;">{t
+00003b60: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00003b70: 5f73 756d 7d3c 2f73 7061 6e3e 3c2f 703e  _sum}</span></p>
+00003b80: 3c62 723e 2729 290d 0a20 2020 2020 2020  <br>'))..       
+00003b90: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00003ba0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00003bb0: 6e73 7765 7220 6973 206e 6f74 204e 6f6e  nswer is not Non
+00003bc0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003bd0: 2020 2020 2020 2020 6370 7269 6e74 2866          cprint(f
+00003be0: 225c 6e3e 3e20 4920 6e6f 7720 6861 7665  "\n>> I now have
+00003bf0: 2074 6865 2066 696e 616c 2061 6e73 7765   the final answe
+00003c00: 723a 5c6e 7b61 6e73 7765 727d 5c6e 222c  r:\n{answer}\n",
+00003c10: 2027 6772 6565 6e27 2c20 6174 7472 733d   'green', attrs=
+00003c20: 5b27 626f 6c64 275d 290d 0a20 2020 2020  ['bold'])..     
+00003c30: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00003c40: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  de is not None:.
+00003c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c60: 2020 2020 2063 7072 696e 7428 6622 3e3e       cprint(f">>
+00003c70: 2048 6572 6520 6973 2074 6865 2066 696e   Here is the fin
+00003c80: 616c 2063 6f64 6520 7468 6174 2061 6363  al code that acc
+00003c90: 6f6d 706c 6973 6865 7320 7468 6520 7461  omplishes the ta
+00003ca0: 736b 3a5c 6e7b 636f 6465 7d5c 6e22 2c20  sk:\n{code}\n", 
+00003cb0: 2767 7265 656e 272c 2061 7474 7273 3d5b  'green', attrs=[
+00003cc0: 2762 6f6c 6427 5d29 0d0a 2020 2020 2020  'bold'])..      
+00003cd0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003ce0: 662e 7665 6374 6f72 5f64 6220 616e 6420  f.vector_db and 
+00003cf0: 7261 6e6b 2069 7320 6e6f 7420 4e6f 6e65  rank is not None
+00003d00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003d10: 2020 2020 2020 2063 7072 696e 7428 6622         cprint(f"
+00003d20: 3e3e 2052 616e 6b3a 5c6e 7b72 616e 6b7d  >> Rank:\n{rank}
+00003d30: 5c6e 222c 2027 6772 6565 6e27 2c20 6174  \n", 'green', at
+00003d40: 7472 733d 5b27 626f 6c64 275d 290d 0a20  trs=['bold']).. 
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003d60: 7072 696e 7428 6622 3e3e 2054 6f74 616c  print(f">> Total
+00003d70: 2074 6f6b 656e 7320 7573 6564 3a5c 6e7b   tokens used:\n{
+00003d80: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+00003d90: 645f 7375 6d7d 5c6e 222c 2027 7965 6c6c  d_sum}\n", 'yell
+00003da0: 6f77 272c 2061 7474 7273 3d5b 2762 6f6c  ow', attrs=['bol
+00003db0: 6427 5d29 0d0a 0d0a 2020 2020 2020 2020  d'])....        
+00003dc0: 6465 6620 6469 7370 6c61 795f 6576 616c  def display_eval
+00003dd0: 2874 6173 6b5f 6576 616c 2c20 7469 746c  (task_eval, titl
+00003de0: 652c 2074 6f74 616c 5f74 6f6b 656e 735f  e, total_tokens_
+00003df0: 7573 6564 5f73 756d 293a 0d0a 2020 2020  used_sum):..    
+00003e00: 2020 2020 2020 2020 6966 2027 6970 796b          if 'ipyk
+00003e10: 6572 6e65 6c27 2069 6e20 7379 732e 6d6f  ernel' in sys.mo
+00003e20: 6475 6c65 733a 0d0a 2020 2020 2020 2020  dules:..        
+00003e30: 2020 2020 2020 2020 2320 4a75 7079 7465          # Jupyte
+00003e40: 7220 6e6f 7465 626f 6f6b 206f 7220 6970  r notebook or ip
+00003e50: 7974 686f 6e0d 0a20 2020 2020 2020 2020  ython..         
+00003e60: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
+00003e70: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
+00003e80: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
+00003e90: 7b74 6974 6c65 7d3c 2f62 3e3c 6272 3e3c  {title}</b><br><
+00003ea0: 7072 6520 7374 796c 653d 2263 6f6c 6f72  pre style="color
+00003eb0: 3a62 6c61 636b 3b20 7768 6974 652d 7370  :black; white-sp
+00003ec0: 6163 653a 2070 7265 2d77 7261 703b 2066  ace: pre-wrap; f
+00003ed0: 6f6e 742d 7765 6967 6874 3a20 626f 6c64  ont-weight: bold
+00003ee0: 3b22 3e7b 7461 736b 5f65 7661 6c7d 3c2f  ;">{task_eval}</
+00003ef0: 7072 653e 3c2f 703e 3c62 723e 2729 290d  pre></p><br>')).
 00003f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f10: 2020 2020 2064 6973 706c 6179 5f65 7661       display_eva
-00003f20: 6c28 7461 736b 5f65 7661 6c2c 2074 6974  l(task_eval, tit
-00003f30: 6c65 2c20 746f 7461 6c5f 746f 6b65 6e73  le, total_tokens
-00003f40: 5f75 7365 645f 7375 6d29 0d0a 2020 2020  _used_sum)..    
-00003f50: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00003f60: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00003f70: 6173 6b20 3d20 7175 6573 7469 6f6e 0d0a  ask = question..
-00003f80: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00003f90: 4361 6c6c 2074 6865 2070 645f 6167 656e  Call the pd_agen
-00003fa0: 7420 6d65 7468 6f64 2077 6974 6820 7468  t method with th
-00003fb0: 6520 7573 6572 2773 2071 7565 7374 696f  e user's questio
-00003fc0: 6e2c 2074 6865 206d 6573 7361 6765 7320  n, the messages 
-00003fd0: 6c69 7374 2c20 616e 6420 7468 6520 6461  list, and the da
-00003fe0: 7461 6672 616d 650d 0a20 2020 2020 2020  taframe..       
-00003ff0: 2020 2020 2061 6e73 7765 722c 2063 6f64       answer, cod
-00004000: 652c 2074 6f74 616c 5f74 6f6b 656e 735f  e, total_tokens_
-00004010: 7573 6564 5f73 756d 203d 2073 656c 662e  used_sum = self.
-00004020: 7064 5f61 6765 6e74 2874 6173 6b2c 206d  pd_agent(task, m
-00004030: 6573 7361 6765 732c 2073 656c 662e 6466  essages, self.df
-00004040: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00004050: 2023 2052 616e 6b20 7468 6520 4c4c 4d20   # Rank the LLM 
-00004060: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00004070: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-00004080: 6e6b 3a0d 0a20 2020 2020 2020 2020 2020  nk:..           
-00004090: 2020 2020 2023 2053 7769 7463 6820 746f       # Switch to
-000040a0: 2067 7074 2d34 2069 6620 6c6c 6d5f 7377   gpt-4 if llm_sw
-000040b0: 6974 6368 2070 6172 616d 6574 6572 2069  itch parameter i
-000040c0: 7320 7365 7420 746f 2054 7275 652e 2054  s set to True. T
-000040d0: 6869 7320 7769 6c6c 2069 6e63 7265 6173  his will increas
-000040e0: 6520 7468 6520 7072 6f63 6573 7369 6e67  e the processing
-000040f0: 2074 696d 6520 616e 6420 636f 7374 0d0a   time and cost..
-00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004110: 6966 2073 656c 662e 6c6c 6d5f 7377 6974  if self.llm_swit
-00004120: 6368 3a0d 0a20 2020 2020 2020 2020 2020  ch:..           
-00004130: 2020 2020 2020 2020 206c 6c6d 5f63 6173           llm_cas
-00004140: 6361 6465 203d 2054 7275 650d 0a20 2020  cade = True..   
-00004150: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00004160: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00004170: 2020 2020 2020 2020 6c6c 6d5f 6361 7363          llm_casc
-00004180: 6164 6520 3d20 4661 6c73 650d 0a20 2020  ade = False..   
-00004190: 2020 2020 2020 2020 2020 2020 2072 616e               ran
-000041a0: 6b20 3d20 7365 6c66 2e72 616e 6b5f 636f  k = self.rank_co
-000041b0: 6465 2863 6f64 652c 7461 736b 2c6c 6c6d  de(code,task,llm
-000041c0: 5f63 6173 6361 6465 3d6c 6c6d 5f63 6173  _cascade=llm_cas
-000041d0: 6361 6465 290d 0a20 2020 2020 2020 2020  cade)..         
-000041e0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000041f0: 2020 2020 2020 2020 2020 7261 6e6b 203d            rank =
-00004200: 2022 220d 0a0d 0a20 2020 2020 2020 2020   ""....         
-00004210: 2020 2064 6973 706c 6179 5f72 6573 756c     display_resul
-00004220: 7473 2861 6e73 7765 722c 2063 6f64 652c  ts(answer, code,
-00004230: 2072 616e 6b2c 2074 6f74 616c 5f74 6f6b   rank, total_tok
-00004240: 656e 735f 7573 6564 5f73 756d 290d 0a20  ens_used_sum).. 
-00004250: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004260: 6e0d 0a20 2020 2020 2020 200d 0a20 2020  n..        ..   
-00004270: 2020 2020 2023 2053 7461 7274 2061 6e20       # Start an 
-00004280: 696e 6669 6e69 7465 206c 6f6f 7020 746f  infinite loop to
-00004290: 206b 6565 7020 6173 6b69 6e67 2074 6865   keep asking the
-000042a0: 2075 7365 7220 666f 7220 7175 6573 7469   user for questi
-000042b0: 6f6e 730d 0a20 2020 2020 2020 2066 6972  ons..        fir
-000042c0: 7374 5f69 7465 7261 7469 6f6e 203d 2054  st_iteration = T
-000042d0: 7275 6520 2023 2046 6c61 6720 666f 7220  rue  # Flag for 
-000042e0: 7468 6520 6669 7273 7420 6974 6572 6174  the first iterat
-000042f0: 696f 6e20 6f66 2074 6865 206c 6f6f 700d  ion of the loop.
-00004300: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
-00004310: 7275 653a 0d0a 2020 2020 2020 2020 2020  rue:..          
-00004320: 2020 2320 5072 6f6d 7074 2074 6865 2075    # Prompt the u
-00004330: 7365 7220 746f 2065 6e74 6572 2061 2071  ser to enter a q
-00004340: 7565 7374 696f 6e20 6f72 2074 7970 6520  uestion or type 
-00004350: 2765 7869 7427 2074 6f20 7175 6974 0d0a  'exit' to quit..
-00004360: 2020 2020 2020 2020 2020 2020 6966 2027              if '
-00004370: 6970 796b 6572 6e65 6c27 2069 6e20 7379  ipykernel' in sy
-00004380: 732e 6d6f 6475 6c65 733a 0d0a 2020 2020  s.modules:..    
-00004390: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-000043a0: 6c61 7928 4854 4d4c 2827 3c62 2073 7479  lay(HTML('<b sty
-000043b0: 6c65 3d22 636f 6c6f 723a 626c 7565 3b22  le="color:blue;"
-000043c0: 3e45 6e74 6572 2079 6f75 7220 7175 6573  >Enter your ques
-000043d0: 7469 6f6e 206f 7220 7479 7065 205c 2765  tion or type \'e
-000043e0: 7869 745c 2720 746f 2071 7569 743a 3c2f  xit\' to quit:</
-000043f0: 623e 2729 290d 0a20 2020 2020 2020 2020  b>'))..         
-00004400: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00004410: 7028 3129 0d0a 2020 2020 2020 2020 2020  p(1)..          
-00004420: 2020 2020 2020 7175 6573 7469 6f6e 203d        question =
-00004430: 2069 6e70 7574 2829 0d0a 2020 2020 2020   input()..      
-00004440: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00004450: 2020 2020 2020 2020 2020 2020 2063 7072               cpr
-00004460: 696e 7428 225c 6e45 6e74 6572 2079 6f75  int("\nEnter you
-00004470: 7220 7175 6573 7469 6f6e 206f 7220 7479  r question or ty
-00004480: 7065 2027 6578 6974 2720 746f 2071 7569  pe 'exit' to qui
-00004490: 743a 222c 2027 626c 7565 272c 2061 7474  t:", 'blue', att
-000044a0: 7273 3d5b 2762 6f6c 6427 5d29 0d0a 2020  rs=['bold'])..  
-000044b0: 2020 2020 2020 2020 2020 2020 2020 7175                qu
-000044c0: 6573 7469 6f6e 203d 2069 6e70 7574 2829  estion = input()
-000044d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000044e0: 2320 4966 2074 6865 2075 7365 7220 7479  # If the user ty
-000044f0: 7065 7320 2765 7869 7427 2c20 6272 6561  pes 'exit', brea
-00004500: 6b20 6f75 7420 6f66 2074 6865 206c 6f6f  k out of the loo
-00004510: 700d 0a20 2020 2020 2020 2020 2020 2069  p..            i
-00004520: 6620 7175 6573 7469 6f6e 2e73 7472 6970  f question.strip
-00004530: 2829 2e6c 6f77 6572 2829 203d 3d20 2765  ().lower() == 'e
-00004540: 7869 7427 3a0d 0a20 2020 2020 2020 2020  xit':..         
-00004550: 2020 2020 2020 2062 7265 616b 0d0a 0d0a         break....
-00004560: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00004570: 6972 7374 5f69 7465 7261 7469 6f6e 3a0d  irst_iteration:.
-00004580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004590: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-000045a0: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
-000045b0: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
-000045c0: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
-000045d0: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
-000045e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000045f0: 2020 6d65 7373 6167 6573 203d 205b 7b22    messages = [{"
-00004600: 726f 6c65 223a 2022 7379 7374 656d 222c  role": "system",
-00004610: 2022 636f 6e74 656e 7422 3a20 7365 6c66   "content": self
-00004620: 2e73 7973 7465 6d5f 7461 736b 2e66 6f72  .system_task.for
-00004630: 6d61 7428 7175 6573 7469 6f6e 297d 5d0d  mat(question)}].
-00004640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004650: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-00004660: 6520 6576 616c 5f6d 6573 7361 6765 7320  e eval_messages 
-00004670: 6c69 7374 0d0a 2020 2020 2020 2020 2020  list..          
-00004680: 2020 2020 2020 6576 616c 5f6d 6573 7361        eval_messa
-00004690: 6765 7320 3d20 5b5d 0d0a 2020 2020 2020  ges = []..      
-000046a0: 2020 2020 2020 2020 2020 6669 7273 745f            first_
-000046b0: 6974 6572 6174 696f 6e20 3d20 4661 6c73  iteration = Fals
-000046c0: 6520 200d 0a20 2020 2020 2020 2020 2020  e  ..           
-000046d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000046e0: 2020 2023 2043 616c 6c20 7468 6520 7461     # Call the ta
-000046f0: 736b 5f65 7661 6c20 6d65 7468 6f64 2077  sk_eval method w
-00004700: 6974 6820 7468 6520 7573 6572 2773 2071  ith the user's q
-00004710: 7565 7374 696f 6e20 6966 2074 6865 2065  uestion if the e
-00004720: 7870 6c6f 7261 746f 7279 206d 6f64 6520  xploratory mode 
-00004730: 6973 2054 7275 650d 0a20 2020 2020 2020  is True..       
-00004740: 2020 2020 2069 6620 7365 6c66 2e65 7870       if self.exp
-00004750: 6c6f 7261 746f 7279 2069 7320 5472 7565  loratory is True
-00004760: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004770: 2020 2065 7661 6c5f 6d65 7373 6167 6573     eval_messages
-00004780: 2e61 7070 656e 6428 7b22 726f 6c65 223a  .append({"role":
-00004790: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
-000047a0: 7422 3a20 7365 6c66 2e74 6173 6b5f 6576  t": self.task_ev
-000047b0: 616c 7561 7469 6f6e 2e66 6f72 6d61 7428  aluation.format(
-000047c0: 7175 6573 7469 6f6e 2c20 7365 6c66 2e64  question, self.d
-000047d0: 665f 6865 6164 297d 290d 0a20 2020 2020  f_head)})..     
-000047e0: 2020 2020 2020 2020 2020 2061 7267 756d             argum
-000047f0: 656e 7473 2c20 666e 5f6e 616d 652c 2074  ents, fn_name, t
-00004800: 6173 6b5f 6576 616c 2c20 7461 736b 5f74  ask_eval, task_t
-00004810: 7970 6520 3d20 7365 6c66 2e74 6173 6b5f  ype = self.task_
-00004820: 6576 616c 2865 7661 6c5f 6d65 7373 6167  eval(eval_messag
-00004830: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-00004840: 2020 2020 2065 7661 6c5f 6d65 7373 6167       eval_messag
-00004850: 6573 2e61 7070 656e 6428 0d0a 2020 2020  es.append(..    
-00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004870: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00004880: 2020 2020 2020 2020 2020 2022 726f 6c65             "role
-00004890: 223a 2022 6173 7369 7374 616e 7422 2c0d  ": "assistant",.
-000048a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000048b0: 2020 2020 2020 2020 2022 636f 6e74 656e           "conten
-000048c0: 7422 3a20 4e6f 6e65 2c0d 0a20 2020 2020  t": None,..     
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 2022 6675 6e63 7469 6f6e 5f63 616c     "function_cal
-000048f0: 6c22 3a20 7b0d 0a20 2020 2020 2020 2020  l": {..         
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2022 6e61 6d65 223a 2066 6e5f 6e61     "name": fn_na
-00004920: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2022 6172 6775 6d65 6e74 7322 3a20 6172   "arguments": ar
-00004950: 6775 6d65 6e74 732c 0d0a 2020 2020 2020  guments,..      
-00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
-00004980: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00004990: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-000049a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000049b0: 2020 2320 5265 6d6f 7665 2074 6865 206f    # Remove the o
-000049c0: 6c64 6573 7420 636f 6e76 6572 7361 7469  ldest conversati
-000049d0: 6f6e 2066 726f 6d20 7468 6520 6d65 7373  on from the mess
-000049e0: 6167 6573 206c 6973 740d 0a20 2020 2020  ages list..     
-000049f0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00004a00: 6e28 6576 616c 5f6d 6573 7361 6765 7329  n(eval_messages)
-00004a10: 203e 2073 656c 662e 4d41 585f 434f 4e56   > self.MAX_CONV
-00004a20: 4552 5341 5449 4f4e 533a 0d0a 2020 2020  ERSATIONS:..    
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 6576 616c 5f6d 6573 7361 6765 732e 706f  eval_messages.po
-00004a50: 7028 3129 0d0a 2020 2020 2020 2020 2020  p(1)..          
-00004a60: 2020 2020 2020 2020 2020 6576 616c 5f6d            eval_m
-00004a70: 6573 7361 6765 732e 706f 7028 3129 0d0a  essages.pop(1)..
-00004a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004a90: 2020 746f 7461 6c5f 746f 6b65 6e73 5f75    total_tokens_u
-00004aa0: 7365 645f 7375 6d20 3d20 7375 6d28 7365  sed_sum = sum(se
-00004ab0: 6c66 2e74 6f74 616c 5f74 6f6b 656e 735f  lf.total_tokens_
-00004ac0: 7573 6564 290d 0a0d 0a20 2020 2020 2020  used)....       
-00004ad0: 2020 2020 2020 2020 2069 6620 7461 736b           if task
-00004ae0: 5f74 7970 6520 3d3d 2027 6e61 7272 6174  _type == 'narrat
-00004af0: 6976 6527 3a0d 0a20 2020 2020 2020 2020  ive':..         
-00004b00: 2020 2020 2020 2020 2020 2074 6974 6c65             title
-00004b10: 203d 2027 4865 7265 2069 7320 616e 2061   = 'Here is an a
-00004b20: 6e73 7765 7220 746f 2079 6f75 7220 7175  nswer to your qu
-00004b30: 6573 7469 6f6e 3a27 2020 2020 2020 2020  estion:'        
-00004b40: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b60: 2064 6973 706c 6179 5f65 7661 6c28 7461   display_eval(ta
-00004b70: 736b 5f65 7661 6c2c 2074 6974 6c65 2c20  sk_eval, title, 
-00004b80: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-00004b90: 645f 7375 6d29 0d0a 2020 2020 2020 2020  d_sum)..        
-00004ba0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00004bb0: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-00004bc0: 2020 2020 2020 6966 2074 6173 6b5f 7479        if task_ty
-00004bd0: 7065 203d 3d20 2766 6f6c 6c6f 775f 7570  pe == 'follow_up
-00004be0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-00004bf0: 2020 2020 2020 2020 7469 746c 6520 3d20          title = 
-00004c00: 2754 6f20 6265 2061 626c 6520 746f 2061  'To be able to a
-00004c10: 6e73 7765 7220 796f 7572 2071 7565 7374  nswer your quest
-00004c20: 696f 6e2c 2049 2061 6d20 676f 696e 6720  ion, I am going 
-00004c30: 746f 206e 6565 6420 736f 6d65 206d 6f72  to need some mor
-00004c40: 6520 696e 666f 3a27 2020 2020 2020 2020  e info:'        
-00004c50: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 2064 6973 706c 6179 5f65 7661 6c28 7461   display_eval(ta
-00004c80: 736b 5f65 7661 6c2c 2074 6974 6c65 2c20  sk_eval, title, 
-00004c90: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-00004ca0: 645f 7375 6d29 0d0a 2020 2020 2020 2020  d_sum)..        
-00004cb0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00004cc0: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-00004cd0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 2074 6974 6c65 203d 2027 4865 7265 2069   title = 'Here i
-00004d00: 7320 6120 7365 7175 656e 6365 206f 6620  s a sequence of 
-00004d10: 7374 6570 7320 7265 7175 6972 6564 2074  steps required t
-00004d20: 6f20 636f 6d70 6c65 7465 2074 6865 2074  o complete the t
-00004d30: 6173 6b3a 270d 0a20 2020 2020 2020 2020  ask:'..         
-00004d40: 2020 2020 2020 2020 2020 2074 6173 6b20             task 
-00004d50: 3d20 7461 736b 5f65 7661 6c0d 0a20 2020  = task_eval..   
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d70: 2064 6973 706c 6179 5f65 7661 6c28 7461   display_eval(ta
-00004d80: 736b 5f65 7661 6c2c 2074 6974 6c65 2c20  sk_eval, title, 
-00004d90: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-00004da0: 645f 7375 6d29 0d0a 2020 2020 2020 2020  d_sum)..        
-00004db0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00004dc0: 2020 2020 2020 2020 2020 2074 6173 6b20             task 
-00004dd0: 3d20 7175 6573 7469 6f6e 0d0a 0d0a 2020  = question....  
-00004de0: 2020 2020 2020 2020 2020 2320 4361 6c6c            # Call
-00004df0: 2074 6865 2070 645f 6167 656e 7420 6d65   the pd_agent me
-00004e00: 7468 6f64 2077 6974 6820 7468 6520 7573  thod with the us
-00004e10: 6572 2773 2071 7565 7374 696f 6e2c 2074  er's question, t
-00004e20: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
-00004e30: 2c20 616e 6420 7468 6520 6461 7461 6672  , and the datafr
-00004e40: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
-00004e50: 2061 6e73 7765 722c 2063 6f64 652c 2074   answer, code, t
-00004e60: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-00004e70: 5f73 756d 203d 2073 656c 662e 7064 5f61  _sum = self.pd_a
-00004e80: 6765 6e74 2874 6173 6b2c 206d 6573 7361  gent(task, messa
-00004e90: 6765 732c 2073 656c 662e 6466 290d 0a0d  ges, self.df)...
-00004ea0: 0a20 2020 2020 2020 2020 2020 2023 2052  .            # R
-00004eb0: 616e 6b20 7468 6520 4c4c 4d20 7265 7370  ank the LLM resp
-00004ec0: 6f6e 7365 0d0a 2020 2020 2020 2020 2020  onse..          
-00004ed0: 2020 6966 2073 656c 662e 7261 6e6b 3a0d    if self.rank:.
-00004ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ef0: 2023 2053 7769 7463 6820 746f 2067 7074   # Switch to gpt
-00004f00: 2d34 2069 6620 6c6c 6d5f 7377 6974 6368  -4 if llm_switch
-00004f10: 2070 6172 616d 6574 6572 2069 7320 7365   parameter is se
-00004f20: 7420 746f 2054 7275 652e 2054 6869 7320  t to True. This 
-00004f30: 7769 6c6c 2069 6e63 7265 6173 6520 7468  will increase th
-00004f40: 6520 7072 6f63 6573 7369 6e67 2074 696d  e processing tim
-00004f50: 6520 616e 6420 636f 7374 0d0a 2020 2020  e and cost..    
-00004f60: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00004f70: 656c 662e 6c6c 6d5f 7377 6974 6368 3a0d  elf.llm_switch:.
-00004f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004f90: 2020 2020 206c 6c6d 5f63 6173 6361 6465       llm_cascade
-00004fa0: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-00004fb0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fd0: 2020 2020 6c6c 6d5f 6361 7363 6164 6520      llm_cascade 
-00004fe0: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-00004ff0: 2020 2020 2020 2020 2072 616e 6b20 3d20           rank = 
-00005000: 7365 6c66 2e72 616e 6b5f 636f 6465 2863  self.rank_code(c
-00005010: 6f64 652c 7461 736b 2c6c 6c6d 5f63 6173  ode,task,llm_cas
-00005020: 6361 6465 3d6c 6c6d 5f63 6173 6361 6465  cade=llm_cascade
-00005030: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00005040: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00005050: 2020 2020 2020 7261 6e6b 203d 2022 220d        rank = "".
-00005060: 0a0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
-00005070: 6973 706c 6179 5f72 6573 756c 7473 2861  isplay_results(a
-00005080: 6e73 7765 722c 2063 6f64 652c 2072 616e  nswer, code, ran
-00005090: 6b2c 2074 6f74 616c 5f74 6f6b 656e 735f  k, total_tokens_
-000050a0: 7573 6564 5f73 756d 290d 0a0d 0a0d 0a20  used_sum)...... 
-000050b0: 2020 2064 6566 2070 645f 6167 656e 7428     def pd_agent(
-000050c0: 7365 6c66 2c20 7175 6573 7469 6f6e 2c20  self, question, 
-000050d0: 6d65 7373 6167 6573 2c20 6466 3d4e 6f6e  messages, df=Non
-000050e0: 6529 3a0d 0a20 2020 2020 2020 2023 2041  e):..        # A
-000050f0: 6464 2061 2075 7365 7220 6d65 7373 6167  dd a user messag
-00005100: 6520 7769 7468 2074 6865 2075 7064 6174  e with the updat
-00005110: 6564 2074 6173 6b20 7072 6f6d 7074 2074  ed task prompt t
-00005120: 6f20 7468 6520 6d65 7373 6167 6573 206c  o the messages l
-00005130: 6973 740d 0a20 2020 2020 2020 206d 6573  ist..        mes
-00005140: 7361 6765 732e 6170 7065 6e64 287b 2272  sages.append({"r
-00005150: 6f6c 6522 3a20 2275 7365 7222 2c20 2263  ole": "user", "c
-00005160: 6f6e 7465 6e74 223a 2073 656c 662e 7573  ontent": self.us
-00005170: 6572 5f74 6173 6b2e 666f 726d 6174 2873  er_task.format(s
-00005180: 656c 662e 6466 5f68 6561 642c 2071 7565  elf.df_head, que
-00005190: 7374 696f 6e29 7d29 0d0a 0d0a 2020 2020  stion)})....    
-000051a0: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
-000051b0: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
-000051c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000051d0: 2320 4a75 7079 7465 7220 6e6f 7465 626f  # Jupyter notebo
-000051e0: 6f6b 206f 7220 6970 7974 686f 6e0d 0a20  ok or ipython.. 
-000051f0: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00005200: 6179 2848 544d 4c28 6627 3c70 2073 7479  ay(HTML(f'<p sty
-00005210: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
-00005220: 613b 223e 5c6e 4361 6c6c 696e 6720 4d6f  a;">\nCalling Mo
-00005230: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 7d3c  del: {self.llm}<
-00005240: 2f70 3e27 2929 0d0a 2020 2020 2020 2020  /p>'))..        
-00005250: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
-00005260: 2866 273c 703e 3c62 2073 7479 6c65 3d22  (f'<p><b style="
-00005270: 636f 6c6f 723a 6d61 6765 6e74 613b 223e  color:magenta;">
-00005280: 4920 6861 7665 2073 656e 7420 796f 7572  I have sent your
-00005290: 2072 6571 7565 7374 2074 6f20 7468 6520   request to the 
-000052a0: 4c4c 4d20 616e 6420 6177 6169 7469 6e67  LLM and awaiting
-000052b0: 2072 6573 706f 6e73 652c 2070 6c65 6173   response, pleas
-000052c0: 6520 7761 6974 2e2e 2e3c 2f62 3e3c 2f70  e wait...</b></p
-000052d0: 3e3c 6272 3e27 2929 0d0a 2020 2020 2020  ><br>'))..      
-000052e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000052f0: 2020 2020 2023 204f 7468 6572 2065 6e76       # Other env
-00005300: 6972 6f6e 6d65 6e74 2028 6c69 6b65 2074  ironment (like t
-00005310: 6572 6d69 6e61 6c29 0d0a 2020 2020 2020  erminal)..      
-00005320: 2020 2020 2020 7072 696e 7428 636f 6c6f        print(colo
-00005330: 7265 6428 6622 5c6e 3e3e 2043 616c 6c69  red(f"\n>> Calli
-00005340: 6e67 204d 6f64 656c 3a20 7b73 656c 662e  ng Model: {self.
-00005350: 6c6c 6d7d 222c 2022 6d61 6765 6e74 6122  llm}", "magenta"
-00005360: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00005370: 6370 7269 6e74 2866 225c 6e3e 3e20 4920  cprint(f"\n>> I 
-00005380: 6861 7665 2073 656e 7420 796f 7572 2072  have sent your r
-00005390: 6571 7565 7374 2074 6f20 7468 6520 4c4c  equest to the LL
-000053a0: 4d20 616e 6420 6177 6169 7469 6e67 2072  M and awaiting r
-000053b0: 6573 706f 6e73 652c 2070 6c65 6173 6520  esponse, please 
-000053c0: 7761 6974 2e2e 2e5c 6e22 2c20 276d 6167  wait...\n", 'mag
-000053d0: 656e 7461 272c 2061 7474 7273 3d5b 2762  enta', attrs=['b
-000053e0: 6f6c 6427 5d29 0d0a 0d0a 2020 2020 2020  old'])....      
-000053f0: 2020 2320 4361 6c6c 2074 6865 204f 7065    # Call the Ope
-00005400: 6e41 4920 4150 490d 0a20 2020 2020 2020  nAI API..       
-00005410: 206c 6c6d 5f72 6573 706f 6e73 652c 2074   llm_response, t
-00005420: 6f6b 656e 735f 7573 6564 203d 2073 656c  okens_used = sel
-00005430: 662e 6c6c 6d5f 6361 6c6c 286d 6573 7361  f.llm_call(messa
-00005440: 6765 7329 0d0a 0d0a 2020 2020 2020 2020  ges)....        
-00005450: 2320 4578 7472 6163 7420 7468 6520 636f  # Extract the co
-00005460: 6465 2066 726f 6d20 7468 6520 4150 4920  de from the API 
-00005470: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00005480: 2020 636f 6465 203d 2073 656c 662e 5f65    code = self._e
-00005490: 7874 7261 6374 5f63 6f64 6528 6c6c 6d5f  xtract_code(llm_
-000054a0: 7265 7370 6f6e 7365 290d 0a0d 0a20 2020  response)....   
-000054b0: 2020 2020 2023 2055 7064 6174 6520 7468       # Update th
-000054c0: 6520 746f 7461 6c20 746f 6b65 6e73 2075  e total tokens u
-000054d0: 7365 640d 0a20 2020 2020 2020 2073 656c  sed..        sel
-000054e0: 662e 746f 7461 6c5f 746f 6b65 6e73 5f75  f.total_tokens_u
-000054f0: 7365 642e 6170 7065 6e64 2874 6f6b 656e  sed.append(token
-00005500: 735f 7573 6564 290d 0a0d 0a20 2020 2020  s_used)....     
-00005510: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
-00005520: 6572 726f 7220 636f 7272 6563 7469 6f6e  error correction
-00005530: 2063 6f75 6e74 6572 0d0a 2020 2020 2020   counter..      
-00005540: 2020 6572 726f 725f 636f 7272 6563 7469    error_correcti
-00005550: 6f6e 7320 3d20 300d 0a0d 0a20 2020 2020  ons = 0....     
-00005560: 2020 2023 2044 6562 7567 2063 6f64 6520     # Debug code 
-00005570: 6966 2064 6562 7567 2070 6172 616d 6574  if debug paramet
-00005580: 6572 2069 7320 7365 7420 746f 2054 7275  er is set to Tru
-00005590: 650d 0a20 2020 2020 2020 2069 6620 7365  e..        if se
-000055a0: 6c66 2e64 6562 7567 3a0d 0a20 2020 2020  lf.debug:..     
-000055b0: 2020 2020 2020 2023 2053 7769 7463 6820         # Switch 
-000055c0: 746f 2067 7074 2d34 2069 6620 6c6c 6d5f  to gpt-4 if llm_
-000055d0: 7377 6974 6368 2070 6172 616d 6574 6572  switch parameter
-000055e0: 2069 7320 7365 7420 746f 2054 7275 652e   is set to True.
-000055f0: 2054 6869 7320 7769 6c6c 2069 6e63 7265   This will incre
-00005600: 6173 6520 7468 6520 7072 6f63 6573 7369  ase the processi
-00005610: 6e67 2074 696d 6520 616e 6420 636f 7374  ng time and cost
-00005620: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00005630: 2073 656c 662e 6c6c 6d5f 7377 6974 6368   self.llm_switch
-00005640: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005650: 2020 206c 6c6d 5f63 6173 6361 6465 203d     llm_cascade =
-00005660: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-00005670: 2020 2020 2020 2069 6620 2769 7079 6b65         if 'ipyke
-00005680: 726e 656c 2720 696e 2073 7973 2e6d 6f64  rnel' in sys.mod
-00005690: 756c 6573 3a0d 0a20 2020 2020 2020 2020  ules:..         
-000056a0: 2020 2020 2020 2020 2020 2023 204a 7570             # Jup
-000056b0: 7974 6572 206e 6f74 6562 6f6f 6b0d 0a20  yter notebook.. 
+00003f10: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
+00003f20: 3c70 3e3c 6220 7374 796c 653d 2263 6f6c  <p><b style="col
+00003f30: 6f72 3a62 6c75 653b 223e 546f 7461 6c20  or:blue;">Total 
+00003f40: 546f 6b65 6e73 2055 7365 643a 3c2f 623e  Tokens Used:</b>
+00003f50: 3c62 723e 3c73 7061 6e20 7374 796c 653d  <br><span style=
+00003f60: 2263 6f6c 6f72 3a62 6c61 636b 3b22 3e7b  "color:black;">{
+00003f70: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+00003f80: 645f 7375 6d7d 3c2f 7370 616e 3e3c 2f70  d_sum}</span></p
+00003f90: 3e3c 6272 3e27 2929 0d0a 2020 2020 2020  ><br>'))..      
+00003fa0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00003fb0: 2020 2020 2020 2020 2020 2020 2023 204f               # O
+00003fc0: 7468 6572 2065 6e76 6972 6f6e 6d65 6e74  ther environment
+00003fd0: 2028 6c69 6b65 2074 6572 6d69 6e61 6c29   (like terminal)
+00003fe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003ff0: 2020 6370 7269 6e74 2866 225c 6e3e 3e20    cprint(f"\n>> 
+00004000: 7b74 6974 6c65 7d5c 6e7b 7461 736b 5f65  {title}\n{task_e
+00004010: 7661 6c7d 5c6e 222c 2027 6d61 6765 6e74  val}\n", 'magent
+00004020: 6127 2c20 6174 7472 733d 5b27 626f 6c64  a', attrs=['bold
+00004030: 275d 290d 0a20 2020 2020 2020 2020 2020  '])..           
+00004040: 2020 2020 2063 7072 696e 7428 6622 3e3e       cprint(f">>
+00004050: 2054 6f74 616c 2074 6f6b 656e 7320 7573   Total tokens us
+00004060: 6564 3a5c 6e7b 746f 7461 6c5f 746f 6b65  ed:\n{total_toke
+00004070: 6e73 5f75 7365 645f 7375 6d7d 5c6e 222c  ns_used_sum}\n",
+00004080: 2027 7965 6c6c 6f77 272c 2061 7474 7273   'yellow', attrs
+00004090: 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a 2020  =['bold'])....  
+000040a0: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
+000040b0: 7a65 2074 6865 2065 7661 6c5f 6d65 7373  ze the eval_mess
+000040c0: 6167 6573 206c 6973 740d 0a20 2020 2020  ages list..     
+000040d0: 2020 2065 7661 6c5f 6d65 7373 6167 6573     eval_messages
+000040e0: 203d 205b 5d0d 0a20 2020 2020 2020 200d   = []..        .
+000040f0: 0a20 2020 2020 2020 2023 2049 6620 6120  .        # If a 
+00004100: 7175 6573 7469 6f6e 2069 7320 7072 6f76  question is prov
+00004110: 6964 6564 2c20 736b 6970 2074 6865 2069  ided, skip the i
+00004120: 6e70 7574 2070 726f 6d70 740d 0a20 2020  nput prompt..   
+00004130: 2020 2020 2069 6620 7175 6573 7469 6f6e       if question
+00004140: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00004150: 2020 2020 2020 2020 2020 2023 2049 6e69             # Ini
+00004160: 7469 616c 697a 6520 7468 6520 6d65 7373  tialize the mess
+00004170: 6167 6573 206c 6973 7420 7769 7468 2061  ages list with a
+00004180: 2073 7973 7465 6d20 6d65 7373 6167 6520   system message 
+00004190: 636f 6e74 6169 6e69 6e67 2074 6865 2074  containing the t
+000041a0: 6173 6b20 7072 6f6d 7074 0d0a 2020 2020  ask prompt..    
+000041b0: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+000041c0: 203d 205b 7b22 726f 6c65 223a 2022 7379   = [{"role": "sy
+000041d0: 7374 656d 222c 2022 636f 6e74 656e 7422  stem", "content"
+000041e0: 3a20 7365 6c66 2e73 7973 7465 6d5f 7461  : self.system_ta
+000041f0: 736b 7d5d 0d0a 2020 2020 2020 2020 2020  sk}]..          
+00004200: 2020 2320 496e 6974 6961 6c69 7a65 2074    # Initialize t
+00004210: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
+00004220: 2077 6974 6820 6120 7379 7374 656d 206d   with a system m
+00004230: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
+00004240: 6720 7468 6520 7461 736b 2070 726f 6d70  g the task promp
+00004250: 740d 0a20 2020 2020 2020 2020 2020 2065  t..            e
+00004260: 7661 6c5f 6d65 7373 6167 6573 2e61 7070  val_messages.app
+00004270: 656e 6428 7b22 726f 6c65 223a 2022 7573  end({"role": "us
+00004280: 6572 222c 2022 636f 6e74 656e 7422 3a20  er", "content": 
+00004290: 7365 6c66 2e74 6173 6b5f 6576 616c 7561  self.task_evalua
+000042a0: 7469 6f6e 2e66 6f72 6d61 7428 7175 6573  tion.format(ques
+000042b0: 7469 6f6e 2c20 7365 6c66 2e64 665f 6865  tion, self.df_he
+000042c0: 6164 297d 290d 0a0d 0a20 2020 2020 2020  ad)})....       
+000042d0: 2020 2020 2023 2043 616c 6c20 7468 6520       # Call the 
+000042e0: 7461 736b 5f65 7661 6c20 6d65 7468 6f64  task_eval method
+000042f0: 2077 6974 6820 7468 6520 7573 6572 2773   with the user's
+00004300: 2071 7565 7374 696f 6e20 6966 2074 6865   question if the
+00004310: 2065 7870 6c6f 7261 746f 7279 206d 6f64   exploratory mod
+00004320: 6520 6973 2054 7275 650d 0a20 2020 2020  e is True..     
+00004330: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+00004340: 7870 6c6f 7261 746f 7279 2069 7320 5472  xploratory is Tr
+00004350: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
+00004360: 2020 2020 2061 7267 756d 656e 7473 2c20       arguments, 
+00004370: 666e 5f6e 616d 652c 2074 6173 6b5f 6576  fn_name, task_ev
+00004380: 616c 2c20 7461 736b 5f74 7970 6520 3d20  al, task_type = 
+00004390: 7365 6c66 2e74 6173 6b5f 6576 616c 2865  self.task_eval(e
+000043a0: 7661 6c5f 6d65 7373 6167 6573 290d 0a20  val_messages).. 
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000043c0: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+000043d0: 5f73 756d 203d 2073 756d 2873 656c 662e  _sum = sum(self.
+000043e0: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+000043f0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00004400: 2020 2020 6966 2074 6173 6b5f 7479 7065      if task_type
+00004410: 203d 3d20 276e 6172 7261 7469 7665 273a   == 'narrative':
+00004420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004430: 2020 2020 2020 7469 746c 6520 3d20 2748        title = 'H
+00004440: 6572 6520 6973 2074 6865 2061 6e73 7765  ere is the answe
+00004450: 7220 746f 2079 6f75 7220 7175 6573 7469  r to your questi
+00004460: 6f6e 3a27 2020 2020 2020 2020 2020 2020  on:'            
+00004470: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00004480: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00004490: 706c 6179 5f65 7661 6c28 7461 736b 5f65  play_eval(task_e
+000044a0: 7661 6c2c 2074 6974 6c65 2c20 746f 7461  val, title, tota
+000044b0: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
+000044c0: 6d29 0d0a 2020 2020 2020 2020 2020 2020  m)..            
+000044d0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 6966 2074 6173 6b5f 7479 7065 203d 3d20  if task_type == 
+00004500: 2766 6f6c 6c6f 775f 7570 273a 0d0a 2020  'follow_up':..  
+00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004520: 2020 7469 746c 6520 3d20 2754 6f20 6265    title = 'To be
+00004530: 2061 626c 6520 746f 2061 6e73 7765 7220   able to answer 
+00004540: 796f 7572 2071 7565 7374 696f 6e2c 2049  your question, I
+00004550: 2061 6d20 676f 696e 6720 746f 206e 6565   am going to nee
+00004560: 6420 736f 6d65 206d 6f72 6520 696e 666f  d some more info
+00004570: 3a27 2020 2020 2020 2020 2020 2020 2020  :'              
+00004580: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00004590: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+000045a0: 6179 5f65 7661 6c28 7461 736b 5f65 7661  ay_eval(task_eva
+000045b0: 6c2c 2074 6974 6c65 2c20 746f 7461 6c5f  l, title, total_
+000045c0: 746f 6b65 6e73 5f75 7365 645f 7375 6d29  tokens_used_sum)
+000045d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000045e0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+000045f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00004600: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00004610: 2020 2020 2020 2020 2074 6974 6c65 203d           title =
+00004620: 2027 4865 7265 2069 7320 7468 6520 7365   'Here is the se
+00004630: 7175 656e 6365 206f 6620 7374 6570 7320  quence of steps 
+00004640: 7265 7175 6972 6564 2074 6f20 636f 6d70  required to comp
+00004650: 6c65 7465 2074 6865 2074 6173 6b3a 270d  lete the task:'.
+00004660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004670: 2020 2020 2074 6173 6b20 3d20 7461 736b       task = task
+00004680: 5f65 7661 6c0d 0a20 2020 2020 2020 2020  _eval..         
+00004690: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+000046a0: 6179 5f65 7661 6c28 7461 736b 5f65 7661  ay_eval(task_eva
+000046b0: 6c2c 2074 6974 6c65 2c20 746f 7461 6c5f  l, title, total_
+000046c0: 746f 6b65 6e73 5f75 7365 645f 7375 6d29  tokens_used_sum)
+000046d0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000046e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000046f0: 2020 2020 2074 6173 6b20 3d20 7175 6573       task = ques
+00004700: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+00004710: 2020 2020 6966 2073 656c 662e 7665 6374      if self.vect
+00004720: 6f72 5f64 623a 0d0a 2020 2020 2020 2020  or_db:..        
+00004730: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
+00004740: 6865 2072 6574 7269 6576 655f 616e 7377  he retrieve_answ
+00004750: 6572 206d 6574 686f 6420 746f 2063 6865  er method to che
+00004760: 636b 2069 6620 7468 6520 7175 6573 7469  ck if the questi
+00004770: 6f6e 2068 6173 2061 6c72 6561 6479 2062  on has already b
+00004780: 6565 6e20 6173 6b65 6420 616e 6420 616e  een asked and an
+00004790: 7377 6572 6564 0d0a 2020 2020 2020 2020  swered..        
+000047a0: 2020 2020 2020 2020 6578 616d 706c 655f          example_
+000047b0: 6f75 7470 7574 203d 2073 656c 662e 7265  output = self.re
+000047c0: 7472 6965 7665 5f61 6e73 7765 7228 7461  trieve_answer(ta
+000047d0: 736b 2c20 7365 6c66 2e64 665f 636f 6c75  sk, self.df_colu
+000047e0: 6d6e 7329 0d0a 2020 2020 2020 2020 2020  mns)..          
+000047f0: 2020 2020 2020 6966 2065 7861 6d70 6c65        if example
+00004800: 5f6f 7574 7075 7420 6973 206e 6f74 204e  _output is not N
+00004810: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00004820: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+00004830: 655f 6f75 7470 7574 203d 2065 7861 6d70  e_output = examp
+00004840: 6c65 5f6f 7574 7075 740d 0a20 2020 2020  le_output..     
+00004850: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00004860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004870: 2020 2020 2020 6578 616d 706c 655f 6f75        example_ou
+00004880: 7470 7574 203d 2073 656c 662e 6465 6661  tput = self.defa
+00004890: 756c 745f 6578 616d 706c 655f 6f75 7470  ult_example_outp
+000048a0: 7574 0d0a 2020 2020 2020 2020 2020 2020  ut..            
+000048b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000048c0: 2020 2020 2020 2065 7861 6d70 6c65 5f6f         example_o
+000048d0: 7574 7075 7420 3d20 7365 6c66 2e64 6566  utput = self.def
+000048e0: 6175 6c74 5f65 7861 6d70 6c65 5f6f 7574  ault_example_out
+000048f0: 7075 740d 0a0d 0a20 2020 2020 2020 2020  put....         
+00004900: 2020 2023 2043 616c 6c20 7468 6520 7064     # Call the pd
+00004910: 5f61 6765 6e74 206d 6574 686f 6420 7769  _agent method wi
+00004920: 7468 2074 6865 2075 7365 7227 7320 7175  th the user's qu
+00004930: 6573 7469 6f6e 2c20 7468 6520 6d65 7373  estion, the mess
+00004940: 6167 6573 206c 6973 742c 2061 6e64 2074  ages list, and t
+00004950: 6865 2064 6174 6166 7261 6d65 0d0a 2020  he dataframe..  
+00004960: 2020 2020 2020 2020 2020 616e 7377 6572            answer
+00004970: 2c20 636f 6465 2c20 746f 7461 6c5f 746f  , code, total_to
+00004980: 6b65 6e73 5f75 7365 645f 7375 6d20 3d20  kens_used_sum = 
+00004990: 7365 6c66 2e70 645f 6167 656e 7428 7461  self.pd_agent(ta
+000049a0: 736b 2c20 6d65 7373 6167 6573 2c20 6578  sk, messages, ex
+000049b0: 616d 706c 655f 6f75 7470 7574 2c20 7365  ample_output, se
+000049c0: 6c66 2e64 6629 0d0a 0d0a 2020 2020 2020  lf.df)....      
+000049d0: 2020 2020 2020 2320 5261 6e6b 2074 6865        # Rank the
+000049e0: 204c 4c4d 2072 6573 706f 6e73 650d 0a20   LLM response.. 
+000049f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00004a00: 6c66 2e76 6563 746f 725f 6462 3a0d 0a20  lf.vector_db:.. 
+00004a10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00004a20: 2053 7769 7463 6820 746f 2067 7074 2d34   Switch to gpt-4
+00004a30: 2069 6620 6c6c 6d5f 7377 6974 6368 2070   if llm_switch p
+00004a40: 6172 616d 6574 6572 2069 7320 7365 7420  arameter is set 
+00004a50: 746f 2054 7275 652e 2054 6869 7320 7769  to True. This wi
+00004a60: 6c6c 2069 6e63 7265 6173 6520 7468 6520  ll increase the 
+00004a70: 7072 6f63 6573 7369 6e67 2074 696d 6520  processing time 
+00004a80: 616e 6420 636f 7374 0d0a 2020 2020 2020  and cost..      
+00004a90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00004aa0: 662e 6c6c 6d5f 7377 6974 6368 3a0d 0a20  f.llm_switch:.. 
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ac0: 2020 206c 6c6d 5f63 6173 6361 6465 203d     llm_cascade =
+00004ad0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+00004ae0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b00: 2020 6c6c 6d5f 6361 7363 6164 6520 3d20    llm_cascade = 
+00004b10: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+00004b20: 2020 2020 2020 2072 616e 6b20 3d20 7365         rank = se
+00004b30: 6c66 2e72 616e 6b5f 636f 6465 2863 6f64  lf.rank_code(cod
+00004b40: 652c 7461 736b 2c6c 6c6d 5f63 6173 6361  e,task,llm_casca
+00004b50: 6465 3d6c 6c6d 5f63 6173 6361 6465 290d  de=llm_cascade).
+00004b60: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00004b70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00004b80: 2020 2020 7261 6e6b 203d 2022 220d 0a0d      rank = ""...
+00004b90: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00004ba0: 706c 6179 5f72 6573 756c 7473 2861 6e73  play_results(ans
+00004bb0: 7765 722c 2063 6f64 652c 2072 616e 6b2c  wer, code, rank,
+00004bc0: 2074 6f74 616c 5f74 6f6b 656e 735f 7573   total_tokens_us
+00004bd0: 6564 5f73 756d 290d 0a0d 0a20 2020 2020  ed_sum)....     
+00004be0: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+00004bf0: 6563 746f 725f 6462 3a0d 0a20 2020 2020  ector_db:..     
+00004c00: 2020 2020 2020 2020 2020 2023 2050 726f             # Pro
+00004c10: 6d70 7420 7468 6520 7573 6572 2074 6f20  mpt the user to 
+00004c20: 746f 2067 6976 6520 6120 6665 6564 6261  to give a feedba
+00004c30: 636b 206f 6e20 7468 6520 7261 6e6b 696e  ck on the rankin
+00004c40: 670d 0a20 2020 2020 2020 2020 2020 2020  g..             
+00004c50: 2020 2069 6620 2769 7079 6b65 726e 656c     if 'ipykernel
+00004c60: 2720 696e 2073 7973 2e6d 6f64 756c 6573  ' in sys.modules
+00004c70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004c80: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
+00004c90: 544d 4c28 273c 6220 7374 796c 653d 2263  TML('<b style="c
+00004ca0: 6f6c 6f72 3a67 7265 656e 3b22 3e41 7265  olor:green;">Are
+00004cb0: 2079 6f75 2068 6170 7079 2077 6974 6820   you happy with 
+00004cc0: 7468 6520 7261 6e6b 696e 6720 3f20 4966  the ranking ? If
+00004cd0: 2059 4553 2074 7970 6520 5c27 7965 735c   YES type \'yes\
+00004ce0: 272e 2049 6620 4e4f 2074 7970 6520 696e  '. If NO type in
+00004cf0: 2074 6865 206e 6577 2072 616e 6b20 6f6e   the new rank on
+00004d00: 2061 2073 6361 6c65 2066 726f 6d20 312d   a scale from 1-
+00004d10: 3130 3a3c 2f62 3e27 2929 0d0a 2020 2020  10:</b>'))..    
+00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d30: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 2020 2072 616e 6b5f 6665 6564 6261 636b     rank_feedback
+00004d60: 203d 2069 6e70 7574 2829 0d0a 2020 2020   = input()..    
+00004d70: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00004d80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004d90: 2020 2020 2020 2063 7072 696e 7428 225c         cprint("\
+00004da0: 6e41 7265 2079 6f75 2068 6170 7079 2077  nAre you happy w
+00004db0: 6974 6820 7468 6520 7261 6e6b 696e 6720  ith the ranking 
+00004dc0: 3f5c 6e49 6620 5945 5320 7479 7065 2027  ?\nIf YES type '
+00004dd0: 7965 7327 2e20 4966 204e 4f20 7479 7065  yes'. If NO type
+00004de0: 2069 6e20 7468 6520 6e65 7720 7261 6e6b   in the new rank
+00004df0: 206f 6e20 6120 7363 616c 6520 6672 6f6d   on a scale from
+00004e00: 2031 2d31 303a 222c 2027 6772 6565 6e27   1-10:", 'green'
+00004e10: 2c20 6174 7472 733d 5b27 626f 6c64 275d  , attrs=['bold']
+00004e20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004e30: 2020 2020 2020 2072 616e 6b5f 6665 6564         rank_feed
+00004e40: 6261 636b 203d 2069 6e70 7574 2829 0d0a  back = input()..
+00004e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004e60: 2020 2320 4966 2074 6865 2075 7365 7220    # If the user 
+00004e70: 7479 7065 7320 2279 6573 222c 2075 7365  types "yes", use
+00004e80: 2074 6865 2072 616e 6b20 6173 2069 732e   the rank as is.
+00004e90: 2049 6620 6e6f 742c 2075 7365 2074 6865   If not, use the
+00004ea0: 2075 7365 7227 7320 7261 6e6b 2e0d 0a20   user's rank... 
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004ec0: 6620 7261 6e6b 5f66 6565 6462 6163 6b2e  f rank_feedback.
+00004ed0: 7374 7269 7028 292e 6c6f 7765 7228 2920  strip().lower() 
+00004ee0: 3d3d 2027 7965 7327 3a0d 0a20 2020 2020  == 'yes':..     
+00004ef0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004f00: 616e 6b20 3d20 7261 6e6b 0d0a 2020 2020  ank = rank..    
+00004f10: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00004f20: 2072 616e 6b5f 6665 6564 6261 636b 2069   rank_feedback i
+00004f30: 6e20 6d61 7028 7374 722c 2072 616e 6765  n map(str, range
+00004f40: 2830 2c20 3131 2929 3a0d 0a20 2020 2020  (0, 11)):..     
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004f60: 616e 6b20 3d20 7261 6e6b 5f66 6565 6462  ank = rank_feedb
+00004f70: 6163 6b0d 0a20 2020 2020 2020 2020 2020  ack..           
+00004f80: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00004f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fa0: 7261 6e6b 203d 2072 616e 6b0d 0a0d 0a20  rank = rank.... 
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00004fc0: 2041 6464 2074 6865 2071 7565 7374 696f   Add the questio
+00004fd0: 6e20 616e 6420 616e 7377 6572 2070 6169  n and answer pai
+00004fe0: 7220 746f 2074 6865 2051 4120 7265 7472  r to the QA retr
+00004ff0: 6965 7661 6c20 696e 6465 780d 0a20 2020  ieval index..   
+00005000: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005010: 662e 6164 645f 7175 6573 7469 6f6e 5f61  f.add_question_a
+00005020: 6e73 7765 725f 7061 6972 2874 6173 6b2c  nswer_pair(task,
+00005030: 2073 656c 662e 6466 5f63 6f6c 756d 6e73   self.df_columns
+00005040: 2c20 636f 6465 2c20 7261 6e6b 290d 0a0d  , code, rank)...
+00005050: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00005060: 7572 6e0d 0a20 2020 2020 2020 200d 0a20  urn..        .. 
+00005070: 2020 2020 2020 2023 2053 7461 7274 2061         # Start a
+00005080: 6e20 696e 6669 6e69 7465 206c 6f6f 7020  n infinite loop 
+00005090: 746f 206b 6565 7020 6173 6b69 6e67 2074  to keep asking t
+000050a0: 6865 2075 7365 7220 666f 7220 7175 6573  he user for ques
+000050b0: 7469 6f6e 730d 0a20 2020 2020 2020 2066  tions..        f
+000050c0: 6972 7374 5f69 7465 7261 7469 6f6e 203d  irst_iteration =
+000050d0: 2054 7275 6520 2023 2046 6c61 6720 666f   True  # Flag fo
+000050e0: 7220 7468 6520 6669 7273 7420 6974 6572  r the first iter
+000050f0: 6174 696f 6e20 6f66 2074 6865 206c 6f6f  ation of the loo
+00005100: 700d 0a20 2020 2020 2020 2077 6869 6c65  p..        while
+00005110: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
+00005120: 2020 2020 2320 5072 6f6d 7074 2074 6865      # Prompt the
+00005130: 2075 7365 7220 746f 2065 6e74 6572 2061   user to enter a
+00005140: 2071 7565 7374 696f 6e20 6f72 2074 7970   question or typ
+00005150: 6520 2765 7869 7427 2074 6f20 7175 6974  e 'exit' to quit
+00005160: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00005170: 2027 6970 796b 6572 6e65 6c27 2069 6e20   'ipykernel' in 
+00005180: 7379 732e 6d6f 6475 6c65 733a 0d0a 2020  sys.modules:..  
+00005190: 2020 2020 2020 2020 2020 2020 2020 6469                di
+000051a0: 7370 6c61 7928 4854 4d4c 2827 3c62 2073  splay(HTML('<b s
+000051b0: 7479 6c65 3d22 636f 6c6f 723a 626c 7565  tyle="color:blue
+000051c0: 3b22 3e45 6e74 6572 2079 6f75 7220 7175  ;">Enter your qu
+000051d0: 6573 7469 6f6e 206f 7220 7479 7065 205c  estion or type \
+000051e0: 2765 7869 745c 2720 746f 2071 7569 743a  'exit\' to quit:
+000051f0: 3c2f 623e 2729 290d 0a20 2020 2020 2020  </b>'))..       
+00005200: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
+00005210: 6565 7028 3129 0d0a 2020 2020 2020 2020  eep(1)..        
+00005220: 2020 2020 2020 2020 7175 6573 7469 6f6e          question
+00005230: 203d 2069 6e70 7574 2829 0d0a 2020 2020   = input()..    
+00005240: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00005250: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00005260: 7072 696e 7428 225c 6e45 6e74 6572 2079  print("\nEnter y
+00005270: 6f75 7220 7175 6573 7469 6f6e 206f 7220  our question or 
+00005280: 7479 7065 2027 6578 6974 2720 746f 2071  type 'exit' to q
+00005290: 7569 743a 222c 2027 626c 7565 272c 2061  uit:", 'blue', a
+000052a0: 7474 7273 3d5b 2762 6f6c 6427 5d29 0d0a  ttrs=['bold'])..
+000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052c0: 7175 6573 7469 6f6e 203d 2069 6e70 7574  question = input
+000052d0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+000052e0: 2020 2320 4966 2074 6865 2075 7365 7220    # If the user 
+000052f0: 7479 7065 7320 2765 7869 7427 2c20 6272  types 'exit', br
+00005300: 6561 6b20 6f75 7420 6f66 2074 6865 206c  eak out of the l
+00005310: 6f6f 700d 0a20 2020 2020 2020 2020 2020  oop..           
+00005320: 2069 6620 7175 6573 7469 6f6e 2e73 7472   if question.str
+00005330: 6970 2829 2e6c 6f77 6572 2829 203d 3d20  ip().lower() == 
+00005340: 2765 7869 7427 3a0d 0a20 2020 2020 2020  'exit':..       
+00005350: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
+00005360: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00005370: 2066 6972 7374 5f69 7465 7261 7469 6f6e   first_iteration
+00005380: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005390: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
+000053a0: 7468 6520 6d65 7373 6167 6573 206c 6973  the messages lis
+000053b0: 7420 7769 7468 2061 2073 7973 7465 6d20  t with a system 
+000053c0: 6d65 7373 6167 6520 636f 6e74 6169 6e69  message containi
+000053d0: 6e67 2074 6865 2074 6173 6b20 7072 6f6d  ng the task prom
+000053e0: 7074 0d0a 2020 2020 2020 2020 2020 2020  pt..            
+000053f0: 2020 2020 6d65 7373 6167 6573 203d 205b      messages = [
+00005400: 7b22 726f 6c65 223a 2022 7379 7374 656d  {"role": "system
+00005410: 222c 2022 636f 6e74 656e 7422 3a20 7365  ", "content": se
+00005420: 6c66 2e73 7973 7465 6d5f 7461 736b 7d5d  lf.system_task}]
+00005430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005440: 2020 6669 7273 745f 6974 6572 6174 696f    first_iteratio
+00005450: 6e20 3d20 4661 6c73 6520 200d 0a20 2020  n = False  ..   
+00005460: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00005470: 2020 2020 2020 2020 2020 2023 2043 616c             # Cal
+00005480: 6c20 7468 6520 7461 736b 5f65 7661 6c20  l the task_eval 
+00005490: 6d65 7468 6f64 2077 6974 6820 7468 6520  method with the 
+000054a0: 7573 6572 2773 2071 7565 7374 696f 6e20  user's question 
+000054b0: 6966 2074 6865 2065 7870 6c6f 7261 746f  if the explorato
+000054c0: 7279 206d 6f64 6520 6973 2054 7275 650d  ry mode is True.
+000054d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000054e0: 7365 6c66 2e65 7870 6c6f 7261 746f 7279  self.exploratory
+000054f0: 2069 7320 5472 7565 3a0d 0a20 2020 2020   is True:..     
+00005500: 2020 2020 2020 2020 2020 2065 7661 6c5f             eval_
+00005510: 6d65 7373 6167 6573 2e61 7070 656e 6428  messages.append(
+00005520: 7b22 726f 6c65 223a 2022 7573 6572 222c  {"role": "user",
+00005530: 2022 636f 6e74 656e 7422 3a20 7365 6c66   "content": self
+00005540: 2e74 6173 6b5f 6576 616c 7561 7469 6f6e  .task_evaluation
+00005550: 2e66 6f72 6d61 7428 7175 6573 7469 6f6e  .format(question
+00005560: 2c20 7365 6c66 2e64 665f 6865 6164 297d  , self.df_head)}
+00005570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005580: 2020 2061 7267 756d 656e 7473 2c20 666e     arguments, fn
+00005590: 5f6e 616d 652c 2074 6173 6b5f 6576 616c  _name, task_eval
+000055a0: 2c20 7461 736b 5f74 7970 6520 3d20 7365  , task_type = se
+000055b0: 6c66 2e74 6173 6b5f 6576 616c 2865 7661  lf.task_eval(eva
+000055c0: 6c5f 6d65 7373 6167 6573 290d 0a20 2020  l_messages)..   
+000055d0: 2020 2020 2020 2020 2020 2020 2065 7661               eva
+000055e0: 6c5f 6d65 7373 6167 6573 2e61 7070 656e  l_messages.appen
+000055f0: 6428 0d0a 2020 2020 2020 2020 2020 2020  d(..            
+00005600: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005620: 2020 2022 726f 6c65 223a 2022 6173 7369     "role": "assi
+00005630: 7374 616e 7422 2c0d 0a20 2020 2020 2020  stant",..       
+00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005650: 2022 636f 6e74 656e 7422 3a20 4e6f 6e65   "content": None
+00005660: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005670: 2020 2020 2020 2020 2020 2022 6675 6e63             "func
+00005680: 7469 6f6e 5f63 616c 6c22 3a20 7b0d 0a20  tion_call": {.. 
+00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056a0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+000056b0: 223a 2066 6e5f 6e61 6d65 2c0d 0a20 2020  ": fn_name,..   
 000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056d0: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
-000056e0: 273c 7370 616e 2073 7479 6c65 3d22 636f  '<span style="co
-000056f0: 6c6f 723a 206d 6167 656e 7461 3b22 3e53  lor: magenta;">S
-00005700: 7769 7463 6869 6e67 206d 6f64 656c 2074  witching model t
-00005710: 6f20 6770 742d 3420 746f 2064 6562 7567  o gpt-4 to debug
-00005720: 2074 6865 2063 6f64 652e 3c2f 7370 616e   the code.</span
-00005730: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
-00005740: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2023 2043 4c49 0d0a 2020 2020 2020 2020   # CLI..        
-00005770: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00005780: 7428 636f 6c6f 7265 6428 225c 6e3e 3e20  t(colored("\n>> 
-00005790: 5377 6974 6368 696e 6720 6d6f 6465 6c20  Switching model 
-000057a0: 746f 2047 5054 2d34 2074 6f20 6465 6275  to GPT-4 to debu
-000057b0: 6720 7468 6520 636f 6465 2e22 2c20 226d  g the code.", "m
-000057c0: 6167 656e 7461 2229 290d 0a20 2020 2020  agenta"))..     
-000057d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000057e0: 2020 2020 2020 2020 2020 2020 2020 6c6c                ll
-000057f0: 6d5f 6361 7363 6164 6520 3d20 4661 6c73  m_cascade = Fals
-00005800: 650d 0a20 2020 2020 2020 2020 2020 2063  e..            c
-00005810: 6f64 6520 3d20 7365 6c66 2e64 6562 7567  ode = self.debug
-00005820: 5f63 6f64 6528 636f 6465 2c20 7175 6573  _code(code, ques
-00005830: 7469 6f6e 2c20 6c6c 6d5f 6361 7363 6164  tion, llm_cascad
-00005840: 653d 6c6c 6d5f 6361 7363 6164 6529 0d0a  e=llm_cascade)..
-00005850: 0d0a 2020 2020 2020 2020 2320 5265 6469  ..        # Redi
-00005860: 7265 6374 2073 7461 6e64 6172 6420 6f75  rect standard ou
-00005870: 7470 7574 2074 6f20 6120 5374 7269 6e67  tput to a String
-00005880: 494f 2062 7566 6665 720d 0a20 2020 2020  IO buffer..     
-00005890: 2020 2077 6974 6820 7265 6469 7265 6374     with redirect
-000058a0: 5f73 7464 6f75 7428 696f 2e53 7472 696e  _stdout(io.Strin
-000058b0: 6749 4f28 2929 2061 7320 6f75 7470 7574  gIO()) as output
-000058c0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-000058d0: 2054 7279 2074 6f20 6578 6563 7574 6520   Try to execute 
-000058e0: 7468 6520 636f 6465 2061 6e64 2068 616e  the code and han
-000058f0: 646c 6520 6572 726f 7273 0d0a 2020 2020  dle errors..    
-00005900: 2020 2020 2020 2020 7768 696c 6520 6572          while er
-00005910: 726f 725f 636f 7272 6563 7469 6f6e 7320  ror_corrections 
-00005920: 3c20 7365 6c66 2e4d 4158 5f45 5252 4f52  < self.MAX_ERROR
-00005930: 5f43 4f52 5245 4354 494f 4e53 3a0d 0a20  _CORRECTIONS:.. 
-00005940: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005950: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00005960: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00005970: 732e 6170 7065 6e64 287b 2272 6f6c 6522  s.append({"role"
-00005980: 3a20 2261 7373 6973 7461 6e74 222c 2022  : "assistant", "
-00005990: 636f 6e74 656e 7422 3a20 6c6c 6d5f 7265  content": llm_re
-000059a0: 7370 6f6e 7365 7d29 0d0a 2020 2020 2020  sponse})..      
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000059c0: 5265 6d6f 7665 2074 6865 206f 6c64 6573  Remove the oldes
-000059d0: 7420 636f 6e76 6572 7361 7469 6f6e 2066  t conversation f
-000059e0: 726f 6d20 7468 6520 6d65 7373 6167 6573  rom the messages
-000059f0: 206c 6973 740d 0a20 2020 2020 2020 2020   list..         
-00005a00: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00005a10: 6e28 6d65 7373 6167 6573 2920 3e20 7365  n(messages) > se
-00005a20: 6c66 2e4d 4158 5f43 4f4e 5645 5253 4154  lf.MAX_CONVERSAT
-00005a30: 494f 4e53 3a0d 0a20 2020 2020 2020 2020  IONS:..         
-00005a40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00005a50: 6573 7361 6765 732e 706f 7028 3129 0d0a  essages.pop(1)..
-00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a70: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
-00005a80: 2e70 6f70 2831 290d 0a20 2020 2020 2020  .pop(1)..       
-00005a90: 2020 2020 2020 2020 2020 2020 2023 2052               # R
-00005aa0: 6573 6574 2064 6620 746f 2074 6865 206f  eset df to the o
-00005ab0: 7269 6769 6e61 6c20 7374 6174 6520 6265  riginal state be
-00005ac0: 666f 7265 2065 7865 6375 7469 6e67 2074  fore executing t
-00005ad0: 6865 2063 6f64 650d 0a20 2020 2020 2020  he code..       
-00005ae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005af0: 662e 6466 203d 2073 656c 662e 6f72 6967  f.df = self.orig
-00005b00: 696e 616c 5f64 662e 636f 7079 2829 0d0a  inal_df.copy()..
-00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 2020 2020 2320 4578 6563 7574 6520 7468      # Execute th
-00005b30: 6520 636f 6465 0d0a 2020 2020 2020 2020  e code..        
-00005b40: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00005b50: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-00005b60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005b70: 2020 2020 2020 2020 2020 6578 6563 2863            exec(c
-00005b80: 6f64 652c 207b 2764 6627 3a20 7365 6c66  ode, {'df': self
-00005b90: 2e64 667d 290d 0a20 2020 2020 2020 2020  .df})..         
-00005ba0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00005bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005bc0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00005bd0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-00005be0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00005bf0: 5072 696e 7420 7468 6520 6572 726f 7220  Print the error 
-00005c00: 6d65 7373 6167 650d 0a20 2020 2020 2020  message..       
-00005c10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005c20: 2769 7079 6b65 726e 656c 2720 696e 2073  'ipykernel' in s
-00005c30: 7973 2e6d 6f64 756c 6573 3a0d 0a20 2020  ys.modules:..   
-00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c50: 2020 2020 2023 204a 7570 7974 6572 206e       # Jupyter n
-00005c60: 6f74 6562 6f6f 6b0d 0a20 2020 2020 2020  otebook..       
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
-00005c90: 3c62 723e 3c62 3e3c 7370 616e 2073 7479  <br><b><span sty
-00005ca0: 6c65 3d22 636f 6c6f 723a 2023 6438 3663  le="color: #d86c
-00005cb0: 3030 3b22 3e49 2072 616e 2069 6e74 6f20  00;">I ran into 
-00005cc0: 616e 2069 7373 7565 3a3c 2f73 7061 6e3e  an issue:</span>
-00005cd0: 3c2f 623e 3c62 723e 3c70 7265 2073 7479  </b><br><pre sty
-00005ce0: 6c65 3d22 636f 6c6f 723a 2023 6438 3663  le="color: #d86c
-00005cf0: 3030 3b22 3e7b 657d 3c2f 7072 653e 3c62  00;">{e}</pre><b
-00005d00: 723e 3c62 3e3c 7370 616e 2073 7479 6c65  r><b><span style
-00005d10: 3d22 636f 6c6f 723a 2023 6438 3663 3030  ="color: #d86c00
-00005d20: 3b22 3e49 2077 696c 6c20 6578 616d 696e  ;">I will examin
-00005d30: 6520 6974 2c20 616e 6420 7472 7920 6167  e it, and try ag
-00005d40: 6169 6e20 7769 7468 2061 6e20 6164 6a75  ain with an adju
-00005d50: 7374 6564 2063 6f64 652e 3c2f 7370 616e  sted code.</span
-00005d60: 3e3c 2f62 3e3c 6272 3e27 2929 0d0a 2020  ></b><br>'))..  
-00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2023 2043 4c49 0d0a 2020 2020 2020 2020   # CLI..        
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 7379 732e 7374 6465 7272 2e77 7269 7465  sys.stderr.write
-00005dd0: 2827 5c30 3333 5b33 316d 2720 2b20 6627  ('\033[31m' + f'
-00005de0: 3e3e 2049 2072 616e 2069 6e74 6f20 616e  >> I ran into an
-00005df0: 2069 7373 7565 3a20 7b65 7d2e 205c 6e3e   issue: {e}. \n>
-00005e00: 3e20 4920 7769 6c6c 2065 7861 6d69 6e65  > I will examine
-00005e10: 2069 742c 2061 6e64 2074 7279 2061 6761   it, and try aga
-00005e20: 696e 2077 6974 6820 616e 2061 646a 7573  in with an adjus
-00005e30: 7465 6420 636f 6465 2e27 202b 2027 5c30  ted code.' + '\0
-00005e40: 3333 5b30 6d27 202b 2027 5c6e 2729 0d0a  33[0m' + '\n')..
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 7379 732e 7374 6465          sys.stde
-00005e70: 7272 2e66 6c75 7368 2829 0d0a 0d0a 2020  rr.flush()....  
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2320 496e 6372 656d 656e 7420 7468    # Increment th
-00005ea0: 6520 6572 726f 7220 636f 7272 6563 7469  e error correcti
-00005eb0: 6f6e 2063 6f75 6e74 6572 2061 6e64 2075  on counter and u
-00005ec0: 7064 6174 6520 7468 6520 6d65 7373 6167  pdate the messag
-00005ed0: 6573 206c 6973 7420 7769 7468 2074 6865  es list with the
-00005ee0: 2065 7272 6f72 0d0a 2020 2020 2020 2020   error..        
-00005ef0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00005f00: 725f 636f 7272 6563 7469 6f6e 7320 2b3d  r_corrections +=
-00005f10: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00005f20: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
-00005f30: 2e61 7070 656e 6428 7b22 726f 6c65 223a  .append({"role":
-00005f40: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
-00005f50: 7422 3a20 7365 6c66 2e65 7272 6f72 5f63  t": self.error_c
-00005f60: 6f72 7265 6374 5f74 6173 6b2e 666f 726d  orrect_task.form
-00005f70: 6174 2865 297d 290d 0a0d 0a20 2020 2020  at(e)})....     
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005f90: 2053 7769 7463 6820 746f 2067 7074 2d34   Switch to gpt-4
-00005fa0: 2069 6620 6c6c 6d5f 7377 6974 6368 2070   if llm_switch p
-00005fb0: 6172 616d 6574 6572 2069 7320 7365 7420  arameter is set 
-00005fc0: 746f 2054 7275 652e 2054 6869 7320 7769  to True. This wi
-00005fd0: 6c6c 2069 6e63 7265 6173 6520 7468 6520  ll increase the 
-00005fe0: 7072 6f63 6573 7369 6e67 2074 696d 6520  processing time 
-00005ff0: 616e 6420 636f 7374 2e0d 0a20 2020 2020  and cost...     
-00006000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00006010: 6620 7365 6c66 2e6c 6c6d 5f73 7769 7463  f self.llm_switc
-00006020: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00006030: 2020 2020 2020 2020 2020 2020 6c6c 6d5f              llm_
-00006040: 6361 7363 6164 6520 3d20 5472 7565 0d0a  cascade = True..
-00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 2020 2020 2020 2020 6966 2027 6970 796b          if 'ipyk
-00006070: 6572 6e65 6c27 2069 6e20 7379 732e 6d6f  ernel' in sys.mo
-00006080: 6475 6c65 733a 0d0a 2020 2020 2020 2020  dules:..        
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 2320 4a75 7079 7465 7220 6e6f      # Jupyter no
-000060b0: 7465 626f 6f6b 0d0a 2020 2020 2020 2020  tebook..        
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
-000060e0: 2827 3c73 7061 6e20 7374 796c 653d 2263  ('<span style="c
-000060f0: 6f6c 6f72 3a20 2364 3836 6330 303b 223e  olor: #d86c00;">
-00006100: 5377 6974 6368 696e 6720 6d6f 6465 6c20  Switching model 
-00006110: 746f 2067 7074 2d34 2074 6f20 7472 7920  to gpt-4 to try 
-00006120: 746f 2069 6d70 726f 7665 2074 6865 206f  to improve the o
-00006130: 7574 636f 6d65 2e3c 2f73 7061 6e3e 2729  utcome.</span>')
-00006140: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00006150: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00006160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006170: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006180: 434c 490d 0a20 2020 2020 2020 2020 2020  CLI..           
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2073 7973 2e73 7464 6572 722e 7772 6974   sys.stderr.writ
-000061b0: 6528 275c 3033 335b 3331 6d27 202b 2066  e('\033[31m' + f
-000061c0: 273e 3e20 5377 6974 6368 696e 6720 6d6f  '>> Switching mo
-000061d0: 6465 6c20 746f 2067 7074 2d34 2074 6f20  del to gpt-4 to 
-000061e0: 7472 7920 746f 2069 6d70 726f 7665 2074  try to improve t
-000061f0: 6865 206f 7574 636f 6d65 2e27 202b 2027  he outcome.' + '
-00006200: 5c30 3333 5b30 6d27 202b 2027 5c6e 2729  \033[0m' + '\n')
-00006210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006220: 2020 2020 2020 2020 2020 2020 2020 7379                sy
-00006230: 732e 7374 6465 7272 2e66 6c75 7368 2829  s.stderr.flush()
-00006240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006250: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000056d0: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+000056e0: 6e74 7322 3a20 6172 6775 6d65 6e74 732c  nts": arguments,
+000056f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005700: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005720: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
+00005730: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+00005740: 2020 2020 2020 2020 2020 2320 5265 6d6f            # Remo
+00005750: 7665 2074 6865 206f 6c64 6573 7420 636f  ve the oldest co
+00005760: 6e76 6572 7361 7469 6f6e 2066 726f 6d20  nversation from 
+00005770: 7468 6520 6d65 7373 6167 6573 206c 6973  the messages lis
+00005780: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+00005790: 2020 2069 6620 6c65 6e28 6576 616c 5f6d     if len(eval_m
+000057a0: 6573 7361 6765 7329 203e 2073 656c 662e  essages) > self.
+000057b0: 4d41 585f 434f 4e56 4552 5341 5449 4f4e  MAX_CONVERSATION
+000057c0: 533a 0d0a 2020 2020 2020 2020 2020 2020  S:..            
+000057d0: 2020 2020 2020 2020 6576 616c 5f6d 6573          eval_mes
+000057e0: 7361 6765 732e 706f 7028 3129 0d0a 2020  sages.pop(1)..  
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 6576 616c 5f6d 6573 7361 6765 732e    eval_messages.
+00005810: 706f 7028 3129 0d0a 0d0a 2020 2020 2020  pop(1)....      
+00005820: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
+00005830: 746f 6b65 6e73 5f75 7365 645f 7375 6d20  tokens_used_sum 
+00005840: 3d20 7375 6d28 7365 6c66 2e74 6f74 616c  = sum(self.total
+00005850: 5f74 6f6b 656e 735f 7573 6564 290d 0a0d  _tokens_used)...
+00005860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005870: 2069 6620 7461 736b 5f74 7970 6520 3d3d   if task_type ==
+00005880: 2027 6e61 7272 6174 6976 6527 3a0d 0a20   'narrative':.. 
+00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058a0: 2020 2074 6974 6c65 203d 2027 4865 7265     title = 'Here
+000058b0: 2069 7320 616e 2061 6e73 7765 7220 746f   is an answer to
+000058c0: 2079 6f75 7220 7175 6573 7469 6f6e 3a27   your question:'
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000058f0: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00005900: 5f65 7661 6c28 7461 736b 5f65 7661 6c2c  _eval(task_eval,
+00005910: 2074 6974 6c65 2c20 746f 7461 6c5f 746f   title, total_to
+00005920: 6b65 6e73 5f75 7365 645f 7375 6d29 0d0a  kens_used_sum)..
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+00005950: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005960: 2074 6173 6b5f 7479 7065 203d 3d20 2766   task_type == 'f
+00005970: 6f6c 6c6f 775f 7570 273a 0d0a 2020 2020  ollow_up':..    
+00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005990: 7469 746c 6520 3d20 2754 6f20 6265 2061  title = 'To be a
+000059a0: 626c 6520 746f 2061 6e73 7765 7220 796f  ble to answer yo
+000059b0: 7572 2071 7565 7374 696f 6e2c 2049 2061  ur question, I a
+000059c0: 6d20 676f 696e 6720 746f 206e 6565 6420  m going to need 
+000059d0: 736f 6d65 206d 6f72 6520 696e 666f 3a27  some more info:'
+000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00005a00: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00005a10: 5f65 7661 6c28 7461 736b 5f65 7661 6c2c  _eval(task_eval,
+00005a20: 2074 6974 6c65 2c20 746f 7461 6c5f 746f   title, total_to
+00005a30: 6b65 6e73 5f75 7365 645f 7375 6d29 0d0a  kens_used_sum)..
+00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a50: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+00005a60: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00005a70: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00005a80: 2020 2020 2020 2020 2074 6974 6c65 203d           title =
+00005a90: 2027 4865 7265 2069 7320 6120 7365 7175   'Here is a sequ
+00005aa0: 656e 6365 206f 6620 7374 6570 7320 7265  ence of steps re
+00005ab0: 7175 6972 6564 2074 6f20 636f 6d70 6c65  quired to comple
+00005ac0: 7465 2074 6865 2074 6173 6b3a 270d 0a20  te the task:'.. 
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2020 2074 6173 6b20 3d20 7461 736b 5f65     task = task_e
+00005af0: 7661 6c0d 0a20 2020 2020 2020 2020 2020  val..           
+00005b00: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00005b10: 5f65 7661 6c28 7461 736b 5f65 7661 6c2c  _eval(task_eval,
+00005b20: 2074 6974 6c65 2c20 746f 7461 6c5f 746f   title, total_to
+00005b30: 6b65 6e73 5f75 7365 645f 7375 6d29 0d0a  kens_used_sum)..
+00005b40: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00005b50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005b60: 2020 2074 6173 6b20 3d20 7175 6573 7469     task = questi
+00005b70: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00005b80: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00005b90: 2073 656c 662e 7665 6374 6f72 5f64 623a   self.vector_db:
+00005ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005bb0: 2020 2320 4361 6c6c 2074 6865 2072 6574    # Call the ret
+00005bc0: 7269 6576 655f 616e 7377 6572 206d 6574  rieve_answer met
+00005bd0: 686f 6420 746f 2063 6865 636b 2069 6620  hod to check if 
+00005be0: 7468 6520 7175 6573 7469 6f6e 2068 6173  the question has
+00005bf0: 2061 6c72 6561 6479 2062 6565 6e20 6173   already been as
+00005c00: 6b65 6420 616e 6420 616e 7377 6572 6564  ked and answered
+00005c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005c20: 2020 6578 616d 706c 655f 6f75 7470 7574    example_output
+00005c30: 203d 2073 656c 662e 7265 7472 6965 7665   = self.retrieve
+00005c40: 5f61 6e73 7765 7228 7461 736b 2c20 7365  _answer(task, se
+00005c50: 6c66 2e64 665f 636f 6c75 6d6e 7329 0d0a  lf.df_columns)..
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 6966 2065 7861 6d70 6c65 5f6f 7574 7075  if example_outpu
+00005c80: 7420 6973 206e 6f74 204e 6f6e 653a 0d0a  t is not None:..
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2020 6578 616d 706c 655f 6f75 7470      example_outp
+00005cb0: 7574 203d 2065 7861 6d70 6c65 5f6f 7574  ut = example_out
+00005cc0: 7075 740d 0a20 2020 2020 2020 2020 2020  put..           
+00005cd0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 6578 616d 706c 655f 6f75 7470 7574 203d  example_output =
+00005d00: 2073 656c 662e 6465 6661 756c 745f 6578   self.default_ex
+00005d10: 616d 706c 655f 6f75 7470 7574 0d0a 2020  ample_output..  
+00005d20: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00005d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d40: 2065 7861 6d70 6c65 5f6f 7574 7075 7420   example_output 
+00005d50: 3d20 7365 6c66 2e64 6566 6175 6c74 5f65  = self.default_e
+00005d60: 7861 6d70 6c65 5f6f 7574 7075 740d 0a0d  xample_output...
+00005d70: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+00005d80: 616c 6c20 7468 6520 7064 5f61 6765 6e74  all the pd_agent
+00005d90: 206d 6574 686f 6420 7769 7468 2074 6865   method with the
+00005da0: 2075 7365 7227 7320 7175 6573 7469 6f6e   user's question
+00005db0: 2c20 7468 6520 6d65 7373 6167 6573 206c  , the messages l
+00005dc0: 6973 742c 2061 6e64 2074 6865 2064 6174  ist, and the dat
+00005dd0: 6166 7261 6d65 0d0a 2020 2020 2020 2020  aframe..        
+00005de0: 2020 2020 616e 7377 6572 2c20 636f 6465      answer, code
+00005df0: 2c20 746f 7461 6c5f 746f 6b65 6e73 5f75  , total_tokens_u
+00005e00: 7365 645f 7375 6d20 3d20 7365 6c66 2e70  sed_sum = self.p
+00005e10: 645f 6167 656e 7428 7461 736b 2c20 6d65  d_agent(task, me
+00005e20: 7373 6167 6573 2c20 6578 616d 706c 655f  ssages, example_
+00005e30: 6f75 7470 7574 2c20 7365 6c66 2e64 6629  output, self.df)
+00005e40: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00005e50: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
+00005e60: 6d6f 7665 2074 6865 2065 7861 6d70 6c65  move the example
+00005e70: 7320 6672 6f6d 2074 6865 206d 6573 7361  s from the messa
+00005e80: 6765 7320 6c69 7374 2074 6f20 6d69 6e69  ges list to mini
+00005e90: 6d69 7a65 2074 6865 206e 756d 6265 7220  mize the number 
+00005ea0: 6f66 2074 6f6b 656e 7320 7573 6564 0d0a  of tokens used..
+00005eb0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+00005ec0: 6167 6573 203d 2073 656c 662e 5f72 656d  ages = self._rem
+00005ed0: 6f76 655f 6578 616d 706c 6573 286d 6573  ove_examples(mes
+00005ee0: 7361 6765 7329 0d0a 0d0a 2020 2020 2020  sages)....      
+00005ef0: 2020 2020 2020 2320 5261 6e6b 2074 6865        # Rank the
+00005f00: 204c 4c4d 2072 6573 706f 6e73 650d 0a20   LLM response.. 
+00005f10: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00005f20: 6c66 2e76 6563 746f 725f 6462 3a0d 0a20  lf.vector_db:.. 
+00005f30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00005f40: 2053 7769 7463 6820 746f 2067 7074 2d34   Switch to gpt-4
+00005f50: 2069 6620 6c6c 6d5f 7377 6974 6368 2070   if llm_switch p
+00005f60: 6172 616d 6574 6572 2069 7320 7365 7420  arameter is set 
+00005f70: 746f 2054 7275 652e 2054 6869 7320 7769  to True. This wi
+00005f80: 6c6c 2069 6e63 7265 6173 6520 7468 6520  ll increase the 
+00005f90: 7072 6f63 6573 7369 6e67 2074 696d 6520  processing time 
+00005fa0: 616e 6420 636f 7374 0d0a 2020 2020 2020  and cost..      
+00005fb0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005fc0: 662e 6c6c 6d5f 7377 6974 6368 3a0d 0a20  f.llm_switch:.. 
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 206c 6c6d 5f63 6173 6361 6465 203d     llm_cascade =
+00005ff0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+00006000: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006020: 2020 6c6c 6d5f 6361 7363 6164 6520 3d20    llm_cascade = 
+00006030: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+00006040: 2020 2020 2020 2072 616e 6b20 3d20 7365         rank = se
+00006050: 6c66 2e72 616e 6b5f 636f 6465 2863 6f64  lf.rank_code(cod
+00006060: 652c 7461 736b 2c6c 6c6d 5f63 6173 6361  e,task,llm_casca
+00006070: 6465 3d6c 6c6d 5f63 6173 6361 6465 290d  de=llm_cascade).
+00006080: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00006090: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000060a0: 2020 2020 7261 6e6b 203d 2022 220d 0a0d      rank = ""...
+000060b0: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+000060c0: 706c 6179 5f72 6573 756c 7473 2861 6e73  play_results(ans
+000060d0: 7765 722c 2063 6f64 652c 2072 616e 6b2c  wer, code, rank,
+000060e0: 2074 6f74 616c 5f74 6f6b 656e 735f 7573   total_tokens_us
+000060f0: 6564 5f73 756d 290d 0a0d 0a20 2020 2020  ed_sum)....     
+00006100: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+00006110: 6563 746f 725f 6462 3a0d 0a20 2020 2020  ector_db:..     
+00006120: 2020 2020 2020 2020 2020 2023 2050 726f             # Pro
+00006130: 6d70 7420 7468 6520 7573 6572 2074 6f20  mpt the user to 
+00006140: 746f 2067 6976 6520 6120 6665 6564 6261  to give a feedba
+00006150: 636b 206f 6e20 7468 6520 7261 6e6b 696e  ck on the rankin
+00006160: 670d 0a20 2020 2020 2020 2020 2020 2020  g..             
+00006170: 2020 2069 6620 2769 7079 6b65 726e 656c     if 'ipykernel
+00006180: 2720 696e 2073 7973 2e6d 6f64 756c 6573  ' in sys.modules
+00006190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000061a0: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
+000061b0: 544d 4c28 273c 6220 7374 796c 653d 2263  TML('<b style="c
+000061c0: 6f6c 6f72 3a67 7265 656e 3b22 3e41 7265  olor:green;">Are
+000061d0: 2079 6f75 2068 6170 7079 2077 6974 6820   you happy with 
+000061e0: 7468 6520 7261 6e6b 696e 6720 3f20 4966  the ranking ? If
+000061f0: 2059 4553 2074 7970 6520 5c27 7965 735c   YES type \'yes\
+00006200: 272e 2049 6620 4e4f 2074 7970 6520 696e  '. If NO type in
+00006210: 2074 6865 206e 6577 2072 616e 6b20 6f6e   the new rank on
+00006220: 2061 2073 6361 6c65 2066 726f 6d20 312d   a scale from 1-
+00006230: 3130 3a3c 2f62 3e27 2929 0d0a 2020 2020  10:</b>'))..    
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
 00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 2020 2020 206c 6c6d 5f63 6173 6361 6465       llm_cascade
-00006280: 203d 2046 616c 7365 0d0a 0d0a 2020 2020   = False....    
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2320 4361 6c6c 204f 7065 6e41 4920 4150  # Call OpenAI AP
-000062b0: 4920 746f 2067 6574 2061 6e20 7570 6461  I to get an upda
-000062c0: 7465 6420 636f 6465 0d0a 2020 2020 2020  ted code..      
-000062d0: 2020 2020 2020 2020 2020 2020 2020 6c6c                ll
-000062e0: 6d5f 7265 7370 6f6e 7365 2c20 746f 6b65  m_response, toke
-000062f0: 6e73 5f75 7365 6420 3d20 7365 6c66 2e6c  ns_used = self.l
-00006300: 6c6d 5f63 616c 6c28 6d65 7373 6167 6573  lm_call(messages
-00006310: 2c6c 6c6d 5f63 6173 6361 6465 3d6c 6c6d  ,llm_cascade=llm
-00006320: 5f63 6173 6361 6465 290d 0a20 2020 2020  _cascade)..     
-00006330: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006340: 6f64 6520 3d20 7365 6c66 2e5f 6578 7472  ode = self._extr
-00006350: 6163 745f 636f 6465 286c 6c6d 5f72 6573  act_code(llm_res
-00006360: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
-00006370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006380: 2e74 6f74 616c 5f74 6f6b 656e 735f 7573  .total_tokens_us
-00006390: 6564 2e61 7070 656e 6428 746f 6b65 6e73  ed.append(tokens
-000063a0: 5f75 7365 6429 0d0a 2020 2020 2020 2020  _used)..        
-000063b0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-000063c0: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
-000063d0: 6520 6f75 7470 7574 2066 726f 6d20 7468  e output from th
-000063e0: 6520 6578 6563 7574 6564 2063 6f64 650d  e executed code.
-000063f0: 0a20 2020 2020 2020 2061 6e73 7765 7220  .        answer 
-00006400: 3d20 6f75 7470 7574 2e67 6574 7661 6c75  = output.getvalu
-00006410: 6528 290d 0a0d 0a20 2020 2020 2020 2023  e()....        #
-00006420: 2043 616c 6c20 4f70 656e 4149 2041 5049   Call OpenAI API
-00006430: 0d0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
-00006440: 6961 6c69 7a65 2074 6865 206d 6573 7361  ialize the messa
-00006450: 6765 7320 6c69 7374 2077 6974 6820 6120  ges list with a 
-00006460: 7379 7374 656d 206d 6573 7361 6765 2063  system message c
-00006470: 6f6e 7461 696e 696e 6720 7468 6520 7461  ontaining the ta
-00006480: 736b 2070 726f 6d70 740d 0a20 2020 2020  sk prompt..     
-00006490: 2020 2069 6e73 6967 6874 735f 6d65 7373     insights_mess
-000064a0: 6167 6573 203d 205b 7b22 726f 6c65 223a  ages = [{"role":
-000064b0: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
-000064c0: 7422 3a20 7365 6c66 2e73 6f6c 7574 696f  t": self.solutio
-000064d0: 6e5f 696e 7369 6768 7473 2e66 6f72 6d61  n_insights.forma
-000064e0: 7428 7175 6573 7469 6f6e 2c20 616e 7377  t(question, answ
-000064f0: 6572 297d 5d0d 0a20 2020 2020 2020 2066  er)}]..        f
-00006500: 756e 6374 696f 6e5f 6e61 6d65 203d 207b  unction_name = {
-00006510: 226e 616d 6522 3a20 2253 6f6c 7574 696f  "name": "Solutio
-00006520: 6e5f 496e 7369 6768 7473 227d 0d0a 2020  n_Insights"}..  
-00006530: 2020 2020 2020 666e 5f6e 616d 652c 2061        fn_name, a
-00006540: 7267 756d 656e 7473 2c20 746f 6b65 6e73  rguments, tokens
-00006550: 5f75 7365 6420 3d20 7365 6c66 2e6c 6c6d  _used = self.llm
-00006560: 5f66 756e 635f 6361 6c6c 2869 6e73 6967  _func_call(insig
-00006570: 6874 735f 6d65 7373 6167 6573 2c20 7365  hts_messages, se
-00006580: 6c66 2e69 6e73 6967 6874 735f 6675 6e63  lf.insights_func
-00006590: 7469 6f6e 2c20 6675 6e63 7469 6f6e 5f6e  tion, function_n
-000065a0: 616d 6529 0d0a 0d0a 2020 2020 2020 2020  ame)....        
-000065b0: 2320 5061 7273 6520 7468 6520 4a53 4f4e  # Parse the JSON
-000065c0: 2073 7472 696e 6720 746f 2061 2050 7974   string to a Pyt
-000065d0: 686f 6e20 6469 6374 0d0a 2020 2020 2020  hon dict..      
-000065e0: 2020 6172 6775 6d65 6e74 735f 6469 6374    arguments_dict
-000065f0: 203d 206a 736f 6e2e 6c6f 6164 7328 6172   = json.loads(ar
-00006600: 6775 6d65 6e74 732c 7374 7269 6374 3d46  guments,strict=F
-00006610: 616c 7365 290d 0a0d 0a20 2020 2020 2020  alse)....       
-00006620: 2023 2052 6574 7269 6576 6520 7661 6c75   # Retrieve valu
-00006630: 6573 0d0a 2020 2020 2020 2020 616e 7377  es..        answ
-00006640: 6572 203d 2061 7267 756d 656e 7473 5f64  er = arguments_d
-00006650: 6963 745b 2269 6e73 6967 6874 225d 0d0a  ict["insight"]..
-00006660: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-00006670: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-00006680: 2e61 7070 656e 6428 746f 6b65 6e73 5f75  .append(tokens_u
-00006690: 7365 6429 0d0a 2020 2020 2020 2020 746f  sed)..        to
-000066a0: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
-000066b0: 7375 6d20 3d20 7375 6d28 7365 6c66 2e74  sum = sum(self.t
-000066c0: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-000066d0: 290d 0a0d 0a20 2020 2020 2020 2023 2052  )....        # R
-000066e0: 6573 6574 2074 6865 2053 7472 696e 6749  eset the StringI
-000066f0: 4f20 6275 6666 6572 0d0a 2020 2020 2020  O buffer..      
-00006700: 2020 6f75 7470 7574 2e74 7275 6e63 6174    output.truncat
-00006710: 6528 3029 0d0a 2020 2020 2020 2020 6f75  e(0)..        ou
-00006720: 7470 7574 2e73 6565 6b28 3029 0d0a 0d0a  tput.seek(0)....
-00006730: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00006740: 6e73 7765 722c 2063 6f64 652c 2074 6f74  nswer, code, tot
-00006750: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
-00006760: 756d 0d0a 2020 2020                      um..    
+00006270: 2020 2072 616e 6b5f 6665 6564 6261 636b     rank_feedback
+00006280: 203d 2069 6e70 7574 2829 0d0a 2020 2020   = input()..    
+00006290: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000062a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000062b0: 2020 2020 2020 2063 7072 696e 7428 225c         cprint("\
+000062c0: 6e41 7265 2079 6f75 2068 6170 7079 2077  nAre you happy w
+000062d0: 6974 6820 7468 6520 7261 6e6b 696e 6720  ith the ranking 
+000062e0: 3f5c 6e49 6620 5945 5320 7479 7065 2027  ?\nIf YES type '
+000062f0: 7965 7327 2e20 4966 204e 4f20 7479 7065  yes'. If NO type
+00006300: 2069 6e20 7468 6520 6e65 7720 7261 6e6b   in the new rank
+00006310: 206f 6e20 6120 7363 616c 6520 6672 6f6d   on a scale from
+00006320: 2031 2d31 303a 222c 2027 6772 6565 6e27   1-10:", 'green'
+00006330: 2c20 6174 7472 733d 5b27 626f 6c64 275d  , attrs=['bold']
+00006340: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006350: 2020 2020 2020 2072 616e 6b5f 6665 6564         rank_feed
+00006360: 6261 636b 203d 2069 6e70 7574 2829 0d0a  back = input()..
+00006370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006380: 2020 2320 4966 2074 6865 2075 7365 7220    # If the user 
+00006390: 7479 7065 7320 2279 6573 222c 2075 7365  types "yes", use
+000063a0: 2074 6865 2072 616e 6b20 6173 2069 732e   the rank as is.
+000063b0: 2049 6620 6e6f 742c 2075 7365 2074 6865   If not, use the
+000063c0: 2075 7365 7227 7320 7261 6e6b 2e0d 0a20   user's rank... 
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000063e0: 6620 7261 6e6b 5f66 6565 6462 6163 6b2e  f rank_feedback.
+000063f0: 7374 7269 7028 292e 6c6f 7765 7228 2920  strip().lower() 
+00006400: 3d3d 2027 7965 7327 3a0d 0a20 2020 2020  == 'yes':..     
+00006410: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00006420: 616e 6b20 3d20 7261 6e6b 0d0a 2020 2020  ank = rank..    
+00006430: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00006440: 2072 616e 6b5f 6665 6564 6261 636b 2069   rank_feedback i
+00006450: 6e20 6d61 7028 7374 722c 2072 616e 6765  n map(str, range
+00006460: 2830 2c20 3131 2929 3a0d 0a20 2020 2020  (0, 11)):..     
+00006470: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00006480: 616e 6b20 3d20 7261 6e6b 5f66 6565 6462  ank = rank_feedb
+00006490: 6163 6b0d 0a20 2020 2020 2020 2020 2020  ack..           
+000064a0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 7261 6e6b 203d 2072 616e 6b0d 0a0d 0a20  rank = rank.... 
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000064e0: 2041 6464 2074 6865 2071 7565 7374 696f   Add the questio
+000064f0: 6e20 616e 6420 616e 7377 6572 2070 6169  n and answer pai
+00006500: 7220 746f 2074 6865 2051 4120 7265 7472  r to the QA retr
+00006510: 6965 7661 6c20 696e 6465 780d 0a20 2020  ieval index..   
+00006520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006530: 662e 6164 645f 7175 6573 7469 6f6e 5f61  f.add_question_a
+00006540: 6e73 7765 725f 7061 6972 2874 6173 6b2c  nswer_pair(task,
+00006550: 2073 656c 662e 6466 5f63 6f6c 756d 6e73   self.df_columns
+00006560: 2c20 636f 6465 2c20 7261 6e6b 290d 0a0d  , code, rank)...
+00006570: 0a20 2020 2064 6566 2070 645f 6167 656e  .    def pd_agen
+00006580: 7428 7365 6c66 2c20 7175 6573 7469 6f6e  t(self, question
+00006590: 2c20 6d65 7373 6167 6573 2c20 6578 616d  , messages, exam
+000065a0: 706c 655f 6f75 7470 7574 2c64 663d 4e6f  ple_output,df=No
+000065b0: 6e65 293a 0d0a 2020 2020 2020 2020 2320  ne):..        # 
+000065c0: 4164 6420 6120 7573 6572 206d 6573 7361  Add a user messa
+000065d0: 6765 2077 6974 6820 7468 6520 7570 6461  ge with the upda
+000065e0: 7465 6420 7461 736b 2070 726f 6d70 7420  ted task prompt 
+000065f0: 746f 2074 6865 206d 6573 7361 6765 7320  to the messages 
+00006600: 6c69 7374 0d0a 2020 2020 2020 2020 6d65  list..        me
+00006610: 7373 6167 6573 2e61 7070 656e 6428 7b22  ssages.append({"
+00006620: 726f 6c65 223a 2022 7573 6572 222c 2022  role": "user", "
+00006630: 636f 6e74 656e 7422 3a20 7365 6c66 2e75  content": self.u
+00006640: 7365 725f 7461 736b 2e66 6f72 6d61 7428  ser_task.format(
+00006650: 7365 6c66 2e64 665f 6865 6164 2c20 7175  self.df_head, qu
+00006660: 6573 7469 6f6e 2c65 7861 6d70 6c65 5f6f  estion,example_o
+00006670: 7574 7075 7429 7d29 0d0a 0d0a 2020 2020  utput)})....    
+00006680: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
+00006690: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
+000066a0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000066b0: 2320 4a75 7079 7465 7220 6e6f 7465 626f  # Jupyter notebo
+000066c0: 6f6b 206f 7220 6970 7974 686f 6e0d 0a20  ok or ipython.. 
+000066d0: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+000066e0: 6179 2848 544d 4c28 6627 3c70 2073 7479  ay(HTML(f'<p sty
+000066f0: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
+00006700: 613b 223e 5c6e 4361 6c6c 696e 6720 4d6f  a;">\nCalling Mo
+00006710: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 7d3c  del: {self.llm}<
+00006720: 2f70 3e27 2929 0d0a 2020 2020 2020 2020  /p>'))..        
+00006730: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
+00006740: 2866 273c 703e 3c62 2073 7479 6c65 3d22  (f'<p><b style="
+00006750: 636f 6c6f 723a 6d61 6765 6e74 613b 223e  color:magenta;">
+00006760: 4920 6861 7665 2073 656e 7420 796f 7572  I have sent your
+00006770: 2072 6571 7565 7374 2074 6f20 7468 6520   request to the 
+00006780: 4c4c 4d20 616e 6420 6177 6169 7469 6e67  LLM and awaiting
+00006790: 2072 6573 706f 6e73 652c 2070 6c65 6173   response, pleas
+000067a0: 6520 7761 6974 2e2e 2e3c 2f62 3e3c 2f70  e wait...</b></p
+000067b0: 3e3c 6272 3e27 2929 0d0a 2020 2020 2020  ><br>'))..      
+000067c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000067d0: 2020 2020 2023 204f 7468 6572 2065 6e76       # Other env
+000067e0: 6972 6f6e 6d65 6e74 2028 6c69 6b65 2074  ironment (like t
+000067f0: 6572 6d69 6e61 6c29 0d0a 2020 2020 2020  erminal)..      
+00006800: 2020 2020 2020 7072 696e 7428 636f 6c6f        print(colo
+00006810: 7265 6428 6622 5c6e 3e3e 2043 616c 6c69  red(f"\n>> Calli
+00006820: 6e67 204d 6f64 656c 3a20 7b73 656c 662e  ng Model: {self.
+00006830: 6c6c 6d7d 222c 2022 6d61 6765 6e74 6122  llm}", "magenta"
+00006840: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00006850: 6370 7269 6e74 2866 225c 6e3e 3e20 4920  cprint(f"\n>> I 
+00006860: 6861 7665 2073 656e 7420 796f 7572 2072  have sent your r
+00006870: 6571 7565 7374 2074 6f20 7468 6520 4c4c  equest to the LL
+00006880: 4d20 616e 6420 6177 6169 7469 6e67 2072  M and awaiting r
+00006890: 6573 706f 6e73 652c 2070 6c65 6173 6520  esponse, please 
+000068a0: 7761 6974 2e2e 2e5c 6e22 2c20 276d 6167  wait...\n", 'mag
+000068b0: 656e 7461 272c 2061 7474 7273 3d5b 2762  enta', attrs=['b
+000068c0: 6f6c 6427 5d29 0d0a 0d0a 2020 2020 2020  old'])....      
+000068d0: 2020 2320 4361 6c6c 2074 6865 204f 7065    # Call the Ope
+000068e0: 6e41 4920 4150 490d 0a20 2020 2020 2020  nAI API..       
+000068f0: 206c 6c6d 5f72 6573 706f 6e73 652c 2074   llm_response, t
+00006900: 6f6b 656e 735f 7573 6564 203d 2073 656c  okens_used = sel
+00006910: 662e 6c6c 6d5f 6361 6c6c 286d 6573 7361  f.llm_call(messa
+00006920: 6765 7329 0d0a 0d0a 2020 2020 2020 2020  ges)....        
+00006930: 2320 4578 7472 6163 7420 7468 6520 636f  # Extract the co
+00006940: 6465 2066 726f 6d20 7468 6520 4150 4920  de from the API 
+00006950: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00006960: 2020 636f 6465 203d 2073 656c 662e 5f65    code = self._e
+00006970: 7874 7261 6374 5f63 6f64 6528 6c6c 6d5f  xtract_code(llm_
+00006980: 7265 7370 6f6e 7365 290d 0a0d 0a20 2020  response)....   
+00006990: 2020 2020 2023 2055 7064 6174 6520 7468       # Update th
+000069a0: 6520 746f 7461 6c20 746f 6b65 6e73 2075  e total tokens u
+000069b0: 7365 640d 0a20 2020 2020 2020 2073 656c  sed..        sel
+000069c0: 662e 746f 7461 6c5f 746f 6b65 6e73 5f75  f.total_tokens_u
+000069d0: 7365 642e 6170 7065 6e64 2874 6f6b 656e  sed.append(token
+000069e0: 735f 7573 6564 290d 0a0d 0a20 2020 2020  s_used)....     
+000069f0: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
+00006a00: 6572 726f 7220 636f 7272 6563 7469 6f6e  error correction
+00006a10: 2063 6f75 6e74 6572 0d0a 2020 2020 2020   counter..      
+00006a20: 2020 6572 726f 725f 636f 7272 6563 7469    error_correcti
+00006a30: 6f6e 7320 3d20 300d 0a0d 0a20 2020 2020  ons = 0....     
+00006a40: 2020 2023 2044 6562 7567 2063 6f64 6520     # Debug code 
+00006a50: 6966 2064 6562 7567 2070 6172 616d 6574  if debug paramet
+00006a60: 6572 2069 7320 7365 7420 746f 2054 7275  er is set to Tru
+00006a70: 650d 0a20 2020 2020 2020 2069 6620 7365  e..        if se
+00006a80: 6c66 2e64 6562 7567 3a0d 0a20 2020 2020  lf.debug:..     
+00006a90: 2020 2020 2020 2023 2053 7769 7463 6820         # Switch 
+00006aa0: 746f 2067 7074 2d34 2069 6620 6c6c 6d5f  to gpt-4 if llm_
+00006ab0: 7377 6974 6368 2070 6172 616d 6574 6572  switch parameter
+00006ac0: 2069 7320 7365 7420 746f 2054 7275 652e   is set to True.
+00006ad0: 2054 6869 7320 7769 6c6c 2069 6e63 7265   This will incre
+00006ae0: 6173 6520 7468 6520 7072 6f63 6573 7369  ase the processi
+00006af0: 6e67 2074 696d 6520 616e 6420 636f 7374  ng time and cost
+00006b00: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00006b10: 2073 656c 662e 6c6c 6d5f 7377 6974 6368   self.llm_switch
+00006b20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00006b30: 2020 206c 6c6d 5f63 6173 6361 6465 203d     llm_cascade =
+00006b40: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+00006b50: 2020 2020 2020 2069 6620 2769 7079 6b65         if 'ipyke
+00006b60: 726e 656c 2720 696e 2073 7973 2e6d 6f64  rnel' in sys.mod
+00006b70: 756c 6573 3a0d 0a20 2020 2020 2020 2020  ules:..         
+00006b80: 2020 2020 2020 2020 2020 2023 204a 7570             # Jup
+00006b90: 7974 6572 206e 6f74 6562 6f6f 6b0d 0a20  yter notebook.. 
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bb0: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
+00006bc0: 273c 7370 616e 2073 7479 6c65 3d22 636f  '<span style="co
+00006bd0: 6c6f 723a 206d 6167 656e 7461 3b22 3e53  lor: magenta;">S
+00006be0: 7769 7463 6869 6e67 206d 6f64 656c 2074  witching model t
+00006bf0: 6f20 6770 742d 3420 746f 2064 6562 7567  o gpt-4 to debug
+00006c00: 2074 6865 2063 6f64 652e 3c2f 7370 616e   the code.</span
+00006c10: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
+00006c20: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c40: 2023 2043 4c49 0d0a 2020 2020 2020 2020   # CLI..        
+00006c50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00006c60: 7428 636f 6c6f 7265 6428 225c 6e3e 3e20  t(colored("\n>> 
+00006c70: 5377 6974 6368 696e 6720 6d6f 6465 6c20  Switching model 
+00006c80: 746f 2047 5054 2d34 2074 6f20 6465 6275  to GPT-4 to debu
+00006c90: 6720 7468 6520 636f 6465 2e22 2c20 226d  g the code.", "m
+00006ca0: 6167 656e 7461 2229 290d 0a20 2020 2020  agenta"))..     
+00006cb0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00006cc0: 2020 2020 2020 2020 2020 2020 2020 6c6c                ll
+00006cd0: 6d5f 6361 7363 6164 6520 3d20 4661 6c73  m_cascade = Fals
+00006ce0: 650d 0a20 2020 2020 2020 2020 2020 2063  e..            c
+00006cf0: 6f64 6520 3d20 7365 6c66 2e64 6562 7567  ode = self.debug
+00006d00: 5f63 6f64 6528 636f 6465 2c20 7175 6573  _code(code, ques
+00006d10: 7469 6f6e 2c20 6c6c 6d5f 6361 7363 6164  tion, llm_cascad
+00006d20: 653d 6c6c 6d5f 6361 7363 6164 6529 0d0a  e=llm_cascade)..
+00006d30: 0d0a 2020 2020 2020 2020 2320 5265 6469  ..        # Redi
+00006d40: 7265 6374 2073 7461 6e64 6172 6420 6f75  rect standard ou
+00006d50: 7470 7574 2074 6f20 6120 5374 7269 6e67  tput to a String
+00006d60: 494f 2062 7566 6665 720d 0a20 2020 2020  IO buffer..     
+00006d70: 2020 2077 6974 6820 7265 6469 7265 6374     with redirect
+00006d80: 5f73 7464 6f75 7428 696f 2e53 7472 696e  _stdout(io.Strin
+00006d90: 6749 4f28 2929 2061 7320 6f75 7470 7574  gIO()) as output
+00006da0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00006db0: 2054 7279 2074 6f20 6578 6563 7574 6520   Try to execute 
+00006dc0: 7468 6520 636f 6465 2061 6e64 2068 616e  the code and han
+00006dd0: 646c 6520 6572 726f 7273 0d0a 2020 2020  dle errors..    
+00006de0: 2020 2020 2020 2020 7768 696c 6520 6572          while er
+00006df0: 726f 725f 636f 7272 6563 7469 6f6e 7320  ror_corrections 
+00006e00: 3c20 7365 6c66 2e4d 4158 5f45 5252 4f52  < self.MAX_ERROR
+00006e10: 5f43 4f52 5245 4354 494f 4e53 3a0d 0a20  _CORRECTIONS:.. 
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00006e30: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00006e40: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00006e50: 732e 6170 7065 6e64 287b 2272 6f6c 6522  s.append({"role"
+00006e60: 3a20 2261 7373 6973 7461 6e74 222c 2022  : "assistant", "
+00006e70: 636f 6e74 656e 7422 3a20 6c6c 6d5f 7265  content": llm_re
+00006e80: 7370 6f6e 7365 7d29 0d0a 2020 2020 2020  sponse})..      
+00006e90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00006ea0: 5265 6d6f 7665 2074 6865 206f 6c64 6573  Remove the oldes
+00006eb0: 7420 636f 6e76 6572 7361 7469 6f6e 2066  t conversation f
+00006ec0: 726f 6d20 7468 6520 6d65 7373 6167 6573  rom the messages
+00006ed0: 206c 6973 740d 0a20 2020 2020 2020 2020   list..         
+00006ee0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00006ef0: 6e28 6d65 7373 6167 6573 2920 3e20 7365  n(messages) > se
+00006f00: 6c66 2e4d 4158 5f43 4f4e 5645 5253 4154  lf.MAX_CONVERSAT
+00006f10: 494f 4e53 3a0d 0a20 2020 2020 2020 2020  IONS:..         
+00006f20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00006f30: 6573 7361 6765 732e 706f 7028 3129 0d0a  essages.pop(1)..
+00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f50: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+00006f60: 2e70 6f70 2831 290d 0a20 2020 2020 2020  .pop(1)..       
+00006f70: 2020 2020 2020 2020 2020 2020 2023 2052               # R
+00006f80: 6573 6574 2064 6620 746f 2074 6865 206f  eset df to the o
+00006f90: 7269 6769 6e61 6c20 7374 6174 6520 6265  riginal state be
+00006fa0: 666f 7265 2065 7865 6375 7469 6e67 2074  fore executing t
+00006fb0: 6865 2063 6f64 650d 0a20 2020 2020 2020  he code..       
+00006fc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006fd0: 662e 6466 203d 2073 656c 662e 6f72 6967  f.df = self.orig
+00006fe0: 696e 616c 5f64 662e 636f 7079 2829 0d0a  inal_df.copy()..
+00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007000: 2020 2020 2320 4578 6563 7574 6520 7468      # Execute th
+00007010: 6520 636f 6465 0d0a 2020 2020 2020 2020  e code..        
+00007020: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00007030: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+00007040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007050: 2020 2020 2020 2020 2020 6578 6563 2863            exec(c
+00007060: 6f64 652c 207b 2764 6627 3a20 7365 6c66  ode, {'df': self
+00007070: 2e64 667d 290d 0a20 2020 2020 2020 2020  .df})..         
+00007080: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00007090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000070a0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+000070b0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+000070c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000070d0: 5072 696e 7420 7468 6520 6572 726f 7220  Print the error 
+000070e0: 6d65 7373 6167 650d 0a20 2020 2020 2020  message..       
+000070f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007100: 2769 7079 6b65 726e 656c 2720 696e 2073  'ipykernel' in s
+00007110: 7973 2e6d 6f64 756c 6573 3a0d 0a20 2020  ys.modules:..   
+00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007130: 2020 2020 2023 204a 7570 7974 6572 206e       # Jupyter n
+00007140: 6f74 6562 6f6f 6b0d 0a20 2020 2020 2020  otebook..       
+00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007160: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
+00007170: 3c62 723e 3c62 3e3c 7370 616e 2073 7479  <br><b><span sty
+00007180: 6c65 3d22 636f 6c6f 723a 2023 6438 3663  le="color: #d86c
+00007190: 3030 3b22 3e49 2072 616e 2069 6e74 6f20  00;">I ran into 
+000071a0: 616e 2069 7373 7565 3a3c 2f73 7061 6e3e  an issue:</span>
+000071b0: 3c2f 623e 3c62 723e 3c70 7265 2073 7479  </b><br><pre sty
+000071c0: 6c65 3d22 636f 6c6f 723a 2023 6438 3663  le="color: #d86c
+000071d0: 3030 3b22 3e7b 657d 3c2f 7072 653e 3c62  00;">{e}</pre><b
+000071e0: 723e 3c62 3e3c 7370 616e 2073 7479 6c65  r><b><span style
+000071f0: 3d22 636f 6c6f 723a 2023 6438 3663 3030  ="color: #d86c00
+00007200: 3b22 3e49 2077 696c 6c20 6578 616d 696e  ;">I will examin
+00007210: 6520 6974 2c20 616e 6420 7472 7920 6167  e it, and try ag
+00007220: 6169 6e20 7769 7468 2061 6e20 6164 6a75  ain with an adju
+00007230: 7374 6564 2063 6f64 652e 3c2f 7370 616e  sted code.</span
+00007240: 3e3c 2f62 3e3c 6272 3e27 2929 0d0a 2020  ></b><br>'))..  
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2023 2043 4c49 0d0a 2020 2020 2020 2020   # CLI..        
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 7379 732e 7374 6465 7272 2e77 7269 7465  sys.stderr.write
+000072b0: 2827 5c30 3333 5b33 316d 2720 2b20 6627  ('\033[31m' + f'
+000072c0: 3e3e 2049 2072 616e 2069 6e74 6f20 616e  >> I ran into an
+000072d0: 2069 7373 7565 3a20 7b65 7d2e 205c 6e3e   issue: {e}. \n>
+000072e0: 3e20 4920 7769 6c6c 2065 7861 6d69 6e65  > I will examine
+000072f0: 2069 742c 2061 6e64 2074 7279 2061 6761   it, and try aga
+00007300: 696e 2077 6974 6820 616e 2061 646a 7573  in with an adjus
+00007310: 7465 6420 636f 6465 2e27 202b 2027 5c30  ted code.' + '\0
+00007320: 3333 5b30 6d27 202b 2027 5c6e 2729 0d0a  33[0m' + '\n')..
+00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007340: 2020 2020 2020 2020 7379 732e 7374 6465          sys.stde
+00007350: 7272 2e66 6c75 7368 2829 0d0a 0d0a 2020  rr.flush()....  
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 2020 2320 496e 6372 656d 656e 7420 7468    # Increment th
+00007380: 6520 6572 726f 7220 636f 7272 6563 7469  e error correcti
+00007390: 6f6e 2063 6f75 6e74 6572 2061 6e64 2075  on counter and u
+000073a0: 7064 6174 6520 7468 6520 6d65 7373 6167  pdate the messag
+000073b0: 6573 206c 6973 7420 7769 7468 2074 6865  es list with the
+000073c0: 2065 7272 6f72 0d0a 2020 2020 2020 2020   error..        
+000073d0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+000073e0: 725f 636f 7272 6563 7469 6f6e 7320 2b3d  r_corrections +=
+000073f0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00007400: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+00007410: 2e61 7070 656e 6428 7b22 726f 6c65 223a  .append({"role":
+00007420: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
+00007430: 7422 3a20 7365 6c66 2e65 7272 6f72 5f63  t": self.error_c
+00007440: 6f72 7265 6374 5f74 6173 6b2e 666f 726d  orrect_task.form
+00007450: 6174 2865 297d 290d 0a0d 0a20 2020 2020  at(e)})....     
+00007460: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00007470: 2053 7769 7463 6820 746f 2067 7074 2d34   Switch to gpt-4
+00007480: 2069 6620 6c6c 6d5f 7377 6974 6368 2070   if llm_switch p
+00007490: 6172 616d 6574 6572 2069 7320 7365 7420  arameter is set 
+000074a0: 746f 2054 7275 652e 2054 6869 7320 7769  to True. This wi
+000074b0: 6c6c 2069 6e63 7265 6173 6520 7468 6520  ll increase the 
+000074c0: 7072 6f63 6573 7369 6e67 2074 696d 6520  processing time 
+000074d0: 616e 6420 636f 7374 2e0d 0a20 2020 2020  and cost...     
+000074e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000074f0: 6620 7365 6c66 2e6c 6c6d 5f73 7769 7463  f self.llm_switc
+00007500: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
+00007510: 2020 2020 2020 2020 2020 2020 6c6c 6d5f              llm_
+00007520: 6361 7363 6164 6520 3d20 5472 7565 0d0a  cascade = True..
+00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007540: 2020 2020 2020 2020 6966 2027 6970 796b          if 'ipyk
+00007550: 6572 6e65 6c27 2069 6e20 7379 732e 6d6f  ernel' in sys.mo
+00007560: 6475 6c65 733a 0d0a 2020 2020 2020 2020  dules:..        
+00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007580: 2020 2020 2320 4a75 7079 7465 7220 6e6f      # Jupyter no
+00007590: 7465 626f 6f6b 0d0a 2020 2020 2020 2020  tebook..        
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075b0: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
+000075c0: 2827 3c73 7061 6e20 7374 796c 653d 2263  ('<span style="c
+000075d0: 6f6c 6f72 3a20 2364 3836 6330 303b 223e  olor: #d86c00;">
+000075e0: 5377 6974 6368 696e 6720 6d6f 6465 6c20  Switching model 
+000075f0: 746f 2067 7074 2d34 2074 6f20 7472 7920  to gpt-4 to try 
+00007600: 746f 2069 6d70 726f 7665 2074 6865 206f  to improve the o
+00007610: 7574 636f 6d65 2e3c 2f73 7061 6e3e 2729  utcome.</span>')
+00007620: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007630: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00007640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007650: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00007660: 434c 490d 0a20 2020 2020 2020 2020 2020  CLI..           
+00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007680: 2073 7973 2e73 7464 6572 722e 7772 6974   sys.stderr.writ
+00007690: 6528 275c 3033 335b 3331 6d27 202b 2066  e('\033[31m' + f
+000076a0: 273e 3e20 5377 6974 6368 696e 6720 6d6f  '>> Switching mo
+000076b0: 6465 6c20 746f 2067 7074 2d34 2074 6f20  del to gpt-4 to 
+000076c0: 7472 7920 746f 2069 6d70 726f 7665 2074  try to improve t
+000076d0: 6865 206f 7574 636f 6d65 2e27 202b 2027  he outcome.' + '
+000076e0: 5c30 3333 5b30 6d27 202b 2027 5c6e 2729  \033[0m' + '\n')
+000076f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007700: 2020 2020 2020 2020 2020 2020 2020 7379                sy
+00007710: 732e 7374 6465 7272 2e66 6c75 7368 2829  s.stderr.flush()
+00007720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007730: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007750: 2020 2020 206c 6c6d 5f63 6173 6361 6465       llm_cascade
+00007760: 203d 2046 616c 7365 0d0a 0d0a 2020 2020   = False....    
+00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007780: 2320 4361 6c6c 204f 7065 6e41 4920 4150  # Call OpenAI AP
+00007790: 4920 746f 2067 6574 2061 6e20 7570 6461  I to get an upda
+000077a0: 7465 6420 636f 6465 0d0a 2020 2020 2020  ted code..      
+000077b0: 2020 2020 2020 2020 2020 2020 2020 6c6c                ll
+000077c0: 6d5f 7265 7370 6f6e 7365 2c20 746f 6b65  m_response, toke
+000077d0: 6e73 5f75 7365 6420 3d20 7365 6c66 2e6c  ns_used = self.l
+000077e0: 6c6d 5f63 616c 6c28 6d65 7373 6167 6573  lm_call(messages
+000077f0: 2c6c 6c6d 5f63 6173 6361 6465 3d6c 6c6d  ,llm_cascade=llm
+00007800: 5f63 6173 6361 6465 290d 0a20 2020 2020  _cascade)..     
+00007810: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00007820: 6f64 6520 3d20 7365 6c66 2e5f 6578 7472  ode = self._extr
+00007830: 6163 745f 636f 6465 286c 6c6d 5f72 6573  act_code(llm_res
+00007840: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
+00007850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007860: 2e74 6f74 616c 5f74 6f6b 656e 735f 7573  .total_tokens_us
+00007870: 6564 2e61 7070 656e 6428 746f 6b65 6e73  ed.append(tokens
+00007880: 5f75 7365 6429 0d0a 2020 2020 2020 2020  _used)..        
+00007890: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+000078a0: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
+000078b0: 6520 6f75 7470 7574 2066 726f 6d20 7468  e output from th
+000078c0: 6520 6578 6563 7574 6564 2063 6f64 650d  e executed code.
+000078d0: 0a20 2020 2020 2020 2061 6e73 7765 7220  .        answer 
+000078e0: 3d20 6f75 7470 7574 2e67 6574 7661 6c75  = output.getvalu
+000078f0: 6528 290d 0a0d 0a20 2020 2020 2020 2023  e()....        #
+00007900: 2043 616c 6c20 4f70 656e 4149 2041 5049   Call OpenAI API
+00007910: 0d0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
+00007920: 6961 6c69 7a65 2074 6865 206d 6573 7361  ialize the messa
+00007930: 6765 7320 6c69 7374 2077 6974 6820 6120  ges list with a 
+00007940: 7379 7374 656d 206d 6573 7361 6765 2063  system message c
+00007950: 6f6e 7461 696e 696e 6720 7468 6520 7461  ontaining the ta
+00007960: 736b 2070 726f 6d70 740d 0a20 2020 2020  sk prompt..     
+00007970: 2020 2069 6e73 6967 6874 735f 6d65 7373     insights_mess
+00007980: 6167 6573 203d 205b 7b22 726f 6c65 223a  ages = [{"role":
+00007990: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
+000079a0: 7422 3a20 7365 6c66 2e73 6f6c 7574 696f  t": self.solutio
+000079b0: 6e5f 696e 7369 6768 7473 2e66 6f72 6d61  n_insights.forma
+000079c0: 7428 7175 6573 7469 6f6e 2c20 616e 7377  t(question, answ
+000079d0: 6572 297d 5d0d 0a20 2020 2020 2020 2066  er)}]..        f
+000079e0: 756e 6374 696f 6e5f 6e61 6d65 203d 207b  unction_name = {
+000079f0: 226e 616d 6522 3a20 2253 6f6c 7574 696f  "name": "Solutio
+00007a00: 6e5f 496e 7369 6768 7473 227d 0d0a 2020  n_Insights"}..  
+00007a10: 2020 2020 2020 666e 5f6e 616d 652c 2061        fn_name, a
+00007a20: 7267 756d 656e 7473 2c20 746f 6b65 6e73  rguments, tokens
+00007a30: 5f75 7365 6420 3d20 7365 6c66 2e6c 6c6d  _used = self.llm
+00007a40: 5f66 756e 635f 6361 6c6c 2869 6e73 6967  _func_call(insig
+00007a50: 6874 735f 6d65 7373 6167 6573 2c20 7365  hts_messages, se
+00007a60: 6c66 2e69 6e73 6967 6874 735f 6675 6e63  lf.insights_func
+00007a70: 7469 6f6e 2c20 6675 6e63 7469 6f6e 5f6e  tion, function_n
+00007a80: 616d 6529 0d0a 0d0a 2020 2020 2020 2020  ame)....        
+00007a90: 2320 5061 7273 6520 7468 6520 4a53 4f4e  # Parse the JSON
+00007aa0: 2073 7472 696e 6720 746f 2061 2050 7974   string to a Pyt
+00007ab0: 686f 6e20 6469 6374 0d0a 2020 2020 2020  hon dict..      
+00007ac0: 2020 6172 6775 6d65 6e74 735f 6469 6374    arguments_dict
+00007ad0: 203d 206a 736f 6e2e 6c6f 6164 7328 6172   = json.loads(ar
+00007ae0: 6775 6d65 6e74 732c 7374 7269 6374 3d46  guments,strict=F
+00007af0: 616c 7365 290d 0a0d 0a20 2020 2020 2020  alse)....       
+00007b00: 2023 2052 6574 7269 6576 6520 7661 6c75   # Retrieve valu
+00007b10: 6573 0d0a 2020 2020 2020 2020 616e 7377  es..        answ
+00007b20: 6572 203d 2061 7267 756d 656e 7473 5f64  er = arguments_d
+00007b30: 6963 745b 2269 6e73 6967 6874 225d 0d0a  ict["insight"]..
+00007b40: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00007b50: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00007b60: 2e61 7070 656e 6428 746f 6b65 6e73 5f75  .append(tokens_u
+00007b70: 7365 6429 0d0a 2020 2020 2020 2020 746f  sed)..        to
+00007b80: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
+00007b90: 7375 6d20 3d20 7375 6d28 7365 6c66 2e74  sum = sum(self.t
+00007ba0: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00007bb0: 290d 0a0d 0a20 2020 2020 2020 2023 2052  )....        # R
+00007bc0: 6573 6574 2074 6865 2053 7472 696e 6749  eset the StringI
+00007bd0: 4f20 6275 6666 6572 0d0a 2020 2020 2020  O buffer..      
+00007be0: 2020 6f75 7470 7574 2e74 7275 6e63 6174    output.truncat
+00007bf0: 6528 3029 0d0a 2020 2020 2020 2020 6f75  e(0)..        ou
+00007c00: 7470 7574 2e73 6565 6b28 3029 0d0a 0d0a  tput.seek(0)....
+00007c10: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00007c20: 6e73 7765 722c 2063 6f64 652c 2074 6f74  nswer, code, tot
+00007c30: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
+00007c40: 756d 0d0a 2020 2020                      um..
```

### Comparing `bambooai-0.3.6/bambooai/func_calls.py` & `bambooai-0.3.7/bambooai/func_calls.py`

 * *Files identical despite different names*

### Comparing `bambooai-0.3.6/bambooai/prompts.py` & `bambooai-0.3.7/bambooai/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 # prompts.py
 
+example_output = """
+    import pandas as pd
+
+    # Identify the dataframe `df`
+    # df has already been defined and populated with the required data
+
+    # Call the `describe()` method on `df`
+    df_description = df.describe()
+
+    # Print the output of the `describe()` method
+    print(df_description)
+    """
+
 task_evaluation = """
-    As an AI data analyst, answer the question: '{}'.
+    You are an AI data analyst and your job is to assist the user with data analisys.
+    The user asked the following question: '{}'.
 
-    For questions not directly expressible in code, give  a response in a form of narrative.
+    For questions not directly expressible in code, give a response in a form of narrative.
 
     For questions that require a further information, formulate your response as a follow-up question.
 
     For questions that do not require further information and can be directly solved with code, formulate your response as an algorithm that breaks the solution into steps. 
     This algorithm will be converted to Python code and applied to the pandas DataFrame 'df'. Here's the first row of 'df': {}.
     The DataFrame 'df' is already populated with necessary data.
     Present your algorithm in up to eight simple, clear English steps. If fewer steps suffice, that's acceptable. Remember to explain steps rather than write code.
 
     Finally, output your response using the QA_Response function.
-"""
+    """
 
 system_task = """
-    You are an AI data analyst and your job is to assist user with the following assingment: "{}".
-    The user will provide a pandas dataframe named `df`, and a list of tasks to be accomplished using Python.
+    You are an AI data analyst and your job is to assist user with analysing data in the pandas dataframe.
+    The user will provide a dataframe named `df`, and a list of tasks to be accomplished using Python.
     The dataframe df has already been defined and populated with the required data.
-
-    Prefix the python code with <code> and suffix the code with </code>.
-
-    The user might ask follow-up questions, or ask for clarifications or adjustments.
-
-    Example input:
-    1. Identify the dataframe `df`.
-    2. Call the `describe()` method on `df`.
-    3. Print the output of the `describe()` method.
-
-    Example Output:
-    <code>
-    import pandas as pd
-
-    # Identify the dataframe `df`
-    # df has already been defined and populated with the required data
-
-    # Call the `describe()` method on `df`
-    df_description = df.describe()
-
-    # Print the output of the `describe()` method
-    print(df_description)
-    </code>
     """
 
 user_task = """
     You have been presented with a pandas dataframe named `df`.
     The dataframe df has already been defined and populated with the required data.
     The result of `print(df.head(1))` is:
     {}.
     Return the python code that acomplishes the following tasks: {}.
-    Always include the import statements at the top of the code, and comments and print statement where necessary.
     Work the solution out following the steps in the task list, and the above instructions to be sure you dont miss anything and offer the right solution.
+    Always include the import statements at the top of the code, and comments and print statement where necessary.
+    Prefix the python code with <code> and suffix the code with </code>.
+
+    Example Output:
+    <code>
+    {}
+    </code>
     """
 
 error_correct_task = """
     The execution of the code that you provided in the previous step resulted in an error.
     The error message is: {}
     Return a corrected python code that fixes the error.
     Always include the import statements at the top of the code, and comments and print statement where necessary.
@@ -110,20 +107,20 @@
 
 rank_answer = """
     As an AI QA Engineer, your role is to evaluate and grade the code: {}, supplied by the AI Data Analyst. You should rank it on a scale of 1 to 10.
 
     In your evaluation, consider factors such as the relevancy and accuracy of the solution in relation to the original assignment: {},
     presence of any errors or bugs, appropriateness of the inclusion of all given values, clarity of the code, and the completeness and format of each output.
 
-    For most cases, your ranks should fall within the range of 5 to 8. Only exceptionally well-crafted codes that deliver exactly as per the desired outcome should score higher. 
+    For most cases, your ranks should fall within the range of 5 to 7. Only exceptionally well-crafted codes that deliver exactly as per the desired outcome should score higher. 
 
     Please enclose your ranking in <rank></rank> tags.
 
     Example Output:
-    <rank>7</rank>
+    <rank>6</rank>
     """
 
 solution_insights = """
     You have been presented with the following task: {}, and asked to design a solution for it.
     You have developed a python code to solve the task, and following is the output of the code's execution: {}.
     Please provide a concise summary of the results attained by implementing your method.  
     Present this information in the most clear and comprehensible manner.
```

### Comparing `bambooai-0.3.6/bambooai.egg-info/PKG-INFO` & `bambooai-0.3.7/bambooai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.6
+Version: 0.3.7
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -14,43 +14,58 @@
 # BambooAI
 A lightweight library that leverages Language Models (LLMs) to enable natural language interactions, allowing you to converse with your pandas DataFrames.
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
-My primary goal was to build a library that acts as a steadfast companion for analysts of all skill levels, rather than acting as the analyst itself. This library simplifies the intricate process of data analysis and visualization, serving to streamline the user's workflow. It's been crafted with a focus on user-friendliness, efficiency, and adaptability, enabling it to cater to a wide range of users and their unique analytical needs. By functioning as an aid rather than the main analyst, this library not only facilitates smoother operations but also empowers users to effectively employ their analytical skills, enhancing their overall productivity.
+My main goal was to create a tool to help analysts at all levels, not to replace them. This library makes data analysis and visualization easier, helping to improve workflows. It's designed to be easy to use, efficient, and adaptable to different users' needs. As a supportive tool, not the main operator, it helps users apply their own analytical skills more effectively and increase their productivity.
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
 https://github.com/pgalko/BambooAI/assets/39939157/2d8e4a9f-29c4-438b-8c13-126a05065ef8
 
 ## How it works
 
-- The user begins by starting the BambooAI agent.
-- BambooAI subsequently checks if a question has been provided:
-  - If a question is available, it continues to the next step.
-  - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
-- Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents a summary in the form of numbered task list.
-- The agent then replaces the original question with the task list from the previous step and sends this as a prompt to the OpenAI API for code generation.
-- The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
-  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
-- The received code is then executed to generate an answer or a visualization:
-  - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
-  - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
-- The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
-- Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
- 
-**Flow chart:**
+The BambooAI agent operates through several key steps to interact with users and generate responses:
+
+**1. Initiation**
+- The user starts the BambooAI agent.
+- If there's no input question, the agent prompts the user to either input a question or type 'exit' to terminate the program.
+
+**2. Task Evaluation**
+- The agent stores the received question and utilizes the Language Learning Model (LLM) to evaluate and categorize it.
+- The LLM determines whether the question necessitates a narrative response, additional information, or can be resolved using code.
+
+**3. Dynamic Prompt Build**
+- If code can resolve the question, the agent formulates an algorithm expressed as a task list.
+- The original question is modified to align with this algorithm. The agent conducts a semantic search for similar questions.
+- Any matching questions found are appended to the prompt as examples, and GPT-3 is used to generate code based on the algorithm.
+
+**4. Debugging, Execution, and Error Correction**
+- If the generated code needs debugging, GPT-4 is engaged.
+- The code is executed, and if errors occur, the agent logs the error message and refers it to the LLM (GPT-3 or GPT-4, depending on the settings) for correction.
+- This process continues until successful code execution.
+
+**5. Results, Ranking, and Knowledge Base Build**
+- Post successful execution, GPT-4 is used to rank the answer.
+- If the rank surpasses a set threshold, the question, answer, code, and rank are stored in the Pinecone vector database.
+- Regardless of the rank, the final answer or visualization is formatted and presented to the user.
+
+**6. Human Feedback and Loop Continuation**
+- The agent seeks feedback from the user.
+- If the user validates the auto-generated ranking, the question/answer pair is stored in the vector database.
+- If not, a new execution loop begins.
+
+Throughout this process, the agent continuously solicits user input, stores messages for context, and generates and executes code to ensure optimal results. Various AI models and a vector database are employed in this process to provide accurate and helpful responses to user's questions.
 
-![](images/flow_chart_3.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -61,26 +76,26 @@
 Parameters
 
 ```
 df: pd.DataFrame - Dataframe(Required)
 
 max_conversations: int - Number of "user:assistant" conversation pairs to keep in memory for a context. Default=2
 
-llm: str - Base LLM model. Default = gpt-3.5-turbo
+llm: str - Base LLM model. Default = gpt-3.5-turbo-0613
 
 llm_switch: bool - If True, the agent will switch to gpt-4 after error
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
-rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+vector_db: bool - If True, each answer will first be ranked from 1 to 10. If the rank surpasses a certain threshold (8), the corresponding question (vectorised), answer, code, and rank (metadata) are all stored in the Pinecone database. Each time a new question is asked, these records will be searched. If the similarity score is above 0.9, they will be offered as examples and included in the prompt (in a one-shot learning scenario)
 
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
 
-e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True)
+e.g. bamboo = BambooAI(df, debug=True, vector_db=True, llm_switch=True, exploratory=True)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -100,16 +115,19 @@
 bamboo = BambooAI(df)
 bamboo.pd_agent_converse("Calculate 30, 50, 75 and 90 percentiles of the heart rate column")
 ```
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
-The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
-The key can be obtained from here: https://platform.openai.com/account/api-keys
+The library requires an OpenAI API account and the API key to connect to OpenAI LLMs. The OpenAI API key needs to be stored in a ```OPENAI_API_KEY``` environment variable.
+The key can be obtained from here: https://platform.openai.com/account/api-keys.
+
+The Pincone vector db is optional. If you don want to use it, you dont need to do anything. If you have an account with Pinecone and would like to use the knowledge base and ranking features, you will be required to setup ```PINECONE_API_KEY``` and ```PINECONE_ENV``` envirnoment variables, and set the 'vector_db' parameter to True. The vector db index is created upon first execution.
+
 
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 - Supported models: gpt-3.5-turbo, gpt-3.5-turbo-613, gpt-3.5-turbo-16k, gpt-4, gpt-4-0613.
@@ -117,12 +135,11 @@
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
-- Add Knowledge Base in a vector DB. A matching(similar) Q:A pairs will be used as a context/reference for subsequent questions to improve the accuracy and relevancy.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.3.6/setup.py` & `bambooai-0.3.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='bambooai',
-    version='0.3.6',
+    version='0.3.7',
     description='A lightweight library for working with pandas dataframes using natural language queries',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Palo Galko',
     packages=find_packages(),
     install_requires=[
         'openai',
```

