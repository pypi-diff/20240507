# Comparing `tmp/whisperplus-0.3.3.tar.gz` & `tmp/whisperplus-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisperplus-0.3.3.tar", last modified: Mon May  6 11:57:35 2024, max compression
+gzip compressed data, was "whisperplus-0.3.4.tar", last modified: Tue May  7 13:07:58 2024, max compression
```

## Comparing `whisperplus-0.3.3.tar` & `whisperplus-0.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-06 11:57:35.919461 whisperplus-0.3.3/
--rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.3.3/LICENSE
--rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.3.3/MANIFEST.in
--rw-r--r--   0 kadirnar   (501) staff       (20)     6165 2024-05-06 11:57:35.919651 whisperplus-0.3.3/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)     5855 2024-05-05 21:41:11.000000 whisperplus-0.3.3/README.md
--rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-04 11:16:41.000000 whisperplus-0.3.3/requirements.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-06 11:57:35.919941 whisperplus-0.3.3/setup.cfg
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.3.3/setup.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-06 11:57:35.915932 whisperplus-0.3.3/whisperplus/
--rw-r--r--   0 kadirnar   (501) staff       (20)      740 2024-05-06 11:57:30.000000 whisperplus-0.3.3/whisperplus/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/app.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2497 2024-05-06 11:55:58.000000 whisperplus-0.3.3/whisperplus/audio_eval.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-06 11:57:35.918790 whisperplus-0.3.3/whisperplus/pipelines/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/pipelines/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/pipelines/autollm_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/pipelines/lancedb_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/pipelines/long_text_summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/pipelines/summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.3.3/whisperplus/pipelines/text2speech.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3208 2024-05-05 21:41:11.000000 whisperplus-0.3.3/whisperplus/pipelines/whisper.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/pipelines/whisper_autocaption.py
--rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/pipelines/whisper_diarize.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1276 2024-05-05 21:41:08.000000 whisperplus-0.3.3/whisperplus/test.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-06 11:57:35.919353 whisperplus-0.3.3/whisperplus/utils/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/utils/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/utils/download_utils.py
--rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.3.3/whisperplus/utils/text_utils.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-06 11:57:35.916732 whisperplus-0.3.3/whisperplus.egg-info/
--rw-r--r--   0 kadirnar   (501) staff       (20)     6165 2024-05-06 11:57:35.000000 whisperplus-0.3.3/whisperplus.egg-info/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)      786 2024-05-06 11:57:35.000000 whisperplus-0.3.3/whisperplus.egg-info/SOURCES.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-06 11:57:35.000000 whisperplus-0.3.3/whisperplus.egg-info/dependency_links.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-06 11:57:35.000000 whisperplus-0.3.3/whisperplus.egg-info/requires.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-06 11:57:35.000000 whisperplus-0.3.3/whisperplus.egg-info/top_level.txt
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-07 13:07:58.602631 whisperplus-0.3.4/
+-rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.3.4/LICENSE
+-rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.3.4/MANIFEST.in
+-rw-r--r--   0 kadirnar   (501) staff       (20)     7102 2024-05-07 13:07:58.602807 whisperplus-0.3.4/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)     6792 2024-05-07 13:07:35.000000 whisperplus-0.3.4/README.md
+-rw-r--r--   0 kadirnar   (501) staff       (20)      132 2024-05-07 13:07:35.000000 whisperplus-0.3.4/requirements.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-07 13:07:58.603121 whisperplus-0.3.4/setup.cfg
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.3.4/setup.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-07 13:07:58.598811 whisperplus-0.3.4/whisperplus/
+-rw-r--r--   0 kadirnar   (501) staff       (20)      772 2024-05-07 13:07:38.000000 whisperplus-0.3.4/whisperplus/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     7717 2024-05-07 13:07:35.000000 whisperplus-0.3.4/whisperplus/app.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2497 2024-05-06 11:55:58.000000 whisperplus-0.3.4/whisperplus/audio_eval.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-07 13:07:58.601707 whisperplus-0.3.4/whisperplus/pipelines/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/pipelines/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/pipelines/autollm_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/pipelines/lancedb_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/pipelines/long_text_summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/pipelines/summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.3.4/whisperplus/pipelines/text2speech.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3208 2024-05-05 21:41:11.000000 whisperplus-0.3.4/whisperplus/pipelines/whisper.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/pipelines/whisper_autocaption.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/pipelines/whisper_diarize.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1268 2024-05-07 13:07:35.000000 whisperplus-0.3.4/whisperplus/test.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-07 13:07:58.602451 whisperplus-0.3.4/whisperplus/utils/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/utils/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2897 2024-05-07 13:07:35.000000 whisperplus-0.3.4/whisperplus/utils/download_utils.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.3.4/whisperplus/utils/text_utils.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-07 13:07:58.599576 whisperplus-0.3.4/whisperplus.egg-info/
+-rw-r--r--   0 kadirnar   (501) staff       (20)     7102 2024-05-07 13:07:58.000000 whisperplus-0.3.4/whisperplus.egg-info/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)      786 2024-05-07 13:07:58.000000 whisperplus-0.3.4/whisperplus.egg-info/SOURCES.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-07 13:07:58.000000 whisperplus-0.3.4/whisperplus.egg-info/dependency_links.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      132 2024-05-07 13:07:58.000000 whisperplus-0.3.4/whisperplus.egg-info/requires.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-07 13:07:58.000000 whisperplus-0.3.4/whisperplus.egg-info/top_level.txt
```

### Comparing `whisperplus-0.3.3/LICENSE` & `whisperplus-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/PKG-INFO` & `whisperplus-0.3.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: whisperplus
-Version: 0.3.3
-Summary: WhisperPlus: A Python library for WhisperPlus API.
-Home-page: https://github.com/kadirnar/whisperplus
-Author: kadirnar
-Author-email: kadir.nar@hotmail.com
-License: Apache License 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 <h2>
     WhisperPlus: Faster, Smarter, and More Capable 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
@@ -24,38 +13,38 @@
     <a href="https://huggingface.co/spaces/ArtGAN/Audio-WebUI"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
-pip install whisperplus git+https://github.com/huggingface/transformers
+pip install git+https://github.com/huggingface/transformers
 pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
 ## 🎙️ Usage
 
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
-from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
+from whisperplus import SpeechToTextPipeline, download_youtube_to_mp3
 from transformers import BitsAndBytesConfig, HqqConfig
 import torch
 
 url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
-audio_path = download_and_convert_to_mp3(url)
+audio_path = download_youtube_to_mp3(url, output_dir="downloads", filename="test")
 
 hqq_config = HqqConfig(
-    nbits=1,
+    nbits=4,
     group_size=64,
     quant_zero=False,
     quant_scale=False,
     axis=0,
     offload_meta=False,
 )  # axis=0 is used by default
 
@@ -85,58 +74,70 @@
 
 print(transcript)
 ```
 
 ### 📰 Summarization
 
 ```python
-from whisperplus import TextSummarizationPipeline
+from whisperplus.pipelines.summarization import TextSummarizationPipeline
 
 summarizer = TextSummarizationPipeline(model_id="facebook/bart-large-cnn")
 summary = summarizer.summarize(transcript)
 print(summary[0]["summary_text"])
 ```
 
 ### 📰 Long Text Support Summarization
 
 ```python
-from whisperplus import LongTextSummarizationPipeline
+from whisperplus.pipelines.long_text_summarization import LongTextSummarizationPipeline
 
 summarizer = LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn")
 summary_text = summarizer.summarize(transcript)
 print(summary_text)
 ```
 
 ### 💬 Speaker Diarization
 
+You must confirm the licensing permissions of these two models.
+
+- https://huggingface.co/pyannote/speaker-diarization-3.1
+- https://huggingface.co/pyannote/segmentation-3.0
+
+```bash
+pip install -r speaker_diarization.txt
+pip install -U "huggingface_hub[cli]"
+huggingface-cli login
+```
+
 ```python
-from whisperplus import (
-    ASRDiarizationPipeline,
-    download_and_convert_to_mp3,
-    format_speech_to_dialogue,
-)
+from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
+from whisperplus import download_youtube_to_mp3, format_speech_to_dialogue
 
-audio_path = download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
+audio_path = download_youtube_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
 
 device = "cuda"  # cpu or mps
 pipeline = ASRDiarizationPipeline.from_pretrained(
     asr_model="openai/whisper-large-v3",
-    diarizer_model="pyannote/speaker-diarization",
+    diarizer_model="pyannote/speaker-diarization-3.1",
     use_auth_token=False,
     chunk_length_s=30,
     device=device,
 )
 
 output_text = pipeline(audio_path, num_speakers=2, min_speaker=1, max_speaker=2)
 dialogue = format_speech_to_dialogue(output_text)
 print(dialogue)
 ```
 
 ### ⭐ RAG - Chat with Video(LanceDB)
 
+```bash
+pip install sentence-transformers ctransformers langchain
+```
+
 ```python
 from whisperplus.pipelines.chatbot import ChatWithVideo
 
 chat = ChatWithVideo(
     input_file="trascript.txt",
     llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
     llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf",
@@ -147,16 +148,20 @@
 query = "what is this video about ?"
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🌠 RAG - Chat with Video(AutoLLM)
 
+```bash
+pip install autollm>=0.1.9
+```
+
 ```python
-from whisperplus import AutoLLMChatWithVideo
+from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
 
 # service_context_params
 system_prompt = """
 You are an friendly ai assistant that help users find the most relevant and accurate answers
 to their questions based on the documents you have access to.
 When answering the questions, mostly rely on the info in documents.
 """
@@ -187,33 +192,46 @@
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🎙️ Speech to Text
 
 ```python
-from whisperplus import TextToSpeechPipeline
+from whisperplus.pipelines.text2speech import TextToSpeechPipeline
 
 tts = TextToSpeechPipeline(model_id="suno/bark")
 audio = tts(text="Hello World", voice_preset="v2/en_speaker_6")
 ```
 
 ### 🎥 AutoCaption
 
+```bash
+pip install moviepy
+apt install imagemagick libmagick++-dev
+cat /etc/ImageMagick-6/policy.xml | sed 's/none/read,write/g'> /etc/ImageMagick-6/policy.xml
+```
+
 ```python
-from whisperplus import WhisperAutoCaptionPipeline
+from whisperplus.pipelines.whisper_autocaption import WhisperAutoCaptionPipeline
+from whisperplus import download_youtube_to_mp4
+
+video_path = download_youtube_to_mp4(
+    "https://www.youtube.com/watch?v=di3rHkEZuUw",
+    output_dir="downloads",
+    filename="test",
+)  # Optional
 
 caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
-caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+caption(video_path=video_path, output_path="output.mp4", language="english")
 ```
 
 ## 😍 Contributing
 
 ```bash
-pip install -r dev-requirements.txt
+pip install pre-commit
 pre-commit install
 pre-commit run --all-files
 ```
 
 ## 📜 License
 
 This project is licensed under the terms of the Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,76 +1,84 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.3.3 Summary: WhisperPlus: A
-Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
-whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
-Apache License 2.0 Description-Content-Type: text/markdown License-File:
-LICENSE
         ********** WWhhiissppeerrPPlluuss:: FFaasstteerr,, SSmmaarrtteerr,, aanndd MMoorree CCaappaabbllee ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
-huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
-ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
-huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
-library, follow the steps below for different tasks: ### ðµ Youtube URL to
-Audio ```python from whisperplus import SpeechToTextPipeline,
-download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
-HqqConfig import torch url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
-audio_path = download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
+## ð ï¸ Installation ```bash pip install git+https://github.com/huggingface/
+transformers pip install flash-attn --no-build-isolation ``` ## ð¤ Model Hub
+You can find the models on the [HuggingFace Model Hub](https://huggingface.co/
+models?search=whisper) ## ðï¸ Usage To use the whisperplus library, follow
+the steps below for different tasks: ### ðµ Youtube URL to Audio ```python
+from whisperplus import SpeechToTextPipeline, download_youtube_to_mp3 from
+transformers import BitsAndBytesConfig, HqqConfig import torch url = "https://
+www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_youtube_to_mp3(url,
+output_dir="downloads", filename="test") hqq_config = HqqConfig( nbits=4,
 group_size=64, quant_zero=False, quant_scale=False, axis=0, offload_meta=False,
 ) # axis=0 is used by default bnb_config = BitsAndBytesConfig
 ( load_in_4bit=True, bnb_4bit_quant_type="nf4",
 bnb_4bit_compute_dtype=torch.bfloat16, bnb_4bit_use_double_quant=True, )
 pipeline = SpeechToTextPipeline( model_id="distil-whisper/distil-large-v3",
 quant_config=hqq_config, hqq=True, flash_attention_2=True, ) transcript =
 pipeline( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
 max_new_tokens=128, batch_size=100, language="english",
 return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
-```python from whisperplus import TextSummarizationPipeline summarizer =
-TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
-summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
-Long Text Support Summarization ```python from whisperplus import
+```python from whisperplus.pipelines.summarization import
+TextSummarizationPipeline summarizer = TextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
+print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
+```python from whisperplus.pipelines.long_text_summarization import
 LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
 (model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
-(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
-from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
-format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
-www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
+(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization You must
+confirm the licensing permissions of these two models. - https://
+huggingface.co/pyannote/speaker-diarization-3.1 - https://huggingface.co/
+pyannote/segmentation-3.0 ```bash pip install -r speaker_diarization.txt pip
+install -U "huggingface_hub[cli]" huggingface-cli login ``` ```python from
+whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline from
+whisperplus import download_youtube_to_mp3, format_speech_to_dialogue
+audio_path = download_youtube_to_mp3("https://www.youtube.com/
+watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
 ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
-diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
+diarizer_model="pyannote/speaker-diarization-3.1", use_auth_token=False,
 chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
 num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
 format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
-with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
-ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
-llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
-v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
-transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
-= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
-(AutoLLM) ```python from whisperplus import AutoLLMChatWithVideo #
-service_context_params system_prompt = """ You are an friendly ai assistant
-that help users find the most relevant and accurate answers to their questions
-based on the documents you have access to. When answering the questions, mostly
-rely on the info in documents. """ query_wrapper_prompt = """ The document
-information is below. --------------------- {context_str} --------------------
-- Using the document information and mostly relying on it, answer the query.
-Query: {query_str} Answer: """ chat = AutoLLMChatWithVideo
-( input_file="input_dir", # path of mp3 file openai_key="YOUR_OPENAI_KEY", #
-optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
-turbo", llm_max_tokens="256", llm_temperature="0.1",
-system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
-embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
-= "what is this video about ?" response = chat.run_query(query) print(response)
-``` ### ðï¸ Speech to Text ```python from whisperplus import
-TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
-tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ### ð¥
-AutoCaption ```python from whisperplus import WhisperAutoCaptionPipeline
+with Video(LanceDB) ```bash pip install sentence-transformers ctransformers
+langchain ``` ```python from whisperplus.pipelines.chatbot import ChatWithVideo
+chat = ChatWithVideo( input_file="trascript.txt", llm_model_name="TheBloke/
+Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf",
+llm_model_type="mistral", embedding_model_name="sentence-transformers/all-
+MiniLM-L6-v2", ) query = "what is this video about ?" response = chat.run_query
+(query) print(response) ``` ### ð  RAG - Chat with Video(AutoLLM) ```bash pip
+install autollm>=0.1.9 ``` ```python from whisperplus.pipelines.autollm_chatbot
+import AutoLLMChatWithVideo # service_context_params system_prompt = """ You
+are an friendly ai assistant that help users find the most relevant and
+accurate answers to their questions based on the documents you have access to.
+When answering the questions, mostly rely on the info in documents. """
+query_wrapper_prompt = """ The document information is below. -----------------
+---- {context_str} --------------------- Using the document information and
+mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
+AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
+openai_key="YOUR_OPENAI_KEY", # optional
+huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
+llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
+query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
+large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
+response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
+```python from whisperplus.pipelines.text2speech import TextToSpeechPipeline
+tts = TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello
+World", voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```bash pip
+install moviepy apt install imagemagick libmagick++-dev cat /etc/ImageMagick-6/
+policy.xml | sed 's/none/read,write/g'> /etc/ImageMagick-6/policy.xml ```
+```python from whisperplus.pipelines.whisper_autocaption import
+WhisperAutoCaptionPipeline from whisperplus import download_youtube_to_mp4
+video_path = download_youtube_to_mp4( "https://www.youtube.com/
+watch?v=di3rHkEZuUw", output_dir="downloads", filename="test", ) # Optional
 caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
-caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
-``` ## ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
-install pre-commit run --all-files ``` ## ð License This project is licensed
-under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
+caption(video_path=video_path, output_path="output.mp4", language="english")
+``` ## ð Contributing ```bash pip install pre-commit pre-commit install pre-
+commit run --all-files ``` ## ð License This project is licensed under the
+terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
 license} } ```
```

### Comparing `whisperplus-0.3.3/README.md` & `whisperplus-0.3.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: whisperplus
+Version: 0.3.4
+Summary: WhisperPlus: A Python library for WhisperPlus API.
+Home-page: https://github.com/kadirnar/whisperplus
+Author: kadirnar
+Author-email: kadir.nar@hotmail.com
+License: Apache License 2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 <h2>
     WhisperPlus: Faster, Smarter, and More Capable 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
@@ -13,38 +24,38 @@
     <a href="https://huggingface.co/spaces/ArtGAN/Audio-WebUI"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
-pip install whisperplus git+https://github.com/huggingface/transformers
+pip install git+https://github.com/huggingface/transformers
 pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
 ## 🎙️ Usage
 
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
-from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
+from whisperplus import SpeechToTextPipeline, download_youtube_to_mp3
 from transformers import BitsAndBytesConfig, HqqConfig
 import torch
 
 url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
-audio_path = download_and_convert_to_mp3(url)
+audio_path = download_youtube_to_mp3(url, output_dir="downloads", filename="test")
 
 hqq_config = HqqConfig(
-    nbits=1,
+    nbits=4,
     group_size=64,
     quant_zero=False,
     quant_scale=False,
     axis=0,
     offload_meta=False,
 )  # axis=0 is used by default
 
@@ -74,58 +85,70 @@
 
 print(transcript)
 ```
 
 ### 📰 Summarization
 
 ```python
-from whisperplus import TextSummarizationPipeline
+from whisperplus.pipelines.summarization import TextSummarizationPipeline
 
 summarizer = TextSummarizationPipeline(model_id="facebook/bart-large-cnn")
 summary = summarizer.summarize(transcript)
 print(summary[0]["summary_text"])
 ```
 
 ### 📰 Long Text Support Summarization
 
 ```python
-from whisperplus import LongTextSummarizationPipeline
+from whisperplus.pipelines.long_text_summarization import LongTextSummarizationPipeline
 
 summarizer = LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn")
 summary_text = summarizer.summarize(transcript)
 print(summary_text)
 ```
 
 ### 💬 Speaker Diarization
 
+You must confirm the licensing permissions of these two models.
+
+- https://huggingface.co/pyannote/speaker-diarization-3.1
+- https://huggingface.co/pyannote/segmentation-3.0
+
+```bash
+pip install -r speaker_diarization.txt
+pip install -U "huggingface_hub[cli]"
+huggingface-cli login
+```
+
 ```python
-from whisperplus import (
-    ASRDiarizationPipeline,
-    download_and_convert_to_mp3,
-    format_speech_to_dialogue,
-)
+from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
+from whisperplus import download_youtube_to_mp3, format_speech_to_dialogue
 
-audio_path = download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
+audio_path = download_youtube_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
 
 device = "cuda"  # cpu or mps
 pipeline = ASRDiarizationPipeline.from_pretrained(
     asr_model="openai/whisper-large-v3",
-    diarizer_model="pyannote/speaker-diarization",
+    diarizer_model="pyannote/speaker-diarization-3.1",
     use_auth_token=False,
     chunk_length_s=30,
     device=device,
 )
 
 output_text = pipeline(audio_path, num_speakers=2, min_speaker=1, max_speaker=2)
 dialogue = format_speech_to_dialogue(output_text)
 print(dialogue)
 ```
 
 ### ⭐ RAG - Chat with Video(LanceDB)
 
+```bash
+pip install sentence-transformers ctransformers langchain
+```
+
 ```python
 from whisperplus.pipelines.chatbot import ChatWithVideo
 
 chat = ChatWithVideo(
     input_file="trascript.txt",
     llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
     llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf",
@@ -136,16 +159,20 @@
 query = "what is this video about ?"
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🌠 RAG - Chat with Video(AutoLLM)
 
+```bash
+pip install autollm>=0.1.9
+```
+
 ```python
-from whisperplus import AutoLLMChatWithVideo
+from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
 
 # service_context_params
 system_prompt = """
 You are an friendly ai assistant that help users find the most relevant and accurate answers
 to their questions based on the documents you have access to.
 When answering the questions, mostly rely on the info in documents.
 """
@@ -176,33 +203,46 @@
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🎙️ Speech to Text
 
 ```python
-from whisperplus import TextToSpeechPipeline
+from whisperplus.pipelines.text2speech import TextToSpeechPipeline
 
 tts = TextToSpeechPipeline(model_id="suno/bark")
 audio = tts(text="Hello World", voice_preset="v2/en_speaker_6")
 ```
 
 ### 🎥 AutoCaption
 
+```bash
+pip install moviepy
+apt install imagemagick libmagick++-dev
+cat /etc/ImageMagick-6/policy.xml | sed 's/none/read,write/g'> /etc/ImageMagick-6/policy.xml
+```
+
 ```python
-from whisperplus import WhisperAutoCaptionPipeline
+from whisperplus.pipelines.whisper_autocaption import WhisperAutoCaptionPipeline
+from whisperplus import download_youtube_to_mp4
+
+video_path = download_youtube_to_mp4(
+    "https://www.youtube.com/watch?v=di3rHkEZuUw",
+    output_dir="downloads",
+    filename="test",
+)  # Optional
 
 caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
-caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+caption(video_path=video_path, output_path="output.mp4", language="english")
 ```
 
 ## 😍 Contributing
 
 ```bash
-pip install -r dev-requirements.txt
+pip install pre-commit
 pre-commit install
 pre-commit run --all-files
 ```
 
 ## 📜 License
 
 This project is licensed under the terms of the Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,71 +1,89 @@
+Metadata-Version: 2.1 Name: whisperplus Version: 0.3.4 Summary: WhisperPlus: A
+Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
+whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
+Apache License 2.0 Description-Content-Type: text/markdown License-File:
+LICENSE
         ********** WWhhiissppeerrPPlluuss:: FFaasstteerr,, SSmmaarrtteerr,, aanndd MMoorree CCaappaabbllee ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
-huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
-ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
-huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
-library, follow the steps below for different tasks: ### ðµ Youtube URL to
-Audio ```python from whisperplus import SpeechToTextPipeline,
-download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
-HqqConfig import torch url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
-audio_path = download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
+## ð ï¸ Installation ```bash pip install git+https://github.com/huggingface/
+transformers pip install flash-attn --no-build-isolation ``` ## ð¤ Model Hub
+You can find the models on the [HuggingFace Model Hub](https://huggingface.co/
+models?search=whisper) ## ðï¸ Usage To use the whisperplus library, follow
+the steps below for different tasks: ### ðµ Youtube URL to Audio ```python
+from whisperplus import SpeechToTextPipeline, download_youtube_to_mp3 from
+transformers import BitsAndBytesConfig, HqqConfig import torch url = "https://
+www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_youtube_to_mp3(url,
+output_dir="downloads", filename="test") hqq_config = HqqConfig( nbits=4,
 group_size=64, quant_zero=False, quant_scale=False, axis=0, offload_meta=False,
 ) # axis=0 is used by default bnb_config = BitsAndBytesConfig
 ( load_in_4bit=True, bnb_4bit_quant_type="nf4",
 bnb_4bit_compute_dtype=torch.bfloat16, bnb_4bit_use_double_quant=True, )
 pipeline = SpeechToTextPipeline( model_id="distil-whisper/distil-large-v3",
 quant_config=hqq_config, hqq=True, flash_attention_2=True, ) transcript =
 pipeline( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
 max_new_tokens=128, batch_size=100, language="english",
 return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
-```python from whisperplus import TextSummarizationPipeline summarizer =
-TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
-summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
-Long Text Support Summarization ```python from whisperplus import
+```python from whisperplus.pipelines.summarization import
+TextSummarizationPipeline summarizer = TextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
+print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
+```python from whisperplus.pipelines.long_text_summarization import
 LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
 (model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
-(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
-from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
-format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
-www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
+(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization You must
+confirm the licensing permissions of these two models. - https://
+huggingface.co/pyannote/speaker-diarization-3.1 - https://huggingface.co/
+pyannote/segmentation-3.0 ```bash pip install -r speaker_diarization.txt pip
+install -U "huggingface_hub[cli]" huggingface-cli login ``` ```python from
+whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline from
+whisperplus import download_youtube_to_mp3, format_speech_to_dialogue
+audio_path = download_youtube_to_mp3("https://www.youtube.com/
+watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
 ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
-diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
+diarizer_model="pyannote/speaker-diarization-3.1", use_auth_token=False,
 chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
 num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
 format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
-with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
-ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
-llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
-v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
-transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
-= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
-(AutoLLM) ```python from whisperplus import AutoLLMChatWithVideo #
-service_context_params system_prompt = """ You are an friendly ai assistant
-that help users find the most relevant and accurate answers to their questions
-based on the documents you have access to. When answering the questions, mostly
-rely on the info in documents. """ query_wrapper_prompt = """ The document
-information is below. --------------------- {context_str} --------------------
-- Using the document information and mostly relying on it, answer the query.
-Query: {query_str} Answer: """ chat = AutoLLMChatWithVideo
-( input_file="input_dir", # path of mp3 file openai_key="YOUR_OPENAI_KEY", #
-optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
-turbo", llm_max_tokens="256", llm_temperature="0.1",
-system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
-embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
-= "what is this video about ?" response = chat.run_query(query) print(response)
-``` ### ðï¸ Speech to Text ```python from whisperplus import
-TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
-tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ### ð¥
-AutoCaption ```python from whisperplus import WhisperAutoCaptionPipeline
+with Video(LanceDB) ```bash pip install sentence-transformers ctransformers
+langchain ``` ```python from whisperplus.pipelines.chatbot import ChatWithVideo
+chat = ChatWithVideo( input_file="trascript.txt", llm_model_name="TheBloke/
+Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf",
+llm_model_type="mistral", embedding_model_name="sentence-transformers/all-
+MiniLM-L6-v2", ) query = "what is this video about ?" response = chat.run_query
+(query) print(response) ``` ### ð  RAG - Chat with Video(AutoLLM) ```bash pip
+install autollm>=0.1.9 ``` ```python from whisperplus.pipelines.autollm_chatbot
+import AutoLLMChatWithVideo # service_context_params system_prompt = """ You
+are an friendly ai assistant that help users find the most relevant and
+accurate answers to their questions based on the documents you have access to.
+When answering the questions, mostly rely on the info in documents. """
+query_wrapper_prompt = """ The document information is below. -----------------
+---- {context_str} --------------------- Using the document information and
+mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
+AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
+openai_key="YOUR_OPENAI_KEY", # optional
+huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
+llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
+query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
+large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
+response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
+```python from whisperplus.pipelines.text2speech import TextToSpeechPipeline
+tts = TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello
+World", voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```bash pip
+install moviepy apt install imagemagick libmagick++-dev cat /etc/ImageMagick-6/
+policy.xml | sed 's/none/read,write/g'> /etc/ImageMagick-6/policy.xml ```
+```python from whisperplus.pipelines.whisper_autocaption import
+WhisperAutoCaptionPipeline from whisperplus import download_youtube_to_mp4
+video_path = download_youtube_to_mp4( "https://www.youtube.com/
+watch?v=di3rHkEZuUw", output_dir="downloads", filename="test", ) # Optional
 caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
-caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
-``` ## ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
-install pre-commit run --all-files ``` ## ð License This project is licensed
-under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
+caption(video_path=video_path, output_path="output.mp4", language="english")
+``` ## ð Contributing ```bash pip install pre-commit pre-commit install pre-
+commit run --all-files ``` ## ð License This project is licensed under the
+terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
 license} } ```
```

### Comparing `whisperplus-0.3.3/setup.cfg` & `whisperplus-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/setup.py` & `whisperplus-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/app.py` & `whisperplus-0.3.4/whisperplus/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import gradio as gr
 
 from whisperplus.pipelines.whisper import SpeechToTextPipeline
 from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
-from whisperplus.utils.download_utils import download_and_convert_to_mp3
+from whisperplus.utils.download_utils import download_youtube_to_mp3
 from whisperplus.utils.text_utils import format_speech_to_dialogue
 
 
 def youtube_url_to_text(url, model_id, language_choice):
     """
     Main function that downloads and converts a video to MP3 format, performs speech-to-text conversion using
     a specified model, and returns the transcript along with the video path.
@@ -16,15 +16,15 @@
         model_id (str): The ID of the speech-to-text model to use.
         language_choice (str): The language choice for the speech-to-text conversion.
 
     Returns:
         transcript (str): The transcript of the speech-to-text conversion.
         video_path (str): The path of the downloaded video.
     """
-    video_path = download_and_convert_to_mp3(url)
+    video_path = download_youtube_to_mp3(url)
     pipeline = SpeechToTextPipeline(model_id)
     transcript = pipeline(audio_path=video_path, model_id=model_id, language=language_choice)
 
     return transcript, video_path
 
 
 def speaker_diarization(url, model_id, device, num_speakers, min_speaker, max_speaker):
@@ -46,15 +46,15 @@
         asr_model=model_id,
         diarizer_model="pyannote/speaker-diarization",
         use_auth_token=False,
         chunk_length_s=30,
         device=device,
     )
 
-    audio_path = download_and_convert_to_mp3(url)
+    audio_path = download_youtube_to_mp3(url)
     output_text = pipeline(
         audio_path, num_speakers=num_speakers, min_speaker=min_speaker, max_speaker=max_speaker)
     dialogue = format_speech_to_dialogue(output_text)
     return dialogue, audio_path
 
 
 def youtube_url_to_text_app():
```

### Comparing `whisperplus-0.3.3/whisperplus/audio_eval.py` & `whisperplus-0.3.4/whisperplus/audio_eval.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/autollm_chatbot.py` & `whisperplus-0.3.4/whisperplus/pipelines/autollm_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/lancedb_chatbot.py` & `whisperplus-0.3.4/whisperplus/pipelines/lancedb_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/long_text_summarization.py` & `whisperplus-0.3.4/whisperplus/pipelines/long_text_summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/summarization.py` & `whisperplus-0.3.4/whisperplus/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/text2speech.py` & `whisperplus-0.3.4/whisperplus/pipelines/text2speech.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/whisper.py` & `whisperplus-0.3.4/whisperplus/pipelines/whisper.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/whisper_autocaption.py` & `whisperplus-0.3.4/whisperplus/pipelines/whisper_autocaption.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/pipelines/whisper_diarize.py` & `whisperplus-0.3.4/whisperplus/pipelines/whisper_diarize.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus/test.py` & `whisperplus-0.3.4/whisperplus/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from hqq.utils.patching import prepare_for_inference
 from pipelines.whisper import SpeechToTextPipeline
 from transformers import BitsAndBytesConfig, HqqConfig
-from utils.download_utils import download_and_convert_to_mp3
+from utils.download_utils import download_youtube_to_mp3
 
 url = "https://www.youtube.com/watch?v=BpN4hEAvDBg"
-audio_path = download_and_convert_to_mp3(url)
+audio_path = download_youtube_to_mp3(url)
 
 hqq_config = HqqConfig(
     nbits=1,
     group_size=64,
     quant_zero=False,
     quant_scale=False,
     axis=0,
```

### Comparing `whisperplus-0.3.3/whisperplus/utils/text_utils.py` & `whisperplus-0.3.4/whisperplus/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.3/whisperplus.egg-info/PKG-INFO` & `whisperplus-0.3.4/whisperplus.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.3.3
+Version: 0.3.4
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,38 +24,38 @@
     <a href="https://huggingface.co/spaces/ArtGAN/Audio-WebUI"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
-pip install whisperplus git+https://github.com/huggingface/transformers
+pip install git+https://github.com/huggingface/transformers
 pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
 ## 🎙️ Usage
 
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
-from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
+from whisperplus import SpeechToTextPipeline, download_youtube_to_mp3
 from transformers import BitsAndBytesConfig, HqqConfig
 import torch
 
 url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
-audio_path = download_and_convert_to_mp3(url)
+audio_path = download_youtube_to_mp3(url, output_dir="downloads", filename="test")
 
 hqq_config = HqqConfig(
-    nbits=1,
+    nbits=4,
     group_size=64,
     quant_zero=False,
     quant_scale=False,
     axis=0,
     offload_meta=False,
 )  # axis=0 is used by default
 
@@ -85,58 +85,70 @@
 
 print(transcript)
 ```
 
 ### 📰 Summarization
 
 ```python
-from whisperplus import TextSummarizationPipeline
+from whisperplus.pipelines.summarization import TextSummarizationPipeline
 
 summarizer = TextSummarizationPipeline(model_id="facebook/bart-large-cnn")
 summary = summarizer.summarize(transcript)
 print(summary[0]["summary_text"])
 ```
 
 ### 📰 Long Text Support Summarization
 
 ```python
-from whisperplus import LongTextSummarizationPipeline
+from whisperplus.pipelines.long_text_summarization import LongTextSummarizationPipeline
 
 summarizer = LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn")
 summary_text = summarizer.summarize(transcript)
 print(summary_text)
 ```
 
 ### 💬 Speaker Diarization
 
+You must confirm the licensing permissions of these two models.
+
+- https://huggingface.co/pyannote/speaker-diarization-3.1
+- https://huggingface.co/pyannote/segmentation-3.0
+
+```bash
+pip install -r speaker_diarization.txt
+pip install -U "huggingface_hub[cli]"
+huggingface-cli login
+```
+
 ```python
-from whisperplus import (
-    ASRDiarizationPipeline,
-    download_and_convert_to_mp3,
-    format_speech_to_dialogue,
-)
+from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
+from whisperplus import download_youtube_to_mp3, format_speech_to_dialogue
 
-audio_path = download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
+audio_path = download_youtube_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
 
 device = "cuda"  # cpu or mps
 pipeline = ASRDiarizationPipeline.from_pretrained(
     asr_model="openai/whisper-large-v3",
-    diarizer_model="pyannote/speaker-diarization",
+    diarizer_model="pyannote/speaker-diarization-3.1",
     use_auth_token=False,
     chunk_length_s=30,
     device=device,
 )
 
 output_text = pipeline(audio_path, num_speakers=2, min_speaker=1, max_speaker=2)
 dialogue = format_speech_to_dialogue(output_text)
 print(dialogue)
 ```
 
 ### ⭐ RAG - Chat with Video(LanceDB)
 
+```bash
+pip install sentence-transformers ctransformers langchain
+```
+
 ```python
 from whisperplus.pipelines.chatbot import ChatWithVideo
 
 chat = ChatWithVideo(
     input_file="trascript.txt",
     llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
     llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf",
@@ -147,16 +159,20 @@
 query = "what is this video about ?"
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🌠 RAG - Chat with Video(AutoLLM)
 
+```bash
+pip install autollm>=0.1.9
+```
+
 ```python
-from whisperplus import AutoLLMChatWithVideo
+from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
 
 # service_context_params
 system_prompt = """
 You are an friendly ai assistant that help users find the most relevant and accurate answers
 to their questions based on the documents you have access to.
 When answering the questions, mostly rely on the info in documents.
 """
@@ -187,33 +203,46 @@
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🎙️ Speech to Text
 
 ```python
-from whisperplus import TextToSpeechPipeline
+from whisperplus.pipelines.text2speech import TextToSpeechPipeline
 
 tts = TextToSpeechPipeline(model_id="suno/bark")
 audio = tts(text="Hello World", voice_preset="v2/en_speaker_6")
 ```
 
 ### 🎥 AutoCaption
 
+```bash
+pip install moviepy
+apt install imagemagick libmagick++-dev
+cat /etc/ImageMagick-6/policy.xml | sed 's/none/read,write/g'> /etc/ImageMagick-6/policy.xml
+```
+
 ```python
-from whisperplus import WhisperAutoCaptionPipeline
+from whisperplus.pipelines.whisper_autocaption import WhisperAutoCaptionPipeline
+from whisperplus import download_youtube_to_mp4
+
+video_path = download_youtube_to_mp4(
+    "https://www.youtube.com/watch?v=di3rHkEZuUw",
+    output_dir="downloads",
+    filename="test",
+)  # Optional
 
 caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
-caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+caption(video_path=video_path, output_path="output.mp4", language="english")
 ```
 
 ## 😍 Contributing
 
 ```bash
-pip install -r dev-requirements.txt
+pip install pre-commit
 pre-commit install
 pre-commit run --all-files
 ```
 
 ## 📜 License
 
 This project is licensed under the terms of the Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,76 +1,89 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.3.3 Summary: WhisperPlus: A
+Metadata-Version: 2.1 Name: whisperplus Version: 0.3.4 Summary: WhisperPlus: A
 Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
 whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
 Apache License 2.0 Description-Content-Type: text/markdown License-File:
 LICENSE
         ********** WWhhiissppeerrPPlluuss:: FFaasstteerr,, SSmmaarrtteerr,, aanndd MMoorree CCaappaabbllee ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
-huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
-ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
-huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
-library, follow the steps below for different tasks: ### ðµ Youtube URL to
-Audio ```python from whisperplus import SpeechToTextPipeline,
-download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
-HqqConfig import torch url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
-audio_path = download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
+## ð ï¸ Installation ```bash pip install git+https://github.com/huggingface/
+transformers pip install flash-attn --no-build-isolation ``` ## ð¤ Model Hub
+You can find the models on the [HuggingFace Model Hub](https://huggingface.co/
+models?search=whisper) ## ðï¸ Usage To use the whisperplus library, follow
+the steps below for different tasks: ### ðµ Youtube URL to Audio ```python
+from whisperplus import SpeechToTextPipeline, download_youtube_to_mp3 from
+transformers import BitsAndBytesConfig, HqqConfig import torch url = "https://
+www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_youtube_to_mp3(url,
+output_dir="downloads", filename="test") hqq_config = HqqConfig( nbits=4,
 group_size=64, quant_zero=False, quant_scale=False, axis=0, offload_meta=False,
 ) # axis=0 is used by default bnb_config = BitsAndBytesConfig
 ( load_in_4bit=True, bnb_4bit_quant_type="nf4",
 bnb_4bit_compute_dtype=torch.bfloat16, bnb_4bit_use_double_quant=True, )
 pipeline = SpeechToTextPipeline( model_id="distil-whisper/distil-large-v3",
 quant_config=hqq_config, hqq=True, flash_attention_2=True, ) transcript =
 pipeline( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
 max_new_tokens=128, batch_size=100, language="english",
 return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
-```python from whisperplus import TextSummarizationPipeline summarizer =
-TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
-summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
-Long Text Support Summarization ```python from whisperplus import
+```python from whisperplus.pipelines.summarization import
+TextSummarizationPipeline summarizer = TextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
+print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
+```python from whisperplus.pipelines.long_text_summarization import
 LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
 (model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
-(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
-from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
-format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
-www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
+(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization You must
+confirm the licensing permissions of these two models. - https://
+huggingface.co/pyannote/speaker-diarization-3.1 - https://huggingface.co/
+pyannote/segmentation-3.0 ```bash pip install -r speaker_diarization.txt pip
+install -U "huggingface_hub[cli]" huggingface-cli login ``` ```python from
+whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline from
+whisperplus import download_youtube_to_mp3, format_speech_to_dialogue
+audio_path = download_youtube_to_mp3("https://www.youtube.com/
+watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
 ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
-diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
+diarizer_model="pyannote/speaker-diarization-3.1", use_auth_token=False,
 chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
 num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
 format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
-with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
-ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
-llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
-v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
-transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
-= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
-(AutoLLM) ```python from whisperplus import AutoLLMChatWithVideo #
-service_context_params system_prompt = """ You are an friendly ai assistant
-that help users find the most relevant and accurate answers to their questions
-based on the documents you have access to. When answering the questions, mostly
-rely on the info in documents. """ query_wrapper_prompt = """ The document
-information is below. --------------------- {context_str} --------------------
-- Using the document information and mostly relying on it, answer the query.
-Query: {query_str} Answer: """ chat = AutoLLMChatWithVideo
-( input_file="input_dir", # path of mp3 file openai_key="YOUR_OPENAI_KEY", #
-optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
-turbo", llm_max_tokens="256", llm_temperature="0.1",
-system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
-embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
-= "what is this video about ?" response = chat.run_query(query) print(response)
-``` ### ðï¸ Speech to Text ```python from whisperplus import
-TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
-tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ### ð¥
-AutoCaption ```python from whisperplus import WhisperAutoCaptionPipeline
+with Video(LanceDB) ```bash pip install sentence-transformers ctransformers
+langchain ``` ```python from whisperplus.pipelines.chatbot import ChatWithVideo
+chat = ChatWithVideo( input_file="trascript.txt", llm_model_name="TheBloke/
+Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf",
+llm_model_type="mistral", embedding_model_name="sentence-transformers/all-
+MiniLM-L6-v2", ) query = "what is this video about ?" response = chat.run_query
+(query) print(response) ``` ### ð  RAG - Chat with Video(AutoLLM) ```bash pip
+install autollm>=0.1.9 ``` ```python from whisperplus.pipelines.autollm_chatbot
+import AutoLLMChatWithVideo # service_context_params system_prompt = """ You
+are an friendly ai assistant that help users find the most relevant and
+accurate answers to their questions based on the documents you have access to.
+When answering the questions, mostly rely on the info in documents. """
+query_wrapper_prompt = """ The document information is below. -----------------
+---- {context_str} --------------------- Using the document information and
+mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
+AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
+openai_key="YOUR_OPENAI_KEY", # optional
+huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
+llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
+query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
+large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
+response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
+```python from whisperplus.pipelines.text2speech import TextToSpeechPipeline
+tts = TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello
+World", voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```bash pip
+install moviepy apt install imagemagick libmagick++-dev cat /etc/ImageMagick-6/
+policy.xml | sed 's/none/read,write/g'> /etc/ImageMagick-6/policy.xml ```
+```python from whisperplus.pipelines.whisper_autocaption import
+WhisperAutoCaptionPipeline from whisperplus import download_youtube_to_mp4
+video_path = download_youtube_to_mp4( "https://www.youtube.com/
+watch?v=di3rHkEZuUw", output_dir="downloads", filename="test", ) # Optional
 caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
-caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
-``` ## ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
-install pre-commit run --all-files ``` ## ð License This project is licensed
-under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
+caption(video_path=video_path, output_path="output.mp4", language="english")
+``` ## ð Contributing ```bash pip install pre-commit pre-commit install pre-
+commit run --all-files ``` ## ð License This project is licensed under the
+terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
 license} } ```
```

### Comparing `whisperplus-0.3.3/whisperplus.egg-info/SOURCES.txt` & `whisperplus-0.3.4/whisperplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

