# Comparing `tmp/microagi_git-0.0.5.tar.gz` & `tmp/microagi_git-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microagi_git-0.0.5.tar", max compression
+gzip compressed data, was "microagi_git-0.0.6.tar", max compression
```

## Comparing `microagi_git-0.0.5.tar` & `microagi_git-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35151 2023-09-27 11:43:27.459244 microagi_git-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1658 2023-09-20 18:19:22.523524 microagi_git-0.0.5/README.pypi.md
--rw-r--r--   0        0        0     4448 2023-09-29 21:33:39.394427 microagi_git-0.0.5/agit/config.py
--rw-r--r--   0        0        0     4049 2023-09-29 22:25:45.489289 microagi_git-0.0.5/agit/grammar.py
--rw-r--r--   0        0        0     1453 2023-09-27 11:41:11.010030 microagi_git-0.0.5/agit/logger.py
--rwxr-xr-x   0        0        0     5304 2023-09-30 17:39:49.371642 microagi_git-0.0.5/agit/main.py
--rw-r--r--   0        0        0     4168 2023-09-27 11:41:34.863306 microagi_git-0.0.5/agit/openai_api.py
--rw-r--r--   0        0        0     2843 2023-09-30 18:16:33.164083 microagi_git-0.0.5/agit/os_iface.py
--rw-r--r--   0        0        0     2095 2023-09-29 22:24:50.891030 microagi_git-0.0.5/agit/security.py
--rw-r--r--   0        0        0     2061 2023-09-27 12:35:42.667289 microagi_git-0.0.5/agit/selfdocument.py
--rw-r--r--   0        0        0     3520 2023-09-29 15:56:34.676174 microagi_git-0.0.5/agit/util.py
--rw-r--r--   0        0        0      818 2023-09-30 17:41:38.140375 microagi_git-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 microagi_git-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35151 2023-11-07 22:18:30.310516 microagi_git-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1658 2023-09-20 18:19:22.523524 microagi_git-0.0.6/README.pypi.md
+-rw-r--r--   0        0        0     4427 2023-11-07 22:18:30.312756 microagi_git-0.0.6/agit/config.py
+-rw-r--r--   0        0        0     4049 2023-11-07 22:18:30.313562 microagi_git-0.0.6/agit/grammar.py
+-rw-r--r--   0        0        0     1453 2023-11-07 22:18:30.314445 microagi_git-0.0.6/agit/logger.py
+-rwxr-xr-x   0        0        0     5423 2024-04-01 15:29:39.776006 microagi_git-0.0.6/agit/main.py
+-rw-r--r--   0        0        0     5559 2024-04-01 11:27:40.854198 microagi_git-0.0.6/agit/openai_api.py
+-rw-r--r--   0        0        0     4251 2023-11-07 22:18:30.317802 microagi_git-0.0.6/agit/os_iface.py
+-rw-r--r--   0        0        0     2205 2024-03-31 18:26:02.430074 microagi_git-0.0.6/agit/rag.py
+-rw-r--r--   0        0        0     2095 2023-11-07 22:18:30.319118 microagi_git-0.0.6/agit/security.py
+-rw-r--r--   0        0        0     2061 2023-11-07 22:18:30.320281 microagi_git-0.0.6/agit/selfdocument.py
+-rw-r--r--   0        0        0     3520 2023-11-07 22:18:30.321525 microagi_git-0.0.6/agit/util.py
+-rw-r--r--   0        0        0      859 2024-04-01 15:31:14.809710 microagi_git-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 microagi_git-0.0.6/PKG-INFO
```

### Comparing `microagi_git-0.0.5/LICENSE.txt` & `microagi_git-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `microagi_git-0.0.5/README.pypi.md` & `microagi_git-0.0.6/README.pypi.md`

 * *Files identical despite different names*

### Comparing `microagi_git-0.0.5/agit/config.py` & `microagi_git-0.0.6/agit/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU General Public License for more details.
 
 
 DESTRUCTIVE_COMMANDS = {
-    "git push --force": "Force pushes can overwrite remote branches, potentially discarding commits.",
-    "git push -f": "Shortened version of 'git push --force'.",
-    "git branch -D": "Force deletes a branch, regardless of its merged status.",
-    "git branch -d": "Deletes a branch. Not generally destructive, but included for completeness.",
-    "git checkout -B": "Creates a new branch or resets an existing branch to a start point. Could overwrite work on existing branches.",
-    "git checkout -b": "Creates a new branch. Not generally destructive, but included for completeness.",
-    "git clean -fd": "Force deletes untracked files and directories in the working copy, potentially erasing work.",
-    "git clean -f": "Force deletes untracked files in the working copy, potentially erasing work.",
+    "push --force": "Force pushes can overwrite remote branches, potentially discarding commits.",
+    "push -f": "Shortened version of 'git push --force'.",
+    "branch -D": "Force deletes a branch, regardless of its merged status.",
+    "branch -d": "Deletes a branch. Not generally destructive, but included for completeness.",
+    "checkout -B": "Creates a new branch or resets an existing branch to a start point. Could overwrite work on existing branches.",
+    "checkout -b": "Creates a new branch. Not generally destructive, but included for completeness.",
+    "clean -fd": "Force deletes untracked files and directories in the working copy, potentially erasing work.",
+    "clean -f": "Force deletes untracked files in the working copy, potentially erasing work.",
     "reset --hard": "Resets the index and working tree to match a specified commit. Any changes to tracked files in the working tree since the specified commit are lost.",
     "reset --soft": "Moves the HEAD to a specified commit. Changes since the specified commit are kept. Can be destructive if not handled properly.",
     "reset --mixed": "Resets the index but not the working tree and reports what has not been updated.",
     "rebase": "Applies your changes on top of another base tip, which can create conflicts.",
     "rm --cached": "Unstages and removes paths only from the index (not the working tree) and can cause loss of work.",
     "rm": "Removes files from the working tree and from the index.",
     "stash clear": "Removes all stashed entries, potentially erasing saved work.",
@@ -85,8 +85,8 @@
     "status",
     "submodule",
     "tag",
     "worktree",
 ]
 
 
-ALLOWED_GIT_COMMANDS = ["git"] + porcelain_commands
+ALLOWED_GIT_COMMANDS = ["git"] + porcelain_commands + ["sort"]
```

### Comparing `microagi_git-0.0.5/agit/grammar.py` & `microagi_git-0.0.6/agit/grammar.py`

 * *Files identical despite different names*

### Comparing `microagi_git-0.0.5/agit/logger.py` & `microagi_git-0.0.6/agit/logger.py`

 * *Files identical despite different names*

### Comparing `microagi_git-0.0.5/agit/main.py` & `microagi_git-0.0.6/agit/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from logging import DEBUG
 import openai
 import argparse
 from argparse import RawTextHelpFormatter
 import autopage
 
 from agit.openai_api import translate_to_git_command, review_patch
+from agit.rag import retrieve_git_data
 from agit.selfdocument import explain
 from agit.security import is_destructive
 from agit.util import (
     print_explanation,
     print_command,
     print_description,
     gather_output,
@@ -41,17 +42,17 @@
 # Setup logging
 from agit.logger import mylogger
 
 
 async def main():
     parser = argparse.ArgumentParser(
         prog="agit",
-        description="AGit is an assistant agent that translates natural language to Git commands.",
+        description="AGit is an secure assistant agent that translates natural language to Git commands.",
         epilog=""
-        "#microAGI, AGit  Copyright (C) 2023  Sivan Grünberg, Vitakka Consulting\n"
+        "#microAGI, AGit  Copyright (C) 2023-2024  Sivan Grünberg, Vitakka Consulting\n"
         "This program comes with *ABSOLUTELY NO WARRANTY*; This is free software, and \n"
         "you are welcome to redistribute it under certain conditions;\n"
         "see LICENSE.txt for details. \n",
         formatter_class=RawTextHelpFormatter,
     )
 
     parser.add_argument(
@@ -83,15 +84,15 @@
 
     args = parser.parse_args()
 
     if args.debug:
         mylogger.setLevel(DEBUG)
 
     if args.version:
-        print("AGit Version v0.0.5")
+        print("AGit Version v0.0.6")
         return
 
     if args.review:
         cmd = "git diff"
         mylogger.debug("Starting review...")
         diff_output = gather_output(cmd=cmd)
         content = await review_patch(
@@ -115,15 +116,18 @@
         print("OpenAI API key was not set, please set it before using AGit.")
         return
 
     natural_language = " ".join(args.command)
     if args.debug:
         mylogger.debug(f"natural language query: {natural_language}")
 
-    git_command = await translate_to_git_command(natural_language, args.explain)
+    context = retrieve_git_data(".")
+    git_command = await translate_to_git_command(
+        natural_language, args.explain, context=context
+    )
 
     if args.debug:
         mylogger.debug(f"Model Response: {git_command}")
 
     with autopage.AutoPager(
         allow_color=True, pager_command=autopage.command.PlatformPager()
     ) as out_stream:
```

### Comparing `microagi_git-0.0.5/agit/os_iface.py` & `microagi_git-0.0.6/agit/os_iface.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,14 +20,27 @@
 
 import subprocess
 from agit.config import ALLOWED_GIT_COMMANDS
 from pyparsing import quotedString
 from agit.util import is_interactive_command
 
 
+def split_piped_command_string(command_string):
+    commands = command_string.split()
+    commands = [cmd.strip() for cmd in commands]
+
+    if "|" in commands:
+        index = commands.index("|")
+        before_pipe = " ".join(commands[:index])
+        after_pipe = " ".join(commands[index + 1 :])
+        return (before_pipe, after_pipe)
+    else:
+        return (None, None)
+
+
 def normalize(command_string: str):
     quoted = quotedString.searchString(command_string)
     quotes = None
     normalized_command_list = None
     if quoted:
         quoted_part = quoted[0][0]
         quotes = quoted_part.split()[0][0]
@@ -47,32 +60,64 @@
         if part.endswith("=") or part.endswith(":"):
             eq_parts.append(part)
 
     normalized_command_list = result_list
     return normalized_command_list
 
 
+def handle_pipe(command_string: str):
+    (cmd1, cmd2) = split_piped_command_string(command_string)
+    if cmd1 and cmd2:
+        cmd1 = normalize(command_string=cmd1)
+        cmd2 = normalize(command_string=cmd2)
+        return (cmd1, cmd2)
+    else:
+        return [normalize(command_string=command_string)]
+
+
+def authorize(cmd_list):
+    if (cmd_list[0] or cmd_list[1]) not in ALLOWED_GIT_COMMANDS:
+        return False
+    return True
+
+
 def execute_git_command(command_string: str):
     if not command_string:
         return "Command list is empty."
 
     interactive = is_interactive_command(command_string)
-    normalized_command_list = normalize(command_string=command_string)
+    normalized_command_list = handle_pipe(command_string)
 
     # Check if the git command is in the list of allowed commands
-    if (
-        normalized_command_list[0] or normalized_command_list[1]
-    ) not in ALLOWED_GIT_COMMANDS:
-        return f"Command '{normalized_command_list[0]}' is not allowed."
+    for cmd_list in normalized_command_list:
+        if not authorize(cmd_list):
+            return f"Command '{cmd_list[0]}' is not allowed."
 
     # Execute the command
-    try:
-        result = subprocess.run(
-            ["git", "-c", "color.ui=always", "-c", "log.decorate=true"]
-            + normalized_command_list[1:],
-            capture_output=not interactive,
-            text=True,
-            check=True,
-        )
-        return result.stdout or ""
-    except subprocess.CalledProcessError as e:
-        return e.stderr
+    piped = len(normalized_command_list) > 1
+    cmd1_output = None
+    result = None
+    for idx, cmd_list in enumerate(normalized_command_list):
+        if idx == 1:
+            try:
+                result = subprocess.run(
+                    cmd_list,
+                    capture_output=not interactive,
+                    text=True,
+                    check=True,
+                    input=cmd1_output,
+                )
+            except subprocess.CalledProcessError as e:
+                return e.stderr
+        else:
+            try:
+                result = subprocess.run(
+                    ["git", "-c", "color.ui=always", "-c", "log.decorate=true"]
+                    + cmd_list[1:],
+                    capture_output=not interactive,
+                    text=True,
+                    check=True,
+                )
+            except subprocess.CalledProcessError as e:
+                return e.stderr
+            cmd1_output = piped and result.stdout
+    return result.stdout or ""
```

### Comparing `microagi_git-0.0.5/agit/security.py` & `microagi_git-0.0.6/agit/security.py`

 * *Files identical despite different names*

### Comparing `microagi_git-0.0.5/agit/selfdocument.py` & `microagi_git-0.0.6/agit/selfdocument.py`

 * *Files identical despite different names*

### Comparing `microagi_git-0.0.5/agit/util.py` & `microagi_git-0.0.6/agit/util.py`

 * *Files identical despite different names*

### Comparing `microagi_git-0.0.5/pyproject.toml` & `microagi_git-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microagi-git"
-version = "0.0.5"
+version = "0.0.6"
 description = "Git For Humans: Predictable, secure and precision tuned command-line assistant that translates natural language into Git commands."
 authors = ["Sivan Grünberg <sivan@vitakka.co>"]
 readme = "README.pypi.md"
 packages = [
     { include = "agit" },
 ]
 
@@ -17,14 +17,16 @@
 openai = "^0.27.8"
 requests = "^2.31.0"
 pydantic = "^2.0.3"
 python-dotenv = "^1.0.0"
 colorama = "^0.4.6"
 autopage = "^0.5.1"
 pyparsing = "^3.1.1"
+aiohttp = "^3.9.1"
+gitpython = "^3.1.40"
 
 [tool.poetry.scripts]
 agit = "agit.main:async_main"
 
 
 
 [build-system]
```

### Comparing `microagi_git-0.0.5/PKG-INFO` & `microagi_git-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: microagi-git
-Version: 0.0.5
+Version: 0.0.6
 Summary: Git For Humans: Predictable, secure and precision tuned command-line assistant that translates natural language into Git commands.
 Home-page: https://github.com/microagi/agit
 Keywords: agi,microagi,git,assistant,agent,AI,GPT
 Author: Sivan Grünberg
 Author-email: sivan@vitakka.co
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: autopage (>=0.5.1,<0.6.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: gitpython (>=3.1.40,<4.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: pyparsing (>=3.1.1,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
```

