# Comparing `tmp/dorkas-0.1.0.tar.gz` & `tmp/dorkas-0.1.2.tar.gz`

## Comparing `dorkas-0.1.0.tar` & `dorkas-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,18 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 dorkas-0.1.0/Cargo.toml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dorkas-0.1.0/dev-requirements.txt
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 dorkas-0.1.0/justfile
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dorkas-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dorkas-0.1.0/dorkas/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dorkas-0.1.0/src/main.rs
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dorkas-0.1.0/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dorkas-0.1.0/LICENSE
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 dorkas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dorkas-0.1.0/readme.md
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dorkas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dorkas-0.1.2/dev-requirements.txt
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 dorkas-0.1.2/justfile
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dorkas-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dorkas-0.1.2/src/dorkas/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dorkas-0.1.2/src/dorkas/q1.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 dorkas-0.1.2/src/dorkas-core/Cargo.toml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 dorkas-0.1.2/src/dorkas-core/pyproject.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dorkas-0.1.2/src/dorkas-core/readme.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dorkas-0.1.2/src/dorkas-core/src/lib.rs
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dorkas-0.1.2/src/dorkas-core/src/main.rs
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dorkas-0.1.2/temp/Cargo.toml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dorkas-0.1.2/temp/src/lib.rs
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dorkas-0.1.2/temp/src/main.rs
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dorkas-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dorkas-0.1.2/LICENSE
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dorkas-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dorkas-0.1.2/readme.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dorkas-0.1.2/PKG-INFO
```

### Comparing `dorkas-0.1.0/justfile` & `dorkas-0.1.2/justfile`

 * *Files 24% similar despite different names*

```diff
@@ -16,54 +16,52 @@
     @pip install -r dev-requirements.txt
 
 # test
 test:
     @cargo test
 
 # build
-build-rs:
-    @cargo build --release
-    @cp target/release/dorkas ~/.cargo/bin
-
-build-py:
-    @python -m build
-
 build:
     just clean
-    just build-rs
-    just build-py
+    @python -m build src/dorkas-core
+    @python -m build
 
 # format
 format:
-    @cargo fmt
-#   @ruff format . || True
+    @cargo fmt --manifest-path src/dorkas-core/Cargo.toml
+    @ruff format . || True
 
 # install
 install:
     @pip install -e '.[all]'
 
 # uninstall
 uninstall:
     @pip uninstall dorkas -y
 
 # publish-test
 release-test:
     just build
+    @twine upload --repository testpypi src/dorkas-core/dist/* -u __token__ -p ${PYPI_TEST_TOKEN}
     @twine upload --repository testpypi dist/* -u __token__ -p ${PYPI_TEST_TOKEN}
 
 # publish
 release:
     just build
+    @twine upload src/dorkas-core/dist/* -u __token__ -p ${PYPI_TOKEN}
     @twine upload dist/* -u __token__ -p ${PYPI_TOKEN}
 
 # streamlit stuff
 app:
     @streamlit run app.py
 
 # smoke-test
 smoke-test:
     ruff format --check .
 
 # clean
 clean:
+    @rm -r src/dorkas-core/target || True
+    @rm -rf src/dorkas-core/dist || True
     @rm -r target || True
     @rm -rf dist || True
+
```

### Comparing `dorkas-0.1.0/LICENSE` & `dorkas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dorkas-0.1.0/pyproject.toml` & `dorkas-0.1.2/src/dorkas-core/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+#requires = ["hatchling"]
+#build-backend = "hatchling.build"
+
+requires = ["maturin>=1.5,<2.0"]
+build-backend = "maturin"
 
 [project]
-name = "dorkas"
-version = "0.1.0"
+name = "dorkas-core"
 authors = [
   { name="Cody", email="cody@dkdc.dev" },
 ]
 description = "dorkas"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = []
+dynamic = ["version"]
+
+[tool.maturin]
+features = ["pyo3/extension-module"]
 
 [project.urls]
 "Homepage" = "https://github.com/lostmygithubaccount/dorkas"
 "Bug Tracker" = "https://github.com/lostmygithubaccount/dorkas/issues"
 
 #[project.scripts]
 #dorkas= "dorkas.cli:app"
```

