# Comparing `tmp/nlhappy-2023.1.31.tar.gz` & `tmp/nlhappy-2024.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlhappy-2023.1.31.tar", max compression
+gzip compressed data, was "nlhappy-2024.5.7.tar", max compression
```

## Comparing `nlhappy-2023.1.31.tar` & `nlhappy-2024.5.7.tar`

### file list

```diff
@@ -1,151 +1,150 @@
--rw-r--r--   0        0        0     1087 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/LICENSE
--rw-r--r--   0        0        0     2519 2022-12-22 05:58:00.412377 nlhappy-2023.1.31/README.md
--rw-r--r--   0        0        0        0 2022-11-21 10:04:15.000000 nlhappy-2023.1.31/nlhappy/__init__.py
--rw-r--r--   0        0        0       28 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/algorithms/__init__.py
--rw-r--r--   0        0        0     4586 2022-11-19 12:59:59.000000 nlhappy-2023.1.31/nlhappy/algorithms/text_match.py
--rw-r--r--   0        0        0      396 2022-11-03 11:04:34.000000 nlhappy-2023.1.31/nlhappy/callbacks/__init__.py
--rw-r--r--   0        0        0     1520 2022-10-28 00:44:16.000000 nlhappy-2023.1.31/nlhappy/callbacks/ckpt_callbacks.py
--rw-r--r--   0        0        0        0 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/__init__.py
--rw-r--r--   0        0        0     1111 2022-12-19 07:50:29.509177 nlhappy-2023.1.31/nlhappy/configs/callbacks/default.yaml
--rw-r--r--   0        0        0      112 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/callbacks/finetune.yaml
--rw-r--r--   0        0        0        0 2022-12-19 08:37:36.947235 nlhappy-2023.1.31/nlhappy/configs/callbacks/none.yaml
--rw-r--r--   0        0        0      938 2022-12-20 14:54:38.725298 nlhappy-2023.1.31/nlhappy/configs/callbacks/swa.yaml
--rw-r--r--   0        0        0      134 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/callbacks/update.yaml
--rw-r--r--   0        0        0     1745 2022-11-20 04:01:08.000000 nlhappy-2023.1.31/nlhappy/configs/config.yaml
--rw-r--r--   0        0        0      194 2022-12-15 02:51:11.097543 nlhappy-2023.1.31/nlhappy/configs/datamodule/entity_extraction.yaml
--rw-r--r--   0        0        0      192 2022-11-26 12:18:22.964619 nlhappy-2023.1.31/nlhappy/configs/datamodule/event_extraction.yaml
--rw-r--r--   0        0        0      229 2022-12-15 02:51:22.909602 nlhappy-2023.1.31/nlhappy/configs/datamodule/prompt_relation_extraction.yaml
--rw-r--r--   0        0        0      238 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/datamodule/prompt_span_extraction.yaml
--rw-r--r--   0        0        0      195 2022-12-11 11:48:04.839369 nlhappy-2023.1.31/nlhappy/configs/datamodule/question_answering.yaml
--rw-r--r--   0        0        0      197 2022-11-25 14:49:54.796238 nlhappy-2023.1.31/nlhappy/configs/datamodule/relation_extraction.yaml
--rw-r--r--   0        0        0      208 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/datamodule/span_extraction.yaml
--rw-r--r--   0        0        0      196 2022-12-13 10:47:19.872417 nlhappy-2023.1.31/nlhappy/configs/datamodule/text_classification.yaml
--rw-r--r--   0        0        0      200 2022-12-13 10:56:56.275283 nlhappy-2023.1.31/nlhappy/configs/datamodule/text_pair_classification.yaml
--rw-r--r--   0        0        0      213 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/datamodule/text_pair_regression.yaml
--rw-r--r--   0        0        0      230 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/datamodule/token_classification.yaml
--rw-r--r--   0        0        0      216 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/log_dir/debug.yaml
--rw-r--r--   0        0        0      226 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/log_dir/default.yaml
--rw-r--r--   0        0        0      227 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/log_dir/evaluation.yaml
--rw-r--r--   0        0        0      125 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/logger/csv.yaml
--rw-r--r--   0        0        0       94 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/logger/many_loggers.yaml
--rw-r--r--   0        0        0      214 2022-11-20 04:02:06.000000 nlhappy-2023.1.31/nlhappy/configs/logger/tensorboard.yaml
--rw-r--r--   0        0        0      394 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/logger/wandb.yaml
--rw-r--r--   0        0        0      135 2022-12-12 02:17:16.734671 nlhappy-2023.1.31/nlhappy/configs/model/bert4qa.yaml
--rw-r--r--   0        0        0      137 2022-11-21 11:32:53.000000 nlhappy-2023.1.31/nlhappy/configs/model/bert4tc.yaml
--rw-r--r--   0        0        0      158 2022-12-21 07:07:31.483530 nlhappy-2023.1.31/nlhappy/configs/model/bert4tpc.yaml
--rw-r--r--   0        0        0       98 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/bert_bi_encoder.yaml
--rw-r--r--   0        0        0      112 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/bert_crf.yaml
--rw-r--r--   0        0        0      137 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/bert_global_span.yaml
--rw-r--r--   0        0        0      115 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/bert_lstm_crf.yaml
--rw-r--r--   0        0        0      112 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/bert_text_multi_classification.yaml
--rw-r--r--   0        0        0      129 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/bert_token_classification.yaml
--rw-r--r--   0        0        0      155 2022-11-26 13:41:35.081440 nlhappy-2023.1.31/nlhappy/configs/model/biaffine4ee.yaml
--rw-r--r--   0        0        0      192 2022-10-28 12:21:49.000000 nlhappy-2023.1.31/nlhappy/configs/model/biaffine4ner.yaml
--rw-r--r--   0        0        0      181 2022-11-13 02:42:55.000000 nlhappy-2023.1.31/nlhappy/configs/model/blinker4re.yaml
--rw-r--r--   0        0        0      168 2022-10-27 12:54:52.000000 nlhappy-2023.1.31/nlhappy/configs/model/casrel.yaml
--rw-r--r--   0        0        0       85 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/cosent.yaml
--rw-r--r--   0        0        0      134 2022-11-20 01:17:00.000000 nlhappy-2023.1.31/nlhappy/configs/model/crf4ner.yaml
--rw-r--r--   0        0        0      185 2022-11-01 11:35:20.000000 nlhappy-2023.1.31/nlhappy/configs/model/globalpointer4clique.yaml
--rw-r--r--   0        0        0      176 2022-10-31 09:56:40.000000 nlhappy-2023.1.31/nlhappy/configs/model/globalpointer4ner.yaml
--rw-r--r--   0        0        0      168 2022-12-11 11:41:19.173352 nlhappy-2023.1.31/nlhappy/configs/model/globalpointer4qa.yaml
--rw-r--r--   0        0        0      154 2022-11-09 10:00:29.000000 nlhappy-2023.1.31/nlhappy/configs/model/gplinker4ee.yaml
--rw-r--r--   0        0        0      177 2022-11-25 14:36:03.912107 nlhappy-2023.1.31/nlhappy/configs/model/gplinker4re.yaml
--rw-r--r--   0        0        0      139 2022-10-27 12:54:52.000000 nlhappy-2023.1.31/nlhappy/configs/model/onerel.yaml
--rw-r--r--   0        0        0      140 2022-12-22 10:50:15.431562 nlhappy-2023.1.31/nlhappy/configs/model/pointer4qa.yaml
--rw-r--r--   0        0        0      158 2022-10-27 12:54:52.000000 nlhappy-2023.1.31/nlhappy/configs/model/prompt_gplinker.yaml
--rw-r--r--   0        0        0      100 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/model/sentence_bert.yaml
--rw-r--r--   0        0        0      240 2022-11-20 02:49:04.000000 nlhappy-2023.1.31/nlhappy/configs/model/w2ner.yaml
--rw-r--r--   0        0        0       71 2022-11-11 23:55:28.000000 nlhappy-2023.1.31/nlhappy/configs/trainer/cpu.yaml
--rw-r--r--   0        0        0      100 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/trainer/ddp.yaml
--rw-r--r--   0        0        0      257 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/configs/trainer/debug.yaml
--rw-r--r--   0        0        0      310 2022-12-19 09:12:41.813701 nlhappy-2023.1.31/nlhappy/configs/trainer/default.yaml
--rw-r--r--   0        0        0      249 2023-01-28 08:45:23.872987 nlhappy-2023.1.31/nlhappy/data/__init__.py
--rw-r--r--   0        0        0     1024 2022-12-21 07:56:01.201997 nlhappy-2023.1.31/nlhappy/data/augmentation.py
--rw-r--r--   0        0        0     3082 2023-01-28 08:56:11.848209 nlhappy-2023.1.31/nlhappy/data/couplet.py
--rw-r--r--   0        0        0     2964 2023-01-28 07:36:37.480470 nlhappy-2023.1.31/nlhappy/data/dataset.py
--rw-r--r--   0        0        0    24287 2022-12-21 12:09:11.953527 nlhappy-2023.1.31/nlhappy/data/doc.py
--rw-r--r--   0        0        0      692 2022-12-11 11:39:39.248855 nlhappy-2023.1.31/nlhappy/datamodules/__init__.py
--rw-r--r--   0        0        0     7621 2022-11-25 08:53:04.000000 nlhappy-2023.1.31/nlhappy/datamodules/entity_extraction.py
--rw-r--r--   0        0        0    15360 2022-11-26 12:25:41.966801 nlhappy-2023.1.31/nlhappy/datamodules/event_extraction.py
--rw-r--r--   0        0        0     4406 2022-11-21 11:14:52.000000 nlhappy-2023.1.31/nlhappy/datamodules/prompt_relation_extraction.py
--rw-r--r--   0        0        0     3501 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/datamodules/prompt_span_extraction.py
--rw-r--r--   0        0        0     4474 2022-12-13 00:11:07.242621 nlhappy-2023.1.31/nlhappy/datamodules/question_answering.py
--rw-r--r--   0        0        0    21894 2022-11-25 14:46:26.111200 nlhappy-2023.1.31/nlhappy/datamodules/relation_extraction.py
--rw-r--r--   0        0        0     2850 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/datamodules/span_extraction.py
--rw-r--r--   0        0        0     2318 2022-12-13 10:48:52.364877 nlhappy-2023.1.31/nlhappy/datamodules/text_classification.py
--rw-r--r--   0        0        0     1572 2022-11-25 06:16:00.000000 nlhappy-2023.1.31/nlhappy/datamodules/text_multi_classification.py
--rw-r--r--   0        0        0     3558 2022-12-13 12:08:18.652576 nlhappy-2023.1.31/nlhappy/datamodules/text_pair_classification.py
--rw-r--r--   0        0        0     2649 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/datamodules/text_pair_regression.py
--rw-r--r--   0        0        0     2212 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/datamodules/token_classification.py
--rw-r--r--   0        0        0      531 2022-11-13 02:03:36.000000 nlhappy-2023.1.31/nlhappy/layers/__init__.py
--rw-r--r--   0        0        0      772 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/layers/activation.py
--rw-r--r--   0        0        0       97 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/layers/attention/__init__.py
--rw-r--r--   0        0        0     4205 2022-11-25 06:18:40.000000 nlhappy-2023.1.31/nlhappy/layers/attention/multi_head_attention.py
--rw-r--r--   0        0        0    14626 2023-01-12 07:20:12.618202 nlhappy-2023.1.31/nlhappy/layers/bert.py
--rw-r--r--   0        0        0      253 2022-11-21 02:59:09.000000 nlhappy-2023.1.31/nlhappy/layers/classifier/__init__.py
--rw-r--r--   0        0        0     6484 2022-11-03 16:11:02.000000 nlhappy-2023.1.31/nlhappy/layers/classifier/biaffine.py
--rw-r--r--   0        0        0    17389 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/layers/classifier/crf.py
--rw-r--r--   0        0        0     9178 2022-11-08 12:53:45.000000 nlhappy-2023.1.31/nlhappy/layers/classifier/global_pointer.py
--rw-r--r--   0        0        0     1449 2022-11-21 03:50:40.000000 nlhappy-2023.1.31/nlhappy/layers/classifier/onerel.py
--rw-r--r--   0        0        0      726 2022-12-15 03:15:28.044787 nlhappy-2023.1.31/nlhappy/layers/classifier/simple_dense.py
--rw-r--r--   0        0        0      661 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/layers/dropout.py
--rw-r--r--   0        0        0       81 2022-11-07 05:39:48.000000 nlhappy-2023.1.31/nlhappy/layers/embedding/__init__.py
--rw-r--r--   0        0        0     6159 2022-11-07 03:33:17.000000 nlhappy-2023.1.31/nlhappy/layers/embedding/position_embedding.py
--rw-r--r--   0        0        0     5170 2022-12-20 10:10:18.384472 nlhappy-2023.1.31/nlhappy/layers/loss.py
--rw-r--r--   0        0        0     2460 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/layers/normalization.py
--rw-r--r--   0        0        0     1822 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/layers/word2vec.py
--rw-r--r--   0        0        0        0 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/metrics/__init__.py
--rw-r--r--   0        0        0     3342 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/metrics/chunk.py
--rw-r--r--   0        0        0     1142 2022-11-25 07:08:52.000000 nlhappy-2023.1.31/nlhappy/metrics/entity.py
--rw-r--r--   0        0        0     1231 2022-11-26 18:08:03.664936 nlhappy-2023.1.31/nlhappy/metrics/event.py
--rw-r--r--   0        0        0     1248 2022-11-25 11:09:58.000000 nlhappy-2023.1.31/nlhappy/metrics/relation.py
--rw-r--r--   0        0        0     2610 2022-12-13 00:10:16.050366 nlhappy-2023.1.31/nlhappy/metrics/span.py
--rw-r--r--   0        0        0     2173 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/metrics/triple.py
--rw-r--r--   0        0        0      812 2023-01-28 07:14:52.629982 nlhappy-2023.1.31/nlhappy/models/__init__.py
--rw-r--r--   0        0        0      190 2022-11-20 02:14:13.000000 nlhappy-2023.1.31/nlhappy/models/entity_extraction/__init__.py
--rw-r--r--   0        0        0     4764 2022-11-25 09:33:05.000000 nlhappy-2023.1.31/nlhappy/models/entity_extraction/biaffine.py
--rw-r--r--   0        0        0     4961 2022-11-25 09:50:59.000000 nlhappy-2023.1.31/nlhappy/models/entity_extraction/crf.py
--rw-r--r--   0        0        0     6942 2022-11-25 11:03:57.000000 nlhappy-2023.1.31/nlhappy/models/entity_extraction/globalpointer.py
--rw-r--r--   0        0        0    13298 2022-11-20 04:09:42.000000 nlhappy-2023.1.31/nlhappy/models/entity_extraction/w2ner.py
--rw-r--r--   0        0        0       97 2022-11-21 02:39:57.000000 nlhappy-2023.1.31/nlhappy/models/event_extraction/__init__.py
--rw-r--r--   0        0        0    11491 2022-11-26 18:08:13.904987 nlhappy-2023.1.31/nlhappy/models/event_extraction/biaffine.py
--rw-r--r--   0        0        0    11305 2022-11-26 14:14:23.727228 nlhappy-2023.1.31/nlhappy/models/event_extraction/gplinker.py
--rw-r--r--   0        0        0       57 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/prompt_relation_extraction/__init__.py
--rw-r--r--   0        0        0    10367 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/prompt_relation_extraction/gplinker.py
--rw-r--r--   0        0        0      152 2022-12-12 09:55:46.087449 nlhappy-2023.1.31/nlhappy/models/question_answering/__init__.py
--rw-r--r--   0        0        0     7305 2022-12-22 02:56:34.970254 nlhappy-2023.1.31/nlhappy/models/question_answering/pointer.py
--rw-r--r--   0        0        0        0 2022-12-23 08:27:50.238661 nlhappy-2023.1.31/nlhappy/models/question_answering/t5.py
--rw-r--r--   0        0        0      383 2022-11-13 02:41:36.000000 nlhappy-2023.1.31/nlhappy/models/relation_extraction/__init__.py
--rw-r--r--   0        0        0    10561 2022-11-25 14:17:53.942687 nlhappy-2023.1.31/nlhappy/models/relation_extraction/biaffine.py
--rw-r--r--   0        0        0    11329 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/relation_extraction/casrel.py
--rw-r--r--   0        0        0     9870 2022-12-21 06:46:33.613276 nlhappy-2023.1.31/nlhappy/models/relation_extraction/gplinker.py
--rw-r--r--   0        0        0    12097 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/relation_extraction/onerel.py
--rw-r--r--   0        0        0       41 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/span_extraction/__init__.py
--rw-r--r--   0        0        0     6290 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/span_extraction/global_pointer.py
--rw-r--r--   0        0        0       43 2022-11-21 11:32:29.000000 nlhappy-2023.1.31/nlhappy/models/text_classification/__init__.py
--rw-r--r--   0        0        0     4417 2022-12-13 10:43:33.659293 nlhappy-2023.1.31/nlhappy/models/text_classification/bert.py
--rw-r--r--   0        0        0       71 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/text_multi_classification/__init__.py
--rw-r--r--   0        0        0     3108 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/text_multi_classification/bert_text_multi_classification.py
--rw-r--r--   0        0        0       89 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/text_pair_classification/__init__.py
--rw-r--r--   0        0        0     3013 2022-11-20 05:19:07.000000 nlhappy-2023.1.31/nlhappy/models/text_pair_classification/bert_bi_encode.py
--rw-r--r--   0        0        0     4098 2022-12-21 08:56:11.731949 nlhappy-2023.1.31/nlhappy/models/text_pair_classification/bert_cross_encode.py
--rw-r--r--   0        0        0       75 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/text_pair_regression/__init__.py
--rw-r--r--   0        0        0     4820 2023-01-13 07:34:21.340007 nlhappy-2023.1.31/nlhappy/models/text_pair_regression/cosent_bert.py
--rw-r--r--   0        0        0     4786 2022-12-20 10:55:34.333976 nlhappy-2023.1.31/nlhappy/models/text_pair_regression/sentence_bert.py
--rw-r--r--   0        0        0      196 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/token_classification/__init__.py
--rw-r--r--   0        0        0     5036 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/token_classification/bert_crf.py
--rw-r--r--   0        0        0     5782 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/token_classification/bert_lstm_crf.py
--rw-r--r--   0        0        0     3301 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/models/token_classification/bert_token_classification.py
--rw-r--r--   0        0        0     4499 2022-10-27 12:54:52.000000 nlhappy-2023.1.31/nlhappy/run.py
--rw-r--r--   0        0        0        3 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/tricks/__init__.py
--rw-r--r--   0        0        0     6053 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/tricks/adversarial_training.py
--rw-r--r--   0        0        0        0 2022-10-26 11:45:15.000000 nlhappy-2023.1.31/nlhappy/utils/__init__.py
--rw-r--r--   0        0        0    14138 2022-11-28 12:28:38.446850 nlhappy-2023.1.31/nlhappy/utils/make_datamodule.py
--rw-r--r--   0        0        0     5814 2022-11-28 11:39:29.384187 nlhappy-2023.1.31/nlhappy/utils/make_dataset.py
--rw-r--r--   0        0        0     3712 2022-11-25 10:01:08.000000 nlhappy-2023.1.31/nlhappy/utils/make_doc.py
--rw-r--r--   0        0        0    20594 2023-01-13 09:23:07.936458 nlhappy-2023.1.31/nlhappy/utils/make_model.py
--rw-r--r--   0        0        0     8254 2022-12-11 02:55:52.536600 nlhappy-2023.1.31/nlhappy/utils/text.py
--rw-r--r--   0        0        0     5976 2022-10-27 12:54:52.000000 nlhappy-2023.1.31/nlhappy/utils/utils.py
--rw-r--r--   0        0        0      791 2023-01-31 01:34:37.797236 nlhappy-2023.1.31/pyproject.toml
--rw-r--r--   0        0        0     4413 2023-01-31 01:35:41.806171 nlhappy-2023.1.31/setup.py
--rw-r--r--   0        0        0     3460 2023-01-31 01:35:41.806589 nlhappy-2023.1.31/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-07 03:30:47.519435 nlhappy-2024.5.7/LICENSE
+-rw-r--r--   0        0        0     2292 2024-05-07 08:35:51.235749 nlhappy-2024.5.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/__init__.py
+-rw-r--r--   0        0        0     4602 2024-05-07 08:31:36.060560 nlhappy-2024.5.7/nlhappy/__main__.py
+-rw-r--r--   0        0        0       28 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/algorithms/__init__.py
+-rw-r--r--   0        0        0     4586 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/algorithms/text_match.py
+-rw-r--r--   0        0        0      396 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/callbacks/__init__.py
+-rw-r--r--   0        0        0     1520 2024-05-07 07:38:51.520529 nlhappy-2024.5.7/nlhappy/callbacks/ckpt_callbacks.py
+-rw-r--r--   0        0        0        0 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/__init__.py
+-rw-r--r--   0        0        0     1111 2024-05-07 07:23:21.412440 nlhappy-2024.5.7/nlhappy/configs/callbacks/default.yaml
+-rw-r--r--   0        0        0      112 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/callbacks/finetune.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/callbacks/none.yaml
+-rw-r--r--   0        0        0      938 2024-05-07 07:21:58.195806 nlhappy-2024.5.7/nlhappy/configs/callbacks/swa.yaml
+-rw-r--r--   0        0        0      134 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/callbacks/update.yaml
+-rw-r--r--   0        0        0     1817 2024-05-07 06:39:15.350547 nlhappy-2024.5.7/nlhappy/configs/config.yaml
+-rw-r--r--   0        0        0      209 2024-05-07 07:42:56.250796 nlhappy-2024.5.7/nlhappy/configs/datamodule/entity_extraction.yaml
+-rw-r--r--   0        0        0      192 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/event_extraction.yaml
+-rw-r--r--   0        0        0      229 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/prompt_relation_extraction.yaml
+-rw-r--r--   0        0        0      238 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/prompt_span_extraction.yaml
+-rw-r--r--   0        0        0      195 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/question_answering.yaml
+-rw-r--r--   0        0        0      197 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/relation_extraction.yaml
+-rw-r--r--   0        0        0      208 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/span_extraction.yaml
+-rw-r--r--   0        0        0      213 2024-05-07 07:53:44.996120 nlhappy-2024.5.7/nlhappy/configs/datamodule/text_classification.yaml
+-rw-r--r--   0        0        0      200 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/text_pair_classification.yaml
+-rw-r--r--   0        0        0      213 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/text_pair_regression.yaml
+-rw-r--r--   0        0        0      230 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/datamodule/token_classification.yaml
+-rw-r--r--   0        0        0      216 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/log_dir/debug.yaml
+-rw-r--r--   0        0        0      226 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/log_dir/default.yaml
+-rw-r--r--   0        0        0      227 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/log_dir/evaluation.yaml
+-rw-r--r--   0        0        0      125 2024-05-07 07:22:13.331919 nlhappy-2024.5.7/nlhappy/configs/logger/csv.yaml
+-rw-r--r--   0        0        0       94 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/logger/many_loggers.yaml
+-rw-r--r--   0        0        0      214 2024-05-07 07:22:21.911984 nlhappy-2024.5.7/nlhappy/configs/logger/tensorboard.yaml
+-rw-r--r--   0        0        0      394 2024-05-07 07:22:31.232055 nlhappy-2024.5.7/nlhappy/configs/logger/wandb.yaml
+-rw-r--r--   0        0        0      135 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert4qa.yaml
+-rw-r--r--   0        0        0      137 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert4tc.yaml
+-rw-r--r--   0        0        0      158 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert4tpc.yaml
+-rw-r--r--   0        0        0       98 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert_bi_encoder.yaml
+-rw-r--r--   0        0        0      112 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert_crf.yaml
+-rw-r--r--   0        0        0      137 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert_global_span.yaml
+-rw-r--r--   0        0        0      115 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert_lstm_crf.yaml
+-rw-r--r--   0        0        0      112 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert_text_multi_classification.yaml
+-rw-r--r--   0        0        0      129 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/bert_token_classification.yaml
+-rw-r--r--   0        0        0      155 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/biaffine4ee.yaml
+-rw-r--r--   0        0        0      192 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/biaffine4ner.yaml
+-rw-r--r--   0        0        0      181 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/blinker4re.yaml
+-rw-r--r--   0        0        0      168 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/casrel.yaml
+-rw-r--r--   0        0        0       85 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/cosent.yaml
+-rw-r--r--   0        0        0      134 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/crf4ner.yaml
+-rw-r--r--   0        0        0      185 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/globalpointer4clique.yaml
+-rw-r--r--   0        0        0      176 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/globalpointer4ner.yaml
+-rw-r--r--   0        0        0      168 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/globalpointer4qa.yaml
+-rw-r--r--   0        0        0      154 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/gplinker4ee.yaml
+-rw-r--r--   0        0        0      177 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/gplinker4re.yaml
+-rw-r--r--   0        0        0      139 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/onerel.yaml
+-rw-r--r--   0        0        0      140 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/pointer4qa.yaml
+-rw-r--r--   0        0        0      158 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/prompt_gplinker.yaml
+-rw-r--r--   0        0        0      100 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/sentence_bert.yaml
+-rw-r--r--   0        0        0      240 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/model/w2ner.yaml
+-rw-r--r--   0        0        0       71 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/trainer/cpu.yaml
+-rw-r--r--   0        0        0      100 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/trainer/ddp.yaml
+-rw-r--r--   0        0        0      257 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/configs/trainer/debug.yaml
+-rw-r--r--   0        0        0      361 2024-05-07 08:07:57.953734 nlhappy-2024.5.7/nlhappy/configs/trainer/default.yaml
+-rw-r--r--   0        0        0      249 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/data/__init__.py
+-rw-r--r--   0        0        0     1024 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/data/augmentation.py
+-rw-r--r--   0        0        0     3082 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/data/couplet.py
+-rw-r--r--   0        0        0     2964 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/data/dataset.py
+-rw-r--r--   0        0        0    24287 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/data/doc.py
+-rw-r--r--   0        0        0      692 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/__init__.py
+-rw-r--r--   0        0        0     7621 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/entity_extraction.py
+-rw-r--r--   0        0        0    15360 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/event_extraction.py
+-rw-r--r--   0        0        0     4406 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/prompt_relation_extraction.py
+-rw-r--r--   0        0        0     3501 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/prompt_span_extraction.py
+-rw-r--r--   0        0        0     4474 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/question_answering.py
+-rw-r--r--   0        0        0    21894 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/relation_extraction.py
+-rw-r--r--   0        0        0     2850 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/span_extraction.py
+-rw-r--r--   0        0        0     2318 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/text_classification.py
+-rw-r--r--   0        0        0     1572 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/text_multi_classification.py
+-rw-r--r--   0        0        0     3558 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/text_pair_classification.py
+-rw-r--r--   0        0        0     2649 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/text_pair_regression.py
+-rw-r--r--   0        0        0     2212 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/datamodules/token_classification.py
+-rw-r--r--   0        0        0      531 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/layers/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-07 03:30:47.523435 nlhappy-2024.5.7/nlhappy/layers/activation.py
+-rw-r--r--   0        0        0       97 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/attention/__init__.py
+-rw-r--r--   0        0        0     4205 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/attention/multi_head_attention.py
+-rw-r--r--   0        0        0    14626 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/bert.py
+-rw-r--r--   0        0        0      253 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/classifier/__init__.py
+-rw-r--r--   0        0        0     6484 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/classifier/biaffine.py
+-rw-r--r--   0        0        0    17389 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/classifier/crf.py
+-rw-r--r--   0        0        0     9178 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/classifier/global_pointer.py
+-rw-r--r--   0        0        0     1449 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/classifier/onerel.py
+-rw-r--r--   0        0        0      726 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/classifier/simple_dense.py
+-rw-r--r--   0        0        0      661 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/dropout.py
+-rw-r--r--   0        0        0       81 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/embedding/__init__.py
+-rw-r--r--   0        0        0     6159 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/embedding/position_embedding.py
+-rw-r--r--   0        0        0     5170 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/loss.py
+-rw-r--r--   0        0        0     2460 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/normalization.py
+-rw-r--r--   0        0        0     1822 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/layers/word2vec.py
+-rw-r--r--   0        0        0        0 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/metrics/__init__.py
+-rw-r--r--   0        0        0     3342 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/metrics/chunk.py
+-rw-r--r--   0        0        0     1142 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/metrics/entity.py
+-rw-r--r--   0        0        0     1231 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/metrics/event.py
+-rw-r--r--   0        0        0     1248 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/metrics/relation.py
+-rw-r--r--   0        0        0     2610 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/metrics/span.py
+-rw-r--r--   0        0        0     2173 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/metrics/triple.py
+-rw-r--r--   0        0        0      812 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/entity_extraction/__init__.py
+-rw-r--r--   0        0        0     4764 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/entity_extraction/biaffine.py
+-rw-r--r--   0        0        0     4961 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/entity_extraction/crf.py
+-rw-r--r--   0        0        0     6942 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/entity_extraction/globalpointer.py
+-rw-r--r--   0        0        0    13298 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/entity_extraction/w2ner.py
+-rw-r--r--   0        0        0       97 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/event_extraction/__init__.py
+-rw-r--r--   0        0        0    11491 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/event_extraction/biaffine.py
+-rw-r--r--   0        0        0    11305 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/event_extraction/gplinker.py
+-rw-r--r--   0        0        0       57 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/prompt_relation_extraction/__init__.py
+-rw-r--r--   0        0        0    10367 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/prompt_relation_extraction/gplinker.py
+-rw-r--r--   0        0        0       48 2024-05-07 06:59:00.337247 nlhappy-2024.5.7/nlhappy/models/question_answering/__init__.py
+-rw-r--r--   0        0        0     7305 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/question_answering/pointer.py
+-rw-r--r--   0        0        0        0 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/question_answering/t5.py
+-rw-r--r--   0        0        0      383 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/relation_extraction/__init__.py
+-rw-r--r--   0        0        0    10561 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/relation_extraction/biaffine.py
+-rw-r--r--   0        0        0    11329 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/relation_extraction/casrel.py
+-rw-r--r--   0        0        0     9870 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/relation_extraction/gplinker.py
+-rw-r--r--   0        0        0    12097 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/relation_extraction/onerel.py
+-rw-r--r--   0        0        0       41 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/span_extraction/__init__.py
+-rw-r--r--   0        0        0     6290 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/span_extraction/global_pointer.py
+-rw-r--r--   0        0        0       43 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_classification/__init__.py
+-rw-r--r--   0        0        0     4474 2024-05-07 08:23:31.481459 nlhappy-2024.5.7/nlhappy/models/text_classification/bert.py
+-rw-r--r--   0        0        0       71 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_multi_classification/__init__.py
+-rw-r--r--   0        0        0     3108 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_multi_classification/bert_text_multi_classification.py
+-rw-r--r--   0        0        0       89 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_pair_classification/__init__.py
+-rw-r--r--   0        0        0     3013 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_pair_classification/bert_bi_encode.py
+-rw-r--r--   0        0        0     4098 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_pair_classification/bert_cross_encode.py
+-rw-r--r--   0        0        0       75 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_pair_regression/__init__.py
+-rw-r--r--   0        0        0     4820 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_pair_regression/cosent_bert.py
+-rw-r--r--   0        0        0     4786 2024-05-07 03:30:47.527435 nlhappy-2024.5.7/nlhappy/models/text_pair_regression/sentence_bert.py
+-rw-r--r--   0        0        0      196 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/models/token_classification/__init__.py
+-rw-r--r--   0        0        0     5036 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/models/token_classification/bert_crf.py
+-rw-r--r--   0        0        0     5782 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/models/token_classification/bert_lstm_crf.py
+-rw-r--r--   0        0        0     3301 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/models/token_classification/bert_token_classification.py
+-rw-r--r--   0        0        0        3 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/tricks/__init__.py
+-rw-r--r--   0        0        0     6053 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/tricks/adversarial_training.py
+-rw-r--r--   0        0        0        0 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/utils/__init__.py
+-rw-r--r--   0        0        0    14353 2024-05-07 08:20:40.214362 nlhappy-2024.5.7/nlhappy/utils/make_datamodule.py
+-rw-r--r--   0        0        0     5814 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/utils/make_dataset.py
+-rw-r--r--   0        0        0     3712 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/utils/make_doc.py
+-rw-r--r--   0        0        0    20594 2024-05-07 07:19:52.198899 nlhappy-2024.5.7/nlhappy/utils/make_model.py
+-rw-r--r--   0        0        0     8254 2024-05-07 03:30:47.531435 nlhappy-2024.5.7/nlhappy/utils/text.py
+-rw-r--r--   0        0        0     6000 2024-05-07 06:20:18.992735 nlhappy-2024.5.7/nlhappy/utils/utils.py
+-rw-r--r--   0        0        0      793 2024-05-07 08:32:38.385362 nlhappy-2024.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 nlhappy-2024.5.7/PKG-INFO
```

### Comparing `nlhappy-2023.1.31/LICENSE` & `nlhappy-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/README.md` & `nlhappy-2024.5.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -8,23 +8,37 @@
 <a href="https://github.com/ashleve/lightning-hydra-template"><img alt="Template" src="https://img.shields.io/badge/-Lightning--Hydra--Template-017F2F?style=flat&logo=github&labelColor=gray"></a>
 <a href="https://wandb.ai/"><img alt="WanDB" src="https://img.shields.io/badge/Log-WanDB-brightgreen"></a>
 </div>
 <br><br>
 
 ## 📌&nbsp;&nbsp; 简介
 
-nlhappy致力于复现自然语言处理各类任务的SOTA模型。
+nlhappy致力于复现自然语言处理各类任务的SOTA模型(不包含LLM相关任务)。
+
 > 文档地址:
 - [notion文档](https://wangmengdi.notion.site/NLHAPPY-264f05d1084848efa42068c83539904a)
 > 它主要的依赖有
 - [transformers](https://huggingface.co/docs/transformers/index): 下载预训练权重
-- [pytorch-lightning](https://pytorch-lightning.readthedocs.io/en/latest/): 模型训练
+- [pytorch-lightning](https://lightning.ai/docs/pytorch/stable/): 模型训练
 - [datasets](https://huggingface.co/docs/datasets/index): 构建数据集
 - [pydantic](https://wandb.ai/): 数据校验
 
+## 📌&nbsp;&nbsp; 支持NLP任务
+
+- [x] 实体抽取
+- [x] 嵌套实体抽取
+- [x] 非连续实体抽取
+- [x] 关系抽取
+- [x] 事件抽取
+- [x] 文本单标签分类
+- [x] 文本多标签分类
+- [x] 阅读理解
+- [x] 文本对分类
+- [x] 文本对相似度(文本向量化)
+
 
 ## 📌&nbsp;&nbsp; 安装
 <details>
 <summary><b>安装nlhappy</b></summary>
 
 > 推荐先去[pytorch官网](https://pytorch.org/get-started/locally/)安装pytorch和对应cuda
 ```bash
@@ -50,32 +64,8 @@
 ```
 - 使用
 ```
 # 命令行训练
 nlhappy datamodule=xxx model=xxx trainer=xxx logger=wandb
 ```
 模型训练开始后去[官网](https://wandb.ai/)查看训练实况
-</details>
-
-
-## 📌&nbsp;&nbsp; 模型复现
-
-### 实体抽取
-|模型名称|参考链接|
-|----|----|
-|GlobalPointer|[科学空间](https://kexue.fm/archives/8373)|
-|EfficientGlobalPointer|[科学空间](https://kexue.fm/archives/8877)|
-
-### 关系抽取
-|模型名称|参考链接|
-|----|----|
-|GPLinker|[科学空间](https://kexue.fm/archives/8888)|
-
-### 事件抽取
-|模型名称|参考链接|
-|----|----|
-|GPLinker|[科学空间](https://kexue.fm/archives/8926)|
-
-### 答案抽取
-|模型名称|参考链接|
-|----|----|
-|GPLinker|-|
+</details>
```

#### html2text {}

```diff
@@ -1,26 +1,23 @@
          # nlhappy_[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_C_o_n_f_i_g_:_ _H_y_d_r_a_]_[_T_e_m_p_l_a_t_e_]_[_W_a_n_D_B_]
 
 
 ## ð   ç®ä»
-nlhappyè´åäºå¤ç°èªç¶è¯­è¨å¤çåç±»ä»»å¡çSOTAæ¨¡åã >
-ææ¡£å°å: - [notionææ¡£](https://wangmengdi.notion.site/NLHAPPY-
-264f05d1084848efa42068c83539904a) > å®ä¸»è¦çä¾èµæ - [transformers]
-(https://huggingface.co/docs/transformers/index): ä¸è½½é¢è®­ç»æé -
-[pytorch-lightning](https://pytorch-lightning.readthedocs.io/en/latest/):
-æ¨¡åè®­ç» - [datasets](https://huggingface.co/docs/datasets/index):
-æå»ºæ°æ®é - [pydantic](https://wandb.ai/): æ°æ®æ ¡éª ## ð   å®è£
-?å?®??è?£?nnllhhaappppyy > æ¨èåå»[pytorchå®ç½](https://pytorch.org/get-started/
-locally/)å®è£pytorchåå¯¹åºcuda ```bash # pip å®è£ pip install --upgrade
-pip pip install --upgrade nlhappy ``` ?å??¶?ä?»??å??¯?é?? >
+nlhappyè´åäºå¤ç°èªç¶è¯­è¨å¤çåç±»ä»»å¡çSOTAæ¨¡å
+(ä¸åå«LLMç¸å³ä»»å¡)ã > ææ¡£å°å: - [notionææ¡£](https://
+wangmengdi.notion.site/NLHAPPY-264f05d1084848efa42068c83539904a) >
+å®ä¸»è¦çä¾èµæ - [transformers](https://huggingface.co/docs/
+transformers/index): ä¸è½½é¢è®­ç»æé - [pytorch-lightning](https://
+lightning.ai/docs/pytorch/stable/): æ¨¡åè®­ç» - [datasets](https://
+huggingface.co/docs/datasets/index): æå»ºæ°æ®é - [pydantic](https://
+wandb.ai/): æ°æ®æ ¡éª ## ð   æ¯æNLPä»»å¡ - [x] å®ä½æ½å - [x]
+åµå¥å®ä½æ½å - [x] éè¿ç»­å®ä½æ½å - [x] å³ç³»æ½å - [x]
+äºä»¶æ½å - [x] ææ¬åæ ç­¾åç±» - [x] ææ¬å¤æ ç­¾åç±» - [x]
+éè¯»çè§£ - [x] ææ¬å¯¹åç±» - [x] ææ¬å¯¹ç¸ä¼¼åº¦(ææ¬åéå) ##
+ð   å®è£ ?å?®??è?£?nnllhhaappppyy > æ¨èåå»[pytorchå®ç½](https://pytorch.org/
+get-started/locally/)å®è£pytorchåå¯¹åºcuda ```bash # pip å®è£ pip
+install --upgrade pip pip install --upgrade nlhappy ``` ?å??¶?ä?»??å??¯?é?? >
 æ¨èå®è£wandbç¨äºå¯è§åè®­ç»æ¥å¿ - å®è£: ```bash pip install
 wandb ``` - æ³¨å: https://wandb.ai/ - è·åè®¤è¯: https://wandb.ai/
 authorize - ç»é: ```bash wandb login ``` - ä½¿ç¨ ``` # å½ä»¤è¡è®­ç»
 nlhappy datamodule=xxx model=xxx trainer=xxx logger=wandb ```
-æ¨¡åè®­ç»å¼å§åå»[å®ç½](https://wandb.ai/)æ¥çè®­ç»å®åµ ## ð  
-æ¨¡åå¤ç° ### å®ä½æ½å |æ¨¡ååç§°|åèé¾æ¥| |----|----
-| |GlobalPointer|[ç§å­¦ç©ºé´](https://kexue.fm/archives/8373)|
-|EfficientGlobalPointer|[ç§å­¦ç©ºé´](https://kexue.fm/archives/8877)| ###
-å³ç³»æ½å |æ¨¡ååç§°|åèé¾æ¥| |----|----| |GPLinker|[ç§å­¦ç©ºé´]
-(https://kexue.fm/archives/8888)| ### äºä»¶æ½å |æ¨¡ååç§°|åèé¾æ¥|
-|----|----| |GPLinker|[ç§å­¦ç©ºé´](https://kexue.fm/archives/8926)| ###
-ç­æ¡æ½å |æ¨¡ååç§°|åèé¾æ¥| |----|----| |GPLinker|-|
+æ¨¡åè®­ç»å¼å§åå»[å®ç½](https://wandb.ai/)æ¥çè®­ç»å®åµ
```

### Comparing `nlhappy-2023.1.31/nlhappy/algorithms/text_match.py` & `nlhappy-2024.5.7/nlhappy/algorithms/text_match.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/callbacks/ckpt_callbacks.py` & `nlhappy-2024.5.7/nlhappy/callbacks/ckpt_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pytorch_lightning import Callback
+from lightning.pytorch import Callback
 import torch
 import os
 import logging
 
 log = logging.getLogger(__name__)
```

### Comparing `nlhappy-2023.1.31/nlhappy/configs/callbacks/default.yaml` & `nlhappy-2024.5.7/nlhappy/configs/callbacks/default.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 model_checkpoint:
-  _target_: pytorch_lightning.callbacks.ModelCheckpoint
+  _target_: lightning.pytorch.callbacks.ModelCheckpoint
   monitor: ${monitor} # name of the logged metric which determines when model is improving
   mode: "max" # "max" means higher metric value is better, can be also "min"
   save_top_k: 1 # save k best models (determined by above metric)
   save_last: False # additionaly always save model from last epoch
   save_weights_only: True
   verbose: False
   dirpath: "checkpoints/"
   filename: epoch{epoch:02d}_{${monitor}:.3f}
   auto_insert_metric_name: False
 
 
 early_stopping:
-  _target_: pytorch_lightning.callbacks.EarlyStopping
+  _target_: lightning.pytorch.callbacks.EarlyStopping
   monitor: ${monitor} # name of the logged metric which determines when model is improving
   mode: "max" # "max" means higher metric value is better, can be also "min"
   patience: 3 # how many validation epochs of not improving until training stops
   min_delta: 0 # minimum change in the monitored metric needed to qualify as an improvement
 
 
 rich_progress_bar:
-  _target_: pytorch_lightning.callbacks.RichProgressBar
+  _target_: lightning.pytorch.callbacks.RichProgressBar
 
 
 lr_monitor:
-  _target_: pytorch_lightning.callbacks.LearningRateMonitor
+  _target_: lightning.pytorch.callbacks.LearningRateMonitor
   logging_interval: step
```

### Comparing `nlhappy-2023.1.31/nlhappy/configs/callbacks/swa.yaml` & `nlhappy-2024.5.7/nlhappy/configs/callbacks/swa.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 model_checkpoint:
-  _target_: pytorch_lightning.callbacks.ModelCheckpoint
+  _target_: lightning.pytorch.callbacks.ModelCheckpoint
   monitor: ${monitor} # name of the logged metric which determines when model is improving
   mode: "max" # "max" means higher metric value is better, can be also "min"
   save_top_k: 1 # save k best models (determined by above metric)
   save_last: True # additionaly always save model from last epoch
   save_weights_only: True
   verbose: False
   dirpath: "checkpoints/"
```

### Comparing `nlhappy-2023.1.31/nlhappy/configs/config.yaml` & `nlhappy-2024.5.7/nlhappy/configs/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -46,13 +46,16 @@
 # should be used along with experiment mode
 model_info: ${model.name}:lr=${model.lr}
 name: ${model_info}&plm=${datamodule.plm}&bs=${datamodule.batch_size}
 
 # monitor of all callbacks
 monitor: val/f1
 
+# use hf-mirror to download hf models and datasets
+use_hf_mirror: True
+
 hydra:
   run:
     dir: logs/runs/${datamodule.dataset}/${model.name}/${now:%Y-%m-%d}_${now:%H-%M-%S}
   sweep:
     dir: logs/multiruns/${datamodule.dataset}/${model.name}/${now:%Y-%m-%d}_${now:%H-%M-%S}
     subdir: ${hydra.job.num}
```

### Comparing `nlhappy-2023.1.31/nlhappy/data/augmentation.py` & `nlhappy-2024.5.7/nlhappy/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/data/couplet.py` & `nlhappy-2024.5.7/nlhappy/data/couplet.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/data/dataset.py` & `nlhappy-2024.5.7/nlhappy/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/data/doc.py` & `nlhappy-2024.5.7/nlhappy/data/doc.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/__init__.py` & `nlhappy-2024.5.7/nlhappy/datamodules/__init__.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/entity_extraction.py` & `nlhappy-2024.5.7/nlhappy/datamodules/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/event_extraction.py` & `nlhappy-2024.5.7/nlhappy/datamodules/event_extraction.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/prompt_relation_extraction.py` & `nlhappy-2024.5.7/nlhappy/datamodules/prompt_relation_extraction.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/prompt_span_extraction.py` & `nlhappy-2024.5.7/nlhappy/datamodules/prompt_span_extraction.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/question_answering.py` & `nlhappy-2024.5.7/nlhappy/datamodules/question_answering.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/relation_extraction.py` & `nlhappy-2024.5.7/nlhappy/datamodules/relation_extraction.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/span_extraction.py` & `nlhappy-2024.5.7/nlhappy/datamodules/span_extraction.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/text_classification.py` & `nlhappy-2024.5.7/nlhappy/datamodules/text_classification.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/text_multi_classification.py` & `nlhappy-2024.5.7/nlhappy/datamodules/text_multi_classification.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/text_pair_classification.py` & `nlhappy-2024.5.7/nlhappy/datamodules/text_pair_classification.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/text_pair_regression.py` & `nlhappy-2024.5.7/nlhappy/datamodules/text_pair_regression.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/datamodules/token_classification.py` & `nlhappy-2024.5.7/nlhappy/datamodules/token_classification.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/__init__.py` & `nlhappy-2024.5.7/nlhappy/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/activation.py` & `nlhappy-2024.5.7/nlhappy/layers/activation.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/attention/multi_head_attention.py` & `nlhappy-2024.5.7/nlhappy/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/bert.py` & `nlhappy-2024.5.7/nlhappy/layers/bert.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/classifier/biaffine.py` & `nlhappy-2024.5.7/nlhappy/layers/classifier/biaffine.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/classifier/crf.py` & `nlhappy-2024.5.7/nlhappy/layers/classifier/crf.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/classifier/global_pointer.py` & `nlhappy-2024.5.7/nlhappy/layers/classifier/global_pointer.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/classifier/onerel.py` & `nlhappy-2024.5.7/nlhappy/layers/classifier/onerel.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/classifier/simple_dense.py` & `nlhappy-2024.5.7/nlhappy/layers/classifier/simple_dense.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/dropout.py` & `nlhappy-2024.5.7/nlhappy/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/embedding/position_embedding.py` & `nlhappy-2024.5.7/nlhappy/layers/embedding/position_embedding.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/loss.py` & `nlhappy-2024.5.7/nlhappy/layers/loss.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/normalization.py` & `nlhappy-2024.5.7/nlhappy/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/layers/word2vec.py` & `nlhappy-2024.5.7/nlhappy/layers/word2vec.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/metrics/chunk.py` & `nlhappy-2024.5.7/nlhappy/metrics/chunk.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/metrics/entity.py` & `nlhappy-2024.5.7/nlhappy/metrics/entity.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/metrics/event.py` & `nlhappy-2024.5.7/nlhappy/metrics/event.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/metrics/relation.py` & `nlhappy-2024.5.7/nlhappy/metrics/relation.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/metrics/span.py` & `nlhappy-2024.5.7/nlhappy/metrics/span.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/metrics/triple.py` & `nlhappy-2024.5.7/nlhappy/metrics/triple.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/__init__.py` & `nlhappy-2024.5.7/nlhappy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/entity_extraction/biaffine.py` & `nlhappy-2024.5.7/nlhappy/models/entity_extraction/biaffine.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/entity_extraction/crf.py` & `nlhappy-2024.5.7/nlhappy/models/entity_extraction/crf.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/entity_extraction/globalpointer.py` & `nlhappy-2024.5.7/nlhappy/models/entity_extraction/globalpointer.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/entity_extraction/w2ner.py` & `nlhappy-2024.5.7/nlhappy/models/entity_extraction/w2ner.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/event_extraction/biaffine.py` & `nlhappy-2024.5.7/nlhappy/models/event_extraction/biaffine.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/event_extraction/gplinker.py` & `nlhappy-2024.5.7/nlhappy/models/event_extraction/gplinker.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/prompt_relation_extraction/gplinker.py` & `nlhappy-2024.5.7/nlhappy/models/prompt_relation_extraction/gplinker.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/question_answering/pointer.py` & `nlhappy-2024.5.7/nlhappy/models/question_answering/pointer.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/relation_extraction/biaffine.py` & `nlhappy-2024.5.7/nlhappy/models/relation_extraction/biaffine.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/relation_extraction/casrel.py` & `nlhappy-2024.5.7/nlhappy/models/relation_extraction/casrel.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/relation_extraction/gplinker.py` & `nlhappy-2024.5.7/nlhappy/models/relation_extraction/gplinker.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/relation_extraction/onerel.py` & `nlhappy-2024.5.7/nlhappy/models/relation_extraction/onerel.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/span_extraction/global_pointer.py` & `nlhappy-2024.5.7/nlhappy/models/span_extraction/global_pointer.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/text_classification/bert.py` & `nlhappy-2024.5.7/nlhappy/models/text_classification/bert.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
                                       output_size=len(self.hparams.id2label))
         self.dropout = MultiDropout()
         
         # 损失函数
         self.criterion = torch.nn.CrossEntropyLoss()
 
         # 评价指标
-        self.train_f1 = F1Score(num_classes=len(self.hparams.id2label), average='macro')
-        self.val_f1= F1Score(num_classes=len(self.hparams.id2label), average='macro')
-        self.test_f1 = F1Score(num_classes=len(self.hparams.id2label), average='macro')
+        self.train_f1 = F1Score(num_classes=len(self.hparams.id2label), average='macro', task='multiclass')
+        self.val_f1= F1Score(num_classes=len(self.hparams.id2label), average='macro', task='multiclass')
+        self.test_f1 = F1Score(num_classes=len(self.hparams.id2label), average='macro', task='multiclass')
         
     def setup(self, stage: str):
         self.trainer.datamodule.dataset.set_transform(self.trainer.datamodule.bert_transform)
 
 
     def forward(self, input_ids, token_type_ids, attention_mask):
         x = self.bert(input_ids=input_ids, token_type_ids=token_type_ids, attention_mask=attention_mask)
```

### Comparing `nlhappy-2023.1.31/nlhappy/models/text_multi_classification/bert_text_multi_classification.py` & `nlhappy-2024.5.7/nlhappy/models/text_multi_classification/bert_text_multi_classification.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/text_pair_classification/bert_bi_encode.py` & `nlhappy-2024.5.7/nlhappy/models/text_pair_classification/bert_bi_encode.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/text_pair_classification/bert_cross_encode.py` & `nlhappy-2024.5.7/nlhappy/models/text_pair_classification/bert_cross_encode.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/text_pair_regression/cosent_bert.py` & `nlhappy-2024.5.7/nlhappy/models/text_pair_regression/cosent_bert.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/text_pair_regression/sentence_bert.py` & `nlhappy-2024.5.7/nlhappy/models/text_pair_regression/sentence_bert.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/token_classification/bert_crf.py` & `nlhappy-2024.5.7/nlhappy/models/token_classification/bert_crf.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/token_classification/bert_lstm_crf.py` & `nlhappy-2024.5.7/nlhappy/models/token_classification/bert_lstm_crf.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/models/token_classification/bert_token_classification.py` & `nlhappy-2024.5.7/nlhappy/models/token_classification/bert_token_classification.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/run.py` & `nlhappy-2024.5.7/nlhappy/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from typing import List, Optional
 from omegaconf import DictConfig
 from .utils import utils
-from pytorch_lightning import (Callback,
+from lightning.pytorch import (Callback,
                                LightningDataModule,
                                LightningModule,
                                Trainer,
                                seed_everything)
-from pytorch_lightning.loggers import LightningLoggerBase
+from lightning.pytorch.loggers import Logger
 import hydra
 import os
 
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 log = utils.get_logger(__name__)
 
 
-@hydra.main(config_path="configs/", config_name="config.yaml")
-def train(config: DictConfig) -> Optional[float]:
+@hydra.main(config_path="configs/", config_name="config.yaml", version_base='1.1')
+def run(config: DictConfig) -> Optional[float]:
     """Contains training pipeline.
     Instantiates all PyTorch Lightning objects from config.
 
     Args:
         config (DictConfig): Configuration composed by Hydra.
 
     Returns:
         Optional[float]: Metric score for hyperparameter optimization.
     """
     
     utils.extras(config)
     if config.get("print_config"):
         utils.print_config(config, resolve=True)
-
+        
+    if config.get("use_hf_mirror"):
+        os.environ["HF_ENDPOINT"] = "https://hf-mirror.com"
+        log.info("Using hf-mirror to download datasets and models!")
+        
     # Set seed for random number generators in pytorch, numpy and python.random
     if config.get("seed"):
         seed_everything(config.seed, workers=True)
 
     # Init lightning datamodule
     if len(config.datamodule) > 0:
         log.info(f"Instantiating datamodule <{config.datamodule._target_}>")
@@ -56,25 +60,24 @@
     if "callbacks" in config:
         for _, cb_conf in config.callbacks.items():
             if "_target_" in cb_conf:
                 log.info(f"Instantiating callback <{cb_conf._target_}>")
                 callbacks.append(hydra.utils.instantiate(cb_conf))
 
     # Init lightning loggers
-    logger: List[LightningLoggerBase] = []
+    logger: List[Logger] = []
     if "logger" in config:
             log.info(f"Instantiating logger <{config.logger._target_}>")
             logger.append(hydra.utils.instantiate(config.logger))
 
     # Init lightning trainer
     log.info(f"Instantiating trainer <{config.trainer._target_}>")
     trainer: Trainer = hydra.utils.instantiate(config.trainer, 
                                                callbacks=callbacks, 
-                                               logger=logger, 
-                                               _convert_="partial")
+                                               logger=logger)
 
     # Send some parameters from config to all lightning loggers
     log.info("Logging hyperparameters!")
     utils.log_hyperparameters(config=config,
                               model=model,
                               datamodule=datamodule,
                               trainer=trainer,
@@ -115,8 +118,8 @@
         log.info(f"Best model ckpt at {trainer.checkpoint_callback.best_model_path}")
 
     # Return metric score for hyperparameter optimization
     return score
 
 
 if __name__ == "__main__":
-    train()
+    run()
```

### Comparing `nlhappy-2023.1.31/nlhappy/tricks/adversarial_training.py` & `nlhappy-2024.5.7/nlhappy/tricks/adversarial_training.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/utils/make_datamodule.py` & `nlhappy-2024.5.7/nlhappy/utils/make_datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from .utils import get_logger
 from typing import Union, List
 from torch.utils.data import DataLoader, BatchSampler, RandomSampler
 from datasets import load_from_disk, load_dataset, DatasetDict
-import pytorch_lightning as pl
 from transformers import AutoConfig, AutoTokenizer, AutoModel, PreTrainedTokenizerFast
 from functools import lru_cache
 from pathlib import Path
 import numpy as np
-from pytorch_lightning import LightningDataModule
+from lightning.pytorch import LightningDataModule
+from huggingface_hub import snapshot_download
 
 
 log = get_logger()
 
 
 def sequence_padding(inputs, length=None, value=0, seq_dims=1, mode='post'):
     """Numpy函数，将序列padding到同一长度
@@ -139,15 +139,19 @@
     path = Path(dataset_dir, dataset_name)
     if path.exists():
         pass
     else:
         log.info('cannot found dataset in {}.'.format(path))
         try:
             log.info(f'download dataset {dataset_name} from huffingface')
+            snapshot_download(dataset_name, 
+                              repo_type='dataset',
+                              endpoint="https://hf-mirror.com")
             dataset = load_dataset(dataset_name)
+            dataset.save_to_disk(path)
             log.info(f'download dataset succeed')
         except Exception as e:
             log.error('download dataset failed')
             raise(e)
             
             
 def prepare_plm(plm_name: str, plm_dir: str) -> None:
@@ -175,15 +179,15 @@
         '''
         下载数据集和预训练模型这个方法只会在一个GPU上执行一次.
         '''
         prepare_dataset(dataset_name=dataset, dataset_dir=dataset_dir)
         prepare_plm(plm_name=plm, plm_dir=plm_dir)
 
 
-class PLMBaseDataModule(pl.LightningModule):
+class PLMBaseDataModule(LightningDataModule):
     """数据模块的基类,子类需要完成setup方法,子类初始化的时候至少包含dataset,plm,batch_size参数,
     内置功能:
     - 自动保存超参数
     - 不同策略自动获取最大文本长度,超过512则取512
     - 下载数据集和预训练模型
     - 自动读取tokenizer
     - 自动读取数据集
```

### Comparing `nlhappy-2023.1.31/nlhappy/utils/make_dataset.py` & `nlhappy-2024.5.7/nlhappy/utils/make_dataset.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/utils/make_doc.py` & `nlhappy-2024.5.7/nlhappy/utils/make_doc.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/utils/make_model.py` & `nlhappy-2024.5.7/nlhappy/utils/make_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import lru_cache
 from typing import Dict, Tuple, Union, List
 import os
 from transformers import AutoTokenizer, AutoConfig, AutoModel, BertModel, BertConfig
 from transformers.optimization import get_linear_schedule_with_warmup, get_cosine_schedule_with_warmup
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
 import torch
 import tempfile
 import json
 from omegaconf import OmegaConf, DictConfig
 from pathlib import Path
 from torch.utils.data import DataLoader, BatchSampler, RandomSampler
 from datasets import load_from_disk, load_dataset
```

### Comparing `nlhappy-2023.1.31/nlhappy/utils/text.py` & `nlhappy-2024.5.7/nlhappy/utils/text.py`

 * *Files identical despite different names*

### Comparing `nlhappy-2023.1.31/nlhappy/utils/utils.py` & `nlhappy-2024.5.7/nlhappy/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import warnings
 from typing import List, Sequence
-import pytorch_lightning as pl
+from lightning.pytorch.loggers import Logger, WandbLogger
+from lightning.pytorch import LightningDataModule, LightningModule, Trainer, Callback
 import rich.syntax
 import rich.tree
 from omegaconf import DictConfig, OmegaConf
-from pytorch_lightning.utilities import rank_zero_only
+from lightning.pytorch.utilities import rank_zero_only
 import os
 
 
 def get_logger(name=__name__) -> logging.Logger:
     """Initializes multi-GPU-friendly python command line logger."""
 
     logger = logging.getLogger(name)
@@ -112,19 +113,19 @@
     with open("config_tree.log", "w") as fp:
         rich.print(tree, file=fp)
 
 
 @rank_zero_only
 def log_hyperparameters(
     config: DictConfig,
-    model: pl.LightningModule,
-    datamodule: pl.LightningDataModule,
-    trainer: pl.Trainer,
-    callbacks: List[pl.Callback],
-    logger: List[pl.loggers.LightningLoggerBase],
+    model: LightningModule,
+    datamodule: LightningDataModule,
+    trainer: Trainer,
+    callbacks: List[Callback],
+    logger: List[Logger],
 ) -> None:
     """This method controls which parameters from Hydra config are saved by Lightning loggers.
 
     Additionaly saves:
         - number of model parameters
     """
     
@@ -154,25 +155,25 @@
 
     # send hparams to all loggers
     trainer.logger.log_hyperparams(hparams)
 
 
 def finish(
     config: DictConfig,
-    model: pl.LightningModule,
-    datamodule: pl.LightningDataModule,
-    trainer: pl.Trainer,
-    callbacks: List[pl.Callback],
-    logger: List[pl.loggers.LightningLoggerBase],
+    model: LightningModule,
+    datamodule: LightningDataModule,
+    trainer: Trainer,
+    callbacks: List[Callback],
+    logger: List[Logger],
 ) -> None:
     """Makes sure everything closed properly."""
 
     # without this sweeps with wandb logger might crash!
     for lg in logger:
-        if isinstance(lg, pl.loggers.wandb.WandbLogger):
+        if isinstance(lg, WandbLogger):
             import wandb
 
             wandb.finish()
 
 
 def zip_all_files(dir,zipFile,pre_dir):
     """递归压缩文件夹下的所有文件
```

### Comparing `nlhappy-2023.1.31/pyproject.toml` & `nlhappy-2024.5.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "nlhappy"
-version = "2023.1.31"
+version = "2024.5.7"
 description = "自然语言处理(NLP)"
 authors = ["wangmengdi <790990241@qq.om>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://wangmengdi.notion.site/NLHAPPY-264f05d1084848efa42068c83539904a"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
-torch = ">=1.8.0"
+torch = ">=2.0.0"
 # pl>1.6.5,<=1.7.7的版本,会出现checkpoint无法加载的问题,原因是实例化model的时候会有datamodule的hparams,暂时无法解决
-pytorch-lightning = ">=1.6.5" 
+lightning = ">=2.0.0" 
 datasets = ">=2.0.0"
 transformers = ">=4.17.0"
-hydra-core = "1.1"
+hydra-core = "==1.3.2"
 hydra-colorlog = ">=1.1.0"
 rich = "^12.4.3"
 srsly = ">=2.4.5"
-pydantic = "1.10.2"
+pydantic = ">=1.10.2"
 
 
 [tool.poetry.scripts]
-nlhappy = "nlhappy.run:train"
+nlhappy = "nlhappy.__main__:train"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nlhappy-2023.1.31/PKG-INFO` & `nlhappy-2024.5.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: nlhappy
-Version: 2023.1.31
+Version: 2024.5.7
 Summary: 自然语言处理(NLP)
 License: MIT
 Author: wangmengdi
 Author-email: 790990241@qq.om
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasets (>=2.0.0)
 Requires-Dist: hydra-colorlog (>=1.1.0)
-Requires-Dist: hydra-core (==1.1)
-Requires-Dist: pydantic (==1.10.2)
-Requires-Dist: pytorch-lightning (>=1.6.5)
+Requires-Dist: hydra-core (==1.3.2)
+Requires-Dist: lightning (>=2.0.0)
+Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: rich (>=12.4.3,<13.0.0)
 Requires-Dist: srsly (>=2.4.5)
-Requires-Dist: torch (>=1.8.0)
+Requires-Dist: torch (>=2.0.0)
 Requires-Dist: transformers (>=4.17.0)
 Project-URL: Documentation, https://wangmengdi.notion.site/NLHAPPY-264f05d1084848efa42068c83539904a
 Description-Content-Type: text/markdown
 
 
 <div align='center'>
 
@@ -34,23 +36,37 @@
 <a href="https://github.com/ashleve/lightning-hydra-template"><img alt="Template" src="https://img.shields.io/badge/-Lightning--Hydra--Template-017F2F?style=flat&logo=github&labelColor=gray"></a>
 <a href="https://wandb.ai/"><img alt="WanDB" src="https://img.shields.io/badge/Log-WanDB-brightgreen"></a>
 </div>
 <br><br>
 
 ## 📌&nbsp;&nbsp; 简介
 
-nlhappy致力于复现自然语言处理各类任务的SOTA模型。
+nlhappy致力于复现自然语言处理各类任务的SOTA模型(不包含LLM相关任务)。
+
 > 文档地址:
 - [notion文档](https://wangmengdi.notion.site/NLHAPPY-264f05d1084848efa42068c83539904a)
 > 它主要的依赖有
 - [transformers](https://huggingface.co/docs/transformers/index): 下载预训练权重
-- [pytorch-lightning](https://pytorch-lightning.readthedocs.io/en/latest/): 模型训练
+- [pytorch-lightning](https://lightning.ai/docs/pytorch/stable/): 模型训练
 - [datasets](https://huggingface.co/docs/datasets/index): 构建数据集
 - [pydantic](https://wandb.ai/): 数据校验
 
+## 📌&nbsp;&nbsp; 支持NLP任务
+
+- [x] 实体抽取
+- [x] 嵌套实体抽取
+- [x] 非连续实体抽取
+- [x] 关系抽取
+- [x] 事件抽取
+- [x] 文本单标签分类
+- [x] 文本多标签分类
+- [x] 阅读理解
+- [x] 文本对分类
+- [x] 文本对相似度(文本向量化)
+
 
 ## 📌&nbsp;&nbsp; 安装
 <details>
 <summary><b>安装nlhappy</b></summary>
 
 > 推荐先去[pytorch官网](https://pytorch.org/get-started/locally/)安装pytorch和对应cuda
 ```bash
@@ -77,31 +93,7 @@
 - 使用
 ```
 # 命令行训练
 nlhappy datamodule=xxx model=xxx trainer=xxx logger=wandb
 ```
 模型训练开始后去[官网](https://wandb.ai/)查看训练实况
 </details>
-
-
-## 📌&nbsp;&nbsp; 模型复现
-
-### 实体抽取
-|模型名称|参考链接|
-|----|----|
-|GlobalPointer|[科学空间](https://kexue.fm/archives/8373)|
-|EfficientGlobalPointer|[科学空间](https://kexue.fm/archives/8877)|
-
-### 关系抽取
-|模型名称|参考链接|
-|----|----|
-|GPLinker|[科学空间](https://kexue.fm/archives/8888)|
-
-### 事件抽取
-|模型名称|参考链接|
-|----|----|
-|GPLinker|[科学空间](https://kexue.fm/archives/8926)|
-
-### 答案抽取
-|模型名称|参考链接|
-|----|----|
-|GPLinker|-|
```

#### html2text {}

```diff
@@ -1,39 +1,37 @@
-Metadata-Version: 2.1 Name: nlhappy Version: 2023.1.31 Summary:
+Metadata-Version: 2.1 Name: nlhappy Version: 2024.5.7 Summary:
 èªç¶è¯­è¨å¤ç(NLP) License: MIT Author: wangmengdi Author-email:
 790990241@qq.om Requires-Python: >=3.7 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Requires-Dist: datasets (>=2.0.0)
-Requires-Dist: hydra-colorlog (>=1.1.0) Requires-Dist: hydra-core (==1.1)
-Requires-Dist: pydantic (==1.10.2) Requires-Dist: pytorch-lightning (>=1.6.5)
-Requires-Dist: rich (>=12.4.3,<13.0.0) Requires-Dist: srsly (>=2.4.5) Requires-
-Dist: torch (>=1.8.0) Requires-Dist: transformers (>=4.17.0) Project-URL:
-Documentation, https://wangmengdi.notion.site/NLHAPPY-
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: datasets (>=2.0.0) Requires-Dist: hydra-colorlog (>=1.1.0) Requires-Dist:
+hydra-core (==1.3.2) Requires-Dist: lightning (>=2.0.0) Requires-Dist: pydantic
+(>=1.10.2) Requires-Dist: rich (>=12.4.3,<13.0.0) Requires-Dist: srsly
+(>=2.4.5) Requires-Dist: torch (>=2.0.0) Requires-Dist: transformers (>=4.17.0)
+Project-URL: Documentation, https://wangmengdi.notion.site/NLHAPPY-
 264f05d1084848efa42068c83539904a Description-Content-Type: text/markdown
          # nlhappy_[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_C_o_n_f_i_g_:_ _H_y_d_r_a_]_[_T_e_m_p_l_a_t_e_]_[_W_a_n_D_B_]
 
 
 ## ð   ç®ä»
-nlhappyè´åäºå¤ç°èªç¶è¯­è¨å¤çåç±»ä»»å¡çSOTAæ¨¡åã >
-ææ¡£å°å: - [notionææ¡£](https://wangmengdi.notion.site/NLHAPPY-
-264f05d1084848efa42068c83539904a) > å®ä¸»è¦çä¾èµæ - [transformers]
-(https://huggingface.co/docs/transformers/index): ä¸è½½é¢è®­ç»æé -
-[pytorch-lightning](https://pytorch-lightning.readthedocs.io/en/latest/):
-æ¨¡åè®­ç» - [datasets](https://huggingface.co/docs/datasets/index):
-æå»ºæ°æ®é - [pydantic](https://wandb.ai/): æ°æ®æ ¡éª ## ð   å®è£
-?å?®??è?£?nnllhhaappppyy > æ¨èåå»[pytorchå®ç½](https://pytorch.org/get-started/
-locally/)å®è£pytorchåå¯¹åºcuda ```bash # pip å®è£ pip install --upgrade
-pip pip install --upgrade nlhappy ``` ?å??¶?ä?»??å??¯?é?? >
+nlhappyè´åäºå¤ç°èªç¶è¯­è¨å¤çåç±»ä»»å¡çSOTAæ¨¡å
+(ä¸åå«LLMç¸å³ä»»å¡)ã > ææ¡£å°å: - [notionææ¡£](https://
+wangmengdi.notion.site/NLHAPPY-264f05d1084848efa42068c83539904a) >
+å®ä¸»è¦çä¾èµæ - [transformers](https://huggingface.co/docs/
+transformers/index): ä¸è½½é¢è®­ç»æé - [pytorch-lightning](https://
+lightning.ai/docs/pytorch/stable/): æ¨¡åè®­ç» - [datasets](https://
+huggingface.co/docs/datasets/index): æå»ºæ°æ®é - [pydantic](https://
+wandb.ai/): æ°æ®æ ¡éª ## ð   æ¯æNLPä»»å¡ - [x] å®ä½æ½å - [x]
+åµå¥å®ä½æ½å - [x] éè¿ç»­å®ä½æ½å - [x] å³ç³»æ½å - [x]
+äºä»¶æ½å - [x] ææ¬åæ ç­¾åç±» - [x] ææ¬å¤æ ç­¾åç±» - [x]
+éè¯»çè§£ - [x] ææ¬å¯¹åç±» - [x] ææ¬å¯¹ç¸ä¼¼åº¦(ææ¬åéå) ##
+ð   å®è£ ?å?®??è?£?nnllhhaappppyy > æ¨èåå»[pytorchå®ç½](https://pytorch.org/
+get-started/locally/)å®è£pytorchåå¯¹åºcuda ```bash # pip å®è£ pip
+install --upgrade pip pip install --upgrade nlhappy ``` ?å??¶?ä?»??å??¯?é?? >
 æ¨èå®è£wandbç¨äºå¯è§åè®­ç»æ¥å¿ - å®è£: ```bash pip install
 wandb ``` - æ³¨å: https://wandb.ai/ - è·åè®¤è¯: https://wandb.ai/
 authorize - ç»é: ```bash wandb login ``` - ä½¿ç¨ ``` # å½ä»¤è¡è®­ç»
 nlhappy datamodule=xxx model=xxx trainer=xxx logger=wandb ```
-æ¨¡åè®­ç»å¼å§åå»[å®ç½](https://wandb.ai/)æ¥çè®­ç»å®åµ ## ð  
-æ¨¡åå¤ç° ### å®ä½æ½å |æ¨¡ååç§°|åèé¾æ¥| |----|----
-| |GlobalPointer|[ç§å­¦ç©ºé´](https://kexue.fm/archives/8373)|
-|EfficientGlobalPointer|[ç§å­¦ç©ºé´](https://kexue.fm/archives/8877)| ###
-å³ç³»æ½å |æ¨¡ååç§°|åèé¾æ¥| |----|----| |GPLinker|[ç§å­¦ç©ºé´]
-(https://kexue.fm/archives/8888)| ### äºä»¶æ½å |æ¨¡ååç§°|åèé¾æ¥|
-|----|----| |GPLinker|[ç§å­¦ç©ºé´](https://kexue.fm/archives/8926)| ###
-ç­æ¡æ½å |æ¨¡ååç§°|åèé¾æ¥| |----|----| |GPLinker|-|
+æ¨¡åè®­ç»å¼å§åå»[å®ç½](https://wandb.ai/)æ¥çè®­ç»å®åµ
```

