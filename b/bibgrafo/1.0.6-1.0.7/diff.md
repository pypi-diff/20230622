# Comparing `tmp/bibgrafo-1.0.6-py3-none-any.whl.zip` & `tmp/bibgrafo-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,25 @@
-Zip file size: 15152 bytes, number of entries: 12
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-14 18:17 bibgrafo/__init__.py
--rw-rw-r--  2.0 unx     3773 b- defN 22-Oct-14 18:17 bibgrafo/aresta.py
--rw-rw-r--  2.0 unx     6855 b- defN 22-Oct-14 18:17 bibgrafo/grafo.py
--rw-rw-r--  2.0 unx      713 b- defN 22-Oct-14 18:17 bibgrafo/grafo_errors.py
--rw-rw-r--  2.0 unx    12900 b- defN 22-Oct-14 18:25 bibgrafo/grafo_lista_adjacencia.py
--rw-rw-r--  2.0 unx    17584 b- defN 22-Oct-14 18:25 bibgrafo/grafo_matriz_adj_dir.py
--rw-rw-r--  2.0 unx    16803 b- defN 22-Oct-14 18:26 bibgrafo/grafo_matriz_adj_nao_dir.py
--rw-rw-r--  2.0 unx     2754 b- defN 22-Oct-14 18:17 bibgrafo/vertice.py
--rw-rw-r--  2.0 unx      234 b- defN 22-Oct-14 20:29 bibgrafo-1.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Oct-14 20:29 bibgrafo-1.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 22-Oct-14 20:29 bibgrafo-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      955 b- defN 22-Oct-14 20:29 bibgrafo-1.0.6.dist-info/RECORD
-12 files, 62672 bytes uncompressed, 13554 bytes compressed:  78.4%
+Zip file size: 40891 bytes, number of entries: 23
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-30 23:02 bibgrafo/__init__.py
+-rw-rw-r--  2.0 unx     3773 b- defN 23-Jun-22 13:10 bibgrafo/aresta.py
+-rw-rw-r--  2.0 unx     6855 b- defN 23-Jun-22 13:10 bibgrafo/grafo.py
+-rw-rw-r--  2.0 unx      713 b- defN 23-Jun-22 13:10 bibgrafo/grafo_errors.py
+-rw-rw-r--  2.0 unx      155 b- defN 22-Jun-30 23:02 bibgrafo/grafo_exceptions.py
+-rw-rw-r--  2.0 unx    12940 b- defN 23-Jun-22 13:10 bibgrafo/grafo_lista_adj.py
+-rw-rw-r--  2.0 unx    12940 b- defN 22-Sep-08 02:44 bibgrafo/grafo_lista_adjacencia.py
+-rw-rw-r--  2.0 unx    17623 b- defN 23-Jun-22 13:10 bibgrafo/grafo_matriz_adj_dir.py
+-rw-rw-r--  2.0 unx    16842 b- defN 23-Jun-22 13:10 bibgrafo/grafo_matriz_adj_nao_dir.py
+-rw-rw-r--  2.0 unx     2754 b- defN 23-Jun-22 13:10 bibgrafo/vertice.py
+-rw-rw-r--  2.0 unx      163 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--  2.0 unx     4336 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/aresta.cpython-310.pyc
+-rw-rw-r--  2.0 unx     8151 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/grafo.cpython-310.pyc
+-rw-rw-r--  2.0 unx     1167 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/grafo_errors.cpython-310.pyc
+-rw-rw-r--  2.0 unx      602 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/grafo_exceptions.cpython-310.pyc
+-rw-rw-r--  2.0 unx    12527 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/grafo_lista_adjacencia.cpython-310.pyc
+-rw-rw-r--  2.0 unx    14589 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/grafo_matriz_adj_dir.cpython-310.pyc
+-rw-rw-r--  2.0 unx    12844 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/grafo_matriz_adj_nao_dir.cpython-310.pyc
+-rw-rw-r--  2.0 unx     3478 b- defN 22-Sep-08 02:33 bibgrafo/__pycache__/vertice.cpython-310.pyc
+-rw-rw-r--  2.0 unx      234 b- defN 23-Jun-22 19:34 bibgrafo-1.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 19:34 bibgrafo-1.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-22 19:34 bibgrafo-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2091 b- defN 23-Jun-22 19:34 bibgrafo-1.0.7.dist-info/RECORD
+23 files, 134878 bytes uncompressed, 37441 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -6,32 +6,65 @@
 
 Filename: bibgrafo/grafo.py
 Comment: 
 
 Filename: bibgrafo/grafo_errors.py
 Comment: 
 
+Filename: bibgrafo/grafo_exceptions.py
+Comment: 
+
+Filename: bibgrafo/grafo_lista_adj.py
+Comment: 
+
 Filename: bibgrafo/grafo_lista_adjacencia.py
 Comment: 
 
 Filename: bibgrafo/grafo_matriz_adj_dir.py
 Comment: 
 
 Filename: bibgrafo/grafo_matriz_adj_nao_dir.py
 Comment: 
 
 Filename: bibgrafo/vertice.py
 Comment: 
 
-Filename: bibgrafo-1.0.6.dist-info/METADATA
+Filename: bibgrafo/__pycache__/__init__.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/aresta.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/grafo.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/grafo_errors.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/grafo_exceptions.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/grafo_lista_adjacencia.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/grafo_matriz_adj_dir.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/grafo_matriz_adj_nao_dir.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo/__pycache__/vertice.cpython-310.pyc
+Comment: 
+
+Filename: bibgrafo-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: bibgrafo-1.0.6.dist-info/WHEEL
+Filename: bibgrafo-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: bibgrafo-1.0.6.dist-info/top_level.txt
+Filename: bibgrafo-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: bibgrafo-1.0.6.dist-info/RECORD
+Filename: bibgrafo-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bibgrafo/grafo_lista_adjacencia.py

```diff
@@ -13,14 +13,17 @@
 
     Attributes:
         _vertices (list): Uma lista dos vértices (ou nodos) do grafo.
         _arestas: Uma dicionário que guarda as arestas do grafo. A chave representa o nome da aresta e o valor é um
         objeto do tipo Aresta que deve conter referências para os vértices
     """
 
+    _vertices: list
+    _arestas: dict
+
     def __init__(self, vertices=None, arestas=None):
         """
         Constrói um objeto do tipo GrafoListaAdjacencia. Se nenhum parâmetro for passado, cria um Grafo vazio.
         Se houver alguma aresta ou algum vértice inválido, um erro é lançado.
         Nessa implementação o Grafo é representado por uma lista de adjacências.
 
         Args:
```

## bibgrafo/grafo_matriz_adj_dir.py

```diff
@@ -13,14 +13,17 @@
     Attributes:
         _vertices (list): Uma lista dos vértices (ou nodos) do grafo.
         _matriz: Uma matriz de adjacência que guarda as arestas do grafo. Cada entrada da matriz tem um
         dicionário de arestas (objetos do tipo Aresta) para que seja possível representar arestas paralelas
         e que cada aresta tenha seus próprios atributos distintos.
     """
 
+    _vertices: list
+    _matriz: list
+
     def __init__(self, vertices: list = None, matriz: list = None):
         """
         Constrói um objeto do tipo grafo direcionado com matriz de adjacência.
         Se nenhum parâmetro for passado, cria um grafo vazio.
         Se houver alguma aresta ou algum vértice inválido, uma exceção é lançada.
         Args:
             vertices: Uma lista dos vértices (ou nodos) do grafo.
```

## bibgrafo/grafo_matriz_adj_nao_dir.py

```diff
@@ -13,14 +13,17 @@
 
     Attributes:
         _vertices (list): Uma lista dos vértices (ou nodos) do grafo.
         _arestas: Uma dicionário que guarda as arestas do grafo. A chave representa o nome da aresta e o valor é um
         objeto do tipo Aresta que deve conter referências para os vértices
     """
 
+    _vertices: list
+    _matriz: list
+
     def __init__(self, vertices=None, matriz=None):
         """
         Constrói um objeto do tipo grafo não direcionado com matriz de adjacência.
         Se nenhum parâmetro for passado, cria um grafo vazio.
         Se houver alguma aresta ou algum vértice inválido, uma exceção é lançada.
         :param vertices: Uma lista dos vértices (ou nodos) do grafo.
         :param matriz: Uma matriz de adjacência que guarda as arestas do grafo. Cada entrada da matriz tem um
```

