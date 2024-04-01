# Comparing `tmp/pyyaml-include-2.0b1.tar.gz` & `tmp/pyyaml-include-2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyaml-include-2.0b1.tar", last modified: Mon Mar 11 03:02:49 2024, max compression
+gzip compressed data, was "pyyaml-include-2.0b2.tar", last modified: Wed Mar 27 03:52:18 2024, max compression
```

## Comparing `pyyaml-include-2.0b1.tar` & `pyyaml-include-2.0b2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:02:49.295756 pyyaml-include-2.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-03-11 03:02:49.295756 pyyaml-include-2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 03:02:49.299756 pyyaml-include-2.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:02:49.295756 pyyaml-include-2.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:02:49.295756 pyyaml-include-2.0b1/src/pyyaml_include.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-03-11 03:02:49.000000 pyyaml-include-2.0b1/src/pyyaml_include.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-11 03:02:49.000000 pyyaml-include-2.0b1/src/pyyaml_include.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 03:02:49.000000 pyyaml-include-2.0b1/src/pyyaml_include.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-11 03:02:49.000000 pyyaml-include-2.0b1/src/pyyaml_include.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-11 03:02:49.000000 pyyaml-include-2.0b1/src/pyyaml_include.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:02:49.295756 pyyaml-include-2.0b1/src/yaml_include/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/src/yaml_include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-11 03:02:49.000000 pyyaml-include-2.0b1/src/yaml_include/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/src/yaml_include/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/src/yaml_include/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/src/yaml_include/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/src/yaml_include/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/src/yaml_include/yaml_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-11 03:02:42.000000 pyyaml-include-2.0b1/src/yaml_include/yaml_types_backward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.245694 pyyaml-include-2.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/src/yaml_include/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/yaml_include/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/yaml_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/yaml_types_backward.py
```

### Comparing `pyyaml-include-2.0b1/CHANGELOG.md` & `pyyaml-include-2.0b2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## 2.0b2
+
+> 📅 **Date** 2024-3-27
+
+- ❎ Breaking Changes:
+  - data-class attribute order changed in `yaml_include.Constructor`
+- Some optimizations and bugfix
+
 ## 2.0b1
 
 > 📅 **Date** 2024-3-11
 
 - ❎ Breaking Changes:
   - namespace changed to `yaml_include`
```

### Comparing `pyyaml-include-2.0b1/LICENSE` & `pyyaml-include-2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyaml-include-2.0b1/PKG-INFO` & `pyyaml-include-2.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: pyyaml-include
-Version: 2.0b1
+Version: 2.0b2
 Summary: An extending constructor of PyYAML: include other YAML files into current YAML document
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/tanbro/pyyaml-include
 Project-URL: Repository, https://github.com/tanbro/pyyaml-include.git
 Project-URL: Documentation, https://pyyaml-include.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/tanbro/pyyaml-include/issues
 Project-URL: Changelog, https://github.com/tanbro/pyyaml-include/blob/main/CHANGELOG.md
 Keywords: yaml,PyYAML,include,yml
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: PyYAML<7.0,>=6.0
@@ -55,15 +62,17 @@
   ```bash
   pip install --pre "pyyaml-include>=2.0" fsspec[s3]
   ```
 
 - see [fsspec][]'s documentation for more
 
 > 🔖 **Tip** \
-> “pyyaml-include” itself depends on [fsspec][], so it will be installed no matter including local or remote files
+>
+> - “pyyaml-include” depends on [fsspec][], which will be installed no matter including local or remote files.
+> - It's advised to use the library on Python version `>=3.8`, early versions are not guaranteed.
 
 ## Basic usages
 
 Consider we have such [YAML][] files:
 
 ```
 ├── 0.yml
@@ -215,15 +224,15 @@
    ```python
    import yaml
    import fsspec
    import yaml_include
 
    http_fs = fsspec.filesystem("http", client_kwargs={"base_url": f"http://{HOST}:{PORT}"})
 
-   ctor = yaml_include.Constructor(http_fs, base_dir="/foo/baz")
+   ctor = yaml_include.Constructor(fs=http_fs, base_dir="/foo/baz")
    yaml.add_constructor("!inc", ctor, yaml.Loader)
    ```
 
 1. then, write a [YAML][] document to include files from `http://${HOST}:${PORT}`:
 
    ```yaml
    key1: !inc doc1.yml    # relative path to "base_dir"
@@ -294,17 +303,17 @@
 
   ```yaml
   files: !inc {urlpath: /foo/baz.yaml, encoding: utf16}
   ```
 
 But the format of parameters has multiple cases, and differs variably in different [fsspec][] implementation backends.
 
-- If a scheme/protocol(“`http://`”, “`sftp://`”, “`file://`”, etc.) is defined in `urlpath`, `Constructor` will invoke [`fsspece.open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open) directly to open it. Which means `Constructor`'s `fs` will be ignored, and a new standalone `fs` will be created implicitly.
+- If a scheme/protocol(“`http://`”, “`sftp://`”, “`file://`”, etc.) is defined, and there is no wildcard in `urlpath`, `Constructor` will invoke [`fsspec.open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open) directly to open it. Which means `Constructor`'s `fs` will be ignored, and a new standalone `fs` will be created implicitly.
 
-  In this situation, `urlpath` will be passed to `fsspece.open`'s first argument, and all other parameters will also be passed to the function.
+  In this situation, `urlpath` will be passed to `fsspec.open`'s first argument, and all other parameters will also be passed to the function.
 
   For example,
 
   - the [YAML][] snippet
 
     ```yaml
     files: !inc [file:///foo/baz.yaml, r]
@@ -326,21 +335,22 @@
     will cause python code like
 
     ```python
     with fsspec.open("file:///foo/baz.yaml", encoding="utf16") as f:
         yaml.load(f, Loader)
     ```
 
-  > 🔖 **Tip** \
-  > `urlpath` with scheme/protocol **SHOULD NOT** include wildcards character(s), `urlpath` like `"file:///etc/foo/*.yml"` is illegal.
+- If `urlpath` has wildcard, and also scheme in it, `Constructor` will:
+
+  Invoke [fsspec][]'s [`open_files`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open_files) function to search, open and load files, and return the results in a list. [YAML][] include statement's parameters are passed to `open_files` function.
 
-- If `urlpath` has wildcards in it, `Constructor` will:
+- If `urlpath` has wildcard, and no scheme in it, `Constructor` will:
 
   1. invoke corresponding [fsspec][] implementation backend's [`glob`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.glob) method to search files,
-  1. then call [`open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.open) method to open the found file(s).
+  1. then call [`open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.open) method to open each found file(s).
 
   `urlpath` will be passed as the first argument to both `glob` and `open` method of the corresponding [fsspec][] implementation backend, and other parameters will also be passed to `glob` and `open` method as their following arguments.
 
   In the case of wildcards, what need to pay special attention to is that there are **two separated parameters** after `urlpath`, the first is for `glob` method, and the second is for `open` method. Each of them could be either sequence, mapping or scalar, corresponds single, positional and named argument(s) in python. For example:
 
   - If we want to include every `.yml` file in directory `etc/app` recursively with max depth at 2, and open them in utf-16 codec, we shall write the [YAML][] as below:
 
@@ -432,15 +442,15 @@
 
 ```yaml
 xyz: !http-include xyz.yml
 ```
 
 the actual URL to access is `http://$HOST:$PORT/sub_1/sub_1_1/xyz.yml`
 
-## Serialization
+### Serialization
 
 When load [YAML][] string with include statement, the including files are default parsed into python objects. Thant is, if we call `yaml.dump()` on the object, what dumped is the parsed python object, and can not serialize the include statement itself.
 
 To serialize the statement, we shall first create an `yaml_include.Constructor` object whose `autoload` is `False`:
 
 ```python
 import yaml
@@ -450,16 +460,16 @@
 ```
 
 then add both Constructor for Loader and Representer for Dumper:
 
 ```python
 yaml.add_constructor("!inc", ctor)
 
-repr_ = yaml_include.Representer("inc")
-yaml.add_representer(yaml_include.Data, repr_)
+rpr = yaml_include.Representer("inc")
+yaml.add_representer(yaml_include.Data, rpr)
 ```
 
 Now, the including files will not be loaded when call `yaml.load()`, and `yaml_include.Data` objects will be placed at the positions where include statements are.
 
 continue above code:
 
 ```python
@@ -471,60 +481,68 @@
 d0 = yaml.load(yaml_str, yaml.Loader)
 # Here, "include.d/1.yaml" and "include.d/2.yaml" not be opened or loaded.
 # d0 is like:
 # [Data(urlpath="include.d/1.yaml"), Data(urlpath="include.d/2.yaml")]
 
 # serialize d0
 s = yaml.dump(d0)
+print(s)
 # ‘s’ will be:
 # - !inc 'include.d/1.yaml'
 # - !inc 'include.d/2.yaml'
-print(s)
 
-# also we can perform a de-serialization
+# de-serialization
 ctor.autoload = True # re-open auto load
 # then load, the file "include.d/1.yaml" and "include.d/2.yaml" will be opened and loaded.
 d1 = yaml.load(s, yaml.Loader)
 
 # Or perform a recursive opening / parsing on the object:
-import yaml_include
+d2 = yaml_include.load(d0) # d2 is equal to d1
+```
 
-# d2 is equal to d1
-d2 = yaml_include.load(d0)
+`autoload` can be used in a `with` statement:
+
+```python
+ctor = yaml_include.Constructor()
+# autoload is True here
+
+with ctor.managed_autoload(False):
+    # temporary set autoload to False
+    yaml.full_load(YAML_TEXT)
+# autoload restore True automatic
 ```
 
 ### Include JSON or TOML
 
 We can include files in different format other than [YAML][], like [JSON][] or [TOML][] -- ``custom_loader`` is for that.
 
 > 📑 **Example** \
 > For example:
 >
 > ```python
 > import json
-> import tomllib
+> import tomllib as toml
 > import yaml
-> import fsspec
 > import yaml_include
 >
 > # Define loader function
 > def my_loader(urlpath, file, Loader):
 >     if urlpath.endswith(".json"):
 >         return json.load(file)
 >     if urlpath.endswith(".toml"):
->         return tomllib.load(file)
+>         return toml.load(file)
 >     return yaml.load(file, Loader)
 >
 > # Create the include constructor, with the custom loader
 > ctor = yaml_include.Constructor(custom_loader=my_loader)
 >
 > # Add the constructor to YAML Loader
 > yaml.add_constructor("!inc", ctor, yaml.Loader)
 >
-> # Then, json files will can be loaded by stdlib's json module, and the same to toml files.
+> # Then, json files will can be loaded by std-lib's json module, and the same to toml files.
 > s = """
 > json: !inc "*.json"
 > toml: !inc "*.toml"
 > yaml: !inc "*.yaml"
 > """
 >
 > yaml.load(s, yaml.Loader)
@@ -537,27 +555,18 @@
    ```bash
    git clone https://github.com/tanbro/pyyaml-include.git
    cd pyyaml-include
    ```
 
 1. create then activate a python virtual-env:
 
-   - POSIX:
-
-     ```bash
-     python3 -m venv .venv
-     .venv/bin/activate
-     ```
-
-   - Windows(PowerShell):
-
-     ```powershell
-     python3 -m venv .venv
-     .venv\Scripts\Activate.ps1
-     ```
+   ```bash
+   python -m venv .venv
+   .venv/bin/activate
+   ```
 
 1. install development requirements and the project itself in editable mode:
 
    ```bash
    pip install -r requirements.txt
    ```
```

### Comparing `pyyaml-include-2.0b1/README.md` & `pyyaml-include-2.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
   ```bash
   pip install --pre "pyyaml-include>=2.0" fsspec[s3]
   ```
 
 - see [fsspec][]'s documentation for more
 
 > 🔖 **Tip** \
-> “pyyaml-include” itself depends on [fsspec][], so it will be installed no matter including local or remote files
+>
+> - “pyyaml-include” depends on [fsspec][], which will be installed no matter including local or remote files.
+> - It's advised to use the library on Python version `>=3.8`, early versions are not guaranteed.
 
 ## Basic usages
 
 Consider we have such [YAML][] files:
 
 ```
 ├── 0.yml
@@ -189,15 +191,15 @@
    ```python
    import yaml
    import fsspec
    import yaml_include
 
    http_fs = fsspec.filesystem("http", client_kwargs={"base_url": f"http://{HOST}:{PORT}"})
 
-   ctor = yaml_include.Constructor(http_fs, base_dir="/foo/baz")
+   ctor = yaml_include.Constructor(fs=http_fs, base_dir="/foo/baz")
    yaml.add_constructor("!inc", ctor, yaml.Loader)
    ```
 
 1. then, write a [YAML][] document to include files from `http://${HOST}:${PORT}`:
 
    ```yaml
    key1: !inc doc1.yml    # relative path to "base_dir"
@@ -268,17 +270,17 @@
 
   ```yaml
   files: !inc {urlpath: /foo/baz.yaml, encoding: utf16}
   ```
 
 But the format of parameters has multiple cases, and differs variably in different [fsspec][] implementation backends.
 
-- If a scheme/protocol(“`http://`”, “`sftp://`”, “`file://`”, etc.) is defined in `urlpath`, `Constructor` will invoke [`fsspece.open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open) directly to open it. Which means `Constructor`'s `fs` will be ignored, and a new standalone `fs` will be created implicitly.
+- If a scheme/protocol(“`http://`”, “`sftp://`”, “`file://`”, etc.) is defined, and there is no wildcard in `urlpath`, `Constructor` will invoke [`fsspec.open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open) directly to open it. Which means `Constructor`'s `fs` will be ignored, and a new standalone `fs` will be created implicitly.
 
-  In this situation, `urlpath` will be passed to `fsspece.open`'s first argument, and all other parameters will also be passed to the function.
+  In this situation, `urlpath` will be passed to `fsspec.open`'s first argument, and all other parameters will also be passed to the function.
 
   For example,
 
   - the [YAML][] snippet
 
     ```yaml
     files: !inc [file:///foo/baz.yaml, r]
@@ -300,21 +302,22 @@
     will cause python code like
 
     ```python
     with fsspec.open("file:///foo/baz.yaml", encoding="utf16") as f:
         yaml.load(f, Loader)
     ```
 
-  > 🔖 **Tip** \
-  > `urlpath` with scheme/protocol **SHOULD NOT** include wildcards character(s), `urlpath` like `"file:///etc/foo/*.yml"` is illegal.
+- If `urlpath` has wildcard, and also scheme in it, `Constructor` will:
+
+  Invoke [fsspec][]'s [`open_files`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open_files) function to search, open and load files, and return the results in a list. [YAML][] include statement's parameters are passed to `open_files` function.
 
-- If `urlpath` has wildcards in it, `Constructor` will:
+- If `urlpath` has wildcard, and no scheme in it, `Constructor` will:
 
   1. invoke corresponding [fsspec][] implementation backend's [`glob`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.glob) method to search files,
-  1. then call [`open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.open) method to open the found file(s).
+  1. then call [`open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.open) method to open each found file(s).
 
   `urlpath` will be passed as the first argument to both `glob` and `open` method of the corresponding [fsspec][] implementation backend, and other parameters will also be passed to `glob` and `open` method as their following arguments.
 
   In the case of wildcards, what need to pay special attention to is that there are **two separated parameters** after `urlpath`, the first is for `glob` method, and the second is for `open` method. Each of them could be either sequence, mapping or scalar, corresponds single, positional and named argument(s) in python. For example:
 
   - If we want to include every `.yml` file in directory `etc/app` recursively with max depth at 2, and open them in utf-16 codec, we shall write the [YAML][] as below:
 
@@ -406,15 +409,15 @@
 
 ```yaml
 xyz: !http-include xyz.yml
 ```
 
 the actual URL to access is `http://$HOST:$PORT/sub_1/sub_1_1/xyz.yml`
 
-## Serialization
+### Serialization
 
 When load [YAML][] string with include statement, the including files are default parsed into python objects. Thant is, if we call `yaml.dump()` on the object, what dumped is the parsed python object, and can not serialize the include statement itself.
 
 To serialize the statement, we shall first create an `yaml_include.Constructor` object whose `autoload` is `False`:
 
 ```python
 import yaml
@@ -424,16 +427,16 @@
 ```
 
 then add both Constructor for Loader and Representer for Dumper:
 
 ```python
 yaml.add_constructor("!inc", ctor)
 
-repr_ = yaml_include.Representer("inc")
-yaml.add_representer(yaml_include.Data, repr_)
+rpr = yaml_include.Representer("inc")
+yaml.add_representer(yaml_include.Data, rpr)
 ```
 
 Now, the including files will not be loaded when call `yaml.load()`, and `yaml_include.Data` objects will be placed at the positions where include statements are.
 
 continue above code:
 
 ```python
@@ -445,60 +448,68 @@
 d0 = yaml.load(yaml_str, yaml.Loader)
 # Here, "include.d/1.yaml" and "include.d/2.yaml" not be opened or loaded.
 # d0 is like:
 # [Data(urlpath="include.d/1.yaml"), Data(urlpath="include.d/2.yaml")]
 
 # serialize d0
 s = yaml.dump(d0)
+print(s)
 # ‘s’ will be:
 # - !inc 'include.d/1.yaml'
 # - !inc 'include.d/2.yaml'
-print(s)
 
-# also we can perform a de-serialization
+# de-serialization
 ctor.autoload = True # re-open auto load
 # then load, the file "include.d/1.yaml" and "include.d/2.yaml" will be opened and loaded.
 d1 = yaml.load(s, yaml.Loader)
 
 # Or perform a recursive opening / parsing on the object:
-import yaml_include
+d2 = yaml_include.load(d0) # d2 is equal to d1
+```
 
-# d2 is equal to d1
-d2 = yaml_include.load(d0)
+`autoload` can be used in a `with` statement:
+
+```python
+ctor = yaml_include.Constructor()
+# autoload is True here
+
+with ctor.managed_autoload(False):
+    # temporary set autoload to False
+    yaml.full_load(YAML_TEXT)
+# autoload restore True automatic
 ```
 
 ### Include JSON or TOML
 
 We can include files in different format other than [YAML][], like [JSON][] or [TOML][] -- ``custom_loader`` is for that.
 
 > 📑 **Example** \
 > For example:
 >
 > ```python
 > import json
-> import tomllib
+> import tomllib as toml
 > import yaml
-> import fsspec
 > import yaml_include
 >
 > # Define loader function
 > def my_loader(urlpath, file, Loader):
 >     if urlpath.endswith(".json"):
 >         return json.load(file)
 >     if urlpath.endswith(".toml"):
->         return tomllib.load(file)
+>         return toml.load(file)
 >     return yaml.load(file, Loader)
 >
 > # Create the include constructor, with the custom loader
 > ctor = yaml_include.Constructor(custom_loader=my_loader)
 >
 > # Add the constructor to YAML Loader
 > yaml.add_constructor("!inc", ctor, yaml.Loader)
 >
-> # Then, json files will can be loaded by stdlib's json module, and the same to toml files.
+> # Then, json files will can be loaded by std-lib's json module, and the same to toml files.
 > s = """
 > json: !inc "*.json"
 > toml: !inc "*.toml"
 > yaml: !inc "*.yaml"
 > """
 >
 > yaml.load(s, yaml.Loader)
@@ -511,27 +522,18 @@
    ```bash
    git clone https://github.com/tanbro/pyyaml-include.git
    cd pyyaml-include
    ```
 
 1. create then activate a python virtual-env:
 
-   - POSIX:
-
-     ```bash
-     python3 -m venv .venv
-     .venv/bin/activate
-     ```
-
-   - Windows(PowerShell):
-
-     ```powershell
-     python3 -m venv .venv
-     .venv\Scripts\Activate.ps1
-     ```
+   ```bash
+   python -m venv .venv
+   .venv/bin/activate
+   ```
 
 1. install development requirements and the project itself in editable mode:
 
    ```bash
    pip install -r requirements.txt
    ```
```

### Comparing `pyyaml-include-2.0b1/pyproject.toml` & `pyyaml-include-2.0b2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -20,21 +20,28 @@
 
 license = { text = "GPLv3+" }
 
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   # "Development Status :: 1 - Planning",
   # "Development Status :: 2 - Pre-Alpha",
-  "Development Status :: 3 - Alpha",
-  # "Development Status :: 4 - Beta",
+  # "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   # "Development Status :: 5 - Production/Stable",
   # "Development Status :: 6 - Mature",
   # "Development Status :: 7 - Inactive",
   "Intended Audience :: Developers",
+  "Programming Language :: Python",
   "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Text Processing :: Markup",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `pyyaml-include-2.0b1/src/pyyaml_include.egg-info/PKG-INFO` & `pyyaml-include-2.0b2/src/pyyaml_include.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: pyyaml-include
-Version: 2.0b1
+Version: 2.0b2
 Summary: An extending constructor of PyYAML: include other YAML files into current YAML document
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/tanbro/pyyaml-include
 Project-URL: Repository, https://github.com/tanbro/pyyaml-include.git
 Project-URL: Documentation, https://pyyaml-include.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/tanbro/pyyaml-include/issues
 Project-URL: Changelog, https://github.com/tanbro/pyyaml-include/blob/main/CHANGELOG.md
 Keywords: yaml,PyYAML,include,yml
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: PyYAML<7.0,>=6.0
@@ -55,15 +62,17 @@
   ```bash
   pip install --pre "pyyaml-include>=2.0" fsspec[s3]
   ```
 
 - see [fsspec][]'s documentation for more
 
 > 🔖 **Tip** \
-> “pyyaml-include” itself depends on [fsspec][], so it will be installed no matter including local or remote files
+>
+> - “pyyaml-include” depends on [fsspec][], which will be installed no matter including local or remote files.
+> - It's advised to use the library on Python version `>=3.8`, early versions are not guaranteed.
 
 ## Basic usages
 
 Consider we have such [YAML][] files:
 
 ```
 ├── 0.yml
@@ -215,15 +224,15 @@
    ```python
    import yaml
    import fsspec
    import yaml_include
 
    http_fs = fsspec.filesystem("http", client_kwargs={"base_url": f"http://{HOST}:{PORT}"})
 
-   ctor = yaml_include.Constructor(http_fs, base_dir="/foo/baz")
+   ctor = yaml_include.Constructor(fs=http_fs, base_dir="/foo/baz")
    yaml.add_constructor("!inc", ctor, yaml.Loader)
    ```
 
 1. then, write a [YAML][] document to include files from `http://${HOST}:${PORT}`:
 
    ```yaml
    key1: !inc doc1.yml    # relative path to "base_dir"
@@ -294,17 +303,17 @@
 
   ```yaml
   files: !inc {urlpath: /foo/baz.yaml, encoding: utf16}
   ```
 
 But the format of parameters has multiple cases, and differs variably in different [fsspec][] implementation backends.
 
-- If a scheme/protocol(“`http://`”, “`sftp://`”, “`file://`”, etc.) is defined in `urlpath`, `Constructor` will invoke [`fsspece.open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open) directly to open it. Which means `Constructor`'s `fs` will be ignored, and a new standalone `fs` will be created implicitly.
+- If a scheme/protocol(“`http://`”, “`sftp://`”, “`file://`”, etc.) is defined, and there is no wildcard in `urlpath`, `Constructor` will invoke [`fsspec.open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open) directly to open it. Which means `Constructor`'s `fs` will be ignored, and a new standalone `fs` will be created implicitly.
 
-  In this situation, `urlpath` will be passed to `fsspece.open`'s first argument, and all other parameters will also be passed to the function.
+  In this situation, `urlpath` will be passed to `fsspec.open`'s first argument, and all other parameters will also be passed to the function.
 
   For example,
 
   - the [YAML][] snippet
 
     ```yaml
     files: !inc [file:///foo/baz.yaml, r]
@@ -326,21 +335,22 @@
     will cause python code like
 
     ```python
     with fsspec.open("file:///foo/baz.yaml", encoding="utf16") as f:
         yaml.load(f, Loader)
     ```
 
-  > 🔖 **Tip** \
-  > `urlpath` with scheme/protocol **SHOULD NOT** include wildcards character(s), `urlpath` like `"file:///etc/foo/*.yml"` is illegal.
+- If `urlpath` has wildcard, and also scheme in it, `Constructor` will:
+
+  Invoke [fsspec][]'s [`open_files`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.open_files) function to search, open and load files, and return the results in a list. [YAML][] include statement's parameters are passed to `open_files` function.
 
-- If `urlpath` has wildcards in it, `Constructor` will:
+- If `urlpath` has wildcard, and no scheme in it, `Constructor` will:
 
   1. invoke corresponding [fsspec][] implementation backend's [`glob`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.glob) method to search files,
-  1. then call [`open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.open) method to open the found file(s).
+  1. then call [`open`](https://filesystem-spec.readthedocs.io/en/stable/api.html#fsspec.spec.AbstractFileSystem.open) method to open each found file(s).
 
   `urlpath` will be passed as the first argument to both `glob` and `open` method of the corresponding [fsspec][] implementation backend, and other parameters will also be passed to `glob` and `open` method as their following arguments.
 
   In the case of wildcards, what need to pay special attention to is that there are **two separated parameters** after `urlpath`, the first is for `glob` method, and the second is for `open` method. Each of them could be either sequence, mapping or scalar, corresponds single, positional and named argument(s) in python. For example:
 
   - If we want to include every `.yml` file in directory `etc/app` recursively with max depth at 2, and open them in utf-16 codec, we shall write the [YAML][] as below:
 
@@ -432,15 +442,15 @@
 
 ```yaml
 xyz: !http-include xyz.yml
 ```
 
 the actual URL to access is `http://$HOST:$PORT/sub_1/sub_1_1/xyz.yml`
 
-## Serialization
+### Serialization
 
 When load [YAML][] string with include statement, the including files are default parsed into python objects. Thant is, if we call `yaml.dump()` on the object, what dumped is the parsed python object, and can not serialize the include statement itself.
 
 To serialize the statement, we shall first create an `yaml_include.Constructor` object whose `autoload` is `False`:
 
 ```python
 import yaml
@@ -450,16 +460,16 @@
 ```
 
 then add both Constructor for Loader and Representer for Dumper:
 
 ```python
 yaml.add_constructor("!inc", ctor)
 
-repr_ = yaml_include.Representer("inc")
-yaml.add_representer(yaml_include.Data, repr_)
+rpr = yaml_include.Representer("inc")
+yaml.add_representer(yaml_include.Data, rpr)
 ```
 
 Now, the including files will not be loaded when call `yaml.load()`, and `yaml_include.Data` objects will be placed at the positions where include statements are.
 
 continue above code:
 
 ```python
@@ -471,60 +481,68 @@
 d0 = yaml.load(yaml_str, yaml.Loader)
 # Here, "include.d/1.yaml" and "include.d/2.yaml" not be opened or loaded.
 # d0 is like:
 # [Data(urlpath="include.d/1.yaml"), Data(urlpath="include.d/2.yaml")]
 
 # serialize d0
 s = yaml.dump(d0)
+print(s)
 # ‘s’ will be:
 # - !inc 'include.d/1.yaml'
 # - !inc 'include.d/2.yaml'
-print(s)
 
-# also we can perform a de-serialization
+# de-serialization
 ctor.autoload = True # re-open auto load
 # then load, the file "include.d/1.yaml" and "include.d/2.yaml" will be opened and loaded.
 d1 = yaml.load(s, yaml.Loader)
 
 # Or perform a recursive opening / parsing on the object:
-import yaml_include
+d2 = yaml_include.load(d0) # d2 is equal to d1
+```
 
-# d2 is equal to d1
-d2 = yaml_include.load(d0)
+`autoload` can be used in a `with` statement:
+
+```python
+ctor = yaml_include.Constructor()
+# autoload is True here
+
+with ctor.managed_autoload(False):
+    # temporary set autoload to False
+    yaml.full_load(YAML_TEXT)
+# autoload restore True automatic
 ```
 
 ### Include JSON or TOML
 
 We can include files in different format other than [YAML][], like [JSON][] or [TOML][] -- ``custom_loader`` is for that.
 
 > 📑 **Example** \
 > For example:
 >
 > ```python
 > import json
-> import tomllib
+> import tomllib as toml
 > import yaml
-> import fsspec
 > import yaml_include
 >
 > # Define loader function
 > def my_loader(urlpath, file, Loader):
 >     if urlpath.endswith(".json"):
 >         return json.load(file)
 >     if urlpath.endswith(".toml"):
->         return tomllib.load(file)
+>         return toml.load(file)
 >     return yaml.load(file, Loader)
 >
 > # Create the include constructor, with the custom loader
 > ctor = yaml_include.Constructor(custom_loader=my_loader)
 >
 > # Add the constructor to YAML Loader
 > yaml.add_constructor("!inc", ctor, yaml.Loader)
 >
-> # Then, json files will can be loaded by stdlib's json module, and the same to toml files.
+> # Then, json files will can be loaded by std-lib's json module, and the same to toml files.
 > s = """
 > json: !inc "*.json"
 > toml: !inc "*.toml"
 > yaml: !inc "*.yaml"
 > """
 >
 > yaml.load(s, yaml.Loader)
@@ -537,27 +555,18 @@
    ```bash
    git clone https://github.com/tanbro/pyyaml-include.git
    cd pyyaml-include
    ```
 
 1. create then activate a python virtual-env:
 
-   - POSIX:
-
-     ```bash
-     python3 -m venv .venv
-     .venv/bin/activate
-     ```
-
-   - Windows(PowerShell):
-
-     ```powershell
-     python3 -m venv .venv
-     .venv\Scripts\Activate.ps1
-     ```
+   ```bash
+   python -m venv .venv
+   .venv/bin/activate
+   ```
 
 1. install development requirements and the project itself in editable mode:
 
    ```bash
    pip install -r requirements.txt
    ```
```

### Comparing `pyyaml-include-2.0b1/src/pyyaml_include.egg-info/SOURCES.txt` & `pyyaml-include-2.0b2/src/pyyaml_include.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 src/pyyaml_include.egg-info/PKG-INFO
 src/pyyaml_include.egg-info/SOURCES.txt
 src/pyyaml_include.egg-info/dependency_links.txt
 src/pyyaml_include.egg-info/requires.txt
 src/pyyaml_include.egg-info/top_level.txt
+src/yaml_include/.gitignore
 src/yaml_include/__init__.py
 src/yaml_include/_version.py
 src/yaml_include/constructor.py
 src/yaml_include/data.py
 src/yaml_include/funcs.py
 src/yaml_include/representer.py
 src/yaml_include/yaml_types.py
```

### Comparing `pyyaml-include-2.0b1/src/yaml_include/constructor.py` & `pyyaml-include-2.0b2/src/yaml_include/constructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from itertools import chain
 from os import PathLike
 from pathlib import Path
 from typing import Any, Callable, Generator, Optional, Union
 
-if sys.version_info < (3, 11):
+if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import Self
-else:
+else:  # pragma: no cover
     from typing import Self
 
 from urllib.parse import urlsplit, urlunsplit
 
 import fsspec
 import yaml
 
 from .data import Data
 
-if sys.version_info < (3, 12):
+if sys.version_info < (3, 12):  # pragma: no cover
     from .yaml_types_backward import TYamlLoaderTypes
-else:
+else:  # pragma: no cover
     from .yaml_types import TYamlLoaderTypes
 
 __all__ = ["Constructor"]
 
 WILDCARDS_PATTERN = re.compile(
     r"^(.*)([\*\?\[\]]+)(.*)$"
 )  # We support "**", "?" and "[..]". We do not support "^" for pattern negation.
@@ -102,14 +102,23 @@
 
     * If it is ``None``, the actual base directory was decided by the :mod:`fsspec` file-system implementation in use.
       For example, the ``base_dir`` is default to be ``cwd`` for ``LocalFileSystem``, and be the value of ``client_kwargs.base_url`` for ``HTTPFileSystem``.
     * Else if it is callable, the actual base directory will be it's return value.
     * Else it will be used directly as the actual base directory.
     """
 
+    autoload: bool = True
+    """Whether if open and parse including file(s) when called.
+
+    * If ``True``:
+      open including file(s) then parse its/their content with current PyYAML Loader, and returns the parsed result.
+    * If ``False``:
+      will **NOT** open including file(s), the return value is a :class:`.Data` object stores include statement.
+    """
+
     custom_loader: Optional[Callable[[str, Any, TYamlLoaderTypes], Any]] = None
     """Custom loader/parser function called when an including file is about to parse.
 
     If ``None``, parse the file as ordinary YAML with current `Loader` class.
 
     Else it shall be a callable object, as the replacement of ordinary YAML `Loader`.
 
@@ -152,23 +161,14 @@
         arg3(typing.Type):
             Type of `PyYAML`'s Loader class in use.
 
     Returns:
         typing.Any: Parsed result
     """
 
-    autoload: bool = True
-    """Whether if open and parse including file(s) when called.
-
-    * If ``True``:
-      open including file(s) then parse its/their content with current PyYAML Loader, and returns the parsed result.
-    * If ``False``:
-      will **NOT** open including file(s), the return value is a :class:`.Data` object stores include statement.
-    """
-
     @contextmanager
     def managed_autoload(self, autoload: bool) -> Generator[Self, Any, None]:
         """``with`` statement context manager for :attr:`autoload`
 
         Args:
             autoload: Temporary value of :attr:`autoload` to be set inside the ``with`` statement
         """
@@ -177,22 +177,22 @@
             yield self
         finally:
             self.autoload = saved
 
     def __call__(self, loader, node):
         if isinstance(node, yaml.ScalarNode):
             params = loader.construct_scalar(node)
-            data = Data(urlpath=params)
+            data = Data(params)
         elif isinstance(node, yaml.SequenceNode):
             params = loader.construct_sequence(node)
-            data = Data(urlpath=params[0], sequence_params=params[1:])
+            data = Data(params[0], sequence_params=params[1:])
         elif isinstance(node, yaml.MappingNode):
             params = loader.construct_mapping(node)
             data = Data(
-                urlpath=params["urlpath"],
+                params["urlpath"],
                 mapping_params={k: v for k, v in params.items() if k != "urlpath"},
             )
         else:  # pragma: no cover
             raise ValueError(f"PyYAML node {node!r} is not supported by {type(self)}")
         if self.autoload:
             return self.load(type(loader), data)
         else:
```

### Comparing `pyyaml-include-2.0b1/src/yaml_include/data.py` & `pyyaml-include-2.0b2/src/yaml_include/data.py`

 * *Files identical despite different names*

### Comparing `pyyaml-include-2.0b1/src/yaml_include/funcs.py` & `pyyaml-include-2.0b2/src/yaml_include/funcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from typing import Any, Generator, Mapping, MutableMapping, MutableSequence, Sequence
 
-if sys.version_info < (3, 12):
+if sys.version_info < (3, 12):  # pragma: no cover
     from .yaml_types_backward import TYamlLoaderTypes
-else:
+else:  # pragma: no cover
     from .yaml_types import TYamlLoaderTypes
 
 from .constructor import Constructor
 from .data import Data
 
 
 __all__ = ["load", "lazy_load"]
@@ -45,21 +45,16 @@
     elif isinstance(obj, Mapping):
         if inplace:
             if not isinstance(obj, MutableMapping):
                 raise ValueError(f"{obj} is not mutable")
             for k, v in obj.items():
                 obj[k] = load(v, loader_type, constructor, inplace, nested)
         else:
-            return {
-                k: load(v, loader_type, constructor, inplace, nested)
-                for k, v in obj.items()
-            }
-    elif isinstance(obj, Sequence) and not isinstance(
-        obj, (bytearray, bytes, memoryview, str)
-    ):
+            return {k: load(v, loader_type, constructor, inplace, nested) for k, v in obj.items()}
+    elif isinstance(obj, Sequence) and not isinstance(obj, (bytearray, bytes, memoryview, str)):
         if inplace:
             if not isinstance(obj, MutableSequence):
                 raise ValueError(f"{obj} is not mutable")
             for i, v in enumerate(obj):
                 obj[i] = load(v, loader_type, constructor, inplace, nested)
         else:
             return [load(m, loader_type, constructor, inplace, nested) for m in obj]
```

### Comparing `pyyaml-include-2.0b1/src/yaml_include/representer.py` & `pyyaml-include-2.0b2/src/yaml_include/representer.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,14 @@
         But we **MUST NOT** put a ``"!"`` at the beginning here,
         because :func:`yaml.add_representer` will add the symbol itself.
     """
 
     def __call__(self, dumper, data):
         if data.mapping_params:
             params = {"urlpath": data.urlpath}
-            params.update({k: v for k, v in data.mapping_params.items()})
+            params.update(data.mapping_params)
             return dumper.represent_mapping(f"!{self.tag}", params)
         if data.sequence_params:
             params = [data.urlpath]
             params.extend(data.sequence_params)
             return dumper.represent_sequence(f"!{self.tag}", params)
         return dumper.represent_scalar(f"!{self.tag}", data.urlpath)
```

### Comparing `pyyaml-include-2.0b1/src/yaml_include/yaml_types.py` & `pyyaml-include-2.0b2/src/yaml_include/yaml_types.py`

 * *Files identical despite different names*

### Comparing `pyyaml-include-2.0b1/src/yaml_include/yaml_types_backward.py` & `pyyaml-include-2.0b2/src/yaml_include/yaml_types_backward.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
+from warnings import warn
 
-if not sys.version_info < (3, 12):
-    raise ImportError("Python version greater than or equal to 3.12 should “from . import yaml_types”")
+if sys.version_info >= (3, 12):
+    warn("Python version greater than or equal to 3.12 should “from . import yaml_types”")
 
 from typing import Type, Union
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
```

