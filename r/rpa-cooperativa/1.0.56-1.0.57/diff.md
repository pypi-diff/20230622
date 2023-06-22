# Comparing `tmp/rpa_cooperativa-1.0.56.tar.gz` & `tmp/rpa_cooperativa-1.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.56.tar", last modified: Fri Jun 16 13:27:15 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.57.tar", last modified: Thu Jun 22 20:18:15 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.56.tar` & `rpa_cooperativa-1.0.57.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.467083 rpa_cooperativa-1.0.56/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.56/LICENSE
--rw-rw-rw-   0        0        0     6875 2023-06-16 13:27:15.464563 rpa_cooperativa-1.0.56/PKG-INFO
--rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.56/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.230706 rpa_cooperativa-1.0.56/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.56/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.420188 rpa_cooperativa-1.0.56/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.56/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.56/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.56/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.56/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.56/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    87556 2023-06-16 13:17:06.000000 rpa_cooperativa-1.0.56/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.458887 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6875 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      567 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 13:27:15.468601 rpa_cooperativa-1.0.56/setup.cfg
--rw-rw-rw-   0        0        0     2336 2023-06-16 13:09:25.000000 rpa_cooperativa-1.0.56/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:15.912941 rpa_cooperativa-1.0.57/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.57/LICENSE
+-rw-rw-rw-   0        0        0     6875 2023-06-22 20:18:15.908190 rpa_cooperativa-1.0.57/PKG-INFO
+-rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.57/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:15.618781 rpa_cooperativa-1.0.57/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.57/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:15.845424 rpa_cooperativa-1.0.57/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.57/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.57/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.57/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.57/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.57/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.57/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.57/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.57/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.57/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.57/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.57/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    87959 2023-06-22 20:16:20.000000 rpa_cooperativa-1.0.57/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:15.902194 rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6875 2023-06-22 20:18:14.000000 rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-06-22 20:18:14.000000 rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:18:14.000000 rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 20:18:14.000000 rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      567 2023-06-22 20:18:14.000000 rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 20:18:14.000000 rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:18:15.917007 rpa_cooperativa-1.0.57/setup.cfg
+-rw-rw-rw-   0        0        0     2336 2023-06-22 20:18:06.000000 rpa_cooperativa-1.0.57/setup.py
```

### Comparing `rpa_cooperativa-1.0.56/LICENSE` & `rpa_cooperativa-1.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/PKG-INFO` & `rpa_cooperativa-1.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.56
+Version: 1.0.57
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.56/README.md` & `rpa_cooperativa-1.0.57/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.57/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.57/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.57/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.57/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.57/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.57/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1273,14 +1273,15 @@
             self.p.click()
             # self.p.doubleClick()
         time.sleep(3)
             
    
 
         num_menu = 0
+        self.janelas = []
         self.janela_sacg = janela
         self.janela_siat = janela
         self.janela_siac = janela
         
         opcoes = [x.upper() for x in opcoes]
         
         for menu in opcoes:
@@ -1289,39 +1290,42 @@
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, grayscale=True)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, grayscale=True)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_sacg = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
+                self.janelas.append(self.janela_sacg)
                 print('clicou no menu: sacg')
-                janela.activate()
+                self.janela_sacg.activate()
             elif menu == 'SIAT':
                 # Abrir SIAT
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, grayscale=True)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, grayscale=True)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_siat = self.p.getWindowsWithTitle('teoff-exe')[num_menu] 
+                self.janelas.append(self.janela_siat)
                 print('clicou no menu: siat')
-                janela.activate()
+                self.janela_siat.activate()
             elif menu == 'SIAC':
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, grayscale=True)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, grayscale=True)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_siac = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
+                self.janelas.append(self.janela_siac)
                 print('clicou no menu: siac')
-                janela.activate()
+                self.janela_siac.activate()
             time.sleep(1)
-        return self.janela_sacg, self.janela_siat, self.janela_siac
+        return self.janelas
 
              
     def select_menu_letras(self, letras, nome_janela=None):
         '''acc.select_menu_letras(letras) \n
          acc.select_menu_letras(letras, nome_janela='sacg')'''
         self.p.sleep(1)
         nome_janela = str(nome_janela).upper()
@@ -1396,54 +1400,56 @@
             self.p.sleep(1)
             self.p.typewrite(letras[6])
             self.p.sleep(1)
         else:
             print('ops funcao entende apenas 2, 3, 4, 5, 6 ou 7 letras')
             
                   
-    def get_text(self, ini_linha: int=22, fim_linha: int=632, topo1: int=410, topo2: int=415, tempo_arrastar_soltar: float=1.5, nome_janela: str | None=None):
+    def get_text(self, ini_linha: int=22, fim_linha: int=632, topo1: int=410, topo2: int=415, tempo_arrastar_soltar: float=1.5, nome_janela: str | None=None, index_janela: int=-1):
         ''' acc.get_text('Retorna ao Sistema')\n
          acc.get_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
         nome_janela = str(nome_janela).upper()
-        if nome_janela == 'SIAT':
-            janela = self.janela_siat
-        elif nome_janela == 'SIAC':
-            janela = self.janela_siac
-        elif nome_janela == 'SACG':
-            janela = self.janela_sacg
+        if index_janela >= 0:
+            janela = self.janelas[index_janela] 
         else:
-            janela = self.p.getWindowsWithTitle('teoff-exe')[0]
+            if nome_janela == 'SIAT':
+                janela = self.janela_siat
+            elif nome_janela == 'SIAC':
+                janela = self.janela_siac
+            elif nome_janela == 'SACG':
+                janela = self.janela_sacg
+            else:
+                janela = self.p.getWindowsWithTitle('teoff-exe')[0]
   
         time.sleep(1)
         janela.activate()
         self.p.moveTo(janela.left + ini_linha, janela.top + topo1)
         self.p.sleep(1)
         self.p.dragTo(janela.left + fim_linha, janela.top + topo2, tempo_arrastar_soltar, button='left')
         self.p.moveTo(janela.left + ini_linha, janela.top + topo2)
         self.p.rightClick()
         capturado = self.pyperclip.paste()
         print(f'texto capturado:{capturado}')
         return capturado            
             
-            
-     
-    def exist_text(self, texto_esperado: str, max_tentativas: int=7, segundos_entre_tentativas: int=3, ini_linha: int=22, fim_linha: int=632, topo1: int=412, topo2: int=412, tempo_arrastar_soltar: float=1.5, continua_seerro: bool=False, nome_janela: str |None=None):
+              
+    def exist_text(self, texto_esperado: str, max_tentativas: int=7, segundos_entre_tentativas: int=3, ini_linha: int=22, fim_linha: int=632, topo1: int=412, topo2: int=412, tempo_arrastar_soltar: float=1.5, continua_seerro: bool=False, nome_janela: str |None=None, index_janela: int=-1):
         ''' acc.exist_text('Retorna ao Sistema')\n
          acc.exist_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
         self.pyperclip.copy('')
         tentativas = 0
         time.sleep(1)
-        captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela)
+        captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela, index_janela=index_janela)
         resultado = True
         while not texto_esperado in captura and tentativas < max_tentativas:
             print('esperando texto: ', texto_esperado)
             self.p.sleep(segundos_entre_tentativas)
-            captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela)
+            captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela, index_janela=index_janela)
             tentativas += 1
             if tentativas == max_tentativas:
                 resultado = False
         print(resultado)
         if resultado == False and continua_seerro == False:
             raise Exception(f'Execução pausada. O texto: "{texto_esperado}" não foi localizado durante a execução do robô.')
         return resultado
```

### Comparing `rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.56
+Version: 1.0.57
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.57/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.56/setup.py` & `rpa_cooperativa-1.0.57/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.56",
+    version="1.0.57",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

