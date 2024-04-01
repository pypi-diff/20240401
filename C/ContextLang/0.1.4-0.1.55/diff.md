# Comparing `tmp/ContextLang-0.1.4.tar.gz` & `tmp/ContextLang-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ContextLang-0.1.4.tar", last modified: Wed Jun 28 13:30:40 2023, max compression
+gzip compressed data, was "ContextLang-0.1.55.tar", last modified: Mon Apr  1 17:33:17 2024, max compression
```

## Comparing `ContextLang-0.1.4.tar` & `ContextLang-0.1.55.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 13:30:40.209553 ContextLang-0.1.4/
--rw-rw-rw-   0        0        0    11546 2023-06-27 17:42:27.000000 ContextLang-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    20467 2023-06-28 13:30:40.208553 ContextLang-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    18742 2023-06-28 10:36:35.000000 ContextLang-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-28 13:30:40.209553 ContextLang-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2275 2023-06-28 13:30:25.000000 ContextLang-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 13:30:40.188553 ContextLang-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 13:30:40.198553 ContextLang-0.1.4/src/ContextLang.egg-info/
--rw-rw-rw-   0        0        0    20467 2023-06-28 13:30:40.000000 ContextLang-0.1.4/src/ContextLang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-06-28 13:30:40.000000 ContextLang-0.1.4/src/ContextLang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 13:30:40.000000 ContextLang-0.1.4/src/ContextLang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-28 13:30:40.000000 ContextLang-0.1.4/src/ContextLang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2023-06-28 13:30:40.000000 ContextLang-0.1.4/src/ContextLang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-28 13:30:40.000000 ContextLang-0.1.4/src/ContextLang.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-28 13:30:40.207554 ContextLang-0.1.4/src/context/
--rw-rw-rw-   0        0        0     4160 2023-06-28 12:56:23.000000 ContextLang-0.1.4/src/context/Context.py
--rw-rw-rw-   0        0        0      619 2023-06-27 17:41:55.000000 ContextLang-0.1.4/src/context/__init__.py
--rw-rw-rw-   0        0        0     4741 2023-06-28 12:56:44.000000 ContextLang-0.1.4/src/context/code_generator.py
--rw-rw-rw-   0        0        0      845 2023-06-28 12:56:44.000000 ContextLang-0.1.4/src/context/config.py
--rw-rw-rw-   0        0        0     1203 2023-06-27 17:43:03.000000 ContextLang-0.1.4/src/context/file_manager.py
--rw-rw-rw-   0        0        0     1578 2023-06-27 17:43:27.000000 ContextLang-0.1.4/src/context/log.py
--rw-rw-rw-   0        0        0     5070 2023-06-28 12:55:59.000000 ContextLang-0.1.4/src/context/openai_interface.py
--rw-rw-rw-   0        0        0     7386 2023-06-28 12:55:59.000000 ContextLang-0.1.4/src/context/tag_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:33:17.148026 ContextLang-0.1.55/
+-rw-rw-rw-   0        0        0    11546 2023-06-27 17:42:27.000000 ContextLang-0.1.55/LICENSE
+-rw-rw-rw-   0        0        0    21078 2024-04-01 17:33:17.148026 ContextLang-0.1.55/PKG-INFO
+-rw-rw-rw-   0        0        0    19116 2023-07-12 22:10:21.000000 ContextLang-0.1.55/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 17:33:17.149023 ContextLang-0.1.55/setup.cfg
+-rw-rw-rw-   0        0        0     2401 2024-04-01 17:31:08.000000 ContextLang-0.1.55/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:33:17.128080 ContextLang-0.1.55/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 17:33:17.146032 ContextLang-0.1.55/src/ContextLang.egg-info/
+-rw-rw-rw-   0        0        0    21078 2024-04-01 17:33:17.000000 ContextLang-0.1.55/src/ContextLang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:33:17.000000 ContextLang-0.1.55/src/ContextLang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 17:33:17.000000 ContextLang-0.1.55/src/ContextLang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-01 17:33:17.000000 ContextLang-0.1.55/src/ContextLang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      140 2024-04-01 17:33:17.000000 ContextLang-0.1.55/src/ContextLang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-01 17:33:17.000000 ContextLang-0.1.55/src/ContextLang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 17:33:17.144037 ContextLang-0.1.55/src/context/
+-rw-rw-rw-   0        0        0     5994 2024-04-01 13:04:52.000000 ContextLang-0.1.55/src/context/Context.py
+-rw-rw-rw-   0        0        0      619 2023-06-27 17:41:55.000000 ContextLang-0.1.55/src/context/__init__.py
+-rw-rw-rw-   0        0        0     4900 2024-04-01 10:04:04.000000 ContextLang-0.1.55/src/context/code_generator.py
+-rw-rw-rw-   0        0        0      845 2023-06-28 12:56:44.000000 ContextLang-0.1.55/src/context/config.py
+-rw-rw-rw-   0        0        0     1714 2024-04-01 16:51:33.000000 ContextLang-0.1.55/src/context/file_manager.py
+-rw-rw-rw-   0        0        0     1578 2023-06-27 17:43:27.000000 ContextLang-0.1.55/src/context/log.py
+-rw-rw-rw-   0        0        0     6461 2024-03-26 18:26:10.000000 ContextLang-0.1.55/src/context/openai_interface.py
+-rw-rw-rw-   0        0        0    10469 2024-04-01 09:33:53.000000 ContextLang-0.1.55/src/context/tag_parser.py
```

### Comparing `ContextLang-0.1.4/LICENSE` & `ContextLang-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `ContextLang-0.1.4/PKG-INFO` & `ContextLang-0.1.55/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ContextLang
-Version: 0.1.4
+Version: 0.1.55
 Summary: Cross-platform, AI code generator CLI tool and ContexLang preprocessor
 Home-page: https://github.com/werfish/Context-Lang
 Author: Robert Mazurowski
 Author-email: werfish1@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/werfish/Context-Lang
 Project-URL: Source, https://github.com/werfish/Context-Lang
@@ -32,14 +32,20 @@
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Visual Basic
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Pre-processors
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests<3.0.0,>=2.24.0
+Requires-Dist: python-dotenv<0.20.0,>=0.15.0
+Requires-Dist: openai==1.14.3
+Requires-Dist: tenacity<7.0.0,>=6.3.1
+Requires-Dist: colorama<1.0.0,>=0.4.3
+Requires-Dist: gitignore_parser==0.1.11
 
 # Context: AI-Powered Code Generation
 
 Context is a revolutionary AI code preprocessor and generator designed to automate the Chat GPT coding workflow, enabling in-code prompting and output via ContextLang tags embedded in code comments. 
 
 With Context, you can:
 
@@ -49,14 +55,16 @@
 
 2. **Seamlessly integrate and use**: Context is easy to install, and ContextLang is non invasive, residing within code comments. ContextLang is language-agnostic and fits seamlessly into any programming language and codebase, large or small. Starting with Context is as easy as pie, and integrating it into your existing work requires minimal effort.
 
 3. **Save on cost and time**: Context aims to use 2 Open AI api calls per prompt making daily usage cost mere cents. With Context, you're not just saving time, but also money.
 
 ### The Developer is dead, long live the AI augmented cyberpunk developer. The CyDeveloper :)
 
+Inspiration for this quote from Angel AI [here](https://www.linkedin.com/posts/angeljsalazar_harness-releases-generative-ai-assistant-activity-7077308844099407873-xvYd?utm_source=share&utm_medium=member_desktop)
+
 ## Table of Contents
 1. [Introduction](#context-ai-powered-code-generation)
 2. [Context Description](#context-description)
     - [Goal](#goal)
     - [ContextLang](#contextlang)
 3. [Prerequisites](#prerequisites)
 4. [Installation](#installation)
@@ -70,14 +78,15 @@
     - [Context Variables](#context-variables)
     - [Prompts](#prompts)
 10. [Features/Specification V2 (TO DO)](#featuresspecification-v2-to-do)
 11. [Features/Specification V3 (TO DO)](#featuresspecification-v3-to-do)
 12. [Documentation](#documentation)
 13. [Contributing](#contributing)
 14. [License](#license)
+15. [ROADMAP](/ROADMAP.md)
 
 
 ## Context Description
 
 Context is a programming tool designed to harness the capabilities of AI to enhance software development. It employs OpenAI's GPT-3.5 Turbo model, uses the custom ContextLang for formatting, and treats contextual descriptions as variables and prompts as functions. This design allows for effective use of AI capabilities, provided the instructions are clear and context is well-described.
 
 Anticipating the development of larger projects such as Engineer-GPT and AutoGPT, which may take years to become practically usable, Context aims to bridge this gap by offering a practical tool for developers to use in their current workflows. It is designed to extract as much as possible from the GPT-3.5 Turbo model until GPT-4 becomes widely accessible. If you already have access to GPT-4, you can use it straight away for potentially better results.
@@ -147,15 +156,15 @@
 	return a + b
 #<context:TEMPLATE/>
 ```
 
 Now, using a prompt tag, we instruct the AI to create three additional functions for multiplication, division, and subtraction. We provide the previously created template by using the TEMPLATE context variable as a context to guide the AI's output. Keep in mind that global context will also be injected into the prompt. 
 
 ```python
-#<prompt:Functions>Write me a subtraction, division and multiplication functions for a and b based on the template function. {TEMPLATE} <prompt/>
+#<prompt:Functions>Write me a subtraction, division and multiplication functions for a and b based on the template function. {TEMPLATE} <prompt:Functions/>
 ```
 To indicate where the Functions prompt should output we use the name of the prompt enclose in {}. This is a one off operation.The output from the prompt will overwrite the following comment in the Python file when we run Context:
 
 ```python
 #{Functions}
 ```
 
@@ -164,15 +173,15 @@
 ```python
 #<Functions>
 #<Functions/>
 ```
 
 The Functions variable can also be used as context in the prompt while it is used as an output tag, allowing modification over the produced or existing code.
 ```python
-#<prompt:Functions>Please correct the multiply function in the code, it should multiply instead of subtract. {Functions} <prompt/>
+#<prompt:Functions>Please correct the multiply function in the code, it should multiply instead of subtract. {Functions} <prompt:Functions/>
 #<Functions>
 def multiply(a,b):
 	return a - b
 #OTHER FUNCTIONS....
 #<Functions/>
 ```
 
@@ -434,10 +443,11 @@
 ```
 
 ## Documentation: 
 A dedicated site is not yet created.
 
 ## Contributing
 If you want to contribute, and you know how to run an open source project then please contact me.
+You can find plans for the project and libraries you can learn in this project in the  [ROADMAP](/ROADMAP.md)
 
 ## License
 [Apache 2.0 License](LICENSE)
```

### Comparing `ContextLang-0.1.4/README.md` & `ContextLang-0.1.55/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 2. **Seamlessly integrate and use**: Context is easy to install, and ContextLang is non invasive, residing within code comments. ContextLang is language-agnostic and fits seamlessly into any programming language and codebase, large or small. Starting with Context is as easy as pie, and integrating it into your existing work requires minimal effort.
 
 3. **Save on cost and time**: Context aims to use 2 Open AI api calls per prompt making daily usage cost mere cents. With Context, you're not just saving time, but also money.
 
 ### The Developer is dead, long live the AI augmented cyberpunk developer. The CyDeveloper :)
 
+Inspiration for this quote from Angel AI [here](https://www.linkedin.com/posts/angeljsalazar_harness-releases-generative-ai-assistant-activity-7077308844099407873-xvYd?utm_source=share&utm_medium=member_desktop)
+
 ## Table of Contents
 1. [Introduction](#context-ai-powered-code-generation)
 2. [Context Description](#context-description)
     - [Goal](#goal)
     - [ContextLang](#contextlang)
 3. [Prerequisites](#prerequisites)
 4. [Installation](#installation)
@@ -31,14 +33,15 @@
     - [Context Variables](#context-variables)
     - [Prompts](#prompts)
 10. [Features/Specification V2 (TO DO)](#featuresspecification-v2-to-do)
 11. [Features/Specification V3 (TO DO)](#featuresspecification-v3-to-do)
 12. [Documentation](#documentation)
 13. [Contributing](#contributing)
 14. [License](#license)
+15. [ROADMAP](/ROADMAP.md)
 
 
 ## Context Description
 
 Context is a programming tool designed to harness the capabilities of AI to enhance software development. It employs OpenAI's GPT-3.5 Turbo model, uses the custom ContextLang for formatting, and treats contextual descriptions as variables and prompts as functions. This design allows for effective use of AI capabilities, provided the instructions are clear and context is well-described.
 
 Anticipating the development of larger projects such as Engineer-GPT and AutoGPT, which may take years to become practically usable, Context aims to bridge this gap by offering a practical tool for developers to use in their current workflows. It is designed to extract as much as possible from the GPT-3.5 Turbo model until GPT-4 becomes widely accessible. If you already have access to GPT-4, you can use it straight away for potentially better results.
@@ -108,15 +111,15 @@
 	return a + b
 #<context:TEMPLATE/>
 ```
 
 Now, using a prompt tag, we instruct the AI to create three additional functions for multiplication, division, and subtraction. We provide the previously created template by using the TEMPLATE context variable as a context to guide the AI's output. Keep in mind that global context will also be injected into the prompt. 
 
 ```python
-#<prompt:Functions>Write me a subtraction, division and multiplication functions for a and b based on the template function. {TEMPLATE} <prompt/>
+#<prompt:Functions>Write me a subtraction, division and multiplication functions for a and b based on the template function. {TEMPLATE} <prompt:Functions/>
 ```
 To indicate where the Functions prompt should output we use the name of the prompt enclose in {}. This is a one off operation.The output from the prompt will overwrite the following comment in the Python file when we run Context:
 
 ```python
 #{Functions}
 ```
 
@@ -125,15 +128,15 @@
 ```python
 #<Functions>
 #<Functions/>
 ```
 
 The Functions variable can also be used as context in the prompt while it is used as an output tag, allowing modification over the produced or existing code.
 ```python
-#<prompt:Functions>Please correct the multiply function in the code, it should multiply instead of subtract. {Functions} <prompt/>
+#<prompt:Functions>Please correct the multiply function in the code, it should multiply instead of subtract. {Functions} <prompt:Functions/>
 #<Functions>
 def multiply(a,b):
 	return a - b
 #OTHER FUNCTIONS....
 #<Functions/>
 ```
 
@@ -395,10 +398,11 @@
 ```
 
 ## Documentation: 
 A dedicated site is not yet created.
 
 ## Contributing
 If you want to contribute, and you know how to run an open source project then please contact me.
+You can find plans for the project and libraries you can learn in this project in the  [ROADMAP](/ROADMAP.md)
 
 ## License
 [Apache 2.0 License](LICENSE)
```

### Comparing `ContextLang-0.1.4/setup.py` & `ContextLang-0.1.55/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ContextLang',
     description='Cross-platform, AI code generator CLI tool and ContexLang preprocessor',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    version='0.1.4',
+    version='0.1.55',
     install_requires=[
-        'requests',
-        'python-dotenv',
-        'openai',
-        'tenacity'
+        'requests>=2.24.0,<3.0.0',
+        'python-dotenv>=0.15.0,<0.20.0',
+        'openai==1.14.3',
+        'tenacity>=6.3.1,<7.0.0',
+        'colorama>=0.4.3,<1.0.0',
+        'gitignore_parser==0.1.11'
     ],
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     entry_points={
         'console_scripts': [
             'Context = context.Context:main',
         ],
```

### Comparing `ContextLang-0.1.4/src/ContextLang.egg-info/PKG-INFO` & `ContextLang-0.1.55/src/ContextLang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ContextLang
-Version: 0.1.4
+Version: 0.1.55
 Summary: Cross-platform, AI code generator CLI tool and ContexLang preprocessor
 Home-page: https://github.com/werfish/Context-Lang
 Author: Robert Mazurowski
 Author-email: werfish1@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/werfish/Context-Lang
 Project-URL: Source, https://github.com/werfish/Context-Lang
@@ -32,14 +32,20 @@
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Visual Basic
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Pre-processors
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests<3.0.0,>=2.24.0
+Requires-Dist: python-dotenv<0.20.0,>=0.15.0
+Requires-Dist: openai==1.14.3
+Requires-Dist: tenacity<7.0.0,>=6.3.1
+Requires-Dist: colorama<1.0.0,>=0.4.3
+Requires-Dist: gitignore_parser==0.1.11
 
 # Context: AI-Powered Code Generation
 
 Context is a revolutionary AI code preprocessor and generator designed to automate the Chat GPT coding workflow, enabling in-code prompting and output via ContextLang tags embedded in code comments. 
 
 With Context, you can:
 
@@ -49,14 +55,16 @@
 
 2. **Seamlessly integrate and use**: Context is easy to install, and ContextLang is non invasive, residing within code comments. ContextLang is language-agnostic and fits seamlessly into any programming language and codebase, large or small. Starting with Context is as easy as pie, and integrating it into your existing work requires minimal effort.
 
 3. **Save on cost and time**: Context aims to use 2 Open AI api calls per prompt making daily usage cost mere cents. With Context, you're not just saving time, but also money.
 
 ### The Developer is dead, long live the AI augmented cyberpunk developer. The CyDeveloper :)
 
+Inspiration for this quote from Angel AI [here](https://www.linkedin.com/posts/angeljsalazar_harness-releases-generative-ai-assistant-activity-7077308844099407873-xvYd?utm_source=share&utm_medium=member_desktop)
+
 ## Table of Contents
 1. [Introduction](#context-ai-powered-code-generation)
 2. [Context Description](#context-description)
     - [Goal](#goal)
     - [ContextLang](#contextlang)
 3. [Prerequisites](#prerequisites)
 4. [Installation](#installation)
@@ -70,14 +78,15 @@
     - [Context Variables](#context-variables)
     - [Prompts](#prompts)
 10. [Features/Specification V2 (TO DO)](#featuresspecification-v2-to-do)
 11. [Features/Specification V3 (TO DO)](#featuresspecification-v3-to-do)
 12. [Documentation](#documentation)
 13. [Contributing](#contributing)
 14. [License](#license)
+15. [ROADMAP](/ROADMAP.md)
 
 
 ## Context Description
 
 Context is a programming tool designed to harness the capabilities of AI to enhance software development. It employs OpenAI's GPT-3.5 Turbo model, uses the custom ContextLang for formatting, and treats contextual descriptions as variables and prompts as functions. This design allows for effective use of AI capabilities, provided the instructions are clear and context is well-described.
 
 Anticipating the development of larger projects such as Engineer-GPT and AutoGPT, which may take years to become practically usable, Context aims to bridge this gap by offering a practical tool for developers to use in their current workflows. It is designed to extract as much as possible from the GPT-3.5 Turbo model until GPT-4 becomes widely accessible. If you already have access to GPT-4, you can use it straight away for potentially better results.
@@ -147,15 +156,15 @@
 	return a + b
 #<context:TEMPLATE/>
 ```
 
 Now, using a prompt tag, we instruct the AI to create three additional functions for multiplication, division, and subtraction. We provide the previously created template by using the TEMPLATE context variable as a context to guide the AI's output. Keep in mind that global context will also be injected into the prompt. 
 
 ```python
-#<prompt:Functions>Write me a subtraction, division and multiplication functions for a and b based on the template function. {TEMPLATE} <prompt/>
+#<prompt:Functions>Write me a subtraction, division and multiplication functions for a and b based on the template function. {TEMPLATE} <prompt:Functions/>
 ```
 To indicate where the Functions prompt should output we use the name of the prompt enclose in {}. This is a one off operation.The output from the prompt will overwrite the following comment in the Python file when we run Context:
 
 ```python
 #{Functions}
 ```
 
@@ -164,15 +173,15 @@
 ```python
 #<Functions>
 #<Functions/>
 ```
 
 The Functions variable can also be used as context in the prompt while it is used as an output tag, allowing modification over the produced or existing code.
 ```python
-#<prompt:Functions>Please correct the multiply function in the code, it should multiply instead of subtract. {Functions} <prompt/>
+#<prompt:Functions>Please correct the multiply function in the code, it should multiply instead of subtract. {Functions} <prompt:Functions/>
 #<Functions>
 def multiply(a,b):
 	return a - b
 #OTHER FUNCTIONS....
 #<Functions/>
 ```
 
@@ -434,10 +443,11 @@
 ```
 
 ## Documentation: 
 A dedicated site is not yet created.
 
 ## Contributing
 If you want to contribute, and you know how to run an open source project then please contact me.
+You can find plans for the project and libraries you can learn in this project in the  [ROADMAP](/ROADMAP.md)
 
 ## License
 [Apache 2.0 License](LICENSE)
```

### Comparing `ContextLang-0.1.4/src/context/__init__.py` & `ContextLang-0.1.55/src/context/__init__.py`

 * *Files identical despite different names*

### Comparing `ContextLang-0.1.4/src/context/code_generator.py` & `ContextLang-0.1.55/src/context/code_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,29 @@
     # Process each prompt in the task
     for prompt_name, prompt in task.prompts.items():
 
         # Assemble the prompt
         final_prompt = __process_prompt(prompt, task)
 
         # Generate the output
-        response = generate_code_with_chat(final_prompt)
+        response = generate_code_with_chat(final_prompt,prompt_name)
 
-        # Parse the response JSON
-        response_json = json.loads(response)
-        
-        # Extract the generated code
-        code = response_json.get('code', '').strip()
+        # Proceed only if response is not None
+        if response is not None:
+            # Parse the response JSON
+            response_json = json.loads(response)
+            
+            # Extract the generated code
+            code = response_json.get('code', '').strip()
 
-        # For now mock the code change
-        Log.logger.debug(f"Generated code for {prompt_name}:\n{code}\n")
+            # For now mock the code change
+            Log.logger.debug(f"Generated code for {prompt_name}:\n{code}\n")
 
-        # Apply the code
-        __apply_code(code, task, prompt_name)
+            if code:  # Ensure there's generated code
+                __apply_code(code, task, prompt_name)
 
 def __process_prompt(prompt, task):
     # Copy the prompt to avoid modifying the original
     constructedPrompt = prompt
 
     # Replace {contextVar} in the prompt with contextVar content
     for var_name, var_content in task.context_dict.items():
```

### Comparing `ContextLang-0.1.4/src/context/config.py` & `ContextLang-0.1.55/src/context/config.py`

 * *Files identical despite different names*

### Comparing `ContextLang-0.1.4/src/context/file_manager.py` & `ContextLang-0.1.55/src/context/file_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,35 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import os
+from gitignore_parser import parse_gitignore
 
 ignore_list = ["Context_Logs"]
 
 def get_file_paths(directory):
     file_paths = []
+    
+    # Construct the path to the .gitignore file
+    gitignore_path = os.path.join(directory, '.gitignore')
+    
+    # Check if .gitignore exists in the directory and parse it
+    if os.path.exists(gitignore_path):
+        matches = parse_gitignore(gitignore_path)
+    else:
+        matches = lambda x: False  # If no .gitignore, default to not matching any files
 
     # Traverse the directory recursively
     for root, directories, files in os.walk(directory):
-        directories[:] = [d for d in directories if d not in ignore_list] # This will ignore directories in the ignore_list
+        directories[:] = [d for d in directories if d not in ignore_list and not matches(os.path.join(root, d))] # Filter ignored directories
+
         for file in files:
             file_path = os.path.join(root, file)
-            # Ignore files in ignore_list
-            if os.path.basename(file_path) not in ignore_list:
+            
+            # Ignore files based on ignore_list and .gitignore rules
+            if os.path.basename(file_path) not in ignore_list and not matches(file_path):
                 file_paths.append(file_path)
 
     return file_paths
```

### Comparing `ContextLang-0.1.4/src/context/log.py` & `ContextLang-0.1.55/src/context/log.py`

 * *Files identical despite different names*

### Comparing `ContextLang-0.1.4/src/context/tag_parser.py` & `ContextLang-0.1.55/src/context/tag_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import re
 import traceback
+import os
 
 from .log import Log
 
 class Task:
     def __init__(self, filepath, global_context, context_dict, prompts, prompt_outputs, prompt_output_tags):
         self.filepath = filepath
         self.global_context = global_context
@@ -46,76 +47,123 @@
     "Prompt_Output_Tags": r"(?s)<(?!context|import|file)(\w+)>(.*?)<\1/>"
 }
 
 def __tag_parsing_process(path):
     with open(path, 'r') as file:
         content = file.read()
 
+    # Initialize error collection
+    errors = []
+
     # Create context_dict, prompts, prompt_outputs, and prompt_outputs_tags
     context_dict = {}
     prompts = {}
     prompt_outputs = []
     prompt_outputs_tags = {}
 
     # Iterating over the regex patterns
     for tag, pattern in regexPatterns.items():
         matches = re.findall(pattern, content)  # Use content for all matches
 
         if tag == "Global" and len(matches) > 1:
-            raise ValueError(f"Multiple Global tags found in file {path}")
+            error_msg = f"{tag}: Multiple Global tags found in file {path}"
+            errors.append(error_msg)
+            Log.logger.error(error_msg)
 
         if tag == "Import_File_Context_Variables":
             for match in matches:
-                varName, filePath = match
-                Log.logger.debug(varName + "------" + filePath.strip())
-                with open(filePath.strip(), 'r') as file:
-                    context_dict[varName] = file.read()
+                try:
+                    varName, filePath = match
+                    Log.logger.debug(varName + "------" + filePath.strip())
+                    if varName in context_dict:
+                        raise ValueError(f"{tag}: File'{varName}' already declared in scope.")
+
+                    with open(filePath.strip(), 'r') as file:
+                        context_dict[varName] = file.read()
+                except Exception as e:
+                    errors.append(f"{os.path.relpath(path)}: {str(e)}")
+                    Log.logger.error(f"Error processing {tag} in {path}: {str(e)}")
 
         if tag == "Import_Context_Variables":
             for match in matches:
-                import_path = matches[0].strip() if matches else None
+                import_path = match.strip() if matches else None
 
                 # Parse the file at import_path for context variables and add them to context_dict
                 Log.logger.debug("IMPORT CONTEXT: -----------" + import_path) 
                 with open(import_path, 'r') as file:
                     import_content = file.read()
                     import_context_variables = re.findall(regexPatterns["Context_Variables"], import_content)
                     for import_varName, import_varContent in import_context_variables:
-                        context_dict[import_varName] = import_varContent.strip()
+                        try:
+                            if import_varName in context_dict:
+                                raise ValueError(f"{tag}: Context variable '{import_varName}' from '{import_path}' already exists in scope.")
+                            context_dict[import_varName] = import_varContent.strip()
+                        except Exception as e:
+                            errors.append(f"{os.path.relpath(path)}: {str(e)}")
+                            Log.logger.error(f"Error processing {tag} in {path}: {str(e)}")
 
         if tag == "Import_Specific_Context_Variable":
             for match in matches:
                 varName = match[0]
                 import_path = match[1].strip()
 
                 # Parse the file at import_path for the specific context variable and add it to context_dict
+                Log.logger.debug("IMPORT SPECIFIC CONTEXT: -----------" + import_path + "----" + varName) 
                 with open(import_path, 'r') as file:
                     import_content = file.read()
                     import_context_variable = re.findall(f"(?s)<context:{varName}>(.*?)<context:{varName}/>", import_content)
+                    if varName in context_dict:
+                        e = (f"{tag}: Context variable '{varName}' from '{import_path}' already exists in scope of {path}.")
+                        errors.append(f"{os.path.relpath(path)}: {str(e)}")
+                        Log.logger.error(f"Error processing {tag} in {path}: {str(e)}")
                     if import_context_variable:
                         context_dict[varName] = import_context_variable[0].strip()
+                    else:
+                        e = (f"{tag}: Context variable '{varName}' does not exists in '{import_path}'.")
+                        errors.append(f"{os.path.relpath(path)}: {str(e)}")
+                        Log.logger.error(f"Error processing {tag} in {path}: {str(e)}")
+
 
         elif tag == "Global":
             global_context = matches[0][0].strip() if matches else None
         elif tag == "Context_Variables":
             for match in matches:
-                context_dict[match[0]] = match[1].strip()
+                try:
+                    varName, varContent = match
+                    if varName in context_dict:
+                        raise ValueError(f"{tag}: Context variable '{varName}' already declared in file.")
+                    context_dict[varName] = varContent.strip()
+                except Exception as e:
+                    errors.append(f"{os.path.relpath(path)}: {str(e)}")
+                    Log.logger.error(f"Error processing {tag} in {path}: {str(e)}")
+
         elif tag == "Prompts":
             for match in matches:
-                prompts[match[0]] = match[1].strip()
+                try:
+                    promptName, promptContent = match
+                    if promptName in prompts:
+                        raise ValueError(f"{tag}: Prompt '{promptName}' already declared in file.")
+                    prompts[promptName] = promptContent.strip()
+                except Exception as e:
+                    errors.append(f"{os.path.relpath(path)}: {str(e)}")
+                    Log.logger.error(f"Error processing {tag} in {path}: {str(e)}")
                 
         elif tag == "Prompt_Output_Tags":
             for match in matches:
-                varName = match[0]
-                tag_content = match[1]
-                
-                if varName in context_dict:
-                    raise ValueError(f"Prompt output variable '{varName}' already exists in context_dict in file {path}")
-                
-                prompt_outputs_tags[varName] = tag_content.strip()
+                try:
+                    varName = match[0]
+                    tag_content = match[1]
+                    
+                    if varName in context_dict:
+                        raise ValueError(f"{tag}: Prompt output variable '{varName}' already declared in file.")
+                    
+                    prompt_outputs_tags[varName] = tag_content.strip()
+                except Exception as e:
+                    errors.append(f"{os.path.relpath(path)}: {str(e)}")
+                    Log.logger.error(f"Error processing {tag} in {path}: {str(e)}")
 
     # After processing all other tags, remove all prompts from the content
     content_without_prompts = content
     for prompt_name, prompt_content in prompts.items():
         prompt = "<prompt:" + prompt_name + ">" + prompt_content + "<" + "<prompt:" + prompt_name + "/>"
         content_without_prompts = content_without_prompts.replace(prompt, '')
     Log.logger.debug("Content without prompts:\n" + content_without_prompts)
@@ -135,26 +183,32 @@
                 prompt_outputs.append(prompt_name)
             else:
                 Log.logger.debug(f"Skipping {prompt_name} because it is inside the prompt content")
         else:
             Log.logger.debug(f"{prompt_name} not found in content_without_prompts")
 
     # A Task is only created if there are prompts in the file
-    return Task(path, global_context, context_dict, prompts, prompt_outputs, prompt_outputs_tags) if len(prompts) > 0 else None
+    if len(prompts) > 0:
+        task = Task(path, global_context, context_dict, prompts, prompt_outputs, prompt_outputs_tags)
+    else:
+        task = None
+    return task, errors
 
 def parse_tags(file_paths, in_comment_signs):
     tasks = []
+    errors = [] 
     comment_signs = in_comment_signs
 
     for path in file_paths:
         try:
-            task = __tag_parsing_process(path)
+            task, file_errors = __tag_parsing_process(path)
             if task is not None:
                 tasks.append(task)
-        except IOError:
-            Log.logger.debug(f"Could not read file: {path}")
-        except ValueError as ve:
-            Log.logger.debug("An error occurred during tag parsing:")
-            Log.logger.debug(traceback.format_exc())
-            continue
+            if file_errors:
+                errors.extend(file_errors)  # Collect errors from each file
+        except Exception as e:  # Catch general exceptions to collect all errors
+            errors.append(f"{os.path.relpath(path)}: {e}")
+            Log.logger.error(f"Error processing file {path}: {e}", exc_info=True)  # Log with stack trace
+
+    return tasks, errors  # Return both tasks and collected errors
 
     return tasks
```

