# Comparing `tmp/model-explorer-0.0.59.tar.gz` & `tmp/model-explorer-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-explorer-0.0.59.tar", last modified: Mon Apr  1 16:56:15 2024, max compression
+gzip compressed data, was "model-explorer-0.0.60.tar", last modified: Mon Apr  1 16:57:53 2024, max compression
```

## Comparing `model-explorer-0.0.59.tar` & `model-explorer-0.0.60.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:56:15.596869 model-explorer-0.0.59/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 16:56:15.596869 model-explorer-0.0.59/PKG-INFO
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      932 2024-04-01 16:50:48.000000 model-explorer-0.0.59/pyproject.toml
--rw-r-----   0 jingjin  (83079) primarygroup (89939)       38 2024-04-01 16:56:15.596869 model-explorer-0.0.59/setup.cfg
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:56:15.580869 model-explorer-0.0.59/src/
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:56:15.580869 model-explorer-0.0.59/src/model_explorer/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      465 2024-03-28 21:34:11.000000 model-explorer-0.0.59/src/model_explorer/__init__.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)       96 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/__main__.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1029 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      789 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/adapter_runner.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1121 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/builtin_graphdef_adapter.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      855 2024-03-28 22:07:59.000000 model-explorer-0.0.59/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1500 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/builtin_tf_direct_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1457 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/builtin_tf_mlir_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1190 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/builtin_tflite_flatbuffer_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1137 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/builtin_tflite_mlir_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1665 2024-04-01 16:56:02.000000 model-explorer-0.0.59/src/model_explorer/cmdline.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)       32 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/consts.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      338 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/extension_base.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1111 2024-03-28 23:18:49.000000 model-explorer-0.0.59/src/model_explorer/extension_class_processor.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     4294 2024-03-28 22:24:29.000000 model-explorer-0.0.59/src/model_explorer/extension_manager.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      198 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/extension_matadata.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     3732 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/graph.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      482 2024-03-28 22:07:45.000000 model-explorer-0.0.59/src/model_explorer/pytorch.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     6768 2024-03-28 22:05:55.000000 model-explorer-0.0.59/src/model_explorer/pytorch_exported_program_adater_impl.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      353 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/registered_extension.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    10365 2024-03-28 22:45:58.000000 model-explorer-0.0.59/src/model_explorer/server.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      349 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/singleton.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      603 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/types.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1021 2024-03-28 21:45:00.000000 model-explorer-0.0.59/src/model_explorer/utils.py
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:56:15.580869 model-explorer-0.0.59/src/model_explorer/web_app/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/web_app/index.html
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:56:15.596869 model-explorer-0.0.59/src/model_explorer/web_app/static_files/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9028 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4020 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15476 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5340 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8332 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8756 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3800 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15208 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5012 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7976 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8700 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3744 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4924 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7764 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8352 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15468 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5424 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9004 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4000 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8528 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15864 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5388 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9100 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4084 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7860 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8592 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3792 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4992 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32907 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextBold.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   144302 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextBold.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32921 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   138086 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32905 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   132192 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32616 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   118904 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png
--rwxr-x---   0 jingjin  (83079) primarygroup (89939)  1160586 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/app_bundle.js
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      979 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/favicon.svg
--rw-r-----   0 jingjin  (83079) primarygroup (89939)   169616 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/google_material_icon.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      828 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/icons_2024021202.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2092 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/icons_2024021202.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   615601 2024-03-27 17:14:33.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/main_deps.js
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   128352 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/material_icon.woff2
--r-xr-x---   0 jingjin  (83079) primarygroup (89939)   245487 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/styles.css
--rwxr-x---   0 jingjin  (83079) primarygroup (89939)  2615494 2024-04-01 06:39:02.000000 model-explorer-0.0.59/src/model_explorer/web_app/static_files/worker_bin.js
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:56:15.596869 model-explorer-0.0.59/src/model_explorer.egg-info/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 16:56:15.000000 model-explorer-0.0.59/src/model_explorer.egg-info/PKG-INFO
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4876 2024-04-01 16:56:15.000000 model-explorer-0.0.59/src/model_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)        1 2024-04-01 16:56:15.000000 model-explorer-0.0.59/src/model_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      108 2024-04-01 16:56:15.000000 model-explorer-0.0.59/src/model_explorer.egg-info/entry_points.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      114 2024-04-01 16:56:15.000000 model-explorer-0.0.59/src/model_explorer.egg-info/requires.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)       15 2024-04-01 16:56:15.000000 model-explorer-0.0.59/src/model_explorer.egg-info/top_level.txt
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:57:53.056018 model-explorer-0.0.60/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 16:57:53.056018 model-explorer-0.0.60/PKG-INFO
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      932 2024-04-01 16:57:49.000000 model-explorer-0.0.60/pyproject.toml
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)       38 2024-04-01 16:57:53.056018 model-explorer-0.0.60/setup.cfg
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:57:53.040018 model-explorer-0.0.60/src/
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:57:53.044019 model-explorer-0.0.60/src/model_explorer/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      465 2024-03-28 21:34:11.000000 model-explorer-0.0.60/src/model_explorer/__init__.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)       96 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/__main__.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1029 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      789 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/adapter_runner.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1121 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/builtin_graphdef_adapter.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      855 2024-03-28 22:07:59.000000 model-explorer-0.0.60/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1500 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/builtin_tf_direct_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1457 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/builtin_tf_mlir_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1190 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/builtin_tflite_flatbuffer_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1137 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/builtin_tflite_mlir_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1666 2024-04-01 16:57:40.000000 model-explorer-0.0.60/src/model_explorer/cmdline.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)       32 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/consts.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      338 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/extension_base.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1111 2024-03-28 23:18:49.000000 model-explorer-0.0.60/src/model_explorer/extension_class_processor.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     4294 2024-03-28 22:24:29.000000 model-explorer-0.0.60/src/model_explorer/extension_manager.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      198 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/extension_matadata.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     3732 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/graph.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      482 2024-03-28 22:07:45.000000 model-explorer-0.0.60/src/model_explorer/pytorch.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     6768 2024-03-28 22:05:55.000000 model-explorer-0.0.60/src/model_explorer/pytorch_exported_program_adater_impl.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      353 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/registered_extension.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    10365 2024-03-28 22:45:58.000000 model-explorer-0.0.60/src/model_explorer/server.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      349 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/singleton.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      603 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/types.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1021 2024-03-28 21:45:00.000000 model-explorer-0.0.60/src/model_explorer/utils.py
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:57:53.044019 model-explorer-0.0.60/src/model_explorer/web_app/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/web_app/index.html
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:57:53.052019 model-explorer-0.0.60/src/model_explorer/web_app/static_files/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9028 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4020 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15476 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5340 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8332 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8756 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3800 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15208 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5012 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7976 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8700 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3744 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4924 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7764 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8352 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15468 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5424 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9004 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4000 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8528 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15864 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5388 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9100 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4084 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7860 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8592 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3792 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4992 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32907 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextBold.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   144302 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextBold.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32921 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   138086 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32905 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   132192 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32616 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   118904 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png
+-rwxr-x---   0 jingjin  (83079) primarygroup (89939)  1160586 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/app_bundle.js
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      979 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/favicon.svg
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)   169616 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/google_material_icon.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      828 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/icons_2024021202.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2092 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/icons_2024021202.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   615601 2024-03-27 17:14:33.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/main_deps.js
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   128352 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/material_icon.woff2
+-r-xr-x---   0 jingjin  (83079) primarygroup (89939)   245487 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/styles.css
+-rwxr-x---   0 jingjin  (83079) primarygroup (89939)  2615494 2024-04-01 06:39:02.000000 model-explorer-0.0.60/src/model_explorer/web_app/static_files/worker_bin.js
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 16:57:53.056018 model-explorer-0.0.60/src/model_explorer.egg-info/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 16:57:53.000000 model-explorer-0.0.60/src/model_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4876 2024-04-01 16:57:53.000000 model-explorer-0.0.60/src/model_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)        1 2024-04-01 16:57:53.000000 model-explorer-0.0.60/src/model_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      108 2024-04-01 16:57:53.000000 model-explorer-0.0.60/src/model_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      114 2024-04-01 16:57:53.000000 model-explorer-0.0.60/src/model_explorer.egg-info/requires.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)       15 2024-04-01 16:57:53.000000 model-explorer-0.0.60/src/model_explorer.egg-info/top_level.txt
```

### Comparing `model-explorer-0.0.59/PKG-INFO` & `model-explorer-0.0.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer
-Version: 0.0.59
+Version: 0.0.60
 Summary: A modern model graph visualizer and debugger
 Author-email: Google LLC <opensource@google.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `model-explorer-0.0.59/pyproject.toml` & `model-explorer-0.0.60/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "model-explorer"
-version = "0.0.59"
+version = "0.0.60"
 authors = [
   { name="Google LLC", email="opensource@google.com" },
 ]
 description = "A modern model graph visualizer and debugger"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `model-explorer-0.0.59/src/model_explorer/adapter.py` & `model-explorer-0.0.60/src/model_explorer/adapter.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/adapter_runner.py` & `model-explorer-0.0.60/src/model_explorer/adapter_runner.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/builtin_graphdef_adapter.py` & `model-explorer-0.0.60/src/model_explorer/builtin_graphdef_adapter.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py` & `model-explorer-0.0.60/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/builtin_tf_direct_adapter.py` & `model-explorer-0.0.60/src/model_explorer/builtin_tf_direct_adapter.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/builtin_tf_mlir_adapter.py` & `model-explorer-0.0.60/src/model_explorer/builtin_tf_mlir_adapter.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/builtin_tflite_flatbuffer_adapter.py` & `model-explorer-0.0.60/src/model_explorer/builtin_tflite_flatbuffer_adapter.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/builtin_tflite_mlir_adapter.py` & `model-explorer-0.0.60/src/model_explorer/builtin_tflite_mlir_adapter.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/cmdline.py` & `model-explorer-0.0.60/src/model_explorer/cmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 
 from . import server
 
 parser = argparse.ArgumentParser(
-    prog='mode_explorer',
+    prog='model_explorer',
     description='A modern model graph visualizer and debugger',
     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument('model_paths',
                     nargs='?',
                     default='',
                     help='comma separated model file paths')
 parser.add_argument('--host',
```

### Comparing `model-explorer-0.0.59/src/model_explorer/extension_class_processor.py` & `model-explorer-0.0.60/src/model_explorer/extension_class_processor.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/extension_manager.py` & `model-explorer-0.0.60/src/model_explorer/extension_manager.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/graph.py` & `model-explorer-0.0.60/src/model_explorer/graph.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/pytorch_exported_program_adater_impl.py` & `model-explorer-0.0.60/src/model_explorer/pytorch_exported_program_adater_impl.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/server.py` & `model-explorer-0.0.60/src/model_explorer/server.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/types.py` & `model-explorer-0.0.60/src/model_explorer/types.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/utils.py` & `model-explorer-0.0.60/src/model_explorer/utils.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextBold.json` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextBold.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextBold.png` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextBold.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/app_bundle.js` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/app_bundle.js`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/favicon.svg` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/favicon.svg`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/google_material_icon.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/google_material_icon.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/icons_2024021202.json` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/icons_2024021202.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/icons_2024021202.png` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/icons_2024021202.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/main_deps.js` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/main_deps.js`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/material_icon.woff2` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/material_icon.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/styles.css` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/styles.css`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer/web_app/static_files/worker_bin.js` & `model-explorer-0.0.60/src/model_explorer/web_app/static_files/worker_bin.js`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.59/src/model_explorer.egg-info/PKG-INFO` & `model-explorer-0.0.60/src/model_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer
-Version: 0.0.59
+Version: 0.0.60
 Summary: A modern model graph visualizer and debugger
 Author-email: Google LLC <opensource@google.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `model-explorer-0.0.59/src/model_explorer.egg-info/SOURCES.txt` & `model-explorer-0.0.60/src/model_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

