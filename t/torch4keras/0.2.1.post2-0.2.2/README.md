# Comparing `tmp/torch4keras-0.2.1.post2.tar.gz` & `tmp/torch4keras-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.2.1.post2.tar", last modified: Sun Mar 17 15:21:18 2024, max compression
+gzip compressed data, was "torch4keras-0.2.2.tar", last modified: Thu Apr 18 15:35:17 2024, max compression
```

## Comparing `torch4keras-0.2.1.post2.tar` & `torch4keras-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 15:21:18.007828 torch4keras-0.2.1.post2/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.2.1.post2/LICENSE
--rw-rw-rw-   0        0        0     5380 2024-03-17 15:21:18.007828 torch4keras-0.2.1.post2/PKG-INFO
--rw-rw-rw-   0        0        0     5120 2024-03-17 15:20:10.000000 torch4keras-0.2.1.post2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-17 15:21:18.007828 torch4keras-0.2.1.post2/setup.cfg
--rw-rw-rw-   0        0        0      548 2024-03-17 15:18:59.000000 torch4keras-0.2.1.post2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:21:17.988828 torch4keras-0.2.1.post2/test/
--rw-rw-rw-   0        0        0      448 2024-01-30 13:35:50.000000 torch4keras-0.2.1.post2/test/test_log.py
--rw-rw-rw-   0        0        0      884 2024-02-03 05:24:08.000000 torch4keras-0.2.1.post2/test/test_time.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:21:17.991836 torch4keras-0.2.1.post2/torch4keras/
--rw-rw-rw-   0        0        0      260 2024-02-26 13:11:12.000000 torch4keras-0.2.1.post2/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    64909 2024-03-15 13:31:06.000000 torch4keras-0.2.1.post2/torch4keras/callbacks.py
--rw-rw-rw-   0        0        0      431 2023-09-10 04:01:15.000000 torch4keras-0.2.1.post2/torch4keras/model.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:21:18.005843 torch4keras-0.2.1.post2/torch4keras/snippets/
--rw-rw-rw-   0        0        0      121 2024-01-16 12:50:44.000000 torch4keras-0.2.1.post2/torch4keras/snippets/__init__.py
--rw-rw-rw-   0        0        0     9571 2024-03-02 07:28:26.000000 torch4keras-0.2.1.post2/torch4keras/snippets/data_process.py
--rw-rw-rw-   0        0        0     1243 2024-01-16 12:50:44.000000 torch4keras-0.2.1.post2/torch4keras/snippets/import_utils.py
--rw-rw-rw-   0        0        0     9525 2024-02-26 13:11:12.000000 torch4keras-0.2.1.post2/torch4keras/snippets/log.py
--rw-rw-rw-   0        0        0     8146 2024-02-29 12:09:01.000000 torch4keras-0.2.1.post2/torch4keras/snippets/misc.py
--rw-rw-rw-   0        0        0    11251 2024-03-05 15:15:33.000000 torch4keras-0.2.1.post2/torch4keras/snippets/monitor.py
--rw-rw-rw-   0        0        0    44288 2024-03-17 03:40:12.000000 torch4keras-0.2.1.post2/torch4keras/trainer.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:21:17.997839 torch4keras-0.2.1.post2/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     5380 2024-03-17 15:21:17.000000 torch4keras-0.2.1.post2/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2024-03-17 15:21:17.000000 torch4keras-0.2.1.post2/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 15:21:17.000000 torch4keras-0.2.1.post2/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-17 15:21:17.000000 torch4keras-0.2.1.post2/torch4keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-17 15:21:17.000000 torch4keras-0.2.1.post2/torch4keras.egg-info/top_level.txt
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/
+-rw-rw-r--   0 lb        (1000) lb        (1000)    11357 2024-03-15 02:30:46.000000 torch4keras-0.2.2/LICENSE
+-rw-r--r--   0 lb        (1000) lb        (1000)     5376 2024-04-18 15:35:17.554753 torch4keras-0.2.2/PKG-INFO
+-rw-rw-r--   0 lb        (1000) lb        (1000)     5086 2024-04-18 15:28:12.000000 torch4keras-0.2.2/README.md
+-rw-rw-r--   0 lb        (1000) lb        (1000)       38 2024-04-18 15:35:17.554753 torch4keras-0.2.2/setup.cfg
+-rw-rw-r--   0 lb        (1000) lb        (1000)      524 2024-04-18 15:34:26.000000 torch4keras-0.2.2/setup.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/test/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      435 2024-03-15 02:30:46.000000 torch4keras-0.2.2/test/test_log.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      842 2024-03-15 02:30:46.000000 torch4keras-0.2.2/test/test_time.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      254 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    67636 2024-04-17 09:13:38.000000 torch4keras-0.2.2/torch4keras/callbacks.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      759 2024-04-17 10:19:39.000000 torch4keras-0.2.2/torch4keras/model.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras/snippets/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      117 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/snippets/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     9337 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/snippets/data_process.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1210 2024-03-15 02:30:46.000000 torch4keras-0.2.2/torch4keras/snippets/import_utils.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12359 2024-04-09 07:03:51.000000 torch4keras-0.2.2/torch4keras/snippets/log.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    13496 2024-04-17 09:15:00.000000 torch4keras-0.2.2/torch4keras/snippets/misc.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12175 2024-04-03 07:32:23.000000 torch4keras-0.2.2/torch4keras/snippets/monitor.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras/trainer/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      128 2024-04-09 02:47:12.000000 torch4keras-0.2.2/torch4keras/trainer/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1872 2024-04-09 02:36:34.000000 torch4keras-0.2.2/torch4keras/trainer/accelerate.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    35899 2024-04-17 10:27:39.000000 torch4keras-0.2.2/torch4keras/trainer/base.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2696 2024-04-09 02:37:24.000000 torch4keras-0.2.2/torch4keras/trainer/ddp.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12040 2024-04-17 10:52:28.000000 torch4keras-0.2.2/torch4keras/trainer/deepspeed.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      403 2024-04-09 02:39:36.000000 torch4keras-0.2.2/torch4keras/trainer/dp.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     3543 2024-04-09 02:39:24.000000 torch4keras-0.2.2/torch4keras/trainer/utils.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:35:17.554753 torch4keras-0.2.2/torch4keras.egg-info/
+-rw-r--r--   0 lb        (1000) lb        (1000)     5376 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/PKG-INFO
+-rw-rw-r--   0 lb        (1000) lb        (1000)      710 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/SOURCES.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)        1 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/dependency_links.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)       16 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/requires.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)       12 2024-04-18 15:35:17.000000 torch4keras-0.2.2/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.2.1.post2/LICENSE` & `torch4keras-0.2.2/LICENSE`

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

### Comparing `torch4keras-0.2.1.post2/PKG-INFO` & `torch4keras-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,91 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.2.1.post2
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![torch4keras](./docs/pics/torch4keras.png)
-
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-
-[Documentation](https://torch4keras.readthedocs.io) |
-[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
-[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-[Source code](https://github.com/Tongjilibo/torch4keras) |
-[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
-
-## 1. 下载安装
-安装稳定版
-```shell
-pip install torch4keras
-```
-安装最新版
-```shell
-pip install git+https://github.com/Tongjilibo/torch4keras.git
-```
-
-## 2. 功能
-- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-- 训练：
-
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
-
-    2022-10-28 23:17:37 - Finish Training
-    ```
-
-## 3. 快速上手
-- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-
-## 4. 版本历史
-|更新日期| 版本 | 版本说明 |
-|------| ----------------- |----------- |
-|20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
-|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
-|20240204|v0.1.9           | 增加Timeit, Timeit2, timeit等时间/速度监控|
-|20240116|v0.1.8           | 重新整理snippets, 重写save_pretrained|
-
-[更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
-
-## 5. 更新历史：
-
-[更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.2.2
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: torch>1.6
+
+![torch4keras](./docs/pics/torch4keras.png)
+
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+
+[Documentation](https://torch4keras.readthedocs.io) |
+[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
+[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+[Source code](https://github.com/Tongjilibo/torch4keras) |
+[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
+
+## 1. 下载安装
+安装稳定版
+```shell
+pip install torch4keras
+```
+安装最新版
+```shell
+pip install git+https://github.com/Tongjilibo/torch4keras.git
+```
+
+## 2. 功能
+- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+- 训练：
+
+    ```text
+    2022-10-28 23:16:10 - Start Training
+    2022-10-28 23:16:10 - Epoch: 1/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+    test_acc: 0.98045. best_test_acc: 0.98045
+
+    2022-10-28 23:16:27 - Epoch: 2/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+    test_acc: 0.98280. best_test_acc: 0.98280
+
+    2022-10-28 23:16:44 - Epoch: 3/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+    test_acc: 0.98365. best_test_acc: 0.98365
+
+    2022-10-28 23:17:03 - Epoch: 4/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+    test_acc: 0.98265. best_test_acc: 0.98365
+
+    2022-10-28 23:17:21 - Epoch: 5/5
+    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+    test_acc: 0.98585. best_test_acc: 0.98585
+
+    2022-10-28 23:17:37 - Finish Training
+    ```
+
+## 3. 快速上手
+- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+
+## 4. 版本历史
+|更新日期| 版本 | 版本说明 |
+|------| ----------------- |----------- |
+|20240418|v0.2.2|增加YamlConfig和IniConfig, 优化deepspeed的使用，修复`_prepare_inputs`的bug，修复断点续训`SmoothMetricsCallback`起点错误的bug, Trainer断点续训记录batch数|
+|20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
+|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
+
+[更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
+
+## 5. 更新历史：
+
+[更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
```

### Comparing `torch4keras-0.2.1.post2/README.md` & `torch4keras-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,79 @@
-![torch4keras](./docs/pics/torch4keras.png)
-
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-
-[Documentation](https://torch4keras.readthedocs.io) |
-[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
-[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-[Source code](https://github.com/Tongjilibo/torch4keras) |
-[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
-
-## 1. 下载安装
-安装稳定版
-```shell
-pip install torch4keras
-```
-安装最新版
-```shell
-pip install git+https://github.com/Tongjilibo/torch4keras.git
-```
-
-## 2. 功能
-- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-- 训练：
-
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
-
-    2022-10-28 23:17:37 - Finish Training
-    ```
-
-## 3. 快速上手
-- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-
-## 4. 版本历史
-|更新日期| 版本 | 版本说明 |
-|------| ----------------- |----------- |
-|20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
-|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
-|20240204|v0.1.9           | 增加Timeit, Timeit2, timeit等时间/速度监控|
-|20240116|v0.1.8           | 重新整理snippets, 重写save_pretrained|
-
-[更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
-
-## 5. 更新历史：
-
-[更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
+![torch4keras](./docs/pics/torch4keras.png)
+
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+
+[Documentation](https://torch4keras.readthedocs.io) |
+[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
+[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+[Source code](https://github.com/Tongjilibo/torch4keras) |
+[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
+
+## 1. 下载安装
+安装稳定版
+```shell
+pip install torch4keras
+```
+安装最新版
+```shell
+pip install git+https://github.com/Tongjilibo/torch4keras.git
+```
+
+## 2. 功能
+- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+- 训练：
+
+    ```text
+    2022-10-28 23:16:10 - Start Training
+    2022-10-28 23:16:10 - Epoch: 1/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+    test_acc: 0.98045. best_test_acc: 0.98045
+
+    2022-10-28 23:16:27 - Epoch: 2/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+    test_acc: 0.98280. best_test_acc: 0.98280
+
+    2022-10-28 23:16:44 - Epoch: 3/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+    test_acc: 0.98365. best_test_acc: 0.98365
+
+    2022-10-28 23:17:03 - Epoch: 4/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+    test_acc: 0.98265. best_test_acc: 0.98365
+
+    2022-10-28 23:17:21 - Epoch: 5/5
+    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+    test_acc: 0.98585. best_test_acc: 0.98585
+
+    2022-10-28 23:17:37 - Finish Training
+    ```
+
+## 3. 快速上手
+- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+
+## 4. 版本历史
+|更新日期| 版本 | 版本说明 |
+|------| ----------------- |----------- |
+|20240418|v0.2.2|增加YamlConfig和IniConfig, 优化deepspeed的使用，修复`_prepare_inputs`的bug，修复断点续训`SmoothMetricsCallback`起点错误的bug, Trainer断点续训记录batch数|
+|20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
+|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
+
+[更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
+
+## 5. 更新历史：
+
+[更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
```

### Comparing `torch4keras-0.2.1.post2/test/test_time.py` & `torch4keras-0.2.2/test/test_time.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from torch4keras.snippets import timeit, Timeit, Timeit2
-import time
-
-
-# 装饰器
-@timeit
-def func(n=10):
-    for _ in range(n):
-        time.sleep(0.1)
-func()
-
-# 上下文管理器 - 统计累计耗时
-with Timeit() as ti:
-    for i in range(10):
-        time.sleep(0.1)
-        ti.lap(name=i, reset=False)  # 统计累计耗时
-
-# 上下文管理器 - 统计每段速度
-with Timeit() as ti:
-    for i in range(10):
-        time.sleep(0.1)
-        ti.lap(count=10, name=i, reset=True)
-    ti(10) # 统计速度
-
-
-# 上下文管理器 - 统计速度
-with Timeit() as ti:
-    for i in range(10):
-        time.sleep(0.1)
-        ti.lap(name=i, reset=True)
-    ti(10) # 统计速度
-
-ti = Timeit2()
-for i in range(10):
-    time.sleep(0.1)
-    ti.lap(name=i)
-
-for i in range(10):
-    time.sleep(0.1)
-    ti.lap(name=i)
-ti.end() # 打印时长
-
+from torch4keras.snippets import timeit, Timeit, Timeit2
+import time
+
+
+# 装饰器
+@timeit
+def func(n=10):
+    for _ in range(n):
+        time.sleep(0.1)
+func()
+
+# 上下文管理器 - 统计累计耗时
+with Timeit() as ti:
+    for i in range(10):
+        time.sleep(0.1)
+        ti.lap(name=i, reset=False)  # 统计累计耗时
+
+# 上下文管理器 - 统计每段速度
+with Timeit() as ti:
+    for i in range(10):
+        time.sleep(0.1)
+        ti.lap(count=10, name=i, reset=True)
+    ti(10) # 统计速度
+
+
+# 上下文管理器 - 统计速度
+with Timeit() as ti:
+    for i in range(10):
+        time.sleep(0.1)
+        ti.lap(name=i, reset=True)
+    ti(10) # 统计速度
+
+ti = Timeit2()
+for i in range(10):
+    time.sleep(0.1)
+    ti.lap(name=i)
+
+for i in range(10):
+    time.sleep(0.1)
+    ti.lap(name=i)
+ti.end() # 打印时长
+
```

### Comparing `torch4keras-0.2.1.post2/torch4keras/snippets/data_process.py` & `torch4keras-0.2.2/torch4keras/snippets/data_process.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-import numpy as np
-import torch
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
-from packaging import version
-from torch.utils.data import Dataset, IterableDataset
-import inspect
-from .import_utils import is_safetensors_available, is_sklearn_available
-import os
-from torch import nn
-
-
-if is_safetensors_available():
-    from safetensors import safe_open
-    from safetensors.torch import load_file as safe_load_file
-    from safetensors.torch import save_file as safe_save_file
-
-if is_sklearn_available():
-    from sklearn.metrics import roc_auc_score
-else:
-    roc_auc_score = None
-
-
-def take_along_dim(input_tensor:torch.Tensor, indices:torch.Tensor, dim:int=None):
-    '''兼容部分低版本pytorch没有torch.take_along_dim
-    '''
-    if version.parse(torch.__version__) > version.parse('1.8.1'):
-        return torch.take_along_dim(input_tensor, indices, dim)
-    else:
-        # 该逻辑仅在少量数据上测试, 如有bug, 欢迎反馈
-        if dim is None:
-            res = input_tensor.flatten()[indices]
-        else:
-            res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
-            res = torch.from_numpy(res).to(input_tensor.device)
-        # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
-        return res
-
-
-def torch_div(input:torch.Tensor, other:torch.Tensor, rounding_mode:Optional[str] = None):
-    ''' torch.div兼容老版本
-    '''
-    if version.parse(torch.__version__) < version.parse('1.7.2'):
-        indices = input // other  # 兼容老版本
-    else:
-        indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
-    return indices
-
-
-def softmax(x:np.ndarray, axis:int=-1):
-    '''numpy版softmax
-    '''
-    x = x - x.max(axis=axis, keepdims=True)
-    x = np.exp(x)
-    return x / x.sum(axis=axis, keepdims=True)
-
-
-def search_layer(model:nn.Module, layer_name:str, retrun_first:bool=True):
-    '''根据layer_name搜索并返回参数/参数list
-    '''
-    return_list = []
-    for name, param in model.named_parameters():
-        if param.requires_grad and layer_name in name:
-            return_list.append(param)
-    if len(return_list) == 0:
-        return None
-    if retrun_first:
-        return return_list[0]
-    else:
-        return return_list
-
-
-class ListDataset(Dataset):
-    '''数据是List格式Dataset, 支持传入file_path或者外部已读入的data(List格式)
-
-    :param file_path: str, 待读取的文件的路径, 若无可以为None
-    :param data: List[Any], list格式的数据, 和file_path至少有一个不为None
-    '''
-    def __init__(self, file_path:Union[str, tuple, list]=None, data:Optional[list]=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.data = self.load_data(file_path)
-        elif isinstance(data, list):
-            self.data = data
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        return self.data[index]
-
-    @staticmethod
-    def load_data(file_path):
-        return file_path
-
-
-class IterDataset(IterableDataset):
-    '''流式读取文件, 用于大数据量、多小文件使用时候需要注意steps_per_epoch != None
-
-    :param file_path: str, 待读取的文件的路径, 若无可以为None
-    '''
-    def __init__(self, file_path:Union[str, tuple, list]=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.file_path = file_path
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-    
-    def __iter__(self):
-        return self.load_data(self.file_path)
-
-    @staticmethod
-    def load_data(file_path:Union[str,tuple,list], verbose=0):
-        if isinstance(file_path, (tuple, list)):
-            for file in file_path:
-                if verbose != 0:
-                    print("Load data: ", file)
-                with open(file, 'r') as file_obj:
-                    for line in file_obj:
-                        yield line
-        elif isinstance(file_path, str):
-            if verbose != 0:
-                print("Load data: ", file_path)
-            with open(file_path, 'r') as file_obj:
-                for line in file_obj:
-                    yield line
-
-
-def set_precision(num:float, dense_round:int=1):
-    '''设置数字的精度
-    '''
-    if np.isinf(num):
-        return num
-    if abs(num) >= 10:
-        return int(round(num))
-
-    precision = [1, 0.1, 0.01, 0.001, 0.0001, 0.00001, 0.000001]
-    for len_, prec in enumerate(precision):
-        if abs(num) >= prec:
-            return round(num, len_ + dense_round)
-    return num
-
-
-def metric_mapping(metric:str, func:Callable, y_pred:Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor]], 
-                   y_true:Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor]]):
-    '''metric的计算
-
-    :param metric: str, 自带metrics的名称
-    :param func: function, 透传的用户自定的计算指标的函数
-    :param y_pred: torch.Tensor, 样本的预测结果
-    :param y_true: torch.Tensor, 样本的真实结果
-    '''
-    # 自定义metrics
-    if inspect.isfunction(func):
-        metric_res = func(y_pred, y_true)
-        if inspect.isfunction(metric):
-            # 如果直接传入回调函数（无key）, 要求回调函数返回Dict[String: Int/Float]类型
-            assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
-        elif isinstance(metric, str):
-            # 如果直接传入回调函数（有key）, 要求回调函数返回Int/Float类型
-            assert isinstance(metric_res, (int, float)), 'Custom metrics callbacks should return `Int/Float value'
-        return metric_res
-    elif metric == 'loss':
-        pass
-    # 自带metrics
-    elif isinstance(metric, str):
-        # 如果forward返回了list, tuple, 则选取第一项
-        y_pred_tmp = y_pred[0] if isinstance(y_pred, (list, tuple)) else y_pred
-        y_true_tmp = y_true[0] if isinstance(y_true, (list, tuple)) else y_true
-        y_pred_tmp = y_pred_tmp.detach()  # 训练过程中评估, detach不进入计算图
-
-        # 根据shape做预处理
-        if len(y_pred_tmp.shape) == len(y_true_tmp.shape) + 1:
-            y_pred_tmp = torch.argmax(y_pred_tmp, dim=-1)
-        elif len(y_pred_tmp.shape) == len(y_true_tmp.shape):
-            pass
-        else:
-            raise ValueError(f'y_pred_tmp.shape={y_pred_tmp.shape} while y_true_tmp.shape={y_true_tmp.shape}')
-
-        # 执行内置的metric
-        if metric in {'accuracy', 'acc'}:
-            return torch.sum(y_pred_tmp.eq(y_true_tmp)).item() / y_true_tmp.numel()
-        elif metric in {'auc'}:
-            if roc_auc_score is None:
-                raise ImportError('roc_auc_score requires the `sklearn` library.')
-            return roc_auc_score(y_true.cpu().numpy(), y_pred_tmp.cpu().numpy())            
-        elif metric in {'mae', 'MAE', 'mean_absolute_error'}:
-            return torch.mean(torch.abs(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mse', 'MSE', 'mean_squared_error'}:
-            return torch.mean(torch.square(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mape', 'MAPE', 'mean_absolute_percentage_error'}:
-            diff = torch.abs((y_true_tmp - y_pred_tmp) / torch.clamp(torch.abs(y_true_tmp), 1e-7, None))
-            return 100. * torch.mean(diff).item()
-        elif metric in {'msle', 'MSLE', 'mean_squared_logarithmic_error'}:
-            first_log = torch.log(torch.clamp(y_pred_tmp, 1e-7, None) + 1.)
-            second_log = torch.log(torch.clamp(y_true_tmp, 1e-7, None) + 1.)
-            return torch.mean(torch.square(first_log - second_log)).item()
-
-    return None
-
-
-def load_checkpoint(checkpoint:str, load_safetensors:bool=False):
-    '''加载ckpt, 支持torch.load和safetensors
-    '''
-    if load_safetensors or checkpoint.endswith(".safetensors"):
-        # 加载safetensors格式
-        with safe_open(checkpoint, framework="pt") as f:
-            metadata = f.metadata()
-        if metadata.get("format") not in ["pt", "tf", "flax"]:
-            raise OSError(
-                f"The safetensors archive passed at {checkpoint} does not contain the valid metadata. Make sure "
-                "you save your model with the `save_pretrained` method."
-            )
-        elif metadata["format"] != "pt":
-            raise NotImplementedError(
-                f"Conversion from a {metadata['format']} safetensors archive to PyTorch is not implemented yet."
-            )
-        return safe_load_file(checkpoint)
-    else:
-        # 正常加载pytorch_model.bin
-        return torch.load(checkpoint, map_location='cpu')
-
-
-def save_checkpoint(state_dict:dict, save_path:str, save_safetensors:bool=False):
-    '''保存ckpt, 支持torch.save和safetensors
-    '''
-    save_dir = os.path.dirname(save_path)
-    if save_dir:
-        os.makedirs(save_dir, exist_ok=True)
-
-    if save_safetensors or save_path.endswith('.safetensors'):
-        safe_save_file(state_dict, save_path, metadata={"format": "pt"})
-    else:
+import numpy as np
+import torch
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from packaging import version
+from torch.utils.data import Dataset, IterableDataset
+import inspect
+from .import_utils import is_safetensors_available, is_sklearn_available
+import os
+from torch import nn
+
+
+if is_safetensors_available():
+    from safetensors import safe_open
+    from safetensors.torch import load_file as safe_load_file
+    from safetensors.torch import save_file as safe_save_file
+
+if is_sklearn_available():
+    from sklearn.metrics import roc_auc_score
+else:
+    roc_auc_score = None
+
+
+def take_along_dim(input_tensor:torch.Tensor, indices:torch.Tensor, dim:int=None):
+    '''兼容部分低版本pytorch没有torch.take_along_dim
+    '''
+    if version.parse(torch.__version__) > version.parse('1.8.1'):
+        return torch.take_along_dim(input_tensor, indices, dim)
+    else:
+        # 该逻辑仅在少量数据上测试, 如有bug, 欢迎反馈
+        if dim is None:
+            res = input_tensor.flatten()[indices]
+        else:
+            res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
+            res = torch.from_numpy(res).to(input_tensor.device)
+        # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
+        return res
+
+
+def torch_div(input:torch.Tensor, other:torch.Tensor, rounding_mode:Optional[str] = None):
+    ''' torch.div兼容老版本
+    '''
+    if version.parse(torch.__version__) < version.parse('1.7.2'):
+        indices = input // other  # 兼容老版本
+    else:
+        indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
+    return indices
+
+
+def softmax(x:np.ndarray, axis:int=-1):
+    '''numpy版softmax
+    '''
+    x = x - x.max(axis=axis, keepdims=True)
+    x = np.exp(x)
+    return x / x.sum(axis=axis, keepdims=True)
+
+
+def search_layer(model:nn.Module, layer_name:str, retrun_first:bool=True):
+    '''根据layer_name搜索并返回参数/参数list
+    '''
+    return_list = []
+    for name, param in model.named_parameters():
+        if param.requires_grad and layer_name in name:
+            return_list.append(param)
+    if len(return_list) == 0:
+        return None
+    if retrun_first:
+        return return_list[0]
+    else:
+        return return_list
+
+
+class ListDataset(Dataset):
+    '''数据是List格式Dataset, 支持传入file_path或者外部已读入的data(List格式)
+
+    :param file_path: str, 待读取的文件的路径, 若无可以为None
+    :param data: List[Any], list格式的数据, 和file_path至少有一个不为None
+    '''
+    def __init__(self, file_path:Union[str, tuple, list]=None, data:Optional[list]=None, **kwargs):
+        self.kwargs = kwargs
+        if isinstance(file_path, (str, tuple, list)):
+            self.data = self.load_data(file_path)
+        elif isinstance(data, list):
+            self.data = data
+        else:
+            raise ValueError('The input args shall be str format file_path / list format dataset')
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        return self.data[index]
+
+    @staticmethod
+    def load_data(file_path):
+        return file_path
+
+
+class IterDataset(IterableDataset):
+    '''流式读取文件, 用于大数据量、多小文件使用时候需要注意steps_per_epoch != None
+
+    :param file_path: str, 待读取的文件的路径, 若无可以为None
+    '''
+    def __init__(self, file_path:Union[str, tuple, list]=None, **kwargs):
+        self.kwargs = kwargs
+        if isinstance(file_path, (str, tuple, list)):
+            self.file_path = file_path
+        else:
+            raise ValueError('The input args shall be str format file_path / list format dataset')
+    
+    def __iter__(self):
+        return self.load_data(self.file_path)
+
+    @staticmethod
+    def load_data(file_path:Union[str,tuple,list], verbose=0):
+        if isinstance(file_path, (tuple, list)):
+            for file in file_path:
+                if verbose != 0:
+                    print("Load data: ", file)
+                with open(file, 'r') as file_obj:
+                    for line in file_obj:
+                        yield line
+        elif isinstance(file_path, str):
+            if verbose != 0:
+                print("Load data: ", file_path)
+            with open(file_path, 'r') as file_obj:
+                for line in file_obj:
+                    yield line
+
+
+def set_precision(num:float, dense_round:int=1):
+    '''设置数字的精度
+    '''
+    if np.isinf(num):
+        return num
+    if abs(num) >= 10:
+        return int(round(num))
+
+    precision = [1, 0.1, 0.01, 0.001, 0.0001, 0.00001, 0.000001]
+    for len_, prec in enumerate(precision):
+        if abs(num) >= prec:
+            return round(num, len_ + dense_round)
+    return num
+
+
+def metric_mapping(metric:str, func:Callable, y_pred:Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor]], 
+                   y_true:Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor]]):
+    '''metric的计算
+
+    :param metric: str, 自带metrics的名称
+    :param func: function, 透传的用户自定的计算指标的函数
+    :param y_pred: torch.Tensor, 样本的预测结果
+    :param y_true: torch.Tensor, 样本的真实结果
+    '''
+    # 自定义metrics
+    if inspect.isfunction(func):
+        metric_res = func(y_pred, y_true)
+        if inspect.isfunction(metric):
+            # 如果直接传入回调函数（无key）, 要求回调函数返回Dict[String: Int/Float]类型
+            assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
+        elif isinstance(metric, str):
+            # 如果直接传入回调函数（有key）, 要求回调函数返回Int/Float类型
+            assert isinstance(metric_res, (int, float)), 'Custom metrics callbacks should return `Int/Float value'
+        return metric_res
+    elif metric == 'loss':
+        pass
+    # 自带metrics
+    elif isinstance(metric, str):
+        # 如果forward返回了list, tuple, 则选取第一项
+        y_pred_tmp = y_pred[0] if isinstance(y_pred, (list, tuple)) else y_pred
+        y_true_tmp = y_true[0] if isinstance(y_true, (list, tuple)) else y_true
+        y_pred_tmp = y_pred_tmp.detach()  # 训练过程中评估, detach不进入计算图
+
+        # 根据shape做预处理
+        if len(y_pred_tmp.shape) == len(y_true_tmp.shape) + 1:
+            y_pred_tmp = torch.argmax(y_pred_tmp, dim=-1)
+        elif len(y_pred_tmp.shape) == len(y_true_tmp.shape):
+            pass
+        else:
+            raise ValueError(f'y_pred_tmp.shape={y_pred_tmp.shape} while y_true_tmp.shape={y_true_tmp.shape}')
+
+        # 执行内置的metric
+        if metric in {'accuracy', 'acc'}:
+            return torch.sum(y_pred_tmp.eq(y_true_tmp)).item() / y_true_tmp.numel()
+        elif metric in {'auc'}:
+            if roc_auc_score is None:
+                raise ImportError('roc_auc_score requires the `sklearn` library.')
+            return roc_auc_score(y_true.cpu().numpy(), y_pred_tmp.cpu().numpy())            
+        elif metric in {'mae', 'MAE', 'mean_absolute_error'}:
+            return torch.mean(torch.abs(y_pred_tmp - y_true_tmp)).item()
+        elif metric in {'mse', 'MSE', 'mean_squared_error'}:
+            return torch.mean(torch.square(y_pred_tmp - y_true_tmp)).item()
+        elif metric in {'mape', 'MAPE', 'mean_absolute_percentage_error'}:
+            diff = torch.abs((y_true_tmp - y_pred_tmp) / torch.clamp(torch.abs(y_true_tmp), 1e-7, None))
+            return 100. * torch.mean(diff).item()
+        elif metric in {'msle', 'MSLE', 'mean_squared_logarithmic_error'}:
+            first_log = torch.log(torch.clamp(y_pred_tmp, 1e-7, None) + 1.)
+            second_log = torch.log(torch.clamp(y_true_tmp, 1e-7, None) + 1.)
+            return torch.mean(torch.square(first_log - second_log)).item()
+
+    return None
+
+
+def load_checkpoint(checkpoint:str, load_safetensors:bool=False):
+    '''加载ckpt, 支持torch.load和safetensors
+    '''
+    if load_safetensors or checkpoint.endswith(".safetensors"):
+        # 加载safetensors格式
+        with safe_open(checkpoint, framework="pt") as f:
+            metadata = f.metadata()
+        if metadata.get("format") not in ["pt", "tf", "flax"]:
+            raise OSError(
+                f"The safetensors archive passed at {checkpoint} does not contain the valid metadata. Make sure "
+                "you save your model with the `save_pretrained` method."
+            )
+        elif metadata["format"] != "pt":
+            raise NotImplementedError(
+                f"Conversion from a {metadata['format']} safetensors archive to PyTorch is not implemented yet."
+            )
+        return safe_load_file(checkpoint)
+    else:
+        # 正常加载pytorch_model.bin
+        return torch.load(checkpoint, map_location='cpu')
+
+
+def save_checkpoint(state_dict:dict, save_path:str, save_safetensors:bool=False):
+    '''保存ckpt, 支持torch.save和safetensors
+    '''
+    save_dir = os.path.dirname(save_path)
+    if save_dir:
+        os.makedirs(save_dir, exist_ok=True)
+
+    if save_safetensors or save_path.endswith('.safetensors'):
+        safe_save_file(state_dict, save_path, metadata={"format": "pt"})
+    else:
         torch.save(state_dict, save_path)
```

### Comparing `torch4keras-0.2.1.post2/torch4keras/snippets/import_utils.py` & `torch4keras-0.2.2/torch4keras/snippets/import_utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import importlib.util
-from typing import Any, Tuple, Union
-from packaging import version
-import sys
-if sys.version_info < (3, 8):
-    import importlib_metadata
-else:
-    import importlib.metadata as importlib_metadata
-
-
-# TODO: This doesn't work for all packages (`bs4`, `faiss`, etc.) Talk to Sylvain to see how to do with it better.
-def is_package_available(pkg_name: str, return_version: bool = False) -> Union[Tuple[bool, str], bool]:
-    # Check we're not importing a "pkg_name" directory somewhere but the actual library by trying to grab the version
-    package_exists = importlib.util.find_spec(pkg_name) is not None
-    package_version = "N/A"
-    if package_exists:
-        try:
-            package_version = importlib.metadata.version(pkg_name)
-            package_exists = True
-        except importlib.metadata.PackageNotFoundError:
-            package_exists = False
-        # print(f"Detected {pkg_name} version {package_version}")
-    if return_version:
-        return package_exists, package_version
-    else:
-        return package_exists
-
-
-def is_safetensors_available():
-    return is_package_available("safetensors")
-
-
-def is_sklearn_available():
+import importlib.util
+from typing import Any, Tuple, Union
+from packaging import version
+import sys
+if sys.version_info < (3, 8):
+    import importlib_metadata
+else:
+    import importlib.metadata as importlib_metadata
+
+
+# TODO: This doesn't work for all packages (`bs4`, `faiss`, etc.) Talk to Sylvain to see how to do with it better.
+def is_package_available(pkg_name: str, return_version: bool = False) -> Union[Tuple[bool, str], bool]:
+    # Check we're not importing a "pkg_name" directory somewhere but the actual library by trying to grab the version
+    package_exists = importlib.util.find_spec(pkg_name) is not None
+    package_version = "N/A"
+    if package_exists:
+        try:
+            package_version = importlib.metadata.version(pkg_name)
+            package_exists = True
+        except importlib.metadata.PackageNotFoundError:
+            package_exists = False
+        # print(f"Detected {pkg_name} version {package_version}")
+    if return_version:
+        return package_exists, package_version
+    else:
+        return package_exists
+
+
+def is_safetensors_available():
+    return is_package_available("safetensors")
+
+
+def is_sklearn_available():
     return is_package_available("sklearn")
```

### Comparing `torch4keras-0.2.1.post2/torch4keras/snippets/monitor.py` & `torch4keras-0.2.2/torch4keras/snippets/monitor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,312 +1,341 @@
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
-import time
-import os
-import traceback
-import copy
-import functools
-from .log import log_info, log_warn, log_error
-from pprint import pprint
-
-
-def format_time(eta, hhmmss=True):
-    '''格式化显示时间
-    :param hhmmss: bool, 是否只以00:00:00格式显示
-    '''
-    if eta > 86400:
-        eta_d, eta_h = eta // 86400, eta % 86400
-        eta_format = '%dd ' % eta_d + ('%d:%02d:%02d' % (eta_h // 3600, (eta_h % 3600) // 60, eta_h % 60))
-    elif eta > 3600:
-        eta_format = ('%d:%02d:%02d' % (eta // 3600, (eta % 3600) // 60, eta % 60))
-    elif hhmmss:
-        eta_format = '%d:%02d' % (eta // 60, eta % 60)
-    elif (eta >= 1) and (eta < 60):
-        eta_format = '%.2fs' % eta
-    elif eta >= 1e-3:
-        eta_format = '%.0fms' % (eta * 1e3)
-    else:
-        eta_format = '%.0fus' % (eta * 1e6)
-    return eta_format
-
-
-def timeit(func):
-    '''装饰器, 计算函数消耗的时间
-    
-    Example
-    --------------------------------------
-    >>> @timeit
-    >>> def main(n=10):
-    >>>     for i in range(n):
-    >>>         time.sleep(0.01)
-
-    >>> main(10)
-    '''
-    def warpper(*args, **kwargs):
-        start = time.time()
-        res = func(*args, **kwargs)
-        end = time.time()
-        consume = format_time(end - start, hhmmss=False)
-        start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(start))
-        end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end))
-
-        log_info(f'Function `{func.__name__}` cost {consume} [{start1} < {end1}]')
-        return res
-    return warpper
-
-
-class Timeit:
-    '''上下文管理器, 记录耗时/平均耗时
-
-    Example
-    ----------------------
-    >>> from torch4keras.snippets import Timeit
-    >>> with Timeit() as ti:
-    >>>     for i in range(10):
-    >>>         time.sleep(0.1)
-    >>>         # ti.lap(name=i, restart=False)  # 统计累计耗时
-    >>>         # ti.lap(name=i, restart=True)  # 统计间隔耗时
-    >>>         # ti.lap(count=10, name=i, restart=True)  # 统计每段速度
-    >>>     # ti(10) # 统计速度
-    '''
-    def __enter__(self, template='Average speed: {:.2f}/s'):
-        self.count = None
-        self.start_tm = time.time()
-        self.template = template
-        return self
-
-    def __call__(self, count):
-        self.count = count
-
-    def reset(self):
-        '''自定义开始记录的地方'''
-        self.start_tm = time.time()
-    
-    def lap(self, name:str=None, count:int=None, reset=False):
-        '''
-        :params name: 打印时候自定义的前缀
-        :params count: 需要计算平均生成速度中统计的次数
-        :params reset: 是否重置start_tm, True只记录时间间隔, 否则记录的是从一开始的累计时间
-        '''
-        if count is not None:
-            self.count = count
-        name = '' if name is None else str(name).strip() + ' - '
-
-        end_tm = time.time()
-        consume = end_tm - self.start_tm
-        if self.count is None:
-            # 只log时间
-            consume = format_time(consume, hhmmss=False)
-            start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.start_tm))
-            end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end_tm))
-            log_info(name + f'Cost {consume} [{start1} < {end1}]')
-        elif consume > 0:
-            speed = self.count / consume
-            log_info(name + self.template.format(speed))
-        else:
-            pass
-            # log_warn('Time duration = 0')
-        
-        if reset:
-            self.reset()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.lap()
-        print()
-
-
-class Timeit2:
-    '''记录耗时
-
-    Example
-    ----------------------
-    >>> ti = Timeit2()
-    >>> for i in range(10):
-    >>>     time.sleep(0.1)
-    >>>     ti.lap(name=i)
-    >>> ti.end() # 打印各个步骤时长
-    '''
-    def __init__(self):
-        self.reset()
-
-    def __call__(self, *args, **kwargs):
-        self.lap(*args, **kwargs)
-
-    def reset(self):
-        '''自定义开始记录的地方'''
-        self.cost = dict()
-        self.count = dict()
-        self.start_tm = time.time()
-
-    def restart(self):
-        self.start_tm = time.time()
-
-    def lap(self, name:str):
-        '''
-        :params name: 打印时候自定义的前缀
-        '''
-        end_tm = time.time()
-        consume = end_tm - self.start_tm
-        name = str(name)
-        self.cost[name] = self.cost.get(name, 0) + consume
-        self.count[name] = self.count.get(name, 0) + 1
-        self.start_tm = time.time()
-
-    def end(self, verbose=1):
-        for k, v in self.count.items():
-            if v > 1:
-                self.cost['avg_' + k] = self.cost[k] / v
-        
-        if verbose > 0:
-            log_info('Cost detail')
-            pprint(self.cost)
-            print()
-
-        self.reset()
-        return self.cost
-
-
-def send_email(mail_receivers:Union[str,list], mail_subject:str, mail_msg:str="", mail_host:str=None, 
-               mail_user:str=None, mail_pwd:str=None, mail_sender:str=None):
-    ''' 发送邮件(默认使用笔者自己注册的邮箱, 若含敏感信息请使用自己注册的邮箱)
-
-    :param mail_subject: str, 邮件主题
-    :param mail_msg: str, 邮件正文
-    :param mail_receivers: str/list, 收件人邮箱
-    :param mail_host: str, 发件服务器host
-    :param mail_user: str, 发件人
-    :param mail_pwd: str, smtp的第三方密码
-    :param mail_sender: str, 发件人邮箱
-    '''
-    import smtplib
-    from email.mime.text import MIMEText
-
-    mail_host = mail_host or 'smtp.163.com'
-    mail_user = mail_user or 'bert4torch'
-    mail_pwd = mail_pwd or 'VDSGQEHFXDZOCVEH'
-    mail_sender = mail_sender or 'bert4torch@163.com'
-
-    #构造邮件内容
-    message = MIMEText(mail_msg,'plain','utf-8')
-    message['Subject'] = mail_subject
-    message['From'] = mail_sender
-    assert isinstance(mail_receivers, (str, tuple, list)), 'Arg `receivers` only receive `str, tuple, list` format'
-    message['To'] = mail_receivers if isinstance(mail_receivers, str) else ';'.join(mail_receivers)
-
-    #登录并发送邮件
-    try:
-        smtpObj = smtplib.SMTP() 
-        smtpObj.connect(mail_host, 25)  # 连接到服务器
-        smtpObj.login(mail_user, mail_pwd)  # 登录到服务器
-        smtpObj.sendmail(mail_sender, mail_receivers, message.as_string())  # 发送
-        smtpObj.quit()  # 退出
-        log_info('Send email success')
-    except smtplib.SMTPException as e:
-        log_error('Send email error : '+str(e))
-        return str(e)
-
-
-def email_when_error(receivers:Union[str,list], **configs):
-    '''装饰器, 异常则发邮件
-    Example:
-    --------
-    >>> @email_when_error(receivers='tongjilibo@163.com')
-    >>> def test():
-    >>>     return 1/0
-    >>> test()  # 调用
-    '''
-    def actual_decorator(func):
-        def new_func(*args, **kwargs):
-            try:
-                res = func(*args, **kwargs)
-            except Exception as e:
-                error_msg = traceback.format_exc()
-                send_email(receivers, func.__name__, error_msg, **configs)
-                raise e
-            return res
-        return new_func
-    return actual_decorator
-
-
-def watch_system_state(log_dir:str, gpu_id_list:List[int]=None, pids:Union[int,List[int]]=None, interval=1):
-    '''监控system的状态
-    
-    :param log_dir: str, tensorboard的地址
-    :param gpu_id_list: List[int], 监控的gpu
-    :param pids: int/List[int], 监控的进程号
-
-    Example:
-    --------
-    >>> watch_system_state(log_dir='./system_states')
-    '''
-    import psutil
-    import pynvml
-    from tensorboardX import SummaryWriter
-
-    pynvml.nvmlInit()
-    os.makedirs(log_dir, exist_ok=True)
-    tb_writer = SummaryWriter(log_dir=str(log_dir))  # prepare summary writer
-
-    pre_time_int = int(time.time())
-    pre_time = time.time()
-    pids = pids or os.getpid()
-    pids = [pids] if isinstance(pids, int) else pids
-    G = 1024*1024*1024
-
-    pre_read = {pid:psutil.Process(pid).io_counters().read_bytes for pid in pids}
-    pre_write = {pid:psutil.Process(pid).io_counters().write_bytes for pid in pids}
-    time_str_init = int(time.time())
-
-    log_info("Watching System Info")
-    while True:
-        time.sleep(interval)
-        now_time = time.time()
-        time_str = int(now_time) - time_str_init
-        for pid in pids:
-            p = psutil.Process(pid)
-
-            # CPU使用情况
-            tb_writer.add_scalar(f"Pid_{pid}/CPU Percent", p.cpu_percent(interval=0.5), time_str)
-
-            # 内存使用情况
-            tb_writer.add_scalar(f"Pid_{pid}/Memory Percent", p.memory_percent(), time_str)
-            tb_writer.add_scalar(f"Pid_{pid}/Memory RSS G_byte", p.memory_info().rss/G, time_str)
-            tb_writer.add_scalar(f"Pid_{pid}/Memory VMS G_byte", p.memory_info().vms/G, time_str)
-
-            # 进程IO信息
-            data = p.io_counters()
-            tb_writer.add_scalar(f"Pid_{pid}/IO read M_byte", data.read_bytes/1024, time_str)
-            tb_writer.add_scalar(f"Pid_{pid}/IO write M_byte", data.write_bytes/1024, time_str)
-            if (time_str - pre_time_int)%5 == 0:
-                tb_writer.add_scalar(f"Pid_{pid}/IO readRate M_byte_s", (data.read_bytes - pre_read[pid])/(now_time-pre_time)/1024, time_str)
-                tb_writer.add_scalar(f"Pid_{pid}/IO writeRate M_byte_s", (data.write_bytes - pre_write[pid])/(now_time-pre_time)/1024, time_str)
-                pre_read[pid] = data.read_bytes
-                pre_write[pid] = data.write_bytes
-            pre_time = now_time
-        
-        # gpu使用情况
-        tesorboard_info_list = []
-        if gpu_id_list is None:
-            deviceCount = pynvml.nvmlDeviceGetCount()
-            device_list = [i for i in range(deviceCount)]
-        else:
-            device_list = gpu_id_list
-
-        tesorboard_info_list = []
-        for i in device_list:
-            tesorboard_info = {}
-            handle = pynvml.nvmlDeviceGetHandleByIndex(i)
-            tesorboard_info['gpu_name'] = pynvml.nvmlDeviceGetName(handle)
-            meminfo = pynvml.nvmlDeviceGetMemoryInfo(handle)
-            tesorboard_info['gpu_mem_used'] = meminfo.used/G
-            UTIL = pynvml.nvmlDeviceGetUtilizationRates(handle)
-            tesorboard_info['gpu_gpu_util'] = UTIL.gpu
-            tesorboard_info['gpu_mem_util'] = UTIL.memory
-            tesorboard_info_list.append(copy.deepcopy(tesorboard_info))
-        for tesorboard_info,i in zip(tesorboard_info_list, device_list):
-            tb_writer.add_scalar(f'GPU/GPU{i} mem_used unit_G', tesorboard_info['gpu_mem_used'], time_str)
-            tb_writer.add_scalar(f'GPU/GPU{i} gpu_util', tesorboard_info['gpu_gpu_util'], time_str)
-            tb_writer.add_scalar(f'GPU/GPU{i} mem_util', tesorboard_info['gpu_mem_util'], time_str)
-
-    tb_writer.close()
-    pynvml.nvmlShutdown()
-
-    return
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+import time
+import os
+import traceback
+import copy
+import functools
+from .log import log_info, log_warn, log_error
+from pprint import pprint
+import datetime
+
+
+def format_timestamp(timestamp, format='%Y-%m-%d %H:%M:%S', verbose=0):
+    '''格式化显示时间戳'''
+    dt_object = datetime.datetime.fromtimestamp(timestamp)  
+    
+    # 格式化 datetime 对象  
+    formatted_time = dt_object.strftime(format)  
+    
+    if verbose > 0:
+        print(formatted_time)
+    return formatted_time
+
+
+def format_time(eta:Union[int, float], hhmmss=True):
+    '''格式化显示时间间隔
+    :param hhmmss: bool, 是否只以00:00:00格式显示
+    '''
+    # 以00:00:00格式显示
+    if hhmmss:
+        if eta > 86400:  # 1d 12:10:36
+            eta_d, eta_h = eta // 86400, eta % 86400
+            eta_format = '%dd ' % eta_d + ('%d:%02d:%02d' % (eta_h // 3600, (eta_h % 3600) // 60, eta_h % 60))
+        elif eta > 3600:  # 12:10:36
+            eta_format = ('%d:%02d:%02d' % (eta // 3600, (eta % 3600) // 60, eta % 60))
+        else:  # 10:36
+            eta_format = '%d:%02d' % (eta // 60, eta % 60)
+
+    else:
+        if eta > 86400:  # 1d 12h 10m 36s
+            eta_d, eta_h = eta // 86400, eta % 86400
+            eta_format = '%dd %dh %dm %ds' % (eta_d, eta_h // 3600, (eta_h % 3600) // 60, eta_h % 60)
+        elif eta > 3600:  # 12h 10m 36s
+            eta_format = ('%dh %dm %ds' % (eta // 3600, (eta % 3600) // 60, eta % 60))
+        elif eta > 60:  # 10m 36s
+            eta_format = ('%dm %ds' % (eta // 60, eta % 60))
+        elif (eta >= 1) and (eta <= 60):  # 36.02s
+            eta_format = '%.2fs' % eta
+        elif eta >= 1e-3:  # 25ms
+            eta_format = '%.0fms' % (eta * 1e3)
+        else:  # 250us
+            eta_format = '%.0fus' % (eta * 1e6)
+    return eta_format
+
+
+def timeit(func):
+    '''装饰器, 计算函数消耗的时间
+    
+    Example
+    --------------------------------------
+    >>> @timeit
+    >>> def main(n=10):
+    >>>     for i in range(n):
+    >>>         time.sleep(0.01)
+
+    >>> main(10)
+    '''
+    def warpper(*args, **kwargs):
+        start = time.time()
+        res = func(*args, **kwargs)
+        end = time.time()
+        consume = format_time(end - start, hhmmss=False)
+        start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(start))
+        end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end))
+
+        log_info(f'Function `{func.__name__}` cost {consume} [{start1} < {end1}]')
+        return res
+    return warpper
+
+
+class Timeit:
+    '''上下文管理器, 记录耗时/平均耗时
+
+    Example
+    ----------------------
+    >>> from torch4keras.snippets import Timeit
+    >>> with Timeit() as ti:
+    >>>     for i in range(10):
+    >>>         time.sleep(0.1)
+    >>>         # ti.lap(name=i, reset=False)  # 统计累计耗时
+    >>>         # ti.lap(name=i, reset=True)  # 统计间隔耗时
+    >>>         # ti.lap(count=10, name=i, restart=True)  # 统计每段速度
+    >>>     # ti(10) # 统计速度
+    '''
+    def __enter__(self, template='Average speed: {:.2f}/s'):
+        self.count = None
+        self.start_tm = time.time()
+        self.template = template
+        return self
+
+    def __call__(self, count):
+        self.count = count
+
+    def reset(self):
+        '''自定义开始记录的地方'''
+        self.start_tm = time.time()
+    
+    def lap(self, name:str=None, count:int=None, reset=False):
+        '''
+        :params name: 打印时候自定义的前缀
+        :params count: 需要计算平均生成速度中统计的次数
+        :params reset: 是否重置start_tm, True只记录时间间隔, 否则记录的是从一开始的累计时间
+        '''
+        if count is not None:
+            self.count = count
+        name = '' if name is None else str(name).strip() + ' - '
+
+        end_tm = time.time()
+        consume = end_tm - self.start_tm
+        if self.count is None:
+            # 只log时间
+            consume = format_time(consume, hhmmss=False)
+            start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.start_tm))
+            end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end_tm))
+            log_info(name + f'Cost {consume} [{start1} < {end1}]')
+        elif consume > 0:
+            speed = self.count / consume
+            log_info(name + self.template.format(speed))
+        else:
+            pass
+            # log_warn('Time duration = 0')
+        
+        if reset:
+            self.reset()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.lap()
+        print()
+
+
+class Timeit2:
+    '''记录耗时
+
+    Example
+    ----------------------
+    >>> ti = Timeit2()
+    >>> for i in range(10):
+    >>>     time.sleep(0.1)
+    >>>     ti.lap(name=i)
+    >>> ti.end() # 打印各个步骤时长
+    '''
+    def __init__(self):
+        self.reset()
+
+    def __call__(self, *args, **kwargs):
+        self.lap(*args, **kwargs)
+
+    def reset(self):
+        '''自定义开始记录的地方'''
+        self.cost = dict()
+        self.count = dict()
+        self.start_tm = time.time()
+
+    def restart(self):
+        self.start_tm = time.time()
+
+    def lap(self, name:str, verbose=0):
+        '''
+        :params name: 打印时候自定义的前缀
+        '''
+        end_tm = time.time()
+        consume = end_tm - self.start_tm
+        name = str(name)
+        self.cost[name] = self.cost.get(name, 0) + consume
+        self.count[name] = self.count.get(name, 0) + 1
+        self.start_tm = time.time()
+        
+        if verbose > 1:
+            start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.start_tm))
+            end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end_tm))
+            log_info(name + f'Cost {consume} [{start1} < {end1}]')
+
+    def end(self, verbose=1):
+        for k, v in self.count.items():
+            if v > 1:
+                self.cost['avg_' + k] = self.cost[k] / v
+        
+        if verbose > 0:
+            log_info('Cost detail')
+            pprint(self.cost)
+            print()
+
+        self.reset()
+        return self.cost
+
+
+def send_email(mail_receivers:Union[str,list], mail_subject:str, mail_msg:str="", mail_host:str=None, 
+               mail_user:str=None, mail_pwd:str=None, mail_sender:str=None):
+    ''' 发送邮件(默认使用笔者自己注册的邮箱, 若含敏感信息请使用自己注册的邮箱)
+
+    :param mail_subject: str, 邮件主题
+    :param mail_msg: str, 邮件正文
+    :param mail_receivers: str/list, 收件人邮箱
+    :param mail_host: str, 发件服务器host
+    :param mail_user: str, 发件人
+    :param mail_pwd: str, smtp的第三方密码
+    :param mail_sender: str, 发件人邮箱
+    '''
+    import smtplib
+    from email.mime.text import MIMEText
+
+    mail_host = mail_host or 'smtp.163.com'
+    mail_user = mail_user or 'bert4torch'
+    mail_pwd = mail_pwd or 'VDSGQEHFXDZOCVEH'
+    mail_sender = mail_sender or 'bert4torch@163.com'
+
+    #构造邮件内容
+    message = MIMEText(mail_msg,'plain','utf-8')
+    message['Subject'] = mail_subject
+    message['From'] = mail_sender
+    assert isinstance(mail_receivers, (str, tuple, list)), 'Arg `receivers` only receive `str, tuple, list` format'
+    message['To'] = mail_receivers if isinstance(mail_receivers, str) else ';'.join(mail_receivers)
+
+    #登录并发送邮件
+    try:
+        smtpObj = smtplib.SMTP() 
+        smtpObj.connect(mail_host, 25)  # 连接到服务器
+        smtpObj.login(mail_user, mail_pwd)  # 登录到服务器
+        smtpObj.sendmail(mail_sender, mail_receivers, message.as_string())  # 发送
+        smtpObj.quit()  # 退出
+        log_info('Send email success')
+    except smtplib.SMTPException as e:
+        log_error('Send email error : '+str(e))
+        return str(e)
+
+
+def email_when_error(receivers:Union[str,list], **configs):
+    '''装饰器, 异常则发邮件
+    Example:
+    --------
+    >>> @email_when_error(receivers='tongjilibo@163.com')
+    >>> def test():
+    >>>     return 1/0
+    >>> test()  # 调用
+    '''
+    def actual_decorator(func):
+        def new_func(*args, **kwargs):
+            try:
+                res = func(*args, **kwargs)
+            except Exception as e:
+                error_msg = traceback.format_exc()
+                send_email(receivers, func.__name__, error_msg, **configs)
+                raise e
+            return res
+        return new_func
+    return actual_decorator
+
+
+def watch_system_state(log_dir:str, gpu_id_list:List[int]=None, pids:Union[int,List[int]]=None, interval=1):
+    '''监控system的状态
+    
+    :param log_dir: str, tensorboard的地址
+    :param gpu_id_list: List[int], 监控的gpu
+    :param pids: int/List[int], 监控的进程号
+
+    Example:
+    --------
+    >>> watch_system_state(log_dir='./system_states')
+    '''
+    import psutil
+    import pynvml
+    from tensorboardX import SummaryWriter
+
+    pynvml.nvmlInit()
+    os.makedirs(log_dir, exist_ok=True)
+    tb_writer = SummaryWriter(log_dir=str(log_dir))  # prepare summary writer
+
+    pre_time_int = int(time.time())
+    pre_time = time.time()
+    pids = pids or os.getpid()
+    pids = [pids] if isinstance(pids, int) else pids
+    G = 1024*1024*1024
+
+    pre_read = {pid:psutil.Process(pid).io_counters().read_bytes for pid in pids}
+    pre_write = {pid:psutil.Process(pid).io_counters().write_bytes for pid in pids}
+    time_str_init = int(time.time())
+
+    log_info("Watching System Info")
+    while True:
+        time.sleep(interval)
+        now_time = time.time()
+        time_str = int(now_time) - time_str_init
+        for pid in pids:
+            p = psutil.Process(pid)
+
+            # CPU使用情况
+            tb_writer.add_scalar(f"Pid_{pid}/CPU Percent", p.cpu_percent(interval=0.5), time_str)
+
+            # 内存使用情况
+            tb_writer.add_scalar(f"Pid_{pid}/Memory Percent", p.memory_percent(), time_str)
+            tb_writer.add_scalar(f"Pid_{pid}/Memory RSS G_byte", p.memory_info().rss/G, time_str)
+            tb_writer.add_scalar(f"Pid_{pid}/Memory VMS G_byte", p.memory_info().vms/G, time_str)
+
+            # 进程IO信息
+            data = p.io_counters()
+            tb_writer.add_scalar(f"Pid_{pid}/IO read M_byte", data.read_bytes/1024, time_str)
+            tb_writer.add_scalar(f"Pid_{pid}/IO write M_byte", data.write_bytes/1024, time_str)
+            if (time_str - pre_time_int)%5 == 0:
+                tb_writer.add_scalar(f"Pid_{pid}/IO readRate M_byte_s", (data.read_bytes - pre_read[pid])/(now_time-pre_time)/1024, time_str)
+                tb_writer.add_scalar(f"Pid_{pid}/IO writeRate M_byte_s", (data.write_bytes - pre_write[pid])/(now_time-pre_time)/1024, time_str)
+                pre_read[pid] = data.read_bytes
+                pre_write[pid] = data.write_bytes
+            pre_time = now_time
+        
+        # gpu使用情况
+        tesorboard_info_list = []
+        if gpu_id_list is None:
+            deviceCount = pynvml.nvmlDeviceGetCount()
+            device_list = [i for i in range(deviceCount)]
+        else:
+            device_list = gpu_id_list
+
+        tesorboard_info_list = []
+        for i in device_list:
+            tesorboard_info = {}
+            handle = pynvml.nvmlDeviceGetHandleByIndex(i)
+            tesorboard_info['gpu_name'] = pynvml.nvmlDeviceGetName(handle)
+            meminfo = pynvml.nvmlDeviceGetMemoryInfo(handle)
+            tesorboard_info['gpu_mem_used'] = meminfo.used/G
+            UTIL = pynvml.nvmlDeviceGetUtilizationRates(handle)
+            tesorboard_info['gpu_gpu_util'] = UTIL.gpu
+            tesorboard_info['gpu_mem_util'] = UTIL.memory
+            tesorboard_info_list.append(copy.deepcopy(tesorboard_info))
+        for tesorboard_info,i in zip(tesorboard_info_list, device_list):
+            tb_writer.add_scalar(f'GPU/GPU{i} mem_used unit_G', tesorboard_info['gpu_mem_used'], time_str)
+            tb_writer.add_scalar(f'GPU/GPU{i} gpu_util', tesorboard_info['gpu_gpu_util'], time_str)
+            tb_writer.add_scalar(f'GPU/GPU{i} mem_util', tesorboard_info['gpu_mem_util'], time_str)
+
+    tb_writer.close()
+    pynvml.nvmlShutdown()
+
+    return
```

### Comparing `torch4keras-0.2.1.post2/torch4keras/trainer.py` & `torch4keras-0.2.2/torch4keras/trainer/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,905 +1,713 @@
-from torch import nn
-import torch
-from torch.optim import Optimizer
-from torch.optim.lr_scheduler import LambdaLR
-from torch.utils.data import DataLoader
-from torch4keras.snippets import DottableDict, metric_mapping, get_parameter_device, log_info, log_warn, log_error, seed_everything
-from torch4keras.snippets import print_trainable_parameters, colorful, send_email, load_checkpoint, save_checkpoint
-from torch4keras.callbacks import KerasProgbar, SmoothMetricsCallback, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, History
-from collections import OrderedDict
-from typing import Union, List, Literal, Tuple, Set, Callable, Optional
-from inspect import isfunction
-import os
-import json
-import math
-import re
-import traceback
-
-
-class Trainer:
-    '''Trainer, 传入Module实例
-
-    :param module: None/nn.Module, nn.Module()的模型实例
-    '''
-    def __init__(self, module:nn.Module=None):
-        super(Trainer, self).__init__()
-        self.initialize(module)
-    
-    def initialize(self, module:nn.Module=None):
-        # 传入Module实例方式
-        if module is not None:
-            assert isinstance(module, nn.Module), 'Args `module` only support nn.Module format'
-            self.module = module
-
-        self.global_step, self.local_step, self.total_steps, self.batch_step = 0, 0, 0, 0
-        self.epoch, self.steps_per_epoch, self.train_dataloader = 0, None, None
-        self.resume_step, self.resume_epoch = 0, 0
-        self.retain_graph = False  # loss.backward()是否保留计算图
-        self.move_to_model_device = True  # 自动把tensor转到model所在的device
-        self.log_first_step = False  # 是否打印第一个step的数据
-        self.criterion = None  # criterion
-        self.optimizer = None  # optimizer
-        self.scheduler = None  # scheduler
-        self.callbacks = []  # 所有的Callbacks, 如果fit中不传入, 则默认为[progbarlogger, smoothmetrics, history]三项
-        self.run_callbacks = True  # 是否运行Callbacks, 目前主要是在DDP模式下运用
-        self.loss2metrics = True  # 把loss_detail打印在进度条的metrics上
-        # add_module(self)  # 增加nn.Module的成员方法
-
-    def compile(self, loss:Optional[Union[Callable, nn.Module]]=None, optimizer:Optimizer=None, scheduler:LambdaLR=None, clip_grad_norm:float=None, 
-                mixed_precision:Literal[True, False, 'fp16', 'bf16']=False, metrics:Union[str, dict, Callable, List[Union[str, dict, Callable]]]=None, 
-                grad_accumulation_steps:int=1, progbar_type:Literal['keras', 'tqdm', 'progressbar2']='keras', progbar_width:int=None,
-                stateful_metrics:Union[str, Set[str], Tuple[str], List[str]]=None, smooth_interval:int=100, **kwargs):
-        '''complile: 定义loss, optimizer, metrics等参数
-        
-        :param loss: loss
-        :param optimizer: 优化器
-        :param scheduler: lr_scheduler
-        :param clip_grad_norm: float, 是否使用梯度裁剪, 默认为False
-        :param mixed_precision: bool, 是否使用混合精度, 默认为False
-        :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric, 形式为{key: func}
-        :param grad_accumulation_steps: int, 梯度累积步数, 默认为1
-        :param bar: str, 使用进度条的种类, 从kwargs中解析, 默认为keras, 可选keras, tqdm, progressbar2
-
-        > 进度条的配置
-            progbar_type: str, 默认为keras, 可选keras, tqdm, progressbar2
-            width: int, keras进度条下表示进度条的长度
-        > 指标平滑的配置, 默认为None表示采取默认平滑设置; 传入False表示不使用平滑
-            stateful_metrics: List[str], 表示不使用指标平滑仅进行状态记录的metric, 指标抖动会更加明显, 默认为None表示使用指标平滑
-            smooth_interval: int, 表示指标平滑时候的累计步数, 默认为100
-
-        :return: None
-        '''
-        self.criterion = loss or self.criterion  # loss
-        self.optimizer = optimizer or self.optimizer  # 优化器
-        self.scheduler = scheduler or self.scheduler  # lr_scheduler
-        self.clip_grad_norm = clip_grad_norm  # 梯度裁剪
-        self.grad_accumulation_steps = grad_accumulation_steps  # 梯度累积
-
-        # 混合精度
-        assert mixed_precision in {True, False, 'fp16', 'bf16'}
-        self.mixed_precision_mode = 'fp16' if mixed_precision is True else mixed_precision
-        if self.mixed_precision_mode:
-            self.autocast = torch.cuda.amp.autocast
-            self.scaler = torch.cuda.amp.GradScaler()
-
-        # 训练过程观测的指标
-        self.metrics = OrderedDict({'loss': None})
-        if metrics is None:
-            metrics = []
-        elif isinstance(metrics, (str, dict)) or isfunction(metrics):
-            metrics = [metrics]
-        for metric in metrics:
-            # 字符类型, 目前仅支持accuracy
-            if isinstance(metric, str) and metric != 'loss':
-                self.metrics[metric] = None
-            # 字典形式 {metric: func}
-            elif isinstance(metric, dict):
-                self.metrics.update(metric)
-            # 函数形式, key和value都赋值metric
-            elif isfunction(metric):
-                self.metrics.update({metric: metric})
-            else:
-                raise TypeError('Args metrics only support `String, Dict, Callable, List[String, Dict, Callable]` format')
-
-        # 进度条参数
-        assert progbar_type in {'keras', 'tqdm', 'progressbar2'}
-        self.progbar_config = {'bar': progbar_type, 'width': progbar_width}
-        self.progbar_config = {k:v for k,v in self.progbar_config.items() if v is not None}
-
-        # smooth_metrics参数: 默认平滑
-        self.smooth_metrics_config = {'stateful_metrics': stateful_metrics, 'interval': smooth_interval, 'verbose': kwargs.get('verbose')}
-        self.smooth_metrics_config = {k:v for k,v in self.smooth_metrics_config.items() if v is not None}
-
-        # 其他参数设置
-        for key, value in kwargs.items():
-            if hasattr(self, key):
-                setattr(self, key, value)
-
-    def print_trainable_parameters(self):
-        '''打印可训练的参数量'''
-        print_trainable_parameters(self.unwrap_model())
-
-    @property
-    def device(self) -> torch.device:
-        '''获取model所在的device'''
-        if hasattr(self, '_device'):
-            return self._device
-        return get_parameter_device(self.unwrap_model())
-
-    @device.setter
-    def device(self, value):
-        '''允许修改self.device'''
-        self._device = value
-
-    def _move_to_model_device(self, inputs:Union[torch.Tensor, tuple, list, dict]):
-        '''遍历并转移到model.device上（递归）'''
-        if self.move_to_model_device:
-            if isinstance(inputs, torch.Tensor) and hasattr(self, 'device') and (inputs.device != self.device):
-                inputs = inputs.to(self.device)
-            elif isinstance(inputs, (tuple, list)):
-                inputs = list(inputs) if isinstance(inputs, tuple) else inputs
-                for i, ts in enumerate(inputs):
-                    inputs[i] = self._move_to_model_device(ts)
-            elif isinstance(inputs, dict):
-                for k, v in inputs.items():
-                    inputs[k] = self._move_to_model_device(v)
-        return inputs
-
-    def _log_first_step(self, resume_step, train_X, train_y):
-        '''打印第一个step的数据'''
-        if self.log_first_step and self.verbose and (self.global_step == resume_step):
-            print(colorful('[Train_data]: ', color='green'), + train_X)
-            print(colorful('[Label]: ', color='green'), + train_y)
-
-    def _forward(self, *inputs, **input_kwargs):
-        '''调用模型的forward, 方便下游继承的时候可以自定义使用哪个模型的forward
-        '''
-        return self._argparse_forward(self.unwrap_model(), *inputs, **input_kwargs)
-
-    def _argparse_forward(self, model, *inputs, **input_kwargs):
-        '''调用模型的forward
-        如果传入了网络结构module, 则调用module的forward; 如果是继承方式, 则调用自身的forward
-        这里声明为staticmethod的话, 使用add_trainer会有问题
-        '''
-        if (len(inputs)==1) and isinstance(inputs[0], (tuple,list)):  # 防止([])嵌套
-            inputs = inputs[0]
-        
-        if isinstance(inputs, torch.Tensor):  # tensor不展开
-            return model.forward(inputs, **input_kwargs)
-        elif isinstance(inputs, (tuple, list)):
-            return model.forward(*inputs, **input_kwargs)
-        else:
-            return model.forward(inputs, **input_kwargs)
-
-    def train_step(self, train_X, train_y):
-        ''' Perform a training step on a batch of inputs. '''
-        # 计算loss
-        if self.mixed_precision_mode:
-            with self.autocast(dtype=torch.float16 if self.mixed_precision_mode=='fp16' else torch.bfloat16):
-                output = self._forward(train_X)
-                loss_detail = self.criterion(output, train_y)
-        else:
-            output = self._forward(train_X)
-            loss_detail = self.criterion(output, train_y)
-
-        # 整理loss
-        if isinstance(loss_detail, torch.Tensor):
-            loss = loss_detail
-            loss_detail = {}
-        elif isinstance(loss_detail, dict):
-            loss = loss_detail['loss']  # 还存在其他loss, 仅用于打印
-            del loss_detail['loss']
-        elif isinstance(loss_detail, (tuple, list)):
-            loss = loss_detail[0]
-            loss_detail = {f'loss{i}':v for i, v in enumerate(loss_detail[1:], start=1)}
-        else:
-            raise ValueError('Return loss only support `Tensor/dict/tuple/list` format')
-
-        # 梯度累积
-        loss = loss / self.grad_accumulation_steps if self.grad_accumulation_steps > 1 else loss
-
-        # loss backward
-        loss = self.loss_backward(loss)
-        loss_detail = {k: (v.item() if isinstance(v, torch.Tensor) else v) / self.grad_accumulation_steps for k, v in loss_detail.items()}
-        return output, loss, loss_detail
-
-    def loss_backward(self, loss):
-        '''loss.backward'''
-        self.scale_before_step = 0
-        if self.mixed_precision_mode:  # 混合精度
-            self.scale_before_step = self.scaler.get_scale()
-            self.scaler.scale(loss).backward(retain_graph=self.retain_graph)
-        else:
-            loss.backward(retain_graph=self.retain_graph)
-        return loss
-    
-    def step(self):
-        '''参数更新'''
-        skip_scheduler = False
-        # 混合精度
-        if self.mixed_precision_mode:
-            self.scaler.unscale_(self.optimizer)
-            if self.clip_grad_norm is not None:  # 梯度裁剪
-                torch.nn.utils.clip_grad_norm_(self.unwrap_model().parameters(), self.clip_grad_norm)
-            self.scaler.step(self.optimizer)
-            self.scaler.update()
-            skip_scheduler = self.scaler.get_scale() != self.scale_before_step
-        else:
-            if self.clip_grad_norm is not None:  # 梯度裁剪
-                torch.nn.utils.clip_grad_norm_(self.unwrap_model().parameters(), self.clip_grad_norm)
-            self.optimizer.step()
-
-        self.optimizer.zero_grad()  # 清梯度
-        if (self.scheduler is not None) and not skip_scheduler:
-            if isinstance(self.scheduler, (tuple, list)):
-                for scheduler in self.scheduler:
-                    scheduler.step()
-            else:
-                self.scheduler.step()
-
-    def _prepare_inputs(self, train_dataloader:DataLoader, steps_per_epoch:Union[int,None], epochs:int, verbose:int):
-        '''对fit的输入进行类型检查并置为成员变量'''
-        if not hasattr(train_dataloader, '__len__'):
-            assert steps_per_epoch is not None, 'Either train_dataloader has attr `__len__` or steps_per_epoch is not None'
-        if steps_per_epoch is None:
-            self.steps_per_epoch = math.ceil(len(train_dataloader) // self.grad_accumulation_steps)
-        else:
-            self.steps_per_epoch = steps_per_epoch
-        self.batch_size = train_dataloader.batch_size
-        self.epochs = epochs
-        self.total_steps = self.steps_per_epoch * epochs
-        self.train_dataloader = train_dataloader  # 设置为成员变量, 可由外部的callbacks进行修改
-        self.train_dataloader_iter = iter(self.train_dataloader)  # 循环epoch时不重生成
-        self.verbose = self.verbose if hasattr(self, 'verbose') else verbose
-
-    def _prepare_callbacks(self, callbacks:Union[Callback, List[Callback]]=None):
-        '''callbacks设置'''
-        if callbacks is None:
-            callbacks = []
-        elif isinstance(callbacks, Callback):
-            callbacks = [callbacks]
-        for callback in callbacks:
-            assert isinstance(callback, Callback), f"Args `callbacks` only support Callback(), but got {type(callback)}"
-
-        history = History()
-        callbacks_ = []
-
-        # 指标平滑
-        if any([isinstance(i, SmoothMetricsCallback) for i in callbacks]):
-            # 用户自定的callbacks中包含了SmoothMetricsCallback
-            log_warn(f'SmoothMetricsCallback already in use and args `smooth_metrics_config` will be ignored')
-            smooth_callback = [callback for callback in callbacks if isinstance(callback, SmoothMetricsCallback)][0]
-            callbacks_.append(smooth_callback)
-            callbacks = [callback for callback in callbacks if not isinstance(callback, SmoothMetricsCallback)]
-        elif self.smooth_metrics_config.get('interval') is not None:
-            smooth_callback = SmoothMetricsCallback(**self.smooth_metrics_config)
-            callbacks_.append(smooth_callback)
-        else:
-            # 不平滑
-            smooth_callback = None
-
-        # 检查指标平滑的设置和后续callback的设置的interval是不是一致
-        for callback in callbacks:
-            if hasattr(callback, 'interval') and (smooth_callback is not None) and (callback != smooth_callback) and \
-                (callback.interval is not None) and (callback.interval % smooth_callback.interval != 0):
-                log_warn(f'{type(callback).__name__}.interval={callback.interval} while SmoothMetricsCallback.interval={smooth_callback.interval}')
-        
-        # 进度条
-        progbarlogger = None
-        if self.verbose:
-            if self.progbar_config['bar'] == 'keras':
-                progbarlogger = KerasProgbar(**self.progbar_config)
-            elif self.progbar_config['bar'] == 'tqdm':
-                progbarlogger = TqdmProgbar(**self.progbar_config)
-            elif self.progbar_config['bar'] == 'progressbar2':
-                progbarlogger = ProgressBar2Progbar(**self.progbar_config)
-            else:
-                progbarlogger = KerasProgbar(**self.progbar_config)
-            callbacks_.append(progbarlogger)
-
-        callbacks_  += callbacks + [history]
-        self.callbacks = CallbackList(callbacks_, run_callbacks=self.run_callbacks)
-        callback_trainer = self
-        callback_model = self.unwrap_model()
-        params = {
-            'epochs': self.epochs,
-            'steps': self.steps_per_epoch,
-            'verbose': self.verbose,
-            'metrics': [i for i in self.metrics.keys() if isinstance(i, str)],
-        }
-        self.callbacks.set_all(trainer=callback_trainer, model=callback_model, optimizer=self.optimizer, scheduler=self.scheduler, params=params)
-        callback_trainer.stop_training = False  # 在EarlyStopping中会重新设置
-        return history, callback_trainer, progbarlogger
-
-    def _prepare_nextbatch(self):
-        '''准备下一个batch数据'''
-        # 循环dataloader, 不要试用itertools的cycle, 遇到过变量不释放的问题
-        try:
-            batch = next(self.train_dataloader_iter)
-            self.batch_step += 1
-        except StopIteration:
-            self.callbacks.on_dataloader_end()  # 适用于数据量较大时, 动态读取文件并重新生成self.train_dataloader的情况, 如预训练
-            # DDP训练时候为了避免每个epoch样本一致, 修改随机种子
-            if isinstance(self.train_dataloader.sampler, torch.utils.data.distributed.DistributedSampler) and \
-                hasattr(self.train_dataloader.sampler, 'set_epoch'):
-                self.train_dataloader.sampler.set_epoch(self.epoch)
-            self.train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候, 其实顺序也重新生成了
-            self.batch_step = 0
-            batch = next(self.train_dataloader_iter)
-
-        batch = self._move_to_model_device(batch)
-        return batch
-
-    def fit(self, train_dataloader:DataLoader, steps_per_epoch:int=None, epochs:int=1, 
-            callbacks:Union[Callback, List[Callback]]=None, verbose:int=1, **kwargs):
-        ''' 模型训练
-        :param train_dataloader: Dataloader, 训练数据集
-        :param steps_per_epoch: int, 每个epoch训练的steps, 默认为None表示自行计算 
-        :param epochs: int, 训练的轮次, 默认为1
-        :param callbacks: Callback/List[Callback], 回调函数, 可调用预制的Callback或者自定义, 默认为None 
-        :param verbose: int, 是否打印, 默认为1表示打印
-        
-        > 其他参数
-        :param mail_receivers_when_error: str, 训练异常时候邮件通知
-        :param save_ckpt_dir_when_error: str, 训练异常时候保存权重的路径
-        :param save_batch_path_when_error: bool, 训练异常时候保存当前batch, 方便debug
-
-        :return: History
-        '''
-        try:
-            return self._fit(train_dataloader, steps_per_epoch, epochs, callbacks, verbose, **kwargs)
-        except Exception as e:
-            # 训练异常则发邮件
-            error_msg = traceback.format_exc()
-            mail_receivers_ = kwargs.get('mail_receivers_when_error')
-            if mail_receivers_ is not None:
-                mail_subject_ = kwargs.get('mail_subject_when_error') or "[ERROR] fit"
-                mail_host_ = kwargs.get('mail_host_when_error')
-                mail_user_ = kwargs.get('mail_user_when_error')
-                mail_pwd_ = kwargs.get('mail_pwd_when_error')
-                mail_sender_ = kwargs.get('mail_sender_when_error')
-                send_email(mail_receivers_, mail_subject_, error_msg, mail_host=mail_host_, 
-                           mail_user=mail_user_, mail_pwd=mail_pwd_, mail_sender=mail_sender_)
-
-            # 训练异常则保存权重
-            if (save_ckpt_dir_when_error := kwargs.get('save_ckpt_dir_when_error')) is not None:
-                self.save_to_checkpoint(save_ckpt_dir_when_error, verbose=verbose, **kwargs)
-
-            # 训练异常则打印当前batch
-            if (save_batch_path_when_error := kwargs.get('save_batch_path_when_error')) is not None:
-                os.makedirs(os.path.dirname(save_batch_path_when_error), exist_ok=True)
-                torch.save({'train_X': self.train_X.cpu(), 'train_y': self.train_y.cpu()}, save_batch_path_when_error)
-            
-            raise e
-
-    def _fit(self, train_dataloader:DataLoader, steps_per_epoch:int=None, epochs:int=1, 
-             callbacks:Union[Callback, List[Callback]]=None, verbose:int=1, **kwargs):
-        '''模型训练'''
-        # 输入处理
-        self._prepare_inputs(train_dataloader, steps_per_epoch, epochs, verbose)
-
-        # 准备callbacks
-        history, callback_trainer, progbarlogger  = self._prepare_callbacks(callbacks)
-
-        #       epoch: 当前epoch
-        # global_step: 当前全局训练步数
-        #  local_step: 当前epoch内的训练步数, 不同epoch中相同local_step对应的batch数据不一定相同, 在steps_per_epoch=None时相同
-        #  batch_step: 在dataloader中的index, 不同epoch中相同的bti对应的batch数据一般相同, 除非重新生成dataloader
-        self.callbacks.on_train_begin()
-        logs = self._log_init()  # 防止数据集为空时候
-        for epoch in range(self.resume_epoch, epochs):
-            self.epoch = epoch
-            # resume_step：判断local_step的起点, 以及进度条的起始位置
-            resume_step = self.resume_step if epoch==self.resume_epoch else 0
-            self.callbacks.on_epoch_begin(self.global_step, self.epoch)
-            if self.verbose:
-                progbarlogger.seen = resume_step  # 这里设置进度条的seen, 在callbacks中也会修改
-            
-            for local_step in range(resume_step, self.steps_per_epoch):
-                self.local_step = local_step
-                self.global_step = self.epoch * self.steps_per_epoch + self.local_step
-                logs = self._log_init()
-                self.callbacks.on_batch_begin(self.global_step, self.local_step, logs)
-
-                # forward和backward
-                if not self.unwrap_model().training:
-                    self.unwrap_model().train()  # 设置为train模式
-                tr_loss, tr_loss_detail = 0, {}
-                for _ in range(self.grad_accumulation_steps):
-                    self.train_X, self.train_y = self._prepare_nextbatch()  # 获取下一个batch的训练数据
-                    self._log_first_step(resume_step, self.train_X, self.train_y)  # log第一个step
-                    output, loss, loss_detail = self.train_step(self.train_X, self.train_y)
-                    self.callbacks.on_train_step_end()
-                    tr_loss += loss.item()
-                    for k, v in loss_detail.items():
-                        tr_loss_detail[k] = tr_loss_detail.get(k, 0) + v
-                # TODO: 理论上梯度累积时需对output和train_y进行合并, 主要是为了metric_mapping计算的准确
-                
-                # 参数更新
-                self.step()
-
-                # 添加loss至log打印
-                logs.update(dict({'loss': tr_loss}, **tr_loss_detail))
-                if self.verbose and self.loss2metrics and (self.global_step == resume_step):
-                    # 把loss_detail添加到进度条metrics中
-                    progbarlogger.add_metrics(list(tr_loss_detail.keys()), add_position=1)
-                    
-                # 添加metrics至log打印
-                for metric, func in self.metrics.items():
-                    perf = metric_mapping(metric, func, output, self.train_y)  # 内置的一些accuracy指标
-                    if perf is not None:
-                        if isfunction(metric):  # 直接传入回调函数(无key)
-                            if self.verbose and (self.global_step == resume_step):
-                                progbarlogger.add_metrics(list(perf.keys()))
-                            logs.update(perf)
-                        elif isinstance(metric, str):  # 直接传入回调函数(有key)
-                            logs[metric] = perf
-
-                self.callbacks.on_batch_end(self.global_step, self.local_step, logs)
-
-            self.callbacks.on_epoch_end(self.global_step, self.epoch, logs)
-            # TerminateOnNaN、EarlyStopping等停止训练策略
-            if callback_trainer.stop_training:
-                break
-        self.callbacks.on_train_end(logs)
-        return history
-
-    def _log_init(self):
-        '''获取batch_size, 主要是用于callback中的BaseLogger和Callback
-        '''
-        logs = {}
-
-        # 添加lr
-        try:
-            logs['lr'] = self.optimizer.param_groups[0]["lr"]
-        except:
-            pass
-        return logs
-
-    @torch.no_grad()
-    def predict(self, *inputs, **input_kwargs):
-        '''模型预测, 调用forward()'''
-        self.unwrap_model().eval()
-        inputs = self._move_to_model_device(inputs)
-        input_kwargs = self._move_to_model_device(input_kwargs)
-        return self._forward(*inputs, **input_kwargs)
-        
-    def load_steps_params(self, save_path:str):
-        '''导入训练过程参数
-        
-        :param save_path: str, 训练过程参数保存路径
-        '''
-        step_params = torch.load(save_path)
-        self.resume_step = step_params['resume_step'] 
-        self.resume_epoch = step_params['resume_epoch']
-        return step_params
-
-    def save_steps_params(self, save_path:str):
-        '''保存训练过程参数
-
-        :param save_path: str, 训练过程参数保存路径
-        '''
-        step_params = {'resume_step': (self.local_step+1) % self.steps_per_epoch, 
-                       'resume_epoch': self.epoch + (self.local_step+1) // self.steps_per_epoch}
-        save_dir = os.path.dirname(save_path)
-        os.makedirs(save_dir, exist_ok=True)
-        torch.save(step_params, save_path)
-
-    def load_weights(self, load_path:Union[str,tuple,list], strict:bool=True, mapping:Union[dict,Callable]=None):
-        '''加载模型权重, 支持加载权重文件list
-
-        :param save_path: str/tuple/list, 权重加载路径
-        :param strict: bool, torch.load()是否严格加载
-        :param mapping: dict/func, 指定key的映射
-            1. mapping=None, 表示按照模型自身结构加载, 一般加载finetune后使用save_weights()保存出来的权重
-            2. mapping自定义, 根据用户自定义mapping来加载权重
-        '''
-        if isinstance(load_path, (tuple, list)):
-            strict = False  # 加载多个权重文件时候, strict设置为False
-        elif isinstance(load_path, str):
-            load_path = [load_path]
-        else:
-            raise ValueError('Args `load_path` only support str/tuple/list format')
-        
-        mapping = mapping or dict()
-        for load_path_i in load_path:
-            state_dict = load_checkpoint(load_path_i)
-            for k in list(state_dict.keys()):
-                if isinstance(mapping, dict) and k in mapping:
-                    state_dict[mapping[k]] = state_dict.pop(k)
-                elif isinstance(mapping, Callable):
-                    state_dict[mapping(k)] = state_dict.pop(k)
-            self.unwrap_model().load_state_dict(state_dict, strict=strict)
-
-    def save_weights(self, save_path:str, mapping:Union[dict,Callable]=None, trainable_only:bool=False):
-        '''保存模型权重
-
-        :param save_path: str, 权重保存路径
-        :param mapping: dict/func, 指定key的映射
-            1. mapping=None, 表示按照模型自身结构的key来保存, 后续可直接load_weights()加载
-            2. mapping自定义, 根据用户自定义mapping来保存权重
-        :param trainable_only: bool, 指定仅保存可训练参数
-        '''
-        state_dict = self.unwrap_model().state_dict()
-        trainable_parameters = set(p for p,v in self.unwrap_model().named_parameters() if v.requires_grad)
-        
-        mapping = mapping or dict()
-        for k in list(state_dict.keys()):
-            # 只保存可训练的模型部分
-            if trainable_only and (k not in trainable_parameters):
-                continue
-            if isinstance(mapping, dict) and k in mapping:
-                state_dict[mapping[k]] = state_dict.pop(k)
-            elif isinstance(mapping, Callable):
-                state_dict[mapping(k)] = state_dict.pop(k)        
-        save_checkpoint(state_dict, save_path)
-        if trainable_only:
-            params_all = sum(p.numel() for p in self.unwrap_model().parameters())
-            params_trainable = sum(p.numel() for p in self.unwrap_model().parameters() if p.requires_grad)
-            ratio = params_trainable/params_all*100
-            log_info(f"Only trainable parameters saved and occupy {params_trainable}/{params_all}={ratio:.2f}%")
-
-    def save_pretrained(self, save_path:str, weight_map:dict=None, mapping:Union[dict,Callable]=None):
-        '''按照预训练模型的key来保存模型, 可供transformers包加载
-
-        :param save_path: str, 保存的文件/文件夹路径
-        '''
-        state_dict = dict()
-        for name, child in self.unwrap_model().named_children():
-            if (name != '') and hasattr(child, 'save_pretrained'):
-                tmp = child.save_pretrained(save_path, weight_map, mapping, write_to_disk=False)
-                state_dict.update(tmp if tmp else {})
-            else:
-                state_dict.update({f'{name}.{k}': v for k,v in child.state_dict().items()})
-        if len(state_dict) > 0:
-            save_dir = None if re.search('\.[a-zA-z0-9]+$', save_path) else save_path
-            save_checkpoint(state_dict, os.path.join(save_dir, 'pytorch_model.bin') if save_dir else save_path)
-    
-    def resume_from_checkpoint(self, save_dir:str=None, model_path:str=None, optimizer_path:str=None, scheduler_path:str=None, 
-                               steps_params_path:str=None, mapping:Union[dict,Callable]=None, verbose:int=0, strict:bool=True, 
-                               device=None, **kwargs):
-        '''同时加载模型、优化器、训练过程参数
-
-        :param save_dir: str, 保存目录
-        :param model_path: str, 模型文件路径
-        :param optimizer_path: str, 优化器文件路径
-        :param scheduler_path: str, scheduler文件路径
-        :param steps_params_path: str, 训练过程参数保存路径
-        :param mapping: dict, 模型文件的mapping
-        '''
-        # 加载模型权重
-        if model_path or save_dir:
-            model_path = model_path or os.path.join(save_dir, 'model.pt')
-            self.load_weights(model_path, strict=strict, mapping=mapping)
-            if verbose == 1:
-                log_info(f'Model weights successfuly resumed from {model_path}')
-
-        # 加载优化器
-        if optimizer_path or save_dir:
-            optimizer_path = optimizer_path or os.path.join(save_dir, 'optimizer.pt')
-            state_dict = torch.load(optimizer_path, map_location = device or self.device)
-            self.optimizer.load_state_dict(state_dict)
-            if verbose == 1:
-                log_info(f'Optimizer successfuly resumed from {optimizer_path}')
-
-        # 加载scheduler
-        if (scheduler_path or save_dir) and (self.scheduler is not None):
-            scheduler_path = scheduler_path or os.path.join(save_dir, 'scheduler.pt')
-            state_dict = torch.load(scheduler_path, map_location = device or self.device)
-            self.scheduler.load_state_dict(state_dict)
-            if verbose == 1:
-                log_info(f'Scheduler successfuly resumed from {scheduler_path}')
-
-        # 加载训练进度参数
-        if steps_params_path or save_dir:
-            steps_params_path = steps_params_path or os.path.join(save_dir, 'steps_params.pt')
-            self.load_steps_params(steps_params_path)
-            if verbose == 1:
-                log_info(f'Steps_params successfuly resumed from {steps_params_path}')
-
-    def save_to_checkpoint(self, save_dir:str=None, model_path:str=None, optimizer_path:str=None, scheduler_path:str=None, 
-                           steps_params_path:str=None, mapping:Union[dict,Callable]=None, trainable_only:bool=False, 
-                           verbose:int=0, **kwargs):
-        '''同时保存模型、优化器、训练过程参数、scheduler
-
-        :param save_dir: str, 保存目录
-        :param model_path: str, 模型文件路径
-        :param optimizer_path: str, 优化器文件路径
-        :param scheduler_path: str, scheduler文件路径
-        :param steps_params_path: str, 训练过程参数保存路径
-        :param mapping: dict/func, 模型文件的mapping
-        :param trainable_only
-        '''
-        if model_path or save_dir:
-            model_path = model_path or os.path.join(save_dir, 'model.pt')
-            self.save_weights(model_path, mapping=mapping, trainable_only=trainable_only)
-            if verbose == 1:
-                log_info(f'Model weights successfuly saved to {model_path}')
-
-        if optimizer_path or save_dir:
-            optimizer_path = optimizer_path or os.path.join(save_dir, 'optimizer.pt')
-            os.makedirs(os.path.dirname(optimizer_path), exist_ok=True)
-            torch.save(self.optimizer.state_dict(), optimizer_path)
-            if verbose == 1:
-                log_info(f'Optimizer successfuly saved to {optimizer_path}')
-
-        if (scheduler_path or save_dir) and (self.scheduler is not None):
-            scheduler_path = scheduler_path or os.path.join(save_dir, 'scheduler.pt')
-            os.makedirs(os.path.dirname(scheduler_path), exist_ok=True)
-            torch.save(self.scheduler.state_dict(), scheduler_path)
-            if verbose == 1:
-                log_info(f'Scheduler successfuly saved to {scheduler_path}')
-
-        if steps_params_path or save_dir:
-            steps_params_path = steps_params_path or os.path.join(save_dir, 'steps_params.pt')
-            self.save_steps_params(steps_params_path)
-            if verbose == 1:
-                log_info(f'Steps_params successfuly saved to {steps_params_path}')
-
-    def unwrap_model(self):
-        '''返回nn.Module模块
-        '''
-        if isinstance(self, nn.Module): return self
-        return self.module if hasattr(self, 'module') else self
-
-
-Trainer.compile_training_components = Trainer.compile
-
-
-class TrainerDP(nn.DataParallel, Trainer):
-    '''DataParallel模式使用多gpu的方法, 
-    1) 父类顺序颠倒也会出问题
-    2) 使用方式和nn.DataParallel一致, TrainerDP(net, *args, **kwargs)来使用
-    '''
-    def __init__(self, *args, **kwargs):
-        Trainer.__init__(self)
-        nn.DataParallel.__init__(self, *args, **kwargs)
-
-
-class TrainerDDP(nn.parallel.DistributedDataParallel, Trainer):
-    '''DistributedDataParallel模式使用多gpu的方法,
-    1) 父类顺序颠倒也会出问题
-    2) 使用方式和DistributedDataParallel一致, TrainerDDP(net, *args, **kwargs)来使用
-    '''
-    def __init__(self, *args, master_rank=0, **kwargs):
-        Trainer.__init__(self)
-        nn.parallel.DistributedDataParallel.__init__(self, *args, **kwargs)
-
-        # 默认仅对master_rank=0打印信息
-        assert isinstance(master_rank, (int, list, tuple)), 'Args `master_rank` only supoorts int, list, tuple'
-        if isinstance(master_rank, int):
-            master_rank = [master_rank]
-        self.master_rank = master_rank
-        self.verbose = (torch.distributed.get_rank() in master_rank)
-    
-    def _prepare_inputs(self, *args):
-        super()._prepare_inputs(*args)
-        from torch.utils.data.distributed import DistributedSampler 
-        if (self.train_dataloader.sampler is None) and (not isinstance(self.train_dataloader.sampler, DistributedSampler)):
-            self.train_dataloader.sampler = DistributedSampler(self.train_dataloader.dataset)
-            self.train_dataloader_iter = iter(self.train_dataloader)
-    
-    def disable_run_callbacks(self, callbacks: Union[Callback, List[Callback]]):
-        for callback in callbacks:
-            if torch.distributed.get_rank() not in self.master_rank:
-                callback.run_callback = False
-
-    @classmethod
-    def init_process_group(master_rank=0, seed=42):
-        if os.name == 'nt':
-            # windows: Diff between backends: https://pytorch.org/docs/stable/distributed.html
-            torch.distributed.init_process_group(backend="gloo")
-        else:  # linux
-            torch.distributed.init_process_group(backend='nccl')
-        
-        ddp = DottableDict()
-        ddp.rank = int(os.environ["RANK"])
-        ddp.local_rank = int(os.getenv('LOCAL_RANK'))
-        ddp.device = torch.device('cuda', ddp.local_rank)
-        ddp.world_size = int(os.environ["WORLD_SIZE"])
-        ddp.master_process = ddp.rank == master_rank
-        torch.cuda.set_device(ddp.local_rank)
-        seed_everything(seed + ddp.rank)
-        return ddp
-
-
-class AccelerateTrainer(Trainer):
-    '''accelerate来训练'''
-    def __init__(self, module: nn.Module, **configs):
-        super().__init__(module)
-        from accelerate import Accelerator
-        accelerator = Accelerator(**configs)
-        self.model = accelerator.prepare(module)
-        self.accelerator = accelerator
-        self.device = accelerator.device
-        self.verbose = 1 if accelerator.is_local_main_process else 0
-        log_warn('AcclerateTrainer may not be compatible with several callbacks, you may use custom callbacks instead.')
-    
-    def compile(self, *args, **kwargs):
-        super().compile(*args, **kwargs)
-        self.optimizer, self.scheduler, self.criterion = self.accelerator.prepare(self.optimizer, self.scheduler, self.criterion)
-
-    def _prepare_inputs(self, *args):
-        super()._prepare_inputs(*args)
-        self.train_dataloader = self.accelerator.prepare(self.train_dataloader)
-        self.train_dataloader_iter = iter(self.train_dataloader)
-
-    def prepare(self, *args, **kwargs):
-        '''调用acclerate的prepare, 如在外面评估时候需要对dev_dataloader使用'''
-        return self.accelerator.prepare(*args, **kwargs)
-
-    def unwrap_model(self):
-        '''返回nn.Module模块'''
-        unwrap_model = self.accelerator.unwrap_model(self.model)
-        if isinstance(unwrap_model, nn.Module): return unwrap_model
-        return unwrap_model.module if hasattr(unwrap_model, 'module') else unwrap_model
-
-    def loss_backward(self, loss):
-        self.accelerator.backward(loss)
-        return loss
-
-
-class DeepSpeedTrainer(Trainer):
-    '''deepspeed来训练'''
-    def __init__(self, module, config_path):
-        super().__init__(module)
-        self.model = module
-        self.config = DottableDict(json.load(open(config_path)))
-        self.config['steps_per_print'] = self.config.get('steps_per_print', 1e9)  # 默认不打印, 防止进度条打印问题
-
-    def compile(self, *args, log_level='warning', inference=False, master_rank=0, **kwargs):
-        super().compile(*args, **kwargs)
-        import deepspeed
-        from deepspeed.utils import logger as ds_logger
-        import logging
-        log_levels = {
-            "debug": logging.DEBUG,
-            "info": logging.INFO,
-            "warning": logging.WARNING,
-            "error": logging.ERROR,
-            "critical": logging.CRITICAL,
-        }
-
-        ds_logger.setLevel(log_levels.get(log_level, logging.WARNING))
-
-        if inference:
-            # only Z3 makes sense for the inference
-            log_warn("ZeRO inference only makes sense with ZeRO Stage 3")
-            self.optimizer, self.scheduler = None, None
-            model_parameters = None
-        else:
-            model_parameters = list(filter(lambda p: p.requires_grad, self.model.parameters()))
-        
-        kwargs = {
-            "model": self.model,  # deepspeed的forward默认是计算到loss输出的
-            "model_parameters": model_parameters,
-            "config_params": self.config,
-            "optimizer": self.optimizer,
-            "lr_scheduler": self.scheduler,
-        }
-        if self.config.get('zero_optimization', {}).get('offload_optimizer', {}).get('device') == 'cpu':
-            kwargs.pop('optimizer')
-            if self.optimizer is not None:
-                self.optimizer = None
-                log_warn('You may not use custom optimizer when offload_optimizer=`cpu`')
-        self.deepspeed_engine, self.optimizer, _, self.scheduler = deepspeed.initialize(**kwargs)
-        self.verbose = 1 if self.deepspeed_engine.local_rank == master_rank else 0
-
-    def unwrap_model(self):
-        # 执行deepspeed_engine的forward
-        return self.deepspeed_engine
-
-    def loss_backward(self, loss):
-        self.deepspeed_engine.backward(loss)
-        return loss
-    
-    def step(self):
-        self.deepspeed_engine.step()
-
-    def resume_from_checkpoint(self, *args, **kwargs):
-        return self.deepspeed_engine.load_checkpoint(*args, **kwargs)
-
-    def save_to_checkpoint(self, *args, **kwargs):
-        return self.deepspeed_engine.save_checkpoint(*args, **kwargs)
-
-
-def add_trainer(obj, include=None, exclude=None, verbose=0, replace_func=False):
-    '''为nn.Module添加Triner对应的方法'''
-    if isinstance(obj, (Trainer, TrainerDP, TrainerDDP)):
-        log_warn('obj is not a Trainer object')
-        return obj
-    elif not isinstance(obj, nn.Module):
-        log_warn('obj is not a nn.Module object')
-        return obj
-
-    if include is None:
-        include = set()
-    elif isinstance(include, str):
-        include = set([include])
-    elif isinstance(include, (tuple, list)):
-        include = set(include)
-    else:
-        raise TypeError(f'Arg `include` only receive str/list format, not {type(include)}')
-
-    if exclude is None:
-        exclude = set()
-    elif isinstance(exclude, (tuple, list)):
-        exclude = set(exclude)
-
-    import types
-    added_funcs = []
-    for k in dir(Trainer):
-        set_func = False
-        if k in include:  # 必须包含的
-            set_func = True
-        elif k in exclude:  # 必须屏蔽的
-            pass
-        elif k.startswith('__') and k.endswith('__'):  # 内部函数不执行
-            pass
-        elif hasattr(obj, k):  # 如果下游重新定义, 则不继
-            if replace_func:
-                set_func = True
-        else:
-            set_func = True
-
-        if set_func and eval(f'isfunction(Trainer.{k})'):
-            exec(f'obj.{k} = types.MethodType(Trainer.{k}, obj)')
-            added_funcs.append(k)
-    obj.initialize()  # 这里初始化会得到一些其他的成员变量, 不可缺省
-
-    if verbose and (len(added_funcs) > 0):
-        log_info(f'Already add `{",".join(added_funcs)}` method')
-    return obj
-
-
-def add_module(obj, include=None, exclude=None, verbose=0, replace_func=False):
-    '''为Trainer增加nn.Module的方法
-    方便外部访问, 如obj.parameters()可以直接访问到obj.module.parameters()
-    '''
-    if isinstance(obj, nn.Module):
-        return obj
-    elif not isinstance(obj, Trainer):
-        log_warn('obj is not a Trainer object')
-        return obj
-    elif not isinstance(obj.unwrap_model(), nn.Module):
-        log_warn('obj.unwrap_model() is not a nn.Module object')
-        return obj
-    
-    if include is None:
-        include = set()
-    elif isinstance(include, str):
-        include = set([include])
-    elif isinstance(include, (tuple, list)):
-        include = set(include)
-    else:
-        raise TypeError(f'Arg `include` only receive str/list format, not {type(include)}')
-
-    if exclude is None:
-        exclude = set()
-    elif isinstance(exclude, (tuple, list)):
-        exclude = set(exclude)
-
-
-    import types
-    added_funcs = []
-    for k in dir(obj.unwrap_model()):
-        set_func = False
-        if k in include:  # 必须包含的
-            set_func = True
-        elif k in exclude:  # 必须屏蔽的
-            pass
-        elif k.startswith('__') and k.endswith('__'):
-            pass
-        elif hasattr(obj, k):  # 如果下游重新定义, 则不继
-            if replace_func:
-                set_func = True
-        else:
-            set_func = True
-        
-        if set_func and eval(f'isinstance(obj.unwrap_model().{k}, types.MethodType)'):
-            exec(f'obj.{k} = obj.unwrap_model().{k}')
-            added_funcs.append(k)
-
-    if verbose and (len(added_funcs) > 0):
-        log_info(f'Already add `{",".join(added_funcs)}` method')
-    return obj
+from torch import nn
+import torch
+from torch.optim import Optimizer
+from torch.optim.lr_scheduler import LambdaLR
+from torch.utils.data import DataLoader
+from torch4keras.snippets import metric_mapping, get_parameter_device, log_info, log_warn, print_table
+from torch4keras.snippets import print_trainable_parameters, colorful, send_email, load_checkpoint, save_checkpoint
+from torch4keras.callbacks import KerasProgbar, SmoothMetricsCallback, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, History
+from collections import OrderedDict
+from typing import Union, List, Literal, Tuple, Set, Callable, Optional
+from inspect import isfunction
+import os
+import math
+import re
+import traceback
+
+
+class Trainer:
+    '''Trainer, 传入Module实例
+
+    :param module: None/nn.Module, nn.Module()的模型实例
+
+    Example
+    -------------------
+    >>> import torch
+    >>> import torch.nn as nn
+    >>> import torch.optim as optim
+    >>> import torchvision
+    >>> from torch4keras.model import Trainer
+    >>> from torch.utils.data import TensorDataset, DataLoader
+    >>> 
+    >>> device = 'cuda' if torch.cuda.is_available() else 'cpu'
+    >>> 
+    >>> # 读取数据
+    >>> mnist = torchvision.datasets.MNIST(root='./', download=True)
+    >>> x, y = mnist.train_data.unsqueeze(1).to(device).float() / 255.0, mnist.train_labels.to(device)
+    >>> train_dataloader = DataLoader(TensorDataset(x, y), batch_size=8)
+    >>> 
+    >>> # 准备模型
+    >>> net = torch.nn.Sequential(
+    >>>             nn.Conv2d(1, 32, kernel_size=3), nn.ReLU(),
+    >>>             nn.MaxPool2d(2, 2), 
+    >>>             nn.Conv2d(32, 64, kernel_size=3), nn.ReLU(),
+    >>>             nn.Flatten(),
+    >>>             nn.Linear(7744, 10)
+    >>>         )
+    >>> 
+    >>> model = Trainer(net.to(device))
+    >>> model.compile(optimizer=optim.Adam(net.parameters()), loss=nn.CrossEntropyLoss())
+    >>>
+    >>> # 模型开始训练
+    >>> model.fit(train_dataloader, steps_per_epoch=None, epochs=5)
+    '''
+    def __init__(self, module:nn.Module=None):
+        super(Trainer, self).__init__()
+        self.initialize(module)
+    
+    def initialize(self, module:nn.Module=None):
+        # 传入Module实例方式
+        if module is not None:
+            if not isinstance(module, nn.Module):
+                raise TypeError(f'Args `module` only support nn.Module format not {type(module)}')
+            self.module = module
+
+        self.global_step, self.local_step, self.total_steps, self.batch_step = 0, 0, 0, 0
+        self.epoch, self.steps_per_epoch, self.train_dataloader = 0, None, None
+        self.resume_step, self.resume_epoch, self.resume_batch = 0, 0, 0
+        self.retain_graph = False  # loss.backward()是否保留计算图
+        self.move_to_model_device = True  # 自动把tensor转到model所在的device
+        self.log_first_step = False  # 是否打印第一个step的数据
+        self.criterion = None  # criterion
+        self.optimizer = None  # optimizer
+        self.scheduler = None  # scheduler
+        self.callbacks = []  # 所有的Callbacks, 如果fit中不传入, 则默认为[progbarlogger, smoothmetrics, history]三项
+        self.run_callbacks = True  # 是否运行Callbacks, 目前主要是在DDP模式下运用
+        self.loss2metrics = True  # 把loss_detail打印在进度条的metrics上
+        # add_module(self)  # 增加nn.Module的成员方法
+
+    def compile(self, loss:Optional[Union[Callable, nn.Module]]=None, optimizer:Optimizer=None, scheduler:LambdaLR=None, clip_grad_norm:float=None, 
+                mixed_precision:Literal[True, False, 'fp16', 'bf16']=False, metrics:Union[str, dict, Callable, List[Union[str, dict, Callable]]]=None, 
+                grad_accumulation_steps:int=1, progbar_type:Literal['keras', 'tqdm', 'progressbar2']='keras', progbar_width:int=None,
+                stateful_metrics:Union[str, Set[str], Tuple[str], List[str]]=None, smooth_interval:int=100, **kwargs):
+        '''complile: 定义loss, optimizer, metrics等参数
+        
+        :param loss: loss
+        :param optimizer: 优化器
+        :param scheduler: lr_scheduler
+        :param clip_grad_norm: float, 是否使用梯度裁剪, 默认为False
+        :param mixed_precision: bool, 是否使用混合精度, 默认为False
+        :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric, 形式为{key: func}
+        :param grad_accumulation_steps: int, 梯度累积步数, 默认为1
+        :param bar: str, 使用进度条的种类, 从kwargs中解析, 默认为keras, 可选keras, tqdm, progressbar2
+
+        > 进度条的配置
+            progbar_type: str, 默认为keras, 可选keras, tqdm, progressbar2
+            width: int, keras进度条下表示进度条的长度
+        > 指标平滑的配置, 默认为None表示采取默认平滑设置; 传入False表示不使用平滑
+            stateful_metrics: List[str], 表示不使用指标平滑仅进行状态记录的metric, 指标抖动会更加明显, 默认为None表示使用指标平滑
+            smooth_interval: int, 表示指标平滑时候的累计步数, 默认为100
+
+        :return: None
+        '''
+        self.criterion = loss or self.criterion  # loss
+        self.optimizer = optimizer or self.optimizer  # 优化器
+        self.scheduler = scheduler or self.scheduler  # lr_scheduler
+        self.clip_grad_norm = clip_grad_norm  # 梯度裁剪
+        self.grad_accumulation_steps = grad_accumulation_steps  # 梯度累积
+
+        # 混合精度
+        assert mixed_precision in {True, False, 'fp16', 'bf16'}
+        self.mixed_precision_mode = 'fp16' if mixed_precision is True else mixed_precision
+        if self.mixed_precision_mode:
+            self.autocast = torch.cuda.amp.autocast
+            self.scaler = torch.cuda.amp.GradScaler()
+
+        # 训练过程观测的指标
+        self.metrics = OrderedDict({'loss': None})
+        if metrics is None:
+            metrics = []
+        elif isinstance(metrics, (str, dict)) or isfunction(metrics):
+            metrics = [metrics]
+        for metric in metrics:
+            # 字符类型, 目前仅支持accuracy
+            if isinstance(metric, str) and metric != 'loss':
+                self.metrics[metric] = None
+            # 字典形式 {metric: func}
+            elif isinstance(metric, dict):
+                self.metrics.update(metric)
+            # 函数形式, key和value都赋值metric
+            elif isfunction(metric):
+                self.metrics.update({metric: metric})
+            else:
+                raise TypeError('Args metrics only support `String, Dict, Callable, List[String, Dict, Callable]` format')
+
+        # 进度条参数
+        assert progbar_type in {'keras', 'tqdm', 'progressbar2'}
+        self.progbar_config = {'bar': progbar_type, 'width': progbar_width}
+        self.progbar_config = {k:v for k,v in self.progbar_config.items() if v is not None}
+
+        # smooth_metrics参数: 默认平滑
+        self.smooth_metrics_config = {'stateful_metrics': stateful_metrics, 'interval': smooth_interval, 'verbose': kwargs.get('verbose')}
+        self.smooth_metrics_config = {k:v for k,v in self.smooth_metrics_config.items() if v is not None}
+
+        # 其他参数设置
+        for key, value in kwargs.items():
+            if hasattr(self, key):
+                setattr(self, key, value)
+
+    def print_trainable_parameters(self):
+        '''打印可训练的参数量'''
+        print_trainable_parameters(self.unwrap_model())
+
+    @property
+    def device(self) -> torch.device:
+        '''获取model所在的device'''
+        if hasattr(self, '_device'):
+            return self._device
+        return get_parameter_device(self.unwrap_model())
+
+    @device.setter
+    def device(self, value):
+        '''允许修改self.device'''
+        self._device = value
+
+    def to_device(self, device:Union[str, torch.device, int]):
+        self.unwrap_model().to(device)
+
+    def _move_to_model_device(self, inputs:Union[torch.Tensor, tuple, list, dict]):
+        '''遍历并转移到model.device上（递归）'''
+        if self.move_to_model_device:
+            if isinstance(inputs, torch.Tensor) and hasattr(self, 'device') and (inputs.device != self.device):
+                inputs = inputs.to(self.device)
+            elif isinstance(inputs, (tuple, list)):
+                inputs = list(inputs) if isinstance(inputs, tuple) else inputs
+                for i, ts in enumerate(inputs):
+                    inputs[i] = self._move_to_model_device(ts)
+            elif isinstance(inputs, dict):
+                for k, v in inputs.items():
+                    inputs[k] = self._move_to_model_device(v)
+        return inputs
+
+    def _log_first_step(self, resume_step, train_X, train_y):
+        '''打印第一个step的数据'''
+        if self.log_first_step and self.verbose and (self.global_step == resume_step):
+            print(colorful('[Train_data]: ', color='green'), + train_X)
+            print(colorful('[Label]: ', color='green'), + train_y)
+
+    def _forward(self, *inputs, **input_kwargs):
+        '''调用模型的forward, 方便下游继承的时候可以自定义使用哪个模型的forward
+        '''
+        return self._argparse_forward(self.unwrap_model(), *inputs, **input_kwargs)
+
+    def _argparse_forward(self, model:nn.Module, *inputs, **input_kwargs):
+        '''调用模型的forward
+        如果传入了网络结构module, 则调用module的forward; 如果是继承方式, 则调用自身的forward
+        这里声明为staticmethod的话, 使用add_trainer会有问题
+        '''
+        if (len(inputs)==1) and isinstance(inputs[0], (tuple,list)):  # 防止([])嵌套
+            inputs = inputs[0]
+        
+        if isinstance(inputs, torch.Tensor):  # tensor不展开
+            return model.forward(inputs, **input_kwargs)
+        elif isinstance(inputs, (tuple, list)):
+            return model.forward(*inputs, **input_kwargs)
+        else:
+            return model.forward(inputs, **input_kwargs)
+
+    def train_step(self, train_X, train_y):
+        ''' Perform a training step on a batch of inputs. '''
+        # 计算loss
+        if self.mixed_precision_mode:
+            with self.autocast(dtype=torch.float16 if self.mixed_precision_mode=='fp16' else torch.bfloat16):
+                output = self._forward(train_X)
+                loss_detail = self.criterion(output, train_y)
+        else:
+            output = self._forward(train_X)
+            loss_detail = self.criterion(output, train_y)
+
+        # 整理loss
+        if isinstance(loss_detail, torch.Tensor):
+            loss = loss_detail
+            loss_detail = {}
+        elif isinstance(loss_detail, dict):
+            loss = loss_detail['loss']  # 还存在其他loss, 仅用于打印
+            del loss_detail['loss']
+        elif isinstance(loss_detail, (tuple, list)):
+            loss = loss_detail[0]
+            loss_detail = {f'loss{i}':v for i, v in enumerate(loss_detail[1:], start=1)}
+        else:
+            raise ValueError('Return loss only support `Tensor/dict/tuple/list` format')
+
+        # 梯度累积
+        loss = loss / self.grad_accumulation_steps if self.grad_accumulation_steps > 1 else loss
+
+        # loss backward
+        loss = self.loss_backward(loss)
+        loss_detail = {k: (v.item() if isinstance(v, torch.Tensor) else v) / self.grad_accumulation_steps for k, v in loss_detail.items()}
+        return output, loss, loss_detail
+
+    def loss_backward(self, loss):
+        '''loss.backward'''
+        self.scale_before_step = 0
+        if self.mixed_precision_mode:  # 混合精度
+            self.scale_before_step = self.scaler.get_scale()
+            self.scaler.scale(loss).backward(retain_graph=self.retain_graph)
+        else:
+            loss.backward(retain_graph=self.retain_graph)
+        return loss
+    
+    def step(self):
+        '''参数更新'''
+        skip_scheduler = False
+        # 混合精度
+        if self.mixed_precision_mode:
+            self.scaler.unscale_(self.optimizer)
+            if self.clip_grad_norm is not None:  # 梯度裁剪
+                torch.nn.utils.clip_grad_norm_(self.unwrap_model().parameters(), self.clip_grad_norm)
+            self.scaler.step(self.optimizer)
+            self.scaler.update()
+            skip_scheduler = self.scaler.get_scale() != self.scale_before_step
+        else:
+            if self.clip_grad_norm is not None:  # 梯度裁剪
+                torch.nn.utils.clip_grad_norm_(self.unwrap_model().parameters(), self.clip_grad_norm)
+            self.optimizer.step()
+
+        self.optimizer.zero_grad()  # 清梯度
+        if (self.scheduler is not None) and not skip_scheduler:
+            if isinstance(self.scheduler, (tuple, list)):
+                for scheduler in self.scheduler:
+                    scheduler.step()
+            else:
+                self.scheduler.step()
+
+    def _prepare_inputs(self, train_dataloader:DataLoader, steps_per_epoch:Union[int,None], epochs:int, verbose:int):
+        '''对fit的输入进行类型检查并置为成员变量'''
+        if not hasattr(train_dataloader, '__len__'):
+            assert steps_per_epoch is not None, 'Either train_dataloader has attr `__len__` or steps_per_epoch is not None'
+        if steps_per_epoch is None:
+            self.steps_per_epoch = math.ceil(len(train_dataloader) // self.grad_accumulation_steps)
+        else:
+            self.steps_per_epoch = steps_per_epoch
+        self.batch_size = train_dataloader.batch_size
+        self.epochs = epochs
+        self.total_steps = self.steps_per_epoch * epochs
+        self.train_dataloader = train_dataloader  # 设置为成员变量, 可由外部的callbacks进行修改
+        self.train_dataloader_iter = iter(self.train_dataloader)  # 循环epoch时不重生成
+        self.verbose = self.verbose if hasattr(self, 'verbose') else verbose
+
+    def _prepare_callbacks(self, callbacks:Union[Callback, List[Callback]]=None):
+        '''callbacks设置'''
+        if callbacks is None:
+            callbacks = []
+        elif isinstance(callbacks, Callback):
+            callbacks = [callbacks]
+        for callback in callbacks:
+            assert isinstance(callback, Callback), f"Args `callbacks` only support Callback(), but got {type(callback)}"
+
+        history = History()
+        callbacks_ = []
+
+        # 指标平滑
+        if any([isinstance(i, SmoothMetricsCallback) for i in callbacks]):
+            # 用户自定的callbacks中包含了SmoothMetricsCallback
+            log_warn(f'SmoothMetricsCallback already in use and args `smooth_metrics_config` will be ignored')
+            smooth_callback = [callback for callback in callbacks if isinstance(callback, SmoothMetricsCallback)][0]
+            callbacks_.append(smooth_callback)
+            callbacks = [callback for callback in callbacks if not isinstance(callback, SmoothMetricsCallback)]
+        elif self.smooth_metrics_config.get('interval') is not None:
+            self.smooth_metrics_config['seen_so_far'] = self.resume_step + self.resume_epoch * self.steps_per_epoch  # 支持断点续训
+            smooth_callback = SmoothMetricsCallback(**self.smooth_metrics_config)
+            callbacks_.append(smooth_callback)
+        else:
+            # 不平滑
+            smooth_callback = None
+
+        # 检查指标平滑的设置和后续callback的设置的interval是不是一致
+        for callback in callbacks:
+            if hasattr(callback, 'interval') and (smooth_callback is not None) and (callback != smooth_callback) and \
+                (callback.interval is not None) and (callback.interval % smooth_callback.interval != 0):
+                log_warn(f'{type(callback).__name__}.interval={callback.interval} while SmoothMetricsCallback.interval={smooth_callback.interval}')
+        
+        # 进度条
+        progbarlogger = None
+        if self.verbose:
+            if self.progbar_config['bar'] == 'keras':
+                progbarlogger = KerasProgbar(**self.progbar_config)
+            elif self.progbar_config['bar'] == 'tqdm':
+                progbarlogger = TqdmProgbar(**self.progbar_config)
+            elif self.progbar_config['bar'] == 'progressbar2':
+                progbarlogger = ProgressBar2Progbar(**self.progbar_config)
+            else:
+                progbarlogger = KerasProgbar(**self.progbar_config)
+            callbacks_.append(progbarlogger)
+
+        callbacks_  += callbacks + [history]
+        self.callbacks = CallbackList(callbacks_, run_callbacks=self.run_callbacks)
+        callback_trainer = self
+        callback_model = self.unwrap_model()
+        params = {
+            'epochs': self.epochs,
+            'steps': self.steps_per_epoch,
+            'verbose': self.verbose,
+            'metrics': [i for i in self.metrics.keys() if isinstance(i, str)],
+        }
+        self.callbacks.set_all(trainer=callback_trainer, model=callback_model, optimizer=self.optimizer, scheduler=self.scheduler, params=params)
+        callback_trainer.stop_training = False  # 在EarlyStopping中会重新设置
+        return history, callback_trainer, progbarlogger
+
+    def prepare_nextbatch(self):
+        '''准备下一个batch数据'''
+        # 循环dataloader, 不要试用itertools的cycle, 遇到过变量不释放的问题
+        def _prepare_nextbatch():
+            try:
+                batch = next(self.train_dataloader_iter)
+            except StopIteration:
+                self.callbacks.on_dataloader_end()  # 适用于数据量较大时, 动态读取文件并重新生成self.train_dataloader的情况, 如预训练
+                # DDP训练时候为了避免每个epoch样本一致, 修改随机种子
+                if isinstance(self.train_dataloader.sampler, torch.utils.data.distributed.DistributedSampler) and \
+                    hasattr(self.train_dataloader.sampler, 'set_epoch'):
+                    self.train_dataloader.sampler.set_epoch(self.epoch)
+                self.train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候, 其实顺序也重新生成了
+                batch = next(self.train_dataloader_iter)
+            self.batch_step += 1
+            return batch
+        
+        # 若使用梯度累计grad_accumulation_steps，则batch_step和global_step会不一致
+        if self.batch_step > self.resume_batch:
+            # 从头开始
+            batch = _prepare_nextbatch()
+        else:
+            # 断点续训
+            while self.batch_step <= self.resume_batch:
+                batch = _prepare_nextbatch()
+        batch = self._move_to_model_device(batch)
+        return batch
+
+    def fit(self, train_dataloader:DataLoader, steps_per_epoch:int=None, epochs:int=1, 
+            callbacks:Union[Callback, List[Callback]]=None, verbose:int=1, **kwargs):
+        ''' 模型训练
+        :param train_dataloader: Dataloader, 训练数据集
+        :param steps_per_epoch: int, 每个epoch训练的steps, 默认为None表示自行计算 
+        :param epochs: int, 训练的轮次, 默认为1
+        :param callbacks: Callback/List[Callback], 回调函数, 可调用预制的Callback或者自定义, 默认为None 
+        :param verbose: int, 是否打印, 默认为1表示打印
+        
+        > 其他参数
+        :param mail_receivers_when_error: str, 训练异常时候邮件通知
+        :param save_ckpt_dir_when_error: str, 训练异常时候保存权重的路径
+        :param save_batch_path_when_error: bool, 训练异常时候保存当前batch, 方便debug
+
+        :return: History
+        '''
+        try:
+            return self._fit(train_dataloader, steps_per_epoch, epochs, callbacks, verbose, **kwargs)
+        except Exception as e:
+            # 训练异常则发邮件
+            error_msg = traceback.format_exc()
+            mail_receivers_ = kwargs.get('mail_receivers_when_error')
+            if mail_receivers_ is not None:
+                mail_subject_ = kwargs.get('mail_subject_when_error') or "[ERROR] fit"
+                mail_host_ = kwargs.get('mail_host_when_error')
+                mail_user_ = kwargs.get('mail_user_when_error')
+                mail_pwd_ = kwargs.get('mail_pwd_when_error')
+                mail_sender_ = kwargs.get('mail_sender_when_error')
+                send_email(mail_receivers_, mail_subject_, error_msg, mail_host=mail_host_, 
+                           mail_user=mail_user_, mail_pwd=mail_pwd_, mail_sender=mail_sender_)
+
+            # 训练异常则保存权重
+            if (save_ckpt_dir_when_error := kwargs.get('save_ckpt_dir_when_error')) is not None:
+                self.save_to_checkpoint(save_ckpt_dir_when_error, verbose=verbose, **kwargs)
+
+            # 训练异常则打印当前batch
+            if (save_batch_path_when_error := kwargs.get('save_batch_path_when_error')) is not None:
+                os.makedirs(os.path.dirname(save_batch_path_when_error), exist_ok=True)
+                torch.save({'train_X': self.train_X.cpu(), 'train_y': self.train_y.cpu()}, save_batch_path_when_error)
+            
+            raise e
+
+    def _fit(self, train_dataloader:DataLoader, steps_per_epoch:int=None, epochs:int=1, 
+             callbacks:Union[Callback, List[Callback]]=None, verbose:int=1, **kwargs):
+        '''模型训练'''
+        # 输入处理
+        self._prepare_inputs(train_dataloader, steps_per_epoch, epochs, verbose)
+
+        # 准备callbacks
+        history, callback_trainer, progbarlogger  = self._prepare_callbacks(callbacks)
+
+        #       epoch: 当前epoch
+        # global_step: 当前全局训练步数
+        #  local_step: 当前epoch内的训练步数, 不同epoch中相同local_step对应的batch数据不一定相同, 在steps_per_epoch=None时相同
+        #  batch_step: 在dataloader中的index, 不同epoch中相同的bti对应的batch数据一般相同, 除非重新生成dataloader
+        self.callbacks.on_train_begin()
+        logs = self._log_init()  # 防止数据集为空时候
+        for epoch in range(self.resume_epoch, epochs):
+            self.epoch = epoch
+            # resume_step：判断local_step的起点, 以及进度条的起始位置
+            resume_step = self.resume_step if epoch==self.resume_epoch else 0
+            self.callbacks.on_epoch_begin(self.global_step, self.epoch)
+            if self.verbose:
+                progbarlogger.seen = resume_step  # 这里设置进度条的seen, 在callbacks中也会修改
+            
+            for local_step in range(resume_step, self.steps_per_epoch):
+                self.local_step = local_step
+                self.global_step = self.epoch * self.steps_per_epoch + self.local_step
+                logs = self._log_init()
+                self.callbacks.on_batch_begin(self.global_step, self.local_step, logs)
+
+                # forward和backward
+                if not self.unwrap_model().training:
+                    self.unwrap_model().train()  # 设置为train模式
+                tr_loss, tr_loss_detail = 0, {}
+                for _ in range(self.grad_accumulation_steps):
+                    self.train_X, self.train_y = self.prepare_nextbatch()  # 获取下一个batch的训练数据
+                    self._log_first_step(resume_step, self.train_X, self.train_y)  # log第一个step
+                    output, loss, loss_detail = self.train_step(self.train_X, self.train_y)
+                    self.callbacks.on_train_step_end()
+                    tr_loss += loss.item()
+                    for k, v in loss_detail.items():
+                        tr_loss_detail[k] = tr_loss_detail.get(k, 0) + v
+                # TODO: 理论上梯度累积时需对output和train_y进行合并, 主要是为了metric_mapping计算的准确
+                
+                # 参数更新
+                self.step()
+
+                # 添加loss至log打印
+                logs.update(dict({'loss': tr_loss}, **tr_loss_detail))
+                if self.verbose and self.loss2metrics and (self.global_step == resume_step):
+                    # 把loss_detail添加到进度条metrics中
+                    progbarlogger.add_metrics(list(tr_loss_detail.keys()), add_position=1)
+                    
+                # 添加metrics至log打印
+                for metric, func in self.metrics.items():
+                    perf = metric_mapping(metric, func, output, self.train_y)  # 内置的一些accuracy指标
+                    if perf is not None:
+                        if isfunction(metric):  # 直接传入回调函数(无key)
+                            if self.verbose and (self.global_step == resume_step):
+                                progbarlogger.add_metrics(list(perf.keys()))
+                            logs.update(perf)
+                        elif isinstance(metric, str):  # 直接传入回调函数(有key)
+                            logs[metric] = perf
+
+                self.callbacks.on_batch_end(self.global_step, self.local_step, logs)
+
+            self.callbacks.on_epoch_end(self.global_step, self.epoch, logs)
+            # TerminateOnNaN、EarlyStopping等停止训练策略
+            if callback_trainer.stop_training:
+                break
+        self.callbacks.on_train_end(logs)
+        return history
+
+    def _log_init(self):
+        '''获取batch_size, 主要是用于callback中的BaseLogger和Callback
+        '''
+        logs = {}
+
+        # 添加lr
+        try:
+            logs['lr'] = self.optimizer.param_groups[0]["lr"]
+        except:
+            pass
+        return logs
+
+    @torch.no_grad()
+    def predict(self, *inputs, **input_kwargs):
+        '''模型预测, 调用forward()'''
+        self.unwrap_model().eval()
+        inputs = self._move_to_model_device(inputs)
+        input_kwargs = self._move_to_model_device(input_kwargs)
+        return self._forward(*inputs, **input_kwargs)
+        
+    def load_steps_params(self, save_path:str):
+        '''导入训练过程参数
+        
+        :param save_path: str, 训练过程参数保存路径
+        '''
+        step_params = torch.load(save_path)
+        self.resume_step = step_params['resume_step'] 
+        self.resume_epoch = step_params['resume_epoch']
+        self.resume_batch = step_params.get('resume_batch', 0)  # 兼容老版本
+        return step_params
+
+    def save_steps_params(self, save_path:str):
+        '''保存训练过程参数
+
+        :param save_path: str, 训练过程参数保存路径
+        '''
+        step_params = {
+            'resume_step': (self.local_step+1) % self.steps_per_epoch,  # 当前epoch下的step数量
+            'resume_epoch': self.epoch + (self.local_step+1) // self.steps_per_epoch,  # 经过的epoch数量
+            'resume_batch': self.batch_step  # 经过的batch数量
+            }
+        save_dir = os.path.dirname(save_path)
+        os.makedirs(save_dir, exist_ok=True)
+        torch.save(step_params, save_path)
+
+    def load_weights(self, load_path:Union[str,tuple,list], strict:bool=True, mapping:Union[dict,Callable]=None):
+        '''加载模型权重, 支持加载权重文件list
+
+        :param save_path: str/tuple/list, 权重加载路径
+        :param strict: bool, torch.load()是否严格加载
+        :param mapping: dict/func, 指定key的映射
+            1. mapping=None, 表示按照模型自身结构加载, 一般加载finetune后使用save_weights()保存出来的权重
+            2. mapping自定义, 根据用户自定义mapping来加载权重
+        '''
+        if isinstance(load_path, (tuple, list)):
+            strict = False  # 加载多个权重文件时候, strict设置为False
+        elif isinstance(load_path, str):
+            load_path = [load_path]
+        else:
+            raise ValueError('Args `load_path` only support str/tuple/list format')
+        
+        mapping = mapping or dict()
+        for load_path_i in load_path:
+            state_dict = load_checkpoint(load_path_i)
+            for k in list(state_dict.keys()):
+                if isinstance(mapping, dict) and k in mapping:
+                    state_dict[mapping[k]] = state_dict.pop(k)
+                elif isinstance(mapping, Callable):
+                    state_dict[mapping(k)] = state_dict.pop(k)
+            self.unwrap_model().load_state_dict(state_dict, strict=strict)
+
+    def save_weights(self, save_path:str, mapping:Union[dict,Callable]=None, trainable_only:bool=False):
+        '''保存模型权重
+
+        :param save_path: str, 权重保存路径
+        :param mapping: dict/func, 指定key的映射
+            1. mapping=None, 表示按照模型自身结构的key来保存, 后续可直接load_weights()加载
+            2. mapping自定义, 根据用户自定义mapping来保存权重
+        :param trainable_only: bool, 指定仅保存可训练参数
+        '''
+        state_dict = self.unwrap_model().state_dict()
+        trainable_parameters = set(p for p,v in self.unwrap_model().named_parameters() if v.requires_grad)
+        
+        mapping = mapping or dict()
+        for k in list(state_dict.keys()):
+            # 只保存可训练的模型部分
+            if trainable_only and (k not in trainable_parameters):
+                continue
+            if isinstance(mapping, dict) and k in mapping:
+                state_dict[mapping[k]] = state_dict.pop(k)
+            elif isinstance(mapping, Callable):
+                state_dict[mapping(k)] = state_dict.pop(k)        
+        save_checkpoint(state_dict, save_path)
+        if trainable_only:
+            params_all = sum(p.numel() for p in self.unwrap_model().parameters())
+            params_trainable = sum(p.numel() for p in self.unwrap_model().parameters() if p.requires_grad)
+            ratio = params_trainable/params_all*100
+            log_info(f"Only trainable parameters saved and occupy {params_trainable}/{params_all}={ratio:.2f}%")
+
+    def save_pretrained(self, save_path:str, weight_map:dict=None, mapping:Union[dict,Callable]=None):
+        '''按照预训练模型的key来保存模型, 可供transformers包加载
+
+        :param save_path: str, 保存的文件/文件夹路径
+        '''
+        state_dict = dict()
+        for name, child in self.unwrap_model().named_children():
+            if (name != '') and hasattr(child, 'save_pretrained'):
+                tmp = child.save_pretrained(save_path, weight_map, mapping, write_to_disk=False)
+                state_dict.update(tmp if tmp else {})
+            else:
+                state_dict.update({f'{name}.{k}': v for k,v in child.state_dict().items()})
+        if len(state_dict) > 0:
+            save_dir = None if re.search(r'\.[a-zA-z0-9]+$', save_path) else save_path
+            save_checkpoint(state_dict, os.path.join(save_dir, 'pytorch_model.bin') if save_dir else save_path)
+    
+    def resume_from_checkpoint(self, save_dir:str=None, mapping:Union[dict,Callable]=None, strict:bool=True, device=None, verbose:int=1, **kwargs):
+        '''同时加载模型、优化器、训练过程参数, 以保证断点续训和不断效果一致或相当
+
+        :param save_dir: str, 保存目录
+        :param mapping: dict, 模型文件的mapping
+        :param strict: bool, 是否严格加载
+        :param device: 加载的device
+        :param verbose: int, 是否打印resume成功的信息, 默认打印
+
+        > 可选参数
+        :param model_path: str, 模型文件路径
+        :param optimizer_path: str, 优化器文件路径
+        :param scheduler_path: str, scheduler文件路径
+        :param steps_params_path: str, 训练过程参数保存路径
+        '''
+        model_path = kwargs.get('model_path')
+        optimizer_path = kwargs.get('optimizer_path')
+        scheduler_path = kwargs.get('scheduler_path')
+        steps_params_path = kwargs.get('steps_params_path')
+
+        resume_info = []
+        # 加载模型权重
+        if model_path or save_dir:
+            model_path = model_path or os.path.join(save_dir, 'model.pt')
+            self.load_weights(model_path, strict=strict, mapping=mapping)
+            resume_info.append(['Model weights', model_path])
+
+        # 加载优化器
+        if optimizer_path or save_dir:
+            optimizer_path = optimizer_path or os.path.join(save_dir, 'optimizer.pt')
+            state_dict = torch.load(optimizer_path, map_location = device or self.device)
+            self.optimizer.load_state_dict(state_dict)
+            resume_info.append(['Optimizer', optimizer_path])
+
+        # 加载scheduler
+        if (scheduler_path or save_dir) and (self.scheduler is not None):
+            scheduler_path = scheduler_path or os.path.join(save_dir, 'scheduler.pt')
+            state_dict = torch.load(scheduler_path, map_location = device or self.device)
+            self.scheduler.load_state_dict(state_dict)
+            resume_info.append(['Scheduler', scheduler_path])
+
+        # 加载训练进度参数
+        if steps_params_path or save_dir:
+            steps_params_path = steps_params_path or os.path.join(save_dir, 'steps_params.pt')
+            self.load_steps_params(steps_params_path)
+            resume_info.append(['Steps_params', steps_params_path])
+
+        if verbose == 1 and len(resume_info) > 0:
+            log_info('Successfuly resume training checkpoint')
+            print_table(resume_info, headers=['File', 'Path'])
+
+    def save_to_checkpoint(self, save_dir:str=None, mapping:Union[dict,Callable]=None, trainable_only:bool=False, verbose:int=0, **kwargs):
+        '''同时保存模型、优化器、训练过程参数、scheduler
+
+        :param save_dir: str, 保存目录
+        :param mapping: dict/func, 模型文件的mapping
+        :param trainable_only
+
+        > 可选参数
+        :param model_path: str, 模型文件路径
+        :param optimizer_path: str, 优化器文件路径
+        :param scheduler_path: str, scheduler文件路径
+        :param steps_params_path: str, 训练过程参数保存路径
+        '''
+        model_path = kwargs.get('model_path')
+        optimizer_path = kwargs.get('optimizer_path')
+        scheduler_path = kwargs.get('scheduler_path')
+        steps_params_path = kwargs.get('steps_params_path')
+
+        load_info = []
+        if model_path or save_dir:
+            model_path = model_path or os.path.join(save_dir, 'model.pt')
+            self.save_weights(model_path, mapping=mapping, trainable_only=trainable_only)
+            load_info.append(['Model weights', model_path])
+
+        if optimizer_path or save_dir:
+            optimizer_path = optimizer_path or os.path.join(save_dir, 'optimizer.pt')
+            os.makedirs(os.path.dirname(optimizer_path), exist_ok=True)
+            torch.save(self.optimizer.state_dict(), optimizer_path)
+            load_info.append(['Optimizer', optimizer_path])
+
+        if (scheduler_path or save_dir) and (self.scheduler is not None):
+            scheduler_path = scheduler_path or os.path.join(save_dir, 'scheduler.pt')
+            os.makedirs(os.path.dirname(scheduler_path), exist_ok=True)
+            torch.save(self.scheduler.state_dict(), scheduler_path)
+            load_info.append(['Scheduler', scheduler_path])
+
+        if steps_params_path or save_dir:
+            steps_params_path = steps_params_path or os.path.join(save_dir, 'steps_params.pt')
+            self.save_steps_params(steps_params_path)
+            load_info.append(['Steps_params', steps_params_path])
+
+        if verbose == 1 and len(load_info) > 0:
+            log_info('Successfuly save training checkpoint')
+            print_table(load_info, headers=['File', 'Path'])
+
+    def unwrap_model(self):
+        '''返回nn.Module模块
+        '''
+        if isinstance(self, nn.Module):
+            return self
+        elif hasattr(self, 'module') and isinstance(self.module, nn.Module):
+            return self.module
+        else:
+            return self
+
+
+Trainer.compile_training_components = Trainer.compile
```

### Comparing `torch4keras-0.2.1.post2/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.2.2/torch4keras.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,91 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.2.1.post2
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![torch4keras](./docs/pics/torch4keras.png)
-
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-
-[Documentation](https://torch4keras.readthedocs.io) |
-[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
-[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-[Source code](https://github.com/Tongjilibo/torch4keras) |
-[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
-
-## 1. 下载安装
-安装稳定版
-```shell
-pip install torch4keras
-```
-安装最新版
-```shell
-pip install git+https://github.com/Tongjilibo/torch4keras.git
-```
-
-## 2. 功能
-- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-- 训练：
-
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
-
-    2022-10-28 23:17:37 - Finish Training
-    ```
-
-## 3. 快速上手
-- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-
-## 4. 版本历史
-|更新日期| 版本 | 版本说明 |
-|------| ----------------- |----------- |
-|20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
-|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
-|20240204|v0.1.9           | 增加Timeit, Timeit2, timeit等时间/速度监控|
-|20240116|v0.1.8           | 重新整理snippets, 重写save_pretrained|
-
-[更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
-
-## 5. 更新历史：
-
-[更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.2.2
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: torch>1.6
+
+![torch4keras](./docs/pics/torch4keras.png)
+
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+
+[Documentation](https://torch4keras.readthedocs.io) |
+[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
+[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+[Source code](https://github.com/Tongjilibo/torch4keras) |
+[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
+
+## 1. 下载安装
+安装稳定版
+```shell
+pip install torch4keras
+```
+安装最新版
+```shell
+pip install git+https://github.com/Tongjilibo/torch4keras.git
+```
+
+## 2. 功能
+- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+- 训练：
+
+    ```text
+    2022-10-28 23:16:10 - Start Training
+    2022-10-28 23:16:10 - Epoch: 1/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+    test_acc: 0.98045. best_test_acc: 0.98045
+
+    2022-10-28 23:16:27 - Epoch: 2/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+    test_acc: 0.98280. best_test_acc: 0.98280
+
+    2022-10-28 23:16:44 - Epoch: 3/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+    test_acc: 0.98365. best_test_acc: 0.98365
+
+    2022-10-28 23:17:03 - Epoch: 4/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+    test_acc: 0.98265. best_test_acc: 0.98365
+
+    2022-10-28 23:17:21 - Epoch: 5/5
+    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+    test_acc: 0.98585. best_test_acc: 0.98585
+
+    2022-10-28 23:17:37 - Finish Training
+    ```
+
+## 3. 快速上手
+- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+
+## 4. 版本历史
+|更新日期| 版本 | 版本说明 |
+|------| ----------------- |----------- |
+|20240418|v0.2.2|增加YamlConfig和IniConfig, 优化deepspeed的使用，修复`_prepare_inputs`的bug，修复断点续训`SmoothMetricsCallback`起点错误的bug, Trainer断点续训记录batch数|
+|20240317|v0.2.1.post2     |训练异常时保存权重，避免空数据集error，默认指标使用滑窗平滑，BaseModelDDP修改的更易用，mapping允许是函数更易用，Checkpoint增加save_on_train_end，增加SystemCallback，修改run_callback=False的bug, 适配build_MiniLLM_from_scratch, 修复ddp中mix_precision和torch重名的bug|
+|20240221|v0.2.0           | fit中修改.train()逻辑较少耗时|
+
+[更多版本](https://github.com/Tongjilibo/torch4keras/blob/master/docs/Update.md)
+
+## 5. 更新历史：
+
+[更多历史](https://github.com/Tongjilibo/torch4keras/blob/master/docs/History.md)
```

### Comparing `torch4keras-0.2.1.post2/torch4keras.egg-info/SOURCES.txt` & `torch4keras-0.2.2/torch4keras.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 README.md
 setup.py
 test/test_log.py
 test/test_time.py
 torch4keras/__init__.py
 torch4keras/callbacks.py
 torch4keras/model.py
-torch4keras/trainer.py
 torch4keras.egg-info/PKG-INFO
 torch4keras.egg-info/SOURCES.txt
 torch4keras.egg-info/dependency_links.txt
 torch4keras.egg-info/requires.txt
 torch4keras.egg-info/top_level.txt
 torch4keras/snippets/__init__.py
 torch4keras/snippets/data_process.py
 torch4keras/snippets/import_utils.py
 torch4keras/snippets/log.py
 torch4keras/snippets/misc.py
-torch4keras/snippets/monitor.py
+torch4keras/snippets/monitor.py
+torch4keras/trainer/__init__.py
+torch4keras/trainer/accelerate.py
+torch4keras/trainer/base.py
+torch4keras/trainer/ddp.py
+torch4keras/trainer/deepspeed.py
+torch4keras/trainer/dp.py
+torch4keras/trainer/utils.py
```

