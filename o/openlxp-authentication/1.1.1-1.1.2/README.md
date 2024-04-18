# Comparing `tmp/openlxp-authentication-1.1.1.tar.gz` & `tmp/openlxp_authentication-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jametobin\Documents\ECC\openlxp-authentication\dist\tmpmzi_9mnk\openlxp-authentication-1.1.1.tar", last modified: Fri Jan 21 18:41:26 2022, max compression
+gzip compressed data, was "openlxp_authentication-1.1.2.tar", last modified: Thu Apr 18 18:13:05 2024, max compression
```

## Comparing `openlxp-authentication-1.1.1.tar` & `openlxp_authentication-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/
--rw-rw-rw-   0        0        0    11558 2021-10-29 19:13:46.000000 openlxp-authentication-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6411 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5416 2021-12-02 16:15:54.000000 openlxp-authentication-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication/
--rw-rw-rw-   0        0        0      207 2021-12-06 18:08:22.000000 openlxp-authentication-1.1.1/openlxp_authentication/admin.py
--rw-rw-rw-   0        0        0      250 2021-11-02 16:29:47.000000 openlxp-authentication-1.1.1/openlxp_authentication/apps.py
-drwxrwxrwx   0        0        0        0 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication/migrations/
--rw-rw-rw-   0        0        0      867 2021-11-02 16:29:47.000000 openlxp-authentication-1.1.1/openlxp_authentication/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2021-10-29 19:09:44.000000 openlxp-authentication-1.1.1/openlxp_authentication/migrations/__init__.py
--rw-rw-rw-   0        0        0     2423 2021-12-06 18:07:55.000000 openlxp-authentication-1.1.1/openlxp_authentication/models.py
--rw-rw-rw-   0        0        0      295 2021-12-06 18:07:25.000000 openlxp-authentication-1.1.1/openlxp_authentication/serializers.py
--rw-rw-rw-   0        0        0      250 2021-12-06 18:08:36.000000 openlxp-authentication-1.1.1/openlxp_authentication/urls.py
--rw-rw-rw-   0        0        0      527 2021-12-06 15:17:29.000000 openlxp-authentication-1.1.1/openlxp_authentication/views.py
-drwxrwxrwx   0        0        0        0 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication.egg-info/
--rw-rw-rw-   0        0        0     6411 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/openlxp_authentication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1148 2022-01-21 18:41:26.000000 openlxp-authentication-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      100 2021-10-29 19:09:44.000000 openlxp-authentication-1.1.1/setup.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.545068 openlxp_authentication-1.1.2/
+-rw-r--r--   0 jametobin   (502) staff       (20)    11357 2022-07-14 15:17:33.000000 openlxp_authentication-1.1.2/LICENSE
+-rw-r--r--   0 jametobin   (502) staff       (20)     6297 2024-04-18 18:13:05.544900 openlxp_authentication-1.1.2/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     5415 2022-07-14 15:24:15.000000 openlxp_authentication-1.1.2/README.md
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.537721 openlxp_authentication-1.1.2/openlxp_authentication/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-04-18 18:06:37.000000 openlxp_authentication-1.1.2/openlxp_authentication/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      199 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/admin.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      242 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/apps.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.543800 openlxp_authentication-1.1.2/openlxp_authentication/migrations/
+-rw-r--r--   0 jametobin   (502) staff       (20)      839 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/migrations/0001_initial.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2021-10-29 19:09:44.000000 openlxp_authentication-1.1.2/openlxp_authentication/migrations/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     2362 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/models.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      283 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/serializers.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      241 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/urls.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      512 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/views.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.544303 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/
+-rw-r--r--   0 jametobin   (502) staff       (20)     6297 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)      593 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       87 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/requires.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       28 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/top_level.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)     1110 2024-04-18 18:13:05.545574 openlxp_authentication-1.1.2/setup.cfg
+-rw-r--r--   0 jametobin   (502) staff       (20)       95 2022-07-14 15:17:33.000000 openlxp_authentication-1.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openlxp-authentication-1.1.1/LICENSE` & `openlxp_authentication-1.1.2/LICENSE`

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

### Comparing `openlxp-authentication-1.1.1/PKG-INFO` & `openlxp_authentication-1.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: openlxp-authentication
-Version: 1.1.1
-Summary: Installable OpenLXP Authentication that adds support for SAML
-Home-page: https://github.com/OpenLXP/openlxp-authentication/
-Author: OpenLXP
-Author-email: openlxphost@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django :: 3.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # OpenLXP-Authentication
 
 This is a Django package built on the social-auth-app-django package to allow additional authentication options for the OpenLXP project.
 
 Currently this package adds support for storing SAML configurations in the database used by Django, to allow for site administrators to set SAML configurations through the admin app.
 
 
@@ -128,28 +104,28 @@
     "givenName": "Support Guy",
     "emailAddress": "support@localhost.com",
 }
 ```
 
 #### USER_ATTRIBUTES
 
-The USER_ATTRIBUTES setting list the attributes of the User model that should be retreived from the IDP.
+The USER_ATTRIBUTES setting list the attributes of the User model that should be retrieved from the IDP.
 
 This setting is used to set the default value for the attribute map in the IDP configuration
 
 ```ini
 USER_ATTRIBUTES = ["user_permanent_id",
         "first_name",
         "last_name",
         "email"]
 ```
 
 #### AUTHENTICATION_BACKENDS
 
-The AUTHENTICATION_BACKENDS setting sets what authentication services should be avaliable.
+The AUTHENTICATION_BACKENDS setting sets what authentication services should be available.
 
 This setting must include `'openlxp_authentication.models.SAMLDBAuth'`, but others can included as desired.
 
 ```ini
 AUTHENTICATION_BACKENDS = (
     ...
     'django.contrib.auth.backends.ModelBackend',
@@ -172,15 +148,15 @@
 ```
 
 
 ### Optional Settings
 
 #### SESSION_EXPIRATION
 
-The SESSION_EXPIRATION setting has the Django session expiration match an experiation supplied by the IDP.
+The SESSION_EXPIRATION setting has the Django session expiration match an expiration supplied by the IDP.
 
 ```ini
 SESSION_EXPIRATION = True
 ```
 
 #### LOGIN_REDIRECT_URL
 
@@ -217,9 +193,7 @@
 #### SOCIAL_AUTH_STRATEGY
 
 The SOCIAL_AUTH_STRATEGY setting is required if using the OVERIDE_HOST setting.  OpenLXP-Authentication provides a strategy but custom solutions can be created and referenced in this setting.
 
 ```ini
 SOCIAL_AUTH_STRATEGY = 'openlxp_authentication.models.SAMLDBStrategy'
 ```
-
-
```

### Comparing `openlxp-authentication-1.1.1/openlxp_authentication/migrations/0001_initial.py` & `openlxp_authentication-1.1.2/openlxp_authentication/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Generated by Django 3.2.7 on 2021-10-25 13:44
-
-from ..models import SAMLConfiguration
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='SAMLConfiguration',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True,
-                 primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=50, unique=True)),
-                ('entity_id', models.CharField(max_length=300)),
-                ('url', models.URLField()),
-                ('cert', models.TextField()),
-                ('attribute_mapping', models.JSONField(
-                    default=SAMLConfiguration.attributes)),
-            ],
-        ),
-    ]
+# Generated by Django 3.2.7 on 2021-10-25 13:44
+
+from ..models import SAMLConfiguration
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='SAMLConfiguration',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True,
+                 primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=50, unique=True)),
+                ('entity_id', models.CharField(max_length=300)),
+                ('url', models.URLField()),
+                ('cert', models.TextField()),
+                ('attribute_mapping', models.JSONField(
+                    default=SAMLConfiguration.attributes)),
+            ],
+        ),
+    ]
```

### Comparing `openlxp-authentication-1.1.1/openlxp_authentication/models.py` & `openlxp_authentication-1.1.2/openlxp_authentication/models.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from django.conf import settings
-from django.db import models
-from django.db.models.base import Model
-from social_core.backends.saml import SAMLAuth, SAMLIdentityProvider
-from social_django.strategy import DjangoStrategy
-
-
-class SAMLConfiguration(Model):
-    """Model for storing SAML configurations in the database"""
-    name = models.CharField(unique=True, max_length=50)
-    entity_id = models.CharField(max_length=300)
-    url = models.URLField()
-    cert = models.TextField()
-
-    def attributes():
-        """Creates JSON dictionary mapping user attributes"""
-        return dict.fromkeys(["attr_" + attr for attr in settings.USER_ATTRIBUTES], '')
-    attribute_mapping = models.JSONField(default=attributes)
-
-    def endpoint(self):
-        """Returns the relative endpoint to trigger a login using this configuration"""
-        return f"/login/{SAMLDBAuth.name}/?idp=" + self.name
-
-
-class SAMLDBAuth(SAMLAuth):
-    """Authentication backend that uses SAML configurations from the database"""
-    name = 'samldb'
-
-    def get_idp(self, idp_name):
-        conf_name = idp_name.split(
-            '/')[-2] if idp_name.split('/')[-1] == '' else idp_name.split('/')[-1]
-        idp_config = SAMLConfiguration.objects.get(name=conf_name)
-        config_map = {"entity_id": idp_config.entity_id,
-                      "url": idp_config.url, "x509cert": idp_config.cert, **idp_config.attribute_mapping}
-        return SAMLIdentityProvider(conf_name, **config_map)
-
-
-class SAMLDBStrategy(DjangoStrategy):
-    """Strategy to use a custom hostname and port if provided"""
-
-    def build_absolute_uri(self, path=None):
-        baseurl = super().build_absolute_uri(path=path)
-        host = getattr(settings, 'OVERIDE_HOST', False)
-        replace = getattr(settings, 'BAD_HOST', False)
-        if(host != False and replace != False and not (baseurl is None)):
-            baseurl = baseurl.replace(replace, host, 1)
-        return baseurl
-
-    def request_host(self):
-        host = getattr(settings, 'OVERIDE_HOST', False)
-        if(host != False):
-            return '//'.join(host.split('//')[1:])
-        else:
-            return super().request_host()
-
-    def request_port(self):
-        port = getattr(settings, 'OVERIDE_HOST', False)
-        if(port != False):
-            return port.split(':')[-1]
-        else:
-            return super().request_port()
+from django.conf import settings
+from django.db import models
+from django.db.models.base import Model
+from social_core.backends.saml import SAMLAuth, SAMLIdentityProvider
+from social_django.strategy import DjangoStrategy
+
+
+class SAMLConfiguration(Model):
+    """Model for storing SAML configurations in the database"""
+    name = models.CharField(unique=True, max_length=50)
+    entity_id = models.CharField(max_length=300)
+    url = models.URLField()
+    cert = models.TextField()
+
+    def attributes():
+        """Creates JSON dictionary mapping user attributes"""
+        return dict.fromkeys(["attr_" + attr for attr in settings.USER_ATTRIBUTES], '')
+    attribute_mapping = models.JSONField(default=attributes)
+
+    def endpoint(self):
+        """Returns the relative endpoint to trigger a login using this configuration"""
+        return f"/login/{SAMLDBAuth.name}/?idp=" + self.name
+
+
+class SAMLDBAuth(SAMLAuth):
+    """Authentication backend that uses SAML configurations from the database"""
+    name = 'samldb'
+
+    def get_idp(self, idp_name):
+        conf_name = idp_name.split(
+            '/')[-2] if idp_name.split('/')[-1] == '' else idp_name.split('/')[-1]
+        idp_config = SAMLConfiguration.objects.get(name=conf_name)
+        config_map = {"entity_id": idp_config.entity_id,
+                      "url": idp_config.url, "x509cert": idp_config.cert, **idp_config.attribute_mapping}
+        return SAMLIdentityProvider(conf_name, **config_map)
+
+
+class SAMLDBStrategy(DjangoStrategy):
+    """Strategy to use a custom hostname and port if provided"""
+
+    def build_absolute_uri(self, path=None):
+        baseurl = super().build_absolute_uri(path=path)
+        host = getattr(settings, 'OVERIDE_HOST', False)
+        replace = getattr(settings, 'BAD_HOST', False)
+        if(host != False and replace != False and not (baseurl is None)):
+            baseurl = baseurl.replace(replace, host, 1)
+        return baseurl
+
+    def request_host(self):
+        host = getattr(settings, 'OVERIDE_HOST', False)
+        if(host != False):
+            return '//'.join(host.split('//')[1:])
+        else:
+            return super().request_host()
+
+    def request_port(self):
+        port = getattr(settings, 'OVERIDE_HOST', False)
+        if(port != False):
+            return port.split(':')[-1]
+        else:
+            return super().request_port()
```

### Comparing `openlxp-authentication-1.1.1/openlxp_authentication.egg-info/PKG-INFO` & `openlxp_authentication-1.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-Metadata-Version: 2.1
-Name: openlxp-authentication
-Version: 1.1.1
-Summary: Installable OpenLXP Authentication that adds support for SAML
-Home-page: https://github.com/OpenLXP/openlxp-authentication/
-Author: OpenLXP
-Author-email: openlxphost@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django :: 3.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# OpenLXP-Authentication
-
-This is a Django package built on the social-auth-app-django package to allow additional authentication options for the OpenLXP project.
-
-Currently this package adds support for storing SAML configurations in the database used by Django, to allow for site administrators to set SAML configurations through the admin app.
-
-
-## Setup
-
-To install this package install the dependencies from the requirements file (this should happen automatically if using pip) (make sure libxml2-dev libxmlsec1-dev are installed if running in Docker).
-
-Add the required settings to the Django settings file, social_django settings may also be used.
-
-Add the included URLs to Django (this will add the social_django URLs for you).
-
-```python
-urlpatterns = [
-    ...
-    url('', include('openlxp_authentication.urls')),
-]
-```
-
-Access the `/saml/metadata/` endpoint to view the configuration XML and verify it is correct (if AssertionConsumerService Location is incorrect, there are optional settings to fix it).
-
-Upload the XML to needed IDPs.
-
-Login to the admin module to add IDP configurations (the name setting will be used to identify which configuration to use).
-
-To test the login configuration: 
-
-1. Logout if you are already logged in
-
-1. Access `/login/samldb/?idp=nameFromConfig`
-
-1. You should be redirected to your chosen IDP
-
-1. Login with your IDP
-
-1. You will be returned to the application and sent to the REDIRECT_URL if set
-
-
-## Settings 
-
-
-### Required Settings
-
-#### JSONFIELD_ENABLED
-
-The JSONFIELD_ENABLED setting is required as it allows storing the attribute mapping as JSON in the database.
-
-```ini
-JSONFIELD_ENABLED = True
-```
-
-#### USER_MODEL
-
-The USER_MODEL setting sets what model should be used when authenticating a User.
-
-```ini
-USER_MODEL = 'core.XDSUser'
-```
-
-#### SP_ENTITY_ID
-
-The SP_ENTITY_ID setting sets Entity ID that IDPs should use for identifying the service.  This settings should be unique to your service.
-
-```ini
-SP_ENTITY_ID = 'http://localhost:8000'
-```
-
-#### SP_PUBLIC_CERT
-
-The SP_PUBLIC_CERT setting sets the public key to be used when authenticating users.
-
-```ini
-SP_PUBLIC_CERT = "******"
-```
-
-#### SP_PRIVATE_KEY
-
-The SP_PRIVATE_KEY setting sets the private key to be used when authenticating users.
-
-```ini
-SP_PRIVATE_KEY = "******"
-```
-
-#### Contact Info
-
-Contact information is set in three settings to provide to IDPs; ORG_INFO, TECHNICAL_CONTACT, and SUPPORT_CONTACT.
-
-```ini
-ORG_INFO = {
-    "en-US": {
-        "name": "example",
-        "displayname": "Example Inc.",
-        "url": "http://localhost",
-    }
-}
-TECHNICAL_CONTACT = {
-    "givenName": "Tech Gal",
-    "emailAddress": "technical@localhost.com"
-}
-SUPPORT_CONTACT = {
-    "givenName": "Support Guy",
-    "emailAddress": "support@localhost.com",
-}
-```
-
-#### USER_ATTRIBUTES
-
-The USER_ATTRIBUTES setting list the attributes of the User model that should be retreived from the IDP.
-
-This setting is used to set the default value for the attribute map in the IDP configuration
-
-```ini
-USER_ATTRIBUTES = ["user_permanent_id",
-        "first_name",
-        "last_name",
-        "email"]
-```
-
-#### AUTHENTICATION_BACKENDS
-
-The AUTHENTICATION_BACKENDS setting sets what authentication services should be avaliable.
-
-This setting must include `'openlxp_authentication.models.SAMLDBAuth'`, but others can included as desired.
-
-```ini
-AUTHENTICATION_BACKENDS = (
-    ...
-    'django.contrib.auth.backends.ModelBackend',
-    'openlxp_authentication.models.SAMLDBAuth',
-)
-```
-
-#### INSTALLED_APPS
-
-The INSTALLED_APPS setting sets what apps Django should load.
-
-Both social_django and openlxp_authentication must be added for this package to work correctly.
-
-```ini
-INSTALLED_APPS = [
-    ...
-    'social_django',
-    'openlxp_authentication',
-]
-```
-
-
-### Optional Settings
-
-#### SESSION_EXPIRATION
-
-The SESSION_EXPIRATION setting has the Django session expiration match an experiation supplied by the IDP.
-
-```ini
-SESSION_EXPIRATION = True
-```
-
-#### LOGIN_REDIRECT_URL
-
-The LOGIN_REDIRECT_URL setting is used by the application to redirect the user upon a successful login.
-
-```ini
-LOGIN_REDIRECT_URL = 'http://www.google.com'
-```
-
-#### OVERIDE_HOST
-
-The OVERIDE_HOST setting is used when Django is not able to accurately determine the host and port being used (this can occur in certain reverse proxy configurations).  
-
-The setting must follow the format `http://www.hostname.com:port`, `https://` may be used instead.
-
-If this setting is supplied, SOCIAL_AUTH_STRATEGY and BAD_HOST should also be set.
-
-```ini
-OVERIDE_HOST = 'http://localhost:8000'
-```
-
-#### BAD_HOST
-
-The BAD_HOST setting is used to remove part of the host and port string if the automatically detected configuration is incorrect.
-
-Similar to OVERIDE_HOST, this setting should also start with either `http://` or `https://`.
-
-The setting is required if using the OVERIDE_HOST setting.
-
-```ini
-BAD_HOST = 'http://localhost'
-```
-
-#### SOCIAL_AUTH_STRATEGY
-
-The SOCIAL_AUTH_STRATEGY setting is required if using the OVERIDE_HOST setting.  OpenLXP-Authentication provides a strategy but custom solutions can be created and referenced in this setting.
-
-```ini
-SOCIAL_AUTH_STRATEGY = 'openlxp_authentication.models.SAMLDBStrategy'
-```
-
-
+Metadata-Version: 2.1
+Name: openlxp-authentication
+Version: 1.1.2
+Summary: Installable OpenLXP Authentication that adds support for SAML
+Home-page: https://github.com/OpenLXP/openlxp-authentication/
+Author: OpenLXP
+Author-email: openlxphost@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django :: 3.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: social-auth-app-django>=5.0.0
+Requires-Dist: social-auth-core[all]>=4.1.0
+Requires-Dist: djangorestframework>=3.13.0
+
+# OpenLXP-Authentication
+
+This is a Django package built on the social-auth-app-django package to allow additional authentication options for the OpenLXP project.
+
+Currently this package adds support for storing SAML configurations in the database used by Django, to allow for site administrators to set SAML configurations through the admin app.
+
+
+## Setup
+
+To install this package install the dependencies from the requirements file (this should happen automatically if using pip) (make sure libxml2-dev libxmlsec1-dev are installed if running in Docker).
+
+Add the required settings to the Django settings file, social_django settings may also be used.
+
+Add the included URLs to Django (this will add the social_django URLs for you).
+
+```python
+urlpatterns = [
+    ...
+    url('', include('openlxp_authentication.urls')),
+]
+```
+
+Access the `/saml/metadata/` endpoint to view the configuration XML and verify it is correct (if AssertionConsumerService Location is incorrect, there are optional settings to fix it).
+
+Upload the XML to needed IDPs.
+
+Login to the admin module to add IDP configurations (the name setting will be used to identify which configuration to use).
+
+To test the login configuration: 
+
+1. Logout if you are already logged in
+
+1. Access `/login/samldb/?idp=nameFromConfig`
+
+1. You should be redirected to your chosen IDP
+
+1. Login with your IDP
+
+1. You will be returned to the application and sent to the REDIRECT_URL if set
+
+
+## Settings 
+
+
+### Required Settings
+
+#### JSONFIELD_ENABLED
+
+The JSONFIELD_ENABLED setting is required as it allows storing the attribute mapping as JSON in the database.
+
+```ini
+JSONFIELD_ENABLED = True
+```
+
+#### USER_MODEL
+
+The USER_MODEL setting sets what model should be used when authenticating a User.
+
+```ini
+USER_MODEL = 'core.XDSUser'
+```
+
+#### SP_ENTITY_ID
+
+The SP_ENTITY_ID setting sets Entity ID that IDPs should use for identifying the service.  This settings should be unique to your service.
+
+```ini
+SP_ENTITY_ID = 'http://localhost:8000'
+```
+
+#### SP_PUBLIC_CERT
+
+The SP_PUBLIC_CERT setting sets the public key to be used when authenticating users.
+
+```ini
+SP_PUBLIC_CERT = "******"
+```
+
+#### SP_PRIVATE_KEY
+
+The SP_PRIVATE_KEY setting sets the private key to be used when authenticating users.
+
+```ini
+SP_PRIVATE_KEY = "******"
+```
+
+#### Contact Info
+
+Contact information is set in three settings to provide to IDPs; ORG_INFO, TECHNICAL_CONTACT, and SUPPORT_CONTACT.
+
+```ini
+ORG_INFO = {
+    "en-US": {
+        "name": "example",
+        "displayname": "Example Inc.",
+        "url": "http://localhost",
+    }
+}
+TECHNICAL_CONTACT = {
+    "givenName": "Tech Gal",
+    "emailAddress": "technical@localhost.com"
+}
+SUPPORT_CONTACT = {
+    "givenName": "Support Guy",
+    "emailAddress": "support@localhost.com",
+}
+```
+
+#### USER_ATTRIBUTES
+
+The USER_ATTRIBUTES setting list the attributes of the User model that should be retrieved from the IDP.
+
+This setting is used to set the default value for the attribute map in the IDP configuration
+
+```ini
+USER_ATTRIBUTES = ["user_permanent_id",
+        "first_name",
+        "last_name",
+        "email"]
+```
+
+#### AUTHENTICATION_BACKENDS
+
+The AUTHENTICATION_BACKENDS setting sets what authentication services should be available.
+
+This setting must include `'openlxp_authentication.models.SAMLDBAuth'`, but others can included as desired.
+
+```ini
+AUTHENTICATION_BACKENDS = (
+    ...
+    'django.contrib.auth.backends.ModelBackend',
+    'openlxp_authentication.models.SAMLDBAuth',
+)
+```
+
+#### INSTALLED_APPS
+
+The INSTALLED_APPS setting sets what apps Django should load.
+
+Both social_django and openlxp_authentication must be added for this package to work correctly.
+
+```ini
+INSTALLED_APPS = [
+    ...
+    'social_django',
+    'openlxp_authentication',
+]
+```
+
+
+### Optional Settings
+
+#### SESSION_EXPIRATION
+
+The SESSION_EXPIRATION setting has the Django session expiration match an expiration supplied by the IDP.
+
+```ini
+SESSION_EXPIRATION = True
+```
+
+#### LOGIN_REDIRECT_URL
+
+The LOGIN_REDIRECT_URL setting is used by the application to redirect the user upon a successful login.
+
+```ini
+LOGIN_REDIRECT_URL = 'http://www.google.com'
+```
+
+#### OVERIDE_HOST
+
+The OVERIDE_HOST setting is used when Django is not able to accurately determine the host and port being used (this can occur in certain reverse proxy configurations).  
+
+The setting must follow the format `http://www.hostname.com:port`, `https://` may be used instead.
+
+If this setting is supplied, SOCIAL_AUTH_STRATEGY and BAD_HOST should also be set.
+
+```ini
+OVERIDE_HOST = 'http://localhost:8000'
+```
+
+#### BAD_HOST
+
+The BAD_HOST setting is used to remove part of the host and port string if the automatically detected configuration is incorrect.
+
+Similar to OVERIDE_HOST, this setting should also start with either `http://` or `https://`.
+
+The setting is required if using the OVERIDE_HOST setting.
+
+```ini
+BAD_HOST = 'http://localhost'
+```
+
+#### SOCIAL_AUTH_STRATEGY
+
+The SOCIAL_AUTH_STRATEGY setting is required if using the OVERIDE_HOST setting.  OpenLXP-Authentication provides a strategy but custom solutions can be created and referenced in this setting.
+
+```ini
+SOCIAL_AUTH_STRATEGY = 'openlxp_authentication.models.SAMLDBStrategy'
+```
```

### Comparing `openlxp-authentication-1.1.1/openlxp_authentication.egg-info/SOURCES.txt` & `openlxp_authentication-1.1.2/openlxp_authentication.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+openlxp_authentication/__init__.py
 openlxp_authentication/admin.py
 openlxp_authentication/apps.py
 openlxp_authentication/models.py
 openlxp_authentication/serializers.py
 openlxp_authentication/urls.py
 openlxp_authentication/views.py
 openlxp_authentication.egg-info/PKG-INFO
```

### Comparing `openlxp-authentication-1.1.1/setup.cfg` & `openlxp_authentication-1.1.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,70 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206f 7065 6e6c 7870 2d61 7574 6865   = openlxp-authe
-00000020: 6e74 6963 6174 696f 6e0d 0a76 6572 7369  ntication..versi
-00000030: 6f6e 203d 2031 2e31 2e31 0d0a 6465 7363  on = 1.1.1..desc
-00000040: 7269 7074 696f 6e20 3d20 496e 7374 616c  ription = Instal
-00000050: 6c61 626c 6520 4f70 656e 4c58 5020 4175  lable OpenLXP Au
-00000060: 7468 656e 7469 6361 7469 6f6e 2074 6861  thentication tha
-00000070: 7420 6164 6473 2073 7570 706f 7274 2066  t adds support f
-00000080: 6f72 2053 414d 4c0d 0a6c 6f6e 675f 6465  or SAML..long_de
-00000090: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-000000a0: 3a52 4541 444d 452e 6d64 0d0a 6c6f 6e67  :README.md..long
-000000b0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-000000c0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-000000d0: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
-000000e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000f0: 636f 6d2f 4f70 656e 4c58 502f 6f70 656e  com/OpenLXP/open
-00000100: 6c78 702d 6175 7468 656e 7469 6361 7469  lxp-authenticati
-00000110: 6f6e 2f0d 0a61 7574 686f 7220 3d20 4f70  on/..author = Op
-00000120: 656e 4c58 500d 0a61 7574 686f 725f 656d  enLXP..author_em
-00000130: 6169 6c20 3d20 6f70 656e 6c78 7068 6f73  ail = openlxphos
-00000140: 7440 676d 6169 6c2e 636f 6d0d 0a6c 6963  t@gmail.com..lic
-00000150: 656e 7365 203d 204d 4954 0d0a 636c 6173  ense = MIT..clas
-00000160: 7369 6669 6572 7320 3d20 0d0a 0944 6576  sifiers = ...Dev
-00000170: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000180: 3a3a 2034 202d 2042 6574 610d 0a09 456e  :: 4 - Beta...En
-00000190: 7669 726f 6e6d 656e 7420 3a3a 2057 6562  vironment :: Web
-000001a0: 2045 6e76 6972 6f6e 6d65 6e74 0d0a 0946   Environment...F
-000001b0: 7261 6d65 776f 726b 203a 3a20 446a 616e  ramework :: Djan
-000001c0: 676f 203a 3a20 332e 320d 0a09 496e 7465  go :: 3.2...Inte
-000001d0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000001e0: 2044 6576 656c 6f70 6572 730d 0a09 4c69   Developers...Li
-000001f0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000200: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000210: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
-00000220: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000230: 6465 7065 6e64 656e 740d 0a09 5072 6f67  dependent...Prog
-00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-00000260: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
-00000270: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000280: 3a20 5079 7468 6f6e 203a 3a20 332e 370d  : Python :: 3.7.
-00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002b0: 203a 3a20 496d 706c 656d 656e 7461 7469   :: Implementati
-000002c0: 6f6e 203a 3a20 4350 7974 686f 6e0d 0a09  on :: CPython...
-000002d0: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
-000002e0: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
-000002f0: 204c 6962 7261 7269 6573 203a 3a20 4170   Libraries :: Ap
-00000300: 706c 6963 6174 696f 6e20 4672 616d 6577  plication Framew
-00000310: 6f72 6b73 0d0a 0954 6f70 6963 203a 3a20  orks...Topic :: 
-00000320: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-00000330: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
-00000340: 7320 3a3a 2050 7974 686f 6e20 4d6f 6475  s :: Python Modu
-00000350: 6c65 730d 0a0d 0a5b 6f70 7469 6f6e 735d  les....[options]
-00000360: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000370: 655f 6461 7461 203d 2074 7275 650d 0a70  e_data = true..p
-00000380: 6163 6b61 6765 7320 3d20 6669 6e64 5f6e  ackages = find_n
-00000390: 616d 6573 7061 6365 3a0d 0a70 7974 686f  amespace:..pytho
-000003a0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000003b0: 2e37 0d0a 7365 7475 705f 7265 7175 6972  .7..setup_requir
-000003c0: 6573 203d 200d 0a09 7365 7475 7074 6f6f  es = ...setuptoo
-000003d0: 6c73 203e 3d20 3338 2e33 2e30 0d0a 696e  ls >= 38.3.0..in
-000003e0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000003f0: 200d 0a09 736f 6369 616c 2d61 7574 682d   ...social-auth-
-00000400: 6170 702d 646a 616e 676f 3e3d 352e 302e  app-django>=5.0.
-00000410: 300d 0a09 736f 6369 616c 2d61 7574 682d  0...social-auth-
-00000420: 636f 7265 5b61 6c6c 5d3e 3d34 2e31 2e30  core[all]>=4.1.0
-00000430: 0d0a 0964 6a61 6e67 6f72 6573 7466 7261  ...djangorestfra
-00000440: 6d65 776f 726b 3e3d 332e 3133 2e30 0d0a  mework>=3.13.0..
-00000450: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000460: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000470: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6f70 656e 6c78 702d 6175 7468 656e  = openlxp-authen
+00000020: 7469 6361 7469 6f6e 0a76 6572 7369 6f6e  tication.version
+00000030: 203d 2031 2e31 2e32 0a64 6573 6372 6970   = 1.1.2.descrip
+00000040: 7469 6f6e 203d 2049 6e73 7461 6c6c 6162  tion = Installab
+00000050: 6c65 204f 7065 6e4c 5850 2041 7574 6865  le OpenLXP Authe
+00000060: 6e74 6963 6174 696f 6e20 7468 6174 2061  ntication that a
+00000070: 6464 7320 7375 7070 6f72 7420 666f 7220  dds support for 
+00000080: 5341 4d4c 0a6c 6f6e 675f 6465 7363 7269  SAML.long_descri
+00000090: 7074 696f 6e20 3d20 6669 6c65 3a52 4541  ption = file:REA
+000000a0: 444d 452e 6d64 0a6c 6f6e 675f 6465 7363  DME.md.long_desc
+000000b0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+000000c0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+000000d0: 646f 776e 0a75 726c 203d 2068 7474 7073  down.url = https
+000000e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f70  ://github.com/Op
+000000f0: 656e 4c58 502f 6f70 656e 6c78 702d 6175  enLXP/openlxp-au
+00000100: 7468 656e 7469 6361 7469 6f6e 2f0a 6175  thentication/.au
+00000110: 7468 6f72 203d 204f 7065 6e4c 5850 0a61  thor = OpenLXP.a
+00000120: 7574 686f 725f 656d 6169 6c20 3d20 6f70  uthor_email = op
+00000130: 656e 6c78 7068 6f73 7440 676d 6169 6c2e  enlxphost@gmail.
+00000140: 636f 6d0a 6c69 6365 6e73 6520 3d20 4d49  com.license = MI
+00000150: 540a 636c 6173 7369 6669 6572 7320 3d20  T.classifiers = 
+00000160: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+00000170: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
+00000180: 0a09 456e 7669 726f 6e6d 656e 7420 3a3a  ..Environment ::
+00000190: 2057 6562 2045 6e76 6972 6f6e 6d65 6e74   Web Environment
+000001a0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
+000001b0: 6a61 6e67 6f20 3a3a 2033 2e32 0a09 496e  jango :: 3.2..In
+000001c0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+000001d0: 3a3a 2044 6576 656c 6f70 6572 730a 094c  :: Developers..L
+000001e0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001f0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000200: 6365 6e73 650a 094f 7065 7261 7469 6e67  cense..Operating
+00000210: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000220: 6465 7065 6e64 656e 740a 0950 726f 6772  dependent..Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
+00000250: 3a20 4f6e 6c79 0a09 5072 6f67 7261 6d6d  : Only..Programm
+00000260: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000270: 5079 7468 6f6e 203a 3a20 332e 370a 0950  Python :: 3.7..P
+00000280: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000290: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002a0: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
+000002b0: 3a3a 2043 5079 7468 6f6e 0a09 546f 7069  :: CPython..Topi
+000002c0: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+000002d0: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+000002e0: 7261 7269 6573 203a 3a20 4170 706c 6963  raries :: Applic
+000002f0: 6174 696f 6e20 4672 616d 6577 6f72 6b73  ation Frameworks
+00000300: 0a09 546f 7069 6320 3a3a 2053 6f66 7477  ..Topic :: Softw
+00000310: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
+00000320: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
+00000330: 5079 7468 6f6e 204d 6f64 756c 6573 0a0a  Python Modules..
+00000340: 5b6f 7074 696f 6e73 5d0a 696e 636c 7564  [options].includ
+00000350: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+00000360: 2074 7275 650a 7061 636b 6167 6573 203d   true.packages =
+00000370: 2066 696e 645f 6e61 6d65 7370 6163 653a   find_namespace:
+00000380: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000390: 203d 203e 3d33 2e37 0a73 6574 7570 5f72   = >=3.7.setup_r
+000003a0: 6571 7569 7265 7320 3d20 0a09 7365 7475  equires = ..setu
+000003b0: 7074 6f6f 6c73 203e 3d20 3338 2e33 2e30  ptools >= 38.3.0
+000003c0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000003d0: 7320 3d20 0a09 736f 6369 616c 2d61 7574  s = ..social-aut
+000003e0: 682d 6170 702d 646a 616e 676f 3e3d 352e  h-app-django>=5.
+000003f0: 302e 300a 0973 6f63 6961 6c2d 6175 7468  0.0..social-auth
+00000400: 2d63 6f72 655b 616c 6c5d 3e3d 342e 312e  -core[all]>=4.1.
+00000410: 300a 0964 6a61 6e67 6f72 6573 7466 7261  0..djangorestfra
+00000420: 6d65 776f 726b 3e3d 332e 3133 2e30 0a0a  mework>=3.13.0..
+00000430: 5b65 6767 5f69 6e66 6f5d 0a74 6167 5f62  [egg_info].tag_b
+00000440: 7569 6c64 203d 200a 7461 675f 6461 7465  uild = .tag_date
+00000450: 203d 2030 0a0a                            = 0..
```

