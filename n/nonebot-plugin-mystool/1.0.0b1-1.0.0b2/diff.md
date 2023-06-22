# Comparing `tmp/nonebot_plugin_mystool-1.0.0b1.tar.gz` & `tmp/nonebot_plugin_mystool-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-1.0.0b1.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-1.0.0b2.tar", max compression
```

## Comparing `nonebot_plugin_mystool-1.0.0b1.tar` & `nonebot_plugin_mystool-1.0.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     3538 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/README.md
--rw-r--r--   0        0        0     1324 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     1794 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     4494 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    12122 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/data_model.py
--rw-r--r--   0        0        0    21278 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    10211 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/game_sign_api.py
--rw-r--r--   0        0        0     5467 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/good_image.py
--rw-r--r--   0        0        0     1959 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0     9562 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    21993 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/myb_missions_api.py
--rw-r--r--   0        0        0    22256 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0    10693 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/plugin_data.py
--rw-r--r--   0        0        0     8912 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    62140 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/simple_api.py
--rw-r--r--   0        0        0     2230 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/user_check.py
--rw-r--r--   0        0        0    11313 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/user_data.py
--rw-r--r--   0        0        0     9199 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     4110 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/README.md
+-rw-r--r--   0        0        0     1324 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1997 2023-06-22 08:40:33.037166 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     4494 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    12132 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/data_model.py
+-rw-r--r--   0        0        0    21315 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    11767 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/game_sign_api.py
+-rw-r--r--   0        0        0     5467 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/good_image.py
+-rw-r--r--   0        0        0     1959 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0     9562 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    21993 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/myb_missions_api.py
+-rw-r--r--   0        0        0    23357 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0    10775 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plugin_data.py
+-rw-r--r--   0        0        0     8912 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    63231 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/simple_api.py
+-rw-r--r--   0        0        0     2244 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_check.py
+-rw-r--r--   0        0        0    11313 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_data.py
+-rw-r--r--   0        0        0    10283 2023-06-22 08:40:33.041160 nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.0.0b2/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/LICENSE` & `nonebot_plugin_mystool-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/README.md` & `nonebot_plugin_mystool-1.0.0b2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,176 +47,211 @@
 000002e0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
 000002f0: 6769 6e2d 6d79 7354 6f6f 6c3f 7374 796c  gin-mysTool?styl
 00000300: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
 00000310: 3e0a 3c2f 6469 763e 0a0a 2320 6d79 7354  >.</div>..# mysT
 00000320: 6f6f 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8  ool - ..........
 00000330: be85 e58a a9e5 b7a5 e585 b7e6 8f92 e4bb  ................
 00000340: b60a 0a2a 2ae7 8988 e69c ac20 2d20 7631  ...**...... - v1
-00000350: 2e30 2e30 2d62 6574 612e 312a 2a0a 0a23  .0.0-beta.1**..#
+00000350: 2e30 2e30 2d62 6574 612e 322a 2a0a 0a23  .0.0-beta.2**..#
 00000360: 2323 20f0 9f93 a320 e69b b4e6 96b0 e586  ## .... ........
 00000370: 85e5 aeb9 0a0a 2323 2323 2032 3032 332e  ......#### 2023.
-00000380: 362e 3130 0a0a e694 b9e5 8aa8 e8be 83e5  6.10............
-00000390: a4a7 efbc 8ce7 9bae e589 8de6 98af 2042  .............. B
-000003a0: 6574 6120 e789 88ef bc8c e58f afe8 83bd  eta ............
-000003b0: e4b8 8de7 a8b3 e5ae 9a0a 0a2d 20e5 a4a7  ...........- ...
-000003c0: e987 8fe7 9a84 e4bb a3e7 a081 e987 8de6  ................
-000003d0: 9e84 efbc 8ce5 8c85 e68b ace7 b1b3 e6b8  ................
-000003e0: b8e7 a4be 4150 49e7 9a84 e5ae a2e6 88b7  ....API.........
-000003f0: e7ab afe5 ae9e e78e b0e3 8081 e794 a8e6  ................
-00000400: 88b7 e695 b0e6 8dae e79b b8e5 85b3 e380  ................
-00000410: 81e6 8f92 e4bb b6e9 858d e7bd aee7 9bb8  ................
-00000420: e585 b3e3 8081 4150 49e7 9bb8 e585 b3e6  ......API.......
-00000430: 95b0 e68d aee6 a8a1 e59e 8b0a 2d20 e4bf  ............- ..
-00000440: aee5 a48d e59c a820 5769 6e64 6f77 7320  ....... Windows 
-00000450: e4b8 8be6 97a0 e6b3 95e5 a49a e8bf 9be7  ................
-00000460: a88b e794 9fe6 8890 e595 86e5 9381 e59b  ................
-00000470: bee7 8987 e79a 84e9 97ae e9a2 980a 2d20  ..............- 
-00000480: e4bb 8ee6 98be e7a4 bae7 94a8 e688 b7e8  ................
-00000490: b4a6 e58f b7e7 bb91 e5ae 9ae7 9a84 e689  ................
-000004a0: 8be6 9cba e58f b7e6 94b9 e4b8 bae6 98be  ................
-000004b0: e7a4 bae8 b4a6 e58f b7e7 9a84 e7b1 b3e6  ................
-000004c0: b8b8 e7a4 be49 440a 2d20 e8ae bee7 bdae  .....ID.- ......
-000004d0: e380 81e5 8591 e68d a2e8 aea1 e588 92e5  ................
-000004e0: 8a9f e883 bde6 94af e68c 81e7 bea4 e881  ................
-000004f0: 8ae4 bdbf e794 a80a 2d20 e799 bbe9 9986  ........- ......
-00000500: e7bb 91e5 ae9a e58f aae9 9c80 e8a6 81e8  ................
-00000510: bf9b e8a1 8ce4 b880 e6ac a1e7 9fad e4bf  ................
-00000520: a1e9 aa8c e8af 810a 2d20 e794 a8e6 88b7  ........- ......
-00000530: e695 b0e6 8dae e696 87e4 bbb6 e380 81e6  ................
-00000540: 8f92 e4bb b6e9 858d e7bd aee6 9687 e4bb  ................
-00000550: b620 2a2a e6a0 bce5 bc8f e69b b4e6 96b0  . **............
-00000560: efbc 8ce4 b88e 2076 312e 302e 3020 e4b9  ...... v1.0.0 ..
-00000570: 8be5 898d e79a 84e7 8988 e69c ace4 b88d  ................
-00000580: e585 bce5 aeb9 2a2a 0a2d 20e4 bfae e5a4  ......**.- .....
-00000590: 8de6 b7bb e58a a0e5 8591 e68d a2e4 bbbb  ................
-000005a0: e58a a1e6 97b6 e587 bae7 8eb0 e79a 8455  ...............U
-000005b0: 4944 e4b8 8de5 ad98 e59c a8e9 9499 e8af  ID..............
-000005c0: af0a 2d20 e4bf aee5 a48d e595 86e5 9381  ..- ............
-000005d0: e59b bee7 8987 e794 9fe6 8890 e5ae 8ce6  ................
-000005e0: 898d e58f 91e5 87ba e590 8ee5 8fb0 e6ad  ................
-000005f0: a3e5 9ca8 e794 9fe6 8890 e68f 90e7 a4ba  ................
-00000600: e79a 84e9 97ae e9a2 980a 2d20 e5bc 82e5  ..........- ....
-00000610: b8b8 e68d 95e8 8eb7 e69b b4e5 8aa0 e587  ................
-00000620: 86e7 a1ae 0a2d 20e6 94b9 e8bf 9be4 ba86  .....- .........
-00000630: e4b8 80e4 ba9b e696 87e6 9cac 0a0a 2323  ..............##
-00000640: 2323 2032 3032 332e 352e 3138 0a2d 20e5  ## 2023.5.18.- .
-00000650: a49a e8bf 9be7 a88b e794 9fe6 8890 e595  ................
-00000660: 86e5 9381 e59b bee7 8987 efbc 88e5 a49a  ................
-00000670: e6a0 b8ef bc89 efbc 8ce5 8aa0 e5bf abe5  ................
-00000680: 9bbe e789 87e7 949f e688 90e9 809f e5ba  ................
-00000690: a60a 2d20 e4bf aee5 a48d e983 a8e5 8886  ..- ............
-000006a0: e595 86e5 9381 e585 91e6 8da2 e697 b6e9  ................
-000006b0: 97b4 e994 99e8 afaf e79a 84e9 97ae e9a2  ................
-000006c0: 98ef bc88 e5a6 82e7 b1b3 e6b8 b8e7 a4be  ................
-000006d0: e595 86e5 9381 e699 9ae4 ba86 e4b8 80e5  ................
-000006e0: 91a8 efbc 890a 0a23 2323 2320 3230 3233  .......#### 2023
-000006f0: 2e35 2e34 0a2d 20e5 a29e e58a a0e5 afb9  .5.4.- .........
-00000700: e698 9fe7 a9b9 e993 81e9 8193 e79a 84e7  ................
-00000710: adbe e588 b0e5 8a9f e883 bde7 9a84 e694  ................
-00000720: afe6 8c81 202d 205b 2338 395d 2868 7474  .... - [#89](htt
-00000730: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000740: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
-00000750: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
-00000760: 7075 6c6c 2f38 3929 2062 7920 4061 7961  pull/89) by @aya
-00000770: 6b61 7375 6b69 0a2d 20e4 bfae e5a4 8de6  kasuki.- .......
-00000780: 8f92 e4bb b6e5 91bd e4bb a4e4 bc98 e585  ................
-00000790: 88e5 baa6 e997 aee9 a298 202d 205b 2338  .......... - [#8
-000007a0: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
-000007b0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-000007c0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-000007d0: 7374 6f6f 6c2f 7075 6c6c 2f38 3829 2062  stool/pull/88) b
-000007e0: 7920 4061 7961 6b61 7375 6b69 0a2d 20e9  y @ayakasuki.- .
-000007f0: 83a8 e588 86e6 9687 e69c ace9 9499 e8af  ................
-00000800: afe4 bfae e6ad a320 2d20 5b23 3930 5d28  ....... - [#90](
-00000810: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000820: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
-00000830: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
-00000840: 6f6c 2f70 756c 6c2f 3930 2920 6279 2040  ol/pull/90) by @
-00000850: 626c 6163 6b2d 7a65 726f 3335 380a 0a2e  black-zero358...
-00000860: 2e2e 0a0a 2323 2323 2032 3032 332e 332e  ....#### 2023.3.
-00000870: 3330 0a2d 20e4 bfae e5a4 8d20 602f e585  30.- ...... `/..
-00000880: 91e6 8da2 6020 e591 bde4 bba4 e58f afe8  ....` ..........
-00000890: 83bd e4b8 8ee5 85b6 e4bb 96e6 8f92 e4bb  ................
-000008a0: b6e5 91bd e4bb a4e5 86b2 e7aa 81e7 9a84  ................
-000008b0: e997 aee9 a298 efbc 8ce5 908c e697 b620  ............... 
-000008c0: 5bf0 9f94 97e7 94a8 e6b3 95e5 8f98 e69b  [...............
-000008d0: b45d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
-000008e0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-000008f0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000900: 7374 6f6f 6c2f 7769 6b69 2f49 6e66 6f72  stool/wiki/Infor
-00000910: 6d61 7469 6f6e 2d45 7863 6861 6e67 6523  mation-Exchange#
-00000920: e5a2 9ee5 8aa0 e588 a0e9 99a4 e585 91e6  ................
-00000930: 8da2 e8ae a1e5 8892 290a 2d20 2e2e 2e0a  ........).- ....
-00000940: 0a23 2320 e58a 9fe8 83bd e592 8ce7 89b9  .## ............
-00000950: e680 a70a 0a2d 20e7 9fad e4bf a1e9 aa8c  .....- .........
-00000960: e8af 81e7 99bb e5bd 95ef bc8c e585 8de6  ................
-00000970: 8a93 e58c 85e8 8eb7 e58f 9620 436f 6f6b  ........... Cook
-00000980: 6965 0a2d 20e8 87aa e58a a8e5 ae8c e688  ie.- ...........
-00000990: 90e6 af8f e697 a5e7 b1b3 e6b8 b8e5 b881  ................
-000009a0: e4bb bbe5 8aa1 0a2d 20e8 87aa e58a a8e8  .......- .......
-000009b0: bf9b e8a1 8ce6 b8b8 e688 8fe7 adbe e588  ................
-000009c0: b00a 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3  ..- ............
-000009d0: e6b8 b8e5 b881 e595 86e5 9381 e585 91e6  ................
-000009e0: 8da2 e8ae a1e5 8892 efbc 8ce5 88b0 e782  ................
-000009f0: b9e5 8591 e68d a20a 2d20 e58f afe6 94af  ........- ......
-00000a00: e68c 81e5 a49a e4b8 aa20 5151 20e8 b4a6  ......... QQ ...
-00000a10: e58f b7ef bc8c e6af 8fe4 b8aa 2051 5120  ............ QQ 
-00000a20: e8b4 a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5  ................
-00000a30: a49a e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4  ................
-00000a40: a6e6 88b7 0a2d 2051 5120 e68e a8e9 8081  .....- QQ ......
-00000a50: e689 a7e8 a18c e7bb 93e6 9e9c e980 9ae7  ................
-00000a60: 9fa5 0a2d 20e5 8e9f e7a5 9ee6 a091 e884  ...- ...........
-00000a70: 82e3 8081 e6b4 9ee5 a4a9 e5ae 9de9 92b1  ................
-00000a80: e380 81e8 b4a8 e987 8fe5 8f82 e58f 98e4  ................
-00000a90: bbaa e5b7 b2e6 bba1 e697 b6e6 8ea8 e980  ................
-00000aa0: 81e9 809a e79f a50a 0a23 2320 e4bd bfe7  .........## ....
-00000ab0: 94a8 e8af b4e6 988e 0a0a 2323 2320 f09f  ..........### ..
-00000ac0: 9ba0 efb8 8f20 4e6f 6e65 426f 7432 20e6  ..... NoneBot2 .
-00000ad0: 9cba e599 a8e4 baba e983 a8e7 bdb2 e592  ................
-00000ae0: 8ce6 8f92 e4bb b6e5 ae89 e8a3 850a 0ae8  ................
-00000af0: afb7 e69f a5e7 9c8b 202d 3e20 5bf0 9f94  ........ -> [...
-00000b00: 9749 6e73 7461 6c6c 6174 696f 6e5d 2868  .Installation](h
+00000380: 362e 3232 202d 2076 312e 302e 302d 6265  6.22 - v1.0.0-be
+00000390: 7461 2e32 0ae6 94b9 e58a a8e8 be83 e5a4  ta.2............
+000003a0: a7ef bc8c e79b aee5 898d e698 af20 4265  ............. Be
+000003b0: 7461 20e7 8988 efbc 8ce5 8faf e883 bde4  ta .............
+000003c0: b88d e7a8 b3e5 ae9a 0a0a 5769 6e64 6f77  ..........Window
+000003d0: 73e3 8081 6d61 634f 5320 e4b8 8be6 97a0  s...macOS ......
+000003e0: e6b3 95e5 a49a e8bf 9be7 a88b e794 9fe6  ................
+000003f0: 8890 e595 86e5 9381 e59b bee7 8987 e79a  ................
+00000400: 84e9 97ae e9a2 98e6 9a82 e697 b6e6 b2a1  ................
+00000410: e69c 89e4 bfae e5a4 8d0a 0a2d 20e6 94af  ...........- ...
+00000420: e68c 81e4 bdbf e794 a8e4 baba e69c bae9  ................
+00000430: aa8c e8af 81e6 8993 e7a0 81e5 b9b3 e58f  ................
+00000440: b0e5 a484 e790 86e4 baba e69c bae9 aa8c  ................
+00000450: e8af 81e4 bbbb e58a a120 5b23 3131 395d  ......... [#119]
+00000460: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000470: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
+00000480: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
+00000490: 6f6f 6c2f 7075 6c6c 2f31 3139 2920 6279  ool/pull/119) by
+000004a0: 2040 4e69 6768 742d 7374 6172 732d 310a   @Night-stars-1.
+000004b0: 2d20 e58e 9fe7 a59e e4be bfe7 acba e88e  - ..............
+000004c0: b7e5 8f96 e5a4 b1e8 b4a5 e697 b6e6 9bb4  ................
+000004d0: e68d a2e4 b8ba e4bd bfe7 94a8 e7b1 b3e6  ................
+000004e0: b8b8 e7a4 be69 4f53 e5b0 8fe7 bb84 e4bb  .....iOS........
+000004f0: b641 5049 e88e b7e5 8f96 205b 2331 3139  .API...... [#119
+00000500: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000510: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00000520: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00000530: 746f 6f6c 2f70 756c 6c2f 3131 3929 2062  tool/pull/119) b
+00000540: 7920 404e 6967 6874 2d73 7461 7273 2d31  y @Night-stars-1
+00000550: 0a2d 20e4 bfae e5a4 8de5 8e9f e7a5 9ee4  .- .............
+00000560: bebf e7ac bae5 928c e8ae a8e8 aeba e58c  ................
+00000570: bae7 adbe e588 b0e5 8faf e883 bde5 9ba0  ................
+00000580: e4b8 ba44 53e6 97a0 e695 88e8 808c e5a4  ...DS...........
+00000590: b1e8 b4a5 e79a 84e9 97ae e9a2 980a 0a23  ...............#
+000005a0: 2323 2320 3230 3233 2e36 2e31 3020 2d20  ### 2023.6.10 - 
+000005b0: 7631 2e30 2e30 2d62 6574 612e 310a e694  v1.0.0-beta.1...
+000005c0: b9e5 8aa8 e8be 83e5 a4a7 efbc 8ce7 9bae  ................
+000005d0: e589 8de6 98af 2042 6574 6120 e789 88ef  ...... Beta ....
+000005e0: bc8c e58f afe8 83bd e4b8 8de7 a8b3 e5ae  ................
+000005f0: 9a0a 0a2d 20e5 a4a7 e987 8fe7 9a84 e4bb  ...- ...........
+00000600: a3e7 a081 e987 8de6 9e84 efbc 8ce5 8c85  ................
+00000610: e68b ace7 b1b3 e6b8 b8e7 a4be 4150 49e7  ............API.
+00000620: 9a84 e5ae a2e6 88b7 e7ab afe5 ae9e e78e  ................
+00000630: b0e3 8081 e794 a8e6 88b7 e695 b0e6 8dae  ................
+00000640: e79b b8e5 85b3 e380 81e6 8f92 e4bb b6e9  ................
+00000650: 858d e7bd aee7 9bb8 e585 b3e3 8081 4150  ..............AP
+00000660: 49e7 9bb8 e585 b3e6 95b0 e68d aee6 a8a1  I...............
+00000670: e59e 8b0a 2d20 7e7e e4bf aee5 a48d e59c  ....- ~~........
+00000680: a820 5769 6e64 6f77 7320 e4b8 8be6 97a0  . Windows ......
+00000690: e6b3 95e5 a49a e8bf 9be7 a88b e794 9fe6  ................
+000006a0: 8890 e595 86e5 9381 e59b bee7 8987 e79a  ................
+000006b0: 84e9 97ae e9a2 987e 7e0a 2d20 e4bb 8ee6  .......~~.- ....
+000006c0: 98be e7a4 bae7 94a8 e688 b7e8 b4a6 e58f  ................
+000006d0: b7e7 bb91 e5ae 9ae7 9a84 e689 8be6 9cba  ................
+000006e0: e58f b7e6 94b9 e4b8 bae6 98be e7a4 bae8  ................
+000006f0: b4a6 e58f b7e7 9a84 e7b1 b3e6 b8b8 e7a4  ................
+00000700: be49 440a 2d20 e8ae bee7 bdae e380 81e5  .ID.- ..........
+00000710: 8591 e68d a2e8 aea1 e588 92e5 8a9f e883  ................
+00000720: bde6 94af e68c 81e7 bea4 e881 8ae4 bdbf  ................
+00000730: e794 a80a 2d20 e799 bbe9 9986 e7bb 91e5  ....- ..........
+00000740: ae9a e58f aae9 9c80 e8a6 81e8 bf9b e8a1  ................
+00000750: 8ce4 b880 e6ac a1e7 9fad e4bf a1e9 aa8c  ................
+00000760: e8af 810a 2d20 e794 a8e6 88b7 e695 b0e6  ....- ..........
+00000770: 8dae e696 87e4 bbb6 e380 81e6 8f92 e4bb  ................
+00000780: b6e9 858d e7bd aee6 9687 e4bb b620 2a2a  ............. **
+00000790: e6a0 bce5 bc8f e69b b4e6 96b0 efbc 8ce4  ................
+000007a0: b88e 2076 312e 302e 3020 e4b9 8be5 898d  .. v1.0.0 ......
+000007b0: e79a 84e7 8988 e69c ace4 b88d e585 bce5  ................
+000007c0: aeb9 2a2a 0a2d 20e4 bfae e5a4 8de6 b7bb  ..**.- .........
+000007d0: e58a a0e5 8591 e68d a2e4 bbbb e58a a1e6  ................
+000007e0: 97b6 e587 bae7 8eb0 e79a 8455 4944 e4b8  ...........UID..
+000007f0: 8de5 ad98 e59c a8e9 9499 e8af af0a 2d20  ..............- 
+00000800: e4bf aee5 a48d e595 86e5 9381 e59b bee7  ................
+00000810: 8987 e794 9fe6 8890 e5ae 8ce6 898d e58f  ................
+00000820: 91e5 87ba e590 8ee5 8fb0 e6ad a3e5 9ca8  ................
+00000830: e794 9fe6 8890 e68f 90e7 a4ba e79a 84e9  ................
+00000840: 97ae e9a2 980a 2d20 e5bc 82e5 b8b8 e68d  ......- ........
+00000850: 95e8 8eb7 e69b b4e5 8aa0 e587 86e7 a1ae  ................
+00000860: 0a2d 20e6 94b9 e8bf 9be4 ba86 e4b8 80e4  .- .............
+00000870: ba9b e696 87e6 9cac 0a0a 2323 2323 2032  ..........#### 2
+00000880: 3032 332e 352e 3138 0a2d 20e5 a49a e8bf  023.5.18.- .....
+00000890: 9be7 a88b e794 9fe6 8890 e595 86e5 9381  ................
+000008a0: e59b bee7 8987 efbc 88e5 a49a e6a0 b8ef  ................
+000008b0: bc89 efbc 8ce5 8aa0 e5bf abe5 9bbe e789  ................
+000008c0: 87e7 949f e688 90e9 809f e5ba a60a 2d20  ..............- 
+000008d0: e4bf aee5 a48d e983 a8e5 8886 e595 86e5  ................
+000008e0: 9381 e585 91e6 8da2 e697 b6e9 97b4 e994  ................
+000008f0: 99e8 afaf e79a 84e9 97ae e9a2 98ef bc88  ................
+00000900: e5a6 82e7 b1b3 e6b8 b8e7 a4be e595 86e5  ................
+00000910: 9381 e699 9ae4 ba86 e4b8 80e5 91a8 efbc  ................
+00000920: 890a 0a23 2323 2320 3230 3233 2e35 2e34  ...#### 2023.5.4
+00000930: 0a2d 20e5 a29e e58a a0e5 afb9 e698 9fe7  .- .............
+00000940: a9b9 e993 81e9 8193 e79a 84e7 adbe e588  ................
+00000950: b0e5 8a9f e883 bde7 9a84 e694 afe6 8c81  ................
+00000960: 202d 205b 2338 395d 2868 7474 7073 3a2f   - [#89](https:/
+00000970: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
+00000980: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
+00000990: 6769 6e2d 6d79 7374 6f6f 6c2f 7075 6c6c  gin-mystool/pull
+000009a0: 2f38 3929 2062 7920 4061 7961 6b61 7375  /89) by @ayakasu
+000009b0: 6b69 0a2d 20e4 bfae e5a4 8de6 8f92 e4bb  ki.- ...........
+000009c0: b6e5 91bd e4bb a4e4 bc98 e585 88e5 baa6  ................
+000009d0: e997 aee9 a298 202d 205b 2338 385d 2868  ...... - [#88](h
+000009e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000009f0: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
+00000a00: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
+00000a10: 6c2f 7075 6c6c 2f38 3829 2062 7920 4061  l/pull/88) by @a
+00000a20: 7961 6b61 7375 6b69 0a2d 20e9 83a8 e588  yakasuki.- .....
+00000a30: 86e6 9687 e69c ace9 9499 e8af afe4 bfae  ................
+00000a40: e6ad a320 2d20 5b23 3930 5d28 6874 7470  ... - [#90](http
+00000a50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00000a60: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+00000a70: 706c 7567 696e 2d6d 7973 746f 6f6c 2f70  plugin-mystool/p
+00000a80: 756c 6c2f 3930 2920 6279 2040 626c 6163  ull/90) by @blac
+00000a90: 6b2d 7a65 726f 3335 380a 0a2e 2e2e 0a0a  k-zero358.......
+00000aa0: 2323 2323 2032 3032 332e 332e 3330 0a2d  #### 2023.3.30.-
+00000ab0: 20e4 bfae e5a4 8d20 602f e585 91e6 8da2   ...... `/......
+00000ac0: 6020 e591 bde4 bba4 e58f afe8 83bd e4b8  ` ..............
+00000ad0: 8ee5 85b6 e4bb 96e6 8f92 e4bb b6e5 91bd  ................
+00000ae0: e4bb a4e5 86b2 e7aa 81e7 9a84 e997 aee9  ................
+00000af0: a298 efbc 8ce5 908c e697 b620 5bf0 9f94  ........... [...
+00000b00: 97e7 94a8 e6b3 95e5 8f98 e69b b45d 2868  .............](h
 00000b10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000b20: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
 00000b30: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000b40: 6c2f 7769 6b69 2f49 6e73 7461 6c6c 6174  l/wiki/Installat
-00000b50: 696f 6e29 0a0a 2323 2320 f09f 9396 20e6  ion)..### .... .
-00000b60: 8f92 e4bb b6e5 85b7 e4bd 93e4 bdbf e794  ................
-00000b70: a8e8 afb4 e698 8e0a 0ae8 afb7 e69f a5e7  ................
-00000b80: 9c8b 202d 3e20 5bf0 9f94 9757 696b 6920  .. -> [....Wiki 
-00000b90: e696 87e6 a1a3 5d28 6874 7470 733a 2f2f  ......](https://
-00000ba0: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
-00000bb0: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
-00000bc0: 696e 2d6d 7973 746f 6f6c 2f77 696b 6929  in-mystool/wiki)
-00000bd0: 0a0a 2323 2320 e29d 9320 e88e b7e5 8f96  ..### ... ......
-00000be0: e68f 92e4 bbb6 e5b8 aee5 8aa9 e4bf a1e6  ................
-00000bf0: 81af 0a0a 2323 2323 20e6 8f92 e4bb b6e5  ....#### .......
-00000c00: 91bd e4bb a40a 0a60 6060 0a2f e5b8 aee5  .......```./....
-00000c10: 8aa9 0a60 6060 0a0a 3e20 e29a a0ef b88f  ...```..> ......
-00000c20: 20e6 b3a8 e684 8f20 e6ad a4e5 a484 e6b2   ...... ........
-00000c30: a1e6 9c89 e4bd bfe7 94a8 205b f09f 9497  .......... [....
-00000c40: 20e6 8f92 e4bb b6e5 91bd e4bb a4e5 a4b4   ...............
-00000c50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000c60: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
-00000c70: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00000c80: 746f 6f6c 2f77 696b 692f 436f 6e66 6967  tool/wiki/Config
-00000c90: 7572 6174 696f 6e2d 436f 6e66 6967 2363  uration-Config#c
-00000ca0: 6f6d 6d61 6e64 7374 6172 7429 0a0a 2323  ommandstart)..##
-00000cb0: 20e5 85b6 e4bb 960a 0a23 2323 205b f09f   ........### [..
-00000cc0: 9383 e6ba 90e7 a081 e8af b4e6 988e 5d28  ..............](
-00000cd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ce0: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
-00000cf0: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
-00000d00: 6f6c 2f77 696b 692f 536f 7572 6365 2d53  ol/wiki/Source-S
-00000d10: 7472 7563 7475 7265 290a 2323 2320 e980  tructure).### ..
-00000d20: 82e9 858d 205b e7bb aae5 b1b1 e79c 9fe5  .... [..........
-00000d30: afbb 426f 745d 2868 7474 7073 3a2f 2f67  ..Bot](https://g
-00000d40: 6974 6875 622e 636f 6d2f 4869 6269 4b69  ithub.com/HibiKi
-00000d50: 6572 2f7a 6865 6e78 756e 5f62 6f74 2920  er/zhenxun_bot) 
-00000d60: e79a 84e5 8886 e694 af0a 2d20 6874 7470  ..........- http
-00000d70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
-00000d80: 5754 4a43 2f7a 6865 6e78 756e 2d70 6c75  WTJC/zhenxun-plu
-00000d90: 6769 6e2d 6d79 7374 6f6f 6c0a 2d20 6874  gin-mystool.- ht
-00000da0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000db0: 2f61 7961 6b61 7375 6b69 2f6e 6f6e 6562  /ayakasuki/noneb
-00000dc0: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000dd0: 6c0a                                     l.
+00000b40: 6c2f 7769 6b69 2f49 6e66 6f72 6d61 7469  l/wiki/Informati
+00000b50: 6f6e 2d45 7863 6861 6e67 6523 e5a2 9ee5  on-Exchange#....
+00000b60: 8aa0 e588 a0e9 99a4 e585 91e6 8da2 e8ae  ................
+00000b70: a1e5 8892 290a 2d20 2e2e 2e0a 0a23 2320  ....).- .....## 
+00000b80: e58a 9fe8 83bd e592 8ce7 89b9 e680 a70a  ................
+00000b90: 0a2d 20e7 9fad e4bf a1e9 aa8c e8af 81e7  .- .............
+00000ba0: 99bb e5bd 95ef bc8c e585 8de6 8a93 e58c  ................
+00000bb0: 85e8 8eb7 e58f 9620 436f 6f6b 6965 0a2d  ....... Cookie.-
+00000bc0: 20e8 87aa e58a a8e5 ae8c e688 90e6 af8f   ...............
+00000bd0: e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb bbe5  ................
+00000be0: 8aa1 0a2d 20e8 87aa e58a a8e8 bf9b e8a1  ...- ...........
+00000bf0: 8ce6 b8b8 e688 8fe7 adbe e588 b00a 2d20  ..............- 
+00000c00: e58f afe5 88b6 e5ae 9ae7 b1b3 e6b8 b8e5  ................
+00000c10: b881 e595 86e5 9381 e585 91e6 8da2 e8ae  ................
+00000c20: a1e5 8892 efbc 8ce5 88b0 e782 b9e5 8591  ................
+00000c30: e68d a20a 2d20 e58f afe6 94af e68c 81e5  ....- ..........
+00000c40: a49a e4b8 aa20 5151 20e8 b4a6 e58f b7ef  ..... QQ .......
+00000c50: bc8c e6af 8fe4 b8aa 2051 5120 e8b4 a6e5  ........ QQ ....
+00000c60: 8fb7 e58f afe7 bb91 e5ae 9ae5 a49a e4b8  ................
+00000c70: aae7 b1b3 e593 88e6 b8b8 e8b4 a6e6 88b7  ................
+00000c80: 0a2d 2051 5120 e68e a8e9 8081 e689 a7e8  .- QQ ..........
+00000c90: a18c e7bb 93e6 9e9c e980 9ae7 9fa5 0a2d  ...............-
+00000ca0: 20e5 8e9f e7a5 9ee6 a091 e884 82e3 8081   ...............
+00000cb0: e6b4 9ee5 a4a9 e5ae 9de9 92b1 e380 81e8  ................
+00000cc0: b4a8 e987 8fe5 8f82 e58f 98e4 bbaa e5b7  ................
+00000cd0: b2e6 bba1 e697 b6e6 8ea8 e980 81e9 809a  ................
+00000ce0: e79f a50a 0a23 2320 e4bd bfe7 94a8 e8af  .....## ........
+00000cf0: b4e6 988e 0a0a 2323 2320 f09f 9ba0 efb8  ......### ......
+00000d00: 8f20 4e6f 6e65 426f 7432 20e6 9cba e599  . NoneBot2 .....
+00000d10: a8e4 baba e983 a8e7 bdb2 e592 8ce6 8f92  ................
+00000d20: e4bb b6e5 ae89 e8a3 850a 0ae8 afb7 e69f  ................
+00000d30: a5e7 9c8b 202d 3e20 5bf0 9f94 9749 6e73  .... -> [....Ins
+00000d40: 7461 6c6c 6174 696f 6e5d 2868 7474 7073  tallation](https
+00000d50: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
+00000d60: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
+00000d70: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
+00000d80: 6b69 2f49 6e73 7461 6c6c 6174 696f 6e29  ki/Installation)
+00000d90: 0a0a 2323 2320 f09f 9396 20e6 8f92 e4bb  ..### .... .....
+00000da0: b6e5 85b7 e4bd 93e4 bdbf e794 a8e8 afb4  ................
+00000db0: e698 8e0a 0ae8 afb7 e69f a5e7 9c8b 202d  .............. -
+00000dc0: 3e20 5bf0 9f94 9757 696b 6920 e696 87e6  > [....Wiki ....
+00000dd0: a1a3 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
+00000de0: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
+00000df0: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
+00000e00: 7973 746f 6f6c 2f77 696b 6929 0a0a 2323  ystool/wiki)..##
+00000e10: 2320 e29d 9320 e88e b7e5 8f96 e68f 92e4  # ... ..........
+00000e20: bbb6 e5b8 aee5 8aa9 e4bf a1e6 81af 0a0a  ................
+00000e30: 2323 2323 20e6 8f92 e4bb b6e5 91bd e4bb  #### ...........
+00000e40: a40a 0a60 6060 0a2f e5b8 aee5 8aa9 0a60  ...```./.......`
+00000e50: 6060 0a0a 3e20 e29a a0ef b88f 20e6 b3a8  ``..> ...... ...
+00000e60: e684 8f20 e6ad a4e5 a484 e6b2 a1e6 9c89  ... ............
+00000e70: e4bd bfe7 94a8 205b f09f 9497 20e6 8f92  ...... [.... ...
+00000e80: e4bb b6e5 91bd e4bb a4e5 a4b4 5d28 6874  ............](ht
+00000e90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000ea0: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
+00000eb0: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
+00000ec0: 2f77 696b 692f 436f 6e66 6967 7572 6174  /wiki/Configurat
+00000ed0: 696f 6e2d 436f 6e66 6967 2363 6f6d 6d61  ion-Config#comma
+00000ee0: 6e64 7374 6172 7429 0a0a 2323 20e5 85b6  ndstart)..## ...
+00000ef0: e4bb 960a 0a23 2323 205b f09f 9383 e6ba  .....### [......
+00000f00: 90e7 a081 e8af b4e6 988e 5d28 6874 7470  ..........](http
+00000f10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00000f20: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+00000f30: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
+00000f40: 696b 692f 536f 7572 6365 2d53 7472 7563  iki/Source-Struc
+00000f50: 7475 7265 290a 2323 2320 e980 82e9 858d  ture).### ......
+00000f60: 205b e7bb aae5 b1b1 e79c 9fe5 afbb 426f   [............Bo
+00000f70: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00000f80: 622e 636f 6d2f 4869 6269 4b69 6572 2f7a  b.com/HibiKier/z
+00000f90: 6865 6e78 756e 5f62 6f74 2920 e79a 84e5  henxun_bot) ....
+00000fa0: 8886 e694 af0a 2d20 6874 7470 733a 2f2f  ......- https://
+00000fb0: 6769 7468 7562 2e63 6f6d 2f4d 5754 4a43  github.com/MWTJC
+00000fc0: 2f7a 6865 6e78 756e 2d70 6c75 6769 6e2d  /zhenxun-plugin-
+00000fd0: 6d79 7374 6f6f 6c0a 2d20 6874 7470 733a  mystool.- https:
+00000fe0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7961  //github.com/aya
+00000ff0: 6b61 7375 6b69 2f6e 6f6e 6562 6f74 2d70  kasuki/nonebot-p
+00001000: 6c75 6769 6e2d 6d79 7374 6f6f 6c0a       lugin-mystool.
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/pyproject.toml` & `nonebot_plugin_mystool-1.0.0b2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v1.0.0-beta.1"
+version = "v1.0.0-beta.2"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,13 +25,20 @@
     \n⚠️你的数据将经过机器人服务器，请确定你信任服务器所有者再使用。\
     \n\n🔗项目地址：https://github.com/Ljzd-PRO/nonebot-plugin-mystool\
     \n🔗详细使用说明：https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki
     """.strip(),
     extra={"version": VERSION}
 )
 
+# 在此处使用 get_driver() 防止多进程生成图片时反复调用
+
+from .utils import CommandBegin
+from nonebot import get_driver
+
+get_driver().on_startup(CommandBegin.set_command_begin)
+
 # 加载其它代码
 
 FILE_PATH = Path(__file__).parent.absolute()
 
 for _, file, _ in pkgutil.iter_modules([str(FILE_PATH)]):
     __import__(file, globals(), level=1)
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/address.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/data_model.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,15 +354,15 @@
     """探索派遣 进行中的数量"""
     max_expedition_num: int
     """探索派遣 最多派遣数"""
     current_home_coin: int
     """洞天财瓮 未收取的宝钱数"""
     max_home_coin: int
     """洞天财瓮 最多可容纳宝钱数"""
-    transformer: Dict[str, Any]
+    transformer: Optional[Dict[str, Any]]
     """参量质变仪相关数据"""
 
     @property
     def transformer_text(self):
         """
         参量质变仪状态文本
         """
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,31 +8,33 @@
 import time
 from datetime import datetime
 from multiprocessing import Manager
 from multiprocessing.pool import Pool
 from multiprocessing.synchronize import Lock
 from typing import List, Union, Callable, Any, Tuple, Optional, Dict
 
+import nonebot
 from apscheduler.events import JobExecutionEvent, EVENT_JOB_EXECUTED
 from nonebot import on_command, get_bot
 from nonebot.adapters.onebot.v11 import (MessageEvent, MessageSegment,
                                          PrivateMessageEvent, GroupMessageEvent)
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.matcher import Matcher
 from nonebot.params import ArgStr, ArgPlainText, T_State, CommandArg, Command
 from nonebot_plugin_apscheduler import scheduler
 
 from .data_model import Good, GameRecord, ExchangeStatus
 from .good_image import game_list_to_image
 from .plugin_data import PluginDataManager, write_plugin_data
 from .simple_api import get_game_record, get_good_detail, get_good_list, good_exchange_sync
 from .user_data import UserAccount, ExchangePlan, ExchangeResult
-from .utils import NtpTime, COMMAND_BEGIN, logger, _driver, get_last_command_sep
+from .utils import NtpTime, COMMAND_BEGIN, logger, get_last_command_sep
 
 _conf = PluginDataManager.plugin_data_obj
+_driver = nonebot.get_driver()
 
 myb_exchange_plan = on_command(f"{_conf.preference.command_start}兑换",
                                aliases={(f"{_conf.preference.command_start}兑换", "+"),
                                         (f"{_conf.preference.command_start}兑换", "-")},
                                priority=5, block=True)
 myb_exchange_plan.name = "兑换"
 myb_exchange_plan.usage = "跟随指引，配置米游币商品自动兑换计划。添加计划之前，请先前往米游社设置好收货地址，" \
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/game_sign_api.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/game_sign_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 ### 米游社的游戏签到相关API
 """
-from typing import List, Optional, Tuple, Literal, Set, Type
+from typing import List, Optional, Tuple, Literal, Set, Type, Callable, Any
 from urllib.parse import urlencode
 
 import httpx
 import tenacity
 
-from .data_model import GameRecord, BaseApiStatus, Award, GameSignInfo
+from .data_model import GameRecord, BaseApiStatus, Award, GameSignInfo, GeetestResult
 from .plugin_data import PluginDataManager
 from .simple_api import ApiResultHandler, HEADERS_API_TAKUMI_MOBILE, is_incorrect_return, device_login, device_save
 from .user_data import UserAccount
 from .utils import logger, generate_ds, \
-    get_async_retry
+    get_async_retry, get_validate
 
 _conf = PluginDataManager.plugin_data_obj
 
 
 class BaseGameSign:
     """
     游戏签到基类
@@ -126,19 +126,23 @@
                 logger.exception(f"获取签到数据 - 服务器没有正确返回")
                 logger.debug(f"网络请求返回: {res.text}")
                 return BaseApiStatus(incorrect_return=True), None
             else:
                 logger.exception(f"获取签到数据 - 请求失败")
                 return BaseApiStatus(network_error=True), None
 
-    async def sign(self, platform: Literal["ios", "android"] = "ios", retry: bool = True) -> BaseApiStatus:
+    async def sign(self,
+                   platform: Literal["ios", "android"] = "ios",
+                   on_geetest_callback: Callable[[], Any] = None,
+                   retry: bool = True) -> BaseApiStatus:
         """
         签到
 
         :param platform: 设备平台
+        :param on_geetest_callback: 开始尝试进行人机验证时调用的回调函数
         :param retry: 是否允许重试
         """
         if not self.record:
             return BaseApiStatus(success=True)
         content = {
             "act_id": self.ACT_ID,
             "region": self.record.region,
@@ -156,43 +160,72 @@
             headers["x-rpc-channel"] = _conf.device_config.X_RPC_CHANNEL_ANDROID
             headers["x-rpc-sys_version"] = _conf.device_config.X_RPC_SYS_VERSION_ANDROID
             headers["x-rpc-client_type"] = "2"
             headers.pop("x-rpc-platform")
             await device_login(self.account)
             await device_save(self.account)
             headers["DS"] = generate_ds(platform="android")
+
+        challenge = ""
+        """人机验证任务 challenge"""
+        geetest_result = GeetestResult("", "")
+        """人机验证结果"""
+
         try:
             async for attempt in get_async_retry(retry):
                 with attempt:
+                    if geetest_result.validate:
+                        headers["x-rpc-validate"] = geetest_result.validate
+                        headers["x-rpc-challenge"] = challenge
+                        headers["x-rpc-seccode"] = f'{geetest_result.validate}|jordan'
+
                     async with httpx.AsyncClient() as client:
-                        res = await client.post(self.URL_SIGN, headers=headers, cookies=self.account.cookies.dict(),
-                                                timeout=_conf.preference.timeout, json=content)
+                        res = await client.post(
+                            self.URL_SIGN,
+                            headers=headers,
+                            cookies=self.account.cookies.dict(),
+                            timeout=_conf.preference.timeout,
+                            json=content
+                        )
 
                     api_result = ApiResultHandler(res.json())
                     if api_result.login_expired:
                         logger.info(
                             f"游戏签到 - 用户 {self.account.bbs_uid} 登录失效")
                         logger.debug(f"网络请求返回: {res.text}")
                         return BaseApiStatus(login_expired=True)
                     if api_result.invalid_ds:
                         logger.info(
                             f"游戏签到 - 用户 {self.account.bbs_uid} DS 校验失败")
                         logger.debug(f"网络请求返回: {res.text}")
                         return BaseApiStatus(invalid_ds=True)
                     if api_result.data.get("risk_code") != 0:
                         logger.warning(
-                            f"{_conf.LOG_HEAD}游戏签到 - 用户 {self.account.bbs_uid} 可能被验证码阻拦")
-                        logger.debug(f"{_conf.LOG_HEAD}网络请求返回: {res.text}")
-                        return BaseApiStatus(need_verify=True)
-                    return BaseApiStatus(success=True)
+                            f"{_conf.preference.log_head}游戏签到 - 用户 {self.account.bbs_uid} 可能被人机验证阻拦")
+                        logger.debug(f"{_conf.preference.log_head}网络请求返回: {res.text}")
+                        gt = api_result.data.get("gt", None)
+                        challenge = api_result.data.get("challenge", None)
+                        if gt and challenge:
+                            geetest_result = await get_validate(gt, challenge)
+                            if _conf.preference.geetest_url:
+                                if on_geetest_callback and attempt.retry_state.attempt_number == 1:
+                                    on_geetest_callback()
+                                continue
+                            else:
+                                return BaseApiStatus(need_verify=True)
+            return BaseApiStatus(success=True)
+
         except tenacity.RetryError as e:
             if is_incorrect_return(e):
                 logger.exception(f"游戏签到 - 服务器没有正确返回")
                 logger.debug(f"网络请求返回: {res.text}")
                 return BaseApiStatus(incorrect_return=True)
+            elif _conf.preference.geetest_url and gt and challenge:
+                logger.error(f"游戏签到 - 进行人机验证失败")
+                return BaseApiStatus(need_verify=True)
             else:
                 logger.exception(f"游戏签到 - 请求失败")
                 return BaseApiStatus(network_error=True)
 
 
 class GenshinImpactSign(BaseGameSign):
     """
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/good_image.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/good_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/myb_missions_api.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/myb_missions_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                                          PrivateMessageEvent, GroupMessageEvent)
 from nonebot_plugin_apscheduler import scheduler
 
 from .exchange import generate_image
 from .game_sign_api import BaseGameSign
 from .myb_missions_api import BaseMission, get_missions_state
 from .plugin_data import PluginDataManager, write_plugin_data
-from .simple_api import genshin_board_bbs, get_game_record
+from .simple_api import genshin_board, get_game_record
 from .utils import get_file, logger, COMMAND_BEGIN
 
 _conf = PluginDataManager.plugin_data_obj
 
 manually_game_sign = on_command(_conf.preference.command_start + '签到', priority=5, block=True)
 manually_game_sign.name = '签到'
 manually_game_sign.usage = '手动进行游戏签到，查看本次签到奖励及本月签到天数'
@@ -30,14 +30,15 @@
     """
     手动游戏签到函数
     """
     bot = get_bot(str(event.self_id))
     user = _conf.users.get(event.user_id)
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
+    await manually_game_sign.send("⏳开始游戏签到...")
     await perform_game_sign(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
 
 
 manually_bbs_sign = on_command(_conf.preference.command_start + '任务', priority=5, block=True)
 manually_bbs_sign.name = '任务'
 manually_bbs_sign.usage = '手动执行米游币每日任务，可以查看米游币任务完成情况'
 
@@ -47,14 +48,15 @@
     """
     手动米游币任务函数
     """
     bot = get_bot(str(event.self_id))
     user = _conf.users.get(event.user_id)
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
+    await manually_game_sign.send("⏳开始执行米游币任务...")
     await perform_bbs_sign(bot=bot, qq=event.user_id, is_auto=False, group_event=event)
 
 
 manually_resin_check = on_command(_conf.preference.command_start + '便笺', priority=5, block=True)
 manually_resin_check.name = '便笺'
 manually_resin_check.usage = '手动查看原神实时便笺，即原神树脂、洞天财瓮等信息'
 has_checked = {}
@@ -62,15 +64,15 @@
     for account in user.accounts.values():
         if account.enable_resin:
             has_checked[account.bbs_uid] = has_checked.get(account.bbs_uid,
                                                            {"resin": False, "coin": False, "transformer": False})
 
 
 @manually_resin_check.handle()
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent]):
+async def _(event: Union[GroupMessageEvent, PrivateMessageEvent]):
     """
     手动查看原神便笺
     """
     bot = get_bot(str(event.self_id))
     user = _conf.users.get(event.user_id)
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
@@ -88,14 +90,16 @@
     :param group_event: 若为群消息触发，则为群消息事件，否则为None
     """
     if isinstance(group_event, PrivateMessageEvent):
         group_event = None
     failed_accounts = []
     user = _conf.users[qq]
     for account in _conf.users.get(qq).accounts.values():
+        signed = False
+        """是否已经完成过签到"""
         game_record_status, records = await get_game_record(account)
         if not game_record_status:
             if group_event:
                 await bot.send(event=group_event, at_sender=True,
                                message=f"⚠️账户 {account.bbs_uid} 获取游戏账号信息失败，请重新尝试")
             else:
                 await bot.send_private_msg(user_id=qq,
@@ -116,15 +120,18 @@
                 else:
                     await bot.send_private_msg(user_id=qq, message=f"⚠️账户 {account.bbs_uid} 获取签到记录失败")
 
             # 自动签到时，要求用户打开了签到功能；手动签到时都可以调用执行。若没签到，则进行签到功能。
             # 若获取今日签到情况失败，仍可继续
             if ((account.enable_game_sign and is_auto) or not is_auto) and (
                     (info and not info.is_sign) or not get_info_status):
-                sign_status = await signer.sign(account.platform)
+                sign_status = await signer.sign(
+                    account.platform,
+                    lambda: bot.send_private_msg(user_id=qq, message=f"⏳正在尝试完成人机验证，请稍后...")
+                )
                 if not sign_status:
                     if sign_status.login_expired:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到时服务器返回登录失效，请尝试重新登录绑定账户"
                     elif sign_status.need_verify:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到时可能遇到验证码拦截，请尝试使用命令『/账号设置』更改设备平台，若仍失败请手动前往米游社签到"
                     else:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到失败，请稍后再试"
@@ -135,27 +142,31 @@
                             await bot.send_msg(message_type="private", user_id=qq, message=message)
                     await asyncio.sleep(_conf.preference.sleep_time)
                     continue
                 await asyncio.sleep(_conf.preference.sleep_time)
             # 若用户未开启自动签到且手动签到过了，不再提醒
             elif not account.enable_game_sign and is_auto:
                 continue
+            else:
+                signed = True
 
             # 用户打开通知或手动签到时，进行通知
             if user.enable_notice or not is_auto:
                 img = ""
                 get_info_status, info = await signer.get_info(account.platform)
                 get_award_status, awards = await signer.get_rewards()
                 if not get_info_status or not get_award_status:
                     msg = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』获取签到结果失败！请手动前往米游社查看"
                 else:
                     award = awards[info.total_sign_day - 1]
                     if info.is_sign:
+                        status = "签到成功！" if not signed else "已经签到过了"
                         msg = f"🪪账户 {account.bbs_uid}" \
-                              f"\n🎮『{signer.NAME}』今日签到成功！" \
+                              f"\n🎮『{signer.NAME}』" \
+                              f"\n🎮状态: {status}" \
                               f"\n{signer.record.nickname}·{signer.record.level}" \
                               "\n\n🎁今日签到奖励：" \
                               f"\n{award.name} * {award.cnt}" \
                               f"\n\n📅本月签到次数：{info.total_sign_day}"
                         img_file = await get_file(award.icon)
                         img = MessageSegment.image(img_file)
                     else:
@@ -313,15 +324,16 @@
     global has_checked
     user = _conf.users[qq]
     for account in user.accounts.values():
         if account.enable_resin:
             has_checked[account.bbs_uid] = has_checked.get(account.bbs_uid,
                                                            {"resin": False, "coin": False, "transformer": False})
         if (account.enable_resin and is_auto) or not is_auto:
-            genshin_board_status, board = await genshin_board_bbs(account)
+            genshin_board_status, board = await genshin_board(account)
+            logger.info(genshin_board_status)
             if not genshin_board_status:
                 if genshin_board_status.login_expired:
                     if not is_auto:
                         if group_event:
                             await bot.send(event=group_event, at_sender=True,
                                            message=f'⚠️账户 {account.bbs_uid} 登录失效，请重新登录')
                         else:
@@ -342,14 +354,21 @@
                     if group_event:
                         await bot.send(event=group_event, at_sender=True,
                                        message=f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
                     else:
                         await bot.send_private_msg(user_id=qq,
                                                    message=f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
                 continue
+            if genshin_board_status.need_verify:
+                if group_event:
+                    await bot.send(event=group_event, at_sender=True,
+                                   message=f'⚠️遇到验证码正在尝试绕过')
+                else:
+                    await bot.send_private_msg(user_id=qq,
+                                               message=f'⚠️遇到验证码正在尝试绕过')
             msg = ''
             # 手动查询体力时，无需判断是否溢出
             if not is_auto:
                 pass
             else:
                 # 体力溢出提醒
                 if board.current_resin == 160:
@@ -368,30 +387,31 @@
                         return
                     else:
                         has_checked[account.bbs_uid]['coin'] = True
                         msg += '❕您的洞天财瓮已经满啦\n'
                 else:
                     has_checked[account.bbs_uid]['coin'] = False
                 # 参量质变仪就绪提醒
-                if board.transformer_text == '已准备就绪':
-                    # 防止重复提醒
-                    if has_checked[account.bbs_uid]['transformer']:
-                        return
+                if board.transformer:
+                    if board.transformer_text == '已准备就绪':
+                        # 防止重复提醒
+                        if has_checked[account.bbs_uid]['transformer']:
+                            return
+                        else:
+                            has_checked[account.bbs_uid]['transformer'] = True
+                            msg += '❕您的参量质变仪已准备就绪\n\n'
                     else:
-                        has_checked[account.bbs_uid]['transformer'] = True
-                        msg += '❕您的参量质变仪已准备就绪\n\n'
-                else:
-                    has_checked[account.bbs_uid]['transformer'] = False
-                    return
+                        has_checked[account.bbs_uid]['transformer'] = False
+                        return
             msg += "❖实时便笺❖" \
                    f"\n⏳树脂数量：{board.current_resin} / 160" \
                    f"\n🕰️探索派遣：{board.current_expedition_num} / {board.max_expedition_num}" \
                    f"\n📅每日委托：{4 - board.finished_task_num} 个任务未完成" \
                    f"\n💰洞天财瓮：{board.current_home_coin} / {board.max_home_coin}" \
-                   f"\n🎰参量质变仪：{board.transformer_text}"
+                   f"\n🎰参量质变仪：{board.transformer_text if board.transformer else 'N/A'}"
             if group_event:
                 await bot.send(event=group_event, at_sender=True, message=msg)
             else:
                 await bot.send_private_msg(user_id=qq, message=msg)
 
 
 @scheduler.scheduled_job("cron", hour='0', minute='0', id="daily_goodImg_update")
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/plugin_data.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/plugin_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Mapping
 
 from loguru import logger
 from pydantic import BaseModel, ValidationError, BaseSettings, validator
 
 from .user_data import UserData, UserAccount
 
-VERSION = "v1.0.0-beta.1"
+VERSION = "v1.0.0-beta.2"
 """程序当前版本"""
 
 ROOT_PATH = Path(__name__).parent.absolute()
 '''NoneBot2 机器人根目录'''
 
 DATA_PATH = ROOT_PATH / "data" / "nonebot-plugin-mystool"
 '''插件数据保存目录'''
@@ -80,14 +80,16 @@
     '''插件内部命令头(若为""空字符串则不启用)'''
     sleep_time: float = 5
     '''任务操作冷却时间(如米游币任务)'''
     plan_time: str = "00:30"
     '''每日自动签到和米游社任务的定时任务执行时间，格式为HH:MM'''
     resin_interval: int = 60
     '''每次检查原神便笺间隔，单位为分钟'''
+    geetest_url: Optional[str]
+    '''极验Geetest人机验证打码接口URL'''
 
     @validator("log_path", allow_reuse=True)
     def _(cls, v: Optional[Path]):
         absolute_path = v.absolute()
         if not os.path.exists(absolute_path) or not os.path.isfile(absolute_path):
             absolute_parent = absolute_path.parent
             try:
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/setting.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/simple_api.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/simple_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 URL_ADDRESS = "https://api-takumi.mihoyo.com/account/address/list?t={}"
 URL_REGISTRABLE = "https://webapi.account.mihoyo.com/Api/is_mobile_registrable?mobile={mobile}&t={t}"
 URL_CREATE_MMT = "https://webapi.account.mihoyo.com/Api/create_mmt?scene_type=1&now={now}&reason=user.mihoyo.com%2523%252Flogin%252Fcaptcha&action_type=login_by_mobile_captcha&t={t}"
 URL_CREATE_MOBILE_CAPTCHA = "https://webapi.account.mihoyo.com/Api/create_mobile_captcha"
 URL_GET_USER_INFO = "https://bbs-api.miyoushe.com/user/api/getUserFullInfo?uid={uid}"
 URL_GENSHIN_STATUS_WIDGET = "https://api-takumi-record.mihoyo.com/game_record/app/card/api/getWidgetData?game_id=2"
 URL_GENSHEN_STATUS_BBS = "https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/dailyNote"
+URL_GENSHEN_STATUS_WIDGET = "https://api-takumi-record.mihoyo.com/game_record/genshin/aapi/widget/v2"
 
 HEADERS_WEBAPI = {
     "Host": "webapi.account.mihoyo.com",
     "Connection": "keep-alive",
     "sec-ch-ua": _conf.device_config.UA,
     "DNT": "1",
     "x-rpc-device_model": _conf.device_config.X_RPC_DEVICE_MODEL_PC,
@@ -1310,21 +1311,20 @@
             return ExchangeStatus(incorrect_return=True), None
         else:
             logger.exception(
                 f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 请求失败")
             return ExchangeStatus(network_error=True), None
 
 
-async def genshin_board_bbs(account: UserAccount, retry: bool = True) -> Tuple[
+async def genshin_board(account: UserAccount) -> Tuple[
     Union[BaseApiStatus, GenshinBoardStatus], Optional[GenshinBoard]]:
     """
-    使用米游社内页面API获取原神实时便笺
+    获取原神实时便笺
 
     :param account: 用户账户数据
-    :param retry: 是否允许重试
     """
     game_record_status, records = await get_game_record(account)
     if not game_record_status:
         return game_record_status, None
     game_list_status, game_list = await get_game_list()
     if not game_list_status:
         return game_list_status, None
@@ -1339,33 +1339,50 @@
         if record.game_id == game_id:
             try:
                 flag = False
                 params = {"role_id": record.game_role_id, "server": record.region}
                 url = f"{URL_GENSHEN_STATUS_BBS}?{urlencode(params)}"
                 headers = HEADERS_GENSHIN_STATUS_BBS.copy()
                 headers["x-rpc-device_id"] = account.device_id_android
-                async for attempt in get_async_retry(retry):
+                async for attempt in get_async_retry(False):
                     with attempt:
                         headers["DS"] = generate_ds(
                             params={"role_id": record.game_role_id, "server": record.region})
                         async with httpx.AsyncClient() as client:
                             res = await client.get(url, headers=headers,
                                                    cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
                                                    timeout=_conf.preference.timeout)
                         api_result = ApiResultHandler(res.json())
                         if api_result.login_expired:
                             logger.info(
                                 f"原神实时便笺: 用户 {account.bbs_uid} 登录失效")
                             logger.debug(f"网络请求返回: {res.text}")
                             return GenshinBoardStatus(login_expired=True), None
+
                         if api_result.invalid_ds:
                             logger.info(
                                 f"原神实时便笺: 用户 {account.bbs_uid} DS 校验失败")
                             logger.debug(f"网络请求返回: {res.text}")
-                            return GenshinBoardStatus(invalid_ds=True), None
+                        if api_result.retcode == 1034:
+                            logger.info(
+                                f"原神实时便笺: 用户 {account.bbs_uid} 可能被验证码阻拦")
+                            logger.debug(f"网络请求返回: {res.text}")
+                        if api_result.invalid_ds or api_result.retcode == 1034:
+                            headers["DS"] = generate_ds()
+                            headers["x-rpc-device_id"] = account.device_id_ios
+                            async with httpx.AsyncClient() as client:
+                                res = await client.get(
+                                    URL_GENSHEN_STATUS_WIDGET,
+                                    headers=headers,
+                                    cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
+                                    timeout=_conf.preference.timeout
+                                )
+                            api_result = ApiResultHandler(res.json())
+                            return GenshinBoardStatus(success=True), \
+                                GenshinBoard.parse_obj(api_result.data)
                         return GenshinBoardStatus(success=True), GenshinBoard.parse_obj(api_result.data)
             except tenacity.RetryError as e:
                 if is_incorrect_return(e):
                     logger.exception(f"原神实时便笺: 服务器没有正确返回")
                     logger.debug(f"网络请求返回: {res.text}")
                     return GenshinBoardStatus(incorrect_return=True), None
                 else:
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/user_check.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 from nonebot import get_driver, on_request
 from nonebot.adapters.onebot.v11 import (Bot, FriendRequestEvent,
                                          GroupRequestEvent, RequestEvent)
 from nonebot_plugin_apscheduler import scheduler
 
 from .plugin_data import PluginDataManager, write_plugin_data
-from .utils import logger, _driver
+from .utils import logger
 
 _conf = PluginDataManager.plugin_data_obj
+_driver = get_driver()
 friendRequest = on_request(priority=1, block=True)
 
 
 @friendRequest.handle()
 async def _(bot: Bot, event: RequestEvent):
     command_start = list(get_driver().config.command_start)[0]
     # 判断为加好友事件
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/user_data.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/user_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-1.0.0b2/src/nonebot_plugin_mystool/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 ### 工具函数
 """
 import hashlib
 import json
 import random
 import string
 import time
-import traceback
 import uuid
 from typing import (TYPE_CHECKING, Dict, Literal,
                     Union, Optional)
 from urllib.parse import urlencode
 
 import httpx
 import nonebot
 import nonebot.log
 import nonebot.plugin
 import ntplib
 import tenacity
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 
+from .data_model import GeetestResult
 from .plugin_data import PluginDataManager
 
 if TYPE_CHECKING:
     from loguru import Logger
 
 _conf = PluginDataManager.plugin_data_obj
-_driver = nonebot.get_driver()
 
 
 class CommandBegin:
     """
     命令开头字段
     （包括例如'/'和插件命令起始字段例如'mystool'）
     已重写__str__方法
@@ -54,19 +53,18 @@
         return cls.string
 
 
 def get_last_command_sep():
     """
     获取第最后一个命令分隔符
     """
-    if _driver.config.command_sep:
-        return list(_driver.config.command_sep)[-1]
+    if nonebot.get_driver().config.command_sep:
+        return list(nonebot.get_driver().config.command_sep)[-1]
 
 
-_driver.on_startup(CommandBegin.set_command_begin)
 COMMAND_BEGIN = CommandBegin()
 '''命令开头字段（包括例如'/'和插件命令起始字段例如'mystool'）'''
 
 
 def set_logger(logger: "Logger"):
     """
     给日志记录器对象增加输出到文件的Handler
@@ -137,16 +135,15 @@
                 return False
             try:
                 for attempt in get_async_retry(True):
                     with attempt:
                         cls.time_offset = ntplib.NTPClient().request(
                             _conf.preference.ntp_server).tx_time - time.time()
             except tenacity.RetryError:
-                logger.error("校对互联网时间失败，改为使用本地时间")
-                logger.debug(traceback.format_exc())
+                logger.exception("校对互联网时间失败，改为使用本地时间")
                 return False
             logger.info("互联网时间校对完成")
             return True
         else:
             logger.info("未开启互联网时间校对，跳过时间同步")
             return True
 
@@ -200,15 +197,16 @@
     获取Headers中所需DS
 
     :param data: 可选，网络请求中需要发送的数据
     :param params: 可选，URL参数
     :param platform: 可选，平台，ios或android
     :param salt: 可选，自定义salt
     """
-    if data is None and params is None or salt != _conf.salt_config.SALT_PROD:
+    if data is None and params is None or \
+            salt is not None and salt != _conf.salt_config.SALT_PROD:
         if platform == "ios":
             salt = salt or _conf.salt_config.SALT_IOS
         else:
             salt = salt or _conf.salt_config.SALT_ANDROID
         t = str(int(NtpTime.time()))
         a = "".join(random.sample(
             string.ascii_lowercase + string.digits, 6))
@@ -237,14 +235,46 @@
         t = str(int(time.time()))
         r = str(random.randint(100000, 200000))
         c = hashlib.md5(
             f"salt={salt}&t={t}&r={r}&b={data}&q={params}".encode()).hexdigest()
         return f"{t},{r},{c}"
 
 
+async def get_validate(gt: str = None, challenge: str = None, retry: bool = True):
+    """
+    使用打码平台获取人机验证validate
+
+    :param gt: 验证码gt
+    :param challenge: challenge
+    :param retry: 是否允许重试
+    :return: 如果配置了平台URL，且 gt, challenge 不为空，返回 GeetestResult
+    """
+    content = {
+        "gt": gt,
+        "challenge": challenge
+    }
+
+    if gt and challenge and _conf.preference.geetest_url:
+        try:
+            async for attempt in get_async_retry(retry):
+                with attempt:
+                    async with httpx.AsyncClient() as client:
+                        res = await client.post(
+                            _conf.preference.geetest_url,
+                            timeout=60,
+                            json=content)
+                    geetest_data = res.json()
+                    if geetest_data['data']['result'] != 'fail':
+                        return GeetestResult(validate=geetest_data['data']['validate'], seccode="")
+        except tenacity.RetryError:
+            logger.exception(f"{_conf.preference.log_head}获取人机验证validate失败")
+    else:
+        return GeetestResult("", "")
+
+
 async def get_file(url: str, retry: bool = True):
     """
     下载文件
 
     :param url: 文件URL
     :param retry: 是否允许重试
     :return: 文件数据
@@ -252,16 +282,15 @@
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
                     res = await client.get(url, timeout=_conf.preference.timeout, follow_redirects=True)
                 return res.content
     except tenacity.RetryError:
-        logger.error(f"{_conf.preference.log_head}下载文件 - {url} 失败")
-        logger.debug(f"{_conf.preference.log_head}{traceback.format_exc()}")
+        logger.exception(f"{_conf.preference.log_head}下载文件 - {url} 失败")
 
 
 def blur_phone(phone: Union[str, int]) -> str:
     """
     模糊手机号
 
     :param phone: 手机号
```

### Comparing `nonebot_plugin_mystool-1.0.0b1/PKG-INFO` & `nonebot_plugin_mystool-1.0.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
@@ -39,24 +39,32 @@
   <img alt="CodeFactor" src="https://www.codefactor.io/repository/github/ljzd-pro/nonebot-plugin-mystool/badge?style=for-the-badge">
   <img alt="最新发行版" src="https://img.shields.io/github/v/release/Ljzd-PRO/nonebot-plugin-mysTool?logo=python&style=for-the-badge">
   <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
 </div>
 
 # mysTool - 米游社辅助工具插件
 
-**版本 - v1.0.0-beta.1**
+**版本 - v1.0.0-beta.2**
 
 ### 📣 更新内容
 
-#### 2023.6.10
+#### 2023.6.22 - v1.0.0-beta.2
+改动较大，目前是 Beta 版，可能不稳定
+
+Windows、macOS 下无法多进程生成商品图片的问题暂时没有修复
+
+- 支持使用人机验证打码平台处理人机验证任务 [#119](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/119) by @Night-stars-1
+- 原神便笺获取失败时更换为使用米游社iOS小组件API获取 [#119](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/119) by @Night-stars-1
+- 修复原神便笺和讨论区签到可能因为DS无效而失败的问题
 
+#### 2023.6.10 - v1.0.0-beta.1
 改动较大，目前是 Beta 版，可能不稳定
 
 - 大量的代码重构，包括米游社API的客户端实现、用户数据相关、插件配置相关、API相关数据模型
-- 修复在 Windows 下无法多进程生成商品图片的问题
+- ~~修复在 Windows 下无法多进程生成商品图片的问题~~
 - 从显示用户账号绑定的手机号改为显示账号的米游社ID
 - 设置、兑换计划功能支持群聊使用
 - 登陆绑定只需要进行一次短信验证
 - 用户数据文件、插件配置文件 **格式更新，与 v1.0.0 之前的版本不兼容**
 - 修复添加兑换任务时出现的UID不存在错误
 - 修复商品图片生成完才发出后台正在生成提示的问题
 - 异常捕获更加准确
```

