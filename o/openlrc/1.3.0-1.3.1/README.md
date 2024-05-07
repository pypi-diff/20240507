# Comparing `tmp/openlrc-1.3.0.tar.gz` & `tmp/openlrc-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-1.3.0.tar", max compression
+gzip compressed data, was "openlrc-1.3.1.tar", max compression
```

## Comparing `openlrc-1.3.0.tar` & `openlrc-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1083 2023-08-11 08:52:51.653235 openlrc-1.3.0/LICENSE
--rw-r--r--   0        0        0      106 2023-08-11 08:52:51.661315 openlrc-1.3.0/openlrc/__init__.py
--rw-r--r--   0        0        0    11309 2024-04-04 05:01:06.668448 openlrc-1.3.0/openlrc/chatbot.py
--rw-r--r--   0        0        0      640 2024-04-03 22:41:13.079458 openlrc-1.3.0/openlrc/cli.py
--rw-r--r--   0        0        0     2932 2024-04-09 10:24:16.345077 openlrc-1.3.0/openlrc/context.py
--rw-r--r--   0        0        0     2293 2024-02-29 03:05:03.448559 openlrc-1.3.0/openlrc/defaults.py
--rw-r--r--   0        0        0     2352 2024-03-29 07:07:40.430771 openlrc-1.3.0/openlrc/exceptions.py
--rw-r--r--   0        0        0    12534 2024-04-09 10:22:46.563501 openlrc-1.3.0/openlrc/gui/home.py
--rw-r--r--   0        0        0     1803 2024-04-03 19:50:52.326151 openlrc-1.3.0/openlrc/gui/pages/1_pricing.py
--rw-r--r--   0        0        0      778 2024-04-03 20:37:45.708579 openlrc-1.3.0/openlrc/gui/pages/2_context.py
--rw-r--r--   0        0        0     2732 2024-04-03 22:24:03.812410 openlrc-1.3.0/openlrc/gui/utils.py
--rw-r--r--   0        0        0      597 2023-08-11 08:52:51.662798 openlrc-1.3.0/openlrc/logger.py
--rw-r--r--   0        0        0    15690 2024-04-09 10:23:19.003854 openlrc-1.3.0/openlrc/openlrc.py
--rw-r--r--   0        0        0     7358 2024-04-07 03:04:25.107647 openlrc-1.3.0/openlrc/opt.py
--rw-r--r--   0        0        0     5705 2024-04-09 09:56:19.521524 openlrc-1.3.0/openlrc/preprocess.py
--rw-r--r--   0        0        0    10549 2024-04-09 10:01:31.480813 openlrc-1.3.0/openlrc/prompter.py
--rw-r--r--   0        0        0    11335 2024-04-09 09:59:22.358134 openlrc-1.3.0/openlrc/subtitle.py
--rw-r--r--   0        0        0     7281 2024-02-17 10:05:29.162227 openlrc-1.3.0/openlrc/transcribe.py
--rw-r--r--   0        0        0    10578 2024-04-09 09:57:03.269769 openlrc-1.3.0/openlrc/translate.py
--rw-r--r--   0        0        0     8526 2024-04-09 09:57:59.552319 openlrc-1.3.0/openlrc/utils.py
--rw-r--r--   0        0        0     1955 2024-04-09 10:22:01.160788 openlrc-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     9226 2024-04-09 10:22:46.235512 openlrc-1.3.0/README.md
--rw-r--r--   0        0        0    10989 1970-01-01 00:00:00.000000 openlrc-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-08-11 08:52:51.653235 openlrc-1.3.1/LICENSE
+-rw-r--r--   0        0        0      106 2023-08-11 08:52:51.661315 openlrc-1.3.1/openlrc/__init__.py
+-rw-r--r--   0        0        0    11568 2024-05-07 08:14:19.723112 openlrc-1.3.1/openlrc/chatbot.py
+-rw-r--r--   0        0        0      640 2024-04-03 22:41:13.079458 openlrc-1.3.1/openlrc/cli.py
+-rw-r--r--   0        0        0     2932 2024-04-09 10:24:16.345077 openlrc-1.3.1/openlrc/context.py
+-rw-r--r--   0        0        0     2293 2024-02-29 03:05:03.448559 openlrc-1.3.1/openlrc/defaults.py
+-rw-r--r--   0        0        0     2352 2024-03-29 07:07:40.430771 openlrc-1.3.1/openlrc/exceptions.py
+-rw-r--r--   0        0        0    12906 2024-04-12 06:14:58.669603 openlrc-1.3.1/openlrc/gui_streamlit/home.py
+-rw-r--r--   0        0        0     1803 2024-04-03 19:50:52.326151 openlrc-1.3.1/openlrc/gui_streamlit/pages/1_pricing.py
+-rw-r--r--   0        0        0      778 2024-04-03 20:37:45.708579 openlrc-1.3.1/openlrc/gui_streamlit/pages/2_context.py
+-rw-r--r--   0        0        0     2732 2024-04-03 22:24:03.812410 openlrc-1.3.1/openlrc/gui_streamlit/utils.py
+-rw-r--r--   0        0        0      597 2023-08-11 08:52:51.662798 openlrc-1.3.1/openlrc/logger.py
+-rw-r--r--   0        0        0    16525 2024-05-07 08:04:15.351803 openlrc-1.3.1/openlrc/openlrc.py
+-rw-r--r--   0        0        0     7358 2024-04-07 03:04:25.107647 openlrc-1.3.1/openlrc/opt.py
+-rw-r--r--   0        0        0     5705 2024-04-09 09:56:19.521524 openlrc-1.3.1/openlrc/preprocess.py
+-rw-r--r--   0        0        0    10615 2024-04-16 08:42:01.093831 openlrc-1.3.1/openlrc/prompter.py
+-rw-r--r--   0        0        0    11088 2024-04-17 03:08:26.389069 openlrc-1.3.1/openlrc/subtitle.py
+-rw-r--r--   0        0        0     7281 2024-05-01 08:23:39.842300 openlrc-1.3.1/openlrc/transcribe.py
+-rw-r--r--   0        0        0    10822 2024-05-07 08:06:15.789287 openlrc-1.3.1/openlrc/translate.py
+-rw-r--r--   0        0        0     8526 2024-04-09 09:57:59.552319 openlrc-1.3.1/openlrc/utils.py
+-rw-r--r--   0        0        0     2012 2024-05-07 08:54:50.025641 openlrc-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    10626 2024-05-07 08:40:44.392314 openlrc-1.3.1/README.md
+-rw-r--r--   0        0        0    12392 1970-01-01 00:00:00.000000 openlrc-1.3.1/PKG-INFO
```

### Comparing `openlrc-1.3.0/LICENSE` & `openlrc-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/chatbot.py` & `openlrc-1.3.1/openlrc/chatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,28 +130,30 @@
 
         return results
 
 
 @_register_chatbot
 class GPTBot(ChatBot):
     def __init__(self, model='gpt-3.5-turbo-0125', temperature=1, top_p=1, retry=8, max_async=16, json_mode=False,
-                 fee_limit=0.05, proxy=None):
+                 fee_limit=0.05, proxy=None, base_url_config=None):
         # Pricing for 1M tokens, info from https://openai.com/pricing
         pricing = {
             'gpt-3.5-turbo-0125': (0.5, 1.5),
             'gpt-3.5-turbo': (0.5, 1.5),
             'gpt-4-0125-preview': (10, 30),
             'gpt-4-turbo-preview': (10, 30)
         }
 
         super().__init__(pricing, temperature, top_p, retry, max_async, fee_limit)
 
-        self.async_client = AsyncGPTClient(api_key=os.environ['OPENAI_API_KEY'], http_client=httpx.AsyncClient(
-            proxies=proxy,
-        ))
+        self.async_client = AsyncGPTClient(
+            api_key=os.environ['OPENAI_API_KEY'],
+            http_client=httpx.AsyncClient(proxies=proxy),
+            base_url=base_url_config['openai'] if base_url_config else None
+        )
 
         self.model = model
         self.temperature = temperature
         self.top_p = top_p
         self.retry = retry
         self.max_async = max_async
         self.json_mode = json_mode
@@ -211,27 +213,31 @@
 
         return response
 
 
 @_register_chatbot
 class ClaudeBot(ChatBot):
     def __init__(self, model='claude-3-sonnet-20240229', temperature=1, top_p=1, retry=8, max_async=16, fee_limit=0.2,
-                 proxy=None):
+                 proxy=None, base_url_config=None):
         # Pricing for 1M tokens, info from https://docs.anthropic.com/claude/docs/models-overview#model-comparison
         pricing = {
             'claude-3-opus-20240229': (15, 75),
             'claude-3-sonnet-20240229': (3, 15),
             'claude-3-haiku-20240307': (0.25, 1.25)
         }
 
         super().__init__(pricing, temperature, top_p, retry, max_async, fee_limit)
 
-        self.async_client = AsyncAnthropic(api_key=os.environ['ANTHROPIC_API_KEY'], http_client=httpx.AsyncClient(
-            proxies=proxy,
-        ))
+        self.async_client = AsyncAnthropic(
+            api_key=os.environ['ANTHROPIC_API_KEY'],
+            http_client=httpx.AsyncClient(
+                proxies=proxy
+            ),
+            base_url=base_url_config['anthropic'] if base_url_config else None
+        )
 
         self.model = model
         self.retry = retry
         self.max_async = max_async
         self.fee_limit = fee_limit
 
     def update_fee(self, response: Message):
```

### Comparing `openlrc-1.3.0/openlrc/cli.py` & `openlrc-1.3.1/openlrc/cli.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/context.py` & `openlrc-1.3.1/openlrc/context.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/defaults.py` & `openlrc-1.3.1/openlrc/defaults.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/exceptions.py` & `openlrc-1.3.1/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/gui/home.py` & `openlrc-1.3.1/openlrc/gui_streamlit/home.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import streamlit as st
 from st_pages import Page, show_pages
 from streamlit_extras.bottom_container import bottom
 from streamlit_extras.mention import mention
 
 from openlrc import LRCer
-from openlrc.gui.utils import get_asr_options, get_vad_options, get_preprocess_options, zip_files
+from openlrc.gui_streamlit.utils import get_asr_options, get_vad_options, get_preprocess_options, zip_files
 
 show_pages([
     Page("home.py", "Home", "🏠"),
 ])
 
 with bottom():
     pass
@@ -31,44 +31,51 @@
     url="https://github.com/zh-plus/openlrc",
 )
 
 # Sidebar - Normal Configuration
 st.sidebar.header('Configuration')
 
 with st.sidebar.popover("API Keys"):
-    openai_api_key = st.text_input("OpenAI API Key", value=os.environ.get('OPENAI_API_KEY'))
-    anthropic_api_key = st.text_input("Anthropic API Key", value=os.environ.get('ANTHROPIC_API_KEY'))
+    openai_api_key = st.text_input("OpenAI API Key", value=os.environ.get('OPENAI_API_KEY'), key='openai_api')
+    anthropic_api_key = st.text_input("Anthropic API Key", value=os.environ.get('ANTHROPIC_API_KEY'),
+                                      key='anthropic_api')
 
 whisper_model = st.sidebar.selectbox('Whisper Model',
                                      ['large-v3', 'medium', 'medium.en', 'small', 'small.en', 'base', 'base.en', 'tiny',
-                                      'tiny.en'], index=0)
-compute_type = st.sidebar.selectbox('Compute Type', ['int8', 'int8_float16', 'int16', 'float16', 'float32'], index=3)
+                                      'tiny.en'], index=0, key='whisper_model')
+compute_type = st.sidebar.selectbox('Compute Type', ['int8', 'int8_float16', 'int16', 'float16', 'float32'], index=3
+                                    , key='compute_type')
 
 if not openai_api_key and not anthropic_api_key:
-    chatbot_model = st.sidebar.selectbox('Chatbot Model', [], disabled=True, help="Please provide an API key first.")
+    chatbot_model = st.sidebar.selectbox('Chatbot Model', [], disabled=True, help="Please provide an API key first.",
+                                         key='chatbot_model')
 elif openai_api_key and not anthropic_api_key:
     chatbot_model = st.sidebar.selectbox('Chatbot Model',
                                          ['gpt-3.5-turbo', 'gpt-4-0125-preview', 'gpt-4-turbo-preview'], index=0,
-                                         help="Model for translation. Check [pricing](/pricing) for more details.")
+                                         help="Model for translation. Check [pricing](/pricing) for more details.",
+                                         key='chatbot_model')
 elif not openai_api_key and anthropic_api_key:
     chatbot_model = st.sidebar.selectbox('Chatbot Model', ['claude-3-haiku-20240307', 'claude-3-sonnet-20240229',
                                                            'claude-3-opus-20240229'], index=0,
-                                         help="Model for translation. Check [pricing](/pricing) for more details.")
+                                         help="Model for translation. Check [pricing](/pricing) for more details.",
+                                         key='chatbot_model')
 else:
     chatbot_model = st.sidebar.selectbox('Chatbot Model',
                                          ['gpt-3.5-turbo', 'gpt-4-0125-preview', 'gpt-4-turbo-preview',
                                           'claude-3-haiku-20240307', 'claude-3-sonnet-20240229',
                                           'claude-3-opus-20240229'],
                                          index=0,
-                                         help="Model for translation. Check [pricing](/pricing) for more details.")
+                                         help="Model for translation. Check [pricing](/pricing) for more details.",
+                                         key='chatbot_model')
 
 # fee_limit = st.sidebar.number_input('Fee Limit', min_value=0.0, value=0.1, step=0.01)
-fee_limit = st.sidebar.slider('Fee Limit (USD)', min_value=0.0, max_value=1.0, value=0.1, step=0.01)
-consumer_thread = st.sidebar.slider('Consumer Thread', min_value=1, max_value=12, value=4, step=1)
-proxy = st.sidebar.text_input('Proxy', help='e.g.: http://127.0.0.1:7890')
+fee_limit = st.sidebar.slider('Fee Limit (USD)', min_value=0.0, max_value=1.0, value=0.1, step=0.01, key='fee_limit')
+consumer_thread = st.sidebar.slider('Consumer Thread', min_value=1, max_value=12, value=4, step=1,
+                                    key='consumer_thread')
+proxy = st.sidebar.text_input('Proxy', help='e.g.: http://127.0.0.1:7890', key='proxy')
 
 # Sidebar: Advanced Configuration
 with st.sidebar.expander("Advanced Configuration", expanded=False):
     st.write("### ASR Options")
     # ASR Options with help messages
     beam_size = st.number_input("Beam Size", value=3, min_value=1, help="Sets the beam size for the ASR.")
     best_of = st.number_input("Best of", value=5, min_value=1, help="Chooses the best result from N beams.")
@@ -144,17 +151,15 @@
     src_lang = st.selectbox("Source Language",
                             options=['Auto Detect', 'ca', 'zh', 'hr', 'da', 'nl', 'en', 'fi', 'fr', 'de', 'el', 'it',
                                      'ja', 'ko', 'lt', 'mk', 'nb', 'pl', 'pt', 'ro', 'ru', 'sl', 'es', 'sv', 'uk'],
                             index=0,
                             format_func=lambda x: 'Auto Detect' if x == 'Auto Detect' else x.upper(),
                             help='Currently bottleneck-ed by Spacy')
     target_lang = st.text_input("Target Language", value='zh-cn', help='Language code for translation target')
-    prompter = st.selectbox("Prompter", options=['base_trans'],
-                            format_func=lambda x: 'Base' if x == 'base_trans' else 'Advanced', disabled=True,
-                            help='Currently, only `base_trans` is supported.')
+    prompter = st.selectbox("Prompter", options=['base'], disabled=True, help='Currently, only `base` is supported.')
     context_path = st.text_input("Context Path",
                                  help='Additional context to aid translation. Check [context](/context) for more details. ')
 
     col1, col2, col3 = st.columns(3)
     with col1:
         skip_trans = st.checkbox("Skip Translation")
     with col2:
```

### Comparing `openlrc-1.3.0/openlrc/gui/pages/1_pricing.py` & `openlrc-1.3.1/openlrc/gui_streamlit/pages/1_pricing.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/gui/pages/2_context.py` & `openlrc-1.3.1/openlrc/gui_streamlit/pages/2_context.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/gui/utils.py` & `openlrc-1.3.1/openlrc/gui_streamlit/utils.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/logger.py` & `openlrc-1.3.1/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/openlrc.py` & `openlrc-1.3.1/openlrc/openlrc.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from faster_whisper.transcribe import Segment
 
 from openlrc.context import Context
 from openlrc.defaults import default_asr_options, default_vad_options, default_preprocess_options
 from openlrc.logger import logger
 from openlrc.opt import SubtitleOptimizer
 from openlrc.preprocess import Preprocessor
-from openlrc.subtitle import Subtitle
+from openlrc.subtitle import Subtitle, BilingualSubtitle
 from openlrc.transcribe import Transcriber
 from openlrc.translate import LLMTranslator
 from openlrc.utils import Timer, extend_filename, get_audio_duration, format_timestamp, extract_audio, \
     get_file_type
 
 
 class LRCer:
@@ -37,25 +37,29 @@
             Anthropic: claude-3-opus-20240229, claude-3-sonnet-20240229, claude-3-haiku-20240307
             Default: ``gpt-3.5-turbo``
         fee_limit: The maximum fee you are willing to pay for one translation call. Default: ``0.1``
         consumer_thread: To prevent exceeding the RPM and TPM limits set by OpenAI, the default is TPM/MAX_TOKEN.
         asr_options: Parameters for whisper model.
         vad_options: Parameters for VAD model.
         proxy: Proxy for openai requests. e.g. 'http://127.0.0.1:7890'
+        base_url_config: Base URL dict for OpenAI & Anthropic.
+            e.g. {'openai': 'https://openai.justsong.cn/', 'anthropic': 'https://api.g4f.icu'}
+            Default: ``None``
     """
 
     def __init__(self, whisper_model='large-v3', compute_type='float16', chatbot_model: str = 'gpt-3.5-turbo',
                  fee_limit=0.1, consumer_thread=4, asr_options=None, vad_options=None, preprocess_options=None,
-                 proxy=None):
+                 proxy=None, base_url_config=None):
         self.chatbot_model = chatbot_model
         self.fee_limit = fee_limit
         self.api_fee = 0  # Can be updated in different thread, operation should be thread-safe
         self.from_video = set()
         self.context: Context = Context()
         self.proxy = proxy
+        self.base_url_config = base_url_config
 
         self._lock = Lock()
         self.exception = None
         self.consumer_thread = consumer_thread
 
         # Default Automatic Speech Recognition (ASR) options
         self.asr_options = default_asr_options
@@ -158,25 +162,33 @@
                 subtitle_path = final_subtitle.to_lrc()
 
             suffix = subtitle_path.suffix
             result_path = subtitle_path.parents[1] / subtitle_path.name.replace(f'_preprocessed{suffix}',
                                                                                 suffix)
             shutil.copy(subtitle_path, result_path)
 
+            # Bilingual
+            if bilingual_sub:
+                bilingual_subtitle = BilingualSubtitle.from_preprocessed(transcribed_path.parent,
+                                                                         audio_name.replace('_preprocessed', ''))
+                bilingual_subtitle.to_lrc()
+                bilingual_lrc_path = bilingual_subtitle.filename.with_suffix(bilingual_subtitle.suffix)
+                shutil.copy(bilingual_lrc_path, result_path.parent / bilingual_lrc_path.name)
+
             logger.info(f'Translation fee til now: {self.api_fee:.4f} USD')
 
             self.transcribed_paths.append(result_path)
 
     def _translate(self, audio_name, prompter, target_lang, transcribed_opt_sub, translated_path):
         json_filename = Path(translated_path.parent / (audio_name + '.json'))
         compare_path = Path(translated_path.parent, f'{audio_name}_compare.json')
         if not translated_path.exists():
             # Translate the transcribed json
             translator = LLMTranslator(chatbot_model=self.chatbot_model, prompter=prompter, fee_limit=self.fee_limit,
-                                       proxy=self.proxy)
+                                       proxy=self.proxy, base_url_config=self.base_url_config)
             context = self.context
 
             target_texts = translator.translate(
                 transcribed_opt_sub.texts,
                 src_lang=transcribed_opt_sub.lang,
                 target_lang=target_lang,
                 title=audio_name,
```

### Comparing `openlrc-1.3.0/openlrc/opt.py` & `openlrc-1.3.1/openlrc/opt.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/preprocess.py` & `openlrc-1.3.1/openlrc/preprocess.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/openlrc/prompter.py` & `openlrc-1.3.1/openlrc/prompter.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,16 @@
         # If message is for claude, use messages[0]
         user_input = messages[1]['content'] if len(messages) == 2 else messages[0]['content']
 
         original = re.findall(r'Original>\n(.*?)\nTranslation>', user_input, re.DOTALL)
         translation = re.findall(r'Translation>\n*(.*?)(?:#\d+|<summary>|\n*$)', content, re.DOTALL)
 
         if not original or not translation:
+            # TODO: Try to change chatbot_model if always fail
+
             logger.warning(f'Fail to extract original or translation.')
             logger.debug(f'Content: {content}')
             return False
 
         if len(original) != len(translation):
             logger.warning(
                 f'Fail to ensure length consistent: original is {len(original)}, translation is {len(translation)}')
```

### Comparing `openlrc-1.3.0/openlrc/subtitle.py` & `openlrc-1.3.1/openlrc/subtitle.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         for i, text in enumerate(texts):
             self.segments[i].text = text
 
         if lang:
             self.lang = lang
 
-    def save(self, filename, update_name=False):
+    def save(self, filename: Union[str, Path], update_name=False):
         results = {
             'language': self.lang,
             'segments': [seg.to_json() for seg in self.segments]
         }
 
         with open(filename, 'w', encoding='utf-8') as f:
             json.dump(results, f, ensure_ascii=False, indent=4)
@@ -259,43 +259,38 @@
                     f'Source and target subtitle start time not equal: {src_seg.start} vs {target_seg.start}')
             self.segments.append(BilingualElement(src_seg.start, src_seg.end, src_seg.text, target_seg.text))
 
         self.filename = Path(filename)
         self.suffix = '.lrc'
 
     @classmethod
-    def from_preprocessed(cls, audio_name: Union[str, Path]):
-        audio_name = Path(audio_name)
-        preprocess_dir = audio_name.parent / 'preprocessed'
-
-        src_file = preprocess_dir / f'{audio_name.stem}_preprocessed_transcribed_optimized.json'
-        target_file = preprocess_dir / f'{audio_name.stem}_preprocessed_transcribed_optimized_translated.json'
+    def from_preprocessed(cls, preprocessed_folder, audio_name):
+        src_file = preprocessed_folder / f'{audio_name}_preprocessed_transcribed_optimized.json'
+        target_file = preprocessed_folder / f'{audio_name}_preprocessed_transcribed_optimized_translated.json'
 
         if not src_file.exists() or not target_file.exists():
             raise ValueError(f'Preprocessed file not found for {audio_name}')
 
         src_sub = Subtitle.from_json(src_file)
         target_sub = Subtitle.from_json(target_file)
 
-        bilingual_sub_name = preprocess_dir / f'{audio_name.stem}_bilingual.json'
+        bilingual_sub_name = preprocessed_folder / f'{audio_name}_bilingual.json'
 
         return cls(src_sub, target_sub, filename=bilingual_sub_name)
 
     def to_lrc(self):
         # If duration larger than 1 hour, use srt file instead
         if self.segments[-1].end >= 3600:
             logger.warning('Duration larger than 1 hour, use srt file instead')
             self.to_srt()
             return self.filename.with_suffix('.srt')
 
         lrc_path = self.filename.with_suffix('.lrc')
         fmt = partial(format_timestamp, fmt='lrc')
         with open(lrc_path, 'w', encoding='utf-8') as f:
-            print(f'# Bilingual LRC generated by openlrc.', file=f, flush=True)
-
             for i, segment in enumerate(self.segments):
                 print(
                     f'[{fmt(segment.start)}] {segment.target_text.strip()}\n[{fmt(segment.start)}] {segment.src_text.strip()}',
                     file=f,
                     flush=True,
                 )
                 if i == len(self.segments) - 1 or segment.end != self.segments[i + 1].start:
@@ -303,16 +298,14 @@
 
         logger.info(f'File saved to {lrc_path}')
 
     def to_srt(self):
         srt_path = self.filename.with_suffix('.srt')
         fmt = partial(format_timestamp, fmt='srt')
         with open(srt_path, 'w', encoding='utf-8') as f:
-            print(f'# Bilingual SRT generated by openlrc.', file=f, flush=True)
-
             for i, segment in enumerate(self.segments, start=1):
                 print(f'{i}\n'
                       f'{fmt(segment.start)} --> {fmt(segment.end)}\n'
                       f'{segment.target_text.strip()}\n'
                       f'{segment.src_text.strip()}\n', file=f, flush=True)
 
         logger.info(f'File saved to {srt_path}')
```

### Comparing `openlrc-1.3.0/openlrc/transcribe.py` & `openlrc-1.3.1/openlrc/transcribe.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                     continue
 
                 word_start += len(split_words)
 
                 entry = seg_from_words(segment, id_cnt, split_words,
                                        segment.tokens[word_start: word_start + len(split_words)])
 
-                if len(split) < (50 if lang in self.non_word_boundary else 150):
+                if len(split) < (50 if lang in self.non_word_boundary else 100):
                     sentences.append(entry)
                     id_cnt += 1
                 else:
                     # Split them in the middle
                     origin_len = len(sentences)
                     sentences.extend(mid_split(entry))
                     id_cnt += (len(sentences) - origin_len)
```

### Comparing `openlrc-1.3.0/openlrc/translate.py` & `openlrc-1.3.1/openlrc/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,32 +22,35 @@
     @abstractmethod
     def translate(self, texts: Union[str, List[str]], src_lang, target_lang):
         pass
 
 
 class LLMTranslator(Translator):
     def __init__(self, chatbot_model: str = 'gpt-3.5-turbo', prompter: str = 'base_trans', fee_limit=0.1,
-                 chunk_size=30, intercept_line=None, proxy=None):
+                 chunk_size=30, intercept_line=None, proxy=None, base_url_config=None):
         """
         Args:
             chatbot_model: Chatbot instance. Choices can be found using `LLMTranslator().list_chatbots()`.
             prompter: Translate prompter instance. Choices can be found in `prompter_map` from `prompter.py`.
             fee_limit (float): Fee limit (USD) for the OpenAI API.
             chunk_size (int): Use a small chunk size (<20) for speed (more asynchronous calls) and to enhance translation
                               stability (keeping audio timeline consistency).
             intercept_line (int): Intercepted text line number.
+            proxy (str): Proxy server. e.g. http://127.0.0.1:7890
+            base_url_config (dict): Base URL configuration for the chatbot API.
         """
         if prompter not in prompter_map:
             raise ValueError(f'Prompter {prompter} not found.')
 
         if chatbot_model not in model2chatbot.keys():
             raise ValueError(f'Chatbot {chatbot_model} not supported.')
 
         chatbot_category = chatbot_map[model2chatbot[chatbot_model]]
-        self.chatbot = chatbot_category(model=chatbot_model, fee_limit=fee_limit, proxy=proxy, temperature=0.7)
+        self.chatbot = chatbot_category(model=chatbot_model, fee_limit=fee_limit, proxy=proxy, temperature=0.7,
+                                        base_url_config=base_url_config)
 
         self.prompter = prompter
         self.fee_limit = fee_limit
         self.chunk_size = chunk_size
         self.api_fee = 0
         self.intercept_line = intercept_line
         self.proxy = proxy
```

### Comparing `openlrc-1.3.0/openlrc/utils.py` & `openlrc-1.3.1/openlrc/utils.py`

 * *Files identical despite different names*

### Comparing `openlrc-1.3.0/pyproject.toml` & `openlrc-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "1.3.0"
+version = "1.3.1"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
@@ -28,14 +28,17 @@
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
     "Operating System :: OS Independent",
 ]
 include = [
     { path = 'openlrc' },
 ]
+exclude = [
+    "openlrc/gui"
+]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9.7 || >3.9.7,<4.0"
 openai = "^1.1.1"
 anthropic = "^0.18.1"
 tiktoken = "^0.6.0"
 langcodes = "^3.3.0"
@@ -52,16 +55,18 @@
 jaconvV2 = "^0.4"
 spacy = "^3.5.4"
 pysbd = "^0.3.4"
 faster-whisper = "^1.0.0"
 soundfile = "^0.12.1"
 ffmpeg-normalize = "^1.27.5"
 deepfilternet = "^0.5.6"
-aiohttp = "^3.8.5"
-streamlit = "^1.32.2"
+aiohttp = "^3.9.4"
+ctranslate2 = "4.2.1"
+gradio = "^4.26.0"
+
 #torch = ">=2.0.0, !=2.0.1"
 #torchaudio = "^2.0.0"
 #torchvision = "^0.17.1"
 #torch = { version = "2.0.1", source = "torch" }
 #torchaudio = { version = "2.0.2", source = "torch" }
 #torchvision = { version = "0.15.2", source = "torch" }
```

### Comparing `openlrc-1.3.0/README.md` & `openlrc-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,40 @@
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/zh-plus/Open-Lyrics/ci.yml)
 
 Open-Lyrics is a Python library that transcribes voice files using
 [faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
 into `.lrc` files in the desired language using LLM,
 e.g. [OpenAI-GPT](https://github.com/openai/openai-python), [Anthropic-Claude](https://github.com/anthropics/anthropic-sdk-python).
 
+#### Key Features:
+
+- Well preprocessed audio to reduce hallucination (Loudness Norm & optional Noise Suppression).
+- Context-aware translation to improve translation quality.
+  Check [prompt](https://github.com/zh-plus/openlrc/blob/master/openlrc/prompter.py) for details.
+
 ## New 🚨
 
 - 2024.3.29: Claude models are now available for translation. According to the testing, Claude 3 Sonnet performs way
   better than GPT-3.5 Turbo. We recommend using Claude 3 Sonnet for non-english audio (source language) translation (For
   now, the default model
   are still GPT-3.5 Turbo):
     ```python
     lrcer = LRCer(chatbot_model='claude-3-sonnet-20240229')
     ```
 - 2024.4.4: Add basic streamlit GUI support. Try `openlrc gui` to start the GUI.
+- 2024.5.7:
+    - Add custom endpoint (base_url) support for OpenAI & Anthropic:
+        ```python
+        lrcer = LRCer(base_url_config={'openai': 'https://api.chatanywhere.tech',
+                                       'anthropic': 'https://api.g4f.icu'})
+        ```
+    - Generating bilingual subtitles
+        ```python
+        lrcer.run('./data/test.mp3', target_lang='zh-cn', bilingual_sub=True)
+        ``` 
 
 ## Installation ⚙️
 
 1. Please install CUDA 11.x and [cuDNN 8 for CUDA 11](https://developer.nvidia.com/cudnn) first according
    to https://opennmt.net/CTranslate2/installation.html to enable `faster-whisper`.
 
    `faster-whisper` also needs [cuBLAS for CUDA 11](https://developer.nvidia.com/cublas) installed.
@@ -62,21 +78,24 @@
     ```shell
     pip install openlrc
     ```
 
    or install directly from GitHub:
 
     ```shell
-    pip install git+https://github.com/zh-plus/Open-Lyrics
+    pip install git+https://github.com/zh-plus/openlrc
     ```
 
 ## Usage 🐍
 
 ### GUI
 
+> [!NOTE]
+> We are migrating the GUI from streamlit to Gradio. The GUI is still under development.
+
 ```shell
 openlrc gui
 ```
 
 ![](https://github.com/zh-plus/openlrc/blob/master/resources/streamlit_app.jpg?raw=true)
 
 ### Python code
@@ -112,14 +131,24 @@
 
     # Enhance the audio using noise suppression (consume more time).
     lrcer.run('./data/test.mp3', target_lang='zh-cn', noise_suppress=True)
 
     # Change the LLM model for translation
     lrcer = LRCer(chatbot_model='claude-3-sonnet-20240229')
     lrcer.run('./data/test.mp3', target_lang='zh-cn')
+
+    # Clear temp folder after processing done
+    lrcer.run('./data/test.mp3', target_lang='zh-cn', clear_temp_folder=True)
+
+    # Change base_url
+    lrcer = LRCer(base_url_config={'openai': 'https://api.chatanywhere.tech',
+                                   'anthropic': 'https://api.g4f.icu'})
+
+    # Bilingual subtitle
+    lrcer.run('./data/test.mp3', target_lang='zh-cn', bilingual_sub=True)
 ```
 
 Check more details in [Documentation](https://zh-plus.github.io/openlrc/#/).
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
@@ -188,14 +217,16 @@
 - [X] [Feature] Multiple translate engine (Anthropic, Microsoft, DeepL, Google, etc.) support.
 - [ ] [**Feature**] Build
   a [electron + fastapi](https://ivanyu2021.hashnode.dev/electron-django-desktop-app-integrate-javascript-and-python)
   GUI for cross-platform application.
 - [x] [Feature] Web-based [streamlit](https://streamlit.io/) GUI.
 - [ ] Add [fine-tuned whisper-large-v2](https://huggingface.co/models?search=whisper-large-v2) models for common
   languages.
+- [x] [Feature] Add custom OpenAI & Anthropic endpoint support.
+- [ ] [Feature] Add local translation model support (e.g. [SakuraLLM](https://github.com/SakuraLLM/Sakura-13B-Galgame)).
 - [ ] [Others] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 
 ## Credits
```

### Comparing `openlrc-1.3.0/PKG-INFO` & `openlrc-1.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 1.3.0
+Version: 1.3.1
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
@@ -14,34 +14,35 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: anthropic (>=0.18.1,<0.19.0)
 Requires-Dist: audioread (>=3.0.0,<4.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
+Requires-Dist: ctranslate2 (==4.2.1)
 Requires-Dist: deepfilternet (>=0.5.6,<0.6.0)
 Requires-Dist: faster-whisper (>=1.0.0,<2.0.0)
 Requires-Dist: ffmpeg-normalize (>=1.27.5,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
+Requires-Dist: gradio (>=4.26.0,<5.0.0)
 Requires-Dist: jaconvV2 (>=0.4,<0.5)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: lingua-language-detector (>=1.3.2,<2.0.0)
 Requires-Dist: openai (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: punctuators (>=0.0.5,<0.0.6)
 Requires-Dist: pysbd (>=0.3.4,<0.4.0)
 Requires-Dist: soundfile (>=0.12.1,<0.13.0)
 Requires-Dist: spacy (>=3.5.4,<4.0.0)
-Requires-Dist: streamlit (>=1.32.2,<2.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: zhconv (>=1.4.3,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Description-Content-Type: text/markdown
 
 # Open-Lyrics
@@ -52,24 +53,40 @@
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/zh-plus/Open-Lyrics/ci.yml)
 
 Open-Lyrics is a Python library that transcribes voice files using
 [faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
 into `.lrc` files in the desired language using LLM,
 e.g. [OpenAI-GPT](https://github.com/openai/openai-python), [Anthropic-Claude](https://github.com/anthropics/anthropic-sdk-python).
 
+#### Key Features:
+
+- Well preprocessed audio to reduce hallucination (Loudness Norm & optional Noise Suppression).
+- Context-aware translation to improve translation quality.
+  Check [prompt](https://github.com/zh-plus/openlrc/blob/master/openlrc/prompter.py) for details.
+
 ## New 🚨
 
 - 2024.3.29: Claude models are now available for translation. According to the testing, Claude 3 Sonnet performs way
   better than GPT-3.5 Turbo. We recommend using Claude 3 Sonnet for non-english audio (source language) translation (For
   now, the default model
   are still GPT-3.5 Turbo):
     ```python
     lrcer = LRCer(chatbot_model='claude-3-sonnet-20240229')
     ```
 - 2024.4.4: Add basic streamlit GUI support. Try `openlrc gui` to start the GUI.
+- 2024.5.7:
+    - Add custom endpoint (base_url) support for OpenAI & Anthropic:
+        ```python
+        lrcer = LRCer(base_url_config={'openai': 'https://api.chatanywhere.tech',
+                                       'anthropic': 'https://api.g4f.icu'})
+        ```
+    - Generating bilingual subtitles
+        ```python
+        lrcer.run('./data/test.mp3', target_lang='zh-cn', bilingual_sub=True)
+        ``` 
 
 ## Installation ⚙️
 
 1. Please install CUDA 11.x and [cuDNN 8 for CUDA 11](https://developer.nvidia.com/cudnn) first according
    to https://opennmt.net/CTranslate2/installation.html to enable `faster-whisper`.
 
    `faster-whisper` also needs [cuBLAS for CUDA 11](https://developer.nvidia.com/cublas) installed.
@@ -108,21 +125,24 @@
     ```shell
     pip install openlrc
     ```
 
    or install directly from GitHub:
 
     ```shell
-    pip install git+https://github.com/zh-plus/Open-Lyrics
+    pip install git+https://github.com/zh-plus/openlrc
     ```
 
 ## Usage 🐍
 
 ### GUI
 
+> [!NOTE]
+> We are migrating the GUI from streamlit to Gradio. The GUI is still under development.
+
 ```shell
 openlrc gui
 ```
 
 ![](https://github.com/zh-plus/openlrc/blob/master/resources/streamlit_app.jpg?raw=true)
 
 ### Python code
@@ -158,14 +178,24 @@
 
     # Enhance the audio using noise suppression (consume more time).
     lrcer.run('./data/test.mp3', target_lang='zh-cn', noise_suppress=True)
 
     # Change the LLM model for translation
     lrcer = LRCer(chatbot_model='claude-3-sonnet-20240229')
     lrcer.run('./data/test.mp3', target_lang='zh-cn')
+
+    # Clear temp folder after processing done
+    lrcer.run('./data/test.mp3', target_lang='zh-cn', clear_temp_folder=True)
+
+    # Change base_url
+    lrcer = LRCer(base_url_config={'openai': 'https://api.chatanywhere.tech',
+                                   'anthropic': 'https://api.g4f.icu'})
+
+    # Bilingual subtitle
+    lrcer.run('./data/test.mp3', target_lang='zh-cn', bilingual_sub=True)
 ```
 
 Check more details in [Documentation](https://zh-plus.github.io/openlrc/#/).
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
@@ -234,14 +264,16 @@
 - [X] [Feature] Multiple translate engine (Anthropic, Microsoft, DeepL, Google, etc.) support.
 - [ ] [**Feature**] Build
   a [electron + fastapi](https://ivanyu2021.hashnode.dev/electron-django-desktop-app-integrate-javascript-and-python)
   GUI for cross-platform application.
 - [x] [Feature] Web-based [streamlit](https://streamlit.io/) GUI.
 - [ ] Add [fine-tuned whisper-large-v2](https://huggingface.co/models?search=whisper-large-v2) models for common
   languages.
+- [x] [Feature] Add custom OpenAI & Anthropic endpoint support.
+- [ ] [Feature] Add local translation model support (e.g. [SakuraLLM](https://github.com/SakuraLLM/Sakura-13B-Galgame)).
 - [ ] [Others] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 
 ## Credits
```

