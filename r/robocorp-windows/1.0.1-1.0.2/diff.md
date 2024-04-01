# Comparing `tmp/robocorp_windows-1.0.1.tar.gz` & `tmp/robocorp_windows-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_windows-1.0.1.tar", max compression
+gzip compressed data, was "robocorp_windows-1.0.2.tar", max compression
```

## Comparing `robocorp_windows-1.0.1.tar` & `robocorp_windows-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1269 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2853 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/README.md
--rw-r--r--   0        0        0     8927 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/__init__.py
--rw-r--r--   0        0        0       93 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_com_error.py
--rw-r--r--   0        0        0     2348 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_config.py
--rw-r--r--   0        0        0      757 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_config_uiautomation.py
--rw-r--r--   0        0        0    65422 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_control_element.py
--rw-r--r--   0        0        0    20601 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_desktop.py
--rw-r--r--   0        0        0      768 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_errors.py
--rw-r--r--   0        0        0    18340 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_find_ui_automation.py
--rw-r--r--   0        0        0     6995 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_find_window.py
--rw-r--r--   0        0        0      383 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_func_lru_cache.py
--rw-r--r--   0        0        0     1219 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_func_robocorp_tasks_cache.py
--rw-r--r--   0        0        0     1827 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_icon_from_file.py
--rw-r--r--   0        0        0    34663 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_inspect.py
--rw-r--r--   0        0        0     5739 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_iter_tree.py
--rw-r--r--   0        0        0    21962 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_match_ast.py
--rw-r--r--   0        0        0     2014 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_match_common.py
--rw-r--r--   0        0        0     5475 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_match_tokenization.py
--rw-r--r--   0        0        0     2741 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_processes.py
--rw-r--r--   0        0        0     1245 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_screenshot.py
--rw-r--r--   0        0        0     4409 2024-01-14 08:19:19.438555 robocorp_windows-1.0.1/src/robocorp/windows/_ui_automation_wrapper.py
--rw-r--r--   0        0        0        0 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/_vendored/__init__.py
--rw-r--r--   0        0        0       73 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/__init__.py
--rw-r--r--   0        0        0   101888 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll
--rw-r--r--   0        0        0    84480 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll
--rw-r--r--   0        0        0   400321 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/uiautomation.py
--rw-r--r--   0        0        0       18 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/version.py
--rw-r--r--   0        0        0    12077 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/_window_element.py
--rw-r--r--   0        0        0       15 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/protocols.py
--rw-r--r--   0        0        0        0 2024-01-14 08:19:19.454180 robocorp_windows-1.0.1/src/robocorp/windows/py.typed
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 robocorp_windows-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1318 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3066 2024-04-01 14:12:19.156920 robocorp_windows-1.0.2/README.md
+-rw-r--r--   0        0        0     9088 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_com_error.py
+-rw-r--r--   0        0        0     2348 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_config.py
+-rw-r--r--   0        0        0      757 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_config_uiautomation.py
+-rw-r--r--   0        0        0    65948 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_control_element.py
+-rw-r--r--   0        0        0    20731 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_desktop.py
+-rw-r--r--   0        0        0      768 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_errors.py
+-rw-r--r--   0        0        0    18340 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_find_ui_automation.py
+-rw-r--r--   0        0        0     6996 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_find_window.py
+-rw-r--r--   0        0        0      383 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_func_lru_cache.py
+-rw-r--r--   0        0        0     1219 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_func_robocorp_tasks_cache.py
+-rw-r--r--   0        0        0     1827 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_icon_from_file.py
+-rw-r--r--   0        0        0    34663 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_inspect.py
+-rw-r--r--   0        0        0     5739 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_iter_tree.py
+-rw-r--r--   0        0        0    21962 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_match_ast.py
+-rw-r--r--   0        0        0     2014 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_match_common.py
+-rw-r--r--   0        0        0     5475 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_match_tokenization.py
+-rw-r--r--   0        0        0     2741 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_processes.py
+-rw-r--r--   0        0        0     1245 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_screenshot.py
+-rw-r--r--   0        0        0     4409 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_ui_automation_wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/__init__.py
+-rw-r--r--   0        0        0   101888 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll
+-rw-r--r--   0        0        0    84480 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll
+-rw-r--r--   0        0        0   400321 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/uiautomation.py
+-rw-r--r--   0        0        0       18 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/version.py
+-rw-r--r--   0        0        0    12077 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/_window_element.py
+-rw-r--r--   0        0        0       15 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:12:19.172544 robocorp_windows-1.0.2/src/robocorp/windows/py.typed
+-rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 robocorp_windows-1.0.2/PKG-INFO
```

### Comparing `robocorp_windows-1.0.1/pyproject.toml` & `robocorp_windows-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-windows"
-version = "1.0.1"
+version = "1.0.2"
 description = "Robocorp Windows Automation (API to automate Windows)"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
@@ -49,7 +49,12 @@
 ignore_missing_imports = true
 
 [tool.robocorp.log]
 
 log_filter_rules = [
     {name = "wincon", kind = "exclude"},
 ]
+
+[tool.ruff]
+exclude = [
+    "_vendored",
+]
```

### Comparing `robocorp_windows-1.0.1/README.md` & `robocorp_windows-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,58 @@
-`robocorp-windows` is a library which can be used for Windows desktop automation.
+# robocorp-windows
 
-The basic idea of the library is enabling windows and controls to be found
-by leveraging `locators` (i.e.: strings which identify how to reach some
-window or control) and then interacting with such elements.
-
-There are 3 basic abstractions in the library:
-
-- `Desktop`: enables finding `WindowElement`s and interacting directly with the 
-  desktop (so, actions which aren't tied to a Window or Control can be used directly
-  through the `Desktop`).
-- `WindowElement`: enables finding `ControlElement`s and interacting with a Window.
-- `ControlElement`: enables finding child `ControlElement`s and interacting with a specific Control.
+The **robocop-windows** package brings a library that can be used for Windows desktop automation.
 
-Note: these classes are always created by the library itself and are not expected
-to be subclassed or instanced directly.
+The basic idea of the library is to enable windows and controls to be found by leveraging "locators" (strings that identify how to reach some window or control), then interacting with such elements.
+
+There are three fundamental abstractions in the library:
+
+- `Desktop`: enables finding `WindowElement`s and interacting directly with the desktop, like opening or closing apps. These actions aren't tied to a specific _Window_ or _Control_.
+- `WindowElement`: enables finding direct `ControlElement`s and interacting with a specific _Window_.
+- `ControlElement`: enables finding child `ControlElement`s and interacting with a specific _Control_.
+
+> Note: The library itself always creates these classes which are not expected to be subclassed or instanced directly.
 
 ## Usage
 
-The library concepts revolve around the idea that the window of interest will be 
-initially found using `find_window` and then, with that window reference, other
-controls can be queried and interacted with (for clicking, entering text, etc).
+[![`robocorp-windows`](https://img.shields.io/pypi/v/robocorp-windows?label=robocorp-windows)](https://pypi.org/project/robocorp-windows/)
+
+> 👉 Check that you have added the dependency in your configuration; this library is not part of the [**robocorp**](https://pypi.org/project/robocorp/) bundle.
+> - _conda.yaml_ for automation [Task Packages](https://robocorp.com/docs/robot-structure)
+> - _package.yaml_ for automation Action Packages
+> - _requirements.txt_, _pyproject.toml_, _setup.py|cfg_ etc. for the rest
 
-Below is an example using the windows calculator:
+The library concepts revolve around the idea that the window of interest will be initially found using `find_window` and then, with that window reference, other controls can be queried and interacted with (for clicking, entering text etc.).
 
+Below is an example using the Windows' Calculator app:
 
 ```python
 from robocorp import windows
 
-# Get the calculator window
+# Get the Calculator window.
 calc = windows.find_window("name:Calculator")
 
-# Press button 0 (the locator is dependent on the windows version).
-button0 = calc.find('(name:Zero or name:0) and class:Button')
+# Press button "0" (the locator may vary based on the Windows version).
+button0 = calc.find("(name:0 or name:num0Button) and type:Button")
 button0.click()
 
-# Clear the calculator (the locator is dependent on the windows version).
-calc.click("id:clearButton or name:Clear")
+# Clear the Calculator (the locator may vary based on the Windows version).
+calc.click("id:clearEntryButton or name:Clear")
 
-# Send the keys directly to the calculator
+# Send the keys directly to the Calculator by typing them from the keyboard.
 calc.send_keys(keys="96+4=")
 ```
 
-
 ## Guides
 
-- [Understanding Locators](https://github.com/robocorp/robocorp/blob/master/windows/docs/guides/00-locators.md)
-- [Building Locators using the builtin inspector](https://github.com/robocorp/robocorp/blob/master/windows/docs/guides/01-locator-inspecting.md)
-- [Special keys](https://github.com/robocorp/robocorp/blob/master/windows/docs/guides/02-special-keys.md)
-
+- [Quickstart](https://github.com/robocorp/robocorp/blob/master/windows/docs/guides/00-quickstart.md)
+- [Understanding Locators](https://github.com/robocorp/robocorp/blob/master/windows/docs/guides/01-locators.md)
+- [Building Locators using the builtin inspector](https://github.com/robocorp/robocorp/blob/master/windows/docs/guides/02-locator-inspecting.md)
+- [Special keys](https://github.com/robocorp/robocorp/blob/master/windows/docs/guides/03-special-keys.md)
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.windows](https://github.com/robocorp/robocorp/blob/master/windows/docs/api/robocorp.windows.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/windows/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/windows/docs/CHANGELOG.md).
-
-## Versioning
-
-This library uses semantic versioning, so, when a breaking change is done
-a new major version is published, but beware that modules starting with an 
-underscore `_` in `robocorp.windows` are not considered
-part of the public API and should not be imported directly (so, only objects/classes
-reached from the `robocorp.windows` namespace should be used -- if access to some
-other method/class is needed, please create a feature request to address it).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/__init__.py` & `robocorp_windows-1.0.2/src/robocorp/windows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # ruff: noqa: F401
 """
-The `robocorp-windows` library is a library to be used to interact
-with native widgets on the Windows OS.
+Module used to interact with native widgets on the Windows OS through UI Automation.
+
+This library can be made available by pinning
+![`robocorp-windows`](https://img.shields.io/pypi/v/robocorp-windows?label=robocorp-windows)
+in your dependencies' configuration.
 """
+
 import time
 import typing
 from functools import lru_cache
 from typing import Callable, List, Literal, Optional, overload
 
 from ._config import Config
 from ._control_element import ControlElement
@@ -21,15 +25,15 @@
 )
 from ._window_element import WindowElement
 from .protocols import Locator
 
 if typing.TYPE_CHECKING:
     from PIL.Image import Image
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def get_icon_from_file(path: str) -> Optional["Image"]:
     """
     Provides the icon stored in the file of the given path.
```

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_config.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_config_uiautomation.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_config_uiautomation.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_control_element.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_control_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,29 @@
 
 
 PatternType = Union["ValuePattern", "LegacyIAccessiblePattern"]
 
 DEFAULT_SEND_KEYS_INTERVAL = 0.01
 
 
+class _SentinelValidator:
+    # Used to determine the validator function for `ControlElement.set_value` method.
+    #  If a validator is not passed explicitly, then the `set_value_validator` function
+    #  will be used as default.
+
+    def __call__(self, *args, **kwargs):
+        pass
+
+    def __repr__(self):
+        return "_SentinelValidator"
+
+    def __str__(self):
+        return "_SentinelValidator"
+
+
 def set_value_validator(expected: str, actual: str) -> bool:
     """Checks the passed against the final set value and returns status."""
     return actual.strip() == expected.strip()  # due to EOLs inconsistency
 
 
 def _wait_time() -> float:
     """
@@ -719,15 +734,15 @@
         if not show_properties:
             for child in iter_in:
                 print(child, file=stream)
         else:
             for child in iter_in:
                 print(child, file=stream)
 
-                space = " " * ((child.depth * 4 + 2))
+                space = " " * (child.depth * 4 + 2)
                 control = child.control
                 print(f"{space}Properties:", file=stream)
                 try:
                     v = control.get_value()
                     print(f"  {space}get_value() = {v!r}", file=stream)
                 except ActionNotPossible:
                     pass
@@ -1451,15 +1466,15 @@
         self,
         value: str,
         *,
         append: bool = False,
         enter: bool = False,
         newline: bool = False,
         send_keys_fallback: bool = True,
-        validator: Optional[Callable] = set_value_validator,
+        validator: Optional[Callable] = _SentinelValidator(),
         locator: Optional[Locator] = None,
         search_depth: int = 8,
         timeout: Optional[float] = None,
     ) -> "ControlElement":
         """
         Set the value in the element (usually used with combo boxes or
         text controls).
@@ -1551,14 +1566,17 @@
             element = self
         else:
             element = self.find(locator, search_depth, timeout=timeout)
 
         get_value_pattern = self._get_value_pattern(element.ui_automation_control)
         action = "Appending" if append else "Setting"
 
+        if isinstance(validator, _SentinelValidator):
+            validator = set_value_validator
+
         if get_value_pattern:
             self._set_value_with_pattern(
                 value,
                 newline_string,
                 action=action,
                 get_value_pattern=get_value_pattern,
                 append=append,
```

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_desktop.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_desktop.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,29 +351,35 @@
         if self.get_win_version() == "11":
             search_cmd = search_cmd.rstrip("s")
         self.send_keys(search_cmd)
         self.send_keys(text)
         self.send_keys("{Enter}")
         time.sleep(wait_time)
 
-    def get_win_version(self) -> str:
+    @staticmethod
+    def get_win_version() -> str:
         """
         Windows only utility which returns the current Windows major version.
 
         Returns:
             The current Windows major version (i.e.: '10', '11').
         """
         # Windows terminal `ver` command is bugged, until that's fixed, check by build
         #  number. (the same applies for `platform.version()`)
         import platform
 
+        WINDOWS_11_BUILD = 22000
+        WINDOWS_10 = "10"
+        WINDOWS_11 = "11"
+
         version_parts = platform.version().split(".")
         major = version_parts[0]
-        if major == "10" and int(version_parts[2]) >= 22000:
-            major = "11"
+
+        if major == WINDOWS_10 and int(version_parts[2]) >= WINDOWS_11_BUILD:
+            major = WINDOWS_11
 
         return major
 
     def wait_for_active_window(
         self,
         locator: Locator,
         timeout: Optional[float] = None,
```

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_errors.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_errors.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_find_ui_automation.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_find_ui_automation.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_find_window.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_find_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ._window_element import WindowElement
 from .protocols import Locator
 
 logger = logging.getLogger(__name__)
 
 
 def restrict_to_window_locators(
-    or_search_params: Tuple[OrSearchParams, ...]
+    or_search_params: Tuple[OrSearchParams, ...],
 ) -> Tuple[OrSearchParams, ...]:
     last_part: OrSearchParams = or_search_params[-1]
     also_add_as_pane = []
     for search_params in last_part.parts:
         assert isinstance(search_params, SearchParams)
 
         # Ok, leave is is (the type is already defined)
```

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_func_robocorp_tasks_cache.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_func_robocorp_tasks_cache.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_icon_from_file.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_icon_from_file.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_inspect.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_inspect.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_iter_tree.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_iter_tree.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_match_ast.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_match_ast.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_match_common.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_match_common.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_match_tokenization.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_match_tokenization.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_processes.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_processes.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_screenshot.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_screenshot.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_ui_automation_wrapper.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_ui_automation_wrapper.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll` & `robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X64.dll`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll` & `robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/bin/UIAutomationClient_VC140_X86.dll`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_vendored/uiautomation/uiautomation.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_vendored/uiautomation/uiautomation.py`

 * *Files identical despite different names*

### Comparing `robocorp_windows-1.0.1/src/robocorp/windows/_window_element.py` & `robocorp_windows-1.0.2/src/robocorp/windows/_window_element.py`

 * *Files identical despite different names*

