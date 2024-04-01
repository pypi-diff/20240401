# Comparing `tmp/atom-tools-0.4.5.tar.gz` & `tmp/atom-tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atom-tools-0.4.5.tar", last modified: Fri Mar 22 20:36:18 2024, max compression
+gzip compressed data, was "atom-tools-0.5.0.tar", last modified: Mon Apr  1 18:50:26 2024, max compression
```

## Comparing `atom-tools-0.4.5.tar` & `atom-tools-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:18.824405 atom-tools-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 20:36:13.000000 atom-tools-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-22 20:36:13.000000 atom-tools-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-22 20:36:18.824405 atom-tools-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-03-22 20:36:13.000000 atom-tools-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:18.816405 atom-tools-0.4.5/atom_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:18.820405 atom-tools-0.4.5/atom_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/command_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:18.820405 atom-tools-0.4.5/atom_tools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/commands/validate_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/cli/logging_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:18.820405 atom-tools-0.4.5/atom_tools/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26224 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/lib/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/lib/regex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/lib/slices.py
--rw-r--r--   0 runner    (1001) docker     (127)    26178 2024-03-22 20:36:13.000000 atom-tools-0.4.5/atom_tools/lib/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:18.820405 atom-tools-0.4.5/atom_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-22 20:36:18.000000 atom-tools-0.4.5/atom_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-22 20:36:18.000000 atom-tools-0.4.5/atom_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 20:36:18.000000 atom-tools-0.4.5/atom_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 20:36:18.000000 atom-tools-0.4.5/atom_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 20:36:18.000000 atom-tools-0.4.5/atom_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 20:36:18.000000 atom-tools-0.4.5/atom_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-22 20:36:13.000000 atom-tools-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 20:36:18.824405 atom-tools-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:36:18.820405 atom-tools-0.4.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)  1237468 2024-03-22 20:36:13.000000 atom-tools-0.4.5/test/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-22 20:36:13.000000 atom-tools-0.4.5/test/test_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:26.118465 atom-tools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 18:50:16.000000 atom-tools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 18:50:16.000000 atom-tools-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-01 18:50:26.118465 atom-tools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-01 18:50:16.000000 atom-tools-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:26.114465 atom-tools-0.5.0/atom_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:26.114465 atom-tools-0.5.0/atom_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/command_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:26.114465 atom-tools-0.5.0/atom_tools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/commands/query_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/commands/validate_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/cli/logging_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:26.118465 atom-tools-0.5.0/atom_tools/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/lib/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/lib/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/lib/regex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/lib/slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-01 18:50:16.000000 atom-tools-0.5.0/atom_tools/lib/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:26.118465 atom-tools-0.5.0/atom_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-01 18:50:26.000000 atom-tools-0.5.0/atom_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-01 18:50:26.000000 atom-tools-0.5.0/atom_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:50:26.000000 atom-tools-0.5.0/atom_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 18:50:26.000000 atom-tools-0.5.0/atom_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 18:50:26.000000 atom-tools-0.5.0/atom_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 18:50:26.000000 atom-tools-0.5.0/atom_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-01 18:50:16.000000 atom-tools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:50:26.118465 atom-tools-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:50:26.118465 atom-tools-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)   831738 2024-04-01 18:50:16.000000 atom-tools-0.5.0/test/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-01 18:50:16.000000 atom-tools-0.5.0/test/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-01 18:50:16.000000 atom-tools-0.5.0/test/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-01 18:50:16.000000 atom-tools-0.5.0/test/test_utils.py
```

### Comparing `atom-tools-0.4.5/LICENSE` & `atom-tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atom-tools-0.4.5/atom_tools/cli/application.py` & `atom-tools-0.5.0/atom_tools/cli/application.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """
 Base console application.
 """
 import logging
+import sys
 from importlib import import_module
 from typing import Callable
 
 from cleo.application import Application as BaseApplication
 from cleo.events.console_command_event import ConsoleCommandEvent
 from cleo.events.console_events import COMMAND
 from cleo.events.event import Event
 from cleo.events.event_dispatcher import EventDispatcher
+from cleo.io.inputs.argv_input import ArgvInput
+from cleo.io.inputs.input import Input
 from cleo.io.io import IO
+from cleo.io.outputs.output import Output
+from cleo.io.outputs.stream_output import StreamOutput
 
 from atom_tools import __version__
 from atom_tools.cli.command_loader import CommandLoader
 from atom_tools.cli.commands.command import Command
 from atom_tools.cli.logging_config import ATOM_TOOLS_FILTER, IOFormatter, IOHandler
 
 
@@ -44,14 +49,16 @@
         return command
 
     return _load
 
 
 COMMANDS = [
     'convert',
+    'filter',
+    'query-endpoints',
     'validate-lines',
 ]
 
 
 class Application(BaseApplication):
     """
     Represents the main application.
@@ -67,23 +74,41 @@
         dispatcher = EventDispatcher()
         dispatcher.add_listener(COMMAND, self.register_command_loggers)
         self.set_event_dispatcher(dispatcher)
         self._io = self.create_io()
         command_loader = CommandLoader({name: load_command(name) for name in COMMANDS})
         self.set_command_loader(command_loader)
 
+    def create_io(
+        self,
+        input: Input | None = None,  # pylint: disable=redefined-builtin
+        output: Output | None = None,
+        error_output: Output | None = None,
+    ) -> IO:
+        if not input:
+            input = ArgvInput()
+            input.set_stream(sys.stdin)
+
+        if output is None:
+            output = StreamOutput(sys.stdout)
+
+        if error_output is None:
+            error_output = StreamOutput(sys.stderr)
+
+        return IO(input, output, error_output)
+
     @staticmethod
     def register_command_loggers(event: Event, event_name: str, _: EventDispatcher) -> None:  # pylint: disable=unused-argument
         """
-        Registers the command loggers.
+        Register command loggers. Based heavily on Poetry's implementation.
 
         Args:
-            event (Event): The event.
-            event_name (str): The event name.
-            _: EventDispatcher: The event dispatcher.
+            event (Event): The event object.
+            event_name (str): The name of the event.
+            _: The event dispatcher.
         """
         assert isinstance(event, ConsoleCommandEvent)
         command = event.command
         if not isinstance(command, Command):
             return
 
         io = event.io
@@ -94,15 +119,16 @@
         handler = IOHandler(io)
         handler.setFormatter(IOFormatter())
 
         level = logging.WARNING
 
         if io.is_debug():
             level = logging.DEBUG
-        elif io.is_very_verbose() or io.is_verbose():
+        # elif io.is_very_verbose() or io.is_verbose():
+        else:
             level = logging.INFO
 
         logging.basicConfig(level=level, handlers=[handler])
 
         # only log third-party packages when very verbose
         if not io.is_very_verbose():
             handler.addFilter(ATOM_TOOLS_FILTER)
```

### Comparing `atom-tools-0.4.5/atom_tools/cli/command_loader.py` & `atom-tools-0.5.0/atom_tools/cli/command_loader.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.4.5/atom_tools/cli/commands/convert.py` & `atom-tools-0.5.0/atom_tools/cli/commands/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Convert Command for the atom-tools CLI.
 """
-import json
 import logging
 import sys
 
 from cleo.helpers import option
 
 from atom_tools.cli.commands.command import Command
 from atom_tools.lib.converter import OpenAPI
+from atom_tools.lib.utils import export_json
+
+
+logger = logging.getLogger(__name__)
 
 
 class ConvertCommand(Command):
     """
     This command handles the conversion of an atom slice to a specified
     destination format.
 
@@ -37,24 +40,16 @@
             default='openapi3.0.1',
         ),
         option(
             'input-slice',
             'i',
             'Usages slice file',
             flag=False,
-            default=None,
             value_required=True,
         ),
-        # option(
-        #     'reachables-slice',
-        #     'r',
-        #     'Reachables slice file',
-        #     flag=False,
-        #     default=None,
-        # ),
         option(
             'type',
             't',
             'Origin type of source on which the atom slice was generated.',
             flag=False,
             default='java',
         ),
@@ -76,26 +71,25 @@
 Currently supports creating an OpenAPI 3.x document based on a usages slice."""
     loggers = ['atom_tools.lib.converter', 'atom_tools.lib.regex_utils', 'atom_tools.lib.slices']
 
     def handle(self):
         """
         Executes the convert command and performs the conversion.
         """
-        supported_types = ['java', 'jar', 'python', 'py', 'javascript', 'js', 'typescript', 'ts']
+        supported_types = {'java', 'jar', 'python', 'py', 'javascript', 'js', 'typescript', 'ts'}
         if self.option('type') not in supported_types:
             raise ValueError(f'Unknown origin type: {self.option("type")}')
         match self.option('format'):
             case 'openapi3.1.0' | 'openapi3.0.1':
                 converter = OpenAPI(
                     self.option('format'),
                     self.option('type'),
                     self.option('input-slice'),
                 )
 
                 if not (result := converter.endpoints_to_openapi(self.option('server'))):
                     logging.warning('No results produced!')
                     sys.exit(1)
-                with open(self.option('output-file'), 'w', encoding='utf-8') as f:
-                    json.dump(result, f, indent=4, sort_keys=True)
-                logging.info(f'OpenAPI document written to {self.option("output-file")}.')
+                export_json(result, self.option('output-file'), 4)
+                logger.info(f'OpenAPI document written to {self.option("output-file")}.')
             case _:
                 raise ValueError(f'Unknown destination format: {self.option("format")}')
```

### Comparing `atom-tools-0.4.5/atom_tools/cli/commands/validate_lines.py` & `atom-tools-0.5.0/atom_tools/cli/commands/validate_lines.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.4.5/atom_tools/cli/logging_config.py` & `atom-tools-0.5.0/atom_tools/cli/logging_config.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.4.5/atom_tools/lib/converter.py` & `atom-tools-0.5.0/atom_tools/lib/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from atom_tools.lib.slices import AtomSlice
 
 
 logger = logging.getLogger(__name__)
 regex = OpenAPIRegexCollection()
 exclusions = ['/content-type', '/application/javascript', '/application/json', '/application/text',
-              '/application/xml', '/*', '/*/*', '/allow']
+              '/application/xml', '/*', '/*/*', '/allow', '/GET', '/POST', '/xml', '/cookie']
 
 
 class OpenAPI:
     """Represents an OpenAPI converter object."""
 
     def __init__(
         self,
@@ -153,14 +153,29 @@
                     new_path_item = self.create_paths_item(key, m)
                     if paths_object:
                         paths_object = merge_path_objects(paths_object, new_path_item)
                     else:
                         paths_object = new_path_item
         return paths_object
 
+    def _add_py_request_methods(self, paths_item_object: Dict) -> Dict:
+        """Add default request methods for flask and django"""
+        if self.usages.custom_attr == 'flask':
+            paths_item_object = merge_path_objects(
+                paths_item_object,
+                {'head': {'responses': {}}, 'options': {'responses': {}}}
+            )
+            pio_ct = len(paths_item_object.keys())
+            if pio_ct == 2 or (pio_ct == 3 and 'x-atom-usages' in paths_item_object):
+                paths_item_object['get'] = {'responses': {}}
+        elif self.usages.custom_attr == 'django':
+            paths_item_object = merge_path_objects(
+                paths_item_object, {'get': {'responses': {}}, 'post': {'responses': {}}})
+        return paths_item_object
+
     def _calls_to_params(self, ep: str, orig_ep: str, call: Dict | None) -> Dict[str, Any]:
         """
         Transforms a call and endpoint into a parameter object and organizes it
         into a dictionary based on the call name.
         Args:
             call (dict): The call object
             ep (str): The endpoint
@@ -172,15 +187,15 @@
             call = {}
         ops = {'get', 'put', 'post', 'delete', 'options', 'head', 'patch'}
         call_name = call.get('callName', '')
         params = []
         if call_name in ops:
             params = self._create_param_object(ep, orig_ep, call)
             result: Dict[str, Dict] = {call_name: {'responses': {}}}
-            if params and self.usages.origin_type not in ('js', 'ts', 'javascript', 'typescript'):
+            if params:
                 result[call_name] |= {'parameters': params}
             return result
         return determine_operations(call, params)
 
     def _check_path_elements_regex(self, ele: str) -> Tuple[str, List]:
         """Try to interpret regexes in the path"""
         if '<' in ele:
@@ -250,14 +265,23 @@
         if self.usages.origin_type in ('js', 'ts', 'javascript', 'typescript'):
             ep = js_helper(ep)
         elif self.usages.origin_type in ('py', 'python'):
             ep, tmp_params = py_helper(ep, regex)
             py_special_case = True
         return ep, py_special_case, tmp_params
 
+    def _extract_unparsed_params(
+            self, ep: str, orig_ep: str, py_special_case: bool, tmp_params: List
+    ) -> Tuple[str, List]:
+        if ':' in ep or '<' in ep:
+            ep, py_special_case, tmp_params = self._extract_params(ep)
+        if '{' in ep and not py_special_case:
+            tmp_params = self._generic_params_helper(ep, orig_ep)
+        return ep, tmp_params
+
     def _filter_matches(self, matches: List[str], code: str) -> List[str]:
         """
         Filters a list of matches based on certain criteria.
 
         Args:
             matches (list[str]): A list of matching strings.
             code (str): The code from which to extract endpoints.
@@ -307,16 +331,16 @@
             )
         return params
 
     def _identify_target_line_nums(self, methods: Dict[str, Any]) -> Dict:
         file_names = list(methods['file_names'].keys())
         if not file_names:
             return {}
-        conditional = [f'fileName==`{i}`' for i in file_names]
-        conditional = '*[?' + ' || '.join(conditional) + (  # type: ignore
+        file_names = [f'fileName==`{i}`' for i in file_names]
+        conditional = '*[?' + ' || '.join(file_names) + (
             '][].{file_name: fileName, methods: usages[].targetObj[].{resolved_method: '
             'resolvedMethod || callName || code || name, line_number: lineNumber}}')
         pattern = jmespath.compile(conditional)  # type: ignore
         result = pattern.search(self.usages.content)
         result = {i['file_name']: i['methods'] for i in result if i['methods']}
         targets: Dict = {i: {} for i in result}
 
@@ -337,30 +361,31 @@
         """
         Creates a paths item object.
         """
         paths_item_object: Dict = {}
         tmp_params: List = []
         py_special_case = False
         orig_ep = ep
-        if ':' in ep or '<' in ep:
-            ep, py_special_case, tmp_params = self._extract_params(ep)
-        if '{' in ep and not py_special_case:
-            tmp_params = self._generic_params_helper(ep, orig_ep)
+        ep, tmp_params = self._extract_unparsed_params(ep, orig_ep, py_special_case, tmp_params)
         if tmp_params:
             paths_item_object['parameters'] = tmp_params
         if calls:
             for call in calls:
-                paths_item_object |= self._calls_to_params(ep, orig_ep, call)
+                paths_item_object = merge_path_objects(
+                    paths_item_object, self._calls_to_params(ep, orig_ep, call)
+                )
         if (call_line_numbers or line_number) and (line_nos := create_ln_entries(
                 filename, list(set(call_line_numbers)), line_number)):
             if 'x-atom-usages' in paths_item_object:
                 paths_item_object['x-atom-usages'] = merge_x_atom(
                     paths_item_object['x-atom-usages'], line_nos)
             else:
                 paths_item_object |= line_nos
+        if self.usages.origin_type in ('py', 'python'):
+            paths_item_object = self._add_py_request_methods(paths_item_object)
         return ep, paths_item_object
 
     def _parse_path_regexes(self, endpoint: str) -> str:
         """
         Parses path regexes in the endpoint, extracts params for later use.
         """
         if '(' in endpoint:
@@ -409,15 +434,21 @@
             'objectSlices[].{file_name: fileName, resolved_methods: usages[].*.resolvedMethod[]}')
 
         calls = self._process_methods_helper(
             'objectSlices[].{file_name: fileName, resolved_methods: usages[].*[?resolvedMethod][]'
             '[].resolvedMethod[]}')
 
         user_defined_types = self._process_methods_helper(
-            'userDefinedTypes[].{file_name: name, resolved_methods: fields[].name}')
+            'userDefinedTypes[].{file_name: fileName, resolved_methods: fields[].name}')
+
+        if self.usages.origin_type in ('py', 'python'):
+            user_defined_types = merge_path_objects(
+                user_defined_types,
+                self._process_methods_helper('userDefinedTypes[].{file_name: fileName, '
+                                             'resolved_methods: procedures[].resolvedMethod}'))
 
         for key, value in calls.items():
             if method_map.get(key):
                 method_map[key]['resolved_methods'].extend(value.get('resolved_methods'))
             else:
                 method_map[key] = {'resolved_methods': value.get('resolved_methods')}
 
@@ -450,16 +481,18 @@
                 i for i in matches
                 if i.get('resolved_methods')
             ]
         resolved: Dict = {}
         for r in result:
             file_name = r['file_name']
             methods = r['resolved_methods']
-            resolved.setdefault(file_name, {'resolved_methods': []})[
-                'resolved_methods'].extend(methods)
+            if resolved.get(file_name):
+                resolved[file_name]['resolved_methods'].extend(methods)
+            else:
+                resolved[file_name] = {'resolved_methods': methods}
 
         return resolved
 
     def _process_regex_matches(
             self,
             element: str,
             param_named: bool,
@@ -535,15 +568,20 @@
 
         Returns:
              list: The result of searching for the calls pattern in the usages.
         """
         pattern = (f'objectSlices[?fileName==`{json.dumps(file_name.encode().decode())}`].usages[]'
                    f'.*[?callName][][]')
         compiled_pattern = jmespath.compile(pattern)
-        return compiled_pattern.search(self.usages.content)
+        result = compiled_pattern.search(self.usages.content)
+        pattern = (f'userDefinedTypes[?fileName==`{json.dumps(file_name.encode().decode())}`][].procedures[]')
+        compiled_pattern = jmespath.compile(pattern)
+        result2 = compiled_pattern.search(self.usages.content)
+        result += result2
+        return result
 
 
 def create_ln_entries(filename: str, call_line_numbers: List, line_number: int | None) -> Dict:
     """
     Creates line number entries for a given filename and line numbers.
 
     Args:
@@ -658,15 +696,17 @@
     """
     for key, value in p2.items():
         if key not in p1:
             p1[key] = value
             continue
         for k, v in value.items():
             if p1[key].get(k):
-                if k == 'x-atom-usages':
+                if k == 'resolved_methods':
+                    p1[key][k].extend(v)
+                elif k == 'x-atom-usages':
                     p1[key][k] = merge_x_atom(p1[key][k], v)
                 elif k == 'parameters':
                     p1[key][k] = merge_params(p1[key][k], v)
                 elif k in {'get', 'put', 'post', 'delete', 'options', 'head', 'patch'}:
                     p1[key][k] = merge_operations(p1[key][k], v)
                 continue
             p1[key][k] = v
```

### Comparing `atom-tools-0.4.5/atom_tools/lib/regex_utils.py` & `atom-tools-0.5.0/atom_tools/lib/regex_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import re
 from dataclasses import dataclass
 from typing import Tuple, List, Dict, Any
 
 
 logger: logging.Logger = logging.getLogger(__name__)
+
 py_type_mapping = {'int': 'integer', 'string': 'string', 'float': 'number', 'path': 'string'}
 
 
 @dataclass
 class OpenAPIRegexCollection:
     """
     Collection of regular expressions needed for conversions.
@@ -54,14 +55,28 @@
     single_char_var = re.compile(r'(?<=[(\s])[a-z](?=[\s),.\[])')
     js_import = re.compile(r'import \{ (?P<lib>[\w,\s]+) } from (?P<mod>\S+)')
     js_require_extract = re.compile(r'require\((?P<lib>\S+)\).(?P<mod>\S+)')
     py_func_name = re.compile(r'(?<=\().+?(?=\))')
     py_mod_members = re.compile(r'(?<=:<module>.)(?P<class>[A-Z][^<.]+)?\.?(?P<func>[^<.]+)?')
 
 
+@dataclass
+class FilteringPatternCollection:
+    """
+    A collection of regular expressions used for filtering.
+    """
+    flattened_loc_index = re.compile(r'(?P<type>objectSlices|userDefinedTypes|usages|invokedCalls|argToCalls|fields|procedures).\[(?P<index>\d+)]')
+    top_level_flat_loc_index = re.compile(r'(?P<type>objectSlices|userDefinedTypes).\[(?P<index>\d+)]')
+    attribute_and_line = re.compile(r'(?P<attrib>[^:]+):(?P<line_nums>[\d,-]+)')
+    top_level_filter_usages = (
+        '{objectSlices: objectSlices[?ATTRIBUTECONDITION`TARGET_VALUE`], '
+        'userDefinedTypes: userDefinedTypes[?ATTRIBUTECONDITION`TARGET_VALUE`]}'
+    )
+
+
 def py_helper(endpoint: str, regex: OpenAPIRegexCollection) -> Tuple[str, List[Dict]]:
     """
     Handles Python path parameters.
     Args:
         endpoint (str): The endpoint string
         regex (OpenAPIRegexCollection): The regex collection
```

### Comparing `atom-tools-0.4.5/atom_tools/lib/validator.py` & `atom-tools-0.5.0/atom_tools/lib/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Classes and functions to validate source file line numbers in an atom slice file."""
 
-import json
 import logging
 import os
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Tuple, List, Dict
 
 import jmespath
 
 from atom_tools.lib.slices import AtomSlice
 from atom_tools.lib.regex_utils import ValidationRegexCollection
-
+from atom_tools.lib.utils import export_json, remove_duplicates_list
 
 logger = logging.getLogger(__name__)
 regex: ValidationRegexCollection = ValidationRegexCollection()
 operator_map: Dict[str, List[str]] = {
     '<operator>.addition': ['+'],
     '<operator>.minus': ['-'],
     '<operator>.multiplication': ['*'],
@@ -278,28 +277,14 @@
             if i in line:
                 return True
     if ('__iter__' in function_name or '__next__' in function_name) and 'for ' in line:
         found = True
     return found
 
 
-def remove_duplicates_list(obj: List[Dict]) -> List[Dict]:
-    """Removes duplicates from a list of dictionaries."""
-    if not obj:
-        return obj
-    unique_objs = []
-    seen = set()
-    for o in obj:
-        key = tuple(o.get(k) for k, v in o.items())
-        if key not in seen:
-            unique_objs.append(o)
-            seen.add(key)
-    return unique_objs
-
-
 @dataclass(init=True)
 class LineStats:
     """
     A data class representing statistics for a line validation process.
 
     Attributes:
         close_match_ct (int): Line numbers with matches within interval range.
@@ -437,16 +422,15 @@
             'invalid': {
                 'missing_line_number': self.unverifiable['missing'],
                 'not_found': self.matches['unmatched'],
                 'invalid_line_number': self.unverifiable['range']
             },
             'inaccessible_files': [str(i) for i in self.problem_files]
         }
-        with open(json_report_path, 'w', encoding='utf-8') as f:
-            json.dump(results, f, indent=4)
+        export_json(results, json_report_path, 4)
 
     def find_reachables(self) -> Dict[str, List[Dict[str, str]]]:
         """Collect reachables for analysis."""
         reachables_pattern = jmespath.compile('reachables[].flows[].{function_name: fullName, '
                                               'code: code, file_name: parentFileName, '
                                               'line_number: lineNumber}')
         res = reachables_pattern.search(self.slc.content)
@@ -583,17 +567,14 @@
         elif code.startswith(line) or code.startswith(line.replace('return ', '')):
             found = True
         return found or self._match_by_lang(code, function_name, line)
 
     def _get_verbose_results(self):
         """
         Add the verbose results of the line number validation.
-
-        Args:
-            f: The file object to write the results to.
         """
         verbose_results = '\n*** INVALID ENTRIES ***\n'
         for i in self.matches['unmatched']:
             for k, v in i.items():
                 try:
                     verbose_results += f'{k}: {v}\n'
                 except UnicodeEncodeError:
```

### Comparing `atom-tools-0.4.5/atom_tools.egg-info/SOURCES.txt` & `atom-tools-0.5.0/atom_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 atom_tools/cli/__init__.py
 atom_tools/cli/application.py
 atom_tools/cli/command_loader.py
 atom_tools/cli/logging_config.py
 atom_tools/cli/commands/__init__.py
 atom_tools/cli/commands/command.py
 atom_tools/cli/commands/convert.py
+atom_tools/cli/commands/filter.py
+atom_tools/cli/commands/query_endpoints.py
 atom_tools/cli/commands/validate_lines.py
 atom_tools/lib/__init__.py
 atom_tools/lib/converter.py
+atom_tools/lib/filtering.py
 atom_tools/lib/regex_utils.py
 atom_tools/lib/slices.py
+atom_tools/lib/utils.py
 atom_tools/lib/validator.py
 test/test_converter.py
-test/test_slices.py
+test/test_filtering.py
+test/test_slices.py
+test/test_utils.py
```

### Comparing `atom-tools-0.4.5/pyproject.toml` & `atom-tools-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "atom-tools"
-version = "0.4.5"
+version = "0.5.0"
 description = "Collection of tools for use with AppThreat/atom."
 authors = [
   { name = "Caroline Russell", email = "caroline@appthreat.dev" },
 ]
-dependencies = ["cleo>=1.0.0", "jmespath>=1.0.0"]
+dependencies = ["cleo>=1.0.0", "jmespath>=1.0.0", "thefuzz>=0.22.1", "json-flatten>=0.3"]
 license = { text = "Apache-2.0" }
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
```

### Comparing `atom-tools-0.4.5/test/test_slices.py` & `atom-tools-0.5.0/test/test_slices.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,13 +37,7 @@
         java_usages_2,
 ):
     usages = AtomSlice('test/data/java-piggymetrics-usages.json', 'java')
     assert usages.content is not None
 
     usages = AtomSlice('test/data/java-sec-code-usages.json', 'java')
     assert usages.content is not None
-
-
-def test_import_slices(js_usages_1):
-
-    # Test invalid JSON file
-    assert AtomSlice('test/data/invalid.json', 'js').content == {}
```

