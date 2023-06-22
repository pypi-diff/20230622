# Comparing `tmp/aicodebot-0.3.0.tar.gz` & `tmp/aicodebot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.3.0.tar", last modified: Thu Jun 22 05:52:30 2023, max compression
+gzip compressed data, was "aicodebot-0.4.0.tar", last modified: Thu Jun 22 18:02:37 2023, max compression
```

## Comparing `aicodebot-0.3.0.tar` & `aicodebot-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.788923 aicodebot-0.3.0/
--rw-r--r--   0 nick       (501) staff       (20)    34523 2023-06-20 19:00:47.000000 aicodebot-0.3.0/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     7095 2023-06-22 05:52:30.788725 aicodebot-0.3.0/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     6460 2023-06-22 05:50:37.000000 aicodebot-0.3.0/README.md
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.786448 aicodebot-0.3.0/aicodebot/
--rw-r--r--   0 nick       (501) staff       (20)       97 2023-06-21 05:21:47.000000 aicodebot-0.3.0/aicodebot/.aicodebot.template
--rw-r--r--   0 nick       (501) staff       (20)       18 2023-06-22 05:51:15.000000 aicodebot-0.3.0/aicodebot/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     6223 2023-06-22 05:41:52.000000 aicodebot-0.3.0/aicodebot/cli.py
--rw-r--r--   0 nick       (501) staff       (20)      366 2023-06-22 00:57:03.000000 aicodebot-0.3.0/aicodebot/helpers.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.788169 aicodebot-0.3.0/aicodebot/prompts/
--rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-22 03:39:34.000000 aicodebot-0.3.0/aicodebot/prompts/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      838 2023-06-22 05:45:33.000000 aicodebot-0.3.0/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 nick       (501) staff       (20)     1018 2023-06-22 01:25:59.000000 aicodebot-0.3.0/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 nick       (501) staff       (20)      212 2023-06-21 05:21:47.000000 aicodebot-0.3.0/aicodebot/prompts/fun_fact.yaml
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.787326 aicodebot-0.3.0/aicodebot.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     7095 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      482 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       48 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 nick       (501) staff       (20)       42 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)       10 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 nick       (501) staff       (20)     2789 2023-06-21 05:21:47.000000 aicodebot-0.3.0/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)       38 2023-06-22 05:52:30.788960 aicodebot-0.3.0/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)     1526 2023-06-22 05:52:18.000000 aicodebot-0.3.0/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.788401 aicodebot-0.3.0/tests/
--rw-r--r--   0 nick       (501) staff       (20)      535 2023-06-22 03:59:54.000000 aicodebot-0.3.0/tests/test_cli.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.891184 aicodebot-0.4.0/
+-rw-r--r--   0 nick       (501) staff       (20)    34523 2023-06-22 18:00:57.000000 aicodebot-0.4.0/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     6655 2023-06-22 18:02:37.891071 aicodebot-0.4.0/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     6020 2023-06-22 18:00:57.000000 aicodebot-0.4.0/README.md
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.889372 aicodebot-0.4.0/aicodebot/
+-rw-r--r--   0 nick       (501) staff       (20)       97 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/.aicodebot.template
+-rw-r--r--   0 nick       (501) staff       (20)       18 2023-06-22 18:01:18.000000 aicodebot-0.4.0/aicodebot/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     7834 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/cli.py
+-rw-r--r--   0 nick       (501) staff       (20)      366 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/helpers.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.890744 aicodebot-0.4.0/aicodebot/prompts/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      838 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 nick       (501) staff       (20)     1018 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 nick       (501) staff       (20)      287 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 nick       (501) staff       (20)      212 2023-06-22 18:00:57.000000 aicodebot-0.4.0/aicodebot/prompts/fun_fact.yaml
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.890157 aicodebot-0.4.0/aicodebot.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     6655 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      511 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       48 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 nick       (501) staff       (20)       42 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)       10 2023-06-22 18:02:37.000000 aicodebot-0.4.0/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 nick       (501) staff       (20)     2789 2023-06-22 18:00:57.000000 aicodebot-0.4.0/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)       38 2023-06-22 18:02:37.891216 aicodebot-0.4.0/setup.cfg
+-rw-r--r--   0 nick       (501) staff       (20)     1526 2023-06-22 18:00:57.000000 aicodebot-0.4.0/setup.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 18:02:37.890884 aicodebot-0.4.0/tests/
+-rw-r--r--   0 nick       (501) staff       (20)      535 2023-06-22 18:00:57.000000 aicodebot-0.4.0/tests/test_cli.py
```

### Comparing `aicodebot-0.3.0/LICENSE` & `aicodebot-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.3.0/PKG-INFO` & `aicodebot-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.3.0
+Version: 0.4.0
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -17,40 +17,50 @@
 
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer.
 
-⚠️ Status: This project is in its infancy with very limited features. Right now it only tells you fun facts, but you can look at the Features list below to get an idea of where it is going. Give the project a star and follow along while we build out more of the foundation.
+⚠️ Status: This project is in its infancy with very limited features. Sometimes it does dumb things.
 
-## MVP
+Right now, it only generates commit messages for you, but you can look at the Features list below to get an idea of where it is going. Give the project a star and follow along while we build out more of the foundation.
 
-For the initial release, you can get a Fun Fact related to AI and Programming.
+## Setup and Usage
 
-`aicodebot fun-fact`
+Follow the steps below to set up AICodeBot on your machine:
 
->>🤖 The first chess program written in Fortran for the IBM 704 computer in 1960 was beaten by a human in just four moves. The program relied heavily on brute force calculation, and had not yet developed sophisticated artificial intelligence algorithms.
+`pip install aicodebot`
 
-Behind the scenes, this is talking to the Open AI API and getting a response via Langchain.
+The first time you run it, you'll be prompted to enter your OpenAI API key, which is required. You can get one for free on your [API key settings](https://platform.openai.com/account/api-keys").
 
-#### Commit Message
+```bash
+> aicodebot --help
+Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
 
-Automate your commits by having aicodebot generate a commit message for you.
+Options:
+  -V, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
 
-`aicodebot commit`
+Commands:
+  alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
+  commit     Generate a git commit message and commit changes after you...
+  debug      Run a command and get debugging advice if it fails.
+  fun-fact   Tell me something interesting about programming or AI.
+  version    Print the version number.
+```
 
 ## Features
 
 ### Code Workflow Improvements
 
 - [X] **Assisted Git Commit**: Automatically generate a commit message.
+- [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 - [ ] **Code Review**: Provides feedback on potential issues in code, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
-- [ ] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 - [ ] **Code Formatting**: Automatically formats code according to a specified style guide.
 - [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code.
 - [ ] **Code Generation**: Generates boilerplate code for common tasks.
 - [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
@@ -75,40 +85,18 @@
 
 ### Fun
 
 - [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
 - [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
 - [ ] **Telling Jokes**: Tells programming jokes. :smiley:
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **Gif Reactions**: Reacts to messages with relevant and fun gifs. It could also react to specific events in the repository, like the merging of a pull request or the closing of an issue.
+- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs. We've gotta figure out how to teach LLMs about humor.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
-## Setup and Usage
-
-Follow the steps below to set up AICodeBot on your machine:
-
-`pip install aicodebot`
-
-The first time you run it, you'll be prompted to enter your OpenAI API key, which is required. You can get one for free on your [API key settings](https://platform.openai.com/account/api-keys").
-
-```bash
-> aicodebot --help
-Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  -V, --version  Show the version and exit.
-  -h, --help     Show this message and exit.
-
-Commands:
-  commit    Generate a git commit message based on the diff, and then...
-  fun-fact  Tell me something interesting about programming or AI.
-  version   Print the version number.
-```
-
 ## Development
 
 1. Clone the repository
 
 ```bash
 git clone git@github.com:novara-ai/aicodebot.git
 ```
@@ -119,9 +107,10 @@
 mkvirtualenv --python=`which python3` aicodebot
 ```
 
 3. Install the dependencies:
 
 ```bash
 pip install -r requirements/requirements-dev.txt
-# Use requirements-dev.txt if you want to contribute to the project
 ```
+
+4. Use aicodebot to build aicodebot 😎
```

### Comparing `aicodebot-0.3.0/README.md` & `aicodebot-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer.
 
-⚠️ Status: This project is in its infancy with very limited features. Right now it only tells you fun facts, but you can look at the Features list below to get an idea of where it is going. Give the project a star and follow along while we build out more of the foundation.
+⚠️ Status: This project is in its infancy with very limited features. Sometimes it does dumb things.
 
-## MVP
+Right now, it only generates commit messages for you, but you can look at the Features list below to get an idea of where it is going. Give the project a star and follow along while we build out more of the foundation.
 
-For the initial release, you can get a Fun Fact related to AI and Programming.
+## Setup and Usage
 
-`aicodebot fun-fact`
+Follow the steps below to set up AICodeBot on your machine:
 
->>🤖 The first chess program written in Fortran for the IBM 704 computer in 1960 was beaten by a human in just four moves. The program relied heavily on brute force calculation, and had not yet developed sophisticated artificial intelligence algorithms.
+`pip install aicodebot`
 
-Behind the scenes, this is talking to the Open AI API and getting a response via Langchain.
+The first time you run it, you'll be prompted to enter your OpenAI API key, which is required. You can get one for free on your [API key settings](https://platform.openai.com/account/api-keys").
 
-#### Commit Message
+```bash
+> aicodebot --help
+Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
 
-Automate your commits by having aicodebot generate a commit message for you.
+Options:
+  -V, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
 
-`aicodebot commit`
+Commands:
+  alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
+  commit     Generate a git commit message and commit changes after you...
+  debug      Run a command and get debugging advice if it fails.
+  fun-fact   Tell me something interesting about programming or AI.
+  version    Print the version number.
+```
 
 ## Features
 
 ### Code Workflow Improvements
 
 - [X] **Assisted Git Commit**: Automatically generate a commit message.
+- [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 - [ ] **Code Review**: Provides feedback on potential issues in code, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
-- [ ] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 - [ ] **Code Formatting**: Automatically formats code according to a specified style guide.
 - [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code.
 - [ ] **Code Generation**: Generates boilerplate code for common tasks.
 - [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
@@ -58,40 +68,18 @@
 
 ### Fun
 
 - [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
 - [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
 - [ ] **Telling Jokes**: Tells programming jokes. :smiley:
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **Gif Reactions**: Reacts to messages with relevant and fun gifs. It could also react to specific events in the repository, like the merging of a pull request or the closing of an issue.
+- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs. We've gotta figure out how to teach LLMs about humor.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
-## Setup and Usage
-
-Follow the steps below to set up AICodeBot on your machine:
-
-`pip install aicodebot`
-
-The first time you run it, you'll be prompted to enter your OpenAI API key, which is required. You can get one for free on your [API key settings](https://platform.openai.com/account/api-keys").
-
-```bash
-> aicodebot --help
-Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  -V, --version  Show the version and exit.
-  -h, --help     Show this message and exit.
-
-Commands:
-  commit    Generate a git commit message based on the diff, and then...
-  fun-fact  Tell me something interesting about programming or AI.
-  version   Print the version number.
-```
-
 ## Development
 
 1. Clone the repository
 
 ```bash
 git clone git@github.com:novara-ai/aicodebot.git
 ```
@@ -102,9 +90,10 @@
 mkvirtualenv --python=`which python3` aicodebot
 ```
 
 3. Install the dependencies:
 
 ```bash
 pip install -r requirements/requirements-dev.txt
-# Use requirements-dev.txt if you want to contribute to the project
 ```
+
+4. Use aicodebot to build aicodebot 😎
```

### Comparing `aicodebot-0.3.0/aicodebot/cli.py` & `aicodebot-0.4.0/aicodebot/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from rich.console import Console
 from rich.style import Style
 import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser
 
 # Create a Console object
 console = Console()
 bot_style = Style(color="#30D5C8")
+DEFAULT_MAX_TOKENS = 1024
 
 
 def setup_environment():
     # Load environment variables from the config file
     config_file = Path(Path.home() / ".aicodebot")
     load_dotenv(config_file)
 
@@ -65,15 +66,15 @@
     """Get a message about Heart-Centered AI Alignment ❤ + 🤖."""
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "alignment.yaml")
 
     # Set up the language model
-    llm = OpenAI(temperature=1, max_tokens=1024)
+    llm = OpenAI(temperature=1, max_tokens=DEFAULT_MAX_TOKENS)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     name = exec_and_get_output(["git", "config", "--get", "user.name"])
 
     with console.status("Thinking", spinner="point"):
@@ -96,24 +97,25 @@
     llm = OpenAI(temperature=0.1, max_tokens=max_tokens)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     # Get the changes from git
     staged_files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
+    base_git_diff = ["git", "diff", "-U10"]  # Tell diff to provide 10 lines of context
     if not staged_files:
         # If no files are staged, stage all changed files
         exec_and_get_output(["git", "add", "-A"])
         # Get the diff for all changes since the last commit
-        diff = exec_and_get_output(["git", "diff", "HEAD"])
+        diff = exec_and_get_output(base_git_diff + ["HEAD"])
         # Get the list of files to be committed
         files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
     else:
         # If some files are staged, get the diff for those files
-        diff = exec_and_get_output(["git", "diff", "--cached"])
+        diff = exec_and_get_output(base_git_diff + ["--cached"])
         # The list of files to be committed is the same as the list of staged files
         files = staged_files
 
     if not diff:
         console.print("No changes to commit.")
         sys.exit(0)
 
@@ -130,32 +132,71 @@
     # Open the temporary file in the user's editor
     editor = os.getenv("EDITOR", "vim")
     subprocess.call([editor, temp_file_name])  # noqa: S603
 
     # Ask the user if they want to commit the changes
     if yes or click.confirm("Do you want to commit the changes?"):
         # Commit the changes using the temporary file for the commit message
-        exec_and_get_output(["git", "commit", "-a", "-F", temp_file_name])
+        exec_and_get_output(["git", "commit", "-F", temp_file_name])
         console.print(f"✅ {len(files.splitlines())} files committed.")
 
     # Delete the temporary file
     Path.unlink(temp_file_name)
 
 
+@cli.command(context_settings={"ignore_unknown_options": True})
+@click.argument("command", nargs=-1)
+@click.option("-v", "--verbose", count=True)
+def debug(command, verbose):
+    """Run a command and get debugging advice if it fails."""
+    setup_environment()
+
+    # Load the prompt
+    prompt = load_prompt(Path(__file__).parent / "prompts" / "debug.yaml")
+
+    # Set up the language model
+    llm = OpenAI(temperature=0.1, max_tokens=DEFAULT_MAX_TOKENS)
+
+    # Set up the chain
+    chat_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+    command_str = " ".join(command)
+
+    # Run the command and capture its output
+    console.print(f"Running:\n{command_str}")
+    process = subprocess.run(command_str, shell=True, capture_output=True, text=True)  # noqa: S602
+
+    # Print the output of the command
+    output = f"Standard Output:\n{process.stdout}\nStandard Error:\n{process.stderr}"
+    console.print(f"Output:\n{output}")
+
+    # Print a message about the exit status
+    if process.returncode == 0:
+        console.print("The command completed successfully.")
+    else:
+        console.print(f"The command exited with status {process.returncode}.")
+
+    # If the command failed, send its output to ChatGPT for analysis
+    if process.returncode != 0:
+        error_output = process.stderr
+        with console.status("Thinking", spinner="point"):
+            response = chat_chain.run(error_output)
+            console.print(response, style=bot_style)
+
+
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 def fun_fact(verbose):
     """Tell me something interesting about programming or AI."""
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "fun_fact.yaml")
 
     # Set up the language model
-    llm = ChatOpenAI(temperature=1, max_tokens=1024)
+    llm = ChatOpenAI(temperature=1, max_tokens=DEFAULT_MAX_TOKENS)
 
     # Set up the chain
     chat_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     with console.status("Thinking", spinner="point"):
         # Select a random year so that we get a different answer each time
         year = random.randint(1942, datetime.datetime.utcnow().year)
```

### Comparing `aicodebot-0.3.0/aicodebot/prompts/alignment.yaml` & `aicodebot-0.4.0/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.3.0/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.4.0/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.3.0/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.4.0/aicodebot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.3.0
+Version: 0.4.0
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -17,40 +17,50 @@
 
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer.
 
-⚠️ Status: This project is in its infancy with very limited features. Right now it only tells you fun facts, but you can look at the Features list below to get an idea of where it is going. Give the project a star and follow along while we build out more of the foundation.
+⚠️ Status: This project is in its infancy with very limited features. Sometimes it does dumb things.
 
-## MVP
+Right now, it only generates commit messages for you, but you can look at the Features list below to get an idea of where it is going. Give the project a star and follow along while we build out more of the foundation.
 
-For the initial release, you can get a Fun Fact related to AI and Programming.
+## Setup and Usage
 
-`aicodebot fun-fact`
+Follow the steps below to set up AICodeBot on your machine:
 
->>🤖 The first chess program written in Fortran for the IBM 704 computer in 1960 was beaten by a human in just four moves. The program relied heavily on brute force calculation, and had not yet developed sophisticated artificial intelligence algorithms.
+`pip install aicodebot`
 
-Behind the scenes, this is talking to the Open AI API and getting a response via Langchain.
+The first time you run it, you'll be prompted to enter your OpenAI API key, which is required. You can get one for free on your [API key settings](https://platform.openai.com/account/api-keys").
 
-#### Commit Message
+```bash
+> aicodebot --help
+Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
 
-Automate your commits by having aicodebot generate a commit message for you.
+Options:
+  -V, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
 
-`aicodebot commit`
+Commands:
+  alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
+  commit     Generate a git commit message and commit changes after you...
+  debug      Run a command and get debugging advice if it fails.
+  fun-fact   Tell me something interesting about programming or AI.
+  version    Print the version number.
+```
 
 ## Features
 
 ### Code Workflow Improvements
 
 - [X] **Assisted Git Commit**: Automatically generate a commit message.
+- [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
 - [ ] **Code Review**: Provides feedback on potential issues in code, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
-- [ ] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 - [ ] **Code Formatting**: Automatically formats code according to a specified style guide.
 - [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code.
 - [ ] **Code Generation**: Generates boilerplate code for common tasks.
 - [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
@@ -75,40 +85,18 @@
 
 ### Fun
 
 - [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
 - [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
 - [ ] **Telling Jokes**: Tells programming jokes. :smiley:
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **Gif Reactions**: Reacts to messages with relevant and fun gifs. It could also react to specific events in the repository, like the merging of a pull request or the closing of an issue.
+- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs. We've gotta figure out how to teach LLMs about humor.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
-## Setup and Usage
-
-Follow the steps below to set up AICodeBot on your machine:
-
-`pip install aicodebot`
-
-The first time you run it, you'll be prompted to enter your OpenAI API key, which is required. You can get one for free on your [API key settings](https://platform.openai.com/account/api-keys").
-
-```bash
-> aicodebot --help
-Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  -V, --version  Show the version and exit.
-  -h, --help     Show this message and exit.
-
-Commands:
-  commit    Generate a git commit message based on the diff, and then...
-  fun-fact  Tell me something interesting about programming or AI.
-  version   Print the version number.
-```
-
 ## Development
 
 1. Clone the repository
 
 ```bash
 git clone git@github.com:novara-ai/aicodebot.git
 ```
@@ -119,9 +107,10 @@
 mkvirtualenv --python=`which python3` aicodebot
 ```
 
 3. Install the dependencies:
 
 ```bash
 pip install -r requirements/requirements-dev.txt
-# Use requirements-dev.txt if you want to contribute to the project
 ```
+
+4. Use aicodebot to build aicodebot 😎
```

### Comparing `aicodebot-0.3.0/pyproject.toml` & `aicodebot-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.3.0/setup.py` & `aicodebot-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.3.0/tests/test_cli.py` & `aicodebot-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

