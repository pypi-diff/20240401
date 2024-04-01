# Comparing `tmp/gronckle-0.0.1.tar.gz` & `tmp/gronckle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gronckle-0.0.1.tar", last modified: Mon Feb 12 18:49:10 2024, max compression
+gzip compressed data, was "gronckle-0.0.2.tar", last modified: Mon Apr  1 19:23:24 2024, max compression
```

## Comparing `gronckle-0.0.1.tar` & `gronckle-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 gclark     (501) staff       (20)        0 2024-02-12 18:49:10.709649 gronckle-0.0.1/
--rw-r--r--   0 gclark     (501) staff       (20)    35149 2024-02-09 23:00:20.000000 gronckle-0.0.1/LICENSE
--rw-r--r--   0 gclark     (501) staff       (20)      563 2024-02-12 18:49:10.709502 gronckle-0.0.1/PKG-INFO
--rw-r--r--   0 gclark     (501) staff       (20)       40 2024-02-12 18:48:53.000000 gronckle-0.0.1/README.md
--rw-r--r--   0 gclark     (501) staff       (20)      504 2024-02-12 18:47:54.000000 gronckle-0.0.1/pyproject.toml
--rw-r--r--   0 gclark     (501) staff       (20)       38 2024-02-12 18:49:10.709689 gronckle-0.0.1/setup.cfg
-drwxr-xr-x   0 gclark     (501) staff       (20)        0 2024-02-12 18:49:10.708219 gronckle-0.0.1/src/
-drwxr-xr-x   0 gclark     (501) staff       (20)        0 2024-02-12 18:49:10.708774 gronckle-0.0.1/src/gronckle/
--rw-r--r--   0 gclark     (501) staff       (20)        0 2024-02-12 18:10:55.000000 gronckle-0.0.1/src/gronckle/__init__.py
--rw-r--r--   0 gclark     (501) staff       (20)       42 2024-02-12 18:11:20.000000 gronckle-0.0.1/src/gronckle/main.py
-drwxr-xr-x   0 gclark     (501) staff       (20)        0 2024-02-12 18:49:10.709346 gronckle-0.0.1/src/gronckle.egg-info/
--rw-r--r--   0 gclark     (501) staff       (20)      563 2024-02-12 18:49:10.000000 gronckle-0.0.1/src/gronckle.egg-info/PKG-INFO
--rw-r--r--   0 gclark     (501) staff       (20)      222 2024-02-12 18:49:10.000000 gronckle-0.0.1/src/gronckle.egg-info/SOURCES.txt
--rw-r--r--   0 gclark     (501) staff       (20)        1 2024-02-12 18:49:10.000000 gronckle-0.0.1/src/gronckle.egg-info/dependency_links.txt
--rw-r--r--   0 gclark     (501) staff       (20)        9 2024-02-12 18:49:10.000000 gronckle-0.0.1/src/gronckle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.320340 gronckle-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 19:23:19.000000 gronckle-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 19:23:24.316340 gronckle-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 19:23:19.000000 gronckle-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle/rag/smart_chunking/
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/demo_streamlit_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/split_text_responsibly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/text_splitter_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-01 19:23:19.000000 gronckle-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:23:24.320340 gronckle-0.0.2/setup.cfg
```

### Comparing `gronckle-0.0.1/LICENSE` & `gronckle-0.0.2/LICENSE`

 * *Files identical despite different names*

