# Comparing `tmp/blackboxai-2.6.tar.gz` & `tmp/blackboxai-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxai-2.6.tar", last modified: Wed Apr  3 19:17:52 2024, max compression
+gzip compressed data, was "blackboxai-2.7.tar", last modified: Tue May  7 12:14:57 2024, max compression
```

## Comparing `blackboxai-2.6.tar` & `blackboxai-2.7.tar`

### file list

```diff
@@ -1,137 +1,160 @@
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.920207 blackboxai-2.6/
--rw-r--r--   0 rizkrichard   (501) staff       (20)    33813 2024-04-03 18:37:22.000000 blackboxai-2.6/LICENSE
--rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-04-03 19:17:52.920036 blackboxai-2.6/PKG-INFO
--rw-r--r--   0 rizkrichard   (501) staff       (20)      635 2024-04-03 18:37:22.000000 blackboxai-2.6/README.md
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.896251 blackboxai-2.6/blackboxai/
--rw-r--r--   0 rizkrichard   (501) staff       (20)       25 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1725 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/chat.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.896529 blackboxai-2.6/blackboxai/interpreter/
--rw-r--r--   0 rizkrichard   (501) staff       (20)      601 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.898255 blackboxai-2.6/blackboxai/interpreter/core/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2820 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.899172 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1293 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3138 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.899372 blackboxai-2.6/blackboxai/interpreter/core/computer/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.899800 blackboxai-2.6/blackboxai/interpreter/core/computer/ai/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/ai/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     5688 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/ai/ai.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.900157 blackboxai-2.6/blackboxai/interpreter/core/computer/browser/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/browser/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      399 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/browser/browser.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.900515 blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      879 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/clipboard.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2526 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/computer.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.900878 blackboxai-2.6/blackboxai/interpreter/core/computer/display/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/display/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     9531 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/display/display.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.901254 blackboxai-2.6/blackboxai/interpreter/core/computer/docs/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/docs/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      749 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/docs/docs.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.901624 blackboxai-2.6/blackboxai/interpreter/core/computer/files/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/files/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1698 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/files/files.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.902005 blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3553 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/keyboard.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.902248 blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    12449 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/mouse.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.902680 blackboxai-2.6/blackboxai/interpreter/core/computer/os/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/os/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2961 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/os/os.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.903101 blackboxai-2.6/blackboxai/interpreter/core/computer/skills/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/skills/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3586 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/skills/skills.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.903631 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1090 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/base_language.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.906907 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     5164 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1812 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      858 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/html.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1924 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    15293 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2193 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      293 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/python.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2360 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/r.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2500 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/react.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2727 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/shell.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     6715 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     4946 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/terminal.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.907969 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     7043 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/computer_vision.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1479 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/get_active_window.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      929 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      396 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/recipient_utils.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    13458 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/core.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1647 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/default_system_message.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.908939 blackboxai-2.6/blackboxai/interpreter/core/llm/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     8998 2024-04-03 19:17:36.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/llm.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     5120 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/run_function_calling_llm.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2616 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/run_text_llm.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.909867 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     7838 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      711 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/merge_deltas.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1800 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      538 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/vision_for_text_llms.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1288 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/render_message.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    14088 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/respond.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     6162 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/server.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.912296 blackboxai-2.6/blackboxai/interpreter/core/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)      630 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      360 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1096 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      920 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/lazy_import.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2118 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/scan_code.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     4415 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/system_debug_info.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1736 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/telemetry.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1098 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/temporary_file.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      510 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/truncate_output.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.914719 blackboxai-2.6/blackboxai/interpreter/terminal_interface/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2433 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.915480 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      611 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/base_block.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2664 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/code_block.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1386 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/message_block.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2905 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/conversation_navigator.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    10586 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/magic_commands.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2304 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/render_past_conversation.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    14679 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    20298 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/terminal_interface.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.919063 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)    25835 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3099 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      512 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      481 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      419 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/cli_input.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1939 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      884 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3069 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_output.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      459 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      250 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      184 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      316 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)       79 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2899 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.919821 blackboxai-2.6/blackboxai.egg-info/
--rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/PKG-INFO
--rw-r--r--   0 rizkrichard   (501) staff       (20)     6297 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/SOURCES.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)        1 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/dependency_links.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)       50 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/entry_points.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)       11 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/top_level.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1959 2024-04-03 18:37:22.000000 blackboxai-2.6/pyproject.toml
--rw-r--r--   0 rizkrichard   (501) staff       (20)       38 2024-04-03 19:17:52.920254 blackboxai-2.6/setup.cfg
--rw-r--r--   0 rizkrichard   (501) staff       (20)      523 2024-04-03 19:12:05.000000 blackboxai-2.6/setup.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.909585 blackboxai-2.7/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    33813 2024-05-06 17:45:40.000000 blackboxai-2.7/LICENSE
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-05-07 12:14:57.909433 blackboxai-2.7/PKG-INFO
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      635 2024-05-07 02:15:32.000000 blackboxai-2.7/README.md
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.859877 blackboxai-2.7/blackboxai/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       25 2024-05-06 17:45:40.000000 blackboxai-2.7/blackboxai/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2698 2024-05-07 05:35:21.000000 blackboxai-2.7/blackboxai/chat.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.860093 blackboxai-2.7/blackboxai/interpreter/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      652 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/__init__.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.862075 blackboxai-2.7/blackboxai/interpreter/core/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2820 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.862848 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1293 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3138 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3046 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/browser.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.863040 blackboxai-2.7/blackboxai/interpreter/core/computer/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/__init__.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.863445 blackboxai-2.7/blackboxai/interpreter/core/computer/ai/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/ai/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     5688 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/ai/ai.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.863959 blackboxai-2.7/blackboxai/interpreter/core/computer/browser/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/browser/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      416 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/browser/browser.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.864343 blackboxai-2.7/blackboxai/interpreter/core/computer/calendar/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/calendar/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    12950 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/calendar/calendar.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.864722 blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      879 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/clipboard.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2831 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/computer.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.866070 blackboxai-2.7/blackboxai/interpreter/core/computer/contacts/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/contacts/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3293 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/contacts/contacts.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.866640 blackboxai-2.7/blackboxai/interpreter/core/computer/display/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/display/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    10556 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/display/display.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.867047 blackboxai-2.7/blackboxai/interpreter/core/computer/docs/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/docs/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      749 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/docs/docs.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.867370 blackboxai-2.7/blackboxai/interpreter/core/computer/files/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/files/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1698 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/files/files.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.867731 blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3553 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/keyboard.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.868058 blackboxai-2.7/blackboxai/interpreter/core/computer/mail/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mail/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     6350 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mail/mail.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.869945 blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    12423 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/mouse.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.871286 blackboxai-2.7/blackboxai/interpreter/core/computer/os/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/os/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2961 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/os/os.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.871717 blackboxai-2.7/blackboxai/interpreter/core/computer/skills/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:30:00.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/skills/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     4535 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/skills/skills.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.873998 blackboxai-2.7/blackboxai/interpreter/core/computer/sms/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/sms/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1399 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/sms/sms.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.874875 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1090 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/base_language.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.881783 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     5164 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1812 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      858 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/html.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1924 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    15293 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2193 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      293 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/python.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2360 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/r.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2503 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/react.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2727 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/shell.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     6715 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     4946 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/terminal.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.883353 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:29:48.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     7097 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/computer_vision.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1479 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/get_active_window.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      929 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      396 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/recipient_utils.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      586 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/run_applescript.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    14529 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/core.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3288 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/core/default_system_message.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.886727 blackboxai-2.7/blackboxai/interpreter/core/llm/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     7323 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/agent_llm.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     9084 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/llm.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     5052 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/run_function_calling_llm.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3899 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/run_text_llm.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.891542 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:30:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    11769 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      711 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/merge_deltas.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1800 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      538 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/vision_for_text_llms.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1688 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/render_message.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    14523 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/respond.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      690 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/search.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     6162 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/server.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.899712 blackboxai-2.7/blackboxai/interpreter/core/utils/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      630 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      360 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1096 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      920 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/lazy_import.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2118 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/scan_code.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     4404 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/system_debug_info.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1736 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/telemetry.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1098 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/temporary_file.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      510 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/truncate_output.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.902435 blackboxai-2.7/blackboxai/interpreter/terminal_interface/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2433 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/__init__.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.903230 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:28:24.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      611 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/base_block.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2664 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/code_block.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1386 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/message_block.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2905 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/conversation_navigator.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    10586 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/magic_commands.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.903773 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:28:36.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)       25 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    40533 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/profiles.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2304 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/render_past_conversation.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    14917 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    27491 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/terminal_interface.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.908099 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)    25835 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3099 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:27:08.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/__init__.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     4954 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/agent_utils.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      512 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      481 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      419 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/cli_input.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     1939 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      884 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     3069 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_output.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      459 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      250 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      184 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)      316 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)       79 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
+-rw-rw-r--   0 rizkrichard   (501) staff       (20)     2887 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.908825 blackboxai-2.7/blackboxai.egg-info/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/PKG-INFO
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     7239 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/SOURCES.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        1 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/dependency_links.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       50 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/entry_points.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       11 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/top_level.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1959 2024-05-07 02:17:56.000000 blackboxai-2.7/pyproject.toml
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       38 2024-05-07 12:14:57.909631 blackboxai-2.7/setup.cfg
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      523 2024-05-07 03:00:25.000000 blackboxai-2.7/setup.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.908937 blackboxai-2.7/tests/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    21812 2024-05-07 02:17:56.000000 blackboxai-2.7/tests/test_interpreter.py
```

### Comparing `blackboxai-2.6/LICENSE` & `blackboxai-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/PKG-INFO` & `blackboxai-2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 2.6
+Version: 2.7
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
```

### Comparing `blackboxai-2.6/README.md` & `blackboxai-2.7/README.md`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py` & `blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py` & `blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py` & `blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/ai/ai.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/ai/ai.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/clipboard.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/computer.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/computer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 import json
 
 from .ai.ai import Ai
 from .browser.browser import Browser
+from .calendar.calendar import Calendar
 from .clipboard.clipboard import Clipboard
+from .contacts.contacts import Contacts
 from .display.display import Display
 from .docs.docs import Docs
 from .keyboard.keyboard import Keyboard
+from .mail.mail import Mail
 from .mouse.mouse import Mouse
 from .os.os import Os
 from .skills.skills import Skills
+from .sms.sms import SMS
 from .terminal.terminal import Terminal
 
 
 class Computer:
-    def __init__(self):
+    def __init__(self, interpreter):
+        self.interpreter = interpreter
+
         self.terminal = Terminal(self)
 
         self.offline = False
         self.verbose = False
+        self.debug = False
 
         self.mouse = Mouse(self)
         self.keyboard = Keyboard(self)
         self.display = Display(self)
         self.clipboard = Clipboard(self)
+        self.mail = Mail(self)
+        self.sms = SMS(self)
+        self.calendar = Calendar(self)
+        self.contacts = Contacts(self)
         self.browser = Browser(self)
         self.os = Os(self)
         self.skills = Skills(self)
         self.docs = Docs(self)
         self.ai = Ai(self)
 
         self.emit_images = True
         self.api_base = "https://api.openinterpreter.com/v0"
         self.save_skills = True
-        # self.api_base = "http://0.0.0.0/v0"
 
         self.import_computer_api = True
         self._has_imported_computer_api = False  # Because we only want to do this once
 
     # Shortcut for computer.terminal.languages
     @property
     def languages(self):
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/display/display.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/display/display.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import os
+import platform
 import pprint
 import time
 import warnings
 from contextlib import redirect_stdout
 from io import BytesIO
 
 import requests
@@ -24,14 +25,15 @@
 
 class Display:
     def __init__(self, computer):
         self.computer = computer
         # set width and height to None initially to prevent pyautogui from importing until it's needed
         self._width = None
         self._height = None
+        self._hashes = {}
 
     # We use properties here so that this code only executes when height/width are accessed for the first time
     @property
     def width(self):
         if self._width is None:
             self._width, _ = pyautogui.size()
         return self._width
@@ -59,20 +61,21 @@
         Redirects to self.screenshot
         """
         return self.screenshot(show, quadrant)
 
     # def get_active_window(self):
     #     return get_active_window()
 
-    def screenshot(self, show=True, quadrant=None, active_app_only=False):
+    def screenshot(
+        self, show=True, quadrant=None, active_app_only=False, force_image=False
+    ):
         """
         Shows you what's on the screen by taking a screenshot of the entire screen or a specified quadrant. Returns a `pil_image` `in case you need it (rarely). **You almost always want to do this first!**
         """
-        time.sleep(2)
-        if not self.computer.emit_images:
+        if not self.computer.emit_images and force_image == False:
             text = self.get_text_as_list_of_lists()
             pp = pprint.PrettyPrinter(indent=4)
             pretty_text = pp.pformat(text)  # language models like it pretty!
             pretty_text = format_to_recipient(pretty_text, "assistant")
             print(pretty_text)
             print(
                 format_to_recipient(
@@ -84,15 +87,18 @@
 
         if quadrant == None:
             # Implement active_app_only!
             if active_app_only:
                 region = self.get_active_window()["region"]
                 screenshot = pyautogui.screenshot(region=region)
             else:
-                screenshot = pyautogui.screenshot()
+                if platform.system() == "Darwin":
+                    screenshot = take_screenshot_to_pil()
+                else:
+                    screenshot = pyautogui.screenshot()
                 # message = format_to_recipient("Taking a screenshot of the entire screen. This is not recommended. You (the language model assistant) will recieve it with low resolution.\n\nTo maximize performance, use computer.display.view(active_app_only=True). This will produce an ultra high quality image of the active application.", "assistant")
                 # print(message)
 
         else:
             screen_width, screen_height = pyautogui.size()
 
             quadrant_width = screen_width // 2
@@ -129,46 +135,57 @@
         return screenshot
 
     def find(self, description, screenshot=None):
         if description.startswith('"') and description.endswith('"'):
             return self.find_text(description.strip('"'), screenshot)
         else:
             try:
-                message = format_to_recipient(
-                    "Locating this icon will take ~10 seconds. Subsequent icons should be found more quickly.",
-                    recipient="user",
-                )
-                print(message)
+                if self.computer.debug:
+                    print("DEBUG MODE ON")
+                    print("NUM HASHES:", len(self._hashes))
+                else:
+                    message = format_to_recipient(
+                        "Locating this icon will take ~15 seconds. Subsequent icons should be found more quickly.",
+                        recipient="user",
+                    )
+                    print(message)
+
+                if len(self._hashes) > 5000:
+                    self._hashes = dict(list(self._hashes.items())[-5000:])
+
                 from .point.point import point
 
-                with open(os.devnull, "w") as f, redirect_stdout(f):
-                    result = point(description, screenshot)
+                result = point(
+                    description, screenshot, self.computer.debug, self._hashes
+                )
+
                 return result
             except:
+                if self.computer.debug:
+                    # We want to know these bugs lmao
+                    raise
                 if self.computer.offline:
                     raise
                 message = format_to_recipient(
                     "Locating this icon will take ~30 seconds. We're working on speeding this up.",
                     recipient="user",
                 )
                 print(message)
 
-                start = time.time()
                 # Take a screenshot
                 if screenshot == None:
                     screenshot = self.screenshot(show=False)
 
                 # Downscale the screenshot to 1920x1080
                 screenshot = screenshot.resize((1920, 1080))
 
                 # Convert the screenshot to base64
                 buffered = BytesIO()
                 screenshot.save(buffered, format="PNG")
                 screenshot_base64 = base64.b64encode(buffered.getvalue()).decode()
-                print("PIC TOOK THIS LONG:", time.time() - start)
 
                 try:
                     response = requests.post(
                         f'{self.computer.api_base.strip("/")}/point/',
                         json={"query": description, "base64": screenshot_base64},
                     )
                     return response.json()
@@ -200,26 +217,26 @@
                 return response
             except:
                 print("Attempting to find the text locally.")
 
         # We'll only get here if 1) self.computer.offline = True, or the API failed
 
         # Find the text in the screenshot
-        centers = find_text_in_image(screenshot, text)
+        centers = find_text_in_image(screenshot, text, self.computer.debug)
 
         return [
             {"coordinates": center, "text": "", "similarity": 1} for center in centers
         ]  # Have it deliver the text properly soon.
 
     def get_text_as_list_of_lists(self, screenshot=None):
         """
         Extracts and returns text from a screenshot or the current screen as a list of lists, each representing a line of text.
         """
         if screenshot == None:
-            screenshot = self.screenshot(show=False)
+            screenshot = self.screenshot(show=False, force_image=True)
 
         if not self.computer.offline:
             # Convert the screenshot to base64
             buffered = BytesIO()
             screenshot.save(buffered, format="PNG")
             screenshot_base64 = base64.b64encode(buffered.getvalue()).decode()
 
@@ -231,14 +248,34 @@
                 response = response.json()
                 return response
             except:
                 print("Attempting to get the text locally.")
 
         # We'll only get here if 1) self.computer.offline = True, or the API failed
 
-        if self.computer.offline == True:
-            try:
-                return pytesseract_get_text(screenshot)
-            except:
-                raise Exception(
-                    "Failed to find text locally.\n\nTo find text in order to use the mouse, please make sure you've installed `pytesseract` along with the Tesseract executable (see this Stack Overflow answer for help installing Tesseract: https://stackoverflow.com/questions/50951955/pytesseract-tesseractnotfound-error-tesseract-is-not-installed-or-its-not-i)."
-                )
+        try:
+            return pytesseract_get_text(screenshot)
+        except:
+            raise Exception(
+                "Failed to find text locally.\n\nTo find text in order to use the mouse, please make sure you've installed `pytesseract` along with the Tesseract executable (see this Stack Overflow answer for help installing Tesseract: https://stackoverflow.com/questions/50951955/pytesseract-tesseractnotfound-error-tesseract-is-not-installed-or-its-not-i)."
+            )
+
+
+import io
+import subprocess
+
+from PIL import Image
+
+
+def take_screenshot_to_pil(filename="temp_screenshot.png"):
+    # Capture the screenshot and save it to a temporary file
+    subprocess.run(["screencapture", "-x", filename], check=True)
+
+    # Open the image file with PIL
+    with open(filename, "rb") as f:
+        image_data = f.read()
+    image = Image.open(io.BytesIO(image_data))
+
+    # Optionally, delete the temporary file if you don't need it after loading
+    os.remove(filename)
+
+    return image
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/docs/docs.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/docs/docs.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/files/files.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/files/files.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/keyboard.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/mouse.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/mouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
                 f"An error occurred while retrieving the mouse position: {e}. "
             )
 
     def move(self, *args, x=None, y=None, icon=None, text=None, screenshot=None):
         """
         Moves the mouse to specified coordinates, an icon, or text.
         """
-        screenshot = None
         if len(args) > 1:
             raise ValueError(
                 "Too many positional arguments provided. To move/click specific coordinates, use kwargs (x=x, y=y).\n\nPlease take a screenshot with computer.display.view() to find text/icons to click, then use computer.mouse.click(text) or computer.mouse.click(icon=description_of_icon) if at all possible. This is **significantly** more accurate than using coordinates. Specifying (x=x, y=y) is highly likely to fail. Specifying ('text to click') is highly likely to succeed."
             )
         elif len(args) == 1 or text != None:
             if len(args) == 1:
                 text = args[0]
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/os/os.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/os/os.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/base_language.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/base_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/applescript.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/html.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/html.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/javascript.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/powershell.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/r.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/r.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/react.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/react.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 
     return False
 
 
 class React(BaseLanguage):
     name = "React"
     file_extension = "html"
-    system_message = "When you execute code with `react`, your react code will be run in a script tag after being inserted into the HTML template, following the installation of React, ReactDOM, and Babel for JSX parsing. **We will handle this! Don't make an HTML file to run React, just execute `react`.**"
+
+    # system_message = "When you execute code with `react`, your react code will be run in a script tag after being inserted into the HTML template, following the installation of React, ReactDOM, and Babel for JSX parsing. **We will handle this! Don't make an HTML file to run React, just execute `react`.**"
 
     def run(self, code):
         if is_incompatible(code):
             yield {
                 "type": "console",
                 "format": "output",
                 "content": f"Error: React format not supported. {self.system_message} Therefore some things like `require` and 'import' aren't supported.",
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/shell.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/shell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/terminal.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/utils/computer_vision.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/utils/computer_vision.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         }
         # Append this box dictionary to the list
         boxes.append(box)
 
     return boxes
 
 
-def find_text_in_image(img, text):
+def find_text_in_image(img, text, debug=False):
     # Convert PIL Image to NumPy array
     img_array = np.array(img)
 
     # Convert the image to grayscale
     gray = cv2.cvtColor(img_array, cv2.COLOR_BGR2GRAY)
 
     # Use pytesseract to get the data from the image
@@ -74,35 +74,38 @@
     # Convert the img_draw grayscale image to RGB
     img_draw = cv2.cvtColor(img_draw, cv2.COLOR_GRAY2RGB)
 
     id = 0
 
     # Loop through each box
     for i in range(n_boxes):
-        # # (DEBUGGING) Draw each box on the grayscale image
-        # cv2.rectangle(
-        #     img_draw,
-        #     (d["left"][i], d["top"][i]),
-        #     (d["left"][i] + d["width"][i], d["top"][i] + d["height"][i]),
-        #     (0, 255, 0),
-        #     2,
-        # )
-        # # Draw the detected text in the rectangle in small font
-        # font = cv2.FONT_HERSHEY_SIMPLEX
-        # font_scale = 0.5
-        # font_color = (0, 0, 255)
-        # line_type = 2
-
-        # cv2.putText(img_draw,
-        #             d["text"][i],
-        #             (d["left"][i], d["top"][i] - 10),
-        #             font,
-        #             font_scale,
-        #             font_color,
-        #             line_type)
+        if debug:
+            # (DEBUGGING) Draw each box on the grayscale image
+            cv2.rectangle(
+                img_draw,
+                (d["left"][i], d["top"][i]),
+                (d["left"][i] + d["width"][i], d["top"][i] + d["height"][i]),
+                (0, 255, 0),
+                2,
+            )
+            # Draw the detected text in the rectangle in small font
+            font = cv2.FONT_HERSHEY_SIMPLEX
+            font_scale = 0.5
+            font_color = (0, 0, 255)
+            line_type = 2
+
+            cv2.putText(
+                img_draw,
+                d["text"][i],
+                (d["left"][i], d["top"][i] - 10),
+                font,
+                font_scale,
+                font_color,
+                line_type,
+            )
 
         # Print the text of the box
         # If the text in the box matches the given text
         if text.lower() in d["text"][i].lower():
             # Find the start index of the matching text in the box
             start_index = d["text"][i].lower().find(text.lower())
             # Calculate the percentage of the box width that the start of the matching text represents
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/utils/get_active_window.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/utils/get_active_window.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py` & `blackboxai-2.7/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/core.py` & `blackboxai-2.7/blackboxai/interpreter/core/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..terminal_interface.terminal_interface import terminal_interface
 from ..terminal_interface.utils.display_markdown_message import display_markdown_message
 from ..terminal_interface.utils.local_storage_path import get_storage_path
 from ..terminal_interface.utils.oi_dir import oi_dir
 from .computer.computer import Computer
 from .default_system_message import default_system_message
 from .llm.llm import Llm
+from .llm.agent_llm import AgentLlm
 from .respond import respond
 from .server import server
 from .utils.telemetry import send_telemetry
 from .utils.truncate_output import truncate_output
 
 
 class OpenInterpreter:
@@ -41,27 +42,35 @@
 
     def __init__(
         self,
         messages=None,
         offline=False,
         auto_run=False,
         verbose=False,
+        debug=False,
         max_output=2800,
         safe_mode="off",
         shrink_images=False,
-        force_task_completion=False,
+        loop=False,
+        loop_message="""Proceed. You CAN run code on my machine. If you want to run code, start your message with "```"! If the entire task I asked for is done, say exactly 'The task is done.' If you need some specific information (like username or password) say EXACTLY 'Please provide more information.' If it's impossible, say 'The task is impossible.' (If I haven't provided a task, say exactly 'Let me know what you'd like to do next.') Otherwise keep going.""",
+        loop_breakers=[
+            "the task is done.",
+            "the task is impossible.",
+            "let me know what you'd like to do next.",
+            "please provide more information.",
+        ],
         anonymous_telemetry=os.getenv("ANONYMIZED_TELEMETRY", "True") == "True",
         in_terminal_interface=False,
         conversation_history=True,
         conversation_filename=None,
         conversation_history_path=get_storage_path("conversations"),
         os=False,
         speak_messages=False,
         llm=None,
-        system_message=default_system_message,
+        system_message="",
         custom_instructions="",
         computer=None,
         sync_computer=True,
         import_computer_api=True,
         skills_path=None,
         import_skills=True,
         multi_line=False,
@@ -71,50 +80,63 @@
         self.responding = False
         self.last_messages_count = 0
 
         # Settings
         self.offline = offline
         self.auto_run = auto_run
         self.verbose = verbose
+        self.debug = debug
         self.max_output = max_output
         self.safe_mode = safe_mode
         self.shrink_images = shrink_images
-        self.force_task_completion = force_task_completion
         self.anonymous_telemetry = anonymous_telemetry
         self.in_terminal_interface = in_terminal_interface
         self.multi_line = multi_line
 
+        # Loop messages
+        self.loop = loop
+        self.loop_message = loop_message
+        self.loop_breakers = loop_breakers
+
         # Conversation history
         self.conversation_history = conversation_history
         self.conversation_filename = conversation_filename
         self.conversation_history_path = conversation_history_path
 
         # OS control mode related attributes
         self.os = os
         self.speak_messages = speak_messages
 
         # LLM
         self.llm = Llm(self) if llm is None else llm
+        self.planner_llm = AgentLlm()
+        self.router_llm = AgentLlm()
+        self.summarizer_llm = AgentLlm()
+        self.serper_endpoint = None
+
 
         # These are LLM related
         self.system_message = system_message
         self.custom_instructions = custom_instructions
+        self.append_decline_message = True
 
         # Computer
-        self.computer = Computer() if computer is None else computer
+        self.computer = Computer(self) if computer is None else computer
 
         self.sync_computer = sync_computer
         self.computer.import_computer_api = import_computer_api
 
         # Skills
         if skills_path:
             self.computer.skills.path = skills_path
 
         self.import_skills = import_skills
         if import_skills:
+            if self.verbose:
+                print("Importing skills")
             self.computer.skills.import_skills()
 
     def server(self, *args, **kwargs):
         server(self, *args, **kwargs)
 
     def wait(self):
         while self.responding:
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/llm/llm.py` & `blackboxai-2.7/blackboxai/interpreter/core/llm/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,16 @@
     display_markdown_message,
 )
 from .run_function_calling_llm import run_function_calling_llm
 from .run_text_llm import run_text_llm
 from .utils.convert_to_openai_messages import convert_to_openai_messages
 
 litellm.suppress_debug_info = True
-import requests
-import json
+import time
 
-def selectionFct(event):
-    try:
-        url = "https://www.useblackbox.io/selection"
-
-        payload = json.dumps({
-            "selected": event,
-            "source": "terminal"
-        })
-        headers = {
-            'Content-Type': 'application/json'
-        }
-
-        response = requests.request("POST", url, headers=headers, data=payload)
-    except Exception as e:
-        print(f"An error occurred: {e}")
 
 class Llm:
     """
     A stateless LMC-style LLM with some helpful properties.
     """
 
     def __init__(self, interpreter):
@@ -48,14 +32,18 @@
 
         # Optional settings
         self.context_window = None
         self.max_tokens = None
         self.api_base = None
         self.api_key = None
         self.api_version = None
+        self.top_p = None
+        self.user_request_prompt = ""
+        self.code_output_sender = "assistant"
+        self.stop=[]
 
         # Budget manager powered by LiteLLM
         self.max_budget = None
 
     def run(self, messages):
         """
         We're responsible for formatting the call into the llm.completions object,
@@ -90,17 +78,17 @@
                 supports_functions = False
 
         # Trim image messages if they're there
         if self.supports_vision:
             image_messages = [msg for msg in messages if msg["type"] == "image"]
 
             if self.interpreter.os:
-                # Keep only the last image if the interpreter is running in OS mode
+                # Keep only the last two images if the interpreter is running in OS mode
                 if len(image_messages) > 1:
-                    for img_msg in image_messages[:-1]:
+                    for img_msg in image_messages[:-2]:
                         messages.remove(img_msg)
                         if self.interpreter.verbose:
                             print("Removing image message!")
             else:
                 # Delete all the middle ones (leave only the first and last 2 images) from messages_for_llm
                 if len(image_messages) > 3:
                     for img_msg in image_messages[1:-2]:
@@ -111,16 +99,27 @@
 
         # Convert to OpenAI messages format
         messages = convert_to_openai_messages(
             messages,
             function_calling=supports_functions,
             vision=self.supports_vision,
             shrink_images=self.interpreter.shrink_images,
+            code_output_sender=self.code_output_sender
         )
 
+        if self.interpreter.debug:
+            print("\n\n\nOPENAI COMPATIBLE MESSAGES\n\n\n")
+            for message in messages:
+                if len(str(message)) > 5000:
+                    print(str(message)[:200] + "...")
+                else:
+                    print(message)
+                print("\n")
+            print("\n\n\n")
+
         system_message = messages[0]["content"]
         messages = messages[1:]
 
         # Trim messages
         try:
             if self.context_window and self.max_tokens:
                 trim_to_be_this_many_tokens = (
@@ -192,38 +191,35 @@
         if self.api_key:
             params["api_key"] = self.api_key
         if self.api_base:
             params["api_base"] = self.api_base
             params["custom_llm_provider"] = "openai"
         if self.api_version:
             params["api_version"] = self.api_version
-        if self.max_tokens:
+        if self.max_tokens is not None:
             params["max_tokens"] = self.max_tokens
-        if self.temperature:
+        if self.temperature is not None:
             params["temperature"] = self.temperature
+        if self.top_p is not None:
+            params["top_p"] = self.top_p
+        if len(self.stop) > 0:
+            params["stop"] = self.stop
 
         # Set some params directly on LiteLLM
         if self.max_budget:
             litellm.max_budget = self.max_budget
         if self.interpreter.verbose:
             litellm.set_verbose = True
 
-        # print("=====>")
-        # print(params)
-        # exit()
-        selectionFct('Chat Request')
         if supports_functions:
-            # print("--------------->")
             yield from run_function_calling_llm(self, params)
         else:
-            # print("---===========>")
             yield from run_text_llm(self, params)
 
 
-
 def fixed_litellm_completions(**params):
     """
     Just uses a dummy API key, since we use litellm without an API key sometimes.
     Hopefully they will fix this!
     """
 
     # Run completion
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/llm/run_function_calling_llm.py` & `blackboxai-2.7/blackboxai/interpreter/core/llm/run_function_calling_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,12 +116,13 @@
                             "format": language,
                             "content": code_delta,
                         }
 
             else:
                 # If name exists and it's not "execute" or "python" or "functions", who knows what's going on.
                 if "name" in accumulated_deltas["function_call"]:
-                    print(
-                        "Encountered an unexpected function call: ",
-                        accumulated_deltas["function_call"],
-                        "\nPlease open an issue and provide the above info at: https://github.com/KillianLucas/open-interpreter",
-                    )
+                    yield {
+                        "type": "code",
+                        "format": "python",
+                        "content": accumulated_deltas["function_call"]["name"],
+                    }
+                    return
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/llm/run_text_llm.py` & `blackboxai-2.7/blackboxai/interpreter/core/llm/run_text_llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+import re
+
+FILE_PATH_REGEX = '''<execute>\\n*File:\s*['"](.*)["']\s*:'''
+
+def is_file_present(text):
+    file_creation_path = None
+    matches = re.findall(FILE_PATH_REGEX,text,re.MULTILINE)
+    if len(matches)>0:
+        file_creation_path = matches[0]
+    return file_creation_path
+
+
 def run_text_llm(llm, params):
     ## Setup
 
     try:
         # Add the system message
         params["messages"][0][
             "content"
@@ -10,15 +22,17 @@
         print('params["messages"][0]', params["messages"][0])
         raise
 
     ## Convert output to LMC format
 
     inside_code_block = False
     accumulated_block = ""
+    full_message = ""
     language = None
+    file_creation_path = None
 
     for chunk in llm.completions(**params):
         if llm.interpreter.verbose:
             print("Chunk in coding_llm", chunk)
 
         if "choices" not in chunk or len(chunk["choices"]) == 0:
             # This happens sometimes
@@ -26,26 +40,40 @@
 
         content = chunk["choices"][0]["delta"].get("content", "")
 
         if content == None:
             continue
 
         accumulated_block += content
+        full_message += content
+        file_creation_path = is_file_present(full_message)
+        
+        
 
-        if accumulated_block.endswith("`"):
+        if accumulated_block.endswith("`") and (not accumulated_block.endswith("```")):
             # We might be writing "```" one token at a time.
             continue
 
         # Did we just enter a code block?
         if "```" in accumulated_block and not inside_code_block:
             inside_code_block = True
             accumulated_block = accumulated_block.split("```")[1]
 
         # Did we just exit a code block?
         if inside_code_block and "```" in accumulated_block:
+            
+            # Fix for fireworks ai
+            if language and "```" in content:
+                content = content.split("```")[0]
+                yield {
+                    "type": "code",
+                    "format": language,
+                    "content": content,
+                }
+                
             return
 
         # If we're in a code block,
         if inside_code_block:
             # If we don't have a `language`, find it
             if language is None and "\n" in accumulated_block:
                 language = accumulated_block.split("\n")[0]
@@ -57,18 +85,29 @@
                     elif llm.interpreter.os == False:
                         # OS mode does this frequently. Takes notes with markdown code blocks
                         language = "text"
                 else:
                     # Removes hallucinations containing spaces or non letters.
                     language = "".join(char for char in language if char.isalpha())
 
+            
             # If we do have a `language`, send it out
             if language:
+                
+                # Fix for fireworks ai
+                # TODO: Fix it , remove language only on codition. Impacting bash calls.
+                content = content.replace(language+"\n", "")
+                if content.strip() == "```":
+                    content = content.replace("```","")
+                elif "```" in content:
+                    content = content.split("```")[1]
+                    
                 yield {
                     "type": "code",
                     "format": language,
-                    "content": content.replace(language, ""),
+                    "content": content,
+                    "file_creation_path":file_creation_path,
                 }
 
         # If we're not in a code block, send the output as a message
         if not inside_code_block:
             yield {"type": "message", "content": content}
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py` & `blackboxai-2.7/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,72 @@
 import base64
 import io
 import json
 
 from PIL import Image
 
+def combine_assistant_messages(new_messages):
+    messages_to_remove = []
+    i = 0
+    while i < len(new_messages):
+        if new_messages[i]['role']=="assistant":
+            j = i+1
+            while j < len(new_messages) and new_messages[j]["role"] == "assistant":
+                new_messages[i]['content']+=(new_messages[j]['content']+"\n")
+                messages_to_remove.append(j)
+                j+=1
+            new_messages[i]['content'] = new_messages[i]['content'].replace("\nexecute>","")
+            i = j+1
+        else:
+            i+=1
+    
+    retained_messages = [_i for idx, _i in enumerate(new_messages) if idx not in messages_to_remove]
+    return retained_messages
+
 
 def convert_to_openai_messages(
-    messages, function_calling=True, vision=False, shrink_images=True
+    messages,
+    function_calling=True,
+    vision=False,
+    shrink_images=True,
+    code_output_sender="assistant",
 ):
     """
     Converts LMC messages into OpenAI messages
     """
     new_messages = []
+    last_code_idx = None
 
-    for message in messages:
+    for idx,message in enumerate(messages):
         # Is this for thine eyes?
         if "recipient" in message and message["recipient"] != "assistant":
             continue
-
+        
+        # skipping inbetween empty output messages
+        if (message['role'] =='computer' and 
+            message['type'] == "console" and 
+            len(messages) > idx+1 and 
+            len(message['content'].strip()) == 0):
+            
+            next_message =  messages[idx + 1]
+            if (next_message['role'] =='computer' and
+                next_message['type'] == "console" and
+                len(next_message['content'].strip()) > 0):
+                continue
+                
         new_message = {}
 
         if message["type"] == "message":
             new_message["role"] = message[
                 "role"
             ]  # This should never be `computer`, right?
             new_message["content"] = message["content"]
 
         elif message["type"] == "code":
+            last_code_idx = idx
             new_message["role"] = "assistant"
             if function_calling:
                 new_message["function_call"] = {
                     "name": "execute",
                     "arguments": json.dumps(
                         {"language": message["format"], "code": message["content"]}
                     ),
@@ -41,41 +77,83 @@
                         "code": message["content"],
                     },
                 }
                 # Add empty content to avoid error "openai.error.InvalidRequestError: 'content' is a required property - 'messages.*'"
                 # especially for the OpenAI service hosted on Azure
                 new_message["content"] = ""
             else:
-                new_message[
-                    "content"
-                ] = f"""```{message["format"]}\n{message["content"]}\n```"""
+                start_execute_tag = "<execute>\n"
+                if idx>0:
+                    prev_message = messages[idx-1]
+                    # If execute tag is existing in the previous end of message, do not add it again.
+                    if prev_message['role'] == "assistant" and prev_message['content'].strip().endswith("<execute>"):
+                        start_execute_tag = ""
+                        
+                if len(message["content"].strip())>0:
+                    new_message[
+                        "content"
+                    ] = f"""{start_execute_tag}```{message["format"]}\n{message["content"]}\n```\n</execute>"""
+                else:
+                    new_message["content"] = message["content"].strip()
 
         elif message["type"] == "console" and message["format"] == "output":
+            
+            additional_message = ""
+            
+            if last_code_idx is not None and messages[last_code_idx]['type'] == "code":
+                if 'pip install' in messages[last_code_idx]['content']:
+                    additional_message = "If the package is installed, write the code again to retry execution:"
+            
             if function_calling:
                 new_message["role"] = "function"
                 new_message["name"] = "execute"
                 if message["content"].strip() == "":
                     new_message[
                         "content"
                     ] = "No output"  # I think it's best to be explicit, but we should test this.
                 else:
                     new_message["content"] = message["content"]
 
             else:
-                if message["content"].strip() == "":
-                    content = "The code above was executed on my machine. It produced no text output. what's next (if anything, or are we done?)"
-                else:
-                    content = (
-                        "Code output: "
-                        + message["content"]
-                        + "\n\nWhat does this output mean / what's next (if anything, or are we done)?"
-                    )
-
-                new_message["role"] = "user"
-                new_message["content"] = content
+                # This should be experimented with.
+                if code_output_sender == "user":
+                    if message["content"].strip() == "":
+                        content = "The code above was executed on my machine. It produced no text output. what's next (if anything, or are we done?)"
+                    #elif "Error" in message["content"] or "Exception" in message["content"]:
+                    #    content = (
+                    #        "Code output: "
+                    #        + message["content"]
+                    #        + "\n\nFix this error. If you need more details about an api / method to fix, you can get help from search - using the search tool command"
+                    #    )
+                    else:
+                        content = (
+                            "Code output: "
+                            + message["content"]
+                            + "\n\nWhat does this output mean / what's next (if anything, or are we done)?"+additional_message
+                        )      
+                        additional_message = ""
+
+                    new_message["role"] = "user"
+                    new_message["content"] = content
+                elif code_output_sender == "assistant":
+                    if "@@@SEND_MESSAGE_AS_USER@@@" in message["content"]:
+                        new_message["role"] = "user"
+                        new_message["content"] = message["content"].replace(
+                            "@@@SEND_MESSAGE_AS_USER@@@", ""
+                        )
+                    else:
+                        if len(message["content"].strip())>0:
+                            new_message["role"] = "assistant"
+                            new_message["content"] = (
+                                "\n```output\n" + message["content"] + "\n```"
+                            )
+                        else:
+                            new_message["role"] = "assistant"
+                            new_message["content"] = message["content"].strip()
+                            
 
         elif message["type"] == "image":
             if vision == False:
                 continue
 
             if "base64" in message["format"]:
                 # Extract the extension from the format, default to 'png' if not specified
@@ -149,15 +227,21 @@
 
         elif message["type"] == "file":
             new_message = {"role": "user", "content": message["content"]}
 
         else:
             raise Exception(f"Unable to convert this message type: {message}")
 
+        new_message["content"] = new_message["content"].strip()
+
         new_messages.append(new_message)
+        
+        
+    new_messages = combine_assistant_messages(new_messages[:])
+   
 
     """
     # Combine adjacent user messages
     combined_messages = []
     i = 0
     while i < len(new_messages):
         message = new_messages[i]
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/llm/utils/merge_deltas.py` & `blackboxai-2.7/blackboxai/interpreter/core/llm/utils/merge_deltas.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/llm/utils/parse_partial_json.py` & `blackboxai-2.7/blackboxai/interpreter/core/llm/utils/parse_partial_json.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/llm/vision_for_text_llms.py` & `blackboxai-2.7/blackboxai/interpreter/core/llm/vision_for_text_llms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/respond.py` & `blackboxai-2.7/blackboxai/interpreter/core/respond.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 import re
 import traceback
 
 import litellm
 
 from ..terminal_interface.utils.display_markdown_message import display_markdown_message
 from .render_message import render_message
+from ..terminal_interface.utils.agent_utils import save_code_file
+
+FILE_PATH_REGEX = '''<execute>\\n*File:\s*['"](.*)["']\s*:'''
 
 
 def respond(interpreter):
     """
     Yields chunks.
     Responds until it decides not to run any more code or say anything else.
     """
 
     last_unsupported_code = ""
-    insert_force_task_completion_message = False
+    insert_loop_message = False
+    file_creation_path = None
 
     while True:
         ## RENDER SYSTEM MESSAGE ##
 
         system_message = interpreter.system_message
 
         # Add language-specific system messages
@@ -47,24 +51,25 @@
             "content": rendered_system_message,
         }
 
         # Create the version of messages that we'll send to the LLM
         messages_for_llm = interpreter.messages.copy()
         messages_for_llm = [rendered_system_message] + messages_for_llm
 
-        if insert_force_task_completion_message:
+        if insert_loop_message:
             messages_for_llm.append(
                 {
                     "role": "user",
                     "type": "message",
-                    "content": force_task_completion_message,
+                    "content": loop_message,
                 }
             )
             # Yield two newlines to seperate the LLMs reply from previous messages.
             yield {"role": "assistant", "type": "message", "content": "\n\n"}
+            insert_loop_message = False
 
         ### RUN THE LLM ###
 
         try:
             for chunk in interpreter.llm.run(messages_for_llm):
                 yield {"role": "assistant", **chunk}
 
@@ -110,35 +115,30 @@
                         "\n\nYou will need to add a payment method and purchase credits for the OpenAI API billing page (different from ChatGPT) to use GPT-4.\n\nhttps://platform.openai.com/account/billing/overview"
                     )
             elif interpreter.offline and not interpreter.os:
                 print(traceback.format_exc())
                 raise Exception(
                     "Error occurred. "
                     + str(e)
-                    + """
-
-If you're running `interpreter --local`, please make sure LM Studio's local server is running.
-
-If LM Studio's local server is running, please try a language model with a different architecture.
-
-                    """
                 )
             else:
                 raise
 
         ### RUN CODE (if it's there) ###
 
         if interpreter.messages[-1]["type"] == "code":
             if interpreter.verbose:
                 print("Running code:", interpreter.messages[-1])
 
             try:
                 # What language/code do you want to run?
                 language = interpreter.messages[-1]["format"].lower().strip()
                 code = interpreter.messages[-1]["content"]
+                file_creation_path = interpreter.messages[-1]["file_creation_path"] if "file_creation_path" in interpreter.messages[-1] else None
+
 
                 if language == "text":
                     # It does this sometimes just to take notes. Let it, it's useful.
                     # In the future we should probably not detect this behavior as code at all.
                     continue
 
                 # Is this language enabled/supported?
@@ -154,94 +154,114 @@
 
                     # Let the response continue so it can deal with the unsupported code in another way. Also prevent looping on the same piece of code.
                     if code != last_unsupported_code:
                         last_unsupported_code = code
                         continue
                     else:
                         break
-
+                
                 # Yield a message, such that the user can stop code execution if they want to
                 try:
                     yield {
                         "role": "computer",
                         "type": "confirmation",
                         "format": "execution",
                         "content": {
                             "type": "code",
                             "format": language,
                             "content": code,
+                            "file_creation_path":file_creation_path
                         },
                     }
                 except GeneratorExit:
                     # The user might exit here.
                     # We need to tell python what we (the generator) should do if they exit
                     break
 
                 # don't let it import computer — we handle that!
                 if interpreter.computer.import_computer_api and language == "python":
                     code = code.replace("import computer\n", "pass\n")
                     code = re.sub(
                         r"import computer\.(\w+) as (\w+)", r"\2 = computer.\1", code
                     )
                     code = re.sub(
-                        r"from computer import (\w+)", r"\1 = computer.\1", code
-                    )
-                    code = re.sub(
                         r"from computer import (.+)",
                         lambda m: "\n".join(
                             f"{x.strip()} = computer.{x.strip()}"
-                            for x in m.group(1).split(",")
+                            for x in m.group(1).split(", ")
                         ),
                         code,
                     )
+                    code = re.sub(r"import computer\.\w+\n", "pass\n", code)
                     # If it does this it sees the screenshot twice (which is expected jupyter behavior)
                     if code.split("\n")[-1] in [
                         "computer.display.view()",
                         "computer.display.screenshot()",
                         "computer.view()",
                         "computer.screenshot()",
                     ]:
                         code = code + "\npass"
 
                 # sync up some things (is this how we want to do this?)
                 interpreter.computer.verbose = interpreter.verbose
+                interpreter.computer.debug = interpreter.debug
                 interpreter.computer.emit_images = interpreter.llm.supports_vision
 
                 # sync up the interpreter's computer with your computer
                 try:
                     if interpreter.sync_computer and language == "python":
                         computer_dict = interpreter.computer.to_dict()
+                        if "_hashes" in computer_dict:
+                            computer_dict.pop("_hashes")
                         if computer_dict:
                             computer_json = json.dumps(computer_dict)
                             sync_code = f"""import json\ncomputer.load_dict(json.loads('''{computer_json}'''))"""
                             interpreter.computer.run("python", sync_code)
                 except Exception as e:
+                    if interpreter.debug:
+                        raise
                     print(str(e))
                     print("Continuing...")
 
                 ## ↓ CODE IS RUN HERE
-
-                for line in interpreter.computer.run(language, code, stream=True):
-                    yield {"role": "computer", **line}
+                
+                if file_creation_path:
+                    _msg = ""
+                    try:
+                        file_creation_path = save_code_file(code,file_creation_path)
+                        _msg = f"File '{file_creation_path}' created successfully."
+                    except Exception as e:
+                        _msg = str(e)
+                        
+                    yield {"role":"computer",
+                           "format":"output",
+                           "type":"console",
+                           "content": _msg}
+                    file_creation_path = None
+                else:
+                    for line in interpreter.computer.run(language, code, stream=True):
+                        yield {"role": "computer", **line}
 
                 ## ↑ CODE IS RUN HERE
 
                 # sync up your computer with the interpreter's computer
                 try:
                     if interpreter.sync_computer and language == "python":
                         # sync up the interpreter's computer with your computer
                         result = interpreter.computer.run(
                             "python",
-                            "import json\ncomputer_dict = computer.to_dict()\nif computer_dict:\n  print(json.dumps(computer_dict))",
+                            "import json\ncomputer_dict = computer.to_dict()\nif computer_dict:\n  if '_hashes' in computer_dict:\n    computer_dict.pop('_hashes')\n  print(json.dumps(computer_dict))",
                         )
                         result = result[-1]["content"]
                         interpreter.computer.load_dict(
                             json.loads(result.strip('"').strip("'"))
                         )
                 except Exception as e:
+                    if interpreter.debug:
+                        raise
                     print(str(e))
                     print("Continuing.")
 
                 # yield final "active_line" message, as if to say, no more code is running. unlightlight active lines
                 # (is this a good idea? is this our responsibility? i think so — we're saying what line of code is running! ...?)
                 yield {
                     "role": "computer",
@@ -255,43 +275,39 @@
                     "role": "computer",
                     "type": "console",
                     "format": "output",
                     "content": traceback.format_exc(),
                 }
 
         else:
-            ## FORCE TASK COMLETION
+            ## LOOP MESSAGE
             # This makes it utter specific phrases if it doesn't want to be told to "Proceed."
 
-            force_task_completion_message = """Proceed. You CAN run code on my machine. If you want to run code, start your message with "```"! If the entire task I asked for is done, say exactly 'The task is done.' If you need some specific information (like username or password) say EXACTLY 'Please provide more information.' If it's impossible, say 'The task is impossible.' (If I haven't provided a task, say exactly 'Let me know what you'd like to do next.') Otherwise keep going."""
+            loop_message = interpreter.loop_message
             if interpreter.os:
-                force_task_completion_message.replace(
+                loop_message = loop_message.replace(
                     "If the entire task I asked for is done,",
                     "If the entire task I asked for is done, take a screenshot to verify it's complete, or if you've already taken a screenshot and verified it's complete,",
                 )
-            force_task_completion_responses = [
-                "the task is done.",
-                "the task is impossible.",
-                "let me know what you'd like to do next.",
-                "please provide more information.",
-            ]
+            loop_breakers = interpreter.loop_breakers
 
             if (
-                interpreter.force_task_completion
+                interpreter.loop
                 and interpreter.messages
+                and interpreter.messages[-1].get("role", "").lower() == "assistant"
                 and not any(
-                    task_status in interpreter.messages[-1].get("content", "").lower()
-                    for task_status in force_task_completion_responses
+                    task_status in interpreter.messages[-1].get("content", "")
+                    for task_status in loop_breakers
                 )
             ):
-                # Remove past force_task_completion messages
+                # Remove past loop_message messages
                 interpreter.messages = [
                     message
                     for message in interpreter.messages
-                    if message.get("content", "") != force_task_completion_message
+                    if message.get("content", "") != loop_message
                 ]
                 # Combine adjacent assistant messages, so hopefully it learns to just keep going!
                 combined_messages = []
                 for message in interpreter.messages:
                     if (
                         combined_messages
                         and message["role"] == "assistant"
@@ -300,16 +316,16 @@
                         and combined_messages[-1]["type"] == "message"
                     ):
                         combined_messages[-1]["content"] += "\n" + message["content"]
                     else:
                         combined_messages.append(message)
                 interpreter.messages = combined_messages
 
-                # Send model the force_task_completion_message:
-                insert_force_task_completion_message = True
+                # Send model the loop_message:
+                insert_loop_message = True
 
                 continue
 
             # Doesn't want to run code. We're done!
             break
 
     return
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/server.py` & `blackboxai-2.7/blackboxai/interpreter/core/server.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_embed.py` & `blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_embed.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py` & `blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/utils/lazy_import.py` & `blackboxai-2.7/blackboxai/interpreter/core/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/utils/scan_code.py` & `blackboxai-2.7/blackboxai/interpreter/core/utils/scan_code.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/utils/system_debug_info.py` & `blackboxai-2.7/blackboxai/interpreter/core/utils/system_debug_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def get_oi_version():
     try:
         oi_version_cmd = subprocess.check_output(
             ["interpreter", "--version"], text=True
         )
     except Exception as e:
         oi_version_cmd = str(e)
-    oi_version_pkg = "v0.2.0" # pkg_resources.get_distribution("open-interpreter").version
+    oi_version_pkg = pkg_resources.get_distribution("open-interpreter").version
     oi_version = oi_version_cmd, oi_version_pkg
     return oi_version
 
 
 def get_os_version():
     return platform.platform()
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/utils/telemetry.py` & `blackboxai-2.7/blackboxai/interpreter/core/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/core/utils/temporary_file.py` & `blackboxai-2.7/blackboxai/interpreter/core/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/base_block.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/base_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/code_block.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/code_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/message_block.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/message_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/conversation_navigator.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/conversation_navigator.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/magic_commands.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/magic_commands.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/render_past_conversation.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/render_past_conversation.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/start_terminal_interface.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/start_terminal_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,21 @@
             "help_text": "optionally enable safety mechanisms like code scanning; valid options are off, ask, and auto",
             "type": str,
             "choices": ["off", "ask", "auto"],
             "default": "off",
             "attribute": {"object": interpreter, "attr_name": "safe_mode"},
         },
         {
+            "name": "debug",
+            "nickname": "debug",
+            "help_text": "debug mode for BlackboxAI Interpreter developers",
+            "type": bool,
+            "attribute": {"object": interpreter, "attr_name": "debug"},
+        },
+        {
             "name": "fast",
             "nickname": "f",
             "help_text": "runs `interpreter --model gpt-3.5-turbo` and asks OI to be extremely concise",
             "type": bool,
         },
         {
             "name": "multi_line",
@@ -183,15 +190,15 @@
             "help_text": "enable multi-line inputs starting and ending with ```",
             "type": bool,
             "attribute": {"object": interpreter, "attr_name": "multi_line"},
         },
         {
             "name": "local",
             "nickname": "l",
-            "help_text": "experimentally run the LLM locally via LM Studio (this changes many more settings than `--offline`)",
+            "help_text": "experimentally run the LLM locally via Llamafile (this changes many more settings than `--offline`)",
             "type": bool,
         },
         {
             "name": "vision",
             "nickname": "vi",
             "help_text": "experimentally use vision for supported languages",
             "type": bool,
@@ -227,15 +234,14 @@
             "type": bool,
         },
     ]
 
     # Check for deprecated flags before parsing arguments
     deprecated_flags = {
         "--debug_mode": "--verbose",
-        "-d": "-v",
     }
 
     for old_flag, new_flag in deprecated_flags.items():
         if old_flag in sys.argv:
             print(f"\n`{old_flag}` has been renamed to `{new_flag}`.\n")
             time.sleep(1.5)
             sys.argv.remove(old_flag)
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/terminal_interface.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/terminal_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,23 @@
 from .components.message_block import MessageBlock
 from .magic_commands import handle_magic_command
 from .utils.check_for_package import check_for_package
 from .utils.display_markdown_message import display_markdown_message
 from .utils.display_output import display_output
 from .utils.find_image_path import find_image_path
 from .utils.cli_input import cli_input
+from .utils.agent_utils import (parse_plan,
+                                parse_router,
+                                parse_summary,
+                                save_code_to_project,
+                                construct_crag_context,
+                                parse_crag_ranking,
+                                reconstruct_search_context,
+                                select_rewrite_query)
+from ..core.search import search
 
 # Add examples to the readline history
 examples = [
     "How many files are on my desktop?",
     "What time is it in Seattle?",
     "Make me a simple Pomodoro app.",
     "Open Chrome and go to YouTube.",
@@ -39,14 +48,16 @@
 try:
     for example in examples:
         readline.add_history(example)
 except:
     # If they don't have readline, that's fine
     pass
 
+conversation_context = ""
+FIRST_CODE_ASSISTANT_CALL = True
 
 def terminal_interface(interpreter, message):
     # Auto run and offline (this.. this isnt right) don't display messages.
     # Probably worth abstracting this to something like "debug_cli" at some point.
     if not interpreter.auto_run and not interpreter.offline:
         interpreter_intro_message = [
             "**BlackboxAI Interpreter** will require approval before running code."
@@ -54,28 +65,32 @@
 
         if interpreter.safe_mode == "ask" or interpreter.safe_mode == "auto":
             if not check_for_package("semgrep"):
                 interpreter_intro_message.append(
                     f"**Safe Mode**: {interpreter.safe_mode}\n\n>Note: **Safe Mode** requires `semgrep` (`pip install semgrep`)"
                 )
         else:
-            interpreter_intro_message.append("Use `blackboxai -y` to bypass this.")
+            interpreter_intro_message.append("Use `interpreter -y` to bypass this.")
 
         interpreter_intro_message.append("Press `CTRL-C` to exit.")
 
         display_markdown_message("\n\n".join(interpreter_intro_message) + "\n")
 
     if message:
         interactive = False
     else:
         interactive = True
 
     active_block = None
     voice_subprocess = None
-
+    search_context = ""
+    plan_messages = []
+    global conversation_context
+    global FIRST_CODE_ASSISTANT_CALL
+    route = None    
     while True:
         try:
             if interactive:
                 ### This is the primary input for BlackboxAI Interpreter.
                 message = cli_input("> ").strip() if interpreter.multi_line else input("> ").strip()
 
                 try:
@@ -129,296 +144,368 @@
                         "role": "user",
                         "type": "image",
                         "format": "path",
                         "content": image_path,
                     }
 
         try:
-            for chunk in interpreter.chat(message, display=False, stream=True):
-                yield chunk
+            if len(conversation_context.strip())>0:
+                router_messages = [{"role":"user","content":f"{conversation_context}#~#~#~#~#{message}"}]
+                router_response = interpreter.router_llm.run(router_messages)
+                route = parse_router(router_response)
+                print(f"\nRouting the request to - {route} ...\n")
+            
+            if route=="planner" or len(conversation_context.strip())==0:
+                print("\nPlanning ...\n")
+                is_first_call = len(conversation_context.strip())==0
+                search_context = ""
+                conversation_context += (f"Request : {message}\nAssistant:\n")
+                planner_context = f"Conversation context:\n{conversation_context}" if not is_first_call else ""
+                plan_messages = plan_messages + [{"role":"user","content":f"{planner_context}#~#~#~#~#{message}"}]
+                plan_response = interpreter.planner_llm.run(plan_messages)
+                conversation_context += (f"Planner : {plan_response}\n")
+                plan_messages = plan_messages + [{'role':'assistant','content': plan_response}]
+                plan_stack = parse_plan(plan_response)
+                print("\n".join([f"{x['call']}" for x in plan_stack ]))
+            else:
+                plan_stack = [{"call":{"tool_name":"code_assistant","query":message}}]
+                
+            valid_plan_stack = [step for step in plan_stack if step["call"]["tool_name"] in ["search","summarizer","code_assistant"]]
+            
+            # if no valid tool call found , route it to code_assistant.
+            if len(valid_plan_stack)==0:
+                valid_plan_stack = [{"call":{"tool_name":"code_assistant","query":message}}]
+            
+            for step in valid_plan_stack:
+                tool_name = step["call"]["tool_name"].strip().lower()
+                query = step["call"]["query"] if "query" in step["call"] else step["call"]["instruction"]
+
+                if tool_name == "search":
+                    if isinstance(query,str):
+                        query = [query]
+                        
+                    if interpreter.debug:
+                        print(f"Searching the web for {query} ...")
+                    rerank_query = select_rewrite_query(query[:3])
+                    search_response = search(search_queries=query[:3],
+                                             rerank_query=rerank_query,
+                                             user_query=message,
+                                             serper_endpoint=interpreter.websearch_endpoint)
+                    search_context += (query[0] + ":\n"+ search_response+"\n\n")
+                    if interpreter.debug:
+                        print(f"Rerank query - {rerank_query} ...")
+                        print("\nSearch context:",search_context)
+                
+                elif tool_name == "summarizer":
+                    summ_messages = [{"role":"user","content":conversation_context}]
+                    summ_response = interpreter.summarizer_llm.run(summ_messages)
+                    parsed_code_list,project_name = parse_summary(summ_response)
+                    save_code_to_project(parsed_code_list,project_name)
+                    print(f"Project created:{project_name}")
+                    
+                elif tool_name == "code_assistant":
+                    # When only code_assistant is called, better replace the request with the original message
+                    if len(plan_stack)==1:
+                        query = message
+                    
+                    query = f"{search_context}#~#~#~#~#{query}" #interpreter.llm.user_request_prompt.format(search_context=search_context,message=query)
+                        
+                    # reset search context after using
+                    search_context = ""
+                    conversation_context+=("Code execution:\n")
+                    for chunk in interpreter.chat(query, display=False, stream=True):
+                        conversation_context+=(chunk['content'] if 'content' in chunk and isinstance(chunk['content'],str) else "")
+                        yield chunk
+
+                        # Is this for thine eyes?
+                        if "recipient" in chunk and chunk["recipient"] != "user":
+                            continue
 
-                # Is this for thine eyes?
-                if "recipient" in chunk and chunk["recipient"] != "user":
-                    continue
-
-                if interpreter.verbose:
-                    print("Chunk in `terminal_interface`:", chunk)
-
-                # Comply with PyAutoGUI fail-safe for OS mode
-                # so people can turn it off by moving their mouse to a corner
-                if interpreter.os:
-                    if (
-                        chunk.get("format") == "output"
-                        and "failsafeexception" in chunk["content"].lower()
-                    ):
-                        print("Fail-safe triggered (mouse in one of the four corners).")
-                        break
-
-                if "end" in chunk and active_block:
-                    active_block.refresh(cursor=False)
-
-                    if chunk["type"] in [
-                        "message",
-                        "console",
-                    ]:  # We don't stop on code's end — code + console output are actually one block.
-                        active_block.end()
-                        active_block = None
-
-                # Assistant message blocks
-                if chunk["type"] == "message":
-                    if "start" in chunk:
-                        active_block = MessageBlock()
-                        render_cursor = True
-
-                    if "content" in chunk:
-                        active_block.message += chunk["content"]
-
-                    if "end" in chunk and interpreter.os:
-                        last_message = interpreter.messages[-1]["content"]
-
-                        # Remove markdown lists and the line above markdown lists
-                        lines = last_message.split("\n")
-                        i = 0
-                        while i < len(lines):
-                            # Match markdown lists starting with hyphen, asterisk or number
-                            if re.match(r"^\s*([-*]|\d+\.)\s", lines[i]):
-                                del lines[i]
-                                if i > 0:
-                                    del lines[i - 1]
-                                    i -= 1
-                            else:
-                                i += 1
-                        message = "\n".join(lines)
-                        # Replace newlines with spaces, escape double quotes and backslashes
-                        sanitized_message = (
-                            message.replace("\\", "\\\\")
-                            .replace("\n", " ")
-                            .replace('"', '\\"')
-                        )
+                        if interpreter.verbose:
+                            print("Chunk in `terminal_interface`:", chunk)
 
-                        # Display notification in OS mode
+                        # Comply with PyAutoGUI fail-safe for OS mode
+                        # so people can turn it off by moving their mouse to a corner
                         if interpreter.os:
-                            interpreter.computer.os.notify(sanitized_message)
-
-                        # Speak message aloud
-                        if platform.system() == "Darwin" and interpreter.speak_messages:
-                            if voice_subprocess:
-                                voice_subprocess.terminate()
-                            voice_subprocess = subprocess.Popen(
-                                [
-                                    "osascript",
-                                    "-e",
-                                    f'say "{sanitized_message}" using "Fred"',
-                                ]
-                            )
-                        else:
-                            pass
-                            # User isn't on a Mac, so we can't do this. You should tell them something about that when they first set this up.
-                            # Or use a universal TTS library.
-
-                # Assistant code blocks
-                elif chunk["role"] == "assistant" and chunk["type"] == "code":
-                    if "start" in chunk:
-                        active_block = CodeBlock()
-                        active_block.language = chunk["format"]
-                        render_cursor = True
-
-                    if "content" in chunk:
-                        active_block.code += chunk["content"]
-
-                # Execution notice
-                if chunk["type"] == "confirmation":
-                    if not interpreter.auto_run:
-                        # OI is about to execute code. The user wants to approve this
+                            if (
+                                chunk.get("format") == "output"
+                                and "failsafeexception" in chunk["content"].lower()
+                            ):
+                                print("Fail-safe triggered (mouse in one of the four corners).")
+                                break
 
-                        # End the active code block so you can run input() below it
-                        if active_block:
+                        if "end" in chunk and active_block:
                             active_block.refresh(cursor=False)
-                            active_block.end()
-                            active_block = None
 
-                        code_to_run = chunk["content"]
-                        language = code_to_run["format"]
-                        code = code_to_run["content"]
-
-                        should_scan_code = False
-
-                        if not interpreter.safe_mode == "off":
-                            if interpreter.safe_mode == "auto":
-                                should_scan_code = True
-                            elif interpreter.safe_mode == "ask":
+                            if chunk["type"] in [
+                                "message",
+                                "console",
+                            ]:  # We don't stop on code's end — code + console output are actually one block.
+                                active_block.end()
+                                active_block = None
+
+                        # Assistant message blocks
+                        if chunk["type"] == "message":
+                            if "start" in chunk:
+                                active_block = MessageBlock()
+                                render_cursor = True
+
+                            if "content" in chunk:
+                                active_block.message += chunk["content"]
+
+                            if "end" in chunk and interpreter.os:
+                                last_message = interpreter.messages[-1]["content"]
+
+                                # Remove markdown lists and the line above markdown lists
+                                lines = last_message.split("\n")
+                                i = 0
+                                while i < len(lines):
+                                    # Match markdown lists starting with hyphen, asterisk or number
+                                    if re.match(r"^\s*([-*]|\d+\.)\s", lines[i]):
+                                        del lines[i]
+                                        if i > 0:
+                                            del lines[i - 1]
+                                            i -= 1
+                                    else:
+                                        i += 1
+                                message = "\n".join(lines)
+                                # Replace newlines with spaces, escape double quotes and backslashes
+                                sanitized_message = (
+                                    message.replace("\\", "\\\\")
+                                    .replace("\n", " ")
+                                    .replace('"', '\\"')
+                                )
+
+                                # Display notification in OS mode
+                                if interpreter.os:
+                                    interpreter.computer.os.notify(sanitized_message)
+
+                                # Speak message aloud
+                                if platform.system() == "Darwin" and interpreter.speak_messages:
+                                    if voice_subprocess:
+                                        voice_subprocess.terminate()
+                                    voice_subprocess = subprocess.Popen(
+                                        [
+                                            "osascript",
+                                            "-e",
+                                            f'say "{sanitized_message}" using "Fred"',
+                                        ]
+                                    )
+                                else:
+                                    pass
+                                    # User isn't on a Mac, so we can't do this. You should tell them something about that when they first set this up.
+                                    # Or use a universal TTS library.
+
+                        # Assistant code blocks
+                        elif chunk["role"] == "assistant" and chunk["type"] == "code":
+                            if "start" in chunk:
+                                active_block = CodeBlock()
+                                active_block.language = chunk["format"]
+                                render_cursor = True
+
+                            if "content" in chunk:
+                                active_block.code += chunk["content"]
+
+                        # Execution notice
+                        if chunk["type"] == "confirmation":
+                            if not interpreter.auto_run:
+                                # OI is about to execute code. The user wants to approve this
+
+                                # End the active code block so you can run input() below it
+                                if active_block:
+                                    active_block.refresh(cursor=False)
+                                    active_block.end()
+                                    active_block = None
+
+                                code_to_run = chunk["content"]
+                                language = code_to_run["format"]
+                                code = code_to_run["content"]
+
+                                should_scan_code = False
+
+                                if not interpreter.safe_mode == "off":
+                                    if interpreter.safe_mode == "auto":
+                                        should_scan_code = True
+                                    elif interpreter.safe_mode == "ask":
+                                        response = input(
+                                            "  Would you like to scan this code? (y/n)\n\n  "
+                                        )
+                                        print("")  # <- Aesthetic choice
+
+                                        if response.strip().lower() == "y":
+                                            should_scan_code = True
+
+                                if should_scan_code:
+                                    scan_code(code, language, interpreter)
+
+                                _ask_msg =  "  Would you like to run this code? (y/n)\n\n  "
+                                 
+                                if "file_creation_path" in chunk["content"] and chunk["content"]["file_creation_path"]:
+                                    _ask_msg =  f"  Would you like to write this code to {chunk['content']['file_creation_path']} ? (y/n)\n\n  "
+                                    
                                 response = input(
-                                    "  Would you like to scan this code? (y/n)\n\n  "
+                                   _ask_msg
                                 )
                                 print("")  # <- Aesthetic choice
 
                                 if response.strip().lower() == "y":
-                                    should_scan_code = True
-
-                        if should_scan_code:
-                            scan_code(code, language, interpreter)
-
-                        response = input(
-                            "  Would you like to run this code? (y/n)\n\n  "
-                        )
-                        print("")  # <- Aesthetic choice
-
-                        if response.strip().lower() == "y":
-                            # Create a new, identical block where the code will actually be run
-                            # Conveniently, the chunk includes everything we need to do this:
-                            active_block = CodeBlock()
-                            active_block.margin_top = False  # <- Aesthetic choice
-                            active_block.language = language
-                            active_block.code = code
-                        else:
-                            # User declined to run code.
-                            interpreter.messages.append(
-                                {
-                                    "role": "user",
-                                    "type": "message",
-                                    "content": "I have declined to run this code.",
-                                }
-                            )
-                            break
-
-                # Computer can display visual types to user,
-                # Which sometimes creates more computer output (e.g. HTML errors, eventually)
-                if (
-                    chunk["role"] == "computer"
-                    and "content" in chunk
-                    and (
-                        chunk["type"] == "image"
-                        or ("format" in chunk and chunk["format"] == "html")
-                        or ("format" in chunk and chunk["format"] == "javascript")
-                    )
-                ):
-                    if interpreter.os and interpreter.verbose == False:
-                        # We don't display things to the user in OS control mode, since we use vision to communicate the screen to the LLM so much.
-                        # But if verbose is true, we do display it!
-                        continue
-
-                    # Display and give extra output back to the LLM
-                    extra_computer_output = display_output(chunk)
-
-                    # We're going to just add it to the messages directly, not changing `recipient` here.
-                    # Mind you, the way we're doing this, this would make it appear to the user if they look at their conversation history,
-                    # because we're not adding "recipient: assistant" to this block. But this is a good simple solution IMO.
-                    # we just might want to change it in the future, once we're sure that a bunch of adjacent type:console blocks will be rendered normally to text-only LLMs
-                    # and that if we made a new block here with "recipient: assistant" it wouldn't add new console outputs to that block (thus hiding them from the user)
-
-                    if (
-                        interpreter.messages[-1].get("format") != "output"
-                        or interpreter.messages[-1]["role"] != "computer"
-                        or interpreter.messages[-1]["type"] != "console"
-                    ):
-                        # If the last message isn't a console output, make a new block
-                        interpreter.messages.append(
-                            {
-                                "role": "computer",
-                                "type": "console",
-                                "format": "output",
-                                "content": extra_computer_output,
-                            }
-                        )
-                    else:
-                        # If the last message is a console output, simply append the extra output to it
-                        interpreter.messages[-1]["content"] += (
-                            "\n" + extra_computer_output
-                        )
-                        interpreter.messages[-1]["content"] = interpreter.messages[-1][
-                            "content"
-                        ].strip()
-
-                # Console
-                if chunk["type"] == "console":
-                    render_cursor = False
-                    if "format" in chunk and chunk["format"] == "output":
-                        active_block.output += "\n" + chunk["content"]
-                        active_block.output = (
-                            active_block.output.strip()
-                        )  # ^ Aesthetic choice
-
-                        # Truncate output
-                        active_block.output = truncate_output(
-                            active_block.output, interpreter.max_output
-                        )
-                    if "format" in chunk and chunk["format"] == "active_line":
-                        active_block.active_line = chunk["content"]
-
-                        # Display action notifications if we're in OS mode
-                        if interpreter.os and active_block.active_line != None:
-                            action = ""
-
-                            code_lines = active_block.code.split("\n")
-                            if active_block.active_line < len(code_lines):
-                                action = code_lines[active_block.active_line].strip()
-
-                            if action.startswith("computer"):
-                                description = None
-
-                                # Extract arguments from the action
-                                start_index = action.find("(")
-                                end_index = action.rfind(")")
-                                if start_index != -1 and end_index != -1:
-                                    # (If we found both)
-                                    arguments = action[start_index + 1 : end_index]
+                                    # Create a new, identical block where the code will actually be run
+                                    # Conveniently, the chunk includes everything we need to do this:
+                                    active_block = CodeBlock()
+                                    active_block.margin_top = False  # <- Aesthetic choice
+                                    active_block.language = language
+                                    active_block.code = code
                                 else:
-                                    arguments = None
+                                    # User declined to run code.
+                                    
+                                    if interpreter.append_decline_message:
+                                        interpreter.messages.append(
+                                            {
+                                                "role": "user",
+                                                "type": "message",
+                                                "content": "I have declined to run this code.",
+                                            }
+                                        )
+                                    break
+
+                        # Computer can display visual types to user,
+                        # Which sometimes creates more computer output (e.g. HTML errors, eventually)
+                        if (
+                            chunk["role"] == "computer"
+                            and "content" in chunk
+                            and (
+                                chunk["type"] == "image"
+                                or ("format" in chunk and chunk["format"] == "html")
+                                or ("format" in chunk and chunk["format"] == "javascript")
+                            )
+                        ):
+                            if interpreter.os and interpreter.verbose == False:
+                                # We don't display things to the user in OS control mode, since we use vision to communicate the screen to the LLM so much.
+                                # But if verbose is true, we do display it!
+                                continue
+
+                            # Display and give extra output back to the LLM
+                            extra_computer_output = display_output(chunk)
+
+                            # We're going to just add it to the messages directly, not changing `recipient` here.
+                            # Mind you, the way we're doing this, this would make it appear to the user if they look at their conversation history,
+                            # because we're not adding "recipient: assistant" to this block. But this is a good simple solution IMO.
+                            # we just might want to change it in the future, once we're sure that a bunch of adjacent type:console blocks will be rendered normally to text-only LLMs
+                            # and that if we made a new block here with "recipient: assistant" it wouldn't add new console outputs to that block (thus hiding them from the user)
+
+                            if (
+                                interpreter.messages[-1].get("format") != "output"
+                                or interpreter.messages[-1]["role"] != "computer"
+                                or interpreter.messages[-1]["type"] != "console"
+                            ):
+                                # If the last message isn't a console output, make a new block
+                                interpreter.messages.append(
+                                    {
+                                        "role": "computer",
+                                        "type": "console",
+                                        "format": "output",
+                                        "content": extra_computer_output,
+                                    }
+                                )
+                            else:
+                                # If the last message is a console output, simply append the extra output to it
+                                interpreter.messages[-1]["content"] += (
+                                    "\n" + extra_computer_output
+                                )
+                                interpreter.messages[-1]["content"] = interpreter.messages[-1][
+                                    "content"
+                                ].strip()
+
+                        # Console
+                        if chunk["type"] == "console":
+                            render_cursor = False
+                            if "format" in chunk and chunk["format"] == "output":
+                                active_block.output += "\n" + chunk["content"]
+                                active_block.output = (
+                                    active_block.output.strip()
+                                )  # ^ Aesthetic choice
+
+                                # Truncate output
+                                active_block.output = truncate_output(
+                                    active_block.output, interpreter.max_output
+                                )
+                            if "format" in chunk and chunk["format"] == "active_line":
+                                active_block.active_line = chunk["content"]
 
-                                # NOTE: Do not put the text you're clicking on screen
-                                # (unless we figure out how to do this AFTER taking the screenshot)
-                                # otherwise it will try to click this notification!
-
-                                if action in [
-                                    "computer.screenshot()",
-                                    "computer.display.screenshot()",
-                                    "computer.display.view()",
-                                    "computer.view()",
-                                ]:
-                                    description = "Viewing screen..."
-                                elif action == "computer.mouse.click()":
-                                    description = "Clicking..."
-                                elif action.startswith("computer.mouse.click("):
-                                    if "icon=" in arguments:
-                                        text_or_icon = "icon"
-                                    else:
-                                        text_or_icon = "text"
-                                    description = f"Clicking {text_or_icon}..."
-                                elif action.startswith("computer.mouse.move("):
-                                    if "icon=" in arguments:
-                                        text_or_icon = "icon"
-                                    else:
-                                        text_or_icon = "text"
-                                    if (
-                                        "click" in active_block.code
-                                    ):  # This could be better
-                                        description = f"Clicking {text_or_icon}..."
-                                    else:
-                                        description = f"Mousing over {text_or_icon}..."
-                                elif action.startswith("computer.keyboard.write("):
-                                    description = f"Typing {arguments}."
-                                elif action.startswith("computer.keyboard.hotkey("):
-                                    description = f"Pressing {arguments}."
-                                elif action.startswith("computer.keyboard.press("):
-                                    description = f"Pressing {arguments}."
-                                elif action == "computer.os.get_selected_text()":
-                                    description = f"Getting selected text."
-
-                                if description:
-                                    interpreter.computer.os.notify(description)
-
-                    if "start" in chunk:
-                        # We need to make a code block if we pushed out an HTML block first, which would have closed our code block.
-                        if not isinstance(active_block, CodeBlock):
-                            if active_block:
-                                active_block.end()
-                            active_block = CodeBlock()
+                                # Display action notifications if we're in OS mode
+                                if interpreter.os and active_block.active_line != None:
+                                    action = ""
+
+                                    code_lines = active_block.code.split("\n")
+                                    if active_block.active_line < len(code_lines):
+                                        action = code_lines[active_block.active_line].strip()
+
+                                    if action.startswith("computer"):
+                                        description = None
+
+                                        # Extract arguments from the action
+                                        start_index = action.find("(")
+                                        end_index = action.rfind(")")
+                                        if start_index != -1 and end_index != -1:
+                                            # (If we found both)
+                                            arguments = action[start_index + 1 : end_index]
+                                        else:
+                                            arguments = None
+
+                                        # NOTE: Do not put the text you're clicking on screen
+                                        # (unless we figure out how to do this AFTER taking the screenshot)
+                                        # otherwise it will try to click this notification!
+
+                                        if action in [
+                                            "computer.screenshot()",
+                                            "computer.display.screenshot()",
+                                            "computer.display.view()",
+                                            "computer.view()",
+                                        ]:
+                                            description = "Viewing screen..."
+                                        elif action == "computer.mouse.click()":
+                                            description = "Clicking..."
+                                        elif action.startswith("computer.mouse.click("):
+                                            if "icon=" in arguments:
+                                                text_or_icon = "icon"
+                                            else:
+                                                text_or_icon = "text"
+                                            description = f"Clicking {text_or_icon}..."
+                                        elif action.startswith("computer.mouse.move("):
+                                            if "icon=" in arguments:
+                                                text_or_icon = "icon"
+                                            else:
+                                                text_or_icon = "text"
+                                            if (
+                                                "click" in active_block.code
+                                            ):  # This could be better
+                                                description = f"Clicking {text_or_icon}..."
+                                            else:
+                                                description = f"Mousing over {text_or_icon}..."
+                                        elif action.startswith("computer.keyboard.write("):
+                                            description = f"Typing {arguments}."
+                                        elif action.startswith("computer.keyboard.hotkey("):
+                                            description = f"Pressing {arguments}."
+                                        elif action.startswith("computer.keyboard.press("):
+                                            description = f"Pressing {arguments}."
+                                        elif action == "computer.os.get_selected_text()":
+                                            description = f"Getting selected text."
+
+                                        if description:
+                                            interpreter.computer.os.notify(description)
+
+                            if "start" in chunk:
+                                # We need to make a code block if we pushed out an HTML block first, which would have closed our code block.
+                                if not isinstance(active_block, CodeBlock):
+                                    if active_block:
+                                        active_block.end()
+                                    active_block = CodeBlock()
 
-                if active_block:
-                    active_block.refresh(cursor=render_cursor)
+                        if active_block:
+                            active_block.refresh(cursor=render_cursor)
 
             # (Sometimes -- like if they CTRL-C quickly -- active_block is still None here)
             if "active_block" in locals():
                 if active_block:
                     active_block.end()
                     active_block = None
                     time.sleep(0.1)
```

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/check_for_package.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/check_for_package.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/count_tokens.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_output.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_output.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/blackboxai/interpreter/terminal_interface/validate_llm_settings.py` & `blackboxai-2.7/blackboxai/interpreter/terminal_interface/validate_llm_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,26 +61,26 @@
             # This is a model we don't have checks for yet.
             break
 
     # If we're here, we passed all the checks.
 
     # Auto-run is for fast, light useage -- no messages.
     # If offline, it's usually a bogus model name for LiteLLM since LM Studio doesn't require one.
-    if True:#not interpreter.auto_run and not interpreter.offline:
+    if not interpreter.auto_run and not interpreter.offline:
         display_markdown_message(f"> Model set to `{interpreter.llm.model}`")
     return
 
 
 def display_welcome_message_once():
     """
     Displays a welcome message only on its first call.
 
     (Uses an internal attribute `_displayed` to track its state.)
     """
-    if True:#not hasattr(display_welcome_message_once, "_displayed"):
+    if not hasattr(display_welcome_message_once, "_displayed"):
         display_markdown_message(
             """
         ●
 
         Welcome to **BlackboxAI Interpreter**.
         """
         )
```

### Comparing `blackboxai-2.6/blackboxai.egg-info/PKG-INFO` & `blackboxai-2.7/blackboxai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 2.6
+Version: 2.7
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
```

### Comparing `blackboxai-2.6/blackboxai.egg-info/SOURCES.txt` & `blackboxai-2.7/blackboxai.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,44 +3,54 @@
 pyproject.toml
 setup.py
 ./blackboxai/__init__.py
 ./blackboxai/chat.py
 ./blackboxai/interpreter/__init__.py
 ./blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
 ./blackboxai/interpreter/core/__init__.py
+./blackboxai/interpreter/core/browser.py
 ./blackboxai/interpreter/core/core.py
 ./blackboxai/interpreter/core/default_system_message.py
 ./blackboxai/interpreter/core/render_message.py
 ./blackboxai/interpreter/core/respond.py
+./blackboxai/interpreter/core/search.py
 ./blackboxai/interpreter/core/server.py
 ./blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
 ./blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
 ./blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
 ./blackboxai/interpreter/core/computer/__init__.py
 ./blackboxai/interpreter/core/computer/computer.py
 ./blackboxai/interpreter/core/computer/ai/__init__.py
 ./blackboxai/interpreter/core/computer/ai/ai.py
 ./blackboxai/interpreter/core/computer/browser/__init__.py
 ./blackboxai/interpreter/core/computer/browser/browser.py
+./blackboxai/interpreter/core/computer/calendar/__init__.py
+./blackboxai/interpreter/core/computer/calendar/calendar.py
 ./blackboxai/interpreter/core/computer/clipboard/__init__.py
 ./blackboxai/interpreter/core/computer/clipboard/clipboard.py
+./blackboxai/interpreter/core/computer/contacts/__init__.py
+./blackboxai/interpreter/core/computer/contacts/contacts.py
 ./blackboxai/interpreter/core/computer/display/__init__.py
 ./blackboxai/interpreter/core/computer/display/display.py
 ./blackboxai/interpreter/core/computer/docs/__init__.py
 ./blackboxai/interpreter/core/computer/docs/docs.py
 ./blackboxai/interpreter/core/computer/files/__init__.py
 ./blackboxai/interpreter/core/computer/files/files.py
 ./blackboxai/interpreter/core/computer/keyboard/__init__.py
 ./blackboxai/interpreter/core/computer/keyboard/keyboard.py
+./blackboxai/interpreter/core/computer/mail/__init__.py
+./blackboxai/interpreter/core/computer/mail/mail.py
 ./blackboxai/interpreter/core/computer/mouse/__init__.py
 ./blackboxai/interpreter/core/computer/mouse/mouse.py
 ./blackboxai/interpreter/core/computer/os/__init__.py
 ./blackboxai/interpreter/core/computer/os/os.py
 ./blackboxai/interpreter/core/computer/skills/__init__.py
 ./blackboxai/interpreter/core/computer/skills/skills.py
+./blackboxai/interpreter/core/computer/sms/__init__.py
+./blackboxai/interpreter/core/computer/sms/sms.py
 ./blackboxai/interpreter/core/computer/terminal/__init__.py
 ./blackboxai/interpreter/core/computer/terminal/base_language.py
 ./blackboxai/interpreter/core/computer/terminal/terminal.py
 ./blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
 ./blackboxai/interpreter/core/computer/terminal/languages/__init__.py
 ./blackboxai/interpreter/core/computer/terminal/languages/applescript.py
 ./blackboxai/interpreter/core/computer/terminal/languages/html.py
@@ -53,15 +63,17 @@
 ./blackboxai/interpreter/core/computer/terminal/languages/shell.py
 ./blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
 ./blackboxai/interpreter/core/computer/utils/__init__.py
 ./blackboxai/interpreter/core/computer/utils/computer_vision.py
 ./blackboxai/interpreter/core/computer/utils/get_active_window.py
 ./blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
 ./blackboxai/interpreter/core/computer/utils/recipient_utils.py
+./blackboxai/interpreter/core/computer/utils/run_applescript.py
 ./blackboxai/interpreter/core/llm/__init__.py
+./blackboxai/interpreter/core/llm/agent_llm.py
 ./blackboxai/interpreter/core/llm/llm.py
 ./blackboxai/interpreter/core/llm/run_function_calling_llm.py
 ./blackboxai/interpreter/core/llm/run_text_llm.py
 ./blackboxai/interpreter/core/llm/vision_for_text_llms.py
 ./blackboxai/interpreter/core/llm/utils/__init__.py
 ./blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
 ./blackboxai/interpreter/core/llm/utils/merge_deltas.py
@@ -84,17 +96,21 @@
 ./blackboxai/interpreter/terminal_interface/start_terminal_interface.py
 ./blackboxai/interpreter/terminal_interface/terminal_interface.py
 ./blackboxai/interpreter/terminal_interface/validate_llm_settings.py
 ./blackboxai/interpreter/terminal_interface/components/__init__.py
 ./blackboxai/interpreter/terminal_interface/components/base_block.py
 ./blackboxai/interpreter/terminal_interface/components/code_block.py
 ./blackboxai/interpreter/terminal_interface/components/message_block.py
+./blackboxai/interpreter/terminal_interface/profiles/__init__.py
+./blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
+./blackboxai/interpreter/terminal_interface/profiles/profiles.py
 ./blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
 ./blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
 ./blackboxai/interpreter/terminal_interface/utils/__init__.py
+./blackboxai/interpreter/terminal_interface/utils/agent_utils.py
 ./blackboxai/interpreter/terminal_interface/utils/check_for_package.py
 ./blackboxai/interpreter/terminal_interface/utils/check_for_update.py
 ./blackboxai/interpreter/terminal_interface/utils/cli_input.py
 ./blackboxai/interpreter/terminal_interface/utils/count_tokens.py
 ./blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
 ./blackboxai/interpreter/terminal_interface/utils/display_output.py
 ./blackboxai/interpreter/terminal_interface/utils/find_image_path.py
@@ -102,8 +118,9 @@
 ./blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
 ./blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
 ./blackboxai/interpreter/terminal_interface/utils/oi_dir.py
 blackboxai.egg-info/PKG-INFO
 blackboxai.egg-info/SOURCES.txt
 blackboxai.egg-info/dependency_links.txt
 blackboxai.egg-info/entry_points.txt
-blackboxai.egg-info/top_level.txt
+blackboxai.egg-info/top_level.txt
+tests/test_interpreter.py
```

### Comparing `blackboxai-2.6/pyproject.toml` & `blackboxai-2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboxai-2.6/setup.py` & `blackboxai-2.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="blackboxai",
-    version="2.6",
+    version="2.7",
     packages=find_packages(),
     package_dir = {'': '.'},
     include_package_data=True,
     setup_requires= ['requests'],
     entry_points={
         "console_scripts": [
             "blackboxai = blackboxai:runChat"
```

