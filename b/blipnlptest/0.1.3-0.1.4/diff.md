# Comparing `tmp/blipnlptest-0.1.3.tar.gz` & `tmp/blipnlptest-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.1.3.tar", max compression
+gzip compressed data, was "blipnlptest-0.1.4.tar", max compression
```

## Comparing `blipnlptest-0.1.3.tar` & `blipnlptest-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-06-22 16:20:12.133924 blipnlptest-0.1.3/blipnlptest/__init__.py
--rw-r--r--   0        0        0     3873 2023-06-22 16:20:12.204742 blipnlptest-0.1.3/blipnlptest/blipnlptest.py
--rw-r--r--   0        0        0     1088 2023-06-22 16:20:12.380299 blipnlptest-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      624 2023-06-22 16:20:12.422816 blipnlptest-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1686 2023-06-22 16:20:12.470694 blipnlptest-0.1.3/README.md
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 blipnlptest-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-22 16:20:12.133924 blipnlptest-0.1.4/blipnlptest/__init__.py
+-rw-r--r--   0        0        0     3879 2023-06-22 17:09:54.406076 blipnlptest-0.1.4/blipnlptest/blipnlptest.py
+-rw-r--r--   0        0        0     1088 2023-06-22 16:20:12.380299 blipnlptest-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      624 2023-06-22 17:08:34.268625 blipnlptest-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1686 2023-06-22 16:20:12.470694 blipnlptest-0.1.4/README.md
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 blipnlptest-0.1.4/PKG-INFO
```

### Comparing `blipnlptest-0.1.3/blipnlptest/blipnlptest.py` & `blipnlptest-0.1.4/blipnlptest/blipnlptest.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
       for i in range(len(df)):
         if df.Entities[i] != '[]':
           ent.append(pd.json_normalize(json.loads(df.Entities[i])).value.tolist())
         else:
           ent.append('')
       
-      df.loc[:, 'Content'] = [cc.test(model='n', intention=df.Intention[x], entities=ent[x]) for x in range(len(df.Entities))]
+      df.loc[:, 'Content'] = [self.test(model='n', intention=df.Intention[x], entities=ent[x]) for x in range(len(df.Entities))]
       
       df = df.sort_values(by='Content',ascending=False)
       return(df)
     
     except KeyError: 
       print("O seu dataframe deve conter as seguintes colunas ['Text', 'Intention', 'Entities', 'Score']. Você pode obtê-las pela tabela vwidentityanalysis.")
 
@@ -45,22 +45,22 @@
     
     if any(col in ['intentions', 'intent', 'intention', 'score', 'entities', 'entity'] for col in self.data.columns.str.lower()):
       print("Ops, o método sentences não é melhor método para a sua operação. Que tal utilizar o identityanalysis?")
 
     else:
 
       df = self.data
-      df = pd.DataFrame([cc.test(model='y',text=t) for t in df.Text])
+      df = pd.DataFrame([self.test(model='y',text=t) for t in df.Text])
 
       df = df[['text','intentions','entities']]
       df['Score'] = df.intentions.apply(lambda s: s[0]['score'])
       df.intentions = df.intentions.apply(lambda i: i[0]['id'])
       df.columns = ['Text', 'Intention', 'Entities', 'Score']
       ent = [pd.json_normalize(df.Entities[i]).value.tolist() if df.Entities[i] != '[]' else '' for i in range(len(df.Text))]
-      df.loc[:, 'Content'] = [cc.test(model='n', intention=df.Intention[x], entities=ent[x]) for x in range(len(df.Entities))]
+      df.loc[:, 'Content'] = [self.test(model='n', intention=df.Intention[x], entities=ent[x]) for x in range(len(df.Entities))]
       df = df.sort_values(by='Content',ascending=False)
 
       return(df)
 
 
   def test(self, model, text=None, intention=None, entities=None):
```

### Comparing `blipnlptest-0.1.3/LICENSE.txt` & `blipnlptest-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.3/pyproject.toml` & `blipnlptest-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blipnlptest"
-version = "0.1.3"
+version = "0.1.4"
 authors = ["Caio Souza <caios@blip.ai>"]
 
 description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo."
 readme = "README.md"
 
 
 classifiers = [
```

### Comparing `blipnlptest-0.1.3/README.md` & `blipnlptest-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.3/PKG-INFO` & `blipnlptest-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.1.3
+Version: 0.1.4
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@blip.ai
 Requires-Python: >=3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

