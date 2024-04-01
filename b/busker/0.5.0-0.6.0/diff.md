# Comparing `tmp/busker-0.5.0.tar.gz` & `tmp/busker-0.6.0.tar.gz`

## Comparing `busker-0.5.0.tar` & `busker-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 busker-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 busker-0.5.0/busker/__init__.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 busker-0.5.0/busker/executive.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 busker-0.5.0/busker/gui.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 busker-0.5.0/busker/history.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 busker-0.5.0/busker/main.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 busker-0.5.0/busker/runner.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 busker-0.5.0/busker/scraper.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 busker-0.5.0/busker/types.py
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 busker-0.5.0/busker/visitor.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 busker-0.5.0/busker/zone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 busker-0.5.0/busker/test/__init__.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 busker-0.5.0/busker/test/test_executive.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 busker-0.5.0/busker/test/test_history.py
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 busker-0.5.0/busker/test/test_scraper.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 busker-0.5.0/busker/test/test_zone.py
--rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 busker-0.5.0/LICENSE
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 busker-0.5.0/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 busker-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    41451 2020-02-02 00:00:00.000000 busker-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 busker-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    49152 2020-02-02 00:00:00.000000 busker-0.6.0/busker/.gui.py.swp
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 busker-0.6.0/busker/__init__.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 busker-0.6.0/busker/executive.py
+-rw-r--r--   0        0        0    19607 2020-02-02 00:00:00.000000 busker-0.6.0/busker/gui.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 busker-0.6.0/busker/history.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 busker-0.6.0/busker/main.py
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 busker-0.6.0/busker/runner.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 busker-0.6.0/busker/scraper.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 busker-0.6.0/busker/tagger.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 busker-0.6.0/busker/types.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 busker-0.6.0/busker/visitor.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 busker-0.6.0/busker/zone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/__init__.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_executive.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_history.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_runner.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_scraper.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_zone.py
+-rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 busker-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 busker-0.6.0/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 busker-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    42031 2020-02-02 00:00:00.000000 busker-0.6.0/PKG-INFO
```

### Comparing `busker-0.5.0/busker/history.py` & `busker-0.6.0/busker/history.py`

 * *Files identical despite different names*

### Comparing `busker-0.5.0/busker/main.py` & `busker-0.6.0/busker/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     except FileNotFoundError:
         config = {}
     except tomllib.TOMLDecodeError as e:
         history.log(f"Error reading config file at {args.config}", level=logging.WARNING)
         history.log(f"{e!s}", level=logging.ERROR)
         return 2
 
-    root = busker.gui.build(config)
+    exclude = [] if args.with_automation else ["automation"]
+    root = busker.gui.build(config, exclude=exclude)
     root.mainloop()
     return 0
 
     witness = Counter()
 
     n = 0
     while n < args.number:
@@ -76,33 +77,39 @@
 
     print(*visitor.toml_lines(visitor.history), sep="\n")
     print({k: witness[k] for k in sorted(witness.keys())})
     return 0
 
 
 def parser(defaults):
-    rv = argparse.ArgumentParser()
+    rv = argparse.ArgumentParser(fromfile_prefix_chars="@")
 
-    setting_options = rv.add_argument_group("Settings")
-    hosting_options = rv.add_argument_group("Hosting")
-    playing_options = rv.add_argument_group("Playing")
-    plugins_options = rv.add_argument_group("Plugins")
+    display_options = rv.add_argument_group("Display")
+    packaging_options = rv.add_argument_group("Packaging")
+    automation_options = rv.add_argument_group("Automation")
+
+    display_options.add_argument(
+        "--with-automation",
+        action="store_true",
+        default=False,
+        help="Show Automation tab in GUI [False]."
+    )
 
-    setting_options.add_argument(
+    automation_options.add_argument(
         "--config",
         type=pathlib.Path,
         default=defaults.config,
         help=f"Set a path to a configuration file [{defaults.config}].",
     )
 
-    plugins_options.add_argument(
+    automation_options.add_argument(
         "--url", default="http://localhost:8080",
         help="Set url path to begin session."
     )
-    plugins_options.add_argument(
+    automation_options.add_argument(
         "--number", type=int, default="64",
         help="Set the number of times to run the plugin."
     )
     return rv
 
 
 def run():
```

### Comparing `busker-0.5.0/busker/runner.py` & `busker-0.6.0/busker/test/test_history.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,67 +13,60 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from collections import defaultdict
 from collections import deque
-import concurrent.futures
+import datetime
 import logging
-import pathlib
-import sys
-import time
+import textwrap
 import tomllib
-import venv
+import unittest
 
+from busker.history import SharedHistory
+from busker.history import SharedLogRecord
 
-from busker.types import ExecutionEnvironment
 
+class TOMLTests(unittest.TestCase):
 
-class Runner:
-
-    @staticmethod
-    def walk_files(path: pathlib.Path, callback=None):
-        callback = callback or pathlib.Path
-        if path.is_dir():
-            try:
-                for p in path.iterdir():
-                    yield from Runner.walk_files(pathlib.Path(p))
-            except Exception:
-                pass
-        yield callback(path)
-
-    @property
-    def jobs(self) -> list:
-        return []
-
-
-class VirtualEnv(Runner):
-
-    def __init__(self, location: pathlib.Path):
-        self.location = location
-
-    def build_virtualenv(self, exenv: ExecutionEnvironment, **kwargs):
-        venv.create(
-            self.location,
-            system_site_packages=True,
-            clear=True,
-            with_pip=True,
-            upgrade_deps=True
+    def test_log_records(self):
+        data = dict(
+            args=("a", "b", "c"),
+            funcName="test_log_records",
+            levelname="INFO",
+            levelno=20,
+            msg="Learn your '{0}{1}{2}'s!",
+            name="TOMLTestLogger",
+            pathname="busker/test/test_history.py",
+            processName="MainProcess",
+        )
+        records = dict(
+            head=[
+                logging.makeLogRecord(dict(data, asctime=datetime.datetime.now().isoformat(), lineno=n * 10))
+                for n in range(12)
+            ],
+            tail=deque([
+                logging.makeLogRecord(dict(data, asctime=datetime.datetime.now().isoformat(), lineno=n * 10))
+                for n in range(12)
+            ])
         )
 
-    def check_virtualenv(self, exenv: ExecutionEnvironment, repeat=100, interval=2, **kwargs):
-        values = []
-        while len(values) < repeat:
-            files = list(self.walk_files(self.location))
-            values.append(len(files))
-            exenv.queue.put(values[-1])
-            if len(values) > 3 and values[-3] == values[-1] and values[-1] <= max(values):
-                break
-            else:
-                time.sleep(interval)
-
-    @property
-    def jobs(self) -> list:
-        return [self.build_virtualenv, self.check_virtualenv]
+        obj = SharedHistory()
+        self.assertIsInstance(obj.history["head"], list)
+        self.assertIsInstance(obj.history["tail"], deque)
+
+        lines = list(obj.toml_lines(records))
+
+        text = "\n".join(lines)
+        data = tomllib.loads("\n".join(lines))
+        self.assertTrue(data)
+
+        for log in ("head", "tail"):
+            with self.subTest(log=log):
+                output = data.get("log", {}).get(log, [])
+                self.assertTrue(output, data)
+
+                record = logging.makeLogRecord(output[0])
+                self.assertIsInstance(record, SharedLogRecord)
+                self.assertEqual(record.getMessage(), "Learn your 'abc's!", vars(record))
```

### Comparing `busker-0.5.0/busker/scraper.py` & `busker-0.6.0/busker/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,22 +82,27 @@
 
 
 class Scraper(SharedHistory):
 
     @staticmethod
     @functools.cache
     def tag_matcher(tag: str):
-        return re.compile(f"<{tag}>(.*?)<\\/{tag}>", re.DOTALL)
+        return re.compile(f"<{tag}.*?>(.*?)<\\/{tag}>", re.DOTALL)
 
     @staticmethod
     def find_forms(body: str):
         root = ET.fromstring(body)
         return root.findall(".//form")
 
     @staticmethod
+    def find_blocks(body: str):
+        matcher = Scraper.tag_matcher("blockquote")
+        return [i.strip() for i in matcher.findall(body, re.DOTALL)]
+
+    @staticmethod
     def find_title(doc: str):
         matcher = Scraper.tag_matcher("title")
         match = matcher.search(doc)
         return match and match[1]
 
     def get_forms(self, body: str):
         root = ET.fromstring(body)
```

### Comparing `busker-0.5.0/busker/types.py` & `busker-0.6.0/busker/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+from collections import namedtuple
 import dataclasses
 import enum
 import multiprocessing
 import multiprocessing.managers
 import multiprocessing.pool
 import pathlib
 
 
+Completion = namedtuple("Completion", ["runner", "exenv", "data"], defaults=[None])
+
+
 class Host(enum.Enum):
 
     IPV4_LOOPBACK = "127.0.0.1"
     IPV4_NET_HOST = "0.0.0.0"
     IPV6_LOOPBACK = "::1"
     IPV6_NET_HOST = "::"
```

### Comparing `busker-0.5.0/busker/visitor.py` & `busker-0.6.0/busker/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,21 @@
         node = scraper.get(url, **kwargs)
 
         body_re = scraper.tag_matcher("body")
         body_match = body_re.search(node.text)
 
         title_match = scraper.find_title(node.text)
         forms = body_match and tuple(scraper.get_forms(body_match[0])) or []
+        blocks = body_match and tuple(scraper.find_blocks(body_match[0])) or []
 
         return node._replace(
             tactic=self.__class__.__name__,
             params=tuple(kwargs.items()),
             title=title_match and title_match.group(),
-
+            blocks=blocks,
             options=tuple(v for f in forms for i in f.inputs for v in i.values),
             actions=forms,
         )
         return node
 
 
 class Write(Tactic):
@@ -92,20 +93,21 @@
 
             rv = scraper.post(self.url, data)
 
             body_re = scraper.tag_matcher("body")
             body_match = body_re.search(rv.text)
 
             forms = body_match and tuple(scraper.get_forms(body_match[0]))
+            blocks = body_match and tuple(scraper.find_blocks(body_match[0])) or []
 
             rv = rv._replace(
                 tactic=self.__class__.__name__,
                 params=tuple(kwargs.items()),
                 title = scraper.find_title(rv.text),
-
+                blocks=blocks,
                 options=tuple(v for f in forms for i in f.inputs for v in i.values),
                 actions=forms,
             )
             return rv
 
 
 class Visitor(SharedHistory):
```

### Comparing `busker-0.5.0/busker/zone.py` & `busker-0.6.0/busker/zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 class Zone(SharedHistory):
 
     registry = defaultdict(list)
 
     def __init__(self, parent, name="", **kwargs):
         super().__init__(log_name=f"busker.gui.{name.lower()}", **kwargs)
         self.registry[self.__class__.__name__].append(self)
+        if name and name not in self.registry:
+            self.registry[name] = self
 
         self.parent = parent
         self.name = name
         self.frame = ttk.LabelFrame(parent, text=name)
 
         container = defaultdict(list)
         for attr, obj in self.build(self.frame):
```

### Comparing `busker-0.5.0/busker/test/test_executive.py` & `busker-0.6.0/busker/test/test_executive.py`

 * *Files identical despite different names*

### Comparing `busker-0.5.0/busker/test/test_scraper.py` & `busker-0.6.0/busker/test/test_scraper.py`

 * *Files identical despite different names*

### Comparing `busker-0.5.0/busker/test/test_zone.py` & `busker-0.6.0/busker/test/test_zone.py`

 * *Files identical despite different names*

### Comparing `busker-0.5.0/LICENSE` & `busker-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `busker-0.5.0/pyproject.toml` & `busker-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # For possible options see https://peps.python.org/pep-0621/
  
 [project]
 name = "busker"
-version = "0.5.0"
+version = "0.6.0"
 description = "A utility for testing Balladeer projects."
 readme = "README.md"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 keywords = ["interactive fiction", "balladeer"]
 authors = [
     {name = "D E Haynes", email = "tundish@gigeconomy.org.uk"}
```

### Comparing `busker-0.5.0/PKG-INFO` & `busker-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: busker
-Version: 0.5.0
+Version: 0.6.0
 Summary: A utility for testing Balladeer projects.
 Author-email: D E Haynes <tundish@gigeconomy.org.uk>
 Maintainer-email: Tundish <tundish@gigeconomy.org.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -685,26 +685,40 @@
 Requires-Python: >=3.11
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 Busker
 ======
 
+Busker is a utility for testing [Balladeer](https://tundish.github.io/balladeer) projects.
+
+It provides a graphical interface for interaction with a Balladeer host.
+
+Busker also allows you to self-host the Balladeer application, simplifying the steps required:
++ Creating a Python virtual environment.
++ Installing the Balladeer package along with its dependencies.
++ Running the Balladeer server.
+
 Operation
 ---------
 
-Python 3.11 or later is required.
+* Busker works on Windows and UNIX systems.
+* Python 3.11 or later is required.
+* No installation is necessary. Simply run from the command line.
 
-This is a work-in-progress.
+```
+python3 -m busker.main --help
 
-    usage: main.py [-h] [--config CONFIG] [--url URL] [--number NUMBER]
+usage: busker.main [-h] [--with-automation] [--config CONFIG] [--url URL] [--number NUMBER]
 
-    options:
-      -h, --help       show this help message and exit
+options:
+  -h, --help         show this help message and exit
 
-    Settings:
-      --config CONFIG  Set a path to a configuration file [/home/user/busker.toml].
+Display:
+  --with-automation  Show Automation tab in GUI [False].
 
-    Plugins:
-      --url URL        Set url path to begin session.
-      --number NUMBER  Set the number of times to run the plugin.
+Automation:
+  --config CONFIG    Set a path to a configuration file [/home/user/busker.toml].
+  --url URL          Set url path to begin session.
+  --number NUMBER    Set the number of times to run the plugin.
 
+```
```

