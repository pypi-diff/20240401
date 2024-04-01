# Comparing `tmp/ipex_llm-2.1.0b20240331-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240401-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5222679 bytes, number of entries: 208
+Zip file size: 5222801 bytes, number of entries: 208
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     2914 b- defN 24-Mar-25 11:36 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12251 b- defN 24-Mar-27 11:49 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,71 +38,71 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx     9866 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-Mar-31 11:38 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Mar-31 11:38 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   440320 b- defN 24-Mar-31 11:38 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   852992 b- defN 24-Mar-31 11:38 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   855552 b- defN 24-Mar-31 11:38 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   843264 b- defN 24-Mar-31 11:38 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-Mar-31 11:38 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   500224 b- defN 24-Mar-31 11:38 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   464384 b- defN 24-Mar-31 11:38 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   441344 b- defN 24-Mar-31 11:38 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   524800 b- defN 24-Mar-31 11:38 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   501248 b- defN 24-Mar-31 11:38 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   518656 b- defN 24-Mar-31 11:38 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   495104 b- defN 24-Mar-31 11:38 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   555520 b- defN 24-Mar-31 11:38 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   531968 b- defN 24-Mar-31 11:38 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Mar-31 11:38 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   494080 b- defN 24-Mar-31 11:38 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Mar-31 11:38 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   724992 b- defN 24-Mar-31 11:38 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-Mar-31 11:38 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Mar-31 11:38 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Mar-31 11:38 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   125952 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   126976 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   103936 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   108544 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   109568 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128000 b- defN 24-Mar-31 11:38 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Mar-31 11:38 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   531456 b- defN 24-Mar-31 11:38 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-Apr-01 11:38 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-Apr-01 11:38 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   440320 b- defN 24-Apr-01 11:38 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   852992 b- defN 24-Apr-01 11:38 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   855552 b- defN 24-Apr-01 11:38 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   843264 b- defN 24-Apr-01 11:38 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-Apr-01 11:38 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   500224 b- defN 24-Apr-01 11:38 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   464384 b- defN 24-Apr-01 11:38 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   441344 b- defN 24-Apr-01 11:38 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   524800 b- defN 24-Apr-01 11:38 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   501248 b- defN 24-Apr-01 11:38 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   518656 b- defN 24-Apr-01 11:38 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   495104 b- defN 24-Apr-01 11:38 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   555520 b- defN 24-Apr-01 11:38 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   531968 b- defN 24-Apr-01 11:38 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-Apr-01 11:38 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   494080 b- defN 24-Apr-01 11:38 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-Apr-01 11:38 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   724992 b- defN 24-Apr-01 11:38 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-Apr-01 11:38 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-Apr-01 11:38 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-Apr-01 11:38 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   125952 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   103936 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   108544 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   109568 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128000 b- defN 24-Apr-01 11:38 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-Apr-01 11:38 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   531456 b- defN 24-Apr-01 11:38 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1142 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    17533 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    11371 b- defN 24-Mar-27 11:49 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx     8692 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    63571 b- defN 24-Mar-28 11:37 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    63542 b- defN 24-Apr-01 11:38 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14256 b- defN 24-Mar-25 11:36 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     2170 b- defN 24-Mar-25 11:36 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     5429 b- defN 24-Mar-25 11:36 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    35476 b- defN 24-Mar-29 11:38 ipex_llm/transformers/low_bit_linear.py
 -rw-------  2.0 unx    34984 b- defN 24-Mar-29 11:38 ipex_llm/transformers/model.py
 -rw-------  2.0 unx     6921 b- defN 24-Mar-25 11:36 ipex_llm/transformers/modelling_bigdl.py
 -rw-------  2.0 unx    14770 b- defN 24-Mar-25 11:36 ipex_llm/transformers/qlora.py
 -rw-------  2.0 unx    16567 b- defN 24-Mar-25 11:36 ipex_llm/transformers/relora.py
 -rw-------  2.0 unx    52490 b- defN 24-Mar-28 11:37 ipex_llm/transformers/speculative.py
 -rw-------  2.0 unx     8404 b- defN 24-Mar-25 11:36 ipex_llm/transformers/training_patch.py
--rw-------  2.0 unx    13132 b- defN 24-Mar-29 11:38 ipex_llm/transformers/utils.py
+-rw-------  2.0 unx    13781 b- defN 24-Apr-01 11:38 ipex_llm/transformers/utils.py
 -rw-------  2.0 unx     7611 b- defN 24-Mar-25 11:36 ipex_llm/transformers/xpu_customize_fwd.py
 -rw-------  2.0 unx      875 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/__init__.py
 -rw-------  2.0 unx     2172 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/act.py
 -rw-------  2.0 unx     8861 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq.py
 -rw-------  2.0 unx     4422 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq_config.py
 -rw-------  2.0 unx    14550 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/linear.py
 -rw-------  2.0 unx      620 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/__init__.py
@@ -196,15 +196,15 @@
 -rw-------  2.0 unx    11428 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_llama.py
 -rw-------  2.0 unx     8770 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_mistral.py
 -rw-------  2.0 unx     8675 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_mixtral.py
 -rw-------  2.0 unx     7699 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_model.py
 -rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/__init__.py
 -rw-------  2.0 unx     8707 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/tokenizer.py
 -rw-------  2.0 unx    13950 b- defN 24-Mar-25 11:36 ipex_llm/vllm/worker/worker.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240331.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240331.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4466 b- defN 24-Mar-31 11:38 ipex_llm-2.1.0b20240331.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Mar-31 11:38 ipex_llm-2.1.0b20240331.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Mar-31 11:38 ipex_llm-2.1.0b20240331.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Mar-31 11:38 ipex_llm-2.1.0b20240331.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    19798 b- defN 24-Mar-31 11:38 ipex_llm-2.1.0b20240331.dist-info/RECORD
-208 files, 12688397 bytes uncompressed, 5191015 bytes compressed:  59.1%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240401.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240401.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4466 b- defN 24-Apr-01 11:39 ipex_llm-2.1.0b20240401.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-Apr-01 11:39 ipex_llm-2.1.0b20240401.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-Apr-01 11:39 ipex_llm-2.1.0b20240401.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-Apr-01 11:39 ipex_llm-2.1.0b20240401.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    19798 b- defN 24-Apr-01 11:39 ipex_llm-2.1.0b20240401.dist-info/RECORD
+208 files, 12689017 bytes uncompressed, 5191137 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -597,29 +597,29 @@
 
 Filename: ipex_llm/vllm/transformers_utils/tokenizer.py
 Comment: 
 
 Filename: ipex_llm/vllm/worker/worker.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240331.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240401.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240331.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240401.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240331.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240401.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240331.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240401.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240331.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240401.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240331.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240401.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240331.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240401.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,16 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	in     (%dx),%al
-   180005635:	rex.WX or %rsp,0x0(%rsi)
+   180005634:	addr32 pushf
+   180005636:	or     0x0(%rsi),%ah
    180005639:	add    %al,(%rax)
    18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004e578
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000004ea00
 SizeOfInitializedData	00000000000bea00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004e578
@@ -104628,16 +104628,16 @@
    18005771a:	add    $0x180,%eax
    18005771f:	add    %dh,0x6(%rax)
    180057722:	add    $0x180,%eax
    180057727:	add    %bh,0x6(%rax)
    18005772a:	add    $0x180,%eax
    18005772f:	add    %al,(%rax)
    180057731:	add    %al,(%rax)
-   180057733:	add    %ch,%ah
-   180057735:	rex.WX or %rsp,0x0(%rsi)
+   180057733:	add    %ah,-0x64(%rdi)
+   180057736:	or     0x0(%rsi),%ah
    180057739:	add    %al,(%rax)
    18005773b:	add    %cl,0x50000000(%rip)        # 0x1d0057741
    180057741:	add    (%rax),%eax
    180057743:	add    %ah,(%rax)
    180057745:	addl   $0x0,0x56f2000(%rip)        # 0x18574974f
 	...
    18005777f:	add    %dl,0x1800584(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,16 +5058,16 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	in     (%dx),%al
-   1800049d5:	rex.WX or %rsp,0x0(%rsi)
+   1800049d4:	addr32 pushf
+   1800049d6:	or     0x0(%rsi),%ah
    1800049d9:	add    %al,(%rax)
    1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055cd8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:17 2024
+Time/Date		Mon Apr  1 11:37:12 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056600
 SizeOfInitializedData	00000000000c5a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055cd8
@@ -115976,16 +115976,16 @@
    18005efbd:	add    %al,(%rax)
    18005efbf:	add    %bh,0x1800586(%rax)
    18005efc5:	add    %al,(%rax)
    18005efc7:	add    %al,%al
    18005efc9:	xchg   %al,0x180(%rip)        # 0x18005f14f
    18005efcf:	add    %al,(%rax)
    18005efd1:	add    %al,(%rax)
-   18005efd3:	add    %ch,%ch
-   18005efd5:	rex.WX or %rsp,0x0(%rsi)
+   18005efd3:	add    %ch,-0x64(%rax)
+   18005efd6:	or     0x0(%rsi),%ah
    18005efd9:	add    %al,(%rax)
    18005efdb:	add    %cl,0x50000000(%rip)        # 0x1d005efe1
    18005efe1:	add    (%rax),%eax
    18005efe3:	add    %al,(%rsp,%rdi,8)
    18005efe6:	add    $0x5e60400,%eax
 	...
    18005efff:	add    %bh,-0x1(%rax)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180053f68
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:38:28 2024
+Time/Date		Mon Apr  1 11:38:20 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000054400
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000053f68
@@ -109705,18 +109705,17 @@
    18005d64a:	add    $0x180,%eax
    18005d64f:	add    %dh,0x66(%rax)
    18005d652:	add    $0x180,%eax
    18005d657:	add    %bh,0x66(%rax)
    18005d65a:	add    $0x180,%eax
    18005d65f:	add    %al,(%rax)
    18005d661:	add    %al,(%rax)
-   18005d663:	add    %dh,(%rbx,%rcx,2)
-   18005d666:	or     %esp,0x0(%rsi)
-   18005d669:	add    %al,(%rax)
-   18005d66b:	add    %cl,0x50000000(%rip)        # 0x1d005d671
+   18005d663:	add    %ch,0x660a(%rsp,%rbx,4)
+   18005d66a:	add    %al,(%rax)
+   18005d66c:	or     $0x50000000,%eax
    18005d671:	add    (%rax),%eax
    18005d673:	add    %ah,(%rax)
    18005d675:	loopne 0x18005d67c
    18005d677:	add    %ah,(%rax)
    18005d679:	enter  $0x5,$0x0
    18005d67d:	add    %al,(%rax)
    18005d67f:	add    %dl,0x18005e3(%rax)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004e788
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:39:39 2024
+Time/Date		Mon Apr  1 11:39:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000004ee00
 SizeOfInitializedData	00000000000bea00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004e788
@@ -104731,16 +104731,17 @@
    1800576fa:	add    $0x180,%eax
    1800576ff:	add    %dh,0x6(%rax)
    180057702:	add    $0x180,%eax
    180057707:	add    %bh,0x6(%rax)
    18005770a:	add    $0x180,%eax
    18005770f:	add    %al,(%rax)
    180057711:	add    %al,(%rax)
-   180057713:	add    %bh,0x4b(%rbx)
-   180057716:	or     %esp,0x0(%rsi)
+   180057713:	add    %ch,%ch
+   180057715:	pushf
+   180057716:	or     0x0(%rsi),%ah
    180057719:	add    %al,(%rax)
    18005771b:	add    %cl,0x50000000(%rip)        # 0x1d0057721
    180057721:	add    (%rax),%eax
    180057723:	add    %ah,(%rax)
    180057725:	addl   $0x0,0x5732000(%rip)        # 0x18578972f
 	...
    18005777f:	add    %dl,0x1800584(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b758
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:38:29 2024
+Time/Date		Mon Apr  1 11:38:21 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c000
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b758
@@ -121123,15 +121123,15 @@
    180063f0f:	add    %bh,0x18005d6(%rax)
    180063f15:	add    %al,(%rax)
    180063f17:	add    %al,%al
    180063f19:	(bad)
    180063f1a:	add    $0x180,%eax
    180063f1f:	add    %al,(%rax)
    180063f21:	add    %al,(%rax)
-   180063f23:	add    %dh,0x66094b(%rip)        # 0x1806c4874
+   180063f23:	add    %ch,0x660a9c(%rbp)
    180063f29:	add    %al,(%rax)
    180063f2b:	add    %cl,0x50000000(%rip)        # 0x1d0063f31
    180063f31:	add    (%rax),%eax
    180063f33:	add    %al,0x3f840006(%rbx,%rcx,2)
    180063f3a:	(bad)
 	...
    180063f7f:	add    %bh,%al
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055ee8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:39:40 2024
+Time/Date		Mon Apr  1 11:39:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056800
 SizeOfInitializedData	00000000000c5c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055ee8
@@ -116151,18 +116151,19 @@
    18005ef9d:	add    %al,(%rax)
    18005ef9f:	add    %bh,0x1800586(%rax)
    18005efa5:	add    %al,(%rax)
    18005efa7:	add    %al,%al
    18005efa9:	xchg   %al,0x180(%rip)        # 0x18005f12f
    18005efaf:	add    %al,(%rax)
    18005efb1:	add    %al,(%rax)
-   18005efb3:	add    %bh,0x9(%rbx,%rcx,2)
-   18005efb7:	data16 add %al,(%rax)
-   18005efba:	add    %al,(%rax)
-   18005efbc:	or     $0x50000000,%eax
+   18005efb3:	add    %ch,%dh
+   18005efb5:	pushf
+   18005efb6:	or     0x0(%rsi),%ah
+   18005efb9:	add    %al,(%rax)
+   18005efbb:	add    %cl,0x50000000(%rip)        # 0x1d005efc1
    18005efc1:	add    (%rax),%eax
    18005efc3:	add    %al,(%rsp,%rdi,8)
    18005efc6:	add    $0x5e80400,%eax
 	...
    18005efff:	add    %bh,-0x1(%rax)
    18005f002:	add    $0x180,%eax
    18005f007:	add    %al,0x18005ff(%rax)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a468
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:38:29 2024
+Time/Date		Mon Apr  1 11:38:21 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005ac00
 SizeOfInitializedData	00000000000c5c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a468
@@ -119900,15 +119900,15 @@
    180062fd0:	enter  $0x5c6,$0x80
    180062fd4:	add    %eax,(%rax)
    180062fd6:	add    %al,(%rax)
    180062fd8:	rol    $1,%dh
    180062fda:	add    $0x180,%eax
    180062fdf:	add    %al,(%rax)
    180062fe1:	add    %al,(%rax)
-   180062fe3:	add    %dh,0x66094b(%rip)        # 0x1806c3934
+   180062fe3:	add    %ch,0x660a9c(%rbp)
    180062fe9:	add    %al,(%rax)
    180062feb:	add    %cl,0x50000000(%rip)        # 0x1d0062ff1
    180062ff1:	add    (%rax),%eax
    180062ff3:	add    %al,(%rax)
    180062ff5:	cmp    $0x6,%al
    180062ff7:	add    %al,(%rax)
    180062ff9:	sub    $0x6,%al
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180054bf8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:39:39 2024
+Time/Date		Mon Apr  1 11:39:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055400
 SizeOfInitializedData	00000000000c5800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000054bf8
@@ -114890,16 +114890,17 @@
    18005e084:	add    %eax,(%rax)
    18005e086:	add    %al,(%rax)
    18005e088:	shlb   $1,0x5(%rsi)
    18005e08b:	addb   $0x0,(%rcx)
    18005e08e:	add    %al,(%rax)
    18005e090:	add    %al,(%rax)
    18005e092:	add    %al,(%rax)
-   18005e094:	jnp    0x18005e0e1
-   18005e096:	or     %esp,0x0(%rsi)
+   18005e094:	out    %al,(%dx)
+   18005e095:	pushf
+   18005e096:	or     0x0(%rsi),%ah
    18005e099:	add    %al,(%rax)
    18005e09b:	add    %cl,0x50000000(%rip)        # 0x1d005e0a1
    18005e0a1:	add    (%rax),%eax
    18005e0a3:	add    %al,(%rax)
    18005e0a5:	in     (%dx),%eax
    18005e0a6:	add    $0x5d50000,%eax
 	...
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800618c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:38:28 2024
+Time/Date		Mon Apr  1 11:38:20 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061e00
 SizeOfInitializedData	00000000000c7800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000618c8
@@ -130450,16 +130450,17 @@
    18006ab45:	add    %al,(%rax)
    18006ab47:	add    %al,%al
    18006ab49:	ss (bad)
    18006ab4b:	addb   $0x0,(%rcx)
    18006ab4e:	add    %al,(%rax)
    18006ab50:	add    %al,(%rax)
    18006ab52:	add    %al,(%rax)
-   18006ab54:	xor    $0x4b,%al
-   18006ab56:	or     %esp,0x0(%rsi)
+   18006ab54:	lods   %ds:(%rsi),%al
+   18006ab55:	pushf
+   18006ab56:	or     0x0(%rsi),%ah
    18006ab59:	add    %al,(%rax)
    18006ab5b:	add    %cl,0x50000000(%rip)        # 0x1d006ab61
    18006ab61:	add    (%rax),%eax
    18006ab63:	add    %dl,%al
    18006ab65:	mov    $0xaed00006,%esp
    18006ab6a:	(bad)
 	...
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c0e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:39:39 2024
+Time/Date		Mon Apr  1 11:39:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c800
 SizeOfInitializedData	00000000000c7200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c0e8
@@ -125324,16 +125324,17 @@
    180065c15:	add    %al,(%rax)
    180065c17:	add    %al,%al
    180065c19:	out    %al,$0x5
    180065c1b:	addb   $0x0,(%rcx)
    180065c1e:	add    %al,(%rax)
    180065c20:	add    %al,(%rax)
    180065c22:	add    %al,(%rax)
-   180065c24:	jnp    0x180065c71
-   180065c26:	or     %esp,0x0(%rsi)
+   180065c24:	in     (%dx),%eax
+   180065c25:	pushf
+   180065c26:	or     0x0(%rsi),%ah
    180065c29:	add    %al,(%rax)
    180065c2b:	add    %cl,0x50000000(%rip)        # 0x1d0065c31
    180065c31:	add    (%rax),%eax
    180065c33:	add    %dl,%al
    180065c35:	insl   (%dx),%es:(%rdi)
    180065c36:	(bad)
    180065c37:	add    %dl,%al
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,16 +5355,16 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	in     (%dx),%al
-   180004a35:	rex.WX or %rsp,0x0(%rsi)
+   180004a34:	addr32 pushf
+   180004a36:	or     0x0(%rsi),%ah
    180004a39:	add    %al,(%rax)
    180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800549e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:17 2024
+Time/Date		Mon Apr  1 11:37:12 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055000
 SizeOfInitializedData	00000000000c5800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000549e8
@@ -114690,16 +114690,16 @@
    18005d0a1:	add    $0x180,%ax
    18005d0a5:	add    %al,(%rax)
    18005d0a7:	add    %dl,%al
    18005d0a9:	add    $0x180,%ax
    18005d0ad:	add    %al,(%rax)
    18005d0af:	add    %al,(%rax)
    18005d0b1:	add    %al,(%rax)
-   18005d0b3:	add    %ch,%ch
-   18005d0b5:	rex.WX or %rsp,0x0(%rsi)
+   18005d0b3:	add    %ch,-0x64(%rax)
+   18005d0b6:	or     0x0(%rsi),%ah
    18005d0b9:	add    %al,(%rax)
    18005d0bb:	add    %cl,0x50000000(%rip)        # 0x1d005d0c1
    18005d0c1:	add    (%rax),%eax
    18005d0c3:	add    %al,(%rax)
    18005d0c5:	fldl   0x5d10000(%rip)        # 0x185d6d0cb
 	...
    18005d0ff:	add    %dh,-0x20(%rax)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,16 +25509,16 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	in     (%dx),%al
-   140014ac5:	rex.WX or %rsp,0x0(%rsi)
+   140014ac4:	addr32 pushf
+   140014ac6:	or     0x0(%rsi),%ah
    140014ac9:	add    %al,(%rax)
    140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836bc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:40:10 2024
+Time/Date		Mon Apr  1 11:39:57 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cba00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836bc
@@ -188927,15 +188927,15 @@
    140093d55:	add    %al,(%rax)
    140093d57:	add    %al,(%rax)
    140093d59:	cltd
    140093d5a:	or     %al,0x1(%rax)
    140093d5d:	add    %al,(%rax)
    140093d5f:	add    %al,(%rax)
    140093d61:	add    %al,(%rax)
-   140093d63:	add    %bl,0x66094b(%rdx)
+   140093d63:	add    %cl,0x660a9d(%rip)        # 0x1406f4806
    140093d69:	add    %al,(%rax)
    140093d6b:	add    %cl,-0x34000000(%rip)        # 0x10c093d71
    140093d71:	add    (%rax),%eax
    140093d73:	add    %dl,-0x6ffff68f(%rax)
    140093d79:	(bad)
    140093d7a:	or     %eax,(%rax)
    140093d7c:	add    %al,(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:17 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,16 +24136,16 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	in     (%dx),%eax
-   140013ef5:	rex.WX or %rsp,0x0(%rsi)
+   140013ef4:	addr32 pushf
+   140013ef6:	or     0x0(%rsi),%ah
    140013ef9:	add    %al,(%rax)
    140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,16 +24679,16 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	in     (%dx),%al
-   140013fc5:	rex.WX or %rsp,0x0(%rsi)
+   140013fc4:	addr32 pushf
+   140013fc6:	or     0x0(%rsi),%ah
    140013fc9:	add    %al,(%rax)
    140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:17 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,16 +40341,16 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %ch,%ch
-   14001f125:	rex.WX or %rsp,0x0(%rsi)
+   14001f123:	add    %ah,-0x64(%rdi)
+   14001f126:	or     0x0(%rsi),%ah
    14001f129:	add    %al,(%rax)
    14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:17 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000acc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32180,16 +32180,16 @@
    140019105:	add    %al,(%rax)
    140019107:	add    %al,(%rax)
    140019109:	push   %rbp
    14001910a:	add    %eax,0x1(%rax)
    14001910d:	add    %al,(%rax)
    14001910f:	add    %al,(%rax)
    140019111:	add    %al,(%rax)
-   140019113:	add    %ch,%ch
-   140019115:	rex.WX or %rsp,0x0(%rsi)
+   140019113:	add    %ah,-0x64(%rdi)
+   140019116:	or     0x0(%rsi),%ah
    140019119:	add    %al,(%rax)
    14001911b:	add    %cl,0x20000000(%rip)        # 0x160019121
    140019121:	add    (%rax),%eax
    140019123:	add    %dh,%al
    140019125:	movabs 0x18ef00001,%al
 	...
    14001917e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:39:39 2024
+Time/Date		Mon Apr  1 11:39:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32322,16 +32322,17 @@
    1400190e5:	add    %al,(%rax)
    1400190e7:	add    %al,(%rax)
    1400190e9:	push   %rbp
    1400190ea:	add    %eax,0x1(%rax)
    1400190ed:	add    %al,(%rax)
    1400190ef:	add    %al,(%rax)
    1400190f1:	add    %al,(%rax)
-   1400190f3:	add    %bh,0x4b(%rbx)
-   1400190f6:	or     %esp,0x0(%rsi)
+   1400190f3:	add    %ch,%ch
+   1400190f5:	pushf
+   1400190f6:	or     0x0(%rsi),%ah
    1400190f9:	add    %al,(%rax)
    1400190fb:	add    %cl,0x20000000(%rip)        # 0x160019101
    140019101:	add    (%rax),%eax
    140019103:	add    %dh,%al
    140019105:	movabs 0x190f00001,%al
 	...
    14001917e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:15 2024
+Time/Date		Mon Apr  1 11:37:10 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27136,16 +27136,16 @@
    140015ef2:	add    %eax,0x1(%rax)
    140015ef5:	add    %al,(%rax)
    140015ef7:	add    %dh,0x23(%rax)
    140015efa:	add    %eax,0x1(%rax)
    140015efd:	add    %al,(%rax)
    140015eff:	add    %al,(%rax)
    140015f01:	add    %al,(%rax)
-   140015f03:	add    %ch,%bl
-   140015f05:	rex.WX or %rsp,0x0(%rsi)
+   140015f03:	add    %ah,-0x64(%rsi)
+   140015f06:	or     0x0(%rsi),%ah
    140015f09:	add    %al,(%rax)
    140015f0b:	add    %cl,-0x70000000(%rip)        # 0xd0015f11
    140015f11:	add    (%rax),%eax
    140015f13:	add    %ch,%al
    140015f15:	add    %eax,%fs:(%rax)
    140015f18:	call   0x14001606f
 	...
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:39:38 2024
+Time/Date		Mon Apr  1 11:39:24 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27264,16 +27264,17 @@
    140015ed0:	push   $0x1400123
    140015ed5:	add    %al,(%rax)
    140015ed7:	add    %dh,0x23(%rax)
    140015eda:	add    %eax,0x1(%rax)
    140015edd:	add    %al,(%rax)
    140015edf:	add    %al,(%rax)
    140015ee1:	add    %al,(%rax)
-   140015ee3:	add    %bh,0x4b(%rdx)
-   140015ee6:	or     %esp,0x0(%rsi)
+   140015ee3:	add    %ch,%ah
+   140015ee5:	pushf
+   140015ee6:	or     0x0(%rsi),%ah
    140015ee9:	add    %al,(%rax)
    140015eeb:	add    %cl,-0x70000000(%rip)        # 0xd0015ef1
    140015ef1:	add    (%rax),%eax
    140015ef3:	add    %ch,0x64(%rax)
    140015ef6:	add    %eax,(%rax)
    140015ef8:	push   $0x154
    140015efd:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:15 2024
+Time/Date		Mon Apr  1 11:37:10 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aaa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28430,16 +28430,16 @@
    140016fad:	add    %al,(%rax)
    140016faf:	add    %cl,0x1400133(%rax)
    140016fb5:	add    %al,(%rax)
    140016fb7:	add    %dl,0x1400133(%rax)
    140016fbd:	add    %al,(%rax)
    140016fbf:	add    %al,(%rax)
    140016fc1:	add    %al,(%rax)
-   140016fc3:	add    %ch,%bl
-   140016fc5:	rex.WX or %rsp,0x0(%rsi)
+   140016fc3:	add    %ah,-0x64(%rsi)
+   140016fc6:	or     0x0(%rsi),%ah
    140016fc9:	add    %al,(%rax)
    140016fcb:	add    %cl,-0x70000000(%rip)        # 0xd0016fd1
    140016fd1:	add    (%rax),%eax
    140016fd3:	add    %ch,0x1(%rbp,%rsi,2)
    140016fd7:	add    %ch,0x1(%rcx,%riz,2)
 	...
    140016fff:	add    %ah,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:39:38 2024
+Time/Date		Mon Apr  1 11:39:24 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aaa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28561,16 +28561,17 @@
    140016f8d:	add    %al,(%rax)
    140016f8f:	add    %cl,0x1400133(%rax)
    140016f95:	add    %al,(%rax)
    140016f97:	add    %dl,0x1400133(%rax)
    140016f9d:	add    %al,(%rax)
    140016f9f:	add    %al,(%rax)
    140016fa1:	add    %al,(%rax)
-   140016fa3:	add    %bh,0x4b(%rdx)
-   140016fa6:	or     %esp,0x0(%rsi)
+   140016fa3:	add    %ch,%ah
+   140016fa5:	pushf
+   140016fa6:	or     0x0(%rsi),%ah
    140016fa9:	add    %al,(%rax)
    140016fab:	add    %cl,-0x70000000(%rip)        # 0xd0016fb1
    140016fb1:	add    (%rax),%eax
    140016fb3:	add    %ch,0x1(%rbp,%rsi,2)
    140016fb7:	add    %ch,0x1(%rbp,%riz,2)
 	...
    140016fff:	add    %ah,(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c60
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c60
@@ -32535,16 +32535,16 @@
    140019205:	add    %al,(%rax)
    140019207:	add    %al,(%rax)
    140019209:	push   %rbp
    14001920a:	add    %eax,0x1(%rax)
    14001920d:	add    %al,(%rax)
    14001920f:	add    %al,(%rax)
    140019211:	add    %al,(%rax)
-   140019213:	add    %ch,%ah
-   140019215:	rex.WX or %rsp,0x0(%rsi)
+   140019213:	add    %ah,-0x64(%rdi)
+   140019216:	or     0x0(%rsi),%ah
    140019219:	add    %al,(%rax)
    14001921b:	add    %cl,0x20000000(%rip)        # 0x160019221
    140019221:	add    (%rax),%eax
    140019223:	add    %bh,%ah
    140019225:	movabs 0x191fc0001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Mar 31 11:39:39 2024
+Time/Date		Mon Apr  1 11:39:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e70
@@ -32652,16 +32652,17 @@
    1400191e5:	add    %al,(%rax)
    1400191e7:	add    %al,(%rax)
    1400191e9:	push   %rbp
    1400191ea:	add    %eax,0x1(%rax)
    1400191ed:	add    %al,(%rax)
    1400191ef:	add    %al,(%rax)
    1400191f1:	add    %al,(%rax)
-   1400191f3:	add    %bh,0x4b(%rbx)
-   1400191f6:	or     %esp,0x0(%rsi)
+   1400191f3:	add    %ch,%ch
+   1400191f5:	pushf
+   1400191f6:	or     0x0(%rsi),%ah
    1400191f9:	add    %al,(%rax)
    1400191fb:	add    %cl,0x20000000(%rip)        # 0x160019201
    140019201:	add    (%rax),%eax
    140019203:	add    %bh,%ah
    140019205:	movabs 0x193fc0001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:16 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,16 +4028,16 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	in     (%dx),%al
-   180004605:	rex.WX or %rsp,0x0(%rsi)
+   180004604:	addr32 pushf
+   180004606:	or     0x0(%rsi),%ah
    180004609:	add    %al,(%rax)
    18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bed8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Mar 31 11:37:17 2024
+Time/Date		Mon Apr  1 11:37:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c600
 SizeOfInitializedData	00000000000c7200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bed8
@@ -125217,16 +125217,16 @@
    180065c35:	add    %al,(%rax)
    180065c37:	add    %al,%al
    180065c39:	out    %al,$0x5
    180065c3b:	addb   $0x0,(%rcx)
    180065c3e:	add    %al,(%rax)
    180065c40:	add    %al,(%rax)
    180065c42:	add    %al,(%rax)
-   180065c44:	in     (%dx),%eax
-   180065c45:	rex.WX or %rsp,0x0(%rsi)
+   180065c44:	addr32 pushf
+   180065c46:	or     0x0(%rsi),%ah
    180065c49:	add    %al,(%rax)
    180065c4b:	add    %cl,0x50000000(%rip)        # 0x1d0065c51
    180065c51:	add    (%rax),%eax
    180065c53:	add    %dl,%al
    180065c55:	insl   (%dx),%es:(%rdi)
    180065c56:	(bad)
    180065c57:	add    %dl,%al
```

## ipex_llm/transformers/convert.py

```diff
@@ -188,15 +188,15 @@
     return ggml_weight
 
 
 def _replace_with_low_bit_linear(model, qtype, modules_to_not_convert=None,
                                  convert_shape_only=False,
                                  cpu_embedding=False, prefix_name='',
                                  imatrix_data=None, embedding_qtype=None,
-                                 model_type=None, torch_dtype=torch.float32,
+                                 model_config=None, torch_dtype=torch.float32,
                                  enable_xetla=False):
     from ipex_llm.transformers.low_bit_linear import LowBitLinear, FP4Params, \
         FP16Linear, BF16Linear
     from ipex_llm.transformers.embedding import LLMEmbedding, LowBitEmbedding
     has_been_replaced = False
 
     for name, module in model.named_children():
@@ -207,14 +207,15 @@
         if any(key in full_module_name for key in modules_to_not_convert):
             continue
 
         if is_linear and not isinstance(module, LowBitLinear):
             in_features, out_features, mp_group = linear_args
             optimize_lm_head = False
             if name == "lm_head":
+                model_type = getattr(model_config, "model_type", None)
                 if model_type in ["gptj", "llama"] and os.environ.get("BIGDL_OPTIMIZE_LM_HEAD",
                                                                       None) == "1":
                     optimize_lm_head = True
             with init_empty_weights():
                 new_linear = None
                 is_gptq = is_auto_gptq_available() and isinstance(module, QuantLinearCudaOld)
                 is_awq = is_auto_awq_available() and isinstance(module, WQLinear_GEMM)
@@ -258,15 +259,15 @@
                         mp_group=mp_group,
                         enable_xetla=enable_xetla,
                         optimize_lm_head=optimize_lm_head
                     )
                     cur_qtype, cur_imatrix = get_cur_qtype_and_imatrix(qtype,
                                                                        full_module_name,
                                                                        imatrix_data,
-                                                                       model_type)
+                                                                       model_config)
                     device = module.weight.data.device
                     # Copy the weights
                     paramsLowBit = FP4Params(data=module.weight.data,
                                              requires_grad=False,
                                              quantized=False,
                                              _shape=None,
                                              convert_shape_only=convert_shape_only,
@@ -374,15 +375,15 @@
                 qtype,
                 modules_to_not_convert,
                 convert_shape_only,
                 cpu_embedding,
                 prefix_name=prefix_name + '.' + name if prefix_name != '' else name,
                 imatrix_data=imatrix_data,
                 embedding_qtype=embedding_qtype,
-                model_type=model_type,
+                model_config=model_config,
                 torch_dtype=torch_dtype,
                 enable_xetla=enable_xetla,
             )
             has_been_replaced = _flag or has_been_replaced
     return model, has_been_replaced
 
 
@@ -648,25 +649,21 @@
     if _enable_ipex:
         model = _optimize_ipex(model, qtype)
         return model
 
     if optimize_model:
         model = _optimize_pre(model)
 
-    # mixed quantization needs model_type to choose custom quantization strategy
-    if hasattr(model, "config"):
-        model_type = getattr(model.config, "model_type", None)
-    else:
-        model_type = None
+    # mixed quantization needs model_config to choose custom quantization strategy
     model, has_been_replaced = _replace_with_low_bit_linear(
         model, qtype, modules_to_not_convert,
         convert_shape_only, cpu_embedding,
         imatrix_data=imatrix_data,
         embedding_qtype=embedding_qtype,
-        model_type=model_type,
+        model_config=getattr(model, "config", None),
         torch_dtype=torch_dtype,
         enable_xetla=enable_xetla,
     )
     if not has_been_replaced:
         warnings.warn(
             "No linear modules were found in "
             "your model. This can happen for some architectures such as gpt2 that uses Conv1D "
```

## ipex_llm/transformers/utils.py

```diff
@@ -263,29 +263,41 @@
         elif len(module_name_list) == 1:
             new_module_name = module_name_list[0]
             layer = None
             cur_module = None
     return new_module_name, layer, cur_module
 
 
-def get_cur_qtype_and_imatrix(qtype, full_module_name, imatrix_data, model_type=None):
+def get_cur_qtype_and_imatrix(qtype, full_module_name, imatrix_data, model_config=None):
     cur_qtype = qtype
+    if model_config is not None:
+        model_type = getattr(model_config, "model_type", None)
+    else:
+        model_dtype = None
     if qtype in [ggml_tensor_qtype["gguf_iq2_xxs"], ggml_tensor_qtype["gguf_iq2_xs"],
                  ggml_tensor_qtype["gguf_iq1_s"]]:
         # For quantization which needs importance matrix
         new_module_name, layer, cur_module = module_name_process(full_module_name)
         # custom mixed quantization strategy
         if model_type == "mixtral":
             if cur_module == 'v':
                 # llama.cpp use q4_K here
                 cur_qtype = ggml_tensor_qtype['sym_int4']
             elif cur_module == 'down' and int(layer) in [0, 1, 2, 3]:
                 cur_qtype = ggml_tensor_qtype['q2_k']
         else:
-            if cur_module == 'v' or (cur_module == 'down' and int(layer) in [0, 1, 10, 11]):
+            num_hidden_layers = getattr(model_config, "num_hidden_layers", None)
+            hidden_size = getattr(model_config, "hidden_size", None)
+            if model_type == "llama" and hidden_size == 8192:
+                # for llama2-70b
+                if cur_module == 'v':
+                    cur_qtype = ggml_tensor_qtype['sym_int4']  # llama.cpp use q4k here
+                if cur_module == 'down' and int(layer) < int(num_hidden_layers/8):
+                    cur_qtype = ggml_tensor_qtype['q2_k']
+            elif cur_module == 'v' or (cur_module == 'down' and int(layer) in [0, 1, 10, 11]):
                 cur_qtype = ggml_tensor_qtype['q2_k']
             if qtype == ggml_tensor_qtype["gguf_iq1_s"] and cur_module == 'o':
                 cur_qtype = ggml_tensor_qtype['gguf_iq2_xxs']
         if imatrix_data is not None and new_module_name in imatrix_data:
             cur_imatrix = imatrix_data[new_module_name]
         else:
             # if no imatrix is available, use sym_int8 for lm_head
```

## Comparing `ipex_llm-2.1.0b20240331.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240401.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240331.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240401.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240331.dist-info/METADATA` & `ipex_llm-2.1.0b20240401.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240331
+Version: 2.1.0b20240401
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240331) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240401) ; extra == 'cpp'
 Provides-Extra: serving
 Requires-Dist: py-cpuinfo ; extra == 'serving'
 Requires-Dist: fschat[model_worker,webui] (==0.2.36) ; extra == 'serving'
 Requires-Dist: protobuf ; extra == 'serving'
 Provides-Extra: xpu
 Requires-Dist: py-cpuinfo ; extra == 'xpu'
 Requires-Dist: protobuf ; extra == 'xpu'
@@ -39,47 +39,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240331) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240401) ; extra == 'xpu'
 Provides-Extra: xpu-2-0
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
 Requires-Dist: protobuf ; extra == 'xpu-2-0'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
 Requires-Dist: tabulate ; extra == 'xpu-2-0'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
 Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240331) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240331) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240401) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240401) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240331) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240401) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240331) ; (platform_system == "Linux") and extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240401) ; (platform_system == "Linux") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240331) ; (platform_system == "Linux") and extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240401) ; (platform_system == "Linux") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240331.dist-info/RECORD` & `ipex_llm-2.1.0b20240401.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -38,70 +38,70 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=0_5-i7FV4pS__4XVLVxyjZJN_uKSG6nSjHzZWIpzzVg,9866
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=NsaJxgrWIstU8wL2hEfDyUGyWK4NDlopZMYQzt5TyIc,36352
-ipex_llm/libs/bloom.dll,sha256=_tqsKmPHIUl8qj7tJItuki5E5qW4jOciNbu5FGonvF4,440320
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=am2Xg7WunImTS-VOwQbY9Ld90r_Jz4OkdoSgZNGGF2s,852992
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=eczq2sZanpQ_oYoM6If690Oy4aLL5VPEiYq4o-shaP0,855552
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=leu82pc1zAVhi8pERYPosSG0zadbRRoPVc-XodXCjv4,843264
-ipex_llm/libs/gptneox-api.dll,sha256=WTPmsusp7uMOe5IEfyFCQWlNliNC7chR0-LX-VKVbfQ,24576
-ipex_llm/libs/gptneox.dll,sha256=mwtBA9QAANX9BVedomdRkn3w2A7UR8U49oW-YcBrN6g,500224
-ipex_llm/libs/libbloom_avx.dll,sha256=a9DjoUkv29De7rE2PjglQ5QRsxyuNCAe4jDVDBIN9mQ,464384
-ipex_llm/libs/libbloom_vnni.dll,sha256=2lZPwLwALCfWiMJXLP8HDHXBInHcW8B8AG5W-pIpxfU,441344
-ipex_llm/libs/libgptneox_avx.dll,sha256=W9Pfx_d-hx_pjLIF80DM1tBV5lIrtEG9IIYJUqYnSVg,524800
-ipex_llm/libs/libgptneox_vnni.dll,sha256=alnDbDS0NjwtIYmoJ95ui9A3Ynf86DEoq7EcC9FLZR0,501248
-ipex_llm/libs/libllama_avx.dll,sha256=oBN_XHeo9NE3zj7-I7QbHK2j1rLWLafkXzIVhOXcHJ0,518656
-ipex_llm/libs/libllama_vnni.dll,sha256=dYFhtMRbwLmQzZ-naUwjkvu789eYQEOOU4EIcIvUWpA,495104
-ipex_llm/libs/libstarcoder_avx.dll,sha256=Iv1kV3j1sphqbf24x6XOiFuRwaabtVziMATTcbUgsm8,555520
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=n18IjeLXotkDxhskZVoKW1oIGo5P-OVJJ1QSuLu6TEI,531968
-ipex_llm/libs/llama-api.dll,sha256=afqsZbYAG2YC4XmLOepAA00Ers2kO5vBqgU7b8LfmzQ,25088
-ipex_llm/libs/llama.dll,sha256=IYtwWkzAc0Y_cF6ZZK04uTVzMurRwLoEEM9alqljwA8,494080
-ipex_llm/libs/main-bloom.exe,sha256=HZSWtVUh50Opnwg5ckxc8U6gTi6zQKieWuM1qOmPexg,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=iQALnAzQAAF3iXBpLQg01pKM6X83RBOyOn3iuPV-gXQ,724992
-ipex_llm/libs/main-gptneox.exe,sha256=87h0kmFsuM16g1wPVNcfk0TjMm4FANOcwXoWeCkHppw,98816
-ipex_llm/libs/main-llama.exe,sha256=GbyUaHLxtTkQofd2yxyZcfqbuVXcEXcMU5tglKV1VHA,99840
-ipex_llm/libs/main-starcoder.exe,sha256=IyXXphUvg6ALU-NTanOJxr_-fnk1ZYzlvULIX3YcOtA,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=jQ2reWzn1FT5uHW1rpRiU8YMpdD6SSKNEqR5NYYLgRE,125952
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=fRHfnuo7fet7BFJaALRSiUX4etakjBIjFZP55V4qBYs,126976
-ipex_llm/libs/quantize-gptneox.exe,sha256=LExwoAG8jQiL0c-qZPMAdmhnaI16RpSZZ0L6QKVlA2w,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=q79GdXr2MD7edtU4UOcX0pHTWp-cSbrl59a23vh2Wh0,103936
-ipex_llm/libs/quantize-llama.exe,sha256=bp69SphM0L-4jcX_H0pugIAk1AscCCDhjfng5wo_yo8,108544
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=oTBftKhXB8ftC95vc6KIHQ_KzqE1JOVtpNygbMbHRqk,109568
-ipex_llm/libs/quantize-starcoder.exe,sha256=UsVdppS_WJH6YMIukPNZgWsL32HZSTaGkUCStTni-iM,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=yJFP5Erh_hYWDIKtenQsng1GOiGHyhLunQ14umvLutw,128000
-ipex_llm/libs/starcoder-api.dll,sha256=pY3qc3iPtCYWkc5xtN57KhFkSktPg0YJGavqvayCL_k,21504
-ipex_llm/libs/starcoder.dll,sha256=rlE4bi0JXDpHN2sO4XYEVjB-d5o-swGx_HwOcdOTBdk,531456
+ipex_llm/libs/bloom-api.dll,sha256=tjWzshhqEhJ1_JS2WxMzJuQXISToC449laaWW5jC0Bs,36352
+ipex_llm/libs/bloom.dll,sha256=utiwQy3lXn7zaeBOMqpu_qO8VeCsXN1R0u2HjGH6x4I,440320
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=QXbA5MTBKcvYdagi-GGAIWVjlzSeBjCcqCv3ZRWqDKc,852992
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=EUjcTsiPPW7oeYW5CelaqF4ZKeZy5ovqJc7i9_gKrtM,855552
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=OEC7HjiHoheoI-OWsCgjwXjDkdFUoL0lAerZgNmGohM,843264
+ipex_llm/libs/gptneox-api.dll,sha256=LMYaXhGa92SkEsu7D3EEu1LHznFJ0IYPs3-d5NurpSw,24576
+ipex_llm/libs/gptneox.dll,sha256=fOlv12dOEmWBKwPXpeaaVNcC3UoCJjfqWXqzfiUdgsQ,500224
+ipex_llm/libs/libbloom_avx.dll,sha256=VwDvO7fwsoTOKfoXjPA3x0QiCIJweS26avr0MUKoqWU,464384
+ipex_llm/libs/libbloom_vnni.dll,sha256=pbB9Iwmsjd3LbR2sGoW7QRiOcM87J3g_uJDFrmDGofQ,441344
+ipex_llm/libs/libgptneox_avx.dll,sha256=BqgLDUs4mdEt3l-W_8IeFKQ4CEABxot-M-pdtIuLbkI,524800
+ipex_llm/libs/libgptneox_vnni.dll,sha256=4_QSKPSc-H2wUukBcaT6WxutlaQhCwrybwbY46yG7_4,501248
+ipex_llm/libs/libllama_avx.dll,sha256=QSh6Xy8yuH_4gOXz8yq2NeZ5NyoqKlHTmNhTwjGmb-8,518656
+ipex_llm/libs/libllama_vnni.dll,sha256=6EYp5rsxdxzToedcPx9Hq_PzxeiaDKRb6pnEx7qE61s,495104
+ipex_llm/libs/libstarcoder_avx.dll,sha256=EMtWXregc4pigDaRN3yLW2v_uxlInuYoXri26XIdEVY,555520
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=PY_58piJ-2opoTukAexaWo4qRILytgYYmEAqpxwO-iU,531968
+ipex_llm/libs/llama-api.dll,sha256=eV6VCNV8UAhyQy_rfmMecu23RZZwo0YATmx9wcg67co,25088
+ipex_llm/libs/llama.dll,sha256=TQHmRldnUj0SMGTwq9v0LRu_d-ClCn2dy2V3pl_6vEs,494080
+ipex_llm/libs/main-bloom.exe,sha256=GLongaClzsk5TMVeuNKSLe45Itq_Pe3eFUwxOA7gn8Q,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=7ZRD3iVoF3z6tBIUKyoDr6BXwz_4CFPTiIptT9wm3us,724992
+ipex_llm/libs/main-gptneox.exe,sha256=Lyg5HIVzP1xUygyadAu7_KVDfmbP2R0yLYLdr-OWkvE,98816
+ipex_llm/libs/main-llama.exe,sha256=6MWPJklKJaY74CRY5l1okm5xZ6VkKmdHJQrniwDwxUM,99840
+ipex_llm/libs/main-starcoder.exe,sha256=xxPd_Jo2rhl3-tMkIyvKFB4EvkuixJAacCG0AFXicdE,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=Y5ofbbTTEC527PyQwywP67tYGj70vCCB1ZhdOjkJRSs,125952
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=usPGM3PJ4aeGlS3mWN5PfQ0g01aTxd6BMwzBNP48fyc,126976
+ipex_llm/libs/quantize-gptneox.exe,sha256=Burr4m90oCdJpqWYjF6hh4pvc0ROUHy-XktN2Z73GGc,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=yxHEvTLgxf-PR53-tvaU0axnuQhRKSTId9Y9kLXYvpA,103936
+ipex_llm/libs/quantize-llama.exe,sha256=OsPYwoq1ttwz-zrTpUrh66zX_QL0aGEqMUrJBne6RIQ,108544
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=naEiirS40-nVKnHCCA2pIwKEKucxUvGh2tCOrlp_mdQ,109568
+ipex_llm/libs/quantize-starcoder.exe,sha256=6jQWlann0n2La1bsB15KfzJbHJR8Y8Z_6-Li2Ps8r8U,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=XS73DCKJK0fWK-YGewCDTqVlEDDzs6FbMwUbmm7HQ6o,128000
+ipex_llm/libs/starcoder-api.dll,sha256=Y7uw2ZHgL5M1owXBkVBO2ZgZf8boADZubqbIRcHrnwM,21504
+ipex_llm/libs/starcoder.dll,sha256=smaA0rCeQll6nNCk76BlLMMc5sDzrMuubcfl_SY514w,531456
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=-WV020bjHBbU9GTaapmlxDYUa6Eaul6rRnlK7WIDiow,1142
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=XDAPHCBtd1EgK2WHLYwHcFLxeMhNA2uY1EoAL0-Jpz0,17533
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=LNMHFYgJqna-4TfIYH7zfKElUXIYMqE0J0ICHpvMGPk,11371
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=x22OLdf0IdvuzHHVspczXb4q6bq4GNldtc3YdZsNGUs,8692
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=z8x9iAvyodc0StuIeBS95rmTjI3yw5OhzmvT8AuM_BY,63571
+ipex_llm/transformers/convert.py,sha256=Yuk7O7JO_y6HPMTJD4ervOE7NG8Krbj4r7AKGgRgK9g,63542
 ipex_llm/transformers/convert_ipex.py,sha256=CkeIR_Uy6FLeOjlj6vagfO1W_EaIp7a9y4n0q0PnAQY,14256
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=MVcInWiEQhFWcAu1VYf-6KPw4imt51FqWu1aJZGMW1E,2170
 ipex_llm/transformers/loader.py,sha256=mC9-RuJGIvpSdP0eyDQ3OY2q1SFTwM-TDlcv2ZSVNIo,5429
 ipex_llm/transformers/low_bit_linear.py,sha256=2vD-qMxMIshaUGus83lszxsCoEVgU5T1LnnPBImEKf8,35476
 ipex_llm/transformers/model.py,sha256=EokyTQdSfVpSVb5FIc6GLMasPHz8fBUOtm2UnGsX0ko,34984
 ipex_llm/transformers/modelling_bigdl.py,sha256=AqbRwpSAiHmKUo2FGOiwKtytlh-35NWb6eDy7YyNzoo,6921
 ipex_llm/transformers/qlora.py,sha256=WwHn2NXwx8SM6k7_xK1veppWiwL3g5PKihrbC3SPm-g,14770
 ipex_llm/transformers/relora.py,sha256=-dYzUV0P-IhO2jFdnzN9-v_sFzJpRj3ZwN9eCJzOoCw,16567
 ipex_llm/transformers/speculative.py,sha256=_xJ7vNig21OgzB--wGv1Ntkr5yOfnQd5iziWiA-qVpU,52490
 ipex_llm/transformers/training_patch.py,sha256=4_eQ2uCtGOnRVC2iPkzquuYnvERdneBb7Ovu_pc-VCA,8404
-ipex_llm/transformers/utils.py,sha256=JgPLf8pKak1SohURVFJYyFYN-2RoKLxfQhbsZ3FfcaA,13132
+ipex_llm/transformers/utils.py,sha256=kqjrM83Ir8o9fdhZ6Ks-XZ-x-xDyBVjGh6q9Wnlo5Io,13781
 ipex_llm/transformers/xpu_customize_fwd.py,sha256=wFpIhs5F6tkNs8gBOrLxWdhLzO3EDHovVkERPIAoAvg,7611
 ipex_llm/transformers/awq/__init__.py,sha256=Du5gu3-eeAkeDO_dEMBTzrDBA66DSN3uL3-rn8WGXQw,875
 ipex_llm/transformers/awq/act.py,sha256=YwomJzOOKwkKtzGrm4L4kwBstBLO1Z8SK4CKi8PSYVQ,2172
 ipex_llm/transformers/awq/awq.py,sha256=cGyRQJWwAEJtOtdSbsBoQ33KX_Ie0pv5OJHC0ACEELE,8861
 ipex_llm/transformers/awq/awq_config.py,sha256=SDZJUCAxuphwwnGqjLrbCJIo4KmFmiNgZOeKJI4DmvY,4422
 ipex_llm/transformers/awq/linear.py,sha256=Ko99_Jkjd5yVcOHCaoM7lxx3_qOGznnXK4Vk367mjUo,14550
 ipex_llm/transformers/gguf/__init__.py,sha256=58u1_Q6Chwd4yXK05iHu6zL8n1TbquUbcBtKd-53ozk,620
@@ -195,14 +195,14 @@
 ipex_llm/vllm/model_executor/models/bigdl_llama.py,sha256=8mjFjUWXql-pmoibwlGLWpPmHAD-_bpwcnAm8V1GIxA,11428
 ipex_llm/vllm/model_executor/models/bigdl_mistral.py,sha256=slF_zjHXFrQUxB-Qsl_vc0AKbnnfC_ahfdDAKGGt7HE,8770
 ipex_llm/vllm/model_executor/models/bigdl_mixtral.py,sha256=AKRYNG366ZMpjORC30IOak2OdctqKS0TG1Y4FKv7XdE,8675
 ipex_llm/vllm/model_executor/models/bigdl_model.py,sha256=ysQ3UNwUDLIZVEPtVd_ADQHeRCN2INYQeFlVIZP8qy4,7699
 ipex_llm/vllm/transformers_utils/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
 ipex_llm/vllm/transformers_utils/tokenizer.py,sha256=PKmEi1ROhf9dKRa-7AuKYwvAY-htP-ZIAz4HhNqhokU,8707
 ipex_llm/vllm/worker/worker.py,sha256=eifKuzefL9HC1R62P0mCYBsZlclo_5hQf01vFgc6mFA,13950
-ipex_llm-2.1.0b20240331.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240331.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240331.dist-info/METADATA,sha256=eQRCKJK31l_vShBiMwIadRYVpxvt5TKU5EJ8A2U3v_4,4466
-ipex_llm-2.1.0b20240331.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240331.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240331.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240331.dist-info/RECORD,,
+ipex_llm-2.1.0b20240401.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240401.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240401.dist-info/METADATA,sha256=H9Pzh73anVVsnuAQkHphU8XJMKbvNd5hpAL6_me2i0c,4466
+ipex_llm-2.1.0b20240401.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240401.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240401.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240401.dist-info/RECORD,,
```

