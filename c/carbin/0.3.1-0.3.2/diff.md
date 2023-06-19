# Comparing `tmp/carbin-0.3.1-py3-none-any.whl.zip` & `tmp/carbin-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 36309 bytes, number of entries: 21
--rw-rw-r--  2.0 unx      608 b- defN 23-Jun-19 04:41 carbin/__init__.py
+Zip file size: 36599 bytes, number of entries: 21
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jun-19 14:16 carbin/__init__.py
 -rw-rw-r--  2.0 unx     4487 b- defN 23-Jun-19 04:44 carbin/builder.py
--rw-rw-r--  2.0 unx    11428 b- defN 23-Jun-19 05:57 carbin/cli.py
--rw-rw-r--  2.0 unx     4125 b- defN 23-Jun-19 06:52 carbin/creater.py
+-rw-rw-r--  2.0 unx    11425 b- defN 23-Jun-19 12:56 carbin/cli.py
+-rw-rw-r--  2.0 unx     5180 b- defN 23-Jun-19 13:11 carbin/creater.py
 -rw-rw-r--  2.0 unx     4784 b- defN 23-Jun-19 04:42 carbin/package.py
--rw-rw-r--  2.0 unx    21460 b- defN 23-Jun-19 04:46 carbin/prefix.py
+-rw-rw-r--  2.0 unx    21833 b- defN 23-Jun-19 14:16 carbin/prefix.py
 -rw-rw-r--  2.0 unx     2791 b- defN 23-Jun-19 04:42 carbin/types.py
 -rw-rw-r--  2.0 unx    12403 b- defN 23-Jun-19 05:17 carbin/util.py
 -rw-rw-r--  2.0 unx     7513 b- defN 23-May-16 22:05 carbin/cmake/autotools.cmake
 -rw-rw-r--  2.0 unx      512 b- defN 23-May-16 22:05 carbin/cmake/binary.cmake
 -rw-rw-r--  2.0 unx    10396 b- defN 23-Jun-18 16:20 carbin/cmake/boost.cmake
 -rw-rw-r--  2.0 unx     1161 b- defN 23-May-16 22:05 carbin/cmake/header.cmake
 -rw-rw-r--  2.0 unx     6387 b- defN 23-May-16 22:05 carbin/cmake/make.cmake
 -rw-rw-r--  2.0 unx     9225 b- defN 23-May-16 22:05 carbin/cmake/meson.cmake
 -rw-rw-r--  2.0 unx      121 b- defN 23-May-16 22:05 carbin/cmake/subdir.cmake
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      276 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1631 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/RECORD
-21 files, 110806 bytes uncompressed, 33703 bytes compressed:  69.6%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-19 14:20 carbin-0.3.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      276 b- defN 23-Jun-19 14:20 carbin-0.3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 14:20 carbin-0.3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 23-Jun-19 14:20 carbin-0.3.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-19 14:20 carbin-0.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1631 b- defN 23-Jun-19 14:20 carbin-0.3.2.dist-info/RECORD
+21 files, 112231 bytes uncompressed, 33993 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: carbin/cmake/meson.cmake
 Comment: 
 
 Filename: carbin/cmake/subdir.cmake
 Comment: 
 
-Filename: carbin-0.3.1.dist-info/LICENSE
+Filename: carbin-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: carbin-0.3.1.dist-info/METADATA
+Filename: carbin-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: carbin-0.3.1.dist-info/WHEEL
+Filename: carbin-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: carbin-0.3.1.dist-info/entry_points.txt
+Filename: carbin-0.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: carbin-0.3.1.dist-info/top_level.txt
+Filename: carbin-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: carbin-0.3.1.dist-info/RECORD
+Filename: carbin-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## carbin/__init__.py

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = '0.3.1'
+__version__ = '0.3.2'
```

## carbin/cli.py

```diff
@@ -145,18 +145,18 @@
 @click.option('--insecure', is_flag=True, help="Don't use https urls")
 @click.argument('pkgs', nargs=-1, type=click.STRING)
 def install_command(prefix, pkgs, define, file, test, test_all, update, generator, cmake, debug, release, build_type,
                     insecure):
     """ Install packages """
     variant = get_build_type(debug, release, build_type)
     if not file and not pkgs:
-        if os.path.exists('dev-requirements.txt'):
-            file = 'dev-requirements.txt'
+        if os.path.exists('dev-carbin_deps.txt'):
+            file = 'dev-carbin_deps.txt'
         else:
-            file = 'requirements.txt'
+            file = 'carbin_deps.txt'
     pbs = [PackageBuild(pkg, cmake=cmake, variant=variant) for pkg in pkgs]
     for pbu in util.flat([prefix.from_file(file), pbs]):
         pb = pbu.merge_defines(define)
         pb.variant = variant
         with prefix.try_("Failed to build package {}".format(pb.to_name()), on_fail=lambda: prefix.remove(pb)):
             click.echo(
                 prefix.install(pb, test=test, test_all=test_all, update=update, generator=generator, insecure=insecure))
```

## carbin/creater.py

```diff
@@ -114,10 +114,38 @@
     def create_benchmark_dir(self, d):
         if self.benchmark:
             util.mkdir('benchmark')
             src = os.path.join(d, 'benchmark/CMakeLists.txt')
             util.copy_to(src, 'benchmark')
 
     def create_requires_file(self, d):
-        if self.requirements:
-            src = os.path.join(d, 'requirements.txt')
+        if not self.requirements:
+            return
+        if os.path.exists('carbin_deps.txt'):
+            return
+        src = os.path.join(d, 'carbin_deps.txt')
+        if os.path.exists(src):
             util.copy_to(src, '.')
+            return
+        f = fw = open('carbin_deps.txt', 'w')
+        content = '''
+#
+# Copyright 2023 The titan-search Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+###########
+# turbo
+#gottingen/turbo@v0.9.4 -DCARBIN_BUILD_TEST=OFF -DCARBIN_BUILD_BENCHMARK=OFF -DCARBIN_BUILD_EXAMPLES=OFF -DBUILD_SHARED_LIBRARY=OFF -DBUILD_STATIC_LIBRARY=ON -DCMAKE_BUILD_TYPE=release
+        '''
+        f.write(content)
+        f.close()
```

## carbin/prefix.py

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import os, shutil, shlex, six, inspect, click, contextlib, sys, functools
+import os, shutil, shlex, six, inspect, click, contextlib, sys, functools, re
 
 from carbin.builder import Builder
 from carbin.package import fname_to_pkg
 from carbin.package import PackageSource
 from carbin.package import PackageBuild
 from carbin.package import parse_pkg_build_tokens
 import carbin.util as util
@@ -290,15 +290,15 @@
                 return PackageBuild(pkg_src)
 
     def from_recipe(self, recipe, pkg=None, name=None):
         recipe_pkg = os.path.join(recipe, "package.txt")
         util.ensure_exists(recipe_pkg)
         p = next(iter(self.from_file(recipe_pkg, no_recipe=True)))
         self.check(lambda: p.pkg_src is not None)
-        requirements = os.path.join(recipe, "requirements.txt")
+        requirements = os.path.join(recipe, "carbin_deps.txt")
         if os.path.exists(requirements): p.requirements = requirements
         p.pkg_src.recipe = None
         # Use original name
         if pkg:
             p.pkg_src.name = pkg.pkg_src.name
         elif name:
             p.pkg_src.name = name
@@ -315,28 +315,37 @@
             self.log("file not found: " + file)
             return
         start = os.path.dirname(file)
         if url is not None and url.startswith('file://'):
             start = url[7:]
         with open(file) as f:
             self.log("parse file: " + file)
+            cache_line = ""
             for line in f.readlines():
-                tokens = shlex.split(line, comments=True)
+                if str.endswith(line, '\\\n'):
+                    if line.lstrip().startswith('#'):
+                        continue
+                    cache_line = cache_line + line.strip('\\\n')
+                    continue
+                cache_line = cache_line + line
+                print(cache_line)
+                tokens = shlex.split(cache_line, comments=True)
+                cache_line = ""
                 if len(tokens) > 0:
                     pb = parse_pkg_build_tokens(tokens)
                     ps = self.from_file(util.actual_path(pb.file, start), no_recipe=no_recipe) if pb.file else [
                         self.parse_pkg_build(pb, start=start, no_recipe=no_recipe)]
                     for p in ps: yield p
 
     def write_parent(self, pb, track=True):
         if track and pb.parent is not None: util.mkfile(self.get_deps_directory(pb.to_fname()), pb.parent, pb.parent)
 
     def install_deps(self, pb, d, test=False, test_all=False, generator=None, insecure=False,
                      ignore_requirements=False):
-        req_txt = os.path.join(d, 'requirements.txt') if not ignore_requirements else None
+        req_txt = os.path.join(d, 'carbin_deps.txt') if not ignore_requirements else None
         for dependent in self.from_file(pb.requirements or req_txt, pb.pkg_src.url):
             transient = dependent.test or dependent.build
             testing = test or test_all
             installable = not dependent.test or dependent.test == testing
             if installable:
                 self.install(dependent.of(pb), test_all=test_all, generator=generator, track=not transient,
                              insecure=insecure)
@@ -401,18 +410,18 @@
         else:
             return "Package {} already installed".format(pb.to_name())
 
     @params(pb=PACKAGE_SOURCE_TYPES, test=bool)
     def build(self, pb, test=False, target=None, generator=None):
         pb = self.parse_pkg_build(pb)
         src_dir = pb.pkg_src.get_src_dir()
-        if os.path.exists(os.path.join(src_dir, 'dev-requirements.txt')):
-            pb.requirements = os.path.join(src_dir, 'dev-requirements.txt')
-        elif os.path.exists(os.path.join(src_dir, 'requirements.txt')):
-            pb.requirements = os.path.join(src_dir, 'requirements.txt')
+        if os.path.exists(os.path.join(src_dir, 'dev-carbin_deps.txt')):
+            pb.requirements = os.path.join(src_dir, 'dev-carbin_deps.txt')
+        elif os.path.exists(os.path.join(src_dir, 'carbin_deps.txt')):
+            pb.requirements = os.path.join(src_dir, 'carbin_deps.txt')
         with self.create_builder(pb.to_fname()) as builder:
             # Install any dependencies first
             self.install_deps(pb, src_dir, generator=generator, test=test)
             # Configure and build
             if not builder.exists: builder.configure(src_dir, defines=pb.define, generator=generator, test=test,
                                                      variant=pb.variant)
             builder.build(variant=pb.variant, target=target)
```

## Comparing `carbin-0.3.1.dist-info/LICENSE` & `carbin-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `carbin-0.3.1.dist-info/RECORD` & `carbin-0.3.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-carbin/__init__.py,sha256=6eiWnshoqP6EqMzIhcEv_A8lX8TtdZVkBoDgTUTz7kI,608
+carbin/__init__.py,sha256=4vwsqXdXykjLgW5FIarpg1C7cbg-ihF30TkClQwAErU,608
 carbin/builder.py,sha256=gG7D9hqDE-S_GfROafz2pdfIyB8y8wEwQocNz4NQY-o,4487
-carbin/cli.py,sha256=AXKMfFFObXb0r845OvlZYvgnxBoDFgaLZpo51Dr4_XI,11428
-carbin/creater.py,sha256=TKvIbpl_qHwFZNMZWgWK8VBHdb3njvVM-D2_UmPBsRY,4125
+carbin/cli.py,sha256=FpcseE1LzIgLBp03WUz3dYPOl_ZZzvmEiMBEnmHYb9U,11425
+carbin/creater.py,sha256=yaywRSNsJpsJsnI0HNcZa5gNxc5fZ5m8H9cpLn24KUo,5180
 carbin/package.py,sha256=j3DeKkhh9YhWe0i8LvJis1OGLzlBF_RRptvOy_XACnQ,4784
-carbin/prefix.py,sha256=gUdTZXnLm7uTrChfCvdFnoZG2B-glUY4qlo4oZ_sYgk,21460
+carbin/prefix.py,sha256=EnJRQ69nG6Kdufc_dQH7U6eN_931g-1DNskZbGgaSdU,21833
 carbin/types.py,sha256=YF4e-RDaDO4Y7i8mMTTcS78RnZkCMxRvmhOPruBzljo,2791
 carbin/util.py,sha256=-6SNYfU8IE6NgjSe4VhlzXJfGDh47D63PNi5ERU3ApQ,12403
 carbin/cmake/autotools.cmake,sha256=asyjvKRMFpSlaZMeMP44-hcw0arGWJGTbfujD95Vo5s,7513
 carbin/cmake/binary.cmake,sha256=lwu9TbC9Ni0Zb7KsrPh98RBRD3D2gS6R4V5MWYRkGB0,512
 carbin/cmake/boost.cmake,sha256=lrFDFluYtng6Lyi2O8KpIW8E6YHucnHv7d2CREJmwsA,10396
 carbin/cmake/header.cmake,sha256=CHyFepXmujahMo5QPs703EsfT2YLgK1FDDuv0O4JmRY,1161
 carbin/cmake/make.cmake,sha256=zX7sr2hA7PMsKJ09RyGzrvxZbpW84uOYcuzpCWVQCes,6387
 carbin/cmake/meson.cmake,sha256=bQ5SnqPuPKUaIWmcWCcV2V91MoSeYdRRHQeWP88TzfY,9225
 carbin/cmake/subdir.cmake,sha256=wxpubdxBKoAnjYUV8Mizxq_YymtwPm3iUjN5Dh3YWNU,121
-carbin-0.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-carbin-0.3.1.dist-info/METADATA,sha256=B0_vafO0JWl74wJ-9nnolzkAnGuUgTiCsruGYXNpGXQ,276
-carbin-0.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-carbin-0.3.1.dist-info/entry_points.txt,sha256=ibqGDVfvnT2ZzaMDaRB5PgOjVdrprvlsAJLrYTjGgHY,42
-carbin-0.3.1.dist-info/top_level.txt,sha256=qRZoXL__kMXE03dJArRq6hL4sOoXUbeufIL5RjVroV4,7
-carbin-0.3.1.dist-info/RECORD,,
+carbin-0.3.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+carbin-0.3.2.dist-info/METADATA,sha256=3pOAsq5qrQHaxfKZ0UuL8KxQG2NcpcSmOzuZZKAZQj0,276
+carbin-0.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+carbin-0.3.2.dist-info/entry_points.txt,sha256=ibqGDVfvnT2ZzaMDaRB5PgOjVdrprvlsAJLrYTjGgHY,42
+carbin-0.3.2.dist-info/top_level.txt,sha256=qRZoXL__kMXE03dJArRq6hL4sOoXUbeufIL5RjVroV4,7
+carbin-0.3.2.dist-info/RECORD,,
```

