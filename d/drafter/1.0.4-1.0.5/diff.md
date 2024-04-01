# Comparing `tmp/drafter-1.0.4.tar.gz` & `tmp/drafter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drafter-1.0.4.tar", last modified: Sat Mar 30 23:32:30 2024, max compression
+gzip compressed data, was "drafter-1.0.5.tar", last modified: Mon Apr  1 19:01:23 2024, max compression
```

## Comparing `drafter-1.0.4.tar` & `drafter-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 23:32:30.539620 drafter-1.0.4/
--rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2024-03-30 23:32:30.539620 drafter-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 23:32:30.538623 drafter-1.0.4/drafter.egg-info/
--rw-rw-rw-   0        0        0      766 2024-03-30 23:32:30.000000 drafter-1.0.4/drafter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-03-30 23:32:30.000000 drafter-1.0.4/drafter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 23:32:30.000000 drafter-1.0.4/drafter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-30 23:32:30.000000 drafter-1.0.4/drafter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-30 23:32:30.000000 drafter-1.0.4/drafter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    58474 2024-03-30 23:30:51.000000 drafter-1.0.4/drafter.py
--rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 23:32:30.540619 drafter-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-09-09 13:39:14.000000 drafter-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:01:23.594720 drafter-1.0.5/
+-rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2024-04-01 19:01:23.593714 drafter-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 19:01:23.592643 drafter-1.0.5/drafter.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    59440 2024-04-01 19:01:10.000000 drafter-1.0.5/drafter.py
+-rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:01:23.594720 drafter-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-09-09 13:39:14.000000 drafter-1.0.5/setup.py
```

### Comparing `drafter-1.0.4/LICENSE.txt` & `drafter-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drafter-1.0.4/PKG-INFO` & `drafter-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.0.4
+Version: 1.0.5
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.0.4/drafter.egg-info/PKG-INFO` & `drafter-1.0.5/drafter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.0.4
+Version: 1.0.5
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.0.4/drafter.py` & `drafter-1.0.5/drafter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 TODO: Finish these
-- [ ] Fix external links
+- [ ] Fix external links (ExternalLink command?)
 - [X] Client-side server mode
 - [?] Other HTML components
 - [ ] set_page_title(title), set_page_style(**attributes)
-- [ ] Copy ALL unique tests button
+- [ ] Reset all button
+- [X] Copy ALL unique tests button
 - [X] Show all of the tests in a nice clean way
 - [X] Make it trivial to copy the route history as tests
 - [X] Show the current route in the debug information
 - [X] classes keyword parameter
 - [ ] Create styling functions
 - [ ] Make it so you can remove the frame and deploy this more easily
 - [ ] Optional bootstrap support
@@ -34,15 +35,15 @@
 - [ ] PreformattedText
 - [X] Header
 - [X] TextArea
 """
 import sys
 import json
 from typing import Any
-from urllib.parse import urlencode, urlparse, parse_qs
+from urllib.parse import urlencode, urlparse, parse_qs, quote_plus
 import traceback
 import inspect
 import re
 from functools import wraps
 from dataclasses import dataclass, is_dataclass, replace, asdict, fields
 from dataclasses import field as dataclass_field
 import logging
@@ -58,19 +59,20 @@
     from bottle import Bottle, abort, request, static_file
 
     DEFAULT_BACKEND = "bottle"
 except ImportError:
     DEFAULT_BACKEND = "none"
     logger.warn("Bottle unavailable; backend will be disabled and run in test-only mode.")
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 
 RESTORABLE_STATE_KEY = "--restorable-state"
 SUBMIT_BUTTON_KEY = '--submit-button'
 PREVIOUSLY_PRESSED_BUTTON = "--last-button"
+LABEL_SEPARATOR = "$@~@$"
 
 try:
     import bakery
 except:
     bakery = None
 
 
@@ -333,34 +335,34 @@
                 raise ValueError(f"Link `{self.url}` is not a valid external url.\n{invalid_external_url_reason}.")
             raise ValueError(f"Link `{self.text}` points to non-existent page `{self.url}`.")
         return True
 
     def create_arguments(self, arguments, label_namespace):
         parameters = self.parse_arguments(arguments, label_namespace)
         if parameters:
-            return "\n".join(f"<input type='hidden' name='{name}' value='{value}' />"
+            return "\n".join(f"<input type='hidden' name='{name}' value='{quote_plus(str(value))}' />"
                              for name, value in parameters.items())
         return ""
 
     def parse_arguments(self, arguments, label_namespace):
         if arguments is None:
             return {}
         if isinstance(arguments, dict):
             return arguments
         if isinstance(arguments, Argument):
-            return {f"{label_namespace}$${arguments.name}": arguments.value}
+            return {f"{label_namespace}{LABEL_SEPARATOR}{arguments.name}": arguments.value}
         if isinstance(arguments, list):
             result = {}
             for arg in arguments:
                 if isinstance(arg, Argument):
                     arg, value = arg.name, arg.value
                     result[arg.name] = arg.value
                 else:
                     arg, value = arg
-                result[f"{label_namespace}$${arg}"] = value
+                result[f"{label_namespace}{LABEL_SEPARATOR}{arg}"] = value
         raise ValueError(f"Could not create arguments from the provided value: {arguments}")
 
 URL_REGEX = r"^(?:http(s)?://)[\w.-]+(?:\.[\w\.-]+)+[\w\-\._~:/?#[\]@!\$&'\(\)\*\+,;=.]+$"
 
 
 def check_invalid_external_url(url: str) -> str:
     if url.startswith("file://"):
@@ -518,19 +520,22 @@
 @dataclass
 class Argument(PageContent):
     name: str
     value: Any
 
     def __init__(self, name: str, value: Any, **kwargs):
         self.name = name
+        if not isinstance(value, (str, int, float, bool)):
+            raise ValueError(f"Argument values must be strings, integers, floats, or booleans. Found {type(value)}")
         self.value = value
         self.extra_settings = kwargs
 
     def __str__(self) -> str:
-        return f"<input type='hidden' name='{self.name}' value='{self.value}' {self.parse_extra_settings()} />"
+        value = quote_plus(self.value)
+        return f"<input type='hidden' name='{self.name}' value='{value}' {self.parse_extra_settings()} />"
 
 
 @dataclass
 class Link(PageContent, LinkContent):
     text: str
     url: str
 
@@ -658,14 +663,23 @@
 @dataclass
 class HorizontalRule(PageContent):
     def __str__(self) -> str:
         return "<hr />"
 
 
 @dataclass
+class Span(PageContent):
+    def __init__(self, *args):
+        self.content = args
+
+    def __str__(self) -> str:
+        return f"<span>{''.join(str(item) for item in self.content)}</span>"
+
+
+@dataclass
 class Button(PageContent, LinkContent):
     text: str
     url: str
     arguments: list[Argument]
     external: bool = False
 
     def __init__(self, text: str, url: str, arguments=None, **kwargs):
@@ -928,18 +942,18 @@
     except Exception as e:
         return repr(content)
 
 
 def remap_hidden_form_parameters(kwargs: dict, button_pressed: str):
     renamed_kwargs = {}
     for key, value in kwargs.items():
-        if button_pressed and key.startswith(f"{button_pressed}$$"):
-            key = key[len(f"{button_pressed}$$"):]
+        if button_pressed and key.startswith(f"{button_pressed}{LABEL_SEPARATOR}"):
+            key = key[len(f"{button_pressed}{LABEL_SEPARATOR}"):]
             renamed_kwargs[key] = value
-        else:
+        elif LABEL_SEPARATOR not in key:
             renamed_kwargs[key] = value
     return renamed_kwargs
 
 
 @dataclass
 class VisitedPage:
     url: str
@@ -1135,14 +1149,20 @@
         # Type conversion if required
         expected_types = {name: p.annotation for name, p in
                           inspect.signature(original_function).parameters.items()}
         args = [self.convert_parameter(param, val, expected_types)
                 for param, val in zip(expected_parameters, args)]
         kwargs = {param: self.convert_parameter(param, val, expected_types)
                   for param, val in kwargs.items()}
+        # Verify all arguments are in expected_parameters
+        for key, value in kwargs.items():
+            if key not in expected_parameters:
+                raise ValueError(
+                    f"Unexpected parameter {key}={value!r} in {original_function.__name__}. "
+                    f"Expected parameters: {expected_parameters}")
         # Final return result
         representation = [repr(arg) for arg in args] + [
             f"{key}={value!r}" if show_names.get(key, False) else repr(value)
             for key, value in sorted(kwargs.items(), key=lambda item: expected_parameters.index(item[0]))]
         return args, kwargs, ", ".join(representation), button_pressed
 
     def handle_images(self):
```

### Comparing `drafter-1.0.4/setup.py` & `drafter-1.0.5/setup.py`

 * *Files identical despite different names*

