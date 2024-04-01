# Comparing `tmp/pymmg-0.1.0.tar.gz` & `tmp/pymmg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymmg-0.1.0.tar", last modified: Mon May  8 14:44:08 2023, max compression
+gzip compressed data, was "pymmg-1.0.0.tar", last modified: Mon Apr  1 15:13:02 2024, max compression
```

## Comparing `pymmg-0.1.0.tar` & `pymmg-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.101271 pymmg-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-05-08 14:34:17.000000 pymmg-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-05-08 14:34:17.000000 pymmg-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-08 14:34:17.000000 pymmg-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-08 14:34:17.000000 pymmg-0.1.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4500 2023-05-08 14:44:08.101271 pymmg-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-05-08 14:34:17.000000 pymmg-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/_skbuild/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/general/
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-08 14:44:08.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/general/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-08 14:44:08.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-08 14:44:08.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   586856 2023-05-08 14:43:11.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/mmg2d_O3
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.097271 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-08 14:44:08.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-08 14:44:08.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)  1147448 2023-05-08 14:43:41.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/mmg3d_O3
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.097271 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-08 14:44:08.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-08 14:44:08.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   580512 2023-05-08 14:43:20.000000 pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/mmgs_O3
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.097271 pymmg-0.1.0/pymmg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4500 2023-05-08 14:44:08.000000 pymmg-0.1.0/pymmg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-05-08 14:44:08.000000 pymmg-0.1.0/pymmg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 14:44:08.000000 pymmg-0.1.0/pymmg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-08 14:44:08.000000 pymmg-0.1.0/pymmg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 14:44:08.000000 pymmg-0.1.0/pymmg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-08 14:44:08.000000 pymmg-0.1.0/pymmg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-08 14:44:08.000000 pymmg-0.1.0/pymmg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-05-08 14:34:17.000000 pymmg-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 14:44:08.101271 pymmg-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-05-08 14:34:17.000000 pymmg-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.093271 pymmg-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.097271 pymmg-0.1.0/src/general/
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-08 14:34:17.000000 pymmg-0.1.0/src/general/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.101271 pymmg-0.1.0/src/mmg2d/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-08 14:34:17.000000 pymmg-0.1.0/src/mmg2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-08 14:34:17.000000 pymmg-0.1.0/src/mmg2d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.101271 pymmg-0.1.0/src/mmg3d/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-08 14:34:17.000000 pymmg-0.1.0/src/mmg3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-08 14:34:17.000000 pymmg-0.1.0/src/mmg3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 14:44:08.101271 pymmg-0.1.0/src/mmgs/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-08 14:34:17.000000 pymmg-0.1.0/src/mmgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-08 14:34:17.000000 pymmg-0.1.0/src/mmgs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.368352 pymmg-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.360351 pymmg-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 15:07:04.000000 pymmg-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.360351 pymmg-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-01 15:07:04.000000 pymmg-1.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-01 15:07:04.000000 pymmg-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-01 15:07:04.000000 pymmg-1.0.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-01 15:13:02.368352 pymmg-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-01 15:07:04.000000 pymmg-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.360351 pymmg-1.0.0/_skbuild/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.360351 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.360351 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.360351 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.364351 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/general/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/general/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.364351 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   586856 2024-04-01 15:12:38.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/mmg2d_O3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.364351 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1147448 2024-04-01 15:12:50.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/mmg3d_O3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.364351 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 15:13:02.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   580512 2024-04-01 15:12:37.000000 pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/mmgs_O3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.368352 pymmg-1.0.0/pymmg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-01 15:13:02.000000 pymmg-1.0.0/pymmg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 15:13:02.000000 pymmg-1.0.0/pymmg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:13:02.000000 pymmg-1.0.0/pymmg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 15:13:02.000000 pymmg-1.0.0/pymmg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:13:02.000000 pymmg-1.0.0/pymmg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 15:13:02.000000 pymmg-1.0.0/pymmg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 15:13:02.000000 pymmg-1.0.0/pymmg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-01 15:07:04.000000 pymmg-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:13:02.368352 pymmg-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 15:07:04.000000 pymmg-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.360351 pymmg-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.368352 pymmg-1.0.0/src/general/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-01 15:07:04.000000 pymmg-1.0.0/src/general/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.368352 pymmg-1.0.0/src/mmg2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 15:07:04.000000 pymmg-1.0.0/src/mmg2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 15:07:04.000000 pymmg-1.0.0/src/mmg2d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.368352 pymmg-1.0.0/src/mmg3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 15:07:04.000000 pymmg-1.0.0/src/mmg3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 15:07:04.000000 pymmg-1.0.0/src/mmg3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:13:02.368352 pymmg-1.0.0/src/mmgs/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 15:07:04.000000 pymmg-1.0.0/src/mmgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 15:07:04.000000 pymmg-1.0.0/src/mmgs/__main__.py
```

### Comparing `pymmg-0.1.0/.github/workflows/main.yml` & `pymmg-1.0.0/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -13,50 +13,51 @@
           - { os: windows-2019, shell: bash }
           - { os: ubuntu-20.04, shell: bash }
           - { os: macos-11, shell: bash }
     defaults:
       run:
         shell: ${{ matrix.sys.shell }}
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - name: Install MSVC if under Windows
         uses: ilammy/msvc-dev-cmd@v1
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.12.3
+        uses: pypa/cibuildwheel@v2.17.0
 
       - name: Make wheels Pythonless
         run: |
           python -m pip install wheel>=0.40.0
           wheel tags --python-tag py3 --abi-tag none --remove ./wheelhouse/*.whl
 
       - if: runner.os == 'Linux'
         name: Build source distribution
         run: |
           pipx run build --sdist --outdir=wheelhouse
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: python-wheels
+          name: python-wheels-${{ matrix.sys.os }}}
           path: |
             ./wheelhouse/*.whl
             ./wheelhouse/*.tar.gz
 
   publish:
     needs: [build_wheels]
     runs-on: ubuntu-latest
     permissions:
       id-token: write
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/download-artifact@v3
+      - uses: actions/checkout@v4
+      - uses: actions/download-artifact@v4
         with:
-          name: python-wheels
+          pattern: python-wheels*
           path: dist
+          merge-multiple: true
 
       - name: Publish package
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `pymmg-0.1.0/CMakeLists.txt` & `pymmg-1.0.0/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include(FetchContent)
 include(ExternalProject)
 
 ExternalProject_Add(
   mmg_src
   SOURCE_DIR "${CMAKE_BINARY_DIR}/mmg"
   GIT_REPOSITORY https://github.com/MmgTools/mmg
-  GIT_TAG "v5.7.1"
+  GIT_TAG "v5.7.2"
   CMAKE_ARGS -DCMAKE_INSTALL_PREFIX=${CMAKE_BINARY_DIR} -DDEF_MMG5_INT=int64_t
 )
 
 # ExternalProject_Get_Property(mmg_src binary_dir)
 add_executable(mmg2d_exe IMPORTED GLOBAL)
 add_dependencies(mmg2d_exe mmg_src)
 add_executable(mmg3d_exe IMPORTED GLOBAL)
```

### Comparing `pymmg-0.1.0/PKG-INFO` & `pymmg-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmg
-Version: 0.1.0
+Version: 1.0.0
 Summary: Surface and volume mesh and remesh generators based on MMG library
 Author: gnikit
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://www.mmgtools.org/
 Project-URL: Source Code, https://github.com/gnikit/pymmg
 Project-URL: Bugs, https://github.com/gnikit/pymmg/issues
 Project-URL: Dicsussions, https://forum.mmgtools.org/
@@ -20,15 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: meshio
 Provides-Extra: all
+Requires-Dist: meshio[all]; extra == "all"
 
 # pymmg - Surface and volume remeshers
 
 [![Build](https://github.com/gnikit/pymmg/actions/workflows/main.yml/badge.svg)](https://github.com/gnikit/pymmg/actions/workflows/main.yml)
 
 Bringing [MMG](https://www.mmgtools.org/) surface and volume remeshers to Python.
 This package is a wrapper around the MMG tools
@@ -72,15 +74,15 @@
 
 ## Installation
 
 ```bash
 pip install pymmg
 ```
 
-> NOTE: you can the full-blown `pymmg` converter with `netcdf4` and `h5py` by doing:
+> NOTE: you can use the full-blown `pymmg` converter with `netcdf4` and `h5py` by doing:
 > `pip install pymmg[all]`
 
 ## Usage
 
 ### Surface remeshing
 
 ```bash
```

### Comparing `pymmg-0.1.0/README.md` & `pymmg-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 ## Installation
 
 ```bash
 pip install pymmg
 ```
 
-> NOTE: you can the full-blown `pymmg` converter with `netcdf4` and `h5py` by doing:
+> NOTE: you can use the full-blown `pymmg` converter with `netcdf4` and `h5py` by doing:
 > `pip install pymmg[all]`
 
 ## Usage
 
 ### Surface remeshing
 
 ```bash
```

### Comparing `pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/general/__init__.py` & `pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/general/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/mmg2d_O3` & `pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/mmg2d_O3`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --symbols {}

```diff
@@ -600,46 +600,46 @@
     72: 0000000000074738    15 OBJECT  LOCAL  DEFAULT   18 __func__.7700
     73: 0000000000074720    20 OBJECT  LOCAL  DEFAULT   18 __func__.7729
     74: 0000000000074700    22 OBJECT  LOCAL  DEFAULT   18 __func__.7811
     75: 00000000000746e0    19 OBJECT  LOCAL  DEFAULT   18 __func__.7930
     76: 00000000000746c0    19 OBJECT  LOCAL  DEFAULT   18 __func__.7937
     77: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS API_functions_2d.c
     78: 0000000000076970    21 OBJECT  LOCAL  DEFAULT   18 __func__.8591
-    79: 0000000000076950    21 OBJECT  LOCAL  DEFAULT   18 __func__.8641
-    80: 0000000000076930    25 OBJECT  LOCAL  DEFAULT   18 __func__.8656
-    81: 0000000000076910    19 OBJECT  LOCAL  DEFAULT   18 __func__.8684
-    82: 00000000000768f0    18 OBJECT  LOCAL  DEFAULT   18 __func__.8696
-    83: 00000000000768d0    29 OBJECT  LOCAL  DEFAULT   18 __func__.8708
-    84: 00000000000768b0    29 OBJECT  LOCAL  DEFAULT   18 __func__.8729
-    85: 0000000000076890    17 OBJECT  LOCAL  DEFAULT   18 __func__.8751
-    86: 0000000000076850    22 OBJECT  LOCAL  DEFAULT   18 __func__.8786
-    87: 0000000000076870    17 OBJECT  LOCAL  DEFAULT   18 __func__.8776
-    88: 0000000000076830    19 OBJECT  LOCAL  DEFAULT   18 __func__.8826
-    89: 0000000000076810    19 OBJECT  LOCAL  DEFAULT   18 __func__.8855
-    90: 00000000000767f0    20 OBJECT  LOCAL  DEFAULT   18 __func__.8872
-    91: 00000000000767d0    24 OBJECT  LOCAL  DEFAULT   18 __func__.8905
-    92: 0000000000087524     4 OBJECT  LOCAL  DEFAULT   26 nqi.8915
-    93: 00000000000767b0    24 OBJECT  LOCAL  DEFAULT   18 __func__.8916
-    94: 00000000000767a0    15 OBJECT  LOCAL  DEFAULT   18 __func__.8948
-    95: 0000000000076790    15 OBJECT  LOCAL  DEFAULT   18 __func__.8974
-    96: 0000000000076770    26 OBJECT  LOCAL  DEFAULT   18 __func__.9007
-    97: 0000000000076750    20 OBJECT  LOCAL  DEFAULT   18 __func__.9013
-    98: 0000000000076730    20 OBJECT  LOCAL  DEFAULT   18 __func__.9019
-    99: 0000000000076710    21 OBJECT  LOCAL  DEFAULT   18 __func__.9025
-   100: 00000000000766f0    20 OBJECT  LOCAL  DEFAULT   18 __func__.9044
-   101: 00000000000766d0    20 OBJECT  LOCAL  DEFAULT   18 __func__.9051
-   102: 00000000000766b0    21 OBJECT  LOCAL  DEFAULT   18 __func__.9059
-   103: 0000000000076690    20 OBJECT  LOCAL  DEFAULT   18 __func__.9081
-   104: 0000000000076670    20 OBJECT  LOCAL  DEFAULT   18 __func__.9090
-   105: 0000000000076650    21 OBJECT  LOCAL  DEFAULT   18 __func__.9098
-   106: 0000000000076620    35 OBJECT  LOCAL  DEFAULT   18 __func__.9123
-   107: 00000000000765e0    35 OBJECT  LOCAL  DEFAULT   18 __func__.9135
-   108: 00000000000765a0    34 OBJECT  LOCAL  DEFAULT   18 __func__.9148
-   109: 0000000000076560    34 OBJECT  LOCAL  DEFAULT   18 __func__.9161
-   110: 0000000000076530    19 OBJECT  LOCAL  DEFAULT   18 __func__.9166
+    79: 0000000000076950    21 OBJECT  LOCAL  DEFAULT   18 __func__.8642
+    80: 0000000000076930    25 OBJECT  LOCAL  DEFAULT   18 __func__.8657
+    81: 0000000000076910    19 OBJECT  LOCAL  DEFAULT   18 __func__.8685
+    82: 00000000000768f0    18 OBJECT  LOCAL  DEFAULT   18 __func__.8697
+    83: 00000000000768d0    29 OBJECT  LOCAL  DEFAULT   18 __func__.8709
+    84: 00000000000768b0    29 OBJECT  LOCAL  DEFAULT   18 __func__.8730
+    85: 0000000000076890    17 OBJECT  LOCAL  DEFAULT   18 __func__.8752
+    86: 0000000000076850    22 OBJECT  LOCAL  DEFAULT   18 __func__.8787
+    87: 0000000000076870    17 OBJECT  LOCAL  DEFAULT   18 __func__.8777
+    88: 0000000000076830    19 OBJECT  LOCAL  DEFAULT   18 __func__.8827
+    89: 0000000000076810    19 OBJECT  LOCAL  DEFAULT   18 __func__.8856
+    90: 00000000000767f0    20 OBJECT  LOCAL  DEFAULT   18 __func__.8873
+    91: 00000000000767d0    24 OBJECT  LOCAL  DEFAULT   18 __func__.8906
+    92: 0000000000087524     4 OBJECT  LOCAL  DEFAULT   26 nqi.8916
+    93: 00000000000767b0    24 OBJECT  LOCAL  DEFAULT   18 __func__.8917
+    94: 00000000000767a0    15 OBJECT  LOCAL  DEFAULT   18 __func__.8949
+    95: 0000000000076790    15 OBJECT  LOCAL  DEFAULT   18 __func__.8975
+    96: 0000000000076770    26 OBJECT  LOCAL  DEFAULT   18 __func__.9008
+    97: 0000000000076750    20 OBJECT  LOCAL  DEFAULT   18 __func__.9014
+    98: 0000000000076730    20 OBJECT  LOCAL  DEFAULT   18 __func__.9020
+    99: 0000000000076710    21 OBJECT  LOCAL  DEFAULT   18 __func__.9026
+   100: 00000000000766f0    20 OBJECT  LOCAL  DEFAULT   18 __func__.9045
+   101: 00000000000766d0    20 OBJECT  LOCAL  DEFAULT   18 __func__.9052
+   102: 00000000000766b0    21 OBJECT  LOCAL  DEFAULT   18 __func__.9060
+   103: 0000000000076690    20 OBJECT  LOCAL  DEFAULT   18 __func__.9082
+   104: 0000000000076670    20 OBJECT  LOCAL  DEFAULT   18 __func__.9091
+   105: 0000000000076650    21 OBJECT  LOCAL  DEFAULT   18 __func__.9099
+   106: 0000000000076620    35 OBJECT  LOCAL  DEFAULT   18 __func__.9124
+   107: 00000000000765e0    35 OBJECT  LOCAL  DEFAULT   18 __func__.9136
+   108: 00000000000765a0    34 OBJECT  LOCAL  DEFAULT   18 __func__.9149
+   109: 0000000000076560    34 OBJECT  LOCAL  DEFAULT   18 __func__.9162
+   110: 0000000000076530    19 OBJECT  LOCAL  DEFAULT   18 __func__.9167
    111: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS inout_2d.c
    112: 00000000000183c0  1123 FUNC    LOCAL  DEFAULT   16 MMG2D_saveSol.part.0
    113: 0000000000077568    15 OBJECT  LOCAL  DEFAULT   18 __func__.8632
    114: 0000000000077530    18 OBJECT  LOCAL  DEFAULT   18 __func__.8740
    115: 0000000000077510    18 OBJECT  LOCAL  DEFAULT   18 __func__.8755
    116: 00000000000774f0    30 OBJECT  LOCAL  DEFAULT   18 __func__.8771
    117: 0000000000077550    22 OBJECT  LOCAL  DEFAULT   18 __func__.8714
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: cf8b96e00f79c4b0101cd859a99156f08c7a4793
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 42cc9a5dcaebd6faaa4639b61917addddb0e23b0
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -827,18 +827,18 @@
   Program killed
   -- INPUT DATA
   ** UNABLE TO OPEN %s.
   %%%% %s OPENED
 parameters
 %d Edge %e %e %e 
   -- WRITING COMPLETED
-Dec. 20, 2022
+Dec. 13, 2022
   -- MMG2D, Release %s (%s) 
-14:43:11
-May  8 2023
+15:12:37
+Apr  1 2024
      %s %s
   ** %s  NOT FOUND.
   -- WRITING DATA FILE %s
 MMG2D_countLocalParamAtEdg
 MMG2D_defaultOption
   ## Error: %s: unable to save of a local parameter file with the default parameters values because local parameters are provided.
   ## WARNING: WRONG SOLUTION NUMBER. IGNORED
@@ -1563,15 +1563,15 @@
 SolAtVertices
   ** Defining %stropic map
   -- GRADATION : %8f 
   ## Error: %s: negative hmax value.
   -- GRADATION : DISABLED (%8f)
      git branch: %s
      git commit: %s
-2022-12-20 09:01:29 +0100
+2023-09-17 12:41:34 +0200
      git date:   %s
 Default parameters values:
 ** Generic options :
 **  Parameters
  for material of ref %d
  based references values. 
 ** Generic options
@@ -1580,15 +1580,15 @@
 **  File specifications
 -met file  load metric file
 -ar     val  angle detection
 -nreg        normal regul.
 -xreg        vertex regul.
      Deleted iso edges: %d
    MODULE MMG%s: %s (%s)
-68c6e0c98e755a5cf0a9ccb9a9be6525d0ab0090
+433519f2e628ab4ecd234d66d8e2a1d4cc9f8125
 verbosity                 (-v)      : %d
 maximal memory size       (-m)      : %zu MB
 angle detection           (-ar)     : %lf
 minimal mesh size         (-hmin)   : %lf
 If not yet computed: 0.001 of the mesh bounding box if no metric is provided, 0.1 times the minimum of the metric sizes otherwise.
 maximal mesh size         (-hmax)   : %lf
  If not yet computed: size of the mesh bounding box without metric, 10 times the maximum of the metric sizes otherwise.
@@ -1784,15 +1784,15 @@
   ## Error: %s: at least 1 naive interpolation.
 MMG2D_intmet_ani
 MMG5_interpmet22
 MMG2D_defsiz_iso
   ## Error: %s: at least 1 negative edge length (l1: %e).
   ## Error: %s: at least 1 negative edge length (l2: %e)
 MMG2D_lencurv_ani
-@GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+@GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.2) 9.4.0
 anisomovpt_2d.c
 MMG5_inxt2
 MMG5_iprv2
 mmgWarn0.8093
 __func__.8100
 MMG2D_movintpt_ani.cold
 MMG5_endcod
@@ -1833,46 +1833,46 @@
 __func__.7700
 __func__.7729
 __func__.7811
 __func__.7930
 __func__.7937
 API_functions_2d.c
 __func__.8591
-__func__.8641
-__func__.8656
-__func__.8684
-__func__.8696
-__func__.8708
-__func__.8729
-__func__.8751
-__func__.8786
-__func__.8776
-__func__.8826
-__func__.8855
-__func__.8872
-__func__.8905
-nqi.8915
-__func__.8916
-__func__.8948
-__func__.8974
-__func__.9007
-__func__.9013
-__func__.9019
-__func__.9025
-__func__.9044
-__func__.9051
-__func__.9059
-__func__.9081
-__func__.9090
-__func__.9098
-__func__.9123
-__func__.9135
-__func__.9148
-__func__.9161
-__func__.9166
+__func__.8642
+__func__.8657
+__func__.8685
+__func__.8697
+__func__.8709
+__func__.8730
+__func__.8752
+__func__.8787
+__func__.8777
+__func__.8827
+__func__.8856
+__func__.8873
+__func__.8906
+nqi.8916
+__func__.8917
+__func__.8949
+__func__.8975
+__func__.9008
+__func__.9014
+__func__.9020
+__func__.9026
+__func__.9045
+__func__.9052
+__func__.9060
+__func__.9082
+__func__.9091
+__func__.9099
+__func__.9124
+__func__.9136
+__func__.9149
+__func__.9162
+__func__.9167
 inout_2d.c
 MMG2D_saveSol.part.0
 __func__.8632
 __func__.8740
 __func__.8755
 __func__.8771
 __func__.8714
@@ -1884,14 +1884,15 @@
 __func__.9164
 __func__.9196
 inoutcpp_2d.cpp
 libmmg2d.c
 myfree.part.0
 libmmg2d_tools.c
 __func__.8745
+__func__.8776
 __func__.8806
 __func__.8818
 lissmet_2d.c
 mmgWarn.8069
 __func__.8070
 locate_2d.c
 mmgWarn0.8044
@@ -1919,15 +1920,14 @@
 mmgWarn0.8086
 mmgWarn1.8087
 __func__.8088
 quality_2d.c
 mmgWarn0.8138
 __func__.8147
 solmap_2d.c
-__func__.8657
 __func__.8692
 split_2d.c
 __func__.8160
 __func__.8214
 __func__.8258
 __func__.8310
 __func__.8375
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -38,20 +38,20 @@
   0x00073230 0a002e6d 6d673264 00776200 0a20202a ...mmg2d.wb..  *
   0x00073240 2a20554e 41424c45 20544f20 4f50454e * UNABLE TO OPEN
   0x00073250 2025732e 0a000a20 20252525 25202573  %s....  %%%% %s
   0x00073260 204f5045 4e45440a 00706172 616d6574  OPENED..paramet
   0x00073270 6572730a 2025640a 00256420 45646765 ers. %d..%d Edge
   0x00073280 20256520 25652025 65200a00 20202d2d  %e %e %e ..  --
   0x00073290 20575249 54494e47 20434f4d 504c4554  WRITING COMPLET
-  0x000732a0 45440a00 4465632e 2032302c 20323032 ED..Dec. 20, 202
-  0x000732b0 3200352e 372e3100 20202d2d 204d4d47 2.5.7.1.  -- MMG
+  0x000732a0 45440a00 4465632e 2031332c 20323032 ED..Dec. 13, 202
+  0x000732b0 3200352e 372e3000 20202d2d 204d4d47 2.5.7.0.  -- MMG
   0x000732c0 32442c20 52656c65 61736520 25732028 2D, Release %s (
   0x000732d0 25732920 0a002020 20202025 730a0031 %s) ..     %s..1
-  0x000732e0 343a3433 3a313100 4d617920 20382032 4:43:11.May  8 2
-  0x000732f0 30323300 20202020 20257320 25730a00 023.     %s %s..
+  0x000732e0 353a3132 3a333700 41707220 20312032 5:12:37.Apr  1 2
+  0x000732f0 30323400 20202020 20257320 25730a00 024.     %s %s..
   0x00073300 20202a2a 20257320 204e4f54 20464f55   ** %s  NOT FOU
   0x00073310 4e442e0a 000a2020 2d2d2057 52495449 ND....  -- WRITI
   0x00073320 4e472044 41544120 46494c45 2025730a NG DATA FILE %s.
   0x00073330 00000000 00000000 00000000 00000000 ................
   0x00073340 c864f9ff c864f9ff a664f9ff c864f9ff .d...d...d...d..
   0x00073350 d264f9ff c864f9ff f164f9ff c864f9ff .d...d...d...d..
   0x00073360 1065f9ff c864f9ff c864f9ff 2f65f9ff .e...d...d../e..
@@ -2220,16 +2220,16 @@
   0x0007ba90 206e6567 61746976 6520686d 61782076  negative hmax v
   0x0007baa0 616c7565 2e0a0000 0a20202d 2d204752 alue.....  -- GR
   0x0007bab0 41444154 494f4e20 3a204449 5341424c ADATION : DISABL
   0x0007bac0 45442028 25386629 0a000200 01010200 ED (%8f)........
   0x0007bad0 01020048 45414400 20202020 20676974 ...HEAD.     git
   0x0007bae0 20627261 6e63683a 2025730a 00202020  branch: %s..   
   0x0007baf0 20206769 7420636f 6d6d6974 3a202573   git commit: %s
-  0x0007bb00 0a003230 32322d31 322d3230 2030393a ..2022-12-20 09:
-  0x0007bb10 30313a32 39202b30 31303000 20202020 01:29 +0100.    
+  0x0007bb00 0a003230 32332d30 392d3137 2031323a ..2023-09-17 12:
+  0x0007bb10 34313a33 34202b30 32303000 20202020 41:34 +0200.    
   0x0007bb20 20676974 20646174 653a2020 2025730a  git date:   %s.
   0x0007bb30 0a000a44 65666175 6c742070 6172616d ...Default param
   0x0007bb40 65746572 73207661 6c756573 3a0a000a eters values:...
   0x0007bb50 2a2a2047 656e6572 6963206f 7074696f ** Generic optio
   0x0007bb60 6e73203a 0a000a2a 2a202050 6172616d ns :...**  Param
   0x0007bb70 65746572 730a0020 666f7220 6d617465 eters.. for mate
   0x0007bb80 7269616c 206f6620 72656620 25640a00 rial of ref %d..
@@ -2249,17 +2249,17 @@
   0x0007bc60 6f726d61 6c207265 67756c2e 0a002d78 ormal regul...-x
   0x0007bc70 72656720 20202020 20202076 65727465 reg        verte
   0x0007bc80 78207265 67756c2e 0a002020 20202044 x regul...     D
   0x0007bc90 656c6574 65642069 736f2065 64676573 eleted iso edges
   0x0007bca0 3a202564 0a000000 0a202025 730a2020 : %d.....  %s.  
   0x0007bcb0 204d4f44 554c4520 4d4d4725 733a2025  MODULE MMG%s: %
   0x0007bcc0 73202825 73290a20 2025730a 00000000 s (%s).  %s.....
-  0x0007bcd0 36386336 65306339 38653735 35613563 68c6e0c98e755a5c
-  0x0007bce0 66306139 63636239 61396265 36353235 f0a9ccb9a9be6525
-  0x0007bcf0 64306162 30303930 00000000 00000000 d0ab0090........
+  0x0007bcd0 34333335 31396632 65363238 61623465 433519f2e628ab4e
+  0x0007bce0 63643233 34643636 64386532 61316434 cd234d66d8e2a1d4
+  0x0007bcf0 63633966 38313235 00000000 00000000 cc9f8125........
   0x0007bd00 76657262 6f736974 79202020 20202020 verbosity       
   0x0007bd10 20202020 20202020 2020282d 76292020           (-v)  
   0x0007bd20 20202020 3a202564 0a000000 00000000     : %d........
   0x0007bd30 6d617869 6d616c20 6d656d6f 72792073 maximal memory s
   0x0007bd40 697a6520 20202020 2020282d 6d292020 ize       (-m)  
   0x0007bd50 20202020 3a20257a 75204d42 0a000000     : %zu MB....
   0x0007bd60 616e676c 65206465 74656374 696f6e20 angle detection
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+  [     0]  GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.2) 9.4.0
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -42,42 +42,42 @@
   0x00000270 36005f5f 66756e63 5f5f2e37 37303000 6.__func__.7700.
   0x00000280 5f5f6675 6e635f5f 2e373732 39005f5f __func__.7729.__
   0x00000290 66756e63 5f5f2e37 38313100 5f5f6675 func__.7811.__fu
   0x000002a0 6e635f5f 2e373933 30005f5f 66756e63 nc__.7930.__func
   0x000002b0 5f5f2e37 39333700 4150495f 66756e63 __.7937.API_func
   0x000002c0 74696f6e 735f3264 2e63005f 5f66756e tions_2d.c.__fun
   0x000002d0 635f5f2e 38353931 005f5f66 756e635f c__.8591.__func_
-  0x000002e0 5f2e3836 3431005f 5f66756e 635f5f2e _.8641.__func__.
-  0x000002f0 38363536 005f5f66 756e635f 5f2e3836 8656.__func__.86
-  0x00000300 3834005f 5f66756e 635f5f2e 38363936 84.__func__.8696
-  0x00000310 005f5f66 756e635f 5f2e3837 3038005f .__func__.8708._
-  0x00000320 5f66756e 635f5f2e 38373239 005f5f66 _func__.8729.__f
-  0x00000330 756e635f 5f2e3837 3531005f 5f66756e unc__.8751.__fun
-  0x00000340 635f5f2e 38373836 005f5f66 756e635f c__.8786.__func_
-  0x00000350 5f2e3837 3736005f 5f66756e 635f5f2e _.8776.__func__.
-  0x00000360 38383236 005f5f66 756e635f 5f2e3838 8826.__func__.88
-  0x00000370 3535005f 5f66756e 635f5f2e 38383732 55.__func__.8872
-  0x00000380 005f5f66 756e635f 5f2e3839 3035006e .__func__.8905.n
-  0x00000390 71692e38 39313500 5f5f6675 6e635f5f qi.8915.__func__
-  0x000003a0 2e383931 36005f5f 66756e63 5f5f2e38 .8916.__func__.8
-  0x000003b0 39343800 5f5f6675 6e635f5f 2e383937 948.__func__.897
-  0x000003c0 34005f5f 66756e63 5f5f2e39 30303700 4.__func__.9007.
-  0x000003d0 5f5f6675 6e635f5f 2e393031 33005f5f __func__.9013.__
-  0x000003e0 66756e63 5f5f2e39 30313900 5f5f6675 func__.9019.__fu
-  0x000003f0 6e635f5f 2e393032 35005f5f 66756e63 nc__.9025.__func
-  0x00000400 5f5f2e39 30343400 5f5f6675 6e635f5f __.9044.__func__
-  0x00000410 2e393035 31005f5f 66756e63 5f5f2e39 .9051.__func__.9
-  0x00000420 30353900 5f5f6675 6e635f5f 2e393038 059.__func__.908
-  0x00000430 31005f5f 66756e63 5f5f2e39 30393000 1.__func__.9090.
-  0x00000440 5f5f6675 6e635f5f 2e393039 38005f5f __func__.9098.__
-  0x00000450 66756e63 5f5f2e39 31323300 5f5f6675 func__.9123.__fu
-  0x00000460 6e635f5f 2e393133 35005f5f 66756e63 nc__.9135.__func
-  0x00000470 5f5f2e39 31343800 5f5f6675 6e635f5f __.9148.__func__
-  0x00000480 2e393136 31005f5f 66756e63 5f5f2e39 .9161.__func__.9
-  0x00000490 31363600 696e6f75 745f3264 2e63004d 166.inout_2d.c.M
+  0x000002e0 5f2e3836 3432005f 5f66756e 635f5f2e _.8642.__func__.
+  0x000002f0 38363537 005f5f66 756e635f 5f2e3836 8657.__func__.86
+  0x00000300 3835005f 5f66756e 635f5f2e 38363937 85.__func__.8697
+  0x00000310 005f5f66 756e635f 5f2e3837 3039005f .__func__.8709._
+  0x00000320 5f66756e 635f5f2e 38373330 005f5f66 _func__.8730.__f
+  0x00000330 756e635f 5f2e3837 3532005f 5f66756e unc__.8752.__fun
+  0x00000340 635f5f2e 38373837 005f5f66 756e635f c__.8787.__func_
+  0x00000350 5f2e3837 3737005f 5f66756e 635f5f2e _.8777.__func__.
+  0x00000360 38383237 005f5f66 756e635f 5f2e3838 8827.__func__.88
+  0x00000370 3536005f 5f66756e 635f5f2e 38383733 56.__func__.8873
+  0x00000380 005f5f66 756e635f 5f2e3839 3036006e .__func__.8906.n
+  0x00000390 71692e38 39313600 5f5f6675 6e635f5f qi.8916.__func__
+  0x000003a0 2e383931 37005f5f 66756e63 5f5f2e38 .8917.__func__.8
+  0x000003b0 39343900 5f5f6675 6e635f5f 2e383937 949.__func__.897
+  0x000003c0 35005f5f 66756e63 5f5f2e39 30303800 5.__func__.9008.
+  0x000003d0 5f5f6675 6e635f5f 2e393031 34005f5f __func__.9014.__
+  0x000003e0 66756e63 5f5f2e39 30323000 5f5f6675 func__.9020.__fu
+  0x000003f0 6e635f5f 2e393032 36005f5f 66756e63 nc__.9026.__func
+  0x00000400 5f5f2e39 30343500 5f5f6675 6e635f5f __.9045.__func__
+  0x00000410 2e393035 32005f5f 66756e63 5f5f2e39 .9052.__func__.9
+  0x00000420 30363000 5f5f6675 6e635f5f 2e393038 060.__func__.908
+  0x00000430 32005f5f 66756e63 5f5f2e39 30393100 2.__func__.9091.
+  0x00000440 5f5f6675 6e635f5f 2e393039 39005f5f __func__.9099.__
+  0x00000450 66756e63 5f5f2e39 31323400 5f5f6675 func__.9124.__fu
+  0x00000460 6e635f5f 2e393133 36005f5f 66756e63 nc__.9136.__func
+  0x00000470 5f5f2e39 31343900 5f5f6675 6e635f5f __.9149.__func__
+  0x00000480 2e393136 32005f5f 66756e63 5f5f2e39 .9162.__func__.9
+  0x00000490 31363700 696e6f75 745f3264 2e63004d 167.inout_2d.c.M
   0x000004a0 4d473244 5f736176 65536f6c 2e706172 MG2D_saveSol.par
   0x000004b0 742e3000 5f5f6675 6e635f5f 2e383633 t.0.__func__.863
   0x000004c0 32005f5f 66756e63 5f5f2e38 37343000 2.__func__.8740.
   0x000004d0 5f5f6675 6e635f5f 2e383735 35005f5f __func__.8755.__
   0x000004e0 66756e63 5f5f2e38 37373100 5f5f6675 func__.8771.__fu
   0x000004f0 6e635f5f 2e383731 34006d6d 67576172 nc__.8714.mmgWar
   0x00000500 6e2e3838 3434005f 5f66756e 635f5f2e n.8844.__func__.
@@ -86,45 +86,45 @@
   0x00000530 005f5f66 756e635f 5f2e3931 3831005f .__func__.9181._
   0x00000540 5f66756e 635f5f2e 39313634 005f5f66 _func__.9164.__f
   0x00000550 756e635f 5f2e3931 39360069 6e6f7574 unc__.9196.inout
   0x00000560 6370705f 32642e63 7070006c 69626d6d cpp_2d.cpp.libmm
   0x00000570 6732642e 63006d79 66726565 2e706172 g2d.c.myfree.par
   0x00000580 742e3000 6c69626d 6d673264 5f746f6f t.0.libmmg2d_too
   0x00000590 6c732e63 005f5f66 756e635f 5f2e3837 ls.c.__func__.87
-  0x000005a0 3435005f 5f66756e 635f5f2e 38383036 45.__func__.8806
-  0x000005b0 005f5f66 756e635f 5f2e3838 3138006c .__func__.8818.l
-  0x000005c0 6973736d 65745f32 642e6300 6d6d6757 issmet_2d.c.mmgW
-  0x000005d0 61726e2e 38303639 005f5f66 756e635f arn.8069.__func_
-  0x000005e0 5f2e3830 3730006c 6f636174 655f3264 _.8070.locate_2d
-  0x000005f0 2e63006d 6d675761 726e302e 38303434 .c.mmgWarn0.8044
-  0x00000600 005f5f66 756e635f 5f2e3830 3435006d .__func__.8045.m
-  0x00000610 6d675761 726e302e 38313234 005f5f66 mgWarn0.8124.__f
-  0x00000620 756e635f 5f2e3831 3236006d 6d675761 unc__.8126.mmgWa
-  0x00000630 726e2e38 31373300 5f5f6675 6e635f5f rn.8173.__func__
-  0x00000640 2e383137 39006d6d 67326431 2e63004d .8179.mmg2d1.c.M
-  0x00000650 4d473244 5f6d6f76 7472692e 636f6e73 MG2D_movtri.cons
-  0x00000660 7470726f 702e3000 5f5f6675 6e635f5f tprop.0.__func__
-  0x00000670 2e383131 33006d6d 67576172 6e302e38 .8113.mmgWarn0.8
-  0x00000680 31303200 6d6d6732 64322e63 005f5f66 102.mmg2d2.c.__f
-  0x00000690 756e635f 5f2e3831 3031006d 6d675761 unc__.8101.mmgWa
-  0x000006a0 726e302e 38303935 006d6d67 5761726e rn0.8095.mmgWarn
-  0x000006b0 322e3831 3638006d 6d675761 726e312e 2.8168.mmgWarn1.
-  0x000006c0 38313637 005f5f66 756e635f 5f2e3831 8167.__func__.81
-  0x000006d0 3735006d 6d675761 726e302e 38313435 75.mmgWarn0.8145
-  0x000006e0 005f5f66 756e635f 5f2e3831 3531005f .__func__.8151._
-  0x000006f0 5f66756e 635f5f2e 38323834 006d6d67 _func__.8284.mmg
-  0x00000700 3264362e 63005f5f 66756e63 5f5f2e38 2d6.c.__func__.8
-  0x00000710 31343400 6d6d6732 64657874 65726e73 144.mmg2dexterns
-  0x00000720 2e63006d 6d675761 726e302e 38303836 .c.mmgWarn0.8086
-  0x00000730 006d6d67 5761726e 312e3830 3837005f .mmgWarn1.8087._
-  0x00000740 5f66756e 635f5f2e 38303838 00717561 _func__.8088.qua
-  0x00000750 6c697479 5f32642e 63006d6d 67576172 lity_2d.c.mmgWar
-  0x00000760 6e302e38 31333800 5f5f6675 6e635f5f n0.8138.__func__
-  0x00000770 2e383134 3700736f 6c6d6170 5f32642e .8147.solmap_2d.
-  0x00000780 63005f5f 66756e63 5f5f2e38 36353700 c.__func__.8657.
+  0x000005a0 3435005f 5f66756e 635f5f2e 38373736 45.__func__.8776
+  0x000005b0 005f5f66 756e635f 5f2e3838 3036005f .__func__.8806._
+  0x000005c0 5f66756e 635f5f2e 38383138 006c6973 _func__.8818.lis
+  0x000005d0 736d6574 5f32642e 63006d6d 67576172 smet_2d.c.mmgWar
+  0x000005e0 6e2e3830 3639005f 5f66756e 635f5f2e n.8069.__func__.
+  0x000005f0 38303730 006c6f63 6174655f 32642e63 8070.locate_2d.c
+  0x00000600 006d6d67 5761726e 302e3830 3434005f .mmgWarn0.8044._
+  0x00000610 5f66756e 635f5f2e 38303435 006d6d67 _func__.8045.mmg
+  0x00000620 5761726e 302e3831 3234005f 5f66756e Warn0.8124.__fun
+  0x00000630 635f5f2e 38313236 006d6d67 5761726e c__.8126.mmgWarn
+  0x00000640 2e383137 33005f5f 66756e63 5f5f2e38 .8173.__func__.8
+  0x00000650 31373900 6d6d6732 64312e63 004d4d47 179.mmg2d1.c.MMG
+  0x00000660 32445f6d 6f767472 692e636f 6e737470 2D_movtri.constp
+  0x00000670 726f702e 30005f5f 66756e63 5f5f2e38 rop.0.__func__.8
+  0x00000680 31313300 6d6d6757 61726e30 2e383130 113.mmgWarn0.810
+  0x00000690 32006d6d 67326432 2e63005f 5f66756e 2.mmg2d2.c.__fun
+  0x000006a0 635f5f2e 38313031 006d6d67 5761726e c__.8101.mmgWarn
+  0x000006b0 302e3830 3935006d 6d675761 726e322e 0.8095.mmgWarn2.
+  0x000006c0 38313638 006d6d67 5761726e 312e3831 8168.mmgWarn1.81
+  0x000006d0 3637005f 5f66756e 635f5f2e 38313735 67.__func__.8175
+  0x000006e0 006d6d67 5761726e 302e3831 3435005f .mmgWarn0.8145._
+  0x000006f0 5f66756e 635f5f2e 38313531 005f5f66 _func__.8151.__f
+  0x00000700 756e635f 5f2e3832 3834006d 6d673264 unc__.8284.mmg2d
+  0x00000710 362e6300 5f5f6675 6e635f5f 2e383134 6.c.__func__.814
+  0x00000720 34006d6d 67326465 78746572 6e732e63 4.mmg2dexterns.c
+  0x00000730 006d6d67 5761726e 302e3830 3836006d .mmgWarn0.8086.m
+  0x00000740 6d675761 726e312e 38303837 005f5f66 mgWarn1.8087.__f
+  0x00000750 756e635f 5f2e3830 38380071 75616c69 unc__.8088.quali
+  0x00000760 74795f32 642e6300 6d6d6757 61726e30 ty_2d.c.mmgWarn0
+  0x00000770 2e383133 38005f5f 66756e63 5f5f2e38 .8138.__func__.8
+  0x00000780 31343700 736f6c6d 61705f32 642e6300 147.solmap_2d.c.
   0x00000790 5f5f6675 6e635f5f 2e383639 32007370 __func__.8692.sp
   0x000007a0 6c69745f 32642e63 005f5f66 756e635f lit_2d.c.__func_
   0x000007b0 5f2e3831 3630005f 5f66756e 635f5f2e _.8160.__func__.
   0x000007c0 38323134 005f5f66 756e635f 5f2e3832 8214.__func__.82
   0x000007d0 3538005f 5f66756e 635f5f2e 38333130 58.__func__.8310
   0x000007e0 005f5f66 756e635f 5f2e3833 37350073 .__func__.8375.s
   0x000007f0 77617061 725f3264 2e630074 6f6f6c73 wapar_2d.c.tools
```

### Comparing `pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/mmg3d_O3` & `pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/mmg3d_O3`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --symbols {}

```diff
@@ -840,17 +840,17 @@
    105: 00000000000f1c80    35 OBJECT  LOCAL  DEFAULT   18 __func__.10782
    106: 00000000000f1c40    35 OBJECT  LOCAL  DEFAULT   18 __func__.10794
    107: 00000000000f1c20    19 OBJECT  LOCAL  DEFAULT   18 __func__.10807
    108: 00000000000f1c00    22 OBJECT  LOCAL  DEFAULT   18 __func__.10852
    109: 00000000000f1be0    17 OBJECT  LOCAL  DEFAULT   18 __func__.10886
    110: 00000000000f1bc0    21 OBJECT  LOCAL  DEFAULT   18 __func__.10902
    111: 00000000000f1ba8    14 OBJECT  LOCAL  DEFAULT   18 __func__.10816
-   112: 00000000000f1b90    21 OBJECT  LOCAL  DEFAULT   18 __func__.10961
-   113: 00000000000f1b70    21 OBJECT  LOCAL  DEFAULT   18 __func__.10976
-   114: 00000000000f1b50    25 OBJECT  LOCAL  DEFAULT   18 __func__.10991
+   112: 00000000000f1b90    21 OBJECT  LOCAL  DEFAULT   18 __func__.10962
+   113: 00000000000f1b70    21 OBJECT  LOCAL  DEFAULT   18 __func__.10977
+   114: 00000000000f1b50    25 OBJECT  LOCAL  DEFAULT   18 __func__.10992
    115: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS anisosiz_3d.c
    116: 000000000001dc80   615 FUNC    LOCAL  DEFAULT   16 MMG5_lenedgCoor_ani
    117: 000000000001def0  1368 FUNC    LOCAL  DEFAULT   16 MMG5_defmetvol
    118: 000000000001e450  2223 FUNC    LOCAL  DEFAULT   16 MMG5_lenSurfEdg_ani
    119: 000000000010c575     1 OBJECT  LOCAL  DEFAULT   26 mmgWarn.9743
    120: 00000000000f2548    12 OBJECT  LOCAL  DEFAULT   18 __func__.9744
    121: 000000000010c576     1 OBJECT  LOCAL  DEFAULT   26 mmgWarn.9762
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 9d45394b1508c8205c90be24681c0f25b6f4dd11
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: de86bc0b96d3ec011937f9f399ce998ac12f6e98
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -1362,18 +1362,18 @@
   *** Program killed
 %d Tetrahedron %e %e %e 
   ** UNABLE TO OPEN %s.
   %%%% %s OPENED
 parameters
   -- WRITING COMPLETED
   -- INPUT DATA
-Dec. 20, 2022
+Dec. 13, 2022
   -- MMG3D, Release %s (%s) 
-14:43:37
-May  8 2023
+15:12:45
+Apr  1 2024
      %s %s
   ** %s  NOT FOUND.
   -- WRITING DATA FILE %s
   *** potential lack of memory.
   *** Floating-point exception
   ## Warning: %s: unable to list the tetra references.
               Uncomplete parameters file.
@@ -2338,15 +2338,15 @@
 SolAtVertices
   ** Defining %stropic map
   -- GRADATION : %8f 
   ## Error: %s: negative hmax value.
   -- GRADATION : DISABLED (%8f)
      git branch: %s
      git commit: %s
-2022-12-20 09:01:29 +0100
+2023-09-17 12:41:34 +0200
      git date:   %s
 Default parameters values:
 ** Generic options :
 **  Parameters
  for material of ref %d
  based references values. 
 ** Generic options
@@ -2355,15 +2355,15 @@
 **  File specifications
 -met file  load metric file
 -ar     val  angle detection
 -nreg        normal regul.
 -xreg        vertex regul.
      Deleted iso edges: %d
    MODULE MMG%s: %s (%s)
-68c6e0c98e755a5cf0a9ccb9a9be6525d0ab0090
+433519f2e628ab4ecd234d66d8e2a1d4cc9f8125
 verbosity                 (-v)      : %d
 maximal memory size       (-m)      : %zu MB
 angle detection           (-ar)     : %lf
 minimal mesh size         (-hmin)   : %lf
 If not yet computed: 0.001 of the mesh bounding box if no metric is provided, 0.1 times the minimum of the metric sizes otherwise.
 maximal mesh size         (-hmax)   : %lf
  If not yet computed: size of the mesh bounding box without metric, 10 times the maximum of the metric sizes otherwise.
@@ -2606,15 +2606,15 @@
          %d: %e %e %e (tag %s)
  AFTER ROTATION (to %e %e %e):
  BEFORE ROTATION:
  metric %e %e %e %e %e %e
      %e %e %e %e %e %e
 MMG5_interpreg_ani
 MMG5_mmgIntmet33_ani
-?GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+?GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.2) 9.4.0
 MMG5_endcod
 MMG5_excfun
 __func__.9733
 MMG3D_defaultOption
 __func__.9764
 crtstuff.c
 deregister_tm_clones
@@ -2688,17 +2688,17 @@
 __func__.10782
 __func__.10794
 __func__.10807
 __func__.10852
 __func__.10886
 __func__.10902
 __func__.10816
-__func__.10961
-__func__.10976
-__func__.10991
+__func__.10962
+__func__.10977
+__func__.10992
 anisosiz_3d.c
 MMG5_lenedgCoor_ani
 MMG5_defmetvol
 MMG5_lenSurfEdg_ani
 mmgWarn.9743
 __func__.9744
 mmgWarn.9762
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -36,20 +36,20 @@
   0x000ee210 20256520 2565200a 002e6d6d 67336400  %e %e ...mmg3d.
   0x000ee220 7762000a 20202a2a 20554e41 424c4520 wb..  ** UNABLE 
   0x000ee230 544f204f 50454e20 25732e0a 000a2020 TO OPEN %s....  
   0x000ee240 25252525 20257320 4f50454e 45440a00 %%%% %s OPENED..
   0x000ee250 70617261 6d657465 72730a20 25640a00 parameters. %d..
   0x000ee260 20202d2d 20575249 54494e47 20434f4d   -- WRITING COM
   0x000ee270 504c4554 45440a00 0a20202d 2d20494e PLETED...  -- IN
-  0x000ee280 50555420 44415441 0a004465 632e2032 PUT DATA..Dec. 2
-  0x000ee290 302c2032 30323200 352e372e 31002020 0, 2022.5.7.1.  
+  0x000ee280 50555420 44415441 0a004465 632e2031 PUT DATA..Dec. 1
+  0x000ee290 332c2032 30323200 352e372e 30002020 3, 2022.5.7.0.  
   0x000ee2a0 2d2d204d 4d473344 2c205265 6c656173 -- MMG3D, Releas
   0x000ee2b0 65202573 20282573 29200a00 20202020 e %s (%s) ..    
-  0x000ee2c0 2025730a 0031343a 34333a33 37004d61  %s..14:43:37.Ma
-  0x000ee2d0 79202038 20323032 33002020 20202025 y  8 2023.     %
+  0x000ee2c0 2025730a 0031353a 31323a34 35004170  %s..15:12:45.Ap
+  0x000ee2d0 72202031 20323032 34002020 20202025 r  1 2024.     %
   0x000ee2e0 73202573 0a002020 2a2a2025 7320204e s %s..  ** %s  N
   0x000ee2f0 4f542046 4f554e44 2e0a000a 20202d2d OT FOUND....  --
   0x000ee300 20575249 54494e47 20444154 41204649  WRITING DATA FI
   0x000ee310 4c452025 730a0000 20202a2a 2a20706f LE %s...  *** po
   0x000ee320 74656e74 69616c20 6c61636b 206f6620 tential lack of 
   0x000ee330 6d656d6f 72792e0a 00000000 00000000 memory..........
   0x000ee340 20202a2a 2a20466c 6f617469 6e672d70   *** Floating-p
@@ -3222,16 +3222,16 @@
   0x000fa930 206e6567 61746976 6520686d 61782076  negative hmax v
   0x000fa940 616c7565 2e0a0000 0a20202d 2d204752 alue.....  -- GR
   0x000fa950 41444154 494f4e20 3a204449 5341424c ADATION : DISABL
   0x000fa960 45442028 25386629 0a000200 01010200 ED (%8f)........
   0x000fa970 01020048 45414400 20202020 20676974 ...HEAD.     git
   0x000fa980 20627261 6e63683a 2025730a 00202020  branch: %s..   
   0x000fa990 20206769 7420636f 6d6d6974 3a202573   git commit: %s
-  0x000fa9a0 0a003230 32322d31 322d3230 2030393a ..2022-12-20 09:
-  0x000fa9b0 30313a32 39202b30 31303000 20202020 01:29 +0100.    
+  0x000fa9a0 0a003230 32332d30 392d3137 2031323a ..2023-09-17 12:
+  0x000fa9b0 34313a33 34202b30 32303000 20202020 41:34 +0200.    
   0x000fa9c0 20676974 20646174 653a2020 2025730a  git date:   %s.
   0x000fa9d0 0a000a44 65666175 6c742070 6172616d ...Default param
   0x000fa9e0 65746572 73207661 6c756573 3a0a000a eters values:...
   0x000fa9f0 2a2a2047 656e6572 6963206f 7074696f ** Generic optio
   0x000faa00 6e73203a 0a000a2a 2a202050 6172616d ns :...**  Param
   0x000faa10 65746572 730a0020 666f7220 6d617465 eters.. for mate
   0x000faa20 7269616c 206f6620 72656620 25640a00 rial of ref %d..
@@ -3251,17 +3251,17 @@
   0x000fab00 6f726d61 6c207265 67756c2e 0a002d78 ormal regul...-x
   0x000fab10 72656720 20202020 20202076 65727465 reg        verte
   0x000fab20 78207265 67756c2e 0a002020 20202044 x regul...     D
   0x000fab30 656c6574 65642069 736f2065 64676573 eleted iso edges
   0x000fab40 3a202564 0a000000 0a202025 730a2020 : %d.....  %s.  
   0x000fab50 204d4f44 554c4520 4d4d4725 733a2025  MODULE MMG%s: %
   0x000fab60 73202825 73290a20 2025730a 00000000 s (%s).  %s.....
-  0x000fab70 36386336 65306339 38653735 35613563 68c6e0c98e755a5c
-  0x000fab80 66306139 63636239 61396265 36353235 f0a9ccb9a9be6525
-  0x000fab90 64306162 30303930 00000000 00000000 d0ab0090........
+  0x000fab70 34333335 31396632 65363238 61623465 433519f2e628ab4e
+  0x000fab80 63643233 34643636 64386532 61316434 cd234d66d8e2a1d4
+  0x000fab90 63633966 38313235 00000000 00000000 cc9f8125........
   0x000faba0 76657262 6f736974 79202020 20202020 verbosity       
   0x000fabb0 20202020 20202020 2020282d 76292020           (-v)  
   0x000fabc0 20202020 3a202564 0a000000 00000000     : %d........
   0x000fabd0 6d617869 6d616c20 6d656d6f 72792073 maximal memory s
   0x000fabe0 697a6520 20202020 2020282d 6d292020 ize       (-m)  
   0x000fabf0 20202020 3a20257a 75204d42 0a000000     : %zu MB....
   0x000fac00 616e676c 65206465 74656374 696f6e20 angle detection
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+  [     0]  GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.2) 9.4.0
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -72,17 +72,17 @@
   0x00000450 31303737 30005f5f 66756e63 5f5f2e31 10770.__func__.1
   0x00000460 30373832 005f5f66 756e635f 5f2e3130 0782.__func__.10
   0x00000470 37393400 5f5f6675 6e635f5f 2e313038 794.__func__.108
   0x00000480 3037005f 5f66756e 635f5f2e 31303835 07.__func__.1085
   0x00000490 32005f5f 66756e63 5f5f2e31 30383836 2.__func__.10886
   0x000004a0 005f5f66 756e635f 5f2e3130 39303200 .__func__.10902.
   0x000004b0 5f5f6675 6e635f5f 2e313038 3136005f __func__.10816._
-  0x000004c0 5f66756e 635f5f2e 31303936 31005f5f _func__.10961.__
-  0x000004d0 66756e63 5f5f2e31 30393736 005f5f66 func__.10976.__f
-  0x000004e0 756e635f 5f2e3130 39393100 616e6973 unc__.10991.anis
+  0x000004c0 5f66756e 635f5f2e 31303936 32005f5f _func__.10962.__
+  0x000004d0 66756e63 5f5f2e31 30393737 005f5f66 func__.10977.__f
+  0x000004e0 756e635f 5f2e3130 39393200 616e6973 unc__.10992.anis
   0x000004f0 6f73697a 5f33642e 63004d4d 47355f6c osiz_3d.c.MMG5_l
   0x00000500 656e6564 67436f6f 725f616e 69004d4d enedgCoor_ani.MM
   0x00000510 47355f64 65666d65 74766f6c 004d4d47 G5_defmetvol.MMG
   0x00000520 355f6c65 6e537572 66456467 5f616e69 5_lenSurfEdg_ani
   0x00000530 006d6d67 5761726e 2e393734 33005f5f .mmgWarn.9743.__
   0x00000540 66756e63 5f5f2e39 37343400 6d6d6757 func__.9744.mmgW
   0x00000550 61726e2e 39373632 005f5f66 756e635f arn.9762.__func_
```

### Comparing `pymmg-0.1.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/mmgs_O3` & `pymmg-1.0.0/_skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/mmgs_O3`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --symbols {}

```diff
@@ -585,17 +585,17 @@
     92: 0000000000076330    20 OBJECT  LOCAL  DEFAULT   18 __func__.8765
     93: 0000000000076300    33 OBJECT  LOCAL  DEFAULT   18 __func__.8791
     94: 00000000000762c0    33 OBJECT  LOCAL  DEFAULT   18 __func__.8804
     95: 0000000000076280    34 OBJECT  LOCAL  DEFAULT   18 __func__.8816
     96: 0000000000076240    34 OBJECT  LOCAL  DEFAULT   18 __func__.8828
     97: 0000000000076220    18 OBJECT  LOCAL  DEFAULT   18 __func__.8833
     98: 0000000000076200    20 OBJECT  LOCAL  DEFAULT   18 __func__.8844
-    99: 00000000000761e0    20 OBJECT  LOCAL  DEFAULT   18 __func__.8889
-   100: 00000000000761c0    20 OBJECT  LOCAL  DEFAULT   18 __func__.8904
-   101: 00000000000761a0    24 OBJECT  LOCAL  DEFAULT   18 __func__.8919
+    99: 00000000000761e0    20 OBJECT  LOCAL  DEFAULT   18 __func__.8890
+   100: 00000000000761c0    20 OBJECT  LOCAL  DEFAULT   18 __func__.8905
+   101: 00000000000761a0    24 OBJECT  LOCAL  DEFAULT   18 __func__.8920
    102: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS inout_s.c
    103: 0000000000017080    21 FUNC    LOCAL  DEFAULT   16 myfree.part.0
    104: 0000000000076ea8    14 OBJECT  LOCAL  DEFAULT   18 __func__.8493
    105: 0000000000076e90    21 OBJECT  LOCAL  DEFAULT   18 __func__.8593
    106: 0000000000086562     1 OBJECT  LOCAL  DEFAULT   26 mmgWarn.8726
    107: 0000000000076e70    17 OBJECT  LOCAL  DEFAULT   18 __func__.8727
    108: 0000000000076e58    13 OBJECT  LOCAL  DEFAULT   18 __func__.8756
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 4cd1536294b429786f9b687fb806bfbe0bec7c8f
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0844b27667e38d6bb865e1abc8f81af1c9da8a77
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -782,18 +782,18 @@
   %%%% Wrong format: %s
 triangle
 lsbasereferences
   -- INPUT DATA
   ** UNABLE TO OPEN %s.
 parameters
   -- WRITING COMPLETED
-Dec. 20, 2022
+Dec. 13, 2022
   -- MMGS, Release %s (%s) 
-14:43:20
-May  8 2023
+15:12:32
+Apr  1 2024
      %s %s
   ** %s  NOT FOUND.
   -- WRITING DATA FILE %s
   *** potential lack of memory.
   *** Floating-point exception
   %%%% Wrong format for lsreferences: %d
 Reading error: fscanf counts %d args while %d provided
@@ -1451,15 +1451,15 @@
   ** Defining %stropic map
   -- GRADATION : %8f 
   ** Grading mesh
   ## Error: %s: negative hmax value.
   -- GRADATION : DISABLED (%8f)
      git branch: %s
      git commit: %s
-2022-12-20 09:01:29 +0100
+2023-09-17 12:41:34 +0200
      git date:   %s
 Default parameters values:
 ** Generic options :
 **  Parameters
  for material of ref %d
  based references values. 
 ** Generic options
@@ -1468,15 +1468,15 @@
 **  File specifications
 -met file  load metric file
 -ar     val  angle detection
 -nreg        normal regul.
 -xreg        vertex regul.
      Deleted iso edges: %d
    MODULE MMG%s: %s (%s)
-68c6e0c98e755a5cf0a9ccb9a9be6525d0ab0090
+433519f2e628ab4ecd234d66d8e2a1d4cc9f8125
 verbosity                 (-v)      : %d
 maximal memory size       (-m)      : %zu MB
 angle detection           (-ar)     : %lf
 minimal mesh size         (-hmin)   : %lf
 If not yet computed: 0.001 of the mesh bounding box if no metric is provided, 0.1 times the minimum of the metric sizes otherwise.
 maximal mesh size         (-hmax)   : %lf
  If not yet computed: size of the mesh bounding box without metric, 10 times the maximum of the metric sizes otherwise.
@@ -1651,15 +1651,15 @@
          %d: %e %e %e (tag %s)
  AFTER ROTATION (to %e %e %e):
  BEFORE ROTATION:
  metric %e %e %e %e %e %e
      %e %e %e %e %e %e
 MMG5_interpreg_ani
 MMG5_mmgIntmet33_ani
-?GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+?GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.2) 9.4.0
 MMG5_endcod
 MMG5_excfun
 MMG5_parsop
 MMGS_defaultOption
 __func__.8466
 crtstuff.c
 deregister_tm_clones
@@ -1720,17 +1720,17 @@
 __func__.8765
 __func__.8791
 __func__.8804
 __func__.8816
 __func__.8828
 __func__.8833
 __func__.8844
-__func__.8889
-__func__.8904
-__func__.8919
+__func__.8890
+__func__.8905
+__func__.8920
 inout_s.c
 myfree.part.0
 __func__.8493
 __func__.8593
 mmgWarn.8726
 __func__.8727
 __func__.8756
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -42,20 +42,20 @@
   0x00073270 25730a00 74726961 6e676c65 006c7362 %s..triangle.lsb
   0x00073280 61736572 65666572 656e6365 73000a20 asereferences.. 
   0x00073290 202d2d20 494e5055 54204441 54410a00  -- INPUT DATA..
   0x000732a0 7762000a 20202a2a 20554e41 424c4520 wb..  ** UNABLE 
   0x000732b0 544f204f 50454e20 25732e0a 00706172 TO OPEN %s...par
   0x000732c0 616d6574 6572730a 2025640a 0020202d ameters. %d..  -
   0x000732d0 2d205752 4954494e 4720434f 4d504c45 - WRITING COMPLE
-  0x000732e0 5445440a 00446563 2e203230 2c203230 TED..Dec. 20, 20
-  0x000732f0 32320035 2e372e31 0020202d 2d204d4d 22.5.7.1.  -- MM
+  0x000732e0 5445440a 00446563 2e203133 2c203230 TED..Dec. 13, 20
+  0x000732f0 32320035 2e372e30 0020202d 2d204d4d 22.5.7.0.  -- MM
   0x00073300 47532c20 52656c65 61736520 25732028 GS, Release %s (
   0x00073310 25732920 0a002020 20202025 730a0031 %s) ..     %s..1
-  0x00073320 343a3433 3a323000 4d617920 20382032 4:43:20.May  8 2
-  0x00073330 30323300 20202020 20257320 25730a00 023.     %s %s..
+  0x00073320 353a3132 3a333200 41707220 20312032 5:12:32.Apr  1 2
+  0x00073330 30323400 20202020 20257320 25730a00 024.     %s %s..
   0x00073340 20202a2a 20257320 204e4f54 20464f55   ** %s  NOT FOU
   0x00073350 4e442e0a 000a2020 2d2d2057 52495449 ND....  -- WRITI
   0x00073360 4e472044 41544120 46494c45 2025730a NG DATA FILE %s.
   0x00073370 00000000 00000000 20202a2a 2a20706f ........  *** po
   0x00073380 74656e74 69616c20 6c61636b 206f6620 tential lack of 
   0x00073390 6d656d6f 72792e0a 00000000 00000000 memory..........
   0x000733a0 20202a2a 2a20466c 6f617469 6e672d70   *** Floating-p
@@ -2028,17 +2028,17 @@
   0x0007ae90 726f723a 2025733a 206e6567 61746976 ror: %s: negativ
   0x0007aea0 6520686d 61782076 616c7565 2e0a0000 e hmax value....
   0x0007aeb0 0a20202d 2d204752 41444154 494f4e20 .  -- GRADATION 
   0x0007aec0 3a204449 5341424c 45442028 25386629 : DISABLED (%8f)
   0x0007aed0 0a000200 01010200 01020048 45414400 ...........HEAD.
   0x0007aee0 20202020 20676974 20627261 6e63683a      git branch:
   0x0007aef0 2025730a 00202020 20206769 7420636f  %s..     git co
-  0x0007af00 6d6d6974 3a202573 0a003230 32322d31 mmit: %s..2022-1
-  0x0007af10 322d3230 2030393a 30313a32 39202b30 2-20 09:01:29 +0
-  0x0007af20 31303000 20202020 20676974 20646174 100.     git dat
+  0x0007af00 6d6d6974 3a202573 0a003230 32332d30 mmit: %s..2023-0
+  0x0007af10 392d3137 2031323a 34313a33 34202b30 9-17 12:41:34 +0
+  0x0007af20 32303000 20202020 20676974 20646174 200.     git dat
   0x0007af30 653a2020 2025730a 0a000a44 65666175 e:   %s....Defau
   0x0007af40 6c742070 6172616d 65746572 73207661 lt parameters va
   0x0007af50 6c756573 3a0a000a 2a2a2047 656e6572 lues:...** Gener
   0x0007af60 6963206f 7074696f 6e73203a 0a000a2a ic options :...*
   0x0007af70 2a202050 6172616d 65746572 730a0020 *  Parameters.. 
   0x0007af80 666f7220 6d617465 7269616c 206f6620 for material of 
   0x0007af90 72656620 25640a00 20626173 65642072 ref %d.. based r
@@ -2057,17 +2057,17 @@
   0x0007b060 20202020 2020206e 6f726d61 6c207265        normal re
   0x0007b070 67756c2e 0a002d78 72656720 20202020 gul...-xreg     
   0x0007b080 20202076 65727465 78207265 67756c2e    vertex regul.
   0x0007b090 0a002020 20202044 656c6574 65642069 ..     Deleted i
   0x0007b0a0 736f2065 64676573 3a202564 0a000000 so edges: %d....
   0x0007b0b0 0a202025 730a2020 204d4f44 554c4520 .  %s.   MODULE 
   0x0007b0c0 4d4d4725 733a2025 73202825 73290a20 MMG%s: %s (%s). 
-  0x0007b0d0 2025730a 00000000 36386336 65306339  %s.....68c6e0c9
-  0x0007b0e0 38653735 35613563 66306139 63636239 8e755a5cf0a9ccb9
-  0x0007b0f0 61396265 36353235 64306162 30303930 a9be6525d0ab0090
+  0x0007b0d0 2025730a 00000000 34333335 31396632  %s.....433519f2
+  0x0007b0e0 65363238 61623465 63643233 34643636 e628ab4ecd234d66
+  0x0007b0f0 64386532 61316434 63633966 38313235 d8e2a1d4cc9f8125
   0x0007b100 00000000 00000000 76657262 6f736974 ........verbosit
   0x0007b110 79202020 20202020 20202020 20202020 y               
   0x0007b120 2020282d 76292020 20202020 3a202564   (-v)      : %d
   0x0007b130 0a000000 00000000 6d617869 6d616c20 ........maximal 
   0x0007b140 6d656d6f 72792073 697a6520 20202020 memory size     
   0x0007b150 2020282d 6d292020 20202020 3a20257a   (-m)      : %z
   0x0007b160 75204d42 0a000000 616e676c 65206465 u MB....angle de
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+  [     0]  GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.2) 9.4.0
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -59,16 +59,16 @@
   0x00000380 37353700 5f5f6675 6e635f5f 2e383736 757.__func__.876
   0x00000390 35005f5f 66756e63 5f5f2e38 37393100 5.__func__.8791.
   0x000003a0 5f5f6675 6e635f5f 2e383830 34005f5f __func__.8804.__
   0x000003b0 66756e63 5f5f2e38 38313600 5f5f6675 func__.8816.__fu
   0x000003c0 6e635f5f 2e383832 38005f5f 66756e63 nc__.8828.__func
   0x000003d0 5f5f2e38 38333300 5f5f6675 6e635f5f __.8833.__func__
   0x000003e0 2e383834 34005f5f 66756e63 5f5f2e38 .8844.__func__.8
-  0x000003f0 38383900 5f5f6675 6e635f5f 2e383930 889.__func__.890
-  0x00000400 34005f5f 66756e63 5f5f2e38 39313900 4.__func__.8919.
+  0x000003f0 38393000 5f5f6675 6e635f5f 2e383930 890.__func__.890
+  0x00000400 35005f5f 66756e63 5f5f2e38 39323000 5.__func__.8920.
   0x00000410 696e6f75 745f732e 63006d79 66726565 inout_s.c.myfree
   0x00000420 2e706172 742e3000 5f5f6675 6e635f5f .part.0.__func__
   0x00000430 2e383439 33005f5f 66756e63 5f5f2e38 .8493.__func__.8
   0x00000440 35393300 6d6d6757 61726e2e 38373236 593.mmgWarn.8726
   0x00000450 005f5f66 756e635f 5f2e3837 3237005f .__func__.8727._
   0x00000460 5f66756e 635f5f2e 38373536 005f5f66 _func__.8756.__f
   0x00000470 756e635f 5f2e3837 3830005f 5f66756e unc__.8780.__fun
```

### Comparing `pymmg-0.1.0/pymmg.egg-info/PKG-INFO` & `pymmg-1.0.0/pymmg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmg
-Version: 0.1.0
+Version: 1.0.0
 Summary: Surface and volume mesh and remesh generators based on MMG library
 Author: gnikit
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://www.mmgtools.org/
 Project-URL: Source Code, https://github.com/gnikit/pymmg
 Project-URL: Bugs, https://github.com/gnikit/pymmg/issues
 Project-URL: Dicsussions, https://forum.mmgtools.org/
@@ -20,15 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: meshio
 Provides-Extra: all
+Requires-Dist: meshio[all]; extra == "all"
 
 # pymmg - Surface and volume remeshers
 
 [![Build](https://github.com/gnikit/pymmg/actions/workflows/main.yml/badge.svg)](https://github.com/gnikit/pymmg/actions/workflows/main.yml)
 
 Bringing [MMG](https://www.mmgtools.org/) surface and volume remeshers to Python.
 This package is a wrapper around the MMG tools
@@ -72,15 +74,15 @@
 
 ## Installation
 
 ```bash
 pip install pymmg
 ```
 
-> NOTE: you can the full-blown `pymmg` converter with `netcdf4` and `h5py` by doing:
+> NOTE: you can use the full-blown `pymmg` converter with `netcdf4` and `h5py` by doing:
 > `pip install pymmg[all]`
 
 ## Usage
 
 ### Surface remeshing
 
 ```bash
```

### Comparing `pymmg-0.1.0/pymmg.egg-info/SOURCES.txt` & `pymmg-1.0.0/pymmg.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 CMakeLists.txt
 README.md
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/workflows/main.yml
 _skbuild/linux-x86_64-3.8/cmake-install/src/general/__init__.py
+_skbuild/linux-x86_64-3.8/cmake-install/src/general/_version.py
 _skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/__init__.py
 _skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/__main__.py
 _skbuild/linux-x86_64-3.8/cmake-install/src/mmg2d/mmg2d_O3
 _skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/__init__.py
 _skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/__main__.py
 _skbuild/linux-x86_64-3.8/cmake-install/src/mmg3d/mmg3d_O3
 _skbuild/linux-x86_64-3.8/cmake-install/src/mmgs/__init__.py
```

### Comparing `pymmg-0.1.0/pyproject.toml` & `pymmg-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 [build-system]
-requires = ["setuptools>=42", "scikit-build>=0.13", "cmake>=3.18", "ninja"]
+requires = [
+    "setuptools>=42",
+    "scikit-build>=0.13",
+    "cmake>=3.18",
+    "ninja",
+    "setuptools_scm>=8",
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymmg"
-version = "0.1.0"
 license = { text = "LGPL-3.0-or-later" }
 authors = [{ name = "gnikit" }]
 requires-python = ">=3.7"
 dependencies = ["meshio"]
 description = "Surface and volume mesh and remesh generators based on MMG library"
 readme = "README.md"
 keywords = ["mesh", "remesh", "mesh generation", "unstructured"]
@@ -23,25 +28,28 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities",
 ]
-dynamic = ["entry-points"]
+dynamic = ["version", "entry-points", "scripts"]
 
 [project.urls]
 Homepage = "https://www.mmgtools.org/"
 "Source Code" = "https://github.com/gnikit/pymmg"
 Bugs = "https://github.com/gnikit/pymmg/issues"
 Dicsussions = "https://forum.mmgtools.org/"
 
 [project.optional-dependencies]
 all = ["meshio[all]"]
 
+[tool.setuptools_scm]
+write_to = "src/general/_version.py"
+
 [tool.cibuildwheel]
 build = "cp311-*" # build wheels only for one Python version
 skip = "pp*"      # skip all pypy builds
 
 
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "arm64"]
```

### Comparing `pymmg-0.1.0/src/general/__init__.py` & `pymmg-1.0.0/src/general/__init__.py`

 * *Files identical despite different names*

