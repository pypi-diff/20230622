# Comparing `tmp/texto_transformer-0.0.3.tar.gz` & `tmp/texto_transformer-0.0.4.tar.gz`

## Comparing `texto_transformer-0.0.3.tar` & `texto_transformer-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/requirements.txt
--rw-r--r--   0        0        0    69971 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/notebooks/ExemplosTextoTransformer.ipynb
--rw-r--r--   0        0        0   529102 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/notebooks/TestesTextoTransformer.ipynb
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/__init__.py
--rw-r--r--   0        0        0    53070 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/textotransformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/__init__.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/medidas.py
--rw-r--r--   0        0        0    37674 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/mensurador.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/mensurador/mensuradorenum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/modeloarguments.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/modeloenum.py
--rw-r--r--   0        0        0    31461 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/modelo/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/pln/__init__.py
--rw-r--r--   0        0        0    16667 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/pln/pln.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/__init__.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utilambiente.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utilarquivo.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utilconstantes.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utiltempo.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/textotransformer/util/utiltexto.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/LICENSE
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/README.md
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 texto_transformer-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/requirements.txt
+-rw-r--r--   0        0        0   113310 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/notebooks/ExemplosTextoTransformer.ipynb
+-rw-r--r--   0        0        0   433470 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/notebooks/TestesTextoTransformer.ipynb
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/__init__.py
+-rw-r--r--   0        0        0    52950 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/textotransformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/mensurador/__init__.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/mensurador/medidas.py
+-rw-r--r--   0        0        0    37803 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/mensurador/mensurador.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/mensurador/mensuradorenum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/modelo/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/modelo/modeloarguments.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/modelo/modeloenum.py
+-rw-r--r--   0        0        0    31479 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/modelo/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/pln/__init__.py
+-rw-r--r--   0        0        0    16667 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/pln/pln.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/util/__init__.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/util/utilambiente.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/util/utilarquivo.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/util/utilconstantes.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/util/utiltempo.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/textotransformer/util/utiltexto.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/README.md
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 texto_transformer-0.0.4/PKG-INFO
```

### Comparing `texto_transformer-0.0.3/textotransformer/textotransformer.py` & `texto_transformer-0.0.4/textotransformer/textotransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,30 +288,31 @@
         Tokeniza um texto para submeter ao modelo de linguagem. 
         Retorna um dicionário listas de mesmo tamanho para garantir o processamento em lote.
         Use a quantidade de tokens para saber até onde deve ser recuperado em uma lista de saída.
         Ou use attention_mask diferente de 1 para saber que posições devem ser utilizadas na lista.
 
         Facilita acesso a classe Transformer.    
 
-        :param texto: Texto a ser tokenizado para o modelo de linguagem.
+        Parâmetros:
+        `texto` - Texto a ser tokenizado para o modelo de linguagem.
          
         Retorna um dicionário com:
             tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
             input_ids uma lista com os ids dos tokens de entrada mapeados em seus índices do vocabuário.
             token_type_ids uma lista com os tipos dos tokens.
             attention_mask uma lista com os as máscaras de atenção indicando com '1' os tokens  pertencentes à sentença.
         '''
         return self.getTransformer().tokenize(texto)
     
     # ============================
     def getCodificacaoCompleta(self, texto: Union[str, List[str]],
-                    tamanho_lote: int = 32, 
-                    mostra_barra_progresso: bool = False,                     
-                    convert_to_numpy: bool = False,         
-                    device: str = None):
+                               tamanho_lote: int = 32, 
+                               mostra_barra_progresso: bool = False,
+                               convert_to_numpy: bool = False,
+                               device: str = None):
 
         '''
         Retorna um dicionário com as informações completas da codificação do texto utilizando o modelo de linguagem.
     
         Parâmetros:
          `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
          `tamanho_lote` - o tamanho do lote usado para o computação
@@ -530,14 +531,15 @@
             input_ids uma lista com os textos indexados.            
             attention_mask uma lista com os as máscaras de atenção
             token_type_ids uma lista com os tipos dos tokens.            
             tokens_texto uma lista com os textos tokenizados com os tokens especiais.
             texto_original uma lista com os textos originais.
             all_layer_embeddings uma lista com os embeddings de todas as camadas.
         '''
+        
         return self.getTransformer().getSaidaRede(texto)
 
    # ============================
     def getEmbeddingTexto(self, texto: Union[str, List[str]], 
                           estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN):
         '''
         Recebe um texto (string ou uma lista de strings) e retorna os embeddings consolidados dos tokens do texto utilizando estratégia pooling especificada(MEAN, MAX).
@@ -569,18 +571,18 @@
                 return self.getCodificacaoTexto(texto)['texto_embeddings_MAX']
             else:              
                 logger.info("Não foi especificado uma estratégia de pooling válida.") 
                 return None  
 
     # ============================
     def getCodificacaoTexto(self, texto: Union[str, List[str]],
-                             tamanho_lote: int = 32, 
-                             mostra_barra_progresso: bool = False,                     
-                             convert_to_numpy: bool = False,         
-                             device: str = None):
+                            tamanho_lote: int = 32, 
+                            mostra_barra_progresso: bool = False,                     
+                            convert_to_numpy: bool = False,         
+                            device: str = None):
         '''        
         De um texto preparado(tokenizado) ou não, retorna a codificação dos textos consolidados dos tokens do textos utilizando estratégia pooling MEAN e MAX.
     
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings dos textos consolidados dos tokens com a estratégia MEAN e MAX utilizando o modelo de linguagem
     
         Retorno:
@@ -609,19 +611,19 @@
                       #'all_layer_embeddings': []
                      }
         )
 
         # Percorre os textos da lista.
         for i, texto in enumerate(texto_embeddings['texto_original']):       
 
-            # Recupera os embeddings do texto  
-            embeddings_texto = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]            
+            # Recupera a lista de embeddings gerados pelo MCL sem CLS e SEP 
+            embeddings_texto = texto_embeddings['token_embeddings'][i][1:-1]
            
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
-            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]            
+            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]
             
             # Calcula a média dos embeddings dos tokens das sentenças do texto
             embedding_documento_media = torch.mean(embeddings_texto, dim=0)
 
             # Calcula a média dos embeddings dos tokens das sentenças do texto
             embedding_documento_maximo, linha = torch.max(embeddings_texto, dim=0)
             
@@ -704,30 +706,30 @@
                                                tamanho_lote,
                                                mostra_barra_progresso,
                                                convert_to_numpy,
                                                device)
 
         # Acumula a saída do método
         saida = {}
-        saida.update({'texto_original' : [],            # Lista com os textos originais
-                      'tokens_texto_mcl' : [],          # Lista com os tokens dos textos originais
-                      'sentencas_texto' : [],           # Lista com as sentenças do texto
+        saida.update({'texto_original' : [],               # Lista com os textos originais
+                      'tokens_texto_mcl' : [],             # Lista com os tokens dos textos originais
+                      'sentencas_texto' : [],              # Lista com as sentenças do texto
                       'sentenca_embeddings_MEAN': [],      # Lista de lista média dos embeddings dos tokens que da sentença.
                       'sentenca_embeddings_MAX': [],       # Lista de lista máximo dos embeddings dos tokens que da sentença.
                      }
         )
 
         # Percorre os textos da lista.
         for i, texto in enumerate(texto_embeddings['texto_original']):       
 
-            # Recupera os embeddings do texto  
-            embeddings_texto = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]            
+            # Recupera a lista de embeddings gerados pelo MCL sem CLS e SEP 
+            embeddings_texto = texto_embeddings['token_embeddings'][i][1:-1]
 
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
-            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]            
+            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]
                         
             # Recupera as sentenças do texto
             lista_sentencas_texto = self.getPln().getListaSentencasTexto(texto_embeddings['texto_original'][i])
 
             # Lista de embeddings das sentenças do texto    
             lista_embeddings_tokens_sentencas_texto_media = []
             lista_embeddings_tokens_sentencas_texto_maximo = []
@@ -737,15 +739,15 @@
 
                 # Tokeniza a sentença
                 sentenca_tokenizada =  self.transformer.getTextoTokenizado(sentenca)
                 
                 # Remove os tokens de início e fim da sentença
                 sentenca_tokenizada.remove('[CLS]')
                 sentenca_tokenizada.remove('[SEP]')    
-                #print(len(sentencaTokenizada))
+                #print(len(sentenca_tokenizada))
 
                 # Localiza os índices dos tokens da sentença no texto
                 inicio, fim = encontrarIndiceSubLista(tokens_texto_mcl, sentenca_tokenizada)
 
                 # Recupera os embeddings dos tokens da sentença a partir dos embeddings do texto
                 embedding_sentenca = embeddings_texto[inicio:fim + 1]
 
@@ -755,22 +757,22 @@
                 # Calcula a média dos embeddings dos tokens das sentenças do texto
                 embedding_sentenca_maximo, linha = torch.max(embedding_sentenca, dim=0)
 
                 # Guarda os tokens e os embeddings das sentenças do texto da média e do máximo
                 lista_embeddings_tokens_sentencas_texto_media.append(embedding_sentenca_media)
                 lista_embeddings_tokens_sentencas_texto_maximo.append(embedding_sentenca_maximo)
             
-            #Acumula a saída do método             
+            # Acumula a saída do método             
             saida['texto_original'].append(texto_embeddings['texto_original'][i])
             saida['tokens_texto_mcl'].append(tokens_texto_mcl)
             saida['sentencas_texto'].append(lista_sentencas_texto)
             saida['sentenca_embeddings_MEAN'].append(lista_embeddings_tokens_sentencas_texto_media)
             saida['sentenca_embeddings_MAX'].append(lista_embeddings_tokens_sentencas_texto_maximo)
 
-        #Se é uma string uma lista com comprimento 1
+        # Se é uma string uma lista com comprimento 1
         if entrada_eh_string:
           saida['texto_original'] = saida['texto_original'][0]
           saida['tokens_texto_mcl'] =  saida['tokens_texto_mcl'][0]
           saida['sentencas_texto'] = saida['sentencas_texto'][0]
           saida['sentenca_embeddings_MEAN'] = saida['sentenca_embeddings_MEAN'][0]
           saida['sentenca_embeddings_MAX'] = saida['sentenca_embeddings_MAX'][0]
 
@@ -843,18 +845,18 @@
         entrada_eh_string = False
         if isinstance(texto, str) or not hasattr(texto, '__len__'):             
             texto = [texto]
             entrada_eh_string = True
 
         # Recupera os embeddings do texto
         texto_embeddings = self.getCodificacaoCompleta(texto,
-                                               tamanho_lote,
-                                               mostra_barra_progresso,
-                                               convert_to_numpy,
-                                               device)
+                                                       tamanho_lote,
+                                                       mostra_barra_progresso,
+                                                       convert_to_numpy,
+                                                       device)
         
         # Acumula a saída do método
         saida = {}
         saida.update({'texto_original' : [],
                       'tokens_texto': [], 
                       'tokens_texto_mcl' : [],
                       'tokens_oov_texto_mcl': [],                      
@@ -867,40 +869,40 @@
 
         # Percorre os textos da lista.
         for i, texto in enumerate(texto_embeddings['texto_original']):
             
             # Recupera o texto tokenizado pela ferramenta de pln do texto original
             lista_tokens_texto_pln = self.getPln().getTokensTexto(texto_embeddings['texto_original'][i])
             
-            # Recupera os embeddings do texto  
-            embeddings_texto = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]            
+            # Recupera a lista de embeddings gerados pelo MCL sem CLS e SEP 
+            embeddings_texto = texto_embeddings['token_embeddings'][i][1:-1]
             
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
-            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]        
+            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]
             
             # Concatena os tokens gerandos pela ferramenta de pln
             tokens_texto_concatenado = " ".join(lista_tokens_texto_pln)
 
             # Recupera os embeddings e tokens de palavra            
             saidaEmbeddingPalavra = self.getTransformer().getTokensEmbeddingsPOSTexto(embeddings_texto,
-                                                                                       tokens_texto_mcl,
-                                                                                       tokens_texto_concatenado,
-                                                                                       self.getPln())
+                                                                                      tokens_texto_mcl,
+                                                                                      tokens_texto_concatenado,
+                                                                                      self.getPln())
 
-            #Acumula a saída do método 
+            # Acumula a saída do método 
             saida['texto_original'].append(texto_embeddings['texto_original'][i])
             saida['tokens_texto'].append(saidaEmbeddingPalavra['tokens_texto'])
             saida['tokens_texto_mcl'].append(tokens_texto_mcl)
             saida['tokens_oov_texto_mcl'].append(saidaEmbeddingPalavra['tokens_oov_texto_mcl'])            
             saida['tokens_texto_pln'].append(lista_tokens_texto_pln)
             saida['pos_texto_pln'].append(saidaEmbeddingPalavra['pos_texto_pln'])            
             saida['embeddings_MEAN'].append(saidaEmbeddingPalavra['embeddings_MEAN'])
             saida['embeddings_MAX'].append(saidaEmbeddingPalavra['embeddings_MAX'])
         
-        #Se é uma string uma lista com comprimento 1
+         # Se é uma string uma lista com comprimento 1
         if entrada_eh_string:
             saida['texto_original'] = saida['texto_original'][0]
             saida['tokens_texto'] = saida['tokens_texto'][0]
             saida['tokens_texto_mcl'] = saida['tokens_texto_mcl'][0]
             saida['tokens_oov_texto_mcl'] = saida['tokens_oov_texto_mcl'][0]
             saida['tokens_texto_pln'] = saida['tokens_texto_pln'][0]
             saida['pos_texto_pln'] = saida['pos_texto_pln'][0]
@@ -940,43 +942,42 @@
         # Se o texto é uma string, coloca em uma lista de comprimento 1
         entrada_eh_string = False
         if isinstance(texto, str) or not hasattr(texto, '__len__'):             
             texto = [texto]
             entrada_eh_string = True
 
         # Recupera os embeddings do texto
-        #texto_embeddings = self.getEmbeddings(texto)
-          
         texto_embeddings = self.getCodificacaoCompleta(texto,
-                                               tamanho_lote,
-                                               mostra_barra_progresso,
-                                               convert_to_numpy,
-                                               device)
+                                                       tamanho_lote,
+                                                       mostra_barra_progresso,
+                                                       convert_to_numpy,
+                                                       device)
         
         # Acumula a saída do método
         saida = {}
         saida.update({'texto_original' : [],
                       'tokens_texto_mcl' : [],                      
                       'token_embeddings': [],        
                       #'all_layer_embeddings': []
                      }
         )
 
         # Percorre os textos da lista.
-        for i, texto in enumerate(texto_embeddings['texto_original']):            
-            # Recupera os embeddings do texto  
-            lista_token_embeddings = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]
+        for i, texto in enumerate(texto_embeddings['texto_original']):    
+
+            # Recupera a lista de embeddings gerados pelo MCL sem CLS e SEP 
+            lista_token_embeddings = texto_embeddings['token_embeddings'][i][1:-1]
 
             # Recupera os embeddings do texto  
-            #lista_all_layer_embeddings = texto_embeddings['all_layer_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]
+            #lista_all_layer_embeddings = texto_embeddings['all_layer_embeddings'][i][1:-1]
             
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
             tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]
 
-            #Acumula a saída do método 
+            # Acumula a saída do método 
             #Se é uma string uma lista com comprimento 1
             if entrada_eh_string:
                 saida['texto_original'] = texto_embeddings['texto_original'][i]
                 saida['tokens_texto_mcl'] = tokens_texto_mcl
                 saida['token_embeddings'] = lista_token_embeddings
             else:
                 saida['texto_original'].append(texto_embeddings['texto_original'][i])
@@ -994,14 +995,15 @@
 
         Parâmetros:
         `texto` - Um texto a ser recuperado o tamanho.
 
         Retorno:
           Um inteiro com tamanho do texto.
         '''
+
         if isinstance(texto, dict):              # caso seja um dic de listas
             return len(next(iter(texto.values())))
         else:
             if not hasattr(texto, '__len__'):      # Objeto não tem o len()
                 return 1
             else:
                 if len(texto) == 0 or isinstance(texto[0], int):  #String vazia ou lista de ints
```

### Comparing `texto_transformer-0.0.3/textotransformer/mensurador/medidas.py` & `texto_transformer-0.0.4/textotransformer/mensurador/medidas.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/mensurador/mensurador.py` & `texto_transformer-0.0.4/textotransformer/mensurador/mensurador.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,26 +127,29 @@
             # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         return texto_tokenizado, input_ids, attention_mask, token_type_ids, outputs
 
     # ============================
     # Cria um buffer com os embeddings de sentenças para economizar memória no processamento.
     buffer_embeddings = {}
     
-    def getEmbeddingsTodasCamadasBuffer(self, S):
+    def getEmbeddingsTodasCamadasBuffer(self, embedding):
         '''
-        Retorna os embeddings de uma sentença de um buffer ou do modelo..
+        Retorna os embeddings de uma sentença de um buffer ou do modelo.
+
+        Parâmetros:
+        `embedding` - Uma sentença a ser recuperado os embeddings.
         '''
         
         # Se está no dicionário retorna o embedding
-        if S in self.buffer_embeddings:
-            return self.buffer_embeddings.get(S)
+        if embedding in self.buffer_embeddings:
+            return self.buffer_embeddings.get(embedding)
         else:
             # Gera o embedding
-            total_camada = self.getEmbeddingsTodasCamadas(S)
-            self.buffer_embeddings.update({S: total_camada})
+            total_camada = self.getEmbeddingsTodasCamadas(embedding)
+            self.buffer_embeddings.update({embedding: total_camada})
             return total_camada
 
     # ============================
     def limpaBufferEmbedding(self):
         '''
         Esvazia o buffer de embeddings das sentenças.
         '''
```

### Comparing `texto_transformer-0.0.3/textotransformer/modelo/modeloarguments.py` & `texto_transformer-0.0.4/textotransformer/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/modelo/modeloenum.py` & `texto_transformer-0.0.4/textotransformer/modelo/modeloenum.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/modelo/transformer.py` & `texto_transformer-0.0.4/textotransformer/modelo/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,18 @@
 logger = logging.getLogger(__name__)
 
 class Transformer(nn.Module):
     '''
     Classe que encapsula a classe AutoModel da Huggingface para gerar embeddings de token, palavra, sentença ou texto.
     Carrega a classe correta, por exemplo BERT / RoBERTa etc.
 
-     :param modelo_args: Argumentos passados para o modelo Huggingface Transformers          
-     :param cache_dir: Cache dir para Huggingface Transformers para armazenar/carregar modelos
-     :param tokenizer_args: Argumentos (chave, pares de valor) passados para o modelo Huggingface Tokenizer
-     :param tokenizer_name_or_path: Nome ou caminho do tokenizer. Quando None, model_name_or_path é usado
-    
+     `modelo_args' - Argumentos passados para o modelo Huggingface Transformers          
+     'cache_dir' - Cache dir para Huggingface Transformers para armazenar/carregar modelos
+     'tokenizer_args' - Argumentos (chave, pares de valor) passados para o modelo Huggingface Tokenizer
+     'tokenizer_name_or_path' - Nome ou caminho do tokenizer. Quando None, model_name_or_path é usado    
     '''
 
     def __init__(self, 
                 modelo_args : ModeloArgumentos,                
                 cache_dir: Optional[str] = None,
                 tokenizer_args: Dict = {}, 
                 tokenizer_name_or_path : str = None):
@@ -61,15 +60,15 @@
         self._load_model(model_name_or_path, 
                          self.config, 
                          cache_dir)
 
         # Carrega o tokenizador
         self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name_or_path if tokenizer_name_or_path is not None else  model_name_or_path, cache_dir=cache_dir, **tokenizer_args)
 
-        #Se max_seq_length não foi especificado, tenta inferir do modelo
+        # Se max_seq_length não foi especificado, tenta inferir do modelo
         if self.modelo_args.max_seq_len is None:
             if hasattr(self.auto_model, "config") and hasattr(self.auto_model.config, "max_position_embeddings") and hasattr(self.tokenizer, "model_max_length"):
                 self.modelo_args.max_seq_len = min(self.auto_model.config.max_position_embeddings,
                                      self.tokenizer.model_max_length)
 
         # Define a classe do tokenizador
         if tokenizer_name_or_path is not None:
@@ -184,16 +183,17 @@
     def tokenize(self, texto: Union[str, List[str]]):
         '''        
         Tokeniza um texto para submeter ao modelo de linguagem. 
         Retorna um dicionário listas de mesmo tamanho para garantir o processamento em lote.
         Use a quantidade de tokens para saber até onde deve ser recuperado em uma lista de saída.
         Ou use attention_mask diferente de 1 para saber que posições devem ser utilizadas na lista.
 
-        :param texto: Texto é uma string ou uma lista de strings a serem tokenizados para o modelo de linguagem.
-         
+        Parâmetros:
+        `texto` - Texto é uma string ou uma lista de strings a serem tokenizados para o modelo de linguagem.
+                          
         Retorna um dicionário com:
             tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
             input_ids uma lista com os ids dos tokens de entrada mapeados em seus índices do vocabuário.
             token_type_ids uma lista com os tipos dos tokens.
             attention_mask uma lista com os as máscaras de atenção indicando com '1' os tokens  pertencentes à sentença.
         '''
         
@@ -388,15 +388,15 @@
             lista_tokens  uma lista com os tokens do texto gerados pelo método.
             texto_pos_pln uma lista com as postagging dos tokens gerados pela ferramenta de pln.
             lista_tokens_oov_mcl uma lista com os tokens OOV do mcl.
             lista_embeddings_MEAN uma lista com os embeddings com a estratégia MEAN.
             lista_embeddings_MAX uma lista com os embeddings com a estratégia MAX.
         '''
        
-        #Guarda os tokens e embeddings de retorno
+        # Guarda os tokens e embeddings de retorno
         lista_tokens = []
         lista_tokens_oov_mcl = []
         lista_embeddings_MEAN = []
         lista_embeddings_MAX = []
         
         # Gera a tokenização e POS-Tagging da sentença    
         lista_tokens_texto_pln, lista_pos_texto_pln = pln.getListaTokensPOSTexto(tokens_texto_concatenado)
@@ -593,15 +593,14 @@
     # ============================   
     def save(self, output_path: str):
         '''
         Salva o modelo.
 
         Parâmetros:
         `output_path` - caminho para salvar o modelo
-
         '''
 
         self.auto_model.save_pretrained(output_path)
         self.tokenizer.save_pretrained(output_path)
 
         with open(os.path.join(output_path, 'modelo_linguagem_config.json'), 'w') as fOut:
             json.dump(self.get_config_dict(), fOut, indent=2)
```

### Comparing `texto_transformer-0.0.3/textotransformer/pln/pln.py` & `texto_transformer-0.0.4/textotransformer/pln/pln.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/util/utilambiente.py` & `texto_transformer-0.0.4/textotransformer/util/utilambiente.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/util/utilarquivo.py` & `texto_transformer-0.0.4/textotransformer/util/utilarquivo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/util/utilconstantes.py` & `texto_transformer-0.0.4/textotransformer/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/util/utiltempo.py` & `texto_transformer-0.0.4/textotransformer/util/utiltempo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/textotransformer/util/utiltexto.py` & `texto_transformer-0.0.4/textotransformer/util/utiltexto.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/LICENSE` & `texto_transformer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.3/README.md` & `texto_transformer-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 Você também pode clonar a versão mais recente do [repositório](https://github.com/osmarbraz/texto-transformer.git) e instalá-la diretamente do código-fonte:
 
 <pre><code>$ pip install -e .</code></pre>
 
 O comando deve ser executado no diretório onde foi realizado o download do repositório.
 
-## Exemplo simples de uso
+## Exemplos 
+
+### Uso simples
 
 ````python
 # Importa a classe
 from textotransformer import TextoTransformer
 
 # Instância uma objeto e baixa o modelo de linguagem
 modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
@@ -51,15 +53,55 @@
 #Embedding: tensor([ 8.3348e-02, -1.8269e-01,  5.9241e-01, -9.5235e-02,  5.0978e-01,...
 #Texto: Vai cair tudo na prova?
 #Embedding: tensor([ 1.3447e-01,  1.1854e-01,  6.0201e-02,  1.0271e-01,  2.6321e-01,...
 #Texto: Aguardo uma resposta, João.
 #Embedding: tensor([ 3.7160e-02, -7.3645e-02,  3.3942e-01,  8.0847e-02,  3.8259e-01,...
 ````
 
-O exemplo pode ser executado no notebook do GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).
+### Recuperando embeddings diversos
+
+````python
+# Importa a classe
+from textotransformer import TextoTransformer
+
+# Instância uma objeto e baixa o modelo de linguagem
+modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
+
+texto = "Você gosta de sorvete de manga? Sim, adoro muito."
+
+# Recupera os embeddings consolidados do texto
+embeddings_texto = modelo.getEmbeddingTexto(texto)
+print("Um texto de tamanho      :",len(embeddings_texto))
+
+# Recupera os embeddings consolidados das sentenças do texto
+embeddings_sentenca = modelo.getEmbeddingSentenca(texto)
+print("\nQuantidade de sentenças  :",len(embeddings_sentenca))
+print("Cada sentença de tamanho :",len(embeddings_sentenca[0]))
+
+# Recupera os embeddings consolidados das palavras do texto
+embeddings_palavra = modelo.getEmbeddingPalavra(texto)
+print("\nQuantidade de palavras   :",len(embeddings_palavra))
+print("Cada palavra de tamanho  :",len(embeddings_palavra[0]))
+
+# Recupera os embeddings dos tokens do texto
+embeddings_token = modelo.getEmbeddingToken(texto)
+print("\nQuantidade de tokens     :",len(embeddings_token))
+print("Cada token de tamanho    :",len(embeddings_token[0]))
+
+#Resultado
+#Um texto de tamanho      : 768
+#Quantidade de sentenças  : 2
+#Cada sentença de tamanho : 768
+#Quantidade de palavras   : 12
+#Cada palavra de tamanho  : 768
+#Quantidade de tokens     : 15
+#Cada token de tamanho    : 768
+````
+
+Os exemplos pode ser executado no notebook do GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).
 
 ## Métodos principais:
 
 Métodos principais para recuperar embeddings de textos, sentenças, palavras e tokens. Os embeddings de textos, sentenças e palavras podem ser consolidados pelas estratégias de pooling média (MEAN) e máximo (MAX) dos embeddings de seus tokens.
 
 - `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling: int)`
     - Retorna uma lista dos embeddings consolidados dos textos.
```

### Comparing `texto_transformer-0.0.3/pyproject.toml` & `texto_transformer-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "texto-transformer"
-version = "0.0.3"
+version = "0.0.4"
 description = "Texto Transformer: Framework para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer"
 readme = "README.md"
 requires-python = ">=3.6.0"
 license = { file = "LICENSE" }
 
 authors = [
     { name = "Osmar de Oliveira Braz Junior", email = "osmar.braz@udesc.br" }
```

### Comparing `texto_transformer-0.0.3/PKG-INFO` & `texto_transformer-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texto-transformer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Texto Transformer: Framework para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer
 Project-URL: repository, https://github.com/osmarbraz/textotransformer/
 Author-email: Osmar de Oliveira Braz Junior <osmar.braz@udesc.br>
 License: MIT License
         
         Copyright (c) 2023 Osmar de Oliveira Braz Junior
         
@@ -56,15 +56,17 @@
 
 Você também pode clonar a versão mais recente do [repositório](https://github.com/osmarbraz/texto-transformer.git) e instalá-la diretamente do código-fonte:
 
 <pre><code>$ pip install -e .</code></pre>
 
 O comando deve ser executado no diretório onde foi realizado o download do repositório.
 
-## Exemplo simples de uso
+## Exemplos 
+
+### Uso simples
 
 ````python
 # Importa a classe
 from textotransformer import TextoTransformer
 
 # Instância uma objeto e baixa o modelo de linguagem
 modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
@@ -91,15 +93,55 @@
 #Embedding: tensor([ 8.3348e-02, -1.8269e-01,  5.9241e-01, -9.5235e-02,  5.0978e-01,...
 #Texto: Vai cair tudo na prova?
 #Embedding: tensor([ 1.3447e-01,  1.1854e-01,  6.0201e-02,  1.0271e-01,  2.6321e-01,...
 #Texto: Aguardo uma resposta, João.
 #Embedding: tensor([ 3.7160e-02, -7.3645e-02,  3.3942e-01,  8.0847e-02,  3.8259e-01,...
 ````
 
-O exemplo pode ser executado no notebook do GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).
+### Recuperando embeddings diversos
+
+````python
+# Importa a classe
+from textotransformer import TextoTransformer
+
+# Instância uma objeto e baixa o modelo de linguagem
+modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
+
+texto = "Você gosta de sorvete de manga? Sim, adoro muito."
+
+# Recupera os embeddings consolidados do texto
+embeddings_texto = modelo.getEmbeddingTexto(texto)
+print("Um texto de tamanho      :",len(embeddings_texto))
+
+# Recupera os embeddings consolidados das sentenças do texto
+embeddings_sentenca = modelo.getEmbeddingSentenca(texto)
+print("\nQuantidade de sentenças  :",len(embeddings_sentenca))
+print("Cada sentença de tamanho :",len(embeddings_sentenca[0]))
+
+# Recupera os embeddings consolidados das palavras do texto
+embeddings_palavra = modelo.getEmbeddingPalavra(texto)
+print("\nQuantidade de palavras   :",len(embeddings_palavra))
+print("Cada palavra de tamanho  :",len(embeddings_palavra[0]))
+
+# Recupera os embeddings dos tokens do texto
+embeddings_token = modelo.getEmbeddingToken(texto)
+print("\nQuantidade de tokens     :",len(embeddings_token))
+print("Cada token de tamanho    :",len(embeddings_token[0]))
+
+#Resultado
+#Um texto de tamanho      : 768
+#Quantidade de sentenças  : 2
+#Cada sentença de tamanho : 768
+#Quantidade de palavras   : 12
+#Cada palavra de tamanho  : 768
+#Quantidade de tokens     : 15
+#Cada token de tamanho    : 768
+````
+
+Os exemplos pode ser executado no notebook do GoogleColab [ExemplosTextoTransformer.ipynb](https://github.com/osmarbraz/texto-transformer/blob/main/notebooks/ExemplosTextoTransformer.ipynb).
 
 ## Métodos principais:
 
 Métodos principais para recuperar embeddings de textos, sentenças, palavras e tokens. Os embeddings de textos, sentenças e palavras podem ser consolidados pelas estratégias de pooling média (MEAN) e máximo (MAX) dos embeddings de seus tokens.
 
 - `getEmbeddingTexto(texto: Union[str, List[str]], estrategia_pooling: int)`
     - Retorna uma lista dos embeddings consolidados dos textos.
```

