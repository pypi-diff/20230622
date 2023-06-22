# Comparing `tmp/discopy-1.1.3.tar.gz` & `tmp/discopy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discopy-1.1.3.tar", last modified: Thu Jun  1 18:45:51 2023, max compression
+gzip compressed data, was "discopy-1.1.4.tar", last modified: Thu Jun 22 11:15:43 2023, max compression
```

## Comparing `discopy-1.1.3.tar` & `discopy-1.1.4.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.908706 discopy-1.1.3/
--rw-r--r--   0 boldi      (502) staff       (20)       33 2022-09-27 14:39:16.000000 discopy-1.1.3/.gitattributes
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.847974 discopy-1.1.3/.github/
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.853726 discopy-1.1.3/.github/workflows/
--rw-r--r--   0 boldi      (502) staff       (20)     1714 2023-05-31 13:21:06.000000 discopy-1.1.3/.github/workflows/build_test.yml
--rw-r--r--   0 boldi      (502) staff       (20)      183 2023-05-31 09:22:59.000000 discopy-1.1.3/.gitignore
--rw-r--r--   0 boldi      (502) staff       (20)    20606 2023-05-31 09:22:59.000000 discopy-1.1.3/.pylintrc
--rw-r--r--   0 boldi      (502) staff       (20)      744 2023-05-31 09:22:59.000000 discopy-1.1.3/.readthedocs.yaml
--rw-r--r--   0 boldi      (502) staff       (20)     1171 2023-05-31 09:22:59.000000 discopy-1.1.3/CONTRIBUTING.md
--rw-r--r--   0 boldi      (502) staff       (20)     1520 2023-05-31 09:22:59.000000 discopy-1.1.3/LICENSE
--rw-r--r--   0 boldi      (502) staff       (20)     7385 2023-06-01 18:45:51.908423 discopy-1.1.3/PKG-INFO
--rw-r--r--   0 boldi      (502) staff       (20)     4532 2023-05-31 09:22:59.000000 discopy-1.1.3/README.md
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.860295 discopy-1.1.3/discopy/
--rw-r--r--   0 boldi      (502) staff       (20)      499 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/__init__.py
--rw-r--r--   0 boldi      (502) staff       (20)     5758 2023-05-31 13:40:28.000000 discopy-1.1.3/discopy/balanced.py
--rw-r--r--   0 boldi      (502) staff       (20)     8305 2023-05-31 13:40:04.000000 discopy-1.1.3/discopy/braided.py
--rw-r--r--   0 boldi      (502) staff       (20)    28177 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/cat.py
--rw-r--r--   0 boldi      (502) staff       (20)    10172 2023-05-31 13:23:34.000000 discopy-1.1.3/discopy/closed.py
--rw-r--r--   0 boldi      (502) staff       (20)     4513 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/compact.py
--rw-r--r--   0 boldi      (502) staff       (20)     1487 2023-06-01 16:43:13.000000 discopy-1.1.3/discopy/config.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.861686 discopy-1.1.3/discopy/drawing/
--rw-r--r--   0 boldi      (502) staff       (20)     1060 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/drawing/__init__.py
--rw-r--r--   0 boldi      (502) staff       (20)    13859 2023-05-31 14:06:48.000000 discopy-1.1.3/discopy/drawing/grid.py
--rw-r--r--   0 boldi      (502) staff       (20)    36817 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/drawing/legacy.py
--rw-r--r--   0 boldi      (502) staff       (20)    11666 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/frobenius.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.863470 discopy-1.1.3/discopy/grammar/
--rw-r--r--   0 boldi      (502) staff       (20)      225 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/grammar/__init__.py
--rw-r--r--   0 boldi      (502) staff       (20)     9422 2023-05-31 13:42:02.000000 discopy-1.1.3/discopy/grammar/categorial.py
--rw-r--r--   0 boldi      (502) staff       (20)     6950 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/grammar/cfg.py
--rw-r--r--   0 boldi      (502) staff       (20)      926 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/grammar/dependency.py
--rw-r--r--   0 boldi      (502) staff       (20)     7191 2023-05-31 14:01:32.000000 discopy-1.1.3/discopy/grammar/pregroup.py
--rw-r--r--   0 boldi      (502) staff       (20)     2424 2023-05-31 14:01:45.000000 discopy-1.1.3/discopy/grammar/thue.py
--rw-r--r--   0 boldi      (502) staff       (20)    48238 2023-05-31 14:06:54.000000 discopy-1.1.3/discopy/hypergraph.py
--rw-r--r--   0 boldi      (502) staff       (20)    14080 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/interaction.py
--rw-r--r--   0 boldi      (502) staff       (20)     8157 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/markov.py
--rw-r--r--   0 boldi      (502) staff       (20)    16209 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/matrix.py
--rw-r--r--   0 boldi      (502) staff       (20)     1555 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/messages.py
--rw-r--r--   0 boldi      (502) staff       (20)    35290 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/monoidal.py
--rw-r--r--   0 boldi      (502) staff       (20)     6871 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/pivotal.py
--rw-r--r--   0 boldi      (502) staff       (20)     7845 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/python.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.865940 discopy-1.1.3/discopy/quantum/
--rw-r--r--   0 boldi      (502) staff       (20)      667 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/__init__.py
--rw-r--r--   0 boldi      (502) staff       (20)     5238 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/ansatze.py
--rw-r--r--   0 boldi      (502) staff       (20)    11626 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/channel.py
--rw-r--r--   0 boldi      (502) staff       (20)    32776 2023-06-01 12:28:37.000000 discopy-1.1.3/discopy/quantum/circuit.py
--rw-r--r--   0 boldi      (502) staff       (20)    24616 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/quantum/gates.py
--rw-r--r--   0 boldi      (502) staff       (20)    15811 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/quantum/pennylane.py
--rw-r--r--   0 boldi      (502) staff       (20)    16429 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/tk.py
--rw-r--r--   0 boldi      (502) staff       (20)    13451 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/zx.py
--rw-r--r--   0 boldi      (502) staff       (20)     6916 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/ribbon.py
--rw-r--r--   0 boldi      (502) staff       (20)    25755 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/rigid.py
--rw-r--r--   0 boldi      (502) staff       (20)     9969 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/symmetric.py
--rw-r--r--   0 boldi      (502) staff       (20)    23157 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/tensor.py
--rw-r--r--   0 boldi      (502) staff       (20)     7706 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/traced.py
--rw-r--r--   0 boldi      (502) staff       (20)    20763 2023-05-31 13:26:18.000000 discopy-1.1.3/discopy/utils.py
--rw-r--r--   0 boldi      (502) staff       (20)      160 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy/version.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.861031 discopy-1.1.3/discopy.egg-info/
--rw-r--r--   0 boldi      (502) staff       (20)     7385 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/PKG-INFO
--rw-r--r--   0 boldi      (502) staff       (20)     6574 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/SOURCES.txt
--rw-r--r--   0 boldi      (502) staff       (20)        1 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/dependency_links.txt
--rw-r--r--   0 boldi      (502) staff       (20)      417 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/requires.txt
--rw-r--r--   0 boldi      (502) staff       (20)        8 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/top_level.txt
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.867089 discopy-1.1.3/docs/
--rw-r--r--   0 boldi      (502) staff       (20)      634 2022-09-27 14:39:16.000000 discopy-1.1.3/docs/Makefile
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.867616 discopy-1.1.3/docs/_ext/
--rw-r--r--   0 boldi      (502) staff       (20)      684 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_ext/bases-fullname.py
--rw-r--r--   0 boldi      (502) staff       (20)     3939 2022-12-13 17:02:09.000000 discopy-1.1.3/docs/_ext/youtube.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.868799 discopy-1.1.3/docs/_static/
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.870849 discopy-1.1.3/docs/_static/balanced/
--rw-r--r--   0 boldi      (502) staff       (20)    14901 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/balanced/ribbon_twist.png
--rw-r--r--   0 boldi      (502) staff       (20)    13367 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/balanced/twist.png
--rw-r--r--   0 boldi      (502) staff       (20)    11712 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/balanced/twist_dual_rail.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.871142 discopy-1.1.3/docs/_static/braided/
--rw-r--r--   0 boldi      (502) staff       (20)     8951 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/braided/hexagons.png
--rw-r--r--   0 boldi      (502) staff       (20)     9432 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/braided/inverse.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.871621 discopy-1.1.3/docs/_static/closed/
--rw-r--r--   0 boldi      (502) staff       (20)    15711 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/closed/curry-left.png
--rw-r--r--   0 boldi      (502) staff       (20)    15643 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/closed/curry-right.png
--rw-r--r--   0 boldi      (502) staff       (20)    19051 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/closed/uncurry.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.872535 discopy-1.1.3/docs/_static/compact/
--rw-r--r--   0 boldi      (502) staff       (20)    14358 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/compact/reidemeister.png
--rw-r--r--   0 boldi      (502) staff       (20)    10190 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/compact/snake.png
--rw-r--r--   0 boldi      (502) staff       (20)    14358 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/compact/yanking.png
--rw-r--r--   0 boldi      (502) staff       (20)    14061 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/compact/yanking_cup_and_cap.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.873083 discopy-1.1.3/docs/_static/drawing/
--rw-r--r--   0 boldi      (502) staff       (20)     5271 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/drawing/diagramize.png
--rw-r--r--   0 boldi      (502) staff       (20)     3578 2023-06-01 16:57:36.000000 discopy-1.1.3/docs/_static/drawing/example.html
--rw-r--r--   0 boldi      (502) staff       (20)    10626 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/drawing/frobenius-axioms.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.873664 discopy-1.1.3/docs/_static/frobenius/
--rw-r--r--   0 boldi      (502) staff       (20)    17147 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/comonoid.png
--rw-r--r--   0 boldi      (502) staff       (20)    14853 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/frobenius.png
--rw-r--r--   0 boldi      (502) staff       (20)    17266 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/monoid.png
--rw-r--r--   0 boldi      (502) staff       (20)     9884 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/special.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.873973 discopy-1.1.3/docs/_static/grammar/
--rw-r--r--   0 boldi      (502) staff       (20)     9591 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/grammar/cfg-example.png
--rw-r--r--   0 boldi      (502) staff       (20)     7224 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/grammar/pregroup-example.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.874624 discopy-1.1.3/docs/_static/hypergraph/
--rw-r--r--   0 boldi      (502) staff       (20)    16894 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/hypergraph/box.png
--rw-r--r--   0 boldi      (502) staff       (20)    20670 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/hypergraph/diagram.png
--rw-r--r--   0 boldi      (502) staff       (20)    15394 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/hypergraph/unfuse.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.876078 discopy-1.1.3/docs/_static/int/
--rw-r--r--   0 boldi      (502) staff       (20)    16145 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/alice-loves-bob.png
--rw-r--r--   0 boldi      (502) staff       (20)    18363 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/braid.png
--rw-r--r--   0 boldi      (502) staff       (20)    16332 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/composition.png
--rw-r--r--   0 boldi      (502) staff       (20)     8274 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/dagger.png
--rw-r--r--   0 boldi      (502) staff       (20)    16257 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/idl.png
--rw-r--r--   0 boldi      (502) staff       (20)    16615 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/idr.png
--rw-r--r--   0 boldi      (502) staff       (20)    16069 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/int-snake-equations.png
--rw-r--r--   0 boldi      (502) staff       (20)    22712 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/simplify.png
--rw-r--r--   0 boldi      (502) staff       (20)    16278 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/tensor.png
--rw-r--r--   0 boldi      (502) staff       (20)   105662 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/logo.ico
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.876767 discopy-1.1.3/docs/_static/markov/
--rw-r--r--   0 boldi      (502) staff       (20)    13158 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/markov/associativity.png
--rw-r--r--   0 boldi      (502) staff       (20)    14407 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/markov/bialgebra.png
--rw-r--r--   0 boldi      (502) staff       (20)    10317 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/markov/copy_and_apply.png
--rw-r--r--   0 boldi      (502) staff       (20)     8979 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/markov/counit.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.879394 discopy-1.1.3/docs/_static/monoidal/
--rw-r--r--   0 boldi      (502) staff       (20)     2875 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/Eckmann-Hilton.gif
--rw-r--r--   0 boldi      (502) staff       (20)    12008 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/EckmannHilton.gif
--rw-r--r--   0 boldi      (502) staff       (20)     3504 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/arrow-example.png
--rw-r--r--   0 boldi      (502) staff       (20)     2166 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/box-example.png
--rw-r--r--   0 boldi      (502) staff       (20)    14662 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/bubble-example.png
--rw-r--r--   0 boldi      (502) staff       (20)    10047 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-1.png
--rw-r--r--   0 boldi      (502) staff       (20)     7535 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-1a.png
--rw-r--r--   0 boldi      (502) staff       (20)     7221 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-1b.png
--rw-r--r--   0 boldi      (502) staff       (20)     4433 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-2.png
--rw-r--r--   0 boldi      (502) staff       (20)     7089 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/functor-example.png
--rw-r--r--   0 boldi      (502) staff       (20)     2617 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/id-example.png
--rw-r--r--   0 boldi      (502) staff       (20)   404531 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/spiral.gif
--rw-r--r--   0 boldi      (502) staff       (20)     2888 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/tensor-example.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.879771 discopy-1.1.3/docs/_static/optics/
--rw-r--r--   0 boldi      (502) staff       (20)     7259 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/optics/fusion.png
--rw-r--r--   0 boldi      (502) staff       (20)    15302 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/optics/spider-decomp.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.880838 discopy-1.1.3/docs/_static/pivotal/
--rw-r--r--   0 boldi      (502) staff       (20)    10105 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/axiom.png
--rw-r--r--   0 boldi      (502) staff       (20)     6542 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/box-conjugate.png
--rw-r--r--   0 boldi      (502) staff       (20)     7722 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/conjugate.png
--rw-r--r--   0 boldi      (502) staff       (20)     6710 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/dagger-transpose.png
--rw-r--r--   0 boldi      (502) staff       (20)     8451 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/dagger.png
--rw-r--r--   0 boldi      (502) staff       (20)    10350 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/pivotal/trace.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.881216 discopy-1.1.3/docs/_static/quantum/
--rw-r--r--   0 boldi      (502) staff       (20)    13104 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/quantum/circuit-example.png
--rw-r--r--   0 boldi      (502) staff       (20)    17758 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/quantum/functor-example.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.881535 discopy-1.1.3/docs/_static/ribbon/
--rw-r--r--   0 boldi      (502) staff       (20)     6787 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/ribbon/strict.png
--rw-r--r--   0 boldi      (502) staff       (20)    15078 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/ribbon/twist-untwist.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.883087 discopy-1.1.3/docs/_static/rigid/
--rw-r--r--   0 boldi      (502) staff       (20)     2296 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/cap.png
--rw-r--r--   0 boldi      (502) staff       (20)     3223 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/caps.png
--rw-r--r--   0 boldi      (502) staff       (20)     2352 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/cup.png
--rw-r--r--   0 boldi      (502) staff       (20)     3131 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/cups.png
--rw-r--r--   0 boldi      (502) staff       (20)     8834 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/curry.png
--rw-r--r--   0 boldi      (502) staff       (20)     4537 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/diagram-example.png
--rw-r--r--   0 boldi      (502) staff       (20)    10267 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/functor-example.png
--rw-r--r--   0 boldi      (502) staff       (20)    11845 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/rotate.png
--rw-r--r--   0 boldi      (502) staff       (20)     9160 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/transpose.png
--rw-r--r--   0 boldi      (502) staff       (20)    13976 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/transpose_box.png
--rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/typed-snake-equation.png
--rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/snake-equation.png
--rw-r--r--   0 boldi      (502) staff       (20)   963196 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/spiral.gif
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.883800 discopy-1.1.3/docs/_static/symmetric/
--rw-r--r--   0 boldi      (502) staff       (20)    13136 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/decorator.png
--rw-r--r--   0 boldi      (502) staff       (20)     9819 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/hexagons.png
--rw-r--r--   0 boldi      (502) staff       (20)     6665 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/inverse.png
--rw-r--r--   0 boldi      (502) staff       (20)     7307 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/naturality.png
--rw-r--r--   0 boldi      (502) staff       (20)    10124 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/yang-baxter.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.884570 discopy-1.1.3/docs/_static/tensor/
--rw-r--r--   0 boldi      (502) staff       (20)    17466 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/chain-rule.png
--rw-r--r--   0 boldi      (502) staff       (20)     4810 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/frobenius-example.png
--rw-r--r--   0 boldi      (502) staff       (20)    10998 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/men-are-mortal.png
--rw-r--r--   0 boldi      (502) staff       (20)     9312 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/product-rule.png
--rw-r--r--   0 boldi      (502) staff       (20)    13435 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/rewrite.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.885914 discopy-1.1.3/docs/_static/traced/
--rw-r--r--   0 boldi      (502) staff       (20)    10121 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/golden.png
--rw-r--r--   0 boldi      (502) staff       (20)    10550 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/traced/right-nat-trace.png
--rw-r--r--   0 boldi      (502) staff       (20)     9691 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/sliding-left.png
--rw-r--r--   0 boldi      (502) staff       (20)     9887 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/sliding-right.png
--rw-r--r--   0 boldi      (502) staff       (20)    10411 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/tightening-left.png
--rw-r--r--   0 boldi      (502) staff       (20)    10550 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/tightening-right.png
--rw-r--r--   0 boldi      (502) staff       (20)    10247 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/trace.png
--rw-r--r--   0 boldi      (502) staff       (20)    12964 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/yanking.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.886065 discopy-1.1.3/docs/_style/
--rw-r--r--   0 boldi      (502) staff       (20)     1811 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_style/custom.css
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.886661 discopy-1.1.3/docs/_templates/
--rw-r--r--   0 boldi      (502) staff       (20)      185 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_templates/class.rst
--rw-r--r--   0 boldi      (502) staff       (20)      100 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_templates/function.rst
--rw-r--r--   0 boldi      (502) staff       (20)       66 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_templates/module.rst
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.888071 discopy-1.1.3/docs/api/
--rw-r--r--   0 boldi      (502) staff       (20)     4581 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/architecture.html
--rw-r--r--   0 boldi      (502) staff       (20)    56460 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/architecture.png
--rw-r--r--   0 boldi      (502) staff       (20)      168 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/drawing.rst
--rw-r--r--   0 boldi      (502) staff       (20)      256 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/grammar.rst
--rw-r--r--   0 boldi      (502) staff       (20)      302 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/quantum.rst
--rw-r--r--   0 boldi      (502) staff       (20)      222 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/semantics.rst
--rw-r--r--   0 boldi      (502) staff       (20)      458 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/syntax.rst
--rw-r--r--   0 boldi      (502) staff       (20)     3037 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/conf.py
--rw-r--r--   0 boldi      (502) staff       (20)    13274 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/discopy.bib
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.888892 discopy-1.1.3/docs/extra/
--rw-r--r--   0 boldi      (502) staff       (20)       57 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/bibliography.rst
--rw-r--r--   0 boldi      (502) staff       (20)     1059 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/blogs.md
--rw-r--r--   0 boldi      (502) staff       (20)     6077 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/papers.md
--rw-r--r--   0 boldi      (502) staff       (20)     1492 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/talks.rst
--rw-r--r--   0 boldi      (502) staff       (20)      780 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/index.rst
--rw-r--r--   0 boldi      (502) staff       (20)      795 2022-09-27 14:39:16.000000 discopy-1.1.3/docs/make.bat
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.894522 discopy-1.1.3/docs/notebooks/
--rw-r--r--   0 boldi      (502) staff       (20)   483325 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/21-05-03-tallcat.ipynb
--rw-r--r--   0 boldi      (502) staff       (20)  1593241 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/21-05-05-tallcat.ipynb
--rw-r--r--   0 boldi      (502) staff       (20)    42815 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/diag-diff.ipynb
--rw-r--r--   0 boldi      (502) staff       (20)   179435 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/diagrams.ipynb
--rw-r--r--   0 boldi      (502) staff       (20)   185975 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/notebooks/qnlp.ipynb
--rw-r--r--   0 boldi      (502) staff       (20)     2203 2023-06-01 11:23:16.000000 discopy-1.1.3/pyproject.toml
--rw-r--r--   0 boldi      (502) staff       (20)       38 2023-06-01 18:45:51.908779 discopy-1.1.3/setup.cfg
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.851771 discopy-1.1.3/test/
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.894795 discopy-1.1.3/test/drawing/
--rw-r--r--   0 boldi      (502) staff       (20)     5573 2023-05-31 13:42:21.000000 discopy-1.1.3/test/drawing/legacy.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.896447 discopy-1.1.3/test/grammar/
--rw-r--r--   0 boldi      (502) staff       (20)     7785 2023-05-31 13:57:44.000000 discopy-1.1.3/test/grammar/categorial.py
--rw-r--r--   0 boldi      (502) staff       (20)     2049 2023-05-31 09:22:59.000000 discopy-1.1.3/test/grammar/pregroup.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.898211 discopy-1.1.3/test/quantum/
--rw-r--r--   0 boldi      (502) staff       (20)      425 2023-05-31 09:22:59.000000 discopy-1.1.3/test/quantum/ansatze.py
--rw-r--r--   0 boldi      (502) staff       (20)     1553 2023-05-31 13:42:16.000000 discopy-1.1.3/test/quantum/channel.py
--rw-r--r--   0 boldi      (502) staff       (20)    25072 2023-05-31 13:59:33.000000 discopy-1.1.3/test/quantum/circuit.py
--rw-r--r--   0 boldi      (502) staff       (20)     2510 2023-05-31 09:22:59.000000 discopy-1.1.3/test/quantum/eval.py
--rw-r--r--   0 boldi      (502) staff       (20)     4335 2023-06-01 10:54:48.000000 discopy-1.1.3/test/quantum/tk.py
--rw-r--r--   0 boldi      (502) staff       (20)     5804 2023-05-31 09:22:59.000000 discopy-1.1.3/test/quantum/zx.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.899100 discopy-1.1.3/test/semantics/
--rw-r--r--   0 boldi      (502) staff       (20)     1203 2023-05-31 13:41:31.000000 discopy-1.1.3/test/semantics/matrix.py
--rw-r--r--   0 boldi      (502) staff       (20)     1304 2023-05-31 09:22:59.000000 discopy-1.1.3/test/semantics/python.py
--rw-r--r--   0 boldi      (502) staff       (20)     8107 2023-05-31 13:41:42.000000 discopy-1.1.3/test/semantics/tensor.py
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.899716 discopy-1.1.3/test/src/
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.902144 discopy-1.1.3/test/src/imgs/
--rw-r--r--   0 boldi      (502) staff       (20)    12008 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/EckmannHilton.gif
--rw-r--r--   0 boldi      (502) staff       (20)     7553 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/bell-state.png
--rw-r--r--   0 boldi      (502) staff       (20)    16964 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/bialgebra.png
--rw-r--r--   0 boldi      (502) staff       (20)    25004 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/crack-eggs.png
--rw-r--r--   0 boldi      (502) staff       (20)     2411 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/empty_diagram.png
--rw-r--r--   0 boldi      (502) staff       (20)     5907 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/long-controlled.png
--rw-r--r--   0 boldi      (502) staff       (20)     8810 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/sentence-as-diagram.png
--rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/snake-equation.png
--rw-r--r--   0 boldi      (502) staff       (20)    10800 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/spiral.png
--rw-r--r--   0 boldi      (502) staff       (20)     6051 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/typed-snake-equation.png
--rw-r--r--   0 boldi      (502) staff       (20)     9525 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/who-ansatz.png
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.904465 discopy-1.1.3/test/src/tikz/
--rw-r--r--   0 boldi      (502) staff       (20)     2228 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bell-state.tikz
--rw-r--r--   0 boldi      (502) staff       (20)      153 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bell-state.tikzstyles
--rw-r--r--   0 boldi      (502) staff       (20)     4906 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bialgebra.tikz
--rw-r--r--   0 boldi      (502) staff       (20)      150 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bialgebra.tikzstyles
--rw-r--r--   0 boldi      (502) staff       (20)     2441 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/copy.tikz
--rw-r--r--   0 boldi      (502) staff       (20)       86 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/copy.tikzstyles
--rw-r--r--   0 boldi      (502) staff       (20)     3441 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/crack-eggs.tikz
--rw-r--r--   0 boldi      (502) staff       (20)     3338 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/long-controlled.tikz
--rw-r--r--   0 boldi      (502) staff       (20)     2223 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/snake-equation.tikz
--rw-r--r--   0 boldi      (502) staff       (20)     1906 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/spiral.tikz
--rw-r--r--   0 boldi      (502) staff       (20)      260 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/spiral.tikzstyles
--rw-r--r--   0 boldi      (502) staff       (20)     3435 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/who-ansatz.tikz
--rw-r--r--   0 boldi      (502) staff       (20)    15562 2022-09-27 14:39:16.000000 discopy-1.1.3/test/src/tree2diagram.pickle
--rw-r--r--   0 boldi      (502) staff       (20)     6324 2022-09-27 14:39:16.000000 discopy-1.1.3/test/src/zx-graph.json
-drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.908131 discopy-1.1.3/test/syntax/
--rw-r--r--   0 boldi      (502) staff       (20)      258 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/balanced.py
--rw-r--r--   0 boldi      (502) staff       (20)      487 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/braided.py
--rw-r--r--   0 boldi      (502) staff       (20)     7687 2023-05-31 13:45:46.000000 discopy-1.1.3/test/syntax/cat.py
--rw-r--r--   0 boldi      (502) staff       (20)     1413 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/closed.py
--rw-r--r--   0 boldi      (502) staff       (20)      828 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/compact.py
--rw-r--r--   0 boldi      (502) staff       (20)     1750 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/frobenius.py
--rw-r--r--   0 boldi      (502) staff       (20)     2044 2023-06-01 18:42:50.000000 discopy-1.1.3/test/syntax/hypergraph.py
--rw-r--r--   0 boldi      (502) staff       (20)      659 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/interaction.py
--rw-r--r--   0 boldi      (502) staff       (20)     1532 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/markov.py
--rw-r--r--   0 boldi      (502) staff       (20)    10196 2023-05-31 13:50:28.000000 discopy-1.1.3/test/syntax/monoidal.py
--rw-r--r--   0 boldi      (502) staff       (20)      178 2023-05-31 13:40:18.000000 discopy-1.1.3/test/syntax/pivotal.py
--rw-r--r--   0 boldi      (502) staff       (20)      553 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/ribbon.py
--rw-r--r--   0 boldi      (502) staff       (20)     3278 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/rigid.py
--rw-r--r--   0 boldi      (502) staff       (20)      962 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/symmetric.py
--rw-r--r--   0 boldi      (502) staff       (20)      391 2023-05-31 13:58:46.000000 discopy-1.1.3/test/syntax/traced.py
--rw-r--r--   0 boldi      (502) staff       (20)      953 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/utils.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.129493 discopy-1.1.4/
+-rw-r--r--   0 boldi      (502) staff       (20)       33 2022-09-27 14:39:16.000000 discopy-1.1.4/.gitattributes
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.909112 discopy-1.1.4/.github/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.914369 discopy-1.1.4/.github/workflows/
+-rw-r--r--   0 boldi      (502) staff       (20)     1714 2023-06-22 11:13:31.000000 discopy-1.1.4/.github/workflows/build_test.yml
+-rw-r--r--   0 boldi      (502) staff       (20)      183 2023-06-22 11:13:31.000000 discopy-1.1.4/.gitignore
+-rw-r--r--   0 boldi      (502) staff       (20)    20606 2023-06-22 11:13:31.000000 discopy-1.1.4/.pylintrc
+-rw-r--r--   0 boldi      (502) staff       (20)      744 2023-06-22 11:13:31.000000 discopy-1.1.4/.readthedocs.yaml
+-rw-r--r--   0 boldi      (502) staff       (20)     1350 2023-06-22 11:13:31.000000 discopy-1.1.4/CONTRIBUTING.md
+-rw-r--r--   0 boldi      (502) staff       (20)     1520 2023-06-22 11:13:31.000000 discopy-1.1.4/LICENSE
+-rw-r--r--   0 boldi      (502) staff       (20)     7395 2023-06-22 11:15:43.129028 discopy-1.1.4/PKG-INFO
+-rw-r--r--   0 boldi      (502) staff       (20)     4542 2023-06-22 11:13:31.000000 discopy-1.1.4/README.md
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.918781 discopy-1.1.4/discopy/
+-rw-r--r--   0 boldi      (502) staff       (20)      499 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)     5758 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/balanced.py
+-rw-r--r--   0 boldi      (502) staff       (20)     8305 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/braided.py
+-rw-r--r--   0 boldi      (502) staff       (20)    28162 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/cat.py
+-rw-r--r--   0 boldi      (502) staff       (20)    10172 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/closed.py
+-rw-r--r--   0 boldi      (502) staff       (20)     4513 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/compact.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1487 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/config.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.919963 discopy-1.1.4/discopy/drawing/
+-rw-r--r--   0 boldi      (502) staff       (20)     1060 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/drawing/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)    13859 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/drawing/grid.py
+-rw-r--r--   0 boldi      (502) staff       (20)    36817 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/drawing/legacy.py
+-rw-r--r--   0 boldi      (502) staff       (20)    11666 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/frobenius.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.921166 discopy-1.1.4/discopy/grammar/
+-rw-r--r--   0 boldi      (502) staff       (20)      225 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/grammar/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)     9422 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/grammar/categorial.py
+-rw-r--r--   0 boldi      (502) staff       (20)     6950 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/grammar/cfg.py
+-rw-r--r--   0 boldi      (502) staff       (20)      926 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/grammar/dependency.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7191 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/grammar/pregroup.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2424 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/grammar/thue.py
+-rw-r--r--   0 boldi      (502) staff       (20)    48238 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/hypergraph.py
+-rw-r--r--   0 boldi      (502) staff       (20)    14080 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/interaction.py
+-rw-r--r--   0 boldi      (502) staff       (20)     8157 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/markov.py
+-rw-r--r--   0 boldi      (502) staff       (20)    16161 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/matrix.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1555 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/messages.py
+-rw-r--r--   0 boldi      (502) staff       (20)    35290 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/monoidal.py
+-rw-r--r--   0 boldi      (502) staff       (20)     6871 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/pivotal.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7845 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/python.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.924588 discopy-1.1.4/discopy/quantum/
+-rw-r--r--   0 boldi      (502) staff       (20)      667 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/quantum/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)     5238 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/quantum/ansatze.py
+-rw-r--r--   0 boldi      (502) staff       (20)    11626 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/quantum/channel.py
+-rw-r--r--   0 boldi      (502) staff       (20)    33003 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/quantum/circuit.py
+-rw-r--r--   0 boldi      (502) staff       (20)    24713 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/quantum/gates.py
+-rw-r--r--   0 boldi      (502) staff       (20)    16262 2023-06-22 11:13:36.000000 discopy-1.1.4/discopy/quantum/pennylane.py
+-rw-r--r--   0 boldi      (502) staff       (20)    16429 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/quantum/tk.py
+-rw-r--r--   0 boldi      (502) staff       (20)    13451 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/quantum/zx.py
+-rw-r--r--   0 boldi      (502) staff       (20)     6916 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/ribbon.py
+-rw-r--r--   0 boldi      (502) staff       (20)    25755 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/rigid.py
+-rw-r--r--   0 boldi      (502) staff       (20)     9969 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/symmetric.py
+-rw-r--r--   0 boldi      (502) staff       (20)    23157 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/tensor.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7707 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/traced.py
+-rw-r--r--   0 boldi      (502) staff       (20)    20763 2023-06-22 11:13:31.000000 discopy-1.1.4/discopy/utils.py
+-rw-r--r--   0 boldi      (502) staff       (20)      160 2023-06-22 11:15:42.000000 discopy-1.1.4/discopy/version.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.919453 discopy-1.1.4/discopy.egg-info/
+-rw-r--r--   0 boldi      (502) staff       (20)     7395 2023-06-22 11:15:42.000000 discopy-1.1.4/discopy.egg-info/PKG-INFO
+-rw-r--r--   0 boldi      (502) staff       (20)     6574 2023-06-22 11:15:42.000000 discopy-1.1.4/discopy.egg-info/SOURCES.txt
+-rw-r--r--   0 boldi      (502) staff       (20)        1 2023-06-22 11:15:42.000000 discopy-1.1.4/discopy.egg-info/dependency_links.txt
+-rw-r--r--   0 boldi      (502) staff       (20)      424 2023-06-22 11:15:42.000000 discopy-1.1.4/discopy.egg-info/requires.txt
+-rw-r--r--   0 boldi      (502) staff       (20)        8 2023-06-22 11:15:42.000000 discopy-1.1.4/discopy.egg-info/top_level.txt
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.929581 discopy-1.1.4/docs/
+-rw-r--r--   0 boldi      (502) staff       (20)      634 2022-09-27 14:39:16.000000 discopy-1.1.4/docs/Makefile
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.931589 discopy-1.1.4/docs/_ext/
+-rw-r--r--   0 boldi      (502) staff       (20)      684 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_ext/bases-fullname.py
+-rw-r--r--   0 boldi      (502) staff       (20)     3939 2022-12-13 17:02:09.000000 discopy-1.1.4/docs/_ext/youtube.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.935217 discopy-1.1.4/docs/_static/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.939398 discopy-1.1.4/docs/_static/balanced/
+-rw-r--r--   0 boldi      (502) staff       (20)    14901 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/balanced/ribbon_twist.png
+-rw-r--r--   0 boldi      (502) staff       (20)    13367 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/balanced/twist.png
+-rw-r--r--   0 boldi      (502) staff       (20)    11712 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/balanced/twist_dual_rail.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.941223 discopy-1.1.4/docs/_static/braided/
+-rw-r--r--   0 boldi      (502) staff       (20)     8951 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/braided/hexagons.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9432 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/braided/inverse.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.943916 discopy-1.1.4/docs/_static/closed/
+-rw-r--r--   0 boldi      (502) staff       (20)    15711 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/closed/curry-left.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15643 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/closed/curry-right.png
+-rw-r--r--   0 boldi      (502) staff       (20)    19051 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/closed/uncurry.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.947580 discopy-1.1.4/docs/_static/compact/
+-rw-r--r--   0 boldi      (502) staff       (20)    14358 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/compact/reidemeister.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10190 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/compact/snake.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14358 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/compact/yanking.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14061 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/compact/yanking_cup_and_cap.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.950428 discopy-1.1.4/docs/_static/drawing/
+-rw-r--r--   0 boldi      (502) staff       (20)     5271 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/drawing/diagramize.png
+-rw-r--r--   0 boldi      (502) staff       (20)     3578 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/drawing/example.html
+-rw-r--r--   0 boldi      (502) staff       (20)    10626 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/drawing/frobenius-axioms.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.954183 discopy-1.1.4/docs/_static/frobenius/
+-rw-r--r--   0 boldi      (502) staff       (20)    17147 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/frobenius/comonoid.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14853 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/frobenius/frobenius.png
+-rw-r--r--   0 boldi      (502) staff       (20)    17266 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/frobenius/monoid.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9884 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/frobenius/special.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.955953 discopy-1.1.4/docs/_static/grammar/
+-rw-r--r--   0 boldi      (502) staff       (20)     9591 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/grammar/cfg-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7224 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/grammar/pregroup-example.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.958695 discopy-1.1.4/docs/_static/hypergraph/
+-rw-r--r--   0 boldi      (502) staff       (20)    16894 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/hypergraph/box.png
+-rw-r--r--   0 boldi      (502) staff       (20)    20670 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/hypergraph/diagram.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15394 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/hypergraph/unfuse.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.966980 discopy-1.1.4/docs/_static/int/
+-rw-r--r--   0 boldi      (502) staff       (20)    16145 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/alice-loves-bob.png
+-rw-r--r--   0 boldi      (502) staff       (20)    18363 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/braid.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16332 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/composition.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8274 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/dagger.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16257 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/idl.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16615 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/idr.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16069 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/int-snake-equations.png
+-rw-r--r--   0 boldi      (502) staff       (20)    22712 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/simplify.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16278 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/int/tensor.png
+-rw-r--r--   0 boldi      (502) staff       (20)   105662 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/logo.ico
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.970672 discopy-1.1.4/docs/_static/markov/
+-rw-r--r--   0 boldi      (502) staff       (20)    13158 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/markov/associativity.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14407 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/markov/bialgebra.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10317 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/markov/copy_and_apply.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8979 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/markov/counit.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.982756 discopy-1.1.4/docs/_static/monoidal/
+-rw-r--r--   0 boldi      (502) staff       (20)     2875 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/Eckmann-Hilton.gif
+-rw-r--r--   0 boldi      (502) staff       (20)    12008 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/EckmannHilton.gif
+-rw-r--r--   0 boldi      (502) staff       (20)     3504 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/arrow-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2166 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/box-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14662 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/bubble-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10047 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/foliate-example-1.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7535 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/foliate-example-1a.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7221 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/foliate-example-1b.png
+-rw-r--r--   0 boldi      (502) staff       (20)     4433 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/foliate-example-2.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7089 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/functor-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2617 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/id-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)   404531 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/spiral.gif
+-rw-r--r--   0 boldi      (502) staff       (20)     2888 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/monoidal/tensor-example.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.984574 discopy-1.1.4/docs/_static/optics/
+-rw-r--r--   0 boldi      (502) staff       (20)     7259 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/optics/fusion.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15302 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/optics/spider-decomp.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.989896 discopy-1.1.4/docs/_static/pivotal/
+-rw-r--r--   0 boldi      (502) staff       (20)    10105 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/pivotal/axiom.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6542 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/pivotal/box-conjugate.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7722 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/pivotal/conjugate.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6710 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/pivotal/dagger-transpose.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8451 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/pivotal/dagger.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10350 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/pivotal/trace.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.991619 discopy-1.1.4/docs/_static/quantum/
+-rw-r--r--   0 boldi      (502) staff       (20)    13104 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/quantum/circuit-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    17758 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/quantum/functor-example.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.993406 discopy-1.1.4/docs/_static/ribbon/
+-rw-r--r--   0 boldi      (502) staff       (20)     6787 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/ribbon/strict.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15078 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/ribbon/twist-untwist.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.003195 discopy-1.1.4/docs/_static/rigid/
+-rw-r--r--   0 boldi      (502) staff       (20)     2296 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/cap.png
+-rw-r--r--   0 boldi      (502) staff       (20)     3223 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/caps.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2352 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/cup.png
+-rw-r--r--   0 boldi      (502) staff       (20)     3131 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/cups.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8834 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/curry.png
+-rw-r--r--   0 boldi      (502) staff       (20)     4537 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/diagram-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10267 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/functor-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    11845 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/rotate.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9160 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/transpose.png
+-rw-r--r--   0 boldi      (502) staff       (20)    13976 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/transpose_box.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/rigid/typed-snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)   963196 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/spiral.gif
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.007936 discopy-1.1.4/docs/_static/symmetric/
+-rw-r--r--   0 boldi      (502) staff       (20)    13136 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/symmetric/decorator.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9819 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/symmetric/hexagons.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6665 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/symmetric/inverse.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7307 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/symmetric/naturality.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10124 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/symmetric/yang-baxter.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.012813 discopy-1.1.4/docs/_static/tensor/
+-rw-r--r--   0 boldi      (502) staff       (20)    17466 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/tensor/chain-rule.png
+-rw-r--r--   0 boldi      (502) staff       (20)     4810 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/tensor/frobenius-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10998 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/tensor/men-are-mortal.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9312 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/tensor/product-rule.png
+-rw-r--r--   0 boldi      (502) staff       (20)    13435 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/tensor/rewrite.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.019994 discopy-1.1.4/docs/_static/traced/
+-rw-r--r--   0 boldi      (502) staff       (20)    10121 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/golden.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10550 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/right-nat-trace.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9691 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/sliding-left.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9887 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/sliding-right.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10411 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/tightening-left.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10550 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/tightening-right.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10247 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/trace.png
+-rw-r--r--   0 boldi      (502) staff       (20)    12964 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_static/traced/yanking.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.020904 discopy-1.1.4/docs/_style/
+-rw-r--r--   0 boldi      (502) staff       (20)     1811 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/_style/custom.css
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.023814 discopy-1.1.4/docs/_templates/
+-rw-r--r--   0 boldi      (502) staff       (20)      185 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/_templates/class.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      100 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/_templates/function.rst
+-rw-r--r--   0 boldi      (502) staff       (20)       66 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/_templates/module.rst
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.030101 discopy-1.1.4/docs/api/
+-rw-r--r--   0 boldi      (502) staff       (20)     4581 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/api/architecture.html
+-rw-r--r--   0 boldi      (502) staff       (20)    56460 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/api/architecture.png
+-rw-r--r--   0 boldi      (502) staff       (20)      168 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/api/drawing.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      256 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/api/grammar.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      302 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/api/quantum.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      222 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/api/semantics.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      458 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/api/syntax.rst
+-rw-r--r--   0 boldi      (502) staff       (20)     3233 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/conf.py
+-rw-r--r--   0 boldi      (502) staff       (20)    13274 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/discopy.bib
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.033558 discopy-1.1.4/docs/extra/
+-rw-r--r--   0 boldi      (502) staff       (20)       57 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/extra/bibliography.rst
+-rw-r--r--   0 boldi      (502) staff       (20)     1063 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/extra/blogs.md
+-rw-r--r--   0 boldi      (502) staff       (20)     6001 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/extra/papers.md
+-rw-r--r--   0 boldi      (502) staff       (20)     1507 2023-06-15 16:31:52.000000 discopy-1.1.4/docs/extra/talks.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      844 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/index.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      795 2022-09-27 14:39:16.000000 discopy-1.1.4/docs/make.bat
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.041768 discopy-1.1.4/docs/notebooks/
+-rw-r--r--   0 boldi      (502) staff       (20)   483325 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/notebooks/21-05-03-tallcat.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)  1593241 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/notebooks/21-05-05-tallcat.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)    42815 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/notebooks/diag-diff.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)   179435 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/notebooks/diagrams.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)   185975 2023-06-22 11:13:31.000000 discopy-1.1.4/docs/notebooks/qnlp.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)     2210 2023-06-22 11:13:31.000000 discopy-1.1.4/pyproject.toml
+-rw-r--r--   0 boldi      (502) staff       (20)       38 2023-06-22 11:15:43.129828 discopy-1.1.4/setup.cfg
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:42.912554 discopy-1.1.4/test/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.043878 discopy-1.1.4/test/drawing/
+-rw-r--r--   0 boldi      (502) staff       (20)     5573 2023-06-22 11:13:31.000000 discopy-1.1.4/test/drawing/legacy.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.047061 discopy-1.1.4/test/grammar/
+-rw-r--r--   0 boldi      (502) staff       (20)     7785 2023-06-22 11:13:31.000000 discopy-1.1.4/test/grammar/categorial.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2049 2023-06-22 11:13:31.000000 discopy-1.1.4/test/grammar/pregroup.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.056980 discopy-1.1.4/test/quantum/
+-rw-r--r--   0 boldi      (502) staff       (20)      425 2023-06-22 11:13:31.000000 discopy-1.1.4/test/quantum/ansatze.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1553 2023-06-22 11:13:31.000000 discopy-1.1.4/test/quantum/channel.py
+-rw-r--r--   0 boldi      (502) staff       (20)    25389 2023-06-22 11:13:36.000000 discopy-1.1.4/test/quantum/circuit.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2510 2023-06-22 11:13:31.000000 discopy-1.1.4/test/quantum/eval.py
+-rw-r--r--   0 boldi      (502) staff       (20)     4335 2023-06-22 11:13:31.000000 discopy-1.1.4/test/quantum/tk.py
+-rw-r--r--   0 boldi      (502) staff       (20)     5804 2023-06-22 11:13:31.000000 discopy-1.1.4/test/quantum/zx.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.061732 discopy-1.1.4/test/semantics/
+-rw-r--r--   0 boldi      (502) staff       (20)     1203 2023-06-22 11:13:31.000000 discopy-1.1.4/test/semantics/matrix.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1304 2023-06-22 11:13:31.000000 discopy-1.1.4/test/semantics/python.py
+-rw-r--r--   0 boldi      (502) staff       (20)     8107 2023-06-22 11:13:31.000000 discopy-1.1.4/test/semantics/tensor.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.065013 discopy-1.1.4/test/src/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.082689 discopy-1.1.4/test/src/imgs/
+-rw-r--r--   0 boldi      (502) staff       (20)    12008 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/EckmannHilton.gif
+-rw-r--r--   0 boldi      (502) staff       (20)     7553 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/bell-state.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16964 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/bialgebra.png
+-rw-r--r--   0 boldi      (502) staff       (20)    25004 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/crack-eggs.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2411 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/empty_diagram.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5907 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/long-controlled.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8810 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/sentence-as-diagram.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10800 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/spiral.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6051 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/typed-snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9525 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/imgs/who-ansatz.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.101646 discopy-1.1.4/test/src/tikz/
+-rw-r--r--   0 boldi      (502) staff       (20)     2228 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/bell-state.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)      153 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/bell-state.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     4906 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/bialgebra.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)      150 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/bialgebra.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     2441 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/copy.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)       86 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/copy.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     3441 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/crack-eggs.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)     3338 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/long-controlled.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)     2223 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/snake-equation.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)     1906 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/spiral.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)      260 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/spiral.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     3435 2023-06-22 11:13:31.000000 discopy-1.1.4/test/src/tikz/who-ansatz.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)    15562 2022-09-27 14:39:16.000000 discopy-1.1.4/test/src/tree2diagram.pickle
+-rw-r--r--   0 boldi      (502) staff       (20)     6324 2022-09-27 14:39:16.000000 discopy-1.1.4/test/src/zx-graph.json
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-22 11:15:43.127297 discopy-1.1.4/test/syntax/
+-rw-r--r--   0 boldi      (502) staff       (20)      258 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/balanced.py
+-rw-r--r--   0 boldi      (502) staff       (20)      487 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/braided.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7687 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/cat.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1413 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/closed.py
+-rw-r--r--   0 boldi      (502) staff       (20)      828 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/compact.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1750 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/frobenius.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2044 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/hypergraph.py
+-rw-r--r--   0 boldi      (502) staff       (20)      659 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/interaction.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1532 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/markov.py
+-rw-r--r--   0 boldi      (502) staff       (20)    10196 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/monoidal.py
+-rw-r--r--   0 boldi      (502) staff       (20)      178 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/pivotal.py
+-rw-r--r--   0 boldi      (502) staff       (20)      553 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/ribbon.py
+-rw-r--r--   0 boldi      (502) staff       (20)     3278 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/rigid.py
+-rw-r--r--   0 boldi      (502) staff       (20)      962 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/symmetric.py
+-rw-r--r--   0 boldi      (502) staff       (20)      391 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/traced.py
+-rw-r--r--   0 boldi      (502) staff       (20)      953 2023-06-22 11:13:31.000000 discopy-1.1.4/test/syntax/utils.py
```

### Comparing `discopy-1.1.3/.github/workflows/build_test.yml` & `discopy-1.1.4/.github/workflows/build_test.yml`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/.pylintrc` & `discopy-1.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/.readthedocs.yaml` & `discopy-1.1.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/CONTRIBUTING.md` & `discopy-1.1.4/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,9 @@
 ```shell
 pip install twine
 git tag X.X.X
 git push origin --tags
 python -m build
 twine upload dist/*
 ```
+
+Finally, [create a release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository#creating-a-release) for the newly created tag.
```

### Comparing `discopy-1.1.3/LICENSE` & `discopy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/PKG-INFO` & `discopy-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.1.3
+Version: 1.1.4
 Summary: The Python toolkit for computing with string diagrams.
 Author: DisCoPy
 Author-email: contact@discopy.org
 License: BSD 3-Clause License
         
         Copyright (c) 2019-2022, DisCoPy
         All rights reserved.
@@ -63,19 +63,19 @@
 [![build](https://github.com/discopy/discopy/actions/workflows/build_test.yml/badge.svg)](https://github.com/discopy/discopy/actions/workflows/build_test.yml)
 [![readthedocs](https://readthedocs.org/projects/discopy/badge/?version=main)](https://docs.discopy.org/)
 [![PyPI version](https://badge.fury.io/py/discopy.svg)](https://badge.fury.io/py/discopy)
 [![DOI: 10.4204/EPTCS.333.13](http://img.shields.io/badge/DOI-10.4204/EPTCS.333.13-brightgreen.svg)](https://doi.org/10.4204/EPTCS.333.13)
 
 DisCoPy is a Python toolkit for computing with [string diagrams](https://en.wikipedia.org/wiki/String_diagram).
 
-* **Organisation:** https://discopy.org
-* **Documentation:** https://docs.discopy.org
-* **Source code:** https://github.com/discopy/discopy
-* **Paper (for applied category theorists):** https://doi.org/10.4204/EPTCS.333.13
-* **Paper (for quantum computer scientists):** https://arxiv.org/abs/2205.05190
+* **Organisation:** <https://discopy.org>
+* **Documentation:** <https://docs.discopy.org>
+* **Source code:** <https://github.com/discopy/discopy>
+* **Paper (for applied category theorists):** <https://doi.org/10.4204/EPTCS.333.13>
+* **Paper (for quantum computer scientists):** <https://arxiv.org/abs/2205.05190>
 
 DisCoPy began as an implementation of [DisCoCat](https://en.wikipedia.org/wiki/DisCoCat) and [QNLP](https://en.wikipedia.org/wiki/Quantum_natural_language_processing). This has now become its own library: [lambeq](https://cqcl.github.io/lambeq).
 
 ## Features
 
 * an `Arrow` data structure for free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
 * a `Diagram` data structure for planar string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (with braids, twists, spiders, etc.)
```

### Comparing `discopy-1.1.3/README.md` & `discopy-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 [![build](https://github.com/discopy/discopy/actions/workflows/build_test.yml/badge.svg)](https://github.com/discopy/discopy/actions/workflows/build_test.yml)
 [![readthedocs](https://readthedocs.org/projects/discopy/badge/?version=main)](https://docs.discopy.org/)
 [![PyPI version](https://badge.fury.io/py/discopy.svg)](https://badge.fury.io/py/discopy)
 [![DOI: 10.4204/EPTCS.333.13](http://img.shields.io/badge/DOI-10.4204/EPTCS.333.13-brightgreen.svg)](https://doi.org/10.4204/EPTCS.333.13)
 
 DisCoPy is a Python toolkit for computing with [string diagrams](https://en.wikipedia.org/wiki/String_diagram).
 
-* **Organisation:** https://discopy.org
-* **Documentation:** https://docs.discopy.org
-* **Source code:** https://github.com/discopy/discopy
-* **Paper (for applied category theorists):** https://doi.org/10.4204/EPTCS.333.13
-* **Paper (for quantum computer scientists):** https://arxiv.org/abs/2205.05190
+* **Organisation:** <https://discopy.org>
+* **Documentation:** <https://docs.discopy.org>
+* **Source code:** <https://github.com/discopy/discopy>
+* **Paper (for applied category theorists):** <https://doi.org/10.4204/EPTCS.333.13>
+* **Paper (for quantum computer scientists):** <https://arxiv.org/abs/2205.05190>
 
 DisCoPy began as an implementation of [DisCoCat](https://en.wikipedia.org/wiki/DisCoCat) and [QNLP](https://en.wikipedia.org/wiki/Quantum_natural_language_processing). This has now become its own library: [lambeq](https://cqcl.github.io/lambeq).
 
 ## Features
 
 * an `Arrow` data structure for free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
 * a `Diagram` data structure for planar string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (with braids, twists, spiders, etc.)
```

### Comparing `discopy-1.1.3/discopy/balanced.py` & `discopy-1.1.4/discopy/balanced.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/braided.py` & `discopy-1.1.4/discopy/braided.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/cat.py` & `discopy-1.1.4/discopy/cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     Box
     Id
     Sum
     Bubble
     Category
     Functor
     Composable
-    AxiomError
 
 .. admonition:: Functions
 
     .. autosummary::
         :template: function.rst
         :nosignatures:
         :toctree:
```

### Comparing `discopy-1.1.3/discopy/closed.py` & `discopy-1.1.4/discopy/closed.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/compact.py` & `discopy-1.1.4/discopy/compact.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/config.py` & `discopy-1.1.4/discopy/config.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/drawing/__init__.py` & `discopy-1.1.4/discopy/drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/drawing/grid.py` & `discopy-1.1.4/discopy/drawing/grid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/drawing/legacy.py` & `discopy-1.1.4/discopy/drawing/legacy.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/frobenius.py` & `discopy-1.1.4/discopy/frobenius.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/grammar/categorial.py` & `discopy-1.1.4/discopy/grammar/categorial.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/grammar/cfg.py` & `discopy-1.1.4/discopy/grammar/cfg.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/grammar/dependency.py` & `discopy-1.1.4/discopy/grammar/dependency.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/grammar/pregroup.py` & `discopy-1.1.4/discopy/grammar/pregroup.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/grammar/thue.py` & `discopy-1.1.4/discopy/grammar/thue.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/hypergraph.py` & `discopy-1.1.4/discopy/hypergraph.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/interaction.py` & `discopy-1.1.4/discopy/interaction.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/markov.py` & `discopy-1.1.4/discopy/markov.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/matrix.py` & `discopy-1.1.4/discopy/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,16 @@
         backend
         set_backend
         get_backend
 
 See also
 --------
 
-* :class:`Tensor` is a subclass of :class:`Matrix` with the Kronecker product
-  as tensor.
-* :class:`Matrix` is used to evaluate :class:`quantum.optics.Diagram`.
+* :class:`discopy.tensor.Tensor` is a subclass of :class:`Matrix` with the
+  Kronecker product as tensor.
 
 """
 from __future__ import annotations
 
 from contextlib import contextmanager
 from types import ModuleType
 from typing import Union, Literal as L, Callable, TYPE_CHECKING
@@ -178,34 +177,35 @@
 
     def __eq__(self, other):
         return isinstance(other, self.factory)\
             and self.dtype == other.dtype\
             and (self.dom, self.cod) == (other.dom, other.cod)\
             and (self.array == other.array).all()
 
-    def is_close(self, other: Matrix, rtol=1.e-8, atol=1.e-8) -> bool:
+    def is_close(self, other: Matrix, rtol: float = 1.e-8, atol: float = 1.e-8
+                 ) -> bool:
         """
         Whether a matrix is numerically close to an ``other``.
 
         Parameters:
             other : The other matrix with which to check closeness.
-            rtol: float
-                    The relative tolerance parameter (see Notes).
-                    Default value for results of order unity is 1.e-5
-            atol : float
-                    The absolute tolerance parameter (see Notes).
-                    Default value for results of order unity is 1.e-8
+            rtol:
+                The relative tolerance parameter (see Notes).
+                Default value for results of order unity is 1.e-5
+            atol :
+                The absolute tolerance parameter (see Notes).
+                Default value for results of order unity is 1.e-8
 
         Notes:
-       (taken from np.isclose documentation)
+        (taken from np.isclose documentation)
 
             For finite values, isclose uses the following equation to
             test whether two floating point values are equivalent.
 
-             absolute(`a` - `b`) <= (`atol` + `rtol` * absolute(`b`))
+            absolute(`a` - `b`) <= (`atol` + `rtol` * absolute(`b`))
 
             Unlike the built-in `math.isclose`, the above equation is not
             symmetric in `a` and `b` -- it assumes `b` is the reference
             value -- so that `isclose(a, b)` might be different from
             `isclose(b, a)`.
 
             Furthermore, the default value of atol is not zero, and is used
```

### Comparing `discopy-1.1.3/discopy/messages.py` & `discopy-1.1.4/discopy/messages.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/monoidal.py` & `discopy-1.1.4/discopy/monoidal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/pivotal.py` & `discopy-1.1.4/discopy/pivotal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/python.py` & `discopy-1.1.4/discopy/python.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/quantum/__init__.py` & `discopy-1.1.4/discopy/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/quantum/ansatze.py` & `discopy-1.1.4/discopy/quantum/ansatze.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/quantum/channel.py` & `discopy-1.1.4/discopy/quantum/channel.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/quantum/circuit.py` & `discopy-1.1.4/discopy/quantum/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,22 @@
             raise ValueError
         self.dim = dim
         super().__init__(name, z)
 
     def __repr__(self):
         return f"{factory_name(type(self))}({self.dim})"
 
+    @classmethod
+    def from_tree(cls, tree: dict) -> Ob:
+        dim, z = tree['dim'], tree.get('z', 0)
+        return cls(dim=dim, z=z)
+
+    def to_tree(self) -> dict:
+        return dict(dim=self.dim, **super().to_tree())
+
 
 class Digit(Ob):
     """
     A digit is a classical unit of information.
 
     Parameters:
         dim : The dimension of the digit, e.g. ``2`` for bits.
```

### Comparing `discopy-1.1.3/discopy/quantum/gates.py` & `discopy-1.1.4/discopy/quantum/gates.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,27 @@
     Controlled
     Parametrized
     Rotation
     Rx
     Ry
     Rz
     CU1
+    CRz
+    CRx
     Scalar
     MixedScalar
     Sqrt
 
 .. admonition:: Functions
 
     .. autosummary::
         :template: function.rst
         :nosignatures:
         :toctree:
 
-        CRz
-        CRx
         sqrt
         scalar
 """
 
 from math import e, pi
 
 from discopy import messages
@@ -566,14 +566,18 @@
 
     def __init__(self, phase, z=0):
         name, n_qubits = type(self).__name__, type(self).n_qubits
         dom = cod = qubit ** n_qubits
         QuantumGate.__init__(self, name, dom, cod, z=z)
         Parametrized.__init__(self, name, dom, cod, is_mixed=False, data=phase)
 
+    @classmethod
+    def from_tree(cls, tree: dict):
+        return cls(tree['data'], tree.get('z', 0))
+
     @property
     def phase(self):
         """ The phase of a rotation gate. """
         return self.data
 
     def dagger(self):
         return type(self)(-self.phase)
```

### Comparing `discopy-1.1.3/discopy/quantum/pennylane.py` & `discopy-1.1.4/discopy/quantum/pennylane.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,30 +97,35 @@
 
     Returns
     -------
     :class:`qml.operation.Operation`
         The PennyLane operation equivalent to the input pytket Op.
     list of (:class:`torch.FloatTensor` or :class:`sympy.core.symbol.Symbol`)
         The parameters of the operation.
+    list of :class:`sympy.core.symbol.Symbol`
+        The free symbols in the parameters of the operation.
     list of int
         The wires/qubits to apply the operation to.
     """
     wires = [x.index[0] for x in tk_op.qubits]
     params = tk_op.op.params
+    symbols = set()
 
     remapped_params = []
     for param in params:
         # scale rotation from [0, 2) to [0, 1), (rescale to [0, 2pi) later)
         param /= 2
         if not isinstance(param, sympy.Expr):
             param = torch.tensor(param)
+        else:
+            symbols.update(param.free_symbols)
 
         remapped_params.append(param)
 
-    return OP_MAP[tk_op.op.type], remapped_params, wires
+    return OP_MAP[tk_op.op.type], remapped_params, symbols, wires
 
 
 def extract_ops_from_tk(tk_circ):
     """
     Extract the operations, and corresponding parameters and wires,
     from a pytket Circuit. Return these as lists to use in
     constructing PennyLane circuit.
@@ -135,25 +140,29 @@
     list of :class:`qml.operation.Operation`
         The PennyLane operations extracted from the pytket circuit.
     list of list of (:class:`torch.FloatTensor` or
                      :class:`sympy.core.symbol.Symbol`)
         The corresponding parameters of the operations.
     list of list of int
         The corresponding wires of the operations.
+    set of :class:`sympy.core.symbol.Symbol`
+        The free symbols in the parameters of the tket circuit.
     """
     op_list, params_list, wires_list = [], [], []
+    symbols_set = set()
 
     for op in tk_circ.__iter__():
         if op.op.type != OpType.Measure:
-            op, params, wires = tk_op_to_pennylane(op)
+            op, params, symbols, wires = tk_op_to_pennylane(op)
             op_list.append(op)
             params_list.append(params)
             wires_list.append(wires)
+            symbols_set.update(symbols)
 
-    return op_list, params_list, wires_list
+    return op_list, params_list, wires_list, symbols_set
 
 
 def get_post_selection_dict(tk_circ):
     """
     Return post-selections based on qubit indices.
 
     Parameters
@@ -208,24 +217,26 @@
         The PennyLane circuit equivalent to the input DisCoPy circuit.
     """
     if disco_circuit.is_mixed:
         raise ValueError('Only pure quantum circuits are currently '
                          'supported.')
 
     tk_circ = disco_circuit.to_tk()
-    op_list, params_list, wires_list = extract_ops_from_tk(tk_circ)
+    op_list, params_list, wires_list, symbols_set = \
+        extract_ops_from_tk(tk_circ)
 
     post_selection = get_post_selection_dict(tk_circ)
 
     scalar = 1
     for box in disco_circuit.boxes:
         if isinstance(box, Scalar):
             scalar *= box.array
 
     return PennyLaneCircuit(op_list,
+                            list(symbols_set),
                             params_list,
                             wires_list,
                             probabilities,
                             post_selection,
                             scalar,
                             tk_circ.n_qubits,
                             backend_config,
@@ -236,18 +247,19 @@
 STATE_DEVICES = ['aer_simulator_statevector', 'statevector_simulator']
 
 
 class PennyLaneCircuit:
     """
     Implement a pennylane circuit with post-selection.
     """
-    def __init__(self, ops, params, wires, probabilities,
+    def __init__(self, ops, symbols, params, wires, probabilities,
                  post_selection, scale, n_qubits, backend_config,
                  diff_method):
         self._ops = ops
+        self._symbols = symbols
         self._params = params
         self._wires = wires
         self._probabilities = probabilities
         self._post_selection = post_selection
         self._scale = scale
         self._n_qubits = n_qubits
         self._backend_config = backend_config
@@ -311,22 +323,23 @@
         -------
         bool
             Whether the circuit parameters contain SymPy symbols.
         """
         return any(isinstance(expr, sympy.Expr) for expr_list in
                    self._params for expr in expr_list)
 
-    def initialise_concrete_params(self, symbols, weights):
+    def initialise_concrete_params(self, symbol_weight_map):
         """
         Given concrete values for each of the SymPy symbols, substitute
         the symbols for the values to obtain concrete parameters, via
         the `param_substitution` method.
         """
         if self._contains_sympy:
-            self._concrete_params = self.param_substitution(symbols, weights)
+            weights = [symbol_weight_map[symbol] for symbol in self._symbols]
+            self._concrete_params = self.param_substitution(weights)
 
     def draw(self):
         """
         Print a string representation of the circuit
         similar to `qml.draw`, but including post-selection.
 
         Parameters
@@ -417,37 +430,35 @@
                                  else self._scale)
 
         if post_selected_states.shape[0] == 1:
             return post_selected_states
         else:
             return torch.reshape(post_selected_states, (2,) * open_wires)
 
-    def param_substitution(self, symbols, weights):
+    def param_substitution(self, weights):
         """
         Substitute symbolic parameters (SymPy symbols) with floats.
 
         Parameters
         ----------
-        symbols : list of :class:`sympy.core.symbol.Symbol`
-            The symbols from the original DisCoPy circuit.
         weights : list of :class:`torch.FloatTensor`
             The weights to substitute for the symbols.
 
         Returns
         -------
         :class:`torch.FloatTensor`
             The concrete (non-symbolic) parameters for the
             circuit.
         """
         concrete_params = []
         for expr_list in self._params:
             concrete_list = []
             for expr in expr_list:
                 if isinstance(expr, sympy.Expr):
-                    f_expr = sympy.lambdify([symbols], expr)
+                    f_expr = sympy.lambdify([self._symbols], expr)
                     expr = f_expr(weights)
                 concrete_list.append(expr)
             concrete_params.append(concrete_list)
 
         return concrete_params
 
     def eval(self):
```

### Comparing `discopy-1.1.3/discopy/quantum/tk.py` & `discopy-1.1.4/discopy/quantum/tk.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/quantum/zx.py` & `discopy-1.1.4/discopy/quantum/zx.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/ribbon.py` & `discopy-1.1.4/discopy/ribbon.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/rigid.py` & `discopy-1.1.4/discopy/rigid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/symmetric.py` & `discopy-1.1.4/discopy/symmetric.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/tensor.py` & `discopy-1.1.4/discopy/tensor.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy/traced.py` & `discopy-1.1.4/discopy/traced.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 >>> from discopy.symmetric import Ty, Box, Swap, Id
 >>> from discopy import symmetric
 >>> symmetric.Diagram.structure_preserving = True
 >>> x = Ty('x')
 >>> f, g = Box('f', x @ x, x @ x), Box('g', x, x)
 
 * Vanishing
+
 >>> assert f.trace(n=0) == f == f.trace(n=0, left=True)
 >>> assert f.trace(n=2) == f.trace().trace()
 >>> assert f.trace(n=2, left=True) == f.trace(left=True).trace(left=True)
 
 * Superposing
 
 >>> assert (x @ f).trace() == x @ f.trace()
```

### Comparing `discopy-1.1.3/discopy/utils.py` & `discopy-1.1.4/discopy/utils.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/discopy.egg-info/PKG-INFO` & `discopy-1.1.4/discopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.1.3
+Version: 1.1.4
 Summary: The Python toolkit for computing with string diagrams.
 Author: DisCoPy
 Author-email: contact@discopy.org
 License: BSD 3-Clause License
         
         Copyright (c) 2019-2022, DisCoPy
         All rights reserved.
@@ -63,19 +63,19 @@
 [![build](https://github.com/discopy/discopy/actions/workflows/build_test.yml/badge.svg)](https://github.com/discopy/discopy/actions/workflows/build_test.yml)
 [![readthedocs](https://readthedocs.org/projects/discopy/badge/?version=main)](https://docs.discopy.org/)
 [![PyPI version](https://badge.fury.io/py/discopy.svg)](https://badge.fury.io/py/discopy)
 [![DOI: 10.4204/EPTCS.333.13](http://img.shields.io/badge/DOI-10.4204/EPTCS.333.13-brightgreen.svg)](https://doi.org/10.4204/EPTCS.333.13)
 
 DisCoPy is a Python toolkit for computing with [string diagrams](https://en.wikipedia.org/wiki/String_diagram).
 
-* **Organisation:** https://discopy.org
-* **Documentation:** https://docs.discopy.org
-* **Source code:** https://github.com/discopy/discopy
-* **Paper (for applied category theorists):** https://doi.org/10.4204/EPTCS.333.13
-* **Paper (for quantum computer scientists):** https://arxiv.org/abs/2205.05190
+* **Organisation:** <https://discopy.org>
+* **Documentation:** <https://docs.discopy.org>
+* **Source code:** <https://github.com/discopy/discopy>
+* **Paper (for applied category theorists):** <https://doi.org/10.4204/EPTCS.333.13>
+* **Paper (for quantum computer scientists):** <https://arxiv.org/abs/2205.05190>
 
 DisCoPy began as an implementation of [DisCoCat](https://en.wikipedia.org/wiki/DisCoCat) and [QNLP](https://en.wikipedia.org/wiki/Quantum_natural_language_processing). This has now become its own library: [lambeq](https://cqcl.github.io/lambeq).
 
 ## Features
 
 * an `Arrow` data structure for free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
 * a `Diagram` data structure for planar string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (with braids, twists, spiders, etc.)
```

### Comparing `discopy-1.1.3/discopy.egg-info/SOURCES.txt` & `discopy-1.1.4/discopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/Makefile` & `discopy-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_ext/bases-fullname.py` & `discopy-1.1.4/docs/_ext/bases-fullname.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_ext/youtube.py` & `discopy-1.1.4/docs/_ext/youtube.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/balanced/ribbon_twist.png` & `discopy-1.1.4/docs/_static/balanced/ribbon_twist.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/balanced/twist.png` & `discopy-1.1.4/docs/_static/balanced/twist.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/balanced/twist_dual_rail.png` & `discopy-1.1.4/docs/_static/balanced/twist_dual_rail.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/braided/hexagons.png` & `discopy-1.1.4/docs/_static/braided/hexagons.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/braided/inverse.png` & `discopy-1.1.4/docs/_static/braided/inverse.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/closed/curry-left.png` & `discopy-1.1.4/docs/_static/closed/curry-left.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/closed/curry-right.png` & `discopy-1.1.4/docs/_static/closed/curry-right.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/closed/uncurry.png` & `discopy-1.1.4/docs/_static/closed/uncurry.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/compact/reidemeister.png` & `discopy-1.1.4/docs/_static/compact/reidemeister.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/compact/snake.png` & `discopy-1.1.4/docs/_static/compact/snake.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/compact/yanking.png` & `discopy-1.1.4/docs/_static/compact/yanking.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/compact/yanking_cup_and_cap.png` & `discopy-1.1.4/docs/_static/compact/yanking_cup_and_cap.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/drawing/diagramize.png` & `discopy-1.1.4/docs/_static/drawing/diagramize.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/drawing/example.html` & `discopy-1.1.4/docs/_static/drawing/example.html`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/drawing/frobenius-axioms.png` & `discopy-1.1.4/docs/_static/drawing/frobenius-axioms.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/frobenius/comonoid.png` & `discopy-1.1.4/docs/_static/frobenius/comonoid.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/frobenius/frobenius.png` & `discopy-1.1.4/docs/_static/frobenius/frobenius.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/frobenius/monoid.png` & `discopy-1.1.4/docs/_static/frobenius/monoid.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/frobenius/special.png` & `discopy-1.1.4/docs/_static/frobenius/special.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/grammar/cfg-example.png` & `discopy-1.1.4/docs/_static/grammar/cfg-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/grammar/pregroup-example.png` & `discopy-1.1.4/docs/_static/grammar/pregroup-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/hypergraph/box.png` & `discopy-1.1.4/docs/_static/hypergraph/box.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/hypergraph/diagram.png` & `discopy-1.1.4/docs/_static/hypergraph/diagram.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/hypergraph/unfuse.png` & `discopy-1.1.4/docs/_static/hypergraph/unfuse.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/alice-loves-bob.png` & `discopy-1.1.4/docs/_static/int/alice-loves-bob.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/braid.png` & `discopy-1.1.4/docs/_static/int/braid.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/composition.png` & `discopy-1.1.4/docs/_static/int/composition.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/dagger.png` & `discopy-1.1.4/docs/_static/int/dagger.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/idl.png` & `discopy-1.1.4/docs/_static/int/idl.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/idr.png` & `discopy-1.1.4/docs/_static/int/idr.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/int-snake-equations.png` & `discopy-1.1.4/docs/_static/int/int-snake-equations.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/simplify.png` & `discopy-1.1.4/docs/_static/int/simplify.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/int/tensor.png` & `discopy-1.1.4/docs/_static/int/tensor.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/logo.ico` & `discopy-1.1.4/docs/_static/logo.ico`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/markov/associativity.png` & `discopy-1.1.4/docs/_static/markov/associativity.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/markov/bialgebra.png` & `discopy-1.1.4/docs/_static/markov/bialgebra.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/markov/copy_and_apply.png` & `discopy-1.1.4/docs/_static/markov/copy_and_apply.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/markov/counit.png` & `discopy-1.1.4/docs/_static/markov/counit.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/Eckmann-Hilton.gif` & `discopy-1.1.4/docs/_static/monoidal/Eckmann-Hilton.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/EckmannHilton.gif` & `discopy-1.1.4/docs/_static/monoidal/EckmannHilton.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/arrow-example.png` & `discopy-1.1.4/docs/_static/monoidal/arrow-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/box-example.png` & `discopy-1.1.4/docs/_static/monoidal/box-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/bubble-example.png` & `discopy-1.1.4/docs/_static/monoidal/bubble-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/foliate-example-1.png` & `discopy-1.1.4/docs/_static/monoidal/foliate-example-1.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/foliate-example-1a.png` & `discopy-1.1.4/docs/_static/monoidal/foliate-example-1a.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/foliate-example-1b.png` & `discopy-1.1.4/docs/_static/monoidal/foliate-example-1b.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/foliate-example-2.png` & `discopy-1.1.4/docs/_static/monoidal/foliate-example-2.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/functor-example.png` & `discopy-1.1.4/docs/_static/monoidal/functor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/id-example.png` & `discopy-1.1.4/docs/_static/monoidal/id-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/spiral.gif` & `discopy-1.1.4/docs/_static/monoidal/spiral.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/monoidal/tensor-example.png` & `discopy-1.1.4/docs/_static/monoidal/tensor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/optics/fusion.png` & `discopy-1.1.4/docs/_static/optics/fusion.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/optics/spider-decomp.png` & `discopy-1.1.4/docs/_static/optics/spider-decomp.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/pivotal/axiom.png` & `discopy-1.1.4/docs/_static/pivotal/axiom.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/pivotal/box-conjugate.png` & `discopy-1.1.4/docs/_static/pivotal/box-conjugate.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/pivotal/conjugate.png` & `discopy-1.1.4/docs/_static/pivotal/conjugate.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/pivotal/dagger-transpose.png` & `discopy-1.1.4/docs/_static/pivotal/dagger-transpose.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/pivotal/dagger.png` & `discopy-1.1.4/docs/_static/pivotal/dagger.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/pivotal/trace.png` & `discopy-1.1.4/docs/_static/pivotal/trace.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/quantum/circuit-example.png` & `discopy-1.1.4/docs/_static/quantum/circuit-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/quantum/functor-example.png` & `discopy-1.1.4/docs/_static/quantum/functor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/ribbon/strict.png` & `discopy-1.1.4/docs/_static/ribbon/strict.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/ribbon/twist-untwist.png` & `discopy-1.1.4/docs/_static/ribbon/twist-untwist.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/cap.png` & `discopy-1.1.4/docs/_static/rigid/cap.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/caps.png` & `discopy-1.1.4/docs/_static/rigid/caps.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/cup.png` & `discopy-1.1.4/docs/_static/rigid/cup.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/cups.png` & `discopy-1.1.4/docs/_static/rigid/cups.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/curry.png` & `discopy-1.1.4/docs/_static/rigid/curry.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/diagram-example.png` & `discopy-1.1.4/docs/_static/rigid/diagram-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/functor-example.png` & `discopy-1.1.4/docs/_static/rigid/functor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/rotate.png` & `discopy-1.1.4/docs/_static/rigid/rotate.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/transpose.png` & `discopy-1.1.4/docs/_static/rigid/transpose.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/transpose_box.png` & `discopy-1.1.4/docs/_static/rigid/transpose_box.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/rigid/typed-snake-equation.png` & `discopy-1.1.4/docs/_static/rigid/typed-snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/snake-equation.png` & `discopy-1.1.4/docs/_static/snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/spiral.gif` & `discopy-1.1.4/docs/_static/spiral.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/symmetric/decorator.png` & `discopy-1.1.4/docs/_static/symmetric/decorator.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/symmetric/hexagons.png` & `discopy-1.1.4/docs/_static/symmetric/hexagons.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/symmetric/inverse.png` & `discopy-1.1.4/docs/_static/symmetric/inverse.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/symmetric/naturality.png` & `discopy-1.1.4/docs/_static/symmetric/naturality.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/symmetric/yang-baxter.png` & `discopy-1.1.4/docs/_static/symmetric/yang-baxter.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/tensor/chain-rule.png` & `discopy-1.1.4/docs/_static/tensor/chain-rule.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/tensor/frobenius-example.png` & `discopy-1.1.4/docs/_static/tensor/frobenius-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/tensor/men-are-mortal.png` & `discopy-1.1.4/docs/_static/tensor/men-are-mortal.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/tensor/product-rule.png` & `discopy-1.1.4/docs/_static/tensor/product-rule.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/tensor/rewrite.png` & `discopy-1.1.4/docs/_static/tensor/rewrite.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/golden.png` & `discopy-1.1.4/docs/_static/traced/golden.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/right-nat-trace.png` & `discopy-1.1.4/docs/_static/traced/right-nat-trace.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/sliding-left.png` & `discopy-1.1.4/docs/_static/traced/sliding-left.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/sliding-right.png` & `discopy-1.1.4/docs/_static/traced/sliding-right.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/tightening-left.png` & `discopy-1.1.4/docs/_static/traced/tightening-left.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/tightening-right.png` & `discopy-1.1.4/docs/_static/traced/tightening-right.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/trace.png` & `discopy-1.1.4/docs/_static/traced/trace.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_static/traced/yanking.png` & `discopy-1.1.4/docs/_static/traced/yanking.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/_style/custom.css` & `discopy-1.1.4/docs/_style/custom.css`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/api/architecture.html` & `discopy-1.1.4/docs/api/architecture.html`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/api/architecture.png` & `discopy-1.1.4/docs/api/architecture.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/conf.py` & `discopy-1.1.4/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.napoleon',
               'sphinx.ext.autosummary',
               'sphinx.ext.viewcode',
-              'm2r2',
+              'myst_parser',
               'sphinx.ext.mathjax',
               'youtube',
               'bases-fullname',
               'sphinxcontrib.bibtex',
               'nbsphinx',
               'IPython.sphinxext.ipython_console_highlighting'
               ]
@@ -86,13 +86,20 @@
 
 html_title = "DisCoPy"
 
 html_theme_options = {
     "repository_url": "https://github.com/discopy/discopy",
     "use_repository_button": True,
     "path_to_docs": "docs",
-    "extra_navbar": "",
+    # "extra_navbar": "",
+}
+myst_enable_extensions = ["attrs_block"]
+myst_url_schemes = {
+    "http": None,
+    "https": None,
+    "doi": "https://doi.org/{{path}}",
+    "arXiv": "https://arxiv.org/abs/{{path}}",
 }
 
 master_doc = 'index'
 
 html_baseurl = "https://docs.discopy.org"
```

### Comparing `discopy-1.1.3/docs/discopy.bib` & `discopy-1.1.4/docs/discopy.bib`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/extra/blogs.md` & `discopy-1.1.4/docs/extra/blogs.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 * ["We did it! On an actual quantum computer!"](https://medium.com/cambridge-quantum-computing/quantum-natural-language-processing-748d6f27b31d)
 * [Now you can try it yourself with lambeq](https://medium.com/cambridge-quantum-computing/quantum-natural-language-processing-ii-6b6a44b319b2)
 
 ## Graphical linear algebra
 
 This blog by [Pawel Sobocinski](https://www.ioc.ee/~pawel/) is what got us hooked to string diagrams.
 
-* https://graphicallinearalgebra.net/
+* <https://graphicallinearalgebra.net>
 
 ## Monads and comonads
 
 Dan Marsden writing about applications of string diagrams to monads, comonads and theoretical computer science.
 
-* https://stringdiagram.com/
+* <https://stringdiagram.com>
 
 ## Azimuth
 
 [John Baez](https://math.ucr.edu/home/baez/)'s blog is a great place to learn about string diagrams and category theory.
 
-* https://johncarlosbaez.wordpress.com/?s=string+diagram
+* <https://johncarlosbaez.wordpress.com/?s=string+diagram>
```

### Comparing `discopy-1.1.3/docs/extra/papers.md` & `discopy-1.1.4/docs/extra/papers.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 # Publications
 
 ## PhD theses
 
 ### Category Theory for Quantum Natural Language Processing
 
-https://arxiv.org/abs/2212.06615
+<arXiv:2212.06615>
 
 Alexis Toumi
 
 **Abstract:**
 This thesis introduces quantum natural language processing (QNLP) models based on a simple yet powerful analogy between computational linguistics and quantum mechanics: grammar as entanglement. The grammatical structure of text and sentences connects the meaning of words in the same way that entanglement structure connects the states of quantum systems. Category theory allows to make this language-to-qubit analogy formal: it is a monoidal functor from grammar to vector spaces. We turn this abstract analogy into a concrete algorithm that translates the grammatical structure onto the architecture of parameterised quantum circuits. We then use a hybrid classical-quantum algorithm to train the model so that evaluating the circuits computes the meaning of sentences in data-driven tasks.
 
 The implementation of QNLP models motivated the development of DisCoPy (Distributional Compositional Python), the toolkit for applied category theory of which the first chapter gives a comprehensive overview. String diagrams are the core data structure of DisCoPy, they allow to reason about computation at a high level of abstraction. We show how they can encode both grammatical structures and quantum circuits, but also logical formulae, neural networks or arbitrary Python code. Monoidal functors allow to translate these abstract diagrams into concrete computation, interfacing with optimised task-specific libraries.
 
 The second chapter uses DisCopy to implement QNLP models as parameterised functors from grammar to quantum circuits. It gives a first proof-of-concept for the more general concept of functorial learning: generalising machine learning from functions to functors by learning from diagram-like data. In order to learn optimal functor parameters via gradient descent, we introduce the notion of diagrammatic differentiation: a graphical calculus for computing the gradients of parameterised diagrams.
 
 ### Categorical Tools for Natural Language Processing
 
-https://arxiv.org/abs/2212.06636
+<arXiv:2212.06636>
 
 Giovanni de Felice
 
 **Abstract:**
 This thesis develops the translation between category theory and computational linguistics as a foundation for natural language processing. The three chapters deal with syntax, semantics and pragmatics. First, string diagrams provide a unified model of syntactic structures in formal grammars. Second, functors compute semantics by turning diagrams into logical, tensor, neural or quantum computation. Third, the resulting functorial models can be composed to form games where equilibria are the solutions of language processing tasks. This framework is implemented as part of DisCoPy, the Python library for computing with string diagrams. We describe the correspondence between categorical, linguistic and computational structures, and demonstrate their applications in compositional natural language processing.
 
 ## Conferences
 
 ### DisCoPy: Monoidal categories in Python
 
-https://doi.org/10.4204/EPTCS.333.13
+<doi:10.4204/EPTCS.333.13>
 
 Giovanni de Felice, Alexis Toumi, Bob Coecke
 
 **Abstract:**
 We introduce DisCoPy, an open source toolbox for computing with monoidal categories. The library provides an intuitive syntax for defining string diagrams and monoidal functors. Its modularity allows the efficient implementation of computational experiments in the various applications of category theory where diagrams have become a lingua franca. As an example, we used DisCoPy to perform natural language processing on quantum hardware for the first time.
 
 ### Diagrammatic Differentiation for Quantum Machine Learning
 
-https://doi.org/10.4204/EPTCS.343.7
+<doi:10.4204/EPTCS.343.7>
 
 Alexis Toumi, Richie Yeung, Giovanni de Felice
 
 **Abstract:**
 We introduce diagrammatic differentiation for tensor calculus by generalising the dual number construction from rigs to monoidal categories. Applying this to ZX diagrams, we show how to calculate diagrammatically the gradient of a linear map with respect to a phase parameter. For diagrams of parametrised quantum circuits, we get the well-known parameter-shift rule at the basis of many variational quantum algorithms. We then extend our method to the automatic differentation of hybrid classical-quantum circuits, using diagrams with bubbles to encode arbitrary non-linear operators. Moreover, diagrammatic differentiation comes with an open-source implementation in DisCoPy, the Python library for monoidal categories. Diagrammatic gradients of classical-quantum circuits can then be simplified using the PyZX library and executed on quantum hardware via the tket compiler. This opens the door to many practical applications harnessing both the structure of string diagrams and the computational power of quantum machine learning.
 
 ### DisCoPy for the quantum computer scientist
 
-https://arxiv.org/abs/2205.05190
+<arXiv:2205.05190>
 
 Alexis Toumi, Giovanni de Felice, Richie Yeung
 
 **Abstract:**
 DisCoPy (Distributional Compositional Python) is an open source toolbox for computing with string diagrams and functors. In particular, the diagram data structure allows to encode various kinds of quantum processes, with functors for classical simulation and optimisation, as well as compilation and evaluation on quantum hardware. This includes the ZX calculus and its many variants, the parameterised circuits used in quantum machine learning, but also linear optical quantum computing. We review the recent developments of the library in this direction, making DisCoPy a toolbox for the quantum computer scientist.
 
 ### Functorial Language Models
 
-https://arxiv.org/abs/2103.14411
+<arXiv:2103.14411>
 
 Alexis Toumi, Alex Koziell-Pipe
 
 **Abstract:** We introduce functorial language models: a principled way to compute probability distributions over word sequences given a monoidal functor from grammar to meaning. This yields a method for training categorical compositional distributional (DisCoCat) models on raw text data. We provide a proof-of-concept implementation in DisCoPy, the Python toolbox for monoidal categories.
```

### Comparing `discopy-1.1.3/docs/extra/talks.rst` & `discopy-1.1.4/docs/extra/talks.rst`

 * *Files 13% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 ---------
 
 The first demo of DisCoPy experiments on quantum hardware was presented at
 `QNLP 2020`_ see the corresponding notebook qnlp-experiment_.
 
 .. youtube:: NJFYXZyeMj0
 
-.. _qnlp-experiment: https://github.com/discopy/discopy/blob/main/docs/notebooks/qnlp-experiment.ipynb
+.. _qnlp-experiment: https://github.com/discopy/discopy/blob/legacy/docs/notebooks/qnlp-experiment.ipynb
 .. _QNLP 2020: https://quantumweek2020.cambridgequantum.com/qnlp.html
 
 QNLP 2019
 ---------
 
 The first demo of DisCoPy was presented at
-`the first QNLP workshop <http://www.cs.ox.ac.uk/QNLP2019/>`_
+`the first QNLP workshop <http://www.cs.ox.ac.uk/QNLP2019>`_
 see the corresponding notebooks alice-loves-bob_ and bob-is-rich_.
 
 .. youtube:: 3UKqpL7Z0Uc
 
-.. _alice-loves-bob: https://github.com/discopy/discopy/blob/main/notebooks/alice-loves-bob.ipynb
-.. _bob-is-rich: https://github.com/discopy/discopy/blob/main/notebooks/bob-is-rich.ipynb
+.. _alice-loves-bob: https://github.com/discopy/discopy/blob/legacy/docs/notebooks/alice-loves-bob.ipynb
+.. _bob-is-rich: https://github.com/discopy/discopy/blob/legacy/docs/notebooks/bob-is-rich.ipynb
```

### Comparing `discopy-1.1.3/docs/make.bat` & `discopy-1.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/notebooks/21-05-03-tallcat.ipynb` & `discopy-1.1.4/docs/notebooks/21-05-03-tallcat.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/notebooks/21-05-05-tallcat.ipynb` & `discopy-1.1.4/docs/notebooks/21-05-05-tallcat.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/notebooks/diag-diff.ipynb` & `discopy-1.1.4/docs/notebooks/diag-diff.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/notebooks/diagrams.ipynb` & `discopy-1.1.4/docs/notebooks/diagrams.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/docs/notebooks/qnlp.ipynb` & `discopy-1.1.4/docs/notebooks/qnlp.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/pyproject.toml` & `discopy-1.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -53,22 +53,22 @@
     "pennylane-qiskit",
     "pennylane-honeywell",
     "lxml",
     "nltk",
     "pylint"
 ]
 docs  = [
-    "sphinx == 4.5.0",
-    "sphinx-book-theme == 0.3.3",
-    "m2r2 == 0.3.2",
-    "nbsphinx == 0.8.9",
-    "ipykernel == 6.17.0",
-    "sphinxcontrib-youtube == 1.2.0",
-    "jinja2 == 3.0.3",
-    "sphinxcontrib-bibtex == 2.4.0",
+    "sphinx == 6.0.*",
+    "sphinx-book-theme == 1.0.*",
+    "myst-parser == 2.0.*",
+    "nbsphinx == 0.9.*",
+    "ipykernel == 6.23.*",
+    "sphinxcontrib-youtube == 1.2.*",
+    "jinja2 == 3.1.*",
+    "sphinxcontrib-bibtex == 2.5.*",
     "IPython"
 ]
 
 [project.urls]
 Homepage = "https://discopy.org"
 Documentation = "https://docs.discopy.org"
 Repository = "https://github.com/discopy/discopy"
```

### Comparing `discopy-1.1.3/test/drawing/legacy.py` & `discopy-1.1.4/test/drawing/legacy.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/grammar/categorial.py` & `discopy-1.1.4/test/grammar/categorial.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/grammar/pregroup.py` & `discopy-1.1.4/test/grammar/pregroup.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/quantum/channel.py` & `discopy-1.1.4/test/quantum/channel.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/quantum/circuit.py` & `discopy-1.1.4/test/quantum/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -574,25 +574,26 @@
 
     assert np.allclose(p_no_open_snake_prob.eval().numpy(),
                        no_open_snake.eval().array)
 
     x, y, z = sympy.symbols('x y z')
     symbols = [x, y, z]
     weights = [torch.tensor(1.), torch.tensor(2.), torch.tensor(3.)]
+    symbol_weight_map = dict(zip(symbols, weights))
 
     var_circ = Circuit.decode(
         dom=qubit ** 0, boxes_and_offsets=zip(
             [Ket(0), Rx(0.552), Rz(x), Rx(0.917), Ket(0, 0, 0), H, H, H,
              CRz(0.18), CRz(y), CX, H, sqrt(2), Bra(0, 0), Ket(0),
              Rx(0.446), Rz(0.256), Rx(z), CX, H, sqrt(2), Bra(0, 0)],
             [0, 0, 0, 0, 0, 0, 1, 2, 0, 1, 2, 2,
              3, 2, 0, 0, 0, 0, 0, 0, 1, 0]))
 
     p_var_circ = var_circ.to_pennylane()
-    p_var_circ.initialise_concrete_params(symbols, weights)
+    p_var_circ.initialise_concrete_params(symbol_weight_map)
     p_var_circ.draw()
 
     captured = capsys.readouterr()
     assert captured.out == \
         ("0: ──RX(2.80)──RZ(1.61)──RX(18.85)─╭●──H─┤0>\n"
          "1: ──H────────╭●───────────────────╰X────┤0>\n"
          "2: ──H────────╰RZ(1.13)─╭●───────────────┤  State\n"
@@ -602,15 +603,15 @@
     var_f = var_circ.lambdify(*symbols)
     conc_circ = var_f(*[a.item() for a in weights])
 
     assert np.allclose(p_var_circ.eval().numpy(),
                        conc_circ.eval().array)
 
     p_var_circ_prob = var_circ.to_pennylane(probabilities=True)
-    p_var_circ_prob.initialise_concrete_params(symbols, weights)
+    p_var_circ_prob.initialise_concrete_params(symbol_weight_map)
     conc_circ_prob = (conc_circ >> Measure())
 
     assert (np.allclose(p_var_circ_prob.eval().numpy(),
                         conc_circ_prob.eval().array))
 
 
 def test_PennyLaneCircuit_mixed_error():
@@ -703,18 +704,19 @@
     with raises(ValueError):
         p_var_circ.eval()
 
 
 def test_pennylane_parameter_reference():
     x = sympy.symbols('x')
     p = torch.nn.Parameter(torch.tensor(1.))
+    symbol_weight_map = {x: p}
 
     circ = Rx(x)
     p_circ = circ.to_pennylane()
-    p_circ.initialise_concrete_params([x], [p])
+    p_circ.initialise_concrete_params(symbol_weight_map)
 
     with torch.no_grad():
         p.add_(1.)
 
     assert p_circ._concrete_params[0][0] == p
 
     with torch.no_grad():
@@ -736,29 +738,36 @@
              3, 2, 0, 0, 0, 0, 0, 0, 1, 0]))
 
     for diff_method in ['backprop', 'parameter-shift', 'finite-diff']:
 
         weights = [torch.tensor(1., requires_grad=True),
                    torch.tensor(2., requires_grad=True),
                    torch.tensor(3., requires_grad=True)]
+        symbol_weight_map = dict(zip(symbols, weights))
 
         p_var_circ = var_circ.to_pennylane(probabilities=True,
                                            diff_method=diff_method)
-        p_var_circ.initialise_concrete_params(symbols, weights)
+        p_var_circ.initialise_concrete_params(symbol_weight_map)
 
         loss = p_var_circ.eval().norm(dim=0, p=2)
         loss.backward()
         assert weights[0].grad is not None
 
     for diff_method in ['backprop']:
 
         weights = [torch.tensor(1., requires_grad=True),
                    torch.tensor(2., requires_grad=True),
                    torch.tensor(3., requires_grad=True)]
+        symbol_weight_map = dict(zip(symbols, weights))
 
         p_var_circ = var_circ.to_pennylane(probabilities=False,
                                            diff_method=diff_method)
-        p_var_circ.initialise_concrete_params(symbols, weights)
+        p_var_circ.initialise_concrete_params(symbol_weight_map)
 
         loss = p_var_circ.eval().norm(dim=0, p=2)
         loss.backward()
         assert weights[0].grad is not None
+
+
+def test_loads_dumps():
+    from discopy.utils import loads, dumps
+    assert loads(dumps(Rx(1))) == Rx(1)
```

### Comparing `discopy-1.1.3/test/quantum/eval.py` & `discopy-1.1.4/test/quantum/eval.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/quantum/tk.py` & `discopy-1.1.4/test/quantum/tk.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/quantum/zx.py` & `discopy-1.1.4/test/quantum/zx.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/semantics/matrix.py` & `discopy-1.1.4/test/semantics/matrix.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/semantics/python.py` & `discopy-1.1.4/test/semantics/python.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/semantics/tensor.py` & `discopy-1.1.4/test/semantics/tensor.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/EckmannHilton.gif` & `discopy-1.1.4/test/src/imgs/EckmannHilton.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/bell-state.png` & `discopy-1.1.4/test/src/imgs/bell-state.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/bialgebra.png` & `discopy-1.1.4/test/src/imgs/bialgebra.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/crack-eggs.png` & `discopy-1.1.4/test/src/imgs/crack-eggs.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/empty_diagram.png` & `discopy-1.1.4/test/src/imgs/empty_diagram.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/long-controlled.png` & `discopy-1.1.4/test/src/imgs/long-controlled.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/sentence-as-diagram.png` & `discopy-1.1.4/test/src/imgs/sentence-as-diagram.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/snake-equation.png` & `discopy-1.1.4/test/src/imgs/snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/spiral.png` & `discopy-1.1.4/test/src/imgs/spiral.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/typed-snake-equation.png` & `discopy-1.1.4/test/src/imgs/typed-snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/imgs/who-ansatz.png` & `discopy-1.1.4/test/src/imgs/who-ansatz.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/bell-state.tikz` & `discopy-1.1.4/test/src/tikz/bell-state.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/bialgebra.tikz` & `discopy-1.1.4/test/src/tikz/bialgebra.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/copy.tikz` & `discopy-1.1.4/test/src/tikz/copy.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/crack-eggs.tikz` & `discopy-1.1.4/test/src/tikz/crack-eggs.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/long-controlled.tikz` & `discopy-1.1.4/test/src/tikz/long-controlled.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/snake-equation.tikz` & `discopy-1.1.4/test/src/tikz/snake-equation.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/spiral.tikz` & `discopy-1.1.4/test/src/tikz/spiral.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tikz/who-ansatz.tikz` & `discopy-1.1.4/test/src/tikz/who-ansatz.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/tree2diagram.pickle` & `discopy-1.1.4/test/src/tree2diagram.pickle`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/src/zx-graph.json` & `discopy-1.1.4/test/src/zx-graph.json`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/cat.py` & `discopy-1.1.4/test/syntax/cat.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/closed.py` & `discopy-1.1.4/test/syntax/closed.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/compact.py` & `discopy-1.1.4/test/syntax/compact.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/frobenius.py` & `discopy-1.1.4/test/syntax/frobenius.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/hypergraph.py` & `discopy-1.1.4/test/syntax/hypergraph.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/interaction.py` & `discopy-1.1.4/test/syntax/interaction.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/markov.py` & `discopy-1.1.4/test/syntax/markov.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/monoidal.py` & `discopy-1.1.4/test/syntax/monoidal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/ribbon.py` & `discopy-1.1.4/test/syntax/ribbon.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/rigid.py` & `discopy-1.1.4/test/syntax/rigid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/symmetric.py` & `discopy-1.1.4/test/syntax/symmetric.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.3/test/syntax/utils.py` & `discopy-1.1.4/test/syntax/utils.py`

 * *Files identical despite different names*

