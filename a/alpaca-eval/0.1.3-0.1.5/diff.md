# Comparing `tmp/alpaca_eval-0.1.3.tar.gz` & `tmp/alpaca_eval-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.1.3.tar", last modified: Sun Jun 11 23:01:49 2023, max compression
+gzip compressed data, was "alpaca_eval-0.1.5.tar", last modified: Thu Jun 22 01:49:46 2023, max compression
```

## Comparing `alpaca_eval-0.1.3.tar` & `alpaca_eval-0.1.5.tar`

### file list

```diff
@@ -1,156 +1,174 @@
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.576854 alpaca_eval-0.1.3/
--rw-r--r--   0 rtaori     (501) staff       (20)    11409 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/LICENSE
--rw-r--r--   0 rtaori     (501) staff       (20)      187 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/MANIFEST.in
--rw-r--r--   0 rtaori     (501) staff       (20)    64419 2023-06-11 23:01:49.576688 alpaca_eval-0.1.3/PKG-INFO
--rw-r--r--   0 rtaori     (501) staff       (20)    63598 2023-06-11 22:46:48.000000 alpaca_eval-0.1.3/README.md
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.559123 alpaca_eval-0.1.3/example/
--rw-r--r--   0 rtaori     (501) staff       (20)   517613 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/example/outputs.json
--rw-r--r--   0 rtaori     (501) staff       (20)       38 2023-06-11 23:01:49.576893 alpaca_eval-0.1.3/setup.cfg
--rw-r--r--   0 rtaori     (501) staff       (20)     2123 2023-06-11 22:46:22.000000 alpaca_eval-0.1.3/setup.py
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.555032 alpaca_eval-0.1.3/src/
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.561843 alpaca_eval-0.1.3/src/alpaca_eval/
--rw-r--r--   0 rtaori     (501) staff       (20)       22 2023-06-11 22:58:03.000000 alpaca_eval-0.1.3/src/alpaca_eval/__init__.py
--rw-r--r--   0 rtaori     (501) staff       (20)    20821 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.563197 alpaca_eval-0.1.3/src/alpaca_eval/annotators/
--rw-r--r--   0 rtaori     (501) staff       (20)       33 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 rtaori     (501) staff       (20)    31305 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 rtaori     (501) staff       (20)     3939 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 rtaori     (501) staff       (20)     5218 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/constants.py
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.564312 alpaca_eval-0.1.3/src/alpaca_eval/decoders/
--rw-r--r--   0 rtaori     (501) staff       (20)     1913 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 rtaori     (501) staff       (20)     4730 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 rtaori     (501) staff       (20)     2835 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 rtaori     (501) staff       (20)     3905 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 rtaori     (501) staff       (20)     4697 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 rtaori     (501) staff       (20)    11804 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/openai.py
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.564494 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 rtaori     (501) staff       (20)     9670 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.564813 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)     1204 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      270 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.567347 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 rtaori     (501) staff       (20)     1650 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     5869 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     2475 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     3721 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     3423 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     6849 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     6797 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     6700 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     6045 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)     1016 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     3969 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     5932 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)     5370 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.567677 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)     7373 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      362 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.567971 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)     1048 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      324 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.568278 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 rtaori     (501) staff       (20)     1116 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      325 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.568584 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 rtaori     (501) staff       (20)     1137 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      317 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.568933 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 rtaori     (501) staff       (20)      259 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)     1087 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569140 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 rtaori     (501) staff       (20)      303 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569320 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)      314 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569624 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 rtaori     (501) staff       (20)     1298 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      452 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569774 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)      322 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569931 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)      317 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.570250 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)      319 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)     1051 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.570563 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 rtaori     (501) staff       (20)     1054 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      367 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.570884 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 rtaori     (501) staff       (20)     1017 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      341 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.556446 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571338 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 rtaori     (501) staff       (20)     1739 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 rtaori     (501) staff       (20)     1744 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 rtaori     (501) staff       (20)      351 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571494 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 rtaori     (501) staff       (20)     2577 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 rtaori     (501) staff       (20)    21692 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/main.py
--rw-r--r--   0 rtaori     (501) staff       (20)     1313 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.558209 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571817 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 rtaori     (501) staff       (20)      382 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)      152 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571964 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 rtaori     (501) staff       (20)      433 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572117 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 rtaori     (501) staff       (20)      456 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572266 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 rtaori     (501) staff       (20)      196 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572528 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 rtaori     (501) staff       (20)      184 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)       34 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572673 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 rtaori     (501) staff       (20)      188 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/cohere/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572811 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 rtaori     (501) staff       (20)      405 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572951 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 rtaori     (501) staff       (20)      401 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573228 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 rtaori     (501) staff       (20)      100 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      178 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573391 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573528 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573657 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573968 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 rtaori     (501) staff       (20)      425 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)      195 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574255 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 rtaori     (501) staff       (20)      407 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574385 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 rtaori     (501) staff       (20)      449 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574705 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 rtaori     (501) staff       (20)      436 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)       42 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574978 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 rtaori     (501) staff       (20)      458 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)       51 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575108 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 rtaori     (501) staff       (20)      438 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575256 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 rtaori     (501) staff       (20)      211 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575554 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 rtaori     (501) staff       (20)      211 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)       34 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575856 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 rtaori     (501) staff       (20)      387 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.576158 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 rtaori     (501) staff       (20)      383 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.576418 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 rtaori     (501) staff       (20)      394 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
--rw-r--r--   0 rtaori     (501) staff       (20)    22484 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/plotting.py
--rw-r--r--   0 rtaori     (501) staff       (20)      283 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/types.py
--rw-r--r--   0 rtaori     (501) staff       (20)    15488 2023-06-11 22:44:32.000000 alpaca_eval-0.1.3/src/alpaca_eval/utils.py
-drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.562847 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/
--rw-r--r--   0 rtaori     (501) staff       (20)    64419 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 rtaori     (501) staff       (20)     5723 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 rtaori     (501) staff       (20)        1 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 rtaori     (501) staff       (20)       54 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 rtaori     (501) staff       (20)      418 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 rtaori     (501) staff       (20)       12 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/top_level.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:46.007835 alpaca_eval-0.1.5/
+-rw-rw-r--   0 rtaori   (20446) root         (0)    11409 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/LICENSE
+-rw-rw-r--   0 rtaori   (20446) root         (0)      187 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/MANIFEST.in
+-rw-rw-r--   0 rtaori   (20446) root         (0)    66360 2023-06-22 01:49:46.005835 alpaca_eval-0.1.5/PKG-INFO
+-rw-rw-r--   0 rtaori   (20446) root         (0)    65538 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/README.md
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.543830 alpaca_eval-0.1.5/example/
+-rw-rw-r--   0 rtaori   (20446) root         (0)   517613 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/example/outputs.json
+-rw-rw-r--   0 rtaori   (20446) root         (0)       38 2023-06-22 01:49:46.008835 alpaca_eval-0.1.5/setup.cfg
+-rw-rw-r--   0 rtaori   (20446) root         (0)     2123 2023-06-12 20:45:15.000000 alpaca_eval-0.1.5/setup.py
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.426829 alpaca_eval-0.1.5/src/
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.585830 alpaca_eval-0.1.5/src/alpaca_eval/
+-rw-rw-r--   0 rtaori   (20446) root         (0)       22 2023-06-22 01:48:21.000000 alpaca_eval-0.1.5/src/alpaca_eval/__init__.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)    21396 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/analyze.py
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.626831 alpaca_eval-0.1.5/src/alpaca_eval/annotators/
+-rw-rw-r--   0 rtaori   (20446) root         (0)       33 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/annotators/__init__.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)    33988 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)     4018 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/completion_parsers.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)     5317 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/constants.py
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.644831 alpaca_eval-0.1.5/src/alpaca_eval/decoders/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1913 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/__init__.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)     4873 2023-06-16 13:47:30.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/anthropic.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)     3476 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/cohere.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)     3905 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_api.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)     4899 2023-06-16 13:47:30.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_local.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)    12623 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/openai.py
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.648831 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     9753 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/README.md
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.655831 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1204 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      270 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.662831 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      905 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1140 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.707832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1650 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     5869 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     2475 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     3721 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     3423 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     6849 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     6797 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     6700 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     6045 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1016 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     3969 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     5932 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)     5370 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.716832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     7373 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      362 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.723832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1048 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      324 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.730832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1116 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      325 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.738832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1197 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      754 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.746832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1137 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      317 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.754832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      259 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1087 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.760832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/cohere/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      303 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.764832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      314 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.773832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1298 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      452 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.778832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      322 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.782832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      317 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.790833 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      319 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1051 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.797833 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1054 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      367 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.805833 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1017 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      341 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.473829 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.819833 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     2037 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-rw-r--   0 rtaori   (20446) root         (0)      904 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1820 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-rw-r--   0 rtaori   (20446) root         (0)      351 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.824833 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/evaluators/
+-rw-rw-r--   0 rtaori   (20446) root         (0)     2929 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-rw-r--   0 rtaori   (20446) root         (0)    21870 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/main.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)     1313 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/metrics.py
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.525830 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.833833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      415 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      171 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.838833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      415 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.846833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      382 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      152 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.851833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      433 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.855833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      456 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.859833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/chatgpt/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      196 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.867833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/claude/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      184 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)       34 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.874833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      199 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)       13 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.878833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere-chat/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      205 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.882834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      405 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.886834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      401 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.894834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/gpt4/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      100 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      178 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.898834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      430 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.902834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      430 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.905834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      430 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.913834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      425 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      195 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.921834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      429 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      186 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.930834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      407 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.934834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      449 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.943834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      436 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)       42 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.952834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      458 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)       51 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.958834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      438 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.963834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      211 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.972834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      211 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)       34 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.981835 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      387 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.990835 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      383 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:46.000835 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-rw-r--   0 rtaori   (20446) root         (0)      394 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)    22484 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/plotting.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)      283 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/types.py
+-rw-rw-r--   0 rtaori   (20446) root         (0)    15815 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/utils.py
+drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.617831 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/
+-rw-rw-r--   0 rtaori   (20446) root         (0)    66360 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/PKG-INFO
+-rw-rw-r--   0 rtaori   (20446) root         (0)     6457 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)        1 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)       54 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/entry_points.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)      418 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/requires.txt
+-rw-rw-r--   0 rtaori   (20446) root         (0)       12 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/top_level.txt
```

### Comparing `alpaca_eval-0.1.3/LICENSE` & `alpaca_eval-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/PKG-INFO` & `alpaca_eval-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,26 @@
-Metadata-Version: 2.1
-Name: alpaca_eval
-Version: 0.1.3
-Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
-Author: The Alpaca Team
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: analysis
-Provides-Extra: dev
-Provides-Extra: local
-Provides-Extra: api
-Provides-Extra: all
-License-File: LICENSE
-
 # <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
 [![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
-[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE)
+[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
 Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
 AlpacaEval provides the following:
 
 - [**Automatic evaluator**](#evaluators): an automatic evaluator that has high agreement with humans (validated on 20K
   annotations). We evaluate a
   model by
-  measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs from that model over
+  measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that model
+  over
   outputs from a reference model. Our evaluators enable caching and output randomization by default.
 - [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
   evaluation set.
 - [**Toolkit for building automatic evaluators**](#analysis): a simple interface for
   building advanced automatic evaluators (e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
   price, speed, statistical power, bias, variance etc).
 - [**Human evaluation data**](#data-release): 20K human preferences between a given and reference model
@@ -86,14 +64,15 @@
     - [Contributing an eval set](#contributing-an-eval-set)
 6. [Limitations](#limitations)
 7. [Citation](#citation)
 8. [Additional information](#additional-information)
     - [Data Release](#data-release)
     - [Differences with AlpacaFarm](#differences-with-alpacafarm)
     - [Related work](#related-work)
+    - [Major updates](#major-updates)
 
 </details>
 
 # Quick Start
 
 To install the stable release, run
 
@@ -116,19 +95,20 @@
 ```
 
 Important parameters are the following:
 
 - **model_outputs** : A path to a json file for the outputs of the model to add to the leaderboard. Each dictionary
   should
   contain the keys `instruction` and `output`.
-- **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`). `alpaca_eval_gpt4` (
+- **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`
+  or `chatgpt_fn`). `alpaca_eval_gpt4` (
   default) has the
-  highest agreement rate with our human annotation data. `claude` has a decent agreement and is free for academics. For
-  a comparison of
-  annotators see [here](#evaluators).
+  highest agreement rate with our human annotation data. `claude` has a decent agreement and is free for
+  academics. `chatgpt_fn` is the worst of the three, but is available to everyone, cheap, and has 2x larger context
+  window (16K tokens). For a comparison of annotators see [here](#evaluators).
 - **reference_outputs**:  The outputs of the reference model. Same format as `model_outputs`. By default, this
   is `text-davinci003` outputs on
   AlpacaEval dataset.
 - **output_path**: Path for saving annotations and leaderboard.
 
 If you don't have the model outputs, you can
 use [`evaluate_from_model`](https://github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and
@@ -164,16 +144,17 @@
 For more information about each function use `alpaca_eval <command> -- --help`.
 
 # Leaderboards and how to interpret them
 
 ## Models
 
 Our leaderboards are computed on the [AlpacaEval dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval).
-We precomputed the leaderboard for important models both using `gpt4` (best quality) and  `claude` (free for academics,
-and high quality). Our full leaderboards can be found at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but
+We precomputed the leaderboard for important models using `alpaca_eval_gpt4` (best quality),  `claude` (free for
+academics, and high quality), and `chatgpt_fn` (cheap and available for everyone). Our full leaderboards can be found
+at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but
 we give minimal leaderboards below.
 Later we also show how to [add your model](https://github.com/tatsu-lab/alpaca_eval#evaluating-a-model) to the
 leaderboard and how to make
 a [new leaderboard for your evaluator/dataset](https://github.com/tatsu-lab/alpaca_eval#making-a-new-leaderboard).
 See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) for the configs of all
 models that are available out of the box.
 
@@ -260,38 +241,58 @@
 | falcon-40b-instruct   |     46.7 |       1.8 |
 | alpaca-farm-ppo-human |     46.5 |       1.8 |
 | alpaca-7b             |     32.3 |       1.6 |
 | text_davinci_001      |     21.5 |       1.4 |
 
 </details>
 
+<details>
+  <summary><b><code>chatgpt_fn</code> minimal leaderboard</b></summary>
+
+|                       | Win Rate | Std Err. |
+|:----------------------|---------:|---------:|
+| gpt4                  |     73.8 |      1.5 |
+| claude                |     70.4 |      1.6 |
+| chatgpt               |     66.1 |      1.7 |
+| wizardlm-13b          |     65.2 |      1.7 |
+| vicuna-13b            |     64.1 |      1.7 |
+| guanaco-65b           |     62.4 |      1.7 |
+| oasst-rlhf-llama-33b  |     62.0 |      1.7 |
+| alpaca-farm-ppo-human |     60.2 |      1.7 |
+| falcon-40b-instruct   |     56.5 |      1.7 |
+| text_davinci_003      |     50.0 |      0.0 |
+| alpaca-7b             |     45.2 |      1.7 |
+| text_davinci_001      |     28.1 |      1.6 |
+
+</details>
+
 ## Evaluators
 
 We evaluate different automatic annotators on the AlpacaEval set by comparing to
 2.5K [human annotations](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/main/alpaca_farm_human_crossannotations.json)
 we collected (~650 instructions each with 4 human annotations).
 Below we show metrics for our suggested evaluator (`alpaca_eval_gpt4`), for prior
 automatic
 evaluators ([`alpaca_farm_greedy_gpt4`](https://github.com/tatsu-lab/alpaca_farm),[`aviary_gpt4`](https://aviary.anyscale.com/),[`lmsys_gpt4`](https://chat.lmsys.org/)),
 for humans (`humans`), and for different base models with essentially the same
-prompt (`gpt4`,`claude`,`text_davinci_003`,`guanaco_33b`, `chatgpt`).
+prompt (`gpt4`,`claude`,`text_davinci_003`,`chatgpt_fn`,`guanaco_33b`, `chatgpt`).
 See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs) for the configs of all
 evaluators that are available out of the box and their associated metrics.
 
 |                         | Human agreement [%] | Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer longer |
 |:------------------------|--------------------:|------------------------:|-----------------------------:|-----:|---------:|---------------------:|
 | alpaca_eval_gpt4        |                69.2 |                    13.6 |                         1455 | 28.4 |     14.6 |                 0.68 |
 | aviary_gpt4             |                69.1 |                    12.8 |                         1869 | 29.5 |     13.1 |                 0.70 |
 | gpt4                    |                66.9 |                    12.5 |                         1037 | 31.5 |     14.6 |                 0.65 |
 | alpaca_farm_greedy_gpt4 |                66.4 |                    15.3 |                          878 | 30.2 |     19.3 |                 0.60 |
-| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |          |                 0.64 |
+| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |     34.3 |                 0.64 |
 | claude                  |                65.5 |                    11.1 |                          173 | 31.9 |     18.0 |                 0.62 |
 | text_davinci_003        |                64.1 |                     8.7 |                          121 | 33.8 |     22.7 |                 0.70 |
 | lmsys_gpt4              |                63.2 |                    13.9 |                        17982 | 34.7 |     16.1 |                 0.74 |
-| guanaco_33b             |                59.1 |                         |                          930 | 54.5 |     27.1 |                 0.70 |
+| chatgpt_fn              |                60.0 |                     1.0 |                          530 | 36.9 |     27.7 |                 0.62 |
 | chatgpt                 |                57.2 |                     0.8 |                          285 | 39.4 |     34.1 |                 0.59 |
 
 <details>
   <summary><b>How exactly are those metrics computed?</b></summary>
 
 We now explain in words how we compute the metrics in the table
 above. [The code is here](https://github.com/tatsu-lab/alpaca_eval/blob/f05cbd651b79ac93906b19d01fe443b45828b0f2/src/alpaca_eval/analyze.py#L366).
@@ -379,16 +380,17 @@
 due to resource (time and price) constraints. This explains why the #parsed is 648, otherwise it should be 2592.
 
 </details>
 
 <details>
   <summary><b>Tips for choosing evaluators</b></summary>
 
-Overall we recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest agreement with humans, and
-`annotators_config=claude` if you have academic (free) access to Claude and have a low budget.
+Overall we recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest agreement with humans,
+`annotators_config=claude` if you have academic (free) access to Claude and have a low budget, and
+`annotators_config=chatgpt_fn` if you don't have access to the other two models.
 
 When choosing an annotator we recommend you to consider the following (the first three are obvious):
 
 - `"Human agreement [%]"`
 - `"Price [$/1000 examples]"`
 - `"Time [seconds/1000 examples]"`
 - `"Proba. prefer longer"` approx. < 0.7. Indeed, we found see that the majority of preference of human annotators have
@@ -453,15 +455,15 @@
 
 [//]: # ()
 
 [//]: # (4. test your installation &#40;assuming you have OpenAI)
 
 [//]: # ()
 
-[//]: # (   key&#41; `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config 'text_davinci_003' --max_instances 3 --caching_path None`)
+[//]: # (   key&#41; `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config 'text_davinci_003' ~~--max_instances 3~~ --caching_path None`)
 
 [//]: # ()
 
 [//]: # (</details>)
 
 ## Evaluating a model
 
@@ -535,15 +537,15 @@
 rn a dictionary of metrics and the key by which to sort the leaderboard.
     -s, --sort_by=SORT_BY
         Type: str
         Default: 'win_rate'
         The key by which to sort the leaderboard.
     --is_cache_leaderboard=IS_CACHE_LEADERBOARD
         Type: Optional
-        Default: False
+        Default: None
         Whether to save the result leaderboard to `precomputed_leaderboard`. If None we save only if max_instances
 . A preferred way of adding models to the leaderboard is to set `precomputed_leaderboard` to the previously saved
 leaderboard at `<output_path>/leaderboard.csv`.
     --max_instances=MAX_INSTANCES
         Type: Optional[Optional]
         Default: None
         The maximum number of instances to annotate. Useful for testing.
@@ -630,15 +632,16 @@
 
 2. Compute the reference outputs `reference_outputs`. By default, we use the outputs of `text-davinci-003` on
    AlpacaEval.
    If you
    want to use a different model or a different dataset follow the same steps as (1.).
 3. Choose an evaluator specified via `annotators_config`. We recommend using `alpaca_eval_gpt4` or `claude` (if you are
    an
-   academic). For options and comparisons see [this table](#evaluators). Depending on the evaluator you might need to
+   academic) or `chatgpt_fn` (if you don't have access to the other two). For options and comparisons
+   see [this table](#evaluators). Depending on the evaluator you might need to
    set the appropriate API_KEY in your environment
    or [here](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/constants.py#L7).
 
 Running all together:
 
 ```bash
 alpaca_eval --model_outputs 'example/outputs.json' \
@@ -1002,53 +1005,58 @@
 colab notebook above.
 
 # Contributing
 
 We are accepting PRs for new models, evaluators, and eval sets, in addition to bug fixes.
 We will update the [leaderboard website](https://tatsu-lab.github.io/alpaca_eval/) regularly with new community
 contributions.
-We have also created a [support discord](https://discord.gg/qVYd69ye) for AlpacaEval in case you run into any issues and
+We have also created a [support discord](https://discord.gg/GJMxJSVZZM) for AlpacaEval in case you run into any issues
+and
 wish to ask help from the community.
 
+To get started, please first fork the repo, and install the package from source `pip install -e .`
+
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing a model</h2></summary>
 
 First, you'll need to add a model config definition in the [models_configs](src/alpaca_eval/models_configs/) folder. As
 an example, you can look at
 the [falcon-7b-instruct yaml](src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml). Please make sure the
 folder name and key name in the yaml match exactly.
 
-Then, please follow the steps in [Evaluating-a-model](#evaluating-a-model) to run inference on the model to produce
+Then, please follow the steps in [Evaluating a model](#evaluating-a-model) to run inference on the model to produce
 outputs on the eval set and score the model according to one of the evaluators.
 An example command may look like:
 
 ```sh
 alpaca_eval evaluate_from_model \
   --model_configs 'falcon-7b-instruct' \
-  --annotators_config 'alpaca_eval_gpt4'
+  --annotators_config 'alpaca_eval_gpt4' 
 ```
 
-After running this command, you should have generated an outputs json and a new entry in the corresponding leaderboard
-file. Please make a PR with the config, outputs file, and updated leaderboard.
+After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
+file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
+with the
+config, outputs file, and updated leaderboard.
 
 </details>
 
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing an evaluator</h2></summary>
 
 Please first follow the directions in [Making a new evaluator](#making-a-new-evaluator).
 Once you're created the annotator config, we ask that you create a new leaderboard for the annotator by evaluating the
 minimal set of models. The outputs for these models can be found by
 downloading [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/main/alpaca_eval_all_outputs.json).
 
 ```bash
 alpaca_eval make_leaderboard \
-  --leaderboard_path <src/alpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \
+  --leaderboard_path src/alpaca_eval/leaderboards/data_AlpacaEval/<evaluator>_leaderboard.csv \
   --all_model_outputs alpaca_eval_all_outputs.json \
-  --annotators_config <path_to_your_config.yaml>
+  --annotators_config <evaluator_config>
 ```
 
 Then, please create a PR with the annotator config and leaderboard csv.
 
 </details>
 
 <details>
@@ -1263,7 +1271,19 @@
   a position bias.
 - [AlpacaFarm Sec. 5.2.](https://arxiv.org/abs/2305.14387)
   and [The False Promise of Imitating Proprietary LLMs](https://arxiv.org/abs/2305.15717) both found that
   automatic
   annotators favor style (e.g. use of list, tone, word choice, length) over factuality.
 
 </details>
+
+
+<details>
+  <summary><h2 tabindex="-1" dir="auto">Major updates</h2></summary>
+
+- 19th June 2023: add leaderboard `chatgpt_fn` that anyone can use (no waiting lists).
+- 19th June 2023: update to
+  use [OpenAI's function calling](https://openai.com/blog/function-calling-and-other-api-updates).
+  Example: [`chatgpt_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/chatgpt_fn)
+  or [`alpaca_eval_gpt4_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn).
+
+</details>
```

#### html2text {}

```diff
@@ -1,39 +1,29 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.1.3 Summary: AlpacaEval : An
-Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Education Classifier: Intended Audience :: Science/Research Classifier: License
-:: OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: analysis Provides-Extra: dev Provides-Extra: local Provides-
-Extra: api Provides-Extra: all License-File: LICENSE # [https://
-raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png]
-AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
-[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
-License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
-[Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
-www.python.org/downloads/release/python-3100/) [![discord](https://
-img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
-/discord.gg/yKbbQga9WE) Evaluation of instruction-following models (e.g.,
-ChatGPT) typically requires human interactions. This is time-consuming,
-expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
-evaluation that is fast, cheap, replicable, and validated against 20K human
-annotations. It is particularly useful for model development. Although we
-improved over prior automatic evaluation pipelines, there are still fundamental
-[limitations](#limitations). AlpacaEval provides the following: - [**Automatic
-evaluator**](#evaluators): an automatic evaluator that has high agreement with
-humans (validated on 20K annotations). We evaluate a model by measuring the
-fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs
-from that model over outputs from a reference model. Our evaluators enable
-caching and output randomization by default. - [**Leaderboard**](https://tatsu-
+# [https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/
+AlpacaFarm_small.png] AlpacaEval : An Automatic Evaluator for Instruction-
+following Language Models [![Code License](https://img.shields.io/badge/
+Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/
+blob/main/LICENSE) [![Data License](https://img.shields.io/badge/
+Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/
+alpaca_farm/blob/main/DATA_LICENSE) [![Python 3.10+](https://img.shields.io/
+badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-
+3100/) [![discord](https://img.shields.io/badge/discord-server-
+blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM) Evaluation
+of instruction-following models (e.g., ChatGPT) typically requires human
+interactions. This is time-consuming, expensive, and hard to replicate.
+AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
+replicable, and validated against 20K human annotations. It is particularly
+useful for model development. Although we improved over prior automatic
+evaluation pipelines, there are still fundamental [limitations](#limitations).
+AlpacaEval provides the following: - [**Automatic evaluator**](#evaluators): an
+automatic evaluator that has high agreement with humans (validated on 20K
+annotations). We evaluate a model by measuring the fraction of times an
+powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that
+model over outputs from a reference model. Our evaluators enable caching and
+output randomization by default. - [**Leaderboard**](https://tatsu-
 lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
 evaluation set. - [**Toolkit for building automatic evaluators**](#analysis): a
 simple interface for building advanced automatic evaluators (e.g. with caching,
 batching, or multi-annotators) and analyzing them (quality, price, speed,
 statistical power, bias, variance etc). - [**Human evaluation data**](#data-
 release): 20K human preferences between a given and reference model on the
 [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
@@ -59,48 +49,51 @@
 4. [Analysis](#additional-analysis-and-plots) - [Analyzing an evaluator]
 (#analyzing-an-evaluator) - [Analyzing an eval set](#analyzing-an-eval-set) 5.
 [Contributing](#contributing) - [Contributing a model](#contributing-a-model) -
 [Contributing an evaluator](#contributing-an-evaluator) - [Contributing an eval
 set](#contributing-an-eval-set) 6. [Limitations](#limitations) 7. [Citation]
 (#citation) 8. [Additional information](#additional-information) - [Data
 Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
-alpacafarm) - [Related work](#related-work)  # Quick Start To install the
-stable release, run ```bash pip install alpaca-eval ``` To install the nightly
-version, run ```bash pip install git+https://github.com/tatsu-lab/alpaca_eval
-``` Then you can use it as follows: ```bash export OPENAI_API_KEY= export
-OPENAI_ORGANIZATION_IDS= # Optional; if not set, this will be your default org
-id. alpaca_eval --model_outputs 'example/outputs.json' ``` Important parameters
-are the following: - **model_outputs** : A path to a json file for the outputs
-of the model to add to the leaderboard. Each dictionary should contain the keys
-`instruction` and `output`. - **annotators_config**: This is the annotator to
-use (e.g., `alpaca_eval_gpt4` or `claude`). `alpaca_eval_gpt4` ( default) has
-the highest agreement rate with our human annotation data. `claude` has a
-decent agreement and is free for academics. For a comparison of annotators see
-[here](#evaluators). - **reference_outputs**: The outputs of the reference
-model. Same format as `model_outputs`. By default, this is `text-davinci003`
-outputs on AlpacaEval dataset. - **output_path**: Path for saving annotations
-and leaderboard. If you don't have the model outputs, you can use
-[`evaluate_from_model`](https://github.com/tatsu-lab/alpaca_eval/tree/
-main#evaluating-a-model) and pass a local path or a name of a HuggingFace
-model, or a model from a standard API (OpenAI, Anthropic, Cohere). Other
-commands:  >>> alpaca_eval -- --help ``` SYNOPSIS alpaca_eval COMMAND COMMANDS
-COMMAND is one of the following: evaluate Evaluate a model based on its
-outputs. This is the default entrypoint if no command is specified.
-evaluate_from_model Evaluate a model from HuggingFace or an API provider. This
-is a wrapper around `evaluate` which includes generating from a desired model.
-make_leaderboard Precompute and save an entire leaderboard for a given dataset
-/ evaluator / set of models generations. analyze_evaluators Analyze an
-evaluator (agreement with human, speed, price,...). ```  For more information
-about each function use `alpaca_eval  -- --help`. # Leaderboards and how to
-interpret them ## Models Our leaderboards are computed on the [AlpacaEval
-dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval). We precomputed
-the leaderboard for important models both using `gpt4` (best quality) and
-`claude` (free for academics, and high quality). Our full leaderboards can be
-found at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but we give
-minimal leaderboards below. Later we also show how to [add your model](https://
+alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
+# Quick Start To install the stable release, run ```bash pip install alpaca-
+eval ``` To install the nightly version, run ```bash pip install git+https://
+github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
+export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
+this will be your default org id. alpaca_eval --model_outputs 'example/
+outputs.json' ``` Important parameters are the following: - **model_outputs** :
+A path to a json file for the outputs of the model to add to the leaderboard.
+Each dictionary should contain the keys `instruction` and `output`. -
+**annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4`
+or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default) has the highest
+agreement rate with our human annotation data. `claude` has a decent agreement
+and is free for academics. `chatgpt_fn` is the worst of the three, but is
+available to everyone, cheap, and has 2x larger context window (16K tokens).
+For a comparison of annotators see [here](#evaluators). -
+**reference_outputs**: The outputs of the reference model. Same format as
+`model_outputs`. By default, this is `text-davinci003` outputs on AlpacaEval
+dataset. - **output_path**: Path for saving annotations and leaderboard. If you
+don't have the model outputs, you can use [`evaluate_from_model`](https://
+github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and pass a local
+path or a name of a HuggingFace model, or a model from a standard API (OpenAI,
+Anthropic, Cohere). Other commands:  >>> alpaca_eval -- --help ``` SYNOPSIS
+alpaca_eval COMMAND COMMANDS COMMAND is one of the following: evaluate Evaluate
+a model based on its outputs. This is the default entrypoint if no command is
+specified. evaluate_from_model Evaluate a model from HuggingFace or an API
+provider. This is a wrapper around `evaluate` which includes generating from a
+desired model. make_leaderboard Precompute and save an entire leaderboard for a
+given dataset / evaluator / set of models generations. analyze_evaluators
+Analyze an evaluator (agreement with human, speed, price,...). ```  For more
+information about each function use `alpaca_eval  -- --help`. # Leaderboards
+and how to interpret them ## Models Our leaderboards are computed on the
+[AlpacaEval dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval). We
+precomputed the leaderboard for important models using `alpaca_eval_gpt4` (best
+quality), `claude` (free for academics, and high quality), and `chatgpt_fn`
+(cheap and available for everyone). Our full leaderboards can be found at [on
+this page](https://tatsu-lab.github.io/alpaca_eval/), but we give minimal
+leaderboards below. Later we also show how to [add your model](https://
 github.com/tatsu-lab/alpaca_eval#evaluating-a-model) to the leaderboard and how
 to make a [new leaderboard for your evaluator/dataset](https://github.com/
 tatsu-lab/alpaca_eval#making-a-new-leaderboard). See [here](https://github.com/
 tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) for the configs
 of all models that are available out of the box. **`alpaca_eval_gpt4` minimal
 leaderboard**: | | Win Rate | Std Error | |:----------------------|---------:|-
 ---------:| | gpt4 | 95.3 | 0.7 | | claude | 88.4 | 1.1 | | chatgpt | 86.1 |
@@ -144,40 +137,47 @@
 Aviary. We make changes to Aviary's prompt to decrease the bias for longer
 outputs. Details in [Related work](#related-work).   claude minimal leaderboard
 | | Win Rate | Std Error | |:----------------------|---------:|----------:| |
 gpt4 | 77.0 | 1.5 | | claude | 75.8 | 1.5 | | chatgpt | 67.7 | 1.6 | |
 wizardlm-13b | 66.1 | 1.7 | | vicuna-13b | 63.2 | 1.7 | | guanaco-65b | 62.6 |
 1.7 | | oasst-rlhf-llama-33b | 57.3 | 1.7 | | text_davinci_003 | 50.0 | 0.0 | |
 falcon-40b-instruct | 46.7 | 1.8 | | alpaca-farm-ppo-human | 46.5 | 1.8 | |
-alpaca-7b | 32.3 | 1.6 | | text_davinci_001 | 21.5 | 1.4 |  ## Evaluators We
+alpaca-7b | 32.3 | 1.6 | | text_davinci_001 | 21.5 | 1.4 |   chatgpt_fn minimal
+leaderboard | | Win Rate | Std Err. | |:----------------------|---------:|-----
+----:| | gpt4 | 73.8 | 1.5 | | claude | 70.4 | 1.6 | | chatgpt | 66.1 | 1.7 | |
+wizardlm-13b | 65.2 | 1.7 | | vicuna-13b | 64.1 | 1.7 | | guanaco-65b | 62.4 |
+1.7 | | oasst-rlhf-llama-33b | 62.0 | 1.7 | | alpaca-farm-ppo-human | 60.2 |
+1.7 | | falcon-40b-instruct | 56.5 | 1.7 | | text_davinci_003 | 50.0 | 0.0 | |
+alpaca-7b | 45.2 | 1.7 | | text_davinci_001 | 28.1 | 1.6 |  ## Evaluators We
 evaluate different automatic annotators on the AlpacaEval set by comparing to
 2.5K [human annotations](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/
 blob/main/alpaca_farm_human_crossannotations.json) we collected (~650
 instructions each with 4 human annotations). Below we show metrics for our
 suggested evaluator (`alpaca_eval_gpt4`), for prior automatic evaluators (
 [`alpaca_farm_greedy_gpt4`](https://github.com/tatsu-lab/alpaca_farm),
 [`aviary_gpt4`](https://aviary.anyscale.com/),[`lmsys_gpt4`](https://
 chat.lmsys.org/)), for humans (`humans`), and for different base models with
-essentially the same prompt (`gpt4`,`claude`,`text_davinci_003`,`guanaco_33b`,
-`chatgpt`). See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/
-alpaca_eval/evaluators_configs) for the configs of all evaluators that are
-available out of the box and their associated metrics. | | Human agreement [%]
-| Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance |
-Proba. prefer longer | |:------------------------|--------------------:|-------
------------------:|-----------------------------:|-----:|---------:|-----------
-----------:| | alpaca_eval_gpt4 | 69.2 | 13.6 | 1455 | 28.4 | 14.6 | 0.68 | |
-aviary_gpt4 | 69.1 | 12.8 | 1869 | 29.5 | 13.1 | 0.70 | | gpt4 | 66.9 | 12.5 |
-1037 | 31.5 | 14.6 | 0.65 | | alpaca_farm_greedy_gpt4 | 66.4 | 15.3 | 878 |
-30.2 | 19.3 | 0.60 | | humans | 65.7 | 300.0 | 36800 | 0.0 | | 0.64 | | claude
-| 65.5 | 11.1 | 173 | 31.9 | 18.0 | 0.62 | | text_davinci_003 | 64.1 | 8.7 |
-121 | 33.8 | 22.7 | 0.70 | | lmsys_gpt4 | 63.2 | 13.9 | 17982 | 34.7 | 16.1 |
-0.74 | | guanaco_33b | 59.1 | | 930 | 54.5 | 27.1 | 0.70 | | chatgpt | 57.2 |
-0.8 | 285 | 39.4 | 34.1 | 0.59 |  How exactly are those metrics computed? We
-now explain in words how we compute the metrics in the table above. [The code
-is here](https://github.com/tatsu-lab/alpaca_eval/blob/
+essentially the same prompt
+(`gpt4`,`claude`,`text_davinci_003`,`chatgpt_fn`,`guanaco_33b`, `chatgpt`). See
+[here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/
+evaluators_configs) for the configs of all evaluators that are available out of
+the box and their associated metrics. | | Human agreement [%] | Price [$/1000
+examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer
+longer | |:------------------------|--------------------:|---------------------
+---:|-----------------------------:|-----:|---------:|---------------------:| |
+alpaca_eval_gpt4 | 69.2 | 13.6 | 1455 | 28.4 | 14.6 | 0.68 | | aviary_gpt4 |
+69.1 | 12.8 | 1869 | 29.5 | 13.1 | 0.70 | | gpt4 | 66.9 | 12.5 | 1037 | 31.5 |
+14.6 | 0.65 | | alpaca_farm_greedy_gpt4 | 66.4 | 15.3 | 878 | 30.2 | 19.3 |
+0.60 | | humans | 65.7 | 300.0 | 36800 | 0.0 | 34.3 | 0.64 | | claude | 65.5 |
+11.1 | 173 | 31.9 | 18.0 | 0.62 | | text_davinci_003 | 64.1 | 8.7 | 121 | 33.8
+| 22.7 | 0.70 | | lmsys_gpt4 | 63.2 | 13.9 | 17982 | 34.7 | 16.1 | 0.74 | |
+chatgpt_fn | 60.0 | 1.0 | 530 | 36.9 | 27.7 | 0.62 | | chatgpt | 57.2 | 0.8 |
+285 | 39.4 | 34.1 | 0.59 |  How exactly are those metrics computed? We now
+explain in words how we compute the metrics in the table above. [The code is
+here](https://github.com/tatsu-lab/alpaca_eval/blob/
 f05cbd651b79ac93906b19d01fe443b45828b0f2/src/alpaca_eval/analyze.py#L366).
 **Human agreement [%]**: this measures the agreement between the current
 annotator and the majority preferences of humans on our ~650 annotations from
 our [cross-annotation set](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_farm_human_crossannotations.json), which contains
 4 human annotations per example. To estimate the agreement between a single
 human (`humans` row in the table above) and the majority of humans, we take one
@@ -240,16 +240,17 @@
 outputs in the prompt, so this should be 0.5. Prior annotators, such as `lmsys`
 and `aviary`, do not. **# parsed**: this is the number of examples that the
 annotator was able to parse. Note that if the variance and bias is empty, it
 means that we only performed one single annotation for each 648 example due to
 resource (time and price) constraints. This explains why the #parsed is 648,
 otherwise it should be 2592.   Tips for choosing evaluators Overall we
 recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest
-agreement with humans, and `annotators_config=claude` if you have academic
-(free) access to Claude and have a low budget. When choosing an annotator we
+agreement with humans, `annotators_config=claude` if you have academic (free)
+access to Claude and have a low budget, and `annotators_config=chatgpt_fn` if
+you don't have access to the other two models. When choosing an annotator we
 recommend you to consider the following (the first three are obvious): -
 `"Human agreement [%]"` - `"Price [$/1000 examples]"` - `"Time [seconds/1000
 examples]"` - `"Proba. prefer longer"` approx. < 0.7. Indeed, we found see that
 the majority of preference of human annotators have strong bias for longer
 answers (as shown by the high [performance=62.2](https://github.com/tatsu-lab/
 alpaca_eval/blob/main/src/alpaca_eval/evaluators_configs/README.md) of the
 `"longest"` evaluator that always prefers the longest output). This suggests
@@ -274,16 +275,16 @@
 it might be easier to install `alpaca_eval` from source.) [//]: # (If so follow
 the following steps:) [//]: # () [//]: # (1. clone the repository) [//]: # ()
 [//]: # (2. install as dev the package: `pip install -e .`) [//]: # () [//]: #
 (3. (optional) export) [//]: # () [//]: # ( all [API_KEYs](https://github.com/
 tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/constants.py#L7)) [//]: # () [/
 /]: # (4. test your installation (assuming you have OpenAI) [//]: # () [//]: #
 ( key) `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config
-'text_davinci_003' --max_instances 3 --caching_path None`) [//]: # () [//]: #
-() ## Evaluating a model  >>> alpaca_eval evaluate -- --help ``` NAME
+'text_davinci_003' ~~--max_instances 3~~ --caching_path None`) [//]: # () [//]:
+# () ## Evaluating a model  >>> alpaca_eval evaluate -- --help ``` NAME
 alpaca_eval evaluate - Evaluate a model based on its outputs. This is the
 default entrypoint if no command is specified. SYNOPSIS alpaca_eval evaluate
 DESCRIPTION Evaluate a model based on its outputs. This is the default
 entrypoint if no command is specified. FLAGS --model_outputs=MODEL_OUTPUTS
 Type: Optional[Union] Default: None The outputs of the model to add to the
 leaderboard. Accepts data (list of dictionary, pd.dataframe, datasets.Dataset)
 or a path to read those (json, csv, tsv) or a function to generate those. Each
@@ -319,15 +320,15 @@
 Whether to return the metrics instead of printing the results. -f, --
 fn_metric=FN_METRIC Type: Union Default: 'pairwise_to_winrate' The function or
 function name in `metrics.py` that will be used to convert preference to
 metrics. The func tion should take a sequence of preferences (0 for draw, 1 for
 base win, 2 when the model to compare wins) and retu rn a dictionary of metrics
 and the key by which to sort the leaderboard. -s, --sort_by=SORT_BY Type: str
 Default: 'win_rate' The key by which to sort the leaderboard. --
-is_cache_leaderboard=IS_CACHE_LEADERBOARD Type: Optional Default: False Whether
+is_cache_leaderboard=IS_CACHE_LEADERBOARD Type: Optional Default: None Whether
 to save the result leaderboard to `precomputed_leaderboard`. If None we save
 only if max_instances . A preferred way of adding models to the leaderboard is
 to set `precomputed_leaderboard` to the previously saved leaderboard at `/
 leaderboard.csv`. --max_instances=MAX_INSTANCES Type: Optional[Optional]
 Default: None The maximum number of instances to annotate. Useful for testing.
 --annotation_kwargs=ANNOTATION_KWARGS Type: Optional[Optional] Default: None
 Additional arguments to pass to `PairwiseAnnotator.annotate_head2head`.
@@ -367,20 +368,21 @@
 your model is a HuggingFace model or from a standard API provider (OpenAI,
 Anthropic, Cohere). Then you can directly use `alpaca_eval evaluate_from_model`
 to also take care of generating outputs. 2. Compute the reference outputs
 `reference_outputs`. By default, we use the outputs of `text-davinci-003` on
 AlpacaEval. If you want to use a different model or a different dataset follow
 the same steps as (1.). 3. Choose an evaluator specified via
 `annotators_config`. We recommend using `alpaca_eval_gpt4` or `claude` (if you
-are an academic). For options and comparisons see [this table](#evaluators).
-Depending on the evaluator you might need to set the appropriate API_KEY in
-your environment or [here](https://github.com/tatsu-lab/alpaca_eval/blob/main/
-src/alpaca_eval/constants.py#L7). Running all together: ```bash alpaca_eval --
-model_outputs 'example/outputs.json' \ --annotators_config 'alpaca_eval_gpt4' \
---reference_outputs  ``` If you don't have decoded outputs, you can use
+are an academic) or `chatgpt_fn` (if you don't have access to the other two).
+For options and comparisons see [this table](#evaluators). Depending on the
+evaluator you might need to set the appropriate API_KEY in your environment or
+[here](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/
+constants.py#L7). Running all together: ```bash alpaca_eval --model_outputs
+'example/outputs.json' \ --annotators_config 'alpaca_eval_gpt4' \ --
+reference_outputs  ``` If you don't have decoded outputs, you can use
 `evaluate_from_model` which takes care of decoding (model and reference) for
 you. Here's an example: ```bash # need a GPU for local models export
 ANTHROPIC_API_KEY= # let's annotate with claude alpaca_eval evaluate_from_model
 \ --model_configs 'oasst_pythia_12b' \ --annotators_config 'claude' \ --
 reference_model_configs  ``` Here the `model_configs` and
 `reference_model_configs` (optional) are paths to a directory that specifies
 the prompt, the model provider (here HuggingFace) and decoding parameters. See
@@ -586,41 +588,43 @@
 one could remove this dataset from the evaluation set. The exact reason should
 be analyzed in future work. For the code and more analysis see [this notebook]
 (https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/
 analyzing_evalset.ipynb), or the colab notebook above. # Contributing We are
 accepting PRs for new models, evaluators, and eval sets, in addition to bug
 fixes. We will update the [leaderboard website](https://tatsu-lab.github.io/
 alpaca_eval/) regularly with new community contributions. We have also created
-a [support discord](https://discord.gg/qVYd69ye) for AlpacaEval in case you run
-into any issues and wish to ask help from the community.
+a [support discord](https://discord.gg/GJMxJSVZZM) for AlpacaEval in case you
+run into any issues and wish to ask help from the community. To get started,
+please first fork the repo, and install the package from source `pip install -
+e .`
 ***** Contributing a model *****
 First, you'll need to add a model config definition in the [models_configs]
 (src/alpaca_eval/models_configs/) folder. As an example, you can look at the
 [falcon-7b-instruct yaml](src/alpaca_eval/models_configs/falcon-7b-instruct/
 configs.yaml). Please make sure the folder name and key name in the yaml match
-exactly. Then, please follow the steps in [Evaluating-a-model](#evaluating-a-
+exactly. Then, please follow the steps in [Evaluating a model](#evaluating-a-
 model) to run inference on the model to produce outputs on the eval set and
 score the model according to one of the evaluators. An example command may look
 like: ```sh alpaca_eval evaluate_from_model \ --model_configs 'falcon-7b-
 instruct' \ --annotators_config 'alpaca_eval_gpt4' ``` After running this
 command, you should have generated an outputs json and a new entry in the
-corresponding leaderboard file. Please make a PR with the config, outputs file,
-and updated leaderboard.
+corresponding [leaderboard file](https://github.com/tatsu-lab/alpaca_eval/tree/
+main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR with the
+config, outputs file, and updated leaderboard.
 ***** Contributing an evaluator *****
 Please first follow the directions in [Making a new evaluator](#making-a-new-
 evaluator). Once you're created the annotator config, we ask that you create a
 new leaderboard for the annotator by evaluating the minimal set of models. The
 outputs for these models can be found by downloading
 [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_eval_all_outputs.json). ```bash alpaca_eval
-make_leaderboard \ --leaderboard_path
-lpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \ --
-all_model_outputs alpaca_eval_all_outputs.json \ --annotators_config
-yaml> ``` Then, please create a PR with the annotator config and leaderboard
-csv.
+make_leaderboard \ --leaderboard_path src/alpaca_eval/leaderboards/
+data_AlpacaEval/_leaderboard.csv \ --all_model_outputs
+alpaca_eval_all_outputs.json \ --annotators_config  ``` Then, please create a
+PR with the annotator config and leaderboard csv.
 ***** Contributing an eval set *****
 To contribute a new eval set, you'll first need to specify a set of textual
 instructions. Then, you'll need to specify a set of reference outputs (model
 win-rates are computed against this reference). For ease of use, you may use
 the default [text-davinci-003](src/alpaca_eval/models_configs/text_davinci_003/
 ) reference config. Place these together into a json, where each entry
 specifies the fields `instruction`, `output`, and `generator`. You can look to
@@ -788,7 +792,15 @@
 evaluators. For example: - [AlpacaFarm Appx C](https://arxiv.org/abs/
 2305.14387) and [Large Language Models are not Fair Evaluators](https://
 arxiv.org/abs/2305.17926v1) both found that automatic annotators have a
 position bias. - [AlpacaFarm Sec. 5.2.](https://arxiv.org/abs/2305.14387) and
 [The False Promise of Imitating Proprietary LLMs](https://arxiv.org/abs/
 2305.15717) both found that automatic annotators favor style (e.g. use of list,
 tone, word choice, length) over factuality.
+***** Major updates *****
+- 19th June 2023: add leaderboard `chatgpt_fn` that anyone can use (no waiting
+lists). - 19th June 2023: update to use [OpenAI's function calling](https://
+openai.com/blog/function-calling-and-other-api-updates). Example:
+[`chatgpt_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/
+alpaca_eval/evaluators_configs/chatgpt_fn) or [`alpaca_eval_gpt4_fn`](https://
+github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/
+alpaca_eval_gpt4_fn).
```

### Comparing `alpaca_eval-0.1.3/README.md` & `alpaca_eval-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,49 @@
+Metadata-Version: 2.1
+Name: alpaca_eval
+Version: 0.1.5
+Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
+Author: The Alpaca Team
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: analysis
+Provides-Extra: dev
+Provides-Extra: local
+Provides-Extra: api
+Provides-Extra: all
+License-File: LICENSE
+
 # <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
 [![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
-[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE)
+[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
 Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
 AlpacaEval provides the following:
 
 - [**Automatic evaluator**](#evaluators): an automatic evaluator that has high agreement with humans (validated on 20K
   annotations). We evaluate a
   model by
-  measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs from that model over
+  measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that model
+  over
   outputs from a reference model. Our evaluators enable caching and output randomization by default.
 - [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
   evaluation set.
 - [**Toolkit for building automatic evaluators**](#analysis): a simple interface for
   building advanced automatic evaluators (e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
   price, speed, statistical power, bias, variance etc).
 - [**Human evaluation data**](#data-release): 20K human preferences between a given and reference model
@@ -63,14 +87,15 @@
     - [Contributing an eval set](#contributing-an-eval-set)
 6. [Limitations](#limitations)
 7. [Citation](#citation)
 8. [Additional information](#additional-information)
     - [Data Release](#data-release)
     - [Differences with AlpacaFarm](#differences-with-alpacafarm)
     - [Related work](#related-work)
+    - [Major updates](#major-updates)
 
 </details>
 
 # Quick Start
 
 To install the stable release, run
 
@@ -93,19 +118,20 @@
 ```
 
 Important parameters are the following:
 
 - **model_outputs** : A path to a json file for the outputs of the model to add to the leaderboard. Each dictionary
   should
   contain the keys `instruction` and `output`.
-- **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`). `alpaca_eval_gpt4` (
+- **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`
+  or `chatgpt_fn`). `alpaca_eval_gpt4` (
   default) has the
-  highest agreement rate with our human annotation data. `claude` has a decent agreement and is free for academics. For
-  a comparison of
-  annotators see [here](#evaluators).
+  highest agreement rate with our human annotation data. `claude` has a decent agreement and is free for
+  academics. `chatgpt_fn` is the worst of the three, but is available to everyone, cheap, and has 2x larger context
+  window (16K tokens). For a comparison of annotators see [here](#evaluators).
 - **reference_outputs**:  The outputs of the reference model. Same format as `model_outputs`. By default, this
   is `text-davinci003` outputs on
   AlpacaEval dataset.
 - **output_path**: Path for saving annotations and leaderboard.
 
 If you don't have the model outputs, you can
 use [`evaluate_from_model`](https://github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and
@@ -141,16 +167,17 @@
 For more information about each function use `alpaca_eval <command> -- --help`.
 
 # Leaderboards and how to interpret them
 
 ## Models
 
 Our leaderboards are computed on the [AlpacaEval dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval).
-We precomputed the leaderboard for important models both using `gpt4` (best quality) and  `claude` (free for academics,
-and high quality). Our full leaderboards can be found at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but
+We precomputed the leaderboard for important models using `alpaca_eval_gpt4` (best quality),  `claude` (free for
+academics, and high quality), and `chatgpt_fn` (cheap and available for everyone). Our full leaderboards can be found
+at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but
 we give minimal leaderboards below.
 Later we also show how to [add your model](https://github.com/tatsu-lab/alpaca_eval#evaluating-a-model) to the
 leaderboard and how to make
 a [new leaderboard for your evaluator/dataset](https://github.com/tatsu-lab/alpaca_eval#making-a-new-leaderboard).
 See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) for the configs of all
 models that are available out of the box.
 
@@ -237,38 +264,58 @@
 | falcon-40b-instruct   |     46.7 |       1.8 |
 | alpaca-farm-ppo-human |     46.5 |       1.8 |
 | alpaca-7b             |     32.3 |       1.6 |
 | text_davinci_001      |     21.5 |       1.4 |
 
 </details>
 
+<details>
+  <summary><b><code>chatgpt_fn</code> minimal leaderboard</b></summary>
+
+|                       | Win Rate | Std Err. |
+|:----------------------|---------:|---------:|
+| gpt4                  |     73.8 |      1.5 |
+| claude                |     70.4 |      1.6 |
+| chatgpt               |     66.1 |      1.7 |
+| wizardlm-13b          |     65.2 |      1.7 |
+| vicuna-13b            |     64.1 |      1.7 |
+| guanaco-65b           |     62.4 |      1.7 |
+| oasst-rlhf-llama-33b  |     62.0 |      1.7 |
+| alpaca-farm-ppo-human |     60.2 |      1.7 |
+| falcon-40b-instruct   |     56.5 |      1.7 |
+| text_davinci_003      |     50.0 |      0.0 |
+| alpaca-7b             |     45.2 |      1.7 |
+| text_davinci_001      |     28.1 |      1.6 |
+
+</details>
+
 ## Evaluators
 
 We evaluate different automatic annotators on the AlpacaEval set by comparing to
 2.5K [human annotations](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/main/alpaca_farm_human_crossannotations.json)
 we collected (~650 instructions each with 4 human annotations).
 Below we show metrics for our suggested evaluator (`alpaca_eval_gpt4`), for prior
 automatic
 evaluators ([`alpaca_farm_greedy_gpt4`](https://github.com/tatsu-lab/alpaca_farm),[`aviary_gpt4`](https://aviary.anyscale.com/),[`lmsys_gpt4`](https://chat.lmsys.org/)),
 for humans (`humans`), and for different base models with essentially the same
-prompt (`gpt4`,`claude`,`text_davinci_003`,`guanaco_33b`, `chatgpt`).
+prompt (`gpt4`,`claude`,`text_davinci_003`,`chatgpt_fn`,`guanaco_33b`, `chatgpt`).
 See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs) for the configs of all
 evaluators that are available out of the box and their associated metrics.
 
 |                         | Human agreement [%] | Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer longer |
 |:------------------------|--------------------:|------------------------:|-----------------------------:|-----:|---------:|---------------------:|
 | alpaca_eval_gpt4        |                69.2 |                    13.6 |                         1455 | 28.4 |     14.6 |                 0.68 |
 | aviary_gpt4             |                69.1 |                    12.8 |                         1869 | 29.5 |     13.1 |                 0.70 |
 | gpt4                    |                66.9 |                    12.5 |                         1037 | 31.5 |     14.6 |                 0.65 |
 | alpaca_farm_greedy_gpt4 |                66.4 |                    15.3 |                          878 | 30.2 |     19.3 |                 0.60 |
-| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |          |                 0.64 |
+| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |     34.3 |                 0.64 |
 | claude                  |                65.5 |                    11.1 |                          173 | 31.9 |     18.0 |                 0.62 |
 | text_davinci_003        |                64.1 |                     8.7 |                          121 | 33.8 |     22.7 |                 0.70 |
 | lmsys_gpt4              |                63.2 |                    13.9 |                        17982 | 34.7 |     16.1 |                 0.74 |
-| guanaco_33b             |                59.1 |                         |                          930 | 54.5 |     27.1 |                 0.70 |
+| chatgpt_fn              |                60.0 |                     1.0 |                          530 | 36.9 |     27.7 |                 0.62 |
 | chatgpt                 |                57.2 |                     0.8 |                          285 | 39.4 |     34.1 |                 0.59 |
 
 <details>
   <summary><b>How exactly are those metrics computed?</b></summary>
 
 We now explain in words how we compute the metrics in the table
 above. [The code is here](https://github.com/tatsu-lab/alpaca_eval/blob/f05cbd651b79ac93906b19d01fe443b45828b0f2/src/alpaca_eval/analyze.py#L366).
@@ -356,16 +403,17 @@
 due to resource (time and price) constraints. This explains why the #parsed is 648, otherwise it should be 2592.
 
 </details>
 
 <details>
   <summary><b>Tips for choosing evaluators</b></summary>
 
-Overall we recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest agreement with humans, and
-`annotators_config=claude` if you have academic (free) access to Claude and have a low budget.
+Overall we recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest agreement with humans,
+`annotators_config=claude` if you have academic (free) access to Claude and have a low budget, and
+`annotators_config=chatgpt_fn` if you don't have access to the other two models.
 
 When choosing an annotator we recommend you to consider the following (the first three are obvious):
 
 - `"Human agreement [%]"`
 - `"Price [$/1000 examples]"`
 - `"Time [seconds/1000 examples]"`
 - `"Proba. prefer longer"` approx. < 0.7. Indeed, we found see that the majority of preference of human annotators have
@@ -430,15 +478,15 @@
 
 [//]: # ()
 
 [//]: # (4. test your installation &#40;assuming you have OpenAI)
 
 [//]: # ()
 
-[//]: # (   key&#41; `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config 'text_davinci_003' --max_instances 3 --caching_path None`)
+[//]: # (   key&#41; `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config 'text_davinci_003' ~~--max_instances 3~~ --caching_path None`)
 
 [//]: # ()
 
 [//]: # (</details>)
 
 ## Evaluating a model
 
@@ -512,15 +560,15 @@
 rn a dictionary of metrics and the key by which to sort the leaderboard.
     -s, --sort_by=SORT_BY
         Type: str
         Default: 'win_rate'
         The key by which to sort the leaderboard.
     --is_cache_leaderboard=IS_CACHE_LEADERBOARD
         Type: Optional
-        Default: False
+        Default: None
         Whether to save the result leaderboard to `precomputed_leaderboard`. If None we save only if max_instances
 . A preferred way of adding models to the leaderboard is to set `precomputed_leaderboard` to the previously saved
 leaderboard at `<output_path>/leaderboard.csv`.
     --max_instances=MAX_INSTANCES
         Type: Optional[Optional]
         Default: None
         The maximum number of instances to annotate. Useful for testing.
@@ -607,15 +655,16 @@
 
 2. Compute the reference outputs `reference_outputs`. By default, we use the outputs of `text-davinci-003` on
    AlpacaEval.
    If you
    want to use a different model or a different dataset follow the same steps as (1.).
 3. Choose an evaluator specified via `annotators_config`. We recommend using `alpaca_eval_gpt4` or `claude` (if you are
    an
-   academic). For options and comparisons see [this table](#evaluators). Depending on the evaluator you might need to
+   academic) or `chatgpt_fn` (if you don't have access to the other two). For options and comparisons
+   see [this table](#evaluators). Depending on the evaluator you might need to
    set the appropriate API_KEY in your environment
    or [here](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/constants.py#L7).
 
 Running all together:
 
 ```bash
 alpaca_eval --model_outputs 'example/outputs.json' \
@@ -979,53 +1028,58 @@
 colab notebook above.
 
 # Contributing
 
 We are accepting PRs for new models, evaluators, and eval sets, in addition to bug fixes.
 We will update the [leaderboard website](https://tatsu-lab.github.io/alpaca_eval/) regularly with new community
 contributions.
-We have also created a [support discord](https://discord.gg/qVYd69ye) for AlpacaEval in case you run into any issues and
+We have also created a [support discord](https://discord.gg/GJMxJSVZZM) for AlpacaEval in case you run into any issues
+and
 wish to ask help from the community.
 
+To get started, please first fork the repo, and install the package from source `pip install -e .`
+
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing a model</h2></summary>
 
 First, you'll need to add a model config definition in the [models_configs](src/alpaca_eval/models_configs/) folder. As
 an example, you can look at
 the [falcon-7b-instruct yaml](src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml). Please make sure the
 folder name and key name in the yaml match exactly.
 
-Then, please follow the steps in [Evaluating-a-model](#evaluating-a-model) to run inference on the model to produce
+Then, please follow the steps in [Evaluating a model](#evaluating-a-model) to run inference on the model to produce
 outputs on the eval set and score the model according to one of the evaluators.
 An example command may look like:
 
 ```sh
 alpaca_eval evaluate_from_model \
   --model_configs 'falcon-7b-instruct' \
-  --annotators_config 'alpaca_eval_gpt4'
+  --annotators_config 'alpaca_eval_gpt4' 
 ```
 
-After running this command, you should have generated an outputs json and a new entry in the corresponding leaderboard
-file. Please make a PR with the config, outputs file, and updated leaderboard.
+After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
+file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
+with the
+config, outputs file, and updated leaderboard.
 
 </details>
 
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing an evaluator</h2></summary>
 
 Please first follow the directions in [Making a new evaluator](#making-a-new-evaluator).
 Once you're created the annotator config, we ask that you create a new leaderboard for the annotator by evaluating the
 minimal set of models. The outputs for these models can be found by
 downloading [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/main/alpaca_eval_all_outputs.json).
 
 ```bash
 alpaca_eval make_leaderboard \
-  --leaderboard_path <src/alpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \
+  --leaderboard_path src/alpaca_eval/leaderboards/data_AlpacaEval/<evaluator>_leaderboard.csv \
   --all_model_outputs alpaca_eval_all_outputs.json \
-  --annotators_config <path_to_your_config.yaml>
+  --annotators_config <evaluator_config>
 ```
 
 Then, please create a PR with the annotator config and leaderboard csv.
 
 </details>
 
 <details>
@@ -1240,7 +1294,19 @@
   a position bias.
 - [AlpacaFarm Sec. 5.2.](https://arxiv.org/abs/2305.14387)
   and [The False Promise of Imitating Proprietary LLMs](https://arxiv.org/abs/2305.15717) both found that
   automatic
   annotators favor style (e.g. use of list, tone, word choice, length) over factuality.
 
 </details>
+
+
+<details>
+  <summary><h2 tabindex="-1" dir="auto">Major updates</h2></summary>
+
+- 19th June 2023: add leaderboard `chatgpt_fn` that anyone can use (no waiting lists).
+- 19th June 2023: update to
+  use [OpenAI's function calling](https://openai.com/blog/function-calling-and-other-api-updates).
+  Example: [`chatgpt_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/chatgpt_fn)
+  or [`alpaca_eval_gpt4_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn).
+
+</details>
```

#### html2text {}

```diff
@@ -1,41 +1,51 @@
-# [https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/
-AlpacaFarm_small.png] AlpacaEval : An Automatic Evaluator for Instruction-
-following Language Models [![Code License](https://img.shields.io/badge/
-Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/
-blob/main/LICENSE) [![Data License](https://img.shields.io/badge/
-Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/
-alpaca_farm/blob/main/DATA_LICENSE) [![Python 3.10+](https://img.shields.io/
-badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-
-3100/) [![discord](https://img.shields.io/badge/discord-server-
-blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE) Evaluation
-of instruction-following models (e.g., ChatGPT) typically requires human
-interactions. This is time-consuming, expensive, and hard to replicate.
-AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
-replicable, and validated against 20K human annotations. It is particularly
-useful for model development. Although we improved over prior automatic
-evaluation pipelines, there are still fundamental [limitations](#limitations).
-AlpacaEval provides the following: - [**Automatic evaluator**](#evaluators): an
-automatic evaluator that has high agreement with humans (validated on 20K
-annotations). We evaluate a model by measuring the fraction of times an
-powerful LLM (e.g. GPT 4 or Claude) prefers the outputs from that model over
-outputs from a reference model. Our evaluators enable caching and output
-randomization by default. - [**Leaderboard**](https://tatsu-lab.github.io/
-alpaca_eval/): a leaderboard of common models on the AlpacaEval evaluation set.
-- [**Toolkit for building automatic evaluators**](#analysis): a simple
-interface for building advanced automatic evaluators (e.g. with caching,
-batching, or multi-annotators) and analyzing them (quality, price, speed,
-statistical power, bias, variance etc). - [**Human evaluation data**](#data-
-release): 20K human preferences between a given and reference model on the
-[AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
-set. 2.5K of these are cross-annotations (4 humans annotating the same 650
-examples). - [**AlpacaEval dataset**](#data-release): a simplification of
-[AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
-set, where "instructions" and " inputs" are merged into one field, and
-reference outputs are longer. **When to use AlpacaEval?** Our automatic
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.1.5 Summary: AlpacaEval : An
+Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: Science/Research Classifier: License
+:: OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.10 Description-Content-Type: text/markdown
+Provides-Extra: analysis Provides-Extra: dev Provides-Extra: local Provides-
+Extra: api Provides-Extra: all License-File: LICENSE # [https://
+raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png]
+AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
+[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
+green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
+License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
+red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
+[Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
+www.python.org/downloads/release/python-3100/) [![discord](https://
+img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
+/discord.gg/GJMxJSVZZM) Evaluation of instruction-following models (e.g.,
+ChatGPT) typically requires human interactions. This is time-consuming,
+expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
+evaluation that is fast, cheap, replicable, and validated against 20K human
+annotations. It is particularly useful for model development. Although we
+improved over prior automatic evaluation pipelines, there are still fundamental
+[limitations](#limitations). AlpacaEval provides the following: - [**Automatic
+evaluator**](#evaluators): an automatic evaluator that has high agreement with
+humans (validated on 20K annotations). We evaluate a model by measuring the
+fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the
+outputs from that model over outputs from a reference model. Our evaluators
+enable caching and output randomization by default. - [**Leaderboard**](https:/
+/tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the
+AlpacaEval evaluation set. - [**Toolkit for building automatic evaluators**]
+(#analysis): a simple interface for building advanced automatic evaluators
+(e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
+price, speed, statistical power, bias, variance etc). - [**Human evaluation
+data**](#data-release): 20K human preferences between a given and reference
+model on the [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main)
+evaluation set. 2.5K of these are cross-annotations (4 humans annotating the
+same 650 examples). - [**AlpacaEval dataset**](#data-release): a simplification
+of [AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main)
+evaluation set, where "instructions" and " inputs" are merged into one field,
+and reference outputs are longer. **When to use AlpacaEval?** Our automatic
 evaluator is a quick and cheap proxy for human evaluation of simple
 instruction-following tasks. It is useful if you have to run many evaluations
 quickly, e.g., during model development. **When not to use AlpacaEval?** As any
 other automatic evaluator, AlpacaEval should **not replace human evaluation in
 high-stake decision-making**, e.g., to decide on model release. In particular,
 AlpacaEval is limited by the fact that (1) the instructions in the eval set
 might not be representative of advanced usage of LLMs; (2) automatic evaluators
@@ -49,48 +59,51 @@
 4. [Analysis](#additional-analysis-and-plots) - [Analyzing an evaluator]
 (#analyzing-an-evaluator) - [Analyzing an eval set](#analyzing-an-eval-set) 5.
 [Contributing](#contributing) - [Contributing a model](#contributing-a-model) -
 [Contributing an evaluator](#contributing-an-evaluator) - [Contributing an eval
 set](#contributing-an-eval-set) 6. [Limitations](#limitations) 7. [Citation]
 (#citation) 8. [Additional information](#additional-information) - [Data
 Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
-alpacafarm) - [Related work](#related-work)  # Quick Start To install the
-stable release, run ```bash pip install alpaca-eval ``` To install the nightly
-version, run ```bash pip install git+https://github.com/tatsu-lab/alpaca_eval
-``` Then you can use it as follows: ```bash export OPENAI_API_KEY= export
-OPENAI_ORGANIZATION_IDS= # Optional; if not set, this will be your default org
-id. alpaca_eval --model_outputs 'example/outputs.json' ``` Important parameters
-are the following: - **model_outputs** : A path to a json file for the outputs
-of the model to add to the leaderboard. Each dictionary should contain the keys
-`instruction` and `output`. - **annotators_config**: This is the annotator to
-use (e.g., `alpaca_eval_gpt4` or `claude`). `alpaca_eval_gpt4` ( default) has
-the highest agreement rate with our human annotation data. `claude` has a
-decent agreement and is free for academics. For a comparison of annotators see
-[here](#evaluators). - **reference_outputs**: The outputs of the reference
-model. Same format as `model_outputs`. By default, this is `text-davinci003`
-outputs on AlpacaEval dataset. - **output_path**: Path for saving annotations
-and leaderboard. If you don't have the model outputs, you can use
-[`evaluate_from_model`](https://github.com/tatsu-lab/alpaca_eval/tree/
-main#evaluating-a-model) and pass a local path or a name of a HuggingFace
-model, or a model from a standard API (OpenAI, Anthropic, Cohere). Other
-commands:  >>> alpaca_eval -- --help ``` SYNOPSIS alpaca_eval COMMAND COMMANDS
-COMMAND is one of the following: evaluate Evaluate a model based on its
-outputs. This is the default entrypoint if no command is specified.
-evaluate_from_model Evaluate a model from HuggingFace or an API provider. This
-is a wrapper around `evaluate` which includes generating from a desired model.
-make_leaderboard Precompute and save an entire leaderboard for a given dataset
-/ evaluator / set of models generations. analyze_evaluators Analyze an
-evaluator (agreement with human, speed, price,...). ```  For more information
-about each function use `alpaca_eval  -- --help`. # Leaderboards and how to
-interpret them ## Models Our leaderboards are computed on the [AlpacaEval
-dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval). We precomputed
-the leaderboard for important models both using `gpt4` (best quality) and
-`claude` (free for academics, and high quality). Our full leaderboards can be
-found at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but we give
-minimal leaderboards below. Later we also show how to [add your model](https://
+alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
+# Quick Start To install the stable release, run ```bash pip install alpaca-
+eval ``` To install the nightly version, run ```bash pip install git+https://
+github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
+export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
+this will be your default org id. alpaca_eval --model_outputs 'example/
+outputs.json' ``` Important parameters are the following: - **model_outputs** :
+A path to a json file for the outputs of the model to add to the leaderboard.
+Each dictionary should contain the keys `instruction` and `output`. -
+**annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4`
+or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default) has the highest
+agreement rate with our human annotation data. `claude` has a decent agreement
+and is free for academics. `chatgpt_fn` is the worst of the three, but is
+available to everyone, cheap, and has 2x larger context window (16K tokens).
+For a comparison of annotators see [here](#evaluators). -
+**reference_outputs**: The outputs of the reference model. Same format as
+`model_outputs`. By default, this is `text-davinci003` outputs on AlpacaEval
+dataset. - **output_path**: Path for saving annotations and leaderboard. If you
+don't have the model outputs, you can use [`evaluate_from_model`](https://
+github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and pass a local
+path or a name of a HuggingFace model, or a model from a standard API (OpenAI,
+Anthropic, Cohere). Other commands:  >>> alpaca_eval -- --help ``` SYNOPSIS
+alpaca_eval COMMAND COMMANDS COMMAND is one of the following: evaluate Evaluate
+a model based on its outputs. This is the default entrypoint if no command is
+specified. evaluate_from_model Evaluate a model from HuggingFace or an API
+provider. This is a wrapper around `evaluate` which includes generating from a
+desired model. make_leaderboard Precompute and save an entire leaderboard for a
+given dataset / evaluator / set of models generations. analyze_evaluators
+Analyze an evaluator (agreement with human, speed, price,...). ```  For more
+information about each function use `alpaca_eval  -- --help`. # Leaderboards
+and how to interpret them ## Models Our leaderboards are computed on the
+[AlpacaEval dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval). We
+precomputed the leaderboard for important models using `alpaca_eval_gpt4` (best
+quality), `claude` (free for academics, and high quality), and `chatgpt_fn`
+(cheap and available for everyone). Our full leaderboards can be found at [on
+this page](https://tatsu-lab.github.io/alpaca_eval/), but we give minimal
+leaderboards below. Later we also show how to [add your model](https://
 github.com/tatsu-lab/alpaca_eval#evaluating-a-model) to the leaderboard and how
 to make a [new leaderboard for your evaluator/dataset](https://github.com/
 tatsu-lab/alpaca_eval#making-a-new-leaderboard). See [here](https://github.com/
 tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) for the configs
 of all models that are available out of the box. **`alpaca_eval_gpt4` minimal
 leaderboard**: | | Win Rate | Std Error | |:----------------------|---------:|-
 ---------:| | gpt4 | 95.3 | 0.7 | | claude | 88.4 | 1.1 | | chatgpt | 86.1 |
@@ -134,40 +147,47 @@
 Aviary. We make changes to Aviary's prompt to decrease the bias for longer
 outputs. Details in [Related work](#related-work).   claude minimal leaderboard
 | | Win Rate | Std Error | |:----------------------|---------:|----------:| |
 gpt4 | 77.0 | 1.5 | | claude | 75.8 | 1.5 | | chatgpt | 67.7 | 1.6 | |
 wizardlm-13b | 66.1 | 1.7 | | vicuna-13b | 63.2 | 1.7 | | guanaco-65b | 62.6 |
 1.7 | | oasst-rlhf-llama-33b | 57.3 | 1.7 | | text_davinci_003 | 50.0 | 0.0 | |
 falcon-40b-instruct | 46.7 | 1.8 | | alpaca-farm-ppo-human | 46.5 | 1.8 | |
-alpaca-7b | 32.3 | 1.6 | | text_davinci_001 | 21.5 | 1.4 |  ## Evaluators We
+alpaca-7b | 32.3 | 1.6 | | text_davinci_001 | 21.5 | 1.4 |   chatgpt_fn minimal
+leaderboard | | Win Rate | Std Err. | |:----------------------|---------:|-----
+----:| | gpt4 | 73.8 | 1.5 | | claude | 70.4 | 1.6 | | chatgpt | 66.1 | 1.7 | |
+wizardlm-13b | 65.2 | 1.7 | | vicuna-13b | 64.1 | 1.7 | | guanaco-65b | 62.4 |
+1.7 | | oasst-rlhf-llama-33b | 62.0 | 1.7 | | alpaca-farm-ppo-human | 60.2 |
+1.7 | | falcon-40b-instruct | 56.5 | 1.7 | | text_davinci_003 | 50.0 | 0.0 | |
+alpaca-7b | 45.2 | 1.7 | | text_davinci_001 | 28.1 | 1.6 |  ## Evaluators We
 evaluate different automatic annotators on the AlpacaEval set by comparing to
 2.5K [human annotations](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/
 blob/main/alpaca_farm_human_crossannotations.json) we collected (~650
 instructions each with 4 human annotations). Below we show metrics for our
 suggested evaluator (`alpaca_eval_gpt4`), for prior automatic evaluators (
 [`alpaca_farm_greedy_gpt4`](https://github.com/tatsu-lab/alpaca_farm),
 [`aviary_gpt4`](https://aviary.anyscale.com/),[`lmsys_gpt4`](https://
 chat.lmsys.org/)), for humans (`humans`), and for different base models with
-essentially the same prompt (`gpt4`,`claude`,`text_davinci_003`,`guanaco_33b`,
-`chatgpt`). See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/
-alpaca_eval/evaluators_configs) for the configs of all evaluators that are
-available out of the box and their associated metrics. | | Human agreement [%]
-| Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance |
-Proba. prefer longer | |:------------------------|--------------------:|-------
------------------:|-----------------------------:|-----:|---------:|-----------
-----------:| | alpaca_eval_gpt4 | 69.2 | 13.6 | 1455 | 28.4 | 14.6 | 0.68 | |
-aviary_gpt4 | 69.1 | 12.8 | 1869 | 29.5 | 13.1 | 0.70 | | gpt4 | 66.9 | 12.5 |
-1037 | 31.5 | 14.6 | 0.65 | | alpaca_farm_greedy_gpt4 | 66.4 | 15.3 | 878 |
-30.2 | 19.3 | 0.60 | | humans | 65.7 | 300.0 | 36800 | 0.0 | | 0.64 | | claude
-| 65.5 | 11.1 | 173 | 31.9 | 18.0 | 0.62 | | text_davinci_003 | 64.1 | 8.7 |
-121 | 33.8 | 22.7 | 0.70 | | lmsys_gpt4 | 63.2 | 13.9 | 17982 | 34.7 | 16.1 |
-0.74 | | guanaco_33b | 59.1 | | 930 | 54.5 | 27.1 | 0.70 | | chatgpt | 57.2 |
-0.8 | 285 | 39.4 | 34.1 | 0.59 |  How exactly are those metrics computed? We
-now explain in words how we compute the metrics in the table above. [The code
-is here](https://github.com/tatsu-lab/alpaca_eval/blob/
+essentially the same prompt
+(`gpt4`,`claude`,`text_davinci_003`,`chatgpt_fn`,`guanaco_33b`, `chatgpt`). See
+[here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/
+evaluators_configs) for the configs of all evaluators that are available out of
+the box and their associated metrics. | | Human agreement [%] | Price [$/1000
+examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer
+longer | |:------------------------|--------------------:|---------------------
+---:|-----------------------------:|-----:|---------:|---------------------:| |
+alpaca_eval_gpt4 | 69.2 | 13.6 | 1455 | 28.4 | 14.6 | 0.68 | | aviary_gpt4 |
+69.1 | 12.8 | 1869 | 29.5 | 13.1 | 0.70 | | gpt4 | 66.9 | 12.5 | 1037 | 31.5 |
+14.6 | 0.65 | | alpaca_farm_greedy_gpt4 | 66.4 | 15.3 | 878 | 30.2 | 19.3 |
+0.60 | | humans | 65.7 | 300.0 | 36800 | 0.0 | 34.3 | 0.64 | | claude | 65.5 |
+11.1 | 173 | 31.9 | 18.0 | 0.62 | | text_davinci_003 | 64.1 | 8.7 | 121 | 33.8
+| 22.7 | 0.70 | | lmsys_gpt4 | 63.2 | 13.9 | 17982 | 34.7 | 16.1 | 0.74 | |
+chatgpt_fn | 60.0 | 1.0 | 530 | 36.9 | 27.7 | 0.62 | | chatgpt | 57.2 | 0.8 |
+285 | 39.4 | 34.1 | 0.59 |  How exactly are those metrics computed? We now
+explain in words how we compute the metrics in the table above. [The code is
+here](https://github.com/tatsu-lab/alpaca_eval/blob/
 f05cbd651b79ac93906b19d01fe443b45828b0f2/src/alpaca_eval/analyze.py#L366).
 **Human agreement [%]**: this measures the agreement between the current
 annotator and the majority preferences of humans on our ~650 annotations from
 our [cross-annotation set](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_farm_human_crossannotations.json), which contains
 4 human annotations per example. To estimate the agreement between a single
 human (`humans` row in the table above) and the majority of humans, we take one
@@ -230,16 +250,17 @@
 outputs in the prompt, so this should be 0.5. Prior annotators, such as `lmsys`
 and `aviary`, do not. **# parsed**: this is the number of examples that the
 annotator was able to parse. Note that if the variance and bias is empty, it
 means that we only performed one single annotation for each 648 example due to
 resource (time and price) constraints. This explains why the #parsed is 648,
 otherwise it should be 2592.   Tips for choosing evaluators Overall we
 recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest
-agreement with humans, and `annotators_config=claude` if you have academic
-(free) access to Claude and have a low budget. When choosing an annotator we
+agreement with humans, `annotators_config=claude` if you have academic (free)
+access to Claude and have a low budget, and `annotators_config=chatgpt_fn` if
+you don't have access to the other two models. When choosing an annotator we
 recommend you to consider the following (the first three are obvious): -
 `"Human agreement [%]"` - `"Price [$/1000 examples]"` - `"Time [seconds/1000
 examples]"` - `"Proba. prefer longer"` approx. < 0.7. Indeed, we found see that
 the majority of preference of human annotators have strong bias for longer
 answers (as shown by the high [performance=62.2](https://github.com/tatsu-lab/
 alpaca_eval/blob/main/src/alpaca_eval/evaluators_configs/README.md) of the
 `"longest"` evaluator that always prefers the longest output). This suggests
@@ -264,16 +285,16 @@
 it might be easier to install `alpaca_eval` from source.) [//]: # (If so follow
 the following steps:) [//]: # () [//]: # (1. clone the repository) [//]: # ()
 [//]: # (2. install as dev the package: `pip install -e .`) [//]: # () [//]: #
 (3. (optional) export) [//]: # () [//]: # ( all [API_KEYs](https://github.com/
 tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/constants.py#L7)) [//]: # () [/
 /]: # (4. test your installation (assuming you have OpenAI) [//]: # () [//]: #
 ( key) `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config
-'text_davinci_003' --max_instances 3 --caching_path None`) [//]: # () [//]: #
-() ## Evaluating a model  >>> alpaca_eval evaluate -- --help ``` NAME
+'text_davinci_003' ~~--max_instances 3~~ --caching_path None`) [//]: # () [//]:
+# () ## Evaluating a model  >>> alpaca_eval evaluate -- --help ``` NAME
 alpaca_eval evaluate - Evaluate a model based on its outputs. This is the
 default entrypoint if no command is specified. SYNOPSIS alpaca_eval evaluate
 DESCRIPTION Evaluate a model based on its outputs. This is the default
 entrypoint if no command is specified. FLAGS --model_outputs=MODEL_OUTPUTS
 Type: Optional[Union] Default: None The outputs of the model to add to the
 leaderboard. Accepts data (list of dictionary, pd.dataframe, datasets.Dataset)
 or a path to read those (json, csv, tsv) or a function to generate those. Each
@@ -309,15 +330,15 @@
 Whether to return the metrics instead of printing the results. -f, --
 fn_metric=FN_METRIC Type: Union Default: 'pairwise_to_winrate' The function or
 function name in `metrics.py` that will be used to convert preference to
 metrics. The func tion should take a sequence of preferences (0 for draw, 1 for
 base win, 2 when the model to compare wins) and retu rn a dictionary of metrics
 and the key by which to sort the leaderboard. -s, --sort_by=SORT_BY Type: str
 Default: 'win_rate' The key by which to sort the leaderboard. --
-is_cache_leaderboard=IS_CACHE_LEADERBOARD Type: Optional Default: False Whether
+is_cache_leaderboard=IS_CACHE_LEADERBOARD Type: Optional Default: None Whether
 to save the result leaderboard to `precomputed_leaderboard`. If None we save
 only if max_instances . A preferred way of adding models to the leaderboard is
 to set `precomputed_leaderboard` to the previously saved leaderboard at `/
 leaderboard.csv`. --max_instances=MAX_INSTANCES Type: Optional[Optional]
 Default: None The maximum number of instances to annotate. Useful for testing.
 --annotation_kwargs=ANNOTATION_KWARGS Type: Optional[Optional] Default: None
 Additional arguments to pass to `PairwiseAnnotator.annotate_head2head`.
@@ -357,20 +378,21 @@
 your model is a HuggingFace model or from a standard API provider (OpenAI,
 Anthropic, Cohere). Then you can directly use `alpaca_eval evaluate_from_model`
 to also take care of generating outputs. 2. Compute the reference outputs
 `reference_outputs`. By default, we use the outputs of `text-davinci-003` on
 AlpacaEval. If you want to use a different model or a different dataset follow
 the same steps as (1.). 3. Choose an evaluator specified via
 `annotators_config`. We recommend using `alpaca_eval_gpt4` or `claude` (if you
-are an academic). For options and comparisons see [this table](#evaluators).
-Depending on the evaluator you might need to set the appropriate API_KEY in
-your environment or [here](https://github.com/tatsu-lab/alpaca_eval/blob/main/
-src/alpaca_eval/constants.py#L7). Running all together: ```bash alpaca_eval --
-model_outputs 'example/outputs.json' \ --annotators_config 'alpaca_eval_gpt4' \
---reference_outputs  ``` If you don't have decoded outputs, you can use
+are an academic) or `chatgpt_fn` (if you don't have access to the other two).
+For options and comparisons see [this table](#evaluators). Depending on the
+evaluator you might need to set the appropriate API_KEY in your environment or
+[here](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/
+constants.py#L7). Running all together: ```bash alpaca_eval --model_outputs
+'example/outputs.json' \ --annotators_config 'alpaca_eval_gpt4' \ --
+reference_outputs  ``` If you don't have decoded outputs, you can use
 `evaluate_from_model` which takes care of decoding (model and reference) for
 you. Here's an example: ```bash # need a GPU for local models export
 ANTHROPIC_API_KEY= # let's annotate with claude alpaca_eval evaluate_from_model
 \ --model_configs 'oasst_pythia_12b' \ --annotators_config 'claude' \ --
 reference_model_configs  ``` Here the `model_configs` and
 `reference_model_configs` (optional) are paths to a directory that specifies
 the prompt, the model provider (here HuggingFace) and decoding parameters. See
@@ -576,41 +598,43 @@
 one could remove this dataset from the evaluation set. The exact reason should
 be analyzed in future work. For the code and more analysis see [this notebook]
 (https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/
 analyzing_evalset.ipynb), or the colab notebook above. # Contributing We are
 accepting PRs for new models, evaluators, and eval sets, in addition to bug
 fixes. We will update the [leaderboard website](https://tatsu-lab.github.io/
 alpaca_eval/) regularly with new community contributions. We have also created
-a [support discord](https://discord.gg/qVYd69ye) for AlpacaEval in case you run
-into any issues and wish to ask help from the community.
+a [support discord](https://discord.gg/GJMxJSVZZM) for AlpacaEval in case you
+run into any issues and wish to ask help from the community. To get started,
+please first fork the repo, and install the package from source `pip install -
+e .`
 ***** Contributing a model *****
 First, you'll need to add a model config definition in the [models_configs]
 (src/alpaca_eval/models_configs/) folder. As an example, you can look at the
 [falcon-7b-instruct yaml](src/alpaca_eval/models_configs/falcon-7b-instruct/
 configs.yaml). Please make sure the folder name and key name in the yaml match
-exactly. Then, please follow the steps in [Evaluating-a-model](#evaluating-a-
+exactly. Then, please follow the steps in [Evaluating a model](#evaluating-a-
 model) to run inference on the model to produce outputs on the eval set and
 score the model according to one of the evaluators. An example command may look
 like: ```sh alpaca_eval evaluate_from_model \ --model_configs 'falcon-7b-
 instruct' \ --annotators_config 'alpaca_eval_gpt4' ``` After running this
 command, you should have generated an outputs json and a new entry in the
-corresponding leaderboard file. Please make a PR with the config, outputs file,
-and updated leaderboard.
+corresponding [leaderboard file](https://github.com/tatsu-lab/alpaca_eval/tree/
+main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR with the
+config, outputs file, and updated leaderboard.
 ***** Contributing an evaluator *****
 Please first follow the directions in [Making a new evaluator](#making-a-new-
 evaluator). Once you're created the annotator config, we ask that you create a
 new leaderboard for the annotator by evaluating the minimal set of models. The
 outputs for these models can be found by downloading
 [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_eval_all_outputs.json). ```bash alpaca_eval
-make_leaderboard \ --leaderboard_path
-lpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \ --
-all_model_outputs alpaca_eval_all_outputs.json \ --annotators_config
-yaml> ``` Then, please create a PR with the annotator config and leaderboard
-csv.
+make_leaderboard \ --leaderboard_path src/alpaca_eval/leaderboards/
+data_AlpacaEval/_leaderboard.csv \ --all_model_outputs
+alpaca_eval_all_outputs.json \ --annotators_config  ``` Then, please create a
+PR with the annotator config and leaderboard csv.
 ***** Contributing an eval set *****
 To contribute a new eval set, you'll first need to specify a set of textual
 instructions. Then, you'll need to specify a set of reference outputs (model
 win-rates are computed against this reference). For ease of use, you may use
 the default [text-davinci-003](src/alpaca_eval/models_configs/text_davinci_003/
 ) reference config. Place these together into a json, where each entry
 specifies the fields `instruction`, `output`, and `generator`. You can look to
@@ -778,7 +802,15 @@
 evaluators. For example: - [AlpacaFarm Appx C](https://arxiv.org/abs/
 2305.14387) and [Large Language Models are not Fair Evaluators](https://
 arxiv.org/abs/2305.17926v1) both found that automatic annotators have a
 position bias. - [AlpacaFarm Sec. 5.2.](https://arxiv.org/abs/2305.14387) and
 [The False Promise of Imitating Proprietary LLMs](https://arxiv.org/abs/
 2305.15717) both found that automatic annotators favor style (e.g. use of list,
 tone, word choice, length) over factuality.
+***** Major updates *****
+- 19th June 2023: add leaderboard `chatgpt_fn` that anyone can use (no waiting
+lists). - 19th June 2023: update to use [OpenAI's function calling](https://
+openai.com/blog/function-calling-and-other-api-updates). Example:
+[`chatgpt_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/
+alpaca_eval/evaluators_configs/chatgpt_fn) or [`alpaca_eval_gpt4_fn`](https://
+github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/
+alpaca_eval_gpt4_fn).
```

### Comparing `alpaca_eval-0.1.3/example/outputs.json` & `alpaca_eval-0.1.5/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/setup.py` & `alpaca_eval-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/analyze.py` & `alpaca_eval-0.1.5/src/alpaca_eval/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,58 +229,72 @@
         )
         return 1 - agreement["accuracy"]
 
     def get_length_biases(
             self, annotations: Union[pd.DataFrame, str], significant_delta_length: int = 30
     ) -> dict[str, float]:
         """Estimate the biases for longer sentences."""
-        df = annotations.drop_duplicates(subset=self.keys).copy()
-        df["best_output"] = np.where(df["preference"] == 1, df.output_1, df.output_2)
-        df["worse_output"] = np.where(df["preference"] == 2, df.output_1, df.output_2)
-
-        # Step 1: Create new columns indicating the length of `best_output` and `worse_output`
-        df["best_output_length"] = df["best_output"].apply(len)
-        df["worse_output_length"] = df["worse_output"].apply(len)
-        # Step 2: Create a new column indicating whether one output is (significantly) longer than the other
-        df["one_is_longer"] = (df["best_output_length"] - df["worse_output_length"]).abs() > significant_delta_length
-        df["is_prefer_longer"] = df["best_output_length"] > df["worse_output_length"]
-        # Step 3: Count the number of times you prefer the longer output
-        prefer_longer = df[df["one_is_longer"] & df["is_prefer_longer"]].shape[0]
-        # Step 4: Count the total number of instances when one output is longer than the other
-        total_one_is_longer = df[df["one_is_longer"]].shape[0]
-        # Step 5: Calculate the probability of preferring the longer output
-        probability_prefer_longer = prefer_longer / total_one_is_longer
-
-        percentage_longer = ((df["best_output_length"] - df["worse_output_length"]) / df["worse_output_length"]).mean()
+        try:
+            df = annotations.drop_duplicates(subset=self.keys).copy()
+            df["best_output"] = np.where(df["preference"] == 1, df.output_1, df.output_2)
+            df["worse_output"] = np.where(df["preference"] == 2, df.output_1, df.output_2)
+
+            # Step 1: Create new columns indicating the length of `best_output` and `worse_output`
+            df["best_output_length"] = df["best_output"].apply(len)
+            df["worse_output_length"] = df["worse_output"].apply(len)
+            # Step 2: Create a new column indicating whether one output is (significantly) longer than the other
+            df["one_is_longer"] = (df["best_output_length"] - df[
+                "worse_output_length"]).abs() > significant_delta_length
+            df["is_prefer_longer"] = df["best_output_length"] > df["worse_output_length"]
+            # Step 3: Count the number of times you prefer the longer output
+            prefer_longer = df[df["one_is_longer"] & df["is_prefer_longer"]].shape[0]
+            # Step 4: Count the total number of instances when one output is longer than the other
+            total_one_is_longer = df[df["one_is_longer"]].shape[0]
+            # Step 5: Calculate the probability of preferring the longer output
+            probability_prefer_longer = prefer_longer / total_one_is_longer
+
+            percentage_longer = (
+                    (df["best_output_length"] - df["worse_output_length"]) / df["worse_output_length"]).mean()
+
+        except Exception as e:
+            logging.warning(f"Could not compute length biases: {e}")
+            probability_prefer_longer = np.nan
+            percentage_longer = np.nan
 
         return dict(
             probability_prefer_longer=probability_prefer_longer,
             percentage_longer=percentage_longer,
         )
 
     def get_list_biases(self, annotations: Union[pd.DataFrame, str]) -> dict[str, float]:
         """Estimate the biases for sentences with lists."""
-        df = annotations.drop_duplicates(subset=self.keys).copy()
-        df["best_output"] = np.where(df["preference"] == 1, df.output_1, df.output_2)
-        df["worse_output"] = np.where(df["preference"] == 2, df.output_1, df.output_2)
-
-        # Step 1: Create new columns indicating whether `best_output` and `worse_output` contain lists
-        df["is_best_list"] = df["best_output"].apply(utils.contains_list)
-        df["is_worse_list"] = df["worse_output"].apply(utils.contains_list)
-        # Step 2: Create a new column indicating whether either `best_output` or `worse_output` has a list but not both
-        df["either_list"] = df["is_best_list"] ^ df["is_worse_list"]
-        # Step 3: Count the number of times you prefer `best_output` when either `best_output` or `worse_output` has
-        # a list but not both
-        prefer_best_either_list = df[(df["either_list"]) & df["is_best_list"]].shape[0]
-        # Step 4: Count number of instances when either `best_output` or `worse_output` has a list but not both
-        total_either_list = df[df["either_list"]].shape[0]
-        # Step 5: Calculate the probability
-        probability_prefer_list = prefer_best_either_list / total_either_list
-
-        percentage_longer = (df["is_best_list"].mean() - df["is_worse_list"].mean()) / df["is_worse_list"].mean()
+        try:
+            df = annotations.drop_duplicates(subset=self.keys).copy()
+            df["best_output"] = np.where(df["preference"] == 1, df.output_1, df.output_2)
+            df["worse_output"] = np.where(df["preference"] == 2, df.output_1, df.output_2)
+
+            # Step 1: Create new columns indicating whether `best_output` and `worse_output` contain lists
+            df["is_best_list"] = df["best_output"].apply(utils.contains_list)
+            df["is_worse_list"] = df["worse_output"].apply(utils.contains_list)
+            # Step 2: Create a new column indicating whether either `best_output` or `worse_output` has a list but
+            # not both
+            df["either_list"] = df["is_best_list"] ^ df["is_worse_list"]
+            # Step 3: Count the number of times you prefer `best_output` when either `best_output` or `worse_output` has
+            # a list but not both
+            prefer_best_either_list = df[(df["either_list"]) & df["is_best_list"]].shape[0]
+            # Step 4: Count number of instances when either `best_output` or `worse_output` has a list but not both
+            total_either_list = df[df["either_list"]].shape[0]
+            # Step 5: Calculate the probability
+            probability_prefer_list = prefer_best_either_list / total_either_list
+
+            percentage_longer = (df["is_best_list"].mean() - df["is_worse_list"].mean()) / df["is_worse_list"].mean()
+        except Exception as e:
+            logging.warning(f"Could not compute list biases: {e}")
+            probability_prefer_list = np.nan
+            percentage_longer = np.nan
 
         return dict(
             probability_prefer_list=probability_prefer_list,
             percentage_longer=percentage_longer,
         )
 
     def _select_n_annotations(self, df, n_annotators=None, is_rm_less_than: bool = True):
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.1.5/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Optional, Sequence, Union
 import os
 
 import numpy as np
 import pandas as pd
-import yaml
 
 from .. import completion_parsers, utils, constants
 from ..decoders import get_fn_completions
 
 CURRENT_DIR = Path(__file__).parent
 logging.getLogger().setLevel(logging.INFO)
 
-__all__ = ["PairwiseAnnotator"]
+__all__ = ["PairwiseAnnotator", "SinglePairwiseAnnotator"]
 
 
 class PairwiseAnnotator:
     """Class for a pool of annotators.
 
     Notes
     -----
@@ -36,15 +35,15 @@
 
     Parameters
     ----------
     annotators_config : Path or list of dict, optional
         A dictionary or path to a yaml file containing the configuration for the pool of annotators. If a directory,
         we search for 'configs.yaml' in it. The keys in the first  dictionary should be the annotator's name, and
         the value should be a dictionary of the annotator's configuration which should have the following keys:
-        The path is to `evaluators_configs/` directory.
+        The path is relative to `evaluators_configs/` directory.
         - prompt_template (str): a prompt template or path to it. The template should contain placeholders for keys in
             the example dictionary, typically {instruction} and {output_1} {output_2}.
         - fn_completions (str): function in `alpaca_farm.decoders` for completions. Needs to accept as first argument
             `prompts` which is a list of string.
         - completions_kwargs (dict): kwargs for fn_completions. E.g. model_name, max_tokens, temperature,
         tokens_to_avoid
         - fn_completion_parser (str) : Function in `completion_parsers.py` to use for parsing the completions into
@@ -76,46 +75,59 @@
 
     other_keys_to_keep : tuple of str, optional
         Other columns to store besides the preferences.
 
     is_store_missing_preferences : bool, optional
         Whether to store missing preferences. If True it will avoid trying to always reannotate examples that have
         errors.
+
+    base_dir : Path, optional
+        Path to the directory containing the annotators configs. I.e. annotators_config will be relative
+        to this directory.
     """
 
     def __init__(
-            self,
-            annotators_config: Union[utils.AnyPath, list[dict[str, Any]]] = "claude",
-            seed: Optional[int] = 0,
-            is_avoid_reannotations: bool = True,
-            caching_path: Optional[utils.AnyPath] = "auto",
-            input_keys: Sequence[str] = ("instruction",),
-            output_keys: Sequence[str] = ("output_1", "output_2"),
-            p_label_flip: Optional[float] = None,
-            other_keys_to_keep: Sequence[str] = ("price_per_example", "time_per_example"),
-            is_store_missing_preferences: bool = True,
+        self,
+        annotators_config: Union[utils.AnyPath, list[dict[str, Any]]] = "claude",
+        seed: Optional[int] = 0,
+        is_avoid_reannotations: bool = True,
+        caching_path: Optional[utils.AnyPath] = "auto",
+        input_keys: Sequence[str] = ("instruction",),
+        output_keys: Sequence[str] = ("output_1", "output_2"),
+        p_label_flip: Optional[float] = None,
+        other_keys_to_keep: Sequence[str] = ("price_per_example", "time_per_example"),
+        is_store_missing_preferences: bool = True,
+        base_dir: utils.AnyPath = constants.EVALUATORS_CONFIG_DIR,
     ):
         logging.info(f"Creating the annotator from `{annotators_config}`.")
+        self.base_dir = Path(base_dir)
 
         # setting it relative to the config directory
-        annotators_config = constants.EVALUATORS_CONFIG_DIR / annotators_config
+        annotators_config = self.base_dir / annotators_config
 
         if annotators_config.is_dir():
             annotators_config = annotators_config / "configs.yaml"
 
         if caching_path == "auto":
             if isinstance(annotators_config, (str, Path, os.PathLike)):
                 stem = Path(annotators_config).stem
-                caching_path = Path(annotators_config).parent / f"annotations_seed{seed}_{stem}.json"
+                caching_path = (
+                    Path(annotators_config).parent
+                    / f"annotations_seed{seed}_{stem}.json"
+                )
                 logging.info(f"Saving annotations to `{caching_path}`.")
             else:
-                logging.warning("caching_path cannot be 'auto' if annotators_config is not a path. Setting to None.")
+                logging.warning(
+                    "caching_path cannot be 'auto' if annotators_config is not a path. Setting to None."
+                )
                 caching_path = None
         elif caching_path is not None:
-            logging.warning("Saving_path is given but not 'auto', make sure that it's different for different seeds.")
+            logging.warning(
+                "Saving_path is given but not 'auto', make sure that it's different for different seeds."
+            )
 
         self.seed = seed
         self.is_avoid_reannotations = is_avoid_reannotations
         self.input_keys = list(input_keys)
         self.output_keys = list(output_keys)
         self.input_output_keys = self.input_keys + self.output_keys
         self.all_keys = self.input_keys + self.output_keys + ["annotator"]
@@ -125,22 +137,29 @@
         self.annotators_config = annotators_config
 
         self.annotators = self._initialize_annotators(annotators_config)
         self.caching_path = caching_path
         self.df_annotations = None
         self.load_()
 
+    ### Helper properties to make it easier to inherit from this class ###
+    @property
+    def SingleAnnotator(self):
+        return SinglePairwiseAnnotator
+
+    #########################################
+
     def annotate_samples(
-            self,
-            all_outputs: utils.AnyData,
-            keys_to_sample_output_2: Optional[Sequence] = None,
-            is_unique_instructions: bool = True,
-            p_label_flip: Optional[float] = None,
-            is_multisample_list: bool = True,
-            **decoding_kwargs,
+        self,
+        all_outputs: utils.AnyData,
+        keys_to_sample_output_2: Optional[Sequence] = None,
+        is_unique_instructions: bool = True,
+        p_label_flip: Optional[float] = None,
+        is_multisample_list: bool = True,
+        **decoding_kwargs,
     ) -> list[dict[str, Any]]:
         """Sample pairs of outputs from a sequence of examples and annotate them.
 
         Parameters
         ----------
         all_outputs : list of dict or pd.DataFrame or datasets.Dataset
             All examples from which we will sample a pair of outputs to annotate. Each dictionary (or row) should
@@ -167,15 +186,19 @@
         decoding_kwargs :
             Additional arguments to pass to the decoder.
         """
 
         all_outputs = utils.convert_to_dataframe(all_outputs)
 
         if is_multisample_list:
-            all_outputs = all_outputs.explode("output").reset_index().rename(columns={"index": "sample_id"})
+            all_outputs = (
+                all_outputs.explode("output")
+                .reset_index()
+                .rename(columns={"index": "sample_id"})
+            )
             all_outputs["sample_id"] = all_outputs.groupby("sample_id").cumcount()
 
         if keys_to_sample_output_2 is None:
             keys_to_sample_output_2 = self.input_keys
         keys_to_sample_output_2 = list(keys_to_sample_output_2)
 
         n_pre_drop = len(all_outputs)
@@ -191,23 +214,27 @@
         if len(df_to_annotate) != n_pre_drop:
             logging.warning(
                 f"""Filtered rows because of duplicate outputs for the same keys_to_sample_output_2=
                 {keys_to_sample_output_2}. {n_pre_drop} -> {len(df_to_annotate)}"""
             )
 
         # sample an output 2 for each output 1 that are different
-        df_to_annotate["output_2"] = df_to_annotate.groupby(list(keys_to_sample_output_2))["output_1"].transform(
+        df_to_annotate["output_2"] = df_to_annotate.groupby(
+            list(keys_to_sample_output_2)
+        )["output_1"].transform(
             lambda x: utils.random_derangement(x.values, seed=self.seed)
         )
 
         if is_unique_instructions:
             n_pre_dedup = len(df_to_annotate)
             df_to_annotate = df_to_annotate.drop_duplicates(subset=self.input_keys)
             if len(df_to_annotate) != n_pre_dedup:
-                logging.info(f"Filtered unique instruction/input pairs: {n_pre_dedup} -> {len(df_to_annotate)}")
+                logging.info(
+                    f"Filtered unique instruction/input pairs: {n_pre_dedup} -> {len(df_to_annotate)}"
+                )
 
         if p_label_flip is not None:
             old_p_label_flip = self.p_label_flip
             self.set_noise(p_label_flip)
 
         try:
             annotated = self.annotate_pairs(df_to_annotate, **decoding_kwargs)
@@ -215,35 +242,35 @@
             # reset even if there is an error
             if p_label_flip is not None:
                 self.set_noise(old_p_label_flip)
 
         return annotated
 
     def annotate_head2head(
-            self,
-            outputs_1: Union[Sequence[dict[str, Any]], pd.DataFrame],
-            outputs_2: Union[Sequence[dict[str, Any]], pd.DataFrame],
-            keys_to_merge: Sequence[str] = ("instruction",),
-            is_ordered: bool = False,
-            **decoding_kwargs,
+        self,
+        outputs_1: Union[Sequence[dict[str, Any]], pd.DataFrame],
+        outputs_2: Union[Sequence[dict[str, Any]], pd.DataFrame],
+        keys_to_merge: Optional[Sequence[str]] = None,
+        is_ordered: bool = False,
+        **decoding_kwargs,
     ) -> list[dict[str, Any]]:
         """Head-to-head comparison between two sequence of outputs.
 
         Parameters
         ----------
         outputs_1 : list of dict or dataframe
             Examples to annotate. Each dictionary (or row) should contain all of `keys_to_merge` and `"output"`.
             `"output"` will become `"output_1"`.
 
         outputs_2 : list of dict or dataframe
             Second  to annotate. Each dictionary (or row) should contain all of `keys_to_merge` and `"output"`.
             `"output"` will become `"output_2"`.
 
         keys_to_merge : tuple of str, optional
-            Keys to use to merge the two sequences of outputs.
+            Keys to use to merge the two sequences of outputs. If None uses `self.input_keys`
 
         is_ordered : bool, optional
             Whether the two sequences of outputs are in matching order. If not we will be merging based on
             `keys_to_merge`, which means that the outputs can actually be shorter than the inputs (if some outputs
             are not found in the other sequence) or longer (if some outputs are duplicated in both sequences =>
             set cartesian products).
 
@@ -253,40 +280,49 @@
         Returns
         -------
         annotated : list of dict
             The annotated examples. Each dictionary will contain all of `keys_to_merge`, `"output_1"`, `"output_2"`, and
             `"preference"`. Preference will be 0 if output_1 == output_2, 1 if output_1 is preferred, and 2 if output_2
             is preferred.
         """
+        if keys_to_merge is None:
+            keys_to_merge = self.input_keys
+
         keys_to_merge = list(keys_to_merge)
 
         outputs_1 = utils.convert_to_dataframe(outputs_1)
         outputs_2 = utils.convert_to_dataframe(outputs_2)
 
         if is_ordered:
             outputs_1 = outputs_1.copy()
             outputs_2 = outputs_2.copy()
             outputs_1["tmp_idx"] = range(len(outputs_1))
             outputs_2["tmp_idx"] = range(len(outputs_1))
             keys_to_merge += ["tmp_idx"]  # add a temporary index to merge on
 
         # find all the columns that are in both
-        other_same_cols = [k for k in outputs_1.columns if k in outputs_2 and k not in (keys_to_merge + ["output"])]
+        other_same_cols = [
+            k
+            for k in outputs_1.columns
+            if k in outputs_2 and k not in (keys_to_merge + ["output"])
+        ]
 
         df_to_annotate = pd.merge(
             outputs_1,
             outputs_2,
             on=keys_to_merge,
             suffixes=("_1", "_2"),
         )
 
         for c in other_same_cols:
             # if the columns are the same, we can drop the _2
             if df_to_annotate[c + "_1"].equals(df_to_annotate[c + "_2"]):
-                df_to_annotate = df_to_annotate.drop(columns=c + "_2").rename(columns={c + "_1": c})
+                df_to_annotate = df_to_annotate.drop(columns=c + "_2").rename(
+                    columns={c + "_1": c}
+                )
 
         if is_ordered:
             df_to_annotate = df_to_annotate.drop(columns="tmp_idx")
         else:
             # if you are taking the cartesian product, you can have undesired duplicates
             df_to_annotate = df_to_annotate.drop_duplicates()
 
@@ -299,17 +335,17 @@
                 )
 
         out = self.annotate_pairs(df_to_annotate, **decoding_kwargs)
 
         return out
 
     def annotate_pairs(
-            self,
-            to_annotate: Union[Sequence[dict[str, Any]], pd.DataFrame],
-            **decoding_kwargs,
+        self,
+        to_annotate: Union[Sequence[dict[str, Any]], pd.DataFrame],
+        **decoding_kwargs,
     ) -> list[dict[str, Any]]:
         """Annotates the given examples, which contain both `"output_1"` and `"output_2"` keys.
 
         Parameters
         ----------
         to_annotate : list of dict or dataframe
             Examples to annotate. Each dictionary (or row) should contain all of `self.input_output_keys`.
@@ -347,15 +383,17 @@
     def _preprocess(self, to_annotate: utils.AnyData) -> pd.DataFrame:
         """Preprocess the examples to annotate. In particular takes care of filtering unnecessary examples."""
 
         df_to_annotate = utils.convert_to_dataframe(to_annotate).copy()
 
         for c in self.other_keys_to_keep + ["preference"]:
             if c in df_to_annotate.columns:
-                logging.warning(f"""{c} column is already in the dataframe. We will overwrite it.""")
+                logging.warning(
+                    f"""{c} column is already in the dataframe. We will overwrite it."""
+                )
                 df_to_annotate[c] = np.nan
 
         # remove duplicates because you only need to annotate one of them
         df_to_annotate = df_to_annotate.drop_duplicates(subset=self.input_output_keys)
 
         # set the annotater for each example
         df_to_annotate["annotator"] = df_to_annotate.apply(
@@ -365,27 +403,31 @@
                 choices=list(self.annotators.keys()),
             ),
             axis=1,
         )
 
         if self.is_avoid_reannotations:
             # merge the old annotations
-            df_to_annotate = self._merge_annotations(df_to_annotate, self.df_annotations)
+            df_to_annotate = self._merge_annotations(
+                df_to_annotate, self.df_annotations
+            )
 
         # adds random noise => avoids annotating examples that will be noised out.
         if self.p_label_flip:
-            logging.info(f"Adding random noise to the labels p_label_flip={self.p_label_flip}.")
+            logging.info(
+                f"Adding random noise to the labels p_label_flip={self.p_label_flip}."
+            )
             # if you have 25% change of flipping the label, you have 50% chance of selecting random label
             p_noise = self.p_label_flip * 2
             noisy_preference = df_to_annotate.apply(
                 # we add "noisy_label" at the beginning to use ~independent seeds between tasks
                 lambda x: utils.random_seeded_choice(  # seed on inputs for reproducibility
                     seed="noisy_preference" + x["instruction"] + str(self.seed),
                     choices=[np.nan, 1, 2],
-                    p=[1 - p_noise, self.p_label_flip, self.p_label_flip],
+                    weights=[1 - p_noise, self.p_label_flip, self.p_label_flip],
                 ),
                 axis=1,
             )
             df_to_annotate["is_noisy_label"] = ~noisy_preference.isna()
             # keeps previously annotated examples when you did not add noise
             df_to_annotate["preference"] = np.where(
                 df_to_annotate["is_noisy_label"],
@@ -395,86 +437,112 @@
 
         idcs_is_same_outputs = df_to_annotate["output_1"] == df_to_annotate["output_2"]
         df_to_annotate.loc[idcs_is_same_outputs, "preference"] = 0
 
         return df_to_annotate
 
     def _initialize_annotators(
-            self, annotators_config: Union[utils.AnyPath, dict[str, dict[str, Any]]]
+        self, annotators_config: Union[utils.AnyPath, dict[str, dict[str, Any]]]
     ) -> dict[str, Callable]:
         """Load all the configs and prompts if necessary."""
-        annotators_config = utils.load_configs(annotators_config, relative_to=CURRENT_DIR)
+        annotators_config = utils.load_configs(annotators_config)
         return {
-            name: SinglePairwiseAnnotator(seed=self.seed, **annotator_config)
+            name: self.SingleAnnotator(
+                seed=self.seed, base_dir=self.base_dir, **annotator_config
+            )
             for name, annotator_config in annotators_config.items()
         }
 
-    def _annotate(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
+    def _annotate(
+        self, df_to_annotate: pd.DataFrame, **decoding_kwargs
+    ) -> pd.DataFrame:
         """Annotate the examples."""
 
         df_annotated = df_to_annotate
         for annotator in self.annotators.keys():
             # only annotate examples that have not been annotated yet
-            curr_idcs = (df_annotated["annotator"] == annotator) & df_annotated["preference"].isna()
+            curr_idcs = (df_annotated["annotator"] == annotator) & df_annotated[
+                "preference"
+            ].isna()
 
             logging.info(f"Annotating {curr_idcs.sum()} examples with {annotator}")
 
             # actual annotation
-            curr_annotated = self.annotators[annotator](df_annotated.loc[curr_idcs, self.all_keys], **decoding_kwargs)
+            curr_annotated = self.annotators[annotator](
+                df_annotated.loc[curr_idcs, self.all_keys], **decoding_kwargs
+            )
 
             df_annotated = self._merge_annotations(df_annotated, curr_annotated)
 
         return df_annotated
 
     def _postprocess_and_store_(
-            self, df_annotated: pd.DataFrame, to_annotate: Union[Sequence[dict[str, Any]], pd.DataFrame]
+        self,
+        df_annotated: pd.DataFrame,
+        to_annotate: Union[Sequence[dict[str, Any]], pd.DataFrame],
     ) -> list[dict[str, Any]]:
         """Convert the dataframe into a list of dictionaries to be returned, and store current anntations."""
 
         df_to_annotate = utils.convert_to_dataframe(to_annotate)
 
         # select available annotations
         if self.is_store_missing_preferences:
             df_annotated["preference"] = df_annotated["preference"].fillna(-1)
         else:
             df_annotated["preference"] = df_annotated["preference"].replace(-1, np.nan)
 
         df_annotated = df_annotated[~df_annotated["preference"].isna()].copy()
 
         # try converting to int now that no nan
-        df_annotated["preference"] = pd.to_numeric(df_annotated["preference"], downcast="integer", errors="ignore")
+        df_annotated["preference"] = pd.to_numeric(
+            df_annotated["preference"], downcast="integer", errors="ignore"
+        )
 
         if "is_noisy_label" in df_annotated.columns:
             # dont' store noisy labels
-            df_annotated_to_store = df_annotated.query("is_noisy_label == False").drop(columns=["is_noisy_label"])
+            df_annotated_to_store = df_annotated.query("is_noisy_label == False").drop(
+                columns=["is_noisy_label"]
+            )
             df_annotated = df_annotated.drop(columns=["is_noisy_label"])
         else:
             df_annotated_to_store = df_annotated
 
-        other_keys_to_keep = [c for c in self.other_keys_to_keep if c in df_annotated_to_store.columns]
+        other_keys_to_keep = [
+            c for c in self.other_keys_to_keep if c in df_annotated_to_store.columns
+        ]
         all_keys_to_keep = self.all_keys + ["preference"] + other_keys_to_keep
         df_annotated_to_store = df_annotated_to_store[all_keys_to_keep]
 
         if self.df_annotations is None:
             df_annotations = df_annotated_to_store
         else:
-            df_annotations = pd.concat([self.df_annotations, df_annotated_to_store], axis=0, ignore_index=True)
+            df_annotations = pd.concat(
+                [self.df_annotations, df_annotated_to_store], axis=0, ignore_index=True
+            )
 
-        self.df_annotations = df_annotations.drop_duplicates(subset=self.all_keys, keep="last")
+        self.df_annotations = df_annotations.drop_duplicates(
+            subset=self.all_keys, keep="last"
+        )
 
         self.save()
 
         if self.is_store_missing_preferences:
             # put back np.nan
             df_annotated["preference"] = df_annotated["preference"].replace(-1, np.nan)
 
         # need to merge with df_to_annotate in case you dropped duplicates
         on = list(self.input_keys + self.output_keys)
         df_annotated = df_annotated[all_keys_to_keep]
-        df_to_annotate = df_to_annotate[[c for c in df_to_annotate.columns if c not in df_annotated.columns or c in on]]
+        df_to_annotate = df_to_annotate[
+            [
+                c
+                for c in df_to_annotate.columns
+                if c not in df_annotated.columns or c in on
+            ]
+        ]
         # need to remove all other columns before merging if not you will
         df_annotated = df_to_annotate.merge(df_annotated, on=on, how="outer")
 
         annotated = df_annotated.to_dict(orient="records")
 
         return annotated
 
@@ -482,15 +550,17 @@
         """Save the annotations to json."""
         path = path or self.caching_path
         if path is not None:
             logging.info(f"Saving all annotations to {path}.")
             # to make sure that we don't overwrite the annotations we load again from file (ideally would use a DB)
             self._refresh_annotations_()
             if not self.is_store_missing_preferences:
-                self.df_annotations = self.df_annotations[~self.df_annotations["preference"].isna()]
+                self.df_annotations = self.df_annotations[
+                    ~self.df_annotations["preference"].isna()
+                ]
             self.df_annotations.to_json(path, orient="records", indent=2)
 
     def _refresh_annotations_(self):
         """Refresh the annotations in memory."""
         curr_df_annotations = self.df_annotations.copy()
         self.load_()
         self.df_annotations = pd.concat(
@@ -502,31 +572,41 @@
         path = path or self.caching_path
         if path is not None:
             path = Path(path)
             if path.exists():
                 logging.info(f"Loading all annotations from {path}.")
                 self.df_annotations = pd.read_json(path)
 
-    def _merge_annotations(self, df_to_annotate: pd.DataFrame, df_partially_annotated: pd.DataFrame) -> pd.DataFrame:
+    def _merge_annotations(
+        self, df_to_annotate: pd.DataFrame, df_partially_annotated: pd.DataFrame
+    ) -> pd.DataFrame:
         """Merge (partial) annotations with the original df to keep the same order and avoid duplicates annotations."""
         if df_partially_annotated is None or df_partially_annotated.empty:
             return df_to_annotate
 
-        other_keys_to_keep = [c for c in self.other_keys_to_keep if c in df_partially_annotated.columns]
+        other_keys_to_keep = [
+            c for c in self.other_keys_to_keep if c in df_partially_annotated.columns
+        ]
+
         df_to_annotate = df_to_annotate.merge(
             df_partially_annotated[self.all_keys + ["preference"] + other_keys_to_keep],
             on=self.all_keys,
             how="left",
             suffixes=("_old", "_new"),
         )
 
         # if columns were in both dataframes, try to merge them
         for c in other_keys_to_keep + ["preference"]:
-            if f"{c}_old" in df_to_annotate.columns and f"{c}_new" in df_to_annotate.columns:
-                df_to_annotate[c] = df_to_annotate[c + "_old"].fillna(df_to_annotate[c + "_new"])
+            if (
+                f"{c}_old" in df_to_annotate.columns
+                and f"{c}_new" in df_to_annotate.columns
+            ):
+                df_to_annotate[c] = df_to_annotate[c + "_old"].fillna(
+                    df_to_annotate[c + "_new"]
+                )
                 df_to_annotate = df_to_annotate.drop(columns=[c + "_old", c + "_new"])
 
         return df_to_annotate
 
 
 class SinglePairwiseAnnotator:
     """A helper class for a single auto annotators.
@@ -558,42 +638,80 @@
         Whether to shuffle the order of the examples before making the prompt. Useful if batch_size > 1.
 
     seed : int
         Seed for randomization.
 
     batch_size : int
         Number of examples that will be added in a single prompt.
+
+    base_dir : Path, optional
+        Path to the directory containing the annotators configs. I.e. annotators_config will be relative
+        to this directory.
     """
 
     def __init__(
-            self,
-            prompt_template: dict[str, str],
-            fn_completion_parser: Union[Callable, str] = "regex_parser",
-            completion_parser_kwargs: Optional[dict[str, Any]] = None,
-            fn_completions: Union[Callable, str] = "openai_completions",
-            completions_kwargs: Optional[dict[str, Any]] = None,
-            is_randomize_output_order: bool = True,
-            is_shuffle: bool = True,
-            seed: Optional[int] = 123,
-            batch_size: int = 1,
+        self,
+        prompt_template: utils.AnyPath,
+        fn_completion_parser: Union[Callable, str] = "regex_parser",
+        completion_parser_kwargs: Optional[dict[str, Any]] = None,
+        fn_completions: Union[Callable, str] = "openai_completions",
+        completions_kwargs: Optional[dict[str, Any]] = None,
+        is_randomize_output_order: bool = True,
+        is_shuffle: bool = True,
+        seed: Optional[int] = 123,
+        batch_size: int = 1,
+        base_dir: utils.AnyPath = constants.EVALUATORS_CONFIG_DIR,
     ):
-        self.prompt_template = utils.read_or_return(constants.EVALUATORS_CONFIG_DIR / prompt_template)
+        self.base_dir = Path(base_dir)
+        self.prompt_template = self._get_prompt_template(prompt_template)
 
         if isinstance(fn_completion_parser, str):
             fn_completion_parser = getattr(completion_parsers, fn_completion_parser)
         completion_parser_kwargs = completion_parser_kwargs or {}
-        self.fn_completion_parser = partial(fn_completion_parser, **completion_parser_kwargs)
+        self.fn_completion_parser = partial(
+            fn_completion_parser, **completion_parser_kwargs
+        )
 
         self.is_randomize_output_order = is_randomize_output_order
         self.fn_completions = get_fn_completions(fn_completions)
         self.completions_kwargs = completions_kwargs or {}
         self.seed = seed
         self.is_shuffle = is_shuffle
         self.batch_size = batch_size
 
+    def _get_prompt_template(self, prompt_template: utils.AnyPath):
+        return utils.read_or_return(self.base_dir / prompt_template)
+
+    def make_prompts(
+        self, df_to_annotate: pd.DataFrame, prompt_template: Optional[str] = None
+    ) -> tuple[list[str], pd.DataFrame]:
+        """Make all the prompts for the given examples.
+
+        Parameters
+        ----------
+        df_to_annotate : pd.DataFrame
+            Examples to annotate
+
+        prompt_template : str
+            Template to use for the prompt. If None, use the one from the constructor.
+
+        Returns
+        -------
+        prompts : list[str]
+            Formatted prompts for the given examples.
+
+        df_to_annotate : pd.DataFrame
+            Examples to annotate in the same order as prompts.
+        """
+        if prompt_template is None:
+            prompt_template = self.prompt_template
+        return utils.make_prompts(
+            df=df_to_annotate, template=prompt_template, batch_size=self.batch_size
+        )
+
     def __call__(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
         """Annotates the given examples.
 
         Parameters
         ----------
         df_to_annotate : pd.DataFrame
             Examples to annotate
@@ -606,21 +724,23 @@
         if df_to_annotate.empty:
             df_to_annotate["preference"] = []
             return df_to_annotate
 
         df_to_annotate = self.preprocess(df_to_annotate)
 
         # prompts and completions here will not be the same length as the dataframe due to batching
-        prompts, df_to_annotate = utils.make_prompts(
-            df=df_to_annotate, template=self.prompt_template, batch_size=self.batch_size
-        )
+        prompts, df_to_annotate = self.make_prompts(df_to_annotate)
 
-        completions = self.fn_completions(prompts=prompts, **self.completions_kwargs, **decoding_kwargs)
+        completions = self.fn_completions(
+            prompts=prompts, **self.completions_kwargs, **decoding_kwargs
+        )
 
-        df_to_annotate["preference"] = self.parse_completions(completions=completions["completions"])
+        df_to_annotate["preference"] = self.parse_completions(
+            completions=completions["completions"]
+        )
         for k, v in completions.items():
             if k != "completions":
                 if len(df_to_annotate["preference"]) == len(v) * self.batch_size:
                     v = [el for el in v for _ in range(self.batch_size)]
                 df_to_annotate[k] = v
                 if "per_example" in k:
                     df_to_annotate[k] = df_to_annotate[k] / self.batch_size
@@ -638,15 +758,17 @@
                 # we add "is_switched_outputs" at the beginning to not use the same seed for all tasks
                 lambda x: utils.random_seeded_choice(
                     seed="is_switched_outputs" + x["instruction"] + str(self.seed),
                     choices=[False, True],
                 ),
                 axis=1,
             )
-            df_to_annotate = utils.shuffle_pairwise_preferences(df_to_annotate, df_to_annotate["is_switched_outputs"])
+            df_to_annotate = utils.shuffle_pairwise_preferences(
+                df_to_annotate, df_to_annotate["is_switched_outputs"]
+            )
 
         if self.is_shuffle:
             df_to_annotate = df_to_annotate.sample(frac=1, random_state=self.seed)
 
         return df_to_annotate
 
     def parse_completions(self, completions: list[str]) -> list[int]:
@@ -664,25 +786,29 @@
             all_preferences += batch_preferences
         return all_preferences
 
     def postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         """Postprocess the annotated examples."""
 
         # remove padding examples when using batch_size > 1
-        df_annotated = df_annotated.query("is_padding == False").drop(columns=["is_padding"])
+        df_annotated = df_annotated.query("is_padding == False").drop(
+            columns=["is_padding"]
+        )
 
         arr_is_na = df_annotated["preference"].isna()
         if arr_is_na.any():
             logging.warning(
                 f"{arr_is_na.sum().item()} samples had no auto annotation. We are filtering them for now. "
                 f"If you are using chain of thought it might be that max_tokens limit is too low. "
             )
             df_annotated = df_annotated[~arr_is_na]
 
         assert set(df_annotated["preference"].unique().tolist()) <= {0, 1, 2}
 
         if self.is_randomize_output_order:
             # unshuffles output 1 and output 2. For binary preference, unshuffling is equivalent to reshuffling
-            df_annotated = utils.shuffle_pairwise_preferences(df_annotated, df_annotated["is_switched_outputs"])
+            df_annotated = utils.shuffle_pairwise_preferences(
+                df_annotated, df_annotated["is_switched_outputs"]
+            )
             df_annotated = df_annotated.drop(columns=["is_switched_outputs"])
 
         return df_annotated
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.1.5/src/alpaca_eval/completion_parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         The values can be either a compiled regex or a string. If a string, it will be compiled to a regex and that will
         be modified inplace.
 
     Examples
     --------
     >>> completion = '\n(b)\n\n### Best output for example 8:\n(a)\n\n### Best output for example 9:\n(b)\n\n### Best
     output for example 10:\n(a)\n\n### Best output for example 11:\n(a)'
-    >>> parse_batched_completion(completion, {1: '\n\(a\)', 2: '\n\(b\)'})
+    >>> regex_parser(completion, {1: '\n\(a\)', 2: '\n\(b\)'})
     [2, 1, 2, 1, 1]
-    >>> parse_batched_completion(' (a)', {1: ' \(a\)', 2: ' \(b\)'})
+    >>> regex_parser(' (a)', {1: ' \(a\)', 2: ' \(b\)'})
     [1]
     >>> completion = '### Preferred output in JSON format for example 4:\r\n{{\r\n"Concise explanation": "Both
     outputs are incorrect, but Output (a) is less confusing and more concise.",\r\n"Output (a) is better than Output
     (b)": true\r\n}}\r\n\r\n### Preferred output in JSON format for example 5:\r\n{{\r\n"Concise explanation": "Both
     outputs are incomplete, but Output (b) seems to start with a more relevant source.",\r\n"Output (a) is better
     than Output (b)": false\r\n}}\r\n\r\n### Preferred output in JSON format for example 6:\r\n{{\r\n"Concise
     explanation": "Both outputs are incorrect, but Output (a) is less confusing and more concise.",\r\n"Output (a) is
@@ -80,15 +80,18 @@
     except Exception as e:
         logging.error(f"{e}\nContent: {completion}\n" "You must manually fix the score pair.")
         return [np.nan]
 
 
 def ranking_parser(completion):
     try:
-        ordered_completions = ast.literal_eval(completion)
+        if isinstance(completion, str):
+            ordered_completions = ast.literal_eval(completion)
+        else:
+            ordered_completions = completion
 
         rank = [c for c in ordered_completions if c["model"] == "model_1"][0]["rank"]
         assert rank in [1, 2]
 
         return [rank]
     except Exception as e:
         logging.error(f"{e}\nContent: {completion}\n" "You must manually fix the score pair.")
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/constants.py` & `alpaca_eval-0.1.5/src/alpaca_eval/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import getpass
 import os
 from pathlib import Path
 
 import datasets
 
 ### API specific ###
-OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY", None)
+OPENAI_API_KEYS = os.environ.get("OPENAI_API_KEYS", os.environ.get("OPENAI_API_KEY", None)).split(",")
 OPENAI_ORGANIZATION_IDS = os.environ.get("OPENAI_ORGANIZATION_IDS", None)
 if isinstance(OPENAI_ORGANIZATION_IDS, str):
     OPENAI_ORGANIZATION_IDS = OPENAI_ORGANIZATION_IDS.split(",")
 
 ANTHROPIC_API_KEY = os.environ.get("ANTHROPIC_API_KEY", None)
 ANTHROPIC_MAX_CONCURRENCY = int(os.environ.get("ANTHROPIC_MAX_CONCURRENCY", 1))
 
@@ -37,25 +37,25 @@
     "alpaca-farm-ppo-human",
     "falcon-40b-instruct",
     "alpaca-7b",
     "text_davinci_001",
 )
 VERIFIED_MODELS = MINIMAL_MODELS + (
     "alpaca-farm-ppo-sim-gpt4-20k",
-    "cohere",
+    # "cohere", we only ran eval not generations
     "falcon-7b-instruct",
     "guanaco-7b",
     "guanaco-13b",
     "guanaco-33b",
     "nous-hermes-13b",
     "oasst-sft-llama-33b",
     "oasst-sft-pythia-12b",
     "pythia-12b-mix-sft",
     "vicuna-7b",
-    "wizardlm-13b"
+    "wizardlm-13b",
 )
 
 MINIMAL_EVALUATORS = (
     "alpaca_eval_gpt4",
     "aviary_gpt4",
     "gpt4",
     "claude",
@@ -137,14 +137,15 @@
 
 
 ALPACAEVAL_LEADERBOARD_PATHS = CURRENT_DIR / "leaderboards/data_AlpacaEval"
 PRECOMPUTED_LEADERBOARDS = {
     (str(ALPACAEVAL_REFERENCE_OUTPUTS), "claude"): ALPACAEVAL_LEADERBOARD_PATHS / "claude_leaderboard.csv",
     (str(ALPACAEVAL_REFERENCE_OUTPUTS), "alpaca_eval_gpt4"): ALPACAEVAL_LEADERBOARD_PATHS
                                                              / "alpaca_eval_gpt4_leaderboard.csv",
+    (str(ALPACAEVAL_REFERENCE_OUTPUTS), "chatgpt_fn"): ALPACAEVAL_LEADERBOARD_PATHS / "chatgpt_fn_leaderboard.csv",
 }
 
 HUMAN_ANNOTATED_MODELS_TO_KEEP = (
     "GPT-4 300 characters",
     "GPT-4",
     "AlpacaFarm PPO sim (step 40)",
     "ChatGPT",
@@ -157,16 +158,22 @@
     "AlpacaFarm PPO human (10k, step 40)",
     "Alpaca 7B",
     "AlpacaFarm FeedMe human",
     "Davinci001",
     "LLaMA 7B",
 )
 
-EVALUATORS_LEADERBOARD_COLS_TO_PRIORITIZE = ["Human agreement [%]", "Price [$/1000 examples]",
-                                             "Time [seconds/1000 examples]",
-                                             "Bias", "Variance", "Proba. prefer longer", "Proba. prefer lists",
-                                             "Proba. prefer 1"]
+EVALUATORS_LEADERBOARD_COLS_TO_PRIORITIZE = [
+    "Human agreement [%]",
+    "Price [$/1000 examples]",
+    "Time [seconds/1000 examples]",
+    "Bias",
+    "Variance",
+    "Proba. prefer longer",
+    "Proba. prefer lists",
+    "Proba. prefer 1",
+]
 EVALUATORS_LEADERBOARD_COLS_TO_PRINT = EVALUATORS_LEADERBOARD_COLS_TO_PRIORITIZE[:6]
 
 CURRENT_USER = getpass.getuser()
 if CURRENT_USER in ["yanndubs"]:
     DEFAULT_CACHE_DIR = "/juice5/scr5/nlp/crfm/human-feedback/cache"
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.1.5/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.1.5/src/alpaca_eval/decoders/anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,18 +61,15 @@
                         desc="prompts",
                         total=len(prompts),
                     )
                 )
     logging.info(f"Completed {n_examples} examples in {t}.")
 
     # anthropic doesn't return total tokens but 1 token approx 4 chars
-    price = [
-        len(prompt) / 4 * _get_price_per_token(model_name)
-        for prompt in prompts
-    ]
+    price = [len(prompt) / 4 * _get_price_per_token(model_name) for prompt in prompts]
 
     avg_time = [t.duration / n_examples] * len(completions)
 
     return dict(completions=completions, price_per_example=price, time_per_example=avg_time)
 
 
 def _anthropic_completion_helper(
@@ -108,15 +105,19 @@
                 time.sleep(sleep_time)
             elif "exceeds max" in str(e):
                 curr_kwargs["max_tokens_to_sample"] = int(curr_kwargs["max_tokens_to_sample"] * 0.8)
                 if curr_kwargs["max_tokens_to_sample"] == 0:
                     raise e
                 logging.warning(f"Reducing target length to {curr_kwargs['max_tokens_to_sample']}, Retrying...")
             else:
-                raise ValueError(f"Unknown ApiException {e}.")
+                if n_retries > 0:
+                    logging.warning(f"{e}. \nRetrying...")
+                    n_retries = n_retries - 1
+                else:
+                    raise ValueError(f"Unknown ApiException {e}.")
         except Exception as e:
             if n_retries > 0:
                 logging.warning(f"{e}. \nRetrying...")
                 n_retries = n_retries - 1
             else:
                 raise e
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.1.5/src/alpaca_eval/decoders/cohere.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 import math
 import multiprocessing
 import os
 import random
 from typing import Optional, Sequence
 import tqdm
 import cohere
+from cohere import CohereError
 
 from .. import constants, utils
 
 __all__ = ["cohere_completions"]
 
 
 def cohere_completions(
         prompts: Sequence[str],
         model_name="command",
+        mode = "instruct",
         num_procs: int = 5,
         **decoding_kwargs,
 ) -> dict[str, list]:
     """Decode with Cohere API.
 
     Parameters
     ----------
@@ -39,16 +41,17 @@
     n_examples = len(prompts)
     if n_examples == 0:
         logging.info("No samples to annotate.")
         return []
     else:
         logging.info(f"Using `cohere_completions` on {n_examples} prompts using {model_name}.")
 
-    kwargs = dict(model=model_name, **decoding_kwargs)
+    kwargs = dict(model=model_name, mode=mode, **decoding_kwargs)
     logging.info(f"Kwargs to completion: {kwargs}")
+
     with utils.Timer() as t:
         if num_procs == 1:
             completions = [_cohere_completion_helper(prompt, **kwargs) for prompt in tqdm.tqdm(prompts, desc="prompts")]
         else:
             with multiprocessing.Pool(num_procs) as p:
                 partial_completion_helper = functools.partial(_cohere_completion_helper, **kwargs)
                 completions = list(
@@ -68,22 +71,38 @@
 
 
 def _cohere_completion_helper(
         prompt: str,
         cohere_api_keys: Optional[Sequence[str]] = (constants.COHERE_API_KEY,),
         max_tokens: Optional[int] = 1000,
         temperature: Optional[float] = 0.7,
+        max_tries = 5,
+        mode = "instruct",
         **kwargs,
 ) -> str:
-    anthropic_api_key = random.choice(cohere_api_keys)
-    client = cohere.Client(anthropic_api_key)
+    cohere_api_key = random.choice(cohere_api_keys)
+    client = cohere.Client(cohere_api_key)
 
     kwargs.update(dict(max_tokens=max_tokens, temperature=temperature))
     curr_kwargs = copy.deepcopy(kwargs)
 
-    # TODO deal with errors as with anthropic and openai
-    response = client.generate(prompt=prompt, **curr_kwargs)
+    for trynum in range(max_tries):  # retry errors
+        try:
+            if mode == "instruct":
+                response = client.generate(prompt=prompt, **curr_kwargs)
+                text = response[0].text
+            elif mode == "chat":
+                response = client.chat(prompt, **curr_kwargs)
+                text = response.text
+            else:
+                raise ValueError(f"Invalid mode {mode} for cohere_completions")
+
+            if text == "":
+                raise CohereError("Empty string response")
+
+            return text
 
-    if response == "":
-        response = " "  # annoying doesn't allow empty string
+        except CohereError as e:
+            print(f"Try #{trynum+1}/{max_tries}: Error running prompt {repr(prompt)}: {e}")
 
-    return response[0].text
+    return " " # placeholder response for errors, doesn't allow empty string
+
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,29 @@
     AutoModelForCausalLM,
     AutoTokenizer,
 )
 import transformers
 from peft import PeftModel
 from .. import utils, constants
 
+from torch.utils.data import Dataset
+from tqdm import tqdm
+
 __all__ = ["huggingface_local_completions"]
 
+class ListDataset(Dataset):
+    def __init__(self, original_list):
+        self.original_list = original_list
+
+    def __len__(self):
+        return len(self.original_list)
+
+    def __getitem__(self, i):
+        return self.original_list[i]
+
 
 def huggingface_local_completions(
         prompts: Sequence[str],
         model_name: str,
         do_sample: bool = False,
         batch_size: int = 1,
         model_kwargs=None,
@@ -83,14 +96,16 @@
         model = model.merge_and_unload()
 
     if batch_size == 1:
         try:
             model = model.to_bettertransformer()
         except NotImplementedError:
             pass
+        except AttributeError:
+            pass
 
     logging.info(f"Model memory: {model.get_memory_footprint() / 1e9} GB")
 
     if batch_size > 1:
         # sort the prompts by length so that we don't necessarily pad them by too much
         # save also index to reorder the completions
         original_order, prompts = zip(*sorted(enumerate(prompts), key=lambda x: len(x[1])))
@@ -107,27 +122,27 @@
         batch_size=batch_size,
     )
     default_kwargs.update(kwargs)
     logging.info(f"Kwargs to completion: {default_kwargs}")
     pipeline = transformers.pipeline(task="text-generation", model=model, tokenizer=tokenizer, **default_kwargs)
 
     ## compute and log the time for completions
+    prompts_dataset = ListDataset(prompts)
+    completions = []
+    
     with utils.Timer() as t:
-        logging.info(f"Starting {n_examples} completions. Hugging face pipeline doesn't allow generators => no"
-                     f"progress bar. Sorry for that.")
-        completions = [completion[0]["generated_text"]
-                       for completion in pipeline(
-                            prompts, return_full_text=False, pad_token_id=tokenizer.pad_token_id
-                      )]
+        
+        for out in tqdm(pipeline(prompts_dataset, return_full_text=False, pad_token_id=tokenizer.pad_token_id)):
+            completions.append(out[0]["generated_text"])
 
     logging.info(f"Time for {n_examples} completions: {t}")
 
     if batch_size > 1:
         # reorder the completions to match the original order
         completions, _ = zip(*sorted(list(zip(completions, original_order)), key=lambda x: x[1]))
         completions = list(completions)
 
     # local => price is really your compute
     price = [np.nan] * len(completions)
     avg_time = [t.duration / n_examples] * len(completions)
 
-    return dict(completions=completions, price_per_example=price, time_per_example=avg_time)
+    return dict(completions=completions, price_per_example=price, time_per_example=avg_time)
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.1.5/src/alpaca_eval/decoders/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import functools
+import json
 import logging
 import math
 import multiprocessing
 import time
 import random
 from typing import Optional, Sequence
 
@@ -158,15 +159,15 @@
 
 
 def _openai_completion_helper(
         prompt_batch: Sequence[str],
         is_chat: bool,
         sleep_time: int = 2,
         openai_organization_ids: Optional[Sequence[str]] = constants.OPENAI_ORGANIZATION_IDS,
-        openai_api_keys: Optional[Sequence[str]] = None,
+        openai_api_keys: Optional[Sequence[str]] = constants.OPENAI_API_KEYS,
         max_tokens: Optional[int] = 1000,
         top_p: Optional[float] = 1.0,
         temperature: Optional[float] = 0.7,
         **kwargs,
 ):
     # randomly select orgs
     if openai_organization_ids is not None:
@@ -188,30 +189,42 @@
                 for choice in choices:
                     assert choice.message.role == "assistant"
                     if choice.message.content == "":
                         choice["text"] = " "  # annoying doesn't allow empty string
                     else:
                         choice["text"] = choice.message.content
 
+                    if choice.message.get("function_call"):
+                        # currently we only use function calls to get a JSON object
+                        # => overwrite text with the JSON object. In the future, we could
+                        # allow actual function calls
+                        all_args = json.loads(choice.message.function_call.arguments)
+                        assert len(all_args) == 1
+                        choice["text"] = all_args[list(all_args.keys())[0]]
+
             else:
                 completion_batch = openai.Completion.create(prompt=prompt_batch, **curr_kwargs)
                 choices = completion_batch.choices
 
             for choice in choices:
                 choice["total_tokens"] = completion_batch.usage.total_tokens / len(prompt_batch)
             break
         except openai.error.OpenAIError as e:
             logging.warning(f"OpenAIError: {e}.")
             if "Please reduce your prompt" in str(e):
                 kwargs["max_tokens"] = int(kwargs["max_tokens"] * 0.8)
                 logging.warning(f"Reducing target length to {kwargs['max_tokens']}, Retrying...")
                 if kwargs["max_tokens"] == 0:
+                    logging.exception("Prompt is already longer than max context length. Error:")
                     raise e
             else:
-                logging.warning("Hit request rate limit; retrying...")
+                if "rate limit" in str(e).lower():
+                    logging.warning("Hit request rate limit; retrying...")
+                else:
+                    logging.warning(f"Unknown error {e}. \n It's likely a rate limit so we are retrying...")
                 if openai_organization_ids is not None and len(openai_organization_ids) > 1:
                     openai.organization = random.choice(
                         [o for o in openai_organization_ids if o != openai.organization]
                     )
                     logging.info(f"Switching OAI organization.")
                 if openai_api_keys is not None and len(openai_api_keys) > 1:
                     openai.api_key = random.choice([o for o in openai_api_keys if o != openai.api_key])
@@ -243,15 +256,15 @@
     <|im_end|>
     <|im_start|>system name=example_assistant
     Who's there?
     <|im_end|>
     <|im_start|>user
     Orange.
     <|im_end|>
-    >>> prompt_to_chatml(prompt)
+    >>> _prompt_to_chatml(prompt)
     [{'role': 'system', 'content': 'You are a helpful assistant.'},
      {'role': 'user', 'content': 'Knock knock.'},
      {'role': 'assistant', 'content': "Who's there?"},
      {'role': 'user', 'content': 'Orange.'}]
     """
     prompt = prompt.strip()
     assert prompt.startswith(start_token)
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,41 +3,40 @@
 ## Evaluator's leaderboard:
 
 Here's the full leaderboard estimated on 4 different seeds, which allows us to also estimate the variance of the
 annotators.
 We compute those metrics on our suggested evaluator `alpaca_eval_gpt4`, on prior
 evaluators (`aviary_gpt4`, `lmsys_gpt4`, `alpaca_farm_greedy_gpt4`), and on different base models with which we use
 essentially the same prompt (`gpt4`, `text_davinci_003`, `claude`, `chatgpt`).
+We also provide partial metrics (only 1 seed) for other evaluators, which include our evaluator using OpenAI's function
+calls (`alpaca_eval_gpt4_fn`), prior work that we
+improved (`improved_aviary_gpt4` and `improved_lmsys_gpt4`), prior work that was not meant to be used as a final
+evaluator (`guanaco_33b`), and a ranking evaluator (`alpaca_farm`), and secondary models that use the same prompt as the
+models above (`cohere`, `guanaco_33b`):
 
 |                         | Human agreement [%] | Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer longer | Proba. prefer lists | Proba. prefer 1 | # parsed | mode     |
 |:------------------------|--------------------:|------------------------:|-----------------------------:|-----:|---------:|---------------------:|--------------------:|----------------:|---------:|:---------|
+| alpaca_eval_gpt4_fn     |                71.0 |                    14.5 |                         5046 | 27.6 |     11.1 |                 0.75 |                0.63 |            0.48 |     2592 | verified |
+| improved_aviary_gpt4    |                69.8 |                    12.8 |                         1831 |      |          |                 0.73 |                0.68 |            0.49 |      648 | verified |
 | alpaca_eval_gpt4        |                69.2 |                    13.6 |                         1455 | 28.4 |     14.6 |                 0.68 |                0.69 |            0.50 |     2592 | minimal  |
 | aviary_gpt4             |                69.1 |                    12.8 |                         1869 | 29.5 |     13.1 |                 0.70 |                0.65 |            0.53 |     2592 | minimal  |
+| claude_ranking          |                67.6 |                     5.0 |                          218 |      |          |                 0.73 |                0.63 |            0.46 |      648 | verified |
 | gpt4                    |                66.9 |                    12.5 |                         1037 | 31.5 |     14.6 |                 0.65 |                0.61 |            0.54 |     2592 | minimal  |
 | alpaca_farm_greedy_gpt4 |                66.4 |                    15.3 |                          878 | 30.2 |     19.3 |                 0.60 |                0.59 |            0.54 |     2592 | minimal  |
-| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |          |                 0.64 |                0.61 |            0.52 |     2592 | minimal  |
+| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |     34.3 |                 0.64 |                0.61 |            0.52 |     2592 | minimal  |
 | claude                  |                65.5 |                    11.1 |                          173 | 31.9 |     18.0 |                 0.62 |                0.58 |            0.49 |     2592 | minimal  |
 | text_davinci_003        |                64.1 |                     8.7 |                          121 | 33.8 |     22.7 |                 0.70 |                0.64 |            0.47 |     2592 | minimal  |
 | lmsys_gpt4              |                63.2 |                    13.9 |                        17982 | 34.7 |     16.1 |                 0.74 |                0.64 |            0.56 |     2592 | minimal  |
+| guanaco_33b             |                62.7 |                         |                          911 |      |          |                 0.70 |                0.72 |            0.43 |      451 | verified |
+| improved_lmsys_gpt4     |                62.3 |                    13.9 |                         5398 |      |          |                 0.75 |                0.67 |            0.51 |      648 | verified |
 | longest                 |                62.2 |                     0.0 |                            0 | 37.8 |      0.0 |                 1.00 |                0.85 |            0.42 |     2592 | verified |
+| alpaca_farm             |                60.0 |                    11.5 |                          820 |      |          |                 0.60 |                0.63 |            0.52 |      648 | verified |
+| chatgpt_fn              |                60.0 |                     1.0 |                          530 | 36.9 |     27.7 |                 0.62 |                0.65 |            0.49 |     2592 | minimal  |
 | chatgpt                 |                57.2 |                     0.8 |                          285 | 39.4 |     34.1 |                 0.59 |                0.56 |            0.49 |     2589 | minimal  |
-
-We also provide partial metrics (only 1 seed) for the following evaluators, which include prior work that we
-improved (`improved_aviary_gpt4` and `improved_lmsys_gpt4`), prior work that was not meant to be used as a final
-evaluator (`guanaco_33b`), and a ranking evaluator (`alpaca_farm`), and secondary models that use the same prompt as the
-models above (`cohere`, `guanaco_33b`):
-
-|                      | Human agreement [%] | Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer longer | Proba. prefer lists | Proba. prefer 1 | # parsed | mode     |
-|:---------------------|--------------------:|------------------------:|-----------------------------:|-----:|---------:|---------------------:|--------------------:|----------------:|---------:|:---------|
-| improved_aviary_gpt4 |                69.8 |                    12.8 |                         1831 |      |          |                 0.73 |                0.68 |            0.49 |      648 | verified |
-| claude_ranking       |                67.6 |                     5.0 |                          218 |      |          |                 0.73 |                0.63 |            0.46 |      648 | verified |
-| guanaco_33b          |                62.7 |                         |                          911 |      |          |                 0.70 |                0.72 |            0.43 |      451 | verified |
-| improved_lmsys_gpt4  |                62.3 |                    13.9 |                         5398 |      |          |                 0.75 |                0.67 |            0.51 |      648 | verified |
-| alpaca_farm          |                60.0 |                    11.5 |                          820 |      |          |                 0.60 |                0.63 |            0.52 |      648 | verified |
-| cohere               |                53.4 |                     3.5 |                          217 |      |          |                 0.50 |                0.51 |            0.47 |      648 | verified |
+| cohere                  |                53.4 |                     3.5 |                          217 |      |          |                 0.50 |                0.51 |            0.47 |      648 | verified |
 
 [//]: # (|                         | Human agreement [%] | Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer longer | Proba. prefer lists | Proba. prefer 1 | # parsed | mode     |)
 
 [//]: # (|:------------------------|--------------------:|------------------------:|-----------------------------:|-----:|---------:|---------------------:|--------------------:|----------------:|---------:|:---------|)
 
 [//]: # (| improved_aviary_gpt4    |                69.8 |                    12.8 |                         1831 |      |          |                 0.73 |                0.68 |            0.49 |      648 | verified |)
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 ,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base
 gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32
 claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89
 chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109
 wizardlm-13b,75.31094527363184,1.5101858292160824,minimal,9,804,601,194
+airoboros-65b,73.91304347826086,1.5285333061227804,verified,16,805,587,202
+airoboros-33b,73.29192546583852,1.55290318216736,verified,6,805,587,212
 guanaco-65b,71.80124223602485,1.586912361158523,minimal,0,805,578,227
 vicuna-13b,70.43478260869566,1.6069688407799696,minimal,2,805,566,237
 oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,minimal,3,805,534,268
+minotaur-13b,66.02484472049689,1.6645545328264226,community,5,805,529,271
 guanaco-33b,65.96273291925466,1.67108537053247,verified,0,805,531,274
 nous-hermes-13b,65.46583850931677,1.669962276077284,verified,6,805,524,275
 vicuna-7b,64.40993788819875,1.6851107260487883,verified,3,805,517,285
-oasst-sft-llama-33b,54.96894409937888,1.7402667933686877,verified,13,805,436,356
+oasst-sft-llama-33b,54.96894409937888,1.7402667933686875,verified,13,805,436,356
 guanaco-13b,52.60869565217391,1.7576690299699242,verified,3,805,422,380
 text_davinci_003,50.0,0.0,minimal,805,805,0,0
 guanaco-7b,46.58385093167702,1.7570464905413992,verified,2,805,374,429
 falcon-40b-instruct,45.71428571428572,1.7524717060805597,minimal,4,805,366,435
 alpaca-farm-ppo-sim-gpt4-20k,44.099378881987576,1.7399772578861137,verified,10,805,350,445
 pythia-12b-mix-sft,41.86335403726708,1.737637146007538,verified,2,805,336,467
 alpaca-farm-ppo-human,41.24223602484472,1.7271813123250834,minimal,8,805,328,469
+cohere-chat,29.565217391304348,1.5949050483247118,community,12,805,232,561
+cohere,28.385093167701864,1.5717547121761728,community,15,805,221,569
 alpaca-7b,26.459627329192543,1.535711469748,minimal,16,805,205,584
 oasst-sft-pythia-12b,25.962732919254663,1.5261079289535309,verified,16,805,201,588
 falcon-7b-instruct,23.60248447204969,1.4898235369056625,verified,6,805,187,612
-cohere,17.51552795031056,1.3172551905907428,verified,16,805,133,656
 text_davinci_001,15.17412935323383,1.235107892276849,minimal,20,804,112,672
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files 23% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 text_davinci_003,50.0,0.0,minimal,805,805,0,0
 alpaca-farm-ppo-sim-gpt4-20k,48.19875776397515,1.7512254507446705,verified,10,805,383,412
 guanaco-7b,47.5776397515528,1.7590989434689512,verified,2,805,382,421
 falcon-40b-instruct,46.70807453416149,1.7551420072945083,minimal,4,805,374,427
 alpaca-farm-ppo-human,46.45962732919255,1.750131850347461,minimal,8,805,370,427
 pythia-12b-mix-sft,43.22981366459627,1.7449120766669366,verified,2,805,347,456
 oasst-sft-pythia-12b,32.79503105590062,1.6369108459870174,verified,16,805,256,533
+cohere-chat,32.79503105590062,1.6416235300873216,community,12,805,258,535
+cohere,32.608695652173914,1.635641080422956,community,15,805,255,535
 alpaca-7b,32.298136645962735,1.630307861230374,minimal,16,805,252,537
 falcon-7b-instruct,29.565217391304348,1.6021542242903124,verified,6,805,235,564
-cohere,27.45341614906832,1.554147922736176,verified,16,805,213,576
 text_davinci_001,21.490683229813666,1.421716368655911,minimal,20,805,163,622
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 ,Human agreement [%],Price [$/1000 examples],Time [seconds/1000 examples],Bias,Variance,Proba. prefer longer,Proba. prefer lists,Proba. prefer 1,# parsed,mode
+alpaca_eval_gpt4_fn,70.98765432098766,14.471944444444444,5046.056233910331,27.623456790123456,11.111111111111104,0.750561797752809,0.6339285714285714,0.4799382716049383,2592,verified
 improved_aviary_gpt4,69.75308641975309,12.781435185185186,1831.2850013,,,0.7280898876404495,0.6785714285714286,0.4861111111111111,648,verified
 alpaca_eval_gpt4,69.1743827160494,13.601944444444444,1455.4169713998845,28.395061728395067,14.621913580246916,0.6831460674157304,0.6875,0.5011574074074074,2592,minimal
 aviary_gpt4,69.05864197530865,12.781666666666668,1868.680324340008,29.475308641975307,13.117283950617288,0.701123595505618,0.6517857142857143,0.533179012345679,2592,minimal
 claude_ranking,67.5925925925926,4.954578395061729,218.4230414438272,,,0.7303370786516854,0.6339285714285714,0.4552469135802468,648,verified
 gpt4,66.93672839506173,12.452592592592593,1036.788589334915,31.48148148148148,14.621913580246904,0.647191011235955,0.6071428571428571,0.5397376543209877,2592,minimal
 alpaca_farm_greedy_gpt4,66.43518518518519,15.28163425925926,877.6250469425926,30.246913580246915,19.29012345679012,0.597752808988764,0.5892857142857143,0.5362654320987654,2592,minimal
 humans,65.66358024691358,300.0,36800.00000000001,0.0,34.336419753086425,0.6359550561797753,0.6071428571428571,0.5177469135802468,2592,minimal
 claude,65.54783950617283,11.070374409722222,173.0299501764275,31.944444444444443,18.016975308641968,0.6157303370786517,0.5803571428571429,0.4926697530864197,2592,minimal
 text_davinci_003,64.0817901234568,8.712680555439814,120.90134619274691,33.79629629629629,22.72376543209876,0.6966292134831461,0.6428571428571429,0.4733796296296295,2592,minimal
 lmsys_gpt4,63.15586419753087,13.945289351851851,17981.91908101215,34.72222222222222,16.126543209876544,0.7389277389277389,0.6422018348623854,0.5625,2592,minimal
 guanaco_33b,62.74944567627494,,910.8929739450112,,,0.6991150442477876,0.7195121951219512,0.4257206208425721,451,verified
 improved_lmsys_gpt4,62.34567901234568,13.938055555555556,5397.837981725772,,,0.7534883720930232,0.6727272727272727,0.5138888888888888,648,verified
 longest,62.19135802469136,0.0,0.0,37.808641975308646,0.0,1.0,0.8482142857142857,0.4166666666666667,2592,verified
 alpaca_farm,60.03086419753087,11.547508744135802,820.2330700344137,,,0.6,0.6339285714285714,0.5246913580246915,648,verified
+chatgpt_fn,59.992283950617285,1.0088333333333337,529.928419875,36.88271604938272,27.73919753086419,0.6247191011235955,0.6517857142857143,0.4911265432098766,2592,minimal
 chatgpt,57.21450617283951,0.8342726921591347,284.9753823429895,39.35185185185185,34.080370942812976,0.5910112359550562,0.5625,0.488991888760139,2589,minimal
 cohere,53.39506172839506,3.452932098765432,216.8668793200617,,,0.503370786516854,0.5089285714285714,0.4737654320987654,648,verified
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/main.py` & `alpaca_eval-0.1.5/src/alpaca_eval/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         precomputed_leaderboard: Optional[Union[str, AnyPath, AnyData]] = "auto",
         is_overwrite_leaderboard: bool = False,
         leaderboard_mode_to_print: Optional[str] = "minimal",
         current_leaderboard_mode: str = "community",
         is_return_instead_of_print: bool = False,
         fn_metric: Union[str, callable] = "pairwise_to_winrate",
         sort_by: str = "win_rate",
-        is_cache_leaderboard: Optional[bool] = False,
+        is_cache_leaderboard: Optional[bool] = None,
         max_instances: Optional[int] = None,
         annotation_kwargs: Optional[dict[str, Any]] = None,
         **annotator_kwargs,
 ):
     """Evaluate a model based on its outputs. This is the default entrypoint if no command is specified.
 
     Parameters
@@ -93,30 +93,33 @@
 
     annotation_kwargs : dict, optional
         Additional arguments to pass to `PairwiseAnnotator.annotate_head2head`.
 
     annotator_kwargs :
         Additional arguments to pass to `PairwiseAnnotator`.
     """
-    if isinstance(current_leaderboard_mode,
-                  str) and current_leaderboard_mode not in constants.ORDERED_LEADERBOARD_MODES:
+    if (
+            isinstance(current_leaderboard_mode, str)
+            and current_leaderboard_mode not in constants.ORDERED_LEADERBOARD_MODES
+    ):
         raise ValueError(f"current_leaderboard_mode should be one of {constants.ORDERED_LEADERBOARD_MODES}")
 
     annotation_kwargs = annotation_kwargs or dict()
 
-    leaderboard = utils.get_precomputed_leaderboard(precomputed_leaderboard, reference_outputs, annotators_config)
+    leaderboard, precomputed_leaderboard = utils.get_precomputed_leaderboard(
+        precomputed_leaderboard, reference_outputs, annotators_config
+    )
     annotations = None
 
     if model_outputs is not None:
         model_outputs = utils.load_or_convert_to_dataframe(model_outputs)
         reference_outputs = utils.load_or_convert_to_dataframe(reference_outputs)
         name = utils.get_generator_name(name, model_outputs)
 
         if (name not in leaderboard) or is_overwrite_leaderboard:
-
             logging.info(f"Evaluating the {name} outputs.")
 
             if max_instances is not None:
                 model_outputs = model_outputs[:max_instances]
                 reference_outputs = reference_outputs[:max_instances]
 
             annotator = annotators.PairwiseAnnotator(annotators_config=annotators_config, **annotator_kwargs)
@@ -130,15 +133,15 @@
             leaderboard[name] = fn_metric(preferences=[a["preference"] for a in annotations])
             leaderboard[name]["mode"] = current_leaderboard_mode
         else:
             logging.info(f"Skipping evaluation of {name} as it is already in the precomputed leaderboard.")
 
     output_path = utils.get_output_path(output_path, model_outputs, name)
 
-    df_leaderboard = pd.DataFrame.from_dict(leaderboard, orient='index').sort_values(by=sort_by, ascending=False)
+    df_leaderboard = pd.DataFrame.from_dict(leaderboard, orient="index").sort_values(by=sort_by, ascending=False)
     df_leaderboard = df_leaderboard[
         utils.prioritize_elements(list(df_leaderboard.columns), ["win_rate", "standard_error"])
     ]
 
     if output_path is not None:
         logging.info(f"Saving all results to {output_path}")
         df_leaderboard.to_csv(output_path / "leaderboard.csv")
@@ -147,24 +150,32 @@
                 output_path / "annotations.json", orient="records", indent=2
             )
 
     if is_cache_leaderboard is None:
         is_cache_leaderboard = max_instances is None
 
     if is_cache_leaderboard:
-        logging.info(f"Saving result to the precomputed leaderboard at {precomputed_leaderboard}")
-        df_leaderboard.to_csv(precomputed_leaderboard)
+        if isinstance(precomputed_leaderboard, AnyPath):
+            logging.info(f"Saving result to the precomputed leaderboard at {precomputed_leaderboard}")
+            df_leaderboard.to_csv(precomputed_leaderboard)
+        else:
+            logging.info(
+                f"Not saving the result to the cached leaderboard because precomputed_leaderboard is not a "
+                f"path but {type(precomputed_leaderboard)}."
+            )
 
     if is_return_instead_of_print:
         return df_leaderboard, annotations
     else:
-        utils.print_leaderboard(df_leaderboard,
-                                leaderboard_mode_to_print,
-                                current_name=name,
-                                cols_to_print=["win_rate", "standard_error", "n_total"])
+        utils.print_leaderboard(
+            df_leaderboard,
+            leaderboard_mode_to_print,
+            current_name=name,
+            cols_to_print=["win_rate", "standard_error", "n_total"],
+        )
 
 
 def evaluate_from_model(
         model_configs: Union[AnyPath, dict],
         reference_model_configs: Optional[Union[AnyPath, dict]] = None,
         evaluation_dataset: Union[AnyPath, AnyData, Callable] = constants.ALPACAEVAL_REFERENCE_OUTPUTS,
         annotators_config: AnyPath = DEFAULT_CONFIGS,
@@ -339,17 +350,17 @@
 
     leaderboard = utils.load_or_convert_to_dataframe(leaderboard_path)
     df_leaderboard = pd.DataFrame(leaderboard)
 
     if is_return_instead_of_print:
         return df_leaderboard, all_annotations
     else:
-        utils.print_leaderboard(df_leaderboard,
-                                leaderboard_mode=None,
-                                cols_to_print=["win_rate", "standard_error", "n_total"])
+        utils.print_leaderboard(
+            df_leaderboard, leaderboard_mode=None, cols_to_print=["win_rate", "standard_error", "n_total"]
+        )
 
 
 def analyze_evaluators(
         annotators_config: Optional[AnyPath] = DEFAULT_CONFIGS,
         Annotator=annotators.PairwiseAnnotator,
         analyzer_kwargs=None,
         precomputed_leaderboard: Optional[Union[AnyPath, AnyData]] = CUR_DIR
@@ -431,41 +442,43 @@
                     is_single_annotator=is_single_annotator,
                 )
 
             leaderboard[key] = analyze.get_metrics_evaluator(analyzer, df_crossannotations, evaluator_name=key)
             leaderboard[key]["mode"] = current_leaderboard_mode
             all_crossannotations[key] = df_crossannotations
 
-    df_leaderboard = pd.DataFrame.from_dict(leaderboard, orient='index').sort_values(by="Human agreement [%]",
-                                                                                     ascending=False)
+    df_leaderboard = pd.DataFrame.from_dict(leaderboard, orient="index").sort_values(
+        by="Human agreement [%]", ascending=False
+    )
 
     df_leaderboard = df_leaderboard[
         utils.prioritize_elements(list(df_leaderboard.columns), constants.EVALUATORS_LEADERBOARD_COLS_TO_PRIORITIZE)
     ]
 
     if is_save_leaderboard:
         df_leaderboard.to_csv(precomputed_leaderboard)
 
     if is_return_instead_of_print:
         return df_leaderboard, all_crossannotations
     else:
-        utils.print_leaderboard(df_leaderboard, leaderboard_mode_to_print,
-                                cols_to_print=constants.EVALUATORS_LEADERBOARD_COLS_TO_PRINT)
+        utils.print_leaderboard(
+            df_leaderboard, leaderboard_mode_to_print, cols_to_print=constants.EVALUATORS_LEADERBOARD_COLS_TO_PRINT
+        )
 
 
 ALL_FUNCTIONS = {
-    'evaluate': evaluate,
-    'evaluate_from_model': evaluate_from_model,
-    'make_leaderboard': make_leaderboard,
-    'analyze_evaluators': analyze_evaluators,
+    "evaluate": evaluate,
+    "evaluate_from_model": evaluate_from_model,
+    "make_leaderboard": make_leaderboard,
+    "analyze_evaluators": analyze_evaluators,
 }
 
 
 def main():
-    is_fn_name = (len(sys.argv) > 1 and "--" not in sys.argv[1])
+    is_fn_name = len(sys.argv) > 1 and "--" not in sys.argv[1]
     is_help = any(a == "--help" for a in sys.argv)
 
     if is_fn_name or is_help:
         fire.Fire(ALL_FUNCTIONS)
     else:
         # default behavior if no function is specified
         fire.Fire(evaluate)
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/metrics.py` & `alpaca_eval-0.1.5/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/plotting.py` & `alpaca_eval-0.1.5/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval/utils.py` & `alpaca_eval-0.1.5/src/alpaca_eval/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,20 +38,22 @@
 
         logging.warning(f"Returning input because file not found. Error: {e}")
         out = to_read
 
     return out
 
 
-def random_seeded_choice(seed: Union[int, str, float], choices):
+def random_seeded_choice(seed: Union[int, str, float], choices, **kwargs):
     """Random choice with a (potentially string) seed."""
-    return random.Random(seed).choice(choices)
+    return random.Random(seed).choices(choices, k=1, **kwargs)[0]
 
 
-def shuffle_pairwise_preferences(df: pd.DataFrame, arr_is_shuffle: Sequence[int]) -> pd.DataFrame:
+def shuffle_pairwise_preferences(
+    df: pd.DataFrame, arr_is_shuffle: Sequence[int]
+) -> pd.DataFrame:
     """Shuffle the outputs of a pairwise preference dataframe.
 
     Examples
     --------
     >>> df = pd.DataFrame([dict(instruction='2+2', output_1='3', output_2='4', preference=2),
                            dict(instruction='2+3', output_1='5', output_2='4', preference=1)])
     >>> print(shuffle_pairwise_preferences(df, [True, False]))
@@ -61,15 +63,17 @@
     """
     col_1 = df["output_1"].copy()
     col_2 = df["output_2"].copy()
     df["output_1"] = np.where(arr_is_shuffle, col_2, col_1)
     df["output_2"] = np.where(arr_is_shuffle, col_1, col_2)
 
     if "preference" in df.columns:
-        df["preference"] = np.where(arr_is_shuffle, 3 - df["preference"], df["preference"])
+        df["preference"] = np.where(
+            arr_is_shuffle, 3 - df["preference"], df["preference"]
+        )
 
     return df
 
 
 def is_derangement(arr1, arr2):
     """Whether 2 arrays are derangements of one another"""
     return all([a != b for a, b in zip(arr1, arr2)])
@@ -90,15 +94,17 @@
 
     for _ in range(max_loop):
         rng.shuffle(shuffled)
         if is_derangement(idcs, shuffled):
             return arr[shuffled]
 
     # if no luck then computes all possibilities
-    deranged_order = list(set([s for s in itertools.permutations(idcs) if is_derangement(s, idcs)]))
+    deranged_order = list(
+        set([s for s in itertools.permutations(idcs) if is_derangement(s, idcs)])
+    )
     return arr[list(rng.choice(deranged_order))]
 
 
 def _find_first_match(text: str, outputs_to_match: dict[str, Any]) -> tuple[Any, Any]:
     """Given text to parse and a dictionary of compiled regex to match, return the first match and corresponding key."""
     first_match = None
     first_key = None
@@ -109,15 +115,15 @@
             first_match = match
             first_key = key
 
     return first_match, first_key
 
 
 def make_prompts(
-        df: pd.DataFrame, template: str, batch_size: int = 1, padding_example=DUMMY_EXAMPLE
+    df: pd.DataFrame, template: str, batch_size: int = 1, padding_example=DUMMY_EXAMPLE
 ) -> tuple[list[str], pd.DataFrame]:
     """Helper function to make batch prompts for a single template.
 
     Parameters
     ----------
     df : pd.DataFrame
         Examples to annotate
@@ -153,15 +159,17 @@
     if df.empty:
         return [], df
 
     text_to_format = re.findall("{([^ \s]+?)}", template)
     n_occurrences = Counter(text_to_format)
 
     if not all([n == batch_size for n in n_occurrences.values()]):
-        raise ValueError(f"All placeholders should be repeated batch_size={batch_size} times but {n_occurrences}.")
+        raise ValueError(
+            f"All placeholders should be repeated batch_size={batch_size} times but {n_occurrences}."
+        )
 
     # padding if you don't have enough examples
     n_to_pad = (batch_size - len(df)) % batch_size
     padding = pd.DataFrame([padding_example] * n_to_pad)
     padding["is_padding"] = True
     df_out = pd.concat([df, padding], axis=0, ignore_index=True)
     df_out["is_padding"] = df_out["is_padding"].fillna(False)
@@ -169,24 +177,26 @@
     prompts = []
     # ugly for loops, not trivial to vectorize because of the batching
     for i in range(0, len(df_out), batch_size):
         current_prompt = copy.deepcopy(template)
         for j in range(batch_size):
             for to_format in n_occurrences.keys():
                 # replace only first occurrence (that's why we don't use .format)
-                current_prompt = current_prompt.replace("{" + to_format + "}", str(df_out.iloc[i + j][to_format]), 1)
+                current_prompt = current_prompt.replace(
+                    "{" + to_format + "}", str(df_out.iloc[i + j][to_format]), 1
+                )
         prompts.append(current_prompt)
 
     return prompts, df_out
 
 
 def convert_ordinal_to_binary_preference(
-        preferences: Union[pd.DataFrame, list[dict[str, Any]]],
-        ordinal_preference_key: str = "preference",
-        binary_preference_key: str = "preference",
+    preferences: Union[pd.DataFrame, list[dict[str, Any]]],
+    ordinal_preference_key: str = "preference",
+    binary_preference_key: str = "preference",
 ):
     """Convert ordinal preference annotations to preference annotations. By merging multiple subcategories together,
     eg A/a/b/B into A/B, or AA/A/a/b/B/BB into A/B.
 
     Parameters
     ----------
     preferences : pd.DataFrame or list of dicts
@@ -222,15 +232,17 @@
     """
     if isinstance(preferences, pd.DataFrame):
         is_df = True
     else:
         is_df = False
         preferences = pd.DataFrame.from_records(preferences)
 
-    preferences[binary_preference_key] = (preferences[ordinal_preference_key].round().astype(int) - 1) // 2 + 1
+    preferences[binary_preference_key] = (
+        preferences[ordinal_preference_key].round().astype(int) - 1
+    ) // 2 + 1
 
     if not is_df:
         preferences = preferences.to_dict(orient="records")
 
     return preferences
 
 
@@ -257,15 +269,15 @@
 
 
 def load_or_convert_to_dataframe(df=Union[AnyPath, AnyData, Callable], **kwargs):
     """Load a dataframe from a path or convert the input to a dataframe if it's not a path."""
     if isinstance(df, Callable):
         df = df(**kwargs)
 
-    if isinstance(df, AnyPath):
+    if isinstance(df, (str, os.PathLike, pathlib.Path)):
         df = Path(df)
 
         # check if it's a globbing pattern
         if "*" in str(df):
             df = pd.concat(
                 [load_or_convert_to_dataframe(f, **kwargs) for f in glob.glob(str(df))],
             )
@@ -306,15 +318,17 @@
 
 
 @contextlib.contextmanager
 def silent():
     """Context manager to remove all outputs and warnings."""
     import IPython
 
-    with open(os.devnull, "w") as f, contextlib.redirect_stdout(f), DisableLogger(), IPython.utils.io.capture_output():
+    with open(os.devnull, "w") as f, contextlib.redirect_stdout(
+        f
+    ), DisableLogger(), IPython.utils.io.capture_output():
         yield
 
 
 class DisableLogger:
     def __enter__(self):
         logging.disable(50)
 
@@ -365,40 +379,48 @@
                 configs = yaml.safe_load(stream)
             except yaml.YAMLError as exc:
                 logging.exception(exc)
 
     return configs
 
 
-def get_precomputed_leaderboard(precomputed_leaderboard, reference_outputs, annotators_config):
+def get_precomputed_leaderboard(
+    precomputed_leaderboard, reference_outputs, annotators_config
+):
     if precomputed_leaderboard == "auto":
         try:
             precomputed_leaderboard = constants.PRECOMPUTED_LEADERBOARDS[
                 (str(reference_outputs), str(annotators_config))
             ]
         except KeyError:
             try:
                 if Path(reference_outputs).is_absolute():
                     logging.warning(
                         f"precomputed_leaderboard = 'auto'. But we have found no corresponding leaderboard for"
                         f" {reference_outputs} and {annotators_config}"
                     )
             except:
-                logging.warning(f"precomputed_leaderboard = 'auto'. But we have found no corresponding leaderboard")
+                logging.warning(
+                    f"precomputed_leaderboard = 'auto'. But we have found no corresponding leaderboard"
+                )
             precomputed_leaderboard = None
 
     if precomputed_leaderboard is not None:
         try:
-            leaderboard = load_or_convert_to_dataframe(precomputed_leaderboard).to_dict(orient="index")
+            leaderboard = load_or_convert_to_dataframe(precomputed_leaderboard).to_dict(
+                orient="index"
+            )
         except FileNotFoundError:
-            logging.warning(f"precomputed_leaderboard = {precomputed_leaderboard} not found => computing from scratch.")
+            logging.warning(
+                f"precomputed_leaderboard = {precomputed_leaderboard} not found => computing from scratch."
+            )
             leaderboard = dict()
     else:
         leaderboard = dict()
-    return leaderboard
+    return leaderboard, precomputed_leaderboard
 
 
 def get_output_path(output_path, model_outputs, name):
     if output_path == "auto":
         if model_outputs is None:
             output_path = None
         else:
@@ -410,24 +432,28 @@
                 else:
                     output_path = "."
     if output_path is not None:
         output_path = Path(output_path)
         output_path.mkdir(exist_ok=True, parents=True)
 
 
-def print_leaderboard(df_leaderboard, leaderboard_mode, cols_to_print, current_name=None):
+def print_leaderboard(
+    df_leaderboard, leaderboard_mode, cols_to_print, current_name=None
+):
     cols_to_print = list(cols_to_print)
-    
+
     if leaderboard_mode is not None:
         if "mode" in df_leaderboard.columns:
             # select all modes that come before
             current_idx = constants.ORDERED_LEADERBOARD_MODES.index(leaderboard_mode)
-            df_leaderboard["mode_idx"] = df_leaderboard["mode"].apply(constants.ORDERED_LEADERBOARD_MODES.index)
+            df_leaderboard["mode_idx"] = df_leaderboard["mode"].apply(
+                constants.ORDERED_LEADERBOARD_MODES.index
+            )
 
-            is_smaller_mode = (df_leaderboard["mode_idx"] <= current_idx)
+            is_smaller_mode = df_leaderboard["mode_idx"] <= current_idx
             is_selected = is_smaller_mode | (df_leaderboard["mode"].isnull())
 
             if current_name is not None:
                 is_selected |= df_leaderboard.index == current_name
 
             df_leaderboard = df_leaderboard[is_selected]
     elif "mode" in df_leaderboard.columns:
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.1.5/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.1.3
+Version: 0.1.5
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -22,27 +22,28 @@
 License-File: LICENSE
 
 # <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
 [![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
-[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE)
+[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
 Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
 AlpacaEval provides the following:
 
 - [**Automatic evaluator**](#evaluators): an automatic evaluator that has high agreement with humans (validated on 20K
   annotations). We evaluate a
   model by
-  measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs from that model over
+  measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that model
+  over
   outputs from a reference model. Our evaluators enable caching and output randomization by default.
 - [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
   evaluation set.
 - [**Toolkit for building automatic evaluators**](#analysis): a simple interface for
   building advanced automatic evaluators (e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
   price, speed, statistical power, bias, variance etc).
 - [**Human evaluation data**](#data-release): 20K human preferences between a given and reference model
@@ -86,14 +87,15 @@
     - [Contributing an eval set](#contributing-an-eval-set)
 6. [Limitations](#limitations)
 7. [Citation](#citation)
 8. [Additional information](#additional-information)
     - [Data Release](#data-release)
     - [Differences with AlpacaFarm](#differences-with-alpacafarm)
     - [Related work](#related-work)
+    - [Major updates](#major-updates)
 
 </details>
 
 # Quick Start
 
 To install the stable release, run
 
@@ -116,19 +118,20 @@
 ```
 
 Important parameters are the following:
 
 - **model_outputs** : A path to a json file for the outputs of the model to add to the leaderboard. Each dictionary
   should
   contain the keys `instruction` and `output`.
-- **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`). `alpaca_eval_gpt4` (
+- **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`
+  or `chatgpt_fn`). `alpaca_eval_gpt4` (
   default) has the
-  highest agreement rate with our human annotation data. `claude` has a decent agreement and is free for academics. For
-  a comparison of
-  annotators see [here](#evaluators).
+  highest agreement rate with our human annotation data. `claude` has a decent agreement and is free for
+  academics. `chatgpt_fn` is the worst of the three, but is available to everyone, cheap, and has 2x larger context
+  window (16K tokens). For a comparison of annotators see [here](#evaluators).
 - **reference_outputs**:  The outputs of the reference model. Same format as `model_outputs`. By default, this
   is `text-davinci003` outputs on
   AlpacaEval dataset.
 - **output_path**: Path for saving annotations and leaderboard.
 
 If you don't have the model outputs, you can
 use [`evaluate_from_model`](https://github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and
@@ -164,16 +167,17 @@
 For more information about each function use `alpaca_eval <command> -- --help`.
 
 # Leaderboards and how to interpret them
 
 ## Models
 
 Our leaderboards are computed on the [AlpacaEval dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval).
-We precomputed the leaderboard for important models both using `gpt4` (best quality) and  `claude` (free for academics,
-and high quality). Our full leaderboards can be found at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but
+We precomputed the leaderboard for important models using `alpaca_eval_gpt4` (best quality),  `claude` (free for
+academics, and high quality), and `chatgpt_fn` (cheap and available for everyone). Our full leaderboards can be found
+at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but
 we give minimal leaderboards below.
 Later we also show how to [add your model](https://github.com/tatsu-lab/alpaca_eval#evaluating-a-model) to the
 leaderboard and how to make
 a [new leaderboard for your evaluator/dataset](https://github.com/tatsu-lab/alpaca_eval#making-a-new-leaderboard).
 See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) for the configs of all
 models that are available out of the box.
 
@@ -260,38 +264,58 @@
 | falcon-40b-instruct   |     46.7 |       1.8 |
 | alpaca-farm-ppo-human |     46.5 |       1.8 |
 | alpaca-7b             |     32.3 |       1.6 |
 | text_davinci_001      |     21.5 |       1.4 |
 
 </details>
 
+<details>
+  <summary><b><code>chatgpt_fn</code> minimal leaderboard</b></summary>
+
+|                       | Win Rate | Std Err. |
+|:----------------------|---------:|---------:|
+| gpt4                  |     73.8 |      1.5 |
+| claude                |     70.4 |      1.6 |
+| chatgpt               |     66.1 |      1.7 |
+| wizardlm-13b          |     65.2 |      1.7 |
+| vicuna-13b            |     64.1 |      1.7 |
+| guanaco-65b           |     62.4 |      1.7 |
+| oasst-rlhf-llama-33b  |     62.0 |      1.7 |
+| alpaca-farm-ppo-human |     60.2 |      1.7 |
+| falcon-40b-instruct   |     56.5 |      1.7 |
+| text_davinci_003      |     50.0 |      0.0 |
+| alpaca-7b             |     45.2 |      1.7 |
+| text_davinci_001      |     28.1 |      1.6 |
+
+</details>
+
 ## Evaluators
 
 We evaluate different automatic annotators on the AlpacaEval set by comparing to
 2.5K [human annotations](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/main/alpaca_farm_human_crossannotations.json)
 we collected (~650 instructions each with 4 human annotations).
 Below we show metrics for our suggested evaluator (`alpaca_eval_gpt4`), for prior
 automatic
 evaluators ([`alpaca_farm_greedy_gpt4`](https://github.com/tatsu-lab/alpaca_farm),[`aviary_gpt4`](https://aviary.anyscale.com/),[`lmsys_gpt4`](https://chat.lmsys.org/)),
 for humans (`humans`), and for different base models with essentially the same
-prompt (`gpt4`,`claude`,`text_davinci_003`,`guanaco_33b`, `chatgpt`).
+prompt (`gpt4`,`claude`,`text_davinci_003`,`chatgpt_fn`,`guanaco_33b`, `chatgpt`).
 See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs) for the configs of all
 evaluators that are available out of the box and their associated metrics.
 
 |                         | Human agreement [%] | Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer longer |
 |:------------------------|--------------------:|------------------------:|-----------------------------:|-----:|---------:|---------------------:|
 | alpaca_eval_gpt4        |                69.2 |                    13.6 |                         1455 | 28.4 |     14.6 |                 0.68 |
 | aviary_gpt4             |                69.1 |                    12.8 |                         1869 | 29.5 |     13.1 |                 0.70 |
 | gpt4                    |                66.9 |                    12.5 |                         1037 | 31.5 |     14.6 |                 0.65 |
 | alpaca_farm_greedy_gpt4 |                66.4 |                    15.3 |                          878 | 30.2 |     19.3 |                 0.60 |
-| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |          |                 0.64 |
+| humans                  |                65.7 |                   300.0 |                        36800 |  0.0 |     34.3 |                 0.64 |
 | claude                  |                65.5 |                    11.1 |                          173 | 31.9 |     18.0 |                 0.62 |
 | text_davinci_003        |                64.1 |                     8.7 |                          121 | 33.8 |     22.7 |                 0.70 |
 | lmsys_gpt4              |                63.2 |                    13.9 |                        17982 | 34.7 |     16.1 |                 0.74 |
-| guanaco_33b             |                59.1 |                         |                          930 | 54.5 |     27.1 |                 0.70 |
+| chatgpt_fn              |                60.0 |                     1.0 |                          530 | 36.9 |     27.7 |                 0.62 |
 | chatgpt                 |                57.2 |                     0.8 |                          285 | 39.4 |     34.1 |                 0.59 |
 
 <details>
   <summary><b>How exactly are those metrics computed?</b></summary>
 
 We now explain in words how we compute the metrics in the table
 above. [The code is here](https://github.com/tatsu-lab/alpaca_eval/blob/f05cbd651b79ac93906b19d01fe443b45828b0f2/src/alpaca_eval/analyze.py#L366).
@@ -379,16 +403,17 @@
 due to resource (time and price) constraints. This explains why the #parsed is 648, otherwise it should be 2592.
 
 </details>
 
 <details>
   <summary><b>Tips for choosing evaluators</b></summary>
 
-Overall we recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest agreement with humans, and
-`annotators_config=claude` if you have academic (free) access to Claude and have a low budget.
+Overall we recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest agreement with humans,
+`annotators_config=claude` if you have academic (free) access to Claude and have a low budget, and
+`annotators_config=chatgpt_fn` if you don't have access to the other two models.
 
 When choosing an annotator we recommend you to consider the following (the first three are obvious):
 
 - `"Human agreement [%]"`
 - `"Price [$/1000 examples]"`
 - `"Time [seconds/1000 examples]"`
 - `"Proba. prefer longer"` approx. < 0.7. Indeed, we found see that the majority of preference of human annotators have
@@ -453,15 +478,15 @@
 
 [//]: # ()
 
 [//]: # (4. test your installation &#40;assuming you have OpenAI)
 
 [//]: # ()
 
-[//]: # (   key&#41; `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config 'text_davinci_003' --max_instances 3 --caching_path None`)
+[//]: # (   key&#41; `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config 'text_davinci_003' ~~--max_instances 3~~ --caching_path None`)
 
 [//]: # ()
 
 [//]: # (</details>)
 
 ## Evaluating a model
 
@@ -535,15 +560,15 @@
 rn a dictionary of metrics and the key by which to sort the leaderboard.
     -s, --sort_by=SORT_BY
         Type: str
         Default: 'win_rate'
         The key by which to sort the leaderboard.
     --is_cache_leaderboard=IS_CACHE_LEADERBOARD
         Type: Optional
-        Default: False
+        Default: None
         Whether to save the result leaderboard to `precomputed_leaderboard`. If None we save only if max_instances
 . A preferred way of adding models to the leaderboard is to set `precomputed_leaderboard` to the previously saved
 leaderboard at `<output_path>/leaderboard.csv`.
     --max_instances=MAX_INSTANCES
         Type: Optional[Optional]
         Default: None
         The maximum number of instances to annotate. Useful for testing.
@@ -630,15 +655,16 @@
 
 2. Compute the reference outputs `reference_outputs`. By default, we use the outputs of `text-davinci-003` on
    AlpacaEval.
    If you
    want to use a different model or a different dataset follow the same steps as (1.).
 3. Choose an evaluator specified via `annotators_config`. We recommend using `alpaca_eval_gpt4` or `claude` (if you are
    an
-   academic). For options and comparisons see [this table](#evaluators). Depending on the evaluator you might need to
+   academic) or `chatgpt_fn` (if you don't have access to the other two). For options and comparisons
+   see [this table](#evaluators). Depending on the evaluator you might need to
    set the appropriate API_KEY in your environment
    or [here](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/constants.py#L7).
 
 Running all together:
 
 ```bash
 alpaca_eval --model_outputs 'example/outputs.json' \
@@ -1002,53 +1028,58 @@
 colab notebook above.
 
 # Contributing
 
 We are accepting PRs for new models, evaluators, and eval sets, in addition to bug fixes.
 We will update the [leaderboard website](https://tatsu-lab.github.io/alpaca_eval/) regularly with new community
 contributions.
-We have also created a [support discord](https://discord.gg/qVYd69ye) for AlpacaEval in case you run into any issues and
+We have also created a [support discord](https://discord.gg/GJMxJSVZZM) for AlpacaEval in case you run into any issues
+and
 wish to ask help from the community.
 
+To get started, please first fork the repo, and install the package from source `pip install -e .`
+
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing a model</h2></summary>
 
 First, you'll need to add a model config definition in the [models_configs](src/alpaca_eval/models_configs/) folder. As
 an example, you can look at
 the [falcon-7b-instruct yaml](src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml). Please make sure the
 folder name and key name in the yaml match exactly.
 
-Then, please follow the steps in [Evaluating-a-model](#evaluating-a-model) to run inference on the model to produce
+Then, please follow the steps in [Evaluating a model](#evaluating-a-model) to run inference on the model to produce
 outputs on the eval set and score the model according to one of the evaluators.
 An example command may look like:
 
 ```sh
 alpaca_eval evaluate_from_model \
   --model_configs 'falcon-7b-instruct' \
-  --annotators_config 'alpaca_eval_gpt4'
+  --annotators_config 'alpaca_eval_gpt4' 
 ```
 
-After running this command, you should have generated an outputs json and a new entry in the corresponding leaderboard
-file. Please make a PR with the config, outputs file, and updated leaderboard.
+After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
+file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
+with the
+config, outputs file, and updated leaderboard.
 
 </details>
 
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing an evaluator</h2></summary>
 
 Please first follow the directions in [Making a new evaluator](#making-a-new-evaluator).
 Once you're created the annotator config, we ask that you create a new leaderboard for the annotator by evaluating the
 minimal set of models. The outputs for these models can be found by
 downloading [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/main/alpaca_eval_all_outputs.json).
 
 ```bash
 alpaca_eval make_leaderboard \
-  --leaderboard_path <src/alpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \
+  --leaderboard_path src/alpaca_eval/leaderboards/data_AlpacaEval/<evaluator>_leaderboard.csv \
   --all_model_outputs alpaca_eval_all_outputs.json \
-  --annotators_config <path_to_your_config.yaml>
+  --annotators_config <evaluator_config>
 ```
 
 Then, please create a PR with the annotator config and leaderboard csv.
 
 </details>
 
 <details>
@@ -1263,7 +1294,19 @@
   a position bias.
 - [AlpacaFarm Sec. 5.2.](https://arxiv.org/abs/2305.14387)
   and [The False Promise of Imitating Proprietary LLMs](https://arxiv.org/abs/2305.15717) both found that
   automatic
   annotators favor style (e.g. use of list, tone, word choice, length) over factuality.
 
 </details>
+
+
+<details>
+  <summary><h2 tabindex="-1" dir="auto">Major updates</h2></summary>
+
+- 19th June 2023: add leaderboard `chatgpt_fn` that anyone can use (no waiting lists).
+- 19th June 2023: update to
+  use [OpenAI's function calling](https://openai.com/blog/function-calling-and-other-api-updates).
+  Example: [`chatgpt_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/chatgpt_fn)
+  or [`alpaca_eval_gpt4_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn).
+
+</details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.1.3 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.1.5 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -14,38 +14,38 @@
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
 green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
 License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
 red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
 [Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
 www.python.org/downloads/release/python-3100/) [![discord](https://
 img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
-/discord.gg/yKbbQga9WE) Evaluation of instruction-following models (e.g.,
+/discord.gg/GJMxJSVZZM) Evaluation of instruction-following models (e.g.,
 ChatGPT) typically requires human interactions. This is time-consuming,
 expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
 evaluation that is fast, cheap, replicable, and validated against 20K human
 annotations. It is particularly useful for model development. Although we
 improved over prior automatic evaluation pipelines, there are still fundamental
 [limitations](#limitations). AlpacaEval provides the following: - [**Automatic
 evaluator**](#evaluators): an automatic evaluator that has high agreement with
 humans (validated on 20K annotations). We evaluate a model by measuring the
-fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs
-from that model over outputs from a reference model. Our evaluators enable
-caching and output randomization by default. - [**Leaderboard**](https://tatsu-
-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
-evaluation set. - [**Toolkit for building automatic evaluators**](#analysis): a
-simple interface for building advanced automatic evaluators (e.g. with caching,
-batching, or multi-annotators) and analyzing them (quality, price, speed,
-statistical power, bias, variance etc). - [**Human evaluation data**](#data-
-release): 20K human preferences between a given and reference model on the
-[AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
-set. 2.5K of these are cross-annotations (4 humans annotating the same 650
-examples). - [**AlpacaEval dataset**](#data-release): a simplification of
-[AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
-set, where "instructions" and " inputs" are merged into one field, and
-reference outputs are longer. **When to use AlpacaEval?** Our automatic
+fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the
+outputs from that model over outputs from a reference model. Our evaluators
+enable caching and output randomization by default. - [**Leaderboard**](https:/
+/tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the
+AlpacaEval evaluation set. - [**Toolkit for building automatic evaluators**]
+(#analysis): a simple interface for building advanced automatic evaluators
+(e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
+price, speed, statistical power, bias, variance etc). - [**Human evaluation
+data**](#data-release): 20K human preferences between a given and reference
+model on the [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main)
+evaluation set. 2.5K of these are cross-annotations (4 humans annotating the
+same 650 examples). - [**AlpacaEval dataset**](#data-release): a simplification
+of [AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main)
+evaluation set, where "instructions" and " inputs" are merged into one field,
+and reference outputs are longer. **When to use AlpacaEval?** Our automatic
 evaluator is a quick and cheap proxy for human evaluation of simple
 instruction-following tasks. It is useful if you have to run many evaluations
 quickly, e.g., during model development. **When not to use AlpacaEval?** As any
 other automatic evaluator, AlpacaEval should **not replace human evaluation in
 high-stake decision-making**, e.g., to decide on model release. In particular,
 AlpacaEval is limited by the fact that (1) the instructions in the eval set
 might not be representative of advanced usage of LLMs; (2) automatic evaluators
@@ -59,48 +59,51 @@
 4. [Analysis](#additional-analysis-and-plots) - [Analyzing an evaluator]
 (#analyzing-an-evaluator) - [Analyzing an eval set](#analyzing-an-eval-set) 5.
 [Contributing](#contributing) - [Contributing a model](#contributing-a-model) -
 [Contributing an evaluator](#contributing-an-evaluator) - [Contributing an eval
 set](#contributing-an-eval-set) 6. [Limitations](#limitations) 7. [Citation]
 (#citation) 8. [Additional information](#additional-information) - [Data
 Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
-alpacafarm) - [Related work](#related-work)  # Quick Start To install the
-stable release, run ```bash pip install alpaca-eval ``` To install the nightly
-version, run ```bash pip install git+https://github.com/tatsu-lab/alpaca_eval
-``` Then you can use it as follows: ```bash export OPENAI_API_KEY= export
-OPENAI_ORGANIZATION_IDS= # Optional; if not set, this will be your default org
-id. alpaca_eval --model_outputs 'example/outputs.json' ``` Important parameters
-are the following: - **model_outputs** : A path to a json file for the outputs
-of the model to add to the leaderboard. Each dictionary should contain the keys
-`instruction` and `output`. - **annotators_config**: This is the annotator to
-use (e.g., `alpaca_eval_gpt4` or `claude`). `alpaca_eval_gpt4` ( default) has
-the highest agreement rate with our human annotation data. `claude` has a
-decent agreement and is free for academics. For a comparison of annotators see
-[here](#evaluators). - **reference_outputs**: The outputs of the reference
-model. Same format as `model_outputs`. By default, this is `text-davinci003`
-outputs on AlpacaEval dataset. - **output_path**: Path for saving annotations
-and leaderboard. If you don't have the model outputs, you can use
-[`evaluate_from_model`](https://github.com/tatsu-lab/alpaca_eval/tree/
-main#evaluating-a-model) and pass a local path or a name of a HuggingFace
-model, or a model from a standard API (OpenAI, Anthropic, Cohere). Other
-commands:  >>> alpaca_eval -- --help ``` SYNOPSIS alpaca_eval COMMAND COMMANDS
-COMMAND is one of the following: evaluate Evaluate a model based on its
-outputs. This is the default entrypoint if no command is specified.
-evaluate_from_model Evaluate a model from HuggingFace or an API provider. This
-is a wrapper around `evaluate` which includes generating from a desired model.
-make_leaderboard Precompute and save an entire leaderboard for a given dataset
-/ evaluator / set of models generations. analyze_evaluators Analyze an
-evaluator (agreement with human, speed, price,...). ```  For more information
-about each function use `alpaca_eval  -- --help`. # Leaderboards and how to
-interpret them ## Models Our leaderboards are computed on the [AlpacaEval
-dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval). We precomputed
-the leaderboard for important models both using `gpt4` (best quality) and
-`claude` (free for academics, and high quality). Our full leaderboards can be
-found at [on this page](https://tatsu-lab.github.io/alpaca_eval/), but we give
-minimal leaderboards below. Later we also show how to [add your model](https://
+alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
+# Quick Start To install the stable release, run ```bash pip install alpaca-
+eval ``` To install the nightly version, run ```bash pip install git+https://
+github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
+export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
+this will be your default org id. alpaca_eval --model_outputs 'example/
+outputs.json' ``` Important parameters are the following: - **model_outputs** :
+A path to a json file for the outputs of the model to add to the leaderboard.
+Each dictionary should contain the keys `instruction` and `output`. -
+**annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4`
+or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default) has the highest
+agreement rate with our human annotation data. `claude` has a decent agreement
+and is free for academics. `chatgpt_fn` is the worst of the three, but is
+available to everyone, cheap, and has 2x larger context window (16K tokens).
+For a comparison of annotators see [here](#evaluators). -
+**reference_outputs**: The outputs of the reference model. Same format as
+`model_outputs`. By default, this is `text-davinci003` outputs on AlpacaEval
+dataset. - **output_path**: Path for saving annotations and leaderboard. If you
+don't have the model outputs, you can use [`evaluate_from_model`](https://
+github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and pass a local
+path or a name of a HuggingFace model, or a model from a standard API (OpenAI,
+Anthropic, Cohere). Other commands:  >>> alpaca_eval -- --help ``` SYNOPSIS
+alpaca_eval COMMAND COMMANDS COMMAND is one of the following: evaluate Evaluate
+a model based on its outputs. This is the default entrypoint if no command is
+specified. evaluate_from_model Evaluate a model from HuggingFace or an API
+provider. This is a wrapper around `evaluate` which includes generating from a
+desired model. make_leaderboard Precompute and save an entire leaderboard for a
+given dataset / evaluator / set of models generations. analyze_evaluators
+Analyze an evaluator (agreement with human, speed, price,...). ```  For more
+information about each function use `alpaca_eval  -- --help`. # Leaderboards
+and how to interpret them ## Models Our leaderboards are computed on the
+[AlpacaEval dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval). We
+precomputed the leaderboard for important models using `alpaca_eval_gpt4` (best
+quality), `claude` (free for academics, and high quality), and `chatgpt_fn`
+(cheap and available for everyone). Our full leaderboards can be found at [on
+this page](https://tatsu-lab.github.io/alpaca_eval/), but we give minimal
+leaderboards below. Later we also show how to [add your model](https://
 github.com/tatsu-lab/alpaca_eval#evaluating-a-model) to the leaderboard and how
 to make a [new leaderboard for your evaluator/dataset](https://github.com/
 tatsu-lab/alpaca_eval#making-a-new-leaderboard). See [here](https://github.com/
 tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) for the configs
 of all models that are available out of the box. **`alpaca_eval_gpt4` minimal
 leaderboard**: | | Win Rate | Std Error | |:----------------------|---------:|-
 ---------:| | gpt4 | 95.3 | 0.7 | | claude | 88.4 | 1.1 | | chatgpt | 86.1 |
@@ -144,40 +147,47 @@
 Aviary. We make changes to Aviary's prompt to decrease the bias for longer
 outputs. Details in [Related work](#related-work).   claude minimal leaderboard
 | | Win Rate | Std Error | |:----------------------|---------:|----------:| |
 gpt4 | 77.0 | 1.5 | | claude | 75.8 | 1.5 | | chatgpt | 67.7 | 1.6 | |
 wizardlm-13b | 66.1 | 1.7 | | vicuna-13b | 63.2 | 1.7 | | guanaco-65b | 62.6 |
 1.7 | | oasst-rlhf-llama-33b | 57.3 | 1.7 | | text_davinci_003 | 50.0 | 0.0 | |
 falcon-40b-instruct | 46.7 | 1.8 | | alpaca-farm-ppo-human | 46.5 | 1.8 | |
-alpaca-7b | 32.3 | 1.6 | | text_davinci_001 | 21.5 | 1.4 |  ## Evaluators We
+alpaca-7b | 32.3 | 1.6 | | text_davinci_001 | 21.5 | 1.4 |   chatgpt_fn minimal
+leaderboard | | Win Rate | Std Err. | |:----------------------|---------:|-----
+----:| | gpt4 | 73.8 | 1.5 | | claude | 70.4 | 1.6 | | chatgpt | 66.1 | 1.7 | |
+wizardlm-13b | 65.2 | 1.7 | | vicuna-13b | 64.1 | 1.7 | | guanaco-65b | 62.4 |
+1.7 | | oasst-rlhf-llama-33b | 62.0 | 1.7 | | alpaca-farm-ppo-human | 60.2 |
+1.7 | | falcon-40b-instruct | 56.5 | 1.7 | | text_davinci_003 | 50.0 | 0.0 | |
+alpaca-7b | 45.2 | 1.7 | | text_davinci_001 | 28.1 | 1.6 |  ## Evaluators We
 evaluate different automatic annotators on the AlpacaEval set by comparing to
 2.5K [human annotations](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/
 blob/main/alpaca_farm_human_crossannotations.json) we collected (~650
 instructions each with 4 human annotations). Below we show metrics for our
 suggested evaluator (`alpaca_eval_gpt4`), for prior automatic evaluators (
 [`alpaca_farm_greedy_gpt4`](https://github.com/tatsu-lab/alpaca_farm),
 [`aviary_gpt4`](https://aviary.anyscale.com/),[`lmsys_gpt4`](https://
 chat.lmsys.org/)), for humans (`humans`), and for different base models with
-essentially the same prompt (`gpt4`,`claude`,`text_davinci_003`,`guanaco_33b`,
-`chatgpt`). See [here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/
-alpaca_eval/evaluators_configs) for the configs of all evaluators that are
-available out of the box and their associated metrics. | | Human agreement [%]
-| Price [$/1000 examples] | Time [seconds/1000 examples] | Bias | Variance |
-Proba. prefer longer | |:------------------------|--------------------:|-------
------------------:|-----------------------------:|-----:|---------:|-----------
-----------:| | alpaca_eval_gpt4 | 69.2 | 13.6 | 1455 | 28.4 | 14.6 | 0.68 | |
-aviary_gpt4 | 69.1 | 12.8 | 1869 | 29.5 | 13.1 | 0.70 | | gpt4 | 66.9 | 12.5 |
-1037 | 31.5 | 14.6 | 0.65 | | alpaca_farm_greedy_gpt4 | 66.4 | 15.3 | 878 |
-30.2 | 19.3 | 0.60 | | humans | 65.7 | 300.0 | 36800 | 0.0 | | 0.64 | | claude
-| 65.5 | 11.1 | 173 | 31.9 | 18.0 | 0.62 | | text_davinci_003 | 64.1 | 8.7 |
-121 | 33.8 | 22.7 | 0.70 | | lmsys_gpt4 | 63.2 | 13.9 | 17982 | 34.7 | 16.1 |
-0.74 | | guanaco_33b | 59.1 | | 930 | 54.5 | 27.1 | 0.70 | | chatgpt | 57.2 |
-0.8 | 285 | 39.4 | 34.1 | 0.59 |  How exactly are those metrics computed? We
-now explain in words how we compute the metrics in the table above. [The code
-is here](https://github.com/tatsu-lab/alpaca_eval/blob/
+essentially the same prompt
+(`gpt4`,`claude`,`text_davinci_003`,`chatgpt_fn`,`guanaco_33b`, `chatgpt`). See
+[here](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/
+evaluators_configs) for the configs of all evaluators that are available out of
+the box and their associated metrics. | | Human agreement [%] | Price [$/1000
+examples] | Time [seconds/1000 examples] | Bias | Variance | Proba. prefer
+longer | |:------------------------|--------------------:|---------------------
+---:|-----------------------------:|-----:|---------:|---------------------:| |
+alpaca_eval_gpt4 | 69.2 | 13.6 | 1455 | 28.4 | 14.6 | 0.68 | | aviary_gpt4 |
+69.1 | 12.8 | 1869 | 29.5 | 13.1 | 0.70 | | gpt4 | 66.9 | 12.5 | 1037 | 31.5 |
+14.6 | 0.65 | | alpaca_farm_greedy_gpt4 | 66.4 | 15.3 | 878 | 30.2 | 19.3 |
+0.60 | | humans | 65.7 | 300.0 | 36800 | 0.0 | 34.3 | 0.64 | | claude | 65.5 |
+11.1 | 173 | 31.9 | 18.0 | 0.62 | | text_davinci_003 | 64.1 | 8.7 | 121 | 33.8
+| 22.7 | 0.70 | | lmsys_gpt4 | 63.2 | 13.9 | 17982 | 34.7 | 16.1 | 0.74 | |
+chatgpt_fn | 60.0 | 1.0 | 530 | 36.9 | 27.7 | 0.62 | | chatgpt | 57.2 | 0.8 |
+285 | 39.4 | 34.1 | 0.59 |  How exactly are those metrics computed? We now
+explain in words how we compute the metrics in the table above. [The code is
+here](https://github.com/tatsu-lab/alpaca_eval/blob/
 f05cbd651b79ac93906b19d01fe443b45828b0f2/src/alpaca_eval/analyze.py#L366).
 **Human agreement [%]**: this measures the agreement between the current
 annotator and the majority preferences of humans on our ~650 annotations from
 our [cross-annotation set](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_farm_human_crossannotations.json), which contains
 4 human annotations per example. To estimate the agreement between a single
 human (`humans` row in the table above) and the majority of humans, we take one
@@ -240,16 +250,17 @@
 outputs in the prompt, so this should be 0.5. Prior annotators, such as `lmsys`
 and `aviary`, do not. **# parsed**: this is the number of examples that the
 annotator was able to parse. Note that if the variance and bias is empty, it
 means that we only performed one single annotation for each 648 example due to
 resource (time and price) constraints. This explains why the #parsed is 648,
 otherwise it should be 2592.   Tips for choosing evaluators Overall we
 recommend using `annotators_config=alpaca_eval_gpt4` if you want the highest
-agreement with humans, and `annotators_config=claude` if you have academic
-(free) access to Claude and have a low budget. When choosing an annotator we
+agreement with humans, `annotators_config=claude` if you have academic (free)
+access to Claude and have a low budget, and `annotators_config=chatgpt_fn` if
+you don't have access to the other two models. When choosing an annotator we
 recommend you to consider the following (the first three are obvious): -
 `"Human agreement [%]"` - `"Price [$/1000 examples]"` - `"Time [seconds/1000
 examples]"` - `"Proba. prefer longer"` approx. < 0.7. Indeed, we found see that
 the majority of preference of human annotators have strong bias for longer
 answers (as shown by the high [performance=62.2](https://github.com/tatsu-lab/
 alpaca_eval/blob/main/src/alpaca_eval/evaluators_configs/README.md) of the
 `"longest"` evaluator that always prefers the longest output). This suggests
@@ -274,16 +285,16 @@
 it might be easier to install `alpaca_eval` from source.) [//]: # (If so follow
 the following steps:) [//]: # () [//]: # (1. clone the repository) [//]: # ()
 [//]: # (2. install as dev the package: `pip install -e .`) [//]: # () [//]: #
 (3. (optional) export) [//]: # () [//]: # ( all [API_KEYs](https://github.com/
 tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/constants.py#L7)) [//]: # () [/
 /]: # (4. test your installation (assuming you have OpenAI) [//]: # () [//]: #
 ( key) `alpaca_eval --model_outputs 'example/outputs.json' --annotators_config
-'text_davinci_003' --max_instances 3 --caching_path None`) [//]: # () [//]: #
-() ## Evaluating a model  >>> alpaca_eval evaluate -- --help ``` NAME
+'text_davinci_003' ~~--max_instances 3~~ --caching_path None`) [//]: # () [//]:
+# () ## Evaluating a model  >>> alpaca_eval evaluate -- --help ``` NAME
 alpaca_eval evaluate - Evaluate a model based on its outputs. This is the
 default entrypoint if no command is specified. SYNOPSIS alpaca_eval evaluate
 DESCRIPTION Evaluate a model based on its outputs. This is the default
 entrypoint if no command is specified. FLAGS --model_outputs=MODEL_OUTPUTS
 Type: Optional[Union] Default: None The outputs of the model to add to the
 leaderboard. Accepts data (list of dictionary, pd.dataframe, datasets.Dataset)
 or a path to read those (json, csv, tsv) or a function to generate those. Each
@@ -319,15 +330,15 @@
 Whether to return the metrics instead of printing the results. -f, --
 fn_metric=FN_METRIC Type: Union Default: 'pairwise_to_winrate' The function or
 function name in `metrics.py` that will be used to convert preference to
 metrics. The func tion should take a sequence of preferences (0 for draw, 1 for
 base win, 2 when the model to compare wins) and retu rn a dictionary of metrics
 and the key by which to sort the leaderboard. -s, --sort_by=SORT_BY Type: str
 Default: 'win_rate' The key by which to sort the leaderboard. --
-is_cache_leaderboard=IS_CACHE_LEADERBOARD Type: Optional Default: False Whether
+is_cache_leaderboard=IS_CACHE_LEADERBOARD Type: Optional Default: None Whether
 to save the result leaderboard to `precomputed_leaderboard`. If None we save
 only if max_instances . A preferred way of adding models to the leaderboard is
 to set `precomputed_leaderboard` to the previously saved leaderboard at `/
 leaderboard.csv`. --max_instances=MAX_INSTANCES Type: Optional[Optional]
 Default: None The maximum number of instances to annotate. Useful for testing.
 --annotation_kwargs=ANNOTATION_KWARGS Type: Optional[Optional] Default: None
 Additional arguments to pass to `PairwiseAnnotator.annotate_head2head`.
@@ -367,20 +378,21 @@
 your model is a HuggingFace model or from a standard API provider (OpenAI,
 Anthropic, Cohere). Then you can directly use `alpaca_eval evaluate_from_model`
 to also take care of generating outputs. 2. Compute the reference outputs
 `reference_outputs`. By default, we use the outputs of `text-davinci-003` on
 AlpacaEval. If you want to use a different model or a different dataset follow
 the same steps as (1.). 3. Choose an evaluator specified via
 `annotators_config`. We recommend using `alpaca_eval_gpt4` or `claude` (if you
-are an academic). For options and comparisons see [this table](#evaluators).
-Depending on the evaluator you might need to set the appropriate API_KEY in
-your environment or [here](https://github.com/tatsu-lab/alpaca_eval/blob/main/
-src/alpaca_eval/constants.py#L7). Running all together: ```bash alpaca_eval --
-model_outputs 'example/outputs.json' \ --annotators_config 'alpaca_eval_gpt4' \
---reference_outputs  ``` If you don't have decoded outputs, you can use
+are an academic) or `chatgpt_fn` (if you don't have access to the other two).
+For options and comparisons see [this table](#evaluators). Depending on the
+evaluator you might need to set the appropriate API_KEY in your environment or
+[here](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/
+constants.py#L7). Running all together: ```bash alpaca_eval --model_outputs
+'example/outputs.json' \ --annotators_config 'alpaca_eval_gpt4' \ --
+reference_outputs  ``` If you don't have decoded outputs, you can use
 `evaluate_from_model` which takes care of decoding (model and reference) for
 you. Here's an example: ```bash # need a GPU for local models export
 ANTHROPIC_API_KEY= # let's annotate with claude alpaca_eval evaluate_from_model
 \ --model_configs 'oasst_pythia_12b' \ --annotators_config 'claude' \ --
 reference_model_configs  ``` Here the `model_configs` and
 `reference_model_configs` (optional) are paths to a directory that specifies
 the prompt, the model provider (here HuggingFace) and decoding parameters. See
@@ -586,41 +598,43 @@
 one could remove this dataset from the evaluation set. The exact reason should
 be analyzed in future work. For the code and more analysis see [this notebook]
 (https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/
 analyzing_evalset.ipynb), or the colab notebook above. # Contributing We are
 accepting PRs for new models, evaluators, and eval sets, in addition to bug
 fixes. We will update the [leaderboard website](https://tatsu-lab.github.io/
 alpaca_eval/) regularly with new community contributions. We have also created
-a [support discord](https://discord.gg/qVYd69ye) for AlpacaEval in case you run
-into any issues and wish to ask help from the community.
+a [support discord](https://discord.gg/GJMxJSVZZM) for AlpacaEval in case you
+run into any issues and wish to ask help from the community. To get started,
+please first fork the repo, and install the package from source `pip install -
+e .`
 ***** Contributing a model *****
 First, you'll need to add a model config definition in the [models_configs]
 (src/alpaca_eval/models_configs/) folder. As an example, you can look at the
 [falcon-7b-instruct yaml](src/alpaca_eval/models_configs/falcon-7b-instruct/
 configs.yaml). Please make sure the folder name and key name in the yaml match
-exactly. Then, please follow the steps in [Evaluating-a-model](#evaluating-a-
+exactly. Then, please follow the steps in [Evaluating a model](#evaluating-a-
 model) to run inference on the model to produce outputs on the eval set and
 score the model according to one of the evaluators. An example command may look
 like: ```sh alpaca_eval evaluate_from_model \ --model_configs 'falcon-7b-
 instruct' \ --annotators_config 'alpaca_eval_gpt4' ``` After running this
 command, you should have generated an outputs json and a new entry in the
-corresponding leaderboard file. Please make a PR with the config, outputs file,
-and updated leaderboard.
+corresponding [leaderboard file](https://github.com/tatsu-lab/alpaca_eval/tree/
+main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR with the
+config, outputs file, and updated leaderboard.
 ***** Contributing an evaluator *****
 Please first follow the directions in [Making a new evaluator](#making-a-new-
 evaluator). Once you're created the annotator config, we ask that you create a
 new leaderboard for the annotator by evaluating the minimal set of models. The
 outputs for these models can be found by downloading
 [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_eval_all_outputs.json). ```bash alpaca_eval
-make_leaderboard \ --leaderboard_path
-lpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \ --
-all_model_outputs alpaca_eval_all_outputs.json \ --annotators_config
-yaml> ``` Then, please create a PR with the annotator config and leaderboard
-csv.
+make_leaderboard \ --leaderboard_path src/alpaca_eval/leaderboards/
+data_AlpacaEval/_leaderboard.csv \ --all_model_outputs
+alpaca_eval_all_outputs.json \ --annotators_config  ``` Then, please create a
+PR with the annotator config and leaderboard csv.
 ***** Contributing an eval set *****
 To contribute a new eval set, you'll first need to specify a set of textual
 instructions. Then, you'll need to specify a set of reference outputs (model
 win-rates are computed against this reference). For ease of use, you may use
 the default [text-davinci-003](src/alpaca_eval/models_configs/text_davinci_003/
 ) reference config. Place these together into a json, where each entry
 specifies the fields `instruction`, `output`, and `generator`. You can look to
@@ -788,7 +802,15 @@
 evaluators. For example: - [AlpacaFarm Appx C](https://arxiv.org/abs/
 2305.14387) and [Large Language Models are not Fair Evaluators](https://
 arxiv.org/abs/2305.17926v1) both found that automatic annotators have a
 position bias. - [AlpacaFarm Sec. 5.2.](https://arxiv.org/abs/2305.14387) and
 [The False Promise of Imitating Proprietary LLMs](https://arxiv.org/abs/
 2305.15717) both found that automatic annotators favor style (e.g. use of list,
 tone, word choice, length) over factuality.
+***** Major updates *****
+- 19th June 2023: add leaderboard `chatgpt_fn` that anyone can use (no waiting
+lists). - 19th June 2023: update to use [OpenAI's function calling](https://
+openai.com/blog/function-calling-and-other-api-updates). Example:
+[`chatgpt_fn`](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/
+alpaca_eval/evaluators_configs/chatgpt_fn) or [`alpaca_eval_gpt4_fn`](https://
+github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/evaluators_configs/
+alpaca_eval_gpt4_fn).
```

### Comparing `alpaca_eval-0.1.3/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.1.5/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 src/alpaca_eval/decoders/cohere.py
 src/alpaca_eval/decoders/huggingface_api.py
 src/alpaca_eval/decoders/huggingface_local.py
 src/alpaca_eval/decoders/openai.py
 src/alpaca_eval/evaluators_configs/README.md
 src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
 src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
@@ -44,14 +46,16 @@
 src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
 src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
 src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
 src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
 src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/claude/configs.yaml
 src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
 src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
 src/alpaca_eval/evaluators_configs/cohere/configs.yaml
 src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
 src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
@@ -61,34 +65,42 @@
 src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
 src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
 src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
 src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
 src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
 src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
 src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
 src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
 src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
 src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
 src/alpaca_eval/models_configs/chatgpt/configs.yaml
 src/alpaca_eval/models_configs/claude/configs.yaml
 src/alpaca_eval/models_configs/claude/prompt.txt
 src/alpaca_eval/models_configs/cohere/configs.yaml
+src/alpaca_eval/models_configs/cohere/prompt.txt
+src/alpaca_eval/models_configs/cohere-chat/configs.yaml
 src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
 src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
 src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
 src/alpaca_eval/models_configs/gpt4/configs.yaml
 src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
 src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
 src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
 src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
```

