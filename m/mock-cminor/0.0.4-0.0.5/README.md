# Comparing `tmp/mock_cminor-0.0.4.tar.gz` & `tmp/mock_cminor-0.0.5.tar.gz`

## Comparing `mock_cminor-0.0.4.tar` & `mock_cminor-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/src/mock_cminor/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/src/mock_cminor/__version__.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/src/mock_cminor/adaptor.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/src/mock_cminor/analyzers.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/src/mock_cminor/generator.py
--rw-r--r--   0        0        0  1828815 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/src/mock_cminor/get_results.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/src/mock_cminor/utils.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/LICENCE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/README.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 mock_cminor-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/src/mock_cminor/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/src/mock_cminor/__version__.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/src/mock_cminor/adaptor.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/src/mock_cminor/analyzers.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/src/mock_cminor/generator.py
+-rw-r--r--   0        0        0  1856332 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/src/mock_cminor/get_results.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/src/mock_cminor/utils.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/LICENCE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 mock_cminor-0.0.5/PKG-INFO
```

### Comparing `mock_cminor-0.0.4/src/mock_cminor/analyzers.py` & `mock_cminor-0.0.5/src/mock_cminor/analyzers.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
     def analyze_catile(self,text,return_result=True,v=1):
         return get_catile()
 
     def analyze_readability(self,text,language="en",return_grades=False,return_result=True):
         return get_readability()
 
+    def analyze_hsk(self,text,outputs=["final_levels"]):
+        return  {}
+
 class AdoVideoAnalyzer:
     def __init__(self, analyser, openai_api_key, temp_dir):
         self.analyser = analyser
         self.openai_api_key = openai_api_key
         self.temp_dir = temp_dir
     
     def get_video_info(self,url):
```

### Comparing `mock_cminor-0.0.4/src/mock_cminor/generator.py` & `mock_cminor-0.0.5/src/mock_cminor/generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,8 +34,11 @@
         
 
     def generate_questions(self, text=None, url=None, words=None, n=10, kind='multiple_choice', skill='reading', level=None, 
                            answer_position=False, explanation=False, question_language=None, explanation_language=None, auto_retry=3,
                            transcribe=False, duration_limit=900):
         
         return get_question_generator()
+
+    def check_answers(self,text, questions, answers, student_answers):
+        return {"correctness": [True,False]}
```

### Comparing `mock_cminor-0.0.4/src/mock_cminor/get_results.py` & `mock_cminor-0.0.5/src/mock_cminor/get_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -63101,8 +63101,1215 @@
         {
             "start": 52.0,
             "end": 57.0,
             "text": "Subscribe to Unconfused Me wherever you listen to podcasts."
         }
     ],
     "speak_duration": 56.0
+    }
+
+def get_hsk():
+    return {
+    "sentences": {
+        "0": {
+            "id": [
+                0,
+                1,
+                2,
+                3,
+                4,
+                5,
+                6,
+                7,
+                8,
+                9,
+                10,
+                11,
+                12,
+                13,
+                14,
+                15,
+                16,
+                17
+            ],
+            "word": [
+                "ä¸€",
+                "ä¸ª",
+                "å§‘å¨˜",
+                "å’Œ",
+                "ä¸€",
+                "ä¸ª",
+                "å°ä¼™å­",
+                "ç»“å©š",
+                "äº†",
+                "ï¼Œ",
+                "ä»–ä»¬",
+                "ç»“å©š",
+                "ä»¥å",
+                "çš„",
+                "ç”Ÿæ´»",
+                "ååˆ†",
+                "å¹¸ç¦",
+                "ã€‚"
+            ],
+            "lemma": [
+                "ä¸€",
+                "ä¸ª",
+                "å§‘å¨˜",
+                "å’Œ",
+                "ä¸€",
+                "ä¸ª",
+                "å°ä¼™å­",
+                "ç»“å©š",
+                "äº†",
+                "ï¼Œ",
+                "ä»–ä»¬",
+                "ç»“å©š",
+                "ä»¥å",
+                "çš„",
+                "ç”Ÿæ´»",
+                "ååˆ†",
+                "å¹¸ç¦",
+                "ã€‚"
+            ],
+            "pos": [
+                "CD",
+                "M",
+                "NN",
+                "P",
+                "CD",
+                "M",
+                "NN",
+                "VV",
+                "AS",
+                "PU",
+                "PN",
+                "VV",
+                "LC",
+                "DEG",
+                "NN",
+                "AD",
+                "VA",
+                "PU"
+            ],
+            "level": [
+                0,
+                0,
+                2,
+                0,
+                0,
+                0,
+                3,
+                2,
+                0,
+                -2,
+                0,
+                2,
+                1,
+                0,
+                1,
+                1,
+                2,
+                -2
+            ]
+        },
+        "1": {
+            "id": [
+                18,
+                19,
+                20,
+                21,
+                22,
+                23,
+                24,
+                25,
+                26,
+                27,
+                28,
+                29,
+                30,
+                31,
+                32,
+                33,
+                34,
+                35,
+                36,
+                37,
+                38,
+                39,
+                40,
+                41,
+                42
+            ],
+            "word": [
+                "å°ä¼™å­",
+                "éå¸¸",
+                "å–œæ¬¢",
+                "è¶³çƒ",
+                "ï¼Œ",
+                "æ¯",
+                "æ¬¡",
+                "ç”µè§†",
+                "ä¸­",
+                "æœ‰",
+                "è¶³çƒ",
+                "æ¯”èµ›",
+                "çš„",
+                "æ—¶å€™",
+                "ï¼Œ",
+                "ä»–",
+                "è¿",
+                "é¥­",
+                "éƒ½",
+                "ä¸",
+                "åƒ",
+                "ä¹Ÿ",
+                "è¦",
+                "çœ‹",
+                "ã€‚"
+            ],
+            "lemma": [
+                "å°ä¼™å­",
+                "éå¸¸",
+                "å–œæ¬¢",
+                "è¶³çƒ",
+                "ï¼Œ",
+                "æ¯",
+                "æ¬¡",
+                "ç”µè§†",
+                "ä¸­",
+                "æœ‰",
+                "è¶³çƒ",
+                "æ¯”èµ›",
+                "çš„",
+                "æ—¶å€™",
+                "ï¼Œ",
+                "ä»–",
+                "è¿",
+                "é¥­",
+                "éƒ½",
+                "ä¸",
+                "åƒ",
+                "ä¹Ÿ",
+                "è¦",
+                "çœ‹",
+                "ã€‚"
+            ],
+            "pos": [
+                "NN",
+                "AD",
+                "VV",
+                "NN",
+                "PU",
+                "DT",
+                "M",
+                "NN",
+                "LC",
+                "VE",
+                "NN",
+                "NN",
+                "DEC",
+                "NN",
+                "PU",
+                "PN",
+                "AD",
+                "NN",
+                "AD",
+                "AD",
+                "VV",
+                "AD",
+                "VV",
+                "VV",
+                "PU"
+            ],
+            "level": [
+                3,
+                0,
+                0,
+                2,
+                -2,
+                2,
+                0,
+                0,
+                0,
+                0,
+                2,
+                2,
+                0,
+                0,
+                -2,
+                0,
+                2,
+                0,
+                0,
+                0,
+                0,
+                0,
+                0,
+                0,
+                -2
+            ]
+        },
+        "2": {
+            "id": [
+                43,
+                44,
+                45,
+                46,
+                47,
+                48,
+                49,
+                50,
+                51,
+                52,
+                53
+            ],
+            "word": [
+                "å¯¹",
+                "æ­¤",
+                "ï¼Œ",
+                "å¹´è½»",
+                "çš„",
+                "å¦»å­",
+                "ä¸€ç‚¹å„¿",
+                "åŠæ³•",
+                "ä¹Ÿ",
+                "æ²¡æœ‰",
+                "ã€‚"
+            ],
+            "lemma": [
+                "å¯¹",
+                "æ­¤",
+                "ï¼Œ",
+                "å¹´è½»",
+                "çš„",
+                "å¦»å­",
+                "ä¸€ç‚¹å„¿",
+                "åŠæ³•",
+                "ä¹Ÿ",
+                "æ²¡æœ‰",
+                "ã€‚"
+            ],
+            "pos": [
+                "P",
+                "PN",
+                "PU",
+                "VA",
+                "DEC",
+                "NN",
+                "CD",
+                "NN",
+                "AD",
+                "VE",
+                "PU"
+            ],
+            "level": [
+                0,
+                3,
+                -2,
+                1,
+                0,
+                3,
+                0,
+                1,
+                0,
+                0,
+                -2
+            ]
+        },
+        "3": {
+            "id": [
+                54,
+                55,
+                56,
+                57,
+                58,
+                59,
+                60,
+                61,
+                62,
+                63,
+                64,
+                65,
+                66,
+                67,
+                68,
+                69,
+                70,
+                71,
+                72,
+                73,
+                74,
+                75,
+                76,
+                77,
+                78,
+                79,
+                80,
+                81,
+                82,
+                83
+            ],
+            "word": [
+                "ä¸€",
+                "å¤©",
+                "ï¼Œ",
+                "ç”µè§†",
+                "é‡Œ",
+                "åˆ",
+                "æ’­æ”¾",
+                "è¶³çƒ",
+                "æ¯”èµ›",
+                "ï¼Œ",
+                "ä¸ˆå¤«",
+                "å",
+                "åœ¨",
+                "ç”µè§†æœº",
+                "å‰",
+                "ä¸€åŠ¨",
+                "ä¹Ÿ",
+                "ä¸",
+                "åŠ¨",
+                "ï¼Œ",
+                "å¦»å­",
+                "è·Ÿ",
+                "ä»–",
+                "è¯´è¯",
+                "ä»–",
+                "ä¹Ÿ",
+                "å¥½åƒ",
+                "æ²¡æœ‰",
+                "å¬åˆ°",
+                "ã€‚"
+            ],
+            "lemma": [
+                "ä¸€",
+                "å¤©",
+                "ï¼Œ",
+                "ç”µè§†",
+                "é‡Œ",
+                "åˆ",
+                "æ’­æ”¾",
+                "è¶³çƒ",
+                "æ¯”èµ›",
+                "ï¼Œ",
+                "ä¸ˆå¤«",
+                "å",
+                "åœ¨",
+                "ç”µè§†æœº",
+                "å‰",
+                "ä¸€åŠ¨",
+                "ä¹Ÿ",
+                "ä¸",
+                "åŠ¨",
+                "ï¼Œ",
+                "å¦»å­",
+                "è·Ÿ",
+                "ä»–",
+                "è¯´è¯",
+                "ä»–",
+                "ä¹Ÿ",
+                "å¥½åƒ",
+                "æ²¡æœ‰",
+                "å¬åˆ°",
+                "ã€‚"
+            ],
+            "pos": [
+                "CD",
+                "M",
+                "PU",
+                "NN",
+                "LC",
+                "AD",
+                "VV",
+                "NN",
+                "NN",
+                "PU",
+                "NN",
+                "VV",
+                "P",
+                "NN",
+                "LC",
+                "AD",
+                "AD",
+                "AD",
+                "VV",
+                "PU",
+                "NN",
+                "P",
+                "PN",
+                "VV",
+                "PN",
+                "AD",
+                "AD",
+                "AD",
+                "VV",
+                "PU"
+            ],
+            "level": [
+                0,
+                0,
+                -2,
+                0,
+                0,
+                1,
+                2,
+                2,
+                2,
+                -2,
+                3,
+                0,
+                0,
+                0,
+                0,
+                0,
+                0,
+                0,
+                0,
+                -2,
+                3,
+                0,
+                0,
+                0,
+                0,
+                0,
+                1,
+                0,
+                0,
+                -2
+            ]
+        },
+        "4": {
+            "id": [
+                84,
+                85,
+                86,
+                87,
+                88,
+                89,
+                90,
+                91,
+                92,
+                93,
+                94,
+                95,
+                96,
+                97,
+                98,
+                99,
+                100,
+                101,
+                102,
+                103,
+                104,
+                105,
+                106,
+                107,
+                108,
+                109,
+                110,
+                111,
+                112,
+                113,
+                114,
+                115,
+                116,
+                117,
+                118,
+                119,
+                120,
+                121
+            ],
+            "word": [
+                "å¹´è½»",
+                "çš„",
+                "å¦»å­",
+                "éå¸¸",
+                "ç”Ÿæ°”",
+                "ï¼Œ",
+                "å¥¹",
+                "å“­",
+                "ç€",
+                "å›åˆ°",
+                "è‡ªå·±",
+                "çš„",
+                "å¦ˆå¦ˆ",
+                "å®¶",
+                "ï¼Œ",
+                "å¯æ˜¯",
+                "å›åˆ°",
+                "å®¶",
+                "çš„",
+                "æ—¶å€™",
+                "å´",
+                "å‘ç°",
+                "å®¶é‡Œ",
+                "åªæœ‰",
+                "çˆ¸çˆ¸",
+                "ä¸€",
+                "ä¸ª",
+                "äºº",
+                "ï¼Œ",
+                "ä¹Ÿ",
+                "å",
+                "åœ¨",
+                "ç”µè§†æœº",
+                "å‰",
+                "çœ‹",
+                "è¶³çƒ",
+                "æ¯”èµ›",
+                "ã€‚"
+            ],
+            "lemma": [
+                "å¹´è½»",
+                "çš„",
+                "å¦»å­",
+                "éå¸¸",
+                "ç”Ÿæ°”",
+                "ï¼Œ",
+                "å¥¹",
+                "å“­",
+                "ç€",
+                "å›åˆ°",
+                "è‡ªå·±",
+                "çš„",
+                "å¦ˆå¦ˆ",
+                "å®¶",
+                "ï¼Œ",
+                "å¯æ˜¯",
+                "å›åˆ°",
+                "å®¶",
+                "çš„",
+                "æ—¶å€™",
+                "å´",
+                "å‘ç°",
+                "å®¶é‡Œ",
+                "åªæœ‰",
+                "çˆ¸çˆ¸",
+                "ä¸€",
+                "ä¸ª",
+                "äºº",
+                "ï¼Œ",
+                "ä¹Ÿ",
+                "å",
+                "åœ¨",
+                "ç”µè§†æœº",
+                "å‰",
+                "çœ‹",
+                "è¶³çƒ",
+                "æ¯”èµ›",
+                "ã€‚"
+            ],
+            "pos": [
+                "VA",
+                "DEC",
+                "NN",
+                "AD",
+                "VV",
+                "PU",
+                "PN",
+                "VV",
+                "AS",
+                "VV",
+                "PN",
+                "DEG",
+                "NN",
+                "NN",
+                "PU",
+                "AD",
+                "VV",
+                "NN",
+                "DEC",
+                "NN",
+                "AD",
+                "VV",
+                "NN",
+                "AD",
+                "NN",
+                "CD",
+                "M",
+                "NN",
+                "PU",
+                "AD",
+                "VV",
+                "P",
+                "NN",
+                "LC",
+                "VV",
+                "NN",
+                "NN",
+                "PU"
+            ],
+            "level": [
+                1,
+                0,
+                3,
+                0,
+                0,
+                -2,
+                0,
+                1,
+                0,
+                0,
+                1,
+                0,
+                0,
+                0,
+                -2,
+                1,
+                0,
+                0,
+                0,
+                0,
+                3,
+                1,
+                0,
+                2,
+                0,
+                0,
+                0,
+                0,
+                -2,
+                0,
+                0,
+                0,
+                0,
+                0,
+                0,
+                2,
+                2,
+                -2
+            ]
+        },
+        "5": {
+            "id": [
+                122,
+                123,
+                124,
+                125,
+                126
+            ],
+            "word": [
+                "â€œ",
+                "å¦ˆå¦ˆ",
+                "å‘¢",
+                "ï¼Ÿ",
+                "â€"
+            ],
+            "lemma": [
+                "â€œ",
+                "å¦ˆå¦ˆ",
+                "å‘¢",
+                "ï¼Ÿ",
+                "â€"
+            ],
+            "pos": [
+                "PU",
+                "NN",
+                "IJ",
+                "PU",
+                "PU"
+            ],
+            "level": [
+                -2,
+                0,
+                0,
+                -2,
+                -2
+            ]
+        },
+        "6": {
+            "id": [
+                127,
+                128,
+                129,
+                130
+            ],
+            "word": [
+                "å¥¹",
+                "å¾ˆ",
+                "å¥‡æ€ª",
+                "ã€‚"
+            ],
+            "lemma": [
+                "å¥¹",
+                "å¾ˆ",
+                "å¥‡æ€ª",
+                "ã€‚"
+            ],
+            "pos": [
+                "PN",
+                "AD",
+                "VA",
+                "PU"
+            ],
+            "level": [
+                0,
+                0,
+                2,
+                -2
+            ]
+        },
+        "7": {
+            "id": [
+                131,
+                132,
+                133,
+                134,
+                135,
+                136,
+                137,
+                138,
+                139
+            ],
+            "word": [
+                "â€œ",
+                "å›",
+                "å¥¹",
+                "çš„",
+                "å¦ˆå¦ˆ",
+                "å®¶",
+                "äº†",
+                "ã€‚",
+                "â€"
+            ],
+            "lemma": [
+                "â€œ",
+                "å›",
+                "å¥¹",
+                "çš„",
+                "å¦ˆå¦ˆ",
+                "å®¶",
+                "äº†",
+                "ã€‚",
+                "â€"
+            ],
+            "pos": [
+                "PU",
+                "VV",
+                "PN",
+                "DEG",
+                "NN",
+                "NN",
+                "SP",
+                "PU",
+                "PU"
+            ],
+            "level": [
+                -2,
+                0,
+                0,
+                0,
+                0,
+                0,
+                0,
+                -2,
+                -2
+            ]
+        },
+        "8": {
+            "id": [
+                140,
+                141,
+                142,
+                143,
+                144,
+                145,
+                146,
+                147
+            ],
+            "word": [
+                "çˆ¶äº²",
+                "å¤´",
+                "ä¹Ÿ",
+                "ä¸",
+                "å›",
+                "åœ°",
+                "è¯´",
+                "ã€‚"
+            ],
+            "lemma": [
+                "çˆ¶äº²",
+                "å¤´",
+                "ä¹Ÿ",
+                "ä¸",
+                "å›",
+                "åœ°",
+                "è¯´",
+                "ã€‚"
+            ],
+            "pos": [
+                "NN",
+                "NN",
+                "AD",
+                "AD",
+                "VV",
+                "DEV",
+                "VV",
+                "PU"
+            ],
+            "level": [
+                2,
+                1,
+                0,
+                0,
+                0,
+                0,
+                0,
+                -2
+            ]
+        }
+    },
+    "wordlists": {
+        "0": {
+            "lemma": [
+                "ä¹Ÿ",
+                "ä¸€",
+                "çš„",
+                "ä¸",
+                "ä¸ª",
+                "ä»–",
+                "å¥¹",
+                "å¦ˆå¦ˆ",
+                "å®¶",
+                "çš„",
+                "å‰",
+                "å›",
+                "å›åˆ°",
+                "åœ¨",
+                "å",
+                "æ—¶å€™",
+                "ç”µè§†",
+                "ç”µè§†æœº",
+                "çœ‹",
+                "éå¸¸",
+                "ä¸€åŠ¨",
+                "ä¸€ç‚¹å„¿",
+                "ä¸­",
+                "äº†",
+                "äº†",
+                "äºº",
+                "ä»–ä»¬",
+                "åŠ¨",
+                "åƒ",
+                "å¬åˆ°",
+                "å‘¢",
+                "å’Œ",
+                "å–œæ¬¢",
+                "åœ°",
+                "å¤©",
+                "å®¶é‡Œ",
+                "å¯¹",
+                "å¾ˆ",
+                "æœ‰",
+                "æ¬¡",
+                "æ²¡æœ‰",
+                "æ²¡æœ‰",
+                "çˆ¸çˆ¸",
+                "ç”Ÿæ°”",
+                "ç€",
+                "è¦",
+                "è¯´",
+                "è¯´è¯",
+                "è·Ÿ",
+                "éƒ½",
+                "é‡Œ",
+                "é¥­"
+            ],
+            "pos": [
+                "AD",
+                "CD",
+                "DEC",
+                "AD",
+                "M",
+                "PN",
+                "PN",
+                "NN",
+                "NN",
+                "DEG",
+                "LC",
+                "VV",
+                "VV",
+                "P",
+                "VV",
+                "NN",
+                "NN",
+                "NN",
+                "VV",
+                "AD",
+                "AD",
+                "CD",
+                "LC",
+                "AS",
+                "SP",
+                "NN",
+                "PN",
+                "VV",
+                "VV",
+                "VV",
+                "IJ",
+                "P",
+                "VV",
+                "DEV",
+                "M",
+                "NN",
+                "P",
+                "AD",
+                "VE",
+                "M",
+                "AD",
+                "VE",
+                "NN",
+                "VV",
+                "AS",
+                "VV",
+                "VV",
+                "VV",
+                "P",
+                "AD",
+                "LC",
+                "NN"
+            ],
+            "size": [
+                6,
+                4,
+                4,
+                3,
+                3,
+                3,
+                3,
+                3,
+                3,
+                3,
+                2,
+                2,
+                2,
+                2,
+                2,
+                2,
+                2,
+                2,
+                2,
+                2,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1
+            ]
+        },
+        "1": {
+            "lemma": [
+                "å¹´è½»",
+                "ä»¥å",
+                "åŠæ³•",
+                "ååˆ†",
+                "åˆ",
+                "å‘ç°",
+                "å¯æ˜¯",
+                "å“­",
+                "å¤´",
+                "å¥½åƒ",
+                "ç”Ÿæ´»",
+                "è‡ªå·±"
+            ],
+            "pos": [
+                "VA",
+                "LC",
+                "NN",
+                "AD",
+                "AD",
+                "VV",
+                "AD",
+                "VV",
+                "NN",
+                "AD",
+                "NN",
+                "PN"
+            ],
+            "size": [
+                2,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1
+            ]
+        },
+        "2": {
+            "lemma": [
+                "è¶³çƒ",
+                "æ¯”èµ›",
+                "ç»“å©š",
+                "åªæœ‰",
+                "å¥‡æ€ª",
+                "å§‘å¨˜",
+                "å¹¸ç¦",
+                "æ’­æ”¾",
+                "æ¯",
+                "çˆ¶äº²",
+                "è¿"
+            ],
+            "pos": [
+                "NN",
+                "NN",
+                "VV",
+                "AD",
+                "VA",
+                "NN",
+                "VA",
+                "VV",
+                "DT",
+                "NN",
+                "AD"
+            ],
+            "size": [
+                4,
+                3,
+                2,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1,
+                1
+            ]
+        },
+        "3": {
+            "lemma": [
+                "å¦»å­",
+                "å°ä¼™å­",
+                "ä¸ˆå¤«",
+                "å´",
+                "æ­¤"
+            ],
+            "pos": [
+                "NN",
+                "NN",
+                "NN",
+                "AD",
+                "PN"
+            ],
+            "size": [
+                3,
+                2,
+                1,
+                1,
+                1
+            ]
+        }
+    },
+    "stats": {
+        "sum_token": {
+            "values": [
+                114,
+                23,
+                32,
+                16,
+                0,
+                0,
+                0,
+                0
+            ]
+        },
+        "cumsum_token": {
+            "values": [
+                0.6162,
+                0.7405,
+                0.9135,
+                1,
+                1,
+                1,
+                1,
+                1
+            ],
+            "constants": [
+                0.10716878453363744,
+                0.05480006412704765,
+                4.171371439607046,
+                1.5715862053781118
+            ]
+        },
+        "sum_type": {
+            "values": [
+                71,
+                21,
+                20,
+                9,
+                0,
+                0,
+                0,
+                0
+            ]
+        },
+        "cumsum_type": {
+            "values": [
+                0.5868,
+                0.7603,
+                0.9256,
+                1,
+                1,
+                1,
+                1,
+                1
+            ],
+            "constants": [
+                0.13618252101235725,
+                0.12194848245384173,
+                3.289397856402208,
+                1.370132441516794
+            ]
+        },
+        "level": {
+            "fit_curve": [
+                2.9186825460327808
+            ],
+            "ninety_five": [
+                2.2187499999999987
+            ],
+            "fit_error": [
+                0.0330230230991995
+            ]
+        }
+    },
+    "final_levels": {
+        "vocabulary_level": 2.9
+    },
+    "final_levels_str": {
+        "vocabulary_level": "HSK3.9"
+    }
     }
```

### Comparing `mock_cminor-0.0.4/LICENCE` & `mock_cminor-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `mock_cminor-0.0.4/README.md` & `mock_cminor-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mock_cminor-0.0.4/pyproject.toml` & `mock_cminor-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mock-cminor"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Cathoven A.I", email="contact@cathoven.com" },
 ]
 description = "Mocking library for Cminor"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/yunusarli/cminor"
-Issues = "https://github.com/yunusarli/cminor/issues"
+Homepage = "https://github.com/Cathoven-AI/cminor"
+Issues = "https://github.com/Cathoven-AI/cminor/issues"
```

### Comparing `mock_cminor-0.0.4/PKG-INFO` & `mock_cminor-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: mock-cminor
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mocking library for Cminor
-Project-URL: Homepage, https://github.com/yunusarli/cminor
-Project-URL: Issues, https://github.com/yunusarli/cminor/issues
+Project-URL: Homepage, https://github.com/Cathoven-AI/cminor
+Project-URL: Issues, https://github.com/Cathoven-AI/cminor/issues
 Author-email: "Cathoven A.I" <contact@cathoven.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

