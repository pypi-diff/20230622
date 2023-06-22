# Comparing `tmp/napari-chatgpt-2023.6.21.tar.gz` & `tmp/napari-chatgpt-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-chatgpt-2023.6.21.tar", last modified: Thu Jun 22 03:40:07 2023, max compression
+gzip compressed data, was "napari-chatgpt-2023.6.3.tar", last modified: Sun Jun  4 04:04:01 2023, max compression
```

## Comparing `napari-chatgpt-2023.6.21.tar` & `napari-chatgpt-2023.6.3.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.749645 napari-chatgpt-2023.6.21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.705642 napari-chatgpt-2023.6.21/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.713643 napari-chatgpt-2023.6.21/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/.github/workflows/just_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.713643 napari-chatgpt-2023.6.21/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-06-22 03:40:07.749645 napari-chatgpt-2023.6.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-22 03:40:07.749645 napari-chatgpt-2023.6.21/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.713643 napari-chatgpt-2023.6.21/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.713643 napari-chatgpt-2023.6.21/src/napari_chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.717643 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/bard_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/conv_agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/enumerate_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/enumerate_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/gpt4all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/gtts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/lanchain_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/openai_list_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/playwright_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/tts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/whisper_cpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.717643 napari-chatgpt-2023.6.21/src/napari_chatgpt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 03:40:07.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.717643 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.717643 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/chat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.717643 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.725644 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/
--rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/_tailwind.css
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/chat.js
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/marked-highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/prism.css
--rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/prism.js
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/sunlight-min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/sunlight.dark.css
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/tailwind.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.729644 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.729644 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/llms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.729644 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.729644 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/test/.pytest_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/test/bard_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.729644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.733644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/memory/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/napari_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.733644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/agent_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.733644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.733644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/async_base_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.733644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/demo/tools_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.733644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.733644 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/cellpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari_base_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/web_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/file_download_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/human_input_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/api_key_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/async_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/async_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/async_utils/run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/gpt4all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.737645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/test/download_files_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/test/summarizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/napari_viewer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/open_in_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/omega_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/omega_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/omega_plugins/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.741645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/dynamic_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/exception_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/exception_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/fix_code_given_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/installed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/missing_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/python_lang_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/required_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.745645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/exception_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/exception_guard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/installed_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/required_imports_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.745645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/qt/download_file_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/qt/qt_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.745645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/extract_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/filter_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/find_function_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/python_code_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.745645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/extract_code_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/extract_url_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.745645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/system/folders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.749645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/metasearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/scrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.749645 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/google_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/metasearch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/scrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/wikipedia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:40:07.713643 napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-06-22 03:40:07.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-22 03:40:07.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:40:07.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-22 03:40:07.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-22 03:40:07.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 03:40:07.000000 napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-22 03:39:47.000000 napari-chatgpt-2023.6.21/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.545266 napari-chatgpt-2023.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.github/workflows/just_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.561267 napari-chatgpt-2023.6.3/src/napari_chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/bard_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/conv_agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gpt4all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gtts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/lanchain_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/openai_list_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/playwright_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/tts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/whisper_cpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.569267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.573267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/_tailwind.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/chat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/marked-highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.css
+-rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/tailwind.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/llms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.577267 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/.pytest_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/test/bard_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/napari_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/async_base_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/tools_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cellpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_base_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.581267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/file_download_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/human_input_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/gpt4all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/download_files_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/summarizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/napari_viewer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/open_in_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.585267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/dynamic_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_code_given_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/installed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/missing_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/python_lang_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/required_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_guard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/installed_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/required_imports_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/download_file_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/qt_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/filter_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_function_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/python_code_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_url_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/system/folders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.589267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/metasearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/scrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.593267 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/google_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/metasearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/scrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/wikipedia_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:04:01.565267 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 04:04:01.000000 napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-04 04:03:45.000000 napari-chatgpt-2023.6.3/tox.ini
```

### Comparing `napari-chatgpt-2023.6.21/.github/workflows/just_deploy.yml` & `napari-chatgpt-2023.6.3/.github/workflows/just_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/.github/workflows/test_and_deploy.yml` & `napari-chatgpt-2023.6.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/.gitignore` & `napari-chatgpt-2023.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/.napari-hub/config.yml` & `napari-chatgpt-2023.6.3/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/.pre-commit-config.yaml` & `napari-chatgpt-2023.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/LICENSE` & `napari-chatgpt-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/PKG-INFO` & `napari-chatgpt-2023.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.6.21
+Version: 2023.6.3
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
```

### Comparing `napari-chatgpt-2023.6.21/README.md` & `napari-chatgpt-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/setup.cfg` & `napari-chatgpt-2023.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/conv_agent_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/conv_agent_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/enumerate_functions.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/enumerate_functions.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/gpt4all_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/gpt4all_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/lanchain_openai.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/lanchain_openai.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/playwright_sandbox.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/playwright_sandbox.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/speech_recognition_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/speech_recognition_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/terminal.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/terminal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/tts_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/tts_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_sandbox/whisper_cpp.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_sandbox/whisper_cpp.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_tests/test_widget.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/_widget.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,28 @@
 see: https://napari.org/stable/plugins/guides.html?#widgets
 
 Replace code below according to your needs.
 """
 import sys
 from typing import TYPE_CHECKING
 
-from napari_chatgpt.chat_server.chat_server import NapariChatServer
-from napari_chatgpt.utils.api_keys.api_key import set_api_key
-from napari_chatgpt.utils.python.installed_packages import \
-    is_package_installed
+import openai
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QApplication, QLabel, QCheckBox
 from PyQt5.QtWidgets import QVBoxLayout, QComboBox
 from napari.viewer import Viewer
 from qtpy.QtWidgets import QPushButton, QWidget
 
-
-
+from napari_chatgpt.chat_server.chat_server import NapariChatServer
+from napari_chatgpt.utils.python.installed_packages import is_package_installed
 
 if TYPE_CHECKING:
     pass
 
-from arbol import aprint, asection
+from arbol import aprint
 
 _creativity_mapping = {}
 _creativity_mapping['normal'] = 0.0
 _creativity_mapping['slightly creative'] = 0.05
 _creativity_mapping['moderately creative'] = 0.1
 _creativity_mapping['creative'] = 0.2
 
@@ -37,15 +34,14 @@
 class OmegaQWidget(QWidget):
     # your QWidget.__init__ can optionally request the napari viewer instance
     # in one of two ways:
     # 1. use a parameter called `napari_viewer`, as done here
     # 2. use a type annotation of 'napari.viewer.Viewer' for any parameter
     def __init__(self, napari_viewer):
         super().__init__()
-        aprint("OmegaQWidget instantiated!")
 
         # Napari viewer instance:
         self.viewer = napari_viewer
 
         # Napari chat server instance:
         self.server: NapariChatServer = None
 
@@ -69,37 +65,31 @@
 
         self._start_omega_button()
 
         # Set the layout on the application's window
         self.setLayout(self.layout)
 
     def _model_selection(self):
-        aprint("Setting up model selection UI.")
-
         # Create a QLabel instance
         self.model_label = QLabel("Select a model:")
         # Add the label to the layout
         self.layout.addWidget(self.model_label)
         # Create a QComboBox instance
         self.model_combo_box = QComboBox()
         # Set tooltip for the combo box
         self.model_combo_box.setToolTip(
             "Choose an LLM model. Best models are GPT4 and GPT3.5, \n"
             "with Claude a bit behind, other models are experimental\n"
             "and unfortunately barely usable.")
 
         # Add OpenAI models to the combo box:
-        with asection(f"Enumerating all OpenAI ChatGPT models:"):
-            import openai
-            set_api_key('OpenAI')
-            for model in openai.Model.list().data:
-                model_id = model.openai_id
-                if 'gpt' in model_id:
-                    aprint(model_id)
-                    self.model_combo_box.addItem(model_id)
+        for model in openai.Model.list().data:
+            model_id = model.openai_id
+            if 'gpt' in model_id:
+                self.model_combo_box.addItem(model_id)
 
         # if is_package_installed('googlebard'):
         self.model_combo_box.addItem('bard')
 
         if is_package_installed('anthropic'):
             # Add Anthropic models to the combo box:
             self.model_combo_box.addItem('claude-v1')
@@ -118,16 +108,14 @@
 
         # Connect the activated signal to a slot
         # self.model_combo_box.activated[str].connect(self.onActivated)
         # Add the combo box to the layout
         self.layout.addWidget(self.model_combo_box)
 
     def _creativity_level(self):
-        aprint("Setting up creativity level UI.")
-
         # Create a QLabel instance
         self.creativity_label = QLabel("Chose the level of creativity:")
         # Add the label to the layout
         self.layout.addWidget(self.creativity_label)
         # Creativity combobox:
         self.creativity_combo_box = QComboBox()
         self.creativity_combo_box.setToolTip(
@@ -143,16 +131,14 @@
         self.creativity_combo_box.addItem('moderately creative')
         self.creativity_combo_box.addItem('creative')
         self.creativity_combo_box.setCurrentIndex(0)
         # Add the creativity combobox to the layout:
         self.layout.addWidget(self.creativity_combo_box)
 
     def _memory_type_selection(self):
-        aprint("Setting up memory type UI.")
-
         # Create a QLabel instance
         self.memory_type_label = QLabel("Select a memory type:")
         # Add the label to the layout
         self.layout.addWidget(self.memory_type_label)
         # Create a QComboBox instance
         self.memory_type_combo_box = QComboBox()
         self.memory_type_combo_box.setToolTip(
@@ -163,16 +149,14 @@
         self.memory_type_combo_box.addItem('hybrid')
         self.memory_type_combo_box.addItem('bounded')
         self.memory_type_combo_box.addItem('infinite')
         # Add the combo box to the layout
         self.layout.addWidget(self.memory_type_combo_box)
 
     def _personality_selection(self):
-        aprint("Setting up personality UI.")
-
         # Create a QLabel instance
         self.agent_personality_label = QLabel("Select a personality:")
         # Add the label to the layout
         self.layout.addWidget(self.agent_personality_label)
         # Create a QComboBox instance
         self.agent_personality_combo_box = QComboBox()
         self.agent_personality_combo_box.setToolTip(
@@ -184,60 +168,52 @@
         self.agent_personality_combo_box.addItem('prof')
         self.agent_personality_combo_box.addItem('mobster')
         self.agent_personality_combo_box.addItem('yoda')
         # Add the combo box to the layout
         self.layout.addWidget(self.agent_personality_combo_box)
 
     def _fix_imports(self):
-        aprint("Setting up fix imports UI.")
-
         # Create a QLabel instance
         self.fix_imports_checkbox = QCheckBox("Fix missing imports")
         self.fix_imports_checkbox.setChecked(True)
         self.fix_imports_checkbox.setToolTip(
             "Uses LLM to check for missing imports.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money."
         )
         # Add the fix_imports checkbox to the layout:
         self.layout.addWidget(self.fix_imports_checkbox)
 
     def _fix_bad_version_calls(self):
-        aprint("Setting up bad version imports UI.")
-
         # Create a QLabel instance
         self.fix_bad_calls_checkbox = QCheckBox("Fix bad function calls")
         self.fix_bad_calls_checkbox.setChecked(True)
         self.fix_bad_calls_checkbox.setToolTip("Uses LLM to fix function calls.\n"
                                               "When turned on, this detects wrong function calls, \n"
                                               "possibly because of library version mismatch and fixes,"
                                               "replaces the offending code with the right version! "
                                               "This involves a LLM call which can incurr additional\n"
                                               "cost in time and possibly money."
                                                )
         # Add the fix_code checkbox to the layout:
         self.layout.addWidget(self.fix_bad_calls_checkbox)
 
     def _install_missing_packages(self):
-        aprint("Setting up install missing packages UI.")
-
         # Create a QLabel instance
         self.install_missing_packages_checkbox = QCheckBox(
             "Install missing packages")
         self.install_missing_packages_checkbox.setChecked(True)
         self.install_missing_packages_checkbox.setToolTip(
             "Uses LLM to figure out which packages to install.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money.")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.install_missing_packages_checkbox)
 
     def _autofix_mistakes(self):
-        aprint("Setting up autofix mistakes UI.")
-
         # Create a QLabel instance
         self.autofix_mistakes_checkbox = QCheckBox(
             "Autofix coding mistakes")
         self.autofix_mistakes_checkbox.setChecked(False)
         self.autofix_mistakes_checkbox.setToolTip(
             "When checked Omega will try to fix on its own coding mistakes\n"
             "when processing data and interacting with the napari viewer.\n"
@@ -245,32 +221,28 @@
             "Works so-so with ChatGPT 3.5, but works well with ChatGPT 4.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money.")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.autofix_mistakes_checkbox)
 
     def _autofix_widgets(self):
-        aprint("Setting up autofix widgets UI.")
-
         # Create a QLabel instance
         self.autofix_widgets_checkbox = QCheckBox(
             "Autofix widget coding mistakes")
         self.autofix_widgets_checkbox.setChecked(False)
         self.autofix_widgets_checkbox.setToolTip(
             "When checked Omega will try to fix its own \n"
             "coding mistakes when making widgets. \n"
             "Works so-so with ChatGPT 3.5, but works well with ChatGPT 4.\n"
             "This involves a LLM call which can incur additional\n"
             "cost in time and possibly money.")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.autofix_widgets_checkbox)
 
     def _verbose(self):
-        aprint("Setting up verbose UI.")
-
         # Create a QLabel instance
         self.verbose_checkbox = QCheckBox(
             "High console verbosity")
         self.verbose_checkbox.setChecked(False)
         self.verbose_checkbox.setToolTip(
             "High level of verbosity in the console\n"
             "This includes a lot of internal logging\n"
@@ -278,29 +250,27 @@
             "Nearly incomprehensible, but usefull\n"
             "if you are interested to see the prompts\n"
             "in action...")
         # Add the install_missing_packages checkbox to the layout:
         self.layout.addWidget(self.verbose_checkbox)
 
     def _start_omega_button(self):
-        aprint("Setting up start Omega button UI.")
-
         # Start Omega button:
         self.start_omega_button = QPushButton("Start Omega")
         self.start_omega_button.clicked.connect(self._on_click)
         self.start_omega_button.setToolTip(
             "Start Omega, this will open a browser window.\n"
             "You can restart Omega with new settings by\n"
             "clicking again this button. This closes the\n"
             "previous session.")
         # Omega button:
         self.layout.addWidget(self.start_omega_button)
 
     def _on_click(self):
-        aprint("Starting Omega now!")
+        aprint("Starting Omega!")
 
         # Stop previous instance if it exists:
         if self.server:
             self.server.stop()
 
         # Temperature:
         temperature = float(_creativity_mapping[
```

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/chat_server.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/chat_server.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/_tailwind.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/_tailwind.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/chat.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/chat.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/marked-highlight.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/marked-highlight.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/prism.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/prism.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/prism.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/sunlight-min.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/sunlight.dark.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.dark.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/sunlight.python-min.js` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/sunlight.python-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/static/tailwind.min.css` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/static/tailwind.min.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/chat_server/templates/index.html` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/chat_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/bard.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/bard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/gpt4all.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/llm/llms.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/llm/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import multiprocessing
 import os
 
-from arbol import aprint
 from langchain.callbacks.manager import AsyncCallbackManager
 from langchain.chat_models import ChatOpenAI, ChatAnthropic
 
 from napari_chatgpt.llm.bard import ChatBard
 from napari_chatgpt.llm.gpt4all import GPT4AllFixed
 from napari_chatgpt.utils.download.gpt4all import get_gpt4all_model
 
@@ -14,15 +13,14 @@
                      temperature: float,
                      tool_temperature: float,
                      chat_callback_handler,
                      tool_callback_handler,
                      memory_callback_handler,
                      verbose: bool = False
                      ):
-    aprint(f"Instantiating LLMs with model: '{llm_model_name}', t={temperature}, t_tool={tool_temperature}. ")
     if 'gpt-' in llm_model_name:
         # Instantiates Main LLM:
         main_llm = ChatOpenAI(
             model_name=llm_model_name,
             verbose=verbose,
             streaming=True,
             temperature=temperature,
```

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/memory/memory.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/memory/memory.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/napari_bridge.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/napari_bridge.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/agent.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/prompts.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/omega_init.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/omega_init.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/async_base_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/async_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/demo/tools_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/demo/tools_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/cellpose.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/file_open_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/file_open_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/napari_base_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/napari_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/web_search_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/web_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/file_download_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/file_download_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/functions_info_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/functions_info_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/omega/tools/special/human_input_tool.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/omega/tools/special/human_input_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/api_key_vault.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/async_utils/run_async.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/async_utils/run_async.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/download_files.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/download_files.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/gpt4all.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/download/test/download_files_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/download/test/download_files_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/summarizer.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/summarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from langchain.chains.summarize import load_summarize_chain
+from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.llms import BaseLLM
 from langchain.text_splitter import CharacterTextSplitter
 
 
 def summarize(text: str, llm: BaseLLM = None):
     # Clean up text:
     text = text.strip()
 
     # Is there anything to summarise?
     if len(text) == 0:
         return text
 
     # Instantiates LLM if needed:
-    from langchain.chat_models import ChatOpenAI
     llm = llm or ChatOpenAI(model_name='gpt-3.5-turbo', temperature=0)
 
     # Splits the text:
     text_splitter = CharacterTextSplitter()
     texts = text_splitter.split_text(text)
 
     # Make documents from the text:
```

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/llm/test/summarizer_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/llm/test/summarizer_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/napari_viewer_info.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/napari_viewer_info.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/open_in_napari.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/open_in_napari.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/dynamic_import.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/exception_description.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_description.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/exception_guard.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/exception_guard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/fix_code_given_error.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/fix_code_given_error.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/installed_packages.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/installed_packages.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/missing_packages.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/missing_packages.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/python_lang_utils.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/python_lang_utils.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/required_imports.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/required_imports.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/exception_description_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/exception_description_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/missing_libraries_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/missing_libraries_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/python/test/required_imports_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/python/test/required_imports_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/qt/download_file_qt.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/qt/download_file_qt.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/camel_case_to_normal.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/camel_case_to_normal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/extract_urls.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/extract_urls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/filter_lines.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/filter_lines.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/python_code_cleanup.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/python_code_cleanup.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/extract_code_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/extract_code_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/strings/test/filter_lines_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/strings/test/filter_lines_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/duckduckgo.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/google.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/google.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/headers.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/headers.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/metasearch.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/metasearch.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/scrapper.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/scrapper.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/duckduckgo_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/duckduckgo_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/metasearch_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/metasearch_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/test/wikipedia_test.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/test/wikipedia_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt/utils/web/wikipedia.py` & `napari-chatgpt-2023.6.3/src/napari_chatgpt/utils/web/wikipedia.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/PKG-INFO` & `napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.6.21
+Version: 2023.6.3
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
```

### Comparing `napari-chatgpt-2023.6.21/src/napari_chatgpt.egg-info/SOURCES.txt` & `napari-chatgpt-2023.6.3/src/napari_chatgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.6.21/tox.ini` & `napari-chatgpt-2023.6.3/tox.ini`

 * *Files identical despite different names*

