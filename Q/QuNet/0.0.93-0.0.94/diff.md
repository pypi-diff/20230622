# Comparing `tmp/QuNet-0.0.93-py3-none-any.whl.zip` & `tmp/QuNet-0.0.94-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 67650 bytes, number of entries: 28
+Zip file size: 67721 bytes, number of entries: 28
 -rw-rw-rw-  2.0 fat      519 b- defN 23-Jun-12 07:32 qunet/__init__.py
 -rw-rw-rw-  2.0 fat      616 b- defN 23-Apr-27 07:47 qunet/batch.py
 -rw-rw-rw-  2.0 fat     5703 b- defN 23-May-05 12:11 qunet/callback.py
 -rw-rw-rw-  2.0 fat     8843 b- defN 23-May-25 11:08 qunet/data.py
 -rw-rw-rw-  2.0 fat     2955 b- defN 23-May-28 11:12 qunet/losses.py
 -rw-rw-rw-  2.0 fat    23518 b- defN 23-Jun-21 08:44 qunet/modelstate.py
 -rw-rw-rw-  2.0 fat    16977 b- defN 23-Apr-20 12:40 qunet/old.py
--rw-rw-rw-  2.0 fat    10560 b- defN 23-Jun-21 12:04 qunet/plots.py
+-rw-rw-rw-  2.0 fat    10969 b- defN 23-Jun-22 11:47 qunet/plots.py
 -rw-rw-rw-  2.0 fat    53971 b- defN 23-Jun-22 07:47 qunet/trainer.py
 -rw-rw-rw-  2.0 fat     6545 b- defN 23-Jun-06 08:41 qunet/utils.py
 -rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-26 10:17 qunet/modules/__init__.py
 -rw-rw-rw-  2.0 fat    25379 b- defN 23-Jun-11 13:06 qunet/modules/cnn.py
 -rw-rw-rw-  2.0 fat     7964 b- defN 23-May-20 06:54 qunet/modules/cnn3D.py
 -rw-rw-rw-  2.0 fat     6302 b- defN 23-Apr-27 12:45 qunet/modules/gnn.py
 -rw-rw-rw-  2.0 fat     4470 b- defN 23-May-20 06:52 qunet/modules/mlp.py
@@ -18,13 +18,13 @@
 -rw-rw-rw-  2.0 fat     1594 b- defN 23-Jun-13 17:44 qunet/modules/total.py
 -rw-rw-rw-  2.0 fat    20312 b- defN 23-May-12 12:52 qunet/modules/transformer.py
 -rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-26 10:17 qunet/optim/__init__.py
 -rw-rw-rw-  2.0 fat     8517 b- defN 23-Jun-07 15:24 qunet/optim/adams.py
 -rw-rw-rw-  2.0 fat    14092 b- defN 23-Apr-25 10:33 qunet/optim/scheduler.py
 -rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-26 10:17 qunet/rl/__init__.py
 -rw-rw-rw-  2.0 fat    15969 b- defN 23-Jun-05 12:31 qunet/rl/dqn.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-Jun-22 07:49 QuNet-0.0.93.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    16131 b- defN 23-Jun-22 07:49 QuNet-0.0.93.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 07:49 QuNet-0.0.93.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-22 07:49 QuNet-0.0.93.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2122 b- defN 23-Jun-22 07:49 QuNet-0.0.93.dist-info/RECORD
-28 files, 257131 bytes uncompressed, 64326 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-Jun-22 11:49 QuNet-0.0.94.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    16131 b- defN 23-Jun-22 11:49 QuNet-0.0.94.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 11:49 QuNet-0.0.94.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-22 11:49 QuNet-0.0.94.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2122 b- defN 23-Jun-22 11:49 QuNet-0.0.94.dist-info/RECORD
+28 files, 257540 bytes uncompressed, 64397 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -63,23 +63,23 @@
 
 Filename: qunet/rl/__init__.py
 Comment: 
 
 Filename: qunet/rl/dqn.py
 Comment: 
 
-Filename: QuNet-0.0.93.dist-info/LICENSE
+Filename: QuNet-0.0.94.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.93.dist-info/METADATA
+Filename: QuNet-0.0.94.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.93.dist-info/WHEEL
+Filename: QuNet-0.0.94.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.93.dist-info/top_level.txt
+Filename: QuNet-0.0.94.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.93.dist-info/RECORD
+Filename: QuNet-0.0.94.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qunet/plots.py

```diff
@@ -55,16 +55,16 @@
     plt.suptitle(fr"samples={samples}, steps:{steps}; lr={lr}; batch=(trn:{bs_trn}, val:{bs_val}); time=(trn:{tm_trn}, val:{tm_val}){t_unit}/$10^{c_unit_power:.0f}$; params={hist.params/1e3:.0f}k", fontsize = 10)
 
     if  not view.loss.show:
         subplot_history(111, val, trn, view=view.score, view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='score')
     elif not view.score.show or (len(hist.trn.scores)==0 and len(hist.val.scores)==0):
         subplot_history(111, val, trn, view=view.loss,  view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='loss')
     else:
-        subplot_history(121, val, trn, view=view.score, view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='score')
-        subplot_history(122, val, trn, view=view.loss,  view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='loss')            
+        subplot_history(121, val, trn, view=view.loss,  view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='loss')            
+        subplot_history(122, val, trn, view=view.score, view_tot=view, c_unit=c_unit, c_unit_power=c_unit_power, unit=view.units.unit, labels=labels, kind='score')        
     if fname:
         plt.savefig(fname, bbox_inches='tight')
     else:
         plt.show()
 
     #---------------------------------------------------------------------------    
 
@@ -75,26 +75,30 @@
         if unit == 'samples':
             x_max = max(val.samples[-1], trn.samples[-1]) if view_tot.x_max is None else view_tot.x_max        
             ax1.set_xlim(view_tot.x_min/c_unit, x_max/c_unit)
         else:
             x_max = max(val.epochs[-1], trn.epochs[-1]) if view_tot.x_max is None else view_tot.x_max        
             ax1.set_xlim(view_tot.x_min, x_max)
 
-    if kind == 'loss':
-        
-        best_loss  = f"{val.best.loss:.4f}"    if val.best.loss is not None  else "?"
-        loss_val   = f"{val.losses[-1]:.4f}"   if len(val.losses)  else "?"
-        loss_trn   = f"{trn.losses[-1]:.4f}"   if len(trn.losses)  else "?"
-        plt.title(f"loss = (min: {best_loss} [{val.best.loss_epochs}], val: {loss_val}, trn: {loss_trn})", fontsize=12, pad=-2)
+    if kind == 'loss':        
+        best_loss   = f"{val.best.loss:.4f}"    if val.best.loss is not None  else "?"
+        loss_val    = f"{val.losses[-1]:.3f}"   if len(val.losses)  else "?"
+        loss_trn    = f"{trn.losses[-1]:.3f}"   if len(trn.losses)  else "?"
+        loss_trn_av = f"{np.mean(trn.losses[-30:]):.3f}"   if len(trn.losses)  else "?"
+        loss_val_av = f"{np.mean(val.losses[-30:]):.3f}"   if len(val.losses)  else "?"
+        plt.title(f"min: {best_loss} [{val.best.loss_epochs}], val: {loss_val_av}({loss_val}), trn: {loss_trn_av}({loss_trn})", fontsize=10, pad=-2)
 
     if kind == 'score':        
         best_score = f"{val.best.score:.4f}"   if val.best.score is not None else "?"
-        score_val  = f"{val.scores[-1]:.4f}"   if len(val.scores) else "?"
-        score_trn  = f"{trn.scores[-1]:.4f}"   if len(trn.scores) else "?"
-        plt.title(f"score = (bst: {best_score} [{val.best.score_epochs}], val: {score_val},  trn: {score_trn})", fontsize=12, pad=-2)
+        score_val  = f"{val.scores[-1]:.3f}"   if len(val.scores) else "?"
+        score_trn  = f"{trn.scores[-1]:.3f}"   if len(trn.scores) else "?"
+        score_trn_av = f"{np.mean(trn.scores[-30:]):.3f}"   if len(trn.losses)  else "?"
+        score_val_av = f"{np.mean(val.scores[-30:]):.3f}"   if len(val.losses)  else "?"
+
+        plt.title(f"bst: {best_score} [{val.best.score_epochs}], val: {score_val_av}({score_val}),  trn:  {score_trn_av}({score_trn})", fontsize=10, pad=-2)
 
     y_min, y_max = view.y_min, view.y_max
     ax1.set_xlabel(fr"$10^{c_unit_power:.0f}$ samples" if unit=='samples' else 'epochs'); ax1.set_ylabel(kind);                     
     if y_min is not None  and y_max is not None:            
         ax1.set_ylim(y_min, y_max)
         if view.ticks:
             ax1.set_yticks(np.linspace(y_min, y_max, view.ticks))
```

## Comparing `QuNet-0.0.93.dist-info/LICENSE` & `QuNet-0.0.94.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `QuNet-0.0.93.dist-info/METADATA` & `QuNet-0.0.94.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuNet
-Version: 0.0.93
+Version: 0.0.94
 Summary: Working with deep learning models
 Home-page: https://github.com/step137/qunet
 Author: synset
 Author-email: steps137ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `QuNet-0.0.93.dist-info/RECORD` & `QuNet-0.0.94.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 qunet/__init__.py,sha256=NSnUKrhrcHjtYOtYjqQE0qxv6NbhpRwUe2uQNlj6K9w,519
 qunet/batch.py,sha256=bBlUctBato37BkDMo69dH1icFvsCpOxH94ScYjKkwfc,616
 qunet/callback.py,sha256=Jic-Ehcg1uxRLX1Qr9H55gAfdIuX2ZdeNbGZEVw9Aq8,5703
 qunet/data.py,sha256=2oOEhaPyqXyuQd_KhaA8ZER_9c3AFzSaZnVG4JqFMAQ,8843
 qunet/losses.py,sha256=-euuc242iM5I8CXZgXTiG7R_hTOea0qUhlNug0D3Ijg,2955
 qunet/modelstate.py,sha256=vaZIJzanCrWCAdQBGLF4RWYGQW9PV-tL06P-rSdKBy0,23518
 qunet/old.py,sha256=wfsu9d4vcptlBT1lgPKHCfqDm8lirDvTTvEEzKGjTig,16977
-qunet/plots.py,sha256=IBS-Iak1O399igi0qmfSdp4rTPfaFzHEmYi_xsw5EJw,10560
+qunet/plots.py,sha256=9VcbB1CyB9kFvKLBjxvG8aQTzABpq-PemDD8nTAhPNw,10969
 qunet/trainer.py,sha256=zw_g-XZOPW7j4I-ayW33mm6TB4owWalraLlTzHnuELc,53971
 qunet/utils.py,sha256=85GOgOkATjgrditptjfBpVK174o5hLO-M7lyNm90lWA,6545
 qunet/modules/__init__.py,sha256=8ZRc1sGeVrPBx4lD717BgRaQekyh78QKV9SKsdt638U,3
 qunet/modules/cnn.py,sha256=GZctxAYDjeuWlg0U54LOl1p4qoVoAWOacqAfySxQqxg,25379
 qunet/modules/cnn3D.py,sha256=Q_htR1sNQccF6BbEjU8QPgJkuTnA910Fa-VfqaTGPgU,7964
 qunet/modules/gnn.py,sha256=FY3rc4hL6HtMYh_Yn9tGYNZqqvBn-Qdwx0O_HJcbuzk,6302
 qunet/modules/mlp.py,sha256=weqNleOfQWuOBXvORLmmVnsL-hG2aE6e3aXgFjG08EI,4470
@@ -17,12 +17,12 @@
 qunet/modules/total.py,sha256=wjjrX4g5gxkH0GSRsyYAMtTjr9KqRKi2zdO-T07Tvxo,1594
 qunet/modules/transformer.py,sha256=Q48tMEiDYR94h1CwRVwCp2p36rTMPu3UMvlCoYFjSDs,20312
 qunet/optim/__init__.py,sha256=8ZRc1sGeVrPBx4lD717BgRaQekyh78QKV9SKsdt638U,3
 qunet/optim/adams.py,sha256=UbaKMSaK3HHjuZKuyPxfLw2m2yrR8mD6CS3BKmCQ3K0,8517
 qunet/optim/scheduler.py,sha256=tAAgUS0LaAOPxVqxDsYAitF3ExX7Pt_dNK4XwzbTYdY,14092
 qunet/rl/__init__.py,sha256=8ZRc1sGeVrPBx4lD717BgRaQekyh78QKV9SKsdt638U,3
 qunet/rl/dqn.py,sha256=Ex18lo17luQuRUhaqaeLhO_IrT_s6ObJexiznSgxoSY,15969
-QuNet-0.0.93.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
-QuNet-0.0.93.dist-info/METADATA,sha256=LG2S3p2fM29Vm6NG9N7C1voP7tHxIuYhCcx4UxUL_2w,16131
-QuNet-0.0.93.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-QuNet-0.0.93.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
-QuNet-0.0.93.dist-info/RECORD,,
+QuNet-0.0.94.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
+QuNet-0.0.94.dist-info/METADATA,sha256=kyFgMVzAdOHeRqjMusa3fyNqRf7ykFEJNYm-z02QYNw,16131
+QuNet-0.0.94.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+QuNet-0.0.94.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
+QuNet-0.0.94.dist-info/RECORD,,
```

