# Comparing `tmp/nnsight-0.2.8.tar.gz` & `tmp/nnsight-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnsight-0.2.8.tar", last modified: Thu Mar 14 21:51:11 2024, max compression
+gzip compressed data, was "nnsight-0.2.9.tar", last modified: Sat Mar 23 16:32:10 2024, max compression
```

## Comparing `nnsight-0.2.8.tar` & `nnsight-0.2.9.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.987650 nnsight-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.935650 nnsight-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.939650 nnsight-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-14 21:51:05.000000 nnsight-0.2.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-14 21:51:05.000000 nnsight-0.2.8/.github/workflows/python-app.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-03-14 21:51:05.000000 nnsight-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-14 21:51:05.000000 nnsight-0.2.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)   131505 2024-03-14 21:51:05.000000 nnsight-0.2.8/NNsight_v0_2.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-03-14 21:51:11.987650 nnsight-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-03-14 21:51:05.000000 nnsight-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.939650 nnsight-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.943650 nnsight-0.2.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.943650 nnsight-0.2.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.943650 nnsight-0.2.8/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/css/front.css
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/css/hljs-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/css/hljs-light.css
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/css/status.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.947650 nnsight-0.2.8/docs/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)   143284 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/attribute_lens.png
--rw-r--r--   0 runner    (1001) docker     (127)   408507 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/execution.png
--rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   210842 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/interleaved.png
--rw-r--r--   0 runner    (1001) docker     (127)   131386 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/ioi.png
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/nnsight_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    79411 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/one.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.947650 nnsight-0.2.8/docs/source/_static/images/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/activation_patching.webp
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/attribution_patching.webp
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/dictionary_learning.webp
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/function_vectors.webp
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/future_lens.webp
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/logit_lens.webp
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/tutorials/walkthrough.webp
--rw-r--r--   0 runner    (1001) docker     (127)    89796 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/images/two.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.947650 nnsight-0.2.8/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/js/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/js/code.js
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.947650 nnsight-0.2.8/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/_templates/ndif_status.html
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.951650 nnsight-0.2.8/docs/source/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation/envoy.rst
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation/intervention.rst
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation/patching.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation/tracing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.935650 nnsight-0.2.8/docs/source/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.951650 nnsight-0.2.8/docs/source/notebooks/features/
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/cross_prompt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/getting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/gradients.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/modules.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/multiple_token.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/operations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/remote_execution.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/setting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   120097 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/features/token_indexing.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.955650 nnsight-0.2.8/docs/source/notebooks/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    66262 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/tutorials/attribution_patching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/tutorials/function_vectors.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/tutorials/future_lens.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  3725756 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/tutorials/ioi_patching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   137015 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/tutorials/logit_lens.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26232 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/tutorials/sae.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   115628 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/notebooks/tutorials/walkthrough.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/start.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/status.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/source/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.955650 nnsight-0.2.8/docs/sourcelatex/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.959650 nnsight-0.2.8/docs/sourcelatex/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/documentation/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/documentation/intervention.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/documentation/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/documentation/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/documentation/patching.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/documentation/tracing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/documentation/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-14 21:51:05.000000 nnsight-0.2.8/docs/sourcelatex/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.963650 nnsight-0.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/adhoc_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/custommodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/diffuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/directinvoker.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)   501485 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/main_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/modulize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/multitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/optim2.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/retain_grad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/test_server_llama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.963650 nnsight-0.2.8/examples/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.963650 nnsight-0.2.8/examples/tl/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (127)  1055349 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/tl/.ipynb_checkpoints/attention-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   481745 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/tl/Main_Demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   171207 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/tl/attention.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/tl/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)   120353 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/tl/attribution_patching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/tl/induction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-14 21:51:05.000000 nnsight-0.2.8/examples/tl/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-14 21:51:05.000000 nnsight-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 21:51:11.987650 nnsight-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.939650 nnsight-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.967650 nnsight-0.2.8/src/nnsight/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.967650 nnsight-0.2.8/src/nnsight/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/contexts/Invoker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/contexts/Runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/contexts/Tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/envoy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/intervention.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.967650 nnsight-0.2.8/src/nnsight/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/models/LanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/models/Mamba.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/models/NNsightModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/models/UnifiedTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.971650 nnsight-0.2.8/src/nnsight/models/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/models/mixins/Generation.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/models/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/nnsight.log
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.971650 nnsight-0.2.8/src/nnsight/pydantics/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/pydantics/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/pydantics/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/pydantics/Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/pydantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.971650 nnsight-0.2.8/src/nnsight/pydantics/format/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/pydantics/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/pydantics/format/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/pydantics/format/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.975650 nnsight-0.2.8/src/nnsight/toolbox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.979650 nnsight-0.2.8/src/nnsight/toolbox/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)  3767008 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/.ipynb_checkpoints/logit_lens-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3829447 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/das.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.983650 nnsight-0.2.8/src/nnsight/toolbox/interventions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.987650 nnsight-0.2.8/src/nnsight/toolbox/interventions/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/interventions/.ipynb_checkpoints/transformations-checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/interventions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/interventions/interventions.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/interventions/interventions_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/interventions/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.987650 nnsight-0.2.8/src/nnsight/toolbox/lens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/lens/__init__.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/lens/lens.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/lens/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)  3767008 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/logit_lens.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.987650 nnsight-0.2.8/src/nnsight/toolbox/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/optim/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/toolbox/optim/softprompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.987650 nnsight-0.2.8/src/nnsight/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/tracing/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/tracing/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/tracing/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-14 21:51:05.000000 nnsight-0.2.8/src/nnsight/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.987650 nnsight-0.2.8/src/nnsight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-03-14 21:51:11.000000 nnsight-0.2.8/src/nnsight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-14 21:51:11.000000 nnsight-0.2.8/src/nnsight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 21:51:11.000000 nnsight-0.2.8/src/nnsight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-14 21:51:11.000000 nnsight-0.2.8/src/nnsight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-14 21:51:11.000000 nnsight-0.2.8/src/nnsight.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:11.987650 nnsight-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 21:51:05.000000 nnsight-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-14 21:51:05.000000 nnsight-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-03-14 21:51:05.000000 nnsight-0.2.8/tests/test_lm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.518334 nnsight-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.466334 nnsight-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.470334 nnsight-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-23 16:32:04.000000 nnsight-0.2.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-23 16:32:04.000000 nnsight-0.2.9/.github/workflows/python-app.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-03-23 16:32:04.000000 nnsight-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-23 16:32:04.000000 nnsight-0.2.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)   133956 2024-03-23 16:32:04.000000 nnsight-0.2.9/NNsight_v0_2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-03-23 16:32:10.518334 nnsight-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-03-23 16:32:04.000000 nnsight-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-23 16:32:04.000000 nnsight-0.2.9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.470334 nnsight-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.474334 nnsight-0.2.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.474334 nnsight-0.2.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.474334 nnsight-0.2.9/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/css/front.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/css/hljs-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/css/hljs-light.css
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/css/status.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.478334 nnsight-0.2.9/docs/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)   143284 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/attribute_lens.png
+-rw-r--r--   0 runner    (1001) docker     (127)   408507 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/execution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   210842 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/interleaved.png
+-rw-r--r--   0 runner    (1001) docker     (127)   131386 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/ioi.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/nnsight_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    79411 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/one.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.478334 nnsight-0.2.9/docs/source/_static/images/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/activation_patching.webp
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/attribution_patching.webp
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/dictionary_learning.webp
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/function_vectors.webp
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/future_lens.webp
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/logit_lens.webp
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/tutorials/walkthrough.webp
+-rw-r--r--   0 runner    (1001) docker     (127)    89796 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/images/two.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.478334 nnsight-0.2.9/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/js/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/js/code.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.478334 nnsight-0.2.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/_templates/ndif_status.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.482334 nnsight-0.2.9/docs/source/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation/envoy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation/intervention.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation/patching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation/tracing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.466334 nnsight-0.2.9/docs/source/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.482334 nnsight-0.2.9/docs/source/notebooks/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/cross_prompt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/getting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/gradients.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/modules.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/multiple_token.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/operations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/remote_execution.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/setting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   120097 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/features/token_indexing.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.486334 nnsight-0.2.9/docs/source/notebooks/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    66262 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/tutorials/attribution_patching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/tutorials/function_vectors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/tutorials/future_lens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  3725756 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/tutorials/ioi_patching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   137015 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/tutorials/logit_lens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26232 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/tutorials/sae.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   118078 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/notebooks/tutorials/walkthrough.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/start.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/status.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/source/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.486334 nnsight-0.2.9/docs/sourcelatex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.490334 nnsight-0.2.9/docs/sourcelatex/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/documentation/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/documentation/intervention.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/documentation/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/documentation/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/documentation/patching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/documentation/tracing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/documentation/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-23 16:32:04.000000 nnsight-0.2.9/docs/sourcelatex/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.490334 nnsight-0.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/adhoc_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/custommodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/diffuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/directinvoker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)   501485 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/main_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/modulize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/multitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/optim2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/retain_grad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/test_server_llama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.494334 nnsight-0.2.9/examples/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.494334 nnsight-0.2.9/examples/tl/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)  1055349 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/tl/.ipynb_checkpoints/attention-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   481745 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/tl/Main_Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   171207 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/tl/attention.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/tl/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120353 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/tl/attribution_patching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/tl/induction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-23 16:32:04.000000 nnsight-0.2.9/examples/tl/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-23 16:32:04.000000 nnsight-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 16:32:10.518334 nnsight-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.470334 nnsight-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.498334 nnsight-0.2.9/src/nnsight/
+-rw-r--r--   0 runner    (1001) docker     (127)    18877 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.498334 nnsight-0.2.9/src/nnsight/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/contexts/Invoker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/contexts/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/contexts/Tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13857 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/envoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.498334 nnsight-0.2.9/src/nnsight/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/models/LanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/models/Mamba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/models/NNsightModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/models/UnifiedTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.498334 nnsight-0.2.9/src/nnsight/models/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/models/mixins/Generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/models/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/nnsight.log
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.498334 nnsight-0.2.9/src/nnsight/pydantics/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/pydantics/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/pydantics/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/pydantics/Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/pydantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.498334 nnsight-0.2.9/src/nnsight/pydantics/format/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/pydantics/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/pydantics/format/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/pydantics/format/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.506334 nnsight-0.2.9/src/nnsight/toolbox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.510334 nnsight-0.2.9/src/nnsight/toolbox/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3767008 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/.ipynb_checkpoints/logit_lens-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3829447 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/das.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.514334 nnsight-0.2.9/src/nnsight/toolbox/interventions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.514334 nnsight-0.2.9/src/nnsight/toolbox/interventions/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/interventions/.ipynb_checkpoints/transformations-checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/interventions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/interventions/interventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/interventions/interventions_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/interventions/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.514334 nnsight-0.2.9/src/nnsight/toolbox/lens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/lens/__init__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/lens/lens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/lens/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3767008 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/logit_lens.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.514334 nnsight-0.2.9/src/nnsight/toolbox/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/optim/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/toolbox/optim/softprompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.514334 nnsight-0.2.9/src/nnsight/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/tracing/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/tracing/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/tracing/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-23 16:32:04.000000 nnsight-0.2.9/src/nnsight/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.518334 nnsight-0.2.9/src/nnsight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-03-23 16:32:10.000000 nnsight-0.2.9/src/nnsight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-03-23 16:32:10.000000 nnsight-0.2.9/src/nnsight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 16:32:10.000000 nnsight-0.2.9/src/nnsight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-23 16:32:10.000000 nnsight-0.2.9/src/nnsight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-23 16:32:10.000000 nnsight-0.2.9/src/nnsight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:10.518334 nnsight-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 16:32:04.000000 nnsight-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-03-23 16:32:04.000000 nnsight-0.2.9/tests/test_lm.py
```

### Comparing `nnsight-0.2.8/.github/workflows/python-app.yml` & `nnsight-0.2.9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/LICENCE` & `nnsight-0.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/NNsight_v0_2.ipynb` & `nnsight-0.2.9/NNsight_v0_2.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.986899582651245%*

 * *Differences: {"'cells'": "{0: {'source': ['<a "*

 * *            'href="https://colab.research.google.com/github/JadenFiotto-Kaufman/nnsight/blob/dev/NNsight_v0_2.ipynb" '*

 * *            'target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" '*

 * *            'alt="Open In Colab"/></a>\\n\']}, 1: {\'source\': {insert: [(4, \'## The API for a '*

 * *            "transparent science on black-box AI\\n'), (6, 'In this era of large-scale deep "*

 * *            "learning, the most interesting AI models are\\n'), (7 […]*

```diff
@@ -3,58 +3,64 @@
         {
             "cell_type": "markdown",
             "metadata": {
                 "colab_type": "text",
                 "id": "view-in-github"
             },
             "source": [
-                "<a href=\"https://colab.research.google.com/github/JadenFiotto-Kaufman/nnsight/blob/dev/NNsight_v0_2.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
+                "<a href=\"https://colab.research.google.com/github/JadenFiotto-Kaufman/nnsight/blob/dev/NNsight_v0_2.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "-Scfr942GwO4"
             },
             "source": [
                 "<img src=\"https://nnsight.net/_static/images/nnsight_logo.svg\" alt=\"drawing\" width=\"200\"/>\n",
                 "\n",
                 "# **NNsight**\n",
-                "## The API for a transparent science on black-box AI\n",
-                "\n",
-                "In this era of large-scale deep learning, the most interesting AI models are massive black boxes that are hard to run. Ordinary commercial inference service APIs let you interact with huge models, but they do not let you access model internals.\n",
                 "\n",
-                "The nnsight library is different: it gives you full access to all the neural network internals. When used together with a remote service like the [National Deep Inference Facility](https://thevisible.net/docs/NDIF-proposal.pdf) (NDIF), it lets you run complex experiments on huge open source models easily, with fully transparent access.\n",
-                "\n",
-                "Our team wants to enable entire labs and independent researchers alike, as we believe a large, passionate, and collaborative community will produce the next big insights on a profoundly important field.\n",
+                "## The API for a transparent science on black-box AI\n",
                 "\n",
-                "\n"
+                "In this era of large-scale deep learning, the most interesting AI models are\n",
+                "massive black boxes that are hard to run. Ordinary commercial inference service\n",
+                "APIs let you interact with huge models, but they do not let you access model\n",
+                "internals.\n",
+                "\n",
+                "The nnsight library is different: it gives you full access to all the neural\n",
+                "network internals. When used together with a remote service like the\n",
+                "[National Deep Inference Facility](https://thevisible.net/docs/NDIF-proposal.pdf)\n",
+                "(NDIF), it lets you run complex experiments on huge open source models easily,\n",
+                "with fully transparent access.\n",
+                "\n",
+                "Our team wants to enable entire labs and independent researchers alike, as we\n",
+                "believe a large, passionate, and collaborative community will produce the next\n",
+                "big insights on a profoundly important field.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "N1OemD2VGyZx"
             },
             "source": [
-                "# 1 First, let's start small\n",
-                "\n",
-                "\n",
-                "\n"
+                "# 1 First, let's start small\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "WyLMmhrAKTNM"
             },
             "source": [
                 "## The Tracing Context\n",
                 "\n",
-                "To demonstrate the core functionality and syntax of nnsight, we'll define and use a tiny two layer neural network."
+                "To demonstrate the core functionality and syntax of nnsight, we'll define and\n",
+                "use a tiny two layer neural network.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "id": "R0RJijD0eXwf"
@@ -71,15 +77,17 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "bgydw7i3HmIH"
             },
             "source": [
-                "Our little model here is composed of four sub-modules, two linear layers ('layer1', 'layer2'). We specify the sizes of each of these modules, and create some complementary example input."
+                "Our little model here is composed of four sub-modules, two linear layers\n",
+                "('layer1', 'layer2'). We specify the sizes of each of these modules, and create\n",
+                "some complementary example input.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "2pX2Wg8Ceo6N"
@@ -89,29 +97,34 @@
                 "from collections import OrderedDict\n",
                 "import torch\n",
                 "\n",
                 "input_size = 5\n",
                 "hidden_dims = 10\n",
                 "output_size = 2\n",
                 "\n",
-                "net = torch.nn.Sequential(OrderedDict([\n",
-                "    ('layer1', torch.nn.Linear(input_size, hidden_dims)),\n",
-                "    ('layer2', torch.nn.Linear(hidden_dims, output_size)),\n",
-                "])).requires_grad_(False)\n",
+                "net = torch.nn.Sequential(\n",
+                "    OrderedDict(\n",
+                "        [\n",
+                "            (\"layer1\", torch.nn.Linear(input_size, hidden_dims)),\n",
+                "            (\"layer2\", torch.nn.Linear(hidden_dims, output_size)),\n",
+                "        ]\n",
+                "    )\n",
+                ").requires_grad_(False)\n",
                 "\n",
                 "input = torch.rand((1, input_size))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "tIPa2h2pJIwl"
             },
             "source": [
-                "The core object of the nnsight package is `NNsight`. This wraps around a given pytorch model to enable the capabilites nnsight provides."
+                "The core object of the nnsight package is `NNsight`. This wraps around a given\n",
+                "pytorch model to enable the capabilities nnsight provides.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "colab": {
@@ -178,15 +191,16 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "2NfISlQ_Ilvp"
             },
             "source": [
-                "Printing a Pytorch model shows a named hierarchy of modules which is very useful when accessing sub-components directly. NNsight models work the same."
+                "Printing a Pytorch model shows a named hierarchy of modules which is very useful\n",
+                "when accessing sub-components directly. NNsight models work the same.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -213,87 +227,109 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "djC5kyJWLuUH"
             },
             "source": [
-                "Before we actually get to using the model we just created, let's talk about Python contexts.\n",
+                "Before we actually get to using the model we just created, let's talk about\n",
+                "Python contexts.\n",
                 "\n",
-                "Python contexts define a scope using the `with` statement and are often used to create some object, or initiate some logic, that you later want to destroy or conclude.\n",
+                "Python contexts define a scope using the `with` statement and are often used to\n",
+                "create some object, or initiate some logic, that you later want to destroy or\n",
+                "conclude.\n",
                 "\n",
                 "The most common application is opening files like the following example:\n",
                 "\n",
                 "```python\n",
                 "with open('myfile.txt', 'r') as file:\n",
                 "  text = file.read()\n",
                 "```\n",
                 "\n",
-                "Python uses the `with` keyword to enter a context-like object. This object defines logic to be run at the start of the `with` block, as well as logic to be run when exiting. When using `with` for a file, entering the context opens the file and exiting the context closes it. Being within the context means we can read from the file. Simple enough! Now we can discuss how `nnsight` uses contexts to enable intuitive access into the internals of a neural network.\n"
+                "Python uses the `with` keyword to enter a context-like object. This object\n",
+                "defines logic to be run at the start of the `with` block, as well as logic to be\n",
+                "run when exiting. When using `with` for a file, entering the context opens the\n",
+                "file and exiting the context closes it. Being within the context means we can\n",
+                "read from the file. Simple enough! Now we can discuss how `nnsight` uses\n",
+                "contexts to enable intuitive access into the internals of a neural network.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "iNvuCOeyojcA"
             },
             "source": [
                 "The main tool with `nnsight` is a context for tracing.\n",
                 "\n",
-                "We enter the tracing context by calling `model.trace(<input>)` on an `NNsight` model, which defines how we want to run the model. Inside the context, we will be able to customize how the neural network runs. The model is actually run upon exiting the tracing context."
+                "We enter the tracing context by calling `model.trace(<input>)` on an `NNsight`\n",
+                "model, which defines how we want to run the model. Inside the context, we will\n",
+                "be able to customize how the neural network runs. The model is actually run upon\n",
+                "exiting the tracing context.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "qEXQ4auPSL-m"
             },
             "outputs": [],
             "source": [
                 "with model.trace(input) as tracer:\n",
-                "  pass"
+                "    pass"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "UZQsHinjqicJ"
             },
             "source": [
-                "But where's the output? To get that, we'll have to learn how to request it from within the tracing conext."
+                "But where's the output? To get that, we'll have to learn how to request it from\n",
+                "within the tracing context.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "xMfBpYzDPMoB"
             },
             "source": [
-                "## Getting"
+                "## Getting\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "B5_aFwFRv0ax"
             },
             "source": [
-                "Earlier, when we wrapped our little neural net with the `NNsight` class. This added a couple properties to each module in the model (including the root model itself). The two most important ones are `.input` and `.output`.\n",
+                "Earlier, when we wrapped our little neural net with the `NNsight` class. This\n",
+                "added a couple properties to each module in the model (including the root model\n",
+                "itself). The two most important ones are `.input` and `.output`.\n",
                 "\n",
                 "```python\n",
                 "model.input\n",
                 "model.output\n",
                 "```\n",
                 "\n",
-                "The names are self explainatory. They correspond to the inputs and outputs of their respective modules during a forward pass of the model. We can use these attributes inside the `with` block.\n",
-                "\n",
-                "However, it is important to understand that the model is not executed until the end of the tracing context. How can we access inputs and outputs before the model is run? The trick is deferred execution.\n",
-                "\n",
-                "`.input` and `.output` are Proxies for the eventual inputs and outputs of a module. In other words, when you access `model.output` what you are communicating to `nnsight` is, \"When you compute the output of `model`, please grab it for me and put the value into its corresponding Proxy object's `.value` attribute.\" Let's try it:"
+                "The names are self explainatory. They correspond to the inputs and outputs of\n",
+                "their respective modules during a forward pass of the model. We can use these\n",
+                "attributes inside the `with` block.\n",
+                "\n",
+                "However, it is important to understand that the model is not executed until the\n",
+                "end of the tracing context. How can we access inputs and outputs before the\n",
+                "model is run? The trick is deferred execution.\n",
+                "\n",
+                "`.input` and `.output` are Proxies for the eventual inputs and outputs of a\n",
+                "module. In other words, when you access `model.output` what you are\n",
+                "communicating to `nnsight` is, \"When you compute the output of `model`, please\n",
+                "grab it for me and put the value into its corresponding Proxy object's `.value`\n",
+                "attribute.\" Let's try it:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -316,30 +352,32 @@
                         "\u001b[0;31mValueError\u001b[0m: Accessing Proxy value before it's been set."
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input) as tracer:\n",
                 "\n",
-                "  output = model.output\n",
+                "    output = model.output\n",
                 "\n",
                 "print(output.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "sBz5qfwuR-6F"
             },
             "source": [
                 "Oh no an error! \"Accessing Proxy value before it's been set.\"\n",
                 "\n",
                 "Why doesn't our `output` have a `value`?\n",
                 "\n",
-                "Proxy objects will only have their value at the end of a context if we call `.save()` on them. This helps to reduce memory costs. Adding `.save()` fixes the error:"
+                "Proxy objects will only have their value at the end of a context if we call\n",
+                "`.save()` on them. This helps to reduce memory costs. Adding `.save()` fixes the\n",
+                "error:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -356,46 +394,52 @@
                         "tensor([[ 0.1473, -0.1518]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input) as tracer:\n",
                 "\n",
-                "  output = model.output.save()\n",
+                "    output = model.output.save()\n",
                 "\n",
                 "print(output.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "t5C0UZCwvrYn"
             },
             "source": [
-                "Success! We now have the model output. You just completed your first intervention using `nnsight`.\n",
-                "\n",
+                "Success! We now have the model output. You just completed your first\n",
+                "intervention using `nnsight`.\n",
                 "\n",
-                "Each time you access a module's input or output, you create an *intervention* in the neural network's forward pass. Collectively these requests form the *intervention graph*. We call the process of executing it alongside the model's normal computation graph, *interleaving*.\n",
+                "Each time you access a module's input or output, you create an _intervention_ in\n",
+                "the neural network's forward pass. Collectively these requests form the\n",
+                "_intervention graph_. We call the process of executing it alongside the model's\n",
+                "normal computation graph, _interleaving_.\n",
                 "\n",
                 "<details>\n",
                 "<summary>On Model output</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
-                "If you don't need to access anything other than the final model output, you can call the tracing context with `trace=False` and not use it as a context:\n",
+                "If you don't need to access anything other than the final model output, you can\n",
+                "call the tracing context with `trace=False` and not use it as a context:\n",
                 "\n",
                 "```python\n",
                 "output = model.trace(<inputs>, trace=False)\n",
                 "```\n",
                 "\n",
                 "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "Just like we saved the output of the model as a whole, we can save the output of any of its submodules. We use normal Python attribute syntax. We can discover how to access them by name by printing out the model:"
+                "Just like we saved the output of the model as a whole, we can save the output of\n",
+                "any of its submodules. We use normal Python attribute syntax. We can discover\n",
+                "how to access them by name by printing out the model:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -439,26 +483,28 @@
                         "          0.2968, -0.8834]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input) as tracer:\n",
                 "\n",
-                "  l1_output = model.layer1.output.save()\n",
+                "    l1_output = model.layer1.output.save()\n",
                 "\n",
                 "print(l1_output.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "85A-aP_03ht6"
             },
             "source": [
-                "Let's do the same for the input of layer2. While we're at it, let's also drop the `as tracer`, as we won't be needing the tracer object itself for a few sections:"
+                "Let's do the same for the input of layer2. While we're at it, let's also drop\n",
+                "the `as tracer`, as we won't be needing the tracer object itself for a few\n",
+                "sections:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -476,61 +522,64 @@
                         "          0.2968, -0.8834]]),), {})\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  l2_input = model.layer2.input.save()\n",
+                "    l2_input = model.layer2.input.save()\n",
                 "\n",
                 "print(l2_input.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "jk-U8zi33Gi-"
             },
             "source": [
                 "<details>\n",
                 "  <summary>On module inputs</summary>\n",
                 "\n",
-                "  ---\n",
+                "---\n",
                 "\n",
-                "  Notice how the value for `l2_input`, was not just a single tensor.\n",
-                "  The type/shape of values from `.input` is in the form of:\n",
+                "Notice how the value for `l2_input`, was not just a single tensor. The\n",
+                "type/shape of values from `.input` is in the form of:\n",
                 "\n",
                 "      tuple(tuple(args), dictionary(kwargs))\n",
                 "\n",
-                "  Where the first index of the tuple is itself a tuple of all positional arguments, and the second index is a dictionary of the keyword arguments.\n",
+                "Where the first index of the tuple is itself a tuple of all positional\n",
+                "arguments, and the second index is a dictionary of the keyword arguments.\n",
                 "\n",
-                "  ---\n",
+                "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "\n",
-                "Now that we can access activations, we also want to do some post-processing on it. Let's find out which dimension of layer1's output has the highest value."
+                "Now that we can access activations, we also want to do some post-processing on\n",
+                "it. Let's find out which dimension of layer1's output has the highest value.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "p7Xo_PHyPr4p"
             },
             "source": [
-                "## Functions, Methods, and Operations"
+                "## Functions, Methods, and Operations\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "ehSofWbx5DSx"
             },
             "source": [
-                "We could do this by calling `torch.argmax(...)` after the tracing context or we can just leverage the fact that `nnsight` handles functions and methods within the tracing context, by creating a Proxy request for it:"
+                "We could do this by calling `torch.argmax(...)` after the tracing context or we\n",
+                "can just leverage the fact that `nnsight` handles functions and methods within\n",
+                "the tracing context, by creating a Proxy request for it:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -547,32 +596,38 @@
                         "tensor(5)\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Note we don't need to call .save() on the output,\n",
-                "  # as we're only using its value within the tracing context.\n",
-                "  l1_output = model.layer1.output\n",
+                "    # Note we don't need to call .save() on the output,\n",
+                "    # as we're only using its value within the tracing context.\n",
+                "    l1_output = model.layer1.output\n",
                 "\n",
-                "  l1_amax = torch.argmax(l1_output, dim=1).save()\n",
+                "    l1_amax = torch.argmax(l1_output, dim=1).save()\n",
                 "\n",
                 "print(l1_amax[0])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "BGPUJvWq_bOp"
             },
             "source": [
-                "Nice! That worked seamlessly, but hold on, how come we didn't need to call `.value[0]` on the result? In previous sections, we were just being explicit to get an understanding of Proxies and their value. In practice, however, `nnsight` knows that when outside of the tracing context we only care about the actual value, and so printing, indexing, and applying functions all immediately return and reflect the data in `.value`. So for the rest of the tutorial we won't use it.\n",
+                "Nice! That worked seamlessly, but hold on, how come we didn't need to call\n",
+                "`.value[0]` on the result? In previous sections, we were just being explicit to\n",
+                "get an understanding of Proxies and their value. In practice, however, `nnsight`\n",
+                "knows that when outside of the tracing context we only care about the actual\n",
+                "value, and so printing, indexing, and applying functions all immediately return\n",
+                "and reflect the data in `.value`. So for the rest of the tutorial we won't use\n",
+                "it.\n",
                 "\n",
-                "The same principles work for methods and operations as well:"
+                "The same principles work for methods and operations as well:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -589,48 +644,57 @@
                         "tensor(2.3416)\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  value = (model.layer1.output.sum() + model.layer2.output.sum()).save()\n",
+                "    value = (model.layer1.output.sum() + model.layer2.output.sum()).save()\n",
                 "\n",
                 "print(value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "V0vNOJtJ2oFR"
             },
             "source": [
-                "By default, torch functiona, methods and all operators work with `nnsight`. We also enable the use of the `einops` library.\n",
-                "\n",
-                "So to recap, the above code block is saying to `nnsight`, \"Run the model with the given `input`. When the output of layer1 is computed, take its sum. Then do the same for layer2. Now that both of those are computed, add them and make sure not to delete this value as I wish to use it outside of the tracing context.\"\n",
+                "By default, torch functions, methods and all operators work with `nnsight`. We\n",
+                "also enable the use of the `einops` library.\n",
                 "\n",
-                "Getting and analyzing the activations from various points in a model can be really insightful, and a number of ML techniques do exactly that. However, often times we not only want to view the computation of a model, but influence it as well."
+                "So to recap, the above code block is saying to `nnsight`, \"Run the model with\n",
+                "the given `input`. When the output of layer1 is computed, take its sum. Then do\n",
+                "the same for layer2. Now that both of those are computed, add them and make sure\n",
+                "not to delete this value as I wish to use it outside of the tracing context.\"\n",
+                "\n",
+                "Getting and analyzing the activations from various points in a model can be\n",
+                "really insightful, and a number of ML techniques do exactly that. However, often\n",
+                "times we not only want to view the computation of a model, but influence it as\n",
+                "well.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "m_5qH5gHPOT_"
             },
             "source": [
-                "## Setting"
+                "## Setting\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "rgju-b_IOLlq"
             },
             "source": [
-                "To demonstrate the effect of editing the flow of information through the model, let's set the first dimension of the first layer's output to 0. `NNsight` makes this really easy using '=' operator:"
+                "To demonstrate the effect of editing the flow of information through the model,\n",
+                "let's set the first dimension of the first layer's output to 0. `NNsight` makes\n",
+                "this really easy using '=' operator:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -650,35 +714,35 @@
                         "          0.2968, -0.8834]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  # Access the 0th index of the hidden state dimension and set it to 0.\n",
-                "  model.layer1.output[:, 0] = 0\n",
+                "    # Access the 0th index of the hidden state dimension and set it to 0.\n",
+                "    model.layer1.output[:, 0] = 0\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "oZz9SMs3Y_iS"
             },
             "source": [
-                "Seems our change was reflected. Now the same for the last dimension:"
+                "Seems our change was reflected. Now the same for the last dimension:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -704,50 +768,67 @@
                         "\u001b[0;31mIndexError\u001b[0m: index 10 is out of bounds for dimension 1 with size 10"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  # Access the last index of the hidden state dimension and set it to 0.\n",
-                "  model.layer1.output[:, hidden_dims] = 0\n",
+                "    # Access the last index of the hidden state dimension and set it to 0.\n",
+                "    model.layer1.output[:, hidden_dims] = 0\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "JCNR_Jkpxr8l"
             },
             "source": [
-                "Ah of course, we needed to index at `hidden_dims - 1` not `hidden_dims`. How did `nnsight` know there was this indexing error before leaving the tracing context?\n",
+                "Ah of course, we needed to index at `hidden_dims - 1` not `hidden_dims`. How did\n",
+                "`nnsight` know there was this indexing error before leaving the tracing context?\n",
                 "\n",
-                "Earlier when discussing contexts in Python, we learned some logic happens upon entering, and some logic happens upon exiting. We know the model is actually run on exit, but what happens on enter? Our input IS actually run though the model, however under its own \"fake\" context. This means the input makes its way through all of the model operations, allowing `nnsight` to record the shapes and data types of module inputs and outputs! The operations are never executed using tensors with real values so it doesn't incur any memory costs. Then, when creating proxy requests like the setting one above, `nnsight` also attempts to execute the request on the \"fake\" values we recorded. Hence, it lets us know if our request is feasible before even running the model.\n",
+                "Earlier when discussing contexts in Python, we learned some logic happens upon\n",
+                "entering, and some logic happens upon exiting. We know the model is actually run\n",
+                "on exit, but what happens on enter? Our input IS actually run though the model,\n",
+                "however under its own \"fake\" context. This means the input makes its way through\n",
+                "all of the model operations, allowing `nnsight` to record the shapes and data\n",
+                "types of module inputs and outputs! The operations are never executed using\n",
+                "tensors with real values so it doesn't incur any memory costs. Then, when\n",
+                "creating proxy requests like the setting one above, `nnsight` also attempts to\n",
+                "execute the request on the \"fake\" values we recorded. Hence, it lets us know if\n",
+                "our request is feasible before even running the model.\n",
                 "\n",
                 "<details>\n",
                 "<summary>On scanning</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
-                "\"Scanning\" is what we call running \"fake\" inputs throught the model to collect information like shapes and types. \"Validating\" is what we call trying to execute your intervention proxies with \"fake\" inputs to see if they work. If you are doing anything in a loop where efficiency is important, you should turn off scanning and validating. You can turn off validating in `.trace(...)` like `.trace(..., validate=False)`. You can turn off scanning in `Tracer.invoke(...)` ([see the Batching section](#batching-id)) like `Tracer.invoke(..., scan=False)`\n",
+                "\"Scanning\" is what we call running \"fake\" inputs through the model to collect\n",
+                "information like shapes and types. \"Validating\" is what we call trying to\n",
+                "execute your intervention proxies with \"fake\" inputs to see if they work. If you\n",
+                "are doing anything in a loop where efficiency is important, you should turn off\n",
+                "scanning and validating. You can turn off validating in `.trace(...)` like\n",
+                "`.trace(..., validate=False)`. You can turn off scanning in `Tracer.invoke(...)`\n",
+                "([see the Batching section](#batching-id)) like `Tracer.invoke(..., scan=False)`\n",
                 "\n",
                 "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "Let's try again with the correct indexing, and view the shape of the output before leaving the tracing context:"
+                "Let's try again with the correct indexing, and view the shape of the output\n",
+                "before leaving the tracing context:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -768,37 +849,39 @@
                         "          0.2968,  0.0000]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  print(f\"layer1 output shape: {model.layer1.output.shape}\")\n",
+                "    print(f\"layer1 output shape: {model.layer1.output.shape}\")\n",
                 "\n",
-                "  # Access the last index of the hidden state dimension and set it to 0.\n",
-                "  model.layer1.output[:, hidden_dims - 1] = 0\n",
+                "    # Access the last index of the hidden state dimension and set it to 0.\n",
+                "    model.layer1.output[:, hidden_dims - 1] = 0\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "9DH7PeL13-WU"
             },
             "source": [
-                "We can also just replace proxy inputs and outputs with tensors of the same shape and type. Let's use the shape information we have at our disposal to add noise to the output, and replace it with this new noised tensor:"
+                "We can also just replace proxy inputs and outputs with tensors of the same shape\n",
+                "and type. Let's use the shape information we have at our disposal to add noise\n",
+                "to the output, and replace it with this new noised tensor:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -818,40 +901,42 @@
                         "          0.3394, -0.9187]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  # Create random noise with variance of .001\n",
-                "  noise = (0.001**0.5)*torch.randn(l1_output_before.shape)\n",
+                "    # Create random noise with variance of .001\n",
+                "    noise = (0.001**0.5) * torch.randn(l1_output_before.shape)\n",
                 "\n",
-                "  # Add to original value and replace.\n",
-                "  model.layer1.output = l1_output_before + noise\n",
+                "    # Add to original value and replace.\n",
+                "    model.layer1.output = l1_output_before + noise\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "s016CelFP8sx"
             },
             "source": [
                 "## Gradients\n",
                 "\n",
-                "`NNsight` can also let you apply backprop and access gradients with respect to a loss. Like `.input` and `.output` on modules, `nnsight` also exposes `.grad` on Proxies themselves (assuming they are proxies of tensors):"
+                "`NNsight` can also let you apply backprop and access gradients with respect to a\n",
+                "loss. Like `.input` and `.output` on modules, `nnsight` also exposes `.grad` on\n",
+                "Proxies themselves (assuming they are proxies of tensors):\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -870,38 +955,40 @@
                         "Layer 2 output gradient: tensor([[1., 1.]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # We need to explicitly have the tensor require grad\n",
-                "  # as the model we defined earlier turned off requiring grad.\n",
-                "  model.layer1.output.requires_grad = True\n",
-                "\n",
-                "  # We call .grad on a tensor Proxy to communicate we want to store its gradient.\n",
-                "  # We need to call .save() of course as .grad is its own Proxy.\n",
-                "  layer1_output_grad = model.layer1.output.grad.save()\n",
-                "  layer2_output_grad = model.layer2.output.grad.save()\n",
-                "\n",
-                "  # Need a loss to propagate through the later modules in order to have a grad.\n",
-                "  loss = model.output.sum()\n",
-                "  loss.backward()\n",
+                "    # We need to explicitly have the tensor require grad\n",
+                "    # as the model we defined earlier turned off requiring grad.\n",
+                "    model.layer1.output.requires_grad = True\n",
+                "\n",
+                "    # We call .grad on a tensor Proxy to communicate we want to store its gradient.\n",
+                "    # We need to call .save() of course as .grad is its own Proxy.\n",
+                "    layer1_output_grad = model.layer1.output.grad.save()\n",
+                "    layer2_output_grad = model.layer2.output.grad.save()\n",
+                "\n",
+                "    # Need a loss to propagate through the later modules in order to have a grad.\n",
+                "    loss = model.output.sum()\n",
+                "    loss.backward()\n",
                 "\n",
                 "print(\"Layer 1 output gradient:\", layer1_output_grad)\n",
-                "print(\"Layer 2 output gradient:\", layer2_output_grad)\n"
+                "print(\"Layer 2 output gradient:\", layer2_output_grad)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "1o0JaaYvWlHG"
             },
             "source": [
-                "All of the features we learned previously, also apply to `.grad`. In other words, we can apply operations to and edit the gradients. Let's zero the grad of `layer1` and double the grad of `layer2`."
+                "All of the features we learned previously, also apply to `.grad`. In other\n",
+                "words, we can apply operations to and edit the gradients. Let's zero the grad of\n",
+                "`layer1` and double the grad of `layer2`.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -919,70 +1006,77 @@
                         "Layer 2 output gradient: tensor([[2., 2.]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # We need to explicitly have the tensor require grad\n",
-                "  # as the model we defined earlier turned off requiring grad.\n",
-                "  model.layer1.output.requires_grad = True\n",
-                "\n",
-                "  model.layer1.output.grad[:] = 0\n",
-                "  model.layer2.output.grad = model.layer2.output.grad.clone() * 2\n",
-                "\n",
-                "  layer1_output_grad = model.layer1.output.grad.save()\n",
-                "  layer2_output_grad = model.layer2.output.grad.save()\n",
-                "\n",
-                "  # Need a loss to propagate through the later modules in order to have a grad.\n",
-                "  loss = model.output.sum()\n",
-                "  loss.backward()\n",
+                "    # We need to explicitly have the tensor require grad\n",
+                "    # as the model we defined earlier turned off requiring grad.\n",
+                "    model.layer1.output.requires_grad = True\n",
+                "\n",
+                "    model.layer1.output.grad[:] = 0\n",
+                "    model.layer2.output.grad = model.layer2.output.grad.clone() * 2\n",
+                "\n",
+                "    layer1_output_grad = model.layer1.output.grad.save()\n",
+                "    layer2_output_grad = model.layer2.output.grad.save()\n",
+                "\n",
+                "    # Need a loss to propagate through the later modules in order to have a grad.\n",
+                "    loss = model.output.sum()\n",
+                "    loss.backward()\n",
                 "\n",
                 "print(\"Layer 1 output gradient:\", layer1_output_grad)\n",
                 "print(\"Layer 2 output gradient:\", layer2_output_grad)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "gvQ1nZgYQDG3"
             },
             "source": [
-                "# 2 Bigger"
+                "# 2 Bigger\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "miQgUY4NAmDQ"
             },
             "source": [
-                "Now that we have the basics of `nnsight` under our belt, we can scale our model up and combine the techniques we've learned into more interesting experiments.\n",
+                "Now that we have the basics of `nnsight` under our belt, we can scale our model\n",
+                "up and combine the techniques we've learned into more interesting experiments.\n",
                 "\n",
-                "The `NNsight` class is very bare bones. It wraps a pre-defined model and does no pre-processing on the inputs we enter. It's designed to be extended with more complex and powerful types of models and we're excited to see what can be done to leverage its features."
+                "The `NNsight` class is very bare bones. It wraps a pre-defined model and does no\n",
+                "pre-processing on the inputs we enter. It's designed to be extended with more\n",
+                "complex and powerful types of models and we're excited to see what can be done\n",
+                "to leverage its features.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "5TJDblHiQpp1"
             },
             "source": [
-                "## LanguageModel"
+                "## LanguageModel\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "9l9mZOY5HFH2"
             },
             "source": [
-                "`LanguageModel` is a subclass of `NNsight`.  While we could define and create a model to pass in directly, `LanguageModel` includes special support for Huggingface language models, including automatically loading models from a Huggingface ID, and loading the model together with the appropriate tokenizer.\n",
+                "`LanguageModel` is a subclass of `NNsight`. While we could define and create a\n",
+                "model to pass in directly, `LanguageModel` includes special support for\n",
+                "Huggingface language models, including automatically loading models from a\n",
+                "Huggingface ID, and loading the model together with the appropriate tokenizer.\n",
                 "\n",
-                "Here is how you can use `LanguageModel` to load `GPT-2`:"
+                "Here is how you can use `LanguageModel` to load `GPT-2`:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1141,15 +1235,15 @@
                         ")\n"
                     ]
                 }
             ],
             "source": [
                 "from nnsight import LanguageModel\n",
                 "\n",
-                "model = LanguageModel('openai-community/gpt2', device_map=\"auto\")\n",
+                "model = LanguageModel(\"openai-community/gpt2\", device_map=\"auto\")\n",
                 "\n",
                 "print(model)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -1159,27 +1253,41 @@
                 "<details>\n",
                 "<summary>On Model Initialization</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "A few important things to note:\n",
                 "\n",
-                "  Keyword arguments passed to the initialization of `LanguageModel` is forwarded to HuggingFace specific loading logic. In this case, `device_map` specifies which devices to use and its value `auto` indicates to evenly distribute it to all available GPUs (and cpu if no GPUs available). Other arguments can be found here: https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModelForCausalLM\n",
-                "\n",
-                "\n",
-                "  When we initialize `LanguageModel`, we aren't yet loading the parameters of the model into memory. We are actually loading a 'meta' version of the model which doesn't take up any memory, but still allows us to view and trace actions on it. After exiting the first tracing context, the model is then fully loaded into memory. To load into memory on initialization, you can pass `dispatch=True` into `LanguageModel` like `LanguageModel('openai-community/gpt2', device_map=\"auto\", dispatch=True)`.\n",
+                "Keyword arguments passed to the initialization of `LanguageModel` is forwarded\n",
+                "to HuggingFace specific loading logic. In this case, `device_map` specifies\n",
+                "which devices to use and its value `auto` indicates to evenly distribute it to\n",
+                "all available GPUs (and cpu if no GPUs available). Other arguments can be found\n",
+                "here:\n",
+                "https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModelForCausalLM\n",
+                "\n",
+                "When we initialize `LanguageModel`, we aren't yet loading the parameters of the\n",
+                "model into memory. We are actually loading a 'meta' version of the model which\n",
+                "doesn't take up any memory, but still allows us to view and trace actions on it.\n",
+                "After exiting the first tracing context, the model is then fully loaded into\n",
+                "memory. To load into memory on initialization, you can pass `dispatch=True` into\n",
+                "`LanguageModel` like\n",
+                "`LanguageModel('openai-community/gpt2', device_map=\"auto\", dispatch=True)`.\n",
                 "\n",
                 "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "\n",
-                "Let's put together some of the features we applied to the small model, but now on `GPT-2`. Unlike `NNsight`, `LanguageModel` does define logic to pre-process inputs upon entering the tracing context. This makes interacting with the model simpler without having to directly access the tokenizer.\n",
-                "\n",
-                "In the following example, we ablate the value coming from the last layer's MLP module and decode the logits to see what token the model predicts without influence from that particular module:"
+                "Let's put together some of the features we applied to the small model, but now\n",
+                "on `GPT-2`. Unlike `NNsight`, `LanguageModel` does define logic to pre-process\n",
+                "inputs upon entering the tracing context. This makes interacting with the model\n",
+                "simpler without having to directly access the tokenizer.\n",
+                "\n",
+                "In the following example, we ablate the value coming from the last layer's MLP\n",
+                "module and decode the logits to see what token the model predicts without\n",
+                "influence from that particular module:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1202,74 +1310,102 @@
                     "text": [
                         "Token IDs: tensor([[ 262,   12,  417, 8765,   11,  257,  262, 3504,  338, 3576]])\n",
                         "Prediction:  London\n"
                     ]
                 }
             ],
             "source": [
-                "with model.trace('The Eiffel Tower is in the city of'):\n",
+                "with model.trace(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "  # Access the last layer using h[-1] as it's a ModuleList\n",
-                "  # Access the first index of .output as that's where the hidden states are.\n",
-                "  model.transformer.h[-1].mlp.output[0][:] = 0\n",
+                "    # Access the last layer using h[-1] as it's a ModuleList\n",
+                "    # Access the first index of .output as that's where the hidden states are.\n",
+                "    model.transformer.h[-1].mlp.output[0][:] = 0\n",
                 "\n",
-                "  # Logits come out of model.lm_head and we apply argmax to get the predicted token ids.\n",
-                "  token_ids = model.lm_head.output.argmax(dim=-1).save()\n",
+                "    # Logits come out of model.lm_head and we apply argmax to get the predicted token ids.\n",
+                "    token_ids = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
                 "print(\"Token IDs:\", token_ids)\n",
                 "\n",
                 "# Apply the tokenizer to decode the ids into words after the tracing context.\n",
-                "print(\"Prediction:\", model.tokenizer.decode(token_ids[0][-1]))\n"
+                "print(\"Prediction:\", model.tokenizer.decode(token_ids[0][-1]))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "X2-HiCQhkv-B"
             },
             "source": [
-                "You just ran a little intervention on a much more complex model with a lot more parameters! An important piece of information we're missing though is what the prediction would look like without our ablation.\n",
-                "\n",
-                "Of course we could just run two tracing contexts and compare the outputs. This, however, would require two forward passes through the model. `NNsight` can do better than that."
+                "You just ran a little intervention on a much more complex model with a lot more\n",
+                "parameters! An important piece of information we're missing though is what the\n",
+                "prediction would look like without our ablation.\n",
+                "\n",
+                "Of course we could just run two tracing contexts and compare the outputs. This,\n",
+                "however, would require two forward passes through the model. `NNsight` can do\n",
+                "better than that.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "vLjHnRyRPXjp"
             },
             "source": [
                 "<a name=\"batching-id\"></a>\n",
-                "## Batching"
+                "\n",
+                "## Batching\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "_Gc-Zr6NmEOn"
             },
             "source": [
-                "It's time to bring back the `Tracer` object we dropped before. See, when you call `.trace(...)` with some input, it's actually creating two different contexts behind the scenes. The second one is the invoker context. Being within this context just means that `.input` and `.output` should refer only to the input you've given invoke. Calling `.trace(...)` with some input just means there's only one input and therefore only one invoker context.\n",
-                "\n",
-                "We can call `.trace()` without input and call `Tracer.invoke(...)` to manually create the invoker context with our input. Now every subsequent time we call `.invoke(...)`, new interventions will only refer to the input in that particular invoke. When exiting the tracing context, the inputs from all of the invokers will be batched together, and they will be executed in one forward pass! So let's do the ablation experiment, and compute a 'control' output to compare to:\n",
+                "It's time to bring back the `Tracer` object we dropped before. See, when you\n",
+                "call `.trace(...)` with some input, it's actually creating two different\n",
+                "contexts behind the scenes. The second one is the invoker context. Being within\n",
+                "this context just means that `.input` and `.output` should refer only to the\n",
+                "input you've given invoke. Calling `.trace(...)` with some input just means\n",
+                "there's only one input and therefore only one invoker context.\n",
+                "\n",
+                "We can call `.trace()` without input and call `Tracer.invoke(...)` to manually\n",
+                "create the invoker context with our input. Now every subsequent time we call\n",
+                "`.invoke(...)`, new interventions will only refer to the input in that\n",
+                "particular invoke. When exiting the tracing context, the inputs from all of the\n",
+                "invokers will be batched together, and they will be executed in one forward\n",
+                "pass! So let's do the ablation experiment, and compute a 'control' output to\n",
+                "compare to:\n",
                 "\n",
                 "<details>\n",
                 "<summary>On the invoker context</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
-                "Note that when injecting data to only the relevant invoker interventions, `nnsight` tries, but can't guarantee, that it can narrow the data into the right batch idxs (in the case of an object as input or output). So there are cases where all invokes will get all of the data.\n",
-                "\n",
-                "Just like `.trace(...)` created a `Tracer` object, `.invoke(...)` creates an `Invoker` object. The `Invoker` object has post-processed inputs at `invoker.inputs`, which can be useful for seeing information about your input. If you are using `.trace(...)` with inputs, you can still access the invoker object at `tracer._invoker`.\n",
-                "\n",
-                "Keyword arguments given to `.invoke(..)` make its way to the input pre-processing. For example in `LanguageModel`, the keyword arguments are used to tokenize like `max_length` and `truncation`. If you need to pass in keyword arguments directly to one input `.trace(...)`, you can pass an `invoker_args` keyword argument that should be a dictionary of keyword arguments for the invoker. `.trace(..., invoker_args={...})`\n",
+                "Note that when injecting data to only the relevant invoker interventions,\n",
+                "`nnsight` tries, but can't guarantee, that it can narrow the data into the right\n",
+                "batch idxs (in the case of an object as input or output). So there are cases\n",
+                "where all invokes will get all of the data.\n",
+                "\n",
+                "Just like `.trace(...)` created a `Tracer` object, `.invoke(...)` creates an\n",
+                "`Invoker` object. The `Invoker` object has post-processed inputs at\n",
+                "`invoker.inputs`, which can be useful for seeing information about your input.\n",
+                "If you are using `.trace(...)` with inputs, you can still access the invoker\n",
+                "object at `tracer._invoker`.\n",
+                "\n",
+                "Keyword arguments given to `.invoke(..)` make its way to the input\n",
+                "pre-processing. For example in `LanguageModel`, the keyword arguments are used\n",
+                "to tokenize like `max_length` and `truncation`. If you need to pass in keyword\n",
+                "arguments directly to one input `.trace(...)`, you can pass an `invoker_args`\n",
+                "keyword argument that should be a dictionary of keyword arguments for the\n",
+                "invoker. `.trace(..., invoker_args={...})`\n",
                 "\n",
                 "---\n",
                 "\n",
-                "</details>"
+                "</details>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1289,26 +1425,26 @@
                         "Intervention prediction:  London\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace() as tracer:\n",
                 "\n",
-                "  with tracer.invoke('The Eiffel Tower is in the city of'):\n",
+                "    with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "    # Ablate the last MLP for only this batch.\n",
-                "    model.transformer.h[-1].mlp.output[0][:] = 0\n",
+                "        # Ablate the last MLP for only this batch.\n",
+                "        model.transformer.h[-1].mlp.output[0][:] = 0\n",
                 "\n",
-                "    # Get the output for only the intervened on batch.\n",
-                "    token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        # Get the output for only the intervened on batch.\n",
+                "        token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
-                "  with tracer.invoke('The Eiffel Tower is in the city of'):\n",
+                "    with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "    # Get the output for only the original batch.\n",
-                "    token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        # Get the output for only the original batch.\n",
+                "        token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
                 "print(\"Original token IDs:\", token_ids_original)\n",
                 "print(\"Intervention token IDs:\", token_ids_intervention)\n",
                 "\n",
                 "print(\"Original prediction:\", model.tokenizer.decode(token_ids_original[0][-1]))\n",
                 "print(\"Intervention prediction:\", model.tokenizer.decode(token_ids_intervention[0][-1]))"
             ]
@@ -1317,15 +1453,18 @@
             "cell_type": "markdown",
             "metadata": {
                 "id": "8BsybgsK2Bbr"
             },
             "source": [
                 "So it did end up affecting what the model predicted. That's pretty neat!\n",
                 "\n",
-                "Another cool thing with multiple invokes is that the Proxies can interact between them. Here we transfer the word token embeddings from a real prompt into another placeholder prompt. Therefore the latter prompt produces the output of the former prompt:"
+                "Another cool thing with multiple invokes is that the Proxies can interact\n",
+                "between them. Here we transfer the word token embeddings from a real prompt into\n",
+                "another placeholder prompt. Therefore the latter prompt produces the output of\n",
+                "the former prompt:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1343,45 +1482,54 @@
                         "Intervention prediction:  Paris\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace() as tracer:\n",
                 "\n",
-                "  with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
+                "    with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "    embeddings = model.transformer.wte.output\n",
+                "        embeddings = model.transformer.wte.output\n",
                 "\n",
-                "  with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
+                "    with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
                 "\n",
-                "    model.transformer.wte.output = embeddings\n",
+                "        model.transformer.wte.output = embeddings\n",
                 "\n",
-                "    token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
-                "  with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
+                "    with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
                 "\n",
-                "    token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
                 "print(\"Original prediction:\", model.tokenizer.decode(token_ids_original[0][-1]))\n",
                 "print(\"Intervention prediction:\", model.tokenizer.decode(token_ids_intervention[0][-1]))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "vvWA-CWqQtah"
             },
             "source": [
                 "## .next()\n",
                 "\n",
-                "Some HuggingFace models define methods to generate multiple outputs at a time. `LanguageModel` wraps that functionality to provide the same tracing features by using `.generate(...)` instead of `.trace(...)`. This calls the underlying model's `.generate` method. It passes the output through a `model.generator` module that we've added onto the model, allowing you to get the generate output at `model.generator.output`.\n",
-                "\n",
-                "In a case like this, the underlying model is called more than once; the modules of said model produce more than one output. Which iteration should a given `module.output` refer to? That's where `Module.next()` comes in.\n",
-                "\n",
-                "Each module has a call idx associated with it and `.next()` simply increments that attribute. At the time of execution, data is injected into the intervention graph only at the iteration that matches the call idx."
+                "Some HuggingFace models define methods to generate multiple outputs at a time.\n",
+                "`LanguageModel` wraps that functionality to provide the same tracing features by\n",
+                "using `.generate(...)` instead of `.trace(...)`. This calls the underlying\n",
+                "model's `.generate` method. It passes the output through a `model.generator`\n",
+                "module that we've added onto the model, allowing you to get the generate output\n",
+                "at `model.generator.output`.\n",
+                "\n",
+                "In a case like this, the underlying model is called more than once; the modules\n",
+                "of said model produce more than one output. Which iteration should a given\n",
+                "`module.output` refer to? That's where `Module.next()` comes in.\n",
+                "\n",
+                "Each module has a call idx associated with it and `.next()` simply increments\n",
+                "that attribute. At the time of execution, data is injected into the intervention\n",
+                "graph only at the iteration that matches the call idx.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1412,21 +1560,21 @@
                         "All prediction:  ['The Eiffel Tower is in the city of Paris, and']\n"
                     ]
                 }
             ],
             "source": [
                 "with model.generate(\"The Eiffel Tower is in the city of\", max_new_tokens=3):\n",
                 "\n",
-                "  token_ids_1 = model.lm_head.output.argmax(dim=-1).save()\n",
+                "    token_ids_1 = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
-                "  token_ids_2 = model.lm_head.next().output.argmax(dim=-1).save()\n",
+                "    token_ids_2 = model.lm_head.next().output.argmax(dim=-1).save()\n",
                 "\n",
-                "  token_ids_3 = model.lm_head.next().output.argmax(dim=-1).save()\n",
+                "    token_ids_3 = model.lm_head.next().output.argmax(dim=-1).save()\n",
                 "\n",
-                "  output = model.generator.output.save()\n",
+                "    output = model.generator.output.save()\n",
                 "\n",
                 "print(\"Prediction 1: \", model.tokenizer.decode(token_ids_1[0][-1]))\n",
                 "print(\"Prediction 2: \", model.tokenizer.decode(token_ids_2[0][-1]))\n",
                 "print(\"Prediction 3: \", model.tokenizer.decode(token_ids_3[0][-1]))\n",
                 "\n",
                 "print(\"All token ids: \", output)\n",
                 "\n",
@@ -1435,48 +1583,58 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "rpkX-LwBQZHo"
             },
             "source": [
-                "# 3 I thought you said huge models?"
+                "# 3 I thought you said huge models?\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "uCZR65VmILEb"
             },
             "source": [
-                "`NNsight` is only one part of our project to democratize access to AI internals. The other half is `NDIF` (National Deep Inference Facility).\n",
+                "`NNsight` is only one part of our project to democratize access to AI internals.\n",
+                "The other half is `NDIF` (National Deep Inference Facility).\n",
                 "\n",
-                "The interaction between the two is fairly straightforward. The `intervention graph` we create via the tracing context can be encoded into a custom json format and sent via an http request to the `NDIF` servers. `NDIF` then decodes the `intervention graph` and `interleaves` it alongside the specified model.\n",
+                "The interaction between the two is fairly straightforward. The\n",
+                "`intervention graph` we create via the tracing context can be encoded into a\n",
+                "custom json format and sent via an http request to the `NDIF` servers. `NDIF`\n",
+                "then decodes the `intervention graph` and `interleaves` it alongside the\n",
+                "specified model.\n",
                 "\n",
-                "To see which models are currently being hosted, check out the following status page: https://nnsight.net/status/"
+                "To see which models are currently being hosted, check out the following status\n",
+                "page: https://nnsight.net/status/\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "65Ks1LUvQaER"
             },
             "source": [
-                "## Remote execution"
+                "## Remote execution\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "Aa-ZuVOFKS5k"
             },
             "source": [
-                "In its current state, `NDIF` requires you to recieve an API key. Therefore, to run the rest of this colab, you would need one of your own. To get one, simply join the [NDIF discord](https://discord.gg/6uFJmCSwW7) and introduce yourself on the `#introductions` channel. Then DM either @JadenFK or @caden and we'll create one for you.\n",
+                "In its current state, `NDIF` requires you to receive an API key. Therefore, to\n",
+                "run the rest of this Colab, you would need one of your own. To get one, simply\n",
+                "join the [NDIF discord](https://discord.gg/6uFJmCSwW7) and introduce yourself on\n",
+                "the `#introductions` channel. Then DM either @JadenFK or @caden and we'll create\n",
+                "one for you.\n",
                 "\n",
-                "Once you have one, to register your api key with `nnsight`, do the following:"
+                "Once you have one, to register your api key with `nnsight`, do the following:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "ax1NWoS9MJeZ"
@@ -1490,17 +1648,19 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "mvXLOh65MXmF"
             },
             "source": [
-                "This only needs to be run once as it will save this api key as the default in a config file along with the `nnsight` installation.\n",
+                "This only needs to be run once as it will save this api key as the default in a\n",
+                "config file along with the `nnsight` installation.\n",
                 "\n",
-                "To amp things up a few levels, let's demonstrate using `nnsight`'s tracing context with one of the larger open source language models, `Llama-2-70b`!"
+                "To amp things up a few levels, let's demonstrate using `nnsight`'s tracing\n",
+                "context with one of the larger open source language models, `Llama-2-70b`!\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "Q1N04sJPZnJt"
@@ -1527,61 +1687,66 @@
             },
             "outputs": [],
             "source": [
                 "# We'll never actually load the parameters so no need to specify a device_map.\n",
                 "model = LanguageModel(\"meta-llama/Llama-2-70b-hf\")\n",
                 "\n",
                 "# All we need to specify using NDIF vs executing locally is remote=True.\n",
-                "with model.trace('The Eiffel Tower is in the city of', remote=True) as runner:\n",
+                "with model.trace(\"The Eiffel Tower is in the city of\", remote=True) as runner:\n",
                 "\n",
                 "    hidden_states = model.model.layers[-1].output.save()\n",
                 "\n",
                 "    output = model.output.save()\n",
                 "\n",
                 "print(hidden_states)\n",
                 "\n",
-                "print(output['logits'])"
+                "print(output[\"logits\"])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "IceVpnZcZ9F0"
             },
             "source": [
-                "It really is as simple as `remote=True`. All of the techniques we went through in earlier sections work just the same when running locally and remotely.\n",
+                "It really is as simple as `remote=True`. All of the techniques we went through\n",
+                "in earlier sections work just the same when running locally and remotely.\n",
                 "\n",
-                "Note that both `nnsight`, but especially `NDIF`, is in active development and therefore there may be caveats, changes, and errors to work through."
+                "Note that both `nnsight`, but especially `NDIF`, is in active development and\n",
+                "therefore there may be caveats, changes, and errors to work through.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "P3zRm-7VRRov"
             },
             "source": [
-                "# Getting Involved!"
+                "# Getting Involved!\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "BnCc9xgjvxEP"
             },
             "source": [
-                "If you're interested in following updates to `nnsight`, contributing, giving feedback, or finding collaborators, please join the [NDIF discord](https://discord.gg/6uFJmCSwW7)!\n",
-                "\n",
-                "The [Mech Interp discord](https://discord.gg/km2RQBzaUn) is also a fantastic place to discuss all things mech interp with a really cool community.\n",
-                "\n",
-                "Our website [nnsight.net](https://nnsight.net/), has a bunch more tutorials detailing more complex interpretability techniques using `nnsight`. If you want to share any of the work you do using `nnsight`, let others know on either of the discords above and we might turn it into a tutorial on our website.\n",
-                "\n",
-                "\ud83d\udc9f\n",
-                "\n",
+                "If you're interested in following updates to `nnsight`, contributing, giving\n",
+                "feedback, or finding collaborators, please join the\n",
+                "[NDIF discord](https://discord.gg/6uFJmCSwW7)!\n",
+                "\n",
+                "The [Mech Interp discord](https://discord.gg/km2RQBzaUn) is also a fantastic\n",
+                "place to discuss all things mech interp with a really cool community.\n",
+                "\n",
+                "Our website [nnsight.net](https://nnsight.net/), has a bunch more tutorials\n",
+                "detailing more complex interpretability techniques using `nnsight`. If you want\n",
+                "to share any of the work you do using `nnsight`, let others know on either of\n",
+                "the discords above and we might turn it into a tutorial on our website.\n",
                 "\n",
-                "\n"
+                "\ud83d\udc9f\n"
             ]
         }
     ],
     "metadata": {
         "colab": {
             "include_colab_link": true,
             "provenance": [],
```

### Comparing `nnsight-0.2.8/PKG-INFO` & `nnsight-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnsight
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package for interpreting and manipulating the internals of deep learning models.
 Author-email: Jaden Fiotto-Kaufman <jadenfk@outlook.com>
 Project-URL: Homepage, https://github.com/JadenFiotto-Kaufman/nnsight
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nnsight Version: 0.2.8 Summary: Package for
+Metadata-Version: 2.1 Name: nnsight Version: 0.2.9 Summary: Package for
 interpreting and manipulating the internals of deep learning models. Author-
 email: Jaden Fiotto-Kaufman
 outlook.com> Project-URL: Homepage, https://github.com/JadenFiotto-Kaufman/
 nnsight Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE Requires-Dist: transformers Requires-Dist: protobuf Requires-Dist:
```

### Comparing `nnsight-0.2.8/README.md` & `nnsight-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/.DS_Store` & `nnsight-0.2.9/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/Makefile` & `nnsight-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/contributing.md` & `nnsight-0.2.9/docs/contributing.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Installation 
+# Installation
 
-Run `pip install -r requirements.txt` while in the `nnsight/docs` directory. 
+Run `pip install -r requirements.txt` while in the `nnsight/docs` directory.
+
+If you haven't already, you should also install pandoc. With brew run: `brew install pandoc`
 
 # Adding Tutorials
 
-Tutorials are written as Jupyter Notebooks in `.ipynb` format, and automatically converted to html by the `nbsphinx` extension. 
+Tutorials are written as Jupyter Notebooks in `.ipynb` format, and automatically converted to html by the `nbsphinx` extension.
 
-The only requirement of `nbsphinx` is that you add a header to the notebook to act as the rendered title on Sphinx docs. To do this, create a markdown cell at the top of your notebook with a header `#`. 
+The only requirement of `nbsphinx` is that you add a header to the notebook to act as the rendered title on Sphinx docs. To do this, create a markdown cell at the top of your notebook with a header `#`.
 
-Then, just add your notebook to the `nnsight/docs/source/notebooks/tutorials` directory. 
+Then, just add your notebook to the `nnsight/docs/source/notebooks/tutorials` directory.
 
 If you're adding a new notebook, navigate to `nnsight/docs/source/tutorials.rst`. At the bottom of the page, add the path to your notebook under the `toctree`.
 
 ```
 .. toctree::
    :maxdepth: 1
```

### Comparing `nnsight-0.2.8/docs/make.bat` & `nnsight-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/.DS_Store` & `nnsight-0.2.9/docs/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/.DS_Store` & `nnsight-0.2.9/docs/source/_static/.DS_Store`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/css/custom.css` & `nnsight-0.2.9/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/css/front.css` & `nnsight-0.2.9/docs/source/_static/css/front.css`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/css/hljs-dark.css` & `nnsight-0.2.9/docs/source/_static/css/hljs-dark.css`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/css/hljs-light.css` & `nnsight-0.2.9/docs/source/_static/css/hljs-light.css`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/.DS_Store` & `nnsight-0.2.9/docs/source/_static/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/attribute_lens.png` & `nnsight-0.2.9/docs/source/_static/images/attribute_lens.png`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/execution.png` & `nnsight-0.2.9/docs/source/_static/images/execution.png`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/icon.ico` & `nnsight-0.2.9/docs/source/_static/images/icon.ico`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/interleaved.png` & `nnsight-0.2.9/docs/source/_static/images/interleaved.png`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/ioi.png` & `nnsight-0.2.9/docs/source/_static/images/ioi.png`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/nnsight_logo.svg` & `nnsight-0.2.9/docs/source/_static/images/nnsight_logo.svg`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/one.png` & `nnsight-0.2.9/docs/source/_static/images/one.png`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/.DS_Store` & `nnsight-0.2.9/docs/source/_static/images/tutorials/.DS_Store`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/activation_patching.webp` & `nnsight-0.2.9/docs/source/_static/images/tutorials/activation_patching.webp`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/attribution_patching.webp` & `nnsight-0.2.9/docs/source/_static/images/tutorials/attribution_patching.webp`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/dictionary_learning.webp` & `nnsight-0.2.9/docs/source/_static/images/tutorials/dictionary_learning.webp`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/function_vectors.webp` & `nnsight-0.2.9/docs/source/_static/images/tutorials/function_vectors.webp`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/future_lens.webp` & `nnsight-0.2.9/docs/source/_static/images/tutorials/future_lens.webp`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/logit_lens.webp` & `nnsight-0.2.9/docs/source/_static/images/tutorials/logit_lens.webp`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/tutorials/walkthrough.webp` & `nnsight-0.2.9/docs/source/_static/images/tutorials/walkthrough.webp`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/images/two.png` & `nnsight-0.2.9/docs/source/_static/images/two.png`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/js/.DS_Store` & `nnsight-0.2.9/docs/source/_static/js/.DS_Store`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/js/code.js` & `nnsight-0.2.9/docs/source/_static/js/code.js`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_static/js/custom.js` & `nnsight-0.2.9/docs/source/_static/js/custom.js`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/_templates/ndif_status.html` & `nnsight-0.2.9/docs/source/_templates/ndif_status.html`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/about.rst` & `nnsight-0.2.9/docs/source/about.rst`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/conf.py` & `nnsight-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/features.rst` & `nnsight-0.2.9/docs/source/features.rst`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/index.rst` & `nnsight-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/cross_prompt.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/cross_prompt.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/getting.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/getting.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/gradients.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/gradients.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/modules.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/modules.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/multiple_token.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/multiple_token.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/operations.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/operations.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/setting.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/setting.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/features/token_indexing.ipynb` & `nnsight-0.2.9/docs/source/notebooks/features/token_indexing.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/tutorials/attribution_patching.ipynb` & `nnsight-0.2.9/docs/source/notebooks/tutorials/attribution_patching.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/tutorials/ioi_patching.ipynb` & `nnsight-0.2.9/docs/source/notebooks/tutorials/ioi_patching.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/tutorials/logit_lens.ipynb` & `nnsight-0.2.9/docs/source/notebooks/tutorials/logit_lens.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/tutorials/sae.ipynb` & `nnsight-0.2.9/docs/source/notebooks/tutorials/sae.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/notebooks/tutorials/walkthrough.ipynb` & `nnsight-0.2.9/docs/source/notebooks/tutorials/walkthrough.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868556961437944%*

 * *Differences: {"'cells'": "{0: {'source': ['# Walkthrough\\n']}, 1: {'source': {insert: [(0, 'An interactive "*

 * *            "version of this walkthrough can be found\\n'), (1, "*

 * *            "'[here](https://colab.research.google.com/github/JadenFiotto-Kaufman/nnsight/blob/dev/NNsight_v0_2.ipynb)\\n'), "*

 * *            "(3, 'In this era of large-scale deep learning, the most interesting AI models "*

 * *            "are\\n'), (4, 'massive black boxes that are hard to run. Ordinary commercial "*

 * *            "inference service\\n'),  […]*

```diff
@@ -1,54 +1,60 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Walkthrough"
+                "# Walkthrough\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "-Scfr942GwO4"
             },
             "source": [
-                "An interactive version of this walkthrough can be found [here](https://colab.research.google.com/github/JadenFiotto-Kaufman/nnsight/blob/dev/NNsight_v0_2.ipynb)\n",
+                "An interactive version of this walkthrough can be found\n",
+                "[here](https://colab.research.google.com/github/JadenFiotto-Kaufman/nnsight/blob/dev/NNsight_v0_2.ipynb)\n",
                 "\n",
-                "In this era of large-scale deep learning, the most interesting AI models are massive black boxes that are hard to run. Ordinary commercial inference service APIs let you interact with huge models, but they do not let you access model internals.\n",
-                "\n",
-                "The nnsight library is different: it gives you full access to all the neural network internals. When used together with a remote service like the [National Deep Inference Facility](https://thevisible.net/docs/NDIF-proposal.pdf) (NDIF), it lets you run complex experiments on huge open source models easily, with fully transparent access.\n",
-                "\n",
-                "Our team wants to enable entire labs and independent researchers alike, as we believe a large, passionate, and collaborative community will produce the next big insights on a profoundly important field.\n",
-                "\n",
-                "\n"
+                "In this era of large-scale deep learning, the most interesting AI models are\n",
+                "massive black boxes that are hard to run. Ordinary commercial inference service\n",
+                "APIs let you interact with huge models, but they do not let you access model\n",
+                "internals.\n",
+                "\n",
+                "The nnsight library is different: it gives you full access to all the neural\n",
+                "network internals. When used together with a remote service like the\n",
+                "[National Deep Inference Facility](https://thevisible.net/docs/NDIF-proposal.pdf)\n",
+                "(NDIF), it lets you run complex experiments on huge open source models easily,\n",
+                "with fully transparent access.\n",
+                "\n",
+                "Our team wants to enable entire labs and independent researchers alike, as we\n",
+                "believe a large, passionate, and collaborative community will produce the next\n",
+                "big insights on a profoundly important field.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "N1OemD2VGyZx"
             },
             "source": [
-                "# 1 First, let's start small\n",
-                "\n",
-                "\n",
-                "\n"
+                "# 1 First, let's start small\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "WyLMmhrAKTNM"
             },
             "source": [
                 "## The Tracing Context\n",
                 "\n",
-                "To demonstrate the core functionality and syntax of nnsight, we'll define and use a tiny two layer neural network."
+                "To demonstrate the core functionality and syntax of nnsight, we'll define and\n",
+                "use a tiny two layer neural network.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "R0RJijD0eXwf"
@@ -65,15 +71,17 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "bgydw7i3HmIH"
             },
             "source": [
-                "Our little model here is composed of four sub-modules, two linear layers ('layer1', 'layer2'). We specify the sizes of each of these modules, and create some complementary example input."
+                "Our little model here is composed of four sub-modules, two linear layers\n",
+                "('layer1', 'layer2'). We specify the sizes of each of these modules, and create\n",
+                "some complementary example input.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "2pX2Wg8Ceo6N"
@@ -83,29 +91,34 @@
                 "from collections import OrderedDict\n",
                 "import torch\n",
                 "\n",
                 "input_size = 5\n",
                 "hidden_dims = 10\n",
                 "output_size = 2\n",
                 "\n",
-                "net = torch.nn.Sequential(OrderedDict([\n",
-                "    ('layer1', torch.nn.Linear(input_size, hidden_dims)),\n",
-                "    ('layer2', torch.nn.Linear(hidden_dims, output_size)),\n",
-                "])).requires_grad_(False)\n",
+                "net = torch.nn.Sequential(\n",
+                "    OrderedDict(\n",
+                "        [\n",
+                "            (\"layer1\", torch.nn.Linear(input_size, hidden_dims)),\n",
+                "            (\"layer2\", torch.nn.Linear(hidden_dims, output_size)),\n",
+                "        ]\n",
+                "    )\n",
+                ").requires_grad_(False)\n",
                 "\n",
                 "input = torch.rand((1, input_size))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "tIPa2h2pJIwl"
             },
             "source": [
-                "The core object of the nnsight package is `NNsight`. This wraps around a given pytorch model to enable the capabilites nnsight provides."
+                "The core object of the nnsight package is `NNsight`. This wraps around a given\n",
+                "pytorch model to enable the capabilities nnsight provides.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "8H9R_ynTJI5y"
@@ -119,15 +132,16 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "2NfISlQ_Ilvp"
             },
             "source": [
-                "Printing a Pytorch model shows a named hierarchy of modules which is very useful when accessing sub-components directly. NNsight models work the same."
+                "Printing a Pytorch model shows a named hierarchy of modules which is very useful\n",
+                "when accessing sub-components directly. NNsight models work the same.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -154,87 +168,109 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "djC5kyJWLuUH"
             },
             "source": [
-                "Before we actually get to using the model we just created, let's talk about Python contexts.\n",
+                "Before we actually get to using the model we just created, let's talk about\n",
+                "Python contexts.\n",
                 "\n",
-                "Python contexts define a scope using the `with` statement and are often used to create some object, or initiate some logic, that you later want to destroy or conclude.\n",
+                "Python contexts define a scope using the `with` statement and are often used to\n",
+                "create some object, or initiate some logic, that you later want to destroy or\n",
+                "conclude.\n",
                 "\n",
                 "The most common application is opening files like the following example:\n",
                 "\n",
                 "```python\n",
                 "with open('myfile.txt', 'r') as file:\n",
                 "  text = file.read()\n",
                 "```\n",
                 "\n",
-                "Python uses the `with` keyword to enter a context-like object. This object defines logic to be run at the start of the `with` block, as well as logic to be run when exiting. When using `with` for a file, entering the context opens the file and exiting the context closes it. Being within the context means we can read from the file. Simple enough! Now we can discuss how `nnsight` uses contexts to enable intuitive access into the internals of a neural network.\n"
+                "Python uses the `with` keyword to enter a context-like object. This object\n",
+                "defines logic to be run at the start of the `with` block, as well as logic to be\n",
+                "run when exiting. When using `with` for a file, entering the context opens the\n",
+                "file and exiting the context closes it. Being within the context means we can\n",
+                "read from the file. Simple enough! Now we can discuss how `nnsight` uses\n",
+                "contexts to enable intuitive access into the internals of a neural network.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "iNvuCOeyojcA"
             },
             "source": [
                 "The main tool with `nnsight` is a context for tracing.\n",
                 "\n",
-                "We enter the tracing context by calling `model.trace(<input>)` on an `NNsight` model, which defines how we want to run the model. Inside the context, we will be able to customize how the neural network runs. The model is actually run upon exiting the tracing context."
+                "We enter the tracing context by calling `model.trace(<input>)` on an `NNsight`\n",
+                "model, which defines how we want to run the model. Inside the context, we will\n",
+                "be able to customize how the neural network runs. The model is actually run upon\n",
+                "exiting the tracing context.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "qEXQ4auPSL-m"
             },
             "outputs": [],
             "source": [
                 "with model.trace(input) as tracer:\n",
-                "  pass"
+                "    pass"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "UZQsHinjqicJ"
             },
             "source": [
-                "But where's the output? To get that, we'll have to learn how to request it from within the tracing conext."
+                "But where's the output? To get that, we'll have to learn how to request it from\n",
+                "within the tracing context.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "xMfBpYzDPMoB"
             },
             "source": [
-                "## Getting"
+                "## Getting\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "B5_aFwFRv0ax"
             },
             "source": [
-                "Earlier, when we wrapped our little neural net with the `NNsight` class. This added a couple properties to each module in the model (including the root model itself). The two most important ones are `.input` and `.output`.\n",
+                "Earlier, when we wrapped our little neural net with the `NNsight` class. This\n",
+                "added a couple properties to each module in the model (including the root model\n",
+                "itself). The two most important ones are `.input` and `.output`.\n",
                 "\n",
                 "```python\n",
                 "model.input\n",
                 "model.output\n",
                 "```\n",
                 "\n",
-                "The names are self explainatory. They correspond to the inputs and outputs of their respective modules during a forward pass of the model. We can use these attributes inside the `with` block.\n",
-                "\n",
-                "However, it is important to understand that the model is not executed until the end of the tracing context. How can we access inputs and outputs before the model is run? The trick is deferred execution.\n",
-                "\n",
-                "`.input` and `.output` are Proxies for the eventual inputs and outputs of a module. In other words, when you access `model.output` what you are communicating to `nnsight` is, \"When you compute the output of `model`, please grab it for me and put the value into its corresponding Proxy object's `.value` attribute.\" Let's try it:"
+                "The names are self explanatory. They correspond to the inputs and outputs of\n",
+                "their respective modules during a forward pass of the model. We can use these\n",
+                "attributes inside the `with` block.\n",
+                "\n",
+                "However, it is important to understand that the model is not executed until the\n",
+                "end of the tracing context. How can we access inputs and outputs before the\n",
+                "model is run? The trick is deferred execution.\n",
+                "\n",
+                "`.input` and `.output` are Proxies for the eventual inputs and outputs of a\n",
+                "module. In other words, when you access `model.output` what you are\n",
+                "communicating to `nnsight` is, \"When you compute the output of `model`, please\n",
+                "grab it for me and put the value into its corresponding Proxy object's `.value`\n",
+                "attribute.\" Let's try it:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -257,30 +293,32 @@
                         "\u001b[0;31mValueError\u001b[0m: Accessing Proxy value before it's been set."
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input) as tracer:\n",
                 "\n",
-                "  output = model.output\n",
+                "    output = model.output\n",
                 "\n",
                 "print(output.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "sBz5qfwuR-6F"
             },
             "source": [
                 "Oh no an error! \"Accessing Proxy value before it's been set.\"\n",
                 "\n",
                 "Why doesn't our `output` have a `value`?\n",
                 "\n",
-                "Proxy objects will only have their value at the end of a context if we call `.save()` on them. This helps to reduce memory costs. Adding `.save()` fixes the error:"
+                "Proxy objects will only have their value at the end of a context if we call\n",
+                "`.save()` on them. This helps to reduce memory costs. Adding `.save()` fixes the\n",
+                "error:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -297,46 +335,52 @@
                         "tensor([[ 0.1473, -0.1518]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input) as tracer:\n",
                 "\n",
-                "  output = model.output.save()\n",
+                "    output = model.output.save()\n",
                 "\n",
                 "print(output.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "t5C0UZCwvrYn"
             },
             "source": [
-                "Success! We now have the model output. You just completed your first intervention using `nnsight`.\n",
+                "Success! We now have the model output. You just completed your first\n",
+                "intervention using `nnsight`.\n",
                 "\n",
-                "\n",
-                "Each time you access a module's input or output, you create an *intervention* in the neural network's forward pass. Collectively these requests form the *intervention graph*. We call the process of executing it alongside the model's normal computation graph, *interleaving*.\n",
+                "Each time you access a module's input or output, you create an _intervention_ in\n",
+                "the neural network's forward pass. Collectively these requests form the\n",
+                "_intervention graph_. We call the process of executing it alongside the model's\n",
+                "normal computation graph, _interleaving_.\n",
                 "\n",
                 "<details>\n",
                 "<summary>On Model output</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
-                "If you don't need to access anything other than the final model output, you can call the tracing context with `trace=False` and not use it as a context:\n",
+                "If you don't need to access anything other than the final model output, you can\n",
+                "call the tracing context with `trace=False` and not use it as a context:\n",
                 "\n",
                 "```python\n",
                 "output = model.trace(<inputs>, trace=False)\n",
                 "```\n",
                 "\n",
                 "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "Just like we saved the output of the model as a whole, we can save the output of any of its submodules. We use normal Python attribute syntax. We can discover how to access them by name by printing out the model:"
+                "Just like we saved the output of the model as a whole, we can save the output of\n",
+                "any of its submodules. We use normal Python attribute syntax. We can discover\n",
+                "how to access them by name by printing out the model:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -380,26 +424,28 @@
                         "          0.2968, -0.8834]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input) as tracer:\n",
                 "\n",
-                "  l1_output = model.layer1.output.save()\n",
+                "    l1_output = model.layer1.output.save()\n",
                 "\n",
                 "print(l1_output.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "85A-aP_03ht6"
             },
             "source": [
-                "Let's do the same for the input of layer2. While we're at it, let's also drop the `as tracer`, as we won't be needing the tracer object itself for a few sections:"
+                "Let's do the same for the input of layer2. While we're at it, let's also drop\n",
+                "the `as tracer`, as we won't be needing the tracer object itself for a few\n",
+                "sections:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -417,61 +463,64 @@
                         "          0.2968, -0.8834]]),), {})\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  l2_input = model.layer2.input.save()\n",
+                "    l2_input = model.layer2.input.save()\n",
                 "\n",
                 "print(l2_input.value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "jk-U8zi33Gi-"
             },
             "source": [
                 "<details>\n",
                 "  <summary>On module inputs</summary>\n",
                 "\n",
-                "  ---\n",
+                "---\n",
                 "\n",
-                "  Notice how the value for `l2_input`, was not just a single tensor.\n",
-                "  The type/shape of values from `.input` is in the form of:\n",
+                "Notice how the value for `l2_input`, was not just a single tensor. The\n",
+                "type/shape of values from `.input` is in the form of:\n",
                 "\n",
                 "      tuple(tuple(args), dictionary(kwargs))\n",
                 "\n",
-                "  Where the first index of the tuple is itself a tuple of all positional arguments, and the second index is a dictionary of the keyword arguments.\n",
+                "Where the first index of the tuple is itself a tuple of all positional\n",
+                "arguments, and the second index is a dictionary of the keyword arguments.\n",
                 "\n",
-                "  ---\n",
+                "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "\n",
-                "Now that we can access activations, we also want to do some post-processing on it. Let's find out which dimension of layer1's output has the highest value."
+                "Now that we can access activations, we also want to do some post-processing on\n",
+                "it. Let's find out which dimension of layer1's output has the highest value.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "p7Xo_PHyPr4p"
             },
             "source": [
-                "## Functions, Methods, and Operations"
+                "## Functions, Methods, and Operations\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "ehSofWbx5DSx"
             },
             "source": [
-                "We could do this by calling `torch.argmax(...)` after the tracing context or we can just leverage the fact that `nnsight` handles functions and methods within the tracing context, by creating a Proxy request for it:"
+                "We could do this by calling `torch.argmax(...)` after the tracing context or we\n",
+                "can just leverage the fact that `nnsight` handles functions and methods within\n",
+                "the tracing context, by creating a Proxy request for it:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -488,32 +537,38 @@
                         "tensor(5)\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Note we don't need to call .save() on the output,\n",
-                "  # as we're only using its value within the tracing context.\n",
-                "  l1_output = model.layer1.output\n",
+                "    # Note we don't need to call .save() on the output,\n",
+                "    # as we're only using its value within the tracing context.\n",
+                "    l1_output = model.layer1.output\n",
                 "\n",
-                "  l1_amax = torch.argmax(l1_output, dim=1).save()\n",
+                "    l1_amax = torch.argmax(l1_output, dim=1).save()\n",
                 "\n",
                 "print(l1_amax[0])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "BGPUJvWq_bOp"
             },
             "source": [
-                "Nice! That worked seamlessly, but hold on, how come we didn't need to call `.value[0]` on the result? In previous sections, we were just being explicit to get an understanding of Proxies and their value. In practice, however, `nnsight` knows that when outside of the tracing context we only care about the actual value, and so printing, indexing, and applying functions all immediately return and reflect the data in `.value`. So for the rest of the tutorial we won't use it.\n",
+                "Nice! That worked seamlessly, but hold on, how come we didn't need to call\n",
+                "`.value[0]` on the result? In previous sections, we were just being explicit to\n",
+                "get an understanding of Proxies and their value. In practice, however, `nnsight`\n",
+                "knows that when outside of the tracing context we only care about the actual\n",
+                "value, and so printing, indexing, and applying functions all immediately return\n",
+                "and reflect the data in `.value`. So for the rest of the tutorial we won't use\n",
+                "it.\n",
                 "\n",
-                "The same principles work for methods and operations as well:"
+                "The same principles work for methods and operations as well:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -530,48 +585,57 @@
                         "tensor(2.3416)\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  value = (model.layer1.output.sum() + model.layer2.output.sum()).save()\n",
+                "    value = (model.layer1.output.sum() + model.layer2.output.sum()).save()\n",
                 "\n",
                 "print(value)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "V0vNOJtJ2oFR"
             },
             "source": [
-                "By default, torch functiona, methods and all operators work with `nnsight`. We also enable the use of the `einops` library.\n",
+                "By default, torch functions, methods and all operators work with `nnsight`. We\n",
+                "also enable the use of the `einops` library.\n",
                 "\n",
-                "So to recap, the above code block is saying to `nnsight`, \"Run the model with the given `input`. When the output of layer1 is computed, take its sum. Then do the same for layer2. Now that both of those are computed, add them and make sure not to delete this value as I wish to use it outside of the tracing context.\"\n",
-                "\n",
-                "Getting and analyzing the activations from various points in a model can be really insightful, and a number of ML techniques do exactly that. However, often times we not only want to view the computation of a model, but influence it as well."
+                "So to recap, the above code block is saying to `nnsight`, \"Run the model with\n",
+                "the given `input`. When the output of layer1 is computed, take its sum. Then do\n",
+                "the same for layer2. Now that both of those are computed, add them and make sure\n",
+                "not to delete this value as I wish to use it outside of the tracing context.\"\n",
+                "\n",
+                "Getting and analyzing the activations from various points in a model can be\n",
+                "really insightful, and a number of ML techniques do exactly that. However, often\n",
+                "times we not only want to view the computation of a model, but influence it as\n",
+                "well.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "m_5qH5gHPOT_"
             },
             "source": [
-                "## Setting"
+                "## Setting\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "rgju-b_IOLlq"
             },
             "source": [
-                "To demonstrate the effect of editing the flow of information through the model, let's set the first dimension of the first layer's output to 0. `NNsight` makes this really easy using '=' operator:"
+                "To demonstrate the effect of editing the flow of information through the model,\n",
+                "let's set the first dimension of the first layer's output to 0. `NNsight` makes\n",
+                "this really easy using '=' operator:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -591,35 +655,35 @@
                         "          0.2968, -0.8834]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  # Access the 0th index of the hidden state dimension and set it to 0.\n",
-                "  model.layer1.output[:, 0] = 0\n",
+                "    # Access the 0th index of the hidden state dimension and set it to 0.\n",
+                "    model.layer1.output[:, 0] = 0\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "oZz9SMs3Y_iS"
             },
             "source": [
-                "Seems our change was reflected. Now the same for the last dimension:"
+                "Seems our change was reflected. Now the same for the last dimension:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -645,50 +709,67 @@
                         "\u001b[0;31mIndexError\u001b[0m: index 10 is out of bounds for dimension 1 with size 10"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  # Access the last index of the hidden state dimension and set it to 0.\n",
-                "  model.layer1.output[:, hidden_dims] = 0\n",
+                "    # Access the last index of the hidden state dimension and set it to 0.\n",
+                "    model.layer1.output[:, hidden_dims] = 0\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "JCNR_Jkpxr8l"
             },
             "source": [
-                "Ah of course, we needed to index at `hidden_dims - 1` not `hidden_dims`. How did `nnsight` know there was this indexing error before leaving the tracing context?\n",
+                "Ah of course, we needed to index at `hidden_dims - 1` not `hidden_dims`. How did\n",
+                "`nnsight` know there was this indexing error before leaving the tracing context?\n",
                 "\n",
-                "Earlier when discussing contexts in Python, we learned some logic happens upon entering, and some logic happens upon exiting. We know the model is actually run on exit, but what happens on enter? Our input IS actually run though the model, however under its own \"fake\" context. This means the input makes its way through all of the model operations, allowing `nnsight` to record the shapes and data types of module inputs and outputs! The operations are never executed using tensors with real values so it doesn't incur any memory costs. Then, when creating proxy requests like the setting one above, `nnsight` also attempts to execute the request on the \"fake\" values we recorded. Hence, it lets us know if our request is feasible before even running the model.\n",
+                "Earlier when discussing contexts in Python, we learned some logic happens upon\n",
+                "entering, and some logic happens upon exiting. We know the model is actually run\n",
+                "on exit, but what happens on enter? Our input IS actually run though the model,\n",
+                "however under its own \"fake\" context. This means the input makes its way through\n",
+                "all of the model operations, allowing `nnsight` to record the shapes and data\n",
+                "types of module inputs and outputs! The operations are never executed using\n",
+                "tensors with real values so it doesn't incur any memory costs. Then, when\n",
+                "creating proxy requests like the setting one above, `nnsight` also attempts to\n",
+                "execute the request on the \"fake\" values we recorded. Hence, it lets us know if\n",
+                "our request is feasible before even running the model.\n",
                 "\n",
                 "<details>\n",
                 "<summary>On scanning</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
-                "\"Scanning\" is what we call running \"fake\" inputs throught the model to collect information like shapes and types. \"Validating\" is what we call trying to execute your intervention proxies with \"fake\" inputs to see if they work. If you are doing anything in a loop where efficiency is important, you should turn off scanning and validating. You can turn off validating in `.trace(...)` like `.trace(..., validate=False)`. You can turn off scanning in `Tracer.invoke(...)` ([see the Batching section](#batching-id)) like `Tracer.invoke(..., scan=False)`\n",
+                "\"Scanning\" is what we call running \"fake\" inputs throught the model to collect\n",
+                "information like shapes and types. \"Validating\" is what we call trying to\n",
+                "execute your intervention proxies with \"fake\" inputs to see if they work. If you\n",
+                "are doing anything in a loop where efficiency is important, you should turn off\n",
+                "scanning and validating. You can turn off validating in `.trace(...)` like\n",
+                "`.trace(..., validate=False)`. You can turn off scanning in `Tracer.invoke(...)`\n",
+                "([see the Batching section](#batching-id)) like `Tracer.invoke(..., scan=False)`\n",
                 "\n",
                 "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "Let's try again with the correct indexing, and view the shape of the output before leaving the tracing context:"
+                "Let's try again with the correct indexing, and view the shape of the output\n",
+                "before leaving the tracing context:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -709,37 +790,39 @@
                         "          0.2968,  0.0000]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  print(f\"layer1 output shape: {model.layer1.output.shape}\")\n",
+                "    print(f\"layer1 output shape: {model.layer1.output.shape}\")\n",
                 "\n",
-                "  # Access the last index of the hidden state dimension and set it to 0.\n",
-                "  model.layer1.output[:, hidden_dims - 1] = 0\n",
+                "    # Access the last index of the hidden state dimension and set it to 0.\n",
+                "    model.layer1.output[:, hidden_dims - 1] = 0\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "9DH7PeL13-WU"
             },
             "source": [
-                "We can also just replace proxy inputs and outputs with tensors of the same shape and type. Let's use the shape information we have at our disposal to add noise to the output, and replace it with this new noised tensor:"
+                "We can also just replace proxy inputs and outputs with tensors of the same shape\n",
+                "and type. Let's use the shape information we have at our disposal to add noise\n",
+                "to the output, and replace it with this new noised tensor:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -759,40 +842,42 @@
                         "          0.3394, -0.9187]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # Save the output before the edit to compare.\n",
-                "  # Notice we apply .clone() before saving as the setting operation is in-place.\n",
-                "  l1_output_before = model.layer1.output.clone().save()\n",
+                "    # Save the output before the edit to compare.\n",
+                "    # Notice we apply .clone() before saving as the setting operation is in-place.\n",
+                "    l1_output_before = model.layer1.output.clone().save()\n",
                 "\n",
-                "  # Create random noise with variance of .001\n",
-                "  noise = (0.001**0.5)*torch.randn(l1_output_before.shape)\n",
+                "    # Create random noise with variance of .001\n",
+                "    noise = (0.001**0.5) * torch.randn(l1_output_before.shape)\n",
                 "\n",
-                "  # Add to original value and replace.\n",
-                "  model.layer1.output = l1_output_before + noise\n",
+                "    # Add to original value and replace.\n",
+                "    model.layer1.output = l1_output_before + noise\n",
                 "\n",
-                "  # Save the output after to see our edit.\n",
-                "  l1_output_after = model.layer1.output.save()\n",
+                "    # Save the output after to see our edit.\n",
+                "    l1_output_after = model.layer1.output.save()\n",
                 "\n",
                 "print(\"Before:\", l1_output_before)\n",
                 "print(\"After:\", l1_output_after)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "s016CelFP8sx"
             },
             "source": [
                 "## Gradients\n",
                 "\n",
-                "`NNsight` can also let you apply backprop and access gradients with respect to a loss. Like `.input` and `.output` on modules, `nnsight` also exposes `.grad` on Proxies themselves (assuming they are proxies of tensors):"
+                "`NNsight` can also let you apply backprop and access gradients with respect to a\n",
+                "loss. Like `.input` and `.output` on modules, `nnsight` also exposes `.grad` on\n",
+                "Proxies themselves (assuming they are proxies of tensors):\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -811,38 +896,40 @@
                         "Layer 2 output gradient: tensor([[1., 1.]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # We need to explicitly have the tensor require grad\n",
-                "  # as the model we defined earlier turned off requiring grad.\n",
-                "  model.layer1.output.requires_grad = True\n",
-                "\n",
-                "  # We call .grad on a tensor Proxy to communicate we want to store its gradient.\n",
-                "  # We need to call .save() of course as .grad is its own Proxy.\n",
-                "  layer1_output_grad = model.layer1.output.grad.save()\n",
-                "  layer2_output_grad = model.layer2.output.grad.save()\n",
-                "\n",
-                "  # Need a loss to propagate through the later modules in order to have a grad.\n",
-                "  loss = model.output.sum()\n",
-                "  loss.backward()\n",
+                "    # We need to explicitly have the tensor require grad\n",
+                "    # as the model we defined earlier turned off requiring grad.\n",
+                "    model.layer1.output.requires_grad = True\n",
+                "\n",
+                "    # We call .grad on a tensor Proxy to communicate we want to store its gradient.\n",
+                "    # We need to call .save() of course as .grad is its own Proxy.\n",
+                "    layer1_output_grad = model.layer1.output.grad.save()\n",
+                "    layer2_output_grad = model.layer2.output.grad.save()\n",
+                "\n",
+                "    # Need a loss to propagate through the later modules in order to have a grad.\n",
+                "    loss = model.output.sum()\n",
+                "    loss.backward()\n",
                 "\n",
                 "print(\"Layer 1 output gradient:\", layer1_output_grad)\n",
-                "print(\"Layer 2 output gradient:\", layer2_output_grad)\n"
+                "print(\"Layer 2 output gradient:\", layer2_output_grad)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "1o0JaaYvWlHG"
             },
             "source": [
-                "All of the features we learned previously, also apply to `.grad`. In other words, we can apply operations to and edit the gradients. Let's zero the grad of `layer1` and double the grad of `layer2`."
+                "All of the features we learned previously, also apply to `.grad`. In other\n",
+                "words, we can apply operations to and edit the gradients. Let's zero the grad of\n",
+                "`layer1` and double the grad of `layer2`.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -860,70 +947,77 @@
                         "Layer 2 output gradient: tensor([[2., 2.]])\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace(input):\n",
                 "\n",
-                "  # We need to explicitly have the tensor require grad\n",
-                "  # as the model we defined earlier turned off requiring grad.\n",
-                "  model.layer1.output.requires_grad = True\n",
-                "\n",
-                "  model.layer1.output.grad[:] = 0\n",
-                "  model.layer2.output.grad = model.layer2.output.grad.clone() * 2\n",
-                "\n",
-                "  layer1_output_grad = model.layer1.output.grad.save()\n",
-                "  layer2_output_grad = model.layer2.output.grad.save()\n",
-                "\n",
-                "  # Need a loss to propagate through the later modules in order to have a grad.\n",
-                "  loss = model.output.sum()\n",
-                "  loss.backward()\n",
+                "    # We need to explicitly have the tensor require grad\n",
+                "    # as the model we defined earlier turned off requiring grad.\n",
+                "    model.layer1.output.requires_grad = True\n",
+                "\n",
+                "    model.layer1.output.grad[:] = 0\n",
+                "    model.layer2.output.grad = model.layer2.output.grad.clone() * 2\n",
+                "\n",
+                "    layer1_output_grad = model.layer1.output.grad.save()\n",
+                "    layer2_output_grad = model.layer2.output.grad.save()\n",
+                "\n",
+                "    # Need a loss to propagate through the later modules in order to have a grad.\n",
+                "    loss = model.output.sum()\n",
+                "    loss.backward()\n",
                 "\n",
                 "print(\"Layer 1 output gradient:\", layer1_output_grad)\n",
                 "print(\"Layer 2 output gradient:\", layer2_output_grad)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "gvQ1nZgYQDG3"
             },
             "source": [
-                "# 2 Bigger"
+                "# 2 Bigger\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "miQgUY4NAmDQ"
             },
             "source": [
-                "Now that we have the basics of `nnsight` under our belt, we can scale our model up and combine the techniques we've learned into more interesting experiments.\n",
+                "Now that we have the basics of `nnsight` under our belt, we can scale our model\n",
+                "up and combine the techniques we've learned into more interesting experiments.\n",
                 "\n",
-                "The `NNsight` class is very bare bones. It wraps a pre-defined model and does no pre-processing on the inputs we enter. It's designed to be extended with more complex and powerful types of models and we're excited to see what can be done to leverage its features."
+                "The `NNsight` class is very bare bones. It wraps a pre-defined model and does no\n",
+                "pre-processing on the inputs we enter. It's designed to be extended with more\n",
+                "complex and powerful types of models and we're excited to see what can be done\n",
+                "to leverage its features.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "5TJDblHiQpp1"
             },
             "source": [
-                "## LanguageModel"
+                "## LanguageModel\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "9l9mZOY5HFH2"
             },
             "source": [
-                "`LanguageModel` is a subclass of `NNsight`.  While we could define and create a model to pass in directly, `LanguageModel` includes special support for Huggingface language models, including automatically loading models from a Huggingface ID, and loading the model together with the appropriate tokenizer.\n",
+                "`LanguageModel` is a subclass of `NNsight`. While we could define and create a\n",
+                "model to pass in directly, `LanguageModel` includes special support for\n",
+                "Huggingface language models, including automatically loading models from a\n",
+                "Huggingface ID, and loading the model together with the appropriate tokenizer.\n",
                 "\n",
-                "Here is how you can use `LanguageModel` to load `GPT-2`:"
+                "Here is how you can use `LanguageModel` to load `GPT-2`:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1082,15 +1176,15 @@
                         ")\n"
                     ]
                 }
             ],
             "source": [
                 "from nnsight import LanguageModel\n",
                 "\n",
-                "model = LanguageModel('openai-community/gpt2', device_map=\"auto\")\n",
+                "model = LanguageModel(\"openai-community/gpt2\", device_map=\"auto\")\n",
                 "\n",
                 "print(model)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -1100,27 +1194,41 @@
                 "<details>\n",
                 "<summary>On Model Initialization</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
                 "A few important things to note:\n",
                 "\n",
-                "  Keyword arguments passed to the initialization of `LanguageModel` is forwarded to HuggingFace specific loading logic. In this case, `device_map` specifies which devices to use and its value `auto` indicates to evenly distribute it to all available GPUs (and cpu if no GPUs available). Other arguments can be found here: https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModelForCausalLM\n",
-                "\n",
-                "\n",
-                "  When we initialize `LanguageModel`, we aren't yet loading the parameters of the model into memory. We are actually loading a 'meta' version of the model which doesn't take up any memory, but still allows us to view and trace actions on it. After exiting the first tracing context, the model is then fully loaded into memory. To load into memory on initialization, you can pass `dispatch=True` into `LanguageModel` like `LanguageModel('openai-community/gpt2', device_map=\"auto\", dispatch=True)`.\n",
+                "Keyword arguments passed to the initialization of `LanguageModel` is forwarded\n",
+                "to HuggingFace specific loading logic. In this case, `device_map` specifies\n",
+                "which devices to use and its value `auto` indicates to evenly distribute it to\n",
+                "all available GPUs (and cpu if no GPUs available). Other arguments can be found\n",
+                "here:\n",
+                "https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModelForCausalLM\n",
+                "\n",
+                "When we initialize `LanguageModel`, we aren't yet loading the parameters of the\n",
+                "model into memory. We are actually loading a 'meta' version of the model which\n",
+                "doesn't take up any memory, but still allows us to view and trace actions on it.\n",
+                "After exiting the first tracing context, the model is then fully loaded into\n",
+                "memory. To load into memory on initialization, you can pass `dispatch=True` into\n",
+                "`LanguageModel` like\n",
+                "`LanguageModel('openai-community/gpt2', device_map=\"auto\", dispatch=True)`.\n",
                 "\n",
                 "---\n",
                 "\n",
                 "</details>\n",
                 "\n",
-                "\n",
-                "Let's put together some of the features we applied to the small model, but now on `GPT-2`. Unlike `NNsight`, `LanguageModel` does define logic to pre-process inputs upon entering the tracing context. This makes interacting with the model simpler without having to directly access the tokenizer.\n",
-                "\n",
-                "In the following example, we ablate the value coming from the last layer's MLP module and decode the logits to see what token the model predicts without influence from that particular module:"
+                "Let's put together some of the features we applied to the small model, but now\n",
+                "on `GPT-2`. Unlike `NNsight`, `LanguageModel` does define logic to pre-process\n",
+                "inputs upon entering the tracing context. This makes interacting with the model\n",
+                "simpler without having to directly access the tokenizer.\n",
+                "\n",
+                "In the following example, we ablate the value coming from the last layer's MLP\n",
+                "module and decode the logits to see what token the model predicts without\n",
+                "influence from that particular module:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1143,74 +1251,102 @@
                     "text": [
                         "Token IDs: tensor([[ 262,   12,  417, 8765,   11,  257,  262, 3504,  338, 3576]])\n",
                         "Prediction:  London\n"
                     ]
                 }
             ],
             "source": [
-                "with model.trace('The Eiffel Tower is in the city of'):\n",
+                "with model.trace(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "  # Access the last layer using h[-1] as it's a ModuleList\n",
-                "  # Access the first index of .output as that's where the hidden states are.\n",
-                "  model.transformer.h[-1].mlp.output[0][:] = 0\n",
+                "    # Access the last layer using h[-1] as it's a ModuleList\n",
+                "    # Access the first index of .output as that's where the hidden states are.\n",
+                "    model.transformer.h[-1].mlp.output[0][:] = 0\n",
                 "\n",
-                "  # Logits come out of model.lm_head and we apply argmax to get the predicted token ids.\n",
-                "  token_ids = model.lm_head.output.argmax(dim=-1).save()\n",
+                "    # Logits come out of model.lm_head and we apply argmax to get the predicted token ids.\n",
+                "    token_ids = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
                 "print(\"Token IDs:\", token_ids)\n",
                 "\n",
                 "# Apply the tokenizer to decode the ids into words after the tracing context.\n",
-                "print(\"Prediction:\", model.tokenizer.decode(token_ids[0][-1]))\n"
+                "print(\"Prediction:\", model.tokenizer.decode(token_ids[0][-1]))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "X2-HiCQhkv-B"
             },
             "source": [
-                "You just ran a little intervention on a much more complex model with a lot more parameters! An important piece of information we're missing though is what the prediction would look like without our ablation.\n",
-                "\n",
-                "Of course we could just run two tracing contexts and compare the outputs. This, however, would require two forward passes through the model. `NNsight` can do better than that."
+                "You just ran a little intervention on a much more complex model with a lot more\n",
+                "parameters! An important piece of information we're missing though is what the\n",
+                "prediction would look like without our ablation.\n",
+                "\n",
+                "Of course we could just run two tracing contexts and compare the outputs. This,\n",
+                "however, would require two forward passes through the model. `NNsight` can do\n",
+                "better than that.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "vLjHnRyRPXjp"
             },
             "source": [
                 "<a name=\"batching-id\"></a>\n",
-                "## Batching"
+                "\n",
+                "## Batching\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "_Gc-Zr6NmEOn"
             },
             "source": [
-                "It's time to bring back the `Tracer` object we dropped before. See, when you call `.trace(...)` with some input, it's actually creating two different contexts behind the scenes. The second one is the invoker context. Being within this context just means that `.input` and `.output` should refer only to the input you've given invoke. Calling `.trace(...)` with some input just means there's only one input and therefore only one invoker context.\n",
-                "\n",
-                "We can call `.trace()` without input and call `Tracer.invoke(...)` to manually create the invoker context with our input. Now every subsequent time we call `.invoke(...)`, new interventions will only refer to the input in that particular invoke. When exiting the tracing context, the inputs from all of the invokers will be batched together, and they will be executed in one forward pass! So let's do the ablation experiment, and compute a 'control' output to compare to:\n",
+                "It's time to bring back the `Tracer` object we dropped before. See, when you\n",
+                "call `.trace(...)` with some input, it's actually creating two different\n",
+                "contexts behind the scenes. The second one is the invoker context. Being within\n",
+                "this context just means that `.input` and `.output` should refer only to the\n",
+                "input you've given invoke. Calling `.trace(...)` with some input just means\n",
+                "there's only one input and therefore only one invoker context.\n",
+                "\n",
+                "We can call `.trace()` without input and call `Tracer.invoke(...)` to manually\n",
+                "create the invoker context with our input. Now every subsequent time we call\n",
+                "`.invoke(...)`, new interventions will only refer to the input in that\n",
+                "particular invoke. When exiting the tracing context, the inputs from all of the\n",
+                "invokers will be batched together, and they will be executed in one forward\n",
+                "pass! So let's do the ablation experiment, and compute a 'control' output to\n",
+                "compare to:\n",
                 "\n",
                 "<details>\n",
                 "<summary>On the invoker context</summary>\n",
                 "\n",
                 "---\n",
                 "\n",
-                "Note that when injecting data to only the relevant invoker interventions, `nnsight` tries, but can't guarantee, that it can narrow the data into the right batch idxs (in the case of an object as input or output). So there are cases where all invokes will get all of the data.\n",
-                "\n",
-                "Just like `.trace(...)` created a `Tracer` object, `.invoke(...)` creates an `Invoker` object. The `Invoker` object has post-processed inputs at `invoker.inputs`, which can be useful for seeing information about your input. If you are using `.trace(...)` with inputs, you can still access the invoker object at `tracer._invoker`.\n",
-                "\n",
-                "Keyword arguments given to `.invoke(..)` make its way to the input pre-processing. For example in `LanguageModel`, the keyword arguments are used to tokenize like `max_length` and `truncation`. If you need to pass in keyword arguments directly to one input `.trace(...)`, you can pass an `invoker_args` keyword argument that should be a dictionary of keyword arguments for the invoker. `.trace(..., invoker_args={...})`\n",
+                "Note that when injecting data to only the relevant invoker interventions,\n",
+                "`nnsight` tries, but can't guarantee, that it can narrow the data into the right\n",
+                "batch idxs (in the case of an object as input or output). So there are cases\n",
+                "where all invokes will get all of the data.\n",
+                "\n",
+                "Just like `.trace(...)` created a `Tracer` object, `.invoke(...)` creates an\n",
+                "`Invoker` object. The `Invoker` object has post-processed inputs at\n",
+                "`invoker.inputs`, which can be useful for seeing information about your input.\n",
+                "If you are using `.trace(...)` with inputs, you can still access the invoker\n",
+                "object at `tracer._invoker`.\n",
+                "\n",
+                "Keyword arguments given to `.invoke(..)` make its way to the input\n",
+                "pre-processing. For example in `LanguageModel`, the keyword arguments are used\n",
+                "to tokenize like `max_length` and `truncation`. If you need to pass in keyword\n",
+                "arguments directly to one input `.trace(...)`, you can pass an `invoker_args`\n",
+                "keyword argument that should be a dictionary of keyword arguments for the\n",
+                "invoker. `.trace(..., invoker_args={...})`\n",
                 "\n",
                 "---\n",
                 "\n",
-                "</details>"
+                "</details>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1230,26 +1366,26 @@
                         "Intervention prediction:  London\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace() as tracer:\n",
                 "\n",
-                "  with tracer.invoke('The Eiffel Tower is in the city of'):\n",
+                "    with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "    # Ablate the last MLP for only this batch.\n",
-                "    model.transformer.h[-1].mlp.output[0][:] = 0\n",
+                "        # Ablate the last MLP for only this batch.\n",
+                "        model.transformer.h[-1].mlp.output[0][:] = 0\n",
                 "\n",
-                "    # Get the output for only the intervened on batch.\n",
-                "    token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        # Get the output for only the intervened on batch.\n",
+                "        token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
-                "  with tracer.invoke('The Eiffel Tower is in the city of'):\n",
+                "    with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "    # Get the output for only the original batch.\n",
-                "    token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        # Get the output for only the original batch.\n",
+                "        token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
                 "print(\"Original token IDs:\", token_ids_original)\n",
                 "print(\"Intervention token IDs:\", token_ids_intervention)\n",
                 "\n",
                 "print(\"Original prediction:\", model.tokenizer.decode(token_ids_original[0][-1]))\n",
                 "print(\"Intervention prediction:\", model.tokenizer.decode(token_ids_intervention[0][-1]))"
             ]
@@ -1258,15 +1394,18 @@
             "cell_type": "markdown",
             "metadata": {
                 "id": "8BsybgsK2Bbr"
             },
             "source": [
                 "So it did end up affecting what the model predicted. That's pretty neat!\n",
                 "\n",
-                "Another cool thing with multiple invokes is that the Proxies can interact between them. Here we transfer the word token embeddings from a real prompt into another placeholder prompt. Therefore the latter prompt produces the output of the former prompt:"
+                "Another cool thing with multiple invokes is that the Proxies can interact\n",
+                "between them. Here we transfer the word token embeddings from a real prompt into\n",
+                "another placeholder prompt. Therefore the latter prompt produces the output of\n",
+                "the former prompt:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1284,45 +1423,54 @@
                         "Intervention prediction:  Paris\n"
                     ]
                 }
             ],
             "source": [
                 "with model.trace() as tracer:\n",
                 "\n",
-                "  with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
+                "    with tracer.invoke(\"The Eiffel Tower is in the city of\"):\n",
                 "\n",
-                "    embeddings = model.transformer.wte.output\n",
+                "        embeddings = model.transformer.wte.output\n",
                 "\n",
-                "  with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
+                "    with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
                 "\n",
-                "    model.transformer.wte.output = embeddings\n",
+                "        model.transformer.wte.output = embeddings\n",
                 "\n",
-                "    token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        token_ids_intervention = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
-                "  with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
+                "    with tracer.invoke(\"_ _ _ _ _ _ _ _ _ _\"):\n",
                 "\n",
-                "    token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
+                "        token_ids_original = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
                 "print(\"Original prediction:\", model.tokenizer.decode(token_ids_original[0][-1]))\n",
                 "print(\"Intervention prediction:\", model.tokenizer.decode(token_ids_intervention[0][-1]))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "vvWA-CWqQtah"
             },
             "source": [
                 "## .next()\n",
                 "\n",
-                "Some HuggingFace models define methods to generate multiple outputs at a time. `LanguageModel` wraps that functionality to provide the same tracing features by using `.generate(...)` instead of `.trace(...)`. This calls the underlying model's `.generate` method. It passes the output through a `model.generator` module that we've added onto the model, allowing you to get the generate output at `model.generator.output`.\n",
-                "\n",
-                "In a case like this, the underlying model is called more than once; the modules of said model produce more than one output. Which iteration should a given `module.output` refer to? That's where `Module.next()` comes in.\n",
-                "\n",
-                "Each module has a call idx associated with it and `.next()` simply increments that attribute. At the time of execution, data is injected into the intervention graph only at the iteration that matches the call idx."
+                "Some HuggingFace models define methods to generate multiple outputs at a time.\n",
+                "`LanguageModel` wraps that functionality to provide the same tracing features by\n",
+                "using `.generate(...)` instead of `.trace(...)`. This calls the underlying\n",
+                "model's `.generate` method. It passes the output through a `model.generator`\n",
+                "module that we've added onto the model, allowing you to get the generate output\n",
+                "at `model.generator.output`.\n",
+                "\n",
+                "In a case like this, the underlying model is called more than once; the modules\n",
+                "of said model produce more than one output. Which iteration should a given\n",
+                "`module.output` refer to? That's where `Module.next()` comes in.\n",
+                "\n",
+                "Each module has a call idx associated with it and `.next()` simply increments\n",
+                "that attribute. At the time of execution, data is injected into the intervention\n",
+                "graph only at the iteration that matches the call idx.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -1353,21 +1501,21 @@
                         "All prediction:  ['The Eiffel Tower is in the city of Paris, and']\n"
                     ]
                 }
             ],
             "source": [
                 "with model.generate(\"The Eiffel Tower is in the city of\", max_new_tokens=3):\n",
                 "\n",
-                "  token_ids_1 = model.lm_head.output.argmax(dim=-1).save()\n",
+                "    token_ids_1 = model.lm_head.output.argmax(dim=-1).save()\n",
                 "\n",
-                "  token_ids_2 = model.lm_head.next().output.argmax(dim=-1).save()\n",
+                "    token_ids_2 = model.lm_head.next().output.argmax(dim=-1).save()\n",
                 "\n",
-                "  token_ids_3 = model.lm_head.next().output.argmax(dim=-1).save()\n",
+                "    token_ids_3 = model.lm_head.next().output.argmax(dim=-1).save()\n",
                 "\n",
-                "  output = model.generator.output.save()\n",
+                "    output = model.generator.output.save()\n",
                 "\n",
                 "print(\"Prediction 1: \", model.tokenizer.decode(token_ids_1[0][-1]))\n",
                 "print(\"Prediction 2: \", model.tokenizer.decode(token_ids_2[0][-1]))\n",
                 "print(\"Prediction 3: \", model.tokenizer.decode(token_ids_3[0][-1]))\n",
                 "\n",
                 "print(\"All token ids: \", output)\n",
                 "\n",
@@ -1376,48 +1524,58 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "rpkX-LwBQZHo"
             },
             "source": [
-                "# 3 I thought you said huge models?"
+                "# 3 I thought you said huge models?\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "uCZR65VmILEb"
             },
             "source": [
-                "`NNsight` is only one part of our project to democratize access to AI internals. The other half is `NDIF` (National Deep Inference Facility).\n",
+                "`NNsight` is only one part of our project to democratize access to AI internals.\n",
+                "The other half is `NDIF` (National Deep Inference Facility).\n",
                 "\n",
-                "The interaction between the two is fairly straightforward. The `intervention graph` we create via the tracing context can be encoded into a custom json format and sent via an http request to the `NDIF` servers. `NDIF` then decodes the `intervention graph` and `interleaves` it alongside the specified model.\n",
+                "The interaction between the two is fairly straightforward. The\n",
+                "`intervention graph` we create via the tracing context can be encoded into a\n",
+                "custom json format and sent via an http request to the `NDIF` servers. `NDIF`\n",
+                "then decodes the `intervention graph` and `interleaves` it alongside the\n",
+                "specified model.\n",
                 "\n",
-                "To see which models are currently being hosted, check out the following status page: https://nnsight.net/status/"
+                "To see which models are currently being hosted, check out the following status\n",
+                "page: https://nnsight.net/status/\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "65Ks1LUvQaER"
             },
             "source": [
-                "## Remote execution"
+                "## Remote execution\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "Aa-ZuVOFKS5k"
             },
             "source": [
-                "In its current state, `NDIF` requires you to recieve an API key. Therefore, to run the rest of this colab, you would need one of your own. To get one, simply join the [NDIF discord](https://discord.gg/6uFJmCSwW7) and introduce yourself on the `#introductions` channel. Then DM either @JadenFK or @caden and we'll create one for you.\n",
+                "In its current state, `NDIF` requires you to receive an API key. Therefore, to\n",
+                "run the rest of this colab, you would need one of your own. To get one, simply\n",
+                "join the [NDIF discord](https://discord.gg/6uFJmCSwW7) and introduce yourself on\n",
+                "the `#introductions` channel. Then DM either @JadenFK or @caden and we'll create\n",
+                "one for you.\n",
                 "\n",
-                "Once you have one, to register your api key with `nnsight`, do the following:"
+                "Once you have one, to register your api key with `nnsight`, do the following:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "ax1NWoS9MJeZ"
@@ -1431,17 +1589,19 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "mvXLOh65MXmF"
             },
             "source": [
-                "This only needs to be run once as it will save this api key as the default in a config file along with the `nnsight` installation.\n",
+                "This only needs to be run once as it will save this api key as the default in a\n",
+                "config file along with the `nnsight` installation.\n",
                 "\n",
-                "To amp things up a few levels, let's demonstrate using `nnsight`'s tracing context with one of the larger open source language models, `Llama-2-70b`!"
+                "To amp things up a few levels, let's demonstrate using `nnsight`'s tracing\n",
+                "context with one of the larger open source language models, `Llama-2-70b`!\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "Q1N04sJPZnJt"
@@ -1468,61 +1628,66 @@
             },
             "outputs": [],
             "source": [
                 "# We'll never actually load the parameters so no need to specify a device_map.\n",
                 "model = LanguageModel(\"meta-llama/Llama-2-70b-hf\")\n",
                 "\n",
                 "# All we need to specify using NDIF vs executing locally is remote=True.\n",
-                "with model.trace('The Eiffel Tower is in the city of', remote=True) as runner:\n",
+                "with model.trace(\"The Eiffel Tower is in the city of\", remote=True) as runner:\n",
                 "\n",
                 "    hidden_states = model.model.layers[-1].output.save()\n",
                 "\n",
                 "    output = model.output.save()\n",
                 "\n",
                 "print(hidden_states)\n",
                 "\n",
-                "print(output['logits'])"
+                "print(output[\"logits\"])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "IceVpnZcZ9F0"
             },
             "source": [
-                "It really is as simple as `remote=True`. All of the techniques we went through in earlier sections work just the same when running locally and remotely.\n",
+                "It really is as simple as `remote=True`. All of the techniques we went through\n",
+                "in earlier sections work just the same when running locally and remotely.\n",
                 "\n",
-                "Note that both `nnsight`, but especially `NDIF`, is in active development and therefore there may be caveats, changes, and errors to work through."
+                "Note that both `nnsight`, but especially `NDIF`, is in active development and\n",
+                "therefore there may be caveats, changes, and errors to work through.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "P3zRm-7VRRov"
             },
             "source": [
-                "# Getting Involved!"
+                "# Getting Involved!\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "BnCc9xgjvxEP"
             },
             "source": [
-                "If you're interested in following updates to `nnsight`, contributing, giving feedback, or finding collaborators, please join the [NDIF discord](https://discord.gg/6uFJmCSwW7)!\n",
-                "\n",
-                "The [Mech Interp discord](https://discord.gg/km2RQBzaUn) is also a fantastic place to discuss all things mech interp with a really cool community.\n",
-                "\n",
-                "Our website [nnsight.net](https://nnsight.net/), has a bunch more tutorials detailing more complex interpretability techniques using `nnsight`. If you want to share any of the work you do using `nnsight`, let others know on either of the discords above and we might turn it into a tutorial on our website.\n",
-                "\n",
-                "\ud83d\udc9f\n",
-                "\n",
+                "If you're interested in following updates to `nnsight`, contributing, giving\n",
+                "feedback, or finding collaborators, please join the\n",
+                "[NDIF discord](https://discord.gg/6uFJmCSwW7)!\n",
+                "\n",
+                "The [Mech Interp discord](https://discord.gg/km2RQBzaUn) is also a fantastic\n",
+                "place to discuss all things mech interp with a really cool community.\n",
+                "\n",
+                "Our website [nnsight.net](https://nnsight.net/), has a bunch more tutorials\n",
+                "detailing more complex interpretability techniques using `nnsight`. If you want\n",
+                "to share any of the work you do using `nnsight`, let others know on either of\n",
+                "the discords above and we might turn it into a tutorial on our website.\n",
                 "\n",
-                "\n"
+                "\ud83d\udc9f\n"
             ]
         }
     ],
     "metadata": {
         "colab": {
             "provenance": [],
             "toc_visible": true
```

### Comparing `nnsight-0.2.8/docs/source/start.rst` & `nnsight-0.2.9/docs/source/start.rst`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/status.rst` & `nnsight-0.2.9/docs/source/status.rst`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/source/tutorials.rst` & `nnsight-0.2.9/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/docs/sourcelatex/conf.py` & `nnsight-0.2.9/docs/sourcelatex/conf.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/adhoc_module.py` & `nnsight-0.2.9/examples/adhoc_module.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/custommodel.py` & `nnsight-0.2.9/examples/custommodel.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/embeddings.py` & `nnsight-0.2.9/examples/embeddings.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/lora.py` & `nnsight-0.2.9/examples/lora.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/main_demo.ipynb` & `nnsight-0.2.9/examples/main_demo.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/multitoken.py` & `nnsight-0.2.9/examples/multitoken.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/optim.py` & `nnsight-0.2.9/examples/optim.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/optim2.py` & `nnsight-0.2.9/examples/optim2.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/retain_grad.py` & `nnsight-0.2.9/examples/retain_grad.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/test.py` & `nnsight-0.2.9/examples/test.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/tl/.ipynb_checkpoints/attention-checkpoint.ipynb` & `nnsight-0.2.9/examples/tl/.ipynb_checkpoints/attention-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/tl/Main_Demo.ipynb` & `nnsight-0.2.9/examples/tl/Main_Demo.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/tl/attention.ipynb` & `nnsight-0.2.9/examples/tl/attention.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/tl/attention.py` & `nnsight-0.2.9/examples/tl/attention.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/tl/attribution_patching.ipynb` & `nnsight-0.2.9/examples/tl/attribution_patching.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/examples/tl/patching.py` & `nnsight-0.2.9/examples/tl/patching.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/pyproject.toml` & `nnsight-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/contexts/Invoker.py` & `nnsight-0.2.9/src/nnsight/contexts/Invoker.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 class Invoker(AbstractContextManager):
     """An Invoker is meant to work in tandem with a :class:`nnsight.contexts.Tracer.Tracer` to enter input and manage intervention tracing.
 
     Attributes:
         tracer (nnsight.contexts.Tracer.Tracer): Tracer object to enter input and manage context.
-        inputs (Tuple[Any]): Initially entered inputs, then post-processed inputs from model's ._prepare_inputs(...) method.
+        inputs (tuple[Any]): Initially entered inputs, then post-processed inputs from model's ._prepare_inputs(...) method.
         scan (bool): If to execute the model using `FakeTensor` in order to update the potential sizes/dtypes of all modules' Envoys' inputs/outputs as well as validate things work correctly.
             Scanning is not free computation wise so you may want to turn this to false when running in a loop.
             When making interventions, you made get shape errors if scan is false as it validates operations based on shapes so
             for looped calls where shapes are consistent, you may want to have scan=True for the first loop. Defaults to True.
         kwargs (Dict[str,Any]): Keyword arguments passed to the model's _prepare_inputs method.
     """
 
     def __init__(
         self,
         tracer: "Tracer",
-        *inputs: Tuple[Any],
+        *inputs: Any,
         scan: bool = True,
         **kwargs,
     ) -> None:
 
         self.tracer = tracer
         self.inputs = inputs
         self.scan = scan
@@ -48,17 +48,15 @@
 
         Returns:
             Invoker: Invoker.
         """
 
         self.tracer._invoker = self
 
-        self.inputs, batch_size = self.tracer._model._prepare_inputs(
-            *self.inputs, **self.kwargs
-        )
+        self.inputs, batch_size = self.tracer._model._prepare_inputs(*self.inputs, **self.kwargs)
 
         if self.scan:
             self.tracer._model._envoy._clear()
 
             with FakeTensorMode(
                 allow_non_fake_inputs=True,
                 shape_env=ShapeEnv(assume_static_by_default=True),
```

### Comparing `nnsight-0.2.8/src/nnsight/contexts/Runner.py` & `nnsight-0.2.9/src/nnsight/contexts/Runner.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/contexts/Tracer.py` & `nnsight-0.2.9/src/nnsight/contexts/Tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import weakref
-from typing import TYPE_CHECKING, Any, Callable, List, Tuple
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple
 
 from ..intervention import InterventionProxy
 from ..tracing.Graph import Graph
 from .Invoker import Invoker
 
 if TYPE_CHECKING:
     from ..models.NNsightModel import NNsight
@@ -35,15 +35,15 @@
 
         self._kwargs = kwargs
 
         self._graph: Graph = Graph(
             self._model._envoy, proxy_class=model.proxy_class, validate=validate
         )
 
-        self._invoker: Invoker = None
+        self._invoker: Optional[Invoker] = None
 
         self._batch_size: int = 0
         self._batch_start: int = 0
 
         self._batched_input: Any = None
 
         # Module Envoys need to know about the current Tracer to create the correct proxies.
@@ -70,15 +70,15 @@
             *self._batched_input,
             **self._kwargs,
         )
 
         self._graph.tracing = False
         self._graph = None
 
-    def invoke(self, *inputs: Tuple[Any], **kwargs) -> Invoker:
+    def invoke(self, *inputs: Any, **kwargs) -> Invoker:
         """Create an Invoker context dor a given input.
 
         Raises:
             Exception: If an Invoker context is already open
 
         Returns:
             Invoker: Invoker.
```

### Comparing `nnsight-0.2.8/src/nnsight/contexts/__init__.py` & `nnsight-0.2.9/src/nnsight/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/envoy.py` & `nnsight-0.2.9/src/nnsight/envoy.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,37 +43,29 @@
         self._sub_envoys: List[Envoy] = []
 
         # Register hook on underlying module to update the _fake_outputs and _fake_inputs on forward pass.
         self._hook_handle = self._module.register_forward_hook(
             self._hook, with_kwargs=True
         )
 
-        if isinstance(module, torch.nn.ModuleList):
-            for i, module in enumerate(self._module):
+        for name, module in self._module.named_children():
 
-                envoy = Envoy(module, module_path=f"{self._module_path}.{i}")
+            envoy = Envoy(module, module_path=f"{self._module_path}.{name}")
 
-                self._sub_envoys.append(envoy)
+            self._sub_envoys.append(envoy)
 
-        else:
-            for name, module in self._module.named_children():
-
-                envoy = Envoy(module, module_path=f"{self._module_path}.{name}")
-
-                self._sub_envoys.append(envoy)
+            # If the module already has a sub-module named 'input' or 'output',
+            # mount the proxy access to 'nns_input' or 'nns_output instead.
+            if hasattr(Envoy, name):
 
-                # If the module already has a sub-module named 'input' or 'output',
-                # mount the proxy access to 'nns_input' or 'nns_output instead.
-                if hasattr(Envoy, name):
+                self._handle_overloaded_mount(envoy, name)
 
-                    self._handle_overloaded_mount(envoy, name)
-
-                else:
+            else:
 
-                    setattr(self, name, envoy)
+                setattr(self, name, envoy)
 
     def _handle_overloaded_mount(self, envoy: Envoy, mount_point: str):
 
         warnings.warn(
             f"Module of type `{type(self._module)}` has pre-defined a `{mount_point}` attribute. nnsight access for `{mount_point}` will be mounted at `.nns_{mount_point}` instead of `.{mount_point}` for this module only."
         )
 
@@ -232,14 +224,17 @@
         extra_repr = self._module.extra_repr()
         # empty string will be split into list ['']
         if extra_repr:
             extra_lines = extra_repr.split("\n")
         child_lines = []
         for attribute_name, attribute in self.__dict__.items():
 
+            if attribute_name == "_tracer":
+                continue
+
             if isinstance(attribute, Envoy):
 
                 mod_str = repr(attribute)
                 mod_str = torch.nn.modules.module._addindent(mod_str, 2)
                 child_lines.append("(" + attribute_name + "): " + mod_str)
 
         lines = extra_lines + child_lines
@@ -303,15 +298,23 @@
 
         Returns:
             InterventionProxy: Module call proxy.
         """
 
         module_proxy = getattr(self._tracer._graph.module_proxy, self._module_path)
 
-        torch.set_default_device(next(self._module.parameters()).device)
+        try:
+
+            device = next(self._module.parameters()).device
+
+        except:
+
+            device = torch.device("cpu")
+
+        torch.set_default_device(device)
 
         proxy = module_proxy.forward(*args, **kwargs)
 
         torch._GLOBAL_DEVICE_CONTEXT.__exit__(None, None, None)
 
         torch._GLOBAL_DEVICE_CONTEXT = None
```

### Comparing `nnsight-0.2.8/src/nnsight/intervention.py` & `nnsight-0.2.9/src/nnsight/intervention.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/logger.py` & `nnsight-0.2.9/src/nnsight/logger.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/models/LanguageModel.py` & `nnsight-0.2.9/src/nnsight/models/LanguageModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,18 @@
         self.automodel = (
             automodel
             if not isinstance(automodel, str)
             else getattr(modeling_auto, automodel)
         )
 
         super().__init__(*args, **kwargs)
+        
+        if not hasattr(self._model, 'generator'):
+            
+            setattr(self._model, 'generator', WrapperModule())
 
     def _load(self, repo_id: str, **kwargs) -> PreTrainedModel:
 
         config = AutoConfig.from_pretrained(repo_id, **kwargs)
 
         if self.tokenizer is None:
 
@@ -150,16 +154,14 @@
             )
             self.tokenizer.pad_token = self.tokenizer.eos_token
 
         if self._model is None:
 
             model = self.automodel.from_config(config, trust_remote_code=True)
 
-            setattr(model, 'generator', WrapperModule())
-
             return model
         
         model = self.automodel.from_pretrained(repo_id, config=config, **kwargs)
 
         setattr(model, 'generator', WrapperModule())
 
         return model
```

### Comparing `nnsight-0.2.8/src/nnsight/models/Mamba.py` & `nnsight-0.2.9/src/nnsight/models/Mamba.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ..patching import Patch, Patcher
 from .LanguageModel import LanguageModel
 
 from torch._guards import detect_fake_mode
 
 class Mamba(LanguageModel):
 
-    def _load(self, repo_id: str, device='meta', **kwargs) -> PreTrainedModel:
+    def _load(self, repo_id: str, device='cpu', **kwargs) -> PreTrainedModel:
 
         config = MambaConfig(**load_config_hf(repo_id))
 
         if self.tokenizer is None:
 
             self.tokenizer = AutoTokenizer.from_pretrained(
                 repo_id, config=config, padding_side="left"
```

### Comparing `nnsight-0.2.8/src/nnsight/models/NNsightModel.py` & `nnsight-0.2.9/src/nnsight/models/NNsightModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 
 import gc
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 import accelerate
 import torch
 from transformers import AutoConfig, AutoModel
+from typing_extensions import Self
 
 from .. import util
 from ..contexts.Runner import Runner
 from ..envoy import Envoy
-from ..intervention import (HookHandler, InterventionHandler,
-                            InterventionProxy, intervene)
+from ..intervention import (
+    HookHandler,
+    InterventionHandler,
+    InterventionProxy,
+    intervene,
+)
 from ..logger import logger
 from ..tracing.Graph import Graph
 
 
 class NNsight:
     """Main class to be implemented as a wrapper for PyTorch models wishing to gain this package's functionality. Can be used "as is" for basic models.
 
@@ -77,27 +82,27 @@
         else:
             self._envoy = Envoy(self._model)
 
         logger.info(f"Initialized `{self._model_key}`")
 
     def trace(
         self,
-        *inputs: Tuple[Any],
+        *inputs: Any,
         trace: bool = True,
         invoker_args: Dict[str, Any] = None,
         scan: bool = True,
         **kwargs: Dict[str, Any],
     ) -> Union[Runner, Any]:
         """Entrypoint into the tracing and interleaving functionality nnsight provides.
 
         In short, allows access to the future inputs and outputs of modules in order to trace what operations you would like to perform on them.
         This can be as simple as accessing and saving activations for inspection, or as complicated as transforming the activations and gradients in a forward pass over multiple inputs.
 
         Args:
-            inputs (Tuple[Any])
+            inputs (tuple[Any])
             trace (bool, optional): If to open a tracing context. Otherwise immediately run the model and return the raw output. Defaults to True.
             invoker_args (Dict[str, Any], optional): Keyword arguments to pass to Invoker initialization, and then downstream to the model's .prepare_inputs(...) method. Used when giving input directly to `.trace(...)`. Defaults to None.
             kwargs (Dict[str, Any]): Keyword arguments passed to Runner/Tracer initialization, and then downstream to the model's ._execute(...) method.
 
         Raises:
             ValueError: If trace is False and no inputs were provided (nothing to run with)
 
@@ -262,24 +267,33 @@
         return output
 
     def dispatch_model(self, *args, **kwargs) -> None:
         """Dispatch ._model to have real parameters  using .load(...)."""
 
         logger.info(f"Dispatching `{self._model_key}`...")
 
-        self._model = self._load(
-            self._model_key, *self._args, *args, **kwargs, **self._kwargs
-        )
+        self._model = self._load(self._model_key, *self._args, *args, **kwargs, **self._kwargs)
 
         self._envoy = Envoy(self._model)
 
         self._dispatched = True
 
         logger.info(f"Dispatched `{self._model_key}`")
 
+    def to(self, *args, **kwargs) -> Self:
+        """Override torch.nn.Module.to so this returns the NNSight model, not the underlying module when doing: model = model.to(...)
+
+        Returns:
+            Envoy: Envoy.
+        """
+
+        self._model = self._model.to(*args, **kwargs)
+
+        return self
+
     def __repr__(self) -> str:
         """Wrapper of ._model's representation as the NNsight model's representation.
 
         Returns:
             str: Representation.
         """
         return repr(self._model)
@@ -310,59 +324,57 @@
 
             config = AutoConfig.from_pretrained(repo_id, *args, **kwargs)
 
             return AutoModel.from_config(config, trust_remote_code=True)
 
         return accelerate.load_checkpoint_and_dispatch(self._model, repo_id, **kwargs)
 
-    def _execute(self, *prepared_inputs: Tuple[Any], **kwargs) -> Any:
+    def _execute(self, *prepared_inputs: Any, **kwargs) -> Any:
         """Virtual method to run the underlying ._model with some inputs.
 
         Default implementation util.applies moving all tensors to the device of the first parameter in ._model and passes the values into the model.
 
         Args:
-            prepared_inputs (Tuple[Any]): Prepared inputs.
+            prepared_inputs (tuple[Any]): Prepared inputs.
         """
         device = next(self._model.parameters()).device
 
-        prepared_inputs = util.apply(
-            prepared_inputs, lambda x: x.to(device), torch.Tensor
-        )
+        prepared_inputs = util.apply(prepared_inputs, lambda x: x.to(device), torch.Tensor)
 
         return self._model(
             *prepared_inputs,
             **kwargs,
         )
 
-    def _prepare_inputs(self, *inputs: Tuple[Any], **kwargs) -> Tuple[Tuple[Any], int]:
+    def _prepare_inputs(self, *inputs: Any, **kwargs) -> Tuple[Tuple[Any], int]:
         """Virtual method to prepare inputs before batching and execution and return batch size of prepared_inputs.
 
         Default implementation just returns inputs and length of first input.
 
         Args:
-            inputs (Tuple[Any]): Inputs to prepare for batching and execution.
+            inputs (tuple[Any]): Inputs to prepare for batching and execution.
             int: Batch size of prepared_inputs.
 
         Returns:
-            Tuple[Tuple[Any], int]: Prepared inputs, batch size of inputs.
+            Tuple[tuple[Any], int]: Prepared inputs, batch size of inputs.
         """
         return inputs, len(inputs[0])
 
     def _batch_inputs(
         self,
         batched_inputs: Optional[Any],
-        *prepared_inputs: Tuple[Any],
+        *prepared_inputs: Any,
     ) -> Any:
         """Virtual method to batch together results from _prepare_inputs.
 
         Default implementation returns list of all prepared_inputs.
 
         Args:
             batched_inputs (Any): Current state of batched_inputs. Initially None.
-            prepared_inputs (Tuple[Any]): Most recent result from _prepare_inputs.
+            prepared_inputs (tuple[Any]): Most recent result from _prepare_inputs.
 
         Returns:
             Any: Batched inputs.
         """
 
         if batched_inputs is None:
             batched_inputs = prepared_inputs
```

### Comparing `nnsight-0.2.8/src/nnsight/models/UnifiedTransformer.py` & `nnsight-0.2.9/src/nnsight/models/UnifiedTransformer.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/models/__init__.py` & `nnsight-0.2.9/src/nnsight/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/models/mixins/Generation.py` & `nnsight-0.2.9/src/nnsight/models/mixins/Generation.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/nnsight.log` & `nnsight-0.2.9/src/nnsight/nnsight.log`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/patching.py` & `nnsight-0.2.9/src/nnsight/patching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The patching module handles patching of classes and functions in modules."""
 from __future__ import annotations
 
 import importlib
 import types
 from contextlib import AbstractContextManager
-from typing import Any, List
+from typing import Any, List, Optional
 
 from . import util
 
 
 class Patch:
     """Class representing a replacement of an attribute on a module.
 
@@ -37,15 +37,15 @@
 class Patcher(AbstractContextManager):
     """Context manager that patches from a list of Patches on __enter__ and restores the patch on __exit__.
 
     Attributes:
         patches (List[Patch]):
     """
 
-    def __init__(self, patches: List[Patch] = None) -> None:
+    def __init__(self, patches: Optional[List[Patch]] = None) -> None:
         self.patches = patches or []
 
     def add(self, patch: Patch) -> None:
         """Adds a Patch to the patches. Also calls `.patch()` on the Patch.
 
         Args:
             patch (Patch): Patch to add.
```

### Comparing `nnsight-0.2.8/src/nnsight/pydantics/Config.py` & `nnsight-0.2.9/src/nnsight/pydantics/Config.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/pydantics/Request.py` & `nnsight-0.2.9/src/nnsight/pydantics/Request.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/pydantics/Response.py` & `nnsight-0.2.9/src/nnsight/pydantics/Response.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/pydantics/format/functions.py` & `nnsight-0.2.9/src/nnsight/pydantics/format/functions.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/pydantics/format/types.py` & `nnsight-0.2.9/src/nnsight/pydantics/format/types.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/.ipynb_checkpoints/logit_lens-checkpoint.ipynb` & `nnsight-0.2.9/src/nnsight/toolbox/.ipynb_checkpoints/logit_lens-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/das.ipynb` & `nnsight-0.2.9/src/nnsight/toolbox/das.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/interventions/.ipynb_checkpoints/transformations-checkpoint.py` & `nnsight-0.2.9/src/nnsight/toolbox/interventions/.ipynb_checkpoints/transformations-checkpoint.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/interventions/interventions.py` & `nnsight-0.2.9/src/nnsight/toolbox/interventions/interventions.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/interventions/transformations.py` & `nnsight-0.2.9/src/nnsight/toolbox/interventions/transformations.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/lens/lens.py` & `nnsight-0.2.9/src/nnsight/toolbox/lens/lens.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/lens/utils.py` & `nnsight-0.2.9/src/nnsight/toolbox/lens/utils.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/logit_lens.ipynb` & `nnsight-0.2.9/src/nnsight/toolbox/logit_lens.ipynb`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/toolbox/optim/lora.py` & `nnsight-0.2.9/src/nnsight/toolbox/optim/lora.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/tracing/Graph.py` & `nnsight-0.2.9/src/nnsight/tracing/Graph.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/tracing/Node.py` & `nnsight-0.2.9/src/nnsight/tracing/Node.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/tracing/Proxy.py` & `nnsight-0.2.9/src/nnsight/tracing/Proxy.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/tracing/__init__.py` & `nnsight-0.2.9/src/nnsight/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight/util.py` & `nnsight-0.2.9/src/nnsight/util.py`

 * *Files identical despite different names*

### Comparing `nnsight-0.2.8/src/nnsight.egg-info/PKG-INFO` & `nnsight-0.2.9/src/nnsight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnsight
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package for interpreting and manipulating the internals of deep learning models.
 Author-email: Jaden Fiotto-Kaufman <jadenfk@outlook.com>
 Project-URL: Homepage, https://github.com/JadenFiotto-Kaufman/nnsight
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nnsight Version: 0.2.8 Summary: Package for
+Metadata-Version: 2.1 Name: nnsight Version: 0.2.9 Summary: Package for
 interpreting and manipulating the internals of deep learning models. Author-
 email: Jaden Fiotto-Kaufman
 outlook.com> Project-URL: Homepage, https://github.com/JadenFiotto-Kaufman/
 nnsight Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE Requires-Dist: transformers Requires-Dist: protobuf Requires-Dist:
```

### Comparing `nnsight-0.2.8/src/nnsight.egg-info/SOURCES.txt` & `nnsight-0.2.9/src/nnsight.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENCE
 NNsight_v0_2.ipynb
 README.md
+conftest.py
 pyproject.toml
 .github/workflows/publish.yml
 .github/workflows/python-app.yml
 docs/.DS_Store
 docs/Makefile
 docs/contributing.md
 docs/make.bat
@@ -150,9 +151,8 @@
 src/nnsight/toolbox/optim/lora.py
 src/nnsight/toolbox/optim/softprompt.py
 src/nnsight/tracing/Graph.py
 src/nnsight/tracing/Node.py
 src/nnsight/tracing/Proxy.py
 src/nnsight/tracing/__init__.py
 tests/__init__.py
-tests/conftest.py
 tests/test_lm.py
```

### Comparing `nnsight-0.2.8/tests/test_lm.py` & `nnsight-0.2.9/tests/test_lm.py`

 * *Files identical despite different names*

