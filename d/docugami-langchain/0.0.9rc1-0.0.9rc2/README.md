# Comparing `tmp/docugami_langchain-0.0.9rc1.tar.gz` & `tmp/docugami_langchain-0.0.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugami_langchain-0.0.9rc1.tar", max compression
+gzip compressed data, was "docugami_langchain-0.0.9rc2.tar", max compression
```

## Comparing `docugami_langchain-0.0.9rc1.tar` & `docugami_langchain-0.0.9rc2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1072 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/LICENSE
--rw-r--r--   0        0        0      361 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/README.md
--rw-r--r--   0        0        0      747 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/__init__.py
--rw-r--r--   0        0        0      487 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/__init__.py
--rw-r--r--   0        0        0     8459 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/base.py
--rw-r--r--   0        0        0     1805 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/models.py
--rw-r--r--   0        0        0    10928 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/re_act_agent.py
--rw-r--r--   0        0        0     8325 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/tool_router_agent.py
--rw-r--r--   0        0        0    16628 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/base_runnable.py
--rw-r--r--   0        0        0     1396 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/__init__.py
--rw-r--r--   0        0        0     2210 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/answer_chain.py
--rw-r--r--   0        0        0     1415 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/base.py
--rw-r--r--   0        0        0      243 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/__init__.py
--rw-r--r--   0        0        0     3390 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
--rw-r--r--   0        0        0     3980 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/summarize_chunk_chain.py
--rw-r--r--   0        0        0      291 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/__init__.py
--rw-r--r--   0        0        0     3838 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/describe_document_set_chain.py
--rw-r--r--   0        0        0     3983 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/summarize_document_chain.py
--rw-r--r--   0        0        0      647 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/__init__.py
--rw-r--r--   0        0        0     3398 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
--rw-r--r--   0        0        0      262 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/models.py
--rw-r--r--   0        0        0     3999 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_fixup_chain.py
--rw-r--r--   0        0        0     4360 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_query_explainer_chain.py
--rw-r--r--   0        0        0     8808 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_chain.py
--rw-r--r--   0        0        0     3522 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_explainer_chain.py
--rw-r--r--   0        0        0      498 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/__init__.py
--rw-r--r--   0        0        0      124 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/models.py
--rw-r--r--   0        0        0     4409 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/simple_rag_chain.py
--rw-r--r--   0        0        0     4006 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/standalone_question_chain.py
--rw-r--r--   0        0        0     4592 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_questions_chain.py
--rw-r--r--   0        0        0     4193 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_report_chain.py
--rw-r--r--   0        0        0     4832 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/tool_final_answer_chain.py
--rw-r--r--   0        0        0      567 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/__init__.py
--rw-r--r--   0        0        0      999 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/common.py
--rw-r--r--   0        0        0     3147 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/data_type_detection_chain.py
--rw-r--r--   0        0        0     3243 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_add_chain.py
--rw-r--r--   0        0        0     2963 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_parse_chain.py
--rw-r--r--   0        0        0     2464 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/timespan_parse_chain.py
--rw-r--r--   0        0        0     1515 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/config.py
--rw-r--r--   0        0        0      109 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0    13516 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0     2798 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/history.py
--rw-r--r--   0        0        0      797 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     4206 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/custom_react_json_single_input.py
--rw-r--r--   0        0        0     2091 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1075 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/key_finding.py
--rw-r--r--   0        0        0     1242 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/line_separated_list.py
--rw-r--r--   0        0        0     2816 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/sql_finding.py
--rw-r--r--   0        0        0      735 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/text_cleaning.py
--rw-r--r--   0        0        0     4502 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/timespan.py
--rw-r--r--   0        0        0      833 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/params.py
--rw-r--r--   0        0        0      122 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/py.typed
--rw-r--r--   0        0        0      165 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/__init__.py
--rw-r--r--   0        0        0     7894 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/fused_summary.py
--rw-r--r--   0        0        0     5472 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/mappings.py
--rw-r--r--   0        0        0      194 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/__init__.py
--rw-r--r--   0        0        0     3958 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/common.py
--rw-r--r--   0        0        0     8697 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/reports.py
--rw-r--r--   0        0        0     6830 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/retrieval.py
--rw-r--r--   0        0        0      708 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/utils/documents.py
--rw-r--r--   0        0        0     8975 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/utils/sql.py
--rw-r--r--   0        0        0     3389 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/utils/string_cleanup.py
--rw-r--r--   0        0        0     2829 2024-05-06 21:38:16.571129 docugami_langchain-0.0.9rc1/pyproject.toml
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/LICENSE
+-rw-r--r--   0        0        0      361 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/README.md
+-rw-r--r--   0        0        0      747 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/__init__.py
+-rw-r--r--   0        0        0     8459 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/base.py
+-rw-r--r--   0        0        0     1805 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/models.py
+-rw-r--r--   0        0        0    10928 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/re_act_agent.py
+-rw-r--r--   0        0        0     8325 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/agents/tool_router_agent.py
+-rw-r--r--   0        0        0    16628 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/base_runnable.py
+-rw-r--r--   0        0        0     1396 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/answer_chain.py
+-rw-r--r--   0        0        0     1415 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/base.py
+-rw-r--r--   0        0        0      243 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/__init__.py
+-rw-r--r--   0        0        0     3390 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
+-rw-r--r--   0        0        0     3980 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/summarize_chunk_chain.py
+-rw-r--r--   0        0        0      291 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/__init__.py
+-rw-r--r--   0        0        0     3838 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/describe_document_set_chain.py
+-rw-r--r--   0        0        0     3983 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/summarize_document_chain.py
+-rw-r--r--   0        0        0      647 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/__init__.py
+-rw-r--r--   0        0        0     3398 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
+-rw-r--r--   0        0        0      262 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/models.py
+-rw-r--r--   0        0        0     3999 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_fixup_chain.py
+-rw-r--r--   0        0        0     4360 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_query_explainer_chain.py
+-rw-r--r--   0        0        0     8808 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_chain.py
+-rw-r--r--   0        0        0     3522 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_explainer_chain.py
+-rw-r--r--   0        0        0      498 2024-05-06 23:27:14.808794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/models.py
+-rw-r--r--   0        0        0     4409 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/simple_rag_chain.py
+-rw-r--r--   0        0        0     4006 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/standalone_question_chain.py
+-rw-r--r--   0        0        0     4592 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_questions_chain.py
+-rw-r--r--   0        0        0     4193 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_report_chain.py
+-rw-r--r--   0        0        0     4832 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/tool_final_answer_chain.py
+-rw-r--r--   0        0        0      567 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/common.py
+-rw-r--r--   0        0        0     3147 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/data_type_detection_chain.py
+-rw-r--r--   0        0        0     3243 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_add_chain.py
+-rw-r--r--   0        0        0     2963 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_parse_chain.py
+-rw-r--r--   0        0        0     2464 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/timespan_parse_chain.py
+-rw-r--r--   0        0        0     1604 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/config.py
+-rw-r--r--   0        0        0      109 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13516 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     2798 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/history.py
+-rw-r--r--   0        0        0      797 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     4206 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/custom_react_json_single_input.py
+-rw-r--r--   0        0        0     2091 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1075 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/key_finding.py
+-rw-r--r--   0        0        0     1242 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/line_separated_list.py
+-rw-r--r--   0        0        0     2816 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/sql_finding.py
+-rw-r--r--   0        0        0      735 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/text_cleaning.py
+-rw-r--r--   0        0        0     4502 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/timespan.py
+-rw-r--r--   0        0        0      833 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/params.py
+-rw-r--r--   0        0        0      122 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/py.typed
+-rw-r--r--   0        0        0      165 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0     7894 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/fused_summary.py
+-rw-r--r--   0        0        0     5760 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/mappings.py
+-rw-r--r--   0        0        0      194 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/common.py
+-rw-r--r--   0        0        0     8697 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/reports.py
+-rw-r--r--   0        0        0     6830 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/tools/retrieval.py
+-rw-r--r--   0        0        0      708 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/utils/documents.py
+-rw-r--r--   0        0        0     8975 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/utils/sql.py
+-rw-r--r--   0        0        0     3389 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/docugami_langchain/utils/string_cleanup.py
+-rw-r--r--   0        0        0     2829 2024-05-06 23:27:14.812794 docugami_langchain-0.0.9rc2/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc2/PKG-INFO
```

### Comparing `docugami_langchain-0.0.9rc1/LICENSE` & `docugami_langchain-0.0.9rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/__init__.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/agents/base.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/agents/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/agents/models.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/agents/models.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/agents/re_act_agent.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/agents/re_act_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/agents/tool_router_agent.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/agents/tool_router_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/base_runnable.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/base_runnable.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/__init__.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/answer_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/base.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/elaborate_chunk_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/elaborate_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/summarize_chunk_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/chunks/summarize_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/describe_document_set_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/describe_document_set_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/summarize_document_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/documents/summarize_document_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/__init__.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_fixup_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_fixup_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_query_explainer_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_query_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_explainer_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/querying/sql_result_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/simple_rag_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/simple_rag_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/standalone_question_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/standalone_question_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_questions_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_questions_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_report_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/suggested_report_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/tool_final_answer_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/rag/tool_final_answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/__init__.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/common.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/data_type_detection_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/data_type_detection_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_add_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_add_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_parse_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/date_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/timespan_parse_chain.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/chains/types/timespan_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/config.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 ________SINGLE_TOKEN_LINE________ = "----------------"
 
-# ************ PARAMETERS TO CONTROL PROMPT SIZES
+# ************ PARAMETERS TO CONTROL PROMPTS
 
 # Lengths are in terms of characters, 1 token ~= 4 chars in English
 # Reference: https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them
 
 # Chunks and docs below this length are not summarized by default
 MIN_LENGTH_TO_SUMMARIZE: int = 2048
 
+# Change this to improve parallelization, or work around late limiting issues
+BATCH_SIZE = 8
+
 # When summarizing full docs we cut off input after this by default
 MAX_FULL_DOCUMENT_TEXT_LENGTH: int = int(1024 * 4 * 8)  # ~8k tokens,
 
 # When summarizing chunks we cut off input after this by default
 MAX_CHUNK_TEXT_LENGTH: int = int(1024 * 4 * 4.5)  # ~4.5k tokens
 MAX_PARAMS_CUTOFF_LENGTH_CHARS: int = int(1024 * 4 * 2)  # ~2k tokens
 DEFAULT_EXAMPLES_PER_PROMPT = 3
```

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/document_loaders/docugami.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/history.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/history.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/__init__.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/custom_react_json_single_input.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/custom_react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/datetime.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/key_finding.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/key_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/line_separated_list.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/line_separated_list.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/sql_finding.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/sql_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/text_cleaning.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/timespan.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/output_parsers/timespan.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/params.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/params.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/fused_summary.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/fused_summary.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/mappings.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/retrievers/mappings.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
 
 from docugami_langchain.chains import SummarizeChunkChain, SummarizeDocumentChain
 from docugami_langchain.config import (
+    BATCH_SIZE,
     INCLUDE_XML_TAGS,
     MAX_CHUNK_TEXT_LENGTH,
     MAX_FULL_DOCUMENT_TEXT_LENGTH,
     MIN_LENGTH_TO_SUMMARIZE,
 )
 from docugami_langchain.retrievers.fused_summary import (
     FULL_DOC_SUMMARY_ID_KEY,
@@ -20,39 +21,45 @@
 )
 
 
 def _build_summary_mappings(
     docs_by_id: dict[str, Document],
     chain: Union[SummarizeChunkChain, SummarizeDocumentChain],
     include_xml_tags: bool,
+    batch_size: int = BATCH_SIZE,
 ) -> dict[str, Document]:
     """
-    Build summaries for all the given documents.
+    Build summaries for all the given documents in batches of a specified size.
     """
     summaries: dict[str, Document] = {}
     format: str = (
         "text"
         if not include_xml_tags
         else "semantic XML without any namespaces or attributes"
     )
 
-    batch_input = [(doc.page_content, format) for _, doc in docs_by_id.items()]
-    batch_summaries = chain.run_batch(batch_input)  # type: ignore
-
-    # Assigning summaries to the respective document IDs
-    for (id, doc), summary in zip(docs_by_id.items(), batch_summaries):
-        summary_id = hashlib.md5(summary.encode()).hexdigest()
-        meta = doc.metadata
-        meta["id"] = summary_id
-        meta[PARENT_DOC_ID_KEY] = id
-
-        summaries[id] = Document(
-            page_content=summary,
-            metadata=meta,
-        )
+    # Create batches of input tuples
+    items = list(docs_by_id.items())
+    batches = [items[i : i + batch_size] for i in range(0, len(items), batch_size)]
+
+    for batch in batches:
+        batch_input = [(doc.page_content, format) for _, doc in batch]
+        batch_summaries = chain.run_batch(batch_input)  # type: ignore
+
+        # Assigning summaries to the respective document IDs
+        for (id, doc), summary in zip(batch, batch_summaries):
+            summary_id = hashlib.md5(summary.encode()).hexdigest()
+            meta = doc.metadata
+            meta["id"] = summary_id
+            meta[PARENT_DOC_ID_KEY] = id
+
+            summaries[id] = Document(
+                page_content=summary,
+                metadata=meta,
+            )
 
     return summaries
 
 
 def build_full_doc_summary_mappings(
     docs_by_id: dict[str, Document],
     llm: BaseLanguageModel,
```

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/tools/common.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/tools/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/tools/reports.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/tools/reports.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/tools/retrieval.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/utils/documents.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/utils/documents.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/utils/sql.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/utils/sql.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/docugami_langchain/utils/string_cleanup.py` & `docugami_langchain-0.0.9rc2/docugami_langchain/utils/string_cleanup.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc1/pyproject.toml` & `docugami_langchain-0.0.9rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docugami-langchain"
-version = "0.0.9rc1"
+version = "0.0.9rc2"
 description = "An integration package connecting Docugami and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/docugami/docugami-langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `docugami_langchain-0.0.9rc1/PKG-INFO` & `docugami_langchain-0.0.9rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugami-langchain
-Version: 0.0.9rc1
+Version: 0.0.9rc2
 Summary: An integration package connecting Docugami and LangChain
 Home-page: https://github.com/docugami/docugami-langchain
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

