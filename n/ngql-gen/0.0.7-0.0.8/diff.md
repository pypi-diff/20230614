# Comparing `tmp/ngql_gen-0.0.7.tar.gz` & `tmp/ngql_gen-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngql_gen-0.0.7.tar", last modified: Wed Jun 14 02:33:48 2023, max compression
+gzip compressed data, was "ngql_gen-0.0.8.tar", last modified: Wed Jun 14 02:44:14 2023, max compression
```

## Comparing `ngql_gen-0.0.7.tar` & `ngql_gen-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.097355 ngql_gen-0.0.7/
--rw-rw-rw-   0        0        0     9229 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/LICENSE
--rw-rw-rw-   0        0        0    10214 2023-06-14 02:33:48.097355 ngql_gen-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.062352 ngql_gen-0.0.7/ngql_gen/
--rw-rw-rw-   0        0        0        0 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.079352 ngql_gen-0.0.7/ngql_gen/config/
--rw-rw-rw-   0        0        0       21 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/config/__init__.py
--rw-rw-rw-   0        0        0      719 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/config/config.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.093355 ngql_gen-0.0.7/ngql_gen/generator/
--rw-rw-rw-   0        0        0      155 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/__init__.py
--rw-rw-rw-   0        0        0      641 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/edge.py
--rw-rw-rw-   0        0        0      769 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/edge_type.py
--rw-rw-rw-   0        0        0     3405 2023-06-14 02:32:50.000000 ngql_gen-0.0.7/ngql_gen/generator/select.py
--rw-rw-rw-   0        0        0     1178 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/space.py
--rw-rw-rw-   0        0        0      883 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/tag.py
--rw-rw-rw-   0        0        0     3691 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/utils.py
--rw-rw-rw-   0        0        0      504 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/generator/vertex.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.096356 ngql_gen-0.0.7/ngql_gen/model/
--rw-rw-rw-   0        0        0       44 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/model/__init__.py
--rw-rw-rw-   0        0        0      163 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/model/edge_type.py
--rw-rw-rw-   0        0        0      158 2023-06-10 07:45:14.000000 ngql_gen-0.0.7/ngql_gen/model/tag.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:33:48.077351 ngql_gen-0.0.7/ngql_gen.egg-info/
--rw-rw-rw-   0        0        0    10214 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 02:33:48.000000 ngql_gen-0.0.7/ngql_gen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      491 2023-06-14 02:33:01.000000 ngql_gen-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 02:33:48.097355 ngql_gen-0.0.7/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-14 02:44:14.038846 ngql_gen-0.0.8/
+-rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/LICENSE
+-rw-r--r--   0 jiayu      (501) staff       (20)    10130 2023-06-14 02:44:14.038674 ngql_gen-0.0.8/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)       98 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-14 02:44:14.035122 ngql_gen-0.0.8/ngql_gen/
+-rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/__init__.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-14 02:44:14.036231 ngql_gen-0.0.8/ngql_gen/config/
+-rw-r--r--   0 jiayu      (501) staff       (20)       21 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/config/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      696 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/config/config.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-14 02:44:14.037903 ngql_gen-0.0.8/ngql_gen/generator/
+-rw-r--r--   0 jiayu      (501) staff       (20)      149 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/generator/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      625 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/generator/edge.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      746 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/generator/edge_type.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     3508 2023-06-14 02:41:39.000000 ngql_gen-0.0.8/ngql_gen/generator/select.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1146 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/generator/space.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      855 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/generator/tag.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     3584 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/generator/utils.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      491 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/generator/vertex.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-14 02:44:14.038431 ngql_gen-0.0.8/ngql_gen/model/
+-rw-r--r--   0 jiayu      (501) staff       (20)       43 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/model/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      156 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/model/edge_type.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      151 2023-06-14 00:42:17.000000 ngql_gen-0.0.8/ngql_gen/model/tag.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-14 02:44:14.035797 ngql_gen-0.0.8/ngql_gen.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)    10130 2023-06-14 02:44:14.000000 ngql_gen-0.0.8/ngql_gen.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      573 2023-06-14 02:44:14.000000 ngql_gen-0.0.8/ngql_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-06-14 02:44:14.000000 ngql_gen-0.0.8/ngql_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       22 2023-06-14 02:44:14.000000 ngql_gen-0.0.8/ngql_gen.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-06-14 02:44:14.000000 ngql_gen-0.0.8/ngql_gen.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      472 2023-06-14 02:41:53.000000 ngql_gen-0.0.8/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-06-14 02:44:14.038898 ngql_gen-0.0.8/setup.cfg
```

### Comparing `ngql_gen-0.0.7/LICENSE` & `ngql_gen-0.0.8/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-Apache License
-Version 2.0, January 2004
-http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-2. Grant of Copyright License.
-
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-3. Grant of Patent License.
-
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-4. Redistribution.
-
-You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-    You must give any other recipients of the Work or Derivative Works a copy of this License; and
-    You must cause any modified files to carry prominent notices stating that You changed the files; and
-    You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-    If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-5. Submission of Contributions.
-
-Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-6. Trademarks.
-
-This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty.
-
-Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability.
-
-In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability.
-
-While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
-
-END OF TERMS AND CONDITIONS
+Apache License
+Version 2.0, January 2004
+http://www.apache.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+
+"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+
+"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+
+"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+
+"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+
+"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+
+"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+
+2. Grant of Copyright License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+
+4. Redistribution.
+
+You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+
+    You must give any other recipients of the Work or Derivative Works a copy of this License; and
+    You must cause any modified files to carry prominent notices stating that You changed the files; and
+    You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+    If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+
+You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+
+5. Submission of Contributions.
+
+Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+
+6. Trademarks.
+
+This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty.
+
+Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability.
+
+In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability.
+
+While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+
+END OF TERMS AND CONDITIONS
```

### Comparing `ngql_gen-0.0.7/PKG-INFO` & `ngql_gen-0.0.8/ngql_gen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 2.1
-Name: ngql_gen
-Version: 0.0.7
-Summary: Nebula Graph Query Language Generator
-Author-email: 东南dnf <zjy2414@outlook.com>
-License: Apache License
-        Version 2.0, January 2004
-        http://www.apache.org/licenses/
-        
-        TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-        1. Definitions.
-        
-        "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-        
-        "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-        
-        "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-        
-        "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-        
-        "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-        
-        "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-        
-        "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-        
-        "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-        
-        "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-        
-        "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-        
-        2. Grant of Copyright License.
-        
-        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-        
-        3. Grant of Patent License.
-        
-        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-        
-        4. Redistribution.
-        
-        You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-        
-            You must give any other recipients of the Work or Derivative Works a copy of this License; and
-            You must cause any modified files to carry prominent notices stating that You changed the files; and
-            You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-            If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-        
-        You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-        
-        5. Submission of Contributions.
-        
-        Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-        
-        6. Trademarks.
-        
-        This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-        
-        7. Disclaimer of Warranty.
-        
-        Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-        
-        8. Limitation of Liability.
-        
-        In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-        
-        9. Accepting Warranty or Additional Liability.
-        
-        While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
-        
-        END OF TERMS AND CONDITIONS
-        
-Project-URL: Home, https://github.com/zjy2414
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ngql_gen
-
-## 1. 介绍
-
-ngql_gen 是一个用于生成 nebula graph 的 ngql 语句的工具。
+Metadata-Version: 2.1
+Name: ngql-gen
+Version: 0.0.8
+Summary: Nebula Graph Query Language Generator
+Author-email: 东南dnf <zjy2414@outlook.com>
+License: Apache License
+        Version 2.0, January 2004
+        http://www.apache.org/licenses/
+        
+        TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+        1. Definitions.
+        
+        "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+        
+        "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+        
+        "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+        
+        "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+        
+        "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+        
+        "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+        
+        "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+        
+        "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+        
+        "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+        
+        "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+        
+        2. Grant of Copyright License.
+        
+        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+        
+        3. Grant of Patent License.
+        
+        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+        
+        4. Redistribution.
+        
+        You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+        
+            You must give any other recipients of the Work or Derivative Works a copy of this License; and
+            You must cause any modified files to carry prominent notices stating that You changed the files; and
+            You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+            If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+        
+        You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+        
+        5. Submission of Contributions.
+        
+        Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+        
+        6. Trademarks.
+        
+        This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+        
+        7. Disclaimer of Warranty.
+        
+        Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+        
+        8. Limitation of Liability.
+        
+        In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+        
+        9. Accepting Warranty or Additional Liability.
+        
+        While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+        
+        END OF TERMS AND CONDITIONS
+        
+Project-URL: Home, https://github.com/zjy2414
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ngql_gen
+
+## 1. 介绍
+
+ngql_gen 是一个用于生成 nebula graph 的 ngql 语句的工具。
```

### Comparing `ngql_gen-0.0.7/ngql_gen/config/config.py` & `ngql_gen-0.0.8/ngql_gen/config/config.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import yaml
-
-# 配置文件
-config = None
-
-# 默认配置
-default_config = {
-    'default_v1_name': 'v1',
-    'default_v2_name': 'v2',
-    'default_e_name': 'e',
-}
-
-# 读取配置文件(config.yaml)
-with open('config.yaml', 'r') as f:
-    config = yaml.load(f, Loader=yaml.FullLoader)
-
-# 如果配置文件中没有配置default_v1_name, default_v2_name, default_e_name, 则使用默认配置
-if 'default_v1_name' not in config:
-    config['default_v1_name'] = default_config['default_v1_name']
-if 'default_v2_name' not in config:
-    config['default_v2_name'] = default_config['default_v2_name']
-if 'default_e_name' not in config:
-    config['default_e_name'] = default_config['default_e_name']
+import yaml
+
+# 配置文件
+config = None
+
+# 默认配置
+default_config = {
+    'default_v1_name': 'v1',
+    'default_v2_name': 'v2',
+    'default_e_name': 'e',
+}
+
+# 读取配置文件(config.yaml)
+with open('config.yaml', 'r') as f:
+    config = yaml.load(f, Loader=yaml.FullLoader)
+
+# 如果配置文件中没有配置default_v1_name, default_v2_name, default_e_name, 则使用默认配置
+if 'default_v1_name' not in config:
+    config['default_v1_name'] = default_config['default_v1_name']
+if 'default_v2_name' not in config:
+    config['default_v2_name'] = default_config['default_v2_name']
+if 'default_e_name' not in config:
+    config['default_e_name'] = default_config['default_e_name']
```

### Comparing `ngql_gen-0.0.7/ngql_gen/generator/edge.py` & `ngql_gen-0.0.8/ngql_gen/generator/edge.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from ngql_gen.generator.utils import *
-
-
-class Edge_Ngql():
-    '''
-    Edge 相关 Ngql语句
-    '''
-
-    # 在NebulaGraph实例的指定图空间中插入一条或多条边
-    def Insert(obj: object, src: str, dst: str, if_not_exists: bool = True):
-        return f"INSERT EDGE{' IF NOT EXISTS' if if_not_exists else ''} {ClassToSchemaWithOnlyKey(obj.__class__)} " \
-            f"VALUES '{src}'->'{dst}':({GetProps(obj)});"
-
-    # 删除边。一次可以删除一条或多条边
-    def Delete(obj: object, src_vid: str, dst_vid: str):
-        return f"DELETE EDGE {obj.__class__.__name__} '{src_vid}'->'{dst_vid}'@0;"
+from ngql_gen.generator.utils import *
+
+
+class Edge_Ngql():
+    '''
+    Edge 相关 Ngql语句
+    '''
+
+    # 在NebulaGraph实例的指定图空间中插入一条或多条边
+    def Insert(obj: object, src: str, dst: str, if_not_exists: bool = True):
+        return f"INSERT EDGE{' IF NOT EXISTS' if if_not_exists else ''} {ClassToSchemaWithOnlyKey(obj.__class__)} " \
+            f"VALUES '{src}'->'{dst}':({GetProps(obj)});"
+
+    # 删除边。一次可以删除一条或多条边
+    def Delete(obj: object, src_vid: str, dst_vid: str):
+        return f"DELETE EDGE {obj.__class__.__name__} '{src_vid}'->'{dst_vid}'@0;"
```

### Comparing `ngql_gen-0.0.7/ngql_gen/generator/select.py` & `ngql_gen-0.0.8/ngql_gen/generator/select.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,73 @@
-from ngql_gen.config import config
-
-
-class Select_Ngql:
-    '''
-    Select 相关 Ngql语句
-    '''
-    def GetAllVertexs(typ: str = "", limit: int = 10):
-        v1 = config['default_v1_name']
-        pattern = f'({v1})' if typ == '' else f'({v1}: {typ})'
-        output = v1
-        return f'MATCH {pattern} RETURN {output} LIMIT {limit};'
-    
-    def GetAllEdges(limit: int = 10):
-        e = config['default_e_name']
-        pattern = f"()-[{e}]->()"
-        output = e
-        return f'MATCH {pattern} RETURN {output} LIMIT {limit};'
-    
-    def GetEdgesFromVertex(obj: object,prop_name: str,prop_value, limit: int = 10):
-        v1 = config['default_v1_name']
-        e = config['default_e_name']
-
-        # 检查prop_value是否为字符串，如果是则加上引号
-        if isinstance(prop_value, str):
-            prop_value = f"'{prop_value}'"
-
-        pattern = f'({v1}: {obj.__name__}{{{prop_name}:{prop_value}}})-[{e}]->()'
-        output = e
-        return f'MATCH {pattern} RETURN {output} LIMIT {limit};'
-    
-    def GetVertexByVid(vid: str):
-        v1 = config['default_v1_name']
-        return f"MATCH ({v1}) WHERE id({v1}) == '{vid}' RETURN {v1};"
-    
-    # 通过一个点获取所有与之相连的点
-    def GetConnectedVertexs(obj:object, prop_name: str,prop_value: str):
-        v1 = config['default_v1_name']
-        v2 = config['default_v2_name']
-
-        return f"MATCH ({v1}: {obj.__class__.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {v2};"
-    
-    # 通过一个点获取所有与之相连的点，限定边的类型
-    def GetConnectedVertexsWithEdgeType(v1_obj: object, prop_name: str,prop_value: str, edge_obj: object = None, v2_obj: object = None):
-        v1 = config['default_v1_name']
-        v2 = config['default_v2_name']
-
-        if edge_obj is None and v2_obj is None:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {v2};"
-        elif edge_obj is None:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}: {v2_obj.__name__}) RETURN {v2};"
-        elif v2_obj is None:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}) RETURN {v2};"
-        else:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}: {v2_obj.__name__}) RETURN {v2};"
-        
-        # 通过一个点获取所有与之相连的点的连接边
-    def GetConnectedEdgesWithEdgeType(v1_obj: object, prop_name: str,prop_value: str, edge_obj: object = None, v2_obj: object = None):
-        v1 = config['default_v1_name']
-        v2 = config['default_v2_name']
-
-        if edge_obj is None and v2_obj is None:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {e};"
-        elif edge_obj is None:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}: {v2_obj.__name__}) RETURN {e};"
-        elif v2_obj is None:
-            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}) RETURN {e};"
-        else:
+from ngql_gen.config import config
+
+
+class Select_Ngql:
+    '''
+    Select 相关 Ngql语句
+    '''
+    def GetAllVertexs(typ: str = "", limit: int = 10):
+        v1 = config['default_v1_name']
+        pattern = f'({v1})' if typ == '' else f'({v1}: {typ})'
+        output = v1
+        return f'MATCH {pattern} RETURN {output} LIMIT {limit};'
+    
+    def GetAllEdges(limit: int = 10):
+        e = config['default_e_name']
+        pattern = f"()-[{e}]->()"
+        output = e
+        return f'MATCH {pattern} RETURN {output} LIMIT {limit};'
+    
+    def GetEdgesFromVertex(obj: object,prop_name: str,prop_value, limit: int = 10):
+        v1 = config['default_v1_name']
+        e = config['default_e_name']
+
+        # 检查prop_value是否为字符串，如果是则加上引号
+        if isinstance(prop_value, str):
+            prop_value = f"'{prop_value}'"
+
+        pattern = f'({v1}: {obj.__name__}{{{prop_name}:{prop_value}}})-[{e}]->()'
+        output = e
+        return f'MATCH {pattern} RETURN {output} LIMIT {limit};'
+    
+    def GetVertex(v_obj:object, vid: str):
+        v1 = config['default_v1_name']
+        return f"MATCH ({v1}: {v_obj.__name__}) WHERE id({v1}) == '{vid}' RETURN {v1};"
+
+    def GetVertexByVid(vid: str):
+        v1 = config['default_v1_name']
+        return f"MATCH ({v1}) WHERE id({v1}) == '{vid}' RETURN {v1};"
+    
+    # 通过一个点获取所有与之相连的点
+    def GetConnectedVertexs(obj:object, prop_name: str,prop_value: str):
+        v1 = config['default_v1_name']
+        v2 = config['default_v2_name']
+
+        return f"MATCH ({v1}: {obj.__class__.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {v2};"
+    
+    # 通过一个点获取所有与之相连的点，限定边的类型
+    def GetConnectedVertexsWithEdgeType(v1_obj: object, prop_name: str,prop_value: str, edge_obj: object = None, v2_obj: object = None):
+        v1 = config['default_v1_name']
+        v2 = config['default_v2_name']
+
+        if edge_obj is None and v2_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {v2};"
+        elif edge_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}: {v2_obj.__name__}) RETURN {v2};"
+        elif v2_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}) RETURN {v2};"
+        else:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}: {v2_obj.__name__}) RETURN {v2};"
+        
+        # 通过一个点获取所有与之相连的点的连接边
+    def GetConnectedEdgesWithEdgeType(v1_obj: object, prop_name: str,prop_value: str, edge_obj: object = None, v2_obj: object = None):
+        v1 = config['default_v1_name']
+        v2 = config['default_v2_name']
+
+        if edge_obj is None and v2_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}) RETURN {e};"
+        elif edge_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})--({v2}: {v2_obj.__name__}) RETURN {e};"
+        elif v2_obj is None:
+            return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}) RETURN {e};"
+        else:
             return f"MATCH ({v1}: {v1_obj.__name__}{{{prop_name}: '{prop_value}'}})-[e: {edge_obj.__name__}]-({v2}: {v2_obj.__name__}) RETURN e;"
```

### Comparing `ngql_gen-0.0.7/ngql_gen/generator/space.py` & `ngql_gen-0.0.8/ngql_gen/generator/space.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Space 相关 Ngql语句
-class Space_Ngql:
-    '''
-    Space 相关 Ngql语句
-    '''
-
-    # 创建Space
-    def Create(space_name:str, vid_type:str="FIXED_STRING(30)",if_not_exists: bool = True):
-        return f"CREATE SPACE{' IF NOT EXISTS' if if_not_exists else ''} {space_name}(vid_type={vid_type});"
-    
-    # 删除Space
-    def Drop(space_name:str,if_exists: bool = True):
-        return f"DROP SPACE{' IF EXISTS' if if_exists else ''} {space_name};"
-    
-    # 显示所有Space
-    def ShowAll():
-        return "SHOW SPACES;"
-    
-    # 使用Space
-    def Use(space_name:str):
-        return f"USE {space_name};"
-    
-    # 显示指定图空间的信息
-    def Describe(space_name:str):
-        return f"DESCRIBE SPACE {space_name};"
-    
-    # 清空图空间中的点和边，但不会删除图空间本身以及其中的 Schema 信息
-    def Clear(space_name:str,if_exists: bool = True):
-        return f"CLEAR SPACE{' IF EXISTS' if if_exists else ''} {space_name};"
-    
-    # 克隆现有图空间的 Schema
-    def Clone(space_name:str, new_space_name:str):
+# Space 相关 Ngql语句
+class Space_Ngql:
+    '''
+    Space 相关 Ngql语句
+    '''
+
+    # 创建Space
+    def Create(space_name:str, vid_type:str="FIXED_STRING(30)",if_not_exists: bool = True):
+        return f"CREATE SPACE{' IF NOT EXISTS' if if_not_exists else ''} {space_name}(vid_type={vid_type});"
+    
+    # 删除Space
+    def Drop(space_name:str,if_exists: bool = True):
+        return f"DROP SPACE{' IF EXISTS' if if_exists else ''} {space_name};"
+    
+    # 显示所有Space
+    def ShowAll():
+        return "SHOW SPACES;"
+    
+    # 使用Space
+    def Use(space_name:str):
+        return f"USE {space_name};"
+    
+    # 显示指定图空间的信息
+    def Describe(space_name:str):
+        return f"DESCRIBE SPACE {space_name};"
+    
+    # 清空图空间中的点和边，但不会删除图空间本身以及其中的 Schema 信息
+    def Clear(space_name:str,if_exists: bool = True):
+        return f"CLEAR SPACE{' IF EXISTS' if if_exists else ''} {space_name};"
+    
+    # 克隆现有图空间的 Schema
+    def Clone(space_name:str, new_space_name:str):
         return f"CREATE SPACE {new_space_name} as {space_name};"
```

### Comparing `ngql_gen-0.0.7/ngql_gen/generator/tag.py` & `ngql_gen-0.0.8/ngql_gen/generator/tag.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Tag 相关 Ngql语句
-from ngql_gen.generator.utils import DictToSchema
-from ngql_gen.model.tag import Tag
-
-
-class Tag_Ngql:
-    '''
-    Tag 相关 Ngql语句
-    '''
-    # 创建Tag
-    def Create(tag: Tag, if_not_exists: bool = True):
-        return f"CREATE TAG{' IF NOT EXISTS' if if_not_exists else ''} { DictToSchema(tag.name, tag.properties) };"
-
-    # 删除当前工作空间内所有点上的指定 Tag
-    def Drop(tag_name: str, if_exists: bool = True):
-        return f"DROP TAG{' IF EXISTS' if if_exists else ''} {tag_name};"
-
-    # 删除指定点上的指定 Tag
-    def DeleteFromTag(tag_name: str, vid: str):
-        return f"DELETE {tag_name} FROM {vid};"
-
-    # 显示所有Tag
-    def ShowAll():
-        return "SHOW TAGS;"
-
-    # 显示指定Tag的信息
-    def Describe(tag_name: str):
-        return f"DESCRIBE TAG {tag_name};"
+# Tag 相关 Ngql语句
+from ngql_gen.generator.utils import DictToSchema
+from ngql_gen.model.tag import Tag
+
+
+class Tag_Ngql:
+    '''
+    Tag 相关 Ngql语句
+    '''
+    # 创建Tag
+    def Create(tag: Tag, if_not_exists: bool = True):
+        return f"CREATE TAG{' IF NOT EXISTS' if if_not_exists else ''} { DictToSchema(tag.name, tag.properties) };"
+
+    # 删除当前工作空间内所有点上的指定 Tag
+    def Drop(tag_name: str, if_exists: bool = True):
+        return f"DROP TAG{' IF EXISTS' if if_exists else ''} {tag_name};"
+
+    # 删除指定点上的指定 Tag
+    def DeleteFromTag(tag_name: str, vid: str):
+        return f"DELETE {tag_name} FROM {vid};"
+
+    # 显示所有Tag
+    def ShowAll():
+        return "SHOW TAGS;"
+
+    # 显示指定Tag的信息
+    def Describe(tag_name: str):
+        return f"DESCRIBE TAG {tag_name};"
```

### Comparing `ngql_gen-0.0.7/ngql_gen/generator/utils.py` & `ngql_gen-0.0.8/ngql_gen/generator/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-# Python类型到Ngsl类型的映射
-import datetime
-
-
-TypeToNgsl = {
-    'str': 'String',
-    'int': 'Int64',
-    'float': 'Float',
-    'bool': 'Bool',
-    'datetime': 'DateTime',
-    'date': 'Date',
-    'time': 'Time',
-    'timestamp': 'Timestamp',
-    'set': 'Set',
-    'map': 'Map',
-}
-
-
-# 从类中获取属性的类型名
-def typeNameFromClass(obj, key) -> str:
-    return obj.__annotations__[key].__name__
-
-
-# 从类中获取属性的键值对
-def ClassToSchema(obj):
-    # 获取obj的所有属性名和类型
-    props = ""
-    for key in obj.__fields__.keys():
-        # 如果属性类型在TypeToNgsl中
-        if typeNameFromClass(obj, key) in TypeToNgsl:
-            props += f'{key} {TypeToNgsl[typeNameFromClass(obj, key)]}, '
-
-    return f'{obj.__name__}({props[:-2]})'
-
-# 从类中获取属性的键值对，只包含主键
-def ClassToSchemaWithOnlyKey(obj):
-    # 获取obj的所有属性名和类型
-    props = ""
-    # print(obj.__annotations__)
-    for key in obj.__annotations__.keys():
-        # print(key)
-        # 如果属性类型在TypeToNgsl中
-        if typeNameFromClass(obj, key) in TypeToNgsl:
-            props += f'{key}, '
-
-    return f'{obj.__name__}({props[:-2]})'
-
-# 实例转换为属性的键值对
-def InstanceToField(obj: object):
-    # 获取obj的所有属性名和属性值
-    props = ""
-    for key in obj.__annotations__.keys():
-        props += f'{obj.__dict__[key]}, '
-
-    return f'{obj.__class__.__name__}({props[:-2]})'
-
-# 检查有无None值，如果有且属性类型为str，则替换为空字符串，如果属性为数字类型，则替换为0
-def CheckNone(obj: object):
-    for key in obj.__annotations__.keys():
-        if obj.__dict__[key] is None:
-            if typeNameFromClass(obj, key) == 'str':
-                obj.__dict__[key] = ""
-            elif typeNameFromClass(obj, key) == 'int':
-                obj.__dict__[key] = 0
-            elif typeNameFromClass(obj, key) == 'float':
-                obj.__dict__[key] = 0.0
-            elif typeNameFromClass(obj, key) == 'bool':
-                obj.__dict__[key] = False
-            elif typeNameFromClass(obj, key) == 'datetime':
-                obj.__dict__[key] = datetime.datetime.now()
-            elif typeNameFromClass(obj, key) == 'date':
-                obj.__dict__[key] = datetime.date.today()
-            elif typeNameFromClass(obj, key) == 'time':
-                obj.__dict__[key] = datetime.datetime.now().time()
-            elif typeNameFromClass(obj, key) == 'timestamp':
-                obj.__dict__[key] = datetime.datetime.now().timestamp()
-            elif typeNameFromClass(obj, key) == 'set':
-                obj.__dict__[key] = set()
-            elif typeNameFromClass(obj, key) == 'map':
-                obj.__dict__[key] = dict()
-            else:
-                obj.__dict__[key] = None
-    return obj
-
- # 获取obj的所有属性值
-def GetProps(obj: object) -> str:
-    props = ""
-
-    # 检查有无None值
-    obj = CheckNone(obj)
-
-    for key in obj.__annotations__.keys():
-        if isinstance(obj.__dict__[key], str):
-            props += f"'{obj.__dict__[key]}', "
-        elif isinstance(obj.__dict__[key], datetime.datetime):
-            props += f"datetime('{obj.__dict__[key]}'), "
-        else:
-            props += f'{obj.__dict__[key]}, '
-    props = props[:-2]
-    return props
-
-# 字典转换为属性的键值对
-def DictToSchema(name: str, props: dict):
-    props_str = ""
-    for key in props.keys():
-        props_str += f"{key} {props[key]}, "
-    props_str = props_str[:-2]
+# Python类型到Ngsl类型的映射
+import datetime
+
+
+TypeToNgsl = {
+    'str': 'String',
+    'int': 'Int64',
+    'float': 'Float',
+    'bool': 'Bool',
+    'datetime': 'DateTime',
+    'date': 'Date',
+    'time': 'Time',
+    'timestamp': 'Timestamp',
+    'set': 'Set',
+    'map': 'Map',
+}
+
+
+# 从类中获取属性的类型名
+def typeNameFromClass(obj, key) -> str:
+    return obj.__annotations__[key].__name__
+
+
+# 从类中获取属性的键值对
+def ClassToSchema(obj):
+    # 获取obj的所有属性名和类型
+    props = ""
+    for key in obj.__fields__.keys():
+        # 如果属性类型在TypeToNgsl中
+        if typeNameFromClass(obj, key) in TypeToNgsl:
+            props += f'{key} {TypeToNgsl[typeNameFromClass(obj, key)]}, '
+
+    return f'{obj.__name__}({props[:-2]})'
+
+# 从类中获取属性的键值对，只包含主键
+def ClassToSchemaWithOnlyKey(obj):
+    # 获取obj的所有属性名和类型
+    props = ""
+    # print(obj.__annotations__)
+    for key in obj.__annotations__.keys():
+        # print(key)
+        # 如果属性类型在TypeToNgsl中
+        if typeNameFromClass(obj, key) in TypeToNgsl:
+            props += f'{key}, '
+
+    return f'{obj.__name__}({props[:-2]})'
+
+# 实例转换为属性的键值对
+def InstanceToField(obj: object):
+    # 获取obj的所有属性名和属性值
+    props = ""
+    for key in obj.__annotations__.keys():
+        props += f'{obj.__dict__[key]}, '
+
+    return f'{obj.__class__.__name__}({props[:-2]})'
+
+# 检查有无None值，如果有且属性类型为str，则替换为空字符串，如果属性为数字类型，则替换为0
+def CheckNone(obj: object):
+    for key in obj.__annotations__.keys():
+        if obj.__dict__[key] is None:
+            if typeNameFromClass(obj, key) == 'str':
+                obj.__dict__[key] = ""
+            elif typeNameFromClass(obj, key) == 'int':
+                obj.__dict__[key] = 0
+            elif typeNameFromClass(obj, key) == 'float':
+                obj.__dict__[key] = 0.0
+            elif typeNameFromClass(obj, key) == 'bool':
+                obj.__dict__[key] = False
+            elif typeNameFromClass(obj, key) == 'datetime':
+                obj.__dict__[key] = datetime.datetime.now()
+            elif typeNameFromClass(obj, key) == 'date':
+                obj.__dict__[key] = datetime.date.today()
+            elif typeNameFromClass(obj, key) == 'time':
+                obj.__dict__[key] = datetime.datetime.now().time()
+            elif typeNameFromClass(obj, key) == 'timestamp':
+                obj.__dict__[key] = datetime.datetime.now().timestamp()
+            elif typeNameFromClass(obj, key) == 'set':
+                obj.__dict__[key] = set()
+            elif typeNameFromClass(obj, key) == 'map':
+                obj.__dict__[key] = dict()
+            else:
+                obj.__dict__[key] = None
+    return obj
+
+ # 获取obj的所有属性值
+def GetProps(obj: object) -> str:
+    props = ""
+
+    # 检查有无None值
+    obj = CheckNone(obj)
+
+    for key in obj.__annotations__.keys():
+        if isinstance(obj.__dict__[key], str):
+            props += f"'{obj.__dict__[key]}', "
+        elif isinstance(obj.__dict__[key], datetime.datetime):
+            props += f"datetime('{obj.__dict__[key]}'), "
+        else:
+            props += f'{obj.__dict__[key]}, '
+    props = props[:-2]
+    return props
+
+# 字典转换为属性的键值对
+def DictToSchema(name: str, props: dict):
+    props_str = ""
+    for key in props.keys():
+        props_str += f"{key} {props[key]}, "
+    props_str = props_str[:-2]
     return f"{name}({props_str})"
```

### Comparing `ngql_gen-0.0.7/ngql_gen.egg-info/PKG-INFO` & `ngql_gen-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 2.1
-Name: ngql-gen
-Version: 0.0.7
-Summary: Nebula Graph Query Language Generator
-Author-email: 东南dnf <zjy2414@outlook.com>
-License: Apache License
-        Version 2.0, January 2004
-        http://www.apache.org/licenses/
-        
-        TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-        1. Definitions.
-        
-        "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-        
-        "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-        
-        "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-        
-        "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-        
-        "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-        
-        "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-        
-        "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-        
-        "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-        
-        "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-        
-        "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-        
-        2. Grant of Copyright License.
-        
-        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-        
-        3. Grant of Patent License.
-        
-        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-        
-        4. Redistribution.
-        
-        You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-        
-            You must give any other recipients of the Work or Derivative Works a copy of this License; and
-            You must cause any modified files to carry prominent notices stating that You changed the files; and
-            You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-            If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-        
-        You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-        
-        5. Submission of Contributions.
-        
-        Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-        
-        6. Trademarks.
-        
-        This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-        
-        7. Disclaimer of Warranty.
-        
-        Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-        
-        8. Limitation of Liability.
-        
-        In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-        
-        9. Accepting Warranty or Additional Liability.
-        
-        While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
-        
-        END OF TERMS AND CONDITIONS
-        
-Project-URL: Home, https://github.com/zjy2414
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ngql_gen
-
-## 1. 介绍
-
-ngql_gen 是一个用于生成 nebula graph 的 ngql 语句的工具。
+Metadata-Version: 2.1
+Name: ngql_gen
+Version: 0.0.8
+Summary: Nebula Graph Query Language Generator
+Author-email: 东南dnf <zjy2414@outlook.com>
+License: Apache License
+        Version 2.0, January 2004
+        http://www.apache.org/licenses/
+        
+        TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+        1. Definitions.
+        
+        "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+        
+        "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+        
+        "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+        
+        "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+        
+        "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+        
+        "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+        
+        "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+        
+        "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+        
+        "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+        
+        "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+        
+        2. Grant of Copyright License.
+        
+        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+        
+        3. Grant of Patent License.
+        
+        Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+        
+        4. Redistribution.
+        
+        You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+        
+            You must give any other recipients of the Work or Derivative Works a copy of this License; and
+            You must cause any modified files to carry prominent notices stating that You changed the files; and
+            You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+            If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+        
+        You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+        
+        5. Submission of Contributions.
+        
+        Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+        
+        6. Trademarks.
+        
+        This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+        
+        7. Disclaimer of Warranty.
+        
+        Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+        
+        8. Limitation of Liability.
+        
+        In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+        
+        9. Accepting Warranty or Additional Liability.
+        
+        While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+        
+        END OF TERMS AND CONDITIONS
+        
+Project-URL: Home, https://github.com/zjy2414
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ngql_gen
+
+## 1. 介绍
+
+ngql_gen 是一个用于生成 nebula graph 的 ngql 语句的工具。
```

### Comparing `ngql_gen-0.0.7/ngql_gen.egg-info/SOURCES.txt` & `ngql_gen-0.0.8/ngql_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

