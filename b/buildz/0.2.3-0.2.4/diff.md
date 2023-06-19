# Comparing `tmp/buildz-0.2.3.tar.gz` & `tmp/buildz-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.2.3.tar", last modified: Sun Jan 29 07:18:52 2023, max compression
+gzip compressed data, was "buildz-0.2.4.tar", last modified: Mon Jun 19 18:25:20 2023, max compression
```

## Comparing `buildz-0.2.3.tar` & `buildz-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-01-29 07:18:52.692658 buildz-0.2.3/
--rw-rw-rw-   0        0        0    11558 2022-08-14 09:12:15.000000 buildz-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       50 2022-08-19 08:12:14.000000 buildz-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5425 2023-01-29 07:18:52.692658 buildz-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5006 2022-09-06 17:06:56.000000 buildz-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-29 07:18:52.645769 buildz-0.2.3/buildz/
--rw-rw-rw-   0        0        0     1066 2022-08-17 02:33:06.000000 buildz-0.2.3/buildz/__init__.py
--rw-rw-rw-   0        0        0      355 2022-08-19 09:14:23.000000 buildz-0.2.3/buildz/__main__.py
--rw-rw-rw-   0        0        0      447 2022-08-14 09:34:12.000000 buildz-0.2.3/buildz/base.py
--rw-rw-rw-   0        0        0     7869 2023-01-18 11:39:53.000000 buildz-0.2.3/buildz/build.py
--rw-rw-rw-   0        0        0    10920 2023-01-29 07:10:45.000000 buildz-0.2.3/buildz/confz.py
-drwxrwxrwx   0        0        0        0 2023-01-29 07:18:52.677028 buildz-0.2.3/buildz/demo/
--rw-rw-rw-   0        0        0      546 2022-08-19 07:49:10.000000 buildz-0.2.3/buildz/demo/demo.confz
--rw-rw-rw-   0        0        0      522 2022-08-14 09:49:50.000000 buildz-0.2.3/buildz/demo/demo.py
--rw-rw-rw-   0        0        0      476 2022-08-14 10:08:58.000000 buildz-0.2.3/buildz/demo/run.confz
--rw-rw-rw-   0        0        0       88 2023-01-18 11:43:44.000000 buildz-0.2.3/buildz/demo/test.py
--rw-rw-rw-   0        0        0      375 2022-08-19 07:49:17.000000 buildz-0.2.3/buildz/demo/value.confz
--rw-rw-rw-   0        0        0     5405 2022-08-19 09:13:25.000000 buildz-0.2.3/buildz/keys.py
--rw-rw-rw-   0        0        0      843 2022-12-05 14:36:08.000000 buildz-0.2.3/buildz/tools.py
-drwxrwxrwx   0        0        0        0 2023-01-29 07:18:52.661398 buildz-0.2.3/buildz.egg-info/
--rw-rw-rw-   0        0        0     5425 2023-01-29 07:18:52.000000 buildz-0.2.3/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-01-29 07:18:52.000000 buildz-0.2.3/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-29 07:18:52.000000 buildz-0.2.3/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-29 07:18:52.000000 buildz-0.2.3/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-29 07:18:52.692658 buildz-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-01-29 07:11:22.000000 buildz-0.2.3/setup.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)    11357 2023-05-10 08:15:22.000000 buildz-0.2.4/LICENSE
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       49 2023-05-10 08:15:22.000000 buildz-0.2.4/MANIFEST.in
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-19 18:25:20.901150 buildz-0.2.4/PKG-INFO
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5193 2023-06-19 17:20:46.000000 buildz-0.2.4/README.md
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1039 2023-06-02 05:54:37.000000 buildz-0.2.4/buildz/__init__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      336 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/__main__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      413 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/base.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     7595 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/build.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)    10421 2023-05-10 08:21:53.000000 buildz-0.2.4/buildz/confz.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz/demo/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      514 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/demo.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      502 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/demo.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      451 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/run.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      203 2023-06-19 17:24:31.000000 buildz-0.2.4/buildz/demo/test.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1026 2023-06-19 17:27:16.000000 buildz-0.2.4/buildz/demo/testz.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      357 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/demo/value.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5173 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/keys.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      804 2023-05-10 08:15:22.000000 buildz-0.2.4/buildz/tools.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz/xconfz/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       45 2023-06-19 17:22:29.000000 buildz-0.2.4/buildz/xconfz/__init__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2886 2023-06-19 17:22:25.000000 buildz-0.2.4/buildz/xconfz/base.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1631 2023-06-19 17:22:23.000000 buildz-0.2.4/buildz/xconfz/buff.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      227 2023-06-19 17:21:53.000000 buildz-0.2.4/buildz/xconfz/fc.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1951 2023-06-19 17:22:20.000000 buildz-0.2.4/buildz/xconfz/fc_item.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1846 2023-06-19 17:22:16.000000 buildz-0.2.4/buildz/xconfz/fc_list.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2116 2023-06-19 17:22:13.000000 buildz-0.2.4/buildz/xconfz/fc_map.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1732 2023-06-19 17:22:08.000000 buildz-0.2.4/buildz/xconfz/fc_set.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2821 2023-06-19 17:22:05.000000 buildz-0.2.4/buildz/xconfz/fc_str.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2762 2023-06-19 17:21:59.000000 buildz-0.2.4/buildz/xconfz/fc_type.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     4020 2023-06-19 17:21:39.000000 buildz-0.2.4/buildz/xconfz/mg.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-19 18:25:20.901150 buildz-0.2.4/buildz.egg-info/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/PKG-INFO
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      661 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)        1 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)        7 2023-06-19 18:25:20.000000 buildz-0.2.4/buildz.egg-info/top_level.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       38 2023-06-19 18:25:20.901150 buildz-0.2.4/setup.cfg
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      746 2023-06-19 17:13:51.000000 buildz-0.2.4/setup.py
```

### Comparing `buildz-0.2.3/LICENSE` & `buildz-0.2.4/LICENSE`

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

### Comparing `buildz-0.2.3/PKG-INFO` & `buildz-0.2.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,153 +1,142 @@
-Metadata-Version: 2.1
-Name: buildz
-Version: 0.2.3
-Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
-Home-page: https://github.com/buildCodeZ/buildz
-Author: Zzz
-Author-email: 1309458652@qq.com
-License: Apache License 2.0
-Keywords: buildz
-Platform: any
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# confz
-```
-一个类似json的数据交换格式，取名叫做confz，并用python实现了读写代码，另外还根据confz写了个代码配置框架
-a json-like file format's read and write code by python, also write a code building framework configure by confz, english description is in "2) english"
-```
-
-## 1) 简介
-```
-1. confz(buildz.confz)
-和json主要区别:
-  1，默认所有值都是字符串，而如果没有包含confz的关键字，不需要用引号引起来；
-  2，换行符\n和逗号,和分号;都作为分割符; 单引号和双引号具有一样的效果
-  3，可以写注释，单行注释用#，多行注释用### 注释 ###
-  4, 字符串可以多行，用'''字符串'''或"""字符串"""
-  5, 如果要confz不把取值当作字符串，要写在尖括号<>里: <数值, 数据类型>，比如整数10写成<10, int>, 浮点数11.1写成<11.1, float>，布尔类型true写成<true, bool>，None写成<-, null>
-写这个东西是为了方便写配置文件和读配置文件，xml感觉有点麻烦，直接用json又要写很多引号，就对json做了简化
-confz的关键字如下:
-  {}[]()<>:'"#\n,;
-一个简单的例子和json作比较:
-  json:
-  {
-    "basedir": "D:\demo",
-    "key": "demo",
-    "maxdepth": 10
-  }
-  confz:
-  {
-    # 基本路径，因为取值包含关键字":", 需要用引号引起来
-    basedir: "D:\demo"
-    # 搜索关键字
-    key: demo
-    # 最大文件深度
-    maxdepth: <10, int>
-  }
-主要方法:
-  read(s): 把confz格式的字符串s转换成object
-  loadfile(s, coding="utf-8"): 从文件s读取confz格式字符串并转换成object，默认编码utf-8
-  output(obj): 把数据obj转换成confz格式字符串，这里要注意的是output输出的字符串做了基本的换行
-目前只有读和写的代码，之后有空的话可能会写一个confz格式校验代码
-
-2. 控制反转框架(buildz.build, buildz.base)
-    根据confz写的控制反转框架（IoC框架）：buildz.Builder或buildz.main
-    具体描述在buildz.keys里，可以调用buildz.keys.help()查看，或者运行"python -m buildz ? ch"来查查，另外包里有个例子可以看下：buildz/demo
-        测试：在demo文件夹中打开命令行，运行：
-            1) python test.py ./demo.confz ./value.confz
-            或
-            2) python test.py ./run.confz
-        1)和2)是等价的，另外如果把buildz当作python来安装，也可以这样运行:
-            1) python -m buildz ./demo.confz ./value.confz
-            或
-            2) python -m buildz ./run.confz
-
-```
-## 2) english:
-```
-1. confz(buildz.confz)
-(1) remain char:
-    {}[]()<>:'"#\n,;
-   to write a string contain remain char, user '' or "" or " x3 or ' x3: 
-    "hello:world, 'zero'" 
-    'hello:world, "zero"'
-    """zero say: "hello, 'world'!" """
-(2) from string to obj:
-    read(s)
-(3) from obj to string:
-    output(obj)
-(4) from filepath to obj:
-    loadfile(filepath, coding="utf-8")
-(5) simple read filepath to string:
-    fread(filepath)
-example:
-demo.txt:
-[
-    # single line note
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    {
-        test: ":test{}??", 
-        val: <10, int>, 
-        cost: <10.0, float>, 
-        check: <true, bool>, 
-        <10, int>: "test"
-    }
-    #multi-line string
-    """test line
-        1
-        2
-        3
-    """
-    1
-    2
-    3
-    # type not string
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-code:
-obj = confz.loadfile("demo.txt")
-obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
-s = confz.output(obj)
-print(s):
-[
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
-    "test line
-        1
-        2
-        3
-    "
-    1
-    2
-    3
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-only realize codes of read and write now,  code of format checking may be writing in future, if I have time.
-PS: None write as <-, null> (confz: '{data: <-,null>}' == json: '{"data":null}')
-2. IoC framework codes(buildz.Builder, buildz.main)
-    description is in buildz.keys, run this code to see: "buildz.keys.help('en')" or "python -m buildz ? en"
-    here is an example in buildz/demo
-    you can open an commond line in demo folder and run like this:
-        1) python test.py ./demo.confz ./value.confz
-        or:
-        2) python test.py ./run.confz
-    1) and 2) is equivalent, besides, if you install buildz as python lib, you can also run like this:
-        1) python -m buildz ./demo.confz ./value.confz
-        or
-        2) python -m buildz ./run.confz
-```
-
-
+# confz
+```
+一个类似json的数据交换格式，取名叫做confz，并用python实现了读写代码，另外还根据confz写了个代码配置框架
+a json-like file format's read and write code by python, also write a code building framework configure by confz, english description is in "2) english"
+
+update:
+新增buildz.xconfz，用模式化的代码重构buildz.confz，让代码更容易维护（相应的速度会更慢些），目前只重构了loads
+add sub module buildz.xconfz, which reconstruct buidlz.confz by modularized code, making it easier to update(and run slower), currently only reconstruct method 'loads'
+```
+
+## 1) 简介
+```
+1. confz(buildz.confz)
+和json主要区别:
+  1，默认所有值都是字符串，而如果没有包含confz的关键字，不需要用引号引起来；
+  2，换行符\n和逗号,和分号;都作为分割符; 单引号和双引号具有一样的效果
+  3，可以写注释，单行注释用#，多行注释用### 注释 ###
+  4, 字符串可以多行，用'''字符串'''或"""字符串"""
+  5, 如果要confz不把取值当作字符串，要写在尖括号<>里: <数值, 数据类型>，比如整数10写成<10, int>, 浮点数11.1写成<11.1, float>，布尔类型true写成<true, bool>，None写成<-, null>
+写这个东西是为了方便写配置文件和读配置文件，xml感觉有点麻烦，直接用json又要写很多引号，就对json做了简化
+confz的关键字如下:
+  {}[]()<>:'"#\n,;
+一个简单的例子和json作比较:
+  json:
+  {
+    "basedir": "D:\demo",
+    "key": "demo",
+    "maxdepth": 10
+  }
+  confz:
+  {
+    # 基本路径，因为取值包含关键字":", 需要用引号引起来
+    basedir: "D:\demo"
+    # 搜索关键字
+    key: demo
+    # 最大文件深度
+    maxdepth: <10, int>
+  }
+主要方法:
+  read(s): 把confz格式的字符串s转换成object
+  loadfile(s, coding="utf-8"): 从文件s读取confz格式字符串并转换成object，默认编码utf-8
+  output(obj): 把数据obj转换成confz格式字符串，这里要注意的是output输出的字符串做了基本的换行
+目前只有读和写的代码，之后有空的话可能会写一个confz格式校验代码
+
+2. 控制反转框架(buildz.build, buildz.base)
+    根据confz写的控制反转框架（IoC框架）：buildz.Builder或buildz.main
+    具体描述在buildz.keys里，可以调用buildz.keys.help()查看，或者运行"python -m buildz ? ch"来查查，另外包里有个例子可以看下：buildz/demo
+        测试：在demo文件夹中打开命令行，运行：
+            1) python test.py ./demo.confz ./value.confz
+            或
+            2) python test.py ./run.confz
+        1)和2)是等价的，另外如果把buildz当作python来安装，也可以这样运行:
+            1) python -m buildz ./demo.confz ./value.confz
+            或
+            2) python -m buildz ./run.confz
+
+```
+## 2) english:
+```
+1. confz(buildz.confz)
+(1) remain char:
+    {}[]()<>:'"#\n,;
+   to write a string contain remain char, user '' or "" or " x3 or ' x3: 
+    "hello:world, 'zero'" 
+    'hello:world, "zero"'
+    """zero say: "hello, 'world'!" """
+(2) from string to obj:
+    read(s)
+(3) from obj to string:
+    output(obj)
+(4) from filepath to obj:
+    loadfile(filepath, coding="utf-8")
+(5) simple read filepath to string:
+    fread(filepath)
+example:
+demo.txt:
+[
+    # single line note
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    {
+        test: ":test{}??", 
+        val: <10, int>, 
+        cost: <10.0, float>, 
+        check: <true, bool>, 
+        <10, int>: "test"
+    }
+    #multi-line string
+    """test line
+        1
+        2
+        3
+    """
+    1
+    2
+    3
+    # type not string
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+code:
+obj = confz.loadfile("demo.txt")
+obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
+s = confz.output(obj)
+print(s):
+[
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
+    "test line
+        1
+        2
+        3
+    "
+    1
+    2
+    3
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+only realize codes of read and write now,  code of format checking may be writing in future, if I have time.
+PS: None write as <-, null> (confz: '{data: <-,null>}' == json: '{"data":null}')
+2. IoC framework codes(buildz.Builder, buildz.main)
+    description is in buildz.keys, run this code to see: "buildz.keys.help('en')" or "python -m buildz ? en"
+    here is an example in buildz/demo
+    you can open an commond line in demo folder and run like this:
+        1) python test.py ./demo.confz ./value.confz
+        or:
+        2) python test.py ./run.confz
+    1) and 2) is equivalent, besides, if you install buildz as python lib, you can also run like this:
+        1) python -m buildz ./demo.confz ./value.confz
+        or
+        2) python -m buildz ./run.confz
+```
```

### Comparing `buildz-0.2.3/README.md` & `buildz-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,157 @@
-# confz
-```
-一个类似json的数据交换格式，取名叫做confz，并用python实现了读写代码，另外还根据confz写了个代码配置框架
-a json-like file format's read and write code by python, also write a code building framework configure by confz, english description is in "2) english"
-```
-
-## 1) 简介
-```
-1. confz(buildz.confz)
-和json主要区别:
-  1，默认所有值都是字符串，而如果没有包含confz的关键字，不需要用引号引起来；
-  2，换行符\n和逗号,和分号;都作为分割符; 单引号和双引号具有一样的效果
-  3，可以写注释，单行注释用#，多行注释用### 注释 ###
-  4, 字符串可以多行，用'''字符串'''或"""字符串"""
-  5, 如果要confz不把取值当作字符串，要写在尖括号<>里: <数值, 数据类型>，比如整数10写成<10, int>, 浮点数11.1写成<11.1, float>，布尔类型true写成<true, bool>，None写成<-, null>
-写这个东西是为了方便写配置文件和读配置文件，xml感觉有点麻烦，直接用json又要写很多引号，就对json做了简化
-confz的关键字如下:
-  {}[]()<>:'"#\n,;
-一个简单的例子和json作比较:
-  json:
-  {
-    "basedir": "D:\demo",
-    "key": "demo",
-    "maxdepth": 10
-  }
-  confz:
-  {
-    # 基本路径，因为取值包含关键字":", 需要用引号引起来
-    basedir: "D:\demo"
-    # 搜索关键字
-    key: demo
-    # 最大文件深度
-    maxdepth: <10, int>
-  }
-主要方法:
-  read(s): 把confz格式的字符串s转换成object
-  loadfile(s, coding="utf-8"): 从文件s读取confz格式字符串并转换成object，默认编码utf-8
-  output(obj): 把数据obj转换成confz格式字符串，这里要注意的是output输出的字符串做了基本的换行
-目前只有读和写的代码，之后有空的话可能会写一个confz格式校验代码
-
-2. 控制反转框架(buildz.build, buildz.base)
-    根据confz写的控制反转框架（IoC框架）：buildz.Builder或buildz.main
-    具体描述在buildz.keys里，可以调用buildz.keys.help()查看，或者运行"python -m buildz ? ch"来查查，另外包里有个例子可以看下：buildz/demo
-        测试：在demo文件夹中打开命令行，运行：
-            1) python test.py ./demo.confz ./value.confz
-            或
-            2) python test.py ./run.confz
-        1)和2)是等价的，另外如果把buildz当作python来安装，也可以这样运行:
-            1) python -m buildz ./demo.confz ./value.confz
-            或
-            2) python -m buildz ./run.confz
-
-```
-## 2) english:
-```
-1. confz(buildz.confz)
-(1) remain char:
-    {}[]()<>:'"#\n,;
-   to write a string contain remain char, user '' or "" or " x3 or ' x3: 
-    "hello:world, 'zero'" 
-    'hello:world, "zero"'
-    """zero say: "hello, 'world'!" """
-(2) from string to obj:
-    read(s)
-(3) from obj to string:
-    output(obj)
-(4) from filepath to obj:
-    loadfile(filepath, coding="utf-8")
-(5) simple read filepath to string:
-    fread(filepath)
-example:
-demo.txt:
-[
-    # single line note
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    {
-        test: ":test{}??", 
-        val: <10, int>, 
-        cost: <10.0, float>, 
-        check: <true, bool>, 
-        <10, int>: "test"
-    }
-    #multi-line string
-    """test line
-        1
-        2
-        3
-    """
-    1
-    2
-    3
-    # type not string
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-code:
-obj = confz.loadfile("demo.txt")
-obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
-s = confz.output(obj)
-print(s):
-[
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
-    "test line
-        1
-        2
-        3
-    "
-    1
-    2
-    3
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-only realize codes of read and write now,  code of format checking may be writing in future, if I have time.
-PS: None write as <-, null> (confz: '{data: <-,null>}' == json: '{"data":null}')
-2. IoC framework codes(buildz.Builder, buildz.main)
-    description is in buildz.keys, run this code to see: "buildz.keys.help('en')" or "python -m buildz ? en"
-    here is an example in buildz/demo
-    you can open an commond line in demo folder and run like this:
-        1) python test.py ./demo.confz ./value.confz
-        or:
-        2) python test.py ./run.confz
-    1) and 2) is equivalent, besides, if you install buildz as python lib, you can also run like this:
-        1) python -m buildz ./demo.confz ./value.confz
-        or
-        2) python -m buildz ./run.confz
-```
+Metadata-Version: 2.1
+Name: buildz
+Version: 0.2.4
+Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
+Home-page: https://github.com/buildCodeZ/buildz
+Author: Zzz
+Author-email: 1309458652@qq.com
+License: Apache License 2.0
+Keywords: buildz
+Platform: any
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# confz
+```
+一个类似json的数据交换格式，取名叫做confz，并用python实现了读写代码，另外还根据confz写了个代码配置框架
+a json-like file format's read and write code by python, also write a code building framework configure by confz, english description is in "2) english"
+
+update:
+新增buildz.xconfz，用模式化的代码重构buildz.confz，让代码更容易维护（相应的速度会更慢些），目前只重构了loads
+add sub module buildz.xconfz, which reconstruct buidlz.confz by modularized code, making it easier to update(and run slower), currently only reconstruct method 'loads'
+```
+
+## 1) 简介
+```
+1. confz(buildz.confz)
+和json主要区别:
+  1，默认所有值都是字符串，而如果没有包含confz的关键字，不需要用引号引起来；
+  2，换行符\n和逗号,和分号;都作为分割符; 单引号和双引号具有一样的效果
+  3，可以写注释，单行注释用#，多行注释用### 注释 ###
+  4, 字符串可以多行，用'''字符串'''或"""字符串"""
+  5, 如果要confz不把取值当作字符串，要写在尖括号<>里: <数值, 数据类型>，比如整数10写成<10, int>, 浮点数11.1写成<11.1, float>，布尔类型true写成<true, bool>，None写成<-, null>
+写这个东西是为了方便写配置文件和读配置文件，xml感觉有点麻烦，直接用json又要写很多引号，就对json做了简化
+confz的关键字如下:
+  {}[]()<>:'"#\n,;
+一个简单的例子和json作比较:
+  json:
+  {
+    "basedir": "D:\demo",
+    "key": "demo",
+    "maxdepth": 10
+  }
+  confz:
+  {
+    # 基本路径，因为取值包含关键字":", 需要用引号引起来
+    basedir: "D:\demo"
+    # 搜索关键字
+    key: demo
+    # 最大文件深度
+    maxdepth: <10, int>
+  }
+主要方法:
+  read(s): 把confz格式的字符串s转换成object
+  loadfile(s, coding="utf-8"): 从文件s读取confz格式字符串并转换成object，默认编码utf-8
+  output(obj): 把数据obj转换成confz格式字符串，这里要注意的是output输出的字符串做了基本的换行
+目前只有读和写的代码，之后有空的话可能会写一个confz格式校验代码
+
+2. 控制反转框架(buildz.build, buildz.base)
+    根据confz写的控制反转框架（IoC框架）：buildz.Builder或buildz.main
+    具体描述在buildz.keys里，可以调用buildz.keys.help()查看，或者运行"python -m buildz ? ch"来查查，另外包里有个例子可以看下：buildz/demo
+        测试：在demo文件夹中打开命令行，运行：
+            1) python test.py ./demo.confz ./value.confz
+            或
+            2) python test.py ./run.confz
+        1)和2)是等价的，另外如果把buildz当作python来安装，也可以这样运行:
+            1) python -m buildz ./demo.confz ./value.confz
+            或
+            2) python -m buildz ./run.confz
+
+```
+## 2) english:
+```
+1. confz(buildz.confz)
+(1) remain char:
+    {}[]()<>:'"#\n,;
+   to write a string contain remain char, user '' or "" or " x3 or ' x3: 
+    "hello:world, 'zero'" 
+    'hello:world, "zero"'
+    """zero say: "hello, 'world'!" """
+(2) from string to obj:
+    read(s)
+(3) from obj to string:
+    output(obj)
+(4) from filepath to obj:
+    loadfile(filepath, coding="utf-8")
+(5) simple read filepath to string:
+    fread(filepath)
+example:
+demo.txt:
+[
+    # single line note
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    {
+        test: ":test{}??", 
+        val: <10, int>, 
+        cost: <10.0, float>, 
+        check: <true, bool>, 
+        <10, int>: "test"
+    }
+    #multi-line string
+    """test line
+        1
+        2
+        3
+    """
+    1
+    2
+    3
+    # type not string
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+code:
+obj = confz.loadfile("demo.txt")
+obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
+s = confz.output(obj)
+print(s):
+[
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
+    "test line
+        1
+        2
+        3
+    "
+    1
+    2
+    3
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+only realize codes of read and write now,  code of format checking may be writing in future, if I have time.
+PS: None write as <-, null> (confz: '{data: <-,null>}' == json: '{"data":null}')
+2. IoC framework codes(buildz.Builder, buildz.main)
+    description is in buildz.keys, run this code to see: "buildz.keys.help('en')" or "python -m buildz ? en"
+    here is an example in buildz/demo
+    you can open an commond line in demo folder and run like this:
+        1) python test.py ./demo.confz ./value.confz
+        or:
+        2) python test.py ./run.confz
+    1) and 2) is equivalent, besides, if you install buildz as python lib, you can also run like this:
+        1) python -m buildz ./demo.confz ./value.confz
+        or
+        2) python -m buildz ./run.confz
+```
+
+
```

### Comparing `buildz-0.2.3/buildz/__init__.py` & `buildz-0.2.4/buildz/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from buildz.confz import read, loadfile, output, fread
-from buildz.build import Builder, main
-from buildz.keys import help
-"""
-json-like(called 'confz' in here) data format function:
-    read: string -> obj
-    output: obj -> string
-    fread(filepath, coding="utf-8"): filepath -> string 
-        #open(filepath, 'rb').read().decode(coding)
-    loadfile(filepath, coding="utf-8"): filepath -> obj 
-        #equals to read(fread(filepath, coding))
-
-a framework to build code:
-    function: main
-    Object: Builder
-    Description:
-        build instance and run from confz format configure file, here is an example in buildz/demo
-        从confz格式文件配置中生成对象实例和运行，例子在buildz/demo里
-
-        you can open an commond line in demo folder and run like this:
-        测试：在demo文件夹中打开命令行，运行：
-
-            1) python test.py ./demo.confz ./value.confz
-            or:
-            2) python test.py ./run.confz
-
-        1) and 2) is equivalent
-        1)和2)是等价的
+#from buildz.confz import read, loadfile, output, fread
+from buildz.build import Builder, main
+from buildz.keys import help
+"""
+json-like(called 'confz' in here) data format function:
+    read: string -> obj
+    output: obj -> string
+    fread(filepath, coding="utf-8"): filepath -> string 
+        #open(filepath, 'rb').read().decode(coding)
+    loadfile(filepath, coding="utf-8"): filepath -> obj 
+        #equals to read(fread(filepath, coding))
+
+a framework to build code:
+    function: main
+    Object: Builder
+    Description:
+        build instance and run from confz format configure file, here is an example in buildz/demo
+        从confz格式文件配置中生成对象实例和运行，例子在buildz/demo里
+
+        you can open an commond line in demo folder and run like this:
+        测试：在demo文件夹中打开命令行，运行：
+
+            1) python test.py ./demo.confz ./value.confz
+            or:
+            2) python test.py ./run.confz
+
+        1) and 2) is equivalent
+        1)和2)是等价的
 """
```

### Comparing `buildz-0.2.3/buildz/build.py` & `buildz-0.2.4/buildz/build.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-#coding=utf-8
-#main
-def get(obj, key, default = None):
-    if key in obj:
-        return obj[key]
-    return default
-
-pass
-def load(md, fc = None):
-    arr = md.split(".")[1:]
-    md = __import__(md)
-    for k in arr:
-        md = getattr(md, k)
-    if fc is not None:
-        fc = getattr(md, fc)
-    else:
-        fc = md
-    return fc
-
-pass
-class EpFc:
-    def __init__(self, fc, n = 1):
-        self.fc = fc
-        self.n = n
-    def __call__(self, *argv):
-        argv = argv[:self.n]
-        return self.fc(*argv)
-
-pass
-import builtins
-def build_list(*argv):
-    return list(argv)
-
-pass
-
-def build_dict(**maps):
-    return dict(maps)
-
-pass
-builtins._list = build_list
-builtins._dict = build_dict
-g_default_import = "buildz"+".base"
-def read_confz(filepath):
-    from buildz import confz
-    s = confz.fread(filepath)
-    obj = confz.read(s)
-    return obj
-
-pass
-def read_json(filepath):
-    from buildz import confz
-    import json
-    s = confz.fread(filepath)
-    obj = json.loads(s)
-    return obj
-
-pass
-    
-class Builder:
-    def __init__(self, default_single = "0", default_import = g_default_import, ref_this = None, format = "confz"):
-        self.ref_this = ref_this
-        self.default_import = default_import
-        self.default_single = default_single
-        self.format = format
-        self.maps = {}
-        self.objs = {}
-        types = {}
-        types['str'] = EpFc(str)
-        types['int'] = EpFc(int)
-        types['float'] = EpFc(float)
-        self.types = types
-        self.types['ref'] = EpFc(self.run)
-        self.types['this'] = EpFc(self.get_this, 2)
-        self.types['call'] = EpFc(self.run, 2)
-        self.types['fc'] = EpFc(self.run, 1)
-        self.types['run'] = EpFc(self.run, 1)
-        self.loadtypes = {}
-        self.loadtypes['json'] = read_json
-        self.loadtypes['confz'] = read_confz
-    def add_file(self, filepath, format = None, update = False):
-        if format is None:
-            format = self.format
-        obj = self.loadtypes[format](filepath)
-        self.add(obj, update)
-    def add(self, data, update = False):
-        if type(data) == dict:
-            data = [data]
-        for obj in data:
-            key = get(obj, "key")
-            if key in self.maps and not update:
-                raise Exception("duple define key: ["+key+"]")
-            self.maps[key] = obj
-            if update and key in self.objs:
-                del self.objs[key]
-    def get_this(self, key, obj):
-        return getattr(obj, key)
-    def deal_args(self, args, obj = None):
-        if type(args)!= list:
-            args = [args]
-        rst = []
-        for _obj in args:
-            if type(_obj) not in [list, tuple]:
-                _obj = [_obj, "str"]
-            val = self.types[_obj[1]](_obj[0], obj)
-            rst.append(val)
-        return rst
-    def deal_maps(self, maps, obj = None):
-        rst = {}
-        for _obj in maps:
-            if len(_obj)==2:
-                _obj.append("str")
-            _key = _obj[0]
-            if type(_key) == list:
-                _key = self.run(_key)
-            val = self.types[_obj[2]](_obj[1], obj)
-            rst[_key] = val
-        return rst
-    def deal_sets(self, sets, obj):
-        for param in sets:
-            if len(param)==2:
-                param.append("str")
-            _key = param[0]
-            val = self.types[param[2]](param[1], obj)
-            setattr(obj, _key, val)
-    def deal_fcs(self, calls, obj):
-        for call in calls:
-            if type(call)!= list:
-                call = [call, "call"]
-            self.types[call[1]](call[0], obj)
-    def get(self, key, src = None, force_new = False):
-        return self.run(key, src, force_new)
-    def set(self, key, val):
-        self.maps[key] = {"single":"1"}
-        self.objs[key] = val
-    def run(self, key, src = None, force_new = False):
-        if self.ref_this is not None and key == self.ref_this:
-            return self
-        if key not in self.maps:
-            raise Exception("Error not such fc:"+key)
-        data = self.maps[key]
-        ref = get(data, "ref")
-        if src is None and ref is not None:
-            src = self.run(ref)
-        if src is not None:
-            force_new = True
-        single = bool(int(get(data, "single", self.default_single)))
-        single &= not force_new
-        if single and key in self.objs:
-            return self.objs[key]
-        val = get(data, "val", None)
-        if val is not None:
-            args = [val]
-        else:
-            args = get(data, "args", [])
-        args = self.deal_args(args, src)
-        maps = get(data, "maps", [])
-        maps = self.deal_maps(maps, src)
-        fc = get(data, "call", None)
-        var = get(data, "var", None)
-        mark_var = False
-        if fc is None:
-            if var is not None:
-                mark_var = True
-                fc = var
-        obj = None
-        _data = get(data, "data", None)
-        if fc is not None or src is not None:
-            fcs = []
-            if fc is not None:
-                fcs = fc.split(".")
-            if src is not None:
-                fc = src
-            else:
-                _import = get(data, "import", self.default_import)
-                md = load(_import)
-                fc = md
-            for nfc in fcs:
-                fc = getattr(fc, nfc)
-            if mark_var:
-                return fc
-            if _data is None:
-                obj = fc(*args, **maps)
-            else:
-                obj = fc(_data)
-            if single:
-                self.objs[key] = obj
-            sets = get(data, "sets", [])
-            self.deal_sets(sets, obj)
-        calls = get(data, "calls", [])
-        self.deal_fcs(calls, obj)
-        if obj is None:
-            if _data is not None:
-                return _data
-            elif val is not None:
-                return val
-            elif args is not None:
-                return args
-            elif maps is not None:
-                return maps
-        return obj
-
-pass
-class Test:
-    def __init__(self, a, b):
-        print("a:", a)
-        self.a = a
-        self.b = b
-    def test(self, obj):
-        print("TEST:", obj)
-    def __call__(self):
-        print(self.a)
-        print(self.b)
-
-pass
-
-import sys
-import os
-def main(paths, default_import = g_default_import, ref_this = "this"):
-    builder = Builder(1, default_import = default_import, ref_this = ref_this)
-    for path in paths:
-        if os.path.isfile(path):
-            builder.add_file(path)
-        elif os.path.isdir(path):
-            files = os.listdir(path)
-            files = [os.path.join(path, file) for file in files]
-            [builder.add_file(file) for file in files]
-        else:
-            print("what is this? :", path)
-    builder.run("main")
-
-pass
-import os
-import re
-class Pattern:
-    def __init__(self, pt):
-        self.pt = pt
-    def __call__(self, s):
-        if self.pt is None:
-            return True
-        return re.findall(self.pt, s)>0
-
-pass
-
-
-def listdir(path, max_depth = -1, pattern = None, nopattern = None, march = None):
-    if max_depth == 0:
-        return []
-    files = os.listdir(path)
-    pt = Pattern(pattern)
-    files = [os.path.join(path, file) for file in files]
-    rst = []
-    for file in files:
-        if os.path.isdir(file):
-            rst += listdir(file, max_depth-1, pattern)
-        else:
-            if pt(os.path.basename(file)):
-                rst.append(file)
-    return rst
-
-pass
-
-    
-def test():
-    builder = Builder(1)
-    argv = sys.argv[1:]
-    main(argv)
-
-pass
-
-if __name__=="__main__":
-    test()
-
-pass
-
+#coding=utf-8
+#main
+def get(obj, key, default = None):
+    if key in obj:
+        return obj[key]
+    return default
+
+pass
+def load(md, fc = None):
+    arr = md.split(".")[1:]
+    md = __import__(md)
+    for k in arr:
+        md = getattr(md, k)
+    if fc is not None:
+        fc = getattr(md, fc)
+    else:
+        fc = md
+    return fc
+
+pass
+class EpFc:
+    def __init__(self, fc, n = 1):
+        self.fc = fc
+        self.n = n
+    def __call__(self, *argv):
+        argv = argv[:self.n]
+        return self.fc(*argv)
+
+pass
+import builtins
+def build_list(*argv):
+    return list(argv)
+
+pass
+
+def build_dict(**maps):
+    return dict(maps)
+
+pass
+builtins._list = build_list
+builtins._dict = build_dict
+g_default_import = "buildz"+".base"
+def read_confz(filepath):
+    from buildz import confz
+    s = confz.fread(filepath)
+    obj = confz.read(s)
+    return obj
+
+pass
+def read_json(filepath):
+    from buildz import confz
+    import json
+    s = confz.fread(filepath)
+    obj = json.loads(s)
+    return obj
+
+pass
+    
+class Builder:
+    def __init__(self, default_single = "0", default_import = g_default_import, ref_this = None, format = "confz"):
+        self.ref_this = ref_this
+        self.default_import = default_import
+        self.default_single = default_single
+        self.format = format
+        self.maps = {}
+        self.objs = {}
+        types = {}
+        types['str'] = EpFc(str)
+        types['int'] = EpFc(int)
+        types['float'] = EpFc(float)
+        self.types = types
+        self.types['ref'] = EpFc(self.run)
+        self.types['this'] = EpFc(self.get_this, 2)
+        self.types['call'] = EpFc(self.run, 2)
+        self.types['fc'] = EpFc(self.run, 1)
+        self.types['run'] = EpFc(self.run, 1)
+        self.loadtypes = {}
+        self.loadtypes['json'] = read_json
+        self.loadtypes['confz'] = read_confz
+    def add_file(self, filepath, format = None, update = False):
+        if format is None:
+            format = self.format
+        obj = self.loadtypes[format](filepath)
+        self.add(obj, update)
+    def add(self, data, update = False):
+        if type(data) == dict:
+            data = [data]
+        for obj in data:
+            key = get(obj, "key")
+            if key in self.maps and not update:
+                raise Exception("duple define key: ["+key+"]")
+            self.maps[key] = obj
+            if update and key in self.objs:
+                del self.objs[key]
+    def get_this(self, key, obj):
+        return getattr(obj, key)
+    def deal_args(self, args, obj = None):
+        if type(args)!= list:
+            args = [args]
+        rst = []
+        for _obj in args:
+            if type(_obj) not in [list, tuple]:
+                _obj = [_obj, "str"]
+            val = self.types[_obj[1]](_obj[0], obj)
+            rst.append(val)
+        return rst
+    def deal_maps(self, maps, obj = None):
+        rst = {}
+        for _obj in maps:
+            if len(_obj)==2:
+                _obj.append("str")
+            _key = _obj[0]
+            if type(_key) == list:
+                _key = self.run(_key)
+            val = self.types[_obj[2]](_obj[1], obj)
+            rst[_key] = val
+        return rst
+    def deal_sets(self, sets, obj):
+        for param in sets:
+            if len(param)==2:
+                param.append("str")
+            _key = param[0]
+            val = self.types[param[2]](param[1], obj)
+            setattr(obj, _key, val)
+    def deal_fcs(self, calls, obj):
+        for call in calls:
+            if type(call)!= list:
+                call = [call, "call"]
+            self.types[call[1]](call[0], obj)
+    def get(self, key, src = None, force_new = False):
+        return self.run(key, src, force_new)
+    def set(self, key, val):
+        self.maps[key] = {"single":"1"}
+        self.objs[key] = val
+    def run(self, key, src = None, force_new = False):
+        if self.ref_this is not None and key == self.ref_this:
+            return self
+        if key not in self.maps:
+            raise Exception("Error not such fc:"+key)
+        data = self.maps[key]
+        ref = get(data, "ref")
+        if src is None and ref is not None:
+            src = self.run(ref)
+        if src is not None:
+            force_new = True
+        single = bool(int(get(data, "single", self.default_single)))
+        single &= not force_new
+        if single and key in self.objs:
+            return self.objs[key]
+        val = get(data, "val", None)
+        if val is not None:
+            args = [val]
+        else:
+            args = get(data, "args", [])
+        args = self.deal_args(args, src)
+        maps = get(data, "maps", [])
+        maps = self.deal_maps(maps, src)
+        fc = get(data, "call", None)
+        var = get(data, "var", None)
+        mark_var = False
+        if fc is None:
+            if var is not None:
+                mark_var = True
+                fc = var
+        obj = None
+        _data = get(data, "data", None)
+        if fc is not None or src is not None:
+            fcs = []
+            if fc is not None:
+                fcs = fc.split(".")
+            if src is not None:
+                fc = src
+            else:
+                _import = get(data, "import", self.default_import)
+                md = load(_import)
+                fc = md
+            for nfc in fcs:
+                fc = getattr(fc, nfc)
+            if mark_var:
+                return fc
+            if _data is None:
+                obj = fc(*args, **maps)
+            else:
+                obj = fc(_data)
+            if single:
+                self.objs[key] = obj
+            sets = get(data, "sets", [])
+            self.deal_sets(sets, obj)
+        calls = get(data, "calls", [])
+        self.deal_fcs(calls, obj)
+        if obj is None:
+            if _data is not None:
+                return _data
+            elif val is not None:
+                return val
+            elif args is not None:
+                return args
+            elif maps is not None:
+                return maps
+        return obj
+
+pass
+class Test:
+    def __init__(self, a, b):
+        print("a:", a)
+        self.a = a
+        self.b = b
+    def test(self, obj):
+        print("TEST:", obj)
+    def __call__(self):
+        print(self.a)
+        print(self.b)
+
+pass
+
+import sys
+import os
+def main(paths, default_import = g_default_import, ref_this = "this"):
+    builder = Builder(1, default_import = default_import, ref_this = ref_this)
+    for path in paths:
+        if os.path.isfile(path):
+            builder.add_file(path)
+        elif os.path.isdir(path):
+            files = os.listdir(path)
+            files = [os.path.join(path, file) for file in files]
+            [builder.add_file(file) for file in files]
+        else:
+            print("what is this? :", path)
+    builder.run("main")
+
+pass
+import os
+import re
+class Pattern:
+    def __init__(self, pt):
+        self.pt = pt
+    def __call__(self, s):
+        if self.pt is None:
+            return True
+        return re.findall(self.pt, s)>0
+
+pass
+
+
+def listdir(path, max_depth = -1, pattern = None, nopattern = None, march = None):
+    if max_depth == 0:
+        return []
+    files = os.listdir(path)
+    pt = Pattern(pattern)
+    files = [os.path.join(path, file) for file in files]
+    rst = []
+    for file in files:
+        if os.path.isdir(file):
+            rst += listdir(file, max_depth-1, pattern)
+        else:
+            if pt(os.path.basename(file)):
+                rst.append(file)
+    return rst
+
+pass
+
+    
+def test():
+    builder = Builder(1)
+    argv = sys.argv[1:]
+    main(argv)
+
+pass
+
+if __name__=="__main__":
+    test()
+
+pass
+
```

### Comparing `buildz-0.2.3/buildz/confz.py` & `buildz-0.2.4/buildz/confz.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,499 +1,499 @@
-#coding=utf-8
-'''
-1, remain char:
-    {}[]()<>:'"#\n,;
-   to write a string contain remain char, user '' or "" or "x3 or 'x3:
-    "hello:world, 'zero'"
-    'hello:world, "zero"'
-    """zero say: "hello, 'world'" """
-2, from string to obj:
-    read(s)
-3, from obj to string:
-    output(obj)
-4, from filepath to obj:
-    loadfile(filepath)
-5, simple read filepath to string:
-    fread(filepath)
-
-
-example:
-demo.txt:
-[
-    # single line note
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    ###
-        multi-line note
-        1
-        2
-        3
-    ###
-    {
-        test: ":test{}??",
-        val: <10, int>,
-        cost: <10.0, float>,
-        check: <true, bool>,
-        <10, int>: "test"
-    }
-    #multi-line string
-    """test line
-        1
-        2
-        3
-    """
-    1
-    2
-    3
-    # type not string
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-
-code:
-
-obj = confz.loadfile("demo.txt")
-obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
-
-s = confz.output(obj)
-print(s):
-[
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
-    "test line
-        1
-        2
-        3
-    "
-    1
-    2
-    3
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-'''
-global G_DEBUG
-G_DEBUG = False
-def debug(on = True):
-    global G_DEBUG
-    G_DEBUG = on
-
-pass
-
-coding="utf-8"
-def bread(filepath):
-    with open(filepath, 'rb') as file:
-        s = file.read()
-    return s
-
-pass
-def decode(s, coding = 'utf-8'):
-    coding = coding.lower()
-    xcoding = 'utf-8'
-    if coding == 'utf-8':
-        xcoding = 'gbk'
-    try:
-        return s.decode(coding)
-    except:
-        return s.decode(xcoding)
-
-pass
-def decode_c(s, coding = 'utf-8'):
-    coding = coding.lower()
-    xcoding = 'utf-8'
-    if coding == 'utf-8':
-        xcoding = 'gbk'
-    try:
-        return s.decode(coding), coding
-    except:
-        return s.decode(xcoding), xcoding
-
-pass
-def fread(filepath, coding = 'utf-8'):
-    s = bread(filepath)
-    return decode(s, coding)
-
-pass
-def fread_c(filepath, coding = 'utf-8'):
-    s = bread(filepath)
-    return decode_c(s, coding)
-
-pass
-def load(md, fc = None):
-    arr = md.split(".")[1:]
-    md = __import__(md)
-    for k in arr:
-        md = getattr(md, k)
-    if fc is not None:
-        fc = getattr(md, fc)
-    else:
-        fc = md
-    return fc
-
-pass
-def sread(s):
-    s = s.strip()
-    if s == "":
-        raise Exception("SR Empty")
-    c = s[0]
-    if c == '#':
-        if s[:3].count(c) < 3:
-            j = s.find("\n")
-            if j < 0:
-                return s, ""
-            a = s[:j+1].strip()
-            b = s[j+1:]
-            return a, b
-    if c == '/':
-        if s[:2].count(c) == 2:
-            j = s.find("\n")
-            if j < 0:
-                return s, ""
-            a = s[:j+1].strip()
-            b = s[j+1:]
-            return a, b
-    if c in "{}[]():<>":
-        return c, s[1:]
-    if c in ['"', "'", '#']:
-        k = s[:3]
-        if k.count(c)==3:
-            j = s[3:].find(k)
-            if j < 0:
-                raise Exception("SR q3:"+k)
-            k = j
-            a = s[:j+3+3].strip()
-            b = s[j+3+3:]
-            return a, b
-        j = s[1:].find(c)
-        if j < 0:
-            raise Exception("SR qt:"+c)
-        a = s[:j+2].strip()
-        b = s[j+2:]
-        return a, b
-    for i in range(len(s)):
-        k = s[i]
-        if k in "{}[]()<>:'\"#":
-            return s[:i].strip(), s[i:]
-        if k in '\n,;':
-            return s[:i].strip(), s[i+1:]
-    return s.strip(), ""
-
-pass
-def q3(s):
-    if s=="":
-        return False
-    c = s[0]
-    if c not in ["'", '"']:
-        return False
-    return s[:3].count(c)==3
-
-pass
-def qt(s):
-    if s=="":
-        return False
-    return s[0] in ['"', "'"]
-
-pass
-def note(s):
-    if s=="":
-        return True
-    if s[:2] == "//":
-        return True
-    return s[0] == "#"
-
-pass
-class Key:
-    def __init__(self, c):
-        self.c = c
-    def __str__(self):
-        return "<obj "+self.c+">"
-    def __repr__(self):
-        return str(self)
-
-pass
-g_keys = "{}[]()<>:'\"#\n,;"
-g_keys = {k:Key(k) for k in g_keys}
-
-def s2i(s):
-    global g_keys
-    return [g_keys[k] for k in s]
-    return list(s.encode("ascii"))
-
-pass
-def c2i(s):
-    global g_keys
-    return g_keys[s]
-    return s.encode("ascii")[0]
-
-pass
-
-
-def getList(stack):
-    rst = []
-    while len(stack)>0:
-        w = stack.pop(-1)
-        if w in s2i("[("):
-            rst.reverse()
-            return rst
-        rst.append(w)
-    raise Exception("getList not [")
-
-pass
-
-def getDict(stack):
-    rst = {}
-    lst = []
-    while len(stack)>0:
-        w = stack.pop(-1)
-        if w == c2i("{"):
-            lst.reverse()
-            for k in lst:
-                rst[k[0]] = k[1]
-            return rst
-        lst.append(w)
-    raise Exception("getDict not {")
-
-pass
-
-def getStr(s):
-    s = s.strip()
-    if s == "":
-        return
-    c = s[0]
-    if c not in ['"', "'"]:
-        return s
-    if s[:3].count(c)<3:
-        return s[1:-1]
-    return s[3:-3]
-
-pass
-
-g_bools = {}
-g_bools['true'] = True
-g_bools['1'] = True
-g_bools['false'] = False
-g_bools['0'] = False
-g_bools[''] = False
-
-def get_bool(s):
-    global g_bools
-    s = s.lower()
-    if s not in g_bools:
-        raise Exception("Error g_bools val: "+s)
-    return g_bools[s]
-
-pass
-def get_none(s):
-    return None
-
-pass
-g_types = {}
-g_types['int'] = int
-g_types['float'] = float
-g_types['str'] = str
-g_types['bool'] = get_bool
-g_types['null'] = get_none
-
-
-g_rtypes = {}
-g_rtypes[int] = 'int'
-g_rtypes[float] = 'float'
-g_rtypes[str] = 'str'
-g_rtypes[bool] = 'bool'
-g_rtypes[type(None)] = 'null'
-def getVal(stack):
-    global g_types
-    rst = []
-    while len(stack)>0:
-        w = stack.pop(-1)
-        if w in s2i("<"):
-            rst.reverse()
-            if len(rst)==1:
-                rst.append("str")
-            if rst[1] not in g_types:
-                raise Exception("Error <type>: "+rst[1])
-            return g_types[rst[1]](rst[0].strip())
-        rst.append(w)
-    raise Exception("getVal not <")
-
-pass
-def symbol(w):
-    return type(w) == Key
-    return type(w)==int
-
-pass
-def get(obj, key, default = None):
-    if key not in obj:
-        return default
-    return obj[key]
-
-pass
-paths = []
-def read(s, path = None):
-    global paths
-    if path is not None:
-        paths.append(path)
-    stack = []
-    while s != "":
-        if G_DEBUG:
-            print("stack:", stack)
-        w, s = sread(s)
-        #print("w:", w)
-        w = w.strip()
-        if note(w):
-            continue
-        if w in "])":
-            obj = getList(stack)
-            stack.append(obj)
-        elif w in "[({<:":
-            stack.append(c2i(w))
-        elif w == ">":
-            obj = getVal(stack)
-            stack.append(obj)
-        elif w == "}":
-            obj = getDict(stack)
-            stack.append(obj)
-        else:
-            w = getStr(w)
-            stack.append(w)
-        if len(stack)>=3:
-            k = stack[-2]
-            if k == c2i(":"):
-                v = stack[-1]
-                if not symbol(v):
-                    val = stack.pop(-1)
-                    stack.pop(-1)
-                    key = stack.pop(-1)
-                    stack.append([key, val])
-    if G_DEBUG:
-        print("stack:", stack)
-    if path is not None:
-        paths.pop(-1)
-    return stack.pop(-1)
-
-pass
-loads = read
-import os
-def loadfile(filepath, coding="utf-8"):
-    global paths
-    if len(paths)>0:
-        if filepath[0] not in ["/", "\\\\"] and filepath.find(":")<0:
-            filepath = os.path.join(paths[-1], filepath)
-    return read(fread(filepath, coding=coding), os.path.dirname(filepath))
-
-pass
-g_types['file'] = loadfile
-import re
-def need_qt(s):
-    pt = "^[a-zA-Z0-9\_\.]+$"
-    return re.match(pt, s) is None
-
-pass
-def out_str(val):
-    global g_rtypes
-    k = type(val)
-    if k not in g_rtypes:
-        raise Exception("Not simple value: "+k)
-    if k == bool:
-        val = str(val).lower()
-    rst = "<"+str(val)+", "+g_rtypes[k]+">"
-    return rst
-
-pass
-def oqt(s):
-    if type(s)!= str:
-        return out_str(s)
-    s = str(s)
-    if '"' in s and "'" in s or "\n" in s:
-        match = '"""'
-        if match in s:
-            match = "'''"
-        return match+s+match
-    if not need_qt(s):
-        return s
-    return '"'+s+'"'
-
-pass
-
-
-def output(data, level = 0, simple = True, orders = [], format = False):
-    rst = []
-    wraps = "()"
-    mark_min = simple
-    if type(data) == dict:
-        wraps = "{}"
-        keys = list(data.keys())
-        keys1 = []
-        for k in keys:
-            if k not in orders:
-                keys1.append(k)
-        keys = orders+keys1
-        for key in keys:
-            val = data[key]
-            if type(val) in [list, dict]:
-                val = output(val, level = level+1, simple = simple, orders = orders, format = format).strip()
-                mark_min = False
-            else:
-                val = oqt(val)
-            rst.append([oqt(key), val])
-        key_map = ": "
-        if not format:
-            key_map = ":"
-        rst = [(key_map.join(k)) for k in rst]
-    elif type(data) in [list,tuple]:
-        wraps = "[]"
-        for val in data:
-            if type(val) in [list, dict]:
-                val = output(val, level = level+1, simple = simple, orders = orders, format = format).strip()
-                mark_min = False
-            else:
-                val = oqt(val)
-            rst.append(val)
-    else:
-        return oqt(data)
-    spt = "\n"
-    spt1 = "\n"
-    spc0 = " "*(level<<2)
-    spc = " "*(level<<2)
-    spc1 = " "*((level+1)<<2)
-    if mark_min:
-        spt1 = ", "
-        spc1 = ""
-        spc = ""
-        spt = ""
-    if not format:
-        spt1 = ","
-        spc1 = ""
-        spc = ""
-        spt = ""
-    rst = [spc1+k for k in rst]
-    rs = spt1.join(rst)
-    rs = spc0+wraps[0]+spt+rs+spt+spc+wraps[1]
-    return rs
-
-pass
-dumps = output
-
-
-def test():
-    import sys
-    fp = sys.argv[1]
-    with open(fp, 'r') as file:
-        s = file.read()
-    rst = read(s)
-    print("rst:", rst)
-
-pass
-
-if __name__=="__main__":
-    test()
-
-pass
+#coding=utf-8
+'''
+1, remain char:
+    {}[]()<>:'"#\n,;
+   to write a string contain remain char, user '' or "" or "x3 or 'x3:
+    "hello:world, 'zero'"
+    'hello:world, "zero"'
+    """zero say: "hello, 'world'" """
+2, from string to obj:
+    read(s)
+3, from obj to string:
+    output(obj)
+4, from filepath to obj:
+    loadfile(filepath)
+5, simple read filepath to string:
+    fread(filepath)
+
+
+example:
+demo.txt:
+[
+    # single line note
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    ###
+        multi-line note
+        1
+        2
+        3
+    ###
+    {
+        test: ":test{}??",
+        val: <10, int>,
+        cost: <10.0, float>,
+        check: <true, bool>,
+        <10, int>: "test"
+    }
+    #multi-line string
+    """test line
+        1
+        2
+        3
+    """
+    1
+    2
+    3
+    # type not string
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+
+code:
+
+obj = confz.loadfile("demo.txt")
+obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
+
+s = confz.output(obj)
+print(s):
+[
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
+    "test line
+        1
+        2
+        3
+    "
+    1
+    2
+    3
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+'''
+global G_DEBUG
+G_DEBUG = False
+def debug(on = True):
+    global G_DEBUG
+    G_DEBUG = on
+
+pass
+
+coding="utf-8"
+def bread(filepath):
+    with open(filepath, 'rb') as file:
+        s = file.read()
+    return s
+
+pass
+def decode(s, coding = 'utf-8'):
+    coding = coding.lower()
+    xcoding = 'utf-8'
+    if coding == 'utf-8':
+        xcoding = 'gbk'
+    try:
+        return s.decode(coding)
+    except:
+        return s.decode(xcoding)
+
+pass
+def decode_c(s, coding = 'utf-8'):
+    coding = coding.lower()
+    xcoding = 'utf-8'
+    if coding == 'utf-8':
+        xcoding = 'gbk'
+    try:
+        return s.decode(coding), coding
+    except:
+        return s.decode(xcoding), xcoding
+
+pass
+def fread(filepath, coding = 'utf-8'):
+    s = bread(filepath)
+    return decode(s, coding)
+
+pass
+def fread_c(filepath, coding = 'utf-8'):
+    s = bread(filepath)
+    return decode_c(s, coding)
+
+pass
+def load(md, fc = None):
+    arr = md.split(".")[1:]
+    md = __import__(md)
+    for k in arr:
+        md = getattr(md, k)
+    if fc is not None:
+        fc = getattr(md, fc)
+    else:
+        fc = md
+    return fc
+
+pass
+def sread(s):
+    s = s.strip()
+    if s == "":
+        raise Exception("SR Empty")
+    c = s[0]
+    if c == '#':
+        if s[:3].count(c) < 3:
+            j = s.find("\n")
+            if j < 0:
+                return s, ""
+            a = s[:j+1].strip()
+            b = s[j+1:]
+            return a, b
+    if c == '/':
+        if s[:2].count(c) == 2:
+            j = s.find("\n")
+            if j < 0:
+                return s, ""
+            a = s[:j+1].strip()
+            b = s[j+1:]
+            return a, b
+    if c in "{}[]():<>":
+        return c, s[1:]
+    if c in ['"', "'", '#']:
+        k = s[:3]
+        if k.count(c)==3:
+            j = s[3:].find(k)
+            if j < 0:
+                raise Exception("SR q3:"+k)
+            k = j
+            a = s[:j+3+3].strip()
+            b = s[j+3+3:]
+            return a, b
+        j = s[1:].find(c)
+        if j < 0:
+            raise Exception("SR qt:"+c)
+        a = s[:j+2].strip()
+        b = s[j+2:]
+        return a, b
+    for i in range(len(s)):
+        k = s[i]
+        if k in "{}[]()<>:'\"#":
+            return s[:i].strip(), s[i:]
+        if k in '\n,;':
+            return s[:i].strip(), s[i+1:]
+    return s.strip(), ""
+
+pass
+def q3(s):
+    if s=="":
+        return False
+    c = s[0]
+    if c not in ["'", '"']:
+        return False
+    return s[:3].count(c)==3
+
+pass
+def qt(s):
+    if s=="":
+        return False
+    return s[0] in ['"', "'"]
+
+pass
+def note(s):
+    if s=="":
+        return True
+    if s[:2] == "//":
+        return True
+    return s[0] == "#"
+
+pass
+class Key:
+    def __init__(self, c):
+        self.c = c
+    def __str__(self):
+        return "<obj "+self.c+">"
+    def __repr__(self):
+        return str(self)
+
+pass
+g_keys = "{}[]()<>:'\"#\n,;"
+g_keys = {k:Key(k) for k in g_keys}
+
+def s2i(s):
+    global g_keys
+    return [g_keys[k] for k in s]
+    return list(s.encode("ascii"))
+
+pass
+def c2i(s):
+    global g_keys
+    return g_keys[s]
+    return s.encode("ascii")[0]
+
+pass
+
+
+def getList(stack):
+    rst = []
+    while len(stack)>0:
+        w = stack.pop(-1)
+        if w in s2i("[("):
+            rst.reverse()
+            return rst
+        rst.append(w)
+    raise Exception("getList not [")
+
+pass
+
+def getDict(stack):
+    rst = {}
+    lst = []
+    while len(stack)>0:
+        w = stack.pop(-1)
+        if w == c2i("{"):
+            lst.reverse()
+            for k in lst:
+                rst[k[0]] = k[1]
+            return rst
+        lst.append(w)
+    raise Exception("getDict not {")
+
+pass
+
+def getStr(s):
+    s = s.strip()
+    if s == "":
+        return
+    c = s[0]
+    if c not in ['"', "'"]:
+        return s
+    if s[:3].count(c)<3:
+        return s[1:-1]
+    return s[3:-3]
+
+pass
+
+g_bools = {}
+g_bools['true'] = True
+g_bools['1'] = True
+g_bools['false'] = False
+g_bools['0'] = False
+g_bools[''] = False
+
+def get_bool(s):
+    global g_bools
+    s = s.lower()
+    if s not in g_bools:
+        raise Exception("Error g_bools val: "+s)
+    return g_bools[s]
+
+pass
+def get_none(s):
+    return None
+
+pass
+g_types = {}
+g_types['int'] = int
+g_types['float'] = float
+g_types['str'] = str
+g_types['bool'] = get_bool
+g_types['null'] = get_none
+
+
+g_rtypes = {}
+g_rtypes[int] = 'int'
+g_rtypes[float] = 'float'
+g_rtypes[str] = 'str'
+g_rtypes[bool] = 'bool'
+g_rtypes[type(None)] = 'null'
+def getVal(stack):
+    global g_types
+    rst = []
+    while len(stack)>0:
+        w = stack.pop(-1)
+        if w in s2i("<"):
+            rst.reverse()
+            if len(rst)==1:
+                rst.append("str")
+            if rst[1] not in g_types:
+                raise Exception("Error <type>: "+rst[1])
+            return g_types[rst[1]](rst[0].strip())
+        rst.append(w)
+    raise Exception("getVal not <")
+
+pass
+def symbol(w):
+    return type(w) == Key
+    return type(w)==int
+
+pass
+def get(obj, key, default = None):
+    if key not in obj:
+        return default
+    return obj[key]
+
+pass
+paths = []
+def read(s, path = None):
+    global paths
+    if path is not None:
+        paths.append(path)
+    stack = []
+    while s != "":
+        if G_DEBUG:
+            print("stack:", stack)
+        w, s = sread(s)
+        #print("w:", w)
+        w = w.strip()
+        if note(w):
+            continue
+        if w in "])":
+            obj = getList(stack)
+            stack.append(obj)
+        elif w in "[({<:":
+            stack.append(c2i(w))
+        elif w == ">":
+            obj = getVal(stack)
+            stack.append(obj)
+        elif w == "}":
+            obj = getDict(stack)
+            stack.append(obj)
+        else:
+            w = getStr(w)
+            stack.append(w)
+        if len(stack)>=3:
+            k = stack[-2]
+            if k == c2i(":"):
+                v = stack[-1]
+                if not symbol(v):
+                    val = stack.pop(-1)
+                    stack.pop(-1)
+                    key = stack.pop(-1)
+                    stack.append([key, val])
+    if G_DEBUG:
+        print("stack:", stack)
+    if path is not None:
+        paths.pop(-1)
+    return stack.pop(-1)
+
+pass
+loads = read
+import os
+def loadfile(filepath, coding="utf-8"):
+    global paths
+    if len(paths)>0:
+        if filepath[0] not in ["/", "\\\\"] and filepath.find(":")<0:
+            filepath = os.path.join(paths[-1], filepath)
+    return read(fread(filepath, coding=coding), os.path.dirname(filepath))
+
+pass
+g_types['file'] = loadfile
+import re
+def need_qt(s):
+    pt = "^[a-zA-Z0-9\_\.]+$"
+    return re.match(pt, s) is None
+
+pass
+def out_str(val):
+    global g_rtypes
+    k = type(val)
+    if k not in g_rtypes:
+        raise Exception("Not simple value: "+k)
+    if k == bool:
+        val = str(val).lower()
+    rst = "<"+str(val)+", "+g_rtypes[k]+">"
+    return rst
+
+pass
+def oqt(s):
+    if type(s)!= str:
+        return out_str(s)
+    s = str(s)
+    if '"' in s and "'" in s or "\n" in s:
+        match = '"""'
+        if match in s:
+            match = "'''"
+        return match+s+match
+    if not need_qt(s):
+        return s
+    return '"'+s+'"'
+
+pass
+
+
+def output(data, level = 0, simple = True, orders = [], format = False):
+    rst = []
+    wraps = "()"
+    mark_min = simple
+    if type(data) == dict:
+        wraps = "{}"
+        keys = list(data.keys())
+        keys1 = []
+        for k in keys:
+            if k not in orders:
+                keys1.append(k)
+        keys = orders+keys1
+        for key in keys:
+            val = data[key]
+            if type(val) in [list, dict]:
+                val = output(val, level = level+1, simple = simple, orders = orders, format = format).strip()
+                mark_min = False
+            else:
+                val = oqt(val)
+            rst.append([oqt(key), val])
+        key_map = ": "
+        if not format:
+            key_map = ":"
+        rst = [(key_map.join(k)) for k in rst]
+    elif type(data) in [list,tuple]:
+        wraps = "[]"
+        for val in data:
+            if type(val) in [list, dict]:
+                val = output(val, level = level+1, simple = simple, orders = orders, format = format).strip()
+                mark_min = False
+            else:
+                val = oqt(val)
+            rst.append(val)
+    else:
+        return oqt(data)
+    spt = "\n"
+    spt1 = "\n"
+    spc0 = " "*(level<<2)
+    spc = " "*(level<<2)
+    spc1 = " "*((level+1)<<2)
+    if mark_min:
+        spt1 = ", "
+        spc1 = ""
+        spc = ""
+        spt = ""
+    if not format:
+        spt1 = ","
+        spc1 = ""
+        spc = ""
+        spt = ""
+    rst = [spc1+k for k in rst]
+    rs = spt1.join(rst)
+    rs = spc0+wraps[0]+spt+rs+spt+spc+wraps[1]
+    return rs
+
+pass
+dumps = output
+
+
+def test():
+    import sys
+    fp = sys.argv[1]
+    with open(fp, 'r') as file:
+        s = file.read()
+    rst = read(s)
+    print("rst:", rst)
+
+pass
+
+if __name__=="__main__":
+    test()
+
+pass
```

### Comparing `buildz-0.2.3/buildz.egg-info/PKG-INFO` & `buildz-0.2.4/buildz.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,157 @@
-Metadata-Version: 2.1
-Name: buildz
-Version: 0.2.3
-Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
-Home-page: https://github.com/buildCodeZ/buildz
-Author: Zzz
-Author-email: 1309458652@qq.com
-License: Apache License 2.0
-Keywords: buildz
-Platform: any
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# confz
-```
-一个类似json的数据交换格式，取名叫做confz，并用python实现了读写代码，另外还根据confz写了个代码配置框架
-a json-like file format's read and write code by python, also write a code building framework configure by confz, english description is in "2) english"
-```
-
-## 1) 简介
-```
-1. confz(buildz.confz)
-和json主要区别:
-  1，默认所有值都是字符串，而如果没有包含confz的关键字，不需要用引号引起来；
-  2，换行符\n和逗号,和分号;都作为分割符; 单引号和双引号具有一样的效果
-  3，可以写注释，单行注释用#，多行注释用### 注释 ###
-  4, 字符串可以多行，用'''字符串'''或"""字符串"""
-  5, 如果要confz不把取值当作字符串，要写在尖括号<>里: <数值, 数据类型>，比如整数10写成<10, int>, 浮点数11.1写成<11.1, float>，布尔类型true写成<true, bool>，None写成<-, null>
-写这个东西是为了方便写配置文件和读配置文件，xml感觉有点麻烦，直接用json又要写很多引号，就对json做了简化
-confz的关键字如下:
-  {}[]()<>:'"#\n,;
-一个简单的例子和json作比较:
-  json:
-  {
-    "basedir": "D:\demo",
-    "key": "demo",
-    "maxdepth": 10
-  }
-  confz:
-  {
-    # 基本路径，因为取值包含关键字":", 需要用引号引起来
-    basedir: "D:\demo"
-    # 搜索关键字
-    key: demo
-    # 最大文件深度
-    maxdepth: <10, int>
-  }
-主要方法:
-  read(s): 把confz格式的字符串s转换成object
-  loadfile(s, coding="utf-8"): 从文件s读取confz格式字符串并转换成object，默认编码utf-8
-  output(obj): 把数据obj转换成confz格式字符串，这里要注意的是output输出的字符串做了基本的换行
-目前只有读和写的代码，之后有空的话可能会写一个confz格式校验代码
-
-2. 控制反转框架(buildz.build, buildz.base)
-    根据confz写的控制反转框架（IoC框架）：buildz.Builder或buildz.main
-    具体描述在buildz.keys里，可以调用buildz.keys.help()查看，或者运行"python -m buildz ? ch"来查查，另外包里有个例子可以看下：buildz/demo
-        测试：在demo文件夹中打开命令行，运行：
-            1) python test.py ./demo.confz ./value.confz
-            或
-            2) python test.py ./run.confz
-        1)和2)是等价的，另外如果把buildz当作python来安装，也可以这样运行:
-            1) python -m buildz ./demo.confz ./value.confz
-            或
-            2) python -m buildz ./run.confz
-
-```
-## 2) english:
-```
-1. confz(buildz.confz)
-(1) remain char:
-    {}[]()<>:'"#\n,;
-   to write a string contain remain char, user '' or "" or " x3 or ' x3: 
-    "hello:world, 'zero'" 
-    'hello:world, "zero"'
-    """zero say: "hello, 'world'!" """
-(2) from string to obj:
-    read(s)
-(3) from obj to string:
-    output(obj)
-(4) from filepath to obj:
-    loadfile(filepath, coding="utf-8")
-(5) simple read filepath to string:
-    fread(filepath)
-example:
-demo.txt:
-[
-    # single line note
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    {
-        test: ":test{}??", 
-        val: <10, int>, 
-        cost: <10.0, float>, 
-        check: <true, bool>, 
-        <10, int>: "test"
-    }
-    #multi-line string
-    """test line
-        1
-        2
-        3
-    """
-    1
-    2
-    3
-    # type not string
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-code:
-obj = confz.loadfile("demo.txt")
-obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
-s = confz.output(obj)
-print(s):
-[
-    {
-        filepath: "D:\demo\demo.txt"
-        key: test.com
-        array: [1, 2, 3]
-    }
-    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
-    "test line
-        1
-        2
-        3
-    "
-    1
-    2
-    3
-    <4, int>
-    <5.0, float>
-    <true, bool>
-]
-only realize codes of read and write now,  code of format checking may be writing in future, if I have time.
-PS: None write as <-, null> (confz: '{data: <-,null>}' == json: '{"data":null}')
-2. IoC framework codes(buildz.Builder, buildz.main)
-    description is in buildz.keys, run this code to see: "buildz.keys.help('en')" or "python -m buildz ? en"
-    here is an example in buildz/demo
-    you can open an commond line in demo folder and run like this:
-        1) python test.py ./demo.confz ./value.confz
-        or:
-        2) python test.py ./run.confz
-    1) and 2) is equivalent, besides, if you install buildz as python lib, you can also run like this:
-        1) python -m buildz ./demo.confz ./value.confz
-        or
-        2) python -m buildz ./run.confz
-```
-
-
+Metadata-Version: 2.1
+Name: buildz
+Version: 0.2.4
+Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
+Home-page: https://github.com/buildCodeZ/buildz
+Author: Zzz
+Author-email: 1309458652@qq.com
+License: Apache License 2.0
+Keywords: buildz
+Platform: any
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# confz
+```
+一个类似json的数据交换格式，取名叫做confz，并用python实现了读写代码，另外还根据confz写了个代码配置框架
+a json-like file format's read and write code by python, also write a code building framework configure by confz, english description is in "2) english"
+
+update:
+新增buildz.xconfz，用模式化的代码重构buildz.confz，让代码更容易维护（相应的速度会更慢些），目前只重构了loads
+add sub module buildz.xconfz, which reconstruct buidlz.confz by modularized code, making it easier to update(and run slower), currently only reconstruct method 'loads'
+```
+
+## 1) 简介
+```
+1. confz(buildz.confz)
+和json主要区别:
+  1，默认所有值都是字符串，而如果没有包含confz的关键字，不需要用引号引起来；
+  2，换行符\n和逗号,和分号;都作为分割符; 单引号和双引号具有一样的效果
+  3，可以写注释，单行注释用#，多行注释用### 注释 ###
+  4, 字符串可以多行，用'''字符串'''或"""字符串"""
+  5, 如果要confz不把取值当作字符串，要写在尖括号<>里: <数值, 数据类型>，比如整数10写成<10, int>, 浮点数11.1写成<11.1, float>，布尔类型true写成<true, bool>，None写成<-, null>
+写这个东西是为了方便写配置文件和读配置文件，xml感觉有点麻烦，直接用json又要写很多引号，就对json做了简化
+confz的关键字如下:
+  {}[]()<>:'"#\n,;
+一个简单的例子和json作比较:
+  json:
+  {
+    "basedir": "D:\demo",
+    "key": "demo",
+    "maxdepth": 10
+  }
+  confz:
+  {
+    # 基本路径，因为取值包含关键字":", 需要用引号引起来
+    basedir: "D:\demo"
+    # 搜索关键字
+    key: demo
+    # 最大文件深度
+    maxdepth: <10, int>
+  }
+主要方法:
+  read(s): 把confz格式的字符串s转换成object
+  loadfile(s, coding="utf-8"): 从文件s读取confz格式字符串并转换成object，默认编码utf-8
+  output(obj): 把数据obj转换成confz格式字符串，这里要注意的是output输出的字符串做了基本的换行
+目前只有读和写的代码，之后有空的话可能会写一个confz格式校验代码
+
+2. 控制反转框架(buildz.build, buildz.base)
+    根据confz写的控制反转框架（IoC框架）：buildz.Builder或buildz.main
+    具体描述在buildz.keys里，可以调用buildz.keys.help()查看，或者运行"python -m buildz ? ch"来查查，另外包里有个例子可以看下：buildz/demo
+        测试：在demo文件夹中打开命令行，运行：
+            1) python test.py ./demo.confz ./value.confz
+            或
+            2) python test.py ./run.confz
+        1)和2)是等价的，另外如果把buildz当作python来安装，也可以这样运行:
+            1) python -m buildz ./demo.confz ./value.confz
+            或
+            2) python -m buildz ./run.confz
+
+```
+## 2) english:
+```
+1. confz(buildz.confz)
+(1) remain char:
+    {}[]()<>:'"#\n,;
+   to write a string contain remain char, user '' or "" or " x3 or ' x3: 
+    "hello:world, 'zero'" 
+    'hello:world, "zero"'
+    """zero say: "hello, 'world'!" """
+(2) from string to obj:
+    read(s)
+(3) from obj to string:
+    output(obj)
+(4) from filepath to obj:
+    loadfile(filepath, coding="utf-8")
+(5) simple read filepath to string:
+    fread(filepath)
+example:
+demo.txt:
+[
+    # single line note
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    {
+        test: ":test{}??", 
+        val: <10, int>, 
+        cost: <10.0, float>, 
+        check: <true, bool>, 
+        <10, int>: "test"
+    }
+    #multi-line string
+    """test line
+        1
+        2
+        3
+    """
+    1
+    2
+    3
+    # type not string
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+code:
+obj = confz.loadfile("demo.txt")
+obj: [{'filepath': 'D:\\demo\\demo.txt', 'key': 'test.com', 'array': ['1', '2', '3']}, {'test': ':test{}??', 'val': 10, 'cost': 10.0, 'check': True, 10: 'test'}, 'test line\n        1\n        2\n        3\n    ', '1', '2', '3', 4, 5.0, True]
+s = confz.output(obj)
+print(s):
+[
+    {
+        filepath: "D:\demo\demo.txt"
+        key: test.com
+        array: [1, 2, 3]
+    }
+    {test: ":test{}??", val: <10, int>, cost: <10.0, float>, check: <true, bool>, <10, int>: test}
+    "test line
+        1
+        2
+        3
+    "
+    1
+    2
+    3
+    <4, int>
+    <5.0, float>
+    <true, bool>
+]
+only realize codes of read and write now,  code of format checking may be writing in future, if I have time.
+PS: None write as <-, null> (confz: '{data: <-,null>}' == json: '{"data":null}')
+2. IoC framework codes(buildz.Builder, buildz.main)
+    description is in buildz.keys, run this code to see: "buildz.keys.help('en')" or "python -m buildz ? en"
+    here is an example in buildz/demo
+    you can open an commond line in demo folder and run like this:
+        1) python test.py ./demo.confz ./value.confz
+        or:
+        2) python test.py ./run.confz
+    1) and 2) is equivalent, besides, if you install buildz as python lib, you can also run like this:
+        1) python -m buildz ./demo.confz ./value.confz
+        or
+        2) python -m buildz ./run.confz
+```
+
+
```

### Comparing `buildz-0.2.3/setup.py` & `buildz-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#!/usr/bin/env python
-# -*- coding:utf-8 -*-
-# Author: Zzz(1309458652@qq.com)
-# Description:
-
-from setuptools import setup, find_packages
-
-setup(
-    name = 'buildz',
-    version = '0.2.3',
-    keywords='buildz',
-    long_description=open('README.md', 'r', encoding="utf-8").read(),
-    long_description_content_type='text/markdown',
-    description = "a json-like file format's read and write code by python, and codes to read and product object from configure file in such format",
-    license = 'Apache License 2.0',
-    url = 'https://github.com/buildCodeZ/buildz',
-    author = 'Zzz',
-    author_email = '1309458652@qq.com',
-    packages = find_packages(),
-    include_package_data = True,
-    platforms = 'any',
-    install_requires = [],
+#!/usr/bin/env python
+# -*- coding:utf-8 -*-
+# Author: Zzz(1309458652@qq.com)
+# Description:
+
+from setuptools import setup, find_packages
+
+setup(
+    name = 'buildz',
+    version = '0.2.4',
+    keywords='buildz',
+    long_description=open('README.md', 'r', encoding="utf-8").read(),
+    long_description_content_type='text/markdown',
+    description = "a json-like file format's read and write code by python, and codes to read and product object from configure file in such format",
+    license = 'Apache License 2.0',
+    url = 'https://github.com/buildCodeZ/buildz',
+    author = 'Zzz',
+    author_email = '1309458652@qq.com',
+    packages = find_packages(),
+    include_package_data = True,
+    platforms = 'any',
+    install_requires = [],
 )
```

