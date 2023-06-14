# Comparing `tmp/broadcast_service-1.3.1.tar.gz` & `tmp/broadcast_service-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broadcast_service-1.3.1.tar", last modified: Thu Jun  1 08:09:15 2023, max compression
+gzip compressed data, was "/home/runner/work/broadcast-service/broadcast-service/dist/.tmp-0ofyddo3/broadcast_service-2.0.0.tar", last modified: Wed Jun 14 11:25:45 2023, max compression
```

## Comparing `broadcast_service-1.3.1.tar` & `broadcast_service-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.362672 broadcast_service-1.3.1/
--rw-rw-rw-   0        0        0    11558 2022-11-21 04:35:58.000000 broadcast_service-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     4579 2023-06-01 08:09:15.361670 broadcast_service-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3712 2023-06-01 08:01:29.000000 broadcast_service-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.343673 broadcast_service-1.3.1/broadcast_service/
--rw-rw-rw-   0        0        0      666 2022-11-21 05:32:10.000000 broadcast_service-1.3.1/broadcast_service/__init__.py
--rw-rw-rw-   0        0        0     7676 2023-06-01 08:03:10.000000 broadcast_service-1.3.1/broadcast_service/_core.py
--rw-rw-rw-   0        0        0      656 2023-05-13 17:09:36.000000 broadcast_service-1.3.1/broadcast_service/singleton.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.352664 broadcast_service-1.3.1/broadcast_service.egg-info/
--rw-rw-rw-   0        0        0     4579 2023-06-01 08:09:14.000000 broadcast_service-1.3.1/broadcast_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-06-01 08:09:15.000000 broadcast_service-1.3.1/broadcast_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:09:14.000000 broadcast_service-1.3.1/broadcast_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-01 08:09:14.000000 broadcast_service-1.3.1/broadcast_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:09:15.362672 broadcast_service-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1800 2023-06-01 08:08:00.000000 broadcast_service-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.358663 broadcast_service-1.3.1/tests/
--rw-rw-rw-   0        0        0      642 2022-11-21 05:32:10.000000 broadcast_service-1.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-01-11 16:52:30.000000 broadcast_service-1.3.1/tests/test_async.py
--rw-rw-rw-   0        0        0     8106 2023-06-01 08:01:29.000000 broadcast_service-1.3.1/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14258 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/test_publisher_callback.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `broadcast_service-1.3.1/LICENSE` & `broadcast_service-2.0.0/LICENSE`

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

### Comparing `broadcast_service-1.3.1/PKG-INFO` & `broadcast_service-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,156 @@
-Metadata-Version: 2.1
-Name: broadcast_service
-Version: 1.3.1
-Summary: A lightweight third-party broadcast/pubsub library
-Home-page: https://github.com/Undertone0809/broadcast-service
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: broadcast,broadcast-service
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
-    broadcast-service
-</h1>
-<p align="center">
-  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
-</p>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
-    </a>
-   <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/stars/Undertone0809/broadcast-service.svg" alt="github stars"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
-   </a>
-</p>
-
-
-## Features
-- A publishing subscriber pattern can be built with a very simple syntax
-- Support different application scenarios, such as asynchronous and synchronous
-- Provide different syntax writing modes for lambda, callback functions, decorators, etc
-- A callback function listens on multiple subscriptions
-
-## Quick Start
-- [document github-pages](https://undertone0809.github.io/broadcast-service/#/)
-- [document gitee-pages](https://zeeland.gitee.io/broadcast-service/#/)
-- [https://pypi.org/project/broadcast-service/](https://pypi.org/project/broadcast-service/)
-
-## Setup
-```sh
-pip install broadcast-service
-```
-
-
-## Usage
-There is a easy demo to show how to use broadcast-service.
-```python
-from broadcast_service import broadcast_service
-
-
-# callback of common method
-def handle_msg(params):
-    print(f"handle_msg receive params: {params}")
-
-
-# callback of decorator
-@broadcast_service.on_listen(['my_topic'])
-def handle_decorator_msg(params):
-    print(f"handle_decorator_msg receive params: {params}")
-
-if __name__ == '__main__':
-    info = 'This is very important msg'
-
-    # subscribe topic
-    broadcast_service.subscribe('my_topic', handle_msg)
-
-    # publish broadcast
-    broadcast_service.publish('my_topic', info)
-```
-
-- You can use `publish, emit, broadcast` to send your topic msg and use `listen, on, subscribe` to listen your topic msg.
-
-- You can also add more arguments or no argument when you publish thr broadcast.
-```python
-from broadcast_service import broadcast_service
-
-# subscribe topic
-@broadcast_service.on_listen(['my_topic'])
-def handle_msg(info, info2):
-    print(info)
-    print(info2)
-
-if __name__ == '__main__':
-    info = 'This is very important msg'
-    info2 = 'This is also a very important msg.'
-
-    # publish broadcast
-    broadcast_service.publish('my_topic', info, info2)
-```
-```python
-from broadcast_service import broadcast_service
-
-# subscribe topic
-@broadcast_service.on_listen(['my_topic'])
-def handle_msg():
-    print('handle_msg callback')
-
-if __name__ == '__main__':
-    # publish broadcast
-    broadcast_service.publish('Test')
-```
-
-You can use decorator to subscirbe your
-
-Moreover, you can see more example in [document](https://undertone0809.github.io/broadcast-service/#/).
-
-## TODO
-- optimize documents and show more examples.
-- ~~optimize the syntax expression of broadcast-service~~
-- provide more test cases
-- privide the ability to subscribe the topic and callback once
-- Support for fuzzy subscriptions
-
-
-## Contribution
-If you want to contribute to this project, you can submit pr or issue. I am glad to see more people involved and optimize it.
+Metadata-Version: 2.1
+Name: broadcast_service
+Version: 2.0.0
+Summary: A lightweight third-party broadcast/pubsub library
+Home-page: https://github.com/Undertone0809/broadcast-service
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: broadcast,broadcast-service,publisher,subscriber,pubsub
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
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    broadcast-service
+</h1>
+<p align="center">
+  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
+</p>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
+    </a>
+   <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/stars/Undertone0809/broadcast-service.svg" alt="github stars"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
+   </a>
+</p>
+
+
+## Features
+- A publishing subscriber pattern can be built with a very simple syntax
+- Support different application scenarios, such as asynchronous and synchronous
+- Provide different syntax writing modes for lambda, callback functions, decorators, etc
+- A callback function listens on multiple subscriptions
+- Provide publisher dispatch callback manage
+
+## Quick Start
+- [document github-pages](https://undertone0809.github.io/broadcast-service/#/)
+- [document gitee-pages](https://zeeland.gitee.io/broadcast-service/#/)
+- [https://pypi.org/project/broadcast-service/](https://pypi.org/project/broadcast-service/)
+
+## Setup
+
+```sh
+pip install broadcast-service
+```
+
+## Usage
+There is an easy demo to show how to use broadcast-service.
+
+```python
+from broadcast_service import broadcast_service
+
+# callback of decorator
+@broadcast_service.on_listen('my_topic')
+def handle_decorator_msg(params):
+    print(f"handle_decorator_msg receive params: {params}")
+
+if __name__ == '__main__':
+    info = 'This is very important msg'
+
+    # publish broadcast
+    broadcast_service.publish('my_topic', info)
+```
+
+- You can use `publish, emit, broadcast` to send your topic msg and use `listen, on, subscribe` to listen your topic msg.
+
+- You can also add more arguments or no argument when you publish thr broadcast.
+
+```python
+from broadcast_service import broadcast_service
+
+# subscribe topic
+@broadcast_service.on_listen(['my_topic'])
+def handle_msg(info, info2):
+    print(info)
+    print(info2)
+
+if __name__ == '__main__':
+    info = 'This is very important msg'
+    info2 = 'This is also a very important msg.'
+
+    # publish broadcast
+    broadcast_service.publish('my_topic', info, info2)
+```
+```python
+from broadcast_service import broadcast_service
+
+# subscribe topic
+@broadcast_service.on_listen(['my_topic'])
+def handle_msg():
+    print('handle_msg callback')
+
+if __name__ == '__main__':
+    # publish broadcast
+    broadcast_service.publish('Test')
+```
+
+You can use `config` to make publisher callback If you want.
+
+```python
+from broadcast_service import broadcast_service
+
+
+@broadcast_service.on_listen("topic")
+def handle_subscriber_callback():
+    print("handle_subscriber_callback")
+
+
+def handle_publisher_callback(*args):
+    print("handle_publisher_callback")
+
+
+if __name__ == '__main__':
+    broadcast_service.config(
+        num_of_executions=5,
+        callback=handle_publisher_callback,
+        enable_final_return=True,
+        interval=0.1
+    ).publish("topic")
+
+```
+
+Moreover, you can see more example in [document](https://undertone0809.github.io/broadcast-service/#/).
+
+## TODO
+- optimize documents and show more examples.
+- ~~optimize the syntax expression of broadcast-service~~
+- provide more test cases
+- provide the ability to subscribe the topic and callback once
+- support for fuzzy subscriptions
+- ~~the publisher of the topic can provide a return value~~
+- optimize usage in class ('self' params problem)
+- build observer mode
+- ~~provide publisher callback when all subscriber have completed callback~~
+
+
+## Contribution
+If you want to contribute to this project, you can submit pr or issue. I am glad to see more people involved and optimize it.
```

### Comparing `broadcast_service-1.3.1/README.md` & `broadcast_service-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,133 @@
-<h1 align="center">
-    broadcast-service
-</h1>
-<p align="center">
-  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
-</p>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
-    </a>
-   <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/stars/Undertone0809/broadcast-service.svg" alt="github stars"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
-   </a>
-</p>
-
-
-## Features
-- A publishing subscriber pattern can be built with a very simple syntax
-- Support different application scenarios, such as asynchronous and synchronous
-- Provide different syntax writing modes for lambda, callback functions, decorators, etc
-- A callback function listens on multiple subscriptions
-
-## Quick Start
-- [document github-pages](https://undertone0809.github.io/broadcast-service/#/)
-- [document gitee-pages](https://zeeland.gitee.io/broadcast-service/#/)
-- [https://pypi.org/project/broadcast-service/](https://pypi.org/project/broadcast-service/)
-
-## Setup
-```sh
-pip install broadcast-service
-```
-
-
-## Usage
-There is a easy demo to show how to use broadcast-service.
-```python
-from broadcast_service import broadcast_service
-
-
-# callback of common method
-def handle_msg(params):
-    print(f"handle_msg receive params: {params}")
-
-
-# callback of decorator
-@broadcast_service.on_listen(['my_topic'])
-def handle_decorator_msg(params):
-    print(f"handle_decorator_msg receive params: {params}")
-
-if __name__ == '__main__':
-    info = 'This is very important msg'
-
-    # subscribe topic
-    broadcast_service.subscribe('my_topic', handle_msg)
-
-    # publish broadcast
-    broadcast_service.publish('my_topic', info)
-```
-
-- You can use `publish, emit, broadcast` to send your topic msg and use `listen, on, subscribe` to listen your topic msg.
-
-- You can also add more arguments or no argument when you publish thr broadcast.
-```python
-from broadcast_service import broadcast_service
-
-# subscribe topic
-@broadcast_service.on_listen(['my_topic'])
-def handle_msg(info, info2):
-    print(info)
-    print(info2)
-
-if __name__ == '__main__':
-    info = 'This is very important msg'
-    info2 = 'This is also a very important msg.'
-
-    # publish broadcast
-    broadcast_service.publish('my_topic', info, info2)
-```
-```python
-from broadcast_service import broadcast_service
-
-# subscribe topic
-@broadcast_service.on_listen(['my_topic'])
-def handle_msg():
-    print('handle_msg callback')
-
-if __name__ == '__main__':
-    # publish broadcast
-    broadcast_service.publish('Test')
-```
-
-You can use decorator to subscirbe your
-
-Moreover, you can see more example in [document](https://undertone0809.github.io/broadcast-service/#/).
-
-## TODO
-- optimize documents and show more examples.
-- ~~optimize the syntax expression of broadcast-service~~
-- provide more test cases
-- privide the ability to subscribe the topic and callback once
-- Support for fuzzy subscriptions
-
-
-## Contribution
-If you want to contribute to this project, you can submit pr or issue. I am glad to see more people involved and optimize it.
+<h1 align="center">
+    broadcast-service
+</h1>
+<p align="center">
+  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
+</p>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
+    </a>
+   <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/stars/Undertone0809/broadcast-service.svg" alt="github stars"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
+   </a>
+</p>
+
+
+## Features
+- A publishing subscriber pattern can be built with a very simple syntax
+- Support different application scenarios, such as asynchronous and synchronous
+- Provide different syntax writing modes for lambda, callback functions, decorators, etc
+- A callback function listens on multiple subscriptions
+- Provide publisher dispatch callback manage
+
+## Quick Start
+- [document github-pages](https://undertone0809.github.io/broadcast-service/#/)
+- [document gitee-pages](https://zeeland.gitee.io/broadcast-service/#/)
+- [https://pypi.org/project/broadcast-service/](https://pypi.org/project/broadcast-service/)
+
+## Setup
+
+```sh
+pip install broadcast-service
+```
+
+## Usage
+There is an easy demo to show how to use broadcast-service.
+
+```python
+from broadcast_service import broadcast_service
+
+# callback of decorator
+@broadcast_service.on_listen('my_topic')
+def handle_decorator_msg(params):
+    print(f"handle_decorator_msg receive params: {params}")
+
+if __name__ == '__main__':
+    info = 'This is very important msg'
+
+    # publish broadcast
+    broadcast_service.publish('my_topic', info)
+```
+
+- You can use `publish, emit, broadcast` to send your topic msg and use `listen, on, subscribe` to listen your topic msg.
+
+- You can also add more arguments or no argument when you publish thr broadcast.
+
+```python
+from broadcast_service import broadcast_service
+
+# subscribe topic
+@broadcast_service.on_listen(['my_topic'])
+def handle_msg(info, info2):
+    print(info)
+    print(info2)
+
+if __name__ == '__main__':
+    info = 'This is very important msg'
+    info2 = 'This is also a very important msg.'
+
+    # publish broadcast
+    broadcast_service.publish('my_topic', info, info2)
+```
+```python
+from broadcast_service import broadcast_service
+
+# subscribe topic
+@broadcast_service.on_listen(['my_topic'])
+def handle_msg():
+    print('handle_msg callback')
+
+if __name__ == '__main__':
+    # publish broadcast
+    broadcast_service.publish('Test')
+```
+
+You can use `config` to make publisher callback If you want.
+
+```python
+from broadcast_service import broadcast_service
+
+
+@broadcast_service.on_listen("topic")
+def handle_subscriber_callback():
+    print("handle_subscriber_callback")
+
+
+def handle_publisher_callback(*args):
+    print("handle_publisher_callback")
+
+
+if __name__ == '__main__':
+    broadcast_service.config(
+        num_of_executions=5,
+        callback=handle_publisher_callback,
+        enable_final_return=True,
+        interval=0.1
+    ).publish("topic")
+
+```
+
+Moreover, you can see more example in [document](https://undertone0809.github.io/broadcast-service/#/).
+
+## TODO
+- optimize documents and show more examples.
+- ~~optimize the syntax expression of broadcast-service~~
+- provide more test cases
+- provide the ability to subscribe the topic and callback once
+- support for fuzzy subscriptions
+- ~~the publisher of the topic can provide a return value~~
+- optimize usage in class ('self' params problem)
+- build observer mode
+- ~~provide publisher callback when all subscriber have completed callback~~
+
+
+## Contribution
+If you want to contribute to this project, you can submit pr or issue. I am glad to see more people involved and optimize it.
```

### Comparing `broadcast_service-1.3.1/broadcast_service/__init__.py` & `broadcast_service-2.0.0/tests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
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
-from ._core import *
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
```

### Comparing `broadcast_service-1.3.1/broadcast_service/singleton.py` & `broadcast_service-2.0.0/broadcast_service/singleton.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""The singleton metaclass for ensuring only one instance of a class."""
-import abc
-
-
-class Singleton(abc.ABCMeta, type):
-    """
-    Singleton metaclass for ensuring only one instance of a class.
-    """
-
-    _instances = {}
-
-    def __call__(cls, *args, **kwargs):
-        """Call method for the singleton metaclass."""
-        if cls not in cls._instances:
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
-        return cls._instances[cls]
-
-
-class AbstractSingleton(abc.ABC, metaclass=Singleton):
-    """
-    Abstract singleton class for ensuring only one instance of a class.
-    """
-
-    pass
+"""The singleton metaclass for ensuring only one instance of a class."""
+import abc
+
+
+class Singleton(abc.ABCMeta, type):
+    """
+    Singleton metaclass for ensuring only one instance of a class.
+    """
+
+    _instances = {}
+
+    def __call__(cls, *args, **kwargs):
+        """Call method for the singleton metaclass."""
+        if cls not in cls._instances:
+            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
+        return cls._instances[cls]
+
+
+class AbstractSingleton(abc.ABC, metaclass=Singleton):
+    """
+    Abstract singleton class for ensuring only one instance of a class.
+    """
+
+    pass
```

### Comparing `broadcast_service-1.3.1/broadcast_service.egg-info/PKG-INFO` & `broadcast_service-2.0.0/broadcast_service.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,156 @@
-Metadata-Version: 2.1
-Name: broadcast-service
-Version: 1.3.1
-Summary: A lightweight third-party broadcast/pubsub library
-Home-page: https://github.com/Undertone0809/broadcast-service
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: broadcast,broadcast-service
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
-    broadcast-service
-</h1>
-<p align="center">
-  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
-</p>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
-    </a>
-   <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/stars/Undertone0809/broadcast-service.svg" alt="github stars"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
-   </a>
-</p>
-
-
-## Features
-- A publishing subscriber pattern can be built with a very simple syntax
-- Support different application scenarios, such as asynchronous and synchronous
-- Provide different syntax writing modes for lambda, callback functions, decorators, etc
-- A callback function listens on multiple subscriptions
-
-## Quick Start
-- [document github-pages](https://undertone0809.github.io/broadcast-service/#/)
-- [document gitee-pages](https://zeeland.gitee.io/broadcast-service/#/)
-- [https://pypi.org/project/broadcast-service/](https://pypi.org/project/broadcast-service/)
-
-## Setup
-```sh
-pip install broadcast-service
-```
-
-
-## Usage
-There is a easy demo to show how to use broadcast-service.
-```python
-from broadcast_service import broadcast_service
-
-
-# callback of common method
-def handle_msg(params):
-    print(f"handle_msg receive params: {params}")
-
-
-# callback of decorator
-@broadcast_service.on_listen(['my_topic'])
-def handle_decorator_msg(params):
-    print(f"handle_decorator_msg receive params: {params}")
-
-if __name__ == '__main__':
-    info = 'This is very important msg'
-
-    # subscribe topic
-    broadcast_service.subscribe('my_topic', handle_msg)
-
-    # publish broadcast
-    broadcast_service.publish('my_topic', info)
-```
-
-- You can use `publish, emit, broadcast` to send your topic msg and use `listen, on, subscribe` to listen your topic msg.
-
-- You can also add more arguments or no argument when you publish thr broadcast.
-```python
-from broadcast_service import broadcast_service
-
-# subscribe topic
-@broadcast_service.on_listen(['my_topic'])
-def handle_msg(info, info2):
-    print(info)
-    print(info2)
-
-if __name__ == '__main__':
-    info = 'This is very important msg'
-    info2 = 'This is also a very important msg.'
-
-    # publish broadcast
-    broadcast_service.publish('my_topic', info, info2)
-```
-```python
-from broadcast_service import broadcast_service
-
-# subscribe topic
-@broadcast_service.on_listen(['my_topic'])
-def handle_msg():
-    print('handle_msg callback')
-
-if __name__ == '__main__':
-    # publish broadcast
-    broadcast_service.publish('Test')
-```
-
-You can use decorator to subscirbe your
-
-Moreover, you can see more example in [document](https://undertone0809.github.io/broadcast-service/#/).
-
-## TODO
-- optimize documents and show more examples.
-- ~~optimize the syntax expression of broadcast-service~~
-- provide more test cases
-- privide the ability to subscribe the topic and callback once
-- Support for fuzzy subscriptions
-
-
-## Contribution
-If you want to contribute to this project, you can submit pr or issue. I am glad to see more people involved and optimize it.
+Metadata-Version: 2.1
+Name: broadcast-service
+Version: 2.0.0
+Summary: A lightweight third-party broadcast/pubsub library
+Home-page: https://github.com/Undertone0809/broadcast-service
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: broadcast,broadcast-service,publisher,subscriber,pubsub
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
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    broadcast-service
+</h1>
+<p align="center">
+  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
+</p>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
+    </a>
+   <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/stars/Undertone0809/broadcast-service.svg" alt="github stars"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
+   </a>
+</p>
+
+
+## Features
+- A publishing subscriber pattern can be built with a very simple syntax
+- Support different application scenarios, such as asynchronous and synchronous
+- Provide different syntax writing modes for lambda, callback functions, decorators, etc
+- A callback function listens on multiple subscriptions
+- Provide publisher dispatch callback manage
+
+## Quick Start
+- [document github-pages](https://undertone0809.github.io/broadcast-service/#/)
+- [document gitee-pages](https://zeeland.gitee.io/broadcast-service/#/)
+- [https://pypi.org/project/broadcast-service/](https://pypi.org/project/broadcast-service/)
+
+## Setup
+
+```sh
+pip install broadcast-service
+```
+
+## Usage
+There is an easy demo to show how to use broadcast-service.
+
+```python
+from broadcast_service import broadcast_service
+
+# callback of decorator
+@broadcast_service.on_listen('my_topic')
+def handle_decorator_msg(params):
+    print(f"handle_decorator_msg receive params: {params}")
+
+if __name__ == '__main__':
+    info = 'This is very important msg'
+
+    # publish broadcast
+    broadcast_service.publish('my_topic', info)
+```
+
+- You can use `publish, emit, broadcast` to send your topic msg and use `listen, on, subscribe` to listen your topic msg.
+
+- You can also add more arguments or no argument when you publish thr broadcast.
+
+```python
+from broadcast_service import broadcast_service
+
+# subscribe topic
+@broadcast_service.on_listen(['my_topic'])
+def handle_msg(info, info2):
+    print(info)
+    print(info2)
+
+if __name__ == '__main__':
+    info = 'This is very important msg'
+    info2 = 'This is also a very important msg.'
+
+    # publish broadcast
+    broadcast_service.publish('my_topic', info, info2)
+```
+```python
+from broadcast_service import broadcast_service
+
+# subscribe topic
+@broadcast_service.on_listen(['my_topic'])
+def handle_msg():
+    print('handle_msg callback')
+
+if __name__ == '__main__':
+    # publish broadcast
+    broadcast_service.publish('Test')
+```
+
+You can use `config` to make publisher callback If you want.
+
+```python
+from broadcast_service import broadcast_service
+
+
+@broadcast_service.on_listen("topic")
+def handle_subscriber_callback():
+    print("handle_subscriber_callback")
+
+
+def handle_publisher_callback(*args):
+    print("handle_publisher_callback")
+
+
+if __name__ == '__main__':
+    broadcast_service.config(
+        num_of_executions=5,
+        callback=handle_publisher_callback,
+        enable_final_return=True,
+        interval=0.1
+    ).publish("topic")
+
+```
+
+Moreover, you can see more example in [document](https://undertone0809.github.io/broadcast-service/#/).
+
+## TODO
+- optimize documents and show more examples.
+- ~~optimize the syntax expression of broadcast-service~~
+- provide more test cases
+- provide the ability to subscribe the topic and callback once
+- support for fuzzy subscriptions
+- ~~the publisher of the topic can provide a return value~~
+- optimize usage in class ('self' params problem)
+- build observer mode
+- ~~provide publisher callback when all subscriber have completed callback~~
+
+
+## Contribution
+If you want to contribute to this project, you can submit pr or issue. I am glad to see more people involved and optimize it.
```

### Comparing `broadcast_service-1.3.1/tests/test_base.py` & `broadcast_service-2.0.0/tests/test_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,201 +1,214 @@
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
-import time
-from unittest import TestCase
-from broadcast_service import broadcast_service, enable_log
-
-enable_log()
-
-
-def wait(seconds=0.1):
-    time.sleep(seconds)
-
-
-class TestBroadcast(TestCase):
-    def test_listen_of_common(self):
-        self.test_listen_of_common_no_params = False
-        self.test_listen_of_common_specify_params = False
-        self.test_listen_multi_topic1_of_common = False
-        self.test_listen_multi_topic2_of_common = False
-        self.counter = 0
-        self.all_counter = 0
-
-        def handle_topic_no_params():
-            self.test_listen_of_common_no_params = True
-
-        def handle_topic_specify_params(a, b, c):
-            self.assertEqual(11, a)
-            self.assertEqual(22, b)
-            self.assertEqual(33, c)
-            self.test_listen_of_common_specify_params = True
-
-        def handle_multi_topics(*args, **kwargs):
-            self.counter += 1
-            if args[0] == 111:
-                self.test_listen_multi_topic1_of_common = True
-            if args[0] == 222:
-                self.test_listen_multi_topic2_of_common = True
-
-        def handle_all_topics(*args, **kwargs):
-            self.all_counter += 1
-
-        # test all topics
-        broadcast_service.subscribe_all(handle_all_topics)
-
-        # test listen of common no params
-        broadcast_service.subscribe(
-            "test_listen_of_common_no_params", handle_topic_no_params)
-        broadcast_service.publish("test_listen_of_common_no_params")
-        wait()
-        self.assertTrue(self.test_listen_of_common_no_params)
-
-        # test listen of common specify params
-        broadcast_service.subscribe(
-            "test_listen_of_common_specify_params", handle_topic_specify_params)
-        broadcast_service.publish(
-            "test_listen_of_common_specify_params", 11, 22, 33)
-        wait()
-        self.assertTrue(self.test_listen_of_common_specify_params)
-
-        # test listen multi topics of common
-        topics = ['test_listen_multi_topic1_of_common', 'test_listen_multi_topic2_of_common']
-        broadcast_service.subscribe(topics, handle_multi_topics)
-        broadcast_service.publish("test_listen_multi_topic1_of_common", 111)
-        broadcast_service.publish("test_listen_multi_topic2_of_common", 222)
-        wait()
-        self.assertTrue(self.test_listen_multi_topic1_of_common)
-        self.assertTrue(self.test_listen_multi_topic2_of_common)
-        self.assertEqual(2, self.counter)
-
-        self.assertEqual(4, self.all_counter)
-
-    def test_listen_of_decorator(self):
-        self.test_listen_of_decorator_no_params1 = False
-        self.test_listen_of_decorator_no_params2 = False
-        self.test_listen_of_decorator_multi_params = False
-        self.test_listen_of_decorator_specify_params = False
-        self.test_listen_of_decorator_listen_all = False
-        self.counter = 0
-
-        @broadcast_service.on_listen("test_listen_of_decorator_no_params1")
-        def handle_topic_no_params():
-            self.test_listen_of_decorator_no_params1 = True
-
-        @broadcast_service.on_listen(["test_listen_of_decorator_no_params2"])
-        def handle_topic_no_params():
-            self.test_listen_of_decorator_no_params2 = True
-
-        @broadcast_service.on_listen(["test_listen_of_decorator_no_params1", "test_listen_of_decorator_no_params2"])
-        def handle_topic_no_params():
-            if self.test_listen_of_decorator_no_params1 and self.test_listen_of_decorator_no_params2:
-                self.test_listen_of_decorator_multi_params = True
-
-        @broadcast_service.on_listen(["test_listen_of_decorator_specify_params"])
-        def handle_topic_specify_params(a, b, c):
-            self.assertEqual(11, a)
-            self.assertEqual(22, b)
-            self.assertEqual(33, c)
-            self.test_listen_of_decorator_specify_params = True
-
-        @broadcast_service.on_listen()
-        def handle_listen_all_topics(*args, **kwargs):
-            self.counter += 1
-            self.test_listen_of_decorator_listen_all = True
-
-        broadcast_service.publish("test_listen_of_decorator_no_params1")
-        wait()
-        self.assertTrue(self.test_listen_of_decorator_no_params1)
-
-        broadcast_service.publish("test_listen_of_decorator_no_params2")
-        wait()
-        self.assertTrue(self.test_listen_of_decorator_no_params2)
-
-        wait()
-        self.assertTrue(self.test_listen_of_decorator_multi_params)
-
-        broadcast_service.publish(
-            "test_listen_of_decorator_specify_params", 11, 22, 33)
-        wait()
-        self.assertTrue(self.test_listen_of_decorator_specify_params)
-
-        broadcast_service.publish("test_listen_of_decorator_listen_all")
-        wait()
-        self.assertTrue(self.test_listen_of_decorator_listen_all)
-        self.assertEqual(4, self.counter)
-
-    def test_listen_of_lambda(self):
-        self.test_listen_of_lambda_no_params = False
-        self.test_listen_of_lambda_specify_params = False
-
-        def handle_topic_no_params():
-            self.test_listen_of_lambda_no_params = True
-
-        def handle_topic_specify_params(params: bool):
-            self.test_listen_of_lambda_specify_params = params
-
-        broadcast_service.subscribe(
-            "test_listen_of_lambda_no_params", lambda: handle_topic_no_params())
-        broadcast_service.publish("test_listen_of_lambda_no_params")
-        wait()
-        self.assertTrue(self.test_listen_of_lambda_no_params)
-
-        broadcast_service.subscribe(
-            "test_listen_of_lambda_specify_params", lambda: handle_topic_specify_params(True))
-        broadcast_service.publish("test_listen_of_lambda_specify_params")
-        wait()
-        self.assertTrue(self.test_listen_of_lambda_no_params)
-
-    def test_broadcast(self):
-        self.test_broadcast_one_topic1 = False
-        self.test_broadcast_one_topic2 = False
-        self.test_broadcast_multi_topic1 = False
-        self.test_broadcast_multi_topic2 = False
-        self.counter = 0
-
-        @broadcast_service.on_listen("test_broadcast_one_topic1")
-        def handle_one_topic1():
-            self.counter += 1
-            self.test_broadcast_one_topic1 = True
-
-        @broadcast_service.on_listen("test_broadcast_one_topic2")
-        def handle_one_topic2():
-            self.counter += 1
-            self.test_broadcast_one_topic2 = True
-
-        @broadcast_service.on_listen("test_broadcast_multi_topic1")
-        def handle_multi_topic1():
-            self.counter += 1
-            self.test_broadcast_multi_topic1 = True
-
-        @broadcast_service.on_listen("test_broadcast_multi_topic2")
-        def handle_multi_topic2():
-            self.counter += 1
-            self.test_broadcast_multi_topic2 = True
-
-        broadcast_service.publish("test_broadcast_one_topic1")
-        wait()
-        self.assertTrue(self.test_broadcast_one_topic1)
-
-        broadcast_service.publish(["test_broadcast_one_topic2"])
-        wait()
-        self.assertTrue(self.test_broadcast_one_topic2)
-
-        broadcast_service.publish(["test_broadcast_multi_topic1", "test_broadcast_multi_topic2"])
-        wait()
-        self.assertTrue(self.test_broadcast_multi_topic1 and self.test_broadcast_multi_topic2)
-
-        broadcast_service.publish_all()
-        wait()
-        self.assertEqual(8, self.counter)
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
+import time
+from unittest import TestCase
+from broadcast_service import broadcast_service
+from broadcast_service.logger import get_logger, enable_log
+
+logger = get_logger()
+
+
+def wait(seconds=0.1):
+    time.sleep(seconds)
+
+
+class TestBroadcast(TestCase):
+    def test_listen_of_common(self):
+        self.test_listen_of_common_no_params = False
+        self.test_listen_of_common_specify_params = False
+        self.test_listen_multi_topic1_of_common = False
+        self.test_listen_multi_topic2_of_common = False
+        self.counter = 0
+        self.all_counter = 0
+
+        def handle_topic_no_params():
+            self.test_listen_of_common_no_params = True
+
+        def handle_topic_specify_params(a, b, c):
+            self.assertEqual(11, a)
+            self.assertEqual(22, b)
+            self.assertEqual(33, c)
+            self.test_listen_of_common_specify_params = True
+
+        def handle_multi_topics(*args, **kwargs):
+            self.counter += 1
+            if args[0] == 111:
+                self.test_listen_multi_topic1_of_common = True
+            if args[0] == 222:
+                self.test_listen_multi_topic2_of_common = True
+
+        def handle_all_topics(*args, **kwargs):
+            self.all_counter += 1
+
+        # test all topics
+        broadcast_service.subscribe_all(handle_all_topics)
+
+        # test listen of common no params
+        broadcast_service.subscribe(
+            "test_listen_of_common_no_params", handle_topic_no_params)
+        broadcast_service.publish("test_listen_of_common_no_params")
+        wait()
+        self.assertTrue(self.test_listen_of_common_no_params)
+
+        # test listen of common specify params
+        broadcast_service.subscribe(
+            "test_listen_of_common_specify_params", handle_topic_specify_params)
+        broadcast_service.publish(
+            "test_listen_of_common_specify_params", 11, 22, 33)
+        wait()
+        self.assertTrue(self.test_listen_of_common_specify_params)
+
+        # test listen multi topics of common
+        topics = ['test_listen_multi_topic1_of_common', 'test_listen_multi_topic2_of_common']
+        broadcast_service.subscribe(topics, handle_multi_topics)
+        broadcast_service.publish("test_listen_multi_topic1_of_common", 111)
+        broadcast_service.publish("test_listen_multi_topic2_of_common", 222)
+        wait()
+        self.assertTrue(self.test_listen_multi_topic1_of_common)
+        self.assertTrue(self.test_listen_multi_topic2_of_common)
+        self.assertEqual(2, self.counter)
+
+        self.assertEqual(4, self.all_counter)
+
+    def test_listen_of_decorator(self):
+        self.test_listen_of_decorator_no_params1 = False
+        self.test_listen_of_decorator_no_params2 = False
+        self.test_listen_of_decorator_multi_params = False
+        self.test_listen_of_decorator_specify_params = False
+        self.test_listen_of_decorator_listen_all = False
+        self.counter = 0
+
+        @broadcast_service.on_listen("test_listen_of_decorator_no_params1")
+        def handle_topic_no_params():
+            self.test_listen_of_decorator_no_params1 = True
+
+        @broadcast_service.on_listen(["test_listen_of_decorator_no_params2"])
+        def handle_topic_no_params():
+            self.test_listen_of_decorator_no_params2 = True
+
+        @broadcast_service.on_listen(["test_listen_of_decorator_no_params1", "test_listen_of_decorator_no_params2"])
+        def handle_topic_no_params():
+            if self.test_listen_of_decorator_no_params1 and self.test_listen_of_decorator_no_params2:
+                self.test_listen_of_decorator_multi_params = True
+
+        @broadcast_service.on_listen(["test_listen_of_decorator_specify_params"])
+        def handle_topic_specify_params(a, b, c):
+            self.assertEqual(11, a)
+            self.assertEqual(22, b)
+            self.assertEqual(33, c)
+            self.test_listen_of_decorator_specify_params = True
+
+        @broadcast_service.on_listen()
+        def handle_listen_all_topics(*args, **kwargs):
+            self.counter += 1
+            self.test_listen_of_decorator_listen_all = True
+
+        broadcast_service.publish("test_listen_of_decorator_no_params1")
+        wait()
+        self.assertTrue(self.test_listen_of_decorator_no_params1)
+
+        broadcast_service.publish("test_listen_of_decorator_no_params2")
+        wait()
+        self.assertTrue(self.test_listen_of_decorator_no_params2)
+
+        wait()
+        self.assertTrue(self.test_listen_of_decorator_multi_params)
+
+        broadcast_service.publish(
+            "test_listen_of_decorator_specify_params", 11, 22, 33)
+        wait()
+        self.assertTrue(self.test_listen_of_decorator_specify_params)
+
+        broadcast_service.publish("test_listen_of_decorator_listen_all")
+        wait()
+        self.assertTrue(self.test_listen_of_decorator_listen_all)
+        self.assertEqual(4, self.counter)
+
+    def test_listen_of_lambda(self):
+        self.test_listen_of_lambda_no_params = False
+        self.test_listen_of_lambda_specify_params = False
+
+        def handle_topic_no_params():
+            self.test_listen_of_lambda_no_params = True
+
+        def handle_topic_specify_params(params: bool):
+            self.test_listen_of_lambda_specify_params = params
+
+        broadcast_service.subscribe(
+            "test_listen_of_lambda_no_params", lambda: handle_topic_no_params())
+        broadcast_service.publish("test_listen_of_lambda_no_params")
+        wait()
+        self.assertTrue(self.test_listen_of_lambda_no_params)
+
+        broadcast_service.subscribe(
+            "test_listen_of_lambda_specify_params", lambda: handle_topic_specify_params(True))
+        broadcast_service.publish("test_listen_of_lambda_specify_params")
+        wait()
+        self.assertTrue(self.test_listen_of_lambda_no_params)
+
+    def test_broadcast(self):
+        self.test_broadcast_one_topic1 = False
+        self.test_broadcast_one_topic2 = False
+        self.test_broadcast_multi_topic1 = False
+        self.test_broadcast_multi_topic2 = False
+        self.counter = 0
+
+        @broadcast_service.on_listen("test_broadcast_one_topic1")
+        def handle_one_topic1():
+            self.counter += 1
+            self.test_broadcast_one_topic1 = True
+
+        @broadcast_service.on_listen("test_broadcast_one_topic2")
+        def handle_one_topic2():
+            self.counter += 1
+            self.test_broadcast_one_topic2 = True
+
+        @broadcast_service.on_listen("test_broadcast_multi_topic1")
+        def handle_multi_topic1():
+            self.counter += 1
+            self.test_broadcast_multi_topic1 = True
+
+        @broadcast_service.on_listen("test_broadcast_multi_topic2")
+        def handle_multi_topic2():
+            self.counter += 1
+            self.test_broadcast_multi_topic2 = True
+
+        broadcast_service.publish("test_broadcast_one_topic1")
+        wait()
+        self.assertTrue(self.test_broadcast_one_topic1)
+
+        broadcast_service.publish(["test_broadcast_one_topic2"])
+        wait()
+        self.assertTrue(self.test_broadcast_one_topic2)
+
+        broadcast_service.publish(["test_broadcast_multi_topic1", "test_broadcast_multi_topic2"])
+        wait()
+        self.assertTrue(self.test_broadcast_multi_topic1 and self.test_broadcast_multi_topic2)
+
+        broadcast_service.publish_all()
+        wait()
+        self.assertEqual(8, self.counter)
+
+    def test_broadcast_multiple_call_one_topic(self):
+        self.counter = 0
+
+        @broadcast_service.on_listen("test_broadcast_multiple_call_one_topic")
+        def handle_multi_topic1():
+            self.counter += 1
+            self.test_broadcast_multi_topic1 = True
+
+        broadcast_service.config(num_of_executions=5).publish("test_broadcast_multiple_call_one_topic")
+        wait()
+        self.assertTrue(5, self.counter)
```

