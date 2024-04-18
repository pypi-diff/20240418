# Comparing `tmp/wolf_comm-0.0.6.tar.gz` & `tmp/wolf_comm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolf_comm-0.0.6.tar", last modified: Sun Feb 25 17:34:44 2024, max compression
+gzip compressed data, was "wolf_comm-0.0.7.tar", last modified: Thu Apr 18 17:57:11 2024, max compression
```

## Comparing `wolf_comm-0.0.6.tar` & `wolf_comm-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 17:34:44.089763 wolf_comm-0.0.6/
--rw-rw-rw-   0        0        0    11558 2024-02-15 15:01:23.000000 wolf_comm-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      909 2024-02-25 17:34:44.084761 wolf_comm-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      423 2024-02-24 06:36:52.000000 wolf_comm-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-02-25 17:34:44.090765 wolf_comm-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      794 2024-02-25 17:33:59.000000 wolf_comm-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-25 17:34:44.046759 wolf_comm-0.0.6/wolf_comm/
--rw-rw-rw-   0        0        0       69 2024-02-10 18:25:03.000000 wolf_comm-0.0.6/wolf_comm/__init__.py
--rw-rw-rw-   0        0        0     1205 2024-02-10 18:13:37.000000 wolf_comm-0.0.6/wolf_comm/constants.py
--rw-rw-rw-   0        0        0      684 2024-02-23 19:06:17.000000 wolf_comm-0.0.6/wolf_comm/create_session.py
--rw-rw-rw-   0        0        0       81 2024-02-10 18:13:37.000000 wolf_comm-0.0.6/wolf_comm/helpers.py
--rw-rw-rw-   0        0        0     5980 2024-02-10 18:13:37.000000 wolf_comm-0.0.6/wolf_comm/models.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:13:37.000000 wolf_comm-0.0.6/wolf_comm/py.typed
--rw-rw-rw-   0        0        0     4538 2024-02-23 18:30:47.000000 wolf_comm-0.0.6/wolf_comm/token_auth.py
--rw-rw-rw-   0        0        0     8486 2024-02-25 17:30:09.000000 wolf_comm-0.0.6/wolf_comm/wolf_client.py
-drwxrwxrwx   0        0        0        0 2024-02-25 17:34:44.080758 wolf_comm-0.0.6/wolf_comm.egg-info/
--rw-rw-rw-   0        0        0      909 2024-02-25 17:34:43.000000 wolf_comm-0.0.6/wolf_comm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-02-25 17:34:43.000000 wolf_comm-0.0.6/wolf_comm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 17:34:43.000000 wolf_comm-0.0.6/wolf_comm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-02-25 17:34:43.000000 wolf_comm-0.0.6/wolf_comm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-25 17:34:43.000000 wolf_comm-0.0.6/wolf_comm.egg-info/top_level.txt
+drwxr-xr-x   0 i037503    (501) staff       (20)        0 2024-04-18 17:57:11.916415 wolf_comm-0.0.7/
+-rw-r--r--   0 i037503    (501) staff       (20)    11357 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/LICENSE.txt
+-rw-r--r--   0 i037503    (501) staff       (20)      831 2024-04-18 17:57:11.916075 wolf_comm-0.0.7/PKG-INFO
+-rw-r--r--   0 i037503    (501) staff       (20)      410 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/README.md
+-rw-r--r--   0 i037503    (501) staff       (20)       38 2024-04-18 17:57:11.916499 wolf_comm-0.0.7/setup.cfg
+-rw-r--r--   0 i037503    (501) staff       (20)      766 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/setup.py
+drwxr-xr-x   0 i037503    (501) staff       (20)        0 2024-04-18 17:57:11.905183 wolf_comm-0.0.7/wolf_comm/
+-rw-r--r--   0 i037503    (501) staff       (20)       67 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/__init__.py
+-rw-r--r--   0 i037503    (501) staff       (20)     1108 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/constants.py
+-rw-r--r--   0 i037503    (501) staff       (20)     1091 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/create_session.py
+-rw-r--r--   0 i037503    (501) staff       (20)       79 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/helpers.py
+-rw-r--r--   0 i037503    (501) staff       (20)     5713 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/models.py
+-rw-r--r--   0 i037503    (501) staff       (20)     4646 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/token_auth.py
+-rw-r--r--   0 i037503    (501) staff       (20)     8539 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/wolf_client.py
+drwxr-xr-x   0 i037503    (501) staff       (20)        0 2024-04-18 17:57:11.915663 wolf_comm-0.0.7/wolf_comm.egg-info/
+-rw-r--r--   0 i037503    (501) staff       (20)      831 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/PKG-INFO
+-rw-r--r--   0 i037503    (501) staff       (20)      357 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/SOURCES.txt
+-rw-r--r--   0 i037503    (501) staff       (20)        1 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/dependency_links.txt
+-rw-r--r--   0 i037503    (501) staff       (20)       26 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/requires.txt
+-rw-r--r--   0 i037503    (501) staff       (20)       10 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/top_level.txt
```

### Comparing `wolf_comm-0.0.6/LICENSE.txt` & `wolf_comm-0.0.7/LICENSE.txt`

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

### Comparing `wolf_comm-0.0.6/wolf_comm/constants.py` & `wolf_comm-0.0.7/wolf_comm/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-"""
-File with all constants
-"""
-
-BASE_URL = "https://www.wolf-smartset.com"
-
-BASE_URL_PORTAL = "https://www.wolf-smartset.com/portal"
-
-AUTHENTICATION_URL = "/idsrv"
-AUTHENTICATION_BASE_URL = BASE_URL + AUTHENTICATION_URL
-AUTHENTICATION_CLIENT = "smartset.web"
-
-SESSION_ID = 'SessionId'
-
-GUI_ID_CHANGED = 'GuiIdChanged'
-
-BUNDLE_ID = 'BundleId'
-
-BUNDLE = 'IsSubBundle'
-
-VALUE_ID_LIST = 'ValueIdList'
-
-ID = 'Id'
-
-SYSTEM_ID = 'SystemId'
-
-TAB_VIEWS = 'TabViews'
-
-MENU_ITEMS = 'MenuItems'
-
-GATEWAY_ID = "GatewayId"
-
-LAST_ACCESS = "LastAccess"
-
-TIMESTAMP = "Timestamp"
-
-ERROR_CODE = "ErrorCode"
-
-ERROR_TYPE = "ErrorType"
-
-ERROR_READ_PARAMETER = 'internal msg: ReadParameterValues error'
-
-ERROR_MESSAGE = 'Message'
-
-NAME = 'Name'
-
-PERCENTAGE = '%'
-
-HOUR = 'Std'
-
-BAR = 'bar'
-
-CELSIUS_TEMPERATURE = '°C'
-
-VALUES = 'Values'
-
-STATE = 'State'
-
-LIST_ITEMS = 'ListItems'
-
-DISPLAY_TEXT = 'DisplayText'
-
-VALUE = 'Value'
-
-PARAMETER_ID = 'ParameterId'
-
-PARAMETER_DESCRIPTORS = 'ParameterDescriptors'
-
-UNIT = 'Unit'
-
-TAB_NAME = 'TabName'
-
-VALUE_ID = 'ValueId'
-
-SYSTEM_LIST = 'SystemList'
-
-GATEWAY_STATE = 'GatewayState'
-
-IS_ONLINE = 'IsOnline'
+"""
+File with all constants
+"""
+
+BASE_URL = "https://www.wolf-smartset.com"
+
+BASE_URL_PORTAL = BASE_URL + "/portal"
+
+AUTHENTICATION_URL = "/idsrv"
+AUTHENTICATION_BASE_URL = BASE_URL + AUTHENTICATION_URL
+AUTHENTICATION_CLIENT = "smartset.web"
+
+SESSION_ID = 'SessionId'
+
+GUI_ID_CHANGED = 'GuiIdChanged'
+
+BUNDLE_ID = 'BundleId'
+
+BUNDLE = 'IsSubBundle'
+
+VALUE_ID_LIST = 'ValueIdList'
+
+ID = 'Id'
+
+SYSTEM_ID = 'SystemId'
+
+TAB_VIEWS = 'TabViews'
+
+MENU_ITEMS = 'MenuItems'
+
+GATEWAY_ID = "GatewayId"
+
+LAST_ACCESS = "LastAccess"
+
+TIMESTAMP = "Timestamp"
+
+ERROR_CODE = "ErrorCode"
+
+ERROR_TYPE = "ErrorType"
+
+ERROR_READ_PARAMETER = 'internal msg: ReadParameterValues error'
+
+ERROR_MESSAGE = 'Message'
+
+NAME = 'Name'
+
+PERCENTAGE = '%'
+
+HOUR = 'Std'
+
+BAR = 'bar'
+
+CELSIUS_TEMPERATURE = '°C'
+
+VALUES = 'Values'
+
+STATE = 'State'
+
+LIST_ITEMS = 'ListItems'
+
+DISPLAY_TEXT = 'DisplayText'
+
+VALUE = 'Value'
+
+PARAMETER_ID = 'ParameterId'
+
+PARAMETER_DESCRIPTORS = 'ParameterDescriptors'
+
+UNIT = 'Unit'
+
+TAB_NAME = 'TabName'
+
+VALUE_ID = 'ValueId'
+
+SYSTEM_LIST = 'SystemList'
+
+GATEWAY_STATE = 'GatewayState'
+
+IS_ONLINE = 'IsOnline'
```

### Comparing `wolf_comm-0.0.6/wolf_comm/create_session.py` & `wolf_comm-0.0.7/wolf_comm/create_session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-from datetime import datetime
-
-from httpx import AsyncClient, Headers
-
-from wolf_comm import constants
-from wolf_comm.constants import TIMESTAMP
-from wolf_comm.helpers import bearer_header
-
-
-async def create_session(client: AsyncClient, token: str):
-    data = {
-        TIMESTAMP: datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    }
-    resp = await client.post(constants.BASE_URL_PORTAL + "/api/portal/CreateSession2",
-                              headers=Headers({**bearer_header(token),
-                                               **{"Content-Type": "application/json"}}),
-                              json=data)
-
-    return resp.json()['BrowserSessionId']
+from datetime import datetime
+
+from httpx import AsyncClient, Headers
+
+from wolf_comm import constants
+from wolf_comm.constants import SESSION_ID, TIMESTAMP
+from wolf_comm.helpers import bearer_header
+
+
+async def create_session(client: AsyncClient, token: str):
+    data = {
+        TIMESTAMP: datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    }
+    resp = await client.post(constants.BASE_URL_PORTAL + "/api/portal/CreateSession2",
+                              headers=Headers({**bearer_header(token),
+                                               **{"Content-Type": "application/json"}}),
+                              json=data)
+
+    return resp.json()['BrowserSessionId']
+
+async def update_session(client: AsyncClient, token: str, session_id: str):
+    data = {
+        SESSION_ID: session_id
+    }
+    resp = await client.post(constants.BASE_URL_PORTAL + "/api/portal/UpdateSession",
+                              headers=Headers({**bearer_header(token),
+                                               **{"Content-Type": "application/json"}}),
+                              json=data)
```

### Comparing `wolf_comm-0.0.6/wolf_comm/wolf_client.py` & `wolf_comm-0.0.7/wolf_comm/wolf_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,199 @@
-import datetime
-from typing import Union
-
-import httpx
-import logging
-from httpx import Headers
-
-from wolf_comm.constants import BASE_URL_PORTAL, ID, GATEWAY_ID, NAME, SYSTEM_ID, MENU_ITEMS, TAB_VIEWS, BUNDLE_ID, \
-    BUNDLE, VALUE_ID_LIST, GUI_ID_CHANGED, SESSION_ID, VALUE_ID, VALUE, STATE, VALUES, PARAMETER_ID, UNIT, \
-    CELSIUS_TEMPERATURE, BAR, PERCENTAGE, LIST_ITEMS, DISPLAY_TEXT, PARAMETER_DESCRIPTORS, TAB_NAME, HOUR, \
-    LAST_ACCESS, ERROR_CODE, ERROR_TYPE, ERROR_MESSAGE, ERROR_READ_PARAMETER, SYSTEM_LIST, GATEWAY_STATE, IS_ONLINE
-from wolf_comm.create_session import create_session
-from wolf_comm.helpers import bearer_header
-from wolf_comm.models import Temperature, Parameter, SimpleParameter, Device, Pressure, ListItemParameter, \
-    PercentageParameter, Value, ListItem, HoursParameter
-from wolf_comm.token_auth import Tokens, TokenAuth
-
-_LOGGER = logging.getLogger(__name__)
-
-
-class WolfClient:
-    session_id: int or None
-    tokens: Tokens or None
-    last_access: datetime or None
-    last_failed: bool
-    
-    
-    @property
-    def client(self):
-        if hasattr(self, '_client') and self._client != None:
-            return self._client
-        elif hasattr(self, '_client_lambda') and self._client_lambda != None:
-            return self._client_lambda()
-        else:
-            raise RuntimeError("No valid client configuration")
-        
-
-    def __init__(self, username: str, password: str, client = None, client_lambda = None):
-        if client != None and client_lambda != None:
-            raise RuntimeError("Only one of client and client_lambda is allowed!")
-        elif client != None:
-            self._client = client
-        elif client_lambda != None:
-            self._client_lambda = client_lambda
-        else:
-            self._client = httpx.AsyncClient()
-        
-        self.tokens = None
-        self.token_auth = TokenAuth(username, password)
-        self.session_id = None
-        self.last_access = None
-        self.last_failed = False
-
-    async def __request(self, method: str, path: str, **kwargs) -> Union[dict, list]:
-        await self.__authorize_and_session()
-
-        headers = kwargs.get('headers')
-
-        if headers is None:
-            headers = bearer_header(self.tokens.access_token)
-        else:
-            headers = {**bearer_header(self.tokens.access_token), **dict(headers)}
-
-        resp = await self.__execute(headers, kwargs, method, path)
-        if resp.status_code == 401 or resp.status_code == 500:
-            _LOGGER.debug('Retrying')
-            await self.__authorize_and_session()
-            headers = {**bearer_header(self.tokens.access_token), **dict(headers)}
-            try:
-                execution = await self.__execute(headers, kwargs, method, path)
-                return execution.json()
-            except FetchFailed as e:
-                self.last_failed = True
-                raise e
-        else:
-            self.last_failed = False
-            return resp.json()
-
-    async def __execute(self, headers, kwargs, method, path):
-        return await self.client.request(method, f"{BASE_URL_PORTAL}/{path}", **dict(kwargs, headers=Headers(headers)))
-
-    async def __authorize_and_session(self):
-        self.tokens = await self.token_auth.token(self.client)
-        self.session_id = await create_session(self.client, self.tokens.access_token)
-
-    # api/portal/GetSystemList
-    async def fetch_system_list(self) -> [Device]:
-        system_list = await self.__request('get', 'api/portal/GetSystemList')
-        _LOGGER.debug('Fetched systems: %s', system_list)
-        return [Device(system[ID], system[GATEWAY_ID], system[NAME]) for system in system_list]
-
-    # api/portal/GetSystemStateList
-    async def fetch_system_state_list(self, system_id, gateway_id) -> bool:
-        payload = {SESSION_ID: self.session_id, SYSTEM_LIST: [{SYSTEM_ID: system_id, GATEWAY_ID: gateway_id}]}
-        system_state_response = await self.__request('post', 'api/portal/GetSystemStateList', json=payload)
-        _LOGGER.debug('Fetched system state: %s', system_state_response)
-        return system_state_response[0][GATEWAY_STATE][IS_ONLINE]
-
-
-    # api/portal/GetGuiDescriptionForGateway?GatewayId={gateway_id}&SystemId={system_id}
-    async def fetch_parameters(self, gateway_id, system_id) -> [Parameter]:
-        payload = {GATEWAY_ID: gateway_id, SYSTEM_ID: system_id}
-        desc = await self.__request('get', 'api/portal/GetGuiDescriptionForGateway', params=payload)
-        _LOGGER.debug('Fetched parameters: %s', desc)
-        tab_views = desc[MENU_ITEMS][0][TAB_VIEWS]
-        result = [WolfClient._map_view(view) for view in tab_views]
-
-        result.reverse()
-        distinct_ids = []
-        flattened = []
-        for sublist in result:
-            distinct_names = []
-            for val in sublist:
-                if val.value_id not in distinct_ids and val.name not in distinct_names:
-                    distinct_ids.append(val.value_id)
-                    distinct_names.append(val.name)
-                    flattened.append(val)
-        return flattened
-
-    # api/portal/CloseSystem
-    async def close_system(self):
-        data = {
-            SESSION_ID: self.session_id
-        }
-        res = await self.__request('post', 'api/portal/CloseSystem', json=data)
-        _LOGGER.debug('Close system response: %s', res)
-
-    # api/portal/GetParameterValues
-    async def fetch_value(self, gateway_id, system_id, parameters: [Parameter]):
-        data = {
-            BUNDLE_ID: 1000,
-            BUNDLE: False,
-            VALUE_ID_LIST: [param.value_id for param in parameters],
-            GATEWAY_ID: gateway_id,
-            SYSTEM_ID: system_id,
-            GUI_ID_CHANGED: False,
-            SESSION_ID: self.session_id,
-            LAST_ACCESS: self.last_access
-        }
-        res = await self.__request('post', 'api/portal/GetParameterValues', json=data,
-                                   headers={"Content-Type": "application/json"})
-
-        _LOGGER.debug('Fetched values: %s', res)
-
-        if ERROR_CODE in res or ERROR_TYPE in res:
-            if ERROR_MESSAGE in res and res[ERROR_MESSAGE] == ERROR_READ_PARAMETER:
-                raise ParameterReadError(res)
-            raise FetchFailed(res)
-
-        self.last_access = res[LAST_ACCESS]
-        return [Value(v[VALUE_ID], v[VALUE], v[STATE]) for v in res[VALUES] if VALUE in v]
-
-    @staticmethod
-    def _map_parameter(parameter: dict, parent: str) -> Parameter:
-        value_id = parameter[VALUE_ID]
-        name = parameter[NAME]
-        parameter_id = parameter[PARAMETER_ID]
-        if UNIT in parameter:
-            unit = parameter[UNIT]
-            if unit == CELSIUS_TEMPERATURE:
-                return Temperature(value_id, name, parent, parameter_id)
-            elif unit == BAR:
-                return Pressure(value_id, name, parent, parameter_id)
-            elif unit == PERCENTAGE:
-                return PercentageParameter(value_id, name, parent, parameter_id)
-            elif unit == HOUR:
-                return HoursParameter(value_id, name, parent, parameter_id)
-        elif LIST_ITEMS in parameter:
-            items = [ListItem(list_item[VALUE], list_item[DISPLAY_TEXT]) for list_item in parameter[LIST_ITEMS]]
-            return ListItemParameter(value_id, name, parent, items, parameter_id)
-        return SimpleParameter(value_id, name, parent, parameter_id)
-
-    @staticmethod
-    def _map_view(view: dict):
-        if 'SVGHeatingSchemaConfigDevices' in view:
-            units = dict([(unit['valueId'], unit['unit']) for unit
-                          in view['SVGHeatingSchemaConfigDevices'][0]['parameters'] if 'unit' in unit])
-
-            new_params = []
-            for param in view[PARAMETER_DESCRIPTORS]:
-                if param[VALUE_ID] in units:
-                    param[UNIT] = units[param[VALUE_ID]]
-                new_params.append(WolfClient._map_parameter(param, view[TAB_NAME]))
-            return new_params
-        else:
-            return [WolfClient._map_parameter(p, view[TAB_NAME]) for p in view[PARAMETER_DESCRIPTORS]]
-
-
-class FetchFailed(Exception):
-    """Server returned 500 code with message while executing query"""
-    pass
-
-class ParameterReadError(Exception):
-    """Server returned RedParameterValues error"""
-    pass
+import datetime
+from typing import Union
+
+import httpx
+import logging
+from httpx import Headers
+
+from wolf_comm.constants import BASE_URL_PORTAL, ID, GATEWAY_ID, NAME, SYSTEM_ID, MENU_ITEMS, TAB_VIEWS, BUNDLE_ID, \
+    BUNDLE, VALUE_ID_LIST, GUI_ID_CHANGED, SESSION_ID, VALUE_ID, VALUE, STATE, VALUES, PARAMETER_ID, UNIT, \
+    CELSIUS_TEMPERATURE, BAR, PERCENTAGE, LIST_ITEMS, DISPLAY_TEXT, PARAMETER_DESCRIPTORS, TAB_NAME, HOUR, \
+    LAST_ACCESS, ERROR_CODE, ERROR_TYPE, ERROR_MESSAGE, ERROR_READ_PARAMETER, SYSTEM_LIST, GATEWAY_STATE, IS_ONLINE
+from wolf_comm.create_session import create_session, update_session
+from wolf_comm.helpers import bearer_header
+from wolf_comm.models import Temperature, Parameter, SimpleParameter, Device, Pressure, ListItemParameter, \
+    PercentageParameter, Value, ListItem, HoursParameter
+from wolf_comm.token_auth import Tokens, TokenAuth
+
+_LOGGER = logging.getLogger(__name__)
+
+
+class WolfClient:
+    session_id: int or None
+    tokens: Tokens or None
+    last_access: datetime or None
+    last_failed: bool
+    
+    
+    @property
+    def client(self):
+        if hasattr(self, '_client') and self._client != None:
+            return self._client
+        elif hasattr(self, '_client_lambda') and self._client_lambda != None:
+            return self._client_lambda()
+        else:
+            raise RuntimeError("No valid client configuration")
+        
+
+    def __init__(self, username: str, password: str, client = None, client_lambda = None):
+        if client != None and client_lambda != None:
+            raise RuntimeError("Only one of client and client_lambda is allowed!")
+        elif client != None:
+            self._client = client
+        elif client_lambda != None:
+            self._client_lambda = client_lambda
+        else:
+            self._client = httpx.AsyncClient()
+        
+        self.tokens = None
+        self.token_auth = TokenAuth(username, password)
+        self.session_id = None
+        self.last_access = None
+        self.last_failed = False
+
+    async def __request(self, method: str, path: str, **kwargs) -> Union[dict, list]:
+        if self.tokens is None or self.tokens.is_expired():
+            await self.__authorize_and_session()
+
+        headers = kwargs.get('headers')
+
+        if headers is None:
+            headers = bearer_header(self.tokens.access_token)
+        else:
+            headers = {**bearer_header(self.tokens.access_token), **dict(headers)}
+
+        await update_session(self.client, self.tokens.access_token, self.session_id)
+        
+        resp = await self.__execute(headers, kwargs, method, path)
+        if resp.status_code == 401 or resp.status_code == 500:
+            _LOGGER.info('Retrying failed request (status code %d)',
+                         resp.status_code)
+            await self.__authorize_and_session()
+            headers = {**bearer_header(self.tokens.access_token), **dict(headers)}
+            try:
+                execution = await self.__execute(headers, kwargs, method, path)
+                return execution.json()
+            except FetchFailed as e:
+                self.last_failed = True
+                raise e
+        else:
+            self.last_failed = False
+            return resp.json()
+
+    async def __execute(self, headers, kwargs, method, path):
+        return await self.client.request(method, f"{BASE_URL_PORTAL}/{path}", **dict(kwargs, headers=Headers(headers)))
+
+    async def __authorize_and_session(self):
+        self.tokens = await self.token_auth.token(self.client)
+        self.session_id = await create_session(self.client, self.tokens.access_token)
+
+    # api/portal/GetSystemList
+    async def fetch_system_list(self) -> [Device]:
+        system_list = await self.__request('get', 'api/portal/GetSystemList')
+        _LOGGER.debug('Fetched systems: %s', system_list)
+        return [Device(system[ID], system[GATEWAY_ID], system[NAME]) for system in system_list]
+
+    # api/portal/GetSystemStateList
+    async def fetch_system_state_list(self, system_id, gateway_id) -> bool:
+        payload = {SESSION_ID: self.session_id, SYSTEM_LIST: [{SYSTEM_ID: system_id, GATEWAY_ID: gateway_id}]}
+        system_state_response = await self.__request('post', 'api/portal/GetSystemStateList', json=payload)
+        _LOGGER.debug('Fetched system state: %s', system_state_response)
+        return system_state_response[0][GATEWAY_STATE][IS_ONLINE]
+
+
+    # api/portal/GetGuiDescriptionForGateway?GatewayId={gateway_id}&SystemId={system_id}
+    async def fetch_parameters(self, gateway_id, system_id) -> [Parameter]:
+        payload = {GATEWAY_ID: gateway_id, SYSTEM_ID: system_id}
+        desc = await self.__request('get', 'api/portal/GetGuiDescriptionForGateway', params=payload)
+        _LOGGER.debug('Fetched parameters: %s', desc)
+        tab_views = desc[MENU_ITEMS][0][TAB_VIEWS]
+        result = [WolfClient._map_view(view) for view in tab_views]
+
+        result.reverse()
+        distinct_ids = []
+        flattened = []
+        for sublist in result:
+            distinct_names = []
+            for val in sublist:
+                if val.value_id not in distinct_ids and val.name not in distinct_names:
+                    distinct_ids.append(val.value_id)
+                    distinct_names.append(val.name)
+                    flattened.append(val)
+        return flattened
+
+    # api/portal/CloseSystem
+    async def close_system(self):
+        data = {
+            SESSION_ID: self.session_id
+        }
+        res = await self.__request('post', 'api/portal/CloseSystem', json=data)
+        _LOGGER.debug('Close system response: %s', res)
+
+    # api/portal/GetParameterValues
+    async def fetch_value(self, gateway_id, system_id, parameters: [Parameter]):
+        data = {
+            BUNDLE_ID: 1000,
+            BUNDLE: False,
+            VALUE_ID_LIST: [param.value_id for param in parameters],
+            GATEWAY_ID: gateway_id,
+            SYSTEM_ID: system_id,
+            GUI_ID_CHANGED: False,
+            SESSION_ID: self.session_id,
+            LAST_ACCESS: self.last_access
+        }
+        res = await self.__request('post', 'api/portal/GetParameterValues', json=data,
+                                   headers={"Content-Type": "application/json"})
+
+        _LOGGER.debug('Fetched values: %s', res)
+
+        if ERROR_CODE in res or ERROR_TYPE in res:
+            if ERROR_MESSAGE in res and res[ERROR_MESSAGE] == ERROR_READ_PARAMETER:
+                raise ParameterReadError(res)
+            raise FetchFailed(res)
+
+        self.last_access = res[LAST_ACCESS]
+        return [Value(v[VALUE_ID], v[VALUE], v[STATE]) for v in res[VALUES] if VALUE in v]
+
+    @staticmethod
+    def _map_parameter(parameter: dict, parent: str) -> Parameter:
+        value_id = parameter[VALUE_ID]
+        name = parameter[NAME]
+        parameter_id = parameter[PARAMETER_ID]
+        if UNIT in parameter:
+            unit = parameter[UNIT]
+            if unit == CELSIUS_TEMPERATURE:
+                return Temperature(value_id, name, parent, parameter_id)
+            elif unit == BAR:
+                return Pressure(value_id, name, parent, parameter_id)
+            elif unit == PERCENTAGE:
+                return PercentageParameter(value_id, name, parent, parameter_id)
+            elif unit == HOUR:
+                return HoursParameter(value_id, name, parent, parameter_id)
+        elif LIST_ITEMS in parameter:
+            items = [ListItem(list_item[VALUE], list_item[DISPLAY_TEXT]) for list_item in parameter[LIST_ITEMS]]
+            return ListItemParameter(value_id, name, parent, items, parameter_id)
+        return SimpleParameter(value_id, name, parent, parameter_id)
+
+    @staticmethod
+    def _map_view(view: dict):
+        if 'SVGHeatingSchemaConfigDevices' in view:
+            units = dict([(unit['valueId'], unit['unit']) for unit
+                          in view['SVGHeatingSchemaConfigDevices'][0]['parameters'] if 'unit' in unit])
+
+            new_params = []
+            for param in view[PARAMETER_DESCRIPTORS]:
+                if param[VALUE_ID] in units:
+                    param[UNIT] = units[param[VALUE_ID]]
+                new_params.append(WolfClient._map_parameter(param, view[TAB_NAME]))
+            return new_params
+        else:
+            return [WolfClient._map_parameter(p, view[TAB_NAME]) for p in view[PARAMETER_DESCRIPTORS]]
+
+
+class FetchFailed(Exception):
+    """Server returned 500 code with message while executing query"""
+    pass
+
+class ParameterReadError(Exception):
+    """Server returned RedParameterValues error"""
+    pass
```

