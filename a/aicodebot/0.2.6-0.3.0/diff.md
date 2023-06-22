# Comparing `tmp/aicodebot-0.2.6.tar.gz` & `tmp/aicodebot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.2.6.tar", last modified: Thu Jun 22 04:06:35 2023, max compression
+gzip compressed data, was "aicodebot-0.3.0.tar", last modified: Thu Jun 22 05:52:30 2023, max compression
```

## Comparing `aicodebot-0.2.6.tar` & `aicodebot-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 04:06:35.153092 aicodebot-0.2.6/
--rw-r--r--   0 nick       (501) staff       (20)    34523 2023-06-20 19:00:47.000000 aicodebot-0.2.6/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     7120 2023-06-22 04:06:35.152947 aicodebot-0.2.6/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     6485 2023-06-22 04:05:25.000000 aicodebot-0.2.6/README.md
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 04:06:35.151026 aicodebot-0.2.6/aicodebot/
--rw-r--r--   0 nick       (501) staff       (20)       97 2023-06-21 05:21:47.000000 aicodebot-0.2.6/aicodebot/.aicodebot.template
--rw-r--r--   0 nick       (501) staff       (20)       18 2023-06-22 03:59:51.000000 aicodebot-0.2.6/aicodebot/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5386 2023-06-22 03:59:50.000000 aicodebot-0.2.6/aicodebot/cli.py
--rw-r--r--   0 nick       (501) staff       (20)      366 2023-06-22 00:57:03.000000 aicodebot-0.2.6/aicodebot/helpers.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 04:06:35.152320 aicodebot-0.2.6/aicodebot/prompts/
--rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-22 03:39:34.000000 aicodebot-0.2.6/aicodebot/prompts/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     1018 2023-06-22 01:25:59.000000 aicodebot-0.2.6/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 nick       (501) staff       (20)      212 2023-06-21 05:21:47.000000 aicodebot-0.2.6/aicodebot/prompts/fun_fact.yaml
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 04:06:35.151886 aicodebot-0.2.6/aicodebot.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     7120 2023-06-22 04:06:35.000000 aicodebot-0.2.6/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      449 2023-06-22 04:06:35.000000 aicodebot-0.2.6/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-22 04:06:35.000000 aicodebot-0.2.6/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       48 2023-06-22 04:06:35.000000 aicodebot-0.2.6/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 nick       (501) staff       (20)      650 2023-06-22 04:06:35.000000 aicodebot-0.2.6/aicodebot.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)       10 2023-06-22 04:06:35.000000 aicodebot-0.2.6/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 nick       (501) staff       (20)     2789 2023-06-21 05:21:47.000000 aicodebot-0.2.6/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)       38 2023-06-22 04:06:35.153129 aicodebot-0.2.6/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)     1528 2023-06-22 03:59:48.000000 aicodebot-0.2.6/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 04:06:35.152627 aicodebot-0.2.6/tests/
--rw-r--r--   0 nick       (501) staff       (20)      535 2023-06-22 03:59:54.000000 aicodebot-0.2.6/tests/test_cli.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.788923 aicodebot-0.3.0/
+-rw-r--r--   0 nick       (501) staff       (20)    34523 2023-06-20 19:00:47.000000 aicodebot-0.3.0/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     7095 2023-06-22 05:52:30.788725 aicodebot-0.3.0/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     6460 2023-06-22 05:50:37.000000 aicodebot-0.3.0/README.md
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.786448 aicodebot-0.3.0/aicodebot/
+-rw-r--r--   0 nick       (501) staff       (20)       97 2023-06-21 05:21:47.000000 aicodebot-0.3.0/aicodebot/.aicodebot.template
+-rw-r--r--   0 nick       (501) staff       (20)       18 2023-06-22 05:51:15.000000 aicodebot-0.3.0/aicodebot/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     6223 2023-06-22 05:41:52.000000 aicodebot-0.3.0/aicodebot/cli.py
+-rw-r--r--   0 nick       (501) staff       (20)      366 2023-06-22 00:57:03.000000 aicodebot-0.3.0/aicodebot/helpers.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.788169 aicodebot-0.3.0/aicodebot/prompts/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-22 03:39:34.000000 aicodebot-0.3.0/aicodebot/prompts/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      838 2023-06-22 05:45:33.000000 aicodebot-0.3.0/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 nick       (501) staff       (20)     1018 2023-06-22 01:25:59.000000 aicodebot-0.3.0/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 nick       (501) staff       (20)      212 2023-06-21 05:21:47.000000 aicodebot-0.3.0/aicodebot/prompts/fun_fact.yaml
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.787326 aicodebot-0.3.0/aicodebot.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     7095 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      482 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       48 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 nick       (501) staff       (20)       42 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)       10 2023-06-22 05:52:30.000000 aicodebot-0.3.0/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 nick       (501) staff       (20)     2789 2023-06-21 05:21:47.000000 aicodebot-0.3.0/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)       38 2023-06-22 05:52:30.788960 aicodebot-0.3.0/setup.cfg
+-rw-r--r--   0 nick       (501) staff       (20)     1526 2023-06-22 05:52:18.000000 aicodebot-0.3.0/setup.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-22 05:52:30.788401 aicodebot-0.3.0/tests/
+-rw-r--r--   0 nick       (501) staff       (20)      535 2023-06-22 03:59:54.000000 aicodebot-0.3.0/tests/test_cli.py
```

### Comparing `aicodebot-0.2.6/LICENSE` & `aicodebot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.2.6/PKG-INFO` & `aicodebot-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.2.6
+Version: 0.3.0
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -33,58 +33,59 @@
 
 Behind the scenes, this is talking to the Open AI API and getting a response via Langchain.
 
 #### Commit Message
 
 Automate your commits by having aicodebot generate a commit message for you.
 
-## Features
+`aicodebot commit`
 
-Once we've set up the bot to be able to use Large Language Models as a decision making engine at the center of Github and Python APIs, we can start to build out the following features:
+## Features
 
 ### Code Workflow Improvements
 
 - [X] **Assisted Git Commit**: Automatically generate a commit message.
 - [ ] **Code Review**: Provides feedback on potential issues in code, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 - [ ] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 - [ ] **Code Formatting**: Automatically formats code according to a specified style guide.
 - [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code.
 - [ ] **Code Generation**: Generates boilerplate code for common tasks.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via Github Actions)
+- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
 - [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems.
 - [ ] **Linting**: Checks code for linting errors and automatically fixes them where possible.
-- [ ] **Handle Github Issues**: Handles issues that you assign to @aicodebot. It could also suggest labels for new issues based on their content.
+- [ ] **Handle GitHub Issues**: Handles issues that you assign to @aicodebot. It could also suggest labels for new issues based on their content.
 
 ### User Interfaces
 
-- [ ] **Command line installable via pip**: aicodebot can be installed as a Python package using pip
-- [ ] **Chat**: CLI chat interface that knows the context of your code base and can answer questions about it. No more going back and forth between ChatGPT and command line.
-- [ ] **Callable as a Github action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+- [X] **Command-line installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+- [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
+- [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
 - [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 - [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
 - [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 - [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
 - [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
 - [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
 - [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
+- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
 - [ ] **Telling Jokes**: Tells programming jokes. :smiley:
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
 - [ ] **Gif Reactions**: Reacts to messages with relevant and fun gifs. It could also react to specific events in the repository, like the merging of a pull request or the closing of an issue.
 
-<img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" style="width:25%">
+<img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Setup and Usage
 
 Follow the steps below to set up AICodeBot on your machine:
 
 `pip install aicodebot`
```

### Comparing `aicodebot-0.2.6/README.md` & `aicodebot-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,58 +16,59 @@
 
 Behind the scenes, this is talking to the Open AI API and getting a response via Langchain.
 
 #### Commit Message
 
 Automate your commits by having aicodebot generate a commit message for you.
 
-## Features
+`aicodebot commit`
 
-Once we've set up the bot to be able to use Large Language Models as a decision making engine at the center of Github and Python APIs, we can start to build out the following features:
+## Features
 
 ### Code Workflow Improvements
 
 - [X] **Assisted Git Commit**: Automatically generate a commit message.
 - [ ] **Code Review**: Provides feedback on potential issues in code, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 - [ ] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 - [ ] **Code Formatting**: Automatically formats code according to a specified style guide.
 - [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code.
 - [ ] **Code Generation**: Generates boilerplate code for common tasks.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via Github Actions)
+- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
 - [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems.
 - [ ] **Linting**: Checks code for linting errors and automatically fixes them where possible.
-- [ ] **Handle Github Issues**: Handles issues that you assign to @aicodebot. It could also suggest labels for new issues based on their content.
+- [ ] **Handle GitHub Issues**: Handles issues that you assign to @aicodebot. It could also suggest labels for new issues based on their content.
 
 ### User Interfaces
 
-- [ ] **Command line installable via pip**: aicodebot can be installed as a Python package using pip
-- [ ] **Chat**: CLI chat interface that knows the context of your code base and can answer questions about it. No more going back and forth between ChatGPT and command line.
-- [ ] **Callable as a Github action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+- [X] **Command-line installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+- [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
+- [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
 - [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 - [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
 - [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 - [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
 - [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
 - [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
 - [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
+- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
 - [ ] **Telling Jokes**: Tells programming jokes. :smiley:
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
 - [ ] **Gif Reactions**: Reacts to messages with relevant and fun gifs. It could also react to specific events in the repository, like the merging of a pull request or the closing of an issue.
 
-<img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" style="width:25%">
+<img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Setup and Usage
 
 Follow the steps below to set up AICodeBot on your machine:
 
 `pip install aicodebot`
```

### Comparing `aicodebot-0.2.6/aicodebot/cli.py` & `aicodebot-0.3.0/aicodebot/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,17 +34,16 @@
     if click.confirm("Do you want me to open the OpenAI API keys page for you in a browser?"):
         webbrowser.open(openai_api_key_url)
 
     if click.confirm(f"Do you want me to create the {config_file} file for you?"):
         api_key = click.prompt("Please enter your OpenAI API key")
 
         # Copy .env.template to .env and insert the API key
-        with Path.open(Path(__file__).parent / ".aicodebot.template", "r") as template, Path.open(
-            config_file, "w"
-        ) as env:
+        template_file = Path(__file__).parent / ".aicodebot.template"
+        with Path.open(template_file, "r") as template, Path.open(config_file, "w") as env:
             for line in template:
                 if line.startswith("OPENAI_API_KEY="):
                     env.write(f"OPENAI_API_KEY={api_key}\n")
                 else:
                     env.write(line)
 
         console.print(f"[bold green]Created {config_file} with your OpenAI API key. You're all set![/bold green]")
@@ -58,27 +57,50 @@
 @click.help_option("--help", "-h")
 def cli():
     pass
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
+def alignment(verbose):
+    """Get a message about Heart-Centered AI Alignment ❤ + 🤖."""
+    setup_environment()
+
+    # Load the prompt
+    prompt = load_prompt(Path(__file__).parent / "prompts" / "alignment.yaml")
+
+    # Set up the language model
+    llm = OpenAI(temperature=1, max_tokens=1024)
+
+    # Set up the chain
+    chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+
+    name = exec_and_get_output(["git", "config", "--get", "user.name"])
+
+    with console.status("Thinking", spinner="point"):
+        response = chain.run(name)
+        console.print(response, style=bot_style)
+
+
+@cli.command()
+@click.option("-v", "--verbose", count=True)
 @click.option("-t", "--max-tokens", type=int, default=250)
-def commit(verbose, max_tokens):
-    """Generate a git commit message based on the diff, and then commit the changes after you approve."""
+@click.option("-y", "--yes", is_flag=True, default=False, help="Don't ask for confirmation before committing.")
+def commit(verbose, max_tokens, yes):
+    """Generate a git commit message and commit changes after you approve."""
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "commit_message.yaml")
 
     # Set up the language model
     llm = OpenAI(temperature=0.1, max_tokens=max_tokens)
 
     # Set up the chain
-    chat_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+    chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     # Get the changes from git
     staged_files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
     if not staged_files:
         # If no files are staged, stage all changed files
         exec_and_get_output(["git", "add", "-A"])
         # Get the diff for all changes since the last commit
@@ -94,29 +116,30 @@
     if not diff:
         console.print("No changes to commit.")
         sys.exit(0)
 
     console.print("The following files will be committed:\n" + files)
 
     with console.status("Thinking", spinner="point"):
-        response = chat_chain.run(diff)
+        response = chain.run(diff)
 
     # Write the commit message to a temporary file
     with tempfile.NamedTemporaryFile(mode="w", delete=False) as temp:
         temp.write(str(response).strip())
         temp_file_name = temp.name
 
     # Open the temporary file in the user's editor
     editor = os.getenv("EDITOR", "vim")
     subprocess.call([editor, temp_file_name])  # noqa: S603
 
     # Ask the user if they want to commit the changes
-    if click.confirm("Do you want to commit the changes?"):
+    if yes or click.confirm("Do you want to commit the changes?"):
         # Commit the changes using the temporary file for the commit message
         exec_and_get_output(["git", "commit", "-a", "-F", temp_file_name])
+        console.print(f"✅ {len(files.splitlines())} files committed.")
 
     # Delete the temporary file
     Path.unlink(temp_file_name)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aicodebot-0.2.6/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.3.0/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.2.6/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.3.0/aicodebot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.2.6
+Version: 0.3.0
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -33,58 +33,59 @@
 
 Behind the scenes, this is talking to the Open AI API and getting a response via Langchain.
 
 #### Commit Message
 
 Automate your commits by having aicodebot generate a commit message for you.
 
-## Features
+`aicodebot commit`
 
-Once we've set up the bot to be able to use Large Language Models as a decision making engine at the center of Github and Python APIs, we can start to build out the following features:
+## Features
 
 ### Code Workflow Improvements
 
 - [X] **Assisted Git Commit**: Automatically generate a commit message.
 - [ ] **Code Review**: Provides feedback on potential issues in code, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 - [ ] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
 - [ ] **Code Formatting**: Automatically formats code according to a specified style guide.
 - [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code.
 - [ ] **Code Generation**: Generates boilerplate code for common tasks.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via Github Actions)
+- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
 - [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems.
 - [ ] **Linting**: Checks code for linting errors and automatically fixes them where possible.
-- [ ] **Handle Github Issues**: Handles issues that you assign to @aicodebot. It could also suggest labels for new issues based on their content.
+- [ ] **Handle GitHub Issues**: Handles issues that you assign to @aicodebot. It could also suggest labels for new issues based on their content.
 
 ### User Interfaces
 
-- [ ] **Command line installable via pip**: aicodebot can be installed as a Python package using pip
-- [ ] **Chat**: CLI chat interface that knows the context of your code base and can answer questions about it. No more going back and forth between ChatGPT and command line.
-- [ ] **Callable as a Github action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+- [X] **Command-line installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+- [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
+- [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
 - [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 - [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
 - [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 - [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
 - [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
 - [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
 - [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
+- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
 - [ ] **Telling Jokes**: Tells programming jokes. :smiley:
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
 - [ ] **Gif Reactions**: Reacts to messages with relevant and fun gifs. It could also react to specific events in the repository, like the merging of a pull request or the closing of an issue.
 
-<img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" style="width:25%">
+<img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Setup and Usage
 
 Follow the steps below to set up AICodeBot on your machine:
 
 `pip install aicodebot`
```

### Comparing `aicodebot-0.2.6/pyproject.toml` & `aicodebot-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.2.6/setup.py` & `aicodebot-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from setuptools import setup
 
 # Pull in the long description from the README
 with Path("README.md").open("r", encoding="utf-8") as f:
     long_description = f.read()
 
-# Get requirements from requirements.txt
-with Path.open("requirements/requirements.txt") as f:
+# Get requirements from requirements.in
+with Path.open("requirements/requirements.in") as f:
     requirements = f.read().splitlines()
 
 if __name__ == "__main__":  # Only run setup if this is the main file (allows this file to be imported for __version__)
     setup(
         name="aicodebot",
         python_requires=">=3.9",
         version=version,
```

### Comparing `aicodebot-0.2.6/tests/test_cli.py` & `aicodebot-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

