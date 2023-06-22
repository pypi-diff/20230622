# Comparing `tmp/cushy-storage-1.1.1.tar.gz` & `tmp/cushy-storage-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cushy-storage-1.1.1.tar", last modified: Wed Jun  7 08:29:06 2023, max compression
+gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-jhrz674e/cushy-storage-1.1.3.tar", last modified: Wed Jun 21 13:46:21 2023, max compression
```

## Comparing `cushy-storage-1.1.1.tar` & `cushy-storage-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/
--rw-rw-rw-   0        0        0    11558 2023-03-08 11:01:44.000000 cushy-storage-1.1.1/LICENSE
--rw-rw-rw-   0        0        0    11758 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10880 2023-06-06 08:53:54.000000 cushy-storage-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/cushy_storage/
--rw-rw-rw-   0        0        0     1013 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/cushy_storage/__init__.py
--rw-rw-rw-   0        0        0     7508 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/cushy_storage/_core.py
--rw-rw-rw-   0        0        0     1431 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/cushy_storage/base.py
--rw-rw-rw-   0        0        0     1959 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/cushy_storage/logger.py
--rw-rw-rw-   0        0        0     6100 2023-06-07 08:18:17.000000 cushy-storage-1.1.1/cushy_storage/orm.py
--rw-rw-rw-   0        0        0     1747 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/cushy_storage/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/cushy_storage.egg-info/
--rw-rw-rw-   0        0        0    11758 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/cushy_storage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/cushy_storage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/cushy_storage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/cushy_storage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1814 2023-06-07 08:18:26.000000 cushy-storage-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:29:06.000000 cushy-storage-1.1.1/tests/
--rw-rw-rw-   0        0        0     1657 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/tests/test_base_dict.py
--rw-rw-rw-   0        0        0     1887 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/tests/test_cushy_dict.py
--rw-rw-rw-   0        0        0     2383 2023-06-06 08:52:30.000000 cushy-storage-1.1.1/tests/test_dict_cache.py
--rw-rw-rw-   0        0        0     4690 2023-06-07 08:18:17.000000 cushy-storage-1.1.1/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/cushy_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/cushy_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/cushy_storage/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/cushy_storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/cushy_storage/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/cushy_storage/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/cushy_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/cushy_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/cushy_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/cushy_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/cushy_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/cushy_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:46:21.000000 cushy-storage-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/tests/test_base_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/tests/test_cushy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/tests/test_dict_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-21 13:46:05.000000 cushy-storage-1.1.3/tests/test_orm.py
```

### Comparing `cushy-storage-1.1.1/LICENSE` & `cushy-storage-1.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `cushy-storage-1.1.1/PKG-INFO` & `cushy-storage-1.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,369 +1,349 @@
-Metadata-Version: 2.1
-Name: cushy-storage
-Version: 1.1.1
-Summary: A data local persistence framework library
-Home-page: https://github.com/Undertone0809/cushy-storage
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: storage,serialization,json,cushy-storage,cushy_storage
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    cushy-storage
-</h1>
-<p align="center">
-  <strong>一个基于磁盘缓存的ORM框架</strong>
-</p>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
-   </a>
-</p>
-
-[English](/README_en.md) [中文](/README.md)
-
-# 简介
-
-cushy-storage是一个基于磁盘缓存的ORM框架，你可以使用轻松的将自定义的数据通过ORM进行增删改查；另一方面，cushy-storage让你无需花费精力在
-如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。如果你有对本地文件数据操作的需求，使用本框架可以轻松的进行数据的本地存储。
-
-# 特性
-
-- 支持ORM存储、基本数据存储、自定义数据存储，兼容所有数据类型
-- 支持ORM框架级对象操作，可以轻松地对对象级数据进行增删改查
-- 存储基本数据时像操作dict一样读写，十分方便
-- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
-- 免去了直接操作文件的工作
-- 提供多种序列化操作
-- 提供多种数据压缩方式
-
-# 安装
-
-```bash
-pip install cushy-storage --upgrade 
-```
-
-# 快速上手
-
-`cushy-storage` 的使用主要分为四个部分，`CushyOrmCache` `CushyDict` `BaseDict` `disk_cache` 
-
-- `CushyOrmCache` 基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查
-- `CushyDict`: `BaseDict`的增强版，存储各种类型的数据，包括基本数据类型与自定义数据类型
-- `BaseDict`: 存储基础的二进制数据
-- `disk_cache`: 函数数据缓存
-
-## CushyOrmCache
-
-CushyOrmCache是一个基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查，下面，我们将会用一些简单的场景介绍其使用方法。
-
-现在我们需要构建一个简单的用户系统，用户系统的数据我们直接保存在本地文件中（当前对象级数据只支持pickle序列化的形式存储），用户的字段简单就好，
-只需要一个name和一个age，则我们可以构建如下的操作。
-
-```python
-from cushy_storage.orm import BaseORMModel, CushyOrmCache
-
-class User(BaseORMModel):
-
-    def __init__(self, name, age):
-        super().__init__()
-        self.name = name
-        self.age = age
-```
-
-这个示例中，我们实现了一个`User`类，并且继承了`BaseORMModel`，在`cushy-storage`中，如果你想让你的类可以进行ORM操作，就必须要继承这个类。
-接着，我们需要初始化`CushyOrmCache`。
-
-```python
-orm_cache = CushyOrmCache()
-```
-
-接着，你就可以直接进行`User`的增删改查操作了。
-
-```python
-"""add user"""
-user = User("jack", 18)
-orm_cache.add(user)
-user = User("jasmine", 18)
-orm_cache.add(user)
-
-"""query all user"""
-users = orm_cache.query(User).all()
-orm_cache.query(User).print_all()
-
-"""query by filter"""
-# get all user, you will get a List[User] type data.
-# Actually, it will get two users named "jack" and "jasmine".
-orm_cache.query("User").filter(age=18).all()
-# get first in queryset, you will get a User type data
-orm_cache.query("User").filter(name="jack").first()
-# filter by multiple parameters
-orm_cache.query("User").filter(name="jack", age=18).first()
-
-"""update"""
-user = orm_cache.query("User").filter(name='jack').first()
-user.age = 18
-orm_cache.update_obj(user)
-
-"""delete"""
-user = orm_cache.query("User").filter(name="jack").first()
-orm_cache.delete(user)
-orm_cache.query(User).print_all()
-
-```
-
-完整代码如下：
-
-```python
-from cushy_storage.orm import BaseORMModel, CushyOrmCache
-
-
-class User(BaseORMModel):
-
-    def __init__(self, name, age):
-        super().__init__()
-        self.name = name
-        self.age = age
-
-
-orm_cache = CushyOrmCache()
-
-"""add user"""
-user = User("jack", 18)
-orm_cache.add(user)
-user = User("jasmine", 18)
-orm_cache.add(user)
-
-"""query all user"""
-users = orm_cache.query(User).all()
-orm_cache.query(User).print_all()
-
-"""query by filter"""
-# get all user, you will get a List[User] type data.
-# Actually, it will get two users named "jack" and "jasmine".
-orm_cache.query("User").filter(age=18).all()
-# get first in queryset, you will get a User type data
-orm_cache.query("User").filter(name="jack").first()
-# filter by multiple parameters
-orm_cache.query("User").filter(name="jack", age=18).first()
-
-"""update"""
-user = orm_cache.query("User").filter(name='jack').first()
-user.age = 18
-orm_cache.update_obj(user)
-
-"""delete"""
-user = orm_cache.query("User").filter(name="jack").first()
-orm_cache.delete(user)
-orm_cache.query(User).print_all()
-
-```
-
-> 需要注意的是，你可以通过在query()中传入User对象来进行数据的查询，也可以直接传入"User"字符串进行数据的查询（这里的设计思路和数据库的表是一样的
-，User是表名）
-
-## BaseDict
-
-BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
-
-```python
-from cushy_storage import BaseDict
-
-# 初始化cache，保存在./data文件夹下
-cache = BaseDict('./data')
-# Base Dict只能存储二进制数据，可以用于流式传输
-cache['key'] = b'value'
-value = cache['key']
-print(value)
-
-```
-
-## CushyDict类
-
-CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
-此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
-一些简单的使用教程。
-
-- 存储Python基本数据类型
-
-```python
-from cushy_storage import CushyDict
-
-# 初始化cache，保存在./data文件夹下
-cache = CushyDict('./data')
-
-cache['key'] = {'value': 42}
-print(cache['key'])
-
-cache['a'] = 1
-print(cache['a'])
-
-cache['b'] = "hello world"
-print(cache['b'])
-
-cache['arr'] = [1, 2, 3, 4, 5]
-print(cache['arr'])
-
-```
-
-> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
-
-- 生成结果
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
-
-- 存储自定义数据类型
-
-```python
-from cushy_storage import CushyDict
-
-
-class User:
-    def __init__(self, name, age):
-        self.name = name
-        self.age = age
-
-
-def main():
-    cache = CushyDict(serialize='pickle')
-    user = User("Jack", 18)
-    cache['user'] = user
-
-    user = cache['user']
-    print(type(user))
-    print(cache['user'].name)
-    print(cache['user'].age)
-
-
-if __name__ == '__main__':
-    main()
-```
-
-> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
-
-- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-```
-
-- 判断key是否存在（和字典操作同理）
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-if 'key' in cache:
-    print("key exist")
-else:
-    print("key not exist")
-
-```
-
-## disk_cache装饰器
-
-disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
-
-```python
-from cushy_storage import disk_cache
-
-
-@disk_cache('./data')
-def my_func():
-    return {'value': 42}
-
-
-result = my_func()
-
-```
-
-# QA
-
-## 如何在一个大项目里全局只使用一个cache?
-
-你可以通过构建一个`utils.py`，对外暴露一个`get_cache()`函数，让需要`cache`的模块都通过`get_cache()`来获取`cache`
-，一个简单的示例如下：
-
-- `utils.py`
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-
-
-def get_cache():
-    return cache
-```
-
-- `app.py`
-
-```python
-from utils import get_cache
-
-
-def main():
-    cache = get_cache()
-
-```
-
-# 待办
-
-- [x] 提供单例模式解决方案，提供更加方便的工具类
-- [x] 支持多种压缩和序列化算法，以满足不同类型数据的需求
-- [x] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
-- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
-- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
-- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
-- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
-- [ ] 改善文档结构和代码注释，方便用户理解和使用库
-- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
-- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
-- [x] 支持更多数据格式的持久化方式，如json的直接存储
-- [x] 提供ORM框架，封装对象级的CRUD操作
-- [ ] 提供ORM的事务模式
-- [ ] 为ORM提供更加细粒度的filter，如模糊匹配、大小比较等
-- [ ] 提供操作日志记录
-- [ ] 提供缓存文件分布记录
-- [ ] 提升json存储数据的可读性
-- [ ] 提供自定义的数据导出、转换形式
-
-# 鸣谢
-
-本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
-进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
-
-This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
-RimoChan for his great work.
-
-# 贡献
-
-如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
+<h1 align="center">
+    cushy-storage
+</h1>
+<p align="center">
+  <strong>一个基于磁盘缓存的ORM框架</strong>
+</p>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
+   </a>
+</p>
+
+[English](/README_en.md) [中文](/README.md)
+
+# 简介
+
+cushy-storage是一个基于磁盘缓存的ORM框架，你可以使用轻松的将自定义的数据通过ORM进行增删改查；另一方面，cushy-storage让你无需花费精力在
+如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。如果你有对本地文件数据操作的需求，使用本框架可以轻松的进行数据的本地存储。
+
+# 特性
+
+- 支持ORM存储、基本数据存储、自定义数据存储，兼容所有数据类型
+- 支持ORM框架级对象操作，可以轻松地对对象级数据进行增删改查
+- 存储基本数据时像操作dict一样读写，十分方便
+- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
+- 免去了直接操作文件的工作
+- 提供多种序列化操作
+- 提供多种数据压缩方式
+
+# 安装
+
+```bash
+pip install cushy-storage --upgrade 
+```
+
+# 快速上手
+
+`cushy-storage` 的使用主要分为四个部分，`CushyOrmCache` `CushyDict` `BaseDict` `disk_cache` 
+
+- `CushyOrmCache` 基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查
+- `CushyDict`: `BaseDict`的增强版，存储各种类型的数据，包括基本数据类型与自定义数据类型
+- `BaseDict`: 存储基础的二进制数据
+- `disk_cache`: 函数数据缓存
+
+## CushyOrmCache
+
+CushyOrmCache是一个基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查，下面，我们将会用一些简单的场景介绍其使用方法。
+
+现在我们需要构建一个简单的用户系统，用户系统的数据我们直接保存在本地文件中（当前对象级数据只支持pickle序列化的形式存储），用户的字段简单就好，
+只需要一个name和一个age，则我们可以构建如下的操作。
+
+```python
+from cushy_storage.orm import BaseORMModel, CushyOrmCache
+
+class User(BaseORMModel):
+
+    def __init__(self, name, age):
+        super().__init__()
+        self.name = name
+        self.age = age
+```
+
+这个示例中，我们实现了一个`User`类，并且继承了`BaseORMModel`，在`cushy-storage`中，如果你想让你的类可以进行ORM操作，就必须要继承这个类。
+接着，我们需要初始化`CushyOrmCache`。
+
+```python
+orm_cache = CushyOrmCache()
+```
+
+接着，你就可以直接进行`User`的增删改查操作了。
+
+```python
+"""add user"""
+user = User("jack", 18)
+orm_cache.add(user)
+user = User("jasmine", 18)
+orm_cache.add(user)
+# or you can pass a list
+orm_cache.add([User("Zeeland", 10), User("Zero", 20)])
+
+"""query all user"""
+users = orm_cache.query(User).all()
+orm_cache.query(User).print_all()
+
+"""query by filter"""
+# get all user, you will get a List[User] type data.
+# Actually, it will get two users named "jack" and "jasmine".
+orm_cache.query("User").filter(age=18).all()
+# get first in queryset, you will get a User type data
+orm_cache.query("User").filter(name="jack").first()
+# filter by multiple parameters
+orm_cache.query("User").filter(name="jack", age=18).first()
+
+"""update"""
+user = orm_cache.query("User").filter(name='jack').first()
+user.age = 18
+orm_cache.update_obj(user)
+
+"""delete"""
+user = orm_cache.query("User").filter(name="jack").first()
+orm_cache.delete(user)
+orm_cache.query(User).print_all()
+
+```
+
+完整代码如下：
+
+```python
+from cushy_storage.orm import BaseORMModel, CushyOrmCache
+
+
+class User(BaseORMModel):
+
+    def __init__(self, name, age):
+        super().__init__()
+        self.name = name
+        self.age = age
+
+
+orm_cache = CushyOrmCache()
+
+"""add user"""
+user = User("jack", 18)
+orm_cache.add(user)
+user = User("jasmine", 18)
+orm_cache.add(user)
+
+"""query all user"""
+users = orm_cache.query(User).all()
+orm_cache.query(User).print_all()
+
+"""query by filter"""
+# get all user, you will get a List[User] type data.
+# Actually, it will get two users named "jack" and "jasmine".
+orm_cache.query("User").filter(age=18).all()
+# get first in queryset, you will get a User type data
+orm_cache.query("User").filter(name="jack").first()
+# filter by multiple parameters
+orm_cache.query("User").filter(name="jack", age=18).first()
+
+"""update"""
+user = orm_cache.query("User").filter(name='jack').first()
+user.age = 18
+orm_cache.update_obj(user)
+
+"""delete"""
+user = orm_cache.query("User").filter(name="jack").first()
+orm_cache.delete(user)
+orm_cache.query(User).print_all()
+
+```
+
+> 需要注意的是，你可以通过在query()中传入User对象来进行数据的查询，也可以直接传入"User"字符串进行数据的查询（这里的设计思路和数据库的表是一样的
+，User是表名）
+
+## BaseDict
+
+BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
+
+```python
+from cushy_storage import BaseDict
+
+# 初始化cache，保存在./data文件夹下
+cache = BaseDict('./data')
+# Base Dict只能存储二进制数据，可以用于流式传输
+cache['key'] = b'value'
+value = cache['key']
+print(value)
+
+```
+
+## CushyDict类
+
+CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
+此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
+一些简单的使用教程。
+
+- 存储Python基本数据类型
+
+```python
+from cushy_storage import CushyDict
+
+# 初始化cache，保存在./data文件夹下
+cache = CushyDict('./data')
+
+cache['key'] = {'value': 42}
+print(cache['key'])
+
+cache['a'] = 1
+print(cache['a'])
+
+cache['b'] = "hello world"
+print(cache['b'])
+
+cache['arr'] = [1, 2, 3, 4, 5]
+print(cache['arr'])
+
+```
+
+> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
+
+- 生成结果
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
+
+- 存储自定义数据类型
+
+```python
+from cushy_storage import CushyDict
+
+
+class User:
+    def __init__(self, name, age):
+        self.name = name
+        self.age = age
+
+
+def main():
+    cache = CushyDict(serialize='pickle')
+    user = User("Jack", 18)
+    cache['user'] = user
+
+    user = cache['user']
+    print(type(user))
+    print(cache['user'].name)
+    print(cache['user'].age)
+
+
+if __name__ == '__main__':
+    main()
+```
+
+> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
+
+- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+```
+
+- 判断key是否存在（和字典操作同理）
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
+
+```
+
+## disk_cache装饰器
+
+disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
+
+```python
+from cushy_storage import disk_cache
+
+
+@disk_cache('./data')
+def my_func():
+    return {'value': 42}
+
+
+result = my_func()
+
+```
+
+# QA
+
+## 如何在一个大项目里全局只使用一个cache?
+
+你可以通过构建一个`utils.py`，对外暴露一个`get_cache()`函数，让需要`cache`的模块都通过`get_cache()`来获取`cache`
+，一个简单的示例如下：
+
+- `utils.py`
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+
+
+def get_cache():
+    return cache
+```
+
+- `app.py`
+
+```python
+from utils import get_cache
+
+
+def main():
+    cache = get_cache()
+
+```
+
+# 待办
+
+- [x] 提供单例模式解决方案，提供更加方便的工具类
+- [x] 支持多种压缩和序列化算法，以满足不同类型数据的需求
+- [x] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
+- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
+- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
+- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
+- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
+- [ ] 改善文档结构和代码注释，方便用户理解和使用库
+- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
+- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
+- [x] 支持更多数据格式的持久化方式，如json的直接存储
+- [x] 提供ORM框架，封装对象级的CRUD操作
+- [ ] 提供ORM的事务模式
+- [ ] 为ORM提供更加细粒度的filter，如模糊匹配、大小比较等
+- [ ] 提供操作日志记录
+- [ ] 提供缓存文件分布记录
+- [ ] 提升json存储数据的可读性
+- [ ] 提供自定义的数据导出、转换形式
+
+# 鸣谢
+
+本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
+进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
+
+This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
+RimoChan for his great work.
+
+# 贡献
+
+如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `cushy-storage-1.1.1/README.md` & `cushy-storage-1.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,347 +1,371 @@
-<h1 align="center">
-    cushy-storage
-</h1>
-<p align="center">
-  <strong>一个基于磁盘缓存的ORM框架</strong>
-</p>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
-   </a>
-</p>
-
-[English](/README_en.md) [中文](/README.md)
-
-# 简介
-
-cushy-storage是一个基于磁盘缓存的ORM框架，你可以使用轻松的将自定义的数据通过ORM进行增删改查；另一方面，cushy-storage让你无需花费精力在
-如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。如果你有对本地文件数据操作的需求，使用本框架可以轻松的进行数据的本地存储。
-
-# 特性
-
-- 支持ORM存储、基本数据存储、自定义数据存储，兼容所有数据类型
-- 支持ORM框架级对象操作，可以轻松地对对象级数据进行增删改查
-- 存储基本数据时像操作dict一样读写，十分方便
-- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
-- 免去了直接操作文件的工作
-- 提供多种序列化操作
-- 提供多种数据压缩方式
-
-# 安装
-
-```bash
-pip install cushy-storage --upgrade 
-```
-
-# 快速上手
-
-`cushy-storage` 的使用主要分为四个部分，`CushyOrmCache` `CushyDict` `BaseDict` `disk_cache` 
-
-- `CushyOrmCache` 基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查
-- `CushyDict`: `BaseDict`的增强版，存储各种类型的数据，包括基本数据类型与自定义数据类型
-- `BaseDict`: 存储基础的二进制数据
-- `disk_cache`: 函数数据缓存
-
-## CushyOrmCache
-
-CushyOrmCache是一个基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查，下面，我们将会用一些简单的场景介绍其使用方法。
-
-现在我们需要构建一个简单的用户系统，用户系统的数据我们直接保存在本地文件中（当前对象级数据只支持pickle序列化的形式存储），用户的字段简单就好，
-只需要一个name和一个age，则我们可以构建如下的操作。
-
-```python
-from cushy_storage.orm import BaseORMModel, CushyOrmCache
-
-class User(BaseORMModel):
-
-    def __init__(self, name, age):
-        super().__init__()
-        self.name = name
-        self.age = age
-```
-
-这个示例中，我们实现了一个`User`类，并且继承了`BaseORMModel`，在`cushy-storage`中，如果你想让你的类可以进行ORM操作，就必须要继承这个类。
-接着，我们需要初始化`CushyOrmCache`。
-
-```python
-orm_cache = CushyOrmCache()
-```
-
-接着，你就可以直接进行`User`的增删改查操作了。
-
-```python
-"""add user"""
-user = User("jack", 18)
-orm_cache.add(user)
-user = User("jasmine", 18)
-orm_cache.add(user)
-
-"""query all user"""
-users = orm_cache.query(User).all()
-orm_cache.query(User).print_all()
-
-"""query by filter"""
-# get all user, you will get a List[User] type data.
-# Actually, it will get two users named "jack" and "jasmine".
-orm_cache.query("User").filter(age=18).all()
-# get first in queryset, you will get a User type data
-orm_cache.query("User").filter(name="jack").first()
-# filter by multiple parameters
-orm_cache.query("User").filter(name="jack", age=18).first()
-
-"""update"""
-user = orm_cache.query("User").filter(name='jack').first()
-user.age = 18
-orm_cache.update_obj(user)
-
-"""delete"""
-user = orm_cache.query("User").filter(name="jack").first()
-orm_cache.delete(user)
-orm_cache.query(User).print_all()
-
-```
-
-完整代码如下：
-
-```python
-from cushy_storage.orm import BaseORMModel, CushyOrmCache
-
-
-class User(BaseORMModel):
-
-    def __init__(self, name, age):
-        super().__init__()
-        self.name = name
-        self.age = age
-
-
-orm_cache = CushyOrmCache()
-
-"""add user"""
-user = User("jack", 18)
-orm_cache.add(user)
-user = User("jasmine", 18)
-orm_cache.add(user)
-
-"""query all user"""
-users = orm_cache.query(User).all()
-orm_cache.query(User).print_all()
-
-"""query by filter"""
-# get all user, you will get a List[User] type data.
-# Actually, it will get two users named "jack" and "jasmine".
-orm_cache.query("User").filter(age=18).all()
-# get first in queryset, you will get a User type data
-orm_cache.query("User").filter(name="jack").first()
-# filter by multiple parameters
-orm_cache.query("User").filter(name="jack", age=18).first()
-
-"""update"""
-user = orm_cache.query("User").filter(name='jack').first()
-user.age = 18
-orm_cache.update_obj(user)
-
-"""delete"""
-user = orm_cache.query("User").filter(name="jack").first()
-orm_cache.delete(user)
-orm_cache.query(User).print_all()
-
-```
-
-> 需要注意的是，你可以通过在query()中传入User对象来进行数据的查询，也可以直接传入"User"字符串进行数据的查询（这里的设计思路和数据库的表是一样的
-，User是表名）
-
-## BaseDict
-
-BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
-
-```python
-from cushy_storage import BaseDict
-
-# 初始化cache，保存在./data文件夹下
-cache = BaseDict('./data')
-# Base Dict只能存储二进制数据，可以用于流式传输
-cache['key'] = b'value'
-value = cache['key']
-print(value)
-
-```
-
-## CushyDict类
-
-CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
-此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
-一些简单的使用教程。
-
-- 存储Python基本数据类型
-
-```python
-from cushy_storage import CushyDict
-
-# 初始化cache，保存在./data文件夹下
-cache = CushyDict('./data')
-
-cache['key'] = {'value': 42}
-print(cache['key'])
-
-cache['a'] = 1
-print(cache['a'])
-
-cache['b'] = "hello world"
-print(cache['b'])
-
-cache['arr'] = [1, 2, 3, 4, 5]
-print(cache['arr'])
-
-```
-
-> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
-
-- 生成结果
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
-
-- 存储自定义数据类型
-
-```python
-from cushy_storage import CushyDict
-
-
-class User:
-    def __init__(self, name, age):
-        self.name = name
-        self.age = age
-
-
-def main():
-    cache = CushyDict(serialize='pickle')
-    user = User("Jack", 18)
-    cache['user'] = user
-
-    user = cache['user']
-    print(type(user))
-    print(cache['user'].name)
-    print(cache['user'].age)
-
-
-if __name__ == '__main__':
-    main()
-```
-
-> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
-
-- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-```
-
-- 判断key是否存在（和字典操作同理）
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-if 'key' in cache:
-    print("key exist")
-else:
-    print("key not exist")
-
-```
-
-## disk_cache装饰器
-
-disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
-
-```python
-from cushy_storage import disk_cache
-
-
-@disk_cache('./data')
-def my_func():
-    return {'value': 42}
-
-
-result = my_func()
-
-```
-
-# QA
-
-## 如何在一个大项目里全局只使用一个cache?
-
-你可以通过构建一个`utils.py`，对外暴露一个`get_cache()`函数，让需要`cache`的模块都通过`get_cache()`来获取`cache`
-，一个简单的示例如下：
-
-- `utils.py`
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-
-
-def get_cache():
-    return cache
-```
-
-- `app.py`
-
-```python
-from utils import get_cache
-
-
-def main():
-    cache = get_cache()
-
-```
-
-# 待办
-
-- [x] 提供单例模式解决方案，提供更加方便的工具类
-- [x] 支持多种压缩和序列化算法，以满足不同类型数据的需求
-- [x] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
-- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
-- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
-- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
-- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
-- [ ] 改善文档结构和代码注释，方便用户理解和使用库
-- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
-- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
-- [x] 支持更多数据格式的持久化方式，如json的直接存储
-- [x] 提供ORM框架，封装对象级的CRUD操作
-- [ ] 提供ORM的事务模式
-- [ ] 为ORM提供更加细粒度的filter，如模糊匹配、大小比较等
-- [ ] 提供操作日志记录
-- [ ] 提供缓存文件分布记录
-- [ ] 提升json存储数据的可读性
-- [ ] 提供自定义的数据导出、转换形式
-
-# 鸣谢
-
-本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
-进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
-
-This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
-RimoChan for his great work.
-
-# 贡献
-
-如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: cushy-storage
+Version: 1.1.3
+Summary: A data local persistence ORM framework
+Home-page: https://github.com/Undertone0809/cushy-storage
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: storage,ORM,serialization,json,cushy-storage,cushy_storage
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    cushy-storage
+</h1>
+<p align="center">
+  <strong>一个基于磁盘缓存的ORM框架</strong>
+</p>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
+   </a>
+</p>
+
+[English](/README_en.md) [中文](/README.md)
+
+# 简介
+
+cushy-storage是一个基于磁盘缓存的ORM框架，你可以使用轻松的将自定义的数据通过ORM进行增删改查；另一方面，cushy-storage让你无需花费精力在
+如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。如果你有对本地文件数据操作的需求，使用本框架可以轻松的进行数据的本地存储。
+
+# 特性
+
+- 支持ORM存储、基本数据存储、自定义数据存储，兼容所有数据类型
+- 支持ORM框架级对象操作，可以轻松地对对象级数据进行增删改查
+- 存储基本数据时像操作dict一样读写，十分方便
+- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
+- 免去了直接操作文件的工作
+- 提供多种序列化操作
+- 提供多种数据压缩方式
+
+# 安装
+
+```bash
+pip install cushy-storage --upgrade 
+```
+
+# 快速上手
+
+`cushy-storage` 的使用主要分为四个部分，`CushyOrmCache` `CushyDict` `BaseDict` `disk_cache` 
+
+- `CushyOrmCache` 基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查
+- `CushyDict`: `BaseDict`的增强版，存储各种类型的数据，包括基本数据类型与自定义数据类型
+- `BaseDict`: 存储基础的二进制数据
+- `disk_cache`: 函数数据缓存
+
+## CushyOrmCache
+
+CushyOrmCache是一个基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查，下面，我们将会用一些简单的场景介绍其使用方法。
+
+现在我们需要构建一个简单的用户系统，用户系统的数据我们直接保存在本地文件中（当前对象级数据只支持pickle序列化的形式存储），用户的字段简单就好，
+只需要一个name和一个age，则我们可以构建如下的操作。
+
+```python
+from cushy_storage.orm import BaseORMModel, CushyOrmCache
+
+class User(BaseORMModel):
+
+    def __init__(self, name, age):
+        super().__init__()
+        self.name = name
+        self.age = age
+```
+
+这个示例中，我们实现了一个`User`类，并且继承了`BaseORMModel`，在`cushy-storage`中，如果你想让你的类可以进行ORM操作，就必须要继承这个类。
+接着，我们需要初始化`CushyOrmCache`。
+
+```python
+orm_cache = CushyOrmCache()
+```
+
+接着，你就可以直接进行`User`的增删改查操作了。
+
+```python
+"""add user"""
+user = User("jack", 18)
+orm_cache.add(user)
+user = User("jasmine", 18)
+orm_cache.add(user)
+# or you can pass a list
+orm_cache.add([User("Zeeland", 10), User("Zero", 20)])
+
+"""query all user"""
+users = orm_cache.query(User).all()
+orm_cache.query(User).print_all()
+
+"""query by filter"""
+# get all user, you will get a List[User] type data.
+# Actually, it will get two users named "jack" and "jasmine".
+orm_cache.query("User").filter(age=18).all()
+# get first in queryset, you will get a User type data
+orm_cache.query("User").filter(name="jack").first()
+# filter by multiple parameters
+orm_cache.query("User").filter(name="jack", age=18).first()
+
+"""update"""
+user = orm_cache.query("User").filter(name='jack').first()
+user.age = 18
+orm_cache.update_obj(user)
+
+"""delete"""
+user = orm_cache.query("User").filter(name="jack").first()
+orm_cache.delete(user)
+orm_cache.query(User).print_all()
+
+```
+
+完整代码如下：
+
+```python
+from cushy_storage.orm import BaseORMModel, CushyOrmCache
+
+
+class User(BaseORMModel):
+
+    def __init__(self, name, age):
+        super().__init__()
+        self.name = name
+        self.age = age
+
+
+orm_cache = CushyOrmCache()
+
+"""add user"""
+user = User("jack", 18)
+orm_cache.add(user)
+user = User("jasmine", 18)
+orm_cache.add(user)
+
+"""query all user"""
+users = orm_cache.query(User).all()
+orm_cache.query(User).print_all()
+
+"""query by filter"""
+# get all user, you will get a List[User] type data.
+# Actually, it will get two users named "jack" and "jasmine".
+orm_cache.query("User").filter(age=18).all()
+# get first in queryset, you will get a User type data
+orm_cache.query("User").filter(name="jack").first()
+# filter by multiple parameters
+orm_cache.query("User").filter(name="jack", age=18).first()
+
+"""update"""
+user = orm_cache.query("User").filter(name='jack').first()
+user.age = 18
+orm_cache.update_obj(user)
+
+"""delete"""
+user = orm_cache.query("User").filter(name="jack").first()
+orm_cache.delete(user)
+orm_cache.query(User).print_all()
+
+```
+
+> 需要注意的是，你可以通过在query()中传入User对象来进行数据的查询，也可以直接传入"User"字符串进行数据的查询（这里的设计思路和数据库的表是一样的
+，User是表名）
+
+## BaseDict
+
+BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
+
+```python
+from cushy_storage import BaseDict
+
+# 初始化cache，保存在./data文件夹下
+cache = BaseDict('./data')
+# Base Dict只能存储二进制数据，可以用于流式传输
+cache['key'] = b'value'
+value = cache['key']
+print(value)
+
+```
+
+## CushyDict类
+
+CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
+此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
+一些简单的使用教程。
+
+- 存储Python基本数据类型
+
+```python
+from cushy_storage import CushyDict
+
+# 初始化cache，保存在./data文件夹下
+cache = CushyDict('./data')
+
+cache['key'] = {'value': 42}
+print(cache['key'])
+
+cache['a'] = 1
+print(cache['a'])
+
+cache['b'] = "hello world"
+print(cache['b'])
+
+cache['arr'] = [1, 2, 3, 4, 5]
+print(cache['arr'])
+
+```
+
+> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
+
+- 生成结果
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
+
+- 存储自定义数据类型
+
+```python
+from cushy_storage import CushyDict
+
+
+class User:
+    def __init__(self, name, age):
+        self.name = name
+        self.age = age
+
+
+def main():
+    cache = CushyDict(serialize='pickle')
+    user = User("Jack", 18)
+    cache['user'] = user
+
+    user = cache['user']
+    print(type(user))
+    print(cache['user'].name)
+    print(cache['user'].age)
+
+
+if __name__ == '__main__':
+    main()
+```
+
+> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
+
+- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+```
+
+- 判断key是否存在（和字典操作同理）
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
+
+```
+
+## disk_cache装饰器
+
+disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
+
+```python
+from cushy_storage import disk_cache
+
+
+@disk_cache('./data')
+def my_func():
+    return {'value': 42}
+
+
+result = my_func()
+
+```
+
+# QA
+
+## 如何在一个大项目里全局只使用一个cache?
+
+你可以通过构建一个`utils.py`，对外暴露一个`get_cache()`函数，让需要`cache`的模块都通过`get_cache()`来获取`cache`
+，一个简单的示例如下：
+
+- `utils.py`
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+
+
+def get_cache():
+    return cache
+```
+
+- `app.py`
+
+```python
+from utils import get_cache
+
+
+def main():
+    cache = get_cache()
+
+```
+
+# 待办
+
+- [x] 提供单例模式解决方案，提供更加方便的工具类
+- [x] 支持多种压缩和序列化算法，以满足不同类型数据的需求
+- [x] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
+- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
+- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
+- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
+- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
+- [ ] 改善文档结构和代码注释，方便用户理解和使用库
+- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
+- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
+- [x] 支持更多数据格式的持久化方式，如json的直接存储
+- [x] 提供ORM框架，封装对象级的CRUD操作
+- [ ] 提供ORM的事务模式
+- [ ] 为ORM提供更加细粒度的filter，如模糊匹配、大小比较等
+- [ ] 提供操作日志记录
+- [ ] 提供缓存文件分布记录
+- [ ] 提升json存储数据的可读性
+- [ ] 提供自定义的数据导出、转换形式
+
+# 鸣谢
+
+本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
+进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
+
+This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
+RimoChan for his great work.
+
+# 贡献
+
+如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `cushy-storage-1.1.1/cushy_storage/__init__.py` & `cushy-storage-1.1.3/cushy_storage/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-
-from cushy_storage._core import disk_cache, CushyDict, BaseDict
-from cushy_storage.orm import BaseORMModel, CushyOrmCache
-
-__all__ = [
-    'disk_cache',
-    'CushyDict',
-    'BaseDict',
-    'BaseORMModel',
-    'CushyOrmCache'
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+
+from cushy_storage._core import disk_cache, CushyDict, BaseDict
+from cushy_storage.orm import BaseORMModel, CushyOrmCache
+
+__all__ = ["disk_cache", "CushyDict", "BaseDict", "BaseORMModel", "CushyOrmCache"]
```

### Comparing `cushy-storage-1.1.1/cushy_storage/_core.py` & `cushy-storage-1.1.3/cushy_storage/_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,220 +1,237 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import os
-import zlib
-import lzma
-import json
-import pickle
-import hashlib
-import threading
-from pathlib import Path
-from typing import MutableMapping, Callable, Tuple, Union, Any, List
-
-from cushy_storage.base import EnhancedList, BASE_TYPE
-from cushy_storage.utils import get_default_cache_path
-
-__all__ = ['BaseDict', 'CushyDict', 'disk_cache']
-
-# Compression algorithms and their corresponding functions
-_COMPRESS = {
-    'zlib': (
-        zlib.compress,
-        zlib.decompress,
-    ),
-    'lzma': (
-        lzma.compress,
-        lzma.decompress,
-    ),
-}
-
-# Serialization algorithms and their corresponding functions
-_SERIALIZATION = {
-    'pickle': (
-        pickle.dumps,
-        pickle.loads,
-    ),
-    'json': (
-        lambda x: json.dumps(x, sort_keys=True, ensure_ascii=False, separators=(',', ':')).encode('utf8'),
-        json.loads,
-    ),
-}
-
-# Locks for each hash value (hexadecimal representation of 0-255)
-_LOCKS = {hex(i)[2:].zfill(2): threading.Lock() for i in range(256)}
-
-
-def _method_convert_helper(s: Union[str, Tuple[Callable, Callable], None], d: dict) -> Tuple[Callable, Callable]:
-    """
-    Helper function to get the compression or serialization functions based on input parameter
-    """
-    if s is None:
-        return lambda x: x, lambda x: x
-    elif isinstance(s, str):
-        return d[s]
-    else:
-        return s
-
-
-class BaseDict(MutableMapping[str, bytes]):
-    def __init__(self, path: str, compress: Union[str, Tuple[Callable, Callable], None] = None):
-        self.path = Path(path)
-        if self.path.is_file():
-            raise Exception('path has exist')  # Raise an exception if the path already exists as a file
-        self.path.mkdir(parents=True, exist_ok=True)
-        self.dirs = set()
-        self.compress, self.decompress = _method_convert_helper(compress, _COMPRESS)
-
-    def __contains__(self, k: str):
-        """
-        Check if the file exists in the cache
-
-        Args:
-            k: key
-
-        Examples:
-            from cushy_storage import CushyDict
-
-            cache = CushyDict()
-            if 'my_key' in cache:
-                print("[my_key] in my cache")
-            else:
-                print("[my_key] not in my cache")
-        """
-        return (self.path / k[:2] / (k[2:] + '_')).is_file()
-
-    def __getitem__(self, k: str):
-        """
-        Retrieve the cached item using its key and decompress it
-        """
-        if k not in self:
-            raise KeyError(k)
-        rk = hashlib.md5(k.encode('utf8')).hexdigest()[:2]
-        with _LOCKS[rk]:
-            with open(self.path / k[:2] / (k[2:] + '_'), 'rb') as f:
-                t = f.read()
-        return self.decompress(t)
-
-    def __setitem__(self, k: str, v: bytes):
-        """
-        Compress the value and store it in the cache using its key
-        """
-        if k[:2] not in self.dirs:
-            (self.path / k[:2]).mkdir(exist_ok=True)
-            self.dirs.add(k[:2])
-        t = self.compress(v)
-        rk = hashlib.md5(k.encode('utf8')).hexdigest()[:2]
-        with _LOCKS[rk]:
-            with open(self.path / k[:2] / (k[2:] + '_'), 'wb') as f:
-                f.write(t)
-
-    def __delitem__(self, k: str):
-        """
-        Remove the cached item using its key
-        """
-        os.remove(self.path / k[:2] / (k[2:] + '_'))
-
-    def __len__(self):
-        """
-        Get the total number of items in the cache
-        """
-        return sum([len(os.listdir(self.path / a)) for a in os.listdir(self.path)])
-
-    def __iter__(self):
-        """
-        Iterate over all keys in the cache
-        """
-        for a in os.listdir(self.path):
-            for b in os.listdir(self.path / a):
-                yield a + b[:-1]
-
-
-class CushyDict(BaseDict):
-    """
-    A subclass of BaseDict that can serialize and deserialize values using different algorithms
-    """
-
-    def __init__(
-            self,
-            path: str = get_default_cache_path(),
-            compress: Union[str, Tuple[Callable, Callable], None] = None,
-            serialize: Union[str, Tuple[Callable, Callable], None] = 'json'
-    ):
-        """
-        Args:
-            path: the path to save
-            compress: zlib or lzma
-            serialize: json or pickle
-        """
-        super().__init__(path, compress)
-        self.serialize, self.deserialize = _method_convert_helper(serialize, _SERIALIZATION)
-
-    def __getitem__(self, k: str) -> Any:
-        ret = self.deserialize(super().__getitem__(k))
-
-        if isinstance(ret, list):
-            ret: List = EnhancedList(ret)
-        return ret
-
-    def __setitem__(self, k: str, v: Any):
-        if isinstance(v, list) and self.deserialize is json.loads and len(v) > 0 and type(v[0]) not in BASE_TYPE:
-            raise ValueError((
-                f"Can not use 'json' to serialize your '{type(v[0])}' data in '{k}'. If you want to store "
-                "complex data or custom data, please use 'pickle' to serialize."
-            ))
-        return super().__setitem__(k, self.serialize(v))
-
-
-def disk_cache(path: str = None, compress: str = None, serialize: str = 'json'):
-    """
-    Decorator that caches the output of a function to disk
-    """
-    if serialize not in ['pickle', 'json']:
-        ValueError("Your serializer must be 'pickle' or 'json'")
-    dump = _method_convert_helper(serialize, _SERIALIZATION)[0]
-
-    def decorator(func):
-        nonlocal path
-        name = func.__name__
-        if path is None:
-            # If no cache path is specified, create a default one based on the function name and serialization algorithm
-            path = f'./_cushycache_{name}_{serialize}'
-        map = CushyDict(path, serialize=serialize, compress=compress)
-
-        def cached_func(*args, **kwargs):
-            # Serialize the function arguments and use their MD5 hash as the cache key
-            input_data = [name, args, kwargs]
-            md5 = hashlib.md5(dump(input_data)).hexdigest()
-            ext = 'pkl' if serialize == 'pickle' else 'json'
-            filename = f'{md5}.{ext}'
-
-            if filename in map:
-                # If the cached output exists, return it
-                input_data, output_data = map[filename]
-                return output_data
-            else:
-                # Otherwise, call the original function and cache its output
-                output_data = func(*args, **kwargs)
-                cache_data = [input_data, output_data]
-                map[filename] = cache_data
-                return output_data
-
-        return cached_func
-
-    return decorator
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import os
+import zlib
+import lzma
+import json
+import pickle
+import hashlib
+import threading
+from pathlib import Path
+from typing import MutableMapping, Callable, Tuple, Union, Any, List
+
+from cushy_storage.base import EnhancedList, BASE_TYPE
+from cushy_storage.utils import get_default_cache_path
+
+__all__ = ["BaseDict", "CushyDict", "disk_cache"]
+
+# Compression algorithms and their corresponding functions
+_COMPRESS = {
+    "zlib": (
+        zlib.compress,
+        zlib.decompress,
+    ),
+    "lzma": (
+        lzma.compress,
+        lzma.decompress,
+    ),
+}
+
+# Serialization algorithms and their corresponding functions
+_SERIALIZATION = {
+    "pickle": (
+        pickle.dumps,
+        pickle.loads,
+    ),
+    "json": (
+        lambda x: json.dumps(
+            x, sort_keys=True, ensure_ascii=False, separators=(",", ":")
+        ).encode("utf8"),
+        json.loads,
+    ),
+}
+
+# Locks for each hash value (hexadecimal representation of 0-255)
+_LOCKS = {hex(i)[2:].zfill(2): threading.Lock() for i in range(256)}
+
+
+def _method_convert_helper(
+        s: Union[str, Tuple[Callable, Callable], None], d: dict
+) -> Tuple[Callable, Callable]:
+    """
+    Helper function to get the compression or serialization functions based on input parameter
+    """
+    if s is None:
+        return lambda x: x, lambda x: x
+    elif isinstance(s, str):
+        return d[s]
+    else:
+        return s
+
+
+class BaseDict(MutableMapping[str, bytes]):
+    def __init__(
+            self, path: str, compress: Union[str, Tuple[Callable, Callable], None] = None
+    ):
+        self.path = Path(path)
+        if self.path.is_file():
+            raise Exception(
+                "path has exist"
+            )  # Raise an exception if the path already exists as a file
+        self.path.mkdir(parents=True, exist_ok=True)
+        self.dirs = set()
+        self.compress, self.decompress = _method_convert_helper(compress, _COMPRESS)
+
+    def __contains__(self, k: str):
+        """
+        Check if the file exists in the cache
+
+        Args:
+            k: key
+
+        Examples:
+            from cushy_storage import CushyDict
+
+            cache = CushyDict()
+            if 'my_key' in cache:
+                print("[my_key] in my cache")
+            else:
+                print("[my_key] not in my cache")
+        """
+        return (self.path / k[:2] / (k[2:] + "_")).is_file()
+
+    def __getitem__(self, k: str):
+        """
+        Retrieve the cached item using its key and decompress it
+        """
+        if k not in self:
+            raise KeyError(k)
+        rk = hashlib.md5(k.encode("utf8")).hexdigest()[:2]
+        with _LOCKS[rk]:
+            with open(self.path / k[:2] / (k[2:] + "_"), "rb") as f:
+                t = f.read()
+        return self.decompress(t)
+
+    def __setitem__(self, k: str, v: bytes):
+        """
+        Compress the value and store it in the cache using its key
+        """
+        if k[:2] not in self.dirs:
+            (self.path / k[:2]).mkdir(exist_ok=True)
+            self.dirs.add(k[:2])
+        t = self.compress(v)
+        rk = hashlib.md5(k.encode("utf8")).hexdigest()[:2]
+        with _LOCKS[rk]:
+            with open(self.path / k[:2] / (k[2:] + "_"), "wb") as f:
+                f.write(t)
+
+    def __delitem__(self, k: str):
+        """
+        Remove the cached item using its key
+        """
+        os.remove(self.path / k[:2] / (k[2:] + "_"))
+
+    def __len__(self):
+        """
+        Get the total number of items in the cache
+        """
+        return sum([len(os.listdir(self.path / a)) for a in os.listdir(self.path)])
+
+    def __iter__(self):
+        """
+        Iterate over all keys in the cache
+        """
+        for a in os.listdir(self.path):
+            for b in os.listdir(self.path / a):
+                yield a + b[:-1]
+
+
+class CushyDict(BaseDict):
+    """
+    A subclass of BaseDict that can serialize and deserialize values using different algorithms
+    """
+
+    def __init__(
+            self,
+            path: str = get_default_cache_path(),
+            compress: Union[str, Tuple[Callable, Callable], None] = None,
+            serialize: Union[str, Tuple[Callable, Callable], None] = "json",
+    ):
+        """
+        Args:
+            path: the path to save
+            compress: zlib or lzma
+            serialize: json or pickle
+        """
+        super().__init__(path, compress)
+        self.serialize, self.deserialize = _method_convert_helper(
+            serialize, _SERIALIZATION
+        )
+
+    def __getitem__(self, k: str) -> Any:
+        ret = self.deserialize(super().__getitem__(k))
+
+        if isinstance(ret, list):
+            ret: List = EnhancedList(ret)
+        return ret
+
+    def __setitem__(self, k: str, v: Any):
+        if (
+                isinstance(v, list)
+                and self.deserialize is json.loads
+                and len(v) > 0
+                and type(v[0]) not in BASE_TYPE
+        ):
+            raise ValueError(
+                (
+                    f"Can not use 'json' to serialize your '{type(v[0])}' data in '{k}'. If you want to store "
+                    "complex data or custom data, please use 'pickle' to serialize."
+                )
+            )
+        return super().__setitem__(k, self.serialize(v))
+
+
+def disk_cache(path: str = None, compress: str = None, serialize: str = "json"):
+    """
+    Decorator that caches the output of a function to disk
+    """
+    if serialize not in ["pickle", "json"]:
+        ValueError("Your serializer must be 'pickle' or 'json'")
+    dump = _method_convert_helper(serialize, _SERIALIZATION)[0]
+
+    def decorator(func):
+        nonlocal path
+        name = func.__name__
+        if path is None:
+            # If no cache path is specified, create a default one based on the function name and serialization algorithm
+            path = f"./_cushycache_{name}_{serialize}"
+        map = CushyDict(path, serialize=serialize, compress=compress)
+
+        def cached_func(*args, **kwargs):
+            # Serialize the function arguments and use their MD5 hash as the cache key
+            input_data = [name, args, kwargs]
+            md5 = hashlib.md5(dump(input_data)).hexdigest()
+            ext = "pkl" if serialize == "pickle" else "json"
+            filename = f"{md5}.{ext}"
+
+            if filename in map:
+                # If the cached output exists, return it
+                input_data, output_data = map[filename]
+                return output_data
+            else:
+                # Otherwise, call the original function and cache its output
+                output_data = func(*args, **kwargs)
+                cache_data = [input_data, output_data]
+                map[filename] = cache_data
+                return output_data
+
+        return cached_func
+
+    return decorator
```

### Comparing `cushy-storage-1.1.1/cushy_storage/base.py` & `cushy-storage-1.1.3/cushy_storage/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-from typing import List
-
-BASE_TYPE = [
-    int, str, float, dict, list, tuple, bytes
-]
-
-
-class EnhancedList(list):
-    """Custom List to provide more functions"""
-
-    def append(self, __object) -> List:
-        super().append(__object)
-        return self
-
-    def remove(self, __value) -> List:
-        super().remove(__value)
-        return self
-
-    def insert(self, __index, __object) -> List:
-        super().insert(__index, __object)
-        return self
-
-    def pop(self, __index=...) -> List:
-        super().pop(__index)
-        return self
-
-    def reverse(self) -> List:
-        super().reverse()
-        return self
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+from typing import List
+
+BASE_TYPE = [int, str, float, dict, list, tuple, bytes]
+
+
+class EnhancedList(list):
+    """Custom List to provide more functions"""
+
+    def append(self, __object) -> List:
+        super().append(__object)
+        return self
+
+    def remove(self, __value) -> List:
+        super().remove(__value)
+        return self
+
+    def insert(self, __index, __object) -> List:
+        super().insert(__index, __object)
+        return self
+
+    def pop(self, __index=...) -> List:
+        super().pop(__index)
+        return self
+
+    def reverse(self) -> List:
+        super().reverse()
+        return self
```

### Comparing `cushy-storage-1.1.1/cushy_storage/utils.py` & `cushy-storage-1.1.3/cushy_storage/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import os
-import tempfile
-import platform
-
-
-def get_project_root_path() -> str:
-    """get project root path"""
-    project_path = os.getcwd()
-    max_depth = 10
-    count = 0
-    while not os.path.exists(os.path.join(project_path, 'README.md')):
-        project_path = os.path.split(project_path)[0]
-        count += 1
-        if count > max_depth:
-            return os.getcwd()
-    return project_path
-
-
-def get_default_storage_path(file_name) -> str:
-    if platform.system() == 'Windows':
-        return f"./{file_name}"
-    elif platform.system() == 'Linux':
-        dir_path = os.environ.get('TMPDIR')
-        if not dir_path:
-            dir_path = tempfile.gettempdir()
-        dir_path = os.path.join(dir_path, "prompt_me")
-        return f"{dir_path}/{file_name}"
-
-
-def get_default_cache_path() -> str:
-    return get_default_storage_path("cache")
-
-
-def get_default_log_path() -> str:
-    return get_default_storage_path("log")
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import os
+import tempfile
+import platform
+
+
+def get_project_root_path() -> str:
+    """get project root path"""
+    project_path = os.getcwd()
+    max_depth = 10
+    count = 0
+    while not os.path.exists(os.path.join(project_path, "README.md")):
+        project_path = os.path.split(project_path)[0]
+        count += 1
+        if count > max_depth:
+            return os.getcwd()
+    return project_path
+
+
+def get_default_storage_path(file_name) -> str:
+    if platform.system() == "Windows":
+        return f"./{file_name}"
+    elif platform.system() == "Linux" or "Darwin":
+        dir_path = os.environ.get("TMPDIR")
+        if not dir_path:
+            dir_path = tempfile.gettempdir()
+        dir_path = os.path.join(dir_path, "cushy_storage")
+        return f"{dir_path}/{file_name}"
+    else:
+        return f"./{file_name}"
+
+
+def get_default_cache_path() -> str:
+    return get_default_storage_path("cache")
+
+
+def get_default_log_path() -> str:
+    return get_default_storage_path("log")
```

### Comparing `cushy-storage-1.1.1/cushy_storage.egg-info/PKG-INFO` & `cushy-storage-1.1.3/cushy_storage.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,369 +1,371 @@
-Metadata-Version: 2.1
-Name: cushy-storage
-Version: 1.1.1
-Summary: A data local persistence framework library
-Home-page: https://github.com/Undertone0809/cushy-storage
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: storage,serialization,json,cushy-storage,cushy_storage
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    cushy-storage
-</h1>
-<p align="center">
-  <strong>一个基于磁盘缓存的ORM框架</strong>
-</p>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
-   </a>
-</p>
-
-[English](/README_en.md) [中文](/README.md)
-
-# 简介
-
-cushy-storage是一个基于磁盘缓存的ORM框架，你可以使用轻松的将自定义的数据通过ORM进行增删改查；另一方面，cushy-storage让你无需花费精力在
-如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。如果你有对本地文件数据操作的需求，使用本框架可以轻松的进行数据的本地存储。
-
-# 特性
-
-- 支持ORM存储、基本数据存储、自定义数据存储，兼容所有数据类型
-- 支持ORM框架级对象操作，可以轻松地对对象级数据进行增删改查
-- 存储基本数据时像操作dict一样读写，十分方便
-- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
-- 免去了直接操作文件的工作
-- 提供多种序列化操作
-- 提供多种数据压缩方式
-
-# 安装
-
-```bash
-pip install cushy-storage --upgrade 
-```
-
-# 快速上手
-
-`cushy-storage` 的使用主要分为四个部分，`CushyOrmCache` `CushyDict` `BaseDict` `disk_cache` 
-
-- `CushyOrmCache` 基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查
-- `CushyDict`: `BaseDict`的增强版，存储各种类型的数据，包括基本数据类型与自定义数据类型
-- `BaseDict`: 存储基础的二进制数据
-- `disk_cache`: 函数数据缓存
-
-## CushyOrmCache
-
-CushyOrmCache是一个基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查，下面，我们将会用一些简单的场景介绍其使用方法。
-
-现在我们需要构建一个简单的用户系统，用户系统的数据我们直接保存在本地文件中（当前对象级数据只支持pickle序列化的形式存储），用户的字段简单就好，
-只需要一个name和一个age，则我们可以构建如下的操作。
-
-```python
-from cushy_storage.orm import BaseORMModel, CushyOrmCache
-
-class User(BaseORMModel):
-
-    def __init__(self, name, age):
-        super().__init__()
-        self.name = name
-        self.age = age
-```
-
-这个示例中，我们实现了一个`User`类，并且继承了`BaseORMModel`，在`cushy-storage`中，如果你想让你的类可以进行ORM操作，就必须要继承这个类。
-接着，我们需要初始化`CushyOrmCache`。
-
-```python
-orm_cache = CushyOrmCache()
-```
-
-接着，你就可以直接进行`User`的增删改查操作了。
-
-```python
-"""add user"""
-user = User("jack", 18)
-orm_cache.add(user)
-user = User("jasmine", 18)
-orm_cache.add(user)
-
-"""query all user"""
-users = orm_cache.query(User).all()
-orm_cache.query(User).print_all()
-
-"""query by filter"""
-# get all user, you will get a List[User] type data.
-# Actually, it will get two users named "jack" and "jasmine".
-orm_cache.query("User").filter(age=18).all()
-# get first in queryset, you will get a User type data
-orm_cache.query("User").filter(name="jack").first()
-# filter by multiple parameters
-orm_cache.query("User").filter(name="jack", age=18).first()
-
-"""update"""
-user = orm_cache.query("User").filter(name='jack').first()
-user.age = 18
-orm_cache.update_obj(user)
-
-"""delete"""
-user = orm_cache.query("User").filter(name="jack").first()
-orm_cache.delete(user)
-orm_cache.query(User).print_all()
-
-```
-
-完整代码如下：
-
-```python
-from cushy_storage.orm import BaseORMModel, CushyOrmCache
-
-
-class User(BaseORMModel):
-
-    def __init__(self, name, age):
-        super().__init__()
-        self.name = name
-        self.age = age
-
-
-orm_cache = CushyOrmCache()
-
-"""add user"""
-user = User("jack", 18)
-orm_cache.add(user)
-user = User("jasmine", 18)
-orm_cache.add(user)
-
-"""query all user"""
-users = orm_cache.query(User).all()
-orm_cache.query(User).print_all()
-
-"""query by filter"""
-# get all user, you will get a List[User] type data.
-# Actually, it will get two users named "jack" and "jasmine".
-orm_cache.query("User").filter(age=18).all()
-# get first in queryset, you will get a User type data
-orm_cache.query("User").filter(name="jack").first()
-# filter by multiple parameters
-orm_cache.query("User").filter(name="jack", age=18).first()
-
-"""update"""
-user = orm_cache.query("User").filter(name='jack').first()
-user.age = 18
-orm_cache.update_obj(user)
-
-"""delete"""
-user = orm_cache.query("User").filter(name="jack").first()
-orm_cache.delete(user)
-orm_cache.query(User).print_all()
-
-```
-
-> 需要注意的是，你可以通过在query()中传入User对象来进行数据的查询，也可以直接传入"User"字符串进行数据的查询（这里的设计思路和数据库的表是一样的
-，User是表名）
-
-## BaseDict
-
-BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
-
-```python
-from cushy_storage import BaseDict
-
-# 初始化cache，保存在./data文件夹下
-cache = BaseDict('./data')
-# Base Dict只能存储二进制数据，可以用于流式传输
-cache['key'] = b'value'
-value = cache['key']
-print(value)
-
-```
-
-## CushyDict类
-
-CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
-此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
-一些简单的使用教程。
-
-- 存储Python基本数据类型
-
-```python
-from cushy_storage import CushyDict
-
-# 初始化cache，保存在./data文件夹下
-cache = CushyDict('./data')
-
-cache['key'] = {'value': 42}
-print(cache['key'])
-
-cache['a'] = 1
-print(cache['a'])
-
-cache['b'] = "hello world"
-print(cache['b'])
-
-cache['arr'] = [1, 2, 3, 4, 5]
-print(cache['arr'])
-
-```
-
-> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
-
-- 生成结果
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
-
-- 存储自定义数据类型
-
-```python
-from cushy_storage import CushyDict
-
-
-class User:
-    def __init__(self, name, age):
-        self.name = name
-        self.age = age
-
-
-def main():
-    cache = CushyDict(serialize='pickle')
-    user = User("Jack", 18)
-    cache['user'] = user
-
-    user = cache['user']
-    print(type(user))
-    print(cache['user'].name)
-    print(cache['user'].age)
-
-
-if __name__ == '__main__':
-    main()
-```
-
-> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
-
-- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-```
-
-- 判断key是否存在（和字典操作同理）
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-if 'key' in cache:
-    print("key exist")
-else:
-    print("key not exist")
-
-```
-
-## disk_cache装饰器
-
-disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
-
-```python
-from cushy_storage import disk_cache
-
-
-@disk_cache('./data')
-def my_func():
-    return {'value': 42}
-
-
-result = my_func()
-
-```
-
-# QA
-
-## 如何在一个大项目里全局只使用一个cache?
-
-你可以通过构建一个`utils.py`，对外暴露一个`get_cache()`函数，让需要`cache`的模块都通过`get_cache()`来获取`cache`
-，一个简单的示例如下：
-
-- `utils.py`
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-
-
-def get_cache():
-    return cache
-```
-
-- `app.py`
-
-```python
-from utils import get_cache
-
-
-def main():
-    cache = get_cache()
-
-```
-
-# 待办
-
-- [x] 提供单例模式解决方案，提供更加方便的工具类
-- [x] 支持多种压缩和序列化算法，以满足不同类型数据的需求
-- [x] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
-- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
-- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
-- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
-- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
-- [ ] 改善文档结构和代码注释，方便用户理解和使用库
-- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
-- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
-- [x] 支持更多数据格式的持久化方式，如json的直接存储
-- [x] 提供ORM框架，封装对象级的CRUD操作
-- [ ] 提供ORM的事务模式
-- [ ] 为ORM提供更加细粒度的filter，如模糊匹配、大小比较等
-- [ ] 提供操作日志记录
-- [ ] 提供缓存文件分布记录
-- [ ] 提升json存储数据的可读性
-- [ ] 提供自定义的数据导出、转换形式
-
-# 鸣谢
-
-本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
-进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
-
-This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
-RimoChan for his great work.
-
-# 贡献
-
-如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: cushy-storage
+Version: 1.1.3
+Summary: A data local persistence ORM framework
+Home-page: https://github.com/Undertone0809/cushy-storage
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: storage,ORM,serialization,json,cushy-storage,cushy_storage
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    cushy-storage
+</h1>
+<p align="center">
+  <strong>一个基于磁盘缓存的ORM框架</strong>
+</p>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/cushy-storage?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
+   </a>
+</p>
+
+[English](/README_en.md) [中文](/README.md)
+
+# 简介
+
+cushy-storage是一个基于磁盘缓存的ORM框架，你可以使用轻松的将自定义的数据通过ORM进行增删改查；另一方面，cushy-storage让你无需花费精力在
+如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。如果你有对本地文件数据操作的需求，使用本框架可以轻松的进行数据的本地存储。
+
+# 特性
+
+- 支持ORM存储、基本数据存储、自定义数据存储，兼容所有数据类型
+- 支持ORM框架级对象操作，可以轻松地对对象级数据进行增删改查
+- 存储基本数据时像操作dict一样读写，十分方便
+- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
+- 免去了直接操作文件的工作
+- 提供多种序列化操作
+- 提供多种数据压缩方式
+
+# 安装
+
+```bash
+pip install cushy-storage --upgrade 
+```
+
+# 快速上手
+
+`cushy-storage` 的使用主要分为四个部分，`CushyOrmCache` `CushyDict` `BaseDict` `disk_cache` 
+
+- `CushyOrmCache` 基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查
+- `CushyDict`: `BaseDict`的增强版，存储各种类型的数据，包括基本数据类型与自定义数据类型
+- `BaseDict`: 存储基础的二进制数据
+- `disk_cache`: 函数数据缓存
+
+## CushyOrmCache
+
+CushyOrmCache是一个基于ORM框架的对象存储，可以十分方便的对对象级数据进行增删改查，下面，我们将会用一些简单的场景介绍其使用方法。
+
+现在我们需要构建一个简单的用户系统，用户系统的数据我们直接保存在本地文件中（当前对象级数据只支持pickle序列化的形式存储），用户的字段简单就好，
+只需要一个name和一个age，则我们可以构建如下的操作。
+
+```python
+from cushy_storage.orm import BaseORMModel, CushyOrmCache
+
+class User(BaseORMModel):
+
+    def __init__(self, name, age):
+        super().__init__()
+        self.name = name
+        self.age = age
+```
+
+这个示例中，我们实现了一个`User`类，并且继承了`BaseORMModel`，在`cushy-storage`中，如果你想让你的类可以进行ORM操作，就必须要继承这个类。
+接着，我们需要初始化`CushyOrmCache`。
+
+```python
+orm_cache = CushyOrmCache()
+```
+
+接着，你就可以直接进行`User`的增删改查操作了。
+
+```python
+"""add user"""
+user = User("jack", 18)
+orm_cache.add(user)
+user = User("jasmine", 18)
+orm_cache.add(user)
+# or you can pass a list
+orm_cache.add([User("Zeeland", 10), User("Zero", 20)])
+
+"""query all user"""
+users = orm_cache.query(User).all()
+orm_cache.query(User).print_all()
+
+"""query by filter"""
+# get all user, you will get a List[User] type data.
+# Actually, it will get two users named "jack" and "jasmine".
+orm_cache.query("User").filter(age=18).all()
+# get first in queryset, you will get a User type data
+orm_cache.query("User").filter(name="jack").first()
+# filter by multiple parameters
+orm_cache.query("User").filter(name="jack", age=18).first()
+
+"""update"""
+user = orm_cache.query("User").filter(name='jack').first()
+user.age = 18
+orm_cache.update_obj(user)
+
+"""delete"""
+user = orm_cache.query("User").filter(name="jack").first()
+orm_cache.delete(user)
+orm_cache.query(User).print_all()
+
+```
+
+完整代码如下：
+
+```python
+from cushy_storage.orm import BaseORMModel, CushyOrmCache
+
+
+class User(BaseORMModel):
+
+    def __init__(self, name, age):
+        super().__init__()
+        self.name = name
+        self.age = age
+
+
+orm_cache = CushyOrmCache()
+
+"""add user"""
+user = User("jack", 18)
+orm_cache.add(user)
+user = User("jasmine", 18)
+orm_cache.add(user)
+
+"""query all user"""
+users = orm_cache.query(User).all()
+orm_cache.query(User).print_all()
+
+"""query by filter"""
+# get all user, you will get a List[User] type data.
+# Actually, it will get two users named "jack" and "jasmine".
+orm_cache.query("User").filter(age=18).all()
+# get first in queryset, you will get a User type data
+orm_cache.query("User").filter(name="jack").first()
+# filter by multiple parameters
+orm_cache.query("User").filter(name="jack", age=18).first()
+
+"""update"""
+user = orm_cache.query("User").filter(name='jack').first()
+user.age = 18
+orm_cache.update_obj(user)
+
+"""delete"""
+user = orm_cache.query("User").filter(name="jack").first()
+orm_cache.delete(user)
+orm_cache.query(User).print_all()
+
+```
+
+> 需要注意的是，你可以通过在query()中传入User对象来进行数据的查询，也可以直接传入"User"字符串进行数据的查询（这里的设计思路和数据库的表是一样的
+，User是表名）
+
+## BaseDict
+
+BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
+
+```python
+from cushy_storage import BaseDict
+
+# 初始化cache，保存在./data文件夹下
+cache = BaseDict('./data')
+# Base Dict只能存储二进制数据，可以用于流式传输
+cache['key'] = b'value'
+value = cache['key']
+print(value)
+
+```
+
+## CushyDict类
+
+CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
+此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
+一些简单的使用教程。
+
+- 存储Python基本数据类型
+
+```python
+from cushy_storage import CushyDict
+
+# 初始化cache，保存在./data文件夹下
+cache = CushyDict('./data')
+
+cache['key'] = {'value': 42}
+print(cache['key'])
+
+cache['a'] = 1
+print(cache['a'])
+
+cache['b'] = "hello world"
+print(cache['b'])
+
+cache['arr'] = [1, 2, 3, 4, 5]
+print(cache['arr'])
+
+```
+
+> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
+
+- 生成结果
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
+
+- 存储自定义数据类型
+
+```python
+from cushy_storage import CushyDict
+
+
+class User:
+    def __init__(self, name, age):
+        self.name = name
+        self.age = age
+
+
+def main():
+    cache = CushyDict(serialize='pickle')
+    user = User("Jack", 18)
+    cache['user'] = user
+
+    user = cache['user']
+    print(type(user))
+    print(cache['user'].name)
+    print(cache['user'].age)
+
+
+if __name__ == '__main__':
+    main()
+```
+
+> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
+
+- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+```
+
+- 判断key是否存在（和字典操作同理）
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
+
+```
+
+## disk_cache装饰器
+
+disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
+
+```python
+from cushy_storage import disk_cache
+
+
+@disk_cache('./data')
+def my_func():
+    return {'value': 42}
+
+
+result = my_func()
+
+```
+
+# QA
+
+## 如何在一个大项目里全局只使用一个cache?
+
+你可以通过构建一个`utils.py`，对外暴露一个`get_cache()`函数，让需要`cache`的模块都通过`get_cache()`来获取`cache`
+，一个简单的示例如下：
+
+- `utils.py`
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+
+
+def get_cache():
+    return cache
+```
+
+- `app.py`
+
+```python
+from utils import get_cache
+
+
+def main():
+    cache = get_cache()
+
+```
+
+# 待办
+
+- [x] 提供单例模式解决方案，提供更加方便的工具类
+- [x] 支持多种压缩和序列化算法，以满足不同类型数据的需求
+- [x] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
+- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
+- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
+- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
+- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
+- [ ] 改善文档结构和代码注释，方便用户理解和使用库
+- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
+- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
+- [x] 支持更多数据格式的持久化方式，如json的直接存储
+- [x] 提供ORM框架，封装对象级的CRUD操作
+- [ ] 提供ORM的事务模式
+- [ ] 为ORM提供更加细粒度的filter，如模糊匹配、大小比较等
+- [ ] 提供操作日志记录
+- [ ] 提供缓存文件分布记录
+- [ ] 提升json存储数据的可读性
+- [ ] 提供自定义的数据导出、转换形式
+
+# 鸣谢
+
+本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
+进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
+
+This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
+RimoChan for his great work.
+
+# 贡献
+
+如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `cushy-storage-1.1.1/setup.py` & `cushy-storage-1.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-# Copyright 2022 Zeeland(https://github.com/Undertone0809/). All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import setuptools
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-setuptools.setup(
-    name="cushy-storage",
-    version="1.1.1",
-    author="Zeeland",
-    author_email="zeeland@foxmail.com",
-    description="A data local persistence framework library",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Undertone0809/cushy-storage",
-    packages=setuptools.find_packages(),
-    license="Apache 2.0",
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-
-    ],
-    keywords="storage, serialization, json, cushy-storage, cushy_storage",
-)
+# Copyright 2022 Zeeland(https://github.com/Undertone0809/). All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import setuptools
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+setuptools.setup(
+    name="cushy-storage",
+    version="1.1.3",
+    author="Zeeland",
+    author_email="zeeland@foxmail.com",
+    description="A data local persistence ORM framework",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Undertone0809/cushy-storage",
+    packages=setuptools.find_packages(),
+    license="Apache 2.0",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    keywords="storage, ORM, serialization, json, cushy-storage, cushy_storage",
+)
```

### Comparing `cushy-storage-1.1.1/tests/test_base_dict.py` & `cushy-storage-1.1.3/tests/test_base_dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import unittest
-from cushy_storage import BaseDict
-
-
-class TestBaseDict(unittest.TestCase):
-    def test_basic_operations(self):
-        cache = BaseDict('./cache/test-base-dict')
-
-        # Test adding items to the cache
-        cache['foo'] = b'bar'
-        self.assertEqual(cache['foo'], b'bar')
-
-        # Test deleting items from the cache
-        del cache['foo']
-        with self.assertRaises(KeyError):
-            cache['foo']
-
-        # Test checking if an item is in the cache
-        self.assertFalse('foo' in cache)
-
-    def test_compression(self):
-        cache = BaseDict('./cache/test-base-dict', compress='lzma')
-
-        # Test storing and retrieving a large string in the cache using LZMA compression
-        data = 'a' * (1024 * 1024)
-        cache['big_data'] = data.encode()
-        self.assertEqual(cache['big_data'].decode(), data)
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import unittest
+from cushy_storage import BaseDict
+
+
+class TestBaseDict(unittest.TestCase):
+    def test_basic_operations(self):
+        cache = BaseDict("./cache/test-base-dict")
+
+        # Test adding items to the cache
+        cache["foo"] = b"bar"
+        self.assertEqual(cache["foo"], b"bar")
+
+        # Test deleting items from the cache
+        del cache["foo"]
+        with self.assertRaises(KeyError):
+            cache["foo"]
+
+        # Test checking if an item is in the cache
+        self.assertFalse("foo" in cache)
+
+    def test_compression(self):
+        cache = BaseDict("./cache/test-base-dict", compress="lzma")
+
+        # Test storing and retrieving a large string in the cache using LZMA compression
+        data = "a" * (1024 * 1024)
+        cache["big_data"] = data.encode()
+        self.assertEqual(cache["big_data"].decode(), data)
```

### Comparing `cushy-storage-1.1.1/tests/test_dict_cache.py` & `cushy-storage-1.1.3/tests/test_dict_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import time
-import unittest
-from cushy_storage import CushyDict, disk_cache
-
-
-class TestDiskCache(unittest.TestCase):
-    def test_basic_usage(self):
-        @disk_cache('./cache/test-disk-cache')
-        def slow_function(x):
-            time.sleep(0.1)
-            return x + 1
-
-        # Test calling the function with different arguments and caching the output
-        self.assertEqual(slow_function(5), 6)
-        self.assertEqual(slow_function(5), 6)  # Should use cache this time
-        self.assertEqual(slow_function(10), 11)
-
-    def test_serialization(self):
-        @disk_cache('./cache/test-disk-cache-serialize', serialize='pickle')
-        def slow_function(x):
-            time.sleep(0.1)
-            return {'result': x}
-
-        # Test caching the output of a function that returns a dictionary using pickle serialization
-        self.assertEqual(slow_function(5), {'result': 5})
-        self.assertEqual(slow_function(5), {'result': 5})  # Should use cache this time
-        self.assertEqual(slow_function(10), {'result': 10})
-
-    def test_compression(self):
-        @disk_cache('./cache/test-disk-cache-compress', compress='lzma')
-        def slow_function(x):
-            time.sleep(0.1)
-            return 'a' * (1024 * 1024)
-
-        # Test caching the output of a function that returns a large string using LZMA compression
-        self.assertEqual(slow_function(5), 'a' * (1024 * 1024))
-        self.assertEqual(slow_function(5), 'a' * (1024 * 1024))  # Should use cache this time
-        self.assertEqual(slow_function(10), 'a' * (1024 * 1024))
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import time
+import unittest
+from cushy_storage import CushyDict, disk_cache
+
+
+class TestDiskCache(unittest.TestCase):
+    def test_basic_usage(self):
+        @disk_cache("./cache/test-disk-cache")
+        def slow_function(x):
+            time.sleep(0.1)
+            return x + 1
+
+        # Test calling the function with different arguments and caching the output
+        self.assertEqual(slow_function(5), 6)
+        self.assertEqual(slow_function(5), 6)  # Should use cache this time
+        self.assertEqual(slow_function(10), 11)
+
+    def test_serialization(self):
+        @disk_cache("./cache/test-disk-cache-serialize", serialize="pickle")
+        def slow_function(x):
+            time.sleep(0.1)
+            return {"result": x}
+
+        # Test caching the output of a function that returns a dictionary using pickle serialization
+        self.assertEqual(slow_function(5), {"result": 5})
+        self.assertEqual(slow_function(5), {"result": 5})  # Should use cache this time
+        self.assertEqual(slow_function(10), {"result": 10})
+
+    def test_compression(self):
+        @disk_cache("./cache/test-disk-cache-compress", compress="lzma")
+        def slow_function(x):
+            time.sleep(0.1)
+            return "a" * (1024 * 1024)
+
+        # Test caching the output of a function that returns a large string using LZMA compression
+        self.assertEqual(slow_function(5), "a" * (1024 * 1024))
+        self.assertEqual(
+            slow_function(5), "a" * (1024 * 1024)
+        )  # Should use cache this time
+        self.assertEqual(slow_function(10), "a" * (1024 * 1024))
```

### Comparing `cushy-storage-1.1.1/tests/test_orm.py` & `cushy-storage-1.1.3/tests/test_orm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,131 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import unittest
-from typing import List
-
-from cushy_storage.orm import QuerySet
-from cushy_storage import CushyOrmCache, BaseORMModel
-from cushy_storage.logger import enable_log
-from tests.utils import delete_cache
-
-cache_file = {
-    "test_orm_add_and_query": "./cache/test-cushy-orm-cache",
-    "test_orm_delete": "./cache/test-cushy-orm-cache-orm-delete",
-    "test_orm_update": "./cache/test-cushy-orm-cache-orm-update",
-}
-enable_log()
-
-
-class User(BaseORMModel):
-
-    def __init__(self, name, age):
-        super().__init__()
-        self.name = name
-        self.age = age
-
-
-class TestORM(unittest.TestCase):
-
-    @classmethod
-    def tearDownClass(cls):
-        delete_cache()
-
-    def test_queryset_base(self):
-        user_list: List[User] = [User("jack", 18), User("jasmine", 18)]
-        queryset = QuerySet(user_list)
-
-        # assert all() and first()
-        self.assertEqual(len(queryset.all()), 2)
-        self.assertEqual(queryset.first().name, "jack")
-        self.assertEqual(queryset.first().age, 18)
-
-        # assert filter()
-        queried_user = queryset.filter(name="jack").first()
-        self.assertEqual(queried_user.name, "jack")
-        self.assertEqual(queried_user.age, 18)
-
-        # filter multiple result
-        queried_users = queryset.filter(age=18).all()
-        self.assertEqual(len(queried_users), 2)
-        self.assertEqual(queried_users[0].name, "jack")
-        self.assertEqual(queried_users[1].name, "jasmine")
-
-        # filter by multiple parameters
-        queried_user = queryset.filter(name="jack", age=18).first()
-        self.assertEqual(queried_user.name, "jack")
-        self.assertEqual(queried_user.age, 18)
-
-    def test_orm_add_and_query(self):
-        orm_cache = CushyOrmCache(cache_file['test_orm_add_and_query'])
-        user = User("jack", 18)
-        # assert add()
-        queryset = orm_cache.add(user)
-        self.assertEqual(len(queryset.all()), 1)
-
-        # assert query()
-        queryset_by_class = orm_cache.query(User)
-        self.assertEqual(queryset_by_class.first().name, "jack")
-        self.assertEqual(queryset_by_class.first().age, 18)
-
-        queryset_by_str = orm_cache.query("User")
-        self.assertEqual(queryset_by_str.first().name, "jack")
-        self.assertEqual(queryset_by_str.first().age, 18)
-
-        # add multiple users
-        user_list: List[User] = [
-            User("zeeland", 22),
-            User("hizeros", 20),
-            User("honey", 18),
-        ]
-        queryset = orm_cache.add(user_list)
-        self.assertEqual(len(queryset.all()), 4)
-        self.assertIsNotNone(queryset.filter(name="zeeland").first())
-
-    def test_orm_delete(self):
-        orm_cache = CushyOrmCache(cache_file['test_orm_delete'])
-
-        # add single user
-        user_a = User("user a", 20)
-        orm_cache.add(user_a)
-        user_b = User("user b", 30)
-        orm_cache.add(user_b)
-        user_c = User("user c", 40)
-        orm_cache.add(user_c)
-
-        self.assertEqual(len(orm_cache.query(User).all()), 3)
-        orm_cache.query(User).print_all()
-
-        # delete single user
-        orm_cache.delete(user_b)
-        orm_cache.query(User).print_all()
-        queryset = orm_cache.query(User)
-        self.assertEqual(len(queryset.all()), 2)
-        self.assertEqual(queryset.first().name, "user a")
-        self.assertEqual(queryset.first().age, 20)
-
-    def test_orm_update(self):
-        orm_cache = CushyOrmCache(cache_file['test_orm_update'])
-        user = User("old username", 18)
-        orm_cache.add(user)
-
-        # assert update
-        user.name = "new username"
-        orm_cache.update_obj(user)
-        queried_user = orm_cache.query(User).filter(name="new username").first()
-        self.assertIsNotNone(queried_user)
-        self.assertEqual(queried_user.name, "new username")
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import unittest
+from typing import List
+
+from cushy_storage.orm import QuerySet
+from cushy_storage import CushyOrmCache, BaseORMModel
+from cushy_storage.logger import enable_log
+from tests.utils import delete_cache
+
+cache_file = {
+    "test_orm_add_and_query": "./cache/test-cushy-orm-cache",
+    "test_orm_delete": "./cache/test-cushy-orm-cache-orm-delete",
+    "test_orm_update": "./cache/test-cushy-orm-cache-orm-update",
+}
+enable_log()
+
+
+class User(BaseORMModel):
+    def __init__(self, name, age):
+        super().__init__()
+        self.name = name
+        self.age = age
+
+
+class TestORM(unittest.TestCase):
+    @classmethod
+    def tearDownClass(cls):
+        delete_cache()
+
+    def test_queryset_base(self):
+        user_list: List[User] = [User("jack", 18), User("jasmine", 18)]
+        queryset = QuerySet(user_list)
+
+        # assert all() and first()
+        self.assertEqual(len(queryset.all()), 2)
+        self.assertEqual(queryset.first().name, "jack")
+        self.assertEqual(queryset.first().age, 18)
+
+        # assert filter()
+        queried_user = queryset.filter(name="jack").first()
+        self.assertEqual(queried_user.name, "jack")
+        self.assertEqual(queried_user.age, 18)
+
+        # filter multiple result
+        queried_users = queryset.filter(age=18).all()
+        self.assertEqual(len(queried_users), 2)
+        self.assertEqual(queried_users[0].name, "jack")
+        self.assertEqual(queried_users[1].name, "jasmine")
+
+        # filter by multiple parameters
+        queried_user = queryset.filter(name="jack", age=18).first()
+        self.assertEqual(queried_user.name, "jack")
+        self.assertEqual(queried_user.age, 18)
+
+    def test_orm_add_and_query(self):
+        orm_cache = CushyOrmCache(cache_file["test_orm_add_and_query"])
+        user = User("jack", 18)
+        # assert add()
+        queryset = orm_cache.add(user)
+        self.assertEqual(len(queryset.all()), 1)
+
+        # assert query()
+        queryset_by_class = orm_cache.query(User)
+        self.assertEqual(queryset_by_class.first().name, "jack")
+        self.assertEqual(queryset_by_class.first().age, 18)
+
+        queryset_by_str = orm_cache.query("User")
+        self.assertEqual(queryset_by_str.first().name, "jack")
+        self.assertEqual(queryset_by_str.first().age, 18)
+
+        # add multiple users
+        user_list: List[User] = [
+            User("zeeland", 22),
+            User("hizeros", 20),
+            User("honey", 18),
+        ]
+        queryset = orm_cache.add(user_list)
+        self.assertEqual(len(queryset.all()), 4)
+        self.assertIsNotNone(queryset.filter(name="zeeland").first())
+
+    def test_orm_delete(self):
+        orm_cache = CushyOrmCache(cache_file["test_orm_delete"])
+
+        # add single user
+        user_a = User("user a", 20)
+        orm_cache.add(user_a)
+        user_b = User("user b", 30)
+        orm_cache.add(user_b)
+        user_c = User("user c", 40)
+        orm_cache.add(user_c)
+
+        self.assertEqual(len(orm_cache.query(User).all()), 3)
+        orm_cache.query(User).print_all()
+
+        # delete single user
+        orm_cache.delete(user_b)
+        orm_cache.query(User).print_all()
+        queryset = orm_cache.query(User)
+        self.assertEqual(len(queryset.all()), 2)
+        self.assertEqual(queryset.first().name, "user a")
+        self.assertEqual(queryset.first().age, 20)
+
+    def test_orm_update(self):
+        orm_cache = CushyOrmCache(cache_file["test_orm_update"])
+        user = User("old username", 18)
+        orm_cache.add(user)
+
+        # assert update
+        user.name = "new username"
+        orm_cache.update_obj(user)
+        queried_user = orm_cache.query(User).filter(name="new username").first()
+        self.assertIsNotNone(queried_user)
+        self.assertEqual(queried_user.name, "new username")
```

