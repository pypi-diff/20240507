# Comparing `tmp/docugami_langchain-0.0.9rc2.tar.gz` & `tmp/docugami_langchain-0.0.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugami_langchain-0.0.9rc2.tar", max compression
+gzip compressed data, was "docugami_langchain-0.0.9rc3.tar", max compression
```

## Comparing `docugami_langchain-0.0.9rc2.tar` & `docugami_langchain-0.0.9rc3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1072 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/LICENSE
--rw-r--r--   0        0        0      361 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/README.md
--rw-r--r--   0        0        0      747 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/__init__.py
--rw-r--r--   0        0        0      487 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/__init__.py
--rw-r--r--   0        0        0     8459 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/base.py
--rw-r--r--   0        0        0     1805 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/models.py
--rw-r--r--   0        0        0    10928 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/re_act_agent.py
--rw-r--r--   0        0        0     8325 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/tool_router_agent.py
--rw-r--r--   0        0        0    16628 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/base_runnable.py
--rw-r--r--   0        0        0     1396 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/__init__.py
--rw-r--r--   0        0        0     2210 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/answer_chain.py
--rw-r--r--   0        0        0     1415 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/base.py
--rw-r--r--   0        0        0      243 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/__init__.py
--rw-r--r--   0        0        0     3390 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
--rw-r--r--   0        0        0     3980 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/summarize_chunk_chain.py
--rw-r--r--   0        0        0      291 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/__init__.py
--rw-r--r--   0        0        0     3838 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/describe_document_set_chain.py
--rw-r--r--   0        0        0     3983 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/summarize_document_chain.py
--rw-r--r--   0        0        0      647 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/__init__.py
--rw-r--r--   0        0        0     3398 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
--rw-r--r--   0        0        0      262 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/models.py
--rw-r--r--   0        0        0     3999 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_fixup_chain.py
--rw-r--r--   0        0        0     4360 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_query_explainer_chain.py
--rw-r--r--   0        0        0     8808 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_chain.py
--rw-r--r--   0        0        0     3522 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_explainer_chain.py
--rw-r--r--   0        0        0      498 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/__init__.py
--rw-r--r--   0        0        0      124 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/models.py
--rw-r--r--   0        0        0     4409 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/simple_rag_chain.py
--rw-r--r--   0        0        0     4006 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/standalone_question_chain.py
--rw-r--r--   0        0        0     4592 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_questions_chain.py
--rw-r--r--   0        0        0     4193 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_report_chain.py
--rw-r--r--   0        0        0     4832 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/tool_final_answer_chain.py
--rw-r--r--   0        0        0      567 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/__init__.py
--rw-r--r--   0        0        0      999 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/common.py
--rw-r--r--   0        0        0     3147 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/data_type_detection_chain.py
--rw-r--r--   0        0        0     3243 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_add_chain.py
--rw-r--r--   0        0        0     2963 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_parse_chain.py
--rw-r--r--   0        0        0     2464 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/timespan_parse_chain.py
--rw-r--r--   0        0        0     1604 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/config.py
--rw-r--r--   0        0        0      109 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0    13516 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0     2798 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/history.py
--rw-r--r--   0        0        0      797 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     4206 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/custom_react_json_single_input.py
--rw-r--r--   0        0        0     2091 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1075 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/key_finding.py
--rw-r--r--   0        0        0     1242 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/line_separated_list.py
--rw-r--r--   0        0        0     2816 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/sql_finding.py
--rw-r--r--   0        0        0      735 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/text_cleaning.py
--rw-r--r--   0        0        0     4502 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/timespan.py
--rw-r--r--   0        0        0      833 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/params.py
--rw-r--r--   0        0        0      122 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/py.typed
--rw-r--r--   0        0        0      165 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/__init__.py
--rw-r--r--   0        0        0     7894 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/fused_summary.py
--rw-r--r--   0        0        0     5760 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/mappings.py
--rw-r--r--   0        0        0      194 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/__init__.py
--rw-r--r--   0        0        0     3958 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/common.py
--rw-r--r--   0        0        0     8697 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/reports.py
--rw-r--r--   0        0        0     6830 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/retrieval.py
--rw-r--r--   0        0        0      708 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/utils/documents.py
--rw-r--r--   0        0        0     8975 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/utils/sql.py
--rw-r--r--   0        0        0     3389 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/utils/string_cleanup.py
--rw-r--r--   0        0        0     2829 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/pyproject.toml
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/LICENSE
+-rw-r--r--   0        0        0      361 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/README.md
+-rw-r--r--   0        0        0      747 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/agents/__init__.py
+-rw-r--r--   0        0        0     8459 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/agents/base.py
+-rw-r--r--   0        0        0     1805 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/agents/models.py
+-rw-r--r--   0        0        0    10928 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/agents/re_act_agent.py
+-rw-r--r--   0        0        0     8325 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/agents/tool_router_agent.py
+-rw-r--r--   0        0        0    16628 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/base_runnable.py
+-rw-r--r--   0        0        0     1396 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/answer_chain.py
+-rw-r--r--   0        0        0     1415 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/base.py
+-rw-r--r--   0        0        0      243 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/chunks/__init__.py
+-rw-r--r--   0        0        0     3390 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
+-rw-r--r--   0        0        0     3980 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/chunks/summarize_chunk_chain.py
+-rw-r--r--   0        0        0      291 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/documents/__init__.py
+-rw-r--r--   0        0        0     3838 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/documents/describe_document_set_chain.py
+-rw-r--r--   0        0        0     3983 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/documents/summarize_document_chain.py
+-rw-r--r--   0        0        0      647 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/__init__.py
+-rw-r--r--   0        0        0     3398 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
+-rw-r--r--   0        0        0      262 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/models.py
+-rw-r--r--   0        0        0     3999 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_fixup_chain.py
+-rw-r--r--   0        0        0     4360 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_query_explainer_chain.py
+-rw-r--r--   0        0        0     8808 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_result_chain.py
+-rw-r--r--   0        0        0     3522 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_result_explainer_chain.py
+-rw-r--r--   0        0        0      498 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/models.py
+-rw-r--r--   0        0        0     4409 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/simple_rag_chain.py
+-rw-r--r--   0        0        0     4006 2024-05-07 17:55:32.084161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/standalone_question_chain.py
+-rw-r--r--   0        0        0     4592 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/suggested_questions_chain.py
+-rw-r--r--   0        0        0     4193 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/suggested_report_chain.py
+-rw-r--r--   0        0        0     4832 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/tool_final_answer_chain.py
+-rw-r--r--   0        0        0      567 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/common.py
+-rw-r--r--   0        0        0     3147 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/data_type_detection_chain.py
+-rw-r--r--   0        0        0     3243 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/date_add_chain.py
+-rw-r--r--   0        0        0     2963 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/date_parse_chain.py
+-rw-r--r--   0        0        0     2464 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/timespan_parse_chain.py
+-rw-r--r--   0        0        0     1604 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/config.py
+-rw-r--r--   0        0        0      109 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13516 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     2798 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/history.py
+-rw-r--r--   0        0        0      797 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     4206 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/custom_react_json_single_input.py
+-rw-r--r--   0        0        0     2091 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1075 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/key_finding.py
+-rw-r--r--   0        0        0     1242 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/line_separated_list.py
+-rw-r--r--   0        0        0     2816 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/sql_finding.py
+-rw-r--r--   0        0        0      735 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/text_cleaning.py
+-rw-r--r--   0        0        0     4502 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/timespan.py
+-rw-r--r--   0        0        0      833 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/params.py
+-rw-r--r--   0        0        0      122 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/py.typed
+-rw-r--r--   0        0        0      165 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0     7894 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/retrievers/fused_summary.py
+-rw-r--r--   0        0        0     5890 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/retrievers/mappings.py
+-rw-r--r--   0        0        0      194 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/tools/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/tools/common.py
+-rw-r--r--   0        0        0     8697 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/tools/reports.py
+-rw-r--r--   0        0        0     6830 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/tools/retrieval.py
+-rw-r--r--   0        0        0      708 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/utils/documents.py
+-rw-r--r--   0        0        0     8975 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/utils/sql.py
+-rw-r--r--   0        0        0     3389 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/docugami_langchain/utils/string_cleanup.py
+-rw-r--r--   0        0        0     2829 2024-05-07 17:55:32.088161 docugami_langchain-0.0.9rc3/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc3/PKG-INFO
```

### Comparing `docugami_langchain-0.0.9rc2/LICENSE` & `docugami_langchain-0.0.9rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/__init__.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/agents/base.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/agents/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/agents/models.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/agents/models.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/agents/re_act_agent.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/agents/re_act_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/agents/tool_router_agent.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/agents/tool_router_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/base_runnable.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/base_runnable.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/__init__.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/answer_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/base.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/elaborate_chunk_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/chunks/elaborate_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/summarize_chunk_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/chunks/summarize_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/describe_document_set_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/documents/describe_document_set_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/summarize_document_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/documents/summarize_document_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/__init__.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_fixup_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_fixup_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_query_explainer_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_query_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_result_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_explainer_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/querying/sql_result_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/simple_rag_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/simple_rag_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/standalone_question_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/standalone_question_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_questions_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/suggested_questions_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_report_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/suggested_report_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/tool_final_answer_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/rag/tool_final_answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/__init__.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/common.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/data_type_detection_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/data_type_detection_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_add_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/date_add_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_parse_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/date_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/timespan_parse_chain.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/chains/types/timespan_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/config.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/config.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/document_loaders/docugami.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/history.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/history.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/__init__.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/custom_react_json_single_input.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/custom_react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/datetime.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/key_finding.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/key_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/line_separated_list.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/line_separated_list.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/sql_finding.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/sql_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/text_cleaning.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/timespan.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/output_parsers/timespan.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/params.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/params.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/fused_summary.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/retrievers/fused_summary.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/mappings.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/retrievers/mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     docs_by_id: dict[str, Document],
     llm: BaseLanguageModel,
     embeddings: Embeddings,
     include_xml_tags: bool = INCLUDE_XML_TAGS,
     min_length_to_summarize: int = MIN_LENGTH_TO_SUMMARIZE,
     max_length_cutoff: int = MAX_FULL_DOCUMENT_TEXT_LENGTH,
     summarize_document_examples_file: Optional[Path] = None,
+    batch_size: int = BATCH_SIZE,
 ) -> dict[str, Document]:
     """
     Build summary mappings for all the given full documents.
     """
 
     chain = SummarizeDocumentChain(llm=llm, embeddings=embeddings)
     chain.min_length_to_summarize = min_length_to_summarize
@@ -79,25 +80,27 @@
     if summarize_document_examples_file:
         chain.load_examples(summarize_document_examples_file)
 
     return _build_summary_mappings(
         docs_by_id=docs_by_id,
         chain=chain,
         include_xml_tags=include_xml_tags,
+        batch_size=batch_size,
     )
 
 
 def build_chunk_summary_mappings(
     docs_by_id: dict[str, Document],
     llm: BaseLanguageModel,
     embeddings: Embeddings,
     include_xml_tags: bool = INCLUDE_XML_TAGS,
     min_length_to_summarize: int = MIN_LENGTH_TO_SUMMARIZE,
     max_length_cutoff: int = MAX_CHUNK_TEXT_LENGTH,
     summarize_chunk_examples_file: Optional[Path] = None,
+    batch_size: int = BATCH_SIZE,
 ) -> dict[str, Document]:
     """
     Build summary mappings for all the given chunks.
     """
 
     chain = SummarizeChunkChain(llm=llm, embeddings=embeddings)
     chain.min_length_to_summarize = min_length_to_summarize
@@ -105,14 +108,15 @@
     if summarize_chunk_examples_file:
         chain.load_examples(summarize_chunk_examples_file)
 
     return _build_summary_mappings(
         docs_by_id=docs_by_id,
         chain=chain,
         include_xml_tags=include_xml_tags,
+        batch_size=batch_size,
     )
 
 
 def build_doc_maps_from_chunks(
     chunks: list[Document],
     chunk_id_key: str = "id",
     parent_id_key: str = PARENT_DOC_ID_KEY,
```

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/tools/common.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/tools/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/tools/reports.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/tools/reports.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/tools/retrieval.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/utils/documents.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/utils/documents.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/utils/sql.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/utils/sql.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/docugami_langchain/utils/string_cleanup.py` & `docugami_langchain-0.0.9rc3/docugami_langchain/utils/string_cleanup.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc2/pyproject.toml` & `docugami_langchain-0.0.9rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docugami-langchain"
-version = "0.0.9rc2"
+version = "0.0.9rc3"
 description = "An integration package connecting Docugami and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/docugami/docugami-langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `docugami_langchain-0.0.9rc2/PKG-INFO` & `docugami_langchain-0.0.9rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugami-langchain
-Version: 0.0.9rc2
+Version: 0.0.9rc3
 Summary: An integration package connecting Docugami and LangChain
 Home-page: https://github.com/docugami/docugami-langchain
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

