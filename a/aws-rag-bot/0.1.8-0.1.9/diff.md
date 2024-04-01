# Comparing `tmp/aws_rag_bot-0.1.8.tar.gz` & `tmp/aws_rag_bot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_rag_bot-0.1.8.tar", max compression
+gzip compressed data, was "aws_rag_bot-0.1.9.tar", max compression
```

## Comparing `aws_rag_bot-0.1.8.tar` & `aws_rag_bot-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2024-02-28 14:24:35.569084 aws_rag_bot-0.1.8/LICENSE
--rw-r--r--   0        0        0     6197 2024-02-29 03:26:28.787937 aws_rag_bot-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-02-28 14:24:35.569790 aws_rag_bot-0.1.8/aws_rag_bot/__init__.py
--rw-r--r--   0        0        0    18903 2024-02-29 15:18:48.678151 aws_rag_bot-0.1.8/aws_rag_bot/aws_opensearch_vector_database.py
--rw-r--r--   0        0        0     1818 2024-02-28 14:24:35.570552 aws_rag_bot-0.1.8/aws_rag_bot/kustomer.py
--rw-r--r--   0        0        0     2614 2024-02-28 14:24:35.570736 aws_rag_bot-0.1.8/aws_rag_bot/prompt_library.py
--rw-r--r--   0        0        0    12926 2024-02-29 13:57:45.861418 aws_rag_bot-0.1.8/aws_rag_bot/rag_chatbot.py
--rw-r--r--   0        0        0      801 2024-02-29 22:45:07.066903 aws_rag_bot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7441 1970-01-01 00:00:00.000000 aws_rag_bot-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-02-28 14:24:35.569084 aws_rag_bot-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6843 2024-03-06 19:20:31.231198 aws_rag_bot-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-28 14:24:35.569790 aws_rag_bot-0.1.9/aws_rag_bot/__init__.py
+-rw-r--r--   0        0        0    18903 2024-02-29 15:18:48.678151 aws_rag_bot-0.1.9/aws_rag_bot/aws_opensearch_vector_database.py
+-rw-r--r--   0        0        0     1818 2024-02-28 14:24:35.570552 aws_rag_bot-0.1.9/aws_rag_bot/kustomer.py
+-rw-r--r--   0        0        0     3654 2024-03-06 19:20:31.231748 aws_rag_bot-0.1.9/aws_rag_bot/prompt_library.py
+-rw-r--r--   0        0        0    15663 2024-03-06 19:20:31.232579 aws_rag_bot-0.1.9/aws_rag_bot/rag_chatbot.py
+-rw-r--r--   0        0        0      876 2024-03-06 19:21:05.254909 aws_rag_bot-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8087 1970-01-01 00:00:00.000000 aws_rag_bot-0.1.9/PKG-INFO
```

### Comparing `aws_rag_bot-0.1.8/LICENSE` & `aws_rag_bot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_rag_bot-0.1.8/README.md` & `aws_rag_bot-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 Content loading also needed to be highly refined allowing me to control each source easily.
 
 This library is meant more to provide a complete working set of examples and less to be an out-of-the-box library to use as-is.
 
 
 ## Features and aspects of interest
 - **LangChain** - Great framework building Generative AI applications. 
-- **LLM Model Support** - Defaults to AWS Bedrock Titan LLM, but supports other Bedrock models (LLama 2, Jurassic) OpenAI (GTP-3.5 and GTP-4), Google Gemini
+- **LLM Model Support** - Defaults to AWS Bedrock Titan LLM, but supports other Bedrock models (LLama 2, Jurassic, Anthropic Claude) OpenAI (GTP-3.5 and GTP-4), Google Gemini
 - **LangChain LLM Callbacks** - Example of using LLM Callbacks, provided here for custom costing 
 - **Conversational Memory** -- Designed to manage chat history memory from the client side - to support a serverless model
 - **OpenSearch** - an AWS hosted semantic search service which has a vector database that is valuable in the retrieval feature of RAG
 - **OpenSearch loading library** - making it easier to load multiple content sources into an OpenSearch vector database.
 - **Langchain LCEL Chains** - for more flexible chaining of steps in the RAG app
-- **Multiple embedding models** - Defaults to Bedrock Titan, but supports OpenAI and Hugging Face
+- **Multiple embedding models** - Defaults to Bedrock Titan, OpenAI and Hugging Face and Coherence
 - **Web and directory crawlers** - for loading content into the vector DB.  Lots of fine-tuning to document selection features - whitelisting, black listing, etc.
 - **Prompt library management** - making it easier to implement query routing to optimize for specific domains of questions
 - **LangSmith logging** - for logging and debugging
 
 ## How to use
 ### Prerequisites
 - Python 3.11 (may work on older, but this was the target version used)
@@ -46,15 +46,15 @@
 ```
 
 Alternatively, you can install the package from PyPi with the following command:
 ```bash
 pip install aws-rag-bot
 ```
 Where the PyPi package is available at https://pypi.org/project/aws-rag-bot/
-
+****
 ### Sample Code
 This is a very simple, high-level example.  Check out the rag_bot_code_samples.ipynb for a more.
 First step is to have content in your vector database.  
 ```python
 from open_search_vector_db.aws_opensearch_vector_database import OpenSearchVectorDBLoader
 content_sources = [{"name": "Internal KB Docs", "type": "PDF", "location": "kb-docs"}]
 vectordb_loader = OpenSearchVectorDBLoader(domain_name=my_open_search_domain_name,  
@@ -88,14 +88,26 @@
 A very simple command line client program has been created as an example and tool to test.  It is called chatbot_client.py.  
 It is a simple command line program that will ask a question and then print the response while retaining the chat history for context.  
 
 ```bash
 python chatbot_client.py my-opensource-domain-name
 ```
 
+### Running tests
+There are two test modules in the tests folder used to run through search and the RAG bot to make sure everything is working as well as provide
+some additional samples of how to use the framework.
+
+### Using Ragas evaluation framework
+Ragas is one of a variety of evaluation tools for RAG applications.  
+It can be used to evaluate both the retrieval and generation aspects of the RAG bot.  
+With an evaluation tool you can then use this project's features to vary whatever aspects you need
+and compare the results to make decisions and tune. 
+A simple example of this can be found in the tests folder.
+
+
 ## References
 **Vector Database:**  May references show using Chroma and FAISS, but I needed a solution that worked well in a Lambda serverless environment.  
 Ideally it would be at AWS keeping my stack uniform.  
 - https://aws.amazon.com/what-is/vector-databases/
 
 Ultimately I chose OpenSearch because of cost, support by LangChain and a serverless version I plan to evaluate
```

### Comparing `aws_rag_bot-0.1.8/aws_rag_bot/aws_opensearch_vector_database.py` & `aws_rag_bot-0.1.9/aws_rag_bot/aws_opensearch_vector_database.py`

 * *Files identical despite different names*

### Comparing `aws_rag_bot-0.1.8/aws_rag_bot/kustomer.py` & `aws_rag_bot-0.1.9/aws_rag_bot/kustomer.py`

 * *Files identical despite different names*

### Comparing `aws_rag_bot-0.1.8/aws_rag_bot/rag_chatbot.py` & `aws_rag_bot-0.1.9/aws_rag_bot/rag_chatbot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from datetime import datetime
-
 import boto3
 from dotenv import find_dotenv, load_dotenv
+
 from langchain.llms.bedrock import Bedrock
 from langchain_core.output_parsers import StrOutputParser
+from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.messages import AIMessage, HumanMessage
 from langchain_openai import ChatOpenAI
 from langchain_google_genai import ChatGoogleGenerativeAI
 from langchain.schema.runnable import RunnableConfig
 from langchain.callbacks.base import BaseCallbackHandler
 
 # Code in this project
 from aws_rag_bot.aws_opensearch_vector_database import (
     EmbeddingTypes,
     OpenSearchVectorDBQuery
 )
-from aws_rag_bot.prompt_library import DefaultPrompts
+from aws_rag_bot.prompt_library import *
+
 
 class LlmModelTypes:
     BEDROCK_LLAMA2 = "bedrock_llama2"
     BEDROCK_JURRASIC2_ULTRA = "bedrock_jurrasic2_ultra"
     BEDROCK_TITAN_EXPRESS = "bedrock_titan_express"
     BEDROCK_CLAUDE_INSTANT = "bedrock_claude_instant"
+    BEDROCK_CLAUDE_21 = "bedrock_claude21"
     OPENAI_GPT4 = "openai_gpt4"
     OPENAI_GPT35 = "openai_gpt35"
     GOOGLE_GEMINI_PRO = "google_gemini_pro"
 
 
 def structure_message_history(chat_history):
     # format of chat history is: {"question": "****", "response": "****"]
@@ -54,15 +57,14 @@
     __total_run_duration = 0
     __last_run_prompt = None
     __last_run_input_tokens = 0
     __last_run_output_tokens = 0
     __last_run_cost = 0
     __last_run_duration = 0
 
-
     __bedrock_model_def_llama2 = {
         "key": "bedrock_llama2",
         "name": "Bedrock Llama 2",
         "id": "meta.llama2-70b-chat-v1",
         "client_name": "bedrock-runtime",
         "region_name": "us-east-1",
         "kwargs": {
@@ -119,16 +121,34 @@
         "kwargs": {
             "max_tokens_to_sample": 1000,
             "temperature": 0.1,
             "top_p": 0.5,
             "top_k": 250,
         },
         "model_cost": {
-            "input_token_cost": 0.00163 / 1000,
-            "output_token_cost": 0.00551 / 1000
+            "input_token_cost": 0.00080 / 1000,
+            "output_token_cost": 0.00240 / 1000
+        }
+    }
+
+    __bedrock_model_def_claude21 = {
+        "key": "bedrock_claude21",
+        "name": "Bedrock Claude v2.1",
+        "id": "anthropic.claude-v2:1",
+        "client_name": "bedrock-runtime",
+        "region_name": "us-east-1",
+        "kwargs": {
+            "max_tokens_to_sample": 1000,
+            "temperature": 0.1,
+            "top_p": 0.5,
+            "top_k": 250,
+        },
+        "model_cost": {
+            "input_token_cost": 0.00080 / 1000,
+            "output_token_cost": 0.00240 / 1000
         }
     }
 
     __open_ai_model_def_gpt4 = {
         "key": "openai_gpt4",
         "name": "OpenAI GPT-4",
         "id": "gpt-4",
@@ -163,25 +183,26 @@
         "name": "Google Gemini Pro",
         "id": "gemini-pro",
         "client_name": "google",
         "kwargs": {
             "maxTokens": 500,
             "temperature": 0.5,
         },
-        "model_cost": { # uses cost/char... estimated at 4 chars per token
+        "model_cost": {  # uses cost/char... estimated at 4 chars per token
             "input_token_cost": 0.000125 * 4 / 1000,
             "output_token_cost": 0.000375 * 4 / 1000
         }
     }
 
     __model_options = [
         __bedrock_model_def_llama2,
         __bedrock_model_def_jurrasic2_ultra,
         __bedrock_model_def_titan_express,
         __bedrock_model_def_claude_instant,
+        __bedrock_model_def_claude21,
         __open_ai_model_def_gpt4,
         __open_ai_model_def_gpt35,
         __google_gemini_pro
     ]
     __current_model = None
     __prompt_model = None
 
@@ -193,15 +214,15 @@
                  , model_key=LlmModelTypes.BEDROCK_TITAN_EXPRESS
                  , prompt_model=None
                  , embedding_model=EmbeddingTypes.BEDROCK_DEFAULT
                  , verbose=False):
 
         load_dotenv(find_dotenv())
         if prompt_model is None:
-            self.__prompt_model = DefaultPrompts()
+            self.__prompt_model = BasePromptModel()
         else:
             self.__prompt_model = prompt_model
 
         self.__log_verbose = verbose
 
         # Set the current model based on input
         for model_option in self.__model_options:
@@ -215,14 +236,50 @@
         # Initialize the LLM model, memory, and chain
         self.__llm_model = self.__get_llm_model()
         vector_db = OpenSearchVectorDBQuery(domain_name=vector_db_domain,
                                             index_name=index_name,
                                             embedding_model=embedding_model)
         self.__vector_db = vector_db.get_client()
 
+    class RagCallback(BaseCallbackHandler):
+        # https://how.wtf/how-to-count-amazon-bedrock-anthropic-tokens-with-langchain.html
+        def __init__(self, llm, verbose=False):
+            self.llm = llm
+            self.prompt = None
+            self.input_tokens = 0
+            self.output_tokens = 0
+            self.verbose = verbose
+
+        def on_llm_start(self, input, prompts, **kwargs):
+            self.prompt = prompts
+            if self.verbose:
+                print("--------------------- Callback On Start LLM Prompts --------------------------------------")
+                print(prompts)
+                print("------------------------------------------------------------------------------------------")
+            for p in prompts:
+                self.input_tokens = self.llm.get_num_tokens(p)
+
+        def on_llm_end(self, output, **kwargs):
+            results = output.flatten()
+            if self.verbose:
+                print("--------------------- Callback On End LLM Results --------------------------------------")
+                print(results)
+                print("----------------------------------------------------------------------------------------")
+            for r in results:
+                self.output_tokens = self.llm.get_num_tokens(r.generations[0][0].text)
+
+        def cost(self, model_info):
+            if 'model_cost' in model_info:
+                return self.input_tokens * model_info['model_cost']['input_token_cost'] + self.output_tokens * \
+                    model_info['model_cost']['output_token_cost']
+
+        # def on_llm_new_token(self, token, **kwargs):
+        #     Says I need streaming enabled for this to work. maybe later
+        #     self.input_tokens += 1
+
     # Create the LLM model
     def __get_llm_model(self):
         if self.__log_verbose:
             print("RagChatbot: Initializing LLM model")
             print(f"Creating LLM model: {self.__current_model['name']}")
             print(f"  - client: {self.__current_model['client_name']}")
             print(f"  - id: {self.__current_model['id']}")
@@ -239,15 +296,14 @@
 
         llm_model = None
         # Handle creating Bedrock Models
         if self.__current_model['client_name'] == 'bedrock-runtime':
             # Explicitly create client with boto3 to get better control and transparency
             bedrock = boto3.client('bedrock-runtime', region_name=self.__current_model['region_name'])
 
-
             llm_model = Bedrock(
                 model_id=self.__current_model['id'],
                 client=bedrock,
                 model_kwargs=llm_model_kwargs
             )
 
         elif self.__current_model['client_name'] == 'openai':
@@ -266,88 +322,87 @@
 
         return llm_model
 
     def get_llm_model(self):
         return self.__llm_model
 
     def ask_question(self, question, conversation_history=None, verbose=False):
-        contextualize_q_chain = self.__prompt_model.contextualize_q_prompt | self.__llm_model | StrOutputParser()
-        retriever = self.__vector_db.as_retriever()
+        my_callback_handler = self.RagCallback(self.__llm_model, verbose=verbose)
+        chain_config = RunnableConfig(callbacks=[my_callback_handler])
 
-        if conversation_history is None:
-            conversation_history = []
+        # --- If we have history, then summarize along with the question to produce a new question ---
+        # format of chat history is: [{"question": "****", "response": "****"},]
+        #  and is managed and formulated by the client to this call
+        restated_question = None
+        if conversation_history is not None:
+            summary_prompt = ChatPromptTemplate.from_template(self.__prompt_model.summary_prompt_template)
+            history = ""
+            for qa_pair in conversation_history:
+                history += f"Question - {qa_pair['question']}\nResponse - {qa_pair['response']}\n"
+            summary_request = summary_prompt.format(chat_history=history, question=question)
+            # chain = LLMChain(llm=self.__llm_model, prompt=summary_request, callbacks=[my_callback_handler])
+            # chain = LLMChain(llm=self.__llm_model, prompt=summary_prompt, callbacks=[my_callback_handler])
+            # chain = LLMChain(llm=self.__llm_model, callbacks=[my_callback_handler])
+            #
+            # restated_question = chain.invoke({"question": question, "chat_history": history})
+            restated_question = self.__llm_model.invoke(summary_request, config=chain_config)
 
-        class MyCallback(BaseCallbackHandler):
-            # https://how.wtf/how-to-count-amazon-bedrock-anthropic-tokens-with-langchain.html
-            def __init__(self, llm):
-                self.llm = llm
-                self.prompt = None
-                self.input_tokens = 0
-                self.output_tokens = 0
-
-            def on_llm_start(self, input, prompts, **kwargs):
-                self.prompt = prompts
-                for p in prompts:
-                    self.input_tokens = self.llm.get_num_tokens(p)
-
-            def on_llm_end(self, output, **kwargs):
-                results = output.flatten()
-                for r in results:
-                    self.output_tokens = self.llm.get_num_tokens(r.generations[0][0].text)
-
-            def cost(self, model_info):
-                if 'model_cost' in model_info:
-                    return self.input_tokens * model_info['model_cost']['input_token_cost'] + self.output_tokens * \
-                        model_info['model_cost']['output_token_cost']
-
-            # def on_llm_new_token(self, token, **kwargs):
-            #     Says I need streaming enabled for this to work. maybe later
-            #     self.input_tokens += 1
-
-        def format_docs(docs):
-            return "\n\n".join([d.page_content for d in docs])
-
-        def contextualized_question(input: dict):
-            if input.get("chat_history"):
-                return contextualize_q_chain
-            else:
-                return input["question"]
 
-        my_callback_handler = MyCallback(self.__llm_model)
-        chain_config = RunnableConfig(callbacks=[my_callback_handler])
 
-        rag_chain = (
-                RunnablePassthrough.assign(
-                    context=contextualized_question | retriever | format_docs
-                )
-                | self.__prompt_model.qa_prompt
+        else:
+            restated_question = question
+
+        # --- Now we have a restated question, we ask the with the intended prompts ---
+        # Get a retriever
+        retriever = self.__vector_db.as_retriever()
+
+        # Register my callback handler
+
+        template = self.__prompt_model.system_prompt_template
+        prompt = ChatPromptTemplate.from_template(template)
+
+        # This takes the context from the retriever, based on the question, then
+        #   passes the resulting context and question to the prompt template
+        #   then executes the query and returns.
+        my_chain = (
+                {"context": retriever, "question": RunnablePassthrough()}
+                | prompt
                 | self.__llm_model
+                | StrOutputParser()
         )
-
-        # Adds in our callback to the chain
-        rag_chain = rag_chain.with_config(chain_config)
+        # provide config to the chain, which at the moment includes the callback handler
+        my_chain = my_chain.with_config(chain_config)
         start_time = datetime.now()
-        response = rag_chain.invoke({"question": question, "chat_history": conversation_history})
+        if type(restated_question) == AIMessage:
+            answer = my_chain.invoke(restated_question.content)
+        else:
+            answer = my_chain.invoke(restated_question)
+
         end_time = datetime.now()
         duration = end_time - start_time
 
         self.__last_run_input_tokens = my_callback_handler.input_tokens
         self.__last_run_output_tokens = my_callback_handler.output_tokens
         self.__last_run_cost = my_callback_handler.cost(self.__current_model)
         self.__total_cost += my_callback_handler.cost(self.__current_model)
         self.__total_input_tokens += my_callback_handler.input_tokens
         self.__total_output_tokens += my_callback_handler.output_tokens
         self.__last_run_prompt = my_callback_handler.prompt
         self.__last_run_duration = duration.total_seconds()
         self.__total_run_duration += duration.total_seconds()
 
-        if type(response) == AIMessage:
-            return response
-        else:  # This is needed because some LLM's will return a string instead of a AIMessage, like Titan Express
-            return AIMessage(content=response)
+        # if type(response) == AIMessage:
+        #     return response
+        # else:  # This is needed because some LLM's will return a string instead of a AIMessage, like Titan Express
+        #     return AIMessage(content=response)
+
+        if type(answer) == AIMessage:
+            return answer.content
+        else:
+            return answer
 
     def get_model_run_summary(self):
         return {
             "total_cost": self.__total_cost,
             "total_input_tokens": self.__total_input_tokens,
             "total_output_tokens": self.__total_output_tokens,
             "total_run_duration": self.__total_run_duration,
@@ -359,7 +414,10 @@
 
             "model_name": self.__current_model,
             "vector_db_index": self.__prompt_model.llm_index
         }
 
     def get_last_run_prompt(self):
         return self.__last_run_prompt
+
+    def get_vector_db(self):
+        return self.__vector_db
```

### Comparing `aws_rag_bot-0.1.8/pyproject.toml` & `aws_rag_bot-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-rag-bot"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["danjamk <dan@risegardens.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["aws", "rag", "bedrock", "opensearch", "vector database"]
 repository = "https://github.com/harvest2o-llc/aws-rag-bot"
 
@@ -26,10 +26,14 @@
 anthropic = "^0.16.0"
 sentence-transformers = "^2.5.0"
 cohere = "^4.51"
 docx2txt = "^0.8"
 
 
 
+[tool.poetry.group.dev.dependencies]
+ragas = "^0.1.3"
+colorama = "^0.4.6"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aws_rag_bot-0.1.8/PKG-INFO` & `aws_rag_bot-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-rag-bot
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/harvest2o-llc/aws-rag-bot
 License: MIT
 Keywords: aws,rag,bedrock,opensearch,vector database
 Author: danjamk
 Author-email: dan@risegardens.com
 Requires-Python: >=3.11,<3.12
@@ -41,21 +41,21 @@
 Content loading also needed to be highly refined allowing me to control each source easily.
 
 This library is meant more to provide a complete working set of examples and less to be an out-of-the-box library to use as-is.
 
 
 ## Features and aspects of interest
 - **LangChain** - Great framework building Generative AI applications. 
-- **LLM Model Support** - Defaults to AWS Bedrock Titan LLM, but supports other Bedrock models (LLama 2, Jurassic) OpenAI (GTP-3.5 and GTP-4), Google Gemini
+- **LLM Model Support** - Defaults to AWS Bedrock Titan LLM, but supports other Bedrock models (LLama 2, Jurassic, Anthropic Claude) OpenAI (GTP-3.5 and GTP-4), Google Gemini
 - **LangChain LLM Callbacks** - Example of using LLM Callbacks, provided here for custom costing 
 - **Conversational Memory** -- Designed to manage chat history memory from the client side - to support a serverless model
 - **OpenSearch** - an AWS hosted semantic search service which has a vector database that is valuable in the retrieval feature of RAG
 - **OpenSearch loading library** - making it easier to load multiple content sources into an OpenSearch vector database.
 - **Langchain LCEL Chains** - for more flexible chaining of steps in the RAG app
-- **Multiple embedding models** - Defaults to Bedrock Titan, but supports OpenAI and Hugging Face
+- **Multiple embedding models** - Defaults to Bedrock Titan, OpenAI and Hugging Face and Coherence
 - **Web and directory crawlers** - for loading content into the vector DB.  Lots of fine-tuning to document selection features - whitelisting, black listing, etc.
 - **Prompt library management** - making it easier to implement query routing to optimize for specific domains of questions
 - **LangSmith logging** - for logging and debugging
 
 ## How to use
 ### Prerequisites
 - Python 3.11 (may work on older, but this was the target version used)
@@ -78,15 +78,15 @@
 ```
 
 Alternatively, you can install the package from PyPi with the following command:
 ```bash
 pip install aws-rag-bot
 ```
 Where the PyPi package is available at https://pypi.org/project/aws-rag-bot/
-
+****
 ### Sample Code
 This is a very simple, high-level example.  Check out the rag_bot_code_samples.ipynb for a more.
 First step is to have content in your vector database.  
 ```python
 from open_search_vector_db.aws_opensearch_vector_database import OpenSearchVectorDBLoader
 content_sources = [{"name": "Internal KB Docs", "type": "PDF", "location": "kb-docs"}]
 vectordb_loader = OpenSearchVectorDBLoader(domain_name=my_open_search_domain_name,  
@@ -120,14 +120,26 @@
 A very simple command line client program has been created as an example and tool to test.  It is called chatbot_client.py.  
 It is a simple command line program that will ask a question and then print the response while retaining the chat history for context.  
 
 ```bash
 python chatbot_client.py my-opensource-domain-name
 ```
 
+### Running tests
+There are two test modules in the tests folder used to run through search and the RAG bot to make sure everything is working as well as provide
+some additional samples of how to use the framework.
+
+### Using Ragas evaluation framework
+Ragas is one of a variety of evaluation tools for RAG applications.  
+It can be used to evaluate both the retrieval and generation aspects of the RAG bot.  
+With an evaluation tool you can then use this project's features to vary whatever aspects you need
+and compare the results to make decisions and tune. 
+A simple example of this can be found in the tests folder.
+
+
 ## References
 **Vector Database:**  May references show using Chroma and FAISS, but I needed a solution that worked well in a Lambda serverless environment.  
 Ideally it would be at AWS keeping my stack uniform.  
 - https://aws.amazon.com/what-is/vector-databases/
 
 Ultimately I chose OpenSearch because of cost, support by LangChain and a serverless version I plan to evaluate
```

