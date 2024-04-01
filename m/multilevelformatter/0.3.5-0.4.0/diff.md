# Comparing `tmp/multilevelformatter-0.3.5.tar.gz` & `tmp/multilevelformatter-0.4.0.tar.gz`

## Comparing `multilevelformatter-0.3.5.tar` & `multilevelformatter-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/codecov.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/demos/multilevelformatter_demo.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/src/multilevelformatter/__init__.py
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/src/multilevelformatter/multilevelformatter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/src/multilevelformatter/py.typed
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/tests/test_multilevelformatter.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/LICENSE
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/README.md
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 multilevelformatter-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/codecov.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/demos/multilevelformatter_demo.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/src/multilevelformatter/__init__.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/src/multilevelformatter/multilevelformatter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/src/multilevelformatter/py.typed
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/tests/test_multilevelformatter.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/README.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 multilevelformatter-0.4.0/PKG-INFO
```

### Comparing `multilevelformatter-0.3.5/.github/workflows/dependency-review.yml` & `multilevelformatter-0.4.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `multilevelformatter-0.3.5/.github/workflows/python-package.yml` & `multilevelformatter-0.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `multilevelformatter-0.3.5/.github/workflows/python-publish.yml` & `multilevelformatter-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multilevelformatter-0.3.5/demos/multilevelformatter_demo.py` & `multilevelformatter-0.4.0/demos/multilevelformatter_demo.py`

 * *Files identical despite different names*

### Comparing `multilevelformatter-0.3.5/src/multilevelformatter/multilevelformatter.py` & `multilevelformatter-0.4.0/src/multilevelformatter/multilevelformatter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import logging
 import sys
 from typing import Literal, Optional, Dict, ClassVar, List
 from pathlib import Path
 
+from deprecated import deprecated  # type: ignore
+
+# from icecream import ic  # type: ignore
+
+MESSAGE: int = logging.WARNING - 5  # 25
+
 
 def addLoggingLevel(
     levelName: str, levelNum: int, methodName: str | None = None
 ) -> None:
     """
     Copyright 2022 Joseph R. Fox-Rabinovitz aka Mad Physicist @StackOverflow.com
     Credits Mad Physicist
@@ -58,15 +64,19 @@
 
     logging.addLevelName(levelNum, levelName)
     setattr(logging, levelName, levelNum)
     setattr(logging.getLoggerClass(), methodName, logForLevel)
     setattr(logging, methodName, logToRoot)
 
 
-addLoggingLevel("MESSAGE", logging.WARNING - 5)
+def addLoggingLevelMessage() -> None:
+    """
+    Add  logging level logging.MESSAGE to the root logger with value 25
+    """
+    addLoggingLevel("MESSAGE", logging.WARNING - 5)
 
 
 class MultilevelFormatter(logging.Formatter):
     """
     logging.Formatter that simplifies setting different log formats for different log levels
 
     Add to the module file:
@@ -80,15 +90,14 @@
 
     """
 
     _levels: ClassVar[List[int]] = [
         logging.NOTSET,
         logging.DEBUG,
         logging.INFO,
-        logging.MESSAGE,  # type: ignore
         logging.WARNING,
         logging.ERROR,
         logging.CRITICAL,
     ]
 
     def __init__(
         self,
@@ -96,92 +105,136 @@
         fmt: Optional[str] = None,
         datefmt: Optional[str] = None,
         style: Literal["%", "{", "$"] = "%",
         validate: bool = True,
         *,
         defaults=None,
     ):
-        assert fmts is not None, "styles cannot be None"
-
-        # self._formatters: Dict[int, logging.Formatter] = dict()
+        assert fmts is not None, "'fmts' cannot be None"
+        assert style in ["%", "{", "$"], "'style' must be '%', '{' or '$'"
+        assert isinstance(validate, bool), "'validate' must be bool"
         self._formatters: Dict[int, logging.Formatter] = dict()
-        for level in self._levels:
-            self._formatters[level] = logging.Formatter(
-                fmt=fmt,
+        for level in set(self._levels) | set(fmts.keys()):
+            _fmt: str | None = fmt
+            if level in fmts.keys():
+                _fmt = fmts[level]
+            self.setFormat(
+                level,
+                fmt=_fmt,
                 datefmt=datefmt,
                 style=style,
                 validate=validate,
                 defaults=defaults,
             )
 
-        for level in fmts.keys():
-            self._formatters[level] = logging.Formatter(fmt=fmts[level], style=style)
-
     @classmethod
+    @deprecated(version="0.5", reason="Renamed, please use setFormats() instead")
     def setLevels(
         cls,
         logger: logging.Logger,
-        fmts: Optional[Dict[int, str]] = None,
+        fmts: Dict[int, str],
+        fmt: Optional[str] = None,
+        datefmt: Optional[str] = None,
+        style: Literal["%", "{", "$"] = "%",
+        validate: bool = True,
+        log_file: Optional[str | Path] = None,
+    ) -> None:
+        """
+        DEPRECIATED: Use setFormats()
+
+        Will be removed
+
+        Setup logging format for multiple levels
+        """
+        cls.setFormats(
+            logger=logger,
+            fmts=fmts,
+            fmt=fmt,
+            datefmt=datefmt,
+            style=style,
+            validate=validate,
+            log_file=log_file,
+        )
+
+    @classmethod
+    def setFormats(
+        cls,
+        logger: logging.Logger,
+        fmts: Dict[int, str],
         fmt: Optional[str] = None,
         datefmt: Optional[str] = None,
         style: Literal["%", "{", "$"] = "%",
         validate: bool = True,
         log_file: Optional[str | Path] = None,
     ) -> None:
-        """Setup logging"""
-        if fmts is not None:
+        """
+        Setup logging format for multiple levels
+        """
+        try:
             multi_formatter = MultilevelFormatter(
-                fmt=fmt, fmts=fmts, datefmt=datefmt, style=style, validate=validate
+                fmts=fmts, fmt=fmt, datefmt=datefmt, style=style, validate=validate
             )
             # log all but errors to STDIN
             stream_handler = logging.StreamHandler(sys.stdout)
             stream_handler.addFilter(lambda record: record.levelno < logging.ERROR)
             stream_handler.setFormatter(multi_formatter)
             logger.addHandler(stream_handler)
-
             # log errors and above to STDERR
             error_handler = logging.StreamHandler(sys.stderr)
             error_handler.setLevel(logging.ERROR)
             error_handler.addFilter(lambda record: record.levelno >= logging.ERROR)
             error_handler.setFormatter(multi_formatter)
             logger.addHandler(error_handler)
-
-        if log_file is not None:
-            file_handler = logging.FileHandler(log_file)
-            log_formatter = logging.Formatter(fmt=fmt, style=style, validate=validate)
-            file_handler.setFormatter(log_formatter)
-            logger.addHandler(file_handler)
+            if log_file is not None:
+                file_handler = logging.FileHandler(log_file)
+                log_formatter = logging.Formatter(
+                    fmt=fmt, style=style, validate=validate
+                )
+                file_handler.setFormatter(log_formatter)
+                logger.addHandler(file_handler)
+        except Exception as err:
+            logging.error(f"Could not set formats: {err}")
 
     @classmethod
     def setDefaults(
         cls,
         logger: logging.Logger,
         log_file: Optional[str | Path] = None,
-        level: int = logging.MESSAGE,  # type: ignore
+        level: int = logging.WARNING,
     ) -> None:
         """Set multi-level formatting defaults
 
         INFO: %(message)s
-        WARN: %(levelname)s: %(message)s
+        WARNING: %(message)s                 ## Used as message() / default
         ERROR: %(levelname)s: %(funcName)s(): %(message)s
         CRITICAL: %(levelname)s: %(funcName)s(): %(message)s
         """
         logger_conf: Dict[int, str] = {
             logging.INFO: "%(message)s",
-            logging.MESSAGE: "%(message)s",  # type: ignore
-            logging.WARNING: "%(levelname)s: %(message)s",
-            # logging.ERROR: 		'%(levelname)s: %(message)s'
+            logging.WARNING: "%(message)s",
+            # logging.ERROR: '%(levelname)s: %(message)s'
         }
+        if level == MESSAGE:
+            logger_conf[MESSAGE] = "%(message)s"
+            logger_conf[logging.WARNING] = "WARN: %(message)s"
+            addLoggingLevelMessage()
 
-        MultilevelFormatter.setLevels(
+        MultilevelFormatter.setFormats(
             logger,
             fmts=logger_conf,
             fmt="%(levelname)s: %(funcName)s(): %(message)s",
             log_file=log_file,
         )
+        logger.setLevel(level=level)
+
+    def setFormat(self, level: int, fmt: str | None = None, **kwargs):
+        """
+        Set log format for a single level
+        """
+        self._formatters[level] = logging.Formatter(fmt=fmt, **kwargs)
 
     def format(self, record: logging.LogRecord) -> str:
         try:
             return self._formatters[record.levelno].format(record)
         except Exception as err:
             logging.error(f"{err}")
             return f"{err}"
@@ -190,7 +243,14 @@
         try:
             return self._formatters[record.levelno].formatTime(
                 record=record, datefmt=datefmt
             )
         except Exception as err:
             logging.error(f"{err}")
             return f"{err}"
+
+
+# def warning(msg: str):
+#     """
+#     Helper to log a warning message.
+#     """
+#     return eval(f"message('WARN: {msg}')")
```

### Comparing `multilevelformatter-0.3.5/tests/test_multilevelformatter.py` & `multilevelformatter-0.4.0/tests/test_multilevelformatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from pathlib import Path
 import logging
 from typer import Typer, Option  # type: ignore
 from click.testing import Result
 from typer.testing import CliRunner  # type: ignore
 from typing import Annotated, Optional
 
-from multilevelformatter import MultilevelFormatter
+from multilevelformatter import MultilevelFormatter, addLoggingLevelMessage, MESSAGE
 
+# from icecream import ic  # type: ignore
 
 logger = logging.getLogger(__name__)
 error = logger.error
-warning = logger.warning
-message = logger.message  # type: ignore
+message = logger.warning
 verbose = logger.info
 debug = logger.debug
 
 app = Typer()
 
 
 @app.callback(invoke_without_command=True)
@@ -26,22 +26,14 @@
         Option(
             "--verbose",
             "-v",
             show_default=False,
             help="verbose logging",
         ),
     ] = False,
-    print_warning: Annotated[
-        bool,
-        Option(
-            "--warning",
-            show_default=False,
-            help="warnings only",
-        ),
-    ] = False,
     print_debug: Annotated[
         bool,
         Option(
             "--debug",
             show_default=False,
             help="debug logging",
         ),
@@ -54,43 +46,43 @@
             help="silent logging",
         ),
     ] = False,
     log: Annotated[Optional[Path], Option(help="log to FILE", metavar="FILE")] = None,
 ) -> None:
     """MultilevelFormatter demo"""
     global logger
+    # try:
+    #     addLoggingLevelMessage()
 
+    # except AttributeError:
+    #     pass
     try:
-        LOG_LEVEL: int = logging.MESSAGE  # type: ignore
+        LOG_LEVEL: int = logging.WARNING
         if print_verbose:
             LOG_LEVEL = logging.INFO
-        elif print_warning:
-            LOG_LEVEL = logging.WARNING
         elif print_debug:
             LOG_LEVEL = logging.DEBUG
         elif print_silent:
             LOG_LEVEL = logging.ERROR
-        MultilevelFormatter.setDefaults(logger, log_file=log)
-        logger.setLevel(LOG_LEVEL)
+        MultilevelFormatter.setDefaults(logger, log_file=log, level=LOG_LEVEL)
     except Exception as err:
         error(f"{err}")
+
     verbose("verbose")
     message("standard")
-    warning("warning")
     error("error")
     debug("debug")
 
 
 @pytest.mark.parametrize(
     "args,lines",
     [
-        ([], 3),
-        (["--verbose"], 4),
-        (["--debug"], 5),
-        (["--warning"], 2),
+        ([], 2),
+        (["--verbose"], 3),
+        (["--debug"], 4),
         (["--silent"], 1),
     ],
 )
 def test_1_multilevelformatter(args: list[str], lines: int) -> None:
     result: Result = CliRunner().invoke(app, [*args])
 
     assert result.exit_code == 0, f"test failed {' '.join(args)}"
@@ -105,13 +97,24 @@
         if param != "silent":
             assert (
                 result.output.find(param) >= 0
             ), f"no expected output found: '{param}'"
     else:
         assert (
             result.output.find("standard") >= 0
-        ), "no expected output found: 'standard'"
+        ), f"no expected output found: 'standard': {result.output}"
     assert result.output.find("error") >= 0, "no expected output found: 'error'"
 
 
+def test_2_addLoggingLevelMessage() -> None:
+    addLoggingLevelMessage()
+    try:
+        logging.message("test message()")  # type: ignore
+        assert True, "logging.message() worked as it should"
+    except Exception as err:
+        assert False, f"could not add logging.message(): {err}"
+
+    assert logging.MESSAGE == MESSAGE, "Added logging.MESSAGE level == 25"  # type: ignore
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `multilevelformatter-0.3.5/.gitignore` & `multilevelformatter-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `multilevelformatter-0.3.5/LICENSE` & `multilevelformatter-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multilevelformatter-0.3.5/README.md` & `multilevelformatter-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 # MultiLevelFormatter
 
 `MultiLevelFormatter` is a Python `logging.Formatter` that simplifies setting log formats for different log levels. Log records with level `logging.ERROR` or higher are printed to STDERR if using defaults with `MultilevelFormatter.setDefaults()`.
 
-Importing `MultiLevelFormatter` adds MESSAGE level (`25`) to logging and an `logging.message()` method. The idea is that you can use `logging.message()` instead of `print()` and use logging levels to control verbosity. See the full example below.  
-
 
 ## Install
 
 *Python 3.11 or later is required.*
 
 ```sh
 pip install multilevelformatter
 ```
 
 ## Usage
 
-*Please note.* If you use `mypy`, you need to add `# type: ignore` to the lines assigning `logging.message` to `message` (function) and whenever using `logging.MESSAGE` log level name. In practice this will be few lines in a module. `mypy` does not recognize the modifications to the `logging` class that is done when importing `multilevelformatter`. See [mypy#5363](https://github.com/python/mypy/issues/5363) for details.
 
 ```python
 
 logger = logging.getLogger(__name__)
 error = logger.error
-warning = logger.warning
-# added when importing multilevelformatter
-message = logging.message  # type: ignore 
+message = logger.warning
 verbose = logger.info
 debug = logger.debug
 
 # Not complete, does not run
 def main() -> None:
     
     ...
 
     # assumes command line arguments have been parsed into 
     # boolean flags: arg_verbose, arg_debug, arg_silent
     
-    # MultiLevelFormatter adds MESSAGE level (25) to logging
-    LOG_LEVEL: int = logging.MESSAGE # type: ignore 
+    LOG_LEVEL: int = logging.WARNING
     if arg_verbose: 
         LOG_LEVEL = logging.INFO
-    elif arg_warning:
-        LOG_LEVEL = logging.WARNING
     elif arg_debug:
         LOG_LEVEL = logging.DEBUG
     elif arg_silent:
         LOG_LEVEL = logging.ERROR
     MultilevelFormatter.setDefaults(logger, log_file=log)
     logger.setLevel(LOG_LEVEL)
 
@@ -61,16 +53,15 @@
 from typer import Typer, Option
 from typing import Annotated, Optional
 from pathlib import Path
 from multilevelformatter import MultilevelFormatter
 
 logger = logging.getLogger(__name__)
 error = logger.error
-# MultiLevelFormatter adds MESSAGE level and message() to logging
-message =  logger.message # type: ignore 
+message =  logger.warning 
 verbose = logger.info
 debug = logger.debug
 
 # the demo uses typer for CLI parsing. 
 # Typer has nothing to do with MultiLevelFormatter
 app = Typer()
 
@@ -103,23 +94,22 @@
     ] = False,
     log: Annotated[Optional[Path], Option(help="log to FILE", metavar="FILE")] = None,
 ) -> None:
     """MultilevelFormatter demo"""
     global logger
 
     try:
-        LOG_LEVEL: int = logging.MESSAGE # type: ignore 
+        LOG_LEVEL: int = logging.WARNING
         if print_verbose:
             LOG_LEVEL = logging.INFO
         elif print_debug:
             LOG_LEVEL = logging.DEBUG
         elif print_silent:
             LOG_LEVEL = logging.ERROR
-        MultilevelFormatter.setDefaults(logger, log_file=log)
-        logger.setLevel(LOG_LEVEL)
+        MultilevelFormatter.setDefaults(logger, log_file=log, level=LOG_LEVEL)        
     except Exception as err:
         error(f"{err}")
     message("standard")
     verbose("verbose")
     error("error")
     debug("debug")
```

### Comparing `multilevelformatter-0.3.5/pyproject.toml` & `multilevelformatter-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [project]
 name = "multilevelformatter"
-version = "0.3.5"
+version = "0.4.0"
 authors = [{ name = "Jylpah", email = "jylpah@gmail.com" }]
 description = "logger.Formatter to simplify setting formatting for multiple logging levels"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries",
 ]
 
+dependencies = ["Deprecated>=1.2.14"]
+
 [project.optional-dependencies]
 dev = [
     "build>=0.10",
     "hatchling>=1.22.4",
     "mypy>=1.8",
     "pip-chill>=1.0",
     "pytest>=8.0",
```

### Comparing `multilevelformatter-0.3.5/PKG-INFO` & `multilevelformatter-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.3
 Name: multilevelformatter
-Version: 0.3.5
+Version: 0.4.0
 Summary: logger.Formatter to simplify setting formatting for multiple logging levels
 Project-URL: Homepage, https://github.com/Jylpah/multilevelformatter
 Project-URL: Bug Tracker, https://github.com/Jylpah/multilevelformatter/issues
 Author-email: Jylpah <jylpah@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.11
+Requires-Dist: deprecated>=1.2.14
 Provides-Extra: dev
 Requires-Dist: build>=0.10; extra == 'dev'
 Requires-Dist: hatchling>=1.22.4; extra == 'dev'
 Requires-Dist: mypy>=1.8; extra == 'dev'
 Requires-Dist: pip-chill>=1.0; extra == 'dev'
 Requires-Dist: pytest-asyncio>=0.23; extra == 'dev'
 Requires-Dist: pytest-cov>=4.1; extra == 'dev'
@@ -26,53 +27,45 @@
 Requires-Dist: typer>=0.9.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # MultiLevelFormatter
 
 `MultiLevelFormatter` is a Python `logging.Formatter` that simplifies setting log formats for different log levels. Log records with level `logging.ERROR` or higher are printed to STDERR if using defaults with `MultilevelFormatter.setDefaults()`.
 
-Importing `MultiLevelFormatter` adds MESSAGE level (`25`) to logging and an `logging.message()` method. The idea is that you can use `logging.message()` instead of `print()` and use logging levels to control verbosity. See the full example below.  
-
 
 ## Install
 
 *Python 3.11 or later is required.*
 
 ```sh
 pip install multilevelformatter
 ```
 
 ## Usage
 
-*Please note.* If you use `mypy`, you need to add `# type: ignore` to the lines assigning `logging.message` to `message` (function) and whenever using `logging.MESSAGE` log level name. In practice this will be few lines in a module. `mypy` does not recognize the modifications to the `logging` class that is done when importing `multilevelformatter`. See [mypy#5363](https://github.com/python/mypy/issues/5363) for details.
 
 ```python
 
 logger = logging.getLogger(__name__)
 error = logger.error
-warning = logger.warning
-# added when importing multilevelformatter
-message = logging.message  # type: ignore 
+message = logger.warning
 verbose = logger.info
 debug = logger.debug
 
 # Not complete, does not run
 def main() -> None:
     
     ...
 
     # assumes command line arguments have been parsed into 
     # boolean flags: arg_verbose, arg_debug, arg_silent
     
-    # MultiLevelFormatter adds MESSAGE level (25) to logging
-    LOG_LEVEL: int = logging.MESSAGE # type: ignore 
+    LOG_LEVEL: int = logging.WARNING
     if arg_verbose: 
         LOG_LEVEL = logging.INFO
-    elif arg_warning:
-        LOG_LEVEL = logging.WARNING
     elif arg_debug:
         LOG_LEVEL = logging.DEBUG
     elif arg_silent:
         LOG_LEVEL = logging.ERROR
     MultilevelFormatter.setDefaults(logger, log_file=log)
     logger.setLevel(LOG_LEVEL)
 
@@ -89,16 +82,15 @@
 from typer import Typer, Option
 from typing import Annotated, Optional
 from pathlib import Path
 from multilevelformatter import MultilevelFormatter
 
 logger = logging.getLogger(__name__)
 error = logger.error
-# MultiLevelFormatter adds MESSAGE level and message() to logging
-message =  logger.message # type: ignore 
+message =  logger.warning 
 verbose = logger.info
 debug = logger.debug
 
 # the demo uses typer for CLI parsing. 
 # Typer has nothing to do with MultiLevelFormatter
 app = Typer()
 
@@ -131,23 +123,22 @@
     ] = False,
     log: Annotated[Optional[Path], Option(help="log to FILE", metavar="FILE")] = None,
 ) -> None:
     """MultilevelFormatter demo"""
     global logger
 
     try:
-        LOG_LEVEL: int = logging.MESSAGE # type: ignore 
+        LOG_LEVEL: int = logging.WARNING
         if print_verbose:
             LOG_LEVEL = logging.INFO
         elif print_debug:
             LOG_LEVEL = logging.DEBUG
         elif print_silent:
             LOG_LEVEL = logging.ERROR
-        MultilevelFormatter.setDefaults(logger, log_file=log)
-        logger.setLevel(LOG_LEVEL)
+        MultilevelFormatter.setDefaults(logger, log_file=log, level=LOG_LEVEL)        
     except Exception as err:
         error(f"{err}")
     message("standard")
     verbose("verbose")
     error("error")
     debug("debug")
```

