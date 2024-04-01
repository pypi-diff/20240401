# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.3.31-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.4.1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,57 @@
-Zip file size: 3094635 bytes, number of entries: 55
--rw-r--r--  2.0 unx      914 b- defN 24-Mar-31 12:58 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-Mar-31 12:58 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-Mar-31 12:58 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10613240 b- defN 24-Mar-31 12:58 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-Mar-31 12:58 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-Mar-31 12:58 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-Mar-31 12:58 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-Mar-31 12:58 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4143 b- defN 24-Mar-31 12:58 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-Mar-31 12:58 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    19841 b- defN 24-Mar-31 12:58 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5774 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26763 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3493 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    66517 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    96843 b- defN 24-Mar-31 12:58 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    40680 b- defN 24-Mar-31 12:58 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-Mar-31 12:58 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      383 b- defN 24-Mar-31 12:58 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-Mar-31 12:58 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-Mar-31 12:58 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-Mar-31 12:58 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-Mar-31 12:58 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      264 b- defN 24-Mar-31 12:58 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx     1464 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4154 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4154 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3369 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3369 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2148 b- defN 24-Mar-31 12:53 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3369 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3369 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3118 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3118 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2394 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2394 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4486 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4486 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3938 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3938 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      650 b- defN 24-Mar-31 12:53 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6136 b- defN 24-Mar-31 12:56 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2602 b- defN 24-Mar-31 12:58 fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-Mar-31 12:58 fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Mar-31 12:58 fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6022 b- defN 24-Mar-31 12:58 fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/RECORD
-55 files, 11025495 bytes uncompressed, 3084547 bytes compressed:  72.0%
+Zip file size: 3094625 bytes, number of entries: 55
+-rw-r--r--  2.0 unx      914 b- defN 24-Apr-01 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-Apr-01 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-Apr-01 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10613240 b- defN 24-Apr-01 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-Apr-01 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-Apr-01 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-Apr-01 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-Apr-01 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4143 b- defN 24-Apr-01 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-Apr-01 12:59 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    19841 b- defN 24-Apr-01 12:59 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5774 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26763 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    66517 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    96843 b- defN 24-Apr-01 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    40680 b- defN 24-Apr-01 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-Apr-01 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      383 b- defN 24-Apr-01 12:59 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-Apr-01 12:59 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-Apr-01 12:59 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-Apr-01 12:59 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-Apr-01 12:59 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      263 b- defN 24-Apr-01 12:59 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx     1464 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4154 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4154 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3369 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3369 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2148 b- defN 24-Apr-01 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3369 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3369 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3118 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3118 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2394 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2394 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4486 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4486 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3938 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3938 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      650 b- defN 24-Apr-01 12:54 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6136 b- defN 24-Apr-01 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2601 b- defN 24-Apr-01 12:59 fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-Apr-01 12:59 fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-01 12:59 fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6018 b- defN 24-Apr-01 12:59 fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/RECORD
+55 files, 11025489 bytes uncompressed, 3084545 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -147,20 +147,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.3.31"
+__version__: str = "2024.4.1"
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2024.3.31
+Version: 2024.4.1
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=S6qWfFzpqNIB8l9N3LAsYfaXSExg53f_b3fl47d1b1U,40680
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=BbAfYbNZsBhO7L5Am4wyBLet4mTY2aXFucyGTxF9IlI,383
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=kboZnkSTWS7K2kKtDhmUiMCN5V1_WBULGTQSZHrCUYY,264
+fbgemm_gpu/docs/version.py,sha256=4N1vqSsmQVp9Z8h7Rqg9gRsQl4wf0j4LTGExYwWcy1I,263
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=-pI93w4U-zJWrU1LDid0ofA5gPxhTDUGUXGivC2dMPQ,1464
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=QkLLWt4EBZ1Vpx4vMDxoQa5vdVN5juDWHycra43Q738,4154
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=QkLLWt4EBZ1Vpx4vMDxoQa5vdVN5juDWHycra43Q738,4154
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=8Z2xh7XBc5-_VXSf5w8m3wHXfbXt6ePw7rpcd5KgotY,3369
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py,sha256=8Z2xh7XBc5-_VXSf5w8m3wHXfbXt6ePw7rpcd5KgotY,3369
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=tqLQjNPy3pnMLLj_ymS2L8O1o2NAWZMxoIEDZuAsvFg,2148
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py,sha256=MMvCnLMfm3lzKd8fD6E29tkmaEjIw16BP1rZ9GI2Gac,3369
@@ -45,11 +45,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py,sha256=IybXfYpmDYof-Lyt8KPhPV_vtL6OUAMYyrB1lm9wFd0,4486
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=UQpaGNC1a_vuUe29-ZmrP2BLDSZC4b5yhzk1ODTWgCE,3938
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py,sha256=UQpaGNC1a_vuUe29-ZmrP2BLDSZC4b5yhzk1ODTWgCE,3938
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=MyJaWYi6f6UUpbNuxOlPEvKEY9xOIVwydpi1RJYcVEs,3736
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=MyJaWYi6f6UUpbNuxOlPEvKEY9xOIVwydpi1RJYcVEs,3736
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=pkpgT1nhXCvAniF7PlseJrxJTZEdiZGRvacnFNHJ6MA,650
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=soARoBsdOnNNZdCIkVmryPHtKyhbcFLqHOTveG-hk6s,6136
-fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/METADATA,sha256=G2TULj3yv-mK7Rr_IEQIiz3YB9y3q7S4u-JSibLXRUE,2602
-fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.3.31.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/METADATA,sha256=hWGnFDMelC-xwlLU26oyLFLXTthM_QksYoO33SLWmQI,2601
+fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
+fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.4.1.dist-info/RECORD,,
```

