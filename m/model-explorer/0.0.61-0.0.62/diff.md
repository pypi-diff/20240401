# Comparing `tmp/model-explorer-0.0.61.tar.gz` & `tmp/model-explorer-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-explorer-0.0.61.tar", last modified: Mon Apr  1 17:01:24 2024, max compression
+gzip compressed data, was "model-explorer-0.0.62.tar", last modified: Mon Apr  1 19:40:09 2024, max compression
```

## Comparing `model-explorer-0.0.61.tar` & `model-explorer-0.0.62.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 17:01:24.630173 model-explorer-0.0.61/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 17:01:24.630173 model-explorer-0.0.61/PKG-INFO
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      932 2024-04-01 17:01:16.000000 model-explorer-0.0.61/pyproject.toml
--rw-r-----   0 jingjin  (83079) primarygroup (89939)       38 2024-04-01 17:01:24.630173 model-explorer-0.0.61/setup.cfg
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 17:01:24.614173 model-explorer-0.0.61/src/
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 17:01:24.618173 model-explorer-0.0.61/src/model_explorer/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      465 2024-03-28 21:34:11.000000 model-explorer-0.0.61/src/model_explorer/__init__.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)       96 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/__main__.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1029 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      789 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/adapter_runner.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1121 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/builtin_graphdef_adapter.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      855 2024-03-28 22:07:59.000000 model-explorer-0.0.61/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1500 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/builtin_tf_direct_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1457 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/builtin_tf_mlir_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1190 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/builtin_tflite_flatbuffer_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1137 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/builtin_tflite_mlir_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1634 2024-04-01 17:00:23.000000 model-explorer-0.0.61/src/model_explorer/cmdline.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)       32 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/consts.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      338 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/extension_base.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1111 2024-03-28 23:18:49.000000 model-explorer-0.0.61/src/model_explorer/extension_class_processor.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     4294 2024-03-28 22:24:29.000000 model-explorer-0.0.61/src/model_explorer/extension_manager.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      198 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/extension_matadata.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     3732 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/graph.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      482 2024-03-28 22:07:45.000000 model-explorer-0.0.61/src/model_explorer/pytorch.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     6768 2024-03-28 22:05:55.000000 model-explorer-0.0.61/src/model_explorer/pytorch_exported_program_adater_impl.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      353 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/registered_extension.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    10365 2024-03-28 22:45:58.000000 model-explorer-0.0.61/src/model_explorer/server.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      349 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/singleton.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      603 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/types.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1021 2024-03-28 21:45:00.000000 model-explorer-0.0.61/src/model_explorer/utils.py
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 17:01:24.618173 model-explorer-0.0.61/src/model_explorer/web_app/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/web_app/index.html
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 17:01:24.626173 model-explorer-0.0.61/src/model_explorer/web_app/static_files/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9028 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4020 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15476 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5340 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8332 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8756 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3800 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15208 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5012 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7976 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8700 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3744 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4924 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7764 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8352 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15468 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5424 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9004 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4000 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8528 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15864 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5388 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9100 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4084 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7860 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8592 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3792 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4992 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32907 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextBold.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   144302 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextBold.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32921 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   138086 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32905 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   132192 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32616 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   118904 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png
--rwxr-x---   0 jingjin  (83079) primarygroup (89939)  1160586 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/app_bundle.js
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      979 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/favicon.svg
--rw-r-----   0 jingjin  (83079) primarygroup (89939)   169616 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/google_material_icon.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      828 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/icons_2024021202.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2092 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/icons_2024021202.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   615601 2024-03-27 17:14:33.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/main_deps.js
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   128352 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/material_icon.woff2
--r-xr-x---   0 jingjin  (83079) primarygroup (89939)   245487 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/styles.css
--rwxr-x---   0 jingjin  (83079) primarygroup (89939)  2615494 2024-04-01 06:39:02.000000 model-explorer-0.0.61/src/model_explorer/web_app/static_files/worker_bin.js
-drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 17:01:24.630173 model-explorer-0.0.61/src/model_explorer.egg-info/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 17:01:24.000000 model-explorer-0.0.61/src/model_explorer.egg-info/PKG-INFO
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4876 2024-04-01 17:01:24.000000 model-explorer-0.0.61/src/model_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)        1 2024-04-01 17:01:24.000000 model-explorer-0.0.61/src/model_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      108 2024-04-01 17:01:24.000000 model-explorer-0.0.61/src/model_explorer.egg-info/entry_points.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      114 2024-04-01 17:01:24.000000 model-explorer-0.0.61/src/model_explorer.egg-info/requires.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)       15 2024-04-01 17:01:24.000000 model-explorer-0.0.61/src/model_explorer.egg-info/top_level.txt
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 19:40:09.279164 model-explorer-0.0.62/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 19:40:09.279164 model-explorer-0.0.62/PKG-INFO
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      932 2024-04-01 19:39:35.000000 model-explorer-0.0.62/pyproject.toml
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)       38 2024-04-01 19:40:09.279164 model-explorer-0.0.62/setup.cfg
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 19:40:09.263164 model-explorer-0.0.62/src/
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 19:40:09.267164 model-explorer-0.0.62/src/model_explorer/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      553 2024-04-01 19:37:22.000000 model-explorer-0.0.62/src/model_explorer/__init__.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)       96 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/__main__.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1023 2024-04-01 19:24:19.000000 model-explorer-0.0.62/src/model_explorer/adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      783 2024-04-01 19:24:02.000000 model-explorer-0.0.62/src/model_explorer/adapter_runner.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1115 2024-04-01 19:24:30.000000 model-explorer-0.0.62/src/model_explorer/builtin_graphdef_adapter.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      849 2024-04-01 19:24:46.000000 model-explorer-0.0.62/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1523 2024-04-01 19:24:53.000000 model-explorer-0.0.62/src/model_explorer/builtin_tf_direct_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1480 2024-04-01 19:24:58.000000 model-explorer-0.0.62/src/model_explorer/builtin_tf_mlir_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1184 2024-04-01 19:25:03.000000 model-explorer-0.0.62/src/model_explorer/builtin_tflite_flatbuffer_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1131 2024-04-01 19:25:08.000000 model-explorer-0.0.62/src/model_explorer/builtin_tflite_mlir_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1634 2024-04-01 17:00:23.000000 model-explorer-0.0.62/src/model_explorer/cmdline.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)       32 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/consts.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      338 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/extension_base.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1111 2024-03-28 23:18:49.000000 model-explorer-0.0.62/src/model_explorer/extension_class_processor.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     4294 2024-03-28 22:24:29.000000 model-explorer-0.0.62/src/model_explorer/extension_manager.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      198 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/extension_matadata.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     3732 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/graph.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     1101 2024-04-01 19:33:09.000000 model-explorer-0.0.62/src/model_explorer/importers.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     6762 2024-04-01 19:25:15.000000 model-explorer-0.0.62/src/model_explorer/pytorch_exported_program_adater_impl.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      353 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/registered_extension.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    10359 2024-04-01 19:26:04.000000 model-explorer-0.0.62/src/model_explorer/server.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      349 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/singleton.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      597 2024-04-01 19:23:49.000000 model-explorer-0.0.62/src/model_explorer/types.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1015 2024-04-01 19:26:11.000000 model-explorer-0.0.62/src/model_explorer/utils.py
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 19:40:09.267164 model-explorer-0.0.62/src/model_explorer/web_app/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/web_app/index.html
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 19:40:09.275164 model-explorer-0.0.62/src/model_explorer/web_app/static_files/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9028 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4020 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15476 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5340 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8332 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8756 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3800 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15208 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5012 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7976 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8700 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3744 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4924 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7764 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8352 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15468 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5424 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9004 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4000 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8528 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15864 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5388 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9100 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4084 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7860 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8592 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3792 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4992 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32907 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextBold.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   144302 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextBold.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32921 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   138086 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32905 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   132192 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32616 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   118904 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png
+-rwxr-x---   0 jingjin  (83079) primarygroup (89939)  1160586 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/app_bundle.js
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      979 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/favicon.svg
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)   169616 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/google_material_icon.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      828 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/icons_2024021202.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2092 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/icons_2024021202.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   615601 2024-03-27 17:14:33.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/main_deps.js
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   128352 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/material_icon.woff2
+-r-xr-x---   0 jingjin  (83079) primarygroup (89939)   245487 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/styles.css
+-rwxr-x---   0 jingjin  (83079) primarygroup (89939)  2615494 2024-04-01 06:39:02.000000 model-explorer-0.0.62/src/model_explorer/web_app/static_files/worker_bin.js
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-01 19:40:09.279164 model-explorer-0.0.62/src/model_explorer.egg-info/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      704 2024-04-01 19:40:09.000000 model-explorer-0.0.62/src/model_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4878 2024-04-01 19:40:09.000000 model-explorer-0.0.62/src/model_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)        1 2024-04-01 19:40:09.000000 model-explorer-0.0.62/src/model_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      108 2024-04-01 19:40:09.000000 model-explorer-0.0.62/src/model_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      114 2024-04-01 19:40:09.000000 model-explorer-0.0.62/src/model_explorer.egg-info/requires.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)       15 2024-04-01 19:40:09.000000 model-explorer-0.0.62/src/model_explorer.egg-info/top_level.txt
```

### Comparing `model-explorer-0.0.61/PKG-INFO` & `model-explorer-0.0.62/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer
-Version: 0.0.61
+Version: 0.0.62
 Summary: A modern model graph visualizer and debugger
 Author-email: Google LLC <opensource@google.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `model-explorer-0.0.61/pyproject.toml` & `model-explorer-0.0.62/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "model-explorer"
-version = "0.0.61"
+version = "0.0.62"
 authors = [
   { name="Google LLC", email="opensource@google.com" },
 ]
 description = "A modern model graph visualizer and debugger"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `model-explorer-0.0.61/src/model_explorer/adapter_runner.py` & `model-explorer-0.0.62/src/model_explorer/adapter_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
-from .types import AdapterCommand, AdapterConvertResponse
+from .types import AdapterCommand, ModelExplorerGraphs
 
 from .registered_extension import RegisteredExtension
 from .utils import get_instance_method
 
 
 class AdapterRunner:
   """A runner to run adapter extension."""
 
-  def run_adapter(self, extension: RegisteredExtension, cmd: AdapterCommand) -> AdapterConvertResponse:
+  def run_adapter(self, extension: RegisteredExtension, cmd: AdapterCommand) -> ModelExplorerGraphs:
     # Get extension class and create an instance.
     extension_class = extension.ext_class
     instance = extension_class()
 
     # Get the method by the cmdId.
     fn = get_instance_method(instance, cmd['cmdId'])
     if fn is None:
```

### Comparing `model-explorer-0.0.61/src/model_explorer/builtin_graphdef_adapter.py` & `model-explorer-0.0.62/src/model_explorer/builtin_graphdef_adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Dict
 
 from model_explorer_adapter import \
     _pywrap_convert_wrapper as convert_wrapper  # type: ignore
 
 from .adapter import Adapter, AdapterMetadata
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 from .utils import convert_builtin_resp
 
 
 class BuiltinGraphdefAdapter(Adapter):
   """Built-in graphdef adapter."""
 
   metadata = AdapterMetadata(id='builtin_graphdef',
                              name='GraphDef adapter',
                              description='A built-in adapter that converts GraphDef file to Model Explorer format.',
                              fileExts=['pb', 'pbtxt', 'graphdef'])
 
   def __init__(self):
     super().__init__()
 
-  def convert(self, model_path: str, settings: Dict) -> AdapterConvertResponse:
+  def convert(self, model_path: str, settings: Dict) -> ModelExplorerGraphs:
     # Construct config.
     config = convert_wrapper.VisualizeConfig()
     if 'const_element_count_limit' in settings:
       config.const_element_count_limit = settings['const_element_count_limit']
 
     # Run
     resp_json_str = convert_wrapper.ConvertGraphDefDirectlyToJson(
```

### Comparing `model-explorer-0.0.61/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py` & `model-explorer-0.0.62/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 import torch
 import torch.fx
 
 from .adapter import Adapter, AdapterMetadata
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 from .pytorch_exported_program_adater_impl import PytorchExportedProgramAdapterImpl
 
 
 class BuiltinPytorchExportedProgramAdapter(Adapter):
   """Built-in pytorch adapter using ExportedProgram."""
 
   metadata = AdapterMetadata(
@@ -20,10 +20,10 @@
       ),
       fileExts=['pt2'],
   )
 
   def __init__(self):
     super().__init__()
 
-  def convert(self, model_path: str, settings: Dict) -> AdapterConvertResponse:
+  def convert(self, model_path: str, settings: Dict) -> ModelExplorerGraphs:
     ep = torch.export.load(model_path)
     return PytorchExportedProgramAdapterImpl(ep).convert()
```

### Comparing `model-explorer-0.0.61/src/model_explorer/builtin_tf_direct_adapter.py` & `model-explorer-0.0.62/src/model_explorer/builtin_tf_direct_adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import os
 from typing import Dict
 
 from model_explorer_adapter import \
     _pywrap_convert_wrapper as convert_wrapper  # type: ignore
 
 from .adapter import Adapter, AdapterMetadata
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 from .utils import convert_builtin_resp
 
 
 class BuiltinTfDirectAdapter(Adapter):
   """Built-in tf adapter by parsing .pb file."""
 
   metadata = AdapterMetadata(id='builtin_tf_direct',
                              name='TF adapter (direct)',
                              description='A built-in adapter that converts a TF saved model to Model Explorer format by directly parsing the .pb file.',
                              fileExts=['pb'])
 
   def __init__(self):
     super().__init__()
 
-  def convert(self, model_path: str, settings: Dict) -> AdapterConvertResponse:
+  def convert(self, model_path: str, settings: Dict) -> ModelExplorerGraphs:
     # Construct config.
     config = convert_wrapper.VisualizeConfig()
     if 'const_element_count_limit' in settings:
       config.const_element_count_limit = settings['const_element_count_limit']
 
     # Normalize model_path
     model_dir = model_path
     if model_path.endswith('.pb'):
       model_dir = os.path.dirname(model_path)
       file_name = os.path.basename(model_path)
 
-      # Rename file to saved_model.pb
+      # Check file name.
       if file_name != 'saved_model.pb':
-        os.rename(model_path, os.path.join(model_dir, 'saved_model.pb'))
+        raise Exception(
+            f'The model file has to be named "saved_model.pb" to work with this adapter')
 
     # Run
     resp_json_str = convert_wrapper.ConvertSavedModelDirectlyToJson(
         config, model_dir)
     return {'graphCollections': convert_builtin_resp(resp_json_str)}
```

### Comparing `model-explorer-0.0.61/src/model_explorer/builtin_tf_mlir_adapter.py` & `model-explorer-0.0.62/src/model_explorer/builtin_tf_mlir_adapter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import os
 from typing import Dict
 
 from model_explorer_adapter import \
     _pywrap_convert_wrapper as convert_wrapper  # type: ignore
 
 from .adapter import Adapter, AdapterMetadata
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 from .utils import convert_builtin_resp
 
 
 class BuiltinTfMlirAdapter(Adapter):
   """Built-in tf adapter using MLIR."""
 
   metadata = AdapterMetadata(id='builtin_tf_mlir',
                              name='TF adapter (MLIR)',
                              description='A built-in adapter that converts a TF saved model to Model Explorer format through MLIR.',
                              fileExts=['pb'])
 
   def __init__(self):
     super().__init__()
 
-  def convert(self, model_path: str, settings: Dict) -> AdapterConvertResponse:
+  def convert(self, model_path: str, settings: Dict) -> ModelExplorerGraphs:
     # Construct config.
     config = convert_wrapper.VisualizeConfig()
     if 'const_element_count_limit' in settings:
       config.const_element_count_limit = settings['const_element_count_limit']
 
     # Normalize model_path
     model_dir = model_path
     if model_path.endswith('.pb'):
       model_dir = os.path.dirname(model_path)
       file_name = os.path.basename(model_path)
 
-      # Rename file to saved_model.pb
+      # Check file name.
       if file_name != 'saved_model.pb':
-        os.rename(model_path, os.path.join(model_dir, 'saved_model.pb'))
+        raise Exception(
+            f'The model file has to be named "saved_model.pb" to work with this adapter')
 
     # Run
     resp_json_str = convert_wrapper.ConvertSavedModelToJson(
         config, model_dir)
     return {'graphCollections': convert_builtin_resp(resp_json_str)}
```

### Comparing `model-explorer-0.0.61/src/model_explorer/builtin_tflite_flatbuffer_adapter.py` & `model-explorer-0.0.62/src/model_explorer/builtin_tflite_flatbuffer_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Dict
 
 from model_explorer_adapter import \
     _pywrap_convert_wrapper as convert_wrapper  # type: ignore
 
 from .adapter import Adapter, AdapterMetadata
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 from .utils import convert_builtin_resp
 
 
 class BuiltinTfliteFlatbufferAdapter(Adapter):
   """Built-in tflite adapter by parsing flatbuffer."""
 
   metadata = AdapterMetadata(id='builtin_tflite_flatbuffer',
                              name='TFLite adapter (Flatbuffer)',
                              description='A built-in adapter that converts a TFLite model to Model Explorer format by directly parsing the flatbuffer.',
                              fileExts=['tflite'])
 
   def __init__(self):
     super().__init__()
 
-  def convert(self, model_path: str, settings: Dict) -> AdapterConvertResponse:
+  def convert(self, model_path: str, settings: Dict) -> ModelExplorerGraphs:
     # Construct config.
     config = convert_wrapper.VisualizeConfig()
     if 'const_element_count_limit' in settings:
       config.const_element_count_limit = settings['const_element_count_limit']
 
     # Run
     resp_json_str = convert_wrapper.ConvertFlatbufferDirectlyToJson(
```

### Comparing `model-explorer-0.0.61/src/model_explorer/builtin_tflite_mlir_adapter.py` & `model-explorer-0.0.62/src/model_explorer/builtin_tflite_mlir_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Dict
 
 from model_explorer_adapter import \
     _pywrap_convert_wrapper as convert_wrapper  # type: ignore
 
 from .adapter import Adapter, AdapterMetadata
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 from .utils import convert_builtin_resp
 
 
 class BuiltinTfliteMlirAdapter(Adapter):
   """Built-in tflite adapter using MLIR."""
 
   metadata = AdapterMetadata(id='builtin_tflite_mlir',
                              name='TFLite adapter (MLIR)',
                              description='A built-in adapter that converts a TFLite model to Model Explorer format through MLIR.',
                              fileExts=['tflite'])
 
   def __init__(self):
     super().__init__()
 
-  def convert(self, model_path: str, settings: Dict) -> AdapterConvertResponse:
+  def convert(self, model_path: str, settings: Dict) -> ModelExplorerGraphs:
     # Construct config.
     config = convert_wrapper.VisualizeConfig()
     if 'const_element_count_limit' in settings:
       config.const_element_count_limit = settings['const_element_count_limit']
 
     # Run
     resp_json_str = convert_wrapper.ConvertFlatbufferToJson(
```

### Comparing `model-explorer-0.0.61/src/model_explorer/cmdline.py` & `model-explorer-0.0.62/src/model_explorer/cmdline.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/extension_class_processor.py` & `model-explorer-0.0.62/src/model_explorer/extension_class_processor.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/extension_manager.py` & `model-explorer-0.0.62/src/model_explorer/extension_manager.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/graph.py` & `model-explorer-0.0.62/src/model_explorer/graph.py`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/pytorch_exported_program_adater_impl.py` & `model-explorer-0.0.62/src/model_explorer/pytorch_exported_program_adater_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 
 import torch
 import torch.fx
 from torch.fx import _pytree as fx_pytree
 
 from .graph import Graph, GraphNode, IncomingEdge, KeyValue, OutputMetadataItem
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 
 
 class PytorchExportedProgramAdapterImpl:
 
   def __init__(self, ep: torch.export.ExportedProgram):
     self.ep = ep
     self.gm = self.ep.graph_module
@@ -190,9 +190,9 @@
 
   def create_graph(self):
     graph = Graph(id='graph', nodes=[])
     for node in self.gm.graph.nodes:
       graph.nodes.append(self.create_node(node))
     return graph
 
-  def convert(self) -> AdapterConvertResponse:
+  def convert(self) -> ModelExplorerGraphs:
     return {'graphs': [self.create_graph()]}
```

### Comparing `model-explorer-0.0.61/src/model_explorer/server.py` & `model-explorer-0.0.62/src/model_explorer/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from flask import Flask, make_response, request, send_from_directory
 from IPython import display
 from packaging.version import parse
 from termcolor import colored, cprint
 
 from .consts import PACKAGE_NAME
 from .extension_manager import ExtensionManager
-from .types import AdapterConvertResponse
+from .types import ModelExplorerGraphs
 from .utils import convert_adapter_response
 
 
 def _make_json_response(obj):
   body = json.dumps(obj)
   resp = make_response(body)
   resp.headers['Content-Type'] = 'application/json'
@@ -87,15 +87,15 @@
 def _js(script):
   display.display(display.Javascript(script))
 
 
 def start(host='localhost',
           port=8080,
           model_paths: list[str] = [],
-          graphs: Union[AdapterConvertResponse, None] = None,
+          graphs: Union[ModelExplorerGraphs, None] = None,
           no_open_in_browser: bool = False,
           extensions: list[str] = [],
           colab: bool = False,
           colab_height: int = 850,
           cors_host: Union[str, None] = None):
   """Starts the local server that serves the web app.
```

### Comparing `model-explorer-0.0.61/src/model_explorer/types.py` & `model-explorer-0.0.62/src/model_explorer/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 AdapterCommand = TypedDict(
     'AdapterCommand',
     {'cmdId': str,
      'modelPath': str,
      'settings': Dict,
      'deleteAfterConversion': bool})
 
-AdapterConvertResponse = TypedDict(
-    'AdapterConvertResponse',
+ModelExplorerGraphs = TypedDict(
+    'ModelExplorerGraphs',
     {'graphs': NotRequired[list[Graph]],
      'graphCollections': NotRequired[list[GraphCollection]]})
```

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextBold.json` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextBold.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextBold.png` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextBold.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/MonoSpaceSemiBold.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/app_bundle.js` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/app_bundle.js`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/favicon.svg` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/favicon.svg`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/google_material_icon.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/google_material_icon.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/icons_2024021202.json` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/icons_2024021202.json`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/icons_2024021202.png` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/icons_2024021202.png`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/main_deps.js` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/main_deps.js`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/material_icon.woff2` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/material_icon.woff2`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/styles.css` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/styles.css`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer/web_app/static_files/worker_bin.js` & `model-explorer-0.0.62/src/model_explorer/web_app/static_files/worker_bin.js`

 * *Files identical despite different names*

### Comparing `model-explorer-0.0.61/src/model_explorer.egg-info/PKG-INFO` & `model-explorer-0.0.62/src/model_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer
-Version: 0.0.61
+Version: 0.0.62
 Summary: A modern model graph visualizer and debugger
 Author-email: Google LLC <opensource@google.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `model-explorer-0.0.61/src/model_explorer.egg-info/SOURCES.txt` & `model-explorer-0.0.62/src/model_explorer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 src/model_explorer/cmdline.py
 src/model_explorer/consts.py
 src/model_explorer/extension_base.py
 src/model_explorer/extension_class_processor.py
 src/model_explorer/extension_manager.py
 src/model_explorer/extension_matadata.py
 src/model_explorer/graph.py
-src/model_explorer/pytorch.py
+src/model_explorer/importers.py
 src/model_explorer/pytorch_exported_program_adater_impl.py
 src/model_explorer/registered_extension.py
 src/model_explorer/server.py
 src/model_explorer/singleton.py
 src/model_explorer/types.py
 src/model_explorer/utils.py
 src/model_explorer.egg-info/PKG-INFO
```

