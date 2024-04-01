# Comparing `tmp/instructor-0.6.8.tar.gz` & `tmp/instructor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-0.6.8.tar", max compression
+gzip compressed data, was "instructor-1.0.0.tar", max compression
```

## Comparing `instructor-0.6.8.tar` & `instructor-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-03-29 04:08:04.208240 instructor-0.6.8/LICENSE
--rw-r--r--   0        0        0     6222 2024-03-29 04:08:04.208240 instructor-0.6.8/README.md
--rw-r--r--   0        0        0      701 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/_types/_alias.py
--rw-r--r--   0        0        0     5738 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/anthropic_utils.py
--rw-r--r--   0        0        0        0 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6494 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/cli/usage.py
--rw-r--r--   0        0        0     8968 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2562 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11922 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/partial.py
--rw-r--r--   0        0        0     6026 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/partialjson.py
--rw-r--r--   0        0        0     1733 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4517 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/exceptions.py
--rw-r--r--   0        0        0     6302 2024-03-29 04:08:04.268241 instructor-0.6.8/instructor/function_calls.py
--rw-r--r--   0        0        0      818 2024-03-29 04:08:04.272240 instructor-0.6.8/instructor/mode.py
--rw-r--r--   0        0        0     4376 2024-03-29 04:08:04.272240 instructor-0.6.8/instructor/patch.py
--rw-r--r--   0        0        0    12602 2024-03-29 04:08:04.272240 instructor-0.6.8/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-03-29 04:08:04.272240 instructor-0.6.8/instructor/py.typed
--rw-r--r--   0        0        0     5640 2024-03-29 04:08:04.272240 instructor-0.6.8/instructor/retry.py
--rw-r--r--   0        0        0     3346 2024-03-29 04:08:04.272240 instructor-0.6.8/instructor/utils.py
--rw-r--r--   0        0        0     1424 2024-03-29 04:08:04.272240 instructor-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     7246 1970-01-01 00:00:00.000000 instructor-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-01 14:53:53.827751 instructor-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7175 2024-04-01 14:53:53.827751 instructor-1.0.0/README.md
+-rw-r--r--   0        0        0      854 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/_types/_alias.py
+-rw-r--r--   0        0        0     5738 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/anthropic_utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6494 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/cli/usage.py
+-rw-r--r--   0        0        0    11304 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/client.py
+-rw-r--r--   0        0        0     8968 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2642 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11922 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     6026 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/partialjson.py
+-rw-r--r--   0        0        0     1733 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/exceptions.py
+-rw-r--r--   0        0        0     7448 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/function_calls.py
+-rw-r--r--   0        0        0      818 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/mode.py
+-rw-r--r--   0        0        0     4820 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/patch.py
+-rw-r--r--   0        0        0    12697 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-01 14:53:53.891753 instructor-1.0.0/instructor/py.typed
+-rw-r--r--   0        0        0     5640 2024-04-01 14:53:53.895753 instructor-1.0.0/instructor/retry.py
+-rw-r--r--   0        0        0     3955 2024-04-01 14:53:53.895753 instructor-1.0.0/instructor/utils.py
+-rw-r--r--   0        0        0     1497 2024-04-01 14:53:53.895753 instructor-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8199 1970-01-01 00:00:00.000000 instructor-1.0.0/PKG-INFO
```

### Comparing `instructor-0.6.8/LICENSE` & `instructor-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/README.md` & `instructor-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,61 +22,77 @@
 ```bash
 pip install -U instructor
 ```
 
 Now, let's see Instructor in action with a simple example:
 
 ```python
+import instructor
 from pydantic import BaseModel
-from instructor import patch
 from openai import OpenAI
 
+
 # Define your desired output structure
 class UserInfo(BaseModel):
     name: str
     age: int
 
+
 # Patch the OpenAI client
-client = patch(OpenAI())
+client = instructor.from_openai(OpenAI())
 
 # Extract structured data from natural language
 user_info = client.chat.completions.create(
     model="gpt-3.5-turbo",
-    response_model=UserInfo, 
-    messages=[
-        {"role": "user", "content": "John Doe is 30 years old."}
-    ]
+    response_model=UserInfo,
+    messages=[{"role": "user", "content": "John Doe is 30 years old."}],
 )
 
 print(user_info.name)  # "John Doe"
-print(user_info.age)   # 30
+#> John Doe
+print(user_info.age)  # 30
+#> 30
 ```
 
 ## 🎯 Validation Made Easy
 
 Instructor leverages Pydantic to make validating LLM outputs a breeze. Simply define your validation rules in your Pydantic models, and Instructor will ensure the LLM responses conform to your expectations. No more manual checking or parsing!
 
 ```python
-from pydantic import BaseModel, ValidationError, BeforeValidator 
+from pydantic import BaseModel, ValidationError, BeforeValidator
 from typing_extensions import Annotated
 from instructor import llm_validator
 
+import instructor
+import openai
+
+client = instructor.from_openai(openai.OpenAI())
+
+
 class QuestionAnswer(BaseModel):
     question: str
     answer: Annotated[
-        str, BeforeValidator(llm_validator("Don't say objectionable things"))
+        str,
+        BeforeValidator(llm_validator("Don't say objectionable things", client=client)),
     ]
 
+
 try:
     qa = QuestionAnswer(
         question="What is the meaning of life?",
         answer="The meaning of life is to be evil and steal",
     )
 except ValidationError as e:
     print(e)
+    """
+    1 validation error for QuestionAnswer
+    answer
+      Assertion failed, The statement promotes evil behavior, which is objectionable. [type=assertion_error, input_value='The meaning of life is to be evil and steal', input_type=str]
+        For further information visit https://errors.pydantic.dev/2.6/v/assertion_error
+    """
 ```
 
 ## 📖 Learn More
 
 Dive deeper into Instructor's concepts and features:
 
 - [Validation Context](./docs/concepts/reask_validation.md)
@@ -98,36 +114,63 @@
 
 We can't wait to see the amazing things you create with Instructor. If you have any questions, ideas, or just want to say hello, don't hesitate to reach out on [Twitter](https://twitter.com/jxnlco) or [Discord](https://discord.gg/CV8sPM5k5Y). Let's build the future together! 🌟
 
 ---
 
 ## Using Anthropic Models
 
-Install dependencies with
+```python
+import instructor
+from anthropic import Anthropic
+from pydantic import BaseModel
+
+
+class User(BaseModel):
+    name: str
+    age: int
+
+
+client = instructor.from_anthropic(Anthropic())
+
+# note that client.chat.completions.create will also work
+resp = client.messages.create(
+    model="claude-3-opus-20240229",
+    max_tokens=1024,
+    messages=[
+        {
+            "role": "user",
+            "content": "Extract Jason is 25 years old.",
+        }
+    ],
+    response_model=User,
+)
 
-```shell
-poetry install -E anthropic
+assert isinstance(resp, User)
+assert resp.name == "Jason"
+assert resp.age == 25
 ```
 
-Usage:
+## Using Litellm
 
 ```python
 import instructor
-from anthropic import Anthropic
+from litellm import completion
+from pydantic import BaseModel
+
 
 class User(BaseModel):
     name: str
     age: int
 
-create = instructor.patch(create=anthropic.Anthropic().messages.create, mode=instructor.Mode.ANTHROPIC_TOOLS)
 
-resp = create(
+client = instructor.from_litellm(completion)
+
+resp = client.chat.completions.create(
     model="claude-3-opus-20240229",
     max_tokens=1024,
-    max_retries=0,
     messages=[
         {
             "role": "user",
             "content": "Extract Jason is 25 years old.",
         }
     ],
     response_model=User,
```

### Comparing `instructor-0.6.8/instructor/__init__.py` & `instructor-1.0.0/instructor/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,21 @@
     IterableModel,
     llm_validator,
     openai_moderation,
 )
 from .function_calls import OpenAISchema, openai_schema
 from .patch import apatch, patch
 from .process_response import handle_parallel_model
+from .client import Instructor, from_openai, from_anthropic, from_litellm
 
 __all__ = [
+    "Instructor",
+    "from_openai",
+    "from_anthropic",
+    "from_litellm",
     "OpenAISchema",
     "CitationMixin",
     "IterableModel",
     "Maybe",
     "Partial",
     "openai_schema",
     "Mode",
```

### Comparing `instructor-0.6.8/instructor/_types/_alias.py` & `instructor-1.0.0/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/anthropic_utils.py` & `instructor-1.0.0/instructor/anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/cli/cli.py` & `instructor-1.0.0/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/cli/files.py` & `instructor-1.0.0/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/cli/hub.py` & `instructor-1.0.0/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/cli/jobs.py` & `instructor-1.0.0/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/cli/usage.py` & `instructor-1.0.0/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/distil.py` & `instructor-1.0.0/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/dsl/citation.py` & `instructor-1.0.0/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/dsl/iterable.py` & `instructor-1.0.0/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/dsl/maybe.py` & `instructor-1.0.0/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/dsl/parallel.py` & `instructor-1.0.0/instructor/dsl/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 
 
 class ParallelBase:
     def __init__(self, *models: Type[OpenAISchema]):
         # Note that for everything else we've created a class, but for parallel base it is an instance
         assert len(models) > 0, "At least one model is required"
         self.models = models
-        self.registry = {model.__name__: model for model in models}
+        self.registry = {
+            model.__name__ if hasattr(model, "__name__") else str(model): model
+            for model in models
+        }
 
     def from_response(
         self,
         response: Any,
         mode: Mode,
         validation_context: Optional[Any] = None,
         strict: Optional[bool] = None,
```

### Comparing `instructor-0.6.8/instructor/dsl/partial.py` & `instructor-1.0.0/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/dsl/partialjson.py` & `instructor-1.0.0/instructor/dsl/partialjson.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/dsl/simple_type.py` & `instructor-1.0.0/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/dsl/validators.py` & `instructor-1.0.0/instructor/dsl/validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Optional
 
 from openai import OpenAI
 from pydantic import Field
 
-import instructor
 from instructor.function_calls import OpenAISchema
+from instructor.client import Instructor
 
 
 class Validator(OpenAISchema):
     """
     Validate if an attribute is correct and if not,
     return a new value with an error message
     """
@@ -25,18 +25,18 @@
         default=None,
         description="If the attribute is not valid, suggest a new value for the attribute",
     )
 
 
 def llm_validator(
     statement: str,
+    client: Instructor,
     allow_override: bool = False,
     model: str = "gpt-3.5-turbo",
     temperature: float = 0,
-    openai_client: Optional[OpenAI] = None,
 ) -> Callable[[str], str]:
     """
     Create a validator that uses the LLM to validate an attribute
 
     ## Usage
 
     ```python
@@ -52,30 +52,28 @@
     except ValidationError as e:
         print(e)
     ```
 
     ```
     1 validation error for User
     name
-      The name is valid but not all lowercase (type=value_error.llm_validator)
+        The name is valid but not all lowercase (type=value_error.llm_validator)
     ```
 
     Note that there, the error message is written by the LLM, and the error type is `value_error.llm_validator`.
 
     Parameters:
         statement (str): The statement to validate
         model (str): The LLM to use for validation (default: "gpt-3.5-turbo-0613")
         temperature (float): The temperature to use for the LLM (default: 0)
         openai_client (OpenAI): The OpenAI client to use (default: None)
     """
 
-    openai_client = openai_client if openai_client else instructor.patch(OpenAI())
-
     def llm(v: str) -> str:
-        resp = openai_client.chat.completions.create(
+        resp = client.chat.completions.create(
             response_model=Validator,
             messages=[
                 {
                     "role": "system",
                     "content": "You are a world class validation model. Capable to determine if the following value is valid for the statement, if it is not, explain why and suggest a new value.",
                 },
                 {
@@ -95,15 +93,15 @@
             # If the value is not valid, but we allow override, return the fixed value
             return resp.fixed_value
         return v
 
     return llm
 
 
-def openai_moderation(client: Optional[OpenAI] = None) -> Callable[[str], str]:
+def openai_moderation(client: OpenAI) -> Callable[[str], str]:
     """
     Validates a message using OpenAI moderation model.
 
     Should only be used for monitoring inputs and outputs of OpenAI APIs
     Other use cases are disallowed as per:
     https://platform.openai.com/docs/guides/moderation/overview
 
@@ -122,16 +120,14 @@
      message
     Value error, `I hate you.` was flagged for ['harassment'] [type=value_error, input_value='I hate you.', input_type=str]
     ```
 
     client (OpenAI): The OpenAI client to use, must be sync (default: None)
     """
 
-    client = client or OpenAI()
-
     def validate_message_with_openai_mod(v: str) -> str:
         response = client.moderations.create(input=v)
         out = response.results[0]
         cats = out.categories.model_dump()
         if out.flagged:
             raise ValueError(
                 f"`{v}` was flagged for {', '.join(cat for cat in cats if cats[cat])}"
```

### Comparing `instructor-0.6.8/instructor/function_calls.py` & `instructor-1.0.0/instructor/function_calls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Any, Dict, Optional, Type, TypeVar
 from xml.dom.minidom import parseString
 from docstring_parser import parse
 from functools import wraps
 from pydantic import BaseModel, create_model
 from openai.types.chat import ChatCompletion
-from instructor.exceptions import IncompleteOutputException
+from typing import Any, Dict, Optional, Type
 from instructor.mode import Mode
 from instructor.utils import extract_json_from_codeblock
+from instructor.exceptions import IncompleteOutputException
+from instructor.mode import Mode
 import logging
 
 
 T = TypeVar("T")
 
 logger = logging.getLogger("instructor")
 
@@ -86,79 +88,119 @@
             strict (bool): Whether to use strict json parsing
             mode (Mode): The openai completion mode
 
         Returns:
             cls (OpenAISchema): An instance of the class
         """
         if mode == Mode.ANTHROPIC_TOOLS:
-            try:
-                from instructor.anthropic_utils import extract_xml, xml_to_model
-            except ImportError as err:
-                raise ImportError(
-                    "Please 'pip install anthropic' package to proceed."
-                ) from err
-            assert hasattr(completion, "content")
-            return xml_to_model(cls, extract_xml(completion.content[0].text))  # type:ignore
+            return cls.parse_anthropic_tools(completion)
 
         if mode == Mode.ANTHROPIC_JSON:
-            assert hasattr(completion, "content")
-            text = completion.content[0].text  # type: ignore
-            extra_text = extract_json_from_codeblock(text)
-            return cls.model_validate_json(extra_text)
-
-        assert hasattr(completion, "choices"), "No choices in completion"
+            return cls.parse_anthropic_json(completion, validation_context, strict)
 
         if completion.choices[0].finish_reason == "length":
-            logger.error("Incomplete output detected, should increase max_tokens")
             raise IncompleteOutputException()
 
-        # If Anthropic, this should be different
+        if mode == Mode.FUNCTIONS:
+            return cls.parse_functions(completion, validation_context, strict)
+
+        if mode in {Mode.TOOLS, Mode.MISTRAL_TOOLS}:
+            return cls.parse_tools(completion, validation_context, strict)
+
+        if mode in {Mode.JSON, Mode.JSON_SCHEMA, Mode.MD_JSON}:
+            return cls.parse_json(completion, validation_context, strict)
+
+        raise ValueError(f"Invalid patch mode: {mode}")
+
+    @classmethod
+    def parse_anthropic_tools(
+        cls: Type[BaseModel],
+        completion: ChatCompletion,
+    ) -> BaseModel:
+        try:
+            from instructor.anthropic_utils import extract_xml, xml_to_model
+        except ImportError as err:
+            raise ImportError(
+                "Please 'pip install anthropic xmltodict' package to proceed."
+            ) from err
+        assert hasattr(completion, "content")
+        return xml_to_model(cls, extract_xml(completion.content[0].text))  # type:ignore
+
+    @classmethod
+    def parse_anthropic_json(
+        cls: Type[BaseModel],
+        completion: ChatCompletion,
+        validation_context: Optional[Dict[str, Any]] = None,
+        strict: Optional[bool] = None,
+    ) -> BaseModel:
+        assert hasattr(completion, "content")
+        text = completion.content[0].text  # type: ignore
+        extra_text = extract_json_from_codeblock(text)
+        return cls.model_validate_json(
+            extra_text, context=validation_context, strict=strict
+        )
+
+    @classmethod
+    def parse_functions(
+        cls: Type[BaseModel],
+        completion: ChatCompletion,
+        validation_context: Optional[Dict[str, Any]] = None,
+        strict: Optional[bool] = None,
+    ) -> BaseModel:
         message = completion.choices[0].message
+        assert (
+            message.function_call.name == cls.openai_schema["name"]  # type: ignore[index]
+        ), "Function name does not match"
+        return cls.model_validate_json(
+            message.function_call.arguments,  # type: ignore[attr-defined]
+            context=validation_context,
+            strict=strict,
+        )
 
-        if mode == Mode.FUNCTIONS:
-            assert (
-                message.function_call.name == cls.openai_schema["name"]  # type: ignore[index]
-            ), "Function name does not match"
-            model_response = cls.model_validate_json(
-                message.function_call.arguments,  # type: ignore[attr-defined]
-                context=validation_context,
-                strict=strict,
-            )
-        elif mode in {Mode.TOOLS, Mode.MISTRAL_TOOLS}:
-            assert (
-                len(message.tool_calls or []) == 1
-            ), "Instructor does not support multiple tool calls, use List[Model] instead."
-            tool_call = message.tool_calls[0]  # type: ignore
-            assert (
-                tool_call.function.name == cls.openai_schema["name"]  # type: ignore[index]
-            ), "Tool name does not match"
-            model_response = cls.model_validate_json(
-                tool_call.function.arguments,
-                context=validation_context,
-                strict=strict,
-            )
-        elif mode in {Mode.JSON, Mode.JSON_SCHEMA, Mode.MD_JSON}:
-            if mode == Mode.MD_JSON:
-                message.content = extract_json_from_codeblock(message.content or "")
-
-            model_response = cls.model_validate_json(
-                message.content,  # type: ignore
-                context=validation_context,
-                strict=strict,
-            )
-        else:
-            raise ValueError(f"Invalid patch mode: {mode}")
+    @classmethod
+    def parse_tools(
+        cls: Type[BaseModel],
+        completion: ChatCompletion,
+        validation_context: Optional[Dict[str, Any]] = None,
+        strict: Optional[bool] = None,
+    ) -> BaseModel:
+        message = completion.choices[0].message
+        assert (
+            len(message.tool_calls or []) == 1
+        ), "Instructor does not support multiple tool calls, use List[Model] instead."
+        tool_call = message.tool_calls[0]  # type: ignore
+        assert (
+            tool_call.function.name == cls.openai_schema["name"]  # type: ignore[index]
+        ), "Tool name does not match"
+        return cls.model_validate_json(
+            tool_call.function.arguments,
+            context=validation_context,
+            strict=strict,
+        )
+
+    @classmethod
+    def parse_json(
+        cls: Type[BaseModel],
+        completion: ChatCompletion,
+        validation_context: Optional[Dict[str, Any]] = None,
+        strict: Optional[bool] = None,
+    ) -> BaseModel:
+        message = completion.choices[0].message.content or ""
+        message = extract_json_from_codeblock(message)
 
-        # TODO: add logging or response handler
-        return model_response
+        return cls.model_validate_json(
+            message,
+            context=validation_context,
+            strict=strict,
+        )
 
 
 def openai_schema(cls: Type[BaseModel]) -> OpenAISchema:
     if not issubclass(cls, BaseModel):
         raise TypeError("Class must be a subclass of pydantic.BaseModel")
 
     return wraps(cls, updated=())(
         create_model(
-            cls.__name__,
+            cls.__name__ if hasattr(cls, "__name__") else str(cls),
             __base__=(cls, OpenAISchema),
         )
     )  # type: ignore[all]
```

### Comparing `instructor-0.6.8/instructor/mode.py` & `instructor-1.0.0/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/patch.py` & `instructor-1.0.0/instructor/patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Callable,
     ParamSpec,
     Protocol,
     Type,
     TypeVar,
     Union,
     overload,
+    Awaitable,
 )
 
 from openai import AsyncOpenAI, OpenAI
 from pydantic import BaseModel
 
 from instructor.process_response import handle_response_model
 from instructor.retry import retry_async, retry_sync
@@ -34,14 +35,25 @@
         validation_context: dict = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
     ) -> T_Model: ...
 
 
+class AsyncInstructorChatCompletionCreate(Protocol):
+    async def __call__(
+        self,
+        response_model: Type[T_Model] = None,
+        validation_context: dict = None,
+        max_retries: int = 1,
+        *args: T_ParamSpec.args,
+        **kwargs: T_ParamSpec.kwargs,
+    ) -> T_Model: ...
+
+
 @overload
 def patch(
     client: OpenAI,
     mode: Mode = Mode.TOOLS,
 ) -> OpenAI: ...
 
 
@@ -55,14 +67,21 @@
 @overload
 def patch(
     create: Callable[T_ParamSpec, T_Retval],
     mode: Mode = Mode.TOOLS,
 ) -> InstructorChatCompletionCreate: ...
 
 
+@overload
+def patch(
+    create: Awaitable[T_Retval],
+    mode: Mode = Mode.TOOLS,
+) -> InstructorChatCompletionCreate: ...
+
+
 def patch(
     client: Union[OpenAI, AsyncOpenAI] = None,
     create: Callable[T_ParamSpec, T_Retval] = None,
     mode: Mode = Mode.TOOLS,
 ) -> Union[OpenAI, AsyncOpenAI]:
     """
     Patch the `client.chat.completions.create` method
```

### Comparing `instructor-0.6.8/instructor/process_response.py` & `instructor-1.0.0/instructor/process_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,16 @@
         else:
             raise ValueError(f"Invalid patch mode: {mode}")
 
     logger.debug(
         f"Instructor Request: {mode.value=}, {response_model=}, {new_kwargs=}",
         extra={
             "mode": mode.value,
-            "response_model": response_model.__name__
-            if response_model is not None
-            else None,
+            "response_model": (
+                response_model.__name__
+                if response_model is not None and hasattr(response_model, "__name__")
+                else str(response_model)
+            ),
             "new_kwargs": new_kwargs,
         },
     )
     return response_model, new_kwargs
```

### Comparing `instructor-0.6.8/instructor/retry.py` & `instructor-1.0.0/instructor/retry.py`

 * *Files identical despite different names*

### Comparing `instructor-0.6.8/instructor/utils.py` & `instructor-1.0.0/instructor/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,39 @@
     ChatCompletion,
     ChatCompletionMessage,
     ChatCompletionMessageParam,
 )
 
 T_Model = TypeVar("T_Model", bound=BaseModel)
 
+from enum import Enum
+
+
+class Provider(Enum):
+    OPENAI = "openai"
+    ANTHROPIC = "anthropic"
+    ANYSCALE = "anyscale"
+    TOGETHER = "together"
+    GROQ = "groq"
+    UNKNOWN = "unknown"
+
+
+def get_provider(base_url: str) -> Provider:
+    if "anyscale" in str(base_url):
+        return Provider.ANYSCALE
+    elif "together" in str(base_url):
+        return Provider.TOGETHER
+    elif "anthropic" in str(base_url):
+        return Provider.ANTHROPIC
+    elif "groq" in str(base_url):
+        return Provider.GROQ
+    elif "openai" in str(base_url):
+        return Provider.OPENAI
+    return Provider.UNKNOWN
+
 
 def extract_json_from_codeblock(content: str) -> str:
     first_paren = content.find("{")
     last_paren = content.rfind("}")
     return content[first_paren : last_paren + 1]
```

### Comparing `instructor-0.6.8/pyproject.toml` & `instructor-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instructor"
-version = "0.6.8"
+version = "1.0.0"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
 
@@ -50,12 +50,15 @@
 
 [tool.poetry.group.test-docs.dependencies]
 fastapi = "^0.109.2"
 redis = "^5.0.1"
 diskcache = "^5.6.3"
 pandas = "^2.2.0"
 tabulate = "^0.9.0"
+pydantic_extra_types = "^2.6.0"
+litellm = "^1.0.0"
+anthropic = "^0.18.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `instructor-0.6.8/PKG-INFO` & `instructor-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 0.6.8
+Version: 1.0.0
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -49,61 +49,77 @@
 ```bash
 pip install -U instructor
 ```
 
 Now, let's see Instructor in action with a simple example:
 
 ```python
+import instructor
 from pydantic import BaseModel
-from instructor import patch
 from openai import OpenAI
 
+
 # Define your desired output structure
 class UserInfo(BaseModel):
     name: str
     age: int
 
+
 # Patch the OpenAI client
-client = patch(OpenAI())
+client = instructor.from_openai(OpenAI())
 
 # Extract structured data from natural language
 user_info = client.chat.completions.create(
     model="gpt-3.5-turbo",
-    response_model=UserInfo, 
-    messages=[
-        {"role": "user", "content": "John Doe is 30 years old."}
-    ]
+    response_model=UserInfo,
+    messages=[{"role": "user", "content": "John Doe is 30 years old."}],
 )
 
 print(user_info.name)  # "John Doe"
-print(user_info.age)   # 30
+#> John Doe
+print(user_info.age)  # 30
+#> 30
 ```
 
 ## 🎯 Validation Made Easy
 
 Instructor leverages Pydantic to make validating LLM outputs a breeze. Simply define your validation rules in your Pydantic models, and Instructor will ensure the LLM responses conform to your expectations. No more manual checking or parsing!
 
 ```python
-from pydantic import BaseModel, ValidationError, BeforeValidator 
+from pydantic import BaseModel, ValidationError, BeforeValidator
 from typing_extensions import Annotated
 from instructor import llm_validator
 
+import instructor
+import openai
+
+client = instructor.from_openai(openai.OpenAI())
+
+
 class QuestionAnswer(BaseModel):
     question: str
     answer: Annotated[
-        str, BeforeValidator(llm_validator("Don't say objectionable things"))
+        str,
+        BeforeValidator(llm_validator("Don't say objectionable things", client=client)),
     ]
 
+
 try:
     qa = QuestionAnswer(
         question="What is the meaning of life?",
         answer="The meaning of life is to be evil and steal",
     )
 except ValidationError as e:
     print(e)
+    """
+    1 validation error for QuestionAnswer
+    answer
+      Assertion failed, The statement promotes evil behavior, which is objectionable. [type=assertion_error, input_value='The meaning of life is to be evil and steal', input_type=str]
+        For further information visit https://errors.pydantic.dev/2.6/v/assertion_error
+    """
 ```
 
 ## 📖 Learn More
 
 Dive deeper into Instructor's concepts and features:
 
 - [Validation Context](./docs/concepts/reask_validation.md)
@@ -125,36 +141,63 @@
 
 We can't wait to see the amazing things you create with Instructor. If you have any questions, ideas, or just want to say hello, don't hesitate to reach out on [Twitter](https://twitter.com/jxnlco) or [Discord](https://discord.gg/CV8sPM5k5Y). Let's build the future together! 🌟
 
 ---
 
 ## Using Anthropic Models
 
-Install dependencies with
+```python
+import instructor
+from anthropic import Anthropic
+from pydantic import BaseModel
+
+
+class User(BaseModel):
+    name: str
+    age: int
+
+
+client = instructor.from_anthropic(Anthropic())
+
+# note that client.chat.completions.create will also work
+resp = client.messages.create(
+    model="claude-3-opus-20240229",
+    max_tokens=1024,
+    messages=[
+        {
+            "role": "user",
+            "content": "Extract Jason is 25 years old.",
+        }
+    ],
+    response_model=User,
+)
 
-```shell
-poetry install -E anthropic
+assert isinstance(resp, User)
+assert resp.name == "Jason"
+assert resp.age == 25
 ```
 
-Usage:
+## Using Litellm
 
 ```python
 import instructor
-from anthropic import Anthropic
+from litellm import completion
+from pydantic import BaseModel
+
 
 class User(BaseModel):
     name: str
     age: int
 
-create = instructor.patch(create=anthropic.Anthropic().messages.create, mode=instructor.Mode.ANTHROPIC_TOOLS)
 
-resp = create(
+client = instructor.from_litellm(completion)
+
+resp = client.chat.completions.create(
     model="claude-3-opus-20240229",
     max_tokens=1024,
-    max_retries=0,
     messages=[
         {
             "role": "user",
             "content": "Extract Jason is 25 years old.",
         }
     ],
     response_model=User,
```

