# Comparing `tmp/pytest_watcher-0.4.1.tar.gz` & `tmp/pytest_watcher-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_watcher-0.4.1.tar", max compression
+gzip compressed data, was "pytest_watcher-0.4.2.tar", max compression
```

## Comparing `pytest_watcher-0.4.1.tar` & `pytest_watcher-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2024-02-06 14:28:12.778794 pytest_watcher-0.4.1/LICENSE
--rw-r--r--   0        0        0     4702 2024-02-06 14:28:12.778794 pytest_watcher-0.4.1/README.md
--rw-r--r--   0        0        0     1800 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       76 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/__init__.py
--rw-r--r--   0        0        0       81 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/__main__.py
--rw-r--r--   0        0        0     4167 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/commands.py
--rw-r--r--   0        0        0     2412 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/config.py
--rw-r--r--   0        0        0       56 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/constants.py
--rw-r--r--   0        0        0     1615 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/event_handler.py
--rw-r--r--   0        0        0     1826 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/parse.py
--rw-r--r--   0        0        0     2090 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/terminal.py
--rw-r--r--   0        0        0      508 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/trigger.py
--rw-r--r--   0        0        0     1965 2024-02-06 14:28:12.782794 pytest_watcher-0.4.1/pytest_watcher/watcher.py
--rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 pytest_watcher-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-01 17:44:52.593827 pytest_watcher-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4702 2024-04-01 17:44:52.593827 pytest_watcher-0.4.2/README.md
+-rw-r--r--   0        0        0     1800 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/__main__.py
+-rw-r--r--   0        0        0     4191 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/commands.py
+-rw-r--r--   0        0        0     2412 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/config.py
+-rw-r--r--   0        0        0       56 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/constants.py
+-rw-r--r--   0        0        0     1615 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/event_handler.py
+-rw-r--r--   0        0        0     1854 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/parse.py
+-rw-r--r--   0        0        0     2090 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/terminal.py
+-rw-r--r--   0        0        0      629 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/trigger.py
+-rw-r--r--   0        0        0     1962 2024-04-01 17:44:52.597827 pytest_watcher-0.4.2/pytest_watcher/watcher.py
+-rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 pytest_watcher-0.4.2/PKG-INFO
```

### Comparing `pytest_watcher-0.4.1/LICENSE` & `pytest_watcher-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.4.1/README.md` & `pytest_watcher-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.4.1/pyproject.toml` & `pytest_watcher-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-watcher"
-version = "0.4.1"
+version = "0.4.2"
 description = "Automatically rerun your tests on file modifications"
 authors = ["Olzhas Arystanov <o.arystanov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/olzhasar/pytest-watcher"
 repository = "https://github.com/olzhasar/pytest-watcher"
 documentation = "https://pytest-watcher.readthedocs.io/en/latest/"
```

### Comparing `pytest_watcher-0.4.1/pytest_watcher/commands.py` & `pytest_watcher-0.4.2/pytest_watcher/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,72 +71,72 @@
 
 class InvokeCommand(Command):
     character = "\n"
     caption = "Enter"
     description = "Invoke test runner"
 
     def run(self, trigger: Trigger, term: Terminal, config: Config) -> None:
-        trigger.emit()
+        trigger.emit_now()
 
 
 class ResetRunnerArgsCommand(Command):
     character = "r"
     caption = "r"
     description = "reset all runner args"
 
     def run(self, trigger: Trigger, term: Terminal, config: Config) -> None:
         config.runner_args.clear()
-        trigger.emit()
+        trigger.emit_now()
 
 
 class ChangeRunnerArgsCommand(Command):
     character = "c"
     caption = "c"
     description = "change runner args"
 
     def run(self, trigger: Trigger, term: Terminal, config: Config) -> None:
         term.reset()
         raw = input("\nEnter new runner args: ")
         new_args = raw.strip().split()
         config.runner_args.clear()
         config.runner_args.extend(new_args)
-        trigger.emit()
+        trigger.emit_now()
 
 
 class OnlyFailedCommand(Command):
     character = "f"
     caption = "f"
     description = "run only failed tests (--lf)"
 
     def run(self, trigger: Trigger, term: Terminal, config: Config) -> None:
         if "--lf" not in config.runner_args:
             config.runner_args.append("--lf")
-        trigger.emit()
+        trigger.emit_now()
 
 
 class PDBCommand(Command):
     character = "p"
     caption = "p"
     description = "drop to pdb on fail (--pdb)"
 
     def run(self, trigger: Trigger, term: Terminal, config: Config) -> None:
         if "--pdb" not in config.runner_args:
             config.runner_args.append("--pdb")
-        trigger.emit()
+        trigger.emit_now()
 
 
 class VerboseCommand(Command):
     character = "v"
     caption = "v"
     description = "increase verbosity (-v)"
 
     def run(self, trigger: Trigger, term: Terminal, config: Config) -> None:
         if "-v" not in config.runner_args:
             config.runner_args.append("-v")
-        trigger.emit()
+        trigger.emit_now()
 
 
 class EraseScreenCommand(Command):
     character = "e"
     caption = "e"
     description = "Erase terminal screen"
```

### Comparing `pytest_watcher-0.4.1/pytest_watcher/config.py` & `pytest_watcher-0.4.2/pytest_watcher/config.py`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.4.1/pytest_watcher/event_handler.py` & `pytest_watcher-0.4.2/pytest_watcher/event_handler.py`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.4.1/pytest_watcher/parse.py` & `pytest_watcher-0.4.2/pytest_watcher/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     parser = argparse.ArgumentParser(
         prog="pytest_watcher",
         description="""
             Watch the <path> for file changes and trigger the test runner (pytest).\n
             Additional arguments are passed directly to the test runner.
         """,
+        allow_abbrev=False,
     )
     parser.add_argument("path", type=Path, help="The path to watch for file changes.")
     parser.add_argument(
         "--now", action="store_true", help="Trigger the test run immediately"
     )
     parser.add_argument(
         "--clear",
```

### Comparing `pytest_watcher-0.4.1/pytest_watcher/terminal.py` & `pytest_watcher-0.4.2/pytest_watcher/terminal.py`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.4.1/pytest_watcher/watcher.py` & `pytest_watcher-0.4.2/pytest_watcher/watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from .parse import parse_arguments
 from .terminal import Terminal, get_terminal
 from .trigger import Trigger
 
 logging.basicConfig(level=logging.INFO, format="[ptw] %(message)s")
 
 
-def main_loop(trigger, config: Config, term: Terminal) -> None:
-    if trigger.check(config.delay):
+def main_loop(trigger: Trigger, config: Config, term: Terminal) -> None:
+    if trigger.check():
         term.reset()
 
         if config.clear:
             term.clear()
 
         try:
             subprocess.run([config.runner, *config.runner_args])
```

### Comparing `pytest_watcher-0.4.1/PKG-INFO` & `pytest_watcher-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-watcher
-Version: 0.4.1
+Version: 0.4.2
 Summary: Automatically rerun your tests on file modifications
 Home-page: https://github.com/olzhasar/pytest-watcher
 License: MIT
 Keywords: pytest,watch,watcher
 Author: Olzhas Arystanov
 Author-email: o.arystanov@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
```

