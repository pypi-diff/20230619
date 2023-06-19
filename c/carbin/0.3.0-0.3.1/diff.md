# Comparing `tmp/carbin-0.3.0-py3-none-any.whl.zip` & `tmp/carbin-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 32244 bytes, number of entries: 20
--rw-rw-r--  2.0 unx       23 b- defN 23-Jun-18 16:57 carbin/__init__.py
--rw-rw-r--  2.0 unx     3900 b- defN 23-Jun-18 16:22 carbin/builder.py
--rw-rw-r--  2.0 unx    10030 b- defN 23-Jun-18 16:22 carbin/cli.py
--rw-rw-r--  2.0 unx     4198 b- defN 23-Jun-18 16:10 carbin/package.py
--rw-rw-r--  2.0 unx    20049 b- defN 23-Jun-18 16:22 carbin/prefix.py
--rw-rw-r--  2.0 unx     2205 b- defN 23-May-16 22:05 carbin/types.py
--rw-rw-r--  2.0 unx    11812 b- defN 23-Jun-18 16:22 carbin/util.py
+Zip file size: 36309 bytes, number of entries: 21
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jun-19 04:41 carbin/__init__.py
+-rw-rw-r--  2.0 unx     4487 b- defN 23-Jun-19 04:44 carbin/builder.py
+-rw-rw-r--  2.0 unx    11428 b- defN 23-Jun-19 05:57 carbin/cli.py
+-rw-rw-r--  2.0 unx     4125 b- defN 23-Jun-19 06:52 carbin/creater.py
+-rw-rw-r--  2.0 unx     4784 b- defN 23-Jun-19 04:42 carbin/package.py
+-rw-rw-r--  2.0 unx    21460 b- defN 23-Jun-19 04:46 carbin/prefix.py
+-rw-rw-r--  2.0 unx     2791 b- defN 23-Jun-19 04:42 carbin/types.py
+-rw-rw-r--  2.0 unx    12403 b- defN 23-Jun-19 05:17 carbin/util.py
 -rw-rw-r--  2.0 unx     7513 b- defN 23-May-16 22:05 carbin/cmake/autotools.cmake
 -rw-rw-r--  2.0 unx      512 b- defN 23-May-16 22:05 carbin/cmake/binary.cmake
 -rw-rw-r--  2.0 unx    10396 b- defN 23-Jun-18 16:20 carbin/cmake/boost.cmake
 -rw-rw-r--  2.0 unx     1161 b- defN 23-May-16 22:05 carbin/cmake/header.cmake
 -rw-rw-r--  2.0 unx     6387 b- defN 23-May-16 22:05 carbin/cmake/make.cmake
 -rw-rw-r--  2.0 unx     9225 b- defN 23-May-16 22:05 carbin/cmake/meson.cmake
 -rw-rw-r--  2.0 unx      121 b- defN 23-May-16 22:05 carbin/cmake/subdir.cmake
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-18 16:58 carbin-0.3.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      276 b- defN 23-Jun-18 16:58 carbin-0.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-18 16:58 carbin-0.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 23-Jun-18 16:58 carbin-0.3.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-18 16:58 carbin-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1556 b- defN 23-Jun-18 16:58 carbin-0.3.0.dist-info/RECORD
-20 files, 100862 bytes uncompressed, 29748 bytes compressed:  70.5%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      276 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1631 b- defN 23-Jun-19 06:57 carbin-0.3.1.dist-info/RECORD
+21 files, 110806 bytes uncompressed, 33703 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: carbin/builder.py
 Comment: 
 
 Filename: carbin/cli.py
 Comment: 
 
+Filename: carbin/creater.py
+Comment: 
+
 Filename: carbin/package.py
 Comment: 
 
 Filename: carbin/prefix.py
 Comment: 
 
 Filename: carbin/types.py
@@ -36,26 +39,26 @@
 
 Filename: carbin/cmake/meson.cmake
 Comment: 
 
 Filename: carbin/cmake/subdir.cmake
 Comment: 
 
-Filename: carbin-0.3.0.dist-info/LICENSE
+Filename: carbin-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: carbin-0.3.0.dist-info/METADATA
+Filename: carbin-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: carbin-0.3.0.dist-info/WHEEL
+Filename: carbin-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: carbin-0.3.0.dist-info/entry_points.txt
+Filename: carbin-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: carbin-0.3.0.dist-info/top_level.txt
+Filename: carbin-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: carbin-0.3.0.dist-info/RECORD
+Filename: carbin-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## carbin/__init__.py

```diff
@@ -1,2 +1,16 @@
-
-__version__ = '0.3.0'
+#
+# Copyright 2023 The Turbo Authors.
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
+__version__ = '0.3.1'
```

## carbin/builder.py

```diff
@@ -1,11 +1,27 @@
+#
+# Copyright 2023 The Turbo Authors.
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
 import click, os, multiprocessing, six
 
 import carbin.util as util
 
+
 class Builder:
     def __init__(self, prefix, top_dir, exists=False):
         self.prefix = prefix
         self.top_dir = top_dir
         self.build_dir = self.get_path('build')
         self.exists = exists
         self.cmake_original_file = '__carbin_original_cmake_file__.cmake'
```

## carbin/cli.py

```diff
@@ -1,15 +1,30 @@
+#
+# Copyright 2023 The Turbo Authors.
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
 import click, os, functools, sys
 
 from carbin import __version__
 from carbin.prefix import CarbinPrefix
 from carbin.prefix import PackageBuild
+from carbin.creater import Creater
 import carbin.util as util
 
-
 aliases = {
     'rm': 'remove',
     'ls': 'list'
 }
 
 
 def get_build_type(debug, release, build_type):
@@ -40,33 +55,52 @@
         return None
 
 
 @click.group(cls=AliasedGroup, context_settings={'help_option_names': ['-h', '--help']})
 @click.version_option(version=__version__, prog_name='carbin')
 @click.option('-p', '--prefix', envvar='CARBIN_PREFIX', help='Set prefix used to install packages')
 @click.option('-v', '--verbose', is_flag=True, envvar='VERBOSE', help="Enable verbose mode")
-@click.option('-B', '--build-path', envvar='CARBIN_BUILD_PATH', help='Set the path for the build directory to use when building the package')
+@click.option('-B', '--build-path', envvar='CARBIN_BUILD_PATH',
+              help='Set the path for the build directory to use when building the package')
 @click.pass_context
 def cli(ctx, prefix, verbose, build_path):
     ctx.obj = {}
     if prefix: ctx.obj['PREFIX'] = prefix
     if verbose: ctx.obj['VERBOSE'] = verbose
     if build_path: ctx.obj['BUILD_PATH'] = build_path
 
+
 def use_prefix(f):
     @click.option('-p', '--prefix', help='Set prefix used to install packages')
     @click.option('-v', '--verbose', is_flag=True, help="Enable verbose mode")
     @click.option('-B', '--build-path', help='Set the path for the build directory to use when building the package')
     @click.pass_obj
     @functools.wraps(f)
     def w(obj, prefix, verbose, build_path, *args, **kwargs):
-        p = CarbinPrefix(prefix or obj.get('PREFIX'), verbose or obj.get('VERBOSE'), build_path or obj.get('BUILD_PATH'))
+        p = CarbinPrefix(prefix or obj.get('PREFIX'), verbose or obj.get('VERBOSE'),
+                         build_path or obj.get('BUILD_PATH'))
         f(p, *args, **kwargs)
+
     return w
 
+
+@cli.command(name='create')
+@use_prefix
+@click.option('--name', required=True, help="Set cmake template")
+@click.option('--test', is_flag=True, help="Create test Dir")
+@click.option('--examples', is_flag=True, help="Create test Dir")
+@click.option('--benchmark', is_flag=True, help="Create test Dir")
+@click.option('--requirements', is_flag=True, help="Create test Dir")
+def create_command(prefix, name, test, examples, benchmark, requirements):
+    print("create cmd\n")
+    c = Creater(prefix, name, test, examples, benchmark, requirements)
+    c.create_project()
+    click.echo('done...')
+
+
 @cli.command(name='init')
 @use_prefix
 @click.option('-t', '--toolchain', required=False, help="Set cmake toolchain file to use")
 @click.option('--cc', required=False, help="Set c compiler")
 @click.option('--cxx', required=False, help="Set c++ compiler")
 @click.option('--cflags', required=False, help="Set additional c flags")
 @click.option('--cxxflags', required=False, help="Set additional c++ flags")
@@ -80,86 +114,99 @@
     if shared and static:
         click.echo("ERROR: shared and static are not supported together")
         sys.exit(1)
     defines = util.to_define_dict(define)
     if shared: defines['BUILD_SHARED_LIBS'] = 'On'
     if static: defines['BUILD_SHARED_LIBS'] = 'Off'
     prefix.write_cmake(
-        always_write=True, 
-        toolchain=toolchain, 
+        always_write=True,
+        toolchain=toolchain,
         cc=cc,
         cxx=cxx,
-        cflags=cflags, 
-        cxxflags=cxxflags, 
-        ldflags=ldflags, 
-        std=std, 
+        cflags=cflags,
+        cxxflags=cxxflags,
+        ldflags=ldflags,
+        std=std,
         defines=defines)
 
+
 @cli.command(name='install')
 @use_prefix
 @click.option('-U', '--update', is_flag=True, help="Update package")
 @click.option('-t', '--test', is_flag=True, help="Test package before installing by running ctest or check target")
-@click.option('--test-all', is_flag=True, help="Test all packages including its dependencies before installing by running ctest or check target")
+@click.option('--test-all', is_flag=True,
+              help="Test all packages including its dependencies before installing by running ctest or check target")
 @click.option('-f', '--file', default=None, help="Install packages listed in the file")
 @click.option('-D', '--define', multiple=True, help="Extra configuration variables to pass to CMake")
 @click.option('-G', '--generator', envvar='CARBIN_GENERATOR', help='Set the generator for CMake to use')
 @click.option('-X', '--cmake', help='Set cmake file to use to build project')
 @click.option('--debug', is_flag=True, help="Install debug version")
 @click.option('--release', is_flag=True, help="Install release version")
 @click.option('--build-type', help="Install custom version [Release, Debug, RelWithDebInfo or other cmake build type]")
 @click.option('--insecure', is_flag=True, help="Don't use https urls")
 @click.argument('pkgs', nargs=-1, type=click.STRING)
-def install_command(prefix, pkgs, define, file, test, test_all, update, generator, cmake, debug, release, build_type, insecure):
+def install_command(prefix, pkgs, define, file, test, test_all, update, generator, cmake, debug, release, build_type,
+                    insecure):
     """ Install packages """
     variant = get_build_type(debug, release, build_type)
     if not file and not pkgs:
-        if os.path.exists('dev-requirements.txt'): file = 'dev-requirements.txt'
-        else: file = 'requirements.txt'
+        if os.path.exists('dev-requirements.txt'):
+            file = 'dev-requirements.txt'
+        else:
+            file = 'requirements.txt'
     pbs = [PackageBuild(pkg, cmake=cmake, variant=variant) for pkg in pkgs]
     for pbu in util.flat([prefix.from_file(file), pbs]):
         pb = pbu.merge_defines(define)
         pb.variant = variant
         with prefix.try_("Failed to build package {}".format(pb.to_name()), on_fail=lambda: prefix.remove(pb)):
-            click.echo(prefix.install(pb, test=test, test_all=test_all, update=update, generator=generator, insecure=insecure))
+            click.echo(
+                prefix.install(pb, test=test, test_all=test_all, update=update, generator=generator, insecure=insecure))
+
 
 @cli.command(name='ignore')
 @use_prefix
 @click.argument('pkgs', nargs=-1, type=click.STRING)
 def ignore_command(prefix, pkgs):
     """ Ignore packages """
     pbs = [PackageBuild(pkg) for pkg in pkgs]
     for pb in pbs:
         with prefix.try_("Failed to ignore package {}".format(pb.to_name()), on_fail=lambda: prefix.remove(pb)):
             click.echo(prefix.ignore(pb))
 
+
 @cli.command(name='build')
 @use_prefix
 @click.option('-t', '--test', is_flag=True, help="Test package by running ctest or check target")
 @click.option('-c', '--configure', is_flag=True, help="Configure cmake")
 @click.option('-C', '--clean', is_flag=True, help="Remove build directory")
 @click.option('-P', '--path', is_flag=True, help="Show path to build directory")
 @click.option('-D', '--define', multiple=True, help="Extra configuration variables to pass to CMake")
 @click.option('-T', '--target', default=None, help="Cmake target to build")
 @click.option('-y', '--yes', is_flag=True, default=False)
 @click.option('-G', '--generator', envvar='CARBIN_GENERATOR', help='Set the generator for CMake to use')
 @click.option('--debug', is_flag=True, help="Build debug version")
 @click.option('--release', is_flag=True, help="Build release version")
 @click.option('--build-type', help="Install custom version [Release, Debug, RelWithDebInfo or other cmake build type]")
 @click.argument('pkg', nargs=1, default='.', type=click.STRING)
-def build_command(prefix, pkg, define, test, configure, clean, path, yes, target, generator, debug, release, build_type):
+def build_command(prefix, pkg, define, test, configure, clean, path, yes, target, generator, debug, release,
+                  build_type):
     """ Build package """
     pb = PackageBuild(pkg).merge_defines(define)
     pb.variant = get_build_type(debug, release, build_type)
     with prefix.try_("Failed to build package {}".format(pb.to_name())):
-        if configure: prefix.build_configure(pb)
-        elif path: click.echo(prefix.build_path(pb))
-        elif clean: 
+        if configure:
+            prefix.build_configure(pb)
+        elif path:
+            click.echo(prefix.build_path(pb))
+        elif clean:
             if not yes: yes = click.confirm("Are you sure you want to delete the build directory?")
             if yes: prefix.build_clean(pb)
-        else: prefix.build(pb, test=test, target=target, generator=generator)
+        else:
+            prefix.build(pb, test=test, target=target, generator=generator)
+
 
 @cli.command(name='remove')
 @use_prefix
 @click.argument('pkgs', nargs=-1, type=click.STRING)
 @click.option('-y', '--yes', is_flag=True, default=False)
 @click.option('-U', '--unlink', is_flag=True, default=False, help="Unlink package but don't remove it")
 @click.option('-A', '--all', is_flag=True, default=False, help="Select all packages installed")
@@ -173,48 +220,52 @@
     if not yes: yes = click.confirm("Are you sure you want to {} these packages?".format(verb))
     if yes:
         for pkg in pkgs_set:
             with prefix.try_("Failed to {} package {}".format(verb, pkg)):
                 prefix.unlink(pkg, delete=not unlink)
                 click.echo("{} package {}".format(verb, pkg))
 
+
 @cli.command(name='list')
 @use_prefix
 def list_command(prefix):
     """ List installed packages """
     for pkg in prefix.list():
         click.echo(pkg.name)
 
+
 # TODO: Make this command hidden
 @cli.command(name='size')
 @use_prefix
 @click.argument('n')
 def size_command(prefix, n):
     pkgs = len(list(util.ls(prefix.get_package_directory(), os.path.isdir)))
     if pkgs != int(n):
         raise util.BuildError("Not the correct number of items: {}".format(pkgs))
 
+
 @cli.command(name='clean')
 @use_prefix
 @click.option('-y', '--yes', is_flag=True, default=False)
 @click.option('--cache', is_flag=True, default=False, help="Removes any cache files")
 def clean_command(prefix, yes, cache):
     """ Clear directory """
     if cache:
         prefix.clean_cache()
     else:
-        if not yes: yes = click.confirm("Are you sure you want to delete all carbin packages in {}?".format(prefix.prefix))
+        if not yes: yes = click.confirm(
+            "Are you sure you want to delete all carbin packages in {}?".format(prefix.prefix))
         if yes: prefix.clean()
 
+
 @cli.command(name='pkg-config', context_settings=dict(
     ignore_unknown_options=True,
 ))
 @use_prefix
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 def pkg_config_command(prefix, args):
     """ Pkg config """
     prefix.cmd.pkg_config(args)
 
 
 if __name__ == '__main__':
     cli()
-
```

## carbin/package.py

```diff
@@ -1,7 +1,22 @@
+#
+# Copyright 2023 The Turbo Authors.
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
 import base64, copy, argparse, six, hashlib
 
 
 def encode_url(url):
     x = six.b(url[url.find('://') + 3:])
     return '_url_' + base64.urlsafe_b64encode(x).decode('utf-8').replace('=', '_')
```

## carbin/prefix.py

```diff
@@ -1,99 +1,129 @@
+#
+# Copyright 2023 The Turbo Authors.
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
 import os, shutil, shlex, six, inspect, click, contextlib, sys, functools
 
 from carbin.builder import Builder
 from carbin.package import fname_to_pkg
 from carbin.package import PackageSource
 from carbin.package import PackageBuild
 from carbin.package import parse_pkg_build_tokens
 import carbin.util as util
 from carbin.types import returns
 from carbin.types import params
 
 __CARBIN_DIR__ = os.path.dirname(os.path.realpath(__file__))
 __CARBIN_CMAKE_DIR__ = os.path.join(__CARBIN_DIR__, 'cmake')
 
+
 @params(s=six.string_types)
 def parse_deprecated_alias(s):
     i = s.find(':', 0, max(s.find('://'), s.find(':\\')))
-    if i > 0: 
+    if i > 0:
         click.echo("WARNING: Using ':' for aliases is now deprecated.")
-        return s[0:i], s[i+1:]
-    else: return None, s
+        return s[0:i], s[i + 1:]
+    else:
+        return None, s
+
 
 @params(s=six.string_types)
 def parse_alias(s):
     i = s.find(',')
-    if i > 0: return s[0:i], s[i+1:]
-    else: return parse_deprecated_alias(s)
+    if i > 0:
+        return s[0:i], s[i + 1:]
+    else:
+        return parse_deprecated_alias(s)
+
 
 @params(s=six.string_types)
 def parse_src_name(url, default=None):
     x = url.split('@')
     p = x[0]
     # If the same name is used, then reduce to the same name
     if '/' in p:
         ps = p.split('/')
         if functools.reduce(lambda x, y: x == y, ps):
             p = ps[0]
     v = default
     if len(x) > 1: v = x[1]
     return (p, v)
 
+
 def cmake_set(var, val, quote=True, cache=None, description=None):
     x = val
     if quote: x = util.quote(val)
     if cache is None or cache.lower() == 'none':
         yield "set({0} {1})".format(var, x)
     else:
         yield 'set({0} {1} CACHE {2} "{3}")'.format(var, x, cache, description or '')
 
+
 def cmake_append(var, *vals, **kwargs):
     quote = True
     if 'quote' in kwargs: quote = kwargs['quote']
     x = ' '.join(vals)
     if quote: x = ' '.join([util.quote(val) for val in vals])
     yield 'list(APPEND {0} {1})'.format(var, x)
 
+
 def cmake_if(cond, *args):
     yield 'if ({})'.format(cond)
     for arg in args:
         for line in arg:
             yield '    ' + line
     yield 'endif()'
 
+
 def cmake_else(*args):
     yield 'else ()'
     for arg in args:
         for line in arg:
             yield '    ' + line
 
+
 def parse_cmake_var_type(key, value):
     if ':' in key:
         p = key.split(':')
         return (p[0], p[1].upper(), value)
-    elif value.lower() in ['on', 'off', 'true', 'false']: 
+    elif value.lower() in ['on', 'off', 'true', 'false']:
         return (key, 'BOOL', value)
     else:
         return (key, 'STRING', value)
 
+
 def find_cmake(p, start):
     if p and not os.path.isabs(p):
         absp = util.actual_path(p, start)
-        if os.path.exists(absp): return absp
+        if os.path.exists(absp):
+            return absp
         else:
             x = util.carbin_dir('cmake', p)
-            if os.path.exists(x): return x
-            elif os.path.exists(x + '.cmake'): return x + '.cmake'
+            if os.path.exists(x):
+                return x
+            elif os.path.exists(x + '.cmake'):
+                return x + '.cmake'
     return p
 
 
-
 PACKAGE_SOURCE_TYPES = (six.string_types, PackageSource, PackageBuild)
 
+
 class CarbinPrefix:
     def __init__(self, prefix, verbose=False, build_path=None):
         self.prefix = os.path.abspath(prefix or 'carbin')
         self.verbose = verbose
         self.build_path_var = build_path
         self.cmd = util.Commander(paths=[self.get_path('bin')], env=self.get_env(), verbose=self.verbose)
         self.toolchain = self.write_cmake()
@@ -101,88 +131,94 @@
     def log(self, *args):
         if self.verbose: click.secho(' '.join([str(arg) for arg in args]), bold=True)
 
     def check(self, f, *args):
         if self.verbose and not f(*args):
             raise util.BuildError('ASSERTION FAILURE: ', ' '.join([str(arg) for arg in args]))
 
-
     def get_env(self):
         return {
             'LD_LIBRARY_PATH': self.get_path('lib'),
             'PKG_CONFIG_PATH': self.pkg_config_path()
         }
 
     def write_cmake(self, always_write=False, **kwargs):
-        return util.mkfile(self.get_private_path(), 'carbin.cmake', self.generate_cmake_toolchain(**kwargs), always_write=always_write)
+        return util.mkfile(self.get_private_path(), 'carbin.cmake', self.generate_cmake_toolchain(**kwargs),
+                           always_write=always_write)
 
     @returns(inspect.isgenerator)
     @util.yield_from
-    def generate_cmake_toolchain(self, toolchain=None, cc=None, cxx=None, cflags=None, cxxflags=None, ldflags=None, std=None, defines=None):
+    def generate_cmake_toolchain(self, toolchain=None, cc=None, cxx=None, cflags=None, cxxflags=None, ldflags=None,
+                                 std=None, defines=None):
         set_ = cmake_set
         if_ = cmake_if
         else_ = cmake_else
         append_ = cmake_append
         yield set_('CARBIN_PREFIX', self.prefix)
         yield set_('CMAKE_PREFIX_PATH', self.prefix)
         yield if_('${CMAKE_VERSION} VERSION_LESS "3.6.0"',
-            ['include_directories(SYSTEM ${CARBIN_PREFIX}/include)'],
-            else_(
-                set_('CMAKE_CXX_STANDARD_INCLUDE_DIRECTORIES', '${CARBIN_PREFIX}/include'),
-                set_('CMAKE_C_STANDARD_INCLUDE_DIRECTORIES', '${CARBIN_PREFIX}/include')
-            )
-        )
+                  ['include_directories(SYSTEM ${CARBIN_PREFIX}/include)'],
+                  else_(
+                      set_('CMAKE_CXX_STANDARD_INCLUDE_DIRECTORIES', '${CARBIN_PREFIX}/include'),
+                      set_('CMAKE_C_STANDARD_INCLUDE_DIRECTORIES', '${CARBIN_PREFIX}/include')
+                  )
+                  )
         if toolchain: yield ['include({})'.format(util.quote(os.path.abspath(toolchain)))]
         yield if_('CMAKE_CROSSCOMPILING',
-            append_('CMAKE_FIND_ROOT_PATH', self.prefix)
-        )
+                  append_('CMAKE_FIND_ROOT_PATH', self.prefix)
+                  )
         yield if_('CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT',
-            set_('CMAKE_INSTALL_PREFIX', self.prefix)
-        )
+                  set_('CMAKE_INSTALL_PREFIX', self.prefix)
+                  )
         if cxx: yield set_('CMAKE_CXX_COMPILER', cxx)
         if cc: yield set_('CMAKE_C_COMPILER', cc)
         if std:
             yield if_('NOT "${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC"',
-                set_('CMAKE_CXX_STD_FLAG', "-std={}".format(std))
-            )
+                      set_('CMAKE_CXX_STD_FLAG', "-std={}".format(std))
+                      )
         yield if_('"${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC"',
-            set_('CMAKE_CXX_ENABLE_PARALLEL_BUILD_FLAG', "/MP")
-        )
+                  set_('CMAKE_CXX_ENABLE_PARALLEL_BUILD_FLAG', "/MP")
+                  )
         if cflags:
-            yield set_('CMAKE_C_FLAGS', "$ENV{{CFLAGS}} ${{CMAKE_C_FLAGS_INIT}} {}".format(cflags or ''), cache='STRING')
+            yield set_('CMAKE_C_FLAGS', "$ENV{{CFLAGS}} ${{CMAKE_C_FLAGS_INIT}} {}".format(cflags or ''),
+                       cache='STRING')
         if cxxflags or std:
-            yield set_('CMAKE_CXX_FLAGS', "$ENV{{CXXFLAGS}} ${{CMAKE_CXX_FLAGS_INIT}} ${{CMAKE_CXX_STD_FLAG}} {}".format(cxxflags or ''), cache='STRING')
+            yield set_('CMAKE_CXX_FLAGS',
+                       "$ENV{{CXXFLAGS}} ${{CMAKE_CXX_FLAGS_INIT}} ${{CMAKE_CXX_STD_FLAG}} {}".format(cxxflags or ''),
+                       cache='STRING')
         if ldflags:
             for link_type in ['STATIC', 'SHARED', 'MODULE', 'EXE']:
-                yield set_('CMAKE_{}_LINKER_FLAGS'.format(link_type), "$ENV{{LDFLAGS}} {0}".format(ldflags), cache='STRING')
+                yield set_('CMAKE_{}_LINKER_FLAGS'.format(link_type), "$ENV{{LDFLAGS}} {0}".format(ldflags),
+                           cache='STRING')
         for dkey in defines or {}:
             name, vtype, value = parse_cmake_var_type(dkey, defines[dkey])
             yield set_(name, value, cache=vtype, quote=(vtype != 'BOOL'))
         yield if_('BUILD_SHARED_LIBS',
-            set_('CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS', 'ON', cache='BOOL')
-        )
+                  set_('CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS', 'ON', cache='BOOL')
+                  )
         yield set_('CMAKE_FIND_FRAMEWORK', 'LAST', cache='STRING')
         yield set_('CMAKE_INSTALL_RPATH', '${CARBIN_PREFIX}/lib', cache='STRING')
 
-
     def get_path(self, *paths):
         return os.path.join(self.prefix, *paths)
 
     def get_private_path(self, *paths):
         return self.get_path('carbin', *paths)
 
     def get_public_path(self, *paths):
         return self.get_path('etc', 'carbin', *paths)
 
     def get_recipe_paths(self):
         return [self.get_public_path('recipes')]
 
     def get_builder_path(self, *paths):
-        if self.build_path_var: return os.path.join(self.build_path_var, *paths)
-        else: return self.get_private_path('build', *paths)
+        if self.build_path_var:
+            return os.path.join(self.build_path_var, *paths)
+        else:
+            return self.get_private_path('build', *paths)
 
     @contextlib.contextmanager
     def create_builder(self, name, tmp=False):
         pre = ''
         if tmp: pre = 'tmp-'
         d = self.get_builder_path(pre + name)
         exists = os.path.exists(d)
@@ -214,16 +250,18 @@
             rp = os.path.normcase(os.path.join(rpath, p, v or ''))
             if os.path.exists(rp):
                 return PackageSource(name=name or p, recipe=rp)
         return None
 
     def parse_src_github(self, name, url):
         p, v = parse_src_name(url, 'HEAD')
-        if '/' in p: url = 'https://github.com/{0}/archive/{1}.tar.gz'.format(p, v)
-        else: url = 'https://github.com/{0}/{0}/archive/{1}.tar.gz'.format(p, v)
+        if '/' in p:
+            url = 'https://github.com/{0}/archive/{1}.tar.gz'.format(p, v)
+        else:
+            url = 'https://github.com/{0}/{0}/archive/{1}.tar.gz'.format(p, v)
         if name is None: name = p
         return PackageSource(name=name, url=url)
 
     @returns(PackageSource)
     @params(pkg=PACKAGE_SOURCE_TYPES)
     def parse_pkg_src(self, pkg, start=None, no_recipe=False):
         if isinstance(pkg, PackageSource): return pkg
@@ -235,107 +273,123 @@
                 (None if no_recipe else self.parse_src_recipe(name, url)) or \
                 self.parse_src_github(name, url)
         return PackageSource(name=name, url=url)
 
     @returns(PackageBuild)
     @params(pkg=PACKAGE_SOURCE_TYPES)
     def parse_pkg_build(self, pkg, start=None, no_recipe=False):
-        if isinstance(pkg, PackageBuild): 
+        if isinstance(pkg, PackageBuild):
             pkg.pkg_src = self.parse_pkg_src(pkg.pkg_src, start, no_recipe)
             if pkg.pkg_src.recipe: pkg = self.from_recipe(pkg.pkg_src.recipe, pkg)
             if pkg.cmake: pkg.cmake = find_cmake(pkg.cmake, start)
             return pkg
         else:
             pkg_src = self.parse_pkg_src(pkg, start, no_recipe)
-            if pkg_src.recipe: return self.from_recipe(pkg_src.recipe, pkg_src.name)
-            else: return PackageBuild(pkg_src)
+            if pkg_src.recipe:
+                return self.from_recipe(pkg_src.recipe, pkg_src.name)
+            else:
+                return PackageBuild(pkg_src)
 
     def from_recipe(self, recipe, pkg=None, name=None):
         recipe_pkg = os.path.join(recipe, "package.txt")
         util.ensure_exists(recipe_pkg)
         p = next(iter(self.from_file(recipe_pkg, no_recipe=True)))
-        self.check(lambda:p.pkg_src is not None)
+        self.check(lambda: p.pkg_src is not None)
         requirements = os.path.join(recipe, "requirements.txt")
         if os.path.exists(requirements): p.requirements = requirements
         p.pkg_src.recipe = None
         # Use original name
-        if pkg: p.pkg_src.name = pkg.pkg_src.name
-        elif name: p.pkg_src.name = name
+        if pkg:
+            p.pkg_src.name = pkg.pkg_src.name
+        elif name:
+            p.pkg_src.name = name
 
-        if pkg: return p.merge(pkg)
-        else: return p
+        if pkg:
+            return p.merge(pkg)
+        else:
+            return p
 
     def from_file(self, file, url=None, no_recipe=False):
         if file is None:
             return
         if not os.path.exists(file):
             self.log("file not found: " + file)
             return
         start = os.path.dirname(file)
         if url is not None and url.startswith('file://'):
             start = url[7:]
         with open(file) as f:
             self.log("parse file: " + file)
             for line in f.readlines():
                 tokens = shlex.split(line, comments=True)
-                if len(tokens) > 0: 
+                if len(tokens) > 0:
                     pb = parse_pkg_build_tokens(tokens)
-                    ps = self.from_file(util.actual_path(pb.file, start), no_recipe=no_recipe) if pb.file else [self.parse_pkg_build(pb, start=start, no_recipe=no_recipe)]
+                    ps = self.from_file(util.actual_path(pb.file, start), no_recipe=no_recipe) if pb.file else [
+                        self.parse_pkg_build(pb, start=start, no_recipe=no_recipe)]
                     for p in ps: yield p
 
     def write_parent(self, pb, track=True):
         if track and pb.parent is not None: util.mkfile(self.get_deps_directory(pb.to_fname()), pb.parent, pb.parent)
 
-    def install_deps(self, pb, d, test=False, test_all=False, generator=None, insecure=False, ignore_requirements=False):
+    def install_deps(self, pb, d, test=False, test_all=False, generator=None, insecure=False,
+                     ignore_requirements=False):
         req_txt = os.path.join(d, 'requirements.txt') if not ignore_requirements else None
         for dependent in self.from_file(pb.requirements or req_txt, pb.pkg_src.url):
             transient = dependent.test or dependent.build
             testing = test or test_all
             installable = not dependent.test or dependent.test == testing
-            if installable: 
-                self.install(dependent.of(pb), test_all=test_all, generator=generator, track=not transient, insecure=insecure)
+            if installable:
+                self.install(dependent.of(pb), test_all=test_all, generator=generator, track=not transient,
+                             insecure=insecure)
 
     @returns(six.string_types)
     @params(pb=PACKAGE_SOURCE_TYPES, test=bool, test_all=bool, update=bool, track=bool)
     def install(self, pb, test=False, test_all=False, generator=None, update=False, track=True, insecure=False):
         pb = self.parse_pkg_build(pb)
         pkg_dir = self.get_package_directory(pb.to_fname())
         unlink_dir = self.get_unlink_directory(pb.to_fname())
         install_dir = self.get_package_directory(pb.to_fname(), 'install')
         # If its been unlinked, then link it in
         if os.path.exists(unlink_dir):
-            if update: shutil.rmtree(unlink_dir)
+            if update:
+                shutil.rmtree(unlink_dir)
             else:
                 self.link(pb)
                 self.write_parent(pb, track=track)
                 return "Linking package {}".format(pb.to_name())
-        if os.path.exists(pkg_dir): 
+        if os.path.exists(pkg_dir):
             self.write_parent(pb, track=track)
-            if update: self.remove(pb)
-            else: return "Package {} already installed".format(pb.to_name())
+            if update:
+                self.remove(pb)
+            else:
+                return "Package {} already installed".format(pb.to_name())
         with self.create_builder(pb.pkg_src.get_hash(), tmp=True) as builder:
             # Fetch package
             src_dir = builder.fetch(pb.pkg_src.url, pb.hash, (pb.cmake != None), insecure=insecure)
             # Install any dependencies first
-            self.install_deps(pb, src_dir, test=test, test_all=test_all, generator=generator, insecure=insecure, ignore_requirements=pb.ignore_requirements)
+            self.install_deps(pb, src_dir, test=test, test_all=test_all, generator=generator, insecure=insecure,
+                              ignore_requirements=pb.ignore_requirements)
             # Setup cmake file
-            if pb.cmake: 
+            if pb.cmake:
                 target = os.path.join(src_dir, 'CMakeLists.txt')
                 if os.path.exists(target):
                     os.rename(target, os.path.join(src_dir, builder.cmake_original_file))
                 shutil.copyfile(pb.cmake, target)
             # Configure and build
-            builder.configure(src_dir, defines=pb.define, generator=generator, install_prefix=install_dir, test=test, variant=pb.variant)
+            builder.configure(src_dir, defines=pb.define, generator=generator, install_prefix=install_dir, test=test,
+                              variant=pb.variant)
             builder.build(variant=pb.variant)
             # Run tests if enabled
             if test or test_all: builder.test(variant=pb.variant)
             # Install
             builder.build(target='install', variant=pb.variant)
-            if util.USE_SYMLINKS: util.symlink_dir(install_dir, self.prefix)
-            else: util.copy_dir(install_dir, self.prefix)
+            if util.USE_SYMLINKS:
+                util.symlink_dir(install_dir, self.prefix)
+            else:
+                util.copy_dir(install_dir, self.prefix)
         self.write_parent(pb, track=track)
         return "Successfully installed {}".format(pb.to_name())
 
     @returns(six.string_types)
     @params(pb=PACKAGE_SOURCE_TYPES)
     def ignore(self, pb):
         pb = self.parse_pkg_build(pb)
@@ -355,15 +409,16 @@
             pb.requirements = os.path.join(src_dir, 'dev-requirements.txt')
         elif os.path.exists(os.path.join(src_dir, 'requirements.txt')):
             pb.requirements = os.path.join(src_dir, 'requirements.txt')
         with self.create_builder(pb.to_fname()) as builder:
             # Install any dependencies first
             self.install_deps(pb, src_dir, generator=generator, test=test)
             # Configure and build
-            if not builder.exists: builder.configure(src_dir, defines=pb.define, generator=generator, test=test, variant=pb.variant)
+            if not builder.exists: builder.configure(src_dir, defines=pb.define, generator=generator, test=test,
+                                                     variant=pb.variant)
             builder.build(variant=pb.variant, target=target)
             # Run tests if enabled
             if test: builder.test(variant=pb.variant)
 
     @params(pb=PACKAGE_SOURCE_TYPES)
     def build_path(self, pb):
         pb = self.parse_pkg_build(pb)
@@ -396,42 +451,47 @@
         self.log("Unlink:", pkg_dir)
         if os.path.exists(pkg_dir):
             if util.USE_SYMLINKS:
                 util.rm_symlink_from(os.path.join(pkg_dir, 'install'), self.prefix)
             else:
                 util.rm_dup_dir(os.path.join(pkg_dir, 'install'), self.prefix, remove_both=False)
             util.rm_empty_dirs(self.prefix)
-            if delete: util.delete_dir(pkg_dir)
+            if delete:
+                util.delete_dir(pkg_dir)
             else:
                 util.mkdir(self.get_unlink_directory())
                 os.rename(pkg_dir, unlink_dir)
 
     @params(pkg=PACKAGE_SOURCE_TYPES)
     def link(self, pkg):
         pkg = self.parse_pkg_src(pkg)
         pkg_dir = self.get_package_directory(pkg.to_fname())
         unlink_dir = self.get_unlink_directory(pkg.to_fname())
         if os.path.exists(unlink_dir):
             util.mkdir(self.get_package_directory())
             os.rename(unlink_dir, pkg_dir)
-            if util.USE_SYMLINKS: util.symlink_dir(os.path.join(pkg_dir, 'install'), self.prefix)
-            else: util.copy_dir(os.path.join(pkg_dir, 'install'), self.prefix)
+            if util.USE_SYMLINKS:
+                util.symlink_dir(os.path.join(pkg_dir, 'install'), self.prefix)
+            else:
+                util.copy_dir(os.path.join(pkg_dir, 'install'), self.prefix)
         # Relink dependencies
         for dep in util.ls(self.get_unlink_directory(), os.path.isdir):
             ls = util.ls(self.get_unlink_deps_directory(dep), os.path.isfile)
             if pkg.to_fname() in ls: self.link(dep)
 
     def _list_files(self, pkg=None, top=True):
         if pkg is None:
             return util.ls(self.get_package_directory(), os.path.isdir)
         else:
             p = self.parse_pkg_src(pkg)
             ls = util.ls(self.get_deps_directory(p.to_fname()), os.path.isfile)
-            if top: return [p.to_fname()]+list(ls)
-            else: return ls
+            if top:
+                return [p.to_fname()] + list(ls)
+            else:
+                return ls
 
     def list(self, pkg=None, recursive=False, top=True):
         for d in self._list_files(pkg, top):
             p = fname_to_pkg(d)
             if os.path.exists(self.get_package_directory(d)): yield p
             if recursive:
                 for child in self.list(p, recursive=recursive, top=False):
@@ -461,20 +521,19 @@
     def try_(self, msg=None, on_fail=None):
         try:
             yield
         except util.BuildError as err:
             if err.msg: click.echo(err.msg)
             if msg: click.echo(msg)
             if on_fail: on_fail()
-            if self.verbose: 
+            if self.verbose:
                 if err.data: click.echo(err.data)
                 raise
             sys.exit(1)
         except:
             extype, exvalue, extraceback = sys.exc_info()
             click.echo("Unexpected error: " + str(extype))
             click.echo(str(exvalue))
             if msg: click.echo(msg)
             if on_fail: on_fail()
             if self.verbose: raise
             sys.exit(1)
-
```

## carbin/types.py

```diff
@@ -1,7 +1,22 @@
+#
+# Copyright 2023 The Turbo Authors.
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
 import six, inspect, os
 
 def decorator_with_args(decorator):
     def f(*args, **kwargs):
         def g(func):
             return decorator(func, *args, **kwargs)
         return g
```

## carbin/util.py

```diff
@@ -1,7 +1,22 @@
+#
+# Copyright 2023 The Turbo Authors.
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
 import click, os, sys, shutil, json, six, hashlib, ssl
 
 if sys.version_info[0] < 3:
     try:
         import contextlib
         import lzma
     except:
@@ -194,14 +209,15 @@
             has_files = True
     if not has_files: os.rmdir(d)
     return has_files
 
 def get_dirs(d):
     return (os.path.join(d,o) for o in os.listdir(d) if os.path.isdir(os.path.join(d,o)))
 
+
 def copy_to(src, dst_dir):
     target = os.path.join(dst_dir, os.path.basename(src))
     if os.path.isfile(src): shutil.copyfile(src, target)
     else: shutil.copytree(src, target)
     return target
 
 def symlink_to(src, dst_dir):
@@ -231,18 +247,20 @@
         if insecure: context = ssl._create_unverified_context()
         CarbinURLOpener(context=context).retrieve(url, filename=file, reporthook=hook, data=None)
         bar.update(bar_len)
     if not os.path.exists(file):
         raise BuildError("Download failed for: {0}".format(url))
     return file
 
+
 def transfer_to(f, dst, copy=False):
     if USE_SYMLINKS and not copy: return symlink_to(f, dst)
     else: return copy_to(f, dst)
 
+
 def retrieve_url(url, dst, copy=False, insecure=False, hash=None):
     remote = not url.startswith('file://')
     # Retrieve from cache
     if remote and hash:
         f = get_cache_file(hash.replace(':', '-'))
         if f: return f
     f = download_to(url, dst, insecure=insecure) if remote else transfer_to(url[7:], dst, copy=copy)
@@ -250,14 +268,15 @@
         click.echo("Computing hash: {}".format(hash))
         if check_hash(f, hash):
             if remote: add_cache_file(hash.replace(':', '-'), f)
         else:
             raise BuildError("Hash doesn't match for {0}: {1}".format(url, hash))
     return f
 
+
 def extract_ar(archive, dst, *kwargs):
     if sys.version_info[0] < 3 and archive.endswith('.xz'):
         with contextlib.closing(lzma.LZMAFile(archive)) as xz:
             with tarfile.open(fileobj=xz, *kwargs) as f:
                 f.extractall(dst)
     elif archive.endswith('.zip'):
         with zipfile.ZipFile(archive,'r') as f:
@@ -269,14 +288,15 @@
             tarfile.open(archive, *kwargs).extractall(dst)
     else:
         # Treat as a single source file
         d = os.path.join(dst, 'header')
         mkdir(d)
         copy_to(archive, d)
 
+
 def hash_file(f, t):
     h = hashlib.new(t)
     h.update(open(f, 'rb').read())
     return h.hexdigest()
 
 def check_hash(f, hash):
     t, h = hash.lower().split(':')
```

## Comparing `carbin-0.3.0.dist-info/LICENSE` & `carbin-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `carbin-0.3.0.dist-info/RECORD` & `carbin-0.3.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-carbin/__init__.py,sha256=vB-FBZL1_7QWXKN2-UYoE6bTAGTthJ4QaSwWP5w7ScM,23
-carbin/builder.py,sha256=zih-lhV0rmdT-dQ6CbV-pgHaY02ErXsomXiN1QLjFII,3900
-carbin/cli.py,sha256=M-zL5B_xpwmdFbRxxMQcQJi2qBk9YMRDSO3_lM4eoFQ,10030
-carbin/package.py,sha256=aLemhQSra_8Zxptu4ZiHnd_P3o_zpfFXYcuNMxnvfig,4198
-carbin/prefix.py,sha256=YEL06_unNrrDpmOawRCd6BvoHQaPVBwlbvozjiqot-U,20049
-carbin/types.py,sha256=pYozdusPeITb2Rzh8JoPgWPTC5YdI9XO9gjMFGOMs4Y,2205
-carbin/util.py,sha256=mBGSsKRh25yFgxMA5KG8l3pzIs6IVvyOfQOay-Dt_8Y,11812
+carbin/__init__.py,sha256=6eiWnshoqP6EqMzIhcEv_A8lX8TtdZVkBoDgTUTz7kI,608
+carbin/builder.py,sha256=gG7D9hqDE-S_GfROafz2pdfIyB8y8wEwQocNz4NQY-o,4487
+carbin/cli.py,sha256=AXKMfFFObXb0r845OvlZYvgnxBoDFgaLZpo51Dr4_XI,11428
+carbin/creater.py,sha256=TKvIbpl_qHwFZNMZWgWK8VBHdb3njvVM-D2_UmPBsRY,4125
+carbin/package.py,sha256=j3DeKkhh9YhWe0i8LvJis1OGLzlBF_RRptvOy_XACnQ,4784
+carbin/prefix.py,sha256=gUdTZXnLm7uTrChfCvdFnoZG2B-glUY4qlo4oZ_sYgk,21460
+carbin/types.py,sha256=YF4e-RDaDO4Y7i8mMTTcS78RnZkCMxRvmhOPruBzljo,2791
+carbin/util.py,sha256=-6SNYfU8IE6NgjSe4VhlzXJfGDh47D63PNi5ERU3ApQ,12403
 carbin/cmake/autotools.cmake,sha256=asyjvKRMFpSlaZMeMP44-hcw0arGWJGTbfujD95Vo5s,7513
 carbin/cmake/binary.cmake,sha256=lwu9TbC9Ni0Zb7KsrPh98RBRD3D2gS6R4V5MWYRkGB0,512
 carbin/cmake/boost.cmake,sha256=lrFDFluYtng6Lyi2O8KpIW8E6YHucnHv7d2CREJmwsA,10396
 carbin/cmake/header.cmake,sha256=CHyFepXmujahMo5QPs703EsfT2YLgK1FDDuv0O4JmRY,1161
 carbin/cmake/make.cmake,sha256=zX7sr2hA7PMsKJ09RyGzrvxZbpW84uOYcuzpCWVQCes,6387
 carbin/cmake/meson.cmake,sha256=bQ5SnqPuPKUaIWmcWCcV2V91MoSeYdRRHQeWP88TzfY,9225
 carbin/cmake/subdir.cmake,sha256=wxpubdxBKoAnjYUV8Mizxq_YymtwPm3iUjN5Dh3YWNU,121
-carbin-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-carbin-0.3.0.dist-info/METADATA,sha256=7IXlpQBgEn_jJ0NWYRu2u92BJ3RBqPwU1M4palolXIE,276
-carbin-0.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-carbin-0.3.0.dist-info/entry_points.txt,sha256=ibqGDVfvnT2ZzaMDaRB5PgOjVdrprvlsAJLrYTjGgHY,42
-carbin-0.3.0.dist-info/top_level.txt,sha256=qRZoXL__kMXE03dJArRq6hL4sOoXUbeufIL5RjVroV4,7
-carbin-0.3.0.dist-info/RECORD,,
+carbin-0.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+carbin-0.3.1.dist-info/METADATA,sha256=B0_vafO0JWl74wJ-9nnolzkAnGuUgTiCsruGYXNpGXQ,276
+carbin-0.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+carbin-0.3.1.dist-info/entry_points.txt,sha256=ibqGDVfvnT2ZzaMDaRB5PgOjVdrprvlsAJLrYTjGgHY,42
+carbin-0.3.1.dist-info/top_level.txt,sha256=qRZoXL__kMXE03dJArRq6hL4sOoXUbeufIL5RjVroV4,7
+carbin-0.3.1.dist-info/RECORD,,
```

