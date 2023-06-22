# Comparing `tmp/blipnlptest-0.1.1.tar.gz` & `tmp/blipnlptest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.1.1.tar", max compression
+gzip compressed data, was "blipnlptest-0.1.3.tar", max compression
```

## Comparing `blipnlptest-0.1.1.tar` & `blipnlptest-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-06-21 14:54:05.694918 blipnlptest-0.1.1/blipnlptest/__init__.py
--rw-r--r--   0        0        0     1312 2023-06-21 13:26:15.520462 blipnlptest-0.1.1/blipnlptest/blipnlptest.py
--rw-r--r--   0        0        0     1088 2023-06-20 19:54:30.133410 blipnlptest-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      624 2023-06-21 14:53:37.056593 blipnlptest-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1328 2023-06-21 13:26:10.082330 blipnlptest-0.1.1/README.md
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 blipnlptest-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-22 16:20:12.133924 blipnlptest-0.1.3/blipnlptest/__init__.py
+-rw-r--r--   0        0        0     3873 2023-06-22 16:20:12.204742 blipnlptest-0.1.3/blipnlptest/blipnlptest.py
+-rw-r--r--   0        0        0     1088 2023-06-22 16:20:12.380299 blipnlptest-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      624 2023-06-22 16:20:12.422816 blipnlptest-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1686 2023-06-22 16:20:12.470694 blipnlptest-0.1.3/README.md
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 blipnlptest-0.1.3/PKG-INFO
```

### Comparing `blipnlptest-0.1.1/LICENSE.txt` & `blipnlptest-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.1/pyproject.toml` & `blipnlptest-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blipnlptest"
-version = "0.1.1"
+version = "0.1.3"
 authors = ["Caio Souza <caios@blip.ai>"]
 
 description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo."
 readme = "README.md"
 
 
 classifiers = [
```

### Comparing `blipnlptest-0.1.1/README.md` & `blipnlptest-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -10,42 +10,54 @@
 
 ## Uso
 
 Após a instalação do pacote, você terá acesso a classe que permitirá a execução do teste.
 
 Os parâmetros necessários são:
 
-df : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
-key  : chave do bot.
-
+df : dataframe de entrada
+key : chave do bot.
 
 Exemplo do código:
 
 <pre><code>
 
 import blipnlptest as bnt
 
-
 cc = bnt.contentchecker(df, key)
-result = cc.test()
-display(result)
 </code></pre>
 
-Com os parâmetros previamente atribuídos, rodando o código acima você terá como saída a exibição do resultado.
+A composição do df definirá qual método deverá ser utilizado.
 
-A saída contém:
+Caso a análise seja de dados já analisados pelo provedor (envie um dataframe que tenha no mínimo as colunas Text, Intentions, Entities e Score), use:
 
-- A mensagem de entrada;
-- Resposta entregue pelo Assistente de Conteudo;
-- Entidades reconhecidas;
-- N intenções, onde N representa o número de colunas/intenções exibidas (onde a primeira é a que obteve maior confiança).
+<pre><code>
+
+import blipnlptest as bnt
+
+cc = bnt.contentchecker(df, key)
+cc.identityanalysis()
+</code></pre>
 
- 
-Para declarar N, insira o número desejado no método test().
+Se a análise for feita com dados que não foram analisados (envie um dataframe que a coluna de texto tenha o nome Text), use:
 
 <pre><code>
-result = bnt.test(3)
+
+import blipnlptest as bnt
+
+cc = bnt.contentchecker(df, key)
+cc.sentences()
 </code></pre>
 
+OBS: A divisão foi feita para que os dados já rotulados não realizem outra análise no provedor.
+
+Com os parâmetros previamente atribuídos, rodando o código acima você terá como saída a exibição do resultado com:
+
+- A mensagem de entrada;
+- A resposta entregue pelo Assistente de Conteudo;
+- As entidades reconhecidas;
+- A intenção reconhecida;
+- O score.
+
 ## Licença
 
 Esse projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
```

### Comparing `blipnlptest-0.1.1/PKG-INFO` & `blipnlptest-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.1.1
+Version: 0.1.3
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@blip.ai
 Requires-Python: >=3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,43 +32,55 @@
 
 ## Uso
 
 Após a instalação do pacote, você terá acesso a classe que permitirá a execução do teste.
 
 Os parâmetros necessários são:
 
-df : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
-key  : chave do bot.
-
+df : dataframe de entrada
+key : chave do bot.
 
 Exemplo do código:
 
 <pre><code>
 
 import blipnlptest as bnt
 
-
 cc = bnt.contentchecker(df, key)
-result = cc.test()
-display(result)
 </code></pre>
 
-Com os parâmetros previamente atribuídos, rodando o código acima você terá como saída a exibição do resultado.
+A composição do df definirá qual método deverá ser utilizado.
 
-A saída contém:
+Caso a análise seja de dados já analisados pelo provedor (envie um dataframe que tenha no mínimo as colunas Text, Intentions, Entities e Score), use:
 
-- A mensagem de entrada;
-- Resposta entregue pelo Assistente de Conteudo;
-- Entidades reconhecidas;
-- N intenções, onde N representa o número de colunas/intenções exibidas (onde a primeira é a que obteve maior confiança).
+<pre><code>
+
+import blipnlptest as bnt
+
+cc = bnt.contentchecker(df, key)
+cc.identityanalysis()
+</code></pre>
 
- 
-Para declarar N, insira o número desejado no método test().
+Se a análise for feita com dados que não foram analisados (envie um dataframe que a coluna de texto tenha o nome Text), use:
 
 <pre><code>
-result = bnt.test(3)
+
+import blipnlptest as bnt
+
+cc = bnt.contentchecker(df, key)
+cc.sentences()
 </code></pre>
 
+OBS: A divisão foi feita para que os dados já rotulados não realizem outra análise no provedor.
+
+Com os parâmetros previamente atribuídos, rodando o código acima você terá como saída a exibição do resultado com:
+
+- A mensagem de entrada;
+- A resposta entregue pelo Assistente de Conteudo;
+- As entidades reconhecidas;
+- A intenção reconhecida;
+- O score.
+
 ## Licença
 
 Esse projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
```

