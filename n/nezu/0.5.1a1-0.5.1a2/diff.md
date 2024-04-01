# Comparing `tmp/nezu-0.5.1a1.tar.gz` & `tmp/nezu-0.5.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nezu-0.5.1a1.tar", max compression
+gzip compressed data, was "nezu-0.5.1a2.tar", max compression
```

## Comparing `nezu-0.5.1a1.tar` & `nezu-0.5.1a2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1075 2024-03-11 08:02:14.874055 nezu-0.5.1a1/LICENSE
--rw-r--r--   0        0        0       39 2024-04-01 07:28:02.200311 nezu-0.5.1a1/nezu/__init__.py
--rw-r--r--   0        0        0      454 2024-03-11 08:02:14.885369 nezu-0.5.1a1/nezu/_os_env.py
--rw-r--r--   0        0        0     2338 2024-04-01 06:55:47.336097 nezu-0.5.1a1/nezu/_parse.py
--rw-r--r--   0        0        0       24 2024-03-17 09:38:35.872995 nezu-0.5.1a1/nezu/manual_tests/__init__.py
--rw-r--r--   0        0        0      315 2024-04-01 08:27:32.386391 nezu-0.5.1a1/nezu/manual_tests/ztest_example.py
--rw-r--r--   0        0        0      146 2024-04-01 08:29:08.085862 nezu-0.5.1a1/nezu/manual_tests/ztest_hide.py
--rw-r--r--   0        0        0      507 2024-04-01 08:29:05.537093 nezu-0.5.1a1/nezu/manual_tests/ztest_nez.py
--rw-r--r--   0        0        0       83 2024-03-17 09:38:35.994840 nezu-0.5.1a1/nezu/manual_tests/ztest_parsing.py
--rw-r--r--   0        0        0       66 2024-04-01 08:25:39.529084 nezu-0.5.1a1/nezu/manual_tests/ztest_say.py
--rw-r--r--   0        0        0       68 2024-04-01 08:26:07.063144 nezu-0.5.1a1/nezu/manual_tests/ztest_say_color.py
--rw-r--r--   0        0        0       53 2024-04-01 08:25:00.835656 nezu-0.5.1a1/nezu/manual_tests/ztest_simple.py
--rw-r--r--   0        0        0       25 2024-03-17 08:53:08.194594 nezu-0.5.1a1/nezu/nezu.json
--rw-r--r--   0        0        0     5715 2024-04-01 08:31:24.254490 nezu-0.5.1a1/nezu/nezu.py
--rw-r--r--   0        0        0        0 2024-03-11 08:02:14.883332 nezu-0.5.1a1/nezu/parts/__init__.py
--rw-r--r--   0        0        0       54 2024-03-17 09:38:35.879504 nezu-0.5.1a1/nezu/parts/cli.py
--rw-r--r--   0        0        0    11605 2024-03-11 08:02:14.886438 nezu-0.5.1a1/nezu/poetry.lock
--rw-r--r--   0        0        0        0 2024-03-11 08:02:14.886438 nezu-0.5.1a1/nezu/tests/__init__.py
--rw-r--r--   0        0        0      244 2024-04-01 08:05:00.183892 nezu-0.5.1a1/nezu/tests/test_class.py
--rw-r--r--   0        0        0     1038 2024-03-17 08:32:01.994393 nezu-0.5.1a1/nezu/tests/test_config.py
--rw-r--r--   0        0        0     3424 2024-04-01 07:51:02.591766 nezu-0.5.1a1/nezu/tests/test_dbg.py
--rw-r--r--   0        0        0      332 2024-04-01 07:50:08.180218 nezu-0.5.1a1/nezu/tests/test_line_checker.py
--rw-r--r--   0        0        0      560 2024-04-01 08:22:18.141723 nezu-0.5.1a1/nezu/tests/test_say.py
--rw-r--r--   0        0        0      686 2024-04-01 08:49:32.823998 nezu-0.5.1a1/pyproject.toml
--rw-r--r--   0        0        0     6562 2024-04-01 07:53:33.796126 nezu-0.5.1a1/README.md
--rw-r--r--   0        0        0     6904 1970-01-01 00:00:00.000000 nezu-0.5.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-11 08:02:14.874055 nezu-0.5.1a2/LICENSE
+-rw-r--r--   0        0        0       39 2024-04-01 07:28:02.200311 nezu-0.5.1a2/nezu/__init__.py
+-rw-r--r--   0        0        0      454 2024-03-11 08:02:14.885369 nezu-0.5.1a2/nezu/_os_env.py
+-rw-r--r--   0        0        0     3145 2024-04-01 19:45:05.344512 nezu-0.5.1a2/nezu/_parse.py
+-rw-r--r--   0        0        0       24 2024-03-17 09:38:35.872995 nezu-0.5.1a2/nezu/manual_tests/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-01 13:22:39.100782 nezu-0.5.1a2/nezu/manual_tests/bps.py
+-rw-r--r--   0        0        0      324 2024-04-01 19:16:17.289405 nezu-0.5.1a2/nezu/manual_tests/example.py
+-rw-r--r--   0        0        0      193 2024-04-01 19:53:07.442758 nezu-0.5.1a2/nezu/manual_tests/multiline.py
+-rw-r--r--   0        0        0      146 2024-04-01 08:29:08.085862 nezu-0.5.1a2/nezu/manual_tests/ztest_hide.py
+-rw-r--r--   0        0        0      507 2024-04-01 08:29:05.537093 nezu-0.5.1a2/nezu/manual_tests/ztest_nez.py
+-rw-r--r--   0        0        0       83 2024-04-01 08:50:45.119324 nezu-0.5.1a2/nezu/manual_tests/ztest_parsing.py
+-rw-r--r--   0        0        0       66 2024-04-01 08:25:39.529084 nezu-0.5.1a2/nezu/manual_tests/ztest_say.py
+-rw-r--r--   0        0        0       68 2024-04-01 08:26:07.063144 nezu-0.5.1a2/nezu/manual_tests/ztest_say_color.py
+-rw-r--r--   0        0        0       53 2024-04-01 08:25:00.835656 nezu-0.5.1a2/nezu/manual_tests/ztest_simple.py
+-rw-r--r--   0        0        0       25 2024-03-17 08:53:08.194594 nezu-0.5.1a2/nezu/nezu.json
+-rw-r--r--   0        0        0     7147 2024-04-01 19:27:01.074978 nezu-0.5.1a2/nezu/nezu.py
+-rw-r--r--   0        0        0        0 2024-03-11 08:02:14.883332 nezu-0.5.1a2/nezu/parts/__init__.py
+-rw-r--r--   0        0        0       54 2024-03-17 09:38:35.879504 nezu-0.5.1a2/nezu/parts/cli.py
+-rw-r--r--   0        0        0    11605 2024-03-11 08:02:14.886438 nezu-0.5.1a2/nezu/poetry.lock
+-rw-r--r--   0        0        0        0 2024-03-11 08:02:14.886438 nezu-0.5.1a2/nezu/tests/__init__.py
+-rw-r--r--   0        0        0      280 2024-04-01 13:09:20.092802 nezu-0.5.1a2/nezu/tests/test_class.py
+-rw-r--r--   0        0        0     1116 2024-04-01 13:19:00.511958 nezu-0.5.1a2/nezu/tests/test_config.py
+-rw-r--r--   0        0        0     3430 2024-04-01 19:51:28.360512 nezu-0.5.1a2/nezu/tests/test_dbg.py
+-rw-r--r--   0        0        0      332 2024-04-01 07:50:08.180218 nezu-0.5.1a2/nezu/tests/test_line_checker.py
+-rw-r--r--   0        0        0      566 2024-04-01 12:43:16.174449 nezu-0.5.1a2/nezu/tests/test_say.py
+-rw-r--r--   0        0        0      686 2024-04-01 19:55:42.082981 nezu-0.5.1a2/pyproject.toml
+-rw-r--r--   0        0        0     8923 2024-04-01 14:56:32.304174 nezu-0.5.1a2/README.md
+-rw-r--r--   0        0        0     9265 1970-01-01 00:00:00.000000 nezu-0.5.1a2/PKG-INFO
```

### Comparing `nezu-0.5.1a1/LICENSE` & `nezu-0.5.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nezu-0.5.1a1/nezu/_parse.py` & `nezu-0.5.1a2/nezu/_parse.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,50 @@
         i = long_str.index(']')
     else:
         i = 0
     key = long_str[:i] if i else long_str
 
     return key
 
+def parse_desc(_type, val, key):
+    if _type == 'function' and val.__doc__:
+        # _desc = (
+        #     f'{val.__doc__}'[:40] + '...'
+        #     if len(val.__doc__) > 43
+        #     else val.__doc__
+        # )
+        _desc = val.__doc__
+    elif _type == 'function':
+        _desc = 'No docstring'
+    else:
+        _desc = str(val)
+    
+    cut_lines = '\n'+' '*12
+    if '\n' in _desc:
+        l = _desc.split('\n')
+        for line in l:
+            while len(line)>80:
+                cut_lines += line[0:80] + '\n'+' '*12
+                line = line[80:]
+            else:
+                cut_lines += line +'\n'+' '*12
+    elif len(_desc)+len(_type)+len(key)>80-7:
+        print(len(_desc))
+        print(len(_type))
+        print(len(key))
+        while len(_desc)>80:
+            print(len(_desc))
+            cut_lines += _desc[0:80] + '\n'+' '*12
+            _desc = _desc[80:]
+        else:
+            cut_lines += _desc
+    else:
+        cut_lines = _desc
+    return cut_lines
+    
 
 def get_output(loc, glob, bins, long_str, color):
     # from .name_parser import parse_name
 
     is_undefined = False
     key = parse_name(long_str)
     _sep0 = ' '
@@ -63,23 +99,15 @@
     if is_undefined:
         _src = '...'
         _val = ''
         _type = ''
         _sep1 = ''
         _sep2 = ''
 
-    if _type == 'function' and _val.__doc__:
-        _desc = (
-            f'{_val.__doc__}'[:40] + '...'
-            if len(_val.__doc__) > 43
-            else _val.__doc__
-        )
-    elif _type == 'function':
-        _desc = 'No docstring'
-    else:
-        _desc = _val
+    _desc = parse_desc(_type,_val, long_str)
+
 
     return (
         f'\u001b[36m{_src}\u001b[35m{_sep0}\u001b[0m{long_str}\u001b[35m{_sep1}\u001b[31m{_type}\u001b[35m{_sep2}\u001b[33m{_desc}\u001b[0m'
         if color
         else f'{_src}{_sep0}{long_str}{_sep1}{_type}{_sep2}{_desc}'
     )
```

### Comparing `nezu-0.5.1a1/nezu/poetry.lock` & `nezu-0.5.1a2/nezu/poetry.lock`

 * *Files identical despite different names*

### Comparing `nezu-0.5.1a1/nezu/tests/test_config.py` & `nezu-0.5.1a2/nezu/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from nezu.nezu import real_nezu
 from os import environ as env
 
 
 def test_no_config():
     env['NEZU_SEEK'] = '0'
     env['NEZU_COLOR'] = '0'
+    env['NEZU_FLOW'] = '5'
     nezu = real_nezu()
-    assert dict(nezu) == {'id': 'nezu', 'seek': 0, 'color': False}
+    assert dict(nezu) == {'id': 'nezu', 'seek': 0, 'flow':5, 'color': False}
 
 
 def test_hard_config_seek():
     nezu = real_nezu()
     nezu(seek=1)
-    assert dict(nezu) == {'id': 'nezu', 'seek': 1, 'color': False}
+    assert dict(nezu) == {'id': 'nezu', 'seek': 1, 'flow':5, 'color': False}
 
 
 def test_hard_config_color():
     nezu = real_nezu()
     nezu(color=True)
-    assert dict(nezu) == {'id': 'nezu', 'seek': 0, 'color': True}
+    assert dict(nezu) == {'id': 'nezu', 'seek': 0, 'flow':5, 'color': True}
 
 
 def test_json_config_seek():
     content = '{"nezu":{"seek":1}}'
     with open('nezu.json', 'w') as f:
         print(content, file=f)
     nezu = real_nezu()
     nezu.json()
-    assert dict(nezu) == {'id': 'nezu', 'seek': 1, 'color': False}
+    assert dict(nezu) == {'id': 'nezu', 'seek': 1, 'flow':5, 'color': False}
 
 
 def test_json_config_color():
     content = '{"nezu":{"color":true}}'
     with open('nezu.json', 'w') as f:
         print(content, file=f)
     nezu = real_nezu()
     nezu.json()
-    assert dict(nezu) == {'id': 'nezu', 'seek': 0, 'color': True}
+    assert dict(nezu) == {'id': 'nezu', 'seek': 0, 'flow':5, 'color': True}
```

### Comparing `nezu-0.5.1a1/nezu/tests/test_dbg.py` & `nezu-0.5.1a2/nezu/tests/test_dbg.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         nezu.dbg('i', hide=i)
         said = capsys.readouterr().out
         assert said[8:-1] == lis[i]
 
 
 def test_color(capsys):
     nezu = real_nezu()
-    nezu(1, True)
+    nezu(1, color=True)
     biggus = 'dickus'
     nezu.dbg('biggus')
     said = capsys.readouterr().out
     expected = f'\u001b[36mL..\u001b[35m \u001b[0mbiggus\u001b[35m:\u001b[31mstr\u001b[35m  =>  \u001b[33mdickus\u001b[0m'
     assert said[8:-1] == expected
 
 
@@ -148,12 +148,12 @@
     nezu = real_nezu()
     nezu(1)
     biggus = 'BIGGUS'
     dickus = 'DICKUS'
     nezu.dbg('biggus', 'dickus')
     said = capsys.readouterr().out
     a, b, c, d, _ = said.split('\n')
-    assert a[8:] == '-' * 70
+    assert a[8:] == '-' * 84
     assert b[8:] == f'L.. biggus:str  =>  BIGGUS'
     assert c[8:] == f'L.. dickus:str  =>  DICKUS'
-    assert d[8:] == '-' * 70
+    assert d[8:] == '-' * 84
     # assert said == ''
```

### Comparing `nezu-0.5.1a1/nezu/tests/test_say.py` & `nezu-0.5.1a2/nezu/tests/test_say.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     for i in range(5):
         nezu.say(f'--{i}--', hide=i)
         said = capsys.readouterr().out
         assert said[8:-1] == lis[i]
 
 def test_color(capsys):
     nezu = real_nezu()
-    nezu(1, True)
+    nezu(1, color=True)
     biggus = 'dickus'
     nezu.say(biggus)
     said = capsys.readouterr().out
     expected = f'\033[92mdickus\033[0m'
     assert said[8:-1] == expected
```

### Comparing `nezu-0.5.1a1/pyproject.toml` & `nezu-0.5.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nezu"
-version = "0.5.1-alpha.1"
+version = "0.5.1-alpha.2"
 description = "Elegant debuging module"
 authors = ["Chuck Cartwright"]
 license = "MIT"
 readme = "README.md"
 packages =[
     # { include = "_os_env.py" },
     # { include = "_parse.py" },
```

### Comparing `nezu-0.5.1a1/README.md` & `nezu-0.5.1a2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 ### Table of Contents
 
 [NEZU](#nezu)
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Output Interpretation](#output-interpretation)
+  - [Debuf Interpretation](#debug-interpretation)
   - [Function dbg](#function-dbg)
+  - [Function say](#function-say)
 - [Config](#config)
   - [Env Vars Config](#env-vars-config)
   - [JSON Config](#json-config)
   - [Hardcoded Config](#hardcoded-config)
 - [Coloring output](#coloring-output)
 - [Hiding output](#hiding-output)
 
@@ -59,114 +60,166 @@
 
   ```bash
   python -m poetry add nezu
   ```
 
 ### Usage
 
-- Inspect variable using [function dbg](#function-dbg) in your code.
-- [Configure](#config) Nezu to show output.
-- [Interpret](#output-interpretation) output and debug.
-
-#### Output Interpretation
-
-```
-@7 ..B print:function  =>  Prints the values to a stream, or to sys...
- │ │   │     │             │
- │ │   │     │             └─ Value of inspected variable
- │ │   │     │
- │ │   │     └─────────────── Type of inspected variable.
- │ │   │
- │ │   └───────────────────── Name of inspected variable.
- │ │
- │ └───────────────────────── Scope of inspected variable (see bollow).
- |
- └─────────────────────────── Line number of inspection.
-```
+- Inspect variables with [function `dbg`](#function-dbg).
+- Display literals with [function `say`](#function-say).
+- [Configure Nezu](#config) to show output.
+- [Interpret output](#debug-interpretation).
+- Fix bugs.
+
+#### Debug Interpretation
+Using debbuging function `dbg` will display something like:
+- **_Example output_**
+  ```
+  @7 ..B print:function  =>  Prints the values to a stream, or to sys...
+  ```
+- **_Interpretation_**
+  ```
+  @7 ..B print:function  =>  Prints the values to a stream, or to sys...
+  │ │   │     │             │
+  │ │   │     │             └─ Value of inspected variable
+  │ │   │     │
+  │ │   │     └─────────────── Type of inspected variable.
+  │ │   │
+  │ │   └───────────────────── Name of inspected variable.
+  │ │
+  │ └───────────────────────── Scope of inspected variable (see bollow).
+  |
+  └─────────────────────────── Line number of inspection.
+  ```
 
 - **_Scope codes_**
   - `L..` - local scope, no shadowing
   - `Lg.` - local scope, shadowing global
   - `L.b` - local scope, shadowing built-in
   - `Lgb` - local scope, shadowing global and built-in
   - `.G.` - Global scope, no shadowing
   - `.Gb` - Global scope, shadowing built-in
   - `..B` - Built-in scope, no shadowing
   - `...` - Undefined 
 
 #### Function `dbg`
 
-Inspect scopes and values of given keys (variable names etc.).
+To debug, use funtion `dbg`, it will inspect scopes and values of given keys (variable names etc.).
 
 - **_Args_**
 
   - `*keys:str`
 
     Names of variables to inspect
 
-  - `note:str = None`
+  - `hide:int = 1`
+
+    This argument is compared with `Nezu.seek`.
+    If `Nezu.seek >= hide` this debug inspection will be displayed.
+
+
+  - `bp:int = 0`
+
+    This argument is compared with `Nezu.flow`.
+    If `Nezu.flow < bp` this debug inspection will be considered breakpoint.
+
+- **_Python Code Example_**
+
+  ```py
+  # file.py
+  from nezu import dbg
+
+  nortius = 3
+  maximus = int()
+  biggus = {'dickus':'sillius'}
+
+  dbg('nortius')          # Works on simple variables.
+  dbg('maximus.real')     # Works on attributes.
+  dbg('print')            # Works on functions and built-ins.
+  dbg('biggus["dickus"]') # DOES NOT work on keys and indexes yet.
+  ```
+
+- **_Note_**
+
+  Output of `dbg` function is hidden by default. If you want to see dbg you need to configure env var `NEZU_SEEK` with value of `1` or more.
+
+#### Function `say`
+
+Simple literal output.
+
+- **_Args_**
+
+  - `*val`
 
-    Optional comment. Ignored if equal to None.
+    Value to display.
 
   - `hide:int = 1`
 
     This argument is compared with `nezu.seek`.
-    If `nezu.seek >= hide` this debug inspection will be displayed.
-    If hide <= 0, this message will be displayed by default.
+    If `nezu.seek >= hide` this call will be displayed.
+
+  - `bp:int = 0`
+
+    This argument is compared with `Nezu.flow`.
+    If `Nezu.flow < bp` this call will be considered breakpoint.
 
 - **_Python Code Example_**
 
   ```py
   # file.py
-  from nezu import dbg
+  from nezu import say
+
+  biggus = 'dickus'
+
+  say('biggus') # displays something like `      @5 biggus`
+  say(biggus)   # displays something like `      @6 dickus`
 
-  egg = 3
-  ham = int()
-  spam = {'spam':'bacon'}
-
-  dbg('egg')          # Works on simple variables.
-  dbg('ham.real')     # Works on attributes.
-  dbg('print')        # Works on functions and built-ins.
-  dbg('spam["spam"]') # DOES NOT work on keys and indexes yet.
   ```
 
 - **_Note_**
 
   Output of `dbg` function is hidden by default. If you want to see dbg you need to configure env var `NEZU_SEEK` with value of `1` or more.
 
 ### Config
 
 Module `nezu` creates `nezu` object that has config attributes used by function `dbg`.
 
 - **_Attributes_**
   - `nezu.seek:int = 0`
+
     Compared to `dbg` argument`hide`, if `nezu.seek >= hide` then `dbg` will be printed.
+
   - `nezu.color:bool = False`
+
     Determines if output of `dbg` function should be colored.
+
   - `nezu.lock:bool = False`
+
     If `nezu.lock = True`, this config cannot be changed later, during runtime.
 
 #### Env Vars Config
 
 If you want to use default config method, change your _env vars_ in terminal and run Python script.
 
 - **_Bash_**
 
   ```bash
   export NEZU_SEEK=1
+  export NEZU_FLOW=5
   export NEZU_COLOR=1
   export NEZU_LOCK=0
   python file.py
   ```
 
 - **_PowerShell_**
   ```powershell
   $env:NEZU_SEEK = 1
+  $env:NEZU_FLOW = 5
   $env:NEZU_COLOR = $True
-  $env:NEZU_LOCK = $True
+  $env:NEZU_LOCK = $False
   python file.py
   ```
 
 #### JSON Config
 
 If you don't want to use _env vars_ as config, you can call `nezu.json()` to read config data from json file.
 It will search for key `nezu` inside chosen file.
@@ -183,38 +236,52 @@
   ```
 
 - **_Example Config File_**
 
   ```json
   "nezu": {
     "seek": 1,
+    "flow": 5,
     "color": true,
     "locked": false
   }
   ```
 
 ---
 
 #### Hardcoded Config
 
 If you don't want to use _env vars_ as config you can also call object `nezu` like function to make hardcoded config.
 
 - **_Args_**
 
-  - `seek:int = 0` - debug level
-  - `color:bool = False` - output coloring
-  - `lock:bool = False` - lock this config
+  - `seek:int = 0`
+
+    Debug level
+
+  - `flow:int = 5` 
+
+    Skipping breakpoits
+
+  - `color:bool = False`
+
+    Output coloring
+
+  - `lock:bool = False` 
+
+    Lock this config
+
 
 - **_Example_**
 
   ```py
   # file.py
   from nezu import nezu, dbg
 
-  nezu(1, True, False)
+  nezu(1, 7, True, False)
   ...
   ```
 
 - **_Tip_**
 
   There is no built-in support for _yaml_, _toml_ or _.env_ in _nezu_
   This is so _nezu_ can stay free of dependencies.
@@ -254,49 +321,110 @@
 
   nezu(color = True)
   ...
   ```
 
 ### Hiding Output
 
-Function `dbg()` can be hidden more by `hide` parameter. By default only `dbg` calls with `hide <= nezu.seek` will be printed. In examples bellow only `dbg` hidden up to level 3 are displayed.
+Functions `dbg()` and `say()` can be hidden more by `hide` parameter. By default only calls with `hide <= nezu.seek` will be printed. In examples bellow only `dbg` hidden up to level 3 are displayed.
 
 - **_Python Code Example_**
 
   ```python
   #file.py
-  from nezu import dbg
+  from nezu import say
 
-  dbg('egg', hide=1)
-  dbg('ham', hide=2)
-  dbg('spam', hide=3)
-  dbg('bacon', hide=4)
-  dbg('lobster', hide=5)
+  say('biggus', hide=1)
+  say('dickus', hide=2)
+  say('nortius', hide=3)
+  say('maximus', hide=4)
+  say('sillius', hide=5)
+  say('soddus', hide=6)
   ```
 
 - **_Bash Example_**
 
   ```bash
   export NEZU_SEEK=3
   python file.py
-        @4 ... egg
-        @5 ... ham
-        @6 ... spam
+        @4 biggus
+        @5 dickus
+        @6 nortius
   ```
 
 - **_PowerShell Example_**
 
   ```powershell
   $ENV:NEZU_SEEK = 3
   python file.py
-        @4 ... egg
-        @5 ... ham
-        @6 ... spam
+        @4 biggus
+        @5 dickus
+        @6 nortius
   ```
 
 - **_JSON File Example_**
 
   ```json
   "nezu": {
-      "seek": 3
+      "seek": 3,
   }
   ```
+- **_Example Hardcoded Config_**
+
+  ```py
+  from nezu import nezu, dbg
+
+  nezu(3)
+  ...
+  ```
+### Breakpoints
+
+Functions `dbg()` and `say()` can be used as breakpoints by `bp` parameter. Calls with `bp > nezu.flow` will stop program execution. Hidden calls are never considered brerakpoints. In examples bellow only second call will behave as breakpoint.
+
+- **_Python Code Example_**
+
+  ```python
+  #file.py
+  from nezu import dbg
+
+  say('biggus' bp=6)
+  say('dickus', bp=7)
+  say('nortius', hide=2, bp=8)
+  ```
+
+- **_Bash Example_**
+
+  ```bash
+  export NEZU_SEEK=1
+  export NEZU_FLOW=6
+  python file.py
+        @4 biggus
+        @5 dickus   # Program stop execution until user press Enter
+        @6 nortius
+  ```
+
+- **_PowerShell Example_**
+
+  ```powershell
+  $ENV:NEZU_SEEK = 1
+  $ENV:NEZU_FLOW = 6
+  python file.py
+        @4 biggus
+        @5 dickus   # Program stop execution until user press Enter
+        @6 nortius
+  ```
+
+- **_JSON File Example_**
+
+  ```json
+  "nezu": {
+      "flow": 6,
+  }
+  ```
+- **_Example Hardcoded Config_**
+
+  ```py
+  from nezu import nezu, dbg
+
+  nezu(flow = 6)
+  ...
+  ```
```

### Comparing `nezu-0.5.1a1/PKG-INFO` & `nezu-0.5.1a2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nezu
-Version: 0.5.1a1
+Version: 0.5.1a2
 Summary: Elegant debuging module
 License: MIT
 Author: Chuck Cartwright
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -46,16 +46,17 @@
 ### Table of Contents
 
 [NEZU](#nezu)
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Output Interpretation](#output-interpretation)
+  - [Debuf Interpretation](#debug-interpretation)
   - [Function dbg](#function-dbg)
+  - [Function say](#function-say)
 - [Config](#config)
   - [Env Vars Config](#env-vars-config)
   - [JSON Config](#json-config)
   - [Hardcoded Config](#hardcoded-config)
 - [Coloring output](#coloring-output)
 - [Hiding output](#hiding-output)
 
@@ -71,114 +72,166 @@
 
   ```bash
   python -m poetry add nezu
   ```
 
 ### Usage
 
-- Inspect variable using [function dbg](#function-dbg) in your code.
-- [Configure](#config) Nezu to show output.
-- [Interpret](#output-interpretation) output and debug.
-
-#### Output Interpretation
-
-```
-@7 ..B print:function  =>  Prints the values to a stream, or to sys...
- │ │   │     │             │
- │ │   │     │             └─ Value of inspected variable
- │ │   │     │
- │ │   │     └─────────────── Type of inspected variable.
- │ │   │
- │ │   └───────────────────── Name of inspected variable.
- │ │
- │ └───────────────────────── Scope of inspected variable (see bollow).
- |
- └─────────────────────────── Line number of inspection.
-```
+- Inspect variables with [function `dbg`](#function-dbg).
+- Display literals with [function `say`](#function-say).
+- [Configure Nezu](#config) to show output.
+- [Interpret output](#debug-interpretation).
+- Fix bugs.
+
+#### Debug Interpretation
+Using debbuging function `dbg` will display something like:
+- **_Example output_**
+  ```
+  @7 ..B print:function  =>  Prints the values to a stream, or to sys...
+  ```
+- **_Interpretation_**
+  ```
+  @7 ..B print:function  =>  Prints the values to a stream, or to sys...
+  │ │   │     │             │
+  │ │   │     │             └─ Value of inspected variable
+  │ │   │     │
+  │ │   │     └─────────────── Type of inspected variable.
+  │ │   │
+  │ │   └───────────────────── Name of inspected variable.
+  │ │
+  │ └───────────────────────── Scope of inspected variable (see bollow).
+  |
+  └─────────────────────────── Line number of inspection.
+  ```
 
 - **_Scope codes_**
   - `L..` - local scope, no shadowing
   - `Lg.` - local scope, shadowing global
   - `L.b` - local scope, shadowing built-in
   - `Lgb` - local scope, shadowing global and built-in
   - `.G.` - Global scope, no shadowing
   - `.Gb` - Global scope, shadowing built-in
   - `..B` - Built-in scope, no shadowing
   - `...` - Undefined 
 
 #### Function `dbg`
 
-Inspect scopes and values of given keys (variable names etc.).
+To debug, use funtion `dbg`, it will inspect scopes and values of given keys (variable names etc.).
 
 - **_Args_**
 
   - `*keys:str`
 
     Names of variables to inspect
 
-  - `note:str = None`
+  - `hide:int = 1`
+
+    This argument is compared with `Nezu.seek`.
+    If `Nezu.seek >= hide` this debug inspection will be displayed.
+
+
+  - `bp:int = 0`
+
+    This argument is compared with `Nezu.flow`.
+    If `Nezu.flow < bp` this debug inspection will be considered breakpoint.
+
+- **_Python Code Example_**
+
+  ```py
+  # file.py
+  from nezu import dbg
+
+  nortius = 3
+  maximus = int()
+  biggus = {'dickus':'sillius'}
+
+  dbg('nortius')          # Works on simple variables.
+  dbg('maximus.real')     # Works on attributes.
+  dbg('print')            # Works on functions and built-ins.
+  dbg('biggus["dickus"]') # DOES NOT work on keys and indexes yet.
+  ```
+
+- **_Note_**
+
+  Output of `dbg` function is hidden by default. If you want to see dbg you need to configure env var `NEZU_SEEK` with value of `1` or more.
+
+#### Function `say`
+
+Simple literal output.
+
+- **_Args_**
+
+  - `*val`
 
-    Optional comment. Ignored if equal to None.
+    Value to display.
 
   - `hide:int = 1`
 
     This argument is compared with `nezu.seek`.
-    If `nezu.seek >= hide` this debug inspection will be displayed.
-    If hide <= 0, this message will be displayed by default.
+    If `nezu.seek >= hide` this call will be displayed.
+
+  - `bp:int = 0`
+
+    This argument is compared with `Nezu.flow`.
+    If `Nezu.flow < bp` this call will be considered breakpoint.
 
 - **_Python Code Example_**
 
   ```py
   # file.py
-  from nezu import dbg
+  from nezu import say
+
+  biggus = 'dickus'
+
+  say('biggus') # displays something like `      @5 biggus`
+  say(biggus)   # displays something like `      @6 dickus`
 
-  egg = 3
-  ham = int()
-  spam = {'spam':'bacon'}
-
-  dbg('egg')          # Works on simple variables.
-  dbg('ham.real')     # Works on attributes.
-  dbg('print')        # Works on functions and built-ins.
-  dbg('spam["spam"]') # DOES NOT work on keys and indexes yet.
   ```
 
 - **_Note_**
 
   Output of `dbg` function is hidden by default. If you want to see dbg you need to configure env var `NEZU_SEEK` with value of `1` or more.
 
 ### Config
 
 Module `nezu` creates `nezu` object that has config attributes used by function `dbg`.
 
 - **_Attributes_**
   - `nezu.seek:int = 0`
+
     Compared to `dbg` argument`hide`, if `nezu.seek >= hide` then `dbg` will be printed.
+
   - `nezu.color:bool = False`
+
     Determines if output of `dbg` function should be colored.
+
   - `nezu.lock:bool = False`
+
     If `nezu.lock = True`, this config cannot be changed later, during runtime.
 
 #### Env Vars Config
 
 If you want to use default config method, change your _env vars_ in terminal and run Python script.
 
 - **_Bash_**
 
   ```bash
   export NEZU_SEEK=1
+  export NEZU_FLOW=5
   export NEZU_COLOR=1
   export NEZU_LOCK=0
   python file.py
   ```
 
 - **_PowerShell_**
   ```powershell
   $env:NEZU_SEEK = 1
+  $env:NEZU_FLOW = 5
   $env:NEZU_COLOR = $True
-  $env:NEZU_LOCK = $True
+  $env:NEZU_LOCK = $False
   python file.py
   ```
 
 #### JSON Config
 
 If you don't want to use _env vars_ as config, you can call `nezu.json()` to read config data from json file.
 It will search for key `nezu` inside chosen file.
@@ -195,38 +248,52 @@
   ```
 
 - **_Example Config File_**
 
   ```json
   "nezu": {
     "seek": 1,
+    "flow": 5,
     "color": true,
     "locked": false
   }
   ```
 
 ---
 
 #### Hardcoded Config
 
 If you don't want to use _env vars_ as config you can also call object `nezu` like function to make hardcoded config.
 
 - **_Args_**
 
-  - `seek:int = 0` - debug level
-  - `color:bool = False` - output coloring
-  - `lock:bool = False` - lock this config
+  - `seek:int = 0`
+
+    Debug level
+
+  - `flow:int = 5` 
+
+    Skipping breakpoits
+
+  - `color:bool = False`
+
+    Output coloring
+
+  - `lock:bool = False` 
+
+    Lock this config
+
 
 - **_Example_**
 
   ```py
   # file.py
   from nezu import nezu, dbg
 
-  nezu(1, True, False)
+  nezu(1, 7, True, False)
   ...
   ```
 
 - **_Tip_**
 
   There is no built-in support for _yaml_, _toml_ or _.env_ in _nezu_
   This is so _nezu_ can stay free of dependencies.
@@ -266,50 +333,110 @@
 
   nezu(color = True)
   ...
   ```
 
 ### Hiding Output
 
-Function `dbg()` can be hidden more by `hide` parameter. By default only `dbg` calls with `hide <= nezu.seek` will be printed. In examples bellow only `dbg` hidden up to level 3 are displayed.
+Functions `dbg()` and `say()` can be hidden more by `hide` parameter. By default only calls with `hide <= nezu.seek` will be printed. In examples bellow only `dbg` hidden up to level 3 are displayed.
 
 - **_Python Code Example_**
 
   ```python
   #file.py
-  from nezu import dbg
+  from nezu import say
 
-  dbg('egg', hide=1)
-  dbg('ham', hide=2)
-  dbg('spam', hide=3)
-  dbg('bacon', hide=4)
-  dbg('lobster', hide=5)
+  say('biggus', hide=1)
+  say('dickus', hide=2)
+  say('nortius', hide=3)
+  say('maximus', hide=4)
+  say('sillius', hide=5)
+  say('soddus', hide=6)
   ```
 
 - **_Bash Example_**
 
   ```bash
   export NEZU_SEEK=3
   python file.py
-        @4 ... egg
-        @5 ... ham
-        @6 ... spam
+        @4 biggus
+        @5 dickus
+        @6 nortius
   ```
 
 - **_PowerShell Example_**
 
   ```powershell
   $ENV:NEZU_SEEK = 3
   python file.py
-        @4 ... egg
-        @5 ... ham
-        @6 ... spam
+        @4 biggus
+        @5 dickus
+        @6 nortius
   ```
 
 - **_JSON File Example_**
 
   ```json
   "nezu": {
-      "seek": 3
+      "seek": 3,
   }
   ```
+- **_Example Hardcoded Config_**
+
+  ```py
+  from nezu import nezu, dbg
+
+  nezu(3)
+  ...
+  ```
+### Breakpoints
+
+Functions `dbg()` and `say()` can be used as breakpoints by `bp` parameter. Calls with `bp > nezu.flow` will stop program execution. Hidden calls are never considered brerakpoints. In examples bellow only second call will behave as breakpoint.
+
+- **_Python Code Example_**
+
+  ```python
+  #file.py
+  from nezu import dbg
+
+  say('biggus' bp=6)
+  say('dickus', bp=7)
+  say('nortius', hide=2, bp=8)
+  ```
+
+- **_Bash Example_**
+
+  ```bash
+  export NEZU_SEEK=1
+  export NEZU_FLOW=6
+  python file.py
+        @4 biggus
+        @5 dickus   # Program stop execution until user press Enter
+        @6 nortius
+  ```
+
+- **_PowerShell Example_**
 
+  ```powershell
+  $ENV:NEZU_SEEK = 1
+  $ENV:NEZU_FLOW = 6
+  python file.py
+        @4 biggus
+        @5 dickus   # Program stop execution until user press Enter
+        @6 nortius
+  ```
+
+- **_JSON File Example_**
+
+  ```json
+  "nezu": {
+      "flow": 6,
+  }
+  ```
+- **_Example Hardcoded Config_**
+
+  ```py
+  from nezu import nezu, dbg
+
+  nezu(flow = 6)
+  ...
+  ```
```

