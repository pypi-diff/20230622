# Comparing `tmp/trulens_eval-0.3.0a0-py3-none-any.whl.zip` & `tmp/trulens_eval-0.3.0b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 91824 bytes, number of entries: 34
+Zip file size: 91810 bytes, number of entries: 34
 -rw-rw-r--  2.0 unx     5164 b- defN 23-Jun-22 21:05 trulens_eval/Example_TruBot.py
 -rw-rw-r--  2.0 unx     3093 b- defN 23-Jun-22 21:05 trulens_eval/Leaderboard.py
--rw-rw-r--  2.0 unx     1227 b- defN 23-Jun-22 21:13 trulens_eval/__init__.py
+-rw-rw-r--  2.0 unx     1227 b- defN 23-Jun-22 21:23 trulens_eval/__init__.py
 -rw-rw-r--  2.0 unx    10979 b- defN 23-Jun-22 21:05 trulens_eval/app.py
 -rw-rw-r--  2.0 unx     5344 b- defN 23-Jun-22 21:05 trulens_eval/benchmark.py
 -rw-rw-r--  2.0 unx    18889 b- defN 23-Jun-22 21:05 trulens_eval/db.py
 -rw-rw-r--  2.0 unx    31403 b- defN 23-Jun-22 21:05 trulens_eval/feedback.py
 -rw-rw-r--  2.0 unx     3443 b- defN 23-Jun-09 21:41 trulens_eval/feedback_prompts.py
 -rw-rw-r--  2.0 unx    20140 b- defN 23-Jun-22 21:05 trulens_eval/instruments.py
 -rw-rw-r--  2.0 unx     1406 b- defN 23-Jun-22 21:05 trulens_eval/keys.py
@@ -25,12 +25,12 @@
 -rw-rw-r--  2.0 unx     5365 b- defN 23-Jun-22 21:05 trulens_eval/utils/langchain.py
 -rw-rw-r--  2.0 unx     4774 b- defN 23-Jun-22 21:05 trulens_eval/utils/llama.py
 -rw-rw-r--  2.0 unx     1001 b- defN 23-Jun-14 03:10 trulens_eval/utils/notebook_utils.py
 -rw-rw-r--  2.0 unx      915 b- defN 23-Jun-09 21:41 trulens_eval/ux/add_logo.py
 -rw-rw-r--  2.0 unx     3790 b- defN 23-Jun-22 21:05 trulens_eval/ux/components.py
 -rw-rw-r--  2.0 unx     1209 b- defN 23-Jun-22 21:05 trulens_eval/ux/styles.py
 -rw-rw-r--  2.0 unx    29567 b- defN 23-Jun-09 21:41 trulens_eval/ux/trulens_logo.svg
--rw-rw-r--  2.0 unx    14878 b- defN 23-Jun-22 21:15 trulens_eval-0.3.0a0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 21:15 trulens_eval-0.3.0a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 23-Jun-22 21:15 trulens_eval-0.3.0a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2834 b- defN 23-Jun-22 21:15 trulens_eval-0.3.0a0.dist-info/RECORD
-34 files, 283874 bytes uncompressed, 87316 bytes compressed:  69.2%
+-rw-rw-r--  2.0 unx    14755 b- defN 23-Jun-22 21:23 trulens_eval-0.3.0b0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 21:23 trulens_eval-0.3.0b0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jun-22 21:23 trulens_eval-0.3.0b0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2834 b- defN 23-Jun-22 21:23 trulens_eval-0.3.0b0.dist-info/RECORD
+34 files, 283751 bytes uncompressed, 87302 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -84,20 +84,20 @@
 
 Filename: trulens_eval/ux/styles.py
 Comment: 
 
 Filename: trulens_eval/ux/trulens_logo.svg
 Comment: 
 
-Filename: trulens_eval-0.3.0a0.dist-info/METADATA
+Filename: trulens_eval-0.3.0b0.dist-info/METADATA
 Comment: 
 
-Filename: trulens_eval-0.3.0a0.dist-info/WHEEL
+Filename: trulens_eval-0.3.0b0.dist-info/WHEEL
 Comment: 
 
-Filename: trulens_eval-0.3.0a0.dist-info/top_level.txt
+Filename: trulens_eval-0.3.0b0.dist-info/top_level.txt
 Comment: 
 
-Filename: trulens_eval-0.3.0a0.dist-info/RECORD
+Filename: trulens_eval-0.3.0b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trulens_eval/__init__.py

```diff
@@ -29,15 +29,15 @@
     - `provider_apis.py` `feedback_prompts.py`
 
     - `schema.py`
 
     - `util.py` `keys.py`
 """
 
-__version__ = "0.3.0a"
+__version__ = "0.3.0b"
 
 from trulens_eval.schema import FeedbackMode
 from trulens_eval.schema import Query, Select
 from trulens_eval.tru import Tru
 from trulens_eval.tru_chain import TruChain
 from trulens_eval.feedback import Feedback
 from trulens_eval.feedback import Huggingface
```

## Comparing `trulens_eval-0.3.0a0.dist-info/METADATA` & `trulens_eval-0.3.0b0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulens-eval
-Version: 0.3.0a0
+Version: 0.3.0b0
 Summary: Library with langchain instrumentation to evaluate LLM based applications.
 Home-page: https://www.trulens.org
 Author: Truera Inc
 Author-email: all@truera.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -47,21 +47,19 @@
 
 ![Architecture Diagram](https://www.trulens.org/Assets/image/TruLens_Architecture.png)
 
 ## Quick Usage
 
 To quickly play around with the TruLens Eval library:
 
-[langchain_quickstart.ipynb](https://github.com/truera/trulens/blob/releases/rc-trulens-eval-0.2.2/trulens_eval/examples/quickstart.ipynb).
+[langchain_quickstart.ipynb](https://github.com/truera/trulens/blob/releases/rc-trulens-eval-0.3.0/trulens_eval/examples/quickstart.ipynb).
 
-[langchain_quickstart.py](https://github.com/truera/trulens/blob/releases/rc-trulens-eval-0.2.2/trulens_eval/examples/quickstart.py).
+[langchain_quickstart.py](https://github.com/truera/trulens/blob/releases/rc-trulens-eval-0.3.0/trulens_eval/examples/quickstart.py).
 
-[llamaindex_quickstart.ipynb](https://github.com/truera/trulens/blob/releases/rc-trulens-eval-0.2.2/trulens_eval/examples/llama_index/quickstart.ipynb).
-
-[llamaindex_quickstart.py](https://github.com/truera/trulens/blob/quickstart-script-links/trulens_eval/examples/llama_quickstart.py)
+[llamaindex_quickstart.ipynb](https://github.com/truera/trulens/blob/releases/rc-trulens-eval-0.3.0/trulens_eval/examples/vector-dbs/llama_index/quickstart.ipynb).
 
 
 
 ## Installation and Setup
 
 Install the trulens-eval pip package from PyPI.
```

## Comparing `trulens_eval-0.3.0a0.dist-info/RECORD` & `trulens_eval-0.3.0b0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 trulens_eval/Example_TruBot.py,sha256=h09iD3TO_Bje86_0PeF1_Q_y7OOehz26NudYOTC1c0U,5164
 trulens_eval/Leaderboard.py,sha256=84--99d_Kn2A96BCW0rSLMfcIo3MkGD0zv1lxxAzelY,3093
-trulens_eval/__init__.py,sha256=z8PSrZ2PwDvdg4ka4qZU9Rt2hwR7BlVJrfC7o7hmm24,1227
+trulens_eval/__init__.py,sha256=UIHWUHGDGdmiDTMGVqXluLv1c1OKqRweNKacDl9jyHM,1227
 trulens_eval/app.py,sha256=wQzkZ0HEOiZ8CpuEtAYbCS5uqMfzoHp6eQTtFj9VRrs,10979
 trulens_eval/benchmark.py,sha256=GI-JmBBr8KswuMaXVoJ2Rm6eAtjtwhYThcNheZakQNo,5344
 trulens_eval/db.py,sha256=lE0lmfBcPqVrCDEphM64HXFz6iQ6BdqQw3oR8g9HqPs,18889
 trulens_eval/feedback.py,sha256=TzxzQycvcDS2yDm9loTeJjxMsr--oTyNqMKLyqYPhUk,31403
 trulens_eval/feedback_prompts.py,sha256=DgW4_f_4g018tYNwca1D1taJhhdwaf2fDR9J8s0Upls,3443
 trulens_eval/instruments.py,sha256=lysx4kcwtl42Rh2_S_2oLHUp8RrtCvSuiRHls9zsJbs,20140
 trulens_eval/keys.py,sha256=8Z9qkMhXMypI1GD39JeUTiibJNLcxm7naWlDUNCK2vo,1406
@@ -24,11 +24,11 @@
 trulens_eval/utils/langchain.py,sha256=3NPeUtDqHtDnEx3MRz-_hx9OFfVQjVKsh4-vioccgYI,5365
 trulens_eval/utils/llama.py,sha256=O8nranBcDrFapRlZpm46NfORZ3WyCI0QCIiiF1hicvw,4774
 trulens_eval/utils/notebook_utils.py,sha256=QTB2tedjSNF5d25sfrJEg20aqcK3Kx3MfcteeWcRzxQ,1001
 trulens_eval/ux/add_logo.py,sha256=Pwl6mfzAX1VSi2VTOZsMBoCstaBuVGoSrs7P5tomP4U,915
 trulens_eval/ux/components.py,sha256=24knLc1UN_0H333w-GccOzGyXoe1iFuxRUhOPBSYJok,3790
 trulens_eval/ux/styles.py,sha256=WYdJIsvUwPla1oZepc1FsmUJNPkT0vW0xt5sCSMs2qA,1209
 trulens_eval/ux/trulens_logo.svg,sha256=92RLTgG0YDPEtZcQWWI7aXTYZAW4wAOAkIIgKUbTiW8,29567
-trulens_eval-0.3.0a0.dist-info/METADATA,sha256=_nA6pw-4oCG5IkuP9l3DUdYmDLvVgsIKLcKMPoYgwys,14878
-trulens_eval-0.3.0a0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-trulens_eval-0.3.0a0.dist-info/top_level.txt,sha256=AKIBExe5S-v-TbsBrhe1ctF06PubKoYmWNS9rJ1Rb_o,13
-trulens_eval-0.3.0a0.dist-info/RECORD,,
+trulens_eval-0.3.0b0.dist-info/METADATA,sha256=EsYhovGyUMnfN5CEJn91uDQLAjZPAfOicjq9KDofNWY,14755
+trulens_eval-0.3.0b0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+trulens_eval-0.3.0b0.dist-info/top_level.txt,sha256=AKIBExe5S-v-TbsBrhe1ctF06PubKoYmWNS9rJ1Rb_o,13
+trulens_eval-0.3.0b0.dist-info/RECORD,,
```

