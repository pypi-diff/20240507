# Comparing `tmp/ipex_llm-2.1.0b20240506-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240507-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5310495 bytes, number of entries: 188
+Zip file size: 5316691 bytes, number of entries: 189
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
--rw-------  2.0 unx     3091 b- defN 24-Apr-17 15:07 ipex_llm/llm_patching.py
+-rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
 -rw-------  2.0 unx      216 b- defN 24-Mar-25 11:36 ipex_llm/cli/prompts/chat-with-llm.txt
 -rw-------  2.0 unx     1272 b- defN 24-Mar-25 11:36 ipex_llm/ggml/__init__.py
 -rw-------  2.0 unx     5417 b- defN 24-Mar-25 11:36 ipex_llm/ggml/convert.py
@@ -38,69 +38,69 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-May-06 15:07 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-May-06 15:07 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   470528 b- defN 24-May-06 15:07 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   853504 b- defN 24-May-06 15:07 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-May-06 15:07 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844288 b- defN 24-May-06 15:07 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-May-06 15:07 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   530432 b- defN 24-May-06 15:07 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   496128 b- defN 24-May-06 15:07 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   471040 b- defN 24-May-06 15:07 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   556032 b- defN 24-May-06 15:07 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   530944 b- defN 24-May-06 15:07 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   549888 b- defN 24-May-06 15:07 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   525312 b- defN 24-May-06 15:07 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   586752 b- defN 24-May-06 15:07 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   561664 b- defN 24-May-06 15:07 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-May-06 15:07 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   524288 b- defN 24-May-06 15:07 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-May-06 15:07 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-May-06 15:07 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-May-06 15:07 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-May-06 15:07 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-May-06 15:07 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-May-06 15:07 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-May-06 15:07 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   561152 b- defN 24-May-06 15:07 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-07 15:08 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-07 15:08 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   470528 b- defN 24-May-07 15:08 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   853504 b- defN 24-May-07 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-07 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844288 b- defN 24-May-07 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-07 15:08 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   530432 b- defN 24-May-07 15:08 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   496128 b- defN 24-May-07 15:08 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   471040 b- defN 24-May-07 15:08 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   556032 b- defN 24-May-07 15:08 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   530944 b- defN 24-May-07 15:08 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   549888 b- defN 24-May-07 15:08 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   525312 b- defN 24-May-07 15:08 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   586752 b- defN 24-May-07 15:08 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   561664 b- defN 24-May-07 15:08 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-07 15:08 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   524288 b- defN 24-May-07 15:08 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-07 15:08 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-May-07 15:08 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-07 15:08 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-07 15:08 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-07 15:08 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-07 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-07 15:08 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   561152 b- defN 24-May-07 15:08 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
--rw-------  2.0 unx    11824 b- defN 24-May-06 15:07 ipex_llm/serving/fastchat/ipex_llm_worker.py
+-rw-------  2.0 unx    18709 b- defN 24-May-07 15:07 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx    10801 b- defN 24-Apr-29 15:08 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    73020 b- defN 24-Apr-29 15:08 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    74281 b- defN 24-May-07 15:07 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14334 b- defN 24-Apr-26 15:08 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4247 b- defN 24-Apr-29 15:08 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     3289 b- defN 24-Apr-18 12:34 ipex_llm/transformers/lisa.py
 -rw-------  2.0 unx     5787 b- defN 24-May-06 15:07 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    14860 b- defN 24-Apr-28 15:07 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    39805 b- defN 24-Apr-26 15:08 ipex_llm/transformers/low_bit_linear.py
 -rw-------  2.0 unx    36102 b- defN 24-Apr-25 15:07 ipex_llm/transformers/model.py
 -rw-------  2.0 unx     6921 b- defN 24-Mar-25 11:36 ipex_llm/transformers/modelling_bigdl.py
--rw-------  2.0 unx    14770 b- defN 24-Mar-25 11:36 ipex_llm/transformers/qlora.py
+-rw-------  2.0 unx    15520 b- defN 24-May-07 15:07 ipex_llm/transformers/qlora.py
 -rw-------  2.0 unx    16567 b- defN 24-Mar-25 11:36 ipex_llm/transformers/relora.py
 -rw-------  2.0 unx    56201 b- defN 24-May-06 15:07 ipex_llm/transformers/speculative.py
 -rw-------  2.0 unx     8404 b- defN 24-Mar-25 11:36 ipex_llm/transformers/training_patch.py
 -rw-------  2.0 unx    13931 b- defN 24-Apr-18 12:34 ipex_llm/transformers/utils.py
 -rw-------  2.0 unx     7611 b- defN 24-Mar-25 11:36 ipex_llm/transformers/xpu_customize_fwd.py
 -rw-------  2.0 unx      875 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/__init__.py
 -rw-------  2.0 unx     2172 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/act.py
@@ -135,27 +135,28 @@
 -rw-------  2.0 unx    24359 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/baichuan.py
 -rw-------  2.0 unx    27008 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/baichuan2.py
 -rw-------  2.0 unx     6085 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/bert.py
 -rw-------  2.0 unx     8971 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/bloom.py
 -rw-------  2.0 unx    13743 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm.py
 -rw-------  2.0 unx    31837 b- defN 24-Apr-30 15:07 ipex_llm/transformers/models/chatglm2.py
 -rw-------  2.0 unx     8697 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm2_32k.py
+-rw-------  2.0 unx    20840 b- defN 24-May-07 15:07 ipex_llm/transformers/models/cohere.py
 -rw-------  2.0 unx     8654 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/decilm.py
 -rw-------  2.0 unx    33549 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/falcon.py
 -rw-------  2.0 unx    12310 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/gemma.py
 -rw-------  2.0 unx     4342 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/gptbigcode.py
 -rw-------  2.0 unx    17973 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptj.py
 -rw-------  2.0 unx     6219 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptneox.py
 -rw-------  2.0 unx    11647 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/internlm.py
 -rw-------  2.0 unx    99215 b- defN 24-Apr-30 15:07 ipex_llm/transformers/models/llama.py
 -rw-------  2.0 unx    45031 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/mistral.py
 -rw-------  2.0 unx    27294 b- defN 24-Apr-23 15:07 ipex_llm/transformers/models/mixtral.py
 -rw-------  2.0 unx     9540 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mpt.py
 -rw-------  2.0 unx     7668 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/phi.py
--rw-------  2.0 unx     7835 b- defN 24-Apr-24 15:07 ipex_llm/transformers/models/phi3.py
+-rw-------  2.0 unx     9210 b- defN 24-May-07 15:07 ipex_llm/transformers/models/phi3.py
 -rw-------  2.0 unx     6268 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/phixtral.py
 -rw-------  2.0 unx    32251 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/qwen.py
 -rw-------  2.0 unx    32651 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/qwen2.py
 -rw-------  2.0 unx    38484 b- defN 24-Apr-26 15:08 ipex_llm/transformers/models/qwen2_moe.py
 -rw-------  2.0 unx    11832 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen_vl.py
 -rw-------  2.0 unx     6135 b- defN 24-Mar-29 11:38 ipex_llm/transformers/models/rwkv4.py
 -rw-------  2.0 unx    10722 b- defN 24-Apr-09 15:06 ipex_llm/transformers/models/rwkv5.py
@@ -176,15 +177,15 @@
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
 -rw-------  2.0 unx    18514 b- defN 24-Apr-26 15:08 ipex_llm/vllm/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
 -rw-------  2.0 unx     5941 b- defN 24-Apr-26 15:08 ipex_llm/vllm/engine/engine.py
 -rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240506.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240506.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     5125 b- defN 24-May-06 15:07 ipex_llm-2.1.0b20240506.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-May-06 15:07 ipex_llm-2.1.0b20240506.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-May-06 15:07 ipex_llm-2.1.0b20240506.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-May-06 15:07 ipex_llm-2.1.0b20240506.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    17824 b- defN 24-May-06 15:07 ipex_llm-2.1.0b20240506.dist-info/RECORD
-188 files, 12953031 bytes uncompressed, 5282015 bytes compressed:  59.2%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240507.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240507.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     5125 b- defN 24-May-07 15:08 ipex_llm-2.1.0b20240507.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-07 15:08 ipex_llm-2.1.0b20240507.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-07 15:08 ipex_llm-2.1.0b20240507.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-07 15:08 ipex_llm-2.1.0b20240507.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17920 b- defN 24-May-07 15:08 ipex_llm-2.1.0b20240507.dist-info/RECORD
+189 files, 12984379 bytes uncompressed, 5288059 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -414,14 +414,17 @@
 
 Filename: ipex_llm/transformers/models/chatglm2.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/chatglm2_32k.py
 Comment: 
 
+Filename: ipex_llm/transformers/models/cohere.py
+Comment: 
+
 Filename: ipex_llm/transformers/models/decilm.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/falcon.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/gemma.py
@@ -537,29 +540,29 @@
 
 Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240506.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240507.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240506.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240507.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240506.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240507.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240506.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240507.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240506.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240507.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240506.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240507.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240506.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240507.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/llm_patching.py

```diff
@@ -13,14 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import transformers
 import importlib
 import sys
+from packaging import version
+
 from ipex_llm.utils.common import invalidInputError
 from enum import Enum
 
 bigdl_patched = None  # None or 'Train' or 'Inference'
 attrs = []
 
 
@@ -53,20 +55,22 @@
         import_peft_check = 'peft' in sys.modules or 'peft.utils' in sys.modules or \
             'peft.tuners' in sys.modules or 'peft.mapping' in sys.modules
         invalidInputError(not import_peft_check,
                           'llm_patch() should be called at the beginning of your code.')
         import peft
         from ipex_llm.transformers.qlora import get_peft_model, prepare_model_for_kbit_training,\
             LoraConfig, TrainingArguments
+        peft_version = peft.__version__
         replace_attr(transformers, "TrainingArguments", TrainingArguments)
         get_peft_model_original = getattr(peft, "get_peft_model")
         replace_attr(peft, "get_peft_model", get_peft_model)
         setattr(peft, "get_peft_model_original", get_peft_model_original)
         replace_attr(peft, "prepare_model_for_kbit_training", prepare_model_for_kbit_training)
-        replace_attr(peft, "prepare_model_for_int8_training", prepare_model_for_kbit_training)
+        if version.parse(peft_version) <= version.parse("0.5.0"):
+            replace_attr(peft, "prepare_model_for_int8_training", prepare_model_for_kbit_training)
         replace_attr(peft, "LoraConfig", LoraConfig)
         bigdl_patched = 'Train'
 
 
 def llm_unpatch():
     '''
     llm_unpatch is an reverse function to llm_patch.
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   180005634:	add    %ecx,%esi
-   180005636:	cmp    %ah,0x0(%rsi)
+   180005634:	pop    %rbx
+   180005635:	rex.XB cmp 0x0(%r14),%spl
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
 start address 0x00000001800551e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055800
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000551e8
@@ -111728,17 +111728,16 @@
    18005e7fa:	add    $0x180,%eax
    18005e7ff:	add    %dh,0x76(%rax)
    18005e802:	add    $0x180,%eax
    18005e807:	add    %bh,0x76(%rax)
    18005e80a:	add    $0x180,%eax
    18005e80f:	add    %al,(%rax)
    18005e811:	add    %al,(%rax)
-   18005e813:	add    %al,(%rbx)
-   18005e815:	int1
-   18005e816:	cmp    %ah,0x0(%rsi)
+   18005e813:	add    %bl,0x43(%rbx)
+   18005e816:	cmp    0x0(%rsi),%ah
    18005e819:	add    %al,(%rax)
    18005e81b:	add    %cl,0x50000000(%rip)        # 0x1d005e821
    18005e821:	add    (%rax),%eax
    18005e823:	add    %ah,(%rax)
    18005e825:	repnz add $0x5de2000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   1800049d4:	add    %ecx,%esi
-   1800049d6:	cmp    %ah,0x0(%rsi)
+   1800049d4:	pop    %rbx
+   1800049d5:	rex.XB cmp 0x0(%r14),%spl
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
 start address 0x000000018005c948
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:02:28 2024
+Time/Date		Tue May  7 15:06:04 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d200
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c948
@@ -123136,16 +123136,16 @@
    1800660bd:	add    %al,(%rax)
    1800660bf:	add    %bh,0x18005f6(%rax)
    1800660c5:	add    %al,(%rax)
    1800660c7:	add    %al,%al
    1800660c9:	testb  $0x0,0x180(%rip)        # 0x180066250
    1800660d0:	add    %al,(%rax)
    1800660d2:	add    %al,(%rax)
-   1800660d4:	add    $0xf1,%al
-   1800660d6:	cmp    %ah,0x0(%rsi)
+   1800660d4:	pop    %rsp
+   1800660d5:	rex.XB cmp 0x0(%r14),%spl
    1800660d9:	add    %al,(%rax)
    1800660db:	add    %cl,0x50000000(%rip)        # 0x1d00660e1
    1800660e1:	add    (%rax),%eax
    1800660e3:	add    %al,0x53040006(,%rbp,2)
    1800660ea:	(bad)
 	...
    1800660ff:	add    %bh,0x70(%rax)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b148
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:03:29 2024
+Time/Date		Tue May  7 15:07:10 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b600
 SizeOfInitializedData	00000000000bf800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b148
@@ -117188,16 +117188,15 @@
    18006472a:	add    $0x180,%eax
    18006472f:	add    %dh,-0x2a(%rax)
    180064732:	add    $0x180,%eax
    180064737:	add    %bh,-0x2a(%rax)
    18006473a:	add    $0x180,%eax
    18006473f:	add    %al,(%rax)
    180064741:	add    %al,(%rax)
-   180064743:	add    %al,-0xf(%rcx)
-   180064746:	cmp    %ah,0x0(%rsi)
+   180064743:	add    %bl,0x663a43(%rsi)
    180064749:	add    %al,(%rax)
    18006474b:	add    %cl,0x50000000(%rip)        # 0x1d0064751
    180064751:	add    (%rax),%eax
    180064753:	add    %ah,(%rax)
    180064755:	push   %rcx
    180064756:	(bad)
    180064757:	add    %ah,(%rax)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800553f8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:04:25 2024
+Time/Date		Tue May  7 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055a00
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000553f8
@@ -111831,16 +111831,15 @@
    18005e7da:	add    $0x180,%eax
    18005e7df:	add    %dh,0x76(%rax)
    18005e7e2:	add    $0x180,%eax
    18005e7e7:	add    %bh,0x76(%rax)
    18005e7ea:	add    $0x180,%eax
    18005e7ef:	add    %al,(%rax)
    18005e7f1:	add    %al,(%rax)
-   18005e7f3:	add    %bh,-0xf(%rcx)
-   18005e7f6:	cmp    %ah,0x0(%rsi)
+   18005e7f3:	add    %cl,0x663a42(%rcx)
    18005e7f9:	add    %al,(%rax)
    18005e7fb:	add    %cl,0x50000000(%rip)        # 0x1d005e801
    18005e801:	add    (%rax),%eax
    18005e803:	add    %ah,(%rax)
    18005e805:	repnz add $0x5e02000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062938
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:03:30 2024
+Time/Date		Tue May  7 15:07:11 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062938
@@ -128639,16 +128639,16 @@
    18006bff7:	add    %al,%al
    18006bff9:	push   %rsi
    18006bffa:	(bad)
    18006bffb:	addb   $0x0,(%rcx)
    18006bffe:	add    %al,(%rax)
    18006c000:	add    %al,(%rax)
    18006c002:	add    %al,(%rax)
-   18006c004:	rex.X int1
-   18006c006:	cmp    %ah,0x0(%rsi)
+   18006c004:	lahf
+   18006c005:	rex.XB cmp 0x0(%r14),%spl
    18006c009:	add    %al,(%rax)
    18006c00b:	add    %cl,0x50000000(%rip)        # 0x1d006c011
    18006c011:	add    (%rax),%eax
    18006c013:	add    %al,-0x4d7bfffa(%rsp,%rcx,8)
    18006c01a:	(bad)
 	...
    18006c07f:	add    %bh,%al
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005cb58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:04:25 2024
+Time/Date		Tue May  7 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d400
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005cb58
@@ -123256,18 +123256,18 @@
    18006609d:	add    %al,(%rax)
    18006609f:	add    %bh,0x18005f6(%rax)
    1800660a5:	add    %al,(%rax)
    1800660a7:	add    %al,%al
    1800660a9:	testb  $0x0,0x180(%rip)        # 0x180066230
    1800660b0:	add    %al,(%rax)
    1800660b2:	add    %al,(%rax)
-   1800660b4:	jns    0x1800660a7
-   1800660b6:	cmp    %ah,0x0(%rsi)
-   1800660b9:	add    %al,(%rax)
-   1800660bb:	add    %cl,0x50000000(%rip)        # 0x1d00660c1
+   1800660b4:	mov    0x3a(%rdx),%al
+   1800660b7:	data16 add %al,(%rax)
+   1800660ba:	add    %al,(%rax)
+   1800660bc:	or     $0x50000000,%eax
    1800660c1:	add    (%rax),%eax
    1800660c3:	add    %al,0x55040006(,%rbp,2)
    1800660ca:	(bad)
 	...
    1800660ff:	add    %bh,0x70(%rax)
    180066102:	(bad)
    180066103:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180061648
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:03:30 2024
+Time/Date		Tue May  7 15:07:10 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061e00
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000061648
@@ -127298,16 +127298,16 @@
    18006a0d6:	add    %al,(%rax)
    18006a0d8:	shlb   $1,(%rsi)
    18006a0da:	(bad)
    18006a0db:	addb   $0x0,(%rcx)
    18006a0de:	add    %al,(%rax)
    18006a0e0:	add    %al,(%rax)
    18006a0e2:	add    %al,(%rax)
-   18006a0e4:	rex.X int1
-   18006a0e6:	cmp    %ah,0x0(%rsi)
+   18006a0e4:	sahf
+   18006a0e5:	rex.XB cmp 0x0(%r14),%spl
    18006a0e9:	add    %al,(%rax)
    18006a0eb:	add    %cl,0x50000000(%rip)        # 0x1d006a0f1
    18006a0f1:	add    (%rax),%eax
    18006a0f3:	add    %al,(%rax)
    18006a0f5:	lods   %ds:(%rsi),%eax
    18006a0f6:	(bad)
    18006a0f7:	add    %al,(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b868
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:04:25 2024
+Time/Date		Tue May  7 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c000
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b868
@@ -121930,16 +121930,15 @@
    180064181:	(bad)
    180064182:	add    $0x180,%eax
    180064187:	add    %dl,%al
    180064189:	(bad)
    18006418a:	add    $0x180,%eax
    18006418f:	add    %al,(%rax)
    180064191:	add    %al,(%rax)
-   180064193:	add    %bh,-0xf(%rcx)
-   180064196:	cmp    %ah,0x0(%rsi)
+   180064193:	add    %cl,0x663a42(%rdx)
    180064199:	add    %al,(%rax)
    18006419b:	add    %cl,0x50000000(%rip)        # 0x1d00641a1
    1800641a1:	add    (%rax),%eax
    1800641a3:	add    %al,(%rax)
    1800641a5:	rex.WRX (bad)
    1800641a7:	add    %al,(%rax)
    1800641a9:	rex.X (bad)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180068aa8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:03:29 2024
+Time/Date		Tue May  7 15:07:10 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069000
 SizeOfInitializedData	00000000000c8200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000068aa8
@@ -137914,16 +137914,16 @@
    180071c27:	add    %al,%al
    180071c29:	cmpsb  %es:(%rdi),%ds:(%rsi)
    180071c2a:	(bad)
    180071c2b:	addb   $0x0,(%rcx)
    180071c2e:	add    %al,(%rax)
    180071c30:	add    %al,(%rax)
    180071c32:	add    %al,(%rax)
-   180071c34:	rex.B int1
-   180071c36:	cmp    %ah,0x0(%rsi)
+   180071c34:	sahf
+   180071c35:	rex.XB cmp 0x0(%r14),%spl
    180071c39:	add    %al,(%rax)
    180071c3b:	add    %cl,0x50000000(%rip)        # 0x1d0071c41
    180071c41:	add    (%rax),%eax
    180071c43:	add    %dl,%al
    180071c45:	sub    $0x21d00007,%eax
    180071c4a:	(bad)
 	...
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062d58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:04:25 2024
+Time/Date		Tue May  7 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063400
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062d58
@@ -132533,18 +132533,18 @@
    18006ccf7:	add    %al,%al
    18006ccf9:	push   %rsi
    18006ccfa:	(bad)
    18006ccfb:	addb   $0x0,(%rcx)
    18006ccfe:	add    %al,(%rax)
    18006cd00:	add    %al,(%rax)
    18006cd02:	add    %al,(%rax)
-   18006cd04:	jns    0x18006ccf7
-   18006cd06:	cmp    %ah,0x0(%rsi)
-   18006cd09:	add    %al,(%rax)
-   18006cd0b:	add    %cl,0x50000000(%rip)        # 0x1d006cd11
+   18006cd04:	mov    %eax,0x3a(%rdx)
+   18006cd07:	data16 add %al,(%rax)
+   18006cd0a:	add    %al,(%rax)
+   18006cd0c:	or     $0x50000000,%eax
    18006cd11:	add    (%rax),%eax
    18006cd13:	add    %dl,%al
    18006cd15:	fiadds (%rsi)
    18006cd17:	add    %dl,%al
    18006cd19:	movb   $0x0,(%rsi)
 	...
    18006cd80:	rex loop 0x18006cd89
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   180004a34:	add    %ecx,%esi
-   180004a36:	cmp    %ah,0x0(%rsi)
+   180004a34:	pop    %rbx
+   180004a35:	rex.XB cmp 0x0(%r14),%spl
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
 start address 0x000000018005b658
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:02:28 2024
+Time/Date		Tue May  7 15:06:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005be00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b658
@@ -121795,16 +121795,16 @@
    1800641a1:	(bad)
    1800641a2:	add    $0x180,%eax
    1800641a7:	add    %dl,%al
    1800641a9:	(bad)
    1800641aa:	add    $0x180,%eax
    1800641af:	add    %al,(%rax)
    1800641b1:	add    %al,(%rax)
-   1800641b3:	add    %al,(%rcx,%rsi,8)
-   1800641b6:	cmp    %ah,0x0(%rsi)
+   1800641b3:	add    %bl,0x43(%rbx)
+   1800641b6:	cmp    0x0(%rsi),%ah
    1800641b9:	add    %al,(%rax)
    1800641bb:	add    %cl,0x50000000(%rip)        # 0x1d00641c1
    1800641c1:	add    (%rax),%eax
    1800641c3:	add    %al,(%rax)
    1800641c5:	rex.WRX (bad)
    1800641c7:	add    %al,(%rax)
    1800641c9:	rex (bad)
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   140014ac4:	add    %ecx,%esi
-   140014ac6:	cmp    %ah,0x0(%rsi)
+   140014ac4:	pop    %rbx
+   140014ac5:	rex.XB cmp 0x0(%r14),%spl
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
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May  6 15:04:52 2024
+Time/Date		Tue May  7 15:03:01 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189047,17 +189047,17 @@
    140093ee5:	add    %al,(%rax)
    140093ee7:	add    %al,(%rax)
    140093ee9:	cltd
    140093eea:	or     %al,0x1(%rax)
    140093eed:	add    %al,(%rax)
    140093eef:	add    %al,(%rax)
    140093ef1:	add    %al,(%rax)
-   140093ef3:	add    %dl,0x6638(%rcx,%rsi,8)
-   140093efa:	add    %al,(%rax)
-   140093efc:	or     $0xcc000000,%eax
+   140093ef3:	add    %ah,0x663a42(%rbp)
+   140093ef9:	add    %al,(%rax)
+   140093efb:	add    %cl,-0x34000000(%rip)        # 0x10c093f01
    140093f01:	add    (%rax),%eax
    140093f03:	add    %dl,-0x6ffff68d(%rax)
    140093f09:	movsxd (%rcx),%ecx
 	...
    140093f7f:	add    %al,0x1400977(%rax)
    140093f85:	add    %al,(%rax)
    140093f87:	add    %al,-0x61(%rbp)
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   140013ef4:	add    %ecx,%esi
-   140013ef6:	cmp    %ah,0x0(%rsi)
+   140013ef4:	pop    %rbx
+   140013ef5:	rex.XB cmp 0x0(%r14),%spl
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   140013fc4:	add    %ecx,%esi
-   140013fc6:	cmp    %ah,0x0(%rsi)
+   140013fc4:	pop    %rbx
+   140013fc5:	rex.XB cmp 0x0(%r14),%spl
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
 
-Time/Date		Mon May  6 15:02:28 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   14001f123:	add    %al,(%rcx,%rsi,8)
-   14001f126:	cmp    %ah,0x0(%rsi)
+   14001f123:	add    %bl,0x43(%rbx)
+   14001f126:	cmp    0x0(%rsi),%ah
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32229,17 +32229,16 @@
    1400191e5:	add    %al,(%rax)
    1400191e7:	add    %al,(%rax)
    1400191e9:	push   %rbp
    1400191ea:	add    %eax,0x1(%rax)
    1400191ed:	add    %al,(%rax)
    1400191ef:	add    %al,(%rax)
    1400191f1:	add    %al,(%rax)
-   1400191f3:	add    %al,(%rbx)
-   1400191f5:	int1
-   1400191f6:	cmp    %ah,0x0(%rsi)
+   1400191f3:	add    %bl,0x43(%rbx)
+   1400191f6:	cmp    0x0(%rsi),%ah
    1400191f9:	add    %al,(%rax)
    1400191fb:	add    %cl,0x20000000(%rip)        # 0x160019201
    140019201:	add    (%rax),%eax
    140019203:	add    %dh,%al
    140019205:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
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
 
-Time/Date		Mon May  6 15:04:25 2024
+Time/Date		Tue May  7 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32355,16 +32355,15 @@
    1400191c5:	add    %al,(%rax)
    1400191c7:	add    %al,(%rax)
    1400191c9:	push   %rbp
    1400191ca:	add    %eax,0x1(%rax)
    1400191cd:	add    %al,(%rax)
    1400191cf:	add    %al,(%rax)
    1400191d1:	add    %al,(%rax)
-   1400191d3:	add    %bh,-0xf(%rcx)
-   1400191d6:	cmp    %ah,0x0(%rsi)
+   1400191d3:	add    %cl,0x663a42(%rcx)
    1400191d9:	add    %al,(%rax)
    1400191db:	add    %cl,0x20000000(%rip)        # 0x1600191e1
    1400191e1:	add    (%rax),%eax
    1400191e3:	add    %dh,-0x5f(%rax)
    1400191e6:	add    %eax,(%rax)
    1400191e8:	jo     0x14001917b
    1400191ea:	add    %eax,(%rax)
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:02 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27178,17 +27178,16 @@
    140015fe0:	push   $0x1400123
    140015fe5:	add    %al,(%rax)
    140015fe7:	add    %dh,0x23(%rax)
    140015fea:	add    %eax,0x1(%rax)
    140015fed:	add    %al,(%rax)
    140015fef:	add    %al,(%rax)
    140015ff1:	add    %al,(%rax)
-   140015ff3:	add    %al,(%rbx)
-   140015ff5:	int1
-   140015ff6:	cmp    %ah,0x0(%rsi)
+   140015ff3:	add    %bl,0x43(%rdx)
+   140015ff6:	cmp    0x0(%rsi),%ah
    140015ff9:	add    %al,(%rax)
    140015ffb:	add    %cl,-0x70000000(%rip)        # 0xd0016001
    140016001:	add    (%rax),%eax
    140016003:	add    %ch,%al
    140016005:	add    %eax,%gs:(%rax)
    140016008:	call   0x140016160
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
 
-Time/Date		Mon May  6 15:04:25 2024
+Time/Date		Tue May  7 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27305,16 +27305,15 @@
    140015fc0:	push   $0x1400123
    140015fc5:	add    %al,(%rax)
    140015fc7:	add    %dh,0x23(%rax)
    140015fca:	add    %eax,0x1(%rax)
    140015fcd:	add    %al,(%rax)
    140015fcf:	add    %al,(%rax)
    140015fd1:	add    %al,(%rax)
-   140015fd3:	add    %bh,-0xf(%rcx)
-   140015fd6:	cmp    %ah,0x0(%rsi)
+   140015fd3:	add    %cl,0x663a42(%rcx)
    140015fd9:	add    %al,(%rax)
    140015fdb:	add    %cl,-0x70000000(%rip)        # 0xd0015fe1
    140015fe1:	add    (%rax),%eax
    140015fe3:	add    %ch,0x65(%rax)
    140015fe6:	add    %eax,(%rax)
    140015fe8:	push   $0x155
 	...
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:02 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28462,17 +28462,16 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %al,(%rbx)
-   1400170e5:	int1
-   1400170e6:	cmp    %ah,0x0(%rsi)
+   1400170e3:	add    %bl,0x43(%rdx)
+   1400170e6:	cmp    0x0(%rsi),%ah
    1400170e9:	add    %al,(%rax)
    1400170eb:	add    %cl,-0x70000000(%rip)        # 0xd00170f1
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rdx,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
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
 
-Time/Date		Mon May  6 15:04:24 2024
+Time/Date		Tue May  7 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28607,16 +28607,15 @@
    1400170ad:	add    %al,(%rax)
    1400170af:	add    %cl,0x1400133(%rax)
    1400170b5:	add    %al,(%rax)
    1400170b7:	add    %dl,0x1400133(%rax)
    1400170bd:	add    %al,(%rax)
    1400170bf:	add    %al,(%rax)
    1400170c1:	add    %al,(%rax)
-   1400170c3:	add    %bh,-0xf(%rax)
-   1400170c6:	cmp    %ah,0x0(%rsi)
+   1400170c3:	add    %cl,0x663a42(%rcx)
    1400170c9:	add    %al,(%rax)
    1400170cb:	add    %cl,-0x70000000(%rip)        # 0xd00170d1
    1400170d1:	add    (%rax),%eax
    1400170d3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170d7:	add    %ch,0x1(%rsi,%riz,2)
 	...
    1400170ff:	add    %ah,(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May  6 15:02:28 2024
+Time/Date		Tue May  7 15:06:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32576,16 +32576,16 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %al,(%rcx,%rsi,8)
-   140019316:	cmp    %ah,0x0(%rsi)
+   140019313:	add    %bl,0x43(%rbx)
+   140019316:	cmp    0x0(%rsi),%ah
    140019319:	add    %al,(%rax)
    14001931b:	add    %cl,0x20000000(%rip)        # 0x160019321
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May  6 15:04:25 2024
+Time/Date		Tue May  7 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32701,16 +32701,15 @@
    1400192e5:	add    %al,(%rax)
    1400192e7:	add    %al,(%rax)
    1400192e9:	push   %rbp
    1400192ea:	add    %eax,0x1(%rax)
    1400192ed:	add    %al,(%rax)
    1400192ef:	add    %al,(%rax)
    1400192f1:	add    %al,(%rax)
-   1400192f3:	add    %bh,-0xf(%rcx)
-   1400192f6:	cmp    %ah,0x0(%rsi)
+   1400192f3:	add    %cl,0x663a42(%rcx)
    1400192f9:	add    %al,(%rax)
    1400192fb:	add    %cl,0x20000000(%rip)        # 0x160019301
    140019301:	add    (%rax),%eax
    140019303:	add    %bh,%ah
    140019305:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
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
 
-Time/Date		Mon May  6 15:02:27 2024
+Time/Date		Tue May  7 15:06:03 2024
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
-   180004604:	add    %ecx,%esi
-   180004606:	cmp    %ah,0x0(%rsi)
+   180004604:	pop    %rbx
+   180004605:	rex.XB cmp 0x0(%r14),%spl
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
 start address 0x0000000180062b48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  6 15:02:28 2024
+Time/Date		Tue May  7 15:06:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062b48
@@ -132428,16 +132428,16 @@
    18006cd17:	add    %al,%al
    18006cd19:	push   %rsi
    18006cd1a:	(bad)
    18006cd1b:	addb   $0x0,(%rcx)
    18006cd1e:	add    %al,(%rax)
    18006cd20:	add    %al,(%rax)
    18006cd22:	add    %al,(%rax)
-   18006cd24:	add    $0xf1,%al
-   18006cd26:	cmp    %ah,0x0(%rsi)
+   18006cd24:	pop    %rbx
+   18006cd25:	rex.XB cmp 0x0(%r14),%spl
    18006cd29:	add    %al,(%rax)
    18006cd2b:	add    %cl,0x50000000(%rip)        # 0x1d006cd31
    18006cd31:	add    (%rax),%eax
    18006cd33:	add    %dl,%al
    18006cd35:	fiadds (%rsi)
    18006cd37:	add    %dl,%al
    18006cd39:	(bad)
```

## ipex_llm/serving/fastchat/ipex_llm_worker.py

```diff
@@ -15,26 +15,30 @@
 #
 
 """
 A model worker that executes the model based on BigDL-LLM.
 Relies on load_model method
 """
 
+import torch
+import torch.nn.functional as F
+import gc
 import argparse
 import asyncio
 import atexit
 import json
 from typing import List
 import uuid
 from threading import Thread
 from fastapi import FastAPI, Request, BackgroundTasks
 from fastapi.concurrency import run_in_threadpool
 from fastapi.responses import StreamingResponse, JSONResponse
 import uvicorn
 
+from fastchat.constants import ErrorCode, SERVER_ERROR_MSG
 from fastchat.serve.base_model_worker import BaseModelWorker
 from fastchat.serve.model_worker import (
     logger,
     worker_id,
 )
 from fastchat.serve.base_model_worker import (
     create_background_tasks,
@@ -59,14 +63,15 @@
         model_names: List[str],
         limit_worker_concurrency: int,
         conv_template: str = None,
         load_in_low_bit: str = "sym_int4",
         device: str = "cpu",
         no_register: bool = False,
         trust_remote_code: bool = False,
+        embed_in_truncate: bool = False,
         speculative: bool = False,
         stream_interval: int = 4,
     ):
         super().__init__(
             controller_addr,
             worker_addr,
             worker_id,
@@ -89,17 +94,166 @@
         self.device = device
         self.speculative = speculative
         self.model, self.tokenizer = load_model(
             model_path, device, self.load_in_low_bit, trust_remote_code, speculative
         )
         self.stream_interval = stream_interval
         self.context_len = get_context_length(self.model.config)
+        self.embed_in_truncate = embed_in_truncate
         if not no_register:
             self.init_heart_beat()
 
+    def __process_embed_chunk(self, input_ids, attention_mask, **model_type_dict):
+        if model_type_dict.get("is_bert"):
+            model_output = self.model(input_ids)
+            if model_type_dict.get("is_robert"):
+                data = model_output.last_hidden_state
+            else:
+                data = model_output[0]
+        elif model_type_dict.get("is_t5"):
+            model_output = self.model(input_ids, decoder_input_ids=input_ids)
+            data = model_output.encoder_last_hidden_state
+        else:
+            model_output = self.model(input_ids, output_hidden_states=True)
+            if model_type_dict.get("is_chatglm"):
+                data = model_output.hidden_states[-1].transpose(0, 1)
+            else:
+                data = model_output.hidden_states[-1]
+
+        if hasattr(self.model, "use_cls_pooling") and self.model.use_cls_pooling:
+            sum_embeddings = data[:, 0]
+        else:
+            mask = attention_mask.unsqueeze(-1).expand(data.size()).float()
+            masked_embeddings = data * mask
+            sum_embeddings = torch.sum(masked_embeddings, dim=1)
+        token_num = torch.sum(attention_mask).item()
+
+        return sum_embeddings, token_num
+
+    @torch.inference_mode()
+    def get_embeddings(self, params):
+        self.call_ct += 1
+
+        try:
+            # Get tokenizer
+            tokenizer = self.tokenizer
+            ret = {"embedding": [], "token_num": 0}
+
+            # Based on conditions of different model_type
+            model_type_dict = {
+                "is_llama": "llama" in str(type(self.model)),
+                "is_t5": "t5" in str(type(self.model)),
+                "is_chatglm": "chatglm" in str(type(self.model)),
+                "is_bert": "bert" in str(type(self.model)),
+                "is_robert": "robert" in str(type(self.model)),
+            }
+
+            if self.embed_in_truncate:
+                encoding = tokenizer.batch_encode_plus(
+                    params["input"],
+                    padding=True,
+                    truncation="longest_first",
+                    return_tensors="pt",
+                    max_length=self.context_len,
+                )
+            else:
+                encoding = tokenizer.batch_encode_plus(
+                    params["input"], padding=True, return_tensors="pt"
+                )
+            input_ids = encoding["input_ids"].to(self.device)
+            # Check if we need attention_mask or not.
+            attention_mask = input_ids != tokenizer.pad_token_id
+
+            base64_encode = params.get("encoding_format", None)
+
+            if self.embed_in_truncate:
+                embedding, token_num = self.__process_embed_chunk(
+                    input_ids, attention_mask, **model_type_dict
+                )
+                if (
+                    not hasattr(self.model, "use_cls_pooling")
+                    or not self.model.use_cls_pooling
+                ):
+                    embedding = embedding / token_num
+                normalized_embeddings = F.normalize(embedding, p=2, dim=1)
+                ret["token_num"] = token_num
+            else:
+                all_embeddings = []
+                all_token_num = 0
+                for i in range(0, input_ids.size(1), self.context_len):
+                    chunk_input_ids = input_ids[:, i:i + self.context_len]
+                    chunk_attention_mask = attention_mask[:, i:i + self.context_len]
+
+                    # add cls token and mask to get cls embedding
+                    if (
+                        hasattr(self.model, "use_cls_pooling")
+                        and self.model.use_cls_pooling
+                    ):
+                        cls_tokens = (
+                            torch.zeros(
+                                (chunk_input_ids.size(0), 1),
+                                dtype=chunk_input_ids.dtype,
+                                device=chunk_input_ids.device,
+                            )
+                            + tokenizer.cls_token_id
+                        )
+                        chunk_input_ids = torch.cat(
+                            [cls_tokens, chunk_input_ids], dim=-1
+                        )
+                        mask = torch.ones(
+                            (chunk_attention_mask.size(0), 1),
+                            dtype=chunk_attention_mask.dtype,
+                            device=chunk_attention_mask.device,
+                        )
+                        chunk_attention_mask = torch.cat(
+                            [mask, chunk_attention_mask], dim=-1
+                        )
+
+                    chunk_embeddings, token_num = self.__process_embed_chunk(
+                        chunk_input_ids, chunk_attention_mask, **model_type_dict
+                    )
+                    if (
+                        hasattr(self.model, "use_cls_pooling")
+                        and self.model.use_cls_pooling
+                    ):
+                        all_embeddings.append(chunk_embeddings * token_num)
+                    else:
+                        all_embeddings.append(chunk_embeddings)
+                    all_token_num += token_num
+
+                all_embeddings_tensor = torch.stack(all_embeddings)
+                embedding = torch.sum(all_embeddings_tensor, dim=0) / all_token_num
+                normalized_embeddings = F.normalize(embedding, p=2, dim=1)
+
+                ret["token_num"] = all_token_num
+
+            if base64_encode == "base64":
+                out_embeddings = self.__encode_base64(normalized_embeddings)
+            else:
+                out_embeddings = normalized_embeddings.tolist()
+            ret["embedding"] = out_embeddings
+
+            gc.collect()
+            torch.cuda.empty_cache()
+            if self.device == "xpu":
+                torch.xpu.empty_cache()
+            if self.device == "npu":
+                torch.npu.empty_cache()
+        except torch.cuda.OutOfMemoryError as e:
+            ret = {
+                "text": f"{SERVER_ERROR_MSG}\n\n({e})",
+                "error_code": ErrorCode.CUDA_OUT_OF_MEMORY,
+            }
+        except (ValueError, RuntimeError) as e:
+            ret = {
+                "text": f"{SERVER_ERROR_MSG}\n\n({e})",
+                "error_code": ErrorCode.INTERNAL_ERROR,
+            }
+        return ret
+
     def generate_stream_gate(self, params):
         self.call_ct += 1
         # context length is self.context_length
         prompt = params["prompt"]
         temperature = float(params.get("temperature", 1.0))
         do_sample = bool(params.get("do_sample", False))
         repetition_penalty = float(params.get("repetition_penalty", 1.0))
@@ -273,14 +427,23 @@
 
 
 @app.post("/worker_get_status")
 async def api_get_status(request: Request):
     return worker.get_status()
 
 
+@app.post("/worker_get_embeddings")
+async def api_get_embeddings(request: Request):
+    params = await request.json()
+    await acquire_worker_semaphore()
+    embedding = worker.get_embeddings(params)
+    release_worker_semaphore()
+    return JSONResponse(content=embedding)
+
+
 @app.post("/count_token")
 async def api_count_token(request: Request):
     params = await request.json()
     return worker.count_token(params)
 
 
 @app.post("/worker_get_conv_template")
@@ -328,24 +491,26 @@
     parser.add_argument(
         "--trust-remote-code",
         action="store_true",
         default=False,
         help="Trust remote code (e.g., from HuggingFace) when"
         "downloading the model and tokenizer.",
     )
+    parser.add_argument("--embed-in-truncate", action="store_true")
 
     args = parser.parse_args()
     worker = BigDLLLMWorker(
         args.controller_address,
         args.worker_address,
         worker_id,
         args.model_path,
         args.model_names,
         args.limit_worker_concurrency,
         args.conv_template,
         args.low_bit,
         args.device,
         args.no_register,
         args.trust_remote_code,
+        args.embed_in_truncate,
         args.speculative,
     )
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

## ipex_llm/transformers/convert.py

```diff
@@ -45,26 +45,39 @@
 from ipex_llm.ggml.quantize import ggml_tensor_qtype
 from .utils import logger, get_cur_qtype_and_imatrix
 from typing import Union
 import numpy as np
 import os
 from ipex_llm.utils.common import invalidInputError
 from typing import List, Optional, Tuple, Union
+import subprocess
+import sys
+
+_IS_VLLM_AVAILABLE = None
 
 
 def is_auto_gptq_available():
     return importlib.util.find_spec("auto_gptq") is not None
 
 
 def is_auto_awq_available():
     return importlib.util.find_spec("awq") is not None
 
 
 def is_vllm_available():
-    return importlib.util.find_spec("vllm") is not None
+    global _IS_VLLM_AVAILABLE
+    if _IS_VLLM_AVAILABLE is not None:
+        return _IS_VLLM_AVAILABLE
+    reqs = subprocess.check_output([sys.executable, '-m', 'pip', 'list'])
+    installed_packages = [r.decode().split('  ')[0] for r in reqs.split()]
+    if 'vllm' in installed_packages:
+        _IS_VLLM_AVAILABLE = True
+    else:
+        _IS_VLLM_AVAILABLE = False
+    return _IS_VLLM_AVAILABLE
 
 
 def is_torch_distributed_initialized():
     return torch.distributed.is_initialized()
 
 
 def is_module_in_classes(module, classes):
@@ -1265,14 +1278,32 @@
                         qwen2moe_moeblock_forward)
         convert_forward(model,
                         module.Qwen2MoeMLP,
                         llama_mlp_forward)
         convert_forward(model,
                         module.Qwen2MoeAttention,
                         qwen2moe_attention_forward)
+    elif model.config.model_type == "cohere":
+        # for CohereForAI/c4ai-command-r-v01
+        modeling_module_name = model.__class__.__module__
+        module = importlib.import_module(modeling_module_name)
+        from ipex_llm.transformers.models.cohere import cohere_attention_forward
+        from ipex_llm.transformers.models.cohere import cohere_model_forward
+        convert_forward(model,
+                        module.CohereModel,
+                        cohere_model_forward)
+        convert_forward(model,
+                        module.CohereAttention,
+                        cohere_attention_forward)
+        convert_forward(model,
+                        module.CohereLayerNorm,
+                        llama_rms_norm_forward)
+        convert_forward(model,
+                        module.CohereMLP,
+                        llama_mlp_forward)
     elif model.config.model_type == "aquila":
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
         from ipex_llm.transformers.models.aquila import aquila_attention_forward
         convert_forward(model,
                         module.AquilaAttention,
                         aquila_attention_forward
```

## ipex_llm/transformers/qlora.py

```diff
@@ -46,188 +46,199 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 import logging
-from torch.nn import Linear, Embedding
+from torch.nn import Linear, Embedding, Module
 from ipex_llm.transformers.low_bit_linear import LowBitLinear, BF16Linear, get_qk_size
 from peft.tuners.lora import LoraLayer
+from typing import Any, Optional, Union
 from ipex_llm.utils.common import invalidInputError
 from ipex_llm.transformers.utils import get_autocast_dtype
 from ipex_llm.ggml.quantize import ggml_tensor_qtype
 import functools
 from ipex_llm.transformers import training_patch
 
 LOG = logging.getLogger("ipex_llm.qlora")
 
 
-class LoraLowBitLinear(LowBitLinear, LoraLayer):
+class LoraLowBitLinear(Module, LoraLayer):
     # Lora implemented in a dense layer
     def __init__(
         self,
+        base_layer,
         adapter_name,
-        in_features,
-        out_features,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         qa_lora: bool = True,
+        # Set this to True if the layer to replace stores weight like (fan_in, fan_out)
+        fan_in_fan_out: bool = False,
+        is_target_conv_1d_layer: bool = False,
+        init_lora_weights: Union[bool, str]=True,
+        use_rslora: bool = False,
+        use_dora: bool = False,
         **kwargs,
     ):
-        LowBitLinear.__init__(
-            self,
-            in_features,
-            out_features,
-            qtype=kwargs.get("qtype"),
-            bias=kwargs.get("bias", True),
-            conver_to_half=False,
-        )
-
+        super().__init__()
         qk_size = get_qk_size(kwargs.get("qtype"))
-        lora_in_features = in_features // qk_size if qa_lora else in_features
-        LoraLayer.__init__(self, in_features=lora_in_features, out_features=out_features)
-
-        # Freezing the pre-trained weight matrix
-        self.weight.requires_grad = False
+        if qa_lora:
+            # qa_lora need to change the in_features of the base_layer
+            in_features = base_layer.in_features
+            base_layer.in_features = in_features // qk_size
+
+        LoraLayer.__init__(self, base_layer, **kwargs)
+
+        self.fan_in_fan_out = fan_in_fan_out
+        self._active_adapter = adapter_name
+        self.update_layer(
+            adapter_name,
+            r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            init_lora_weights=init_lora_weights,
+            use_rslora=use_rslora,
+            use_dora=use_dora,
+        )
+        self.is_target_conv_1d_layer = is_target_conv_1d_layer
 
-        init_lora_weights = kwargs.pop("init_lora_weights", True)
-        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
-        self.active_adapter = adapter_name
         if qa_lora:
             self.qa_pool = torch.nn.AvgPool1d(qk_size)
         else:
             self.qa_pool = torch.nn.Identity()
 
     def forward(self, x: torch.Tensor):
         autocast_dtype = get_autocast_dtype(x)
         if x.device.type == "xpu":
             # force to use bf16 on gpu
             x = x.to(torch.bfloat16)
         elif autocast_dtype is not None:
             x = x.to(autocast_dtype)
-        result = super().forward(x)
+        result = self.base_layer.forward(x)
 
-        if self.disable_adapters or self.active_adapter not in self.lora_A.keys():
+        if self.disable_adapters or self.merged:
             return result
-        elif self.r[self.active_adapter] > 0:
-            result = result.clone()
+        else:
             if autocast_dtype is None and x.device.type == "cpu":
                 expected_dtype = result.dtype
-                x = x.to(self.lora_A[self.active_adapter].weight.dtype)
-                output = (
-                    self.lora_B[self.active_adapter](
-                        self.lora_A[self.active_adapter](
-                            self.lora_dropout[self.active_adapter](self.qa_pool(x)))
-                    ).to(expected_dtype)
-                    * self.scaling[self.active_adapter]
-                )
+                for active_adapter in self.active_adapters:
+                    if active_adapter not in self.lora_A.keys():
+                        continue
+                    x = x.to(self.lora_A[active_adapter].weight.dtype)
+                    lora_A = self.lora_A[active_adapter]
+                    lora_B = self.lora_B[active_adapter]
+                    dropout = self.lora_dropout[active_adapter]
+                    scaling = self.scaling[active_adapter]
+                    result += lora_B(lora_A(dropout(self.qa_pool(x)))).to(expected_dtype) * scaling
             else:
-                output = (
-                    self.lora_B[self.active_adapter](
-                        self.lora_A[self.active_adapter](
-                            self.lora_dropout[self.active_adapter](self.qa_pool(x)))
-                    )
-                    * self.scaling[self.active_adapter]
-                )
-            result += output
+                for active_adapter in self.active_adapters:
+                    if active_adapter not in self.lora_A.keys():
+                        continue
+                    lora_A = self.lora_A[active_adapter]
+                    lora_B = self.lora_B[active_adapter]
+                    dropout = self.lora_dropout[active_adapter]
+                    scaling = self.scaling[active_adapter]
+                    result += lora_B(lora_A(dropout(self.qa_pool(x)))) * scaling
         return result
 
 
-class LoraBF16Linear(BF16Linear, LoraLayer):
+class LoraBF16Linear(Module, LoraLayer):
     # Lora implemented in a dense layer
     def __init__(
         self,
+        base_layer,
         adapter_name,
-        in_features,
-        out_features,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
+        # Set this to True if the layer to replace stores weight like (fan_in, fan_out)
+        fan_in_fan_out: bool = False,
+        is_target_conv_1d_layer: bool = False,
+        init_lora_weights: Union[bool, str]=True,
+        use_rslora: bool = False,
+        use_dora: bool = False,
         **kwargs,
     ):
-        BF16Linear.__init__(
-            self,
-            in_features,
-            out_features,
-            bias=kwargs.get("bias", True),
-            compute_dtype=torch.bfloat16,
-        )
-
-        LoraLayer.__init__(self, in_features=in_features, out_features=out_features)
-
-        # Freezing the pre-trained weight matrix
-        self.weight.requires_grad = False
+        super().__init__()
+        LoraLayer.__init__(self, base_layer, **kwargs)
 
-        init_lora_weights = kwargs.pop("init_lora_weights", True)
-        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
-        self.active_adapter = adapter_name
+        self.fan_in_fan_out = fan_in_fan_out
+        self._active_adapter = adapter_name
+        self.update_layer(
+            adapter_name,
+            r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            init_lora_weights=init_lora_weights,
+            use_rslora=use_rslora,
+            use_dora=use_dora,
+        )
+        self.is_target_conv_1d_layer = is_target_conv_1d_layer
 
     def forward(self, x: torch.Tensor):
         autocast_dtype = get_autocast_dtype(x)
         if x.device.type == "xpu":
             # force to use bf16 on gpu
             x = x.to(torch.bfloat16)
         elif autocast_dtype is not None:
             x = x.to(autocast_dtype)
-        result = super().forward(x)
+        result = self.base_layer.forward(x)
 
-        if self.disable_adapters or self.active_adapter not in self.lora_A.keys():
+        if self.disable_adapters or self.merged:
             return result
-        elif self.r[self.active_adapter] > 0:
-            result = result.clone()
+        else:
             if autocast_dtype is None and x.device.type == "cpu":
                 expected_dtype = result.dtype
-                x = x.to(self.lora_A[self.active_adapter].weight.dtype)
-                output = (
-                    self.lora_B[self.active_adapter](
-                        self.lora_A[self.active_adapter](
-                            self.lora_dropout[self.active_adapter](x))
-                    ).to(expected_dtype)
-                    * self.scaling[self.active_adapter]
-                )
+                for active_adapter in self.active_adapters:
+                    if active_adapter not in self.lora_A.keys():
+                        continue
+                    x = x.to(self.lora_A[active_adapter].weight.dtype)
+                    lora_A = self.lora_A[active_adapter]
+                    lora_B = self.lora_B[active_adapter]
+                    dropout = self.lora_dropout[active_adapter]
+                    scaling = self.scaling[active_adapter]
+                    result += lora_B(lora_A(dropout(x))).to(expected_dtype) * scaling
             else:
-                output = (
-                    self.lora_B[self.active_adapter](
-                        self.lora_A[self.active_adapter](
-                            self.lora_dropout[self.active_adapter](x))
-                    )
-                    * self.scaling[self.active_adapter]
-                )
-            result += output
+                for active_adapter in self.active_adapters:
+                    if active_adapter not in self.lora_A.keys():
+                        continue
+                    lora_A = self.lora_A[active_adapter]
+                    lora_B = self.lora_B[active_adapter]
+                    dropout = self.lora_dropout[active_adapter]
+                    scaling = self.scaling[active_adapter]
+                    result += lora_B(lora_A(dropout(x))) * scaling
         return result
 
 
 def _create_new_module(create_new_module_func, lora_config, adapter_name, target, **kwargs):
 
     if isinstance(target, LowBitLinear) or isinstance(target, BF16Linear):
         low_bit_kwargs = kwargs.copy()
         bias = low_bit_kwargs.pop("bias", False)
 
         if hasattr(lora_config, "training_mode") and lora_config.training_mode == "lora":
-            new_module = LoraBF16Linear(adapter_name,
-                                        target.in_features,
-                                        target.out_features,
+            new_module = LoraBF16Linear(target,
+                                        adapter_name,
                                         bias=bias,
                                         **low_bit_kwargs)
         else:
             if hasattr(lora_config, "training_mode"):
                 qa_lora = lora_config.training_mode == "qalora"
             else:
                 qa_lora = False
             low_bit_kwargs.update(
                 {
                     "qtype": target.qtype,
                     "qa_lora": qa_lora
                 }
             )
-            new_module = LoraLowBitLinear(adapter_name,
-                                          target.in_features,
-                                          target.out_features,
+            new_module = LoraLowBitLinear(target,
+                                          adapter_name,
                                           bias=bias,
                                           **low_bit_kwargs)
     else:
         new_module = create_new_module_func(lora_config, adapter_name, target, **kwargs)
 
     return new_module
```

## ipex_llm/transformers/models/phi3.py

```diff
@@ -36,15 +36,17 @@
 import warnings
 
 from ipex_llm.transformers.models.utils import (
     rotate_half, should_use_fuse_rope,
     apply_rotary_pos_emb_cache_freq_xpu
 )
 from ipex_llm.transformers.models.utils import mlp_fusion_check, SILU
-from ipex_llm.transformers.kv import DynamicNormalCache
+from ipex_llm.transformers.models.utils import use_new_esimd_sdp_fp16, use_quantize_kv_cache
+from ipex_llm.transformers.models.utils import use_sdp_fp8, restore_fp8_kv_cache
+from ipex_llm.transformers.kv import DynamicNormalCache, DynamicFp8Cache
 
 from typing import Optional, Tuple, List
 from transformers.models.phi.modeling_phi import repeat_kv
 from transformers.cache_utils import Cache
 
 
 def apply_rotary_pos_emb(q, k, cos, sin, position_ids=None, unsqueeze_dim=1):
@@ -89,30 +91,42 @@
         query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
                                                         cos, sin, position_ids)
 
     if past_key_value is not None:
         key_states, value_states = past_key_value.update(key_states, value_states,
                                                          self.layer_idx, None)
 
-    # repeat k/v heads if n_kv_heads < n_heads
-    key_states = repeat_kv(key_states, self.num_key_value_groups)
-    value_states = repeat_kv(value_states, self.num_key_value_groups)
-
-    attn_weights = torch.matmul(query_states,
-                                key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
-
-    if attention_mask is not None:
-        attn_weights = attn_weights + attention_mask
-
-    # upcast attention to fp32
-    attn_weights = torch.nn.functional.softmax(attn_weights, dim=-1,
-                                               dtype=torch.float32).to(value_states.dtype)
-    attn_weights = torch.nn.functional.dropout(attn_weights, p=self.attention_dropout,
-                                               training=self.training)
-    attn_output = torch.matmul(attn_weights, value_states)
+    if (isinstance(past_key_value, DynamicFp8Cache) and
+            use_sdp_fp8(q_len, kv_seq_len, query_states)):
+        import linear_q4_0
+        attn_output = linear_q4_0.sdp_fp8(query_states, key_states, value_states, attention_mask)
+    elif (isinstance(past_key_value, DynamicNormalCache) and
+            use_new_esimd_sdp_fp16(q_len, kv_seq_len, self.head_dim, query_states)):
+        import linear_q4_0
+        attn_output = linear_q4_0.sdp_fp16(query_states, key_states, value_states, attention_mask)
+    else:
+        if isinstance(past_key_value, DynamicFp8Cache):
+            key_states, value_states = restore_fp8_kv_cache(key_states, value_states,
+                                                            query_states.dtype)
+        # repeat k/v heads if n_kv_heads < n_heads
+        key_states = repeat_kv(key_states, self.num_key_value_groups)
+        value_states = repeat_kv(value_states, self.num_key_value_groups)
+
+        attn_weights = torch.matmul(query_states,
+                                    key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
+
+        if attention_mask is not None:
+            attn_weights = attn_weights + attention_mask
+
+        # upcast attention to fp32
+        attn_weights = torch.nn.functional.softmax(attn_weights, dim=-1,
+                                                   dtype=torch.float32).to(value_states.dtype)
+        attn_weights = torch.nn.functional.dropout(attn_weights, p=self.attention_dropout,
+                                                   training=self.training)
+        attn_output = torch.matmul(attn_weights, value_states)
 
     attn_output = attn_output.transpose(1, 2).contiguous()
     attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
 
     attn_output = self.o_proj(attn_output)
 
     if not output_attentions:
@@ -171,16 +185,20 @@
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ):
         # IPEX-LLM OPT: kv cache but no sdp (its head_dim 96, cannot use sdp)
         use_cache = use_cache if use_cache is not None else self.config.use_cache
+        use_quantize_kv = (use_quantize_kv_cache(self.layers[0].mlp.down_proj, input_ids) and
+                           self.config.hidden_size // self.config.num_attention_heads in [64, 128])
         if use_cache:
-            if not isinstance(past_key_values, DynamicNormalCache):
+            if use_quantize_kv and not isinstance(past_key_values, DynamicFp8Cache):
+                past_key_values = DynamicFp8Cache.from_legacy_cache(past_key_values)
+            if not use_quantize_kv and not isinstance(past_key_values, DynamicNormalCache):
                 past_key_values = DynamicNormalCache.from_legacy_cache(past_key_values)
         return origin_model_forward(
             self=self,
             input_ids=input_ids,
             attention_mask=attention_mask,
             position_ids=position_ids,
             past_key_values=past_key_values,
```

## Comparing `ipex_llm-2.1.0b20240506.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240507.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240506.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240507.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240506.dist-info/METADATA` & `ipex_llm-2.1.0b20240507.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240506
+Version: 2.1.0b20240507
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
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240506) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240507) ; extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
 Requires-Dist: numpy (==1.26.4) ; extra == 'llama-index'
 Requires-Dist: sentencepiece ; extra == 'llama-index'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'llama-index'
@@ -51,47 +51,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240506) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240506) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240507) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240507) ; extra == 'xpu'
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
-Requires-Dist: bigdl-core-xe (==2.5.0b20240506) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240506) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240507) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240507) ; (platform_system == "Linux") and extra == 'xpu-2-0'
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
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240506) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240506) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240507) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240507) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240506.dist-info/RECORD` & `ipex_llm-2.1.0b20240507.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ipex_llm/__init__.py,sha256=tNm3iVPD_xcJ9adnPKktX0H6mpR7jqoj4eS8VXTEBg4,1898
 ipex_llm/convert_model.py,sha256=jopEe6wu88ZPZfNFhgnQUu7807iciiWW_EMyTsVni5A,6816
-ipex_llm/llm_patching.py,sha256=nlooh_kPc_WdZCRXMqhMCa7pVIjn1qjt7ci94A6vl-o,3091
+ipex_llm/llm_patching.py,sha256=becMYcawtR8lgl2yeRQhvvX6CLaq09WZGm9dDmLJWL0,3232
 ipex_llm/models.py,sha256=f0nyter0vAUExzdDJZwlRnsieguJYF8ZJoE8WH3zTwg,1177
 ipex_llm/optimize.py,sha256=lqtvg5hCyEXiYlFe80GQcYqnDykKrg21ZmW7wKa4WiA,12404
 ipex_llm/cli/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
 ipex_llm/cli/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
 ipex_llm/cli/prompts/chat-with-llm.txt,sha256=PpSyd4FQQd-T7ptfXL9jZp7dgstevu1fsxWFa0IQ5Oc,216
 ipex_llm/ggml/__init__.py,sha256=FzapYBUiTdZf0LzlN9hfJI-HE1OTi_2dzaYELJ9Mw8s,1272
 ipex_llm/ggml/convert.py,sha256=VLkrgWHwRPW9VpBG1ayHdJVdk7Vs_vvl-s1x9qgQsCk,5417
@@ -38,68 +38,68 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=Vn4UYMHdsdjlHRUIVco7x9QCCZbNYFYwpQeFpgZgFkY,36352
-ipex_llm/libs/bloom.dll,sha256=P4kbWI3sSXrEG2uZVpm_lKvbrGFbZ2Cs8NZlju25VgU,470528
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=MlOX9mlID7pW73Q5MBq_6evqTqCAypxkQI_ms1Hn-Ik,853504
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=UwZ3NqIbZJSSF_SmnaZw2-asaFk2WmOF0I8yl205yGI,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=KQnP2eGGHpWNQyi8FYnkxY0kgcUjKC9xuaZjMHvic5o,844288
-ipex_llm/libs/gptneox-api.dll,sha256=g6bPdmeYR3bsvOnkQmg5Wmc9UXSpONGP-mhQ5GhRzus,24576
-ipex_llm/libs/gptneox.dll,sha256=D5wMxlw1bqDXrouXs9mpcUUQ5e2PBlotSOvOt2JwyFM,530432
-ipex_llm/libs/libbloom_avx.dll,sha256=83nr0RukNfkwnfRuGhdbo-1HAq-QleM2E-GVMgZlDAk,496128
-ipex_llm/libs/libbloom_vnni.dll,sha256=IspTFl-T76gB6qmclpLt0Izg19afqq5CgcMn3BwVZgQ,471040
-ipex_llm/libs/libgptneox_avx.dll,sha256=sn-JeiIhzwIEWqfyZHu2-0qMqHjCLBqQojQk9dkQqZ0,556032
-ipex_llm/libs/libgptneox_vnni.dll,sha256=lZrs6Mz4Ow0l2SS9-FT-NJBeXhOTFeQBwnKp3xlIBsA,530944
-ipex_llm/libs/libllama_avx.dll,sha256=r61xxZNtap5Wkz9tvOAJfUBQ9n_4QjmtpzGJ1EUKbfA,549888
-ipex_llm/libs/libllama_vnni.dll,sha256=YSjTn9dg7tEG2psPKKIcZIe143_0Ff22--jLUfmLY8I,525312
-ipex_llm/libs/libstarcoder_avx.dll,sha256=EZuMibEKSGB7iED0C8mXId7oEoVwUSwecps8-dRGcaU,586752
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=lY4QPhqJp-VXcG5poHpk2uSXzKuzxBlMZas1IJbTq04,561664
-ipex_llm/libs/llama-api.dll,sha256=kiNufl39sANGrY7yfKkzwGGOxZNMASP-q0DeEDTVZE0,25088
-ipex_llm/libs/llama.dll,sha256=ynJxzf-Q7XixkQhFdW_mtnIybIxtEpTZpI2nYwVxEnA,524288
-ipex_llm/libs/main-bloom.exe,sha256=cby_bFtn2k986iJL0QxTM8nzG9RxMApN0lbLUw2KXAc,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=1VPg44Xu1Z3OYcFINiRKg1ivO8JUflfGZgHMvuuO1Qc,726016
-ipex_llm/libs/main-gptneox.exe,sha256=vLZk41KpMJPPpbQGoSiYuB2By84O6jkxphGyUqU7Vjw,98816
-ipex_llm/libs/main-llama.exe,sha256=AACJj4gIGkrSGVAXSR7kvgVtKrcIw0Whh7lTjlxA4ps,99840
-ipex_llm/libs/main-starcoder.exe,sha256=32ktqLKiysVeG6wGNAMzCRgz1qMeomRrqSeUvZFfu6c,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=QmX6_VC1ywJR9NII4kTuN4BOdbVsIkLo-_9DCCT7DJU,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=LOUlS4XbXUFjfm4NlinBzrdwCoNuQCx91e5_EnlfQzg,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=3K8x_v1Zcy7BY0f18OYev-QjdvojtQbyHUDS7v9BxlA,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=eWXP239aah4vF76K1BSDHgJw7LpfjZbtFngBLZnhsK8,104448
-ipex_llm/libs/quantize-llama.exe,sha256=AW0mE_UrTJDYLjEPShhtw90NsAactTMJf1ZOrXtn2qo,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=M7QQIh0G7nWP7wyG5hyGouVCEyzIOSVV-3aF3BtNdb4,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=aHOvJtkYRqOVQel8ZacJxwxGKc6Snr7Fc4HqK3tT8EM,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=0GpsRSOmuh25I4I7ykLtVCdt3Zk1B8CuASoyFOkjjuE,128512
-ipex_llm/libs/starcoder-api.dll,sha256=UHX3QCK4lR3dpRjvI3-1Fq-fnosoPJ2zBSWfMDauCBc,21504
-ipex_llm/libs/starcoder.dll,sha256=BH6aZAxVOOlFHk95APYGKS_5S-uculKT1-JNpmCG3S8,561152
+ipex_llm/libs/bloom-api.dll,sha256=JRIyFfRobOSI5hEN5bKm5DslMcgofbbHEshCbD606gY,36352
+ipex_llm/libs/bloom.dll,sha256=DlmOF_8-McxmISJkQYtSkTYLNe8mVzMkbP8K5ZJTQRQ,470528
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=jufieOWWZzQmRYVyPDjM0lHiQP6DOkz2sw0RnGQU8OA,853504
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=vzbv2ltqT42OoFUX-WVorxFu9KP0NlWHAJPQWKM_-Vs,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=wUsmDAeUQFfRsBoS47VNlvtS1Iwgsm1vsEPIGQdr6PE,844288
+ipex_llm/libs/gptneox-api.dll,sha256=oFK8Z8CqkeNLOS_5oe6eOHLOSuemWvOw3u6XlWrdqoE,24576
+ipex_llm/libs/gptneox.dll,sha256=3oSu-w5f427hUm0LuD2dDbTHXQEXwClA1lv4zuLsnzw,530432
+ipex_llm/libs/libbloom_avx.dll,sha256=vHTc_Lq8UsZWItpP54W8x67KELKmQS0D5EGjNnpCAl8,496128
+ipex_llm/libs/libbloom_vnni.dll,sha256=kXllkYiR1bO57_s7VjTtOVLefQa7n_OhT9RkijNmfI0,471040
+ipex_llm/libs/libgptneox_avx.dll,sha256=Zo36gYhyyM5kQUeZ3ub3xvuVWy-OlMPXQ1SrFIarXXw,556032
+ipex_llm/libs/libgptneox_vnni.dll,sha256=gVze-IT1q6zllIWTyU1dVEsNkMKFNG-TY-QKhg4aqoA,530944
+ipex_llm/libs/libllama_avx.dll,sha256=ksROSCevn0psPJrcjHQgTYkorbaOjq3PYcR3DCwJ-14,549888
+ipex_llm/libs/libllama_vnni.dll,sha256=PBsrA-ZmsC8lSynKkhrQS6mTN5pWhkzr4z7hc0g6vWE,525312
+ipex_llm/libs/libstarcoder_avx.dll,sha256=-xB69UnRKP5GUDXfPdnA8PL74x2G4qYMC6XylDD-0Bs,586752
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=acZ9poTbIyQYD3B8pVh0UhmLZZZl7maPnR1aZBsk7Ds,561664
+ipex_llm/libs/llama-api.dll,sha256=FZT86zg7oOtWz0GBUhhEIzk3mWsfRC_sQBQkU28cs-0,25088
+ipex_llm/libs/llama.dll,sha256=4P0rTcwBgw1tiOI3MKiPWVauVn8xju1rd3iNcnc4U6M,524288
+ipex_llm/libs/main-bloom.exe,sha256=KTRsnUYX9wT_PrCGtCtZBUOV8TMfMFTZbag1YpkZcTM,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=fC26Gs-tEdFccUL2CIwWg0s-iwO8qMt05NrQQ1_wG2E,726016
+ipex_llm/libs/main-gptneox.exe,sha256=VzQisMkMNmhS7XeIa4iylbTtAaP65QY7MUmzgKYcUUU,98816
+ipex_llm/libs/main-llama.exe,sha256=WQ7-rLWavVHcdBiFLxhRLVfvoesxPRo6rBXbJY08KNk,99840
+ipex_llm/libs/main-starcoder.exe,sha256=jwxCeBIMDKCkFarlDs3uVmos03mXvAclaJkYS7eu9_o,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=JVqj3djydD4CTAcLWHu-9_6FVbVxt-j_DU518PILLPg,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=5Yp3czv-K7tiF0OorO5__R8EVs4RXjSwuoJmJBwVeAg,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=DL3sC2YRJLca_ilBYPQPmD6IcLZ6n3_YiVcb19glRS8,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=JjyHPgln3tx0NH44AVsN0LwyTwRQEfBzVgshunVBSNY,104448
+ipex_llm/libs/quantize-llama.exe,sha256=aF5rn2Hvd6yGc_odiUwB3uGeZVazItoupYqtxKDoeRE,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=mW2HHXaF5p4soOFGmNYFI5Cm7eC-Ggp5d2UbQiCAg1A,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=J8Vn4fwUDlA9aBA9U37t91ycrBWdIBVWOeieSzrbfS0,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=BI5xe_DogQkMn1q3hyx6NFBBRTgb-838rkhvw47BrhY,128512
+ipex_llm/libs/starcoder-api.dll,sha256=dcerPoxtlqkOJsafC6xD7VK7ZjRP0dzezagjzhFQFk8,21504
+ipex_llm/libs/starcoder.dll,sha256=68RPpPzRh_cpU5pO9rk1FQjwVGKoSkAvUm5eZ02g_C4,561152
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
-ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=jqingmsJeK414KelAWG0EFZxoAg9ECGzVXMssDc85oI,11824
+ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=cxg-L4hPIUPr9tQ5TVwCdH2nt7IdcAmPmkKcK13vI7s,18709
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=r_2yiI4v69w8teNzh8mZrKMsJ0l6NvWFl8TxEkvq0ug,10801
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=5Vmc7UJt_WWOCCWfe9Ct8CK_2e7CJJQNcE5mqFPEPho,73020
+ipex_llm/transformers/convert.py,sha256=mw-VH7adROosvv1vkxkw0Ntw_RAH7pUMIDGuYg6dHy4,74281
 ipex_llm/transformers/convert_ipex.py,sha256=iKXo0n8fVFTOA2fNYYrByMFK0dovL-kLd2sVDk88AlQ,14334
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=PDdcXWElpiPvzVJQdkkx6Vez0mhROW4K59sngYaX0yY,4247
 ipex_llm/transformers/lisa.py,sha256=F5WxbtXQ7RdKulj83h_2DnEIgKiKGZf7zvOmg6QBl2s,3289
 ipex_llm/transformers/loader.py,sha256=I2UnUGz985Y5dElsJStUB_rQ-K8SScrYisDEqFDvBfY,5787
 ipex_llm/transformers/lookup.py,sha256=qwY7glWICvBoDVB1UeoSGcmwOgf8SCE7zBGkm3uCfHk,14860
 ipex_llm/transformers/low_bit_linear.py,sha256=6Rerga4ZfTlT0OYOvWaJcFZwIDkosnHpnxuzXkb8iYc,39805
 ipex_llm/transformers/model.py,sha256=vXxqOj4gXqgZPlK4E_nBudLJhdG_9OcGDjljKqLaUw8,36102
 ipex_llm/transformers/modelling_bigdl.py,sha256=AqbRwpSAiHmKUo2FGOiwKtytlh-35NWb6eDy7YyNzoo,6921
-ipex_llm/transformers/qlora.py,sha256=WwHn2NXwx8SM6k7_xK1veppWiwL3g5PKihrbC3SPm-g,14770
+ipex_llm/transformers/qlora.py,sha256=Zo-XeDvTjw_Yzc7Pc3GtyV29SQuy_Zongl1B4iYQID8,15520
 ipex_llm/transformers/relora.py,sha256=-dYzUV0P-IhO2jFdnzN9-v_sFzJpRj3ZwN9eCJzOoCw,16567
 ipex_llm/transformers/speculative.py,sha256=rLpYtPPXgE5dm2ubDIWZXQVL3V8bsbsg2xYPwsw3Cfg,56201
 ipex_llm/transformers/training_patch.py,sha256=4_eQ2uCtGOnRVC2iPkzquuYnvERdneBb7Ovu_pc-VCA,8404
 ipex_llm/transformers/utils.py,sha256=DZJ4Tz-WVeGORkE_Ld8YYCz4WrePiQvtfwPOK5KJlnE,13931
 ipex_llm/transformers/xpu_customize_fwd.py,sha256=wFpIhs5F6tkNs8gBOrLxWdhLzO3EDHovVkERPIAoAvg,7611
 ipex_llm/transformers/awq/__init__.py,sha256=Du5gu3-eeAkeDO_dEMBTzrDBA66DSN3uL3-rn8WGXQw,875
 ipex_llm/transformers/awq/act.py,sha256=YwomJzOOKwkKtzGrm4L4kwBstBLO1Z8SK4CKi8PSYVQ,2172
@@ -134,27 +134,28 @@
 ipex_llm/transformers/models/baichuan.py,sha256=nW-CGAf9DKVEK40_5DtVw-K4--BdiidI3LYP21989pE,24359
 ipex_llm/transformers/models/baichuan2.py,sha256=KBjvTuOD2uJ4nBvleE5NoTT9DXn6RlyZPXCxEdIhK24,27008
 ipex_llm/transformers/models/bert.py,sha256=bJNic2pt1kph0kBwdK5MRGyWupFfx2Ts0V3D1L-5kWo,6085
 ipex_llm/transformers/models/bloom.py,sha256=IfR1rEwQb157lY2yIBQmrsS185jsBpKhgPYXEeLDQVQ,8971
 ipex_llm/transformers/models/chatglm.py,sha256=crFSh7Df1xSpND27PPBtuDUOzT1aniNjW7xMHUiIcis,13743
 ipex_llm/transformers/models/chatglm2.py,sha256=LVpz3sFOtkeKGW7rahWid_-242TIPwj_r3SFTzzT2OY,31837
 ipex_llm/transformers/models/chatglm2_32k.py,sha256=ch9Mw7T4haXcXMgqqubIi-mIQvlsdZ8gw6RhSbaUrao,8697
+ipex_llm/transformers/models/cohere.py,sha256=btBl6haf_Gx4OMYCllHftrIDTTV55SVyfIEL1AUJ6M4,20840
 ipex_llm/transformers/models/decilm.py,sha256=oAKyfB2_9GWheuqi3SyQXCBcRd6ixr6jeuYhN1z_d6A,8654
 ipex_llm/transformers/models/falcon.py,sha256=f5BzMbv4E-R5Pete8zBscbgiueXGIaWGs-5RbcMlUo4,33549
 ipex_llm/transformers/models/gemma.py,sha256=ZMn_BizM1ekqZ3erJep8L_QNLSEDgJNrUm1hEJWsQLQ,12310
 ipex_llm/transformers/models/gptbigcode.py,sha256=93l2PRLk1aLEhCGpio_7Y93amALS4SPrD5VXWiRl6hs,4342
 ipex_llm/transformers/models/gptj.py,sha256=TTIx461X2nOcIkrAcZhEf7d7mjJ3yvEC9KLVc1-hrpc,17973
 ipex_llm/transformers/models/gptneox.py,sha256=MVVdTbxV2oGzpCCzBMUy6oysVlnMtohJkl7SiC0xMAA,6219
 ipex_llm/transformers/models/internlm.py,sha256=mHyKQswtAHpT8R44gVvH7N57jjbk_GNtxjZWJy7ioog,11647
 ipex_llm/transformers/models/llama.py,sha256=gwZDIwed9KZP7O3Nt8fP5aqHDd-ULfnXIul5a9okusw,99215
 ipex_llm/transformers/models/mistral.py,sha256=X9HRxR7ej73kAQ86Y9tdXaunh3VoToO_tCUFpHWY8LY,45031
 ipex_llm/transformers/models/mixtral.py,sha256=lO7R_Aa5GP4WPb64laSykOBfL4lvQz9RLmx2MVIANKA,27294
 ipex_llm/transformers/models/mpt.py,sha256=z02NwHogJZVh-Mk4sYoIzR90SFIKhoNN_-ifsD907TQ,9540
 ipex_llm/transformers/models/phi.py,sha256=7TG4NZrQY7L8ONeYv7Rav1-ogFtQl4vd_cl5GndUmcE,7668
-ipex_llm/transformers/models/phi3.py,sha256=kMtUNl1Yrb8P6xwVIlxEu-xXTjhWvslyUV8pbLN1ug4,7835
+ipex_llm/transformers/models/phi3.py,sha256=bYaYZq6_jrSM-pEsqC4NXTx0nzVTcW40IQq9fXVJbCc,9210
 ipex_llm/transformers/models/phixtral.py,sha256=4B_2iE26GlzTVdaemd6mwYQ8mp4Yo4Yq9DgSFkF0yvc,6268
 ipex_llm/transformers/models/qwen.py,sha256=SCnqmWy57XjoEunYbpjezzGRvPiOBDPdpBbSSEhpY2A,32251
 ipex_llm/transformers/models/qwen2.py,sha256=A4kWbTSPNAryuX4XJQ9DJnA1fK2U8U_w7Z8cr-2ej4Y,32651
 ipex_llm/transformers/models/qwen2_moe.py,sha256=xO4aGuwdu9QP4lmbPrH5VqFUx3atC__0URXNzbpWEiw,38484
 ipex_llm/transformers/models/qwen_vl.py,sha256=8uu4OS-KipkMxUZxCnjjx28LfIwdqz2ue-Ul1ZwtdO0,11832
 ipex_llm/transformers/models/rwkv4.py,sha256=Kzu6QlEi0KDXiJrfoZ71TI_D2nju2-sOeaKSZqdJz8U,6135
 ipex_llm/transformers/models/rwkv5.py,sha256=nNtWQROVAUc82SClzHrbaYVsr6CALnlVos0I2TX0YUc,10722
@@ -175,14 +176,14 @@
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
 ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/ipex_llm_gpu_executor.py,sha256=pY-8XxRRX1_9MTW0TUTidxHmjmXKGsvs1AIIVWU21yM,18514
 ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/engine/engine.py,sha256=mVuCyoTcCX7KnK819-8fL_rNAu05WF_gql6jEcZ9bn8,5941
 ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
-ipex_llm-2.1.0b20240506.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240506.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240506.dist-info/METADATA,sha256=FoCZ1Klv86HfZOWyYZFWGonc095zwfEbeHmD6NVMKWA,5125
-ipex_llm-2.1.0b20240506.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240506.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240506.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240506.dist-info/RECORD,,
+ipex_llm-2.1.0b20240507.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240507.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240507.dist-info/METADATA,sha256=uWbw0PyaIIXud3jRoCYnka7LaUjlLAnE2WBAMJcuSh8,5125
+ipex_llm-2.1.0b20240507.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240507.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240507.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240507.dist-info/RECORD,,
```

