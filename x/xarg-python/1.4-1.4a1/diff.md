# Comparing `tmp/xarg-python-1.4.tar.gz` & `tmp/xarg-python-1.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-1.4.tar", last modified: Mon Apr  1 16:54:31 2024, max compression
+gzip compressed data, was "xarg-python-1.4a1.tar", last modified: Wed Feb 28 06:55:34 2024, max compression
```

## Comparing `xarg-python-1.4.tar` & `xarg-python-1.4a1.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:54:31.816936 xarg-python-1.4/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1267 2024-04-01 16:54:31.816936 xarg-python-1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4/README.md
--rw-r--r--   0 root         (0) root         (0)      523 2024-04-01 16:54:31.816936 xarg-python-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:54:31.806936 xarg-python-1.4/xarg/
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-01 15:33:01.000000 xarg-python-1.4/xarg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22737 2024-04-01 16:48:28.000000 xarg-python-1.4/xarg/actuator.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-01 16:53:51.000000 xarg-python-1.4/xarg/attribute.py
--rw-r--r--   0 root         (0) root         (0)     6327 2024-04-01 15:33:01.000000 xarg-python-1.4/xarg/colorful.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4/xarg/complete.py
--rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4/xarg/parser.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4/xarg/safefile.py
--rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4/xarg/scanner.py
--rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4/xarg/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:54:31.816936 xarg-python-1.4/xarg_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1267 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 06:55:34.084564 xarg-python-1.4a1/
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-12-26 08:19:24.000000 xarg-python-1.4a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-02-28 06:55:34.084564 xarg-python-1.4a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-12-26 08:19:24.000000 xarg-python-1.4a1/README.md
+-rw-r--r--   0 root         (0) root         (0)      527 2024-02-28 06:55:34.084564 xarg-python-1.4a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      773 2024-01-15 02:43:52.000000 xarg-python-1.4a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 06:55:34.084564 xarg-python-1.4a1/xarg/
+-rw-r--r--   0 root         (0) root         (0)      379 2024-02-28 06:36:02.000000 xarg-python-1.4a1/xarg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22410 2024-01-15 02:43:52.000000 xarg-python-1.4a1/xarg/actuator.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-02-28 06:53:07.000000 xarg-python-1.4a1/xarg/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8039 2024-01-15 02:43:52.000000 xarg-python-1.4a1/xarg/complete.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2024-01-15 02:43:52.000000 xarg-python-1.4a1/xarg/parser.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2023-12-28 08:08:34.000000 xarg-python-1.4a1/xarg/scanner.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-02-28 06:29:01.000000 xarg-python-1.4a1/xarg/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 06:55:34.084564 xarg-python-1.4a1/xarg_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-02-28 06:55:33.000000 xarg-python-1.4a1/xarg_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2024-02-28 06:55:34.000000 xarg-python-1.4a1/xarg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 06:55:33.000000 xarg-python-1.4a1/xarg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-02-28 06:55:33.000000 xarg-python-1.4a1/xarg_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-02-28 06:55:33.000000 xarg-python-1.4a1/xarg_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-02-28 06:55:33.000000 xarg-python-1.4a1/xarg_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 06:55:33.000000 xarg-python-1.4a1/xarg_python.egg-info/zip-safe
```

### Comparing `xarg-python-1.4/LICENSE` & `xarg-python-1.4a1/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Mingzhe Zou <zoumingzhe@outlook.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Mingzhe Zou <zoumingzhe@outlook.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `xarg-python-1.4/PKG-INFO` & `xarg-python-1.4a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4
+Version: 1.4a1
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
 Project-URL: Documentation, https://github.com/bondbox/xarg-python/
 Keywords: command,command-line,argparse,xarg
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argcomplete>=3.2.1
+Requires-Dist: tabulate
 
 xarg
 ====
 
 Simple command-line tool based on `argparse`.
 
 Language
@@ -49,9 +52,7 @@
 
 or build via shell:
 
 ```shell
 rm -rf "build" "dist" "*.egg-info"
 python setup.py check sdist bdist_wheel --universal
 ```
-
-
```

### Comparing `xarg-python-1.4/README.md` & `xarg-python-1.4a1/README.md`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/setup.cfg` & `xarg-python-1.4a1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 
 [options]
 zip_safe = True
 include_package_data = True
+python_requires = >=3.8
 install_requires = 
 	argcomplete >= 3.2.1
-	colorama
-	colorlog
 	tabulate
 
 [options.entry_points]
 console_scripts = 
 	xargcomplete = xarg.complete:main
 
 [egg_info]
```

### Comparing `xarg-python-1.4/setup.py` & `xarg-python-1.4a1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 from xarg.util import __author__
 from xarg.util import __author_email__
 from xarg.util import __description__
-from xarg.util import __project__
+from xarg.util import __name__
 from xarg.util import __url_bugs__
 from xarg.util import __url_code__
 from xarg.util import __url_docs__
 from xarg.util import __url_home__
 from xarg.util import __version__
 
 setup(
-    name=__project__,
+    name=__name__,
     version=__version__,
     description=__description__,
     url=__url_home__,
     author=__author__,
     author_email=__author_email__,
     project_urls={"Source Code": __url_code__,
                   "Bug Tracker": __url_bugs__,
```

### Comparing `xarg-python-1.4/xarg/actuator.py` & `xarg-python-1.4a1/xarg/actuator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,32 +9,21 @@
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
-from colorlog import ColoredFormatter
-
 from .parser import argp
 from .util import singleton
 
 
-DEFAULT_LOG_FORMAT = "%(log_color)s%(message)s"
-DEFAULT_LOG_COLORS = {
-    "DEBUG": "black",
-    "INFO": "white",
-    "WARNING": "yellow",
-    "ERROR": "red",
-    "CRITICAL": "light_red",
-}
-
-
 class add_command:
-    '''Define a new command-line node.
+    '''
+    Define a new command-line node.
 
     For example:
 
     >>> from xarg import add_command\n
     >>> from xarg import argp\n
 
     >>> @add_command("example")\n
@@ -134,15 +123,16 @@
             node = node.prev
             subs.insert(0, node.name)
         name = "_".join(subs)
         return f"__sub_dest_{name}__"
 
 
 class run_command:
-    '''Define the main callback function, and bind it to a node and subcommands.
+    '''
+    Define the main callback function, and bind it to a node and subcommands.
 
     For example:
 
     >>> from xarg import commands\n
     >>> from xarg import run_command\n
 
     >>> @run_command(cmd, cmd_get, cmd_set)\n
@@ -208,15 +198,16 @@
 
     @property
     def skip(self) -> bool:
         return self.__skip
 
 
 class pre_command:
-    '''Define prepare callback function, and bind it with main callback.
+    '''
+    Define prepare callback function, and bind it with main callback.
 
     For example:
 
     >>> from xarg import commands\n
     >>> from xarg import pre_command\n
     >>> from xarg import run_command\n
 
@@ -248,15 +239,16 @@
 
     @property
     def main(self) -> run_command:
         return self.__main
 
 
 class end_command:
-    '''Define purge callback function, and bind it with main callback.
+    '''
+    Define purge callback function, and bind it with main callback.
 
     For example:
 
     >>> from xarg import commands\n
     >>> from xarg import end_command\n
     >>> from xarg import run_command\n
 
@@ -289,15 +281,16 @@
     @property
     def main(self) -> run_command:
         return self.__main
 
 
 @singleton
 class commands:
-    '''Singleton command-line tool based on argparse.
+    '''
+    Singleton command-line tool based on argparse.
 
     Define and bind all callback functions before calling run() or parse().
 
     For example:
 
     >>> from typing import Optional\n
     >>> from typing import Sequence\n
@@ -347,38 +340,41 @@
 
     @property
     def prog(self) -> str:
         return self.__prog
 
     @property
     def root(self) -> Optional[add_command]:
-        '''Root Command.
+        '''
+        Root Command.
         '''
         return self.__root
 
     @root.setter
     def root(self, value: add_command):
         assert isinstance(value, add_command)
         self.__root = value
 
     @property
     def args(self) -> Namespace:
-        '''Namespace after parse arguments.
+        '''
+        Namespace after parse arguments.
         '''
         assert isinstance(self.__args, Namespace)
         return self.__args
 
     @args.setter
     def args(self, value: Namespace):
         assert isinstance(value, Namespace)
         self.__args = value
 
     @property
     def version(self) -> Optional[str]:
-        '''Custom version for "-v" or "--version" output.
+        '''
+        Custom version for "-v" or "--version" output.
         '''
         return self.__version
 
     @version.setter
     def version(self, value: str):
         assert isinstance(value, str)
         _version = value.strip()
@@ -391,26 +387,29 @@
     @enable_logger.setter
     def enable_logger(self, value: bool):
         assert isinstance(value, bool)
         self.__enable_logger = value
 
     @property
     def logger(self) -> logging.Logger:
-        '''Logger.
+        '''
+        Logger.
         '''
         return logging.getLogger(self.prog)
 
     def stdout(self, context: Any):
-        '''Output string to sys.stdout.
+        '''
+        Output string to sys.stdout.
         '''
         sys.stdout.write(f"{context}\n")
         sys.stdout.flush()
 
     def stderr(self, context: Any):
-        '''Output string to sys.stderr.
+        '''
+        Output string to sys.stderr.
         '''
         sys.stderr.write(f"{context}\n")
         sys.stderr.flush()
 
     def __add_optional_version(self, argp: argp):
         version = self.version
         if not isinstance(version, str):
@@ -484,25 +483,24 @@
                                help="Logger output to file.")
 
         def add_optional_format():
             option = filter_optional_name("--format", "--log-format")
             if not isinstance(option, str):
                 return
 
-            DEFAULT_LOG_FMT = "%(log_color)s%(asctime)s"\
-                " %(process)d %(threadName)s %(levelname)s"\
-                " %(funcName)s %(filename)s:%(lineno)s"\
+            DEFAULT_FMT = "%(asctime)s %(process)d %(threadName)s"\
+                " %(levelname)s %(funcName)s %(filename)s:%(lineno)s"\
                 " %(message)s"
 
             group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group.add_argument(option,
                                type=str,
                                nargs="?",
-                               const=DEFAULT_LOG_FMT,
-                               default=DEFAULT_LOG_FORMAT,
+                               const=DEFAULT_FMT,
+                               default=None,
                                metavar="STRING",
                                dest="_log_format_",
                                help="Logger output format.")
 
         def add_optional_console():
             group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group_std = group.add_mutually_exclusive_group()
@@ -535,21 +533,20 @@
 
         # save debug level to local variable
         if hasattr(args, "_log_level_str_") and\
            isinstance(args._log_level_str_, str):
             level_name = args._log_level_str_.upper()
             self.logger.setLevel(logging._nameToLevel[level_name])
 
+        formatter = logging.Formatter(
+            fmt=args._log_format_ if hasattr(args, "_log_format_")
+            and isinstance(args._log_format_, str) else None,
+            datefmt=None)
+
         def addHandler(handler: logging.Handler):
-            formatter: logging.Formatter = ColoredFormatter(
-                fmt=args._log_format_ if hasattr(args, "_log_format_")
-                and isinstance(args._log_format_, str) else None,
-                datefmt=None,
-                log_colors=DEFAULT_LOG_COLORS,
-                no_color=isinstance(handler, logging.FileHandler))
             handler.setFormatter(formatter)
             self.logger.addHandler(handler)
 
         if hasattr(args, "_log_console_") and args._log_console_ is not None:
             addHandler(logging.StreamHandler(stream=args._log_console_))
 
         if hasattr(args, "_log_files_"):
@@ -580,15 +577,16 @@
     def __add_option(self, _map: Dict[add_command, argp]):
         for _cmd, _arg in _map.items():
             _cmd.func(_arg)
             self.__add_inner_parser_tail(_arg)
 
     def parse(self, root: Optional[add_command] = None,
               argv: Optional[Sequence[str]] = None, **kwargs) -> Namespace:
-        '''Parse the command line.
+        '''
+        Parse the command line.
         '''
         if root is None:
             root = self.root
         assert isinstance(root, add_command)
 
         _map: Dict[add_command, argp] = dict()
         _arg = argp(argv=argv, **kwargs)
@@ -603,15 +601,16 @@
         assert isinstance(args, Namespace)
         self.__parse_logger(args)
         self.args = args
         return self.args
 
     def has_sub(self, root: add_command,
                 args: Optional[Namespace] = None) -> bool:
-        '''If the root command node has any subcommand nodes, return true.
+        '''
+        If the root command node has any subcommand nodes, return true.
 
         @param root: Command node
         @type root: add_command
 
         @param args: Command arguments
         @type args: Namespace or None (default self.args if None is specified)
 
@@ -675,15 +674,16 @@
                         return self.__pre(args, sub)
         return 0
 
     def run(self,
             root: Optional[add_command] = None,
             argv: Optional[Sequence[str]] = None,
             **kwargs) -> int:
-        '''Parse and run the command line.
+        '''
+        Parse and run the command line.
         '''
         if root is None:
             root = self.root
 
         if not isinstance(root, add_command):
             self.logger.debug("cannot find root")
             return ENOENT
```

### Comparing `xarg-python-1.4/xarg/complete.py` & `xarg-python-1.4a1/xarg/complete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # coding:utf-8
 
 from base64 import b16decode
 from base64 import b16encode
 from configparser import ConfigParser
-from errno import EPERM
 import os
 import shutil
-import sys
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Set
 from typing import Tuple
@@ -20,16 +18,16 @@
 from pip._internal.commands.show import search_packages_info
 from tabulate import tabulate
 
 from .actuator import add_command
 from .actuator import commands
 from .actuator import run_command
 from .parser import argp
+from .util import __name__
 from .util import __prog_complete__
-from .util import __project__
 from .util import __url_home__
 from .util import __version__
 from .util import singleton
 
 USER_BASH_COMPLETION_CFG = "~/.bash_completion"
 USER_BASH_COMPLETION_DIR = "~/.bash_completion.d"
 
@@ -87,15 +85,15 @@
 
 
 @singleton
 class collections:
 
     def __init__(self):
         self.__cmds: Set[str] = set()
-        for _pkg in {"argcomplete", __project__}:
+        for _pkg in {"argcomplete", __name__}:
             for _req in {i for i in self.get_package_info(_pkg).required_by}:
                 config = ConfigParser()
                 package_info = self.get_package_info(_req)
                 config.read_string(os.linesep.join(package_info.entry_points))
                 if config.has_section("console_scripts"):
                     for _cmd in config["console_scripts"]:
                         self.__cmds.add(_cmd)
@@ -222,17 +220,14 @@
 def add_cmd(_arg: argp):
     pass
 
 
 @run_command(add_cmd, add_cmd_enable, add_cmd_update, add_cmd_remove,
              add_cmd_list)
 def run_cmd(cmds: commands) -> int:
-    if sys.version_info < (3, 8):
-        cmds.logger.error("Require Python>=3.8")
-        return EPERM
     return 0
 
 
 def main(argv: Optional[Sequence[str]] = None) -> int:
     cmds = commands()
     cmds.version = __version__
     return cmds.run(
```

### Comparing `xarg-python-1.4/xarg/parser.py` & `xarg-python-1.4a1/xarg/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,41 +8,40 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Set
 from typing import Tuple
 
-from .util import __url_home__ as __url__
+from argcomplete import autocomplete
 
-try:
-    from argcomplete import autocomplete
-except ModuleNotFoundError:
-    pass
+from .util import __url_home__ as __url__
 
 
 class checker():
 
     prefix_chars = "-"
 
     @classmethod
     def check_name_pos(cls, fn):
-        '''check positional argument name
+        '''
+        check positional argument name
         '''
 
         def inner(self, name: str, **kwargs):
             assert isinstance(name, str) and name[0] not in cls.prefix_chars, \
                 f"{name} is not a positional argument name"
             return fn(self, name, **kwargs)
 
         return inner
 
     @classmethod
     def check_name_opt(cls, fn):
-        '''check optional argument name
+        '''
+        check optional argument name
         '''
 
         def inner(self, *name: str, **kwargs):
             # 1. check short form optional argument ("-x")
             # 2. check long form optional argument ("--xx")
             # 3. only short form or long form or short form + long form
             # 模棱两可的数据（-1可以是一个负数的位置参数）
@@ -51,15 +50,16 @@
                     f"{n} is not an optional argument name"
             return fn(self, *name, **kwargs)
 
         return inner
 
     @classmethod
     def check_nargs_opt(cls, fn):
-        '''nargs hook function:
+        '''
+        nargs hook function:
             nargs < -1: using "?", 0 or 1 argument, default value
             nargs = -1: using "+", arguments list, at least 1
             nargs = 0: using "*", arguments list, allow to be empty
             nargs = 1: redirect to "?", 0 or 1 argument
             nargs > 1: N arguments list
         '''
 
@@ -70,15 +70,16 @@
             kwargs.update({"nargs": _nargs})
             return fn(self, *args, **kwargs)
 
         return inner
 
 
 class argp(ArgumentParser):
-    '''Simple command-line tool based on argparse.
+    '''
+    Simple command-line tool based on argparse.
     '''
 
     def __init__(self,
                  argv: Optional[Sequence[str]] = None,
                  prog: Optional[str] = None,
                  usage: Optional[str] = None,
                  prev_parser: Optional["argp"] = None,
@@ -108,80 +109,84 @@
             root = root.__prev_parser
         return root
 
     def argument_group(self,
                        title: Optional[str] = None,
                        description: Optional[str] = None,
                        **kwargs) -> _ArgumentGroup:
-        '''Find the created argument group by title, create if not exist.
+        '''
+        Find the created argument group by title, create if not exist.
         '''
         for group in self._action_groups:
             if title == group.title:
                 return group
         return self.add_argument_group(title, description, **kwargs)
 
     @checker.check_name_opt
     def filter_optional_name(self, *name: str) -> Sequence[str]:
-        '''Filter defined optional argument name.
+        '''
+        Filter defined optional argument name.
         '''
         option_strings: Set[str] = set()
         for action in self._get_optional_actions():
             option_strings.update(action.option_strings)
         return [n for n in name if n not in option_strings]
 
     @checker.check_name_pos
     def add_pos(self, name: str, **kwargs) -> None:
-        '''Add positional argument.
+        '''
+        Add positional argument.
         '''
         assert "dest" not in kwargs, \
             "dest supplied twice for positional argument"
         self.add_argument(name, **kwargs)
 
     @checker.check_name_opt
     @checker.check_nargs_opt
     def add_opt(self, *name: str, **kwargs) -> None:
-        '''Add optional argument.
+        '''
+        Add optional argument.
         '''
         self.add_argument(*name, **kwargs)
 
     @checker.check_name_opt
     def add_opt_on(self, *name: str, **kwargs) -> None:
-        '''Add boolean optional argument, default value is False.
+        '''
+        Add boolean optional argument, default value is False.
         '''
         kwargs.update({"action": "store_true"})
         for key in ("type", "nargs", "const", "default", "choices"):
             assert key not in kwargs, f"'{key}' is an invalid argument"
         self.add_argument(*name, **kwargs)
 
     @checker.check_name_opt
     def add_opt_off(self, *name: str, **kwargs) -> None:
-        '''Add boolean optional argument, default value is True.
+        '''
+        Add boolean optional argument, default value is True.
         '''
         kwargs.update({"action": "store_false"})
         for key in ("type", "nargs", "const", "default", "choices"):
             assert key not in kwargs, f"'{key}' is an invalid argument"
         self.add_argument(*name, **kwargs)
 
     def add_subparsers(self, *args, **kwargs) -> _SubParsersAction:
-        '''Add subparsers.
+        '''
+        Add subparsers.
         '''
         # subparser: cannot have multiple subparser arguments
         kwargs.setdefault("title", "subcommands")
         kwargs.setdefault("description", None)
         kwargs.setdefault("dest", f"subcmd_{self.prog}")
         kwargs.setdefault("help", None)
         kwargs.setdefault("metavar", None)
         return ArgumentParser.add_subparsers(self, *args, **kwargs)
 
     def parse_args(self, args: Optional[Sequence[str]] = None,
                    namespace: Optional[Namespace] = None) -> Namespace:
-        try:
-            autocomplete(self)  # For tab completion
-        except NameError:
-            pass
+        autocomplete(self)  # For tab completion
         return super().parse_args(args=args, namespace=namespace)
 
     def parse_known_args(self, args: Optional[Sequence[str]] = None,
                          namespace: Optional[Namespace] = None
                          ) -> Tuple[Namespace, List[str]]:
         return super().parse_known_args(args=args, namespace=namespace)
 
@@ -196,15 +201,16 @@
         for option, action in self._option_string_actions.items():
             if isinstance(action, _HelpAction):
                 self.__help_option[option] = action
         for option in self.__help_option:
             self._option_string_actions.pop(option)
 
     def preparse_from_sys_argv(self) -> Namespace:
-        '''Preparse some arguments from sys.argv for tab completion.
+        '''
+        Preparse some arguments from sys.argv for tab completion.
 
         When arguments contain the help option, call parse_known_args()
         will print help message and exit. The command line can parse
         normally.
 
         But parameters added after calling preparse_from_sys_argv() will
         not show in the help message, because the exit occurred before
```

### Comparing `xarg-python-1.4/xarg/safefile.py` & `xarg-python-1.4a1/xarg/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 # coding=utf-8
 
+
 import os
 import shutil
+from typing import List
 
+from .attribute import __author__
+from .attribute import __author_email__
+from .attribute import __description__
+from .attribute import __name__
+from .attribute import __prog_complete__
+from .attribute import __prog_name__
+from .attribute import __url_bugs__
+from .attribute import __url_code__
+from .attribute import __url_docs__
+from .attribute import __url_home__
+from .attribute import __version__
+
+
+def singleton(cls):
+    instance = {}
+
+    def _singleton_wrapper(*args, **kwargs):
+        if cls not in instance:
+            instance[cls] = cls(*args, **kwargs)
+        return instance[cls]
+
+    return _singleton_wrapper
+
+
+@singleton
+class chdir:
+    '''Change directory
+    '''
 
-class safile:
-    '''Secure read and write files
+    def __init__(self):
+        self.__stack: List[str] = []
 
-    Backup before writing and restore (if backup exists) before reading.
-    '''
+    def pushd(self, path: str):
+        '''Add directory to stack.
+        '''
+        assert isinstance(path, str), f"type '{type(path)}' is not str"
+        assert os.path.isdir(path), f"path '{path}' is not directory"
+        self.__stack.append(os.getcwd())
+        os.chdir(path)
 
-    @classmethod
-    def get_backup_path(cls, origin: str) -> str:
-        '''Unified backup path
+    def popd(self):
+        '''Remove directory from stack.
         '''
-        return f"{origin}.bak"
+        assert len(self.__stack) > 0
+        os.chdir(self.__stack.pop())
 
-    @classmethod
-    def create_backup(cls, path: str, copy: bool = False) -> bool:
-        '''Create a backup before writing file
 
-        Backup files with '.bak' suffix will be created in the same directory.
-        By default shutil.move() is used to create the backup file, which will
-        use os.rename() to rename the original file. This will make the backup
-        very efficient.
-        But, if you wish to append to the original file, you need to specify
-        'copy=True' to use shutil.copy2().
-        '''
-        pbak: str = cls.get_backup_path(path)
-        if os.path.isfile(pbak):  # Restore before creating a new backup
-            assert cls.restore(path), f"restore '{path}' failed"
-        assert not os.path.exists(pbak), f"backup file '{pbak}' already exists"
-        if not os.path.exists(path):  # No need for backup
+class safile:
+    '''Secure read and write files
+    '''
+
+    @classmethod
+    def backup(cls, path: str) -> bool:
+        pbak: str = f"{path}.bak"
+        assert not os.path.exists(pbak), f"backup '{pbak}' already exists"
+        if not os.path.exists(path):
             return True
         assert os.path.isfile(path), f"'{path}' is not a regular file"
-        method = shutil.copy2 if copy else shutil.move
-        assert method(src=path, dst=pbak) == pbak, f"backup '{path}' failed"
+        assert shutil.move(src=path, dst=pbak) == pbak
         return os.path.exists(pbak)
 
     @classmethod
-    def delete_backup(cls, path: str) -> bool:
-        '''Delete backup after writing file
-        '''
-        pbak: str = cls.get_backup_path(path)
-        if os.path.isfile(pbak):
-            os.remove(pbak)
-        return not os.path.exists(pbak)
-
-    @classmethod
     def restore(cls, path: str) -> bool:
-        '''Restore (if backup exists) before reading file
-        '''
-        pbak: str = cls.get_backup_path(path)
+        pbak: str = f"{path}.bak"
         if os.path.isfile(pbak):
             if os.path.isfile(path):
                 os.remove(path)
-            assert not os.path.exists(path), f"file '{path}' still exists"
-            assert shutil.move(src=pbak, dst=path) == path, \
-                f"restore backup file '{pbak}' to '{path}' failed"
+            assert not os.path.exists(path), f"restore {path} still exists"
+            assert shutil.move(src=pbak, dst=path) == path
         return not os.path.exists(pbak)
```

### Comparing `xarg-python-1.4/xarg/scanner.py` & `xarg-python-1.4a1/xarg/scanner.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/xarg_python.egg-info/PKG-INFO` & `xarg-python-1.4a1/xarg_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4
+Version: 1.4a1
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
 Project-URL: Documentation, https://github.com/bondbox/xarg-python/
 Keywords: command,command-line,argparse,xarg
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argcomplete>=3.2.1
+Requires-Dist: tabulate
 
 xarg
 ====
 
 Simple command-line tool based on `argparse`.
 
 Language
@@ -49,9 +52,7 @@
 
 or build via shell:
 
 ```shell
 rm -rf "build" "dist" "*.egg-info"
 python setup.py check sdist bdist_wheel --universal
 ```
-
-
```

