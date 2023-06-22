# Comparing `tmp/texto_transformer-0.0.2.tar.gz` & `tmp/texto_transformer-0.0.3.tar.gz`

## Comparing `texto_transformer-0.0.2.tar` & `texto_transformer-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/requirements.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/__init__.py
--rw-r--r--   0        0        0    52677 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/textotransformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/medidas.py
--rw-r--r--   0        0        0    37639 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/mensurador.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/mensuradorenum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/modeloarguments.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/modeloenum.py
--rw-r--r--   0        0        0    29287 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/pln/__init__.py
--rw-r--r--   0        0        0    15485 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/pln/pln.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/__init__.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utilambiente.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utilarquivo.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utilconstantes.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utiltempo.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utiltexto.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/LICENSE
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/README.md
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/requirements.txt
+-rw-r--r--   0        0        0    69971 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/notebooks/ExemplosTextoTransformer.ipynb
+-rw-r--r--   0        0        0   529102 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/notebooks/TestesTextoTransformer.ipynb
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/__init__.py
+-rw-r--r--   0        0        0    53070 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/textotransformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/__init__.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/medidas.py
+-rw-r--r--   0        0        0    37674 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/mensurador.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/mensuradorenum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/modeloarguments.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/modeloenum.py
+-rw-r--r--   0        0        0    31461 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/pln/__init__.py
+-rw-r--r--   0        0        0    16667 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/pln/pln.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/__init__.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utilambiente.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utilarquivo.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utilconstantes.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utiltempo.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utiltexto.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/README.md
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/PKG-INFO
```

### Comparing `texto_transformer-0.0.2/textotransformer/textotransformer.py` & `texto_transformer-0.0.3/textotransformer/textotransformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,18 @@
         # Parâmetro recebido para o modelo da ferramenta de pln
         modelo_argumentos.modelo_spacy = modelo_spacy
                 
         # Carrega o modelo de linguagem da classe transformador
         self.transformer = Transformer(modelo_args=modelo_argumentos)
     
         # Recupera o modelo de linguagem.
-        self.model = self.transformer.get_auto_model()
+        self.model = self.transformer.getAutoMmodel()
     
         # Recupera o tokenizador.     
-        self.tokenizer = self.transformer.get_tokenizer()
+        self.tokenizer = self.transformer.getTokenizer()
         
         # Especifica de qual camada utilizar os embeddings                
         logger.info("Utilizando embeddings do modelo da {} camada(s).".format(listaTipoCamadas[modelo_argumentos.camadas_embeddings][LISTATIPOCAMADA_NOME]))
                     
         # Especifica camadas para recuperar os embeddings
         modelo_argumentos.camadas_embeddings = camadas_embeddings
       
@@ -103,19 +103,22 @@
 
         # Mensagem de carregamento da classe
         logger.info("Classe TextoTransformer carregada: {}.".format(modelo_argumentos))
     
     # ============================   
     def __repr__(self):
         '''
-        Retorna uma string com descrição do objeto
+        Retorna uma string com descrição do objeto.
         '''
-        return "Classe ({}) com modelo Transformer: {} e NLP: {} ".format(self.__class__.__name__, 
-                                                                          self.get_transformer().auto_model.__class__.__name__,
-                                                                          self.get_pln().model_pln.__class__.__name__)
+        
+        return "Classe ({}) com Transformer {} carregada com o modelo {} e NLP {} carregado com o modelo {} ".format(self.__class__.__name__, 
+                                                                                                            self.getTransformer().auto_model.__class__.__name__,
+                                                                                                            modelo_argumentos.pretrained_model_name_or_path,
+                                                                                                            self.getPln().model_pln.__class__.__name__,
+                                                                                                            modelo_argumentos.modelo_spacy)
     
     # ============================
     def _defineEstrategiaPooling(self, estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN):
         ''' 
         Define a estratégia de pooling para os parâmetros do modelo.
 
         Parâmetros:
@@ -293,15 +296,15 @@
          
         Retorna um dicionário com:
             tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
             input_ids uma lista com os ids dos tokens de entrada mapeados em seus índices do vocabuário.
             token_type_ids uma lista com os tipos dos tokens.
             attention_mask uma lista com os as máscaras de atenção indicando com '1' os tokens  pertencentes à sentença.
         '''
-        return self.get_transformer().tokenize(texto)
+        return self.getTransformer().tokenize(texto)
     
     # ============================
     def getCodificacaoCompleta(self, texto: Union[str, List[str]],
                     tamanho_lote: int = 32, 
                     mostra_barra_progresso: bool = False,                     
                     convert_to_numpy: bool = False,         
                     device: str = None):
@@ -360,24 +363,24 @@
                                   desc="Lotes", 
                                   disable=not mostra_barra_progresso):
             
             # Recupera um lote
             lote_textos = texto[start_index:start_index+tamanho_lote]
 
             # Tokeniza o lote usando o modelo
-            lote_textos_tokenizados = self.get_transformer().tokenize(lote_textos)
+            lote_textos_tokenizados = self.getTransformer().tokenize(lote_textos)
 
             # Adiciona ao device gpu ou cpu
-            lote_textos_tokenizados = self.get_transformer().batch_to_device(lote_textos_tokenizados, device)
+            lote_textos_tokenizados = self.getTransformer().batchToDevice(lote_textos_tokenizados, device)
             
             # Recupera os embeddings do modelo
             with torch.no_grad():
 
                 # Recupera a saída da rede
-                output_rede = self.get_transformer().getSaidaRede(lote_textos_tokenizados)
+                output_rede = self.getTransformer().getSaidaRede(lote_textos_tokenizados)
 
                 # Lista para os embeddings do texto
                 embeddings = []
 
                 # Percorre todas as saídas(textos) do lote
                 #for token_embeddings, attention_mask in zip(output_rede['token_embeddings'], output_rede['attention_mask']):                    
                 for token_embeddings, input_ids, attention_mask,token_type_ids, tokens_texto_mcl,texto_original,all_layer_embeddings in zip(output_rede['token_embeddings'], 
@@ -470,23 +473,23 @@
                                   tamanho_lote, 
                                   desc="Lotes", 
                                   disable=not mostra_barra_progresso):
             # Recupera um lote
             lote_textos = textos_ordenados[start_index:start_index+tamanho_lote]
 
             # Tokeniza o lote
-            lote_textos_tokenizados = self.get_transformer().tokenize(lote_textos)
+            lote_textos_tokenizados = self.getTransformer().tokenize(lote_textos)
             # Adiciona ao device gpu ou cpu
-            lote_textos_tokenizados = self.get_transformer().batch_to_device(lote_textos_tokenizados, device)
+            lote_textos_tokenizados = self.getTransformer().batchToDevice(lote_textos_tokenizados, device)
             
             # Recupera os embeddings do modelo
             with torch.no_grad():
 
                 # Recupera a saída da rede
-                output_rede = self.get_transformer().getSaidaRede(lote_textos_tokenizados)
+                output_rede = self.getTransformer().getSaidaRede(lote_textos_tokenizados)
 
                 embeddings = []
                 # Percorre todas as saídas(textos) do lote
                 for token_emb, attention in zip(output_rede['token_embeddings'], output_rede['attention_mask']):                    
                     ultimo_mask_id = len(attention)-1
                     
                     # Localiza o último token de "attention_mask" igual a 1
@@ -527,15 +530,15 @@
             input_ids uma lista com os textos indexados.            
             attention_mask uma lista com os as máscaras de atenção
             token_type_ids uma lista com os tipos dos tokens.            
             tokens_texto uma lista com os textos tokenizados com os tokens especiais.
             texto_original uma lista com os textos originais.
             all_layer_embeddings uma lista com os embeddings de todas as camadas.
         '''
-        return self.get_transformer().getSaidaRede(texto)
+        return self.getTransformer().getSaidaRede(texto)
 
    # ============================
     def getEmbeddingTexto(self, texto: Union[str, List[str]], 
                           estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN):
         '''
         Recebe um texto (string ou uma lista de strings) e retorna os embeddings consolidados dos tokens do texto utilizando estratégia pooling especificada(MEAN, MAX).
             
@@ -719,15 +722,15 @@
             # Recupera os embeddings do texto  
             embeddings_texto = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]            
 
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
             tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]            
                         
             # Recupera as sentenças do texto
-            lista_sentencas_texto = self.get_pln().getListaSentencasTexto(texto_embeddings['texto_original'][i])
+            lista_sentencas_texto = self.getPln().getListaSentencasTexto(texto_embeddings['texto_original'][i])
 
             # Lista de embeddings das sentenças do texto    
             lista_embeddings_tokens_sentencas_texto_media = []
             lista_embeddings_tokens_sentencas_texto_maximo = []
             
             # Percorre as sentenças do texto
             for j, sentenca in enumerate(lista_sentencas_texto):
@@ -862,30 +865,30 @@
                      }
         )
 
         # Percorre os textos da lista.
         for i, texto in enumerate(texto_embeddings['texto_original']):
             
             # Recupera o texto tokenizado pela ferramenta de pln do texto original
-            lista_tokens_texto_pln = self.get_pln().getTokensTexto(texto_embeddings['texto_original'][i])
+            lista_tokens_texto_pln = self.getPln().getTokensTexto(texto_embeddings['texto_original'][i])
             
             # Recupera os embeddings do texto  
             embeddings_texto = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]            
             
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
             tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]        
             
             # Concatena os tokens gerandos pela ferramenta de pln
             tokens_texto_concatenado = " ".join(lista_tokens_texto_pln)
 
             # Recupera os embeddings e tokens de palavra            
-            saidaEmbeddingPalavra = self.get_transformer().getTokensEmbeddingsPOSTexto(embeddings_texto,
+            saidaEmbeddingPalavra = self.getTransformer().getTokensEmbeddingsPOSTexto(embeddings_texto,
                                                                                        tokens_texto_mcl,
                                                                                        tokens_texto_concatenado,
-                                                                                       self.get_pln())
+                                                                                       self.getPln())
 
             #Acumula a saída do método 
             saida['texto_original'].append(texto_embeddings['texto_original'][i])
             saida['tokens_texto'].append(saidaEmbeddingPalavra['tokens_texto'])
             saida['tokens_texto_mcl'].append(tokens_texto_mcl)
             saida['tokens_oov_texto_mcl'].append(saidaEmbeddingPalavra['tokens_oov_texto_mcl'])            
             saida['tokens_texto_pln'].append(lista_tokens_texto_pln)
@@ -1003,25 +1006,25 @@
             else:
                 if len(texto) == 0 or isinstance(texto[0], int):  #String vazia ou lista de ints
                     return len(texto)
                 else:
                     return sum([len(t) for t in texto])      ##Soma do comprimento de strings individuais
     
     # ============================
-    def get_model(self):
+    def getModel(self):
         return self.model
 
     # ============================
-    def get_tokenizer(self):
+    def getTokenizer(self):
         return self.tokenizer
 
     # ============================
-    def get_transformer(self):
+    def getTransformer(self):
         return self.transformer
 
     # ============================    
-    def get_mensurador(self):
+    def getMensurador(self):
         return self.mensurador        
         
     # ============================        
-    def get_pln(self):
+    def getPln(self):
         return self.pln
```

### Comparing `texto_transformer-0.0.2/textotransformer/mensurador/medidas.py` & `texto_transformer-0.0.3/textotransformer/mensurador/medidas.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 # ============================  
 def similaridadeCoseno(texto1, texto2):
     '''
     Similaridade do cosseno dos embeddgins dos textos.
     
     Parâmetros:
     `texto1` - Um texto a ser medido.           
-    `texto2` - Um texto a ser medido.                 
+    `texto2` - Um texto a ser medido. 
+
+    Retorno:
+    A similaridade do cosseno entre os textos.                
     '''
     
     similaridade = 1 - cosine(texto1, texto2)
     
     return similaridade
 
 def PytorchSimilaridadeCoseno(a: torch.Tensor, b: torch.Tensor):
@@ -41,24 +44,28 @@
         a = a.unsqueeze(0)
 
     if len(b.shape) == 1:
         b = b.unsqueeze(0)
 
     a_norm = torch.nn.functional.normalize(a, p=2, dim=1)
     b_norm = torch.nn.functional.normalize(b, p=2, dim=1)
+
     return torch.mm(a_norm, b_norm.transpose(0, 1))
 
 # ============================  
 def similaridadeCoseno(texto1, texto2):
     '''
     Similaridade do cosseno dos embeddgins dos textos.
     
     Parâmetros:
     `texto1` - Um texto a ser medido.           
-    `texto2` - Um texto a ser medido.                 
+    `texto2` - Um texto a ser medido.
+
+    Retorno:
+    A similaridade do cosseno entre os textos.
     '''
     
     similaridade = 1 - cosine(texto1, texto2)
     
     return similaridade
 
 # ============================  
@@ -66,14 +73,17 @@
     '''
     Distância euclidiana entre os embeddings dos textos.
     Possui outros nomes como distância L2 ou norma L2.
     
     Parâmetros:
     `texto1` - Um texto a ser medido.           
     `texto2` - Um texto a ser medido.
+
+    Retorno:
+    A distância euclidiana entre os textos.
     '''
     
     distancia = euclidean(texto1, texto2)
     
     return distancia
 
 # ============================  
@@ -81,12 +91,15 @@
     '''
     Distância Manhattan entre os embeddings das sentenças. 
     Possui outros nomes como distância Cityblock, distância L1, norma L1 e métrica do táxi.
     
     Parâmetros:
     `texto1` - Um texto a ser medido.           
     `texto2` - Um texto a ser medido.
+
+    Retorno:
+    A distância Manhattan entre os textos.
     '''
     
     distancia = cityblock(texto1, texto2)
 
     return distancia
```

### Comparing `texto_transformer-0.0.2/textotransformer/mensurador/mensurador.py` & `texto_transformer-0.0.3/textotransformer/mensurador/mensurador.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,33 +37,34 @@
         # Parâmetros do modelo
         self.model_args = modelo_args
     
         # Recupera o objeto do transformer.
         self.transformer = transformer
     
         # Recupera o modelo.
-        self.auto_model = transformer.get_auto_model()
+        self.auto_model = transformer.getAutoMmodel()
     
         # Recupera o tokenizador.     
-        self.tokenizer = transformer.get_tokenizer()
+        self.tokenizer = transformer.getTokenizer()
         
         # Recupera a classe PLN
         self.pln = pln
         
         logger.info("Classe Mensurador carregada: {}.".format(modelo_args))
 
     # ============================   
     def __repr__(self):
         '''
-        Retorna uma string com descrição do objeto
+        Retorna uma string com descrição do objeto.
         '''
-        return "Classe ({}) com modelo Transformer: {}, tokenizador: {} e NLP: {} ".format(self.__class__.__name__, 
-                                                                          self.auto_model.__class__.__name__,
-                                                                          self.tokenizer.__class__.__name__,
-                                                                          self.pln.__class__.__name__)
+        
+        return "Classe ({}) com  Transformer: {}, tokenizador: {} e NLP: {} ".format(self.__class__.__name__, 
+                                                                                     self.auto_model.__class__.__name__,
+                                                                                     self.tokenizer.__class__.__name__,
+                                                                                     self.pln.__class__.__name__)
 
     # ============================
     def getEmbeddingsTodasCamadas(self, texto):    
         '''   
         Retorna os embeddings de todas as camadas de um texto.
         
         Parâmetros:
```

### Comparing `texto_transformer-0.0.2/textotransformer/modelo/modeloarguments.py` & `texto_transformer-0.0.3/textotransformer/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.2/textotransformer/modelo/modeloenum.py` & `texto_transformer-0.0.3/textotransformer/modelo/modeloenum.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.2/textotransformer/modelo/transformer.py` & `texto_transformer-0.0.3/textotransformer/modelo/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
      :param modelo_args: Argumentos passados para o modelo Huggingface Transformers          
      :param cache_dir: Cache dir para Huggingface Transformers para armazenar/carregar modelos
      :param tokenizer_args: Argumentos (chave, pares de valor) passados para o modelo Huggingface Tokenizer
      :param tokenizer_name_or_path: Nome ou caminho do tokenizer. Quando None, model_name_or_path é usado
     
     '''
+
     def __init__(self, 
                 modelo_args : ModeloArgumentos,                
                 cache_dir: Optional[str] = None,
                 tokenizer_args: Dict = {}, 
                 tokenizer_name_or_path : str = None):
         
         # Inicializa o construtor da superclasse
@@ -75,28 +76,37 @@
             self.auto_model.config.tokenizer_class = self.tokenizer.__class__.__name__
             
         logger.info("Classe Transformer carregada: {}.".format(modelo_args))            
 
     # ============================   
     def __repr__(self):
         '''
-        Retorna uma string com descrição do objeto
+        Retorna uma string com descrição do objeto.
         '''
-        return "Classe ({}) com AutoConfig: {}, modelo Transformer: {} e tokenizador: {}.".format(self.__class__.__name__, 
+
+        return "Classe ({}) carregada com o modelo {}, m AutoConfig {}, Transformer {} e tokenizador: {}.".format(self.__class__.__name__, 
+                                                                                                             self.modelo_args.pretrained_model_name_or_path,
                                                                                                              self.config.__class__.__name__,
-                                                                                                             self.auto_model.__class__.__name__,
+                                                                                                             self.auto_model.__class__.__name__,                                                                                                             
                                                                                                              self.tokenizer.__class__.__name__)
 
     # ============================   
     def _load_model(self, 
                     model_name_or_path: str, 
-                    config, cache_dir):
+                    config, 
+                    cache_dir):
         '''
         Carrega o modelo transformer
+
+        Parâmetros:
+        `model_name_or_path` - Nome ou caminho do modelo.
+        `config` - Configuração do modelo.
+        `cache_dir` - Diretório de cache.
         '''
+
         # Carregamento T5
         if isinstance(config, T5Config):
             self._load_t5_model(model_name_or_path, 
                                 config, 
                                 cache_dir)
         
         else:
@@ -113,28 +123,40 @@
 
     # ============================   
     def _load_t5_model(self, model_name_or_path: str, 
                        config, 
                        cache_dir):
         '''
         Carrega codificador do modelo¨T5
+
+        Parâmetros:
+        `model_name_or_path` - Nome ou caminho do modelo.
+        `config` - Configuração do modelo.
+        `cache_dir` - Diretório de cache.
         '''
+
         from transformers import T5EncoderModel
         T5EncoderModel._keys_to_ignore_on_load_unexpected = ["decoder.*"]
         self.auto_model = T5EncoderModel.from_pretrained(model_name_or_path, 
                                                          config=config, 
                                                          cache_dir=cache_dir)
 
     # ============================   
     def _load_mt5_model(self, model_name_or_path: str, 
                         config, 
                         cache_dir):
         '''
         Carrega codificador do modelo MT5
+
+        Parâmetros:
+        `model_name_or_path` - Nome ou caminho do modelo.
+        `config` - Configuração do modelo.
+        `cache_dir` - Diretório de cache.
         '''
+
         from transformers import MT5EncoderModel
         MT5EncoderModel._keys_to_ignore_on_load_unexpected = ["decoder.*"]
         self.auto_model = MT5EncoderModel.from_pretrained(model_name_or_path, 
                                                           config=config, 
                                                           cache_dir=cache_dir)
    
     # ============================      
@@ -142,24 +164,24 @@
         '''
         Retorna um texto tokenizado e concatenado com tokens especiais '[CLS]' no início e o token '[SEP]' no fim para ser submetido ao modelo de linguagem.
         
         Parâmetros:
         `texto` - Um texto a ser tokenizado.
         
         Retorno:
-        `textoTokenizado` - Texto tokenizado.
+        `texto_tokenizado` - Texto tokenizado.
         '''
 
         # Adiciona os tokens especiais.
-        textoMarcado = '[CLS] ' + texto + ' [SEP]'
+        texto_marcado = '[CLS] ' + texto + ' [SEP]'
 
         # Tokeniza o texto
-        textoTokenizado = self.tokenizer.tokenize(textoMarcado)
+        texto_tokenizado = self.tokenizer.tokenize(texto_marcado)
 
-        return textoTokenizado
+        return texto_tokenizado
 
     # ============================    
 
     def tokenize(self, texto: Union[str, List[str]]):
         '''        
         Tokeniza um texto para submeter ao modelo de linguagem. 
         Retorna um dicionário listas de mesmo tamanho para garantir o processamento em lote.
@@ -171,14 +193,15 @@
         Retorna um dicionário com:
             tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
             input_ids uma lista com os ids dos tokens de entrada mapeados em seus índices do vocabuário.
             token_type_ids uma lista com os tipos dos tokens.
             attention_mask uma lista com os as máscaras de atenção indicando com '1' os tokens  pertencentes à sentença.
         '''
         
+        # Dicionário com a saída do tokenizador
         saida = {}
         
         # Se o texto for uma string coloca em uma lista de listas para tokenizar
         if isinstance(texto, str):
             to_tokenize = [[texto]]
         else:
             # Se for uma lista de strings coloca em uma lista para tokenizar
@@ -275,16 +298,15 @@
         saida = {}
         saida.update({'token_embeddings': last_hidden_state,  # Embeddings da última camada
                       'input_ids': texto['input_ids'],
                       'attention_mask': texto['attention_mask'],
                       'token_type_ids': texto['token_type_ids'],        
                       'tokens_texto_mcl': texto['tokens_texto_mcl'],
                       'texto_original': texto['texto_original']
-                      }
-                     )
+                      })
 
         # output_hidden_states == True existem embeddings nas camadas ocultas
         if self.auto_model.config.output_hidden_states:
             # 2 é o índice da saída com todos os embeddings em outputs
             all_layer_idx = 2
             if len(outputs) < 3: #Alguns modelos apenas geram last_hidden_states e all_hidden_states
                 all_layer_idx = 1
@@ -301,27 +323,45 @@
     
     # Dicionário de tokens de exceções e seus deslocamentos para considerar mais tokens do BERT em relação ao spaCy
     # A tokenização do BERT gera mais tokens que a tokenização das palavras do spaCy
     _dic_excecao_maior = {"":-1,
                          }
                              
     def _getExcecaoDicMaior(self, token: str):   
+        '''
+        Retorna o deslocamento do token no texto para considerar mais tokens do BERT em relação ao spaCy.
+
+        Parâmetros:
+        `token` - Um token a ser verificado se é uma exceção.
+
+        Retorno:
+        O deslocamento do token no texto para considerar mais tokens do BERT em relação ao spaCy.
+        '''
     
         valor = self._dic_excecao_maior.get(token)
         if valor != None:
             return valor
         else:
             return -1                             
     
     # Dicionário de tokens de exceções e seus deslocamentos para considerar menos tokens do BERT em relação ao spaCy
     # A tokenização do BERT gera menos tokens que a tokenização das palavras do spaCy
     _dic_excecao_menor = {"1°":1,
                           }
     
-    def _getExcecaoDicMenor(self, token: str):   
+    def _getExcecaoDicMenor(self, token: str): 
+        '''
+        Retorna o deslocamento do token no texto para considerar menos tokens do BERT em relação ao spaCy.
+
+        Parâmetros:
+        `token` - Um token a ser verificado se é uma exceção.
+
+        Retorno:
+        O deslocamento do token no texto para considerar menos tokens do BERT em relação ao spaCy.
+        '''  
         
         valor = self._dic_excecao_menor.get(token)
         if valor != None:
             return valor
         else:
             return -1
 
@@ -335,19 +375,23 @@
         Retorna 5 listas, os tokens(palavras), as postagging, tokens OOV, e os embeddings dos tokens igualando a quantidade de tokens do spaCy com a tokenização do MCL de acordo com a estratégia. 
         Utiliza duas estratégias para realizar o pooling de tokens que forma uma palavra.
             - Estratégia MEAN para calcular a média dos embeddings dos tokens que formam uma palavra.
             - Estratégia MAX para calcular o valor máximo dos embeddings dos tokens que formam uma palavra.
             
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings das palavras do modelo de linguagem
+        `embeddings_texto` - Os embeddings do texto gerados pelo método getEmbeddingsTexto
+        `tokens_texto_mcl` - Os tokens do texto gerados pelo método getEmbeddingsTexto
+        `tokens_texto_concatenado` - Os tokens do texto concatenado gerados pelo método getEmbeddingsTexto
+        `pln` - Uma instância da classe PLN para realizar a tokenização e POS-Tagging do texto.
     
         Retorna um dicionário com 5 lista:            
             lista_tokens  uma lista com os tokens do texto gerados pelo método.
             texto_pos_pln uma lista com as postagging dos tokens gerados pela ferramenta de pln.
-            lista_tokens_OOV_mcl uma lista com os tokens OOV do mcl.
+            lista_tokens_oov_mcl uma lista com os tokens OOV do mcl.
             lista_embeddings_MEAN uma lista com os embeddings com a estratégia MEAN.
             lista_embeddings_MAX uma lista com os embeddings com a estratégia MAX.
         '''
        
         #Guarda os tokens e embeddings de retorno
         lista_tokens = []
         lista_tokens_oov_mcl = []
@@ -539,43 +583,59 @@
         return saida
 
     # ============================   
     def getDimensaoEmbedding(self) -> int:
         '''
         Retorna a dimensão do embedding
         '''
+
         return self.auto_model.config.hidden_size        
         
     # ============================   
     def save(self, output_path: str):
         '''
         Salva o modelo.
+
+        Parâmetros:
+        `output_path` - caminho para salvar o modelo
+
         '''
+
         self.auto_model.save_pretrained(output_path)
         self.tokenizer.save_pretrained(output_path)
 
         with open(os.path.join(output_path, 'modelo_linguagem_config.json'), 'w') as fOut:
             json.dump(self.get_config_dict(), fOut, indent=2)
 
     # ============================   
-    def get_auto_model(self):
+    def getAutoMmodel(self):
         '''
         Recupera o modelo.
         '''
+
         return self.auto_model
 
     # ============================   
-    def get_tokenizer(self):
+    def getTokenizer(self):
         '''
         Recupera o tokenizador.
         '''
+
         return self.tokenizer
 
     # ============================   
-    def batch_to_device(self, lote, target_device: device):
+    def batchToDevice(self, lote, target_device: device):
         '''
         Envia lote pytorch batch para um dispositivo (CPU/GPU)
+
+        Parâmetros:
+         `lote` - lote pytorch
+         `target_device` - dispositivo de destino (CPU/GPU)
+        
+        Retorno:
+         lote enviado para o dispositivo        
         '''
+
         for key in lote:
             if isinstance(lote[key], Tensor):
                 lote[key] = lote[key].to(target_device)
         return lote
```

### Comparing `texto_transformer-0.0.2/textotransformer/pln/pln.py` & `texto_transformer-0.0.3/textotransformer/pln/pln.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Realiza o processamento de linguagem natural.
      
     Parâmetros:
     `modelo_args` - Parâmetros da classe PLN a ser carregado.    
     ''' 
 
     # Construtor da classe
-    def __init__(self, modelo_args):
+    def __init__(self, modelo_args):        
     
         # Parâmetros do modelo
         self.modelo_args = modelo_args
         
         #Instala a ferramenta pln spaCy
         InstaladorModelo(modelo_args=modelo_args)
         
@@ -36,24 +36,24 @@
         self.carrega()
             
         logger.info("Classe PLN carregada: {}.".format(modelo_args))    
             
     # ============================   
     def __repr__(self):
         '''
-        Retorna uma string com descrição do objeto
+        Retorna uma string com descrição do objeto.
         '''
-        return "Classe ({}) com modelo: {}".format(self.__class__.__name__,
-                                                   self.model_pln.__class__.__name__)            
+
+        return "Classe ({}) carregada com o modelo: {}".format(self.__class__.__name__,
+                                                               self.modelo_args.modelo_spacy)            
     
     # ============================    
     def carrega(self):
         '''
-        Realiza o carregamento da ferramenta de PLN.
-     
+        Realiza o carregamento da ferramenta de PLN.     
         '''
        
         # Carrega o modelo spacy            
         self.model_pln = spacy.load(self.modelo_args.modelo_spacy)    
         # Opção para remover funcionalidades
         #self.model_pln = spacy.load(self.modelo_args.modelo_spacy,disable=['tokenizer', 'lemmatizer', 'ner', 'parser', 'textcat', 'custom'])                
         logger.info("Modelo spaCy versão {} carregado!".format(self.modelo_args.modelo_spacy))    
@@ -63,15 +63,20 @@
     def getPOSTaggingUniversalTraduzido(postagging):
         '''
         Retorna a tradução das POS-Tagging.
         
         Tags de palavras universal https://universaldependencies.org/u/pos/
 
         Detalhes das tags em português: http://www.dbd.puc-rio.br/pergamum/tesesabertas/1412298_2016_completo.pdf
-        
+
+        Parâmetros:
+        `postagging` - Uma tag de uma palavra.
+
+        Retorno:
+        Uma string com a tradução da tag.        
         '''
     
         #dicionário que contêm pos tag universal e suas explicações
         postagging_universal_dict = {
           "X"    : "Outro",
           "VERB" : "Verbo ",
           "SYM"  : "Símbolo",
@@ -98,28 +103,33 @@
             traduzido = "NA" 
         return traduzido
     
     # ============================
     def getStopwords(self):
         '''
         Recupera as stop words do model_pln(Spacy).
-                
+
+        Retorno:
+        Uma lista com as stopwords.                
         '''
         
         spacy_stopwords = self.model_pln.Defaults.stop_words
         
         return spacy_stopwords 
 
     # ============================
     def removeStopWord(self, texto):
         '''
         Remove as stopwords de um texto.
         
         Parâmetros:
         `texto` - Um texto com stopwords.
+
+        Retorno:
+        Uma string com o texto sem as stopwords.
         '''
 
         # Recupera as stopwords
         stopwords = self.getStopwords()
 
         # Remoção das stop words do texto
         textoSemStopwords = [palavra for palavra in texto.split() if palavra.lower() not in stopwords]
@@ -157,16 +167,18 @@
        
     # ============================
     def getListaSentencasTexto(self, texto):
         '''
         Retorna uma lista com as sentenças de um texto. Utiliza o spacy para dividir o texto em sentenças.
         
         Parâmetros:
-        `texto` - Um texto a ser convertido em uma lista de sentenças.           
-                 
+        `texto` - Um texto a ser convertido em uma lista de sentenças.
+
+        Retorno:
+        `lista` - Lista com as sentenças do texto.
         '''
 
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
             doc = self.model_pln(texto)
         else:
@@ -187,32 +199,42 @@
         Retorna duas listas, uma com as sentenças de um texto e outra com a lista de lista de tokens de cada sentença.
         
         Parâmetros:
         `texto` - Um texto a ser processado em uma lista de sentenças e tokens.           
 
         Retorno:
         `lista_sentencas` - Lista com as sentenças do texto.
-        `lista_tokens` - Lista com os tokens de cada sentença do texto.
-                 
+        `lista_tokens` - Lista com os tokens de cada sentença do texto.                 
         '''
 
         # Retorna uma lista com as sentenlas do texto        
         lista_sentencas = self.getListaSentencasTexto(texto)
 
         # Lista para os tokens
         lista_tokens = []
         # Percorre as sentenças
         for sentenca in lista_sentencas:
             # Adiciona os tokens a lista
             lista_tokens.append(self.getListaTokensSentenca(sentenca))
+        
+        # @TODO: Verificar se é necessário retornar a lista de tokens. Converter para um dicionário?
 
         return lista_sentencas, lista_tokens
 
     # ============================
     def getVerbosTexto(self, texto):
+        '''
+        Retorna uma lista com os verbos de um texto.
+
+        Parâmetros:
+        `texto` - Um texto a ser processado em uma lista de sentenças e tokens.
+        
+        Retorno:
+        `lista_verbos` - Lista com os verbos do texto.
+        '''
         
         # (verbo normal como auxilar ou auxilar) + vários verbos auxiliares +verbo principal ou verbo auxiliar
         gramaticav1 =  [
                         {"POS": "AUX", "OP": "?", "DEP": {"IN": ["aux","aux:pass"]}},  #verbo auxiliar                                  
                         {"POS": "VERB", "OP": "?", "DEP": {"IN": ["ROOT","aux","xcomp","aux:pass"]}},  #verbo normal como auxiliar
                         {"POS": "AUX", "OP": "*", "DEP": {"IN": ["aux","xcomp","aux:pass"]}},  #verbo auxiliar   
                         {"POS": "VERB", "OP": "+"}, #verbo principal
@@ -267,15 +289,17 @@
     # ============================
     def getDicPOSQtde(self, texto):
         '''
         Retorna a quantidade de cada POS Tagging existentes em um texto.
         
         Parâmetros:
         `texto` - Um texto a ser convertido em uma lista de sentenças.           
-                 
+
+        Retorno:
+        Um dicionário com as POS-Tagging e suas quantidades.                 
         '''
         
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
             doc = self.model_pln(texto)
         else:
@@ -296,16 +320,19 @@
     # ============================
     def getDicTodasPOSQtde(self, texto):
         '''
         Retorna a quantidade de cada POS Tagging em um texto. Considera um conjunto fixo de POS-Tagging.
         
         Parâmetros:
         `texto` - Um texto a ser convertido em uma lista de sentenças.           
-                 
+
+        Retorno:
+        Um dicionário com as classes POS-Tagging e suas quantidades.                 
         '''
+
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
             doc = self.model_pln(texto)
         else:
             doc = texto
 
@@ -323,16 +350,18 @@
 
     # ============================
     def getDicTodasPOSListaQtde(self, lista):
         '''
         Retorna a quantidade de cada POS Tagging de uma lista. Considera um conjunto fixo de POS-Tagging.
         
         Parâmetros:
-        `lista` - Uma lista com as POS-Tagging.           
-                 
+        `lista` - Uma lista com as POS-Tagging.
+
+        Retorno:
+        Um dicionário com as POS-Tagging e suas quantidades.
         '''
 
         # Dicionário com as tags e quantidades
         conjunto = {"PRON":0, "VERB":0, "PUNCT":0, "DET":0, "NOUN":0, "AUX":0, "CCONJ":0, "ADP":0, "PROPN":0, "ADJ":0, "ADV":0, "NUM":0, "SCONJ":0, "SYM":0, "SPACE":0, "INTJ": 0}
 
         for x in lista:
             valor = conjunto.get(x)
@@ -346,15 +375,17 @@
     # ============================
     def getTokensTexto(self, texto):
         '''
         Retorna a lista de tokens do texto.
         
         Parâmetros:
         `texto` - Um texto a ser recuperado os tokens.
-                 
+
+        Retorno:
+        Uma lista com os tokens do texto.                 
         '''
 
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
             doc = self.model_pln(texto)
         else:
@@ -373,14 +404,16 @@
     def getPOSTokensTexto(self, texto):
         '''
         Retorna a lista das POS-Tagging dos tokens do texto.
         
         Parâmetros:
         `texto` - Um texto a ser recuperado as POS-Tagging.
                  
+        Retorno:
+        Uma lista com as POS-Tagging dos tokens do texto.
         '''
 
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
             doc = self.model_pln(texto)
         else:
@@ -398,16 +431,19 @@
     # ============================
     def getListaTokensPOSTexto(self, texto):
         '''
         Retorna duas listas uma com os tokens e a outra com a POS-Tagging dos tokens do texto.
         
         Parâmetros:
         `texto` - Um texto a ser recuperado as listas de tokens e POS-Tagging.
-                 
+
+        Retorno:
+        Duas listas com os tokens e a POS-Tagging do texto.                 
         '''
+
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
             doc = self.model_pln(texto)
         else:
             doc = texto
 
@@ -424,17 +460,20 @@
 
     # ============================   
     def getTextoSemStopWord(self, listaTokens):
         '''
         Retorna uma lista com tokens de um texto excluindo as stopwords.
         
         Parâmetros:
-        `listaTokens` - Uma lista com os tokens de um texto.
-                 
+        `listaTokens` - Uma lista com os tokens de um texto.    
+
+        Retorno:
+        Uma lista com os tokens sem as stopwords.             
         '''
+
         # Recupera as stopwords do modelo
         stopwords = self.getStopwords()
         
         # Lista dos tokens
         lista = []
 
         # Percorre os tokens do texto
@@ -444,14 +483,14 @@
             if token.lower() not in stopwords:
                 lista.append(token)
 
         # Retorna a lista de tokens sem as stopwords
         return lista
 
     # ============================   
-    def get_model_pln(self):
+    def getModelPln(self):
         '''
         Recupera o modelo de PLN.
         '''
+
         return self.model_pln
-        
-   
+
```

### Comparing `texto_transformer-0.0.2/textotransformer/util/utilambiente.py` & `texto_transformer-0.0.3/textotransformer/util/utilambiente.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,31 +12,37 @@
 class InstaladorModelo:
     ''' 
     Realiza a instalação do modelo spaCy.
      
     Parâmetros:
     `modelo_args` - Um objeto com os parâmetros do modelo.
     ''' 
+    
     def __init__(self, modelo_args: ModeloArgumentos):
         #Atualiza os parâmetros
         self.modelo_args = modelo_args
         
         # Executa o processo de atualização e instalação do spaCy
         self.install_model_spacy()
 
     # ============================
     def __repr__(self):
         '''
         Retorna uma string com descrição do objeto
         '''
+
         return "Classe ({}) de instalação do modelo {}.".format(self.__class__.__name__, 
                                                        self.modelo_args.modelo_spacy.__class__.__name__)
 
     # ============================
     def install_model_spacy(self):
+        '''
+        Realiza a instalação do modelo spaCy.
+        '''
+
         try:
             # Download do modelo de linguagem na linguagem solicitada
             subprocess.run(["python", "-m", "spacy", "download", self.modelo_args.modelo_spacy])
             logger.info("Download do modelo spaCy {} realizado!".format(self.modelo_args.modelo_spacy))    
         except subprocess.CalledProcessError as e:
             logger.info("Falha em instalar modelo spaCy {}. Erro: {}.".format(self.modelo_args.modelo_spacy, e))
```

### Comparing `texto_transformer-0.0.2/textotransformer/util/utilarquivo.py` & `texto_transformer-0.0.3/textotransformer/util/utilarquivo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.2/textotransformer/util/utilconstantes.py` & `texto_transformer-0.0.3/textotransformer/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.2/textotransformer/util/utiltempo.py` & `texto_transformer-0.0.3/textotransformer/util/utiltempo.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,31 +10,52 @@
  
 logger = logging.getLogger(__name__)
  
 # ============================    
 def formataTempo(tempo):
     '''
     Pega a tempo em segundos e retorna uma string hh:mm:ss
+
+    Parâmetros:
+    'tempo' - Tempo em segundos.
+
+    Retorno:
+    Uma string no formato hh:mm:ss
     '''
         
     # Arredonda para o segundo mais próximo.
     tempoArredondado = int(round((tempo)))
    
     # Formata como hh:mm:ss
     return str(datetime.timedelta(seconds=tempoArredondado))  
 
 # ============================      
 def mediaAngulo(deg):
+    '''
+    Calcula a média de uma lista de ângulos em graus.
+
+    Parâmetros:
+    'deg' - Uma lista de ângulos em graus.
+
+    Retorno:
+    Um ângulo em graus.
+    '''
     
     return degrees(phase(sum(rect(1, radians(d)) for d in deg) / len(deg)))
  
 # ============================  
 def mediaTempo(tempos):
     '''
     Calcula a média de uma lista de tempo string no formato hh:mm:ss
+
+    Parâmetros:
+    'tempos' - Uma lista de tempo string no formato hh:mm:ss
+
+    Retorno:
+    Uma string no formato hh:mm:ss
     '''
     
     t = (tempo.split(':') for tempo in tempos)
     # Converte para segundos
     segundos = ((float(s) + int(m) * 60 + int(h) * 3600) for h, m, s in t)
     # Verifica se deu algum dia
     dia = 24 * 60 * 60
@@ -52,14 +73,20 @@
     
     return '{:02d}:{:02d}:{:02d}'.format(int(h), int(m), int(s))    
 
 # ============================    
 def somaTempo(tempos):
     '''
     Calcula a soma de uma lista de tempo string no formato hh:mm:ss
+
+    Parâmetros:
+    'tempos' - Uma lista de tempo string no formato hh:mm:ss
+
+    Retorno:
+    Uma string no formato hh:mm:ss
     '''
     
     t = (tempo.split(':') for tempo in tempos)
     # Converte para segundos
     segundos = ((float(s) + int(m) * 60 + int(h) * 3600) for h, m, s in t)
     # Soma os segundos
     soma_segundos = sum([s * 1. for s in segundos])
```

### Comparing `texto_transformer-0.0.2/textotransformer/util/utiltexto.py` & `texto_transformer-0.0.3/textotransformer/util/utiltexto.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.2/LICENSE` & `texto_transformer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.2/README.md` & `texto_transformer-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,54 +27,57 @@
 from textotransformer import TextoTransformer
 
 # Instância uma objeto e baixa o modelo de linguagem
 modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
 
 # Alguns textos a serem codificados
 textos = ["Bom Dia, professor.",
-      "Qual o conteúdo da prova?",
-      "Vai cair tudo na prova?",
-      "Aguardo uma resposta, João."]
+          "Qual o conteúdo da prova?",
+          "Vai cair tudo na prova?",
+          "Aguardo uma resposta, João."]
 
 # Recupera os embeddings consolidados dos textos
 embeddings_texto = modelo.getEmbeddingTexto(textos)      
 
 # Mostra os textos e seus embeddings
-for texto, embedding in zip(texto, embeddings_texto):
+for texto, embedding in zip(textos, embeddings_texto):
     print("Texto:", texto)
     print("Embedding:", embedding)
     print("")
 
+#Resultado
 #Texto: Bom Dia, professor.
 #Embedding: tensor([ 1.3736e-01,  6.1996e-02,  3.2554e-01, -3.1146e-02,  3.5892e-01,...
 #Texto: Qual o conteúdo da prova?
 #Embedding: tensor([ 8.3348e-02, -1.8269e-01,  5.9241e-01, -9.5235e-02,  5.0978e-01,...
 #Texto: Vai cair tudo na prova?
 #Embedding: tensor([ 1.3447e-01,  1.1854e-01,  6.0201e-02,  1.0271e-01,  2.6321e-01,...
 #Texto: Aguardo uma resposta, João.
 #Embedding: tensor([ 3.7160e-02, -7.3645e-02,  3.3942e-01,  8.0847e-02,  3.8259e-01,...
 ````
 
+O exemplo pode ser executado no notebook do GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).
+
 ## Métodos principais:
 
 Métodos principais para recuperar embeddings de textos, sentenças, palavras e tokens. Os embeddings de textos, sentenças e palavras podem ser consolidados pelas estratégias de pooling média (MEAN) e máximo (MAX) dos embeddings de seus tokens.
 
-- `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling)`
+- `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling: int)`
     - Retorna uma lista dos embeddings consolidados dos textos.
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
         - `estrategia_pooling`: Especifica a estratégia de pooling dos tokens do texto. Valores possívels 0 - MEAN ou 1 - MAX. Valor default 0(MEAN).
 
-- `getEmbeddingSentenca(texto: Union[str, List[str]], estrategia_pooling)` 
+- `getEmbeddingSentenca(texto: Union[str, List[str]], estrategia_pooling: int)` 
     - Retorna uma lista dos embeddings consolidados das sentenças dos textos.    
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
         - `estrategia_pooling`: Especifica a estratégia de pooling dos tokens do texto. Valores possívels 0 - MEAN ou 1 - MAX. Valor default 0(MEAN).
 
-- `getEmbeddingPalavra(texto: Union[str, List[str]], estrategia_pooling)` 
+- `getEmbeddingPalavra(texto: Union[str, List[str]], estrategia_pooling: int)` 
     - Retorna uma lista dos embeddings consolidados das palavras dos textos.
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
         - `estrategia_pooling`: Especifica a estratégia de pooling dos tokens do texto. Valores possívels 0 - MEAN ou 1 - MAX. Valor default 0(MEAN).
 
 - `getEmbeddingToken(texto: Union[str, List[str]])` 
     - Retorna uma lista dos embeddings dos tokens dos textos.
```

### Comparing `texto_transformer-0.0.2/pyproject.toml` & `texto_transformer-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "texto-transformer"
-version = "0.0.2"
+version = "0.0.3"
 description = "Texto Transformer: Framework para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer"
 readme = "README.md"
 requires-python = ">=3.6.0"
 license = { file = "LICENSE" }
 
 authors = [
     { name = "Osmar de Oliveira Braz Junior", email = "osmar.braz@udesc.br" }
```

### Comparing `texto_transformer-0.0.2/PKG-INFO` & `texto_transformer-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texto-transformer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Texto Transformer: Framework para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer
 Project-URL: repository, https://github.com/osmarbraz/textotransformer/
 Author-email: Osmar de Oliveira Braz Junior <osmar.braz@udesc.br>
 License: MIT License
         
         Copyright (c) 2023 Osmar de Oliveira Braz Junior
         
@@ -67,54 +67,57 @@
 from textotransformer import TextoTransformer
 
 # Instância uma objeto e baixa o modelo de linguagem
 modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
 
 # Alguns textos a serem codificados
 textos = ["Bom Dia, professor.",
-      "Qual o conteúdo da prova?",
-      "Vai cair tudo na prova?",
-      "Aguardo uma resposta, João."]
+          "Qual o conteúdo da prova?",
+          "Vai cair tudo na prova?",
+          "Aguardo uma resposta, João."]
 
 # Recupera os embeddings consolidados dos textos
 embeddings_texto = modelo.getEmbeddingTexto(textos)      
 
 # Mostra os textos e seus embeddings
-for texto, embedding in zip(texto, embeddings_texto):
+for texto, embedding in zip(textos, embeddings_texto):
     print("Texto:", texto)
     print("Embedding:", embedding)
     print("")
 
+#Resultado
 #Texto: Bom Dia, professor.
 #Embedding: tensor([ 1.3736e-01,  6.1996e-02,  3.2554e-01, -3.1146e-02,  3.5892e-01,...
 #Texto: Qual o conteúdo da prova?
 #Embedding: tensor([ 8.3348e-02, -1.8269e-01,  5.9241e-01, -9.5235e-02,  5.0978e-01,...
 #Texto: Vai cair tudo na prova?
 #Embedding: tensor([ 1.3447e-01,  1.1854e-01,  6.0201e-02,  1.0271e-01,  2.6321e-01,...
 #Texto: Aguardo uma resposta, João.
 #Embedding: tensor([ 3.7160e-02, -7.3645e-02,  3.3942e-01,  8.0847e-02,  3.8259e-01,...
 ````
 
+O exemplo pode ser executado no notebook do GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).
+
 ## Métodos principais:
 
 Métodos principais para recuperar embeddings de textos, sentenças, palavras e tokens. Os embeddings de textos, sentenças e palavras podem ser consolidados pelas estratégias de pooling média (MEAN) e máximo (MAX) dos embeddings de seus tokens.
 
-- `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling)`
+- `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling: int)`
     - Retorna uma lista dos embeddings consolidados dos textos.
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
         - `estrategia_pooling`: Especifica a estratégia de pooling dos tokens do texto. Valores possívels 0 - MEAN ou 1 - MAX. Valor default 0(MEAN).
 
-- `getEmbeddingSentenca(texto: Union[str, List[str]], estrategia_pooling)` 
+- `getEmbeddingSentenca(texto: Union[str, List[str]], estrategia_pooling: int)` 
     - Retorna uma lista dos embeddings consolidados das sentenças dos textos.    
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
         - `estrategia_pooling`: Especifica a estratégia de pooling dos tokens do texto. Valores possívels 0 - MEAN ou 1 - MAX. Valor default 0(MEAN).
 
-- `getEmbeddingPalavra(texto: Union[str, List[str]], estrategia_pooling)` 
+- `getEmbeddingPalavra(texto: Union[str, List[str]], estrategia_pooling: int)` 
     - Retorna uma lista dos embeddings consolidados das palavras dos textos.
     - Parâmetros:
         - `texto`: Um texto ou uma lista de textos para obter os embeddings.
         - `estrategia_pooling`: Especifica a estratégia de pooling dos tokens do texto. Valores possívels 0 - MEAN ou 1 - MAX. Valor default 0(MEAN).
 
 - `getEmbeddingToken(texto: Union[str, List[str]])` 
     - Retorna uma lista dos embeddings dos tokens dos textos.
```

