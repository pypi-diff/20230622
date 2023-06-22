# Comparing `tmp/readme_ai-0.1.0.tar.gz` & `tmp/readme_ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ai-0.1.0.tar", max compression
+gzip compressed data, was "readme_ai-0.1.1.tar", max compression
```

## Comparing `readme_ai-0.1.0.tar` & `readme_ai-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.1.0/LICENSE
--rw-r--r--   0        0        0    15526 2023-06-22 11:12:16.216069 readme_ai-0.1.0/README.md
--rw-r--r--   0        0        0     1826 2023-06-22 11:08:39.950457 readme_ai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     5949 2023-06-22 11:07:06.076279 readme_ai-0.1.0/src/builder.py
--rw-r--r--   0        0        0     3858 2023-06-22 10:55:41.792898 readme_ai-0.1.0/src/conf.py
--rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.1.0/src/factory.py
--rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.1.0/src/logger.py
--rwxr-xr-x   0        0        0     4591 2023-06-22 11:08:40.164072 readme_ai-0.1.0/src/main.py
--rw-r--r--   0        0        0     7203 2023-06-22 11:13:10.481964 readme_ai-0.1.0/src/model.py
--rw-r--r--   0        0        0     7270 2023-06-22 11:15:22.537516 readme_ai-0.1.0/src/parse.py
--rw-r--r--   0        0        0     6682 2023-06-22 11:13:10.490809 readme_ai-0.1.0/src/preprocess.py
--rw-r--r--   0        0        0     3785 2023-06-22 11:13:10.463162 readme_ai-0.1.0/src/utils.py
--rw-r--r--   0        0        0    16893 1970-01-01 00:00:00.000000 readme_ai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.1.1/LICENSE
+-rw-r--r--   0        0        0    15980 2023-06-22 12:25:52.523548 readme_ai-0.1.1/README.md
+-rw-r--r--   0        0        0     2371 2023-06-22 12:43:11.853511 readme_ai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.1.1/src/readme_ai/__init__.py
+-rw-r--r--   0        0        0     5949 2023-06-22 12:21:52.222176 readme_ai-0.1.1/src/readme_ai/builder.py
+-rw-r--r--   0        0        0     3858 2023-06-22 10:55:41.792898 readme_ai-0.1.1/src/readme_ai/conf.py
+-rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.1.1/src/readme_ai/factory.py
+-rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.1.1/src/readme_ai/logger.py
+-rwxr-xr-x   0        0        0     4606 2023-06-22 12:21:52.303932 readme_ai-0.1.1/src/readme_ai/main.py
+-rw-r--r--   0        0        0     7392 2023-06-22 12:21:52.188140 readme_ai-0.1.1/src/readme_ai/model.py
+-rw-r--r--   0        0        0     7258 2023-06-22 12:21:52.279983 readme_ai-0.1.1/src/readme_ai/parse.py
+-rw-r--r--   0        0        0     6620 2023-06-22 12:21:52.087982 readme_ai-0.1.1/src/readme_ai/preprocess.py
+-rw-r--r--   0        0        0     3769 2023-06-22 12:21:52.244679 readme_ai-0.1.1/src/readme_ai/utils.py
+-rw-r--r--   0        0        0    17736 1970-01-01 00:00:00.000000 readme_ai-0.1.1/PKG-INFO
```

### Comparing `readme_ai-0.1.0/LICENSE` & `readme_ai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.0/README.md` & `readme_ai-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
     <img src="https://img.shields.io/badge/Python-3776AB.svg?stylee&logo=Python&logoColor=white" alt="Python" />
     <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?stylee&logo=Pytest&logoColor=white" alt="pytest" />
     <img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?stylee&logo=GNU-Bash&logoColor=white" alt="Bash" />
     <img src="https://img.shields.io/badge/Anaconda-44A833.svg?&logo=Anaconda&logoColor=white" alt="Anaconda" />
   </p>
 
-  ![GitHub top language](https://img.shields.io/github/languages/top/eli64s/README-AI?color=5D6D7E)
+  ![PyPI](https://img.shields.io/pypi/v/README-AI?logo=python&color=5D6D7E)
+  ![GitHub license](https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E)
   ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/eli64s/README-AI?color=5D6D7E)
   ![GitHub last commit](https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E)
-  ![GitHub license](https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E)
+
 </div>
 
 ---
 
 ## 📒 Table of Contents
 
 - [📒 Table of Contents](#-table-of-contents)
@@ -59,15 +60,15 @@
 
 Additionally, regularly monitor your API usage and costs by visiting the [OpenAI API Usage](https://platform.openai.com/account/usage).
 
 ---
 
 ## 👾 Demo
 
-[![demo](./examples/imgs/demo.png)](https://youtu.be/0wbgjL0FMxY)
+[![demo](https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/demo.png)](https://youtu.be/0wbgjL0FMxY)
 
 ---
 
 
 ## ⚙️ Features
 
 <h1 align="center">1.<br>👇<br><br>📑 Codebase Documentation</h1>
@@ -79,15 +80,15 @@
         <li>Code summaries are generated for each file via OpenAI's <i>gpt-3.5-turbo</i> engine.</li>
         <li>Summaries are processed to check formatting and displayed in Markdown tables.</li>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/modules.png" alt="docs">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/modules.png" alt="docs">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒉<br>👇<br><br>🎖 Badges</h1>
 <table>
   <tr>
@@ -98,15 +99,15 @@
         <li>Project dependencies and metadata are visualized using <a href="https://shields.io/">Shields.io</a> badges.</li>
         <li>Badges are sorted by hex code, displayed from light to dark hues.</li>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/header.png" alt="docs">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/header.png" alt="docs">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒊<br>👇<br><br>🧚 Prompted Text Generation</h1>
 <table>
   <tr>
@@ -121,25 +122,25 @@
           </li>
         </ul>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/features.png" alt="features">
-      <img src="./examples/imgs/overview.png" alt="overview">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/features.png" alt="features">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/overview.png" alt="overview">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒋<br>👇<br><br>🌲 Repository Tree</h1>
 <table>
   <tr>
     <td>
-      <img src="./examples/imgs/tree.png" alt="tree">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/tree.png" alt="tree">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒌<br>👇<br><br>📦 Dynamic User Setup Guides</h1>
 <table>
   <tr>
@@ -154,24 +155,24 @@
           </li>
         </ul>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/getting_started.png" alt="getting_started">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/getting_started.png" alt="getting_started">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒍<br>👇<br><br>👩‍💻Contributing Guidelines & more!</h1>
 
 | |
 |-----------------------------------------------|
-| ![contribute](./examples/imgs/closing.png) |
+| ![contribute](https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/closing.png) |
 
 <h1 align="center">⒎<br>👇<br><br>💥 Example Files</h1>
 <p align="center">Markdown example files generated by the README-AI app!</p>
 <div align="center">
   <table align="center">
     <tr>
       <th></th>
@@ -329,14 +330,20 @@
 
 2. Navigate to the README-AI directory.
 ```sh
 cd README-AI
 ```
 
 3. Use one of the following methods to install the required dependencies:
+
+```sh
+# With Pip
+pip install readme-ai
+```
+
 ```sh
 # With Bash
 $ bash setup/setup.sh
 ```
 
 ```sh
 # With Conda
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
     ****** [https://img.icons8.com/?size=512&id=55494&format=png] [https://
              img.icons8.com/?size=512&id=kTuxVYRKeKEY&format=png]
                                README-AI ******
       **** â¦ Generate beautiful and informative README documents. ****
         **** â¦ Developed with OpenAI's GPT language model APIs. ****
 
             [Markdown] [OpenAI] [Python] [pytest] [Bash] [Anaconda]
-  ![GitHub top language](https://img.shields.io/github/languages/top/eli64s/
-   README-AI?color=5D6D7E) ![GitHub commit activity](https://img.shields.io/
- github/commit-activity/m/eli64s/README-AI?color=5D6D7E) ![GitHub last commit]
-  (https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E) !
+  ![PyPI](https://img.shields.io/pypi/v/README-AI?logo=python&color=5D6D7E) !
      [GitHub license](https://img.shields.io/github/license/eli64s/README-
-                               AI?color=5D6D7E)
+   AI?color=5D6D7E) ![GitHub commit activity](https://img.shields.io/github/
+commit-activity/m/eli64s/README-AI?color=5D6D7E) ![GitHub last commit](https://
+       img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E)
 --- ## ð Table of Contents - [ð Table of Contents](#-table-of-contents) -
 [ð« Overview](#-overview) - [ð¯ *Motivation*](#-motivation) - [â ï¸
 *Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [âï¸ Features](#ï¸-
 features) - [ð Getting Started](#-getting-started) - [âï¸ Dependencies]
 (#ï¸-dependencies) - [ð Repository](#-repository) - [ð OpenAI API Setup]
 (#-openai-api-setup) - [ð» Installation](#-installation) - [ð® Using
 README-AI](#-using-readme-ai) - [ð§ª Running Tests](#-running-tests) - [ð 
@@ -33,16 +32,17 @@
 use open-source tools. #### â ï¸ *Disclaimer* README-AI is currently under
 development and has an opinionated configuration and setup. While this tool
 provides an excellent starting point for documentation, its important to review
 all text generated by the OpenAI API to ensure it accurately represents your
 codebase. Ensure all content in your repository is free of sensitive
 information before executing. Additionally, regularly monitor your API usage
 and costs by visiting the [OpenAI API Usage](https://platform.openai.com/
-account/usage). --- ## ð¾ Demo [![demo](./examples/imgs/demo.png)](https://
-youtu.be/0wbgjL0FMxY) --- ## âï¸ Features
+account/usage). --- ## ð¾ Demo [![demo](https://raw.githubusercontent.com/
+eli64s/README-AI/main/examples/imgs/demo.png)](https://youtu.be/0wbgjL0FMxY) --
+- ## âï¸ Features
                                    ****** 1.
                                      ð
 
                       ð Codebase Documentation ******
 **** â¦ Repository File Summaries ****
     * Code summaries are generated for each file via OpenAI's gpt-3.5-turbo
       engine.
@@ -85,16 +85,16 @@
     * README-AI currently supports this feature for code written with:
           o Python, Rust, Go, C, Kotlin, Java, JavaScript, TypeScript.
 [getting_started]
                                   ****** â
                                      ð
 
                ð©âð»Contributing Guidelines & more! ******
-| | |-----------------------------------------------| | ![contribute](./
-examples/imgs/closing.png) |
+| | |-----------------------------------------------| | ![contribute](https://
+raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/closing.png) |
                                   ****** â
                                      ð
 
                            ð¥ Example Files ******
             Markdown example files generated by the README-AI app!
         Example File         Repository          Language               Bytes
 1ï¸�readme-python.md     readme-ai           Python                 19,839
@@ -146,37 +146,37 @@
 API is not free and you will be charged for each request made, which can
 accumulate rapidly. > > - The generation of the README.md file should typically
 complete in under 1 minute. If it takes longer than a few minutes, please
 terminate the process. > --- ### ð» Installation 1. Clone the README-AI
 repository to your local machine. ```sh git clone https://github.com/eli64s/
 README-AI ``` 2. Navigate to the README-AI directory. ```sh cd README-AI ``` 3.
 Use one of the following methods to install the required dependencies: ```sh #
-With Bash $ bash setup/setup.sh ``` ```sh # With Conda $ conda env create -
-f setup/environment.yaml $ conda activate readme_ai $ pip install -
-r requirements.txt ``` ```sh # With Poetry $ poetry install ``` ```sh # With
-Docker $ docker pull zeroxeli/readme-ai:v0.1.0 ``` ### ð® Using README-AI Use
-the command-line to provide the OpenAI API key (if not already set) and specify
-an output path for your README file, along with the path to your local
-repository or remote code repository. You can also provide the output path in
-the [configuration file](./conf/conf.toml) Command-Line Arguments: - `-k` or `-
--api-key`: Your OpenAI API key. - `-o` or `--output`: The output path for your
-README.md file. - `-r` or `--repository`: The URL or path to your code
-repository. - `-t` or `--template`: The README template format to use. (Coming
-soon!) ```sh python src/main.py --api-key abc123 --output readme-ai.md --
-repository https://github.com/eli64s/readme-ai ``` Alternatively, export your
-OpenAI API key as an environment variable and run the following command: ```sh
-conda activate readme_ai export OPENAI_API_KEY=sk123abc456def7890 python src/
-main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai ``` ```sh # With
-Poetry poetry shell export OPENAI_API_KEY=sk123abc456def7890 poetry run python
-src/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai ``` ```sh #
-Run with Docker docker run -it -e OPENAI_API_KEY="your-api-key" -v "$(pwd)":/
-app -w /app zeroxeli/readme-ai:v0.1.0 \ python src/main.py -o readme-ai.md -
-r https://github.com/eli64s/readme-ai ``` ### ð§ª Running Tests To run the
-unit-tests for README-AI, use the following command. ```bash bash scripts/
-test.sh ```
+With Pip pip install readme-ai ``` ```sh # With Bash $ bash setup/setup.sh ```
+```sh # With Conda $ conda env create -f setup/environment.yaml $ conda
+activate readme_ai $ pip install -r requirements.txt ``` ```sh # With Poetry $
+poetry install ``` ```sh # With Docker $ docker pull zeroxeli/readme-ai:v0.1.0
+``` ### ð® Using README-AI Use the command-line to provide the OpenAI API key
+(if not already set) and specify an output path for your README file, along
+with the path to your local repository or remote code repository. You can also
+provide the output path in the [configuration file](./conf/conf.toml) Command-
+Line Arguments: - `-k` or `--api-key`: Your OpenAI API key. - `-o` or `--
+output`: The output path for your README.md file. - `-r` or `--repository`: The
+URL or path to your code repository. - `-t` or `--template`: The README
+template format to use. (Coming soon!) ```sh python src/main.py --api-key
+abc123 --output readme-ai.md --repository https://github.com/eli64s/readme-ai
+``` Alternatively, export your OpenAI API key as an environment variable and
+run the following command: ```sh conda activate readme_ai export
+OPENAI_API_KEY=sk123abc456def7890 python src/main.py -o readme-ai.md -r https:/
+/github.com/eli64s/readme-ai ``` ```sh # With Poetry poetry shell export
+OPENAI_API_KEY=sk123abc456def7890 poetry run python src/main.py -o readme-ai.md
+-r https://github.com/eli64s/readme-ai ``` ```sh # Run with Docker docker run -
+it -e OPENAI_API_KEY="your-api-key" -v "$(pwd)":/app -w /app zeroxeli/readme-
+ai:v0.1.0 \ python src/main.py -o readme-ai.md -r https://github.com/eli64s/
+readme-ai ``` ### ð§ª Running Tests To run the unit-tests for README-AI, use
+the following command. ```bash bash scripts/test.sh ```
                                                                     ð_Return
 --- ## ð  Future Development - [X] Add additional language support for
 populating the *installation*, *usage*, and *test* README sections. - [ ]
 Design and implement a variety of README template formats and styles. - [ ] Add
 feature to select the output language of the README file (i.e. CN, ES, FR, JA,
 KO, RU). - [ ] Create UI with [Textual](https://github.com/Textualize/textual)
 or another framework to improve user experience. --- ## ð¤ Contributing
```

### Comparing `readme_ai-0.1.0/src/builder.py` & `readme_ai-0.1.1/src/readme_ai/builder.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.0/src/conf.py` & `readme_ai-0.1.1/src/readme_ai/conf.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.0/src/factory.py` & `readme_ai-0.1.1/src/readme_ai/factory.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.0/src/logger.py` & `readme_ai-0.1.1/src/readme_ai/logger.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.0/src/main.py` & `readme_ai-0.1.1/src/readme_ai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,16 @@
         await gpt.close()
 
     format_text_to_markdown(name, slogan, overview, features)
     builder.build_markdown(CONF, CONF_HELPER, dependencies, code_summary)
     LOGGER.info("README-AI execution complete.\n")
 
 
-def get_dependencies(
-    scanner: preprocess.RepositoryParserWrapper, repository: str
-) -> Tuple[List[str], str]:
+def get_dependencies(scanner: preprocess.RepositoryParserWrapper,
+                     repository: str) -> Tuple[List[str], str]:
     """Extracts dependencies and file_text using the scanner."""
     dependencies, file_text = scanner.get_dependencies(repository)
     LOGGER.info(f"Codebase dependencies: {dependencies}")
     LOGGER.info(f"Total files: {len(file_text)}")
     return dependencies, file_text
```

### Comparing `readme_ai-0.1.0/src/model.py` & `readme_ai-0.1.1/src/readme_ai/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,16 @@
             http2=True,
             timeout=30,
             limits=httpx.Limits(max_keepalive_connections=10, max_connections=100),
         )
         self.last_request_time = time.monotonic()
         self.rate_limit_semaphore = asyncio.Semaphore(self.rate_limit)
 
-    async def code_to_text(
-        self, ignore: dict, files: Dict[str, str], prompt: str
-    ) -> Dict[str, str]:
+    async def code_to_text(self, ignore: dict, files: Dict[str, str],
+                           prompt: str) -> Dict[str, str]:
         """Converts code to natural language text using large language models.
 
         Parameters
         ----------
         ignore : dict
             Files, directories, or file extensions to ignore.
         files : Dict[str, str]
@@ -65,17 +64,17 @@
         -------
         Dict[str, str]
             Dictionary of file paths and their corresponding summaries.
         """
         tasks = []
         for path, contents in files.items():
             if not (
-                all(idir not in path.parts for idir in ignore.get("directories", []))
-                and path.name not in ignore.get("files", [])
-                and path.suffix not in ignore.get("extensions", [])
+                all(idir not in path.parts for idir in ignore.get("directories", [])
+                   ) and path.name not in ignore.get("files", []) and
+                path.suffix not in ignore.get("extensions", [])
             ):
                 self.LOGGER.warning(f"Ignoring file: {path}")
                 continue
 
             prompt_code = prompt.format(contents)
             prompt_length = len(prompt_code.split())
             if prompt_length > self.tokens_max:
@@ -130,21 +129,20 @@
         response_list = [summary for _, summary in sorted(results)]
         return response_list
 
     @retry(
         stop=stop_after_attempt(3),
         wait=wait_exponential(multiplier=1, min=4, max=10),
         retry=(
-            retry_if_exception_type(Exception)
-            | retry_if_exception_type(httpx.HTTPStatusError)
+            retry_if_exception_type(Exception) |
+            retry_if_exception_type(httpx.HTTPStatusError)
         ),
     )
-    async def generate_text(
-        self, index: str, prompt: str, type: str, tokens: int
-    ) -> Tuple[str, str]:
+    async def generate_text(self, index: str, prompt: str, type: str,
+                            tokens: int) -> Tuple[str, str]:
         """Handles the request to the OpenAI API to generate text.
 
         Parameters
         ----------
         index
             Unique identifier for current prompt (i.e file path or index)
         prompt
@@ -160,21 +158,25 @@
         """
         try:
             async with self.rate_limit_semaphore:
                 response = await self.http_client.post(
                     self.endpoint,
                     headers={"Authorization": f"Bearer {openai.api_key}"},
                     json={
-                        "messages": [
-                            {
-                                "role": "system",
-                                "content": "You're a brilliant Tech Lead.",
-                            },
-                            {"role": "user", "content": prompt},
-                        ],
+                        "messages":
+                            [
+                                {
+                                    "role": "system",
+                                    "content": "You're a brilliant Tech Lead.",
+                                },
+                                {
+                                    "role": "user",
+                                    "content": prompt
+                                },
+                            ],
                         "model": self.engine,
                         "temperature": self.temperature,
                         "max_tokens": tokens,
                     },
                 )
                 response.raise_for_status()
                 data = response.json()
```

### Comparing `readme_ai-0.1.0/src/parse.py` & `readme_ai-0.1.1/src/readme_ai/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,15 @@
 def parse_pyproject_toml(toml_content: str) -> List[str]:
     """Extracts dependencies from a pyproject.toml file."""
     try:
         data = toml.loads(toml_content)
         dependencies = data.get("dependencies", {})
         optional_dependencies = data.get("optional-dependencies", {})
         return list(dependencies.keys()) + [
-            dep_name
-            for dep_list in optional_dependencies.values()
+            dep_name for dep_list in optional_dependencies.values()
             for dep_name in dep_list
         ]
     except toml.TomlDecodeError as exc:
         LOGGER.error(f"Error parsing pyproject.toml: {str(exc)}")
     return []
```

### Comparing `readme_ai-0.1.0/src/preprocess.py` & `readme_ai-0.1.1/src/readme_ai/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,27 +115,25 @@
         )
         if "setup" not in df.columns:
             df["setup"] = [None] * len(df)
 
         df[["install", "run", "test"]] = pd.DataFrame.from_records(
             df["setup"].to_list(), columns=["install", "run", "test"]
         )
-        return df[
-            [
-                "name",
-                "tokens",
-                "content",
-                "install",
-                "run",
-                "test",
-                "extension",
-                "language",
-                "path",
-            ]
-        ]
+        return df[[
+            "name",
+            "tokens",
+            "content",
+            "install",
+            "run",
+            "test",
+            "extension",
+            "language",
+            "path",
+        ]]
 
     def get_dependency_file_contents(self, df: pd.DataFrame) -> List[str]:
         """Extracts dependency file contents from the DataFrame."""
         file_parsers = self._get_file_parsers()
         dependency_files = df[df["name"].str.contains("|".join(file_parsers.keys()))]
 
         parsed_contents = []
```

### Comparing `readme_ai-0.1.0/src/utils.py` & `readme_ai-0.1.1/src/readme_ai/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,16 @@
 
 def is_valid_file(helper: conf.ConfigHelper, path: Path) -> bool:
     """Checks if a file is valid for processing."""
     ignore_dirs = helper.ignore_files.get("directories", [])
     ignore_files = helper.ignore_files.get("filenames", [])
     ignore_extensions = helper.ignore_files.get("extensions", [])
     return (
-        path.is_file()
-        and all(dir not in path.parts for dir in ignore_dirs)
-        and path.name not in ignore_files
-        and path.suffix not in ignore_extensions
+        path.is_file() and all(dir not in path.parts for dir in ignore_dirs) and
+        path.name not in ignore_files and path.suffix not in ignore_extensions
     )
 
 
 def is_valid_url(url: str) -> bool:
     """Check if a given string is a valid URL."""
     regex = re.compile(
         r"^(?:http|ftp)s?://"
```

### Comparing `readme_ai-0.1.0/PKG-INFO` & `readme_ai-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: readme-ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: 🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫
+Home-page: https://github.com/eli64s/README-AI
 License: MIT
+Keywords: markdown,readme,readme-badges,documentation-generator,markdown-generator,automated-documentation,awesome-readme,readme-generator,python-ai,gpt-3,openai-api,shieldsio-badges,gpt-4,llms,openai-python,chatgpt-python,llmops,openai-chatbot,gpt-35-turbo
 Author: Eli
 Author-email: 43382407+eli64s@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,14 +29,15 @@
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: responses (>=0.23.1,<0.24.0)
 Requires-Dist: setuptools (>=68.0.0,<69.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Project-URL: Documentation, https://github.com/eli64s/README-AI/blob/main/README.md
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1 align="center">
     <img src="https://img.icons8.com/?size=512&id=55494&format=png" width="80"/>
     <img src="https://img.icons8.com/?size=512&id=kTuxVYRKeKEY&format=png" width="80"/>
     <br>README-AI
@@ -47,18 +50,19 @@
     <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
     <img src="https://img.shields.io/badge/Python-3776AB.svg?stylee&logo=Python&logoColor=white" alt="Python" />
     <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?stylee&logo=Pytest&logoColor=white" alt="pytest" />
     <img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?stylee&logo=GNU-Bash&logoColor=white" alt="Bash" />
     <img src="https://img.shields.io/badge/Anaconda-44A833.svg?&logo=Anaconda&logoColor=white" alt="Anaconda" />
   </p>
 
-  ![GitHub top language](https://img.shields.io/github/languages/top/eli64s/README-AI?color=5D6D7E)
+  ![PyPI](https://img.shields.io/pypi/v/README-AI?logo=python&color=5D6D7E)
+  ![GitHub license](https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E)
   ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/eli64s/README-AI?color=5D6D7E)
   ![GitHub last commit](https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E)
-  ![GitHub license](https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E)
+
 </div>
 
 ---
 
 ## 📒 Table of Contents
 
 - [📒 Table of Contents](#-table-of-contents)
@@ -94,15 +98,15 @@
 
 Additionally, regularly monitor your API usage and costs by visiting the [OpenAI API Usage](https://platform.openai.com/account/usage).
 
 ---
 
 ## 👾 Demo
 
-[![demo](./examples/imgs/demo.png)](https://youtu.be/0wbgjL0FMxY)
+[![demo](https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/demo.png)](https://youtu.be/0wbgjL0FMxY)
 
 ---
 
 
 ## ⚙️ Features
 
 <h1 align="center">1.<br>👇<br><br>📑 Codebase Documentation</h1>
@@ -114,15 +118,15 @@
         <li>Code summaries are generated for each file via OpenAI's <i>gpt-3.5-turbo</i> engine.</li>
         <li>Summaries are processed to check formatting and displayed in Markdown tables.</li>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/modules.png" alt="docs">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/modules.png" alt="docs">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒉<br>👇<br><br>🎖 Badges</h1>
 <table>
   <tr>
@@ -133,15 +137,15 @@
         <li>Project dependencies and metadata are visualized using <a href="https://shields.io/">Shields.io</a> badges.</li>
         <li>Badges are sorted by hex code, displayed from light to dark hues.</li>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/header.png" alt="docs">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/header.png" alt="docs">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒊<br>👇<br><br>🧚 Prompted Text Generation</h1>
 <table>
   <tr>
@@ -156,25 +160,25 @@
           </li>
         </ul>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/features.png" alt="features">
-      <img src="./examples/imgs/overview.png" alt="overview">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/features.png" alt="features">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/overview.png" alt="overview">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒋<br>👇<br><br>🌲 Repository Tree</h1>
 <table>
   <tr>
     <td>
-      <img src="./examples/imgs/tree.png" alt="tree">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/tree.png" alt="tree">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒌<br>👇<br><br>📦 Dynamic User Setup Guides</h1>
 <table>
   <tr>
@@ -189,24 +193,24 @@
           </li>
         </ul>
       </ul>
     </td>
   </tr>
   <tr>
     <td>
-      <img src="./examples/imgs/getting_started.png" alt="getting_started">
+      <img src="https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/getting_started.png" alt="getting_started">
     </td>
   </tr>
 </table>
 
 <h1 align="center">⒍<br>👇<br><br>👩‍💻Contributing Guidelines & more!</h1>
 
 | |
 |-----------------------------------------------|
-| ![contribute](./examples/imgs/closing.png) |
+| ![contribute](https://raw.githubusercontent.com/eli64s/README-AI/main/examples/imgs/closing.png) |
 
 <h1 align="center">⒎<br>👇<br><br>💥 Example Files</h1>
 <p align="center">Markdown example files generated by the README-AI app!</p>
 <div align="center">
   <table align="center">
     <tr>
       <th></th>
@@ -364,14 +368,20 @@
 
 2. Navigate to the README-AI directory.
 ```sh
 cd README-AI
 ```
 
 3. Use one of the following methods to install the required dependencies:
+
+```sh
+# With Pip
+pip install readme-ai
+```
+
 ```sh
 # With Bash
 $ bash setup/setup.sh
 ```
 
 ```sh
 # With Conda
```

