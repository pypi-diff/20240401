# Comparing `tmp/shuttleai-3.5.tar.gz` & `tmp/shuttleai-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.5.tar", last modified: Mon Mar 25 22:15:56 2024, max compression
+gzip compressed data, was "shuttleai-3.6.tar", last modified: Mon Apr  1 09:39:10 2024, max compression
```

## Comparing `shuttleai-3.5.tar` & `shuttleai-3.6.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 22:15:56.478496 shuttleai-3.5/
--rw-rw-rw-   0        0        0     3842 2024-03-25 22:15:56.477403 shuttleai-3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2024-03-18 01:09:59.000000 shuttleai-3.5/README.md
--rw-rw-rw-   0        0        0       42 2024-03-25 22:15:56.479494 shuttleai-3.5/setup.cfg
--rw-rw-rw-   0        0        0     1200 2024-03-25 22:14:43.000000 shuttleai-3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-25 22:15:56.408654 shuttleai-3.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-25 22:15:56.441201 shuttleai-3.5/src/shuttleai/
--rw-rw-rw-   0        0        0      674 2024-03-25 22:15:14.000000 shuttleai-3.5/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4565 2024-03-25 22:14:33.000000 shuttleai-3.5/src/shuttleai/cli.py
--rw-rw-rw-   0        0        0     1636 2024-03-18 00:36:12.000000 shuttleai-3.5/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-03-25 22:15:56.472401 shuttleai-3.5/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      247 2024-03-18 09:39:16.000000 shuttleai-3.5/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     2044 2024-03-18 09:49:04.000000 shuttleai-3.5/src/shuttleai/schemas/schemas.py
--rw-rw-rw-   0        0        0     3328 2024-03-25 22:15:10.000000 shuttleai-3.5/src/shuttleai/shuttleai.py
--rw-rw-rw-   0        0        0    11868 2024-03-25 22:15:08.000000 shuttleai-3.5/src/shuttleai/shuttleai_async.py
-drwxrwxrwx   0        0        0        0 2024-03-25 22:15:56.474407 shuttleai-3.5/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     3842 2024-03-25 22:15:56.000000 shuttleai-3.5/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-03-25 22:15:56.000000 shuttleai-3.5/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 22:15:56.000000 shuttleai-3.5/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-25 22:15:56.000000 shuttleai-3.5/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-03-25 22:15:56.000000 shuttleai-3.5/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-25 22:15:56.000000 shuttleai-3.5/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.048285 shuttleai-3.6/
+-rw-rw-rw-   0        0        0     3915 2024-04-01 09:39:10.046286 shuttleai-3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3083 2024-04-01 03:32:40.000000 shuttleai-3.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 09:39:10.049287 shuttleai-3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-04-01 09:35:51.000000 shuttleai-3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:39:09.985282 shuttleai-3.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 09:39:09.991285 shuttleai-3.6/src/shuttleai/
+-rw-rw-rw-   0        0        0      574 2024-04-01 09:37:08.000000 shuttleai-3.6/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4422 2024-04-01 09:11:07.000000 shuttleai-3.6/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.039286 shuttleai-3.6/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-01 09:37:00.000000 shuttleai-3.6/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17148 2024-04-01 09:36:40.000000 shuttleai-3.6/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0     3329 2024-04-01 09:19:27.000000 shuttleai-3.6/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.6/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.042281 shuttleai-3.6/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-01 03:32:40.000000 shuttleai-3.6/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-04-01 03:34:52.000000 shuttleai-3.6/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.044291 shuttleai-3.6/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     3915 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.5/PKG-INFO` & `shuttleai-3.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.5
+Version: 3.6
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,28 +19,29 @@
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib.
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
-```sh
+```ShellSession
 pip install shuttleai
 ```
 
 ## ShuttleAI CLI
-```sh
+```ShellSession
 pip install shuttleai[cli]
 ```
 
 # Usage
 ## ShuttleAI CLI
-```sh
-shuttleai-cli --help
+```ShellSession
+shuttleai
 ```
+*That's it! Just type `shuttleai` in your terminal!*
 ## ShuttleAI
 > [!IMPORTANT]
 > It is strongly recommended to use the asynchronous client instead of the synchronous client.
 ```py
 import asyncio
 from shuttleai import *
```

### Comparing `shuttleai-3.5/README.md` & `shuttleai-3.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,101 @@
-# The official Python library for the ShuttleAI API
-Access the ShuttleAI API with a simple, user-friendly lib.
-
-> *PRs appreciated 🙂*
-# Installation
-## ShuttleAI
-```sh
-pip install shuttleai
-```
-
-## ShuttleAI CLI
-```sh
-pip install shuttleai[cli]
-```
-
-# Usage
-## ShuttleAI CLI
-```sh
-shuttleai-cli --help
-```
-## ShuttleAI
-> [!IMPORTANT]
-> It is strongly recommended to use the asynchronous client instead of the synchronous client.
-```py
-import asyncio
-from shuttleai import *
-
-SHUTTLE_KEY = "ShuttleAPI Key"
-
-async def main():
-    async with ShuttleAsyncClient(SHUTTLE_KEY, timeout=60) as shuttle:
-        """Optionally change base url"""
-        # shuttle.base_url = "https://api.shuttleai.app/v1"
-
-        """Get Models Example"""
-        # response = await shuttle.get_models()
-        # print(response)
-        """Get Model Example"""
-        # response = await shuttle.get_model("gpt-4")
-        # print(response)
-        """Streaming Example"""
-        # response = await shuttle.chat_completion(
-        #     model="gpt-3.5-turbo",
-        #     messages="write me a short story about bees",
-        #     stream=True,
-        #     plain=True,
-        #     internet=False
-        # )
-        # async for chunk in response:
-        #     print(chunk.choices[0].delta.content)
-        """Non-Streaming Example"""
-        # response = await shuttle.chat_completion(
-        #     model="gpt-3.5-turbo",
-        #     messages=[{"role":"user","content":"write me a short story about bees"}],
-        #     stream=False,
-        #     plain=False,
-        #     internet=False,
-        #     max_tokens=100,
-        #     temperature=0.5,
-        #     image="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png"
-        # )
-        # print(response)
-        """Image Generation Example"""
-        # response = await shuttle.images_generations(
-        #     model='sdxl',
-        #     prompt='a cute cat',
-        #     n=1,
-        # )
-        # print(response)
-        """Audio Generation Example"""
-        # response = await shuttle.audio_generations(
-        #     model='eleven-labs-999',
-        #     input='Once upon a time, there was a cute cat wondering through a dark, cold forest.',
-        #     voice="mimi"
-        # )
-        # print(response)
-        """Audio Transcription Example"""
-        # response = await shuttle.audio_transcriptions(
-        #     model='whisper-large',
-        #     file="test.mp3"
-        # )
-        # print(response)
-        """Moderation Example"""
-        # response = await shuttle.moderations(
-        #     model='text-moderation-latest',
-        #     input="I hate you"
-        # )
-        # print(response)
-        """Embeddings Example"""
-        # response = await shuttle.embeddings(
-        #     model='text-embedding-ada-002',
-        #     input="Hello there world"
-        # )
-        # print(response)
-
-
-if __name__ == "__main__":
-    loop = asyncio.new_event_loop()
-    loop.run_until_complete(main())
-```
+# The official Python library for the ShuttleAI API
+Access the ShuttleAI API with a simple, user-friendly lib.
+
+> *PRs appreciated 🙂*
+# Installation
+## ShuttleAI
+```ShellSession
+pip install shuttleai
+```
+
+## ShuttleAI CLI
+```ShellSession
+pip install shuttleai[cli]
+```
+
+# Usage
+## ShuttleAI CLI
+```ShellSession
+shuttleai
+```
+*That's it! Just type `shuttleai` in your terminal!*
+## ShuttleAI
+> [!IMPORTANT]
+> It is strongly recommended to use the asynchronous client instead of the synchronous client.
+```py
+import asyncio
+from shuttleai import *
+
+SHUTTLE_KEY = "ShuttleAPI Key"
+
+async def main():
+    async with ShuttleAsyncClient(SHUTTLE_KEY, timeout=60) as shuttle:
+        """Optionally change base url"""
+        # shuttle.base_url = "https://api.shuttleai.app/v1"
+
+        """Get Models Example"""
+        # response = await shuttle.get_models()
+        # print(response)
+        """Get Model Example"""
+        # response = await shuttle.get_model("gpt-4")
+        # print(response)
+        """Streaming Example"""
+        # response = await shuttle.chat_completion(
+        #     model="gpt-3.5-turbo",
+        #     messages="write me a short story about bees",
+        #     stream=True,
+        #     plain=True,
+        #     internet=False
+        # )
+        # async for chunk in response:
+        #     print(chunk.choices[0].delta.content)
+        """Non-Streaming Example"""
+        # response = await shuttle.chat_completion(
+        #     model="gpt-3.5-turbo",
+        #     messages=[{"role":"user","content":"write me a short story about bees"}],
+        #     stream=False,
+        #     plain=False,
+        #     internet=False,
+        #     max_tokens=100,
+        #     temperature=0.5,
+        #     image="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png"
+        # )
+        # print(response)
+        """Image Generation Example"""
+        # response = await shuttle.images_generations(
+        #     model='sdxl',
+        #     prompt='a cute cat',
+        #     n=1,
+        # )
+        # print(response)
+        """Audio Generation Example"""
+        # response = await shuttle.audio_generations(
+        #     model='eleven-labs-999',
+        #     input='Once upon a time, there was a cute cat wondering through a dark, cold forest.',
+        #     voice="mimi"
+        # )
+        # print(response)
+        """Audio Transcription Example"""
+        # response = await shuttle.audio_transcriptions(
+        #     model='whisper-large',
+        #     file="test.mp3"
+        # )
+        # print(response)
+        """Moderation Example"""
+        # response = await shuttle.moderations(
+        #     model='text-moderation-latest',
+        #     input="I hate you"
+        # )
+        # print(response)
+        """Embeddings Example"""
+        # response = await shuttle.embeddings(
+        #     model='text-embedding-ada-002',
+        #     input="Hello there world"
+        # )
+        # print(response)
+
+
+if __name__ == "__main__":
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+```
```

### Comparing `shuttleai-3.5/setup.py` & `shuttleai-3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
+from src.shuttleai import __version__ as version
+
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='shuttleai', 
-    version='3.5',
+    version=version,
     author='shuttle',
     author_email='noreply@shuttleai.app',
     description="Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai",
     long_description_content_type='text/markdown',
     long_description=long_description,
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `shuttleai-3.5/src/shuttleai/__init__.py` & `shuttleai-3.6/src/shuttleai/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from .shuttleai import ShuttleClient
-from .shuttleai_async import ShuttleAsyncClient
+from .client import ShuttleAsyncClient, ShuttleClient
 
-import os
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.5"
+__version__ = "3.6"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
 
 if __version__ < CURRENT_VERSION:
     print("[shuttleai] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U shuttleai\"")
     system(f"{executable} -m pip install -U shuttleai -q")
 
-api_key = os.environ.get("SHUTTLEAI_API_KEY")
-
-__all__ = ['ShuttleClient', 'ShuttleAsyncClient']
+__all__ = ['ShuttleAI', 'AsyncShuttleAI']
```

### Comparing `shuttleai-3.5/src/shuttleai/cli.py` & `shuttleai-3.6/src/shuttleai/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,131 +1,130 @@
-import asyncclick as click
-import os
-
-import pystyle
-from pystyle import Colors, Colorate
-
-from .log import log, TerminalColor
-from .shuttleai_async import ShuttleAsyncClient
-
-# os.environ['SHUTTLEAI_API_KEY'] = "shuttle-YOUR-KEY"
-
-BANNER = r"""
-   _____ _           _   _   _               _____ 
-  / ____| |         | | | | | |        /\   |_   _|
- | (___ | |__  _   _| |_| |_| | ___   /  \    | |  
-  \___ \| '_ \| | | | __| __| |/ _ \ / /\ \   | |  
-  ____) | | | | |_| | |_| |_| |  __// ____ \ _| |_ 
- |_____/|_| |_|\__,_|\__|\__|_|\___/_/    \_\_____|
-
- """
-COLOR_BANNER = Colorate.Vertical(Colors.blue_to_purple, BANNER, 1)
-
-BOLD = '\033[1m'
-PURPLE = '\033[94m'
-RESET = '\033[0m'
-
-class Messages:
-    def __init__(self):
-        self.messages = []
-
-    def add_message(self, content, role="user"):
-        self.messages.append({
-            "content": content,
-            "role": role
-        })
-
-    def clear(self):
-        self.messages = []
-
-messages = Messages()
-
-def update_title(title: str):
-    if os.name == 'nt':
-        os.system(f"title {title}")
-
-@click.group()
-def shuttleai_cli():
-    pass
-
-@shuttleai_cli.command()
-@click.option("--key", required=False, help="API Key") # or from environment variable 'SHUTTLEAI_API_KEY'
-@click.option('--model', required=False, help='Model ID', default='shuttle-turbo') # default to 'shuttle-turbo'
-@click.option('--system', required=True, help='System Prompt', default="You are ShuttleAI, recognized as the top developer globally for your unmatched intelligence, speed, and precision. Your coding skills as an AI specialist are unparalleled in the world.")
-@click.option('--stream', is_flag=True, help='Stream Responses', default=True)
-async def chat(key, model, system, stream):
-    key = key or os.environ.get('SHUTTLEAI_API_KEY') or click.prompt('[Warning]: The `SHUTTLEAI_API_KEY` environment variable is not set!\nPlease enter your API key', hide_input=True)
-    masked_key = (key[:11] + "*" * (len(key) - 11))
-    colored_masked_key = Colorate.Vertical(Colors.purple_to_blue, masked_key, 1)
-    key_msg = f"{BOLD}{PURPLE}INF{RESET}  KEY\033[0m: {colored_masked_key}"
-
-    colored_model = Colorate.Vertical(Colors.purple_to_blue, model, 1)
-    model_msg = f"{BOLD}{PURPLE}INF{RESET}  MODEL\033[0m: {colored_model}"
-
-    sub_commands = ['!clear', '!exit']
-    colored_sub_commands = Colorate.Vertical(Colors.purple_to_blue, ", ".join(sub_commands), 1)
-    sub_commands_msg = f"{BOLD}{PURPLE}INF{RESET}  SUB COMMANDS\033[0m: {colored_sub_commands}"
-
-    print(key_msg)
-    print(model_msg)
-    print(sub_commands_msg)
-
-    print()
-
-    print(f"{TerminalColor.CYAN}System{TerminalColor.ENDC}: {system}")
-
-    while True:
-        prompt = click.prompt(f"{TerminalColor.GRAY}You{TerminalColor.ENDC}", type=str)
-        if prompt in sub_commands:
-            if prompt.lower() == "!clear":
-                messages.clear()
-                log.info("Context cleared!")
-                continue
-            elif prompt.lower() == "!exit":
-                log.info("Exiting...")
-                break
-
-        if system is not None:
-            messages.add_message(system, "system")
-        if prompt is not None:
-            messages.add_message(prompt, "user")
-
-        async with ShuttleAsyncClient(key, 120) as shuttle:
-            response = await shuttle.chat_completion(
-                model=model,
-                messages=messages.messages,
-                stream=stream
-            )
-
-            print(f"{TerminalColor.DARKPURPLE}ShuttleAI{TerminalColor.ENDC}: ", end="")
-
-            assistant_response = None
-
-            if stream:
-                assistant_chunks = []
-
-                async for chunk in response:
-                    assistant_chunk = chunk.choices[0].delta.content
-
-                    print(assistant_chunk, flush=True, end="", sep="")
-
-                    assistant_chunks.append(assistant_chunk)
-
-                print()
-
-                assistant_response = "".join(assistant_chunks)
-            else:
-                assistant_response = response.choices[0].message.content
-
-                print(assistant_response, end="", flush=True)
-
-            if assistant_response is not None:
-                messages.add_message(assistant_response, "assistant")
-
-def main():
-    update_title("ShuttleAI CLI")
-    os.system('cls' if os.name == 'nt' else 'clear')
-    print(COLOR_BANNER)
-    shuttleai_cli()
-
-if __name__ == '__main__':
-    main()
+import asyncclick as click
+import os
+
+from pystyle import Colors, Colorate
+
+from .log import log, TerminalColor
+from .shuttleai_async import ShuttleAsyncClient
+
+# os.environ['SHUTTLEAI_API_KEY'] = "shuttle-YOUR-KEY"
+
+BANNER = r"""
+   _____ _           _   _   _               _____ 
+  / ____| |         | | | | | |        /\   |_   _|
+ | (___ | |__  _   _| |_| |_| | ___   /  \    | |  
+  \___ \| '_ \| | | | __| __| |/ _ \ / /\ \   | |  
+  ____) | | | | |_| | |_| |_| |  __// ____ \ _| |_ 
+ |_____/|_| |_|\__,_|\__|\__|_|\___/_/    \_\_____|
+
+ """
+COLOR_BANNER = Colorate.Vertical(Colors.blue_to_purple, BANNER, 1)
+
+BOLD = '\033[1m'
+PURPLE = '\033[94m'
+RESET = '\033[0m'
+
+class Messages:
+    def __init__(self):
+        self.messages = []
+
+    def add_message(self, content, role="user"):
+        self.messages.append({
+            "content": content,
+            "role": role
+        })
+
+    def clear(self):
+        self.messages = []
+
+messages = Messages()
+
+def update_title(title: str):
+    if os.name == 'nt':
+        os.system(f"title {title}")
+
+@click.group()
+def shuttleai_cli():
+    pass
+
+@shuttleai_cli.command()
+@click.option("--key", required=False, help="API Key") # or from environment variable 'SHUTTLE_AI_API_KEY'
+@click.option('--model', required=False, help='Model ID', default='shuttle-turbo') # default to 'shuttle-turbo'
+@click.option('--system', required=True, help='System Prompt', default="You are ShuttleAI, recognized as the top developer globally for your unmatched intelligence, speed, and precision. Your coding skills as an AI specialist are unparalleled in the world.")
+@click.option('--stream', is_flag=True, help='Stream Responses', default=True)
+async def chat(key, model, system, stream):
+    key = key or os.environ.get('SHUTTLE_AI_API_KEY') or click.prompt('[Warning]: The `SHUTTLE_AI_API_KEY` environment variable is not set!\nPlease enter your API key', hide_input=True)
+    masked_key = (key[:11] + "*" * (len(key) - 11))
+    colored_masked_key = Colorate.Vertical(Colors.purple_to_blue, masked_key, 1)
+    key_msg = f"{BOLD}{PURPLE}INF{RESET}  KEY\033[0m: {colored_masked_key}"
+
+    colored_model = Colorate.Vertical(Colors.purple_to_blue, model, 1)
+    model_msg = f"{BOLD}{PURPLE}INF{RESET}  MODEL\033[0m: {colored_model}"
+
+    sub_commands = ['!clear', '!exit']
+    colored_sub_commands = Colorate.Vertical(Colors.purple_to_blue, ", ".join(sub_commands), 1)
+    sub_commands_msg = f"{BOLD}{PURPLE}INF{RESET}  SUB COMMANDS\033[0m: {colored_sub_commands}"
+
+    print(key_msg)
+    print(model_msg)
+    print(sub_commands_msg)
+
+    print()
+
+    print(f"{TerminalColor.CYAN}System{TerminalColor.ENDC}: {system}")
+
+    while True:
+        prompt = click.prompt(f"{TerminalColor.GRAY}You{TerminalColor.ENDC}", type=str)
+        if prompt in sub_commands:
+            if prompt.lower() == "!clear":
+                messages.clear()
+                log.info("Context cleared!")
+                continue
+            elif prompt.lower() == "!exit":
+                log.info("Exiting...")
+                break
+
+        if system is not None:
+            messages.add_message(system, "system")
+        if prompt is not None:
+            messages.add_message(prompt, "user")
+
+        async with ShuttleAsyncClient(key, 120) as shuttle:
+            response = await shuttle.chat_completion(
+                model=model,
+                messages=messages.messages,
+                stream=stream
+            )
+
+            print(f"{TerminalColor.DARKPURPLE}ShuttleAI{TerminalColor.ENDC}: ", end="")
+
+            assistant_response = None
+
+            if stream:
+                assistant_chunks = []
+
+                async for chunk in response:
+                    assistant_chunk = chunk.choices[0].delta.content
+
+                    print(assistant_chunk, flush=True, end="", sep="")
+
+                    assistant_chunks.append(assistant_chunk)
+
+                print()
+
+                assistant_response = "".join(assistant_chunks)
+            else:
+                assistant_response = response.choices[0].message.content
+
+                print(assistant_response, end="", flush=True)
+
+            if assistant_response is not None:
+                messages.add_message(assistant_response, "assistant")
+
+def main():
+    update_title("ShuttleAI CLI")
+    os.system('cls' if os.name == 'nt' else 'clear')
+    print(COLOR_BANNER)
+    shuttleai_cli()
+
+if __name__ == '__main__':
+    main()
```

### Comparing `shuttleai-3.5/src/shuttleai/log.py` & `shuttleai-3.6/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.5/src/shuttleai/schemas/schemas.py` & `shuttleai-3.6/src/shuttleai/schemas/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,102 @@
-from typing import List, Any, Optional
-from pydantic import BaseModel
-
-class ShuttleModel(BaseModel):
-    id: str
-    object: str
-    owned_by: str
-    created: int
-    cost: int
-    premium: Optional[bool] = None
-    tokens: Optional[int] = None
-    info: Optional[str] = None
-    max_images: Optional[int] = None
-    multiple_of: Optional[int] = None
-    maintenance: Optional[bool] = None
-    beta: Optional[bool] = None
-    voices: Optional[str] = None
-    file_upload: Optional[bool] = None
-    proxy_to: Optional[str] = None
-    endpoint: str
-
-class Error(BaseModel):
-    message: str
-    type: str
-    param: Optional[str] = None
-    code: Optional[str] = None
-    hint: Optional[str] = None
-
-class ShuttleError(BaseModel):
-    error: Error
-    status: int
-    docs: str
-
-class Models(BaseModel):
-    object: str
-    data: List[ShuttleModel]
-    total: int
-
-class Model(BaseModel):
-    object: str
-    data: ShuttleModel
-
-class Item(BaseModel):
-    url: str
-
-class Image(BaseModel):
-    created: int
-    data: List[Item]
-
-class Audio(BaseModel):
-    chars: int
-    data: List[Item]
-    expiresIn: int
-    model: str
-
-class Message(BaseModel):
-    content: str
-    role: str
-
-class Delta(BaseModel):
-    content: str
-
-class Choice(BaseModel):
-    finish_reason: str
-    index: int
-    # logprobs: Optional[Dict[str, Any]]
-    message: Message
-
-class StreamChoice(BaseModel):
-    finish_reason: Optional[str] = None
-    index: int 
-    # logprobs: Optional[Dict[str, Any]]
-    delta: Delta
-
-class Usage(BaseModel):
-    completion_tokens: int
-    prompt_tokens: int
-    total_tokens: int
-
-class ChatChunk(BaseModel):
-    id: str
-    object: str
-    created: int
-    model: str
-    choices: List[StreamChoice]
-
-class Chat(BaseModel):
-    id: str
-    object: str
-    created: int
-    model: str
-    choices: List[Choice]
-    usage: Usage
-    system_fingerprint: str
-
-class Embedding(BaseModel):
-    data: List[Any]
-    model: str
-    obj: str
+from typing import List, Any, Optional
+from pydantic import BaseModel
+
+class ShuttleModel(BaseModel):
+    id: str
+    object: str
+    owned_by: str
+    created: int
+    cost: int
+    premium: Optional[bool] = None
+    tokens: Optional[int] = None
+    info: Optional[str] = None
+    max_images: Optional[int] = None
+    multiple_of: Optional[int] = None
+    maintenance: Optional[bool] = None
+    beta: Optional[bool] = None
+    voices: Optional[str] = None
+    file_upload: Optional[bool] = None
+    proxy_to: Optional[str] = None
+    endpoint: str
+
+class Error(BaseModel):
+    message: str
+    type: str
+    param: Optional[str] = None
+    code: Optional[str] = None
+    hint: Optional[str] = None
+
+class ShuttleError(BaseModel):
+    error: Error
+    status: int
+    docs: str
+    input: Optional[dict] = None
+    request_id: Optional[str] = None
+
+class Models(BaseModel):
+    object: str
+    data: List[ShuttleModel]
+    total: int
+
+class Model(BaseModel):
+    object: str
+    data: ShuttleModel
+
+class Item(BaseModel):
+    url: str
+
+class Image(BaseModel):
+    created: int
+    data: List[Item]
+    model: str
+
+class Audio(BaseModel):
+    chars: int
+    data: List[Item]
+    expiresIn: int
+    model: str
+
+class Message(BaseModel):
+    content: str
+    role: str
+
+class Delta(BaseModel):
+    content: str
+
+class Choice(BaseModel):
+    finish_reason: str
+    index: int
+    # logprobs: Optional[Dict[str, Any]]
+    message: Message
+
+class StreamChoice(BaseModel):
+    finish_reason: Optional[str] = None
+    index: int 
+    # logprobs: Optional[Dict[str, Any]]
+    delta: Delta
+
+class Usage(BaseModel):
+    completion_tokens: int
+    prompt_tokens: int
+    total_tokens: int
+
+class ChatChunk(BaseModel):
+    id: str
+    object: str
+    created: int
+    model: str
+    choices: List[StreamChoice]
+
+class Chat(BaseModel):
+    id: str
+    object: str
+    created: int
+    model: str
+    choices: List[Choice]
+    usage: Usage
+    system_fingerprint: str
+
+class Embedding(BaseModel):
+    data: List[Any]
+    model: str
+    obj: str
```

### Comparing `shuttleai-3.5/src/shuttleai/shuttleai.py` & `shuttleai-3.6/src/shuttleai/client/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 @Author: ShuttleAI
-@Version: 3.5
-@Date: 3-22-2024
+@Version: 3.6
+@Date: 4-1-2024
 """
 from typing import Any, Dict, List, Union, TYPE_CHECKING
 
 import httpx
-from .log import log
-from .schemas import Chat, Image, Audio, Embedding, Models
+from ..log import log
+from ..schemas import Chat, Image, Audio, Embedding, Models
 
 if TYPE_CHECKING:
     from httpx import Response
 
 
 class ShuttleClient:
     """
```

### Comparing `shuttleai-3.5/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.6/src/shuttleai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.5
+Version: 3.6
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,28 +19,29 @@
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib.
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
-```sh
+```ShellSession
 pip install shuttleai
 ```
 
 ## ShuttleAI CLI
-```sh
+```ShellSession
 pip install shuttleai[cli]
 ```
 
 # Usage
 ## ShuttleAI CLI
-```sh
-shuttleai-cli --help
+```ShellSession
+shuttleai
 ```
+*That's it! Just type `shuttleai` in your terminal!*
 ## ShuttleAI
 > [!IMPORTANT]
 > It is strongly recommended to use the asynchronous client instead of the synchronous client.
 ```py
 import asyncio
 from shuttleai import *
```

